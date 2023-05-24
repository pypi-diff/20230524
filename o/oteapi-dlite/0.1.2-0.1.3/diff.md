# Comparing `tmp/oteapi-dlite-0.1.2.tar.gz` & `tmp/oteapi-dlite-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oteapi-dlite-0.1.2.tar", last modified: Tue Apr 18 14:20:15 2023, max compression
+gzip compressed data, was "oteapi-dlite-0.1.3.tar", last modified: Wed May 24 14:07:59 2023, max compression
```

## Comparing `oteapi-dlite-0.1.2.tar` & `oteapi-dlite-0.1.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:20:15.482499 oteapi-dlite-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-18 14:20:15.482499 oteapi-dlite-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:20:15.478499 oteapi-dlite-0.1.2/oteapi_dlite/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-18 14:19:42.000000 oteapi-dlite-0.1.2/oteapi_dlite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:20:15.478499 oteapi-dlite-0.1.2/oteapi_dlite/models/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/models/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:20:15.482499 oteapi-dlite-0.1.2/oteapi_dlite/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/strategies/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/strategies/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/strategies/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/strategies/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/strategies/parse_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/strategies/parse_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/strategies/serialise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:20:15.482499 oteapi-dlite-0.1.2/oteapi_dlite/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/utils/nputils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/oteapi_dlite/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:20:15.478499 oteapi-dlite-0.1.2/oteapi_dlite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-18 14:20:15.000000 oteapi-dlite-0.1.2/oteapi_dlite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-18 14:20:15.000000 oteapi-dlite-0.1.2/oteapi_dlite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:20:15.000000 oteapi-dlite-0.1.2/oteapi_dlite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-18 14:20:15.000000 oteapi-dlite-0.1.2/oteapi_dlite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-18 14:20:15.000000 oteapi-dlite-0.1.2/oteapi_dlite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 14:20:15.000000 oteapi-dlite-0.1.2/oteapi_dlite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-18 14:20:15.486499 oteapi-dlite-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-18 14:17:38.000000 oteapi-dlite-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:07:59.107520 oteapi-dlite-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-24 14:01:11.000000 oteapi-dlite-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-24 14:01:11.000000 oteapi-dlite-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-24 14:07:59.107520 oteapi-dlite-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-24 14:01:11.000000 oteapi-dlite-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:07:59.103520 oteapi-dlite-0.1.3/oteapi_dlite/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-24 14:07:28.000000 oteapi-dlite-0.1.3/oteapi_dlite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:07:59.103520 oteapi-dlite-0.1.3/oteapi_dlite/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-24 14:01:11.000000 oteapi-dlite-0.1.3/oteapi_dlite/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-24 14:01:11.000000 oteapi-dlite-0.1.3/oteapi_dlite/models/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:07:59.107520 oteapi-dlite-0.1.3/oteapi_dlite/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:01:11.000000 oteapi-dlite-0.1.3/oteapi_dlite/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-24 14:01:11.000000 oteapi-dlite-0.1.3/oteapi_dlite/strategies/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-24 14:01:11.000000 oteapi-dlite-0.1.3/oteapi_dlite/strategies/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-24 14:01:11.000000 oteapi-dlite-0.1.3/oteapi_dlite/strategies/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-24 14:01:11.000000 oteapi-dlite-0.1.3/oteapi_dlite/strategies/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-24 14:01:11.000000 oteapi-dlite-0.1.3/oteapi_dlite/strategies/parse_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-05-24 14:01:11.000000 oteapi-dlite-0.1.3/oteapi_dlite/strategies/parse_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-24 14:01:11.000000 oteapi-dlite-0.1.3/oteapi_dlite/strategies/serialise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:07:59.107520 oteapi-dlite-0.1.3/oteapi_dlite/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-24 14:01:11.000000 oteapi-dlite-0.1.3/oteapi_dlite/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-24 14:01:11.000000 oteapi-dlite-0.1.3/oteapi_dlite/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-24 14:01:11.000000 oteapi-dlite-0.1.3/oteapi_dlite/utils/nputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-24 14:01:11.000000 oteapi-dlite-0.1.3/oteapi_dlite/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:07:59.103520 oteapi-dlite-0.1.3/oteapi_dlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-24 14:07:59.000000 oteapi-dlite-0.1.3/oteapi_dlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-24 14:07:59.000000 oteapi-dlite-0.1.3/oteapi_dlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:07:59.000000 oteapi-dlite-0.1.3/oteapi_dlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-24 14:07:59.000000 oteapi-dlite-0.1.3/oteapi_dlite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-24 14:07:59.000000 oteapi-dlite-0.1.3/oteapi_dlite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-24 14:07:59.000000 oteapi-dlite-0.1.3/oteapi_dlite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-24 14:01:11.000000 oteapi-dlite-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-24 14:01:11.000000 oteapi-dlite-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-24 14:01:11.000000 oteapi-dlite-0.1.3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-24 14:01:11.000000 oteapi-dlite-0.1.3/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-24 14:07:59.107520 oteapi-dlite-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-24 14:01:11.000000 oteapi-dlite-0.1.3/setup.py
```

### Comparing `oteapi-dlite-0.1.2/LICENSE` & `oteapi-dlite-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oteapi-dlite-0.1.2/PKG-INFO` & `oteapi-dlite-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oteapi-dlite
-Version: 0.1.2
+Version: 0.1.3
 Summary: DLite plugin for OTEAPI.
 Home-page: https://github.com/EMMC-ASBL/oteapi-dlite
 Author: team4.0@sintef.no
 Author-email: team4.0@sintef.no
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `oteapi-dlite-0.1.2/README.md` & `oteapi-dlite-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `oteapi-dlite-0.1.2/oteapi_dlite/strategies/filter.py` & `oteapi-dlite-0.1.3/oteapi_dlite/strategies/filter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Trivial filter that adds an empty collection to the session."""
 # pylint: disable=unused-argument
 from typing import TYPE_CHECKING, Any, Dict
 
 import dlite
+from oteapi.datacache import DataCache
 from oteapi.models import FilterConfig
 from pydantic import Field
 from pydantic.dataclasses import dataclass
 
 from oteapi_dlite.models import DLiteSessionUpdate
 
 if TYPE_CHECKING:
@@ -36,20 +37,25 @@
         self, session: "Optional[Dict[str, Any]]" = None
     ) -> DLiteSessionUpdate:
         """Initialize."""
         if session is None:
             raise ValueError("Missing session")
         if "collection_id" in session:
             raise KeyError("`collection_id` already exists in session.")
+
         coll = dlite.Collection()
 
         # Make sure that collection stays alive
         # It will never be deallocated...
         coll._incref()  # pylint: disable=protected-access
 
+        # Store the collection in the data cache
+        cache = DataCache()
+        cache.add(value=coll.asjson(), key=coll.uuid)
+
         return DLiteSessionUpdate(collection_id=coll.uuid)
 
     def get(
         self, session: "Optional[Dict[str, Any]]" = None
     ) -> DLiteSessionUpdate:
         """Execute the strategy."""
         if session is None:
```

### Comparing `oteapi-dlite-0.1.2/oteapi_dlite/strategies/function.py` & `oteapi-dlite-0.1.3/oteapi_dlite/strategies/function.py`

 * *Files identical despite different names*

### Comparing `oteapi-dlite-0.1.2/oteapi_dlite/strategies/mapping.py` & `oteapi-dlite-0.1.3/oteapi_dlite/strategies/mapping.py`

 * *Files identical despite different names*

### Comparing `oteapi-dlite-0.1.2/oteapi_dlite/strategies/parse.py` & `oteapi-dlite-0.1.3/oteapi_dlite/strategies/parse.py`

 * *Files identical despite different names*

### Comparing `oteapi-dlite-0.1.2/oteapi_dlite/strategies/parse_excel.py` & `oteapi-dlite-0.1.3/oteapi_dlite/strategies/parse_excel.py`

 * *Files 3% similar despite different names*

```diff
@@ -132,18 +132,14 @@
         for name in names:
             inst[name] = rec[name]
 
         # Insert inst into collection
         coll = get_collection(session)
         coll.add(config.label, inst)
 
-        # # Increase refcount of instance to avoid that it is freed when
-        # # returning from this function
-        # inst._incref()  # pylint: disable=protected-access
-
         update_collection(coll)
         return DLiteExcelSessionUpdate(
             collection_id=coll.uuid,
             inst_uuid=inst.uuid,
             label=config.label,
         )
```

### Comparing `oteapi-dlite-0.1.2/oteapi_dlite/strategies/parse_image.py` & `oteapi-dlite-0.1.3/oteapi_dlite/strategies/parse_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         )
         output = ImageDataParseStrategy(core_config).get(parse_strategy_session)
 
         cache = DataCache()
         data = cache.get(output["image_key"])
 
         meta = get_meta("http://onto-ns.com/meta/1.0/Image")
-        inst = meta(dims=data.shape)
+        inst = meta(dimensions=data.shape)
         inst["data"] = data
 
         LOGGER.info("session: %s", session)
 
         coll = get_collection(session)
         coll.add(config.image_label, inst)
```

### Comparing `oteapi-dlite-0.1.2/oteapi_dlite/strategies/serialise.py` & `oteapi-dlite-0.1.3/oteapi_dlite/strategies/serialise.py`

 * *Files identical despite different names*

### Comparing `oteapi-dlite-0.1.2/oteapi_dlite/utils/nputils.py` & `oteapi-dlite-0.1.3/oteapi_dlite/utils/nputils.py`

 * *Files identical despite different names*

### Comparing `oteapi-dlite-0.1.2/oteapi_dlite/utils/utils.py` & `oteapi-dlite-0.1.3/oteapi_dlite/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     if id_ is None:
         collection = dlite.Collection()
         cache.add(collection.asjson(), key=collection.uuid)
     elif id_ not in cache:
         raise CollectionNotFound(
             "Could not find DLite Collection with "
-            f"uuid={session['collection_id']!r}"
+            f"uuid='{session['collection_id']}'"
         )
     else:
         collection = dlite.Collection.from_json(cache.get(id_), id=id_)
 
     if "collection_id" not in session:
         session["collection_id"] = collection.uuid
```

### Comparing `oteapi-dlite-0.1.2/oteapi_dlite.egg-info/PKG-INFO` & `oteapi-dlite-0.1.3/oteapi_dlite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oteapi-dlite
-Version: 0.1.2
+Version: 0.1.3
 Summary: DLite plugin for OTEAPI.
 Home-page: https://github.com/EMMC-ASBL/oteapi-dlite
 Author: team4.0@sintef.no
 Author-email: team4.0@sintef.no
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `oteapi-dlite-0.1.2/oteapi_dlite.egg-info/SOURCES.txt` & `oteapi-dlite-0.1.3/oteapi_dlite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oteapi-dlite-0.1.2/oteapi_dlite.egg-info/entry_points.txt` & `oteapi-dlite-0.1.3/oteapi_dlite.egg-info/entry_points.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,12 +9,13 @@
 
 [oteapi.parse]
 oteapi_dlite.application/vnd.dlite-json = oteapi_dlite.strategies.parse:DLiteParseStrategy
 oteapi_dlite.application/vnd.dlite-parse = oteapi_dlite.strategies.parse:DLiteParseStrategy
 oteapi_dlite.application/vnd.dlite-xlsx = oteapi_dlite.strategies.parse_excel:DLiteExcelStrategy
 oteapi_dlite.application/vnd.dlite-yaml = oteapi_dlite.strategies.parse:DLiteParseStrategy
 oteapi_dlite.image/vnd.dlite-gif = oteapi_dlite.strategies.parse_image:DLiteImageParseStrategy
+oteapi_dlite.image/vnd.dlite-image = oteapi_dlite.strategies.parse_image:DLiteImageParseStrategy
 oteapi_dlite.image/vnd.dlite-jp2 = oteapi_dlite.strategies.parse_image:DLiteImageParseStrategy
 oteapi_dlite.image/vnd.dlite-jpeg = oteapi_dlite.strategies.parse_image:DLiteImageParseStrategy
 oteapi_dlite.image/vnd.dlite-jpg = oteapi_dlite.strategies.parse_image:DLiteImageParseStrategy
 oteapi_dlite.image/vnd.dlite-png = oteapi_dlite.strategies.parse_image:DLiteImageParseStrategy
 oteapi_dlite.image/vnd.dlite-tiff = oteapi_dlite.strategies.parse_image:DLiteImageParseStrategy
```

### Comparing `oteapi-dlite-0.1.2/pyproject.toml` & `oteapi-dlite-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oteapi-dlite-0.1.2/setup.cfg` & `oteapi-dlite-0.1.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [options.entry_points]
 oteapi.parse = 
 	oteapi_dlite.application/vnd.dlite-parse = oteapi_dlite.strategies.parse:DLiteParseStrategy
 	
+	oteapi_dlite.application/vnd.dlite-xlsx = oteapi_dlite.strategies.parse_excel:DLiteExcelStrategy
+	oteapi_dlite.image/vnd.dlite-image = oteapi_dlite.strategies.parse_image:DLiteImageParseStrategy
+	
 	oteapi_dlite.application/vnd.dlite-json = oteapi_dlite.strategies.parse:DLiteParseStrategy
 	oteapi_dlite.application/vnd.dlite-yaml = oteapi_dlite.strategies.parse:DLiteParseStrategy
-	oteapi_dlite.application/vnd.dlite-xlsx = oteapi_dlite.strategies.parse_excel:DLiteExcelStrategy
 	oteapi_dlite.image/vnd.dlite-gif = oteapi_dlite.strategies.parse_image:DLiteImageParseStrategy
 	oteapi_dlite.image/vnd.dlite-jpeg = oteapi_dlite.strategies.parse_image:DLiteImageParseStrategy
 	oteapi_dlite.image/vnd.dlite-jpg = oteapi_dlite.strategies.parse_image:DLiteImageParseStrategy
 	oteapi_dlite.image/vnd.dlite-jp2 = oteapi_dlite.strategies.parse_image:DLiteImageParseStrategy
 	oteapi_dlite.image/vnd.dlite-png = oteapi_dlite.strategies.parse_image:DLiteImageParseStrategy
 	oteapi_dlite.image/vnd.dlite-tiff = oteapi_dlite.strategies.parse_image:DLiteImageParseStrategy
 oteapi.function =
```

### Comparing `oteapi-dlite-0.1.2/setup.py` & `oteapi-dlite-0.1.3/setup.py`

 * *Files identical despite different names*

