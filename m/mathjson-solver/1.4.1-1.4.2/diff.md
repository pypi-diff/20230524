# Comparing `tmp/mathjson-solver-1.4.1.tar.gz` & `tmp/mathjson-solver-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathjson-solver-1.4.1.tar", last modified: Tue Apr  4 14:15:01 2023, max compression
+gzip compressed data, was "mathjson-solver-1.4.2.tar", last modified: Mon May 22 07:19:12 2023, max compression
```

## Comparing `mathjson-solver-1.4.1.tar` & `mathjson-solver-1.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-04-04 14:15:01.343377 mathjson-solver-1.4.1/
--rw-rw-r--   0 martins   (1000) martins   (1000)     1071 2022-05-02 08:10:45.000000 mathjson-solver-1.4.1/LICENSE
--rw-rw-r--   0 martins   (1000) martins   (1000)     7039 2023-04-04 14:15:01.343377 mathjson-solver-1.4.1/PKG-INFO
--rw-rw-r--   0 martins   (1000) martins   (1000)     6510 2023-04-04 13:14:44.000000 mathjson-solver-1.4.1/README.md
--rw-rw-r--   0 martins   (1000) martins   (1000)       85 2022-05-02 14:01:31.000000 mathjson-solver-1.4.1/pyproject.toml
--rw-rw-r--   0 martins   (1000) martins   (1000)      654 2023-04-04 14:15:01.343377 mathjson-solver-1.4.1/setup.cfg
--rw-rw-r--   0 martins   (1000) martins   (1000)      829 2023-04-04 14:13:49.000000 mathjson-solver-1.4.1/setup.py
-drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-04-04 14:15:01.343377 mathjson-solver-1.4.1/src/
-drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-04-04 14:15:01.343377 mathjson-solver-1.4.1/src/mathjson_solver/
--rw-rw-r--   0 martins   (1000) martins   (1000)      102 2022-05-23 07:31:11.000000 mathjson-solver-1.4.1/src/mathjson_solver/__init__.py
--rw-rw-r--   0 martins   (1000) martins   (1000)     6215 2023-04-04 14:13:22.000000 mathjson-solver-1.4.1/src/mathjson_solver/__main__.py
-drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-04-04 14:15:01.343377 mathjson-solver-1.4.1/src/mathjson_solver.egg-info/
--rw-rw-r--   0 martins   (1000) martins   (1000)     7039 2023-04-04 14:15:01.000000 mathjson-solver-1.4.1/src/mathjson_solver.egg-info/PKG-INFO
--rw-rw-r--   0 martins   (1000) martins   (1000)      313 2023-04-04 14:15:01.000000 mathjson-solver-1.4.1/src/mathjson_solver.egg-info/SOURCES.txt
--rw-rw-r--   0 martins   (1000) martins   (1000)        1 2023-04-04 14:15:01.000000 mathjson-solver-1.4.1/src/mathjson_solver.egg-info/dependency_links.txt
--rw-rw-r--   0 martins   (1000) martins   (1000)       16 2023-04-04 14:15:01.000000 mathjson-solver-1.4.1/src/mathjson_solver.egg-info/top_level.txt
-drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-04-04 14:15:01.343377 mathjson-solver-1.4.1/tests/
--rw-rw-r--   0 martins   (1000) martins   (1000)     4317 2023-04-04 14:12:39.000000 mathjson-solver-1.4.1/tests/test_with_pytest.py
+drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-05-22 07:19:12.752879 mathjson-solver-1.4.2/
+-rw-rw-r--   0 martins   (1000) martins   (1000)     1071 2022-05-02 08:10:45.000000 mathjson-solver-1.4.2/LICENSE
+-rw-rw-r--   0 martins   (1000) martins   (1000)     7111 2023-05-22 07:19:12.752879 mathjson-solver-1.4.2/PKG-INFO
+-rw-rw-r--   0 martins   (1000) martins   (1000)     6582 2023-05-22 07:13:26.000000 mathjson-solver-1.4.2/README.md
+-rw-rw-r--   0 martins   (1000) martins   (1000)       85 2022-05-02 14:01:31.000000 mathjson-solver-1.4.2/pyproject.toml
+-rw-rw-r--   0 martins   (1000) martins   (1000)      654 2023-05-22 07:19:12.752879 mathjson-solver-1.4.2/setup.cfg
+-rw-rw-r--   0 martins   (1000) martins   (1000)      829 2023-05-17 13:21:52.000000 mathjson-solver-1.4.2/setup.py
+drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-05-22 07:19:12.752879 mathjson-solver-1.4.2/src/
+drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-05-22 07:19:12.752879 mathjson-solver-1.4.2/src/mathjson_solver/
+-rw-rw-r--   0 martins   (1000) martins   (1000)      102 2022-05-23 07:31:11.000000 mathjson-solver-1.4.2/src/mathjson_solver/__init__.py
+-rw-rw-r--   0 martins   (1000) martins   (1000)     6402 2023-05-22 07:02:10.000000 mathjson-solver-1.4.2/src/mathjson_solver/__main__.py
+drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-05-22 07:19:12.752879 mathjson-solver-1.4.2/src/mathjson_solver.egg-info/
+-rw-rw-r--   0 martins   (1000) martins   (1000)     7111 2023-05-22 07:19:12.000000 mathjson-solver-1.4.2/src/mathjson_solver.egg-info/PKG-INFO
+-rw-rw-r--   0 martins   (1000) martins   (1000)      313 2023-05-22 07:19:12.000000 mathjson-solver-1.4.2/src/mathjson_solver.egg-info/SOURCES.txt
+-rw-rw-r--   0 martins   (1000) martins   (1000)        1 2023-05-22 07:19:12.000000 mathjson-solver-1.4.2/src/mathjson_solver.egg-info/dependency_links.txt
+-rw-rw-r--   0 martins   (1000) martins   (1000)       16 2023-05-22 07:19:12.000000 mathjson-solver-1.4.2/src/mathjson_solver.egg-info/top_level.txt
+drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-05-22 07:19:12.752879 mathjson-solver-1.4.2/tests/
+-rw-rw-r--   0 martins   (1000) martins   (1000)     4621 2023-05-22 07:05:01.000000 mathjson-solver-1.4.2/tests/test_with_pytest.py
```

### Comparing `mathjson-solver-1.4.1/LICENSE` & `mathjson-solver-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mathjson-solver-1.4.1/PKG-INFO` & `mathjson-solver-1.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathjson-solver
-Version: 1.4.1
+Version: 1.4.2
 Summary: Utilities for MathJSON evaluation
 Home-page: https://github.com/LongenesisLtd/mathjson-solver
 Author: Martins Mednis
 Author-email: mrt@mednis.info
 Project-URL: Bug Tracker, https://github.com/LongenesisLtd/mathjson-solver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,14 +18,18 @@
 [![Gitter](https://badges.gitter.im/mathjson-solver/community.svg)](https://gitter.im/mathjson-solver/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 
 _MathJSON Solver_ is a Python module to numerically evaluate MathJSON expressions. It was created by [Longenesis](https://longenesis.com/team) to add numerical evaluation capability of user generated mathematical expressions in Longenesis digital health products and later released as open source project. Its development was inspired by [CortexJS](https://cortexjs.io/compute-engine/) Compute Engine.
 
 Please ask questions and share feedback in our Gitter chat [https://gitter.im/mathjson-solver/community](https://gitter.im/mathjson-solver/community).
 
 ## What's new
+
+### 1.4.2
+Added `Str` construct. It tries to convert value to string.
+
 ### 1.4.0
 We changed the behavior of `Average` to be more forgiving. In version 1.4.0 `Average` accepts arrays like `[2, 4 ,"6"]` and internally converts numeric strings to floats.
 Also, it skips values that cannot be converted to numeric. Internally `Average` will convert array `[2, "three", 4 ,"6"]` to `[2.0, 4.0 ,6.0]`. When given an empty array, `Average` now returns `None` instead of throwing an error.
 
 ## How to use
 ```python
 from mathjson_solver import create_solver
```

### Comparing `mathjson-solver-1.4.1/README.md` & `mathjson-solver-1.4.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 [![Gitter](https://badges.gitter.im/mathjson-solver/community.svg)](https://gitter.im/mathjson-solver/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 
 _MathJSON Solver_ is a Python module to numerically evaluate MathJSON expressions. It was created by [Longenesis](https://longenesis.com/team) to add numerical evaluation capability of user generated mathematical expressions in Longenesis digital health products and later released as open source project. Its development was inspired by [CortexJS](https://cortexjs.io/compute-engine/) Compute Engine.
 
 Please ask questions and share feedback in our Gitter chat [https://gitter.im/mathjson-solver/community](https://gitter.im/mathjson-solver/community).
 
 ## What's new
+
+### 1.4.2
+Added `Str` construct. It tries to convert value to string.
+
 ### 1.4.0
 We changed the behavior of `Average` to be more forgiving. In version 1.4.0 `Average` accepts arrays like `[2, 4 ,"6"]` and internally converts numeric strings to floats.
 Also, it skips values that cannot be converted to numeric. Internally `Average` will convert array `[2, "three", 4 ,"6"]` to `[2.0, 4.0 ,6.0]`. When given an empty array, `Average` now returns `None` instead of throwing an error.
 
 ## How to use
 ```python
 from mathjson_solver import create_solver
```

### Comparing `mathjson-solver-1.4.1/setup.cfg` & `mathjson-solver-1.4.2/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mathjson-solver
-version = 1.4.1
+version = 1.4.2
 author = Martins Mednis
 author_email = mrt@mednis.info
 description = Utilities for MathJSON evaluation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/LongenesisLtd/mathjson-solver
 project_urls =
```

### Comparing `mathjson-solver-1.4.1/setup.py` & `mathjson-solver-1.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mathjson-solver",
-    version="1.4.1",
+    version="1.4.2",
     author="Martins Mednis",
     author_email="mrt@mednis.info",
     description="Utilities for MathJSON evaluation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LongenesisLtd/mathjson-solver",
     project_urls={
```

### Comparing `mathjson-solver-1.4.1/src/mathjson_solver/__main__.py` & `mathjson-solver-1.4.2/src/mathjson_solver/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,19 @@
                 for x in s[1:-1]:
                     if len(x) != 2:
                         raise ValueError(f"Wrong if or elif in 'If'")
                     if f(x[0], c):
                         return f(x[1], c)
                 return f(s[-1], c)
 
+            def Str(s):
+                if len(s) < 2:
+                    raise ValueError(f"Wrong parameters for 'Str'")
+                return f"{f(s[1])}"
+
             constructs = {
                 "Add": lambda s: sum([f(x, c) for x in s[1:]]),
                 "Sum": lambda s: sum([f(x, c) for x in s[1:]]),
                 "Subtract": lambda s: reduce(
                     lambda a, b: a - b, [f(x, c) for x in s[1:]]
                 ),
                 "Constants": Constants,
@@ -165,14 +170,15 @@
                 "Median": Median,
                 "Length": Length,
                 "Any": Any,
                 "All": All,
                 "Array": Arr,
                 "Int": Int,
                 "Float": Float,
+                "Str": Str
             }
             if s[0] in constructs:
                 try:
                     return constructs[s[0]](s)
                 except Exception as e:
                     raise MathJSONException(e, s, mathjson_construct=s[0])
             else:
```

### Comparing `mathjson-solver-1.4.1/src/mathjson_solver.egg-info/PKG-INFO` & `mathjson-solver-1.4.2/src/mathjson_solver.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathjson-solver
-Version: 1.4.1
+Version: 1.4.2
 Summary: Utilities for MathJSON evaluation
 Home-page: https://github.com/LongenesisLtd/mathjson-solver
 Author: Martins Mednis
 Author-email: mrt@mednis.info
 Project-URL: Bug Tracker, https://github.com/LongenesisLtd/mathjson-solver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,14 +18,18 @@
 [![Gitter](https://badges.gitter.im/mathjson-solver/community.svg)](https://gitter.im/mathjson-solver/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 
 _MathJSON Solver_ is a Python module to numerically evaluate MathJSON expressions. It was created by [Longenesis](https://longenesis.com/team) to add numerical evaluation capability of user generated mathematical expressions in Longenesis digital health products and later released as open source project. Its development was inspired by [CortexJS](https://cortexjs.io/compute-engine/) Compute Engine.
 
 Please ask questions and share feedback in our Gitter chat [https://gitter.im/mathjson-solver/community](https://gitter.im/mathjson-solver/community).
 
 ## What's new
+
+### 1.4.2
+Added `Str` construct. It tries to convert value to string.
+
 ### 1.4.0
 We changed the behavior of `Average` to be more forgiving. In version 1.4.0 `Average` accepts arrays like `[2, 4 ,"6"]` and internally converts numeric strings to floats.
 Also, it skips values that cannot be converted to numeric. Internally `Average` will convert array `[2, "three", 4 ,"6"]` to `[2.0, 4.0 ,6.0]`. When given an empty array, `Average` now returns `None` instead of throwing an error.
 
 ## How to use
 ```python
 from mathjson_solver import create_solver
```

### Comparing `mathjson-solver-1.4.1/tests/test_with_pytest.py` & `mathjson-solver-1.4.2/tests/test_with_pytest.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,16 @@
         ({}, ["Round", ["Exp", 2], 3], 7.389),
         ({}, ["Divide", 10, ["Add", 2, 3]], 2),
         ({}, ["Round", ["Log", 2.7183], 3], 1.0),
         ({}, ["Log2", 8], 3),
         ({}, ["Log10", 1000], 3),
         ({}, ["Equal", 10, 10], True),
         ({}, ["Equal", 10, 12], False),
+        ({}, ["Equal", "aaa", "aaa"], True),
+        ({}, ["Equal", "aaa", "baa"], False),
         ({}, ["Abs", -3.5], 3.5),
         ({}, ["Round", -5.123456, 2], -5.12),
         ({}, ["Round", -5.123456, 0], -5),
         ({}, ["Round", 5.4], 5),
         ({}, ["Round", 5.5], 6),
         ({}, ["Constants", ["a", 1], ["b", 2], "a"], 1),
         ({}, ["Constants", ["a", 1], ["b", 2], ["c", 100], ["Sum", "a", "b"]], 3),
@@ -81,14 +83,21 @@
         ({}, ["Int", "12.2"], 12),
         ({}, ["Float", "12.2"], 12.2),
         ({}, ["Any", ["Array", 0, 0, False, 0, 0]], False),
         ({}, ["Any", ["Array", 0, 1, False, 0, 0]], True),
         ({}, ["All", ["Array", 0, 1, False, 0, 0]], False),
         ({}, ["All", ["Array", 0, 1, False, "", 0]], False),
         ({}, ["All", ["Array", 2, 1, True, "zz", 2]], True),
+        ({}, ["Str", 12], "12"),
+        ({}, ["Str", "12"], "12"),
+        ({}, ["Str", "aabb"], "aabb"),
+        ({}, "aabb", "aabb"),
+        ({}, 11, 11),
+        ({}, True, True),
+        ({}, False, False),
     ],
 )
 def test_solver_simple(parameters, expression, expected_result):
     solver = create_solver(parameters)
     assert solver(expression) == expected_result
```

