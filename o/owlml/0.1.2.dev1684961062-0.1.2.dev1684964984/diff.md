# Comparing `tmp/owlml-0.1.2.dev1684961062.tar.gz` & `tmp/owlml-0.1.2.dev1684964984.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owlml-0.1.2.dev1684961062.tar", last modified: Wed May 24 20:44:36 2023, max compression
+gzip compressed data, was "owlml-0.1.2.dev1684964984.tar", last modified: Wed May 24 21:49:58 2023, max compression
```

## Comparing `owlml-0.1.2.dev1684961062.tar` & `owlml-0.1.2.dev1684964984.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:44:36.412382 owlml-0.1.2.dev1684961062/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-24 20:43:40.000000 owlml-0.1.2.dev1684961062/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-24 20:44:36.412382 owlml-0.1.2.dev1684961062/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-24 20:43:40.000000 owlml-0.1.2.dev1684961062/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:44:36.412382 owlml-0.1.2.dev1684961062/owlml/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-24 20:43:40.000000 owlml-0.1.2.dev1684961062/owlml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-24 20:43:40.000000 owlml-0.1.2.dev1684961062/owlml/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-24 20:43:40.000000 owlml-0.1.2.dev1684961062/owlml/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-24 20:43:40.000000 owlml-0.1.2.dev1684961062/owlml/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-24 20:43:40.000000 owlml-0.1.2.dev1684961062/owlml/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-24 20:43:40.000000 owlml-0.1.2.dev1684961062/owlml/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-24 20:43:40.000000 owlml-0.1.2.dev1684961062/owlml/experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-24 20:43:40.000000 owlml-0.1.2.dev1684961062/owlml/images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:44:36.412382 owlml-0.1.2.dev1684961062/owlml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-24 20:44:36.000000 owlml-0.1.2.dev1684961062/owlml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-24 20:44:36.000000 owlml-0.1.2.dev1684961062/owlml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:44:36.000000 owlml-0.1.2.dev1684961062/owlml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-24 20:44:36.000000 owlml-0.1.2.dev1684961062/owlml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 20:44:36.000000 owlml-0.1.2.dev1684961062/owlml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 20:44:36.000000 owlml-0.1.2.dev1684961062/owlml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-24 20:44:36.416382 owlml-0.1.2.dev1684961062/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 20:43:40.000000 owlml-0.1.2.dev1684961062/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:49:58.635543 owlml-0.1.2.dev1684964984/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-24 21:49:01.000000 owlml-0.1.2.dev1684964984/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-24 21:49:58.635543 owlml-0.1.2.dev1684964984/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-24 21:49:01.000000 owlml-0.1.2.dev1684964984/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:49:58.631543 owlml-0.1.2.dev1684964984/owlml/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-24 21:49:01.000000 owlml-0.1.2.dev1684964984/owlml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-24 21:49:01.000000 owlml-0.1.2.dev1684964984/owlml/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-24 21:49:01.000000 owlml-0.1.2.dev1684964984/owlml/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-24 21:49:01.000000 owlml-0.1.2.dev1684964984/owlml/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-24 21:49:01.000000 owlml-0.1.2.dev1684964984/owlml/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-05-24 21:49:01.000000 owlml-0.1.2.dev1684964984/owlml/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-24 21:49:01.000000 owlml-0.1.2.dev1684964984/owlml/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-24 21:49:01.000000 owlml-0.1.2.dev1684964984/owlml/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-24 21:49:01.000000 owlml-0.1.2.dev1684964984/owlml/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:49:58.635543 owlml-0.1.2.dev1684964984/owlml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-24 21:49:58.000000 owlml-0.1.2.dev1684964984/owlml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-24 21:49:58.000000 owlml-0.1.2.dev1684964984/owlml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 21:49:58.000000 owlml-0.1.2.dev1684964984/owlml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-24 21:49:58.000000 owlml-0.1.2.dev1684964984/owlml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 21:49:58.000000 owlml-0.1.2.dev1684964984/owlml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 21:49:58.000000 owlml-0.1.2.dev1684964984/owlml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-24 21:49:58.635543 owlml-0.1.2.dev1684964984/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 21:49:01.000000 owlml-0.1.2.dev1684964984/setup.py
```

### Comparing `owlml-0.1.2.dev1684961062/LICENSE` & `owlml-0.1.2.dev1684964984/LICENSE`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684961062/README.md` & `owlml-0.1.2.dev1684964984/README.md`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684961062/owlml/annotations.py` & `owlml-0.1.2.dev1684964984/owlml/annotations.py`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684961062/owlml/api.py` & `owlml-0.1.2.dev1684964984/owlml/api.py`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684961062/owlml/auth.py` & `owlml-0.1.2.dev1684964984/owlml/auth.py`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684961062/owlml/datasets.py` & `owlml-0.1.2.dev1684964984/owlml/datasets.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """OwlML datasets API."""
 import json
 import time
 import warnings
+from functools import partial
 from pathlib import Path
 from typing import Any, Callable, Optional, Union
 
 from farmhash import fingerprint64
 from tqdm import tqdm
 
 from .annotations import read_annotations
 from .api import OwlMLAPI
 from .images import _download_image, generate_image_id, list_local_images
+from .utils import pagination_iterator
 
 
 def create_dataset(org: str, slug: str, labels: list[str]) -> dict[str, Any]:
     """Create a dataset."""
     payload = dict(org=org, slug=slug, labels=labels)
     return OwlMLAPI.post("datasets", payload)
 
@@ -22,28 +24,28 @@
 def download_dataset(
     dataset: str,
     version: Optional[str] = None,
     output_path: Union[str, Path] = "./",
 ) -> dict[str, Any]:
     """Download dataset version."""
     output_path = Path(output_path)
-    if version_slug is None:
-        version = version_dataset(dataset)
-        version_slug = version["slug"]
-    version = OwlMLAPI.get(f"dataset-versions/{version_slug}")
-    if len(version["images"]) == 0:
-        raise ValueError(f"No images in dataset version {version_slug}.")
-    image = next(iter(version["images"]))
+    if version is None:
+        version_response = version_dataset(dataset)
+        version = version_response["slug"]
+    version_response = OwlMLAPI.get(f"dataset-versions/{version}")
+    if len(version_response["images"]) == 0:
+        raise ValueError(f"No images in dataset version {version}.")
+    image = next(iter(version_response["images"]))
     image_path = output_path / Path(image["image_id"] + image["extension"])
     dataset_path = image_path.parent.parent.parent
-    annotations_path = dataset_path / "annotations" / f"{version_slug}.json"
+    annotations_path = dataset_path / "annotations" / f"{version}.json"
     annotations_path.parent.mkdir(parents=True, exist_ok=True)
     with open(annotations_path, "w") as f:
-        f.write(json.dumps(version["annotations"]))
-    for image in tqdm(version["images"]):
+        f.write(json.dumps(version_response["annotations"]))
+    for image in tqdm(version_response["images"]):
         image_path = output_path / Path(image["image_id"] + image["extension"])
         image_path.parent.mkdir(parents=True, exist_ok=True)
         _download_image(image["presigned_get"], image_path)
 
 
 def generate_records(
     dataset_directory: Union[str, Path],
@@ -66,14 +68,28 @@
         label_ids = []
         for annotation in item["annotations"]:
             label_ids.append(annotation["label_id"])
         records.append(dict(image_path=image_path, label_ids=label_ids))
     return records
 
 
+def list_versions(dataset: Optional[str] = None) -> list[dict[str, Any]]:
+    """List dataset versions."""
+
+    def _list_versions_page(page: int, dataset: Optional[str] = None) -> dict[str, Any]:
+        """Get a dataset versions page."""
+        route = f"dataset-versions?page={page}"
+        if dataset is not None:
+            route += f"&dataset={dataset}"
+        return OwlMLAPI.get(route)
+
+    _list_version_partial = partial(_list_versions_page, dataset=dataset)
+    return list(pagination_iterator(_list_version_partial))
+
+
 def version_dataset(dataset: str, slug: Optional[str] = None) -> dict[str, Any]:
     """Version a dataset."""
     payload = dict(dataset=dataset)
     if slug is not None:
         payload["slug"] = slug
     version = OwlMLAPI.post("dataset-versions", payload)
     while version == {}:
```

### Comparing `owlml-0.1.2.dev1684961062/owlml/images.py` & `owlml-0.1.2.dev1684964984/owlml/images.py`

 * *Files identical despite different names*

