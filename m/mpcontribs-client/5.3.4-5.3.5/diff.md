# Comparing `tmp/mpcontribs-client-5.3.4.tar.gz` & `tmp/mpcontribs-client-5.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpcontribs-client-5.3.4.tar", last modified: Wed May 17 18:12:42 2023, max compression
+gzip compressed data, was "mpcontribs-client-5.3.5.tar", last modified: Tue May 23 23:51:53 2023, max compression
```

## Comparing `mpcontribs-client-5.3.4.tar` & `mpcontribs-client-5.3.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:42.809394 mpcontribs-client-5.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-17 18:12:42.809394 mpcontribs-client-5.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:42.797393 mpcontribs-client-5.3.4/mpcontribs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:42.797393 mpcontribs-client-5.3.4/mpcontribs/client/
--rw-r--r--   0 runner    (1001) docker     (123)    85863 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/mpcontribs/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:42.801393 mpcontribs-client-5.3.4/mpcontribs_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-17 18:12:42.000000 mpcontribs-client-5.3.4/mpcontribs_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-17 18:12:42.000000 mpcontribs-client-5.3.4/mpcontribs_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:12:42.000000 mpcontribs-client-5.3.4/mpcontribs_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:12:42.000000 mpcontribs-client-5.3.4/mpcontribs_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-17 18:12:42.000000 mpcontribs-client-5.3.4/mpcontribs_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 18:12:42.000000 mpcontribs-client-5.3.4/mpcontribs_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:42.805394 mpcontribs-client-5.3.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/macos-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/macos-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 18:12:42.809394 mpcontribs-client-5.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:42.805394 mpcontribs-client-5.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-17 18:12:28.000000 mpcontribs-client-5.3.4/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:51:53.870851 mpcontribs-client-5.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-23 23:51:53.870851 mpcontribs-client-5.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:51:53.866851 mpcontribs-client-5.3.5/mpcontribs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:51:53.866851 mpcontribs-client-5.3.5/mpcontribs/client/
+-rw-r--r--   0 runner    (1001) docker     (123)    86143 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/mpcontribs/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:51:53.870851 mpcontribs-client-5.3.5/mpcontribs_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-23 23:51:53.000000 mpcontribs-client-5.3.5/mpcontribs_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-23 23:51:53.000000 mpcontribs-client-5.3.5/mpcontribs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 23:51:53.000000 mpcontribs-client-5.3.5/mpcontribs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 23:51:53.000000 mpcontribs-client-5.3.5/mpcontribs_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-23 23:51:53.000000 mpcontribs-client-5.3.5/mpcontribs_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 23:51:53.000000 mpcontribs-client-5.3.5/mpcontribs_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:51:53.870851 mpcontribs-client-5.3.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/macos-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/macos-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 23:51:53.870851 mpcontribs-client-5.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:51:53.870851 mpcontribs-client-5.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/tests/test_client.py
```

### Comparing `mpcontribs-client-5.3.4/LICENSE` & `mpcontribs-client-5.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.3.4/PKG-INFO` & `mpcontribs-client-5.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcontribs-client
-Version: 5.3.4
+Version: 5.3.5
 Summary: client library for MPContribs API
 Home-page: https://github.com/materialsproject/MPContribs/tree/master/mpcontribs-client
 Author: Patrick Huck
 Author-email: phuck@lbl.gov
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mpcontribs-client-5.3.4/README.md` & `mpcontribs-client-5.3.5/README.md`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.3.4/mpcontribs/client/__init__.py` & `mpcontribs-client-5.3.5/mpcontribs/client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -731,29 +731,38 @@
         op: str = "query",
         resource: str = "contributions",
         pages: int = -1,
     ) -> List[dict]:
         """Avoid URI too long errors"""
         pp_default, pp_max = self._get_per_page_default_max(op=op, resource=resource)
         per_page = pp_default if any(k.endswith("__in") for k in query.keys()) else pp_max
-        query["per_page"] = per_page
         nr_params_to_split = sum(
             len(v) > per_page for v in query.values() if isinstance(v, list)
         )
         if nr_params_to_split > 1:
             raise MPContribsClientError(
                 f"More than one list in query with length > {per_page} not supported!"
             )
 
         queries = []
 
         for k, v in query.items():
-            if isinstance(v, list) and len(v) > per_page:
-                for chunk in grouper(per_page, v):
-                    queries.append({k: list(chunk)})
+            if isinstance(v, list):
+                line_len = len(",".join(v).encode("utf-8"))
+
+                while line_len > 3800:
+                    per_page = int(0.9 * per_page)
+                    vv = v[:per_page]
+                    line_len = len(",".join(vv).encode("utf-8"))
+
+                if len(v) > per_page:
+                    for chunk in grouper(per_page, v):
+                        queries.append({k: list(chunk)})
+
+        query["per_page"] = per_page
 
         if not queries:
             queries = [query]
 
         if len(queries) == 1 and pages and pages > 0:
             queries = []
             for page in range(1, pages+1):
```

### Comparing `mpcontribs-client-5.3.4/mpcontribs_client.egg-info/PKG-INFO` & `mpcontribs-client-5.3.5/mpcontribs_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcontribs-client
-Version: 5.3.4
+Version: 5.3.5
 Summary: client library for MPContribs API
 Home-page: https://github.com/materialsproject/MPContribs/tree/master/mpcontribs-client
 Author: Patrick Huck
 Author-email: phuck@lbl.gov
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mpcontribs-client-5.3.4/mpcontribs_client.egg-info/SOURCES.txt` & `mpcontribs-client-5.3.5/mpcontribs_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.3.4/requirements/deployment.txt` & `mpcontribs-client-5.3.5/requirements/deployment.txt`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
     #   pandas
 pyyaml==6.0
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
-requests==2.30.0
+requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.0
@@ -229,15 +229,15 @@
     # via
     #   mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.5.0
+typing-extensions==4.6.0
     # via
     #   bravado
     #   emmet-core
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
```

### Comparing `mpcontribs-client-5.3.4/requirements/macos-latest_py3.10.txt` & `mpcontribs-client-5.3.5/requirements/macos-latest_py3.10.txt`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
     #   pandas
 pyyaml==6.0
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
-requests==2.30.0
+requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.0
@@ -225,15 +225,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.5.0
+typing-extensions==4.6.0
     # via
     #   bravado
     #   emmet-core
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
```

### Comparing `mpcontribs-client-5.3.4/requirements/macos-latest_py3.10_extras.txt` & `mpcontribs-client-5.3.5/requirements/macos-latest_py3.10_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
     #   pandas
 pyyaml==6.0
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
-requests==2.30.0
+requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.0
@@ -266,15 +266,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.5.0
+typing-extensions==4.6.0
     # via
     #   bravado
     #   emmet-core
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
```

### Comparing `mpcontribs-client-5.3.4/requirements/macos-latest_py3.8.txt` & `mpcontribs-client-5.3.5/requirements/macos-latest_py3.8.txt`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     #   pandas
 pyyaml==6.0
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
-requests==2.30.0
+requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.0
@@ -231,15 +231,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.5.0
+typing-extensions==4.6.0
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
```

### Comparing `mpcontribs-client-5.3.4/requirements/macos-latest_py3.8_extras.txt` & `mpcontribs-client-5.3.5/requirements/macos-latest_py3.8_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,15 @@
     #   pandas
 pyyaml==6.0
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
-requests==2.30.0
+requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.0
@@ -272,15 +272,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.5.0
+typing-extensions==4.6.0
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
```

### Comparing `mpcontribs-client-5.3.4/requirements/macos-latest_py3.9.txt` & `mpcontribs-client-5.3.5/requirements/macos-latest_py3.9.txt`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
     #   pandas
 pyyaml==6.0
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
-requests==2.30.0
+requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.0
@@ -227,15 +227,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.5.0
+typing-extensions==4.6.0
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
```

### Comparing `mpcontribs-client-5.3.4/requirements/macos-latest_py3.9_extras.txt` & `mpcontribs-client-5.3.5/requirements/macos-latest_py3.9_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
     #   pandas
 pyyaml==6.0
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
-requests==2.30.0
+requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.0
@@ -268,15 +268,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.5.0
+typing-extensions==4.6.0
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
```

### Comparing `mpcontribs-client-5.3.4/requirements/ubuntu-latest_py3.10.txt` & `mpcontribs-client-5.3.5/requirements/ubuntu-latest_py3.10.txt`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
     #   pandas
 pyyaml==6.0
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
-requests==2.30.0
+requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.0
@@ -223,15 +223,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.5.0
+typing-extensions==4.6.0
     # via
     #   bravado
     #   emmet-core
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
```

### Comparing `mpcontribs-client-5.3.4/requirements/ubuntu-latest_py3.10_extras.txt` & `mpcontribs-client-5.3.5/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -201,15 +201,15 @@
     #   pandas
 pyyaml==6.0
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
-requests==2.30.0
+requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.0
@@ -264,15 +264,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.5.0
+typing-extensions==4.6.0
     # via
     #   bravado
     #   emmet-core
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
```

### Comparing `mpcontribs-client-5.3.4/requirements/ubuntu-latest_py3.8.txt` & `mpcontribs-client-5.3.5/requirements/ubuntu-latest_py3.8.txt`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
     #   pandas
 pyyaml==6.0
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
-requests==2.30.0
+requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.0
@@ -229,15 +229,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.5.0
+typing-extensions==4.6.0
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
```

### Comparing `mpcontribs-client-5.3.4/requirements/ubuntu-latest_py3.8_extras.txt` & `mpcontribs-client-5.3.5/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -207,15 +207,15 @@
     #   pandas
 pyyaml==6.0
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
-requests==2.30.0
+requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.0
@@ -270,15 +270,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.5.0
+typing-extensions==4.6.0
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
```

### Comparing `mpcontribs-client-5.3.4/requirements/ubuntu-latest_py3.9.txt` & `mpcontribs-client-5.3.5/requirements/ubuntu-latest_py3.9.txt`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
     #   pandas
 pyyaml==6.0
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
-requests==2.30.0
+requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.0
@@ -225,15 +225,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.5.0
+typing-extensions==4.6.0
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
```

### Comparing `mpcontribs-client-5.3.4/requirements/ubuntu-latest_py3.9_extras.txt` & `mpcontribs-client-5.3.5/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
     #   pandas
 pyyaml==6.0
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
-requests==2.30.0
+requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.0
@@ -266,15 +266,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.5.0
+typing-extensions==4.6.0
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
```

### Comparing `mpcontribs-client-5.3.4/setup.py` & `mpcontribs-client-5.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.3.4/tests/test_client.py` & `mpcontribs-client-5.3.5/tests/test_client.py`

 * *Files identical despite different names*

