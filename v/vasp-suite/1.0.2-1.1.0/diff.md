# Comparing `tmp/vasp_suite-1.0.2.tar.gz` & `tmp/vasp_suite-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vasp_suite-1.0.2.tar", last modified: Wed May 24 09:30:05 2023, max compression
+gzip compressed data, was "vasp_suite-1.1.0.tar", last modified: Wed May 24 09:39:08 2023, max compression
```

## Comparing `vasp_suite-1.0.2.tar` & `vasp_suite-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:30:05.293350 vasp_suite-1.0.2/
--rw-rw-rw-   0 root         (0) root         (0)    35079 2023-05-24 09:29:51.000000 vasp_suite-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3381 2023-05-24 09:30:05.292350 vasp_suite-1.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2933 2023-05-24 09:29:51.000000 vasp_suite-1.0.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-05-24 09:29:51.000000 vasp_suite-1.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 09:30:05.293350 vasp_suite-1.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1371 2023-05-24 09:30:02.000000 vasp_suite-1.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:30:05.291350 vasp_suite-1.0.2/vasp_suite/
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-05-24 09:29:51.000000 vasp_suite-1.0.2/vasp_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-05-24 09:30:02.000000 vasp_suite-1.0.2/vasp_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    10765 2023-05-24 09:29:51.000000 vasp_suite-1.0.2/vasp_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     3461 2023-05-24 09:29:51.000000 vasp_suite-1.0.2/vasp_suite/core.py
--rw-rw-rw-   0 root         (0) root         (0)    16932 2023-05-24 09:29:51.000000 vasp_suite-1.0.2/vasp_suite/ewald.py
--rw-rw-rw-   0 root         (0) root         (0)     2689 2023-05-24 09:29:51.000000 vasp_suite-1.0.2/vasp_suite/input.py
--rw-rw-rw-   0 root         (0) root         (0)    16913 2023-05-24 09:29:51.000000 vasp_suite-1.0.2/vasp_suite/structure.py
--rw-rw-rw-   0 root         (0) root         (0)     1711 2023-05-24 09:29:51.000000 vasp_suite-1.0.2/vasp_suite/submission.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:30:05.292350 vasp_suite-1.0.2/vasp_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3381 2023-05-24 09:30:05.000000 vasp_suite-1.0.2/vasp_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      422 2023-05-24 09:30:05.000000 vasp_suite-1.0.2/vasp_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 09:30:05.000000 vasp_suite-1.0.2/vasp_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-05-24 09:30:05.000000 vasp_suite-1.0.2/vasp_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-24 09:30:05.000000 vasp_suite-1.0.2/vasp_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-24 09:30:05.000000 vasp_suite-1.0.2/vasp_suite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:39:08.904469 vasp_suite-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35079 2023-05-24 09:38:55.000000 vasp_suite-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-05-24 09:39:08.904469 vasp_suite-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2933 2023-05-24 09:38:55.000000 vasp_suite-1.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-05-24 09:38:55.000000 vasp_suite-1.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 09:39:08.904469 vasp_suite-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2023-05-24 09:39:06.000000 vasp_suite-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:39:08.902469 vasp_suite-1.1.0/vasp_suite/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-05-24 09:38:55.000000 vasp_suite-1.1.0/vasp_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-05-24 09:39:06.000000 vasp_suite-1.1.0/vasp_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10765 2023-05-24 09:38:55.000000 vasp_suite-1.1.0/vasp_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     3461 2023-05-24 09:38:55.000000 vasp_suite-1.1.0/vasp_suite/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    16932 2023-05-24 09:38:55.000000 vasp_suite-1.1.0/vasp_suite/ewald.py
+-rw-rw-rw-   0 root         (0) root         (0)     2690 2023-05-24 09:38:55.000000 vasp_suite-1.1.0/vasp_suite/input.py
+-rw-rw-rw-   0 root         (0) root         (0)    16913 2023-05-24 09:38:55.000000 vasp_suite-1.1.0/vasp_suite/structure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1711 2023-05-24 09:38:55.000000 vasp_suite-1.1.0/vasp_suite/submission.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:39:08.903469 vasp_suite-1.1.0/vasp_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-05-24 09:39:08.000000 vasp_suite-1.1.0/vasp_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      422 2023-05-24 09:39:08.000000 vasp_suite-1.1.0/vasp_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 09:39:08.000000 vasp_suite-1.1.0/vasp_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-05-24 09:39:08.000000 vasp_suite-1.1.0/vasp_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-24 09:39:08.000000 vasp_suite-1.1.0/vasp_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-24 09:39:08.000000 vasp_suite-1.1.0/vasp_suite.egg-info/top_level.txt
```

### Comparing `vasp_suite-1.0.2/LICENSE` & `vasp_suite-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.0.2/PKG-INFO` & `vasp_suite-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasp_suite
-Version: 1.0.2
+Version: 1.1.0
 Summary: A package for creating and handling input files for vasp
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `vasp_suite-1.0.2/README.md` & `vasp_suite-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.0.2/setup.py` & `vasp_suite-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 # pylint: disable=line-too-long,missing-module-docstring,exec-used
 import setuptools
 
 # DO NOT EDIT THIS NUMBER!
 # It is changed automatically by python-semantic-release
-__version__ = "1.0.2"
+__version__ = "1.1.0"
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
     name='vasp_suite',
     version=__version__,
```

### Comparing `vasp_suite-1.0.2/vasp_suite/cli.py` & `vasp_suite-1.1.0/vasp_suite/cli.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.0.2/vasp_suite/core.py` & `vasp_suite-1.1.0/vasp_suite/core.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.0.2/vasp_suite/ewald.py` & `vasp_suite-1.1.0/vasp_suite/ewald.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.0.2/vasp_suite/input.py` & `vasp_suite-1.1.0/vasp_suite/input.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     InputFileGenerator is a class which generates input files for VASP calculations.
     '''
     def __init__(self, filename: str, calculation: str):
         '''
         Initializes the class.
         '''
         self._s = Structure(filename)
-        self._calculation = calculation
+        self.configuration = calculation
         hostname = socket.gethostname()
         if 'csf3' in hostname: 
             self.pseudopotentials = '/opt/apps/apps/intel-19.1/vasp/5.4.4/pseudopotentials/potpaw_PBE.54'
             self.module = 'apps/intel-19.1/vasp/5.4.4'
         elif 'csf4' in hostname: 
             self.pseudopotentials = '/opt/software/RI/apps/VASP/5.4.4-iomkl-2020.02/pseudopotentials/potpaw_PBE.54'
             self.module = 'VASP/5.4.4-iomkl-2020.02'
```

### Comparing `vasp_suite-1.0.2/vasp_suite/structure.py` & `vasp_suite-1.1.0/vasp_suite/structure.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.0.2/vasp_suite/submission.py` & `vasp_suite-1.1.0/vasp_suite/submission.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.0.2/vasp_suite.egg-info/PKG-INFO` & `vasp_suite-1.1.0/vasp_suite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasp-suite
-Version: 1.0.2
+Version: 1.1.0
 Summary: A package for creating and handling input files for vasp
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

