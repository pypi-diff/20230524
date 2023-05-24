# Comparing `tmp/dav_tools-0.0.2.tar.gz` & `tmp/dav_tools-0.0.4.tar.gz`

## Comparing `dav_tools-0.0.2.tar` & `dav_tools-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 dav_tools-0.0.2/Makefile
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 dav_tools-0.0.2/src/dav_tools/__init__.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 dav_tools-0.0.2/src/dav_tools/_arg_parser.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 dav_tools-0.0.2/src/dav_tools/_text_format.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 dav_tools-0.0.2/src/dav_tools/commands.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dav_tools-0.0.2/src/dav_tools/devtools.py
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 dav_tools-0.0.2/src/dav_tools/messages.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 dav_tools-0.0.2/src/dav_tools/text_color.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dav_tools-0.0.2/src/dav_tools/user.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 dav_tools-0.0.2/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 dav_tools-0.0.2/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 dav_tools-0.0.2/README.md
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dav_tools-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 dav_tools-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 dav_tools-0.0.4/Makefile
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 dav_tools-0.0.4/src/dav_tools/__init__.py
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 dav_tools-0.0.4/src/dav_tools/_arg_parser.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 dav_tools-0.0.4/src/dav_tools/_text_format.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 dav_tools-0.0.4/src/dav_tools/commands.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dav_tools-0.0.4/src/dav_tools/devtools.py
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 dav_tools-0.0.4/src/dav_tools/messages.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 dav_tools-0.0.4/src/dav_tools/text_color.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dav_tools-0.0.4/src/dav_tools/user.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 dav_tools-0.0.4/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 dav_tools-0.0.4/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 dav_tools-0.0.4/README.md
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dav_tools-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 dav_tools-0.0.4/PKG-INFO
```

### Comparing `dav_tools-0.0.2/Makefile` & `dav_tools-0.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `dav_tools-0.0.2/src/dav_tools/_arg_parser.py` & `dav_tools-0.0.4/src/dav_tools/_arg_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,27 +12,29 @@
     EXTEND = 'extend'
     BOOLEAN_OPTIONAL = argparse.BooleanOptionalAction
 
 
 class ArgumentParser:
     def __init__(self) -> None:
         self.parser = argparse.ArgumentParser(
-            formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-            epilog = text_color.get_colored_text('--Developed by Davide Ponzini (davide.ponzini95@gmail.com)', text_color.TextFormat.Style.ITALIC)
-        )
+            formatter_class=argparse.ArgumentDefaultsHelpFormatter
+            )
 
         self.__groups = {}
 
 
     def set_version(self, version: str):
         self.parser.add_argument('--version', action='version', version=f'%(prog)s {version}')
 
     def set_description(self, description) -> None:
         self.parser.description = description
 
+    def set_developer_info(self, name, email):
+        self.parser.epilog = text_color.get_colored_text(f'--Developed by {name} ({email})', text_color.TextFormat.Style.ITALIC)
+
     @property
     def args(self) -> argparse.Namespace:
         return self.parser.parse_args()
     
 
     def __group(self, name: str, description: str = None) -> argparse._ArgumentGroup:
         if name in self.__groups:
```

### Comparing `dav_tools-0.0.2/src/dav_tools/_text_format.py` & `dav_tools-0.0.4/src/dav_tools/_text_format.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.0.2/src/dav_tools/commands.py` & `dav_tools-0.0.4/src/dav_tools/commands.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.0.2/src/dav_tools/messages.py` & `dav_tools-0.0.4/src/dav_tools/messages.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,102 +3,104 @@
 from .text_color import TextFormat
 from .text_color import print_colored_text as _print_colored_text
 from .text_color import input_colored as _input_colored
 from .text_color import clear_line as _clear_line
 
 
 # generic and customizable message
-def message(text: str | object, icon=None, text_options=[], icon_options=[], blink=False, end='\n', file=_sys.stderr):
+def message(*text: str | object, icon=None, text_options=[[]], icon_options=[], blink=False, end='\n', file=_sys.stderr):
     _clear_line()
 
     if icon is not None:
         _print_colored_text('[', *icon_options, TextFormat.Style.BOLD, end='', file=file)
         
         if blink:
             _print_colored_text(icon, *icon_options, TextFormat.Style.BOLD, TextFormat.Style.BLINK, end='', file=file)
         else:
             _print_colored_text(icon, *icon_options, TextFormat.Style.BOLD, end='', file=file)
         
         _print_colored_text(']', *icon_options, TextFormat.Style.BOLD, end='', file=file)
         _print_colored_text(' ', end='', file=file)
     
-    _print_colored_text(str(text), *text_options, end=end, file=file, flush=True)
+    for t,o in zip(text, text_options):
+        _print_colored_text(str(t), *o, end=' ', file=file, flush=True)
+    print(end=end)
     
-
 # message indicating an information
-def info(text: str, blink=False) -> None:
-    message(text,
+def info(*text: str | object, text_options=[[]], blink=False) -> None:
+    message(*text,
              icon='*',
              icon_options=[
                  TextFormat.Color.BLUE
-             ], 
+             ],
+             text_options=text_options,
              blink=blink)
-    
+
 # messages indicating an action which is still happening
 def progress(text: str) -> None:
     message(text,
             icon=' ',
             end='\r',
-            text_options=[
+            text_options=[[
                 TextFormat.Color.DARKGRAY,
                 TextFormat.Style.ITALIC
-            ])
+            ]])
 
 # message indicating an error
 def error(text: str, blink=False) -> None:
     message(text, 
              icon='-', 
              blink=blink,
              icon_options=[
                  TextFormat.Color.RED
              ],
-             text_options=[
+             text_options=[[
                  TextFormat.Color.RED
-             ]
+             ]]
     )
 
 # message indicating a critical error. The program terminates after showing this message
 def critical_error(text: str, blink=False, exit_code=1) -> None:
     message(text, 
              icon='x', 
              blink=blink,
              icon_options=[
                  TextFormat.Color.RED
              ],
-             text_options=[
+             text_options=[[
                  TextFormat.Color.RED
-             ]
+             ]]
     )
 
     _sys.exit(exit_code)
 
 # message indicating a warning
 def warning(text: str, blink=False) -> None:
     message(text, 
              icon='!', 
              blink=blink,
              icon_options=[
                  TextFormat.Color.YELLOW
              ],
-             text_options=[
+             text_options=[[
                  TextFormat.Color.YELLOW
-             ]
+             ]]
     )
 
 # message indicating a successfully completed action
 def success(text: str, blink=False) -> None:
     message(text, 
              icon='+', 
              blink=blink,
              icon_options=[
                  TextFormat.Color.GREEN
              ],
-             text_options=[
+             text_options=[[
                  TextFormat.Color.GREEN
-             ]
+             ]]
     )
 
 # prints a question and returns the answer
 def ask(question: str, end=': ') -> str:
     message(f'{question}{end}',
              icon='?',
              icon_options=[
```

### Comparing `dav_tools-0.0.2/src/dav_tools/text_color.py` & `dav_tools-0.0.4/src/dav_tools/text_color.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.0.2/LICENSE` & `dav_tools-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dav_tools-0.0.2/pyproject.toml` & `dav_tools-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dav_tools"
-version = "0.0.2"
+version = "0.0.4"
 authors = [
   { name="Davide Ponzini", email="davide.ponzini95@gmail.com" },
 ]
 description = "Various utilies to aid in program development"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dav_tools-0.0.2/PKG-INFO` & `dav_tools-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dav_tools
-Version: 0.0.2
+Version: 0.0.4
 Summary: Various utilies to aid in program development
 Project-URL: Homepage, https://github.com/DavidePonzini/dav-utils
 Project-URL: Bug Tracker, https://github.com/DavidePonzini/dav-utils/issues
 Author-email: Davide Ponzini <davide.ponzini95@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

