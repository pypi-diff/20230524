# Comparing `tmp/mud-py-1.2.8.tar.gz` & `tmp/mud-py-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mud-py-1.2.8.tar", last modified: Sat Sep  4 19:40:47 2021, max compression
+gzip compressed data, was "mud-py-1.2.9.tar", last modified: Tue Jul 26 22:30:18 2022, max compression
```

## Comparing `mud-py-1.2.8.tar` & `mud-py-1.2.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2021-09-04 19:40:47.656133 mud-py-1.2.8/
--rw-rw-r--   0 fuji      (1000) fuji      (1000)    35149 2019-11-12 04:27:37.000000 mud-py-1.2.8/LICENSE
--rw-rw-r--   0 fuji      (1000) fuji      (1000)       91 2021-08-26 20:20:29.000000 mud-py-1.2.8/MANIFEST.in
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     5460 2021-09-04 19:40:47.656133 mud-py-1.2.8/PKG-INFO
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     4708 2021-09-03 18:53:40.000000 mud-py-1.2.8/README.md
-drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2021-09-04 19:40:47.584132 mud-py-1.2.8/mud_py.egg-info/
--rw-r--r--   0 fuji      (1000) fuji      (1000)     5460 2021-09-04 19:40:47.000000 mud-py-1.2.8/mud_py.egg-info/PKG-INFO
--rw-r--r--   0 fuji      (1000) fuji      (1000)     1221 2021-09-04 19:40:47.000000 mud-py-1.2.8/mud_py.egg-info/SOURCES.txt
--rw-r--r--   0 fuji      (1000) fuji      (1000)        1 2021-09-04 19:40:47.000000 mud-py-1.2.8/mud_py.egg-info/dependency_links.txt
--rw-r--r--   0 fuji      (1000) fuji      (1000)       37 2021-09-04 19:40:47.000000 mud-py-1.2.8/mud_py.egg-info/requires.txt
--rw-r--r--   0 fuji      (1000) fuji      (1000)        6 2021-09-04 19:40:47.000000 mud-py-1.2.8/mud_py.egg-info/top_level.txt
-drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2021-09-04 19:40:47.584132 mud-py-1.2.8/mud_src/
--rw-rw-r--   0 fuji      (1000) fuji      (1000)    21832 2021-08-28 20:55:40.000000 mud-py-1.2.8/mud_src/mud.c
--rw-rw-r--   0 fuji      (1000) fuji      (1000)    27875 2021-09-03 18:53:40.000000 mud-py-1.2.8/mud_src/mud.h
--rw-r--r--   0 fuji      (1000) fuji      (1000)     6853 2019-08-15 04:24:31.000000 mud-py-1.2.8/mud_src/mud_all.c
--rw-r--r--   0 fuji      (1000) fuji      (1000)    10305 2019-07-25 07:31:42.000000 mud-py-1.2.8/mud_src/mud_encode.c
--rw-rw-r--   0 fuji      (1000) fuji      (1000)    47224 2021-08-26 19:27:17.000000 mud-py-1.2.8/mud_src/mud_friendly.c
--rw-rw-r--   0 fuji      (1000) fuji      (1000)    31872 2021-08-28 20:55:40.000000 mud-py-1.2.8/mud_src/mud_gen.c
--rw-r--r--   0 fuji      (1000) fuji      (1000)     2709 2012-11-14 02:01:37.000000 mud-py-1.2.8/mud_src/mud_misc.c
--rw-r--r--   0 fuji      (1000) fuji      (1000)     4758 2013-12-17 05:23:24.000000 mud-py-1.2.8/mud_src/mud_new.c
--rw-r--r--   0 fuji      (1000) fuji      (1000)     7886 2019-08-15 04:29:22.000000 mud-py-1.2.8/mud_src/mud_tri_ti.c
-drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2021-09-04 19:40:47.656133 mud-py-1.2.8/mudpy/
--rw-rw-r--   0 fuji      (1000) fuji      (1000)      160 2021-08-26 18:29:40.000000 mud-py-1.2.8/mudpy/__init__.py
--rw-r--r--   0 fuji      (1000) fuji      (1000)      245 2021-03-11 20:42:17.000000 mud-py-1.2.8/mudpy/containers.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)       72 2021-09-04 19:40:03.000000 mud-py-1.2.8/mudpy/global_variables.py
--rw-r--r--   0 fuji      (1000) fuji      (1000)      626 2021-03-11 21:30:44.000000 mud-py-1.2.8/mudpy/mcomment.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     5198 2021-06-07 18:39:13.000000 mud-py-1.2.8/mudpy/mcontainer.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)    19459 2021-06-07 18:40:04.000000 mud-py-1.2.8/mudpy/mdata.py
--rw-r--r--   0 fuji      (1000) fuji      (1000)      877 2021-03-11 20:38:05.000000 mud-py-1.2.8/mudpy/mdict.py
--rw-r--r--   0 fuji      (1000) fuji      (1000)     9463 2021-03-11 21:30:58.000000 mud-py-1.2.8/mudpy/mhist.py
--rw-r--r--   0 fuji      (1000) fuji      (1000)     1312 2021-03-11 20:40:23.000000 mud-py-1.2.8/mudpy/mlist.py
--rw-r--r--   0 fuji      (1000) fuji      (1000)      611 2021-03-11 21:24:54.000000 mud-py-1.2.8/mudpy/mscaler.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)  2045447 2021-08-26 19:44:26.000000 mud-py-1.2.8/mudpy/mud_friendly_wrapper.c
--rw-rw-r--   0 fuji      (1000) fuji      (1000)    53917 2021-08-26 19:30:32.000000 mud-py-1.2.8/mudpy/mud_friendly_wrapper.pyx
--rw-r--r--   0 fuji      (1000) fuji      (1000)     1131 2021-03-11 21:24:08.000000 mud-py-1.2.8/mudpy/mvar.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)       38 2021-09-04 19:40:47.656133 mud-py-1.2.8/setup.cfg
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     2412 2021-09-04 19:15:27.000000 mud-py-1.2.8/setup.py
-drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2021-09-04 19:40:47.656133 mud-py-1.2.8/test/
--rw-rw-r--   0 fuji      (1000) fuji      (1000)    14155 2021-06-07 18:47:49.000000 mud-py-1.2.8/test/test_mud_friendly_read.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)    14155 2021-05-31 23:09:31.000000 mud-py-1.2.8/test/test_mud_friendly_write.py
+drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2022-07-26 22:30:18.302387 mud-py-1.2.9/
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)    35149 2019-11-12 04:27:37.000000 mud-py-1.2.9/LICENSE
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)       91 2021-08-26 20:20:29.000000 mud-py-1.2.9/MANIFEST.in
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     5464 2022-07-26 22:30:18.302387 mud-py-1.2.9/PKG-INFO
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     4712 2022-07-26 17:11:15.000000 mud-py-1.2.9/README.md
+drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2022-07-26 22:30:18.202385 mud-py-1.2.9/mud_py.egg-info/
+-rw-r--r--   0 fuji      (1000) fuji      (1000)     5464 2022-07-26 22:30:17.000000 mud-py-1.2.9/mud_py.egg-info/PKG-INFO
+-rw-r--r--   0 fuji      (1000) fuji      (1000)      812 2022-07-26 22:30:17.000000 mud-py-1.2.9/mud_py.egg-info/SOURCES.txt
+-rw-r--r--   0 fuji      (1000) fuji      (1000)        1 2022-07-26 22:30:17.000000 mud-py-1.2.9/mud_py.egg-info/dependency_links.txt
+-rw-r--r--   0 fuji      (1000) fuji      (1000)       37 2022-07-26 22:30:17.000000 mud-py-1.2.9/mud_py.egg-info/requires.txt
+-rw-r--r--   0 fuji      (1000) fuji      (1000)        6 2022-07-26 22:30:17.000000 mud-py-1.2.9/mud_py.egg-info/top_level.txt
+drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2022-07-26 22:30:18.210385 mud-py-1.2.9/mud_src/
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)    21832 2021-08-28 20:55:40.000000 mud-py-1.2.9/mud_src/mud.c
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)    27875 2021-09-03 18:53:40.000000 mud-py-1.2.9/mud_src/mud.h
+-rw-r--r--   0 fuji      (1000) fuji      (1000)     6853 2019-08-15 04:24:31.000000 mud-py-1.2.9/mud_src/mud_all.c
+-rw-r--r--   0 fuji      (1000) fuji      (1000)    10305 2019-07-25 07:31:42.000000 mud-py-1.2.9/mud_src/mud_encode.c
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)    47224 2021-08-26 19:27:17.000000 mud-py-1.2.9/mud_src/mud_friendly.c
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)    31872 2021-08-28 20:55:40.000000 mud-py-1.2.9/mud_src/mud_gen.c
+-rw-r--r--   0 fuji      (1000) fuji      (1000)     2709 2012-11-14 02:01:37.000000 mud-py-1.2.9/mud_src/mud_misc.c
+-rw-r--r--   0 fuji      (1000) fuji      (1000)     4758 2013-12-17 05:23:24.000000 mud-py-1.2.9/mud_src/mud_new.c
+-rw-r--r--   0 fuji      (1000) fuji      (1000)     7886 2019-08-15 04:29:22.000000 mud-py-1.2.9/mud_src/mud_tri_ti.c
+drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2022-07-26 22:30:18.278386 mud-py-1.2.9/mudpy/
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)      160 2021-08-26 18:29:40.000000 mud-py-1.2.9/mudpy/__init__.py
+-rw-r--r--   0 fuji      (1000) fuji      (1000)      245 2021-03-11 20:42:17.000000 mud-py-1.2.9/mudpy/containers.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)       72 2022-07-26 22:29:42.000000 mud-py-1.2.9/mudpy/global_variables.py
+-rw-r--r--   0 fuji      (1000) fuji      (1000)      626 2021-03-11 21:30:44.000000 mud-py-1.2.9/mudpy/mcomment.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     5198 2021-06-07 18:39:13.000000 mud-py-1.2.9/mudpy/mcontainer.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)    19459 2021-06-07 18:40:04.000000 mud-py-1.2.9/mudpy/mdata.py
+-rw-r--r--   0 fuji      (1000) fuji      (1000)      877 2021-03-11 20:38:05.000000 mud-py-1.2.9/mudpy/mdict.py
+-rw-r--r--   0 fuji      (1000) fuji      (1000)     9538 2022-07-26 20:50:27.000000 mud-py-1.2.9/mudpy/mhist.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     1352 2022-07-26 22:28:48.000000 mud-py-1.2.9/mudpy/mlist.py
+-rw-r--r--   0 fuji      (1000) fuji      (1000)      611 2021-03-11 21:24:54.000000 mud-py-1.2.9/mudpy/mscaler.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)  2045447 2021-08-26 19:44:26.000000 mud-py-1.2.9/mudpy/mud_friendly_wrapper.c
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)    53917 2021-08-26 19:30:32.000000 mud-py-1.2.9/mudpy/mud_friendly_wrapper.pyx
+-rw-r--r--   0 fuji      (1000) fuji      (1000)     1131 2021-03-11 21:24:08.000000 mud-py-1.2.9/mudpy/mvar.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)       38 2022-07-26 22:30:18.302387 mud-py-1.2.9/setup.cfg
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     2412 2021-09-04 19:15:27.000000 mud-py-1.2.9/setup.py
+drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2022-07-26 22:30:18.294387 mud-py-1.2.9/test/
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)    14155 2021-06-07 18:47:49.000000 mud-py-1.2.9/test/test_mud_friendly_read.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)    14155 2021-05-31 23:09:31.000000 mud-py-1.2.9/test/test_mud_friendly_write.py
```

### Comparing `mud-py-1.2.8/LICENSE` & `mud-py-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mud-py-1.2.8/PKG-INFO` & `mud-py-1.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mud-py
-Version: 1.2.8
+Version: 1.2.9
 Summary: MUon Data file reader
 Home-page: https://github.com/dfujim/mudpy
 Author: Derek Fujimoto
 Author-email: fujimoto@phas.ubc.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -46,15 +46,15 @@
 * Provide low-level wrappers of the [`mud_friendly`] API. 
 
 ## Citing
 
 If you use [mudpy] in your work, please cite:
 
 - D. Fujimoto.
-  <i>bfit: A Python Application For Beta-Detected NMR</i>.
+  <i>Digging Into MUD With Python: mudpy, bdata, and bfit</i>.
   <a href="https://arxiv.org/abs/2004.10395">
   arXiv:2004.10395 [physics.data-an]</a>.
 
 
 ## Community Guidelines
 
 * Please submit contributions to [mudpy] via a pull request
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mud-py Version: 1.2.8 Summary: MUon Data file
+Metadata-Version: 2.1 Name: mud-py Version: 1.2.9 Summary: MUon Data file
 reader Home-page: https://github.com/dfujim/mudpy Author: Derek Fujimoto
 Author-email: fujimoto@phas.ubc.ca License: UNKNOWN Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Cython Classifier: License :: OSI Approved
 :: GNU Lesser General Public License v3 (LGPLv3) Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: MacOS Classifier: Operating
@@ -21,15 +21,15 @@
 radioactive nuclei or a [muon] as the [NMR] probe in place of a stable isotope.
 The intended user of [mudpy] is anyone analyzing data in [TRIUMF]'s [MUD] file
 format. A key goal of the project is to alleviate much of the technical tedium
 that is often encountered during any analysis. [mudpy] has been written to
 fullfill the following needs: * Provide a pythonic means of interfacing with
 [MUD] files in [Python]. * Provide low-level wrappers of the [`mud_friendly`]
 API. ## Citing If you use [mudpy] in your work, please cite: - D. Fujimoto.
-bfit: A Python Application For Beta-Detected NMR. arXiv:2004.10395_
+Digging Into MUD With Python: mudpy, bdata, and bfit. arXiv:2004.10395_
 [physics.data-an]. ## Community Guidelines * Please submit contributions to
 [mudpy] via a pull request * To report issues or get support, please file a new
 issue ## Installation and Use ### Dependencies The following packages/
 applications are needed prior to installation: - [Python] 3.6 or higher: a
 dynamically typed programming language. [[install](https://wiki.python.org/
 moin/BeginnersGuide/Download)] ### Install Instructions | | Command | |:-- | :-
 -| From the [PyPI] as user (recommended) | `pip install --user mud-py` | From
```

### Comparing `mud-py-1.2.8/README.md` & `mud-py-1.2.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 * Provide low-level wrappers of the [`mud_friendly`] API. 
 
 ## Citing
 
 If you use [mudpy] in your work, please cite:
 
 - D. Fujimoto.
-  <i>bfit: A Python Application For Beta-Detected NMR</i>.
+  <i>Digging Into MUD With Python: mudpy, bdata, and bfit</i>.
   <a href="https://arxiv.org/abs/2004.10395">
   arXiv:2004.10395 [physics.data-an]</a>.
 
 
 ## Community Guidelines
 
 * Please submit contributions to [mudpy] via a pull request
```

#### html2text {}

```diff
@@ -11,15 +11,15 @@
 radioactive nuclei or a [muon] as the [NMR] probe in place of a stable isotope.
 The intended user of [mudpy] is anyone analyzing data in [TRIUMF]'s [MUD] file
 format. A key goal of the project is to alleviate much of the technical tedium
 that is often encountered during any analysis. [mudpy] has been written to
 fullfill the following needs: * Provide a pythonic means of interfacing with
 [MUD] files in [Python]. * Provide low-level wrappers of the [`mud_friendly`]
 API. ## Citing If you use [mudpy] in your work, please cite: - D. Fujimoto.
-bfit: A Python Application For Beta-Detected NMR. arXiv:2004.10395_
+Digging Into MUD With Python: mudpy, bdata, and bfit. arXiv:2004.10395_
 [physics.data-an]. ## Community Guidelines * Please submit contributions to
 [mudpy] via a pull request * To report issues or get support, please file a new
 issue ## Installation and Use ### Dependencies The following packages/
 applications are needed prior to installation: - [Python] 3.6 or higher: a
 dynamically typed programming language. [[install](https://wiki.python.org/
 moin/BeginnersGuide/Download)] ### Install Instructions | | Command | |:-- | :-
 -| From the [PyPI] as user (recommended) | `pip install --user mud-py` | From
```

### Comparing `mud-py-1.2.8/mud_py.egg-info/PKG-INFO` & `mud-py-1.2.9/mud_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mud-py
-Version: 1.2.8
+Version: 1.2.9
 Summary: MUon Data file reader
 Home-page: https://github.com/dfujim/mudpy
 Author: Derek Fujimoto
 Author-email: fujimoto@phas.ubc.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -46,15 +46,15 @@
 * Provide low-level wrappers of the [`mud_friendly`] API. 
 
 ## Citing
 
 If you use [mudpy] in your work, please cite:
 
 - D. Fujimoto.
-  <i>bfit: A Python Application For Beta-Detected NMR</i>.
+  <i>Digging Into MUD With Python: mudpy, bdata, and bfit</i>.
   <a href="https://arxiv.org/abs/2004.10395">
   arXiv:2004.10395 [physics.data-an]</a>.
 
 
 ## Community Guidelines
 
 * Please submit contributions to [mudpy] via a pull request
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mud-py Version: 1.2.8 Summary: MUon Data file
+Metadata-Version: 2.1 Name: mud-py Version: 1.2.9 Summary: MUon Data file
 reader Home-page: https://github.com/dfujim/mudpy Author: Derek Fujimoto
 Author-email: fujimoto@phas.ubc.ca License: UNKNOWN Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Cython Classifier: License :: OSI Approved
 :: GNU Lesser General Public License v3 (LGPLv3) Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: MacOS Classifier: Operating
@@ -21,15 +21,15 @@
 radioactive nuclei or a [muon] as the [NMR] probe in place of a stable isotope.
 The intended user of [mudpy] is anyone analyzing data in [TRIUMF]'s [MUD] file
 format. A key goal of the project is to alleviate much of the technical tedium
 that is often encountered during any analysis. [mudpy] has been written to
 fullfill the following needs: * Provide a pythonic means of interfacing with
 [MUD] files in [Python]. * Provide low-level wrappers of the [`mud_friendly`]
 API. ## Citing If you use [mudpy] in your work, please cite: - D. Fujimoto.
-bfit: A Python Application For Beta-Detected NMR. arXiv:2004.10395_
+Digging Into MUD With Python: mudpy, bdata, and bfit. arXiv:2004.10395_
 [physics.data-an]. ## Community Guidelines * Please submit contributions to
 [mudpy] via a pull request * To report issues or get support, please file a new
 issue ## Installation and Use ### Dependencies The following packages/
 applications are needed prior to installation: - [Python] 3.6 or higher: a
 dynamically typed programming language. [[install](https://wiki.python.org/
 moin/BeginnersGuide/Download)] ### Install Instructions | | Command | |:-- | :-
 -| From the [PyPI] as user (recommended) | `pip install --user mud-py` | From
```

### Comparing `mud-py-1.2.8/mud_py.egg-info/SOURCES.txt` & `mud-py-1.2.9/mud_py.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -5,21 +5,14 @@
 ./mud_src/mud.c
 ./mud_src/mud_all.c
 ./mud_src/mud_encode.c
 ./mud_src/mud_gen.c
 ./mud_src/mud_misc.c
 ./mud_src/mud_new.c
 ./mud_src/mud_tri_ti.c
-/home/fuji/Documents/Research/src/mudpy/mud_src/mud.c
-/home/fuji/Documents/Research/src/mudpy/mud_src/mud_all.c
-/home/fuji/Documents/Research/src/mudpy/mud_src/mud_encode.c
-/home/fuji/Documents/Research/src/mudpy/mud_src/mud_gen.c
-/home/fuji/Documents/Research/src/mudpy/mud_src/mud_misc.c
-/home/fuji/Documents/Research/src/mudpy/mud_src/mud_new.c
-/home/fuji/Documents/Research/src/mudpy/mud_src/mud_tri_ti.c
 mud_py.egg-info/PKG-INFO
 mud_py.egg-info/SOURCES.txt
 mud_py.egg-info/dependency_links.txt
 mud_py.egg-info/requires.txt
 mud_py.egg-info/top_level.txt
 mud_src/mud.c
 mud_src/mud.h
```

### Comparing `mud-py-1.2.8/mud_src/mud.c` & `mud-py-1.2.9/mud_src/mud.c`

 * *Files identical despite different names*

### Comparing `mud-py-1.2.8/mud_src/mud.h` & `mud-py-1.2.9/mud_src/mud.h`

 * *Files identical despite different names*

### Comparing `mud-py-1.2.8/mud_src/mud_all.c` & `mud-py-1.2.9/mud_src/mud_all.c`

 * *Files identical despite different names*

### Comparing `mud-py-1.2.8/mud_src/mud_encode.c` & `mud-py-1.2.9/mud_src/mud_encode.c`

 * *Files identical despite different names*

### Comparing `mud-py-1.2.8/mud_src/mud_friendly.c` & `mud-py-1.2.9/mud_src/mud_friendly.c`

 * *Files identical despite different names*

### Comparing `mud-py-1.2.8/mud_src/mud_gen.c` & `mud-py-1.2.9/mud_src/mud_gen.c`

 * *Files identical despite different names*

### Comparing `mud-py-1.2.8/mud_src/mud_misc.c` & `mud-py-1.2.9/mud_src/mud_misc.c`

 * *Files identical despite different names*

### Comparing `mud-py-1.2.8/mud_src/mud_new.c` & `mud-py-1.2.9/mud_src/mud_new.c`

 * *Files identical despite different names*

### Comparing `mud-py-1.2.8/mud_src/mud_tri_ti.c` & `mud-py-1.2.9/mud_src/mud_tri_ti.c`

 * *Files identical despite different names*

### Comparing `mud-py-1.2.8/mudpy/mcomment.py` & `mud-py-1.2.9/mudpy/mcomment.py`

 * *Files identical despite different names*

### Comparing `mud-py-1.2.8/mudpy/mcontainer.py` & `mud-py-1.2.9/mudpy/mcontainer.py`

 * *Files identical despite different names*

### Comparing `mud-py-1.2.8/mudpy/mdata.py` & `mud-py-1.2.9/mudpy/mdata.py`

 * *Files identical despite different names*

### Comparing `mud-py-1.2.8/mudpy/mdict.py` & `mud-py-1.2.9/mudpy/mdict.py`

 * *Files identical despite different names*

### Comparing `mud-py-1.2.8/mudpy/mhist.py` & `mud-py-1.2.9/mudpy/mhist.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,14 +84,17 @@
     def __ior__(self, other):       self.data.__ior__(self._get_oval(other)); return self
     def __ipow__(self, other):      self.data **= self._get_oval(other); return self
     def __irshift__(self, other):   self.data.__irshift__(self._get_oval(other)); return self
     def __isub__(self, other):      self.data -= self._get_oval(other); return self
     def __itruediv__(self, other):  self.data /= self._get_oval(other); return self
     def __ixor__(self, other):      self.data.__ixor__(self._get_oval(other)); return self
 
+    # dict-like
+    def keys(self):                 return self.__slots__
+
     # copied from np.ndarray
     def all(self, *args, **kwargs):             return self.data.all(*args, **kwargs)
     def any(self, *args, **kwargs):             return self.data.any(*args, **kwargs)
     def argmax(self, *args, **kwargs):          return self.data.argmax(*args, **kwargs)
     def argmin(self, *args, **kwargs):          return self.data.argmin(*args, **kwargs)
     def argpartition(self, *args, **kwargs):    return self.data.argpartition(*args, **kwargs)
     def argsort(self, *args, **kwargs):         return self.data.argsort(*args, **kwargs)
```

### Comparing `mud-py-1.2.8/mudpy/mlist.py` & `mud-py-1.2.9/mudpy/mlist.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,23 +7,23 @@
     """
 
     # ======================================================================= #
     def __getattr__(self, name):
         """
             Get attribute of underlying data as a list.
         """
-
+        
         # fetch from top level
         try:
             return getattr(object, name)
 
         # fetch from lower levels
         except AttributeError:
             out = mlist([getattr(d, name) for d in self])
-
+            
             # if base level, return as array
             if type(out[0]) in (float, int):
                 return np.array(out)
             else:
                 return out
 
     # ======================================================================= #
@@ -33,14 +33,14 @@
         """
         # fetch from top level
         try:
             return list.__getitem__(self, name)
 
         # fetch from lower levels
         except TypeError:
-            out = mlist([d[name] for d in self])
+            out = mlist([d[name] for d in self if name in d.keys()])
 
             # if base level, return as array
             if type(out[0]) in (float, int):
                 return np.array(out)
             else:
                 return out
```

### Comparing `mud-py-1.2.8/mudpy/mscaler.py` & `mud-py-1.2.9/mudpy/mscaler.py`

 * *Files identical despite different names*

### Comparing `mud-py-1.2.8/mudpy/mud_friendly_wrapper.c` & `mud-py-1.2.9/mudpy/mud_friendly_wrapper.c`

 * *Files identical despite different names*

### Comparing `mud-py-1.2.8/mudpy/mud_friendly_wrapper.pyx` & `mud-py-1.2.9/mudpy/mud_friendly_wrapper.pyx`

 * *Files identical despite different names*

### Comparing `mud-py-1.2.8/mudpy/mvar.py` & `mud-py-1.2.9/mudpy/mvar.py`

 * *Files identical despite different names*

### Comparing `mud-py-1.2.8/setup.py` & `mud-py-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `mud-py-1.2.8/test/test_mud_friendly_read.py` & `mud-py-1.2.9/test/test_mud_friendly_read.py`

 * *Files identical despite different names*

### Comparing `mud-py-1.2.8/test/test_mud_friendly_write.py` & `mud-py-1.2.9/test/test_mud_friendly_write.py`

 * *Files identical despite different names*

