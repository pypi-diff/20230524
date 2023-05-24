# Comparing `tmp/Fletxible-0.5.3.tar.gz` & `tmp/Fletxible-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fletxible-0.5.3.tar", last modified: Sun May 21 13:05:38 2023, max compression
+gzip compressed data, was "Fletxible-0.5.4.tar", last modified: Wed May 24 15:03:39 2023, max compression
```

## Comparing `Fletxible-0.5.3.tar` & `Fletxible-0.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 13:05:38.173826 Fletxible-0.5.3/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 13:05:38.168952 Fletxible-0.5.3/Fletxible.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-21 13:05:38.000000 Fletxible-0.5.3/Fletxible.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)      429 2023-05-21 13:05:38.000000 Fletxible-0.5.3/Fletxible.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-21 13:05:38.000000 Fletxible-0.5.3/Fletxible.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       86 2023-05-21 13:05:38.000000 Fletxible-0.5.3/Fletxible.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       37 2023-05-21 13:05:38.000000 Fletxible-0.5.3/Fletxible.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        6 2023-05-21 13:05:38.000000 Fletxible-0.5.3/Fletxible.egg-info/top_level.txt
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 Fletxible-0.5.3/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-21 13:05:38.173585 Fletxible-0.5.3/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     4106 2023-05-01 16:06:19.000000 Fletxible-0.5.3/README.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 13:05:38.172292 Fletxible-0.5.3/logic/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-20 17:37:40.000000 Fletxible-0.5.3/logic/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2201 2023-05-21 12:36:22.000000 Fletxible-0.5.3/logic/build.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2251 2023-05-17 15:53:13.000000 Fletxible-0.5.3/logic/cli.py
--rw-r--r--   0 ahmad      (501) staff       (20)     7832 2023-05-21 08:03:38.000000 Fletxible-0.5.3/logic/controls.py
--rw-r--r--   0 ahmad      (501) staff       (20)      909 2023-05-21 12:43:58.000000 Fletxible-0.5.3/logic/main.py
--rw-r--r--   0 ahmad      (501) staff       (20)       95 2023-05-21 08:59:30.000000 Fletxible-0.5.3/logic/mapped.py
--rw-r--r--   0 ahmad      (501) staff       (20)      531 2023-05-21 10:41:00.000000 Fletxible-0.5.3/logic/route.py
--rw-r--r--   0 ahmad      (501) staff       (20)     6629 2023-05-21 08:58:38.000000 Fletxible-0.5.3/logic/script.py
--rw-r--r--   0 ahmad      (501) staff       (20)      908 2023-05-21 08:03:38.000000 Fletxible-0.5.3/logic/styles.py
--rw-r--r--   0 ahmad      (501) staff       (20)    12162 2023-05-21 08:59:39.000000 Fletxible-0.5.3/logic/utilities.py
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-21 13:05:38.173893 Fletxible-0.5.3/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)     1182 2023-05-21 13:05:32.000000 Fletxible-0.5.3/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-21 13:05:38.173000 Fletxible-0.5.3/tests/
--rw-r--r--   0 ahmad      (501) staff       (20)     1049 2023-05-21 07:43:28.000000 Fletxible-0.5.3/tests/test_controls.py
--rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-01 14:25:50.000000 Fletxible-0.5.3/tests/test_route.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-24 15:03:39.740515 Fletxible-0.5.4/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-24 15:03:39.735769 Fletxible-0.5.4/Fletxible.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-24 15:03:39.000000 Fletxible-0.5.4/Fletxible.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)      429 2023-05-24 15:03:39.000000 Fletxible-0.5.4/Fletxible.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-24 15:03:39.000000 Fletxible-0.5.4/Fletxible.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       86 2023-05-24 15:03:39.000000 Fletxible-0.5.4/Fletxible.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       37 2023-05-24 15:03:39.000000 Fletxible-0.5.4/Fletxible.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        6 2023-05-24 15:03:39.000000 Fletxible-0.5.4/Fletxible.egg-info/top_level.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 Fletxible-0.5.4/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-24 15:03:39.740275 Fletxible-0.5.4/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     4106 2023-05-01 16:06:19.000000 Fletxible-0.5.4/README.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-24 15:03:39.738899 Fletxible-0.5.4/logic/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-20 17:37:40.000000 Fletxible-0.5.4/logic/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2201 2023-05-21 12:36:22.000000 Fletxible-0.5.4/logic/build.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2251 2023-05-17 15:53:13.000000 Fletxible-0.5.4/logic/cli.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     7832 2023-05-21 08:03:38.000000 Fletxible-0.5.4/logic/controls.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1592 2023-05-23 19:03:08.000000 Fletxible-0.5.4/logic/main.py
+-rw-r--r--   0 ahmad      (501) staff       (20)       95 2023-05-21 08:59:30.000000 Fletxible-0.5.4/logic/mapped.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      563 2023-05-23 18:58:11.000000 Fletxible-0.5.4/logic/route.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     5011 2023-05-23 19:02:08.000000 Fletxible-0.5.4/logic/script.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      908 2023-05-21 08:03:38.000000 Fletxible-0.5.4/logic/styles.py
+-rw-r--r--   0 ahmad      (501) staff       (20)    12162 2023-05-21 08:59:39.000000 Fletxible-0.5.4/logic/utilities.py
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-24 15:03:39.740601 Fletxible-0.5.4/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)     1182 2023-05-24 15:03:31.000000 Fletxible-0.5.4/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-24 15:03:39.739653 Fletxible-0.5.4/tests/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1049 2023-05-21 07:43:28.000000 Fletxible-0.5.4/tests/test_controls.py
+-rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-01 14:25:50.000000 Fletxible-0.5.4/tests/test_route.py
```

### Comparing `Fletxible-0.5.3/Fletxible.egg-info/PKG-INFO` & `Fletxible-0.5.4/Fletxible.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.5.3
+Version: 0.5.4
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.5.3/LICENSE` & `Fletxible-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.3/PKG-INFO` & `Fletxible-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.5.3
+Version: 0.5.4
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.5.3/README.md` & `Fletxible-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.3/logic/build.py` & `Fletxible-0.5.4/logic/build.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.3/logic/cli.py` & `Fletxible-0.5.4/logic/cli.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.3/logic/controls.py` & `Fletxible-0.5.4/logic/controls.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.3/logic/route.py` & `Fletxible-0.5.4/logic/route.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from script import route_keys
+
+
 def route(e, route):
     current = -1
     index: int
 
     for view in e.page.views[:]:
         if view.route == route:
             index = e.page.views.index(view)
```

### Comparing `Fletxible-0.5.3/logic/script.py` & `Fletxible-0.5.4/logic/script.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-import os, importlib.util
+import os
 import yaml
-import pickle
 import flet as ft
 
 from utilities import (
     route_string_method,
     set_app_route_method,
     set_app_default_pages,
     navigation_example_method,
 )
 
-#
-route_keys: dict = {}
-
 
 def open_yaml_script() -> dict:
     # Load the YAML file
     with open("flet_config.yml", "r") as file:
         docs = yaml.safe_load(file)
 
     return docs
@@ -83,20 +79,14 @@
     # 2. Loop through navigation tree and append the file_list with the filepaths
     for page in docs["nav"]:
         for key in page:
             filename = f"{page[key]}"
             filepath = os.path.join("pages", filename)
             file_list.append(filepath)
 
-        filename = os.path.splitext(filename)[0]
-
-        route_keys["/" + filename] = importlib.util.spec_from_file_location(
-            filename, filepath
-        )
-
     # 3. Loop through the file_list and create the corresponding pages
     for filepath in file_list:
         method = set_app_default_pages()
         if not os.path.exists(filepath):
             with open(filepath, "w") as f:
                 f.write(f"{method}")
 
@@ -128,35 +118,16 @@
 
             with open(f"./pages/{file}", "w") as f:
                 f.write(modified_string)
 
         else:
             pass
 
-    # 5. The route.pickle file is a binary file!
-    with open("./logic/route.pickle", "wb") as f:
-        pickle.dump(route_keys, f)
-
-    # 6. Finally, return the route_keys so we use itin the route.py logic
-    return route_keys
-
 
-def map_yaml(yaml_file_path, output_file_path):
-    # 1. open the flet_config.yml file and safe load the data
-    with open(yaml_file_path) as f:
-        yaml_data = yaml.safe_load(f)
-
-    # 2. Simply write the contents to a variable that will show up in the set location
-    # with the set filename: mapped.py
-    with open(output_file_path, "w") as f:
-        f.write("mapped_data = ")
-        f.write(str(yaml_data))
-
-
-def script(page: ft.Page):
+def script():
     # Get the YAML file
     try:
         docs = open_yaml_script()
 
     except FileNotFoundError as e:
         print(e)
 
@@ -186,31 +157,7 @@
     # which contains the application routing logic
     try:
         # Make sure to create a function that returns a list of the modules for routing!!!
         set_application_routing_script(docs)
 
     except Exception as e:
         print(e)
-
-    # Next, we have to handle the page logic, which requires
-    # several step. First, adding the default method into each page
-    try:
-        route_keys: dict = set_default_methods_script(docs)
-
-        for keys, __ in route_keys.items():
-            page.views.append(route_keys[keys].loader.load_module().View())
-
-        # Set's the index.py page as the first page.
-        index = -1
-        current = 1
-        page.views[index], page.views[current] = page.views[current], page.views[index]
-        page.update()
-
-    except Exception as e:
-        print(e)
-
-    # Map out the .yml file into a python dict
-    try:
-        map_yaml("flet_config.yml", "./logic/mapped.py")
-
-    except Exception as e:
-        print(e)
```

### Comparing `Fletxible-0.5.3/logic/styles.py` & `Fletxible-0.5.4/logic/styles.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.3/logic/utilities.py` & `Fletxible-0.5.4/logic/utilities.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.3/setup.py` & `Fletxible-0.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="Fletxible",
-    version="0.5.3",
+    version="0.5.4",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Web Boilerplate for Flet Library",
     long_description="Fletxible is a Python web boilerplate project designed to provide a solid foundation for building web applications with Python and Flet. The project comes pre-configured with a range of tools and features to make it easy for developers to get started building their applications, without the need to spend time setting up infrastructure or configuring tools.",
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/fletxible",
     packages=["logic"],
```

### Comparing `Fletxible-0.5.3/tests/test_controls.py` & `Fletxible-0.5.4/tests/test_controls.py`

 * *Files identical despite different names*

