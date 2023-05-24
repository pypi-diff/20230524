# Comparing `tmp/bdata-6.8.3.tar.gz` & `tmp/bdata-6.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdata-6.8.3.tar", last modified: Tue Jul 26 22:32:00 2022, max compression
+gzip compressed data, was "bdata-6.9.0.tar", last modified: Mon Oct 31 08:05:13 2022, max compression
```

## Comparing `bdata-6.8.3.tar` & `bdata-6.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2022-07-26 22:32:00.104811 bdata-6.8.3/
--rw-rw-r--   0 fuji      (1000) fuji      (1000)    35149 2019-11-12 04:27:37.000000 bdata-6.8.3/LICENSE
--rw-rw-r--   0 fuji      (1000) fuji      (1000)       76 2018-07-24 22:25:32.000000 bdata-6.8.3/MANIFEST.in
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     6634 2022-07-26 22:32:00.104811 bdata-6.8.3/PKG-INFO
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     5893 2021-11-02 19:51:46.000000 bdata-6.8.3/README.md
-drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2022-07-26 22:32:00.104811 bdata-6.8.3/bdata/
--rw-rw-r--   0 fuji      (1000) fuji      (1000)      490 2022-01-25 22:24:33.000000 bdata-6.8.3/bdata/__init__.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)   104431 2021-11-02 18:22:36.000000 bdata-6.8.3/bdata/bdata.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)    11238 2021-08-09 01:00:59.000000 bdata-6.8.3/bdata/bjoined.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)    12044 2022-07-26 21:38:12.000000 bdata-6.8.3/bdata/bmerged.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     3206 2022-07-26 17:11:12.000000 bdata-6.8.3/bdata/calc.py
--rw-r--r--   0 fuji      (1000) fuji      (1000)     1073 2021-11-02 18:56:14.000000 bdata-6.8.3/bdata/containers.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)      236 2021-04-08 20:28:14.000000 bdata-6.8.3/bdata/exceptions.py
--rw-r--r--   0 fuji      (1000) fuji      (1000)     2132 2021-03-11 22:30:24.000000 bdata-6.8.3/bdata/life.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)       36 2022-07-26 22:31:06.000000 bdata-6.8.3/bdata/version.py
-drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2022-07-26 22:32:00.104811 bdata-6.8.3/bdata.egg-info/
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     6634 2022-07-26 22:31:59.000000 bdata-6.8.3/bdata.egg-info/PKG-INFO
--rw-rw-r--   0 fuji      (1000) fuji      (1000)      334 2022-07-26 22:31:59.000000 bdata-6.8.3/bdata.egg-info/SOURCES.txt
--rw-rw-r--   0 fuji      (1000) fuji      (1000)        1 2022-07-26 22:31:59.000000 bdata-6.8.3/bdata.egg-info/dependency_links.txt
--rw-rw-r--   0 fuji      (1000) fuji      (1000)       84 2022-07-26 22:31:59.000000 bdata-6.8.3/bdata.egg-info/requires.txt
--rw-rw-r--   0 fuji      (1000) fuji      (1000)        6 2022-07-26 22:31:59.000000 bdata-6.8.3/bdata.egg-info/top_level.txt
--rw-rw-r--   0 fuji      (1000) fuji      (1000)       38 2022-07-26 22:32:00.104811 bdata-6.8.3/setup.cfg
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     1363 2022-07-26 22:30:57.000000 bdata-6.8.3/setup.py
+drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2022-10-31 08:05:13.713405 bdata-6.9.0/
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)    35149 2022-01-26 20:26:35.000000 bdata-6.9.0/LICENSE
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       76 2022-01-26 20:26:35.000000 bdata-6.9.0/MANIFEST.in
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     6634 2022-10-31 08:05:13.713405 bdata-6.9.0/PKG-INFO
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     5893 2022-01-26 20:26:35.000000 bdata-6.9.0/README.md
+drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2022-10-31 08:05:13.713405 bdata-6.9.0/bdata/
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)      490 2022-01-26 20:26:35.000000 bdata-6.9.0/bdata/__init__.py
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)   105426 2022-10-31 08:02:50.000000 bdata-6.9.0/bdata/bdata.py
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)    11238 2022-01-26 20:26:35.000000 bdata-6.9.0/bdata/bjoined.py
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)    12044 2022-10-31 08:04:22.000000 bdata-6.9.0/bdata/bmerged.py
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     3206 2022-01-26 21:39:22.000000 bdata-6.9.0/bdata/calc.py
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     1073 2022-01-26 20:26:35.000000 bdata-6.9.0/bdata/containers.py
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)      236 2022-01-26 20:26:35.000000 bdata-6.9.0/bdata/exceptions.py
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     2132 2022-01-26 20:26:35.000000 bdata-6.9.0/bdata/life.py
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       36 2022-10-31 08:04:36.000000 bdata-6.9.0/bdata/version.py
+drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2022-10-31 08:05:13.713405 bdata-6.9.0/bdata.egg-info/
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     6634 2022-10-31 08:05:13.000000 bdata-6.9.0/bdata.egg-info/PKG-INFO
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)      334 2022-10-31 08:05:13.000000 bdata-6.9.0/bdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)        1 2022-10-31 08:05:13.000000 bdata-6.9.0/bdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       84 2022-10-31 08:05:13.000000 bdata-6.9.0/bdata.egg-info/requires.txt
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)        6 2022-10-31 08:05:13.000000 bdata-6.9.0/bdata.egg-info/top_level.txt
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       38 2022-10-31 08:05:13.713405 bdata-6.9.0/setup.cfg
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     1363 2022-10-31 08:04:22.000000 bdata-6.9.0/setup.py
```

### Comparing `bdata-6.8.3/LICENSE` & `bdata-6.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bdata-6.8.3/PKG-INFO` & `bdata-6.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdata
-Version: 6.8.3
+Version: 6.9.0
 Summary: β-NMR/β-NQR MUD file reader and asymmetry calculator
 Home-page: https://github.com/dfujim/bdata
 Author: Derek Fujimoto
 Author-email: fujimoto@phas.ubc.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bdata Version: 6.8.3 Summary: Î²-NMR/Î²-NQR MUD
+Metadata-Version: 2.1 Name: bdata Version: 6.9.0 Summary: Î²-NMR/Î²-NQR MUD
 file reader and asymmetry calculator Home-page: https://github.com/dfujim/bdata
 Author: Derek Fujimoto Author-email: fujimoto@phas.ubc.ca License: UNKNOWN
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: MacOS Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `bdata-6.8.3/README.md` & `bdata-6.9.0/README.md`

 * *Files identical despite different names*

### Comparing `bdata-6.8.3/bdata/bdata.py` & `bdata-6.9.0/bdata/bdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -679,14 +679,39 @@
         
         # Fix inconsistent area for old runs
         if self.area == 'ISAC':
             if self.run >= 45000:   self.area = 'BNQR'
             else:                   self.area = 'BNMR'
     
     # ======================================================================= #
+    def __add__(self, other):
+        """
+            Return a bmerged object if adding to another bdata object
+        """    
+        if type(other) is bd.bdata or type(other) is bd.bmerged: 
+            return bd.bmerged([self, other])
+    
+    # ======================================================================= #
+    def __iadd__(self, other):
+        """
+            Return a bmerged object if adding to another bdata object
+        """    
+        if type(other) is bd.bdata or type(other) is bd.bmerged: 
+            self = bd.bmerged([self, other])
+            return self
+    
+    # ======================================================================= #
+    def __radd__(self, other):      
+        """
+            Return a bmerged object if adding to another bdata object
+        """ 
+        if type(other) is bd.bdata or type(other) is bd.bmerged: 
+            return self.__add__(other)
+    
+    # ======================================================================= #
     def __getattr__(self, name):
         
         if name in ('hist', 'camp', 'ppg', 'epics'):
             return getattr(object, name)
         
         else:
```

### Comparing `bdata-6.8.3/bdata/bjoined.py` & `bdata-6.9.0/bdata/bjoined.py`

 * *Files identical despite different names*

### Comparing `bdata-6.8.3/bdata/bmerged.py` & `bdata-6.9.0/bdata/bmerged.py`

 * *Files identical despite different names*

### Comparing `bdata-6.8.3/bdata/calc.py` & `bdata-6.9.0/bdata/calc.py`

 * *Files identical despite different names*

### Comparing `bdata-6.8.3/bdata/containers.py` & `bdata-6.9.0/bdata/containers.py`

 * *Files identical despite different names*

### Comparing `bdata-6.8.3/bdata/life.py` & `bdata-6.9.0/bdata/life.py`

 * *Files identical despite different names*

### Comparing `bdata-6.8.3/bdata.egg-info/PKG-INFO` & `bdata-6.9.0/bdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdata
-Version: 6.8.3
+Version: 6.9.0
 Summary: β-NMR/β-NQR MUD file reader and asymmetry calculator
 Home-page: https://github.com/dfujim/bdata
 Author: Derek Fujimoto
 Author-email: fujimoto@phas.ubc.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bdata Version: 6.8.3 Summary: Î²-NMR/Î²-NQR MUD
+Metadata-Version: 2.1 Name: bdata Version: 6.9.0 Summary: Î²-NMR/Î²-NQR MUD
 file reader and asymmetry calculator Home-page: https://github.com/dfujim/bdata
 Author: Derek Fujimoto Author-email: fujimoto@phas.ubc.ca License: UNKNOWN
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: MacOS Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `bdata-6.8.3/setup.py` & `bdata-6.9.0/setup.py`

 * *Files identical despite different names*

