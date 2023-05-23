# Comparing `tmp/vegafusion-1.3.0rc2.tar.gz` & `tmp/vegafusion-1.3.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vegafusion-1.3.0rc2.tar", last modified: Thu May 18 17:15:23 2023, max compression
+gzip compressed data, was "vegafusion-1.3.0rc3.tar", last modified: Tue May 23 21:55:31 2023, max compression
```

## Comparing `vegafusion-1.3.0rc2.tar` & `vegafusion-1.3.0rc3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:15:23.952783 vegafusion-1.3.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-18 17:15:23.952783 vegafusion-1.3.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-18 17:15:23.952783 vegafusion-1.3.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:15:23.948783 vegafusion-1.3.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/tests/test_conext_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/tests/test_input_utc.py
--rw-r--r--   0 runner    (1001) docker     (123)    36521 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/tests/test_pretransform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/tests/test_pretransform_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/tests/test_row_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/tests/test_save.py
--rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/tests/test_transformed_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/tests/test_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:15:23.948783 vegafusion-1.3.0rc2/vegafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/vegafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/vegafusion/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/vegafusion/compilers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:15:23.948783 vegafusion-1.3.0rc2/vegafusion/connection/
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/vegafusion/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12904 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/vegafusion/connection/duckdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/vegafusion/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/vegafusion/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/vegafusion/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/vegafusion/local_tz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/vegafusion/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    21782 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/vegafusion/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/vegafusion/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/vegafusion/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-18 17:14:10.000000 vegafusion-1.3.0rc2/vegafusion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:15:23.948783 vegafusion-1.3.0rc2/vegafusion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-18 17:15:23.000000 vegafusion-1.3.0rc2/vegafusion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-18 17:15:23.000000 vegafusion-1.3.0rc2/vegafusion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:15:23.000000 vegafusion-1.3.0rc2/vegafusion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 17:15:23.000000 vegafusion-1.3.0rc2/vegafusion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-18 17:15:23.000000 vegafusion-1.3.0rc2/vegafusion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:31.045259 vegafusion-1.3.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-23 21:55:31.045259 vegafusion-1.3.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-23 21:55:31.045259 vegafusion-1.3.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:31.041258 vegafusion-1.3.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/tests/test_conext_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/tests/test_input_utc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38103 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/tests/test_pretransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/tests/test_pretransform_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/tests/test_row_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/tests/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/tests/test_transformed_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/tests/test_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:31.045259 vegafusion-1.3.0rc3/vegafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/compilers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:31.045259 vegafusion-1.3.0rc3/vegafusion/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12904 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/connection/duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/local_tz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21782 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:31.045259 vegafusion-1.3.0rc3/vegafusion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-23 21:55:31.000000 vegafusion-1.3.0rc3/vegafusion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-23 21:55:31.000000 vegafusion-1.3.0rc3/vegafusion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:55:31.000000 vegafusion-1.3.0rc3/vegafusion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-23 21:55:31.000000 vegafusion-1.3.0rc3/vegafusion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 21:55:31.000000 vegafusion-1.3.0rc3/vegafusion.egg-info/top_level.txt
```

### Comparing `vegafusion-1.3.0rc2/LICENSE.txt` & `vegafusion-1.3.0rc3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc2/PKG-INFO` & `vegafusion-1.3.0rc3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegafusion
-Version: 1.3.0rc2
+Version: 1.3.0rc3
 Summary: Core tools for using VegaFusion from Python
 License: BSD-3-Clause
 Keywords: vega,altair,vegafusion,arrow
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vegafusion-1.3.0rc2/README.md` & `vegafusion-1.3.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc2/setup.cfg` & `vegafusion-1.3.0rc3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [bdist_wheel]
 universal = 0
 
 [metadata]
 name = vegafusion
 description = Core tools for using VegaFusion from Python
-version = 1.3.0-rc2
+version = 1.3.0-rc3
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = vega, altair, vegafusion, arrow
 license = BSD-3-Clause
 license_file = LICENSE.txt
 python = "^3.7"
 homepage = "https://vegafusion.io"
@@ -30,14 +30,14 @@
 	altair>=4.2.0
 	pyarrow>=5
 	pandas
 	psutil
 
 [options.extras_require]
 embed = 
-	vegafusion-python-embed==1.3.0-rc2
+	vegafusion-python-embed==1.3.0-rc3
 	vl-convert-python>=0.7.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `vegafusion-1.3.0rc2/tests/test_conext_manager.py` & `vegafusion-1.3.0rc3/tests/test_conext_manager.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc2/tests/test_input_utc.py` & `vegafusion-1.3.0rc3/tests/test_input_utc.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc2/tests/test_pretransform.py` & `vegafusion-1.3.0rc3/tests/test_pretransform.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,25 @@
 import vegafusion as vf
 import json
 import polars as pl
 from datetime import date
 import decimal
 
 
+def get_connections():
+    connections = ["datafusion"]
+    try:
+        import duckdb
+        connections.append("duckdb")
+    except ImportError:
+        pass
+
+    return connections
+
+
 def order_items_spec():
     return json.loads(r"""
 {
   "$schema": "https://vega.github.io/schema/vega/v5.json",
   "background": "white",
   "padding": 5,
   "height": 200,
@@ -1330,14 +1341,59 @@
     vf.runtime.set_connection("duckdb")
     movies = pd.read_json("https://raw.githubusercontent.com/vega/vega-datasets/main/data/movies.json")
     spec = gh_268_hang_spec()
     for i in range(2):
         vf.runtime.pre_transform_datasets(spec, ["data_3"], "UTC", inline_datasets=dict(movies_clean=movies))
 
 
+@pytest.mark.parametrize("connection", get_connections())
+def test_pivot_mixed_case(connection):
+    vf.runtime.set_connection(connection)
+    source_0 = pd.DataFrame.from_records([
+        {"country": "Norway", "type": "gold", "count": 14},
+        {"country": "Norway", "type": "silver", "count": 14},
+        {"country": "Norway", "type": "Gold", "count": 11},
+        {"country": "Germany", "type": "gold", "count": 14},
+        {"country": "Germany", "type": "silver", "count": 10},
+        {"country": "Germany", "type": "bronze", "count": 7},
+        {"country": "Canada", "type": "gold", "count": 11},
+        {"country": "Canada", "type": "silver", "count": 8},
+        {"country": "Canada", "type": "bronze", "count": 10}
+    ])
+    spec = json.loads(r"""
+{
+  "$schema": "https://vega.github.io/schema/vega/v5.json",
+  "data": [
+    {
+      "name": "source_0",
+      "url": "table://source_0"
+    },
+    {
+      "name": "data_0",
+      "source": "source_0",
+      "transform": [
+        {
+          "type": "pivot",
+          "field": "type",
+          "value": "count",
+          "groupby": ["country"]
+        }
+      ]
+    }
+  ]
+}   
+    """)
+
+    datasets, warnings = vf.runtime.pre_transform_datasets(
+        spec, ["data_0"], "UTC", inline_datasets=dict(source_0=source_0)
+    )
+
+    assert set(datasets[0].columns.tolist()) == {"gold", "Gold", "silver", "bronze", "country"}
+
+
 def gh_268_hang_spec():
     return json.loads(r""" 
     {
       "$schema": "https://vega.github.io/schema/vega/v5.json",
       "data": [
         {
           "name": "interval_intervalselection__store"
```

### Comparing `vegafusion-1.3.0rc2/tests/test_pretransform_specs.py` & `vegafusion-1.3.0rc3/tests/test_pretransform_specs.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc2/tests/test_row_limit.py` & `vegafusion-1.3.0rc3/tests/test_row_limit.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc2/tests/test_save.py` & `vegafusion-1.3.0rc3/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc2/tests/test_transformed_data.py` & `vegafusion-1.3.0rc3/tests/test_transformed_data.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc2/tests/test_transformer.py` & `vegafusion-1.3.0rc3/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc2/vegafusion/__init__.py` & `vegafusion-1.3.0rc3/vegafusion/__init__.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc2/vegafusion/compilers.py` & `vegafusion-1.3.0rc3/vegafusion/compilers.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc2/vegafusion/connection/__init__.py` & `vegafusion-1.3.0rc3/vegafusion/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc2/vegafusion/connection/duckdb.py` & `vegafusion-1.3.0rc3/vegafusion/connection/duckdb.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc2/vegafusion/evaluation.py` & `vegafusion-1.3.0rc3/vegafusion/evaluation.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc2/vegafusion/local_tz.py` & `vegafusion-1.3.0rc3/vegafusion/local_tz.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc2/vegafusion/renderer.py` & `vegafusion-1.3.0rc3/vegafusion/renderer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc2/vegafusion/runtime.py` & `vegafusion-1.3.0rc3/vegafusion/runtime.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc2/vegafusion/save.py` & `vegafusion-1.3.0rc3/vegafusion/save.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc2/vegafusion/transformer.py` & `vegafusion-1.3.0rc3/vegafusion/transformer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc2/vegafusion/utils.py` & `vegafusion-1.3.0rc3/vegafusion/utils.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc2/vegafusion.egg-info/PKG-INFO` & `vegafusion-1.3.0rc3/vegafusion.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegafusion
-Version: 1.3.0rc2
+Version: 1.3.0rc3
 Summary: Core tools for using VegaFusion from Python
 License: BSD-3-Clause
 Keywords: vega,altair,vegafusion,arrow
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vegafusion-1.3.0rc2/vegafusion.egg-info/SOURCES.txt` & `vegafusion-1.3.0rc3/vegafusion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

