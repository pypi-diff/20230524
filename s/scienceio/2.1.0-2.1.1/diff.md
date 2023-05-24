# Comparing `tmp/scienceio-2.1.0.tar.gz` & `tmp/scienceio-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scienceio-2.1.0.tar", last modified: Mon May 22 20:14:26 2023, max compression
+gzip compressed data, was "scienceio-2.1.1.tar", last modified: Wed May 24 16:09:01 2023, max compression
```

## Comparing `scienceio-2.1.0.tar` & `scienceio-2.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      148 2023-05-22 20:14:09.208550 scienceio-2.1.0/.flake8
--rw-r--r--   0        0        0        2 2023-05-22 20:14:09.208550 scienceio-2.1.0/.fourmat
--rw-r--r--   0        0        0      107 2023-05-22 20:14:09.208550 scienceio-2.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0      226 2023-05-22 20:14:09.208550 scienceio-2.1.0/.github/pull_request_template.md
--rw-r--r--   0        0        0     1773 2023-05-22 20:14:09.208550 scienceio-2.1.0/.github/workflows/deploy_staging.yml
--rw-r--r--   0        0        0     1485 2023-05-22 20:14:09.208550 scienceio-2.1.0/.github/workflows/pull_request.yml
--rw-r--r--   0        0        0     1728 2023-05-22 20:14:09.208550 scienceio-2.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     2371 2023-05-22 20:14:09.208550 scienceio-2.1.0/.gitignore
--rw-r--r--   0        0        0      234 2023-05-22 20:14:09.208550 scienceio-2.1.0/CODEOWNERS
--rw-r--r--   0        0        0     2588 2023-05-22 20:14:09.212550 scienceio-2.1.0/PUBLISHING.md
--rw-r--r--   0        0        0      336 2023-05-22 20:14:09.212550 scienceio-2.1.0/Pipfile
--rw-r--r--   0        0        0    36713 2023-05-22 20:14:09.212550 scienceio-2.1.0/Pipfile.lock
--rw-r--r--   0        0        0     1366 2023-05-22 20:14:09.212550 scienceio-2.1.0/README.md
--rw-r--r--   0        0        0     3083 2023-05-22 20:14:09.212550 scienceio-2.1.0/examples/analytics.py
--rw-r--r--   0        0        0     2591 2023-05-22 20:14:09.212550 scienceio-2.1.0/examples/convert_data_model.py
--rw-r--r--   0        0        0    10051 2023-05-22 20:14:09.212550 scienceio-2.1.0/examples/example-analytics-1.ipynb
--rw-r--r--   0        0        0    46436 2023-05-22 20:14:09.212550 scienceio-2.1.0/examples/example-analytics-2.ipynb
--rw-r--r--   0        0        0    12058 2023-05-22 20:14:09.212550 scienceio-2.1.0/examples/example-annotate-onboarding-text.ipynb
--rw-r--r--   0        0        0     9677 2023-05-22 20:14:09.212550 scienceio-2.1.0/examples/example-onboarding.ipynb
--rw-r--r--   0        0        0      877 2023-05-22 20:14:09.212550 scienceio-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      165 2023-05-22 20:14:09.212550 scienceio-2.1.0/src/scienceio/__init__.py
--rw-r--r--   0        0        0    10571 2023-05-22 20:14:09.212550 scienceio-2.1.0/src/scienceio/scienceio.py
--rwxr-xr-x   0        0        0       47 2023-05-22 20:14:09.212550 scienceio-2.1.0/test.sh
--rw-r--r--   0        0        0        0 2023-05-22 20:14:09.212550 scienceio-2.1.0/tests/__init__.py
--rw-r--r--   0        0        0    13798 2023-05-22 20:14:09.212550 scienceio-2.1.0/tests/__snapshots__/test_scienceio.ambr
--rw-r--r--   0        0        0     4839 2023-05-22 20:14:09.212550 scienceio-2.1.0/tests/conftest.py
--rw-r--r--   0        0        0     2634 2023-05-22 20:14:09.212550 scienceio-2.1.0/tests/test_scienceio.py
--rw-r--r--   0        0        0     1854 1970-01-01 00:00:00.000000 scienceio-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      148 2023-05-24 16:08:46.229284 scienceio-2.1.1/.flake8
+-rw-r--r--   0        0        0        2 2023-05-24 16:08:46.229284 scienceio-2.1.1/.fourmat
+-rw-r--r--   0        0        0      107 2023-05-24 16:08:46.229284 scienceio-2.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      226 2023-05-24 16:08:46.229284 scienceio-2.1.1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1773 2023-05-24 16:08:46.229284 scienceio-2.1.1/.github/workflows/deploy_staging.yml
+-rw-r--r--   0        0        0     1485 2023-05-24 16:08:46.229284 scienceio-2.1.1/.github/workflows/pull_request.yml
+-rw-r--r--   0        0        0     1728 2023-05-24 16:08:46.229284 scienceio-2.1.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2371 2023-05-24 16:08:46.229284 scienceio-2.1.1/.gitignore
+-rw-r--r--   0        0        0      234 2023-05-24 16:08:46.229284 scienceio-2.1.1/CODEOWNERS
+-rw-r--r--   0        0        0     2588 2023-05-24 16:08:46.229284 scienceio-2.1.1/PUBLISHING.md
+-rw-r--r--   0        0        0      336 2023-05-24 16:08:46.229284 scienceio-2.1.1/Pipfile
+-rw-r--r--   0        0        0    36713 2023-05-24 16:08:46.229284 scienceio-2.1.1/Pipfile.lock
+-rw-r--r--   0        0        0     1366 2023-05-24 16:08:46.229284 scienceio-2.1.1/README.md
+-rw-r--r--   0        0        0     3083 2023-05-24 16:08:46.229284 scienceio-2.1.1/examples/analytics.py
+-rw-r--r--   0        0        0     2591 2023-05-24 16:08:46.229284 scienceio-2.1.1/examples/convert_data_model.py
+-rw-r--r--   0        0        0    10051 2023-05-24 16:08:46.229284 scienceio-2.1.1/examples/example-analytics-1.ipynb
+-rw-r--r--   0        0        0    46436 2023-05-24 16:08:46.233284 scienceio-2.1.1/examples/example-analytics-2.ipynb
+-rw-r--r--   0        0        0    12058 2023-05-24 16:08:46.233284 scienceio-2.1.1/examples/example-annotate-onboarding-text.ipynb
+-rw-r--r--   0        0        0     9677 2023-05-24 16:08:46.233284 scienceio-2.1.1/examples/example-onboarding.ipynb
+-rw-r--r--   0        0        0      877 2023-05-24 16:08:46.233284 scienceio-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0      165 2023-05-24 16:08:46.233284 scienceio-2.1.1/src/scienceio/__init__.py
+-rw-r--r--   0        0        0    10465 2023-05-24 16:08:46.233284 scienceio-2.1.1/src/scienceio/scienceio.py
+-rwxr-xr-x   0        0        0       47 2023-05-24 16:08:46.233284 scienceio-2.1.1/test.sh
+-rw-r--r--   0        0        0        0 2023-05-24 16:08:46.233284 scienceio-2.1.1/tests/__init__.py
+-rw-r--r--   0        0        0    14998 2023-05-24 16:08:46.233284 scienceio-2.1.1/tests/__snapshots__/test_scienceio.ambr
+-rw-r--r--   0        0        0     4839 2023-05-24 16:08:46.233284 scienceio-2.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     2634 2023-05-24 16:08:46.233284 scienceio-2.1.1/tests/test_scienceio.py
+-rw-r--r--   0        0        0     1854 1970-01-01 00:00:00.000000 scienceio-2.1.1/PKG-INFO
```

### Comparing `scienceio-2.1.0/.github/workflows/deploy_staging.yml` & `scienceio-2.1.1/.github/workflows/deploy_staging.yml`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.0/.github/workflows/pull_request.yml` & `scienceio-2.1.1/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.0/.github/workflows/release.yml` & `scienceio-2.1.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.0/.gitignore` & `scienceio-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.0/PUBLISHING.md` & `scienceio-2.1.1/PUBLISHING.md`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.0/Pipfile.lock` & `scienceio-2.1.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.0/README.md` & `scienceio-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.0/examples/analytics.py` & `scienceio-2.1.1/examples/analytics.py`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.0/examples/convert_data_model.py` & `scienceio-2.1.1/examples/convert_data_model.py`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.0/examples/example-analytics-1.ipynb` & `scienceio-2.1.1/examples/example-analytics-1.ipynb`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.0/examples/example-analytics-2.ipynb` & `scienceio-2.1.1/examples/example-analytics-2.ipynb`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.0/examples/example-annotate-onboarding-text.ipynb` & `scienceio-2.1.1/examples/example-annotate-onboarding-text.ipynb`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.0/examples/example-onboarding.ipynb` & `scienceio-2.1.1/examples/example-onboarding.ipynb`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.0/pyproject.toml` & `scienceio-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.0/src/scienceio/scienceio.py` & `scienceio-2.1.1/src/scienceio/scienceio.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,17 +208,14 @@
 def _response_handler(response: requests.Response) -> dict:
     status_code = response.status_code
     payload = response.json()
 
     if 400 <= status_code <= 599:
         error_payload = payload.get("detail", DEFAULT_ERROR_MESSAGE)
 
-        if status_code == HTTPStatus.TOO_MANY_REQUESTS:
-            error_payload = payload.get("error")
-
         error_json_str = json.dumps(error_payload)
 
         raise HTTPError(
             status_code=status_code, message=error_json_str, headers=response.headers
         )
 
     return payload
```

### Comparing `scienceio-2.1.0/tests/__snapshots__/test_scienceio.ambr` & `scienceio-2.1.1/tests/__snapshots__/test_scienceio.ambr`

 * *Files 4% similar despite different names*

```diff
@@ -10,56 +10,68 @@
   '''
 # ---
 # name: test_autogenerated__process[identify_phi][payload]
   dict({
     'annotations': list([
       dict({
         'labels': dict({
+          'category': dict({
+            'label': '[PERSON]',
+          }),
           'phi_type': dict({
             'label': '[PATIENT]',
-            'score': 0.857,
+            'score': 0.998,
           }),
         }),
         'span': dict({
           'end': 12,
           'start': 0,
         }),
         'text': 'Romeo Santos',
       }),
       dict({
         'labels': dict({
+          'category': dict({
+            'label': '[PERSON]',
+          }),
           'phi_type': dict({
             'label': '[DOCTOR]',
-            'score': 0.998,
+            'score': 0.999,
           }),
         }),
         'span': dict({
           'end': 56,
           'start': 42,
         }),
         'text': 'Geoffrey Royce',
       }),
       dict({
         'labels': dict({
+          'category': dict({
+            'label': '[DATE]',
+          }),
           'phi_type': dict({
             'label': '[DATE]',
-            'score': 0.997,
+            'score': 1.0,
           }),
         }),
         'span': dict({
           'end': 77,
           'start': 60,
         }),
         'text': 'December 21, 2020',
       }),
       dict({
         'labels': dict({
+          'category': dict({
+            'label': '[PERSON]',
+          }),
           'phi_type': dict({
             'label': '[PATIENT]',
-            'score': 0.991,
+            'score': 0.999,
           }),
         }),
         'span': dict({
           'end': 89,
           'start': 83,
         }),
         'text': 'Santos',
@@ -80,56 +92,68 @@
   '''
 # ---
 # name: test_autogenerated__process[redact_phi][payload]
   dict({
     'annotations': list([
       dict({
         'labels': dict({
+          'category': dict({
+            'label': '[PERSON]',
+          }),
           'phi_type': dict({
             'label': '[PATIENT]',
-            'score': 0.857,
+            'score': 0.998,
           }),
         }),
         'span': dict({
           'end': 9,
           'start': 0,
         }),
         'text': '[PATIENT]',
       }),
       dict({
         'labels': dict({
+          'category': dict({
+            'label': '[PERSON]',
+          }),
           'phi_type': dict({
             'label': '[DOCTOR]',
-            'score': 0.998,
+            'score': 0.999,
           }),
         }),
         'span': dict({
           'end': 47,
           'start': 39,
         }),
         'text': '[DOCTOR]',
       }),
       dict({
         'labels': dict({
+          'category': dict({
+            'label': '[DATE]',
+          }),
           'phi_type': dict({
             'label': '[DATE]',
-            'score': 0.997,
+            'score': 1.0,
           }),
         }),
         'span': dict({
           'end': 57,
           'start': 51,
         }),
         'text': '[DATE]',
       }),
       dict({
         'labels': dict({
+          'category': dict({
+            'label': '[PERSON]',
+          }),
           'phi_type': dict({
             'label': '[PATIENT]',
-            'score': 0.991,
+            'score': 0.999,
           }),
         }),
         'span': dict({
           'end': 72,
           'start': 63,
         }),
         'text': '[PATIENT]',
@@ -205,56 +229,68 @@
   })
 # ---
 # name: test_autogenerated__submit_and_poll[identify_phi][payload]
   dict({
     'annotations': list([
       dict({
         'labels': dict({
+          'category': dict({
+            'label': '[PERSON]',
+          }),
           'phi_type': dict({
             'label': '[PATIENT]',
-            'score': 0.857,
+            'score': 0.998,
           }),
         }),
         'span': dict({
           'end': 12,
           'start': 0,
         }),
         'text': 'Romeo Santos',
       }),
       dict({
         'labels': dict({
+          'category': dict({
+            'label': '[PERSON]',
+          }),
           'phi_type': dict({
             'label': '[DOCTOR]',
-            'score': 0.998,
+            'score': 0.999,
           }),
         }),
         'span': dict({
           'end': 56,
           'start': 42,
         }),
         'text': 'Geoffrey Royce',
       }),
       dict({
         'labels': dict({
+          'category': dict({
+            'label': '[DATE]',
+          }),
           'phi_type': dict({
             'label': '[DATE]',
-            'score': 0.997,
+            'score': 1.0,
           }),
         }),
         'span': dict({
           'end': 77,
           'start': 60,
         }),
         'text': 'December 21, 2020',
       }),
       dict({
         'labels': dict({
+          'category': dict({
+            'label': '[PERSON]',
+          }),
           'phi_type': dict({
             'label': '[PATIENT]',
-            'score': 0.991,
+            'score': 0.999,
           }),
         }),
         'span': dict({
           'end': 89,
           'start': 83,
         }),
         'text': 'Santos',
@@ -286,56 +322,68 @@
   '''
 # ---
 # name: test_autogenerated__submit_and_poll[redact_phi][payload]
   dict({
     'annotations': list([
       dict({
         'labels': dict({
+          'category': dict({
+            'label': '[PERSON]',
+          }),
           'phi_type': dict({
             'label': '[PATIENT]',
-            'score': 0.857,
+            'score': 0.998,
           }),
         }),
         'span': dict({
           'end': 9,
           'start': 0,
         }),
         'text': '[PATIENT]',
       }),
       dict({
         'labels': dict({
+          'category': dict({
+            'label': '[PERSON]',
+          }),
           'phi_type': dict({
             'label': '[DOCTOR]',
-            'score': 0.998,
+            'score': 0.999,
           }),
         }),
         'span': dict({
           'end': 47,
           'start': 39,
         }),
         'text': '[DOCTOR]',
       }),
       dict({
         'labels': dict({
+          'category': dict({
+            'label': '[DATE]',
+          }),
           'phi_type': dict({
             'label': '[DATE]',
-            'score': 0.997,
+            'score': 1.0,
           }),
         }),
         'span': dict({
           'end': 57,
           'start': 51,
         }),
         'text': '[DATE]',
       }),
       dict({
         'labels': dict({
+          'category': dict({
+            'label': '[PERSON]',
+          }),
           'phi_type': dict({
             'label': '[PATIENT]',
-            'score': 0.991,
+            'score': 0.999,
           }),
         }),
         'span': dict({
           'end': 72,
           'start': 63,
         }),
         'text': '[PATIENT]',
```

### Comparing `scienceio-2.1.0/tests/conftest.py` & `scienceio-2.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.0/tests/test_scienceio.py` & `scienceio-2.1.1/tests/test_scienceio.py`

 * *Files identical despite different names*

### Comparing `scienceio-2.1.0/PKG-INFO` & `scienceio-2.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scienceio
-Version: 2.1.0
+Version: 2.1.1
 Summary: ScienceIO Python SDK
 Author-email: ScienceIO <info@science.io>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Dist: requests >=2.26
```

