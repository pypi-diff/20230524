# Comparing `tmp/mlx.robot2rst-3.2.1.tar.gz` & `tmp/mlx.robot2rst-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mlx.robot2rst-3.2.1.tar", last modified: Thu Apr 27 08:54:31 2023, max compression
+gzip compressed data, was "dist/mlx.robot2rst-3.3.0.tar", last modified: Wed May 24 07:26:08 2023, max compression
```

## Comparing `mlx.robot2rst-3.2.1.tar` & `mlx.robot2rst-3.3.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/doc/source/example.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/doc/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/doc/source/requirements.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/doc/source/robot/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/doc/source/robot/example.robot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/mlx/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/mlx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/mlx/robot2rst.mako
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/mlx/robot2rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/mlx/robot_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/mlx.robot2rst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/mlx.robot2rst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/mlx.robot2rst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/mlx.robot2rst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/mlx.robot2rst.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/mlx.robot2rst.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/mlx.robot2rst.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/mlx.robot2rst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/mlx.robot2rst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-27 08:54:31.000000 mlx.robot2rst-3.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-27 08:54:10.000000 mlx.robot2rst-3.2.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:26:08.000000 mlx.robot2rst-3.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:26:08.000000 mlx.robot2rst-3.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:26:08.000000 mlx.robot2rst-3.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-24 07:25:47.000000 mlx.robot2rst-3.3.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-24 07:25:47.000000 mlx.robot2rst-3.3.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-24 07:25:47.000000 mlx.robot2rst-3.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 07:25:47.000000 mlx.robot2rst-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-24 07:25:47.000000 mlx.robot2rst-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-24 07:26:08.000000 mlx.robot2rst-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-24 07:25:47.000000 mlx.robot2rst-3.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 07:25:47.000000 mlx.robot2rst-3.3.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:26:08.000000 mlx.robot2rst-3.3.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-24 07:25:47.000000 mlx.robot2rst-3.3.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:26:08.000000 mlx.robot2rst-3.3.0/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-24 07:25:47.000000 mlx.robot2rst-3.3.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-24 07:25:47.000000 mlx.robot2rst-3.3.0/doc/source/example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-24 07:25:47.000000 mlx.robot2rst-3.3.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-24 07:25:47.000000 mlx.robot2rst-3.3.0/doc/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-24 07:25:47.000000 mlx.robot2rst-3.3.0/doc/source/requirements.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:26:08.000000 mlx.robot2rst-3.3.0/doc/source/robot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-24 07:25:47.000000 mlx.robot2rst-3.3.0/doc/source/robot/example.robot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:26:08.000000 mlx.robot2rst-3.3.0/mlx/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-24 07:25:47.000000 mlx.robot2rst-3.3.0/mlx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-24 07:25:47.000000 mlx.robot2rst-3.3.0/mlx/robot2rst.mako
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-05-24 07:25:47.000000 mlx.robot2rst-3.3.0/mlx/robot2rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-24 07:25:47.000000 mlx.robot2rst-3.3.0/mlx/robot_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:26:08.000000 mlx.robot2rst-3.3.0/mlx.robot2rst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-24 07:26:08.000000 mlx.robot2rst-3.3.0/mlx.robot2rst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-24 07:26:08.000000 mlx.robot2rst-3.3.0/mlx.robot2rst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 07:26:08.000000 mlx.robot2rst-3.3.0/mlx.robot2rst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-24 07:26:08.000000 mlx.robot2rst-3.3.0/mlx.robot2rst.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-24 07:26:08.000000 mlx.robot2rst-3.3.0/mlx.robot2rst.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 07:26:08.000000 mlx.robot2rst-3.3.0/mlx.robot2rst.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-24 07:26:08.000000 mlx.robot2rst-3.3.0/mlx.robot2rst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-24 07:26:08.000000 mlx.robot2rst-3.3.0/mlx.robot2rst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-24 07:25:47.000000 mlx.robot2rst-3.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-24 07:26:08.000000 mlx.robot2rst-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-24 07:25:47.000000 mlx.robot2rst-3.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-24 07:25:47.000000 mlx.robot2rst-3.3.0/tox.ini
```

### Comparing `mlx.robot2rst-3.2.1/.github/workflows/codeql-analysis.yml` & `mlx.robot2rst-3.3.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.2.1/.github/workflows/python-package.yml` & `mlx.robot2rst-3.3.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.2.1/.gitignore` & `mlx.robot2rst-3.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.2.1/LICENSE` & `mlx.robot2rst-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.2.1/PKG-INFO` & `mlx.robot2rst-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx.robot2rst
-Version: 3.2.1
+Version: 3.3.0
 Summary: Python script for converting a Robot Framework file to a reStructuredText (.rst) file
 Home-page: https://github.com/melexis/robot2rst
 Author: Jasper Craeghs
 Author-email: jce@melexis.com
 License: Apache License Version 2.0
 Description: .. image:: https://github.com/melexis/robot2rst/actions/workflows/python-package.yml/badge.svg?branch=master
             :target: https://github.com/melexis/robot2rst/actions/workflows/python-package.yml
```

### Comparing `mlx.robot2rst-3.2.1/README.rst` & `mlx.robot2rst-3.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.2.1/doc/Makefile` & `mlx.robot2rst-3.3.0/doc/Makefile`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 SPHINXBUILD   ?= sphinx-build
 SOURCEDIR     = source
 BUILDDIR      = _build
 ROBOT2RST	  = robot2rst
 ROBOT2RST_OPTS += -i $(SOURCEDIR)/robot/example.robot
 ROBOT2RST_OPTS += -o $(SOURCEDIR)/example_usage_qtp.rst
 ROBOT2RST_OPTS += -t ^SWRQT- ^SYSRQT-
-ROBOT2RST_OPTS += -c 100 50.0
+ROBOT2RST_OPTS += -c 100 40.0
 ROBOT2RST_OPTS += -r validates ext_toolname
 ROBOT2RST_OPTS += --only FLASH
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `mlx.robot2rst-3.2.1/doc/source/conf.py` & `mlx.robot2rst-3.3.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.2.1/doc/source/robot/example.robot` & `mlx.robot2rst-3.3.0/doc/source/robot/example.robot`

 * *Files 15% similar despite different names*

```diff
@@ -33,12 +33,16 @@
 Another Test
     [Documentation]
     ...  Test case with for-loop.
     [Tags]              RQT-SOME_RQT  SYSRQT-SOME_SYSTEM_RQT
                         FOR     ${var}  IN  @{NAMES}
                                 Log     ${var}
 
+Comp1: testing 'Special" characters & prefix (with brackets)
+    [Documentation]     The item ID will contain COMP1-TESTING_SPECIAL_CHARACTERS_AND_PREFIX_WITH_BRACKETS.
+                        Log     Special characters in test case names are supported but not recommended.
+
 *** Keywords ***
 My Keyword
     [Documentation]     My keyword's documentation string.
     [Arguments]         ${path}
                         Directory Should Exist    ${path}
```

### Comparing `mlx.robot2rst-3.2.1/mlx/robot2rst.mako` & `mlx.robot2rst-3.3.0/mlx/robot2rst.mako`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,20 @@
     Returns:
         str: The name of the traceable item name of the given anything
     '''
     # Apply prefix
     name = prefix + name
     # Move to capitals
     name = name.upper()
-    # Move ' : ' (or alike) to '-'
+    # Replace ' : ' (or alike) by '-'
     name = re.sub('\s*:\s*', '-', name)
+    # Replace '&' by 'AND'
+    name = name.replace('&', 'AND')
+    # Remove other special characters
+    name = re.sub('[^\w\s_-]', '', name)
     # Replace spaces with single underscore
     name = re.sub('\s+', '_', name)
     return name
 
 
 def generate_body(input_string):
     ''' Generates the body of the item based on the raw docstring of the robot test case.
```

### Comparing `mlx.robot2rst-3.2.1/mlx/robot2rst.py` & `mlx.robot2rst-3.3.0/mlx/robot2rst.py`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.2.1/mlx/robot_parser.py` & `mlx.robot2rst-3.3.0/mlx/robot_parser.py`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.2.1/mlx.robot2rst.egg-info/PKG-INFO` & `mlx.robot2rst-3.3.0/mlx.robot2rst.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx.robot2rst
-Version: 3.2.1
+Version: 3.3.0
 Summary: Python script for converting a Robot Framework file to a reStructuredText (.rst) file
 Home-page: https://github.com/melexis/robot2rst
 Author: Jasper Craeghs
 Author-email: jce@melexis.com
 License: Apache License Version 2.0
 Description: .. image:: https://github.com/melexis/robot2rst/actions/workflows/python-package.yml/badge.svg?branch=master
             :target: https://github.com/melexis/robot2rst/actions/workflows/python-package.yml
```

### Comparing `mlx.robot2rst-3.2.1/mlx.robot2rst.egg-info/SOURCES.txt` & `mlx.robot2rst-3.3.0/mlx.robot2rst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.2.1/setup.py` & `mlx.robot2rst-3.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.2.1/tox.ini` & `mlx.robot2rst-3.3.0/tox.ini`

 * *Files identical despite different names*

