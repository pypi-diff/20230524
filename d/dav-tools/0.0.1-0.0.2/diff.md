# Comparing `tmp/dav_tools-0.0.1.tar.gz` & `tmp/dav_tools-0.0.2.tar.gz`

## Comparing `dav_tools-0.0.1.tar` & `dav_tools-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 dav_tools-0.0.1/Makefile
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 dav_tools-0.0.1/src/dav_tools/__init__.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 dav_tools-0.0.1/src/dav_tools/_arg_parser.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 dav_tools-0.0.1/src/dav_tools/_text_format.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 dav_tools-0.0.1/src/dav_tools/commands.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dav_tools-0.0.1/src/dav_tools/devtools.py
--rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 dav_tools-0.0.1/src/dav_tools/messages.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 dav_tools-0.0.1/src/dav_tools/text_color.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dav_tools-0.0.1/src/dav_tools/user.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 dav_tools-0.0.1/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 dav_tools-0.0.1/LICENSE
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 dav_tools-0.0.1/README.md
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 dav_tools-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 dav_tools-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 dav_tools-0.0.2/Makefile
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 dav_tools-0.0.2/src/dav_tools/__init__.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 dav_tools-0.0.2/src/dav_tools/_arg_parser.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 dav_tools-0.0.2/src/dav_tools/_text_format.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 dav_tools-0.0.2/src/dav_tools/commands.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dav_tools-0.0.2/src/dav_tools/devtools.py
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 dav_tools-0.0.2/src/dav_tools/messages.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 dav_tools-0.0.2/src/dav_tools/text_color.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dav_tools-0.0.2/src/dav_tools/user.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 dav_tools-0.0.2/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 dav_tools-0.0.2/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 dav_tools-0.0.2/README.md
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dav_tools-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 dav_tools-0.0.2/PKG-INFO
```

### Comparing `dav_tools-0.0.1/Makefile` & `dav_tools-0.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `dav_tools-0.0.1/src/dav_tools/_arg_parser.py` & `dav_tools-0.0.2/src/dav_tools/_arg_parser.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.0.1/src/dav_tools/_text_format.py` & `dav_tools-0.0.2/src/dav_tools/_text_format.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.0.1/src/dav_tools/commands.py` & `dav_tools-0.0.2/src/dav_tools/commands.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.0.1/src/dav_tools/messages.py` & `dav_tools-0.0.2/src/dav_tools/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             _print_colored_text(icon, *icon_options, TextFormat.Style.BOLD, TextFormat.Style.BLINK, end='', file=file)
         else:
             _print_colored_text(icon, *icon_options, TextFormat.Style.BOLD, end='', file=file)
         
         _print_colored_text(']', *icon_options, TextFormat.Style.BOLD, end='', file=file)
         _print_colored_text(' ', end='', file=file)
     
-    _print_colored_text(str(text), *text_options, end=end, file=file)
+    _print_colored_text(str(text), *text_options, end=end, file=file, flush=True)
     
 
 # message indicating an information
 def info(text: str, blink=False) -> None:
     message(text,
              icon='*',
              icon_options=[
@@ -98,15 +98,15 @@
     )
 
 # prints a question and returns the answer
 def ask(question: str, end=': ') -> str:
     message(f'{question}{end}',
              icon='?',
              icon_options=[
-                 TextFormat.Color.BLUE
+                 TextFormat.Color.PURPLE
              ],
              end='')
     
     return _input_colored(
         TextFormat.Style.ITALIC,
     )
```

### Comparing `dav_tools-0.0.1/src/dav_tools/text_color.py` & `dav_tools-0.0.2/src/dav_tools/text_color.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,21 +19,21 @@
     result = ''
     result += get_format(*format_options)
     result += text
     result += get_format(TextFormat.RESET)
 
     return result
 
-def print_colored_text(text: str, *format_options, end: str='\n', file=_sys.stdout):
+def print_colored_text(text: str, *format_options, end: str='\n', file=_sys.stdout, flush=False):
     text = get_colored_text(text, *format_options)
-    print(text, end=end, file=file)
+    print(text, end=end, file=file, flush=flush)
 
 def input_colored(*format_options):
     set_format(*format_options, file=_sys.stderr)
     result = input()
     set_format(TextFormat.RESET)
 
     return result
 
-def clear_line(file=_sys.stdout):
+def clear_line(file=_sys.stdout, flush=False):
     print('\r', ' ' * TextFormat.get_term_len(), '\r',
-          sep='', end='', file=file)
+          sep='', end='', file=file, flush=flush)
```

### Comparing `dav_tools-0.0.1/LICENSE` & `dav_tools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dav_tools-0.0.1/pyproject.toml` & `dav_tools-0.0.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dav_tools"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Davide Ponzini", email="davide.ponzini95@gmail.com" },
 ]
-description = "Various utilies to aid in program developent"
+description = "Various utilies to aid in program development"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
```

### Comparing `dav_tools-0.0.1/PKG-INFO` & `dav_tools-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: dav_tools
-Version: 0.0.1
-Summary: Various utilies to aid in program developent
+Version: 0.0.2
+Summary: Various utilies to aid in program development
 Project-URL: Homepage, https://github.com/DavidePonzini/dav-utils
 Project-URL: Bug Tracker, https://github.com/DavidePonzini/dav-utils/issues
 Author-email: Davide Ponzini <davide.ponzini95@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# DavUtils
+# dav_tools
+Personal Python library to aid in software development
```

