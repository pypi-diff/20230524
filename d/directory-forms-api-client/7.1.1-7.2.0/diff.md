# Comparing `tmp/directory_forms_api_client-7.1.1-py3-none-any.whl.zip` & `tmp/directory_forms_api_client-7.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8287 bytes, number of entries: 10
--rw-r--r--  2.0 unx       95 b- defN 23-Apr-21 10:18 directory_forms_api_client/__init__.py
--rw-r--r--  2.0 unx     3457 b- defN 23-Apr-21 10:18 directory_forms_api_client/actions.py
--rw-r--r--  2.0 unx     1134 b- defN 23-Apr-21 10:18 directory_forms_api_client/client.py
--rw-r--r--  2.0 unx     1695 b- defN 23-Apr-21 10:18 directory_forms_api_client/forms.py
--rw-r--r--  2.0 unx     1828 b- defN 23-Apr-21 10:18 directory_forms_api_client/helpers.py
--rw-r--r--  2.0 unx     1091 b- defN 23-Apr-21 10:19 directory_forms_api_client-7.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     9864 b- defN 23-Apr-21 10:19 directory_forms_api_client-7.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 10:19 directory_forms_api_client-7.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       27 b- defN 23-Apr-21 10:19 directory_forms_api_client-7.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      947 b- defN 23-Apr-21 10:19 directory_forms_api_client-7.1.1.dist-info/RECORD
-10 files, 20230 bytes uncompressed, 6631 bytes compressed:  67.2%
+Zip file size: 8288 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       95 b- defN 23-May-24 08:04 directory_forms_api_client/__init__.py
+-rw-r--r--  2.0 unx     3457 b- defN 23-May-24 08:04 directory_forms_api_client/actions.py
+-rw-r--r--  2.0 unx     1134 b- defN 23-May-24 08:04 directory_forms_api_client/client.py
+-rw-r--r--  2.0 unx     1695 b- defN 23-May-24 08:04 directory_forms_api_client/forms.py
+-rw-r--r--  2.0 unx     1828 b- defN 23-May-24 08:04 directory_forms_api_client/helpers.py
+-rw-r--r--  2.0 unx     1091 b- defN 23-May-24 08:04 directory_forms_api_client-7.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9885 b- defN 23-May-24 08:04 directory_forms_api_client-7.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-24 08:04 directory_forms_api_client-7.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       27 b- defN 23-May-24 08:04 directory_forms_api_client-7.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      947 b- defN 23-May-24 08:04 directory_forms_api_client-7.2.0.dist-info/RECORD
+10 files, 20251 bytes uncompressed, 6632 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: directory_forms_api_client/forms.py
 Comment: 
 
 Filename: directory_forms_api_client/helpers.py
 Comment: 
 
-Filename: directory_forms_api_client-7.1.1.dist-info/LICENSE
+Filename: directory_forms_api_client-7.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: directory_forms_api_client-7.1.1.dist-info/METADATA
+Filename: directory_forms_api_client-7.2.0.dist-info/METADATA
 Comment: 
 
-Filename: directory_forms_api_client-7.1.1.dist-info/WHEEL
+Filename: directory_forms_api_client-7.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: directory_forms_api_client-7.1.1.dist-info/top_level.txt
+Filename: directory_forms_api_client-7.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: directory_forms_api_client-7.1.1.dist-info/RECORD
+Filename: directory_forms_api_client-7.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `directory_forms_api_client-7.1.1.dist-info/LICENSE` & `directory_forms_api_client-7.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `directory_forms_api_client-7.1.1.dist-info/METADATA` & `directory_forms_api_client-7.2.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 Metadata-Version: 2.1
 Name: directory-forms-api-client
-Version: 7.1.1
+Version: 7.2.0
 Summary: Python API client for Directory forms .
 Home-page: https://github.com/uktrade/directory-forms-api-client
 Author: Department for International Trade
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Requires-Dist: directory-client-core (<8.0.0,>=6.1.0)
 Provides-Extra: test
-Requires-Dist: django (<4.0.0,>=2.2.10) ; extra == 'test'
+Requires-Dist: django (<=4.2,>=2.2.10) ; extra == 'test'
 Requires-Dist: flake8 (==3.8.3) ; extra == 'test'
 Requires-Dist: pytest-codecov ; extra == 'test'
 Requires-Dist: pytest-cov ; extra == 'test'
 Requires-Dist: GitPython ; extra == 'test'
 Requires-Dist: pytest-django (==3.10.0) ; extra == 'test'
 Requires-Dist: pytest (==6.1.0) ; extra == 'test'
 Requires-Dist: requests (<3.0.0,>=2.22.0) ; extra == 'test'
 Requires-Dist: requests-mock (==1.8.0) ; extra == 'test'
 Requires-Dist: setuptools (<50.0.0,>=45.2.0) ; extra == 'test'
-Requires-Dist: twine (<4.0.0,>=3.1.1) ; extra == 'test'
+Requires-Dist: twine ; extra == 'test'
 Requires-Dist: wheel (<1.0.0,>=0.34.2) ; extra == 'test'
 
 # directory-forms-api-client
 
 [![code-climate-image]][code-climate]
 [![circle-ci-image]][circle-ci]
 [![codecov-image]][codecov]
```

