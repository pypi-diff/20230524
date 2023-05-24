# Comparing `tmp/calitp_map_utils-2023.5.19.7.tar.gz` & `tmp/calitp_map_utils-2023.5.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calitp_map_utils-2023.5.19.7.tar", max compression
+gzip compressed data, was "calitp_map_utils-2023.5.24.tar", max compression
```

## Comparing `calitp_map_utils-2023.5.19.7.tar` & `calitp_map_utils-2023.5.24.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      944 2023-05-18 19:13:08.501349 calitp_map_utils-2023.5.19.7/README.md
--rw-r--r--   0        0        0     3369 2023-05-19 17:51:42.728852 calitp_map_utils-2023.5.19.7/calitp_map_utils/__init__.py
--rw-r--r--   0        0        0       44 2023-05-19 17:31:40.764053 calitp_map_utils-2023.5.19.7/calitp_map_utils/__main__.py
--rw-r--r--   0        0        0     1321 2023-05-19 17:39:43.981472 calitp_map_utils-2023.5.19.7/calitp_map_utils/cli.py
--rw-r--r--   0        0        0      612 2023-05-19 18:02:17.046050 calitp_map_utils-2023.5.19.7/pyproject.toml
--rw-r--r--   0        0        0     1531 1970-01-01 00:00:00.000000 calitp_map_utils-2023.5.19.7/PKG-INFO
+-rw-r--r--   0        0        0      944 2023-05-23 18:00:10.633586 calitp_map_utils-2023.5.24/README.md
+-rw-r--r--   0        0        0     4290 2023-05-24 15:33:39.118930 calitp_map_utils-2023.5.24/calitp_map_utils/__init__.py
+-rw-r--r--   0        0        0       44 2023-05-23 18:00:10.635825 calitp_map_utils-2023.5.24/calitp_map_utils/__main__.py
+-rw-r--r--   0        0        0     1409 2023-05-24 15:28:37.116341 calitp_map_utils-2023.5.24/calitp_map_utils/cli.py
+-rw-r--r--   0        0        0      626 2023-05-24 18:37:37.869199 calitp_map_utils-2023.5.24/pyproject.toml
+-rw-r--r--   0        0        0     1566 1970-01-01 00:00:00.000000 calitp_map_utils-2023.5.24/PKG-INFO
```

### Comparing `calitp_map_utils-2023.5.19.7/README.md` & `calitp_map_utils-2023.5.24/README.md`

 * *Files identical despite different names*

### Comparing `calitp_map_utils-2023.5.19.7/calitp_map_utils/__init__.py` & `calitp_map_utils-2023.5.24/calitp_map_utils/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,45 @@
+import base64
 import gzip
 import json
+import os
 from enum import Enum
-from typing import Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import requests
 import typer
-import urllib3
 from calitp_data.storage import get_fs  # type: ignore
+from furl import furl
 from geojson_pydantic import Feature, FeatureCollection, MultiPolygon, Point, Polygon
 from geojson_pydantic.types import Position
-from pydantic import BaseModel, HttpUrl, ValidationError, root_validator
+from pydantic import BaseModel, HttpUrl, ValidationError, conlist, root_validator
 from tqdm import tqdm
 
+MAP_APP_URL_ENV_VAR = "CALITP_MAP_APP_URL"
+MAP_APP_URL = os.getenv(MAP_APP_URL_ENV_VAR)
+
 
 class Analysis(str, Enum):
     speedmaps = "speedmap"
     hqta_areas = "hqta_areas"
     hqta_stops = "hqta_stops"
 
 
+class Tooltip(BaseModel):
+    html: str
+    style: Optional[Dict[str, Any]]
+
+
 class Speedmap(BaseModel):
     stop_id: Optional[str]
     stop_name: Optional[str]
     route_id: Optional[str]
+    tooltip: Tooltip
+    color: conlist(int, min_items=3, max_items=3)  # we add alpha in the JS
+    highlight_color: Optional[List[int]]
 
     @root_validator
     def some_identifier_exists(cls, values):
         assert any(key in values for key in ["stop_id", "stop_name", "route_id"])
         return values
 
 
@@ -80,37 +93,59 @@
             except ValidationError:
                 typer.secho(feature.json(), fg=typer.colors.RED)
                 raise
 
     return collection
 
 
+class Layer(BaseModel):
+    name: str
+    url: HttpUrl
+    analysis: Optional[Analysis]
+
+
+class BasemapConfig(BaseModel):
+    url: str
+    options: Dict[str, Any]
+
+
 # Any positions in this are flipped from typical geojson
 # leaflet wants lat/lon
 class State(BaseModel):
-    name: str
-    url: HttpUrl
+    name: Optional[str]
+    layers: conlist(Layer, min_items=1)
     lat_lon: Optional[Position]
     zoom: Optional[int]
     bbox: Optional[Tuple[Position, Position]]
-    analysis: Optional[Analysis]
+    basemap_config: Optional[BasemapConfig]
 
-    def validate_url(
+    def validate_layers(
         self,
         data: bool = False,
         verbose: bool = False,
-        analysis: Optional[Analysis] = None,
     ):
-        if verbose:
-            typer.secho(
-                f"Checking that {typer.style(self.url, fg=typer.colors.CYAN)} exists..."
-            )
-        resp = requests.head(self.url)
+        for layer in self.layers:
+            if verbose:
+                typer.secho(
+                    f"Checking that {typer.style(layer.url, fg=typer.colors.CYAN)} exists..."
+                )
+            resp = requests.head(layer.url)
 
-        try:
-            resp.raise_for_status()
-        except requests.exceptions.HTTPError:
-            typer.secho(f"Failed to find file at {self.url}", fg=typer.colors.RED)
-            raise
+            try:
+                resp.raise_for_status()
+            except requests.exceptions.HTTPError:
+                typer.secho(f"Failed to find file at {layer.url}", fg=typer.colors.RED)
+                raise
 
-        if data:
-            validate_geojson(self.url, analysis or self.analysis, verbose=verbose)
+            if data:
+                validate_geojson(layer.url, layer.analysis, verbose=verbose)
+
+    @property
+    def iframe_url(self) -> str:
+        if not MAP_APP_URL:
+            raise RuntimeError("Must provide MAP_APP_URL environment variable.")
+
+        return (
+            furl(MAP_APP_URL)
+            .add({"state": base64.urlsafe_b64encode(self.json().encode()).decode()})
+            .url
+        )
```

### Comparing `calitp_map_utils-2023.5.19.7/calitp_map_utils/cli.py` & `calitp_map_utils-2023.5.24/calitp_map_utils/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,29 +25,31 @@
 @app.command()
 def validate_state(
     infile: Optional[str] = None,
     base64url: bool = False,
     compressed: bool = False,
     data: bool = False,
     verbose: bool = False,
-    analysis: Optional[Analysis] = None,
 ):
     if infile:
         typer.secho(f"Reading {infile}.")
         with open(infile) as f:
             contents = f.read()
     else:
         typer.secho("Reading from stdin...")
         contents = sys.stdin.read()
 
     if base64url:
-        typer.secho("Decoding base64 contents...")
+        typer.secho("\tdecoding base64...")
         byts = base64.urlsafe_b64decode(contents.encode())
 
         if compressed:
+            typer.secho("\tdecompressing...")
             byts = gzip.decompress(byts)
 
         contents = byts.decode()
 
     state = State(**json.loads(contents))
-    state.validate_url(verbose=verbose, data=data, analysis=analysis)
+    state.validate_layers(verbose=verbose, data=data)
     typer.secho("Validation successful!", fg=typer.colors.GREEN)
+    typer.secho(f"Creating URL from state {state.json()}...")
+    typer.secho(f"URL: {state.iframe_url}")
```

### Comparing `calitp_map_utils-2023.5.19.7/pyproject.toml` & `calitp_map_utils-2023.5.24/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "calitp_map_utils"
-version = "2023.5.19.7"
+version = "2023.5.24"
 description = ""
 authors = ["Andrew Vaccaro <andrew.v@jarv.us>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "~3.9"
 pyyaml = "^6.0"
 typer = "^0.9.0"
 pydantic = "^1.10.7"
 tqdm = "^4.64.0"
 geojson-pydantic = "^0.6.1"
 calitp-data = "2023.2.13.1"
 requests = "^2.24.0"
+furl = "^2.1.3"
 
 
 [tool.poetry.group.dev.dependencies]
 pydantic-to-typescript = "^1.0.10"
 mypy = "^1.3.0"
 types-tqdm = "^4.65.0.1"
 types-requests = "^2.30.0.0"
```

### Comparing `calitp_map_utils-2023.5.19.7/PKG-INFO` & `calitp_map_utils-2023.5.24/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: calitp-map-utils
-Version: 2023.5.19.7
+Version: 2023.5.24
 Summary: 
 Author: Andrew Vaccaro
 Author-email: andrew.v@jarv.us
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: calitp-data (==2023.2.13.1)
+Requires-Dist: furl (>=2.1.3,<3.0.0)
 Requires-Dist: geojson-pydantic (>=0.6.1,<0.7.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.24.0,<3.0.0)
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
```

