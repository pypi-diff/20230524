# Comparing `tmp/HawaData-0.5.2.tar.gz` & `tmp/HawaData-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.5.2.tar", last modified: Tue May 23 08:58:08 2023, max compression
+gzip compressed data, was "HawaData-0.5.3.tar", last modified: Wed May 24 07:07:31 2023, max compression
```

## Comparing `HawaData-0.5.2.tar` & `HawaData-0.5.3.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:58:08.564461 HawaData-0.5.2/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:58:08.559531 HawaData-0.5.2/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2389 2023-05-23 08:58:08.000000 HawaData-0.5.2/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      521 2023-05-23 08:58:08.000000 HawaData-0.5.2/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-23 08:58:08.000000 HawaData-0.5.2/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-05-23 08:58:08.000000 HawaData-0.5.2/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     2389 2023-05-23 08:58:08.564219 HawaData-0.5.2/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.5.2/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:58:08.559975 HawaData-0.5.2/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.5.2/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:58:08.560883 HawaData-0.5.2/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.5.2/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.5.2/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.5.2/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.5.2/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:58:08.561804 HawaData-0.5.2/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.5.2/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     9282 2023-05-23 07:49:48.000000 HawaData-0.5.2/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5323 2023-05-23 06:47:14.000000 HawaData-0.5.2/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2784 2023-05-05 08:28:22.000000 HawaData-0.5.2/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.5.2/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:58:08.562940 HawaData-0.5.2/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.5.2/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.5.2/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.5.2/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.5.2/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      564 2023-05-22 09:15:45.000000 HawaData-0.5.2/hawa/data/school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:58:08.563675 HawaData-0.5.2/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.5.2/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    24132 2023-05-23 08:57:47.000000 HawaData-0.5.2/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.5.2/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-23 08:58:08.564527 HawaData-0.5.2/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.5.2/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:58:08.563914 HawaData-0.5.2/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.5.2/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:07:31.829424 HawaData-0.5.3/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:07:31.819055 HawaData-0.5.3/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2414 2023-05-24 07:07:31.000000 HawaData-0.5.3/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      541 2023-05-24 07:07:31.000000 HawaData-0.5.3/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-24 07:07:31.000000 HawaData-0.5.3/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-05-24 07:07:31.000000 HawaData-0.5.3/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2414 2023-05-24 07:07:31.829112 HawaData-0.5.3/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.5.3/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:07:31.819623 HawaData-0.5.3/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.5.3/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:07:31.821627 HawaData-0.5.3/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.5.3/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.5.3/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.5.3/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.5.3/hawa/base/errors.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.5.3/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:07:31.823679 HawaData-0.5.3/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.5.3/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     9282 2023-05-24 07:01:18.000000 HawaData-0.5.3/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5323 2023-05-23 06:47:14.000000 HawaData-0.5.3/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2784 2023-05-05 08:28:22.000000 HawaData-0.5.3/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.5.3/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:07:31.826379 HawaData-0.5.3/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.5.3/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.5.3/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.5.3/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.5.3/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      564 2023-05-22 09:15:45.000000 HawaData-0.5.3/hawa/data/school.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:07:31.827821 HawaData-0.5.3/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.5.3/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    24276 2023-05-24 07:06:51.000000 HawaData-0.5.3/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.5.3/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-24 07:07:31.829509 HawaData-0.5.3/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.5.3/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:07:31.828424 HawaData-0.5.3/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.5.3/test/test_query.py
```

### Comparing `HawaData-0.5.2/HawaData.egg-info/PKG-INFO` & `HawaData-0.5.3/HawaData.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.5.2
+Version: 0.5.3
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -84,7 +84,8 @@
 - 0.3.7 update pandas to 2+
 - 0.3.8 fix loss data
 - 0.4.0 add case project_id
 - 0.4.1 fix miss grade data
 - 0.5.0 add health api data
 - 0.5.1 add grade param
 - 0.5.2 fix score rank percent
+- 0.5.3 add NoCasesError
```

### Comparing `HawaData-0.5.2/HawaData.egg-info/SOURCES.txt` & `HawaData-0.5.3/HawaData.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 HawaData.egg-info/dependency_links.txt
 HawaData.egg-info/top_level.txt
 hawa/__init__.py
 hawa/config.py
 hawa/base/__init__.py
 hawa/base/db.py
 hawa/base/decos.py
+hawa/base/errors.py
 hawa/base/init.py
 hawa/common/__init__.py
 hawa/common/data.py
 hawa/common/query.py
 hawa/common/utils.py
 hawa/data/__init__.py
 hawa/data/city.py
```

### Comparing `HawaData-0.5.2/PKG-INFO` & `HawaData-0.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.5.2
+Version: 0.5.3
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -84,7 +84,8 @@
 - 0.3.7 update pandas to 2+
 - 0.3.8 fix loss data
 - 0.4.0 add case project_id
 - 0.4.1 fix miss grade data
 - 0.5.0 add health api data
 - 0.5.1 add grade param
 - 0.5.2 fix score rank percent
+- 0.5.3 add NoCasesError
```

### Comparing `HawaData-0.5.2/README.md` & `HawaData-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.2/hawa/base/db.py` & `HawaData-0.5.3/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.2/hawa/base/init.py` & `HawaData-0.5.3/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.2/hawa/common/data.py` & `HawaData-0.5.3/hawa/common/data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.2/hawa/common/query.py` & `HawaData-0.5.3/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.2/hawa/common/utils.py` & `HawaData-0.5.3/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.2/hawa/config.py` & `HawaData-0.5.3/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.2/hawa/data/klass.py` & `HawaData-0.5.3/hawa/data/klass.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.2/hawa/data/school.py` & `HawaData-0.5.3/hawa/data/school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.2/hawa/paper/health.py` & `HawaData-0.5.3/hawa/paper/health.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from dataclasses import dataclass, field
 from typing import Union, Set, Optional
 
 import pandas as pd
 from munch import Munch
 from pingouin import cronbach_alpha
 
+from hawa.base.errors import NoCasesError
 from hawa.common.data import CommonData
 from hawa.config import project
 
 
 @dataclass
 class HealthData(CommonData):
     """健康测评数据，不应直接使用，应向下继承 city/district/school 等"""
@@ -36,14 +37,16 @@
         """如果有年级参数，则筛选年级暑假"""
         super()._to_init_d_cases()
         if self.grade:
             self.cases = self.cases.loc[self.cases['id'] % 100 == self.grade, :]
             self.case_ids = self.cases['id'].tolist()
             self.case_project_ids = Counter(self.cases['project_id'].tolist())
             project.logger.debug(f'cases: {len(self.cases)}')
+        if len(self.cases) == 0:
+            raise NoCasesError(f'grade {self.grade} cases is empty')
 
     def score_rank(self, grade: int):
         """某年级 健康素养水平各等级占比"""
         base = {'优秀': 0, '良好': 0, '中等': 0, '待提高': 0}
         final_scores = self.final_scores[self.final_scores['grade'] == grade]
         raw = dict(final_scores['level'].value_counts())
         data = base | raw
```

### Comparing `HawaData-0.5.2/hawa/paper/mht.py` & `HawaData-0.5.3/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.2/setup.py` & `HawaData-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.2/test/test_query.py` & `HawaData-0.5.3/test/test_query.py`

 * *Files identical despite different names*

