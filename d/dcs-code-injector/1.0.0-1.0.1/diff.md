# Comparing `tmp/dcs-code-injector-1.0.0.tar.gz` & `tmp/dcs-code-injector-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcs-code-injector-1.0.0.tar", last modified: Wed May 24 07:43:36 2023, max compression
+gzip compressed data, was "dcs-code-injector-1.0.1.tar", last modified: Wed May 24 07:50:48 2023, max compression
```

## Comparing `dcs-code-injector-1.0.0.tar` & `dcs-code-injector-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:43:36.836287 dcs-code-injector-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 07:43:22.000000 dcs-code-injector-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-24 07:43:36.832287 dcs-code-injector-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-24 07:43:22.000000 dcs-code-injector-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:43:36.832287 dcs-code-injector-1.0.0/dcs_code_injector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:43:22.000000 dcs-code-injector-1.0.0/dcs_code_injector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-24 07:43:22.000000 dcs-code-injector-1.0.0/dcs_code_injector/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-05-24 07:43:22.000000 dcs-code-injector-1.0.0/dcs_code_injector/dcs_code_injector_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-24 07:43:22.000000 dcs-code-injector-1.0.0/dcs_code_injector/log_highlighter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-24 07:43:22.000000 dcs-code-injector-1.0.0/dcs_code_injector/lua_syntax_highlighter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-24 07:43:22.000000 dcs-code-injector-1.0.0/dcs_code_injector/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-24 07:43:22.000000 dcs-code-injector-1.0.0/dcs_code_injector/settings_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:43:36.832287 dcs-code-injector-1.0.0/dcs_code_injector/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:43:22.000000 dcs-code-injector-1.0.0/dcs_code_injector/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-24 07:43:22.000000 dcs-code-injector-1.0.0/dcs_code_injector/ui/dcs_code_injector_settings_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-24 07:43:22.000000 dcs-code-injector-1.0.0/dcs_code_injector/ui/dcs_code_injector_window_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-24 07:43:22.000000 dcs-code-injector-1.0.0/dcs_code_injector/variables_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:43:36.832287 dcs-code-injector-1.0.0/dcs_code_injector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-24 07:43:36.000000 dcs-code-injector-1.0.0/dcs_code_injector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-24 07:43:36.000000 dcs-code-injector-1.0.0/dcs_code_injector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 07:43:36.000000 dcs-code-injector-1.0.0/dcs_code_injector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-24 07:43:36.000000 dcs-code-injector-1.0.0/dcs_code_injector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-24 07:43:36.000000 dcs-code-injector-1.0.0/dcs_code_injector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 07:43:36.000000 dcs-code-injector-1.0.0/dcs_code_injector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 07:43:36.836287 dcs-code-injector-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-24 07:43:22.000000 dcs-code-injector-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:50:48.825496 dcs-code-injector-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-24 07:50:48.825496 dcs-code-injector-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:50:48.817495 dcs-code-injector-1.0.1/dcs_code_injector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/dcs_code_injector_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/log_highlighter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/lua_syntax_highlighter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/settings_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:50:48.817495 dcs-code-injector-1.0.1/dcs_code_injector/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/dcs_code_injector_settings_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/dcs_code_injector_window_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:50:48.817495 dcs-code-injector-1.0.1/dcs_code_injector/ui/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/icons/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:50:48.821496 dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   629069 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/splash_01.png
+-rw-r--r--   0 runner    (1001) docker     (123)   831944 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/splash_02.png
+-rw-r--r--   0 runner    (1001) docker     (123)   927761 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/splash_03.png
+-rw-r--r--   0 runner    (1001) docker     (123)   932507 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/splash_04.png
+-rw-r--r--   0 runner    (1001) docker     (123)   723796 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/splash_05.png
+-rw-r--r--   0 runner    (1001) docker     (123)   916284 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/splash_06.png
+-rw-r--r--   0 runner    (1001) docker     (123)   968922 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/ui/splashscreens/splash_07.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/dcs_code_injector/variables_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:50:48.817495 dcs-code-injector-1.0.1/dcs_code_injector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-24 07:50:48.000000 dcs-code-injector-1.0.1/dcs_code_injector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-24 07:50:48.000000 dcs-code-injector-1.0.1/dcs_code_injector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 07:50:48.000000 dcs-code-injector-1.0.1/dcs_code_injector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-24 07:50:48.000000 dcs-code-injector-1.0.1/dcs_code_injector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-24 07:50:48.000000 dcs-code-injector-1.0.1/dcs_code_injector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 07:50:48.000000 dcs-code-injector-1.0.1/dcs_code_injector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 07:50:48.825496 dcs-code-injector-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-24 07:50:37.000000 dcs-code-injector-1.0.1/setup.py
```

### Comparing `dcs-code-injector-1.0.0/LICENSE` & `dcs-code-injector-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.0/dcs_code_injector/app.py` & `dcs-code-injector-1.0.1/dcs_code_injector/app.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.0/dcs_code_injector/dcs_code_injector_window.py` & `dcs-code-injector-1.0.1/dcs_code_injector/dcs_code_injector_window.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.0/dcs_code_injector/log_highlighter.py` & `dcs-code-injector-1.0.1/dcs_code_injector/log_highlighter.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.0/dcs_code_injector/lua_syntax_highlighter.py` & `dcs-code-injector-1.0.1/dcs_code_injector/lua_syntax_highlighter.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.0/dcs_code_injector/server.py` & `dcs-code-injector-1.0.1/dcs_code_injector/server.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.0/dcs_code_injector/settings_dialog.py` & `dcs-code-injector-1.0.1/dcs_code_injector/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.0/dcs_code_injector/ui/dcs_code_injector_settings_ui.py` & `dcs-code-injector-1.0.1/dcs_code_injector/ui/dcs_code_injector_settings_ui.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.0/dcs_code_injector/ui/dcs_code_injector_window_ui.py` & `dcs-code-injector-1.0.1/dcs_code_injector/ui/dcs_code_injector_window_ui.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.0/dcs_code_injector/variables_tree.py` & `dcs-code-injector-1.0.1/dcs_code_injector/variables_tree.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.0.0/setup.py` & `dcs-code-injector-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 data_files_to_include = ["*.png", "*.jpg"]
 
 setup(
     name='dcs-code-injector',
-    version='1.0.0',
+    version='1.0.1',
     packages=find_packages(),
     package_data={
         "": data_files_to_include,
     },
     url='https://www.github.com/nielsvaes/dcs_code_injector',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

