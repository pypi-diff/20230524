# Comparing `tmp/jorun-0.0.7.tar.gz` & `tmp/jorun-0.1.0.tar.gz`

## Comparing `jorun-0.0.7.tar` & `jorun-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,30 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.0.7/src/jorun/__init__.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 jorun-0.0.7/src/jorun/configuration.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 jorun-0.0.7/src/jorun/logger.py
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 jorun-0.0.7/src/jorun/main.py
--rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 jorun-0.0.7/src/jorun/runner.py
--rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 jorun-0.0.7/src/jorun/runner_threading.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 jorun-0.0.7/src/jorun/task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jorun-0.0.7/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 jorun-0.0.7/LICENSE
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 jorun-0.0.7/README.md
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jorun-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 jorun-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/__init__.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/configuration.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/constants.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/errors.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/logger.py
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/main.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/runner.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/scanner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/handler/__init__.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/handler/base.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/handler/docker.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/handler/group.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/handler/shell.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/palette/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/palette/base.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/palette/darcula.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/types/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/types/options.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/types/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/ui/__init__.py
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/ui/application.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/ui/data_signals.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/ui/main_window.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 jorun-0.1.0/src/jorun/ui/task_panel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jorun-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 jorun-0.1.0/LICENSE
+-rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 jorun-0.1.0/README.md
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jorun-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 jorun-0.1.0/PKG-INFO
```

### Comparing `jorun-0.0.7/LICENSE` & `jorun-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jorun-0.0.7/pyproject.toml` & `jorun-0.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jorun"
-version = "0.0.7"
+version = "0.1.0"
 authors = [
   { name="Paolo Infante", email="info@paoloinfante.it" },
 ]
 description = "A customizable task runner"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "PyYAML==6.0"
+    "PyYAML==6.0",
+    "PyQt6==6.5.0",
+    "tinyioc==0.1.4"
 ]
 
 [project.scripts]
 jorun = "jorun.main:main"
 
 [project.urls]
 "Homepage" = "https://github.com/paolo-projects/jorun"
```

