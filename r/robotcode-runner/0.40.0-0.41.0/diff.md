# Comparing `tmp/robotcode_runner-0.40.0.tar.gz` & `tmp/robotcode_runner-0.41.0.tar.gz`

## Comparing `robotcode_runner-0.40.0.tar` & `robotcode_runner-0.41.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.40.0/src/robotcode/runner/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.40.0/src/robotcode/runner/__version__.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 robotcode_runner-0.40.0/src/robotcode/runner/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.40.0/src/robotcode/runner/py.typed
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.40.0/src/robotcode/runner/cli/__init__.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 robotcode_runner-0.40.0/src/robotcode/runner/cli/libdoc.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 robotcode_runner-0.40.0/src/robotcode/runner/cli/rebot.py
--rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 robotcode_runner-0.40.0/src/robotcode/runner/cli/robot.py
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 robotcode_runner-0.40.0/src/robotcode/runner/cli/testdoc.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.40.0/src/robotcode/runner/cli/discover/__init__.py
--rw-r--r--   0        0        0    20426 2020-02-02 00:00:00.000000 robotcode_runner-0.40.0/src/robotcode/runner/cli/discover/discover.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.40.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.40.0/LICENSE.txt
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.40.0/README.md
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 robotcode_runner-0.40.0/pyproject.toml
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 robotcode_runner-0.40.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/src/robotcode/runner/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/src/robotcode/runner/__version__.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/src/robotcode/runner/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/src/robotcode/runner/py.typed
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/src/robotcode/runner/cli/__init__.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/src/robotcode/runner/cli/libdoc.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/src/robotcode/runner/cli/rebot.py
+-rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/src/robotcode/runner/cli/robot.py
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/src/robotcode/runner/cli/testdoc.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/src/robotcode/runner/cli/discover/__init__.py
+-rw-r--r--   0        0        0    20419 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/src/robotcode/runner/cli/discover/discover.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/LICENSE.txt
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/README.md
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/pyproject.toml
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 robotcode_runner-0.41.0/PKG-INFO
```

### Comparing `robotcode_runner-0.40.0/src/robotcode/runner/cli/libdoc.py` & `robotcode_runner-0.41.0/src/robotcode/runner/cli/libdoc.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.40.0/src/robotcode/runner/cli/rebot.py` & `robotcode_runner-0.41.0/src/robotcode/runner/cli/rebot.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.40.0/src/robotcode/runner/cli/robot.py` & `robotcode_runner-0.41.0/src/robotcode/runner/cli/robot.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.40.0/src/robotcode/runner/cli/testdoc.py` & `robotcode_runner-0.41.0/src/robotcode/runner/cli/testdoc.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.40.0/src/robotcode/runner/cli/discover/discover.py` & `robotcode_runner-0.41.0/src/robotcode/runner/cli/discover/discover.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     old_get_file = FileReader._get_file
 
     def get_file(self: FileReader, source: Union[str, Path, IOBase], accept_text: bool) -> Any:
         path = self._get_path(source, accept_text)
         if path:
             if _stdin_data is not None and (data := _stdin_data.get(str(path))) is not None:
                 if data is not None:
-                    return old_get_file(self, data, accept_text)
+                    return old_get_file(self, data, True)
 
         return old_get_file(self, source, accept_text)
 
     FileReader._get_file = get_file
 
 
 @dataclass
```

### Comparing `robotcode_runner-0.40.0/.gitignore` & `robotcode_runner-0.41.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.40.0/LICENSE.txt` & `robotcode_runner-0.41.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.40.0/README.md` & `robotcode_runner-0.41.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.40.0/pyproject.toml` & `robotcode_runner-0.41.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -24,17 +24,17 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-robot==0.40.0",
-  "robotcode-modifiers==0.40.0",
-  "robotcode==0.40.0",
+  "robotcode-robot==0.41.0",
+  "robotcode-modifiers==0.41.0",
+  "robotcode==0.41.0",
 ]
 
 [project.entry-points.robotcode]
 runner = "robotcode.runner.hooks"
 
 [project.urls]
 Homepage = "https://robotcode.io"
```

### Comparing `robotcode_runner-0.40.0/PKG-INFO` & `robotcode_runner-0.41.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-runner
-Version: 0.40.0
+Version: 0.41.0
 Summary: RobotCode runner plugin for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,17 +21,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-modifiers==0.40.0
-Requires-Dist: robotcode-robot==0.40.0
-Requires-Dist: robotcode==0.40.0
+Requires-Dist: robotcode-modifiers==0.41.0
+Requires-Dist: robotcode-robot==0.41.0
+Requires-Dist: robotcode==0.41.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-runner
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
```

