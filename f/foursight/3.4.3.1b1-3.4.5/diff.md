# Comparing `tmp/foursight-3.4.3.1b1.tar.gz` & `tmp/foursight-3.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight-3.4.3.1b1.tar", max compression
+gzip compressed data, was "foursight-3.4.5.tar", max compression
```

## Comparing `foursight-3.4.3.1b1.tar` & `foursight-3.4.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1083 2022-09-07 10:59:14.705392 foursight-3.4.3.1b1/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-01-19 14:12:17.947754 foursight-3.4.3.1b1/chalicelib_fourfront/__init__.py
--rw-r--r--   0        0        0     1055 2023-03-29 20:27:15.171164 foursight-3.4.3.1b1/chalicelib_fourfront/app_utils.py
--rw-r--r--   0        0        0     5405 2023-01-19 14:12:17.952115 foursight-3.4.3.1b1/chalicelib_fourfront/check_schedules.py
--rw-r--r--   0        0        0    53878 2023-02-27 17:05:51.839220 foursight-3.4.3.1b1/chalicelib_fourfront/check_setup.json
--rw-r--r--   0        0        0      249 2023-01-19 14:12:17.956201 foursight-3.4.3.1b1/chalicelib_fourfront/checks/__init__.py
--rw-r--r--   0        0        0    60938 2023-05-01 15:36:32.611790 foursight-3.4.3.1b1/chalicelib_fourfront/checks/audit_checks.py
--rw-r--r--   0        0        0    37766 2023-01-19 14:12:17.963001 foursight-3.4.3.1b1/chalicelib_fourfront/checks/badge_checks.py
--rw-r--r--   0        0        0    11548 2023-01-19 14:12:17.965655 foursight-3.4.3.1b1/chalicelib_fourfront/checks/deployment_checks.py
--rw-r--r--   0        0        0     2939 2023-01-25 11:36:46.617974 foursight-3.4.3.1b1/chalicelib_fourfront/checks/ecs_checks.py
--rw-r--r--   0        0        0     3914 2023-01-19 14:12:17.970674 foursight-3.4.3.1b1/chalicelib_fourfront/checks/es_checks.py
--rw-r--r--   0        0        0    14578 2023-01-19 14:12:17.974522 foursight-3.4.3.1b1/chalicelib_fourfront/checks/header_checks.py
--rw-r--r--   0        0        0      262 2023-01-19 14:12:17.974848 foursight-3.4.3.1b1/chalicelib_fourfront/checks/helpers/confchecks.py
--rw-r--r--   0        0        0    44428 2023-01-19 14:12:17.975418 foursight-3.4.3.1b1/chalicelib_fourfront/checks/helpers/google_utils.py
--rw-r--r--   0        0        0    95229 2023-01-19 14:12:17.978748 foursight-3.4.3.1b1/chalicelib_fourfront/checks/helpers/wfr_utils.py
--rw-r--r--   0        0        0    17372 2023-01-19 14:12:17.979325 foursight-3.4.3.1b1/chalicelib_fourfront/checks/helpers/wfrset_utils.py
--rw-r--r--   0        0        0     3686 2023-01-19 14:12:17.979607 foursight-3.4.3.1b1/chalicelib_fourfront/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0    97361 2023-01-19 14:12:17.983575 foursight-3.4.3.1b1/chalicelib_fourfront/checks/higlass_checks.py
--rw-r--r--   0        0        0    32926 2023-01-19 14:12:17.989004 foursight-3.4.3.1b1/chalicelib_fourfront/checks/release_updates_checks.py
--rw-r--r--   0        0        0    45209 2023-04-27 02:48:56.047051 foursight-3.4.3.1b1/chalicelib_fourfront/checks/system_checks.py
--rw-r--r--   0        0        0   127978 2023-01-26 16:17:00.941264 foursight-3.4.3.1b1/chalicelib_fourfront/checks/wfr_checks.py
--rw-r--r--   0        0        0    43470 2023-01-19 14:12:18.009971 foursight-3.4.3.1b1/chalicelib_fourfront/checks/wfr_encode_checks.py
--rw-r--r--   0        0        0   137820 2023-01-25 11:33:59.675086 foursight-3.4.3.1b1/chalicelib_fourfront/checks/wrangler_checks.py
--rw-r--r--   0        0        0      621 2023-03-29 20:27:15.171432 foursight-3.4.3.1b1/chalicelib_fourfront/package.py
--rw-r--r--   0        0        0      316 2023-03-29 19:16:47.518681 foursight-3.4.3.1b1/chalicelib_fourfront/vars.py
--rw-r--r--   0        0        0     1265 2023-05-03 19:31:54.131994 foursight-3.4.3.1b1/pyproject.toml
--rw-r--r--   0        0        0     1539 1970-01-01 00:00:00.000000 foursight-3.4.3.1b1/setup.py
--rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 foursight-3.4.3.1b1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-09-07 10:59:14.705392 foursight-3.4.5/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-01-19 14:12:17.947754 foursight-3.4.5/chalicelib_fourfront/__init__.py
+-rw-r--r--   0        0        0     1055 2023-03-29 20:27:15.171164 foursight-3.4.5/chalicelib_fourfront/app_utils.py
+-rw-r--r--   0        0        0     5405 2023-01-19 14:12:17.952115 foursight-3.4.5/chalicelib_fourfront/check_schedules.py
+-rw-r--r--   0        0        0    54459 2023-05-19 14:11:42.736082 foursight-3.4.5/chalicelib_fourfront/check_setup.json
+-rw-r--r--   0        0        0      249 2023-01-19 14:12:17.956201 foursight-3.4.5/chalicelib_fourfront/checks/__init__.py
+-rw-r--r--   0        0        0    60950 2023-05-19 14:11:42.736936 foursight-3.4.5/chalicelib_fourfront/checks/audit_checks.py
+-rw-r--r--   0        0        0    37766 2023-01-19 14:12:17.963001 foursight-3.4.5/chalicelib_fourfront/checks/badge_checks.py
+-rw-r--r--   0        0        0    11548 2023-01-19 14:12:17.965655 foursight-3.4.5/chalicelib_fourfront/checks/deployment_checks.py
+-rw-r--r--   0        0        0     2939 2023-01-25 11:36:46.617974 foursight-3.4.5/chalicelib_fourfront/checks/ecs_checks.py
+-rw-r--r--   0        0        0     3914 2023-01-19 14:12:17.970674 foursight-3.4.5/chalicelib_fourfront/checks/es_checks.py
+-rw-r--r--   0        0        0    15609 2023-05-19 14:11:42.737293 foursight-3.4.5/chalicelib_fourfront/checks/header_checks.py
+-rw-r--r--   0        0        0      262 2023-01-19 14:12:17.974848 foursight-3.4.5/chalicelib_fourfront/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0    44428 2023-01-19 14:12:17.975418 foursight-3.4.5/chalicelib_fourfront/checks/helpers/google_utils.py
+-rw-r--r--   0        0        0    95229 2023-01-19 14:12:17.978748 foursight-3.4.5/chalicelib_fourfront/checks/helpers/wfr_utils.py
+-rw-r--r--   0        0        0    17372 2023-01-19 14:12:17.979325 foursight-3.4.5/chalicelib_fourfront/checks/helpers/wfrset_utils.py
+-rw-r--r--   0        0        0     3686 2023-01-19 14:12:17.979607 foursight-3.4.5/chalicelib_fourfront/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0    97361 2023-01-19 14:12:17.983575 foursight-3.4.5/chalicelib_fourfront/checks/higlass_checks.py
+-rw-r--r--   0        0        0    32926 2023-01-19 14:12:17.989004 foursight-3.4.5/chalicelib_fourfront/checks/release_updates_checks.py
+-rw-r--r--   0        0        0    45209 2023-04-27 02:48:56.047051 foursight-3.4.5/chalicelib_fourfront/checks/system_checks.py
+-rw-r--r--   0        0        0   127978 2023-01-26 16:17:00.941264 foursight-3.4.5/chalicelib_fourfront/checks/wfr_checks.py
+-rw-r--r--   0        0        0    43470 2023-01-19 14:12:18.009971 foursight-3.4.5/chalicelib_fourfront/checks/wfr_encode_checks.py
+-rw-r--r--   0        0        0   137808 2023-05-19 14:11:42.738749 foursight-3.4.5/chalicelib_fourfront/checks/wrangler_checks.py
+-rw-r--r--   0        0        0      621 2023-03-29 20:27:15.171432 foursight-3.4.5/chalicelib_fourfront/package.py
+-rw-r--r--   0        0        0      316 2023-03-29 19:16:47.518681 foursight-3.4.5/chalicelib_fourfront/vars.py
+-rw-r--r--   0        0        0     1257 2023-05-19 15:21:58.800911 foursight-3.4.5/pyproject.toml
+-rw-r--r--   0        0        0     1531 1970-01-01 00:00:00.000000 foursight-3.4.5/setup.py
+-rw-r--r--   0        0        0     1072 1970-01-01 00:00:00.000000 foursight-3.4.5/PKG-INFO
```

### Comparing `foursight-3.4.3.1b1/LICENSE.txt` & `foursight-3.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight-3.4.3.1b1/chalicelib_fourfront/app_utils.py` & `foursight-3.4.5/chalicelib_fourfront/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.3.1b1/chalicelib_fourfront/check_schedules.py` & `foursight-3.4.5/chalicelib_fourfront/check_schedules.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.3.1b1/chalicelib_fourfront/check_setup.json` & `foursight-3.4.5/chalicelib_fourfront/check_setup.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.991304347826087%*

 * *Differences: {"'prepare_static_headers_Chromatin_Tracing'": "OrderedDict([('title', 'Chromatin Tracing'), "*

 * *                                               "('group', 'Static headers checks'), ('schedule', "*

 * *                                               "OrderedDict([('morning_checks_3', "*

 * *                                               "OrderedDict([('data', "*

 * *                                               "OrderedDict([('dependencies', []), ('kwargs', "*

 * *                                               "OrderedDict([('pri […]*

```diff
@@ -1358,14 +1358,34 @@
                         "primary": true
                     }
                 }
             }
         },
         "title": "Prepare static headers"
     },
+    "prepare_static_headers_Chromatin_Tracing": {
+        "group": "Static headers checks",
+        "schedule": {
+            "morning_checks_3": {
+                "data": {
+                    "dependencies": [],
+                    "kwargs": {
+                        "primary": true
+                    }
+                },
+                "hotseat": {
+                    "dependencies": [],
+                    "kwargs": {
+                        "primary": true
+                    }
+                }
+            }
+        },
+        "title": "Chromatin Tracing"
+    },
     "prepare_static_headers_DNase_HiC": {
         "group": "Static headers checks",
         "schedule": {
             "morning_checks_2": {
                 "data": {
                     "dependencies": [],
                     "kwargs": {
```

### Comparing `foursight-3.4.3.1b1/chalicelib_fourfront/checks/audit_checks.py` & `foursight-3.4.5/chalicelib_fourfront/checks/audit_checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -453,15 +453,15 @@
                 continue
             elif 'biorxiv.org' in url.lower():
                 # biorxiv does not allow programmatic requests - skip
                 continue
             if url.startswith('#'):  # section of static page
                 url = result['@id'] + url
             if url.startswith('/'):  # fill in appropriate url for relative link
-                url = server + url
+                url = server.rstrip('/') + url
             if url.startswith(server.rstrip('/') + '/search/') or url.startswith(server.rstrip('/') + '/browse/'):
                 continue
             try:
                 headers = {'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/50.0.2661.102 Safari/537.36'}
                 request = requests.get(url.replace('&amp;', '&'), timeout=2, headers=headers)
                 if request.status_code == 403 and 'doi.org' in url:
                     # requests to doi.org that get redirected to biorxiv fail with 403
```

### Comparing `foursight-3.4.3.1b1/chalicelib_fourfront/checks/badge_checks.py` & `foursight-3.4.5/chalicelib_fourfront/checks/badge_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.3.1b1/chalicelib_fourfront/checks/deployment_checks.py` & `foursight-3.4.5/chalicelib_fourfront/checks/deployment_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.3.1b1/chalicelib_fourfront/checks/ecs_checks.py` & `foursight-3.4.5/chalicelib_fourfront/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.3.1b1/chalicelib_fourfront/checks/es_checks.py` & `foursight-3.4.5/chalicelib_fourfront/checks/es_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.3.1b1/chalicelib_fourfront/checks/header_checks.py` & `foursight-3.4.5/chalicelib_fourfront/checks/header_checks.py`

 * *Files 5% similar despite different names*

```diff
@@ -308,7 +308,27 @@
 
 @action_function()
 def patch_static_headers_DNase_HiC(connection, **kwargs):
     action = ActionResult(connection, 'patch_static_headers_DNase_HiC')
     # get latest results from prepare_static_headers
     patch_items_with_headers(connection, action, kwargs)
     return action
+
+#Chromatin Tracing
+@check_function()
+def prepare_static_headers_Chromatin_Tracing(connection, **kwargs):
+     check = CheckResult(connection, 'prepare_static_headers_Chromatin_Tracing')
+     add_search = '/search/?experiments_in_set.experiment_type.display_title=multiplexed+FISH'
+     remove_search = '/search/?type=ExperimentSetReplicate&experimentset_type=replicate&experiments_in_set.experiment_type.display_title%21=multiplexed+FISH'
+     header_at_id = '/static-sections/a09a2833-b56b-4e81-8eff-bb8ae6aaa596/'
+     check.action = 'patch_static_headers_Chromatin_Tracing'
+     find_items_for_header_processing(connection, check, header_at_id,
+                                      add_search, remove_search)
+     return check
+
+
+@action_function()
+def patch_static_headers_Chromatin_Tracing(connection, **kwargs):
+     action = ActionResult(connection, 'patch_static_headers_Chromatin_Tracing')
+     # get latest results from prepare_static_headers
+     patch_items_with_headers(connection, action, kwargs)
+     return action
```

### Comparing `foursight-3.4.3.1b1/chalicelib_fourfront/checks/helpers/google_utils.py` & `foursight-3.4.5/chalicelib_fourfront/checks/helpers/google_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.3.1b1/chalicelib_fourfront/checks/helpers/wfr_utils.py` & `foursight-3.4.5/chalicelib_fourfront/checks/helpers/wfr_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.3.1b1/chalicelib_fourfront/checks/helpers/wfrset_utils.py` & `foursight-3.4.5/chalicelib_fourfront/checks/helpers/wfrset_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.3.1b1/chalicelib_fourfront/checks/helpers/wrangler_utils.py` & `foursight-3.4.5/chalicelib_fourfront/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.3.1b1/chalicelib_fourfront/checks/higlass_checks.py` & `foursight-3.4.5/chalicelib_fourfront/checks/higlass_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.3.1b1/chalicelib_fourfront/checks/release_updates_checks.py` & `foursight-3.4.5/chalicelib_fourfront/checks/release_updates_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.3.1b1/chalicelib_fourfront/checks/system_checks.py` & `foursight-3.4.5/chalicelib_fourfront/checks/system_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.3.1b1/chalicelib_fourfront/checks/wfr_checks.py` & `foursight-3.4.5/chalicelib_fourfront/checks/wfr_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.3.1b1/chalicelib_fourfront/checks/wfr_encode_checks.py` & `foursight-3.4.5/chalicelib_fourfront/checks/wfr_encode_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.3.1b1/chalicelib_fourfront/checks/wrangler_checks.py` & `foursight-3.4.5/chalicelib_fourfront/checks/wrangler_checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1335,17 +1335,17 @@
         "dna-dna multi-way interactions of selected loci": "3/4/5-C (multi-contact)",
         "dna-dna pairwise interactions of enriched regions": "IP-based 3C",
         "dna-dna pairwise interactions of selected loci": "3/4/5-C",
         "ligation-free 3c": "Ligation-free 3C",
         "transcription": "Transcription",
         "transcription - single cell": "Transcription",
         "rna-dna pairwise interactions": "RNA-DNA HiC",
-        "fixed sample dna localization": "DNA FISH",
-        "chromatin tracing": "DNA FISH",
-        "fixed sample rna localization": "RNA FISH",
+        "fixed sample dna localization": "FISH",
+        "chromatin tracing": "FISH",
+        "fixed sample rna localization": "FISH",
         "single particle tracking": "SPT",
         "context-dependent reporter expression": "Reporter Expression",
         "scanning electron microscopy": "SEM",
         "transmission electron microscopy": "TEM",
         "immunofluorescence": "Immunofluorescence",
         "synthetic condensation": "OptoDroplet",
         "capture hi-c": "Enrichment Hi-C"
```

### Comparing `foursight-3.4.3.1b1/chalicelib_fourfront/package.py` & `foursight-3.4.5/chalicelib_fourfront/package.py`

 * *Files identical despite different names*

### Comparing `foursight-3.4.3.1b1/pyproject.toml` & `foursight-3.4.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight"
-version = "3.4.3.1b1"
+version = "3.4.5"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "chalicelib_fourfront" }
 ]
 
@@ -20,15 +20,15 @@
 elasticsearch = "^7.13.4"
 elasticsearch-dsl = "^7.0.0"
 gitpython = "^3.1.2"
 pytz = "^2020.1"
 tibanna_ff = ">=0.22.5"
 ## adding foursight-core
 # use below for deployment
-foursight-core = "4.1.1.1b1"
+foursight-core = "4.1.2"
 # use below for tests but not for deployment
 # foursight-core = { git = "https://github.com/4dn-dcic/foursight-core.git", branch="master" }
 pytest = "5.1.2"
 gspread = ">=3.6.0"
 oauth2client = ">=4.1.3"
 pandas = ">=1.1.4"
```

### Comparing `foursight-3.4.3.1b1/setup.py` & `foursight-3.4.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ['Jinja2==2.10.1',
  'MarkupSafe==1.1.1',
  'PyJWT>=2.5.0,<3.0.0',
  'click>=7.1.2,<8.0.0',
  'dcicutils==7.4.0',
  'elasticsearch-dsl>=7.0.0,<8.0.0',
  'elasticsearch>=7.13.4,<8.0.0',
- 'foursight-core==4.1.1.1b1',
+ 'foursight-core==4.1.2',
  'geocoder==1.38.1',
  'gitpython>=3.1.2,<4.0.0',
  'google-api-python-client>=1.7.4,<2.0.0',
  'gspread>=3.6.0',
  'oauth2client>=4.1.3',
  'pandas>=1.1.4',
  'pytest==5.1.2',
@@ -34,15 +34,15 @@
                      'encrypt-accounts-file = '
                      'foursight_core.scripts.encrypt_accounts_file:main',
                      'publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'foursight',
-    'version': '3.4.3.1b1',
+    'version': '3.4.5',
     'description': 'Serverless Chalice Application for Monitoring',
     'long_description': 'None',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `foursight-3.4.3.1b1/PKG-INFO` & `foursight-3.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight
-Version: 3.4.3.1b1
+Version: 3.4.5
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Requires-Dist: Jinja2 (==2.10.1)
 Requires-Dist: MarkupSafe (==1.1.1)
 Requires-Dist: PyJWT (>=2.5.0,<3.0.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
 Requires-Dist: dcicutils (==7.4.0)
 Requires-Dist: elasticsearch (>=7.13.4,<8.0.0)
 Requires-Dist: elasticsearch-dsl (>=7.0.0,<8.0.0)
-Requires-Dist: foursight-core (==4.1.1.1b1)
+Requires-Dist: foursight-core (==4.1.2)
 Requires-Dist: geocoder (==1.38.1)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: google-api-python-client (>=1.7.4,<2.0.0)
 Requires-Dist: gspread (>=3.6.0)
 Requires-Dist: oauth2client (>=4.1.3)
 Requires-Dist: pandas (>=1.1.4)
 Requires-Dist: pytest (==5.1.2)
```

