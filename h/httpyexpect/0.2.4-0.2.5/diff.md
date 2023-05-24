# Comparing `tmp/httpyexpect-0.2.4.tar.gz` & `tmp/httpyexpect-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpyexpect-0.2.4.tar", last modified: Thu Nov 17 08:24:02 2022, max compression
+gzip compressed data, was "httpyexpect-0.2.5.tar", last modified: Wed May 24 07:46:44 2023, max compression
```

## Comparing `httpyexpect-0.2.4.tar` & `httpyexpect-0.2.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:24:02.381610 httpyexpect-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (121)    11428 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3781 2022-11-17 08:24:02.381610 httpyexpect-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3107 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:24:02.377611 httpyexpect-0.2.4/httpyexpect/
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/httpyexpect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      982 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/httpyexpect/base_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:24:02.377611 httpyexpect-0.2.4/httpyexpect/client/
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/httpyexpect/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/httpyexpect/client/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     3433 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/httpyexpect/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     9269 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/httpyexpect/client/mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)     4302 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/httpyexpect/client/translator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2207 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/httpyexpect/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:24:02.377611 httpyexpect-0.2.4/httpyexpect/server/
--rw-r--r--   0 runner    (1001) docker     (121)      888 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/httpyexpect/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5832 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/httpyexpect/server/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:24:02.377611 httpyexpect-0.2.4/httpyexpect/server/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/httpyexpect/server/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/httpyexpect/server/handlers/fastapi_.py
--rw-r--r--   0 runner    (1001) docker     (121)     1949 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/httpyexpect/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:24:02.377611 httpyexpect-0.2.4/httpyexpect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3781 2022-11-17 08:24:02.000000 httpyexpect-0.2.4/httpyexpect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-11-17 08:24:02.000000 httpyexpect-0.2.4/httpyexpect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 08:24:02.000000 httpyexpect-0.2.4/httpyexpect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 08:24:02.000000 httpyexpect-0.2.4/httpyexpect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-11-17 08:24:02.000000 httpyexpect-0.2.4/httpyexpect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-17 08:24:02.000000 httpyexpect-0.2.4/httpyexpect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1014 2022-11-17 08:24:02.381610 httpyexpect-0.2.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      841 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:24:02.377611 httpyexpect-0.2.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:24:02.377611 httpyexpect-0.2.4/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/tests/fixtures/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:24:02.377611 httpyexpect-0.2.4/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:24:02.381610 httpyexpect-0.2.4/tests/integration/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)      720 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/tests/integration/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/tests/integration/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2798 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2006 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/tests/integration/test_fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:24:02.381610 httpyexpect-0.2.4/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 08:24:02.381610 httpyexpect-0.2.4/tests/unit/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)      783 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/tests/unit/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/tests/unit/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8358 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/tests/unit/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/tests/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     5444 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/tests/unit/test_server_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5981 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/tests/unit/test_translator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2314 2022-11-17 08:23:47.000000 httpyexpect-0.2.4/tests/unit/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:46:44.363299 httpyexpect-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-24 07:46:44.363299 httpyexpect-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:46:44.359299 httpyexpect-0.2.5/httpyexpect/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/base_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:46:44.363299 httpyexpect-0.2.5/httpyexpect/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/client/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/client/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/client/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:46:44.363299 httpyexpect-0.2.5/httpyexpect/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/server/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:46:44.363299 httpyexpect-0.2.5/httpyexpect/server/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/server/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/server/handlers/fastapi_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:46:44.359299 httpyexpect-0.2.5/httpyexpect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-24 07:46:44.000000 httpyexpect-0.2.5/httpyexpect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-24 07:46:44.000000 httpyexpect-0.2.5/httpyexpect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 07:46:44.000000 httpyexpect-0.2.5/httpyexpect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 07:46:44.000000 httpyexpect-0.2.5/httpyexpect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-24 07:46:44.000000 httpyexpect-0.2.5/httpyexpect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 07:46:44.000000 httpyexpect-0.2.5/httpyexpect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-24 07:46:44.367299 httpyexpect-0.2.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:46:44.355299 httpyexpect-0.2.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:46:44.363299 httpyexpect-0.2.5/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/fixtures/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:46:44.363299 httpyexpect-0.2.5/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:46:44.363299 httpyexpect-0.2.5/tests/integration/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/integration/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/integration/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/integration/test_fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:46:44.363299 httpyexpect-0.2.5/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:46:44.363299 httpyexpect-0.2.5/tests/unit/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/unit/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/unit/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/unit/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/unit/test_server_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/unit/test_translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/unit/test_validation.py
```

### Comparing `httpyexpect-0.2.4/LICENSE` & `httpyexpect-0.2.5/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+   Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
    for the German Human Genome-Phenome Archive (GHGA)
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `httpyexpect-0.2.4/PKG-INFO` & `httpyexpect-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpyexpect
-Version: 0.2.4
+Version: 0.2.5
 Summary: An opinionated way to translate server side HTTP errors to the client side.
 Home-page: https://github.com/ghga-de/httpyexpect
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `httpyexpect-0.2.4/README.md` & `httpyexpect-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.4/httpyexpect/__init__.py` & `httpyexpect-0.2.5/httpyexpect/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -11,8 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """An opinionated way to translate server side HTTP errors to the client side."""
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
```

### Comparing `httpyexpect-0.2.4/httpyexpect/base_exception.py` & `httpyexpect-0.2.5/httpyexpect/base_exception.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `httpyexpect-0.2.4/httpyexpect/client/__init__.py` & `httpyexpect-0.2.5/httpyexpect/client/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `httpyexpect-0.2.4/httpyexpect/client/custom_types.py` & `httpyexpect-0.2.5/httpyexpect/client/custom_types.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `httpyexpect-0.2.4/httpyexpect/client/exceptions.py` & `httpyexpect-0.2.5/httpyexpect/client/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `httpyexpect-0.2.4/httpyexpect/client/mapping.py` & `httpyexpect-0.2.5/httpyexpect/client/mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `httpyexpect-0.2.4/httpyexpect/client/translator.py` & `httpyexpect-0.2.5/httpyexpect/client/translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `httpyexpect-0.2.4/httpyexpect/models.py` & `httpyexpect-0.2.5/httpyexpect/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `httpyexpect-0.2.4/httpyexpect/server/__init__.py` & `httpyexpect-0.2.5/tests/integration/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,16 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-#
-
-"""A sub-package for creating and managing HTTP errors with a specific schema on the
-server side.
-"""
 
-# shortcuts:
-from httpyexpect.server.exceptions import (  # noqa: F401
-    HttpCustomExceptionBase,
-    HttpException,
-)
+"""Package containing integration tests"""
```

### Comparing `httpyexpect-0.2.4/httpyexpect/server/exceptions.py` & `httpyexpect-0.2.5/httpyexpect/server/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,15 +13,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Exception Base models used across all servers."""
 
 from abc import ABC
-from typing import Literal
+
+try:  # workaround for https://github.com/pydantic/pydantic/issues/5821
+    from typing_extensions import Literal
+except ImportError:
+    from typing import Literal  # type: ignore
 
 import pydantic
 
 from httpyexpect.base_exception import HttpyExpectError
 from httpyexpect.models import HttpExceptionBody
 from httpyexpect.validation import ValidationError, assert_error_code
```

### Comparing `httpyexpect-0.2.4/httpyexpect/server/handlers/__init__.py` & `httpyexpect-0.2.5/tests/unit/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-#
 
-"""Logic for handling httpyexpect exceptions with different backend frameworks.
-"""
+"""Package containing unit tests"""
```

### Comparing `httpyexpect-0.2.4/httpyexpect/server/handlers/fastapi_.py` & `httpyexpect-0.2.5/httpyexpect/server/handlers/fastapi_.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `httpyexpect-0.2.4/httpyexpect/validation.py` & `httpyexpect-0.2.5/httpyexpect/validation.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `httpyexpect-0.2.4/httpyexpect.egg-info/PKG-INFO` & `httpyexpect-0.2.5/httpyexpect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpyexpect
-Version: 0.2.4
+Version: 0.2.5
 Summary: An opinionated way to translate server side HTTP errors to the client side.
 Home-page: https://github.com/ghga-de/httpyexpect
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `httpyexpect-0.2.4/httpyexpect.egg-info/SOURCES.txt` & `httpyexpect-0.2.5/httpyexpect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.4/setup.py` & `httpyexpect-0.2.5/tests/fixtures/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,16 @@
-#!/usr/bin/env python3
-
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Setup script for pip. This setup configs are specified in the `setup.cfg` file"""
-
-import setuptools
-
-if __name__ == "__main__":
-    setuptools.setup()
+"""Fixtures that are used in both integration and unit tests"""
```

### Comparing `httpyexpect-0.2.4/tests/fixtures/__init__.py` & `httpyexpect-0.2.5/tests/integration/fixtures/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Fixtures that are used in both integration and unit tests"""
+"""Fixtures that exclusively used in integration tests"""
```

### Comparing `httpyexpect-0.2.4/tests/fixtures/utils.py` & `httpyexpect-0.2.5/tests/unit/fixtures/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Utils for Fixture handling"""
+"""Fixtures that exclusively used in unit tests"""
 
 from pathlib import Path
 
 BASE_DIR = Path(__file__).parent.resolve()
```

### Comparing `httpyexpect-0.2.4/tests/integration/__init__.py` & `httpyexpect-0.2.5/tests/fixtures/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Package containing integration tests"""
+"""Utils for Fixture handling"""
+
+from pathlib import Path
+
+BASE_DIR = Path(__file__).parent.resolve()
```

### Comparing `httpyexpect-0.2.4/tests/integration/fixtures/utils.py` & `httpyexpect-0.2.5/tests/integration/fixtures/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `httpyexpect-0.2.4/tests/integration/test_client.py` & `httpyexpect-0.2.5/tests/integration/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `httpyexpect-0.2.4/tests/integration/test_fastapi.py` & `httpyexpect-0.2.5/tests/integration/test_fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `httpyexpect-0.2.4/tests/unit/__init__.py` & `httpyexpect-0.2.5/tests/unit/fixtures/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Package containing unit tests"""
+"""Utils for Fixture handling"""
+
+from pathlib import Path
+
+BASE_DIR = Path(__file__).parent.resolve()
```

### Comparing `httpyexpect-0.2.4/tests/unit/fixtures/utils.py` & `httpyexpect-0.2.5/httpyexpect/server/handlers/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+#
 
-"""Utils for Fixture handling"""
-
-from pathlib import Path
-
-BASE_DIR = Path(__file__).parent.resolve()
+"""Logic for handling httpyexpect exceptions with different backend frameworks.
+"""
```

### Comparing `httpyexpect-0.2.4/tests/unit/test_mapping.py` & `httpyexpect-0.2.5/tests/unit/test_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `httpyexpect-0.2.4/tests/unit/test_models.py` & `httpyexpect-0.2.5/tests/unit/test_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `httpyexpect-0.2.4/tests/unit/test_server_exceptions.py` & `httpyexpect-0.2.5/tests/unit/test_server_exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `httpyexpect-0.2.4/tests/unit/test_translator.py` & `httpyexpect-0.2.5/tests/unit/test_translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `httpyexpect-0.2.4/tests/unit/test_validation.py` & `httpyexpect-0.2.5/tests/unit/test_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2022 Universität Tübingen, DKFZ and EMBL
+# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

