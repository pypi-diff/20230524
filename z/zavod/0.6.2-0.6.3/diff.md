# Comparing `tmp/zavod-0.6.2.tar.gz` & `tmp/zavod-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zavod-0.6.2.tar", last modified: Wed Apr 19 18:11:30 2023, max compression
+gzip compressed data, was "zavod-0.6.3.tar", last modified: Wed May 24 15:48:35 2023, max compression
```

## Comparing `zavod-0.6.2.tar` & `zavod-0.6.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:11:30.937906 zavod-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-19 18:09:39.000000 zavod-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-19 18:09:39.000000 zavod-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-19 18:11:30.937906 zavod-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-19 18:09:39.000000 zavod-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 18:11:30.937906 zavod-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-19 18:09:39.000000 zavod-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:11:30.937906 zavod-0.6.2/zavod/
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:11:30.937906 zavod-0.6.2/zavod/parse/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/parse/addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/parse/names.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/parse/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:11:30.937906 zavod-0.6.2/zavod/sinks/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/sinks/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/sinks/json_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/sinks/json_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:11:30.937906 zavod-0.6.2/zavod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-19 18:11:30.000000 zavod-0.6.2/zavod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-19 18:11:30.000000 zavod-0.6.2/zavod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:11:30.000000 zavod-0.6.2/zavod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-19 18:11:30.000000 zavod-0.6.2/zavod.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:11:30.000000 zavod-0.6.2/zavod.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:11:13.000000 zavod-0.6.2/zavod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-19 18:11:30.000000 zavod-0.6.2/zavod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 18:11:30.000000 zavod-0.6.2/zavod.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:48:35.758710 zavod-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-24 15:46:22.000000 zavod-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-24 15:46:22.000000 zavod-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-24 15:48:35.758710 zavod-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-24 15:46:22.000000 zavod-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 15:48:35.758710 zavod-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-24 15:46:22.000000 zavod-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:48:35.758710 zavod-0.6.3/zavod/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-24 15:46:22.000000 zavod-0.6.3/zavod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-24 15:46:22.000000 zavod-0.6.3/zavod/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-24 15:46:22.000000 zavod-0.6.3/zavod/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-24 15:46:22.000000 zavod-0.6.3/zavod/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-24 15:46:22.000000 zavod-0.6.3/zavod/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-24 15:46:22.000000 zavod-0.6.3/zavod/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-24 15:46:22.000000 zavod-0.6.3/zavod/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:48:35.758710 zavod-0.6.3/zavod/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-24 15:46:22.000000 zavod-0.6.3/zavod/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-05-24 15:46:22.000000 zavod-0.6.3/zavod/parse/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-24 15:46:22.000000 zavod-0.6.3/zavod/parse/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-24 15:46:22.000000 zavod-0.6.3/zavod/parse/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:22.000000 zavod-0.6.3/zavod/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-24 15:46:22.000000 zavod-0.6.3/zavod/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:48:35.758710 zavod-0.6.3/zavod/sinks/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-24 15:46:22.000000 zavod-0.6.3/zavod/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-24 15:46:22.000000 zavod-0.6.3/zavod/sinks/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-24 15:46:22.000000 zavod-0.6.3/zavod/sinks/json_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-24 15:46:22.000000 zavod-0.6.3/zavod/sinks/json_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-24 15:46:22.000000 zavod-0.6.3/zavod/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:48:35.758710 zavod-0.6.3/zavod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-24 15:48:35.000000 zavod-0.6.3/zavod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-24 15:48:35.000000 zavod-0.6.3/zavod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:48:35.000000 zavod-0.6.3/zavod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-24 15:48:35.000000 zavod-0.6.3/zavod.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:48:35.000000 zavod-0.6.3/zavod.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:48:16.000000 zavod-0.6.3/zavod.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-24 15:48:35.000000 zavod-0.6.3/zavod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 15:48:35.000000 zavod-0.6.3/zavod.egg-info/top_level.txt
```

### Comparing `zavod-0.6.2/LICENSE` & `zavod-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zavod-0.6.2/PKG-INFO` & `zavod-0.6.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: zavod
-Version: 0.6.2
+Version: 0.6.3
 Summary: Data factory for followthemoney data.
 Home-page: https://github.com/opensanctions/zavod
 Author: Friedrich Lindenberg
 Author-email: friedrich@opensanctions.org
 License: MIT
 Keywords: data mapping identity followthemoney etl parsing
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # zavod
 
 Zavod is the FollowTheMoney data factory. It contains a variety of useful functions for building small and reproducible data pipelines that generate FtM graphs.
-
```

### Comparing `zavod-0.6.2/setup.py` & `zavod-0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="zavod",
-    version="0.6.2",
+    version="0.6.3",
     description="Data factory for followthemoney data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="data mapping identity followthemoney etl parsing",
     author="Friedrich Lindenberg",
     author_email="friedrich@opensanctions.org",
     url="https://github.com/opensanctions/zavod",
```

### Comparing `zavod-0.6.2/zavod/__init__.py` & `zavod-0.6.3/zavod/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from zavod import settings
 from zavod.context import GenericZavod
 from zavod.dataset import ZavodDataset, ZD
 from zavod.logs import configure_logging, get_logger
 from zavod.sinks.common import Sink
 from zavod.sinks.json_entity import JSONEntitySink
 
-__version__ = "0.6.2"
+__version__ = "0.6.3"
 __all__ = [
     "init",
     "context",
     "Zavod",
     "ZavodDataset",
     "ZD",
     "PathLike",
```

### Comparing `zavod-0.6.2/zavod/audit.py` & `zavod-0.6.3/zavod/audit.py`

 * *Files identical despite different names*

### Comparing `zavod-0.6.2/zavod/context.py` & `zavod-0.6.3/zavod/context.py`

 * *Files identical despite different names*

### Comparing `zavod-0.6.2/zavod/dataset.py` & `zavod-0.6.3/zavod/dataset.py`

 * *Files identical despite different names*

### Comparing `zavod-0.6.2/zavod/http.py` & `zavod-0.6.3/zavod/http.py`

 * *Files identical despite different names*

### Comparing `zavod-0.6.2/zavod/logs.py` & `zavod-0.6.3/zavod/logs.py`

 * *Files identical despite different names*

### Comparing `zavod-0.6.2/zavod/parse/addresses.py` & `zavod-0.6.3/zavod/parse/addresses.py`

 * *Files identical despite different names*

### Comparing `zavod-0.6.2/zavod/parse/names.py` & `zavod-0.6.3/zavod/parse/names.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,34 +16,38 @@
     name3: Optional[str] = None,
     patronymic: Optional[str] = None,
     matronymic: Optional[str] = None,
     name4: Optional[str] = None,
     name5: Optional[str] = None,
     tail_name: Optional[str] = None,
     last_name: Optional[str] = None,
+    prefix: Optional[str] = None,
+    suffix: Optional[str] = None,
 ) -> Optional[str]:
     """Provides a standardised way of assembling the components of a human name.
     This does a whole lot of cultural ignorance work, so YMMV."""
     full = collapse_spaces(full)
     if full is not None and len(full) > 1:
         return full
     return join_text(
+        prefix,
         name1,
         first_name,
         given_name,
         name2,
         second_name,
         middle_name,
         name3,
         patronymic,
         matronymic,
         name4,
         name5,
         tail_name,
         last_name,
+        suffix,
     )
 
 
 def set_name_part(
     entity: CE, prop: str, value: Optional[str], quiet: bool, lang: Optional[str]
 ) -> None:
     if value is None:
@@ -69,14 +73,16 @@
     patronymic: Optional[str] = None,
     matronymic: Optional[str] = None,
     name4: Optional[str] = None,
     name5: Optional[str] = None,
     tail_name: Optional[str] = None,
     last_name: Optional[str] = None,
     maiden_name: Optional[str] = None,
+    prefix: Optional[str] = None,
+    suffix: Optional[str] = None,
     alias: bool = False,
     name_prop: str = "name",
     is_weak: bool = False,
     quiet: bool = False,
     lang: Optional[str] = None,
 ) -> None:
     if not is_weak:
@@ -108,10 +114,12 @@
         name3=name3,
         patronymic=patronymic,
         matronymic=matronymic,
         name4=name4,
         name5=name5,
         tail_name=tail_name,
         last_name=last_name,
+        prefix=prefix,
+        suffix=suffix,
     )
     if full is not None and len(full):
         entity.add(name_prop, full, quiet=quiet, lang=lang)
```

### Comparing `zavod-0.6.2/zavod/parse/xml.py` & `zavod-0.6.3/zavod/parse/xml.py`

 * *Files identical despite different names*

### Comparing `zavod-0.6.2/zavod/sinks/common.py` & `zavod-0.6.3/zavod/sinks/common.py`

 * *Files identical despite different names*

### Comparing `zavod-0.6.2/zavod/util.py` & `zavod-0.6.3/zavod/util.py`

 * *Files identical despite different names*

### Comparing `zavod-0.6.2/zavod.egg-info/PKG-INFO` & `zavod-0.6.3/zavod.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: zavod
-Version: 0.6.2
+Version: 0.6.3
 Summary: Data factory for followthemoney data.
 Home-page: https://github.com/opensanctions/zavod
 Author: Friedrich Lindenberg
 Author-email: friedrich@opensanctions.org
 License: MIT
 Keywords: data mapping identity followthemoney etl parsing
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # zavod
 
 Zavod is the FollowTheMoney data factory. It contains a variety of useful functions for building small and reproducible data pipelines that generate FtM graphs.
-
```

### Comparing `zavod-0.6.2/zavod.egg-info/SOURCES.txt` & `zavod-0.6.3/zavod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

