# Comparing `tmp/HawaData-0.5.4.tar.gz` & `tmp/HawaData-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.5.4.tar", last modified: Wed May 24 07:17:50 2023, max compression
+gzip compressed data, was "HawaData-0.5.5.tar", last modified: Wed May 24 09:02:37 2023, max compression
```

## Comparing `HawaData-0.5.4.tar` & `HawaData-0.5.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:17:50.367324 HawaData-0.5.4/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:17:50.355543 HawaData-0.5.4/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2439 2023-05-24 07:17:50.000000 HawaData-0.5.4/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      541 2023-05-24 07:17:50.000000 HawaData-0.5.4/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-24 07:17:50.000000 HawaData-0.5.4/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-05-24 07:17:50.000000 HawaData-0.5.4/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     2439 2023-05-24 07:17:50.366923 HawaData-0.5.4/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.5.4/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:17:50.356102 HawaData-0.5.4/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.5.4/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:17:50.359160 HawaData-0.5.4/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.5.4/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.5.4/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.5.4/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.5.4/hawa/base/errors.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.5.4/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:17:50.360892 HawaData-0.5.4/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.5.4/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     9327 2023-05-24 07:17:27.000000 HawaData-0.5.4/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5323 2023-05-23 06:47:14.000000 HawaData-0.5.4/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2784 2023-05-05 08:28:22.000000 HawaData-0.5.4/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.5.4/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:17:50.363634 HawaData-0.5.4/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.5.4/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.5.4/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.5.4/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.5.4/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      564 2023-05-22 09:15:45.000000 HawaData-0.5.4/hawa/data/school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:17:50.365531 HawaData-0.5.4/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.5.4/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    24276 2023-05-24 07:06:51.000000 HawaData-0.5.4/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.5.4/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-24 07:17:50.367433 HawaData-0.5.4/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.5.4/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 07:17:50.366279 HawaData-0.5.4/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.5.4/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 09:02:37.945219 HawaData-0.5.5/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 09:02:37.934469 HawaData-0.5.5/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2485 2023-05-24 09:02:37.000000 HawaData-0.5.5/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      541 2023-05-24 09:02:37.000000 HawaData-0.5.5/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-24 09:02:37.000000 HawaData-0.5.5/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-05-24 09:02:37.000000 HawaData-0.5.5/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2485 2023-05-24 09:02:37.944932 HawaData-0.5.5/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.5.5/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 09:02:37.935192 HawaData-0.5.5/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.5.5/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 09:02:37.937672 HawaData-0.5.5/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.5.5/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.5.5/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.5.5/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.5.5/hawa/base/errors.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.5.5/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 09:02:37.939390 HawaData-0.5.5/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.5.5/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     9327 2023-05-24 07:17:27.000000 HawaData-0.5.5/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5323 2023-05-23 06:47:14.000000 HawaData-0.5.5/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2784 2023-05-05 08:28:22.000000 HawaData-0.5.5/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.5.5/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 09:02:37.942517 HawaData-0.5.5/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.5.5/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.5.5/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.5.5/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.5.5/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      564 2023-05-22 09:15:45.000000 HawaData-0.5.5/hawa/data/school.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 09:02:37.943667 HawaData-0.5.5/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.5.5/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    24938 2023-05-24 09:00:00.000000 HawaData-0.5.5/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.5.5/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-24 09:02:37.945299 HawaData-0.5.5/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.5.5/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 09:02:37.944256 HawaData-0.5.5/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.5.5/test/test_query.py
```

### Comparing `HawaData-0.5.4/HawaData.egg-info/PKG-INFO` & `HawaData-0.5.5/HawaData.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.5.4
+Version: 0.5.5
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -86,7 +86,8 @@
 - 0.4.0 add case project_id
 - 0.4.1 fix miss grade data
 - 0.5.0 add health api data
 - 0.5.1 add grade param
 - 0.5.2 fix score rank percent
 - 0.5.3 add NoCasesError
 - 0.5.4 add NoCasesError
+- 0.5.5 add gender compare data to health api
```

### Comparing `HawaData-0.5.4/HawaData.egg-info/SOURCES.txt` & `HawaData-0.5.5/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.4/PKG-INFO` & `HawaData-0.5.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.5.4
+Version: 0.5.5
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -86,7 +86,8 @@
 - 0.4.0 add case project_id
 - 0.4.1 fix miss grade data
 - 0.5.0 add health api data
 - 0.5.1 add grade param
 - 0.5.2 fix score rank percent
 - 0.5.3 add NoCasesError
 - 0.5.4 add NoCasesError
+- 0.5.5 add gender compare data to health api
```

### Comparing `HawaData-0.5.4/README.md` & `HawaData-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.4/hawa/base/db.py` & `HawaData-0.5.5/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.4/hawa/base/init.py` & `HawaData-0.5.5/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.4/hawa/common/data.py` & `HawaData-0.5.5/hawa/common/data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.4/hawa/common/query.py` & `HawaData-0.5.5/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.4/hawa/common/utils.py` & `HawaData-0.5.5/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.4/hawa/config.py` & `HawaData-0.5.5/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.4/hawa/data/klass.py` & `HawaData-0.5.5/hawa/data/klass.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.4/hawa/data/school.py` & `HawaData-0.5.5/hawa/data/school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.4/hawa/paper/health.py` & `HawaData-0.5.5/hawa/paper/health.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
             return text.replace('还', '')
 
 
 @dataclass
 class HealthApiData(HealthData):
     """为 yingde api 项目提供基类"""
     grade: Optional[int] = None  # 必填
+    grade_final_scores: pd.DataFrame = field(default_factory=pd.DataFrame)
 
     def _to_init_d_cases(self):
         """如果有年级参数，则筛选年级暑假"""
         super()._to_init_d_cases()
         if self.grade:
             self.cases = self.cases.loc[self.cases['id'] % 100 == self.grade, :]
             self.case_ids = self.cases['id'].tolist()
@@ -43,23 +44,38 @@
             project.logger.debug(f'cases: {len(self.cases)}')
         if len(self.cases) == 0:
             raise NoCasesError(f'grade {self.grade} cases is empty')
 
     def score_rank(self, grade: int):
         """某年级 健康素养水平各等级占比"""
         base = {'优秀': 0, '良好': 0, '中等': 0, '待提高': 0}
-        final_scores = self.final_scores[self.final_scores['grade'] == grade]
-        raw = dict(final_scores['level'].value_counts())
+        final_scores = self.__get_grade_final_scores(grade=grade)
+        raw = final_scores.level.value_counts().to_dict()
         data = base | raw
         sum_data = sum(data.values())
         if not sum_data:
             raise ValueError(f'grade {grade} score rank is empty')
         percent = {k: round(v * 100 / sum_data, 2) for k, v in data.items()}
         return percent
 
+    def gender_compare(self, grade: int):
+        """某年级"""
+        final_scores = self.__get_grade_final_scores(grade=grade)
+        total_score = final_scores.score.mean()
+        m_score = final_scores.loc[final_scores.gender == 'M'].score.mean()
+        f_score = final_scores.loc[final_scores.gender == 'F'].score.mean()
+        return {
+            "total": round(total_score, 2),
+            "M": round(m_score, 2),
+            "F": round(f_score, 2)
+        }
+
+    def __get_grade_final_scores(self, grade: int):
+        return self.final_scores[self.final_scores['grade'] == grade]
+
 
 @dataclass
 class HealthReportData(HealthData):
     # 计算数据
     code_scores: pd.DataFrame = field(default_factory=pd.DataFrame)
     summary_scores: dict = field(default_factory=dict)
     grade_good_bad = None  # 优势 优先关注点
```

### Comparing `HawaData-0.5.4/hawa/paper/mht.py` & `HawaData-0.5.5/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.4/setup.py` & `HawaData-0.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.4/test/test_query.py` & `HawaData-0.5.5/test/test_query.py`

 * *Files identical despite different names*

