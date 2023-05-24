# Comparing `tmp/stdl-0.4.4.tar.gz` & `tmp/stdl-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdl-0.4.4.tar", last modified: Mon May 15 18:47:43 2023, max compression
+gzip compressed data, was "stdl-0.4.5.tar", last modified: Wed May 24 20:22:12 2023, max compression
```

## Comparing `stdl-0.4.4.tar` & `stdl-0.4.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:47:43.444609 stdl-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 18:47:32.000000 stdl-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-15 18:47:43.444609 stdl-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-15 18:47:32.000000 stdl-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-15 18:47:32.000000 stdl-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 18:47:43.444609 stdl-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 18:47:32.000000 stdl-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:47:43.440609 stdl-0.4.4/stdl/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-15 18:47:32.000000 stdl-0.4.4/stdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-15 18:47:32.000000 stdl-0.4.4/stdl/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-15 18:47:32.000000 stdl-0.4.4/stdl/dt.py
--rw-r--r--   0 runner    (1001) docker     (123)    27845 2023-05-15 18:47:32.000000 stdl-0.4.4/stdl/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-15 18:47:32.000000 stdl-0.4.4/stdl/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-15 18:47:32.000000 stdl-0.4.4/stdl/lst.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-15 18:47:32.000000 stdl-0.4.4/stdl/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-05-15 18:47:32.000000 stdl-0.4.4/stdl/str_u.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:47:43.444609 stdl-0.4.4/stdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-15 18:47:43.000000 stdl-0.4.4/stdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-15 18:47:43.000000 stdl-0.4.4/stdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 18:47:43.000000 stdl-0.4.4/stdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-15 18:47:43.000000 stdl-0.4.4/stdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-15 18:47:43.000000 stdl-0.4.4/stdl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:22:12.500075 stdl-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-24 20:21:57.000000 stdl-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-24 20:22:12.500075 stdl-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-24 20:21:57.000000 stdl-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-24 20:21:57.000000 stdl-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 20:22:12.500075 stdl-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 20:21:57.000000 stdl-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:22:12.500075 stdl-0.4.5/stdl/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-24 20:21:57.000000 stdl-0.4.5/stdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-24 20:21:57.000000 stdl-0.4.5/stdl/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-24 20:21:57.000000 stdl-0.4.5/stdl/dt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27845 2023-05-24 20:21:57.000000 stdl-0.4.5/stdl/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-24 20:21:57.000000 stdl-0.4.5/stdl/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-24 20:21:57.000000 stdl-0.4.5/stdl/lst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-24 20:21:57.000000 stdl-0.4.5/stdl/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-05-24 20:21:57.000000 stdl-0.4.5/stdl/str_u.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:22:12.500075 stdl-0.4.5/stdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-24 20:22:12.000000 stdl-0.4.5/stdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-24 20:22:12.000000 stdl-0.4.5/stdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:22:12.000000 stdl-0.4.5/stdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-24 20:22:12.000000 stdl-0.4.5/stdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 20:22:12.000000 stdl-0.4.5/stdl.egg-info/top_level.txt
```

### Comparing `stdl-0.4.4/LICENSE` & `stdl-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `stdl-0.4.4/PKG-INFO` & `stdl-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdl
-Version: 0.4.4
+Version: 0.4.5
 Summary: Extended Python Standard Library
 Author-email: Žiga Ivanšek <ziga.ivansek@gmail.com>
 Project-URL: Repository, https://github.com/zigai/stdl
 Keywords: python utilites,filesystem,string manipulation,logging configuration,list utils,standard library
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `stdl-0.4.4/README.md` & `stdl-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `stdl-0.4.4/pyproject.toml` & `stdl-0.4.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-[build-system]
-requires = ["setuptools", "setuptools-scm"]
-build-backend = "setuptools.build_meta"
-
 [project]
 name = "stdl"
-version = "0.4.4"
+version = "0.4.5"
 description = "Extended Python Standard Library"
 authors = [{ name = "Žiga Ivanšek", email = "ziga.ivansek@gmail.com" }]
 license = { file = "LICENSE.txt" }
 readme = "README.md"
 requires-python = ">=3.10"
+dependencies = ["PyYAML>=6.0", "tqdm", "python-dateutil==2.8.2"]
 
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.10",
@@ -26,15 +23,14 @@
     "filesystem",
     "string manipulation",
     "logging configuration",
     "list utils",
     "standard library",
 ]
 
-dependencies = ["PyYAML>=6.0", "tqdm", "python-dateutil==2.8.2"]
 
 [project.optional-dependencies]
 test = ["pytest"]
 dev = ["black", "pytest", "flake8"]
 
 [project.urls]
 Repository = "https://github.com/zigai/stdl"
@@ -68,7 +64,11 @@
     "node_modules",
     "venv",
     "tests",
 ]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401", "E402"]
+
+[build-system]
+requires = ["setuptools", "setuptools-scm"]
+build-backend = "setuptools.build_meta"
```

### Comparing `stdl-0.4.4/stdl/dataclass.py` & `stdl-0.4.5/stdl/dataclass.py`

 * *Files identical despite different names*

### Comparing `stdl-0.4.4/stdl/dt.py` & `stdl-0.4.5/stdl/dt.py`

 * *Files identical despite different names*

### Comparing `stdl-0.4.4/stdl/fs.py` & `stdl-0.4.5/stdl/fs.py`

 * *Files identical despite different names*

### Comparing `stdl-0.4.4/stdl/log.py` & `stdl-0.4.5/stdl/log.py`

 * *Files identical despite different names*

### Comparing `stdl-0.4.4/stdl/lst.py` & `stdl-0.4.5/stdl/lst.py`

 * *Files identical despite different names*

### Comparing `stdl-0.4.4/stdl/net.py` & `stdl-0.4.5/stdl/net.py`

 * *Files identical despite different names*

### Comparing `stdl-0.4.4/stdl/str_u.py` & `stdl-0.4.5/stdl/str_u.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import re
 import textwrap
 from platform import system
 from sys import stdout
 
 CSI_RESET = "\033["
+NO_COLOR = bool(os.environ.get("NO_COLOR", False))
 
 
 def ansi_code(n: int) -> str:
     return f"{CSI_RESET}{n}m"
 
 
 def _get_ansi_val(val: str | None, handler) -> str:
@@ -18,15 +19,16 @@
         clr = handler[val]
         return clr
     except KeyError:
         return val
 
 
 class ColorANSI:
-    if not stdout.isatty():  # Cancel SGR codes if we don't write to a terminal
+    # Cancel SGR codes if we don't write to a terminal
+    if not stdout.isatty():
         for _ in dir():
             if isinstance(_, str) and _[0] != "_":
                 locals()[_] = ""
     else:
         if system() == "Windows":  # Enable VT mode
             kernel32 = __import__("ctypes").windll.kernel32
             kernel32.SetConsoleMode(kernel32.GetStdHandle(-11), 7)
@@ -42,15 +44,15 @@
     @classmethod
     @property
     def dict(cls) -> dict[str, str]:
         d = {}
         ignored = ["dict", "print_all", "get_all"]
         for i in dir(cls):
             if i[0] != "_" and i not in ignored:
-                d[i] = cls.__class_getitem__(i)
+                d[i] = cls[i]
         return d
 
     @classmethod
     def get_all(cls) -> list[str]:
         return [i for i in cls.dict.keys()]
 
     @classmethod
@@ -128,14 +130,16 @@
         color (str, optional): The color to use for the text.
         background (str, optional): The color to use for the background.
         style (str, optional): The style to use for the text.
 
     Returns:
         str: The colorized text.
     """
+    if NO_COLOR:
+        return text
     color = _get_ansi_val(color, FG)
     background = _get_ansi_val(background, BG)
     style = _get_ansi_val(style, ST)
     return f"{color}{background}{style}{text}{ST.RESET}"
 
 
 def terminal_link(
@@ -195,15 +199,14 @@
 
     Args:
         s (str): Input string
         chrs (str | set): Characters to keep
         replacement (str, optional): If provided, replace other characters with this value.
 
     """
-    # return re.compile("[^" + "".join(set(chrs)) + "]").sub(replacement, s)
     string = []
     chrs = set(chrs)
     for c in s:
         if c in chrs:
             string.append(c)
         else:
             if replacement:
```

### Comparing `stdl-0.4.4/stdl.egg-info/PKG-INFO` & `stdl-0.4.5/stdl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdl
-Version: 0.4.4
+Version: 0.4.5
 Summary: Extended Python Standard Library
 Author-email: Žiga Ivanšek <ziga.ivansek@gmail.com>
 Project-URL: Repository, https://github.com/zigai/stdl
 Keywords: python utilites,filesystem,string manipulation,logging configuration,list utils,standard library
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

