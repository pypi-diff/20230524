# Comparing `tmp/HawaData-0.5.5.tar.gz` & `tmp/HawaData-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.5.5.tar", last modified: Wed May 24 09:02:37 2023, max compression
+gzip compressed data, was "HawaData-0.5.6.tar", last modified: Wed May 24 13:26:41 2023, max compression
```

## Comparing `HawaData-0.5.5.tar` & `HawaData-0.5.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 09:02:37.945219 HawaData-0.5.5/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 09:02:37.934469 HawaData-0.5.5/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2485 2023-05-24 09:02:37.000000 HawaData-0.5.5/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      541 2023-05-24 09:02:37.000000 HawaData-0.5.5/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-24 09:02:37.000000 HawaData-0.5.5/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-05-24 09:02:37.000000 HawaData-0.5.5/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     2485 2023-05-24 09:02:37.944932 HawaData-0.5.5/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.5.5/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 09:02:37.935192 HawaData-0.5.5/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.5.5/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 09:02:37.937672 HawaData-0.5.5/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.5.5/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.5.5/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.5.5/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.5.5/hawa/base/errors.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.5.5/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 09:02:37.939390 HawaData-0.5.5/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.5.5/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     9327 2023-05-24 07:17:27.000000 HawaData-0.5.5/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5323 2023-05-23 06:47:14.000000 HawaData-0.5.5/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2784 2023-05-05 08:28:22.000000 HawaData-0.5.5/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.5.5/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 09:02:37.942517 HawaData-0.5.5/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.5.5/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.5.5/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.5.5/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.5.5/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      564 2023-05-22 09:15:45.000000 HawaData-0.5.5/hawa/data/school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 09:02:37.943667 HawaData-0.5.5/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.5.5/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    24938 2023-05-24 09:00:00.000000 HawaData-0.5.5/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.5.5/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-24 09:02:37.945299 HawaData-0.5.5/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.5.5/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 09:02:37.944256 HawaData-0.5.5/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.5.5/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 13:26:41.887565 HawaData-0.5.6/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 13:26:41.877208 HawaData-0.5.6/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2544 2023-05-24 13:26:41.000000 HawaData-0.5.6/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      541 2023-05-24 13:26:41.000000 HawaData-0.5.6/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-24 13:26:41.000000 HawaData-0.5.6/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-05-24 13:26:41.000000 HawaData-0.5.6/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2544 2023-05-24 13:26:41.887285 HawaData-0.5.6/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.5.6/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 13:26:41.877805 HawaData-0.5.6/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.5.6/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 13:26:41.880754 HawaData-0.5.6/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.5.6/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.5.6/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.5.6/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.5.6/hawa/base/errors.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.5.6/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 13:26:41.882420 HawaData-0.5.6/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.5.6/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     9327 2023-05-24 07:17:27.000000 HawaData-0.5.6/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5323 2023-05-23 06:47:14.000000 HawaData-0.5.6/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2784 2023-05-05 08:28:22.000000 HawaData-0.5.6/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.5.6/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 13:26:41.885020 HawaData-0.5.6/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.5.6/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.5.6/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.5.6/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.5.6/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      564 2023-05-22 09:15:45.000000 HawaData-0.5.6/hawa/data/school.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 13:26:41.886128 HawaData-0.5.6/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.5.6/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    26310 2023-05-24 13:25:10.000000 HawaData-0.5.6/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.5.6/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-24 13:26:41.887639 HawaData-0.5.6/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.5.6/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 13:26:41.886681 HawaData-0.5.6/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.5.6/test/test_query.py
```

### Comparing `HawaData-0.5.5/HawaData.egg-info/PKG-INFO` & `HawaData-0.5.6/HawaData.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.5.5
+Version: 0.5.6
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -87,7 +87,8 @@
 - 0.4.1 fix miss grade data
 - 0.5.0 add health api data
 - 0.5.1 add grade param
 - 0.5.2 fix score rank percent
 - 0.5.3 add NoCasesError
 - 0.5.4 add NoCasesError
 - 0.5.5 add gender compare data to health api
+- 0.5.6 add dim or field gender compare data to health api
```

### Comparing `HawaData-0.5.5/HawaData.egg-info/SOURCES.txt` & `HawaData-0.5.6/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.5/PKG-INFO` & `HawaData-0.5.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.5.5
+Version: 0.5.6
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -87,7 +87,8 @@
 - 0.4.1 fix miss grade data
 - 0.5.0 add health api data
 - 0.5.1 add grade param
 - 0.5.2 fix score rank percent
 - 0.5.3 add NoCasesError
 - 0.5.4 add NoCasesError
 - 0.5.5 add gender compare data to health api
+- 0.5.6 add dim or field gender compare data to health api
```

### Comparing `HawaData-0.5.5/README.md` & `HawaData-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.5/hawa/base/db.py` & `HawaData-0.5.6/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.5/hawa/base/init.py` & `HawaData-0.5.6/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.5/hawa/common/data.py` & `HawaData-0.5.6/hawa/common/data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.5/hawa/common/query.py` & `HawaData-0.5.6/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.5/hawa/common/utils.py` & `HawaData-0.5.6/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.5/hawa/config.py` & `HawaData-0.5.6/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.5/hawa/data/klass.py` & `HawaData-0.5.6/hawa/data/klass.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.5/hawa/data/school.py` & `HawaData-0.5.6/hawa/data/school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.5/hawa/paper/health.py` & `HawaData-0.5.6/hawa/paper/health.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,25 +54,59 @@
         sum_data = sum(data.values())
         if not sum_data:
             raise ValueError(f'grade {grade} score rank is empty')
         percent = {k: round(v * 100 / sum_data, 2) for k, v in data.items()}
         return percent
 
     def gender_compare(self, grade: int):
-        """某年级"""
+        """某年级学生健康素养水平及性别比较图"""
         final_scores = self.__get_grade_final_scores(grade=grade)
         total_score = final_scores.score.mean()
         m_score = final_scores.loc[final_scores.gender == 'M'].score.mean()
         f_score = final_scores.loc[final_scores.gender == 'F'].score.mean()
         return {
             "total": round(total_score, 2),
             "M": round(m_score, 2),
             "F": round(f_score, 2)
         }
 
+    def dim_field_gender_compare(self, grade: int, item_code: str):
+        """某年级六大领域/四大维度测评得分及性别比较图"""
+        final_answers = self.__get_grade_final_answers(grade=grade)
+        answers = final_answers.loc[~final_answers[item_code].isnull(), :]
+        raw_data = {
+            'total': answers,
+            'M': answers.loc[answers.gender == 'M', :],
+            'F': answers.loc[answers.gender == 'F', :]
+        }
+        res = {}
+        for gender_k, gender_v in raw_data.items():
+            res[gender_k] = {}
+            for this_item_code, code_group in gender_v.groupby(item_code):
+                score = round(code_group.score.mean() * 100, 2)
+                res[gender_k][this_item_code] = score
+        codes = answers[item_code].unique().tolist()
+        gender_box = []
+        for gender_k, gender_data in res.items():
+            row_data = {
+                "name": gender_k,
+                "value": []
+            }
+            for c in codes:
+                row_data["value"].append(res[gender_k][c])
+            gender_box.append(row_data)
+
+        return {
+            "category": codes,
+            "values": gender_box,
+        }
+
+    def __get_grade_final_answers(self, grade: int):
+        return self.final_answers[self.final_answers['grade'] == grade]
+
     def __get_grade_final_scores(self, grade: int):
         return self.final_scores[self.final_scores['grade'] == grade]
 
 
 @dataclass
 class HealthReportData(HealthData):
     # 计算数据
```

### Comparing `HawaData-0.5.5/hawa/paper/mht.py` & `HawaData-0.5.6/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.5/setup.py` & `HawaData-0.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.5/test/test_query.py` & `HawaData-0.5.6/test/test_query.py`

 * *Files identical despite different names*

