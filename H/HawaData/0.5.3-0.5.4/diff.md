# Comparing `tmp/HawaData-0.5.3.tar.gz` & `tmp/HawaData-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.5.3.tar", last modified: Wed May 24 07:07:31 2023, max compression
+gzip compressed data, was "HawaData-0.5.4.tar", last modified: Wed May 24 07:17:50 2023, max compression
```

## Comparing `HawaData-0.5.3.tar` & `HawaData-0.5.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:07:31.829424 HawaData-0.5.3/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:07:31.819055 HawaData-0.5.3/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2414 2023-05-24 07:07:31.000000 HawaData-0.5.3/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      541 2023-05-24 07:07:31.000000 HawaData-0.5.3/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-24 07:07:31.000000 HawaData-0.5.3/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-05-24 07:07:31.000000 HawaData-0.5.3/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     2414 2023-05-24 07:07:31.829112 HawaData-0.5.3/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.5.3/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:07:31.819623 HawaData-0.5.3/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.5.3/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:07:31.821627 HawaData-0.5.3/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.5.3/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.5.3/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.5.3/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.5.3/hawa/base/errors.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.5.3/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:07:31.823679 HawaData-0.5.3/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.5.3/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     9282 2023-05-24 07:01:18.000000 HawaData-0.5.3/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5323 2023-05-23 06:47:14.000000 HawaData-0.5.3/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2784 2023-05-05 08:28:22.000000 HawaData-0.5.3/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.5.3/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:07:31.826379 HawaData-0.5.3/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.5.3/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.5.3/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.5.3/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.5.3/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      564 2023-05-22 09:15:45.000000 HawaData-0.5.3/hawa/data/school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:07:31.827821 HawaData-0.5.3/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.5.3/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    24276 2023-05-24 07:06:51.000000 HawaData-0.5.3/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.5.3/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-24 07:07:31.829509 HawaData-0.5.3/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.5.3/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:07:31.828424 HawaData-0.5.3/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.5.3/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:17:50.367324 HawaData-0.5.4/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:17:50.355543 HawaData-0.5.4/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2439 2023-05-24 07:17:50.000000 HawaData-0.5.4/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      541 2023-05-24 07:17:50.000000 HawaData-0.5.4/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-24 07:17:50.000000 HawaData-0.5.4/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-05-24 07:17:50.000000 HawaData-0.5.4/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2439 2023-05-24 07:17:50.366923 HawaData-0.5.4/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.5.4/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:17:50.356102 HawaData-0.5.4/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.5.4/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:17:50.359160 HawaData-0.5.4/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.5.4/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.5.4/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.5.4/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.5.4/hawa/base/errors.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.5.4/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:17:50.360892 HawaData-0.5.4/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.5.4/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     9327 2023-05-24 07:17:27.000000 HawaData-0.5.4/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5323 2023-05-23 06:47:14.000000 HawaData-0.5.4/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2784 2023-05-05 08:28:22.000000 HawaData-0.5.4/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.5.4/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:17:50.363634 HawaData-0.5.4/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.5.4/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.5.4/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.5.4/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.5.4/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      564 2023-05-22 09:15:45.000000 HawaData-0.5.4/hawa/data/school.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:17:50.365531 HawaData-0.5.4/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.5.4/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    24276 2023-05-24 07:06:51.000000 HawaData-0.5.4/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.5.4/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-24 07:17:50.367433 HawaData-0.5.4/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.5.4/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:17:50.366279 HawaData-0.5.4/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.5.4/test/test_query.py
```

### Comparing `HawaData-0.5.3/HawaData.egg-info/PKG-INFO` & `HawaData-0.5.4/HawaData.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.5.3
+Version: 0.5.4
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -85,7 +85,8 @@
 - 0.3.8 fix loss data
 - 0.4.0 add case project_id
 - 0.4.1 fix miss grade data
 - 0.5.0 add health api data
 - 0.5.1 add grade param
 - 0.5.2 fix score rank percent
 - 0.5.3 add NoCasesError
+- 0.5.4 add NoCasesError
```

### Comparing `HawaData-0.5.3/HawaData.egg-info/SOURCES.txt` & `HawaData-0.5.4/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.3/PKG-INFO` & `HawaData-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.5.3
+Version: 0.5.4
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -85,7 +85,8 @@
 - 0.3.8 fix loss data
 - 0.4.0 add case project_id
 - 0.4.1 fix miss grade data
 - 0.5.0 add health api data
 - 0.5.1 add grade param
 - 0.5.2 fix score rank percent
 - 0.5.3 add NoCasesError
+- 0.5.4 add NoCasesError
```

### Comparing `HawaData-0.5.3/README.md` & `HawaData-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.3/hawa/base/db.py` & `HawaData-0.5.4/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.3/hawa/base/init.py` & `HawaData-0.5.4/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.3/hawa/common/data.py` & `HawaData-0.5.4/hawa/common/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Optional, ClassVar, Any, Set
 
 import pandas as pd
 import pendulum
 from munch import Munch
 
 from hawa.base.db import DbUtil, RedisUtil
+from hawa.base.errors import NoCasesError
 from hawa.common.query import DataQuery
 from hawa.common.utils import GradeData, CaseData, Measurement
 from hawa.config import project
 
 
 class MetaCommomData(type):
     def __new__(cls, name, bases, attrs):
@@ -126,15 +127,15 @@
         self.cases = self.query.query_cases(
             school_ids=self.school_ids,
             paper_ids=paper_ids,
             valid_to_start=start_stamp_str,
             valid_to_end=end_stamp_str,
         )
         if self.cases.empty:
-            raise Exception(f'no cases:{self.meta_unit} {self.school_ids}')
+            raise NoCasesError(f'no cases:{self.meta_unit} {self.school_ids}')
         self.case_ids = self.cases['id'].tolist()
         self.case_project_ids = Counter(self.cases['project_id'].tolist())
         project.logger.debug(f'cases: {len(self.cases)}')
 
     def _to_init_e_answers(self):
         self.answers = self.query.query_answers(case_ids=self.case_ids)
         project.logger.debug(f'answers: {len(self.answers)}')
```

### Comparing `HawaData-0.5.3/hawa/common/query.py` & `HawaData-0.5.4/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.3/hawa/common/utils.py` & `HawaData-0.5.4/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.3/hawa/config.py` & `HawaData-0.5.4/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.3/hawa/data/klass.py` & `HawaData-0.5.4/hawa/data/klass.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.3/hawa/data/school.py` & `HawaData-0.5.4/hawa/data/school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.3/hawa/paper/health.py` & `HawaData-0.5.4/hawa/paper/health.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.3/hawa/paper/mht.py` & `HawaData-0.5.4/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.3/setup.py` & `HawaData-0.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.3/test/test_query.py` & `HawaData-0.5.4/test/test_query.py`

 * *Files identical despite different names*

