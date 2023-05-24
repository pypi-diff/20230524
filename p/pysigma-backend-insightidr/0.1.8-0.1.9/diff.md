# Comparing `tmp/pysigma-backend-insightidr-0.1.8.tar.gz` & `tmp/pysigma-backend-insightidr-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma-backend-insightidr-0.1.8.tar", max compression
+gzip compressed data, was "pysigma-backend-insightidr-0.1.9.tar", max compression
```

## Comparing `pysigma-backend-insightidr-0.1.8.tar` & `pysigma-backend-insightidr-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    26526 2022-09-17 23:25:28.414988 pysigma-backend-insightidr-0.1.8/LICENSE
--rw-r--r--   0        0        0      555 2022-09-17 23:25:28.414988 pysigma-backend-insightidr-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       43 2022-09-17 23:25:28.414988 pysigma-backend-insightidr-0.1.8/sigma/backends/insight_idr/__init__.py
--rw-r--r--   0        0        0    10558 2022-09-17 23:25:28.414988 pysigma-backend-insightidr-0.1.8/sigma/backends/insight_idr/insight_idr.py
--rw-r--r--   0        0        0       45 2022-09-17 23:25:28.414988 pysigma-backend-insightidr-0.1.8/sigma/pipelines/insight_idr/__init__.py
--rw-r--r--   0        0        0    10360 2022-09-17 23:25:28.414988 pysigma-backend-insightidr-0.1.8/sigma/pipelines/insight_idr/insight_idr.py
--rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 pysigma-backend-insightidr-0.1.8/setup.py
--rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 pysigma-backend-insightidr-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-05-24 15:32:01.026600 pysigma-backend-insightidr-0.1.9/LICENSE
+-rw-r--r--   0        0        0      555 2023-05-24 15:32:01.026600 pysigma-backend-insightidr-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       96 2023-05-24 15:32:01.026600 pysigma-backend-insightidr-0.1.9/sigma/backends/insight_idr/__init__.py
+-rw-r--r--   0        0        0    10559 2023-05-24 15:32:01.026600 pysigma-backend-insightidr-0.1.9/sigma/backends/insight_idr/insight_idr.py
+-rw-r--r--   0        0        0      112 2023-05-24 15:32:01.026600 pysigma-backend-insightidr-0.1.9/sigma/pipelines/insight_idr/__init__.py
+-rw-r--r--   0        0        0    10360 2023-05-24 15:32:01.026600 pysigma-backend-insightidr-0.1.9/sigma/pipelines/insight_idr/insight_idr.py
+-rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 pysigma-backend-insightidr-0.1.9/setup.py
+-rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 pysigma-backend-insightidr-0.1.9/PKG-INFO
```

### Comparing `pysigma-backend-insightidr-0.1.8/LICENSE` & `pysigma-backend-insightidr-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma-backend-insightidr-0.1.8/pyproject.toml` & `pysigma-backend-insightidr-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "pysigma-backend-insightidr"
-version = "0.1.8"
+version = "0.1.9"
 description = "pySigma Rapid7 InsightIDR backend"
 authors = ["Micah Babinski <m.babinski.88@gmail.com>"]
 license = "LGPL-2.1-only"
 repository = "https://github.com/SigmaHQ/pySigma-backend-insightidr"
 packages = [
     { include = "sigma" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pysigma = "^0.8.1"
+pysigma = "^0.9.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.1"
 pytest-cov = "^3.0.0"
 coverage = "^6.3.2"
 
 [build-system]
```

### Comparing `pysigma-backend-insightidr-0.1.8/sigma/backends/insight_idr/insight_idr.py` & `pysigma-backend-insightidr-0.1.9/sigma/backends/insight_idr/insight_idr.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
         return f"""where({query})"""
 
     # finalize query the way it appears under Detection Rules -> Attacker Behavior Analytics -> Rule Logic
     def finalize_query_leql_detection_definition(self, rule: SigmaRule, query: str, index: int, state: ConversionState) -> str:
         entry_type = rule.logsource.category
         formatted_query = "\n  ".join(re.split("(AND |OR )", query))
         return f"""from(
-  entry_type = {entry_type}"
+  entry_type = "{entry_type}"
 )
 where(
   {formatted_query}
 )"""
 
     def finalize_output_leql_advanced_search(self, queries: List[str]) -> List[str]:
         return self.finalize_output_default(queries)
```

### Comparing `pysigma-backend-insightidr-0.1.8/sigma/pipelines/insight_idr/insight_idr.py` & `pysigma-backend-insightidr-0.1.9/sigma/pipelines/insight_idr/insight_idr.py`

 * *Files identical despite different names*

### Comparing `pysigma-backend-insightidr-0.1.8/setup.py` & `pysigma-backend-insightidr-0.1.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['sigma', 'sigma.backends.insight_idr', 'sigma.pipelines.insight_idr']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pysigma>=0.8.1,<0.9.0']
+['pysigma>=0.9.5,<0.10.0']
 
 setup_kwargs = {
     'name': 'pysigma-backend-insightidr',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'pySigma Rapid7 InsightIDR backend',
     'long_description': 'None',
     'author': 'Micah Babinski',
     'author_email': 'm.babinski.88@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/SigmaHQ/pySigma-backend-insightidr',
```

### Comparing `pysigma-backend-insightidr-0.1.8/PKG-INFO` & `pysigma-backend-insightidr-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-insightidr
-Version: 0.1.8
+Version: 0.1.9
 Summary: pySigma Rapid7 InsightIDR backend
 Home-page: https://github.com/SigmaHQ/pySigma-backend-insightidr
 License: LGPL-2.1-only
 Author: Micah Babinski
 Author-email: m.babinski.88@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: pysigma (>=0.8.1,<0.9.0)
+Requires-Dist: pysigma (>=0.9.5,<0.10.0)
 Project-URL: Repository, https://github.com/SigmaHQ/pySigma-backend-insightidr
```

