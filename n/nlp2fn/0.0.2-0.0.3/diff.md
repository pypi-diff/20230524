# Comparing `tmp/nlp2fn-0.0.2.tar.gz` & `tmp/nlp2fn-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp2fn-0.0.2.tar", last modified: Mon May 22 08:05:59 2023, max compression
+gzip compressed data, was "nlp2fn-0.0.3.tar", last modified: Wed May 24 13:25:17 2023, max compression
```

## Comparing `nlp2fn-0.0.2.tar` & `nlp2fn-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 jennie     (502) staff       (20)        0 2023-05-22 08:05:59.925998 nlp2fn-0.0.2/
--rw-r--r--   0 jennie     (502) staff       (20)     2390 2023-05-22 08:05:59.925861 nlp2fn-0.0.2/PKG-INFO
--rw-r--r--   0 jennie     (502) staff       (20)     1855 2023-05-22 08:02:04.000000 nlp2fn-0.0.2/README.md
-drwxr-xr-x   0 jennie     (502) staff       (20)        0 2023-05-22 08:05:59.923090 nlp2fn-0.0.2/nlp2fn/
--rw-r--r--   0 jennie     (502) staff       (20)     1663 2023-05-20 22:48:22.000000 nlp2fn-0.0.2/nlp2fn/__init__.py
--rw-r--r--   0 jennie     (502) staff       (20)        0 2023-05-20 21:04:58.000000 nlp2fn-0.0.2/nlp2fn/constants.py
--rw-r--r--   0 jennie     (502) staff       (20)     2732 2023-05-20 22:48:22.000000 nlp2fn-0.0.2/nlp2fn/fncloader.py
-drwxr-xr-x   0 jennie     (502) staff       (20)        0 2023-05-22 08:05:59.925516 nlp2fn-0.0.2/nlp2fn/utils/
--rw-r--r--   0 jennie     (502) staff       (20)     1912 2023-05-20 22:34:33.000000 nlp2fn-0.0.2/nlp2fn/utils/__init__.py
--rw-r--r--   0 jennie     (502) staff       (20)      542 2023-05-20 22:26:48.000000 nlp2fn-0.0.2/nlp2fn/utils/colorpriniting.py
--rw-r--r--   0 jennie     (502) staff       (20)      648 2023-05-20 22:38:13.000000 nlp2fn-0.0.2/nlp2fn/utils/commands.py
--rw-r--r--   0 jennie     (502) staff       (20)     2143 2023-05-19 22:37:53.000000 nlp2fn-0.0.2/nlp2fn/utils/configparser.py
--rw-r--r--   0 jennie     (502) staff       (20)     3395 2023-05-19 22:40:17.000000 nlp2fn-0.0.2/nlp2fn/utils/detectenv.py
-drwxr-xr-x   0 jennie     (502) staff       (20)        0 2023-05-22 08:05:59.924095 nlp2fn-0.0.2/nlp2fn.egg-info/
--rw-r--r--   0 jennie     (502) staff       (20)     2390 2023-05-22 08:05:59.000000 nlp2fn-0.0.2/nlp2fn.egg-info/PKG-INFO
--rw-r--r--   0 jennie     (502) staff       (20)      395 2023-05-22 08:05:59.000000 nlp2fn-0.0.2/nlp2fn.egg-info/SOURCES.txt
--rw-r--r--   0 jennie     (502) staff       (20)        1 2023-05-22 08:05:59.000000 nlp2fn-0.0.2/nlp2fn.egg-info/dependency_links.txt
--rw-r--r--   0 jennie     (502) staff       (20)       42 2023-05-22 08:05:59.000000 nlp2fn-0.0.2/nlp2fn.egg-info/entry_points.txt
--rw-r--r--   0 jennie     (502) staff       (20)        9 2023-05-22 08:05:59.000000 nlp2fn-0.0.2/nlp2fn.egg-info/requires.txt
--rw-r--r--   0 jennie     (502) staff       (20)       14 2023-05-22 08:05:59.000000 nlp2fn-0.0.2/nlp2fn.egg-info/top_level.txt
--rw-r--r--   0 jennie     (502) staff       (20)       38 2023-05-22 08:05:59.926038 nlp2fn-0.0.2/setup.cfg
--rw-r--r--   0 jennie     (502) staff       (20)     1000 2023-05-22 08:05:54.000000 nlp2fn-0.0.2/setup.py
+drwxr-xr-x   0 jennie     (502) staff       (20)        0 2023-05-24 13:25:17.316139 nlp2fn-0.0.3/
+-rw-r--r--   0 jennie     (502) staff       (20)     2742 2023-05-24 13:25:17.315969 nlp2fn-0.0.3/PKG-INFO
+-rw-r--r--   0 jennie     (502) staff       (20)     2208 2023-05-24 13:22:33.000000 nlp2fn-0.0.3/README.md
+drwxr-xr-x   0 jennie     (502) staff       (20)        0 2023-05-24 13:25:17.312805 nlp2fn-0.0.3/nlp2fn/
+-rw-r--r--   0 jennie     (502) staff       (20)     2038 2023-05-24 13:17:43.000000 nlp2fn-0.0.3/nlp2fn/__init__.py
+-rw-r--r--   0 jennie     (502) staff       (20)      810 2023-05-24 13:20:40.000000 nlp2fn-0.0.3/nlp2fn/clonefromgit.py
+-rw-r--r--   0 jennie     (502) staff       (20)        0 2023-05-20 21:04:58.000000 nlp2fn-0.0.3/nlp2fn/constants.py
+-rw-r--r--   0 jennie     (502) staff       (20)     2732 2023-05-20 22:48:22.000000 nlp2fn-0.0.3/nlp2fn/fncloader.py
+drwxr-xr-x   0 jennie     (502) staff       (20)        0 2023-05-24 13:25:17.314212 nlp2fn-0.0.3/nlp2fn/git/
+-rw-r--r--   0 jennie     (502) staff       (20)       25 2023-05-24 12:25:45.000000 nlp2fn-0.0.3/nlp2fn/git/__init__.py
+-rw-r--r--   0 jennie     (502) staff       (20)     3994 2023-05-24 12:18:57.000000 nlp2fn-0.0.3/nlp2fn/git/repo.py
+drwxr-xr-x   0 jennie     (502) staff       (20)        0 2023-05-24 13:25:17.315564 nlp2fn-0.0.3/nlp2fn/utils/
+-rw-r--r--   0 jennie     (502) staff       (20)     1950 2023-05-24 13:20:25.000000 nlp2fn-0.0.3/nlp2fn/utils/__init__.py
+-rw-r--r--   0 jennie     (502) staff       (20)      542 2023-05-20 22:26:48.000000 nlp2fn-0.0.3/nlp2fn/utils/colorpriniting.py
+-rw-r--r--   0 jennie     (502) staff       (20)      687 2023-05-24 13:16:04.000000 nlp2fn-0.0.3/nlp2fn/utils/commands.py
+-rw-r--r--   0 jennie     (502) staff       (20)     2143 2023-05-19 22:37:53.000000 nlp2fn-0.0.3/nlp2fn/utils/configparser.py
+-rw-r--r--   0 jennie     (502) staff       (20)     3395 2023-05-19 22:40:17.000000 nlp2fn-0.0.3/nlp2fn/utils/detectenv.py
+drwxr-xr-x   0 jennie     (502) staff       (20)        0 2023-05-24 13:25:17.313812 nlp2fn-0.0.3/nlp2fn.egg-info/
+-rw-r--r--   0 jennie     (502) staff       (20)     2742 2023-05-24 13:25:17.000000 nlp2fn-0.0.3/nlp2fn.egg-info/PKG-INFO
+-rw-r--r--   0 jennie     (502) staff       (20)      460 2023-05-24 13:25:17.000000 nlp2fn-0.0.3/nlp2fn.egg-info/SOURCES.txt
+-rw-r--r--   0 jennie     (502) staff       (20)        1 2023-05-24 13:25:17.000000 nlp2fn-0.0.3/nlp2fn.egg-info/dependency_links.txt
+-rw-r--r--   0 jennie     (502) staff       (20)       42 2023-05-24 13:25:17.000000 nlp2fn-0.0.3/nlp2fn.egg-info/entry_points.txt
+-rw-r--r--   0 jennie     (502) staff       (20)        9 2023-05-24 13:25:17.000000 nlp2fn-0.0.3/nlp2fn.egg-info/requires.txt
+-rw-r--r--   0 jennie     (502) staff       (20)       14 2023-05-24 13:25:17.000000 nlp2fn-0.0.3/nlp2fn.egg-info/top_level.txt
+-rw-r--r--   0 jennie     (502) staff       (20)       38 2023-05-24 13:25:17.316205 nlp2fn-0.0.3/setup.cfg
+-rw-r--r--   0 jennie     (502) staff       (20)     1000 2023-05-24 13:25:12.000000 nlp2fn-0.0.3/setup.py
```

### Comparing `nlp2fn-0.0.2/PKG-INFO` & `nlp2fn-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: nlp2fn
-Version: 0.0.2
+Version: 0.0.3
 Summary: With the ability to load and read Python functions from any specified location, `nlp2fn` brings all your automation tasks together.
 Home-page: https://github.com/dextrop/nlp2fn
 Author: Jennie Developers <saurabh@ask-jennie.com>
 Author-email: Jennie Developers <saurabh@ask-jennie.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 
-# Python Automation Made Simple: nlp2fn
+# Python Automation Made Simple: [nlp2fn](https://pypi.org/project/nlp2fn/)
 
 Welcome to `nlp2fn`, a seamless and intuitive software tool for Python automation. With the ability to load and read Python functions from any specified location, `nlp2fn` brings all your automation tasks together. Whether your functions reside in local directories or remote servers, `nlp2fn` fetches, loads, and prepares them for execution — as simple as a statement.
 
+
 ## The Magic of nlp2fn
 
 A typical function for `nlp2fn` follows this format:
 
 ```python
 # Write you execute statement, this shall be an 
 # input by user to execute your events, make sure all the 
@@ -34,26 +35,35 @@
     return True
 ```
 
 The `execute` function is the heart of the operation where the actual task takes place.
 
 ## Quick Start Guide
 
-Here's how to install and get started with [`nlp2fn`]()f:
+Here's how to install and get started with [`nlp2fn`](https://pypi.org/project/nlp2fn/):
 
 ```bash
 pip install nlp2fn
 ```
 
 Next, add the source directory where your Python functions are located:
 
 ```bash
-nlp2fn set source /path/to/directory
+nlp2fn set-source local /path/to/directory
+```
+
+or 
+
+```bash
+nlp2fn set-source git https://github.com/{githubid}/{repo}
 ```
 
+make sure repo is public.
+
+
 Ready to launch `nlp2fn` as a chatbot? Use this command:
 
 ```bash
 nlp2fn run
 ```
 
 To run a single statement, use the `exec` command:
@@ -73,7 +83,12 @@
 We welcome your contributions! Feel free to submit pull requests and create issues on our [GitHub page](https://github.com/dextrop/nlp2fn/issues).
 
 ## Contact
 
 For questions, suggestions, or any kind of discussion, feel free to open an issue on our GitHub page.
 
 Embrace the simplification of Python automation with `nlp2fn`.
+
+## Events
+
+- Langchain Automations : https://github.com/dextrop/evt-langchain
+- https://medium.com/@askjennie/creating-your-own-automation-library-with-nlp2fn-6657b1276361
```

### Comparing `nlp2fn-0.0.2/README.md` & `nlp2fn-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Python Automation Made Simple: nlp2fn
+# Python Automation Made Simple: [nlp2fn](https://pypi.org/project/nlp2fn/)
 
 Welcome to `nlp2fn`, a seamless and intuitive software tool for Python automation. With the ability to load and read Python functions from any specified location, `nlp2fn` brings all your automation tasks together. Whether your functions reside in local directories or remote servers, `nlp2fn` fetches, loads, and prepares them for execution — as simple as a statement.
 
+
 ## The Magic of nlp2fn
 
 A typical function for `nlp2fn` follows this format:
 
 ```python
 # Write you execute statement, this shall be an 
 # input by user to execute your events, make sure all the 
@@ -22,26 +23,35 @@
     return True
 ```
 
 The `execute` function is the heart of the operation where the actual task takes place.
 
 ## Quick Start Guide
 
-Here's how to install and get started with [`nlp2fn`]()f:
+Here's how to install and get started with [`nlp2fn`](https://pypi.org/project/nlp2fn/):
 
 ```bash
 pip install nlp2fn
 ```
 
 Next, add the source directory where your Python functions are located:
 
 ```bash
-nlp2fn set source /path/to/directory
+nlp2fn set-source local /path/to/directory
+```
+
+or 
+
+```bash
+nlp2fn set-source git https://github.com/{githubid}/{repo}
 ```
 
+make sure repo is public.
+
+
 Ready to launch `nlp2fn` as a chatbot? Use this command:
 
 ```bash
 nlp2fn run
 ```
 
 To run a single statement, use the `exec` command:
@@ -60,8 +70,13 @@
 
 We welcome your contributions! Feel free to submit pull requests and create issues on our [GitHub page](https://github.com/dextrop/nlp2fn/issues).
 
 ## Contact
 
 For questions, suggestions, or any kind of discussion, feel free to open an issue on our GitHub page.
 
-Embrace the simplification of Python automation with `nlp2fn`.
+Embrace the simplification of Python automation with `nlp2fn`.
+
+## Events
+
+- Langchain Automations : https://github.com/dextrop/evt-langchain
+- https://medium.com/@askjennie/creating-your-own-automation-library-with-nlp2fn-6657b1276361
```

### Comparing `nlp2fn-0.0.2/nlp2fn/__init__.py` & `nlp2fn-0.0.3/nlp2fn/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 import sys, os
 from nlp2fn.utils.commands import COMMANDS, map_command_to_function
 from nlp2fn.fncloader import FunctionLoader
 from nlp2fn.utils import update_py_fnc_dir, get_py_fnc_dir, delete_py_fnc_dir_info
 from nlp2fn.utils.colorpriniting import error
+from nlp2fn.clonefromgit import GitEvents
 
 fnLoader = FunctionLoader()
 
 def reset_src_dir(args):
     delete_py_fnc_dir_info()
 
+def set_github_source(args):
+    if len(args) < 1:
+        raise ValueError("Missing Githib link.")
+    GitEvents(args[0])
+
 def set_source_dir(args):
     if len(args) < 1:
         raise ValueError("Missing directory link.")
 
     directory = args[0]
     if not os.path.exists(directory) and directory[:4] != "http":
         raise ValueError(f"Directory {directory} does not exits")
 
-    update_py_fnc_dir(directory)
+    if os.path.expanduser("~/") in directory:
+        update_py_fnc_dir(directory)
+    else:
+        update_py_fnc_dir(os.path.join(os.getcwd(), directory))
 
 def run(args):
     directories = get_py_fnc_dir()
     if len(directories) < 1:
         raise ValueError("Missing source directory")
 
     fnLoader.set_source(directories)
@@ -43,16 +52,18 @@
     fnLoader.execute(
         args[0]
     )
 
 def execute():
     try:
         fn_name, args = map_command_to_function(sys.argv[1:], COMMANDS)
-        if fn_name == "set_function_source":
+        if fn_name == "set_local_source":
             return set_source_dir(args)
+        elif fn_name == "set_github_source":
+            return set_github_source(args)
         elif fn_name == "run":
             return run(args)
         elif fn_name == "run_single_function":
             return run_command(args)
         elif fn_name == "reset":
             return reset_src_dir(args)
```

### Comparing `nlp2fn-0.0.2/nlp2fn/fncloader.py` & `nlp2fn-0.0.3/nlp2fn/fncloader.py`

 * *Files identical despite different names*

### Comparing `nlp2fn-0.0.2/nlp2fn/utils/__init__.py` & `nlp2fn-0.0.3/nlp2fn/utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
+from nlp2fn.utils.colorpriniting import error
 
 # Set up the location of the configuration file.
-TOKEN_PATH = os.path.expanduser("~/.jennie-ai.conf.json")
+TOKEN_PATH = os.path.expanduser("~/.nlp2fn.conf.json")
 
 
 def get_py_fnc_dir():
     """
     This function reads the configuration file specified by TOKEN_PATH.
     It expects each line of the file to represent a location (either a URL or a filesystem path).
     It then checks if the filesystem paths exist, and returns all locations.
@@ -38,18 +39,21 @@
     If the directory is a URL, it is added without any existence check.
 
     Args:
         directory (str): The directory to add. Can be a local filesystem path or a URL.
     """
 
     # If the directory doesn't start with "http", assume it's a filesystem path.
-    if not directory.startswith("http"):
-        # Check if the local directory exists. If not, return without doing anything.
-        if not os.path.exists(directory):
-            raise ValueError(f"Directory {directory} does not exits")
+    if not os.path.exists(directory):
+        raise ValueError(f"Directory {directory} does not exits")
+
+    lines = open(TOKEN_PATH).read().splitlines()
+    if directory in lines:
+        error("Source Already Exits")
+        return
 
     with open(TOKEN_PATH, 'a') as file:
         file.write(f"{directory}\n")
 
     return get_py_fnc_dir()
 
 def delete_py_fnc_dir_info():
```

### Comparing `nlp2fn-0.0.2/nlp2fn/utils/colorpriniting.py` & `nlp2fn-0.0.3/nlp2fn/utils/colorpriniting.py`

 * *Files identical despite different names*

### Comparing `nlp2fn-0.0.2/nlp2fn/utils/commands.py` & `nlp2fn-0.0.3/nlp2fn/utils/commands.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 COMMANDS = {
-    "set": {
-        "source": "set_function_source",
+    "set-source": {
+        "local": "set_local_source",
+        "git": "set_github_source",
     },
     "run": "run",
     "reset": "reset",
     "exec": {
         "-m": "run_single_function"
     }
 }
```

### Comparing `nlp2fn-0.0.2/nlp2fn/utils/configparser.py` & `nlp2fn-0.0.3/nlp2fn/utils/configparser.py`

 * *Files identical despite different names*

### Comparing `nlp2fn-0.0.2/nlp2fn/utils/detectenv.py` & `nlp2fn-0.0.3/nlp2fn/utils/detectenv.py`

 * *Files identical despite different names*

### Comparing `nlp2fn-0.0.2/nlp2fn.egg-info/PKG-INFO` & `nlp2fn-0.0.3/nlp2fn.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: nlp2fn
-Version: 0.0.2
+Version: 0.0.3
 Summary: With the ability to load and read Python functions from any specified location, `nlp2fn` brings all your automation tasks together.
 Home-page: https://github.com/dextrop/nlp2fn
 Author: Jennie Developers <saurabh@ask-jennie.com>
 Author-email: Jennie Developers <saurabh@ask-jennie.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 
-# Python Automation Made Simple: nlp2fn
+# Python Automation Made Simple: [nlp2fn](https://pypi.org/project/nlp2fn/)
 
 Welcome to `nlp2fn`, a seamless and intuitive software tool for Python automation. With the ability to load and read Python functions from any specified location, `nlp2fn` brings all your automation tasks together. Whether your functions reside in local directories or remote servers, `nlp2fn` fetches, loads, and prepares them for execution — as simple as a statement.
 
+
 ## The Magic of nlp2fn
 
 A typical function for `nlp2fn` follows this format:
 
 ```python
 # Write you execute statement, this shall be an 
 # input by user to execute your events, make sure all the 
@@ -34,26 +35,35 @@
     return True
 ```
 
 The `execute` function is the heart of the operation where the actual task takes place.
 
 ## Quick Start Guide
 
-Here's how to install and get started with [`nlp2fn`]()f:
+Here's how to install and get started with [`nlp2fn`](https://pypi.org/project/nlp2fn/):
 
 ```bash
 pip install nlp2fn
 ```
 
 Next, add the source directory where your Python functions are located:
 
 ```bash
-nlp2fn set source /path/to/directory
+nlp2fn set-source local /path/to/directory
+```
+
+or 
+
+```bash
+nlp2fn set-source git https://github.com/{githubid}/{repo}
 ```
 
+make sure repo is public.
+
+
 Ready to launch `nlp2fn` as a chatbot? Use this command:
 
 ```bash
 nlp2fn run
 ```
 
 To run a single statement, use the `exec` command:
@@ -73,7 +83,12 @@
 We welcome your contributions! Feel free to submit pull requests and create issues on our [GitHub page](https://github.com/dextrop/nlp2fn/issues).
 
 ## Contact
 
 For questions, suggestions, or any kind of discussion, feel free to open an issue on our GitHub page.
 
 Embrace the simplification of Python automation with `nlp2fn`.
+
+## Events
+
+- Langchain Automations : https://github.com/dextrop/evt-langchain
+- https://medium.com/@askjennie/creating-your-own-automation-library-with-nlp2fn-6657b1276361
```

### Comparing `nlp2fn-0.0.2/setup.py` & `nlp2fn-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 __description__ = 'With the ability to load and read Python functions from any specified location, `nlp2fn` brings all your automation tasks together.'
 __author__ = 'Jennie Developers <saurabh@ask-jennie.com>'
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
```

