# Comparing `tmp/edm-arch-1.0.34.tar.gz` & `tmp/edm-arch-1.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edm-arch-1.0.34.tar", last modified: Thu May 11 11:41:47 2023, max compression
+gzip compressed data, was "edm-arch-1.0.35.tar", last modified: Wed May 24 07:57:28 2023, max compression
```

## Comparing `edm-arch-1.0.34.tar` & `edm-arch-1.0.35.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 11:41:47.004973 edm-arch-1.0.34/
--rw-rw-rw-   0        0        0     1096 2022-06-07 20:35:30.000000 edm-arch-1.0.34/LICENSE
--rw-rw-rw-   0        0        0    16069 2023-05-11 11:41:47.004973 edm-arch-1.0.34/PKG-INFO
--rw-rw-rw-   0        0        0    15175 2023-05-08 09:53:16.000000 edm-arch-1.0.34/README.md
--rw-rw-rw-   0        0        0      523 2023-05-11 08:29:35.000000 edm-arch-1.0.34/pyproject.toml
--rw-rw-rw-   0        0        0     1255 2023-05-11 11:41:47.006966 edm-arch-1.0.34/setup.cfg
--rw-rw-rw-   0        0        0       73 2022-06-16 14:04:21.000000 edm-arch-1.0.34/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:41:46.935937 edm-arch-1.0.34/src/
-drwxrwxrwx   0        0        0        0 2023-05-11 11:41:46.976843 edm-arch-1.0.34/src/edm_arch.egg-info/
--rw-rw-rw-   0        0        0    16069 2023-05-11 11:41:46.000000 edm-arch-1.0.34/src/edm_arch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      658 2023-05-11 11:41:46.000000 edm-arch-1.0.34/src/edm_arch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 11:41:46.000000 edm-arch-1.0.34/src/edm_arch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-06-22 11:44:30.000000 edm-arch-1.0.34/src/edm_arch.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      162 2023-05-11 11:41:46.000000 edm-arch-1.0.34/src/edm_arch.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-11 11:41:46.000000 edm-arch-1.0.34/src/edm_arch.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-11 11:41:46.992852 edm-arch-1.0.34/src/edmpy/
--rw-rw-rw-   0        0        0        0 2021-08-16 15:52:39.000000 edm-arch-1.0.34/src/edmpy/__init__.py
--rw-rw-rw-   0        0        0       79 2022-06-21 13:54:13.000000 edm-arch-1.0.34/src/edmpy/__main__.py
--rw-rw-rw-   0        0        0    28032 2023-05-11 11:24:27.000000 edm-arch-1.0.34/src/edmpy/cfg.py
--rw-rw-rw-   0        0        0       18 2023-03-08 09:12:03.000000 edm-arch-1.0.34/src/edmpy/constants.py
--rw-rw-rw-   0        0        0     5301 2023-05-11 11:23:24.000000 edm-arch-1.0.34/src/edmpy/db.py
--rw-rw-rw-   0        0        0    13461 2023-05-08 09:53:16.000000 edm-arch-1.0.34/src/edmpy/edm.kv
--rw-rw-rw-   0        0        0   123243 2023-05-11 11:39:52.000000 edm-arch-1.0.34/src/edmpy/edm.py
--rw-rw-rw-   0        0        0     5691 2023-05-08 09:53:16.000000 edm-arch-1.0.34/src/edmpy/geo.py
--rw-rw-rw-   0        0        0     2508 2023-05-11 11:24:10.000000 edm-arch-1.0.34/src/edmpy/ini.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:41:47.004033 edm-arch-1.0.34/src/edmpy/lib/
--rw-rw-rw-   0        0        0        0 2021-08-16 15:52:39.000000 edm-arch-1.0.34/src/edmpy/lib/__init__.py
--rw-rw-rw-   0        0        0     4220 2023-05-11 11:23:24.000000 edm-arch-1.0.34/src/edmpy/lib/blockdata.py
--rw-rw-rw-   0        0        0     4338 2023-05-11 11:23:24.000000 edm-arch-1.0.34/src/edmpy/lib/colorscheme.py
--rw-rw-rw-   0        0        0     2334 2023-05-08 09:53:16.000000 edm-arch-1.0.34/src/edmpy/lib/constants.py
--rw-rw-rw-   0        0        0     4035 2023-03-08 08:56:31.000000 edm-arch-1.0.34/src/edmpy/lib/dbs.py
--rw-rw-rw-   0        0        0   175959 2023-05-11 11:21:32.000000 edm-arch-1.0.34/src/edmpy/lib/e5_widgets.py
--rw-rw-rw-   0        0        0     1792 2023-05-08 09:53:16.000000 edm-arch-1.0.34/src/edmpy/lib/misc.py
--rw-rw-rw-   0        0        0        0 2022-06-07 20:43:53.000000 edm-arch-1.0.34/src/edmpy/py.typed
--rw-rw-rw-   0        0        0    44655 2023-05-11 11:23:24.000000 edm-arch-1.0.34/src/edmpy/totalstation.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:57:28.558853 edm-arch-1.0.35/
+-rw-rw-rw-   0        0        0     1096 2022-06-07 20:35:30.000000 edm-arch-1.0.35/LICENSE
+-rw-rw-rw-   0        0        0    17591 2023-05-24 07:57:28.559853 edm-arch-1.0.35/PKG-INFO
+-rw-rw-rw-   0        0        0    16697 2023-05-24 07:51:33.000000 edm-arch-1.0.35/README.md
+-rw-rw-rw-   0        0        0      523 2023-05-11 08:29:35.000000 edm-arch-1.0.35/pyproject.toml
+-rw-rw-rw-   0        0        0     1255 2023-05-24 07:57:28.560890 edm-arch-1.0.35/setup.cfg
+-rw-rw-rw-   0        0        0       73 2022-06-16 14:04:21.000000 edm-arch-1.0.35/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:57:28.521871 edm-arch-1.0.35/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 07:57:28.536855 edm-arch-1.0.35/src/edm_arch.egg-info/
+-rw-rw-rw-   0        0        0    17591 2023-05-24 07:57:28.000000 edm-arch-1.0.35/src/edm_arch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      658 2023-05-24 07:57:28.000000 edm-arch-1.0.35/src/edm_arch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 07:57:28.000000 edm-arch-1.0.35/src/edm_arch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-06-22 11:44:30.000000 edm-arch-1.0.35/src/edm_arch.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      162 2023-05-24 07:57:28.000000 edm-arch-1.0.35/src/edm_arch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-24 07:57:28.000000 edm-arch-1.0.35/src/edm_arch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 07:57:28.549852 edm-arch-1.0.35/src/edmpy/
+-rw-rw-rw-   0        0        0        0 2021-08-16 15:52:39.000000 edm-arch-1.0.35/src/edmpy/__init__.py
+-rw-rw-rw-   0        0        0       79 2022-06-21 13:54:13.000000 edm-arch-1.0.35/src/edmpy/__main__.py
+-rw-rw-rw-   0        0        0    28427 2023-05-16 12:08:43.000000 edm-arch-1.0.35/src/edmpy/cfg.py
+-rw-rw-rw-   0        0        0       18 2023-03-08 09:12:03.000000 edm-arch-1.0.35/src/edmpy/constants.py
+-rw-rw-rw-   0        0        0     5450 2023-05-22 10:08:25.000000 edm-arch-1.0.35/src/edmpy/db.py
+-rw-rw-rw-   0        0        0    13461 2023-05-08 09:53:16.000000 edm-arch-1.0.35/src/edmpy/edm.kv
+-rw-rw-rw-   0        0        0   126492 2023-05-24 07:51:36.000000 edm-arch-1.0.35/src/edmpy/edm.py
+-rw-rw-rw-   0        0        0     5691 2023-05-08 09:53:16.000000 edm-arch-1.0.35/src/edmpy/geo.py
+-rw-rw-rw-   0        0        0     2508 2023-05-11 11:24:10.000000 edm-arch-1.0.35/src/edmpy/ini.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:57:28.558853 edm-arch-1.0.35/src/edmpy/lib/
+-rw-rw-rw-   0        0        0        0 2021-08-16 15:52:39.000000 edm-arch-1.0.35/src/edmpy/lib/__init__.py
+-rw-rw-rw-   0        0        0     4220 2023-05-11 11:23:24.000000 edm-arch-1.0.35/src/edmpy/lib/blockdata.py
+-rw-rw-rw-   0        0        0     4338 2023-05-11 11:23:24.000000 edm-arch-1.0.35/src/edmpy/lib/colorscheme.py
+-rw-rw-rw-   0        0        0     2334 2023-05-08 09:53:16.000000 edm-arch-1.0.35/src/edmpy/lib/constants.py
+-rw-rw-rw-   0        0        0     4035 2023-03-08 08:56:31.000000 edm-arch-1.0.35/src/edmpy/lib/dbs.py
+-rw-rw-rw-   0        0        0   177497 2023-05-23 07:50:54.000000 edm-arch-1.0.35/src/edmpy/lib/e5_widgets.py
+-rw-rw-rw-   0        0        0     1792 2023-05-08 09:53:16.000000 edm-arch-1.0.35/src/edmpy/lib/misc.py
+-rw-rw-rw-   0        0        0        0 2022-06-07 20:43:53.000000 edm-arch-1.0.35/src/edmpy/py.typed
+-rw-rw-rw-   0        0        0    44664 2023-05-16 12:03:19.000000 edm-arch-1.0.35/src/edmpy/totalstation.py
```

### Comparing `edm-arch-1.0.34/LICENSE` & `edm-arch-1.0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.34/PKG-INFO` & `edm-arch-1.0.35/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edm-arch
-Version: 1.0.34
+Version: 1.0.35
 Summary: Total stations for archaeologists
 Home-page: https://github.com/surf3s/EDM
 Author: Shannon P. McPherron
 Author-email: mcpherron@eva.mpg.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/surf3s/EDM/issues
 Platform: unix
@@ -107,14 +107,47 @@
 
 Short answer, I don't know.  I have simulated having 1000 points in the database and it is still reasonably fast and responsive on my laptop.  As you add more points, you can expect certain parts of the program to slow (e.g. opening the data grid to view all points).  I never intended my programs to be the main database a person uses.  I always envisioned doing some data entry with these programs (E5 and EDM) before moving the data into a real database.  However, I know lots of people who keep their entire dataset in these programs.  I think that is okay, but remember to always keep backups.
 
 #### Why can't I plot the points with this program?
 
 I am working on this.  Once this program is working smoothly, I will add plot functionality.
 
+##### Changes for Version 1.0.35 (May 24, 2023)
+  Bug in file import fixed
+  Bug in CFG when no field type is specified fixed as well
+  Bug in Filter records that crashed program is fixed
+  Importing CSV now takes seconds rather than many many minutes (tested on import of 3996 records)
+  Saving a point is now faster when record count is high
+  Reworked a number of features because JSON files are not in doc_id order
+  Add a "SIMULATION mode on" warning to maing screen when simulating points
+  Suffix values on import csv are retained as integers
+  Tried to improve open CFG so that if a non-EDM CFG is opened, it is not also trashed
+  Fixed important bugs in station setup when using Manual XYZ or Manual VHD options
+  Error trap continuation shot on an empty data file
+
+##### Changes for Version 1.0.34
+  Yet more fixes for Windows/PyPi installations
+
+##### Changes for Version 1.0.33
+  Fixed installation issues
+
+##### Changes for Version 1.0.32
+  Fixing issues with GeoCom and station setup
+
+##### Changes for Version 1.0.31
+  Fixed issue with numeric values saved as text in JSON after initial save
+  Added Help JSON to view raw data in JSON file
+
+##### Changes for Version 1.0.31
+  BlueTooth tested with Leica GeoCom stations
+  UI fixes
+  Tested with 1000 records in DB
+  Made JSON files better formatted so that they are more human readable
+  Made geoJSON files work with QGIS (points and lines are separate layers)
+  Substantial refactoring of Python classes and file structure
 
 ##### Update (March 2, 2023)
 1.   Added and debugged Topcon stations
 2.   Added and debugged Leica and Leica GeoCom stations
 3.   Stopped program from exiting when escape is pressed
 4.   Fixed default locations for ini, log, and data
 5.   Program remembers last size and location of the screen
```

### Comparing `edm-arch-1.0.34/README.md` & `edm-arch-1.0.35/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -80,14 +80,47 @@
 
 Short answer, I don't know.  I have simulated having 1000 points in the database and it is still reasonably fast and responsive on my laptop.  As you add more points, you can expect certain parts of the program to slow (e.g. opening the data grid to view all points).  I never intended my programs to be the main database a person uses.  I always envisioned doing some data entry with these programs (E5 and EDM) before moving the data into a real database.  However, I know lots of people who keep their entire dataset in these programs.  I think that is okay, but remember to always keep backups.
 
 #### Why can't I plot the points with this program?
 
 I am working on this.  Once this program is working smoothly, I will add plot functionality.
 
+##### Changes for Version 1.0.35 (May 24, 2023)
+  Bug in file import fixed
+  Bug in CFG when no field type is specified fixed as well
+  Bug in Filter records that crashed program is fixed
+  Importing CSV now takes seconds rather than many many minutes (tested on import of 3996 records)
+  Saving a point is now faster when record count is high
+  Reworked a number of features because JSON files are not in doc_id order
+  Add a "SIMULATION mode on" warning to maing screen when simulating points
+  Suffix values on import csv are retained as integers
+  Tried to improve open CFG so that if a non-EDM CFG is opened, it is not also trashed
+  Fixed important bugs in station setup when using Manual XYZ or Manual VHD options
+  Error trap continuation shot on an empty data file
+
+##### Changes for Version 1.0.34
+  Yet more fixes for Windows/PyPi installations
+
+##### Changes for Version 1.0.33
+  Fixed installation issues
+
+##### Changes for Version 1.0.32
+  Fixing issues with GeoCom and station setup
+
+##### Changes for Version 1.0.31
+  Fixed issue with numeric values saved as text in JSON after initial save
+  Added Help JSON to view raw data in JSON file
+
+##### Changes for Version 1.0.31
+  BlueTooth tested with Leica GeoCom stations
+  UI fixes
+  Tested with 1000 records in DB
+  Made JSON files better formatted so that they are more human readable
+  Made geoJSON files work with QGIS (points and lines are separate layers)
+  Substantial refactoring of Python classes and file structure
 
 ##### Update (March 2, 2023)
 1.   Added and debugged Topcon stations
 2.   Added and debugged Leica and Leica GeoCom stations
 3.   Stopped program from exiting when escape is pressed
 4.   Fixed default locations for ini, log, and data
 5.   Program remembers last size and location of the screen
```

### Comparing `edm-arch-1.0.34/pyproject.toml` & `edm-arch-1.0.35/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.34/setup.cfg` & `edm-arch-1.0.35/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 646d 2d61 7263 680d 0a64 6573   = edm-arch..des
 00000020: 6372 6970 7469 6f6e 203d 2054 6f74 616c  cription = Total
 00000030: 2073 7461 7469 6f6e 7320 666f 7220 6172   stations for ar
 00000040: 6368 6165 6f6c 6f67 6973 7473 0d0a 7665  chaeologists..ve
-00000050: 7273 696f 6e20 3d20 312e 302e 3334 0d0a  rsion = 1.0.34..
+00000050: 7273 696f 6e20 3d20 312e 302e 3335 0d0a  rsion = 1.0.35..
 00000060: 6175 7468 6f72 203d 2053 6861 6e6e 6f6e  author = Shannon
 00000070: 2050 2e20 4d63 5068 6572 726f 6e0d 0a61   P. McPherron..a
 00000080: 7574 686f 725f 656d 6169 6c20 3d20 6d63  uthor_email = mc
 00000090: 7068 6572 726f 6e40 6576 612e 6d70 672e  pherron@eva.mpg.
 000000a0: 6465 0d0a 6c6f 6e67 5f64 6573 6372 6970  de..long_descrip
 000000b0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 000000c0: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
@@ -52,16 +52,16 @@
 00000330: 792e 6c69 620d 0a69 6e73 7461 6c6c 5f72  y.lib..install_r
 00000340: 6571 7569 7265 7320 3d20 0d0a 096b 6976  equires = ...kiv
 00000350: 793e 3d32 0d0a 0974 696e 7964 623e 3d34  y>=2...tinydb>=4
 00000360: 0d0a 0970 7973 6572 6961 6c3e 3d33 2e35  ...pyserial>=3.5
 00000370: 0d0a 0961 6e67 6c65 733e 3d32 0d0a 0970  ...angles>=2...p
 00000380: 7965 6e63 6861 6e74 3e3d 332e 322e 320d  yenchant>=3.2.2.
 00000390: 0a09 6170 7064 6174 613e 3d32 2e32 0d0a  ..appdata>=2.2..
-000003a0: 0972 6571 7565 7374 733e 3d32 2e32 382e  .requests>=2.28.
-000003b0: 310d 0a70 7974 686f 6e5f 7265 7175 6972  1..python_requir
+000003a0: 0972 6571 7565 7374 733e 3d32 2e33 312e  .requests>=2.31.
+000003b0: 300d 0a70 7974 686f 6e5f 7265 7175 6972  0..python_requir
 000003c0: 6573 203d 203e 3d33 2e36 0d0a 7061 636b  es = >=3.6..pack
 000003d0: 6167 655f 6469 7220 3d20 0d0a 093d 7372  age_dir = ...=sr
 000003e0: 630d 0a7a 6970 5f73 6166 6520 3d20 6e6f  c..zip_safe = no
 000003f0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 7874  ....[options.ext
 00000400: 7261 735f 7265 7175 6972 655d 0d0a 7465  ras_require]..te
 00000410: 7374 696e 6720 3d20 0d0a 0970 7974 6573  sting = ...pytes
 00000420: 743e 3d36 2e30 0d0a 0970 7974 6573 742d  t>=6.0...pytest-
```

### Comparing `edm-arch-1.0.34/src/edm_arch.egg-info/PKG-INFO` & `edm-arch-1.0.35/src/edm_arch.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edm-arch
-Version: 1.0.34
+Version: 1.0.35
 Summary: Total stations for archaeologists
 Home-page: https://github.com/surf3s/EDM
 Author: Shannon P. McPherron
 Author-email: mcpherron@eva.mpg.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/surf3s/EDM/issues
 Platform: unix
@@ -107,14 +107,47 @@
 
 Short answer, I don't know.  I have simulated having 1000 points in the database and it is still reasonably fast and responsive on my laptop.  As you add more points, you can expect certain parts of the program to slow (e.g. opening the data grid to view all points).  I never intended my programs to be the main database a person uses.  I always envisioned doing some data entry with these programs (E5 and EDM) before moving the data into a real database.  However, I know lots of people who keep their entire dataset in these programs.  I think that is okay, but remember to always keep backups.
 
 #### Why can't I plot the points with this program?
 
 I am working on this.  Once this program is working smoothly, I will add plot functionality.
 
+##### Changes for Version 1.0.35 (May 24, 2023)
+  Bug in file import fixed
+  Bug in CFG when no field type is specified fixed as well
+  Bug in Filter records that crashed program is fixed
+  Importing CSV now takes seconds rather than many many minutes (tested on import of 3996 records)
+  Saving a point is now faster when record count is high
+  Reworked a number of features because JSON files are not in doc_id order
+  Add a "SIMULATION mode on" warning to maing screen when simulating points
+  Suffix values on import csv are retained as integers
+  Tried to improve open CFG so that if a non-EDM CFG is opened, it is not also trashed
+  Fixed important bugs in station setup when using Manual XYZ or Manual VHD options
+  Error trap continuation shot on an empty data file
+
+##### Changes for Version 1.0.34
+  Yet more fixes for Windows/PyPi installations
+
+##### Changes for Version 1.0.33
+  Fixed installation issues
+
+##### Changes for Version 1.0.32
+  Fixing issues with GeoCom and station setup
+
+##### Changes for Version 1.0.31
+  Fixed issue with numeric values saved as text in JSON after initial save
+  Added Help JSON to view raw data in JSON file
+
+##### Changes for Version 1.0.31
+  BlueTooth tested with Leica GeoCom stations
+  UI fixes
+  Tested with 1000 records in DB
+  Made JSON files better formatted so that they are more human readable
+  Made geoJSON files work with QGIS (points and lines are separate layers)
+  Substantial refactoring of Python classes and file structure
 
 ##### Update (March 2, 2023)
 1.   Added and debugged Topcon stations
 2.   Added and debugged Leica and Leica GeoCom stations
 3.   Stopped program from exiting when escape is pressed
 4.   Fixed default locations for ini, log, and data
 5.   Program remembers last size and location of the screen
```

### Comparing `edm-arch-1.0.34/src/edm_arch.egg-info/SOURCES.txt` & `edm-arch-1.0.35/src/edm_arch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.34/src/edmpy/cfg.py` & `edm-arch-1.0.35/src/edmpy/cfg.py`

 * *Files 7% similar despite different names*

```diff
@@ -339,45 +339,54 @@
                 self.unique_together = ['UNIT', 'ID', 'SUFFIX']
             if 'ID' in field_names and 'SUFFIX' in field_names:
                 self.update_value('EDM', 'UNIQUE_TOGETHER', 'ID,SUFFIX')
                 self.unique_together = ['ID', 'SUFFIX']
 
         for field_name in field_names:
             if any((c in set(bad_characters)) for c in field_name):
-                self.errors.append(f"The field name '{field_name}' has non-standard characters in it that cause a problem in JSON files.  "\
-                                    "Do not use any of these '{bad_characters}' characters.  Change the name before collecting data.")
+                self.errors.append(f"The field name '{field_name}' has non-standard characters in it that cause a problem in JSON files.  "
+                                    f"Do not use any of these '{bad_characters}' characters.  Change the name before collecting data.")
                 self.has_errors = True
             f = self.get(field_name)
 
             if not self.is_numeric(f.length):
-                self.errors.append(f'The length specified for field {field_name} must be a valid number.  If you do not want to limit the length, '\
+                self.errors.append(f'The length specified for field {field_name} must be a valid number.  If you do not want to limit the length, '
                                      'delete the Length specification in the CFG.')
                 self.has_errors = True
 
             if f.prompt == '':
                 f.prompt = field_name
 
             f.inputtype = f.inputtype.upper()
+
+            if f.inputtype == '':
+                if field_name in ['X', 'Y', 'Z', 'SLOPED', 'VANGLE', 'HANGLE', 'STATIONX', 'STATIONY', 'STATIONZ', 'LOCALX', 'LOCALY', 'LOCALZ', 'PRISM']:
+                    f.inputtype = 'NUMERIC'
+                elif field_name in ['DATE']:
+                    f.inputtype = 'DATETIME'
+                else:
+                    f.inputtype = 'TEXT'
+
             if f.inputtype not in ['TEXT', 'NOTE', 'NUMERIC', 'MENU', 'DATETIME', 'BOOLEAN', 'CAMERA', 'GPS', 'INSTRUMENT']:
-                self.errors.append(f"The value '{f.inputtype}' for the field {field_name} is not a valid TYPE.  \
-                                    Valid TYPES include Text, Note, Numeric, and Menu.")
+                self.errors.append(f"The value '{f.inputtype}' for the field {field_name} is not a valid TYPE. "
+                                    "Valid TYPES include Text, Note, Numeric, and Menu.")
                 self.has_errors = True
 
             if field_name in ['UNIT', 'ID', 'SUFFIX', 'X', 'Y', 'Z']:
                 self.update_value(field_name, 'REQUIRED', 'TRUE')
 
             if field_name == 'ID':
                 self.update_value(field_name, 'INCREMENT', 'TRUE')
 
             if f.link_fields:
                 self.link_fields.append(field_name)
                 # uppercase the link fields
                 for link_field_name in f.link_fields:
                     if link_field_name not in field_names:
-                        self.errors.append(f"The field {field_name} is set to link to {link_field_name} but the field {link_field_name} "\
+                        self.errors.append(f"The field {field_name} is set to link to {link_field_name} but the field {link_field_name} "
                                             "does not exist in the CFG.")
                         self.has_errors = True
             self.put(field_name, f)
 
             for field_option in ['UNIQUE', 'CARRY', 'INCREMENT', 'REQUIRED', 'SORTED']:
                 if self.get_value(field_name, field_option):
                     if self.get_value(field_name, field_option).upper() == 'YES':
```

### Comparing `edm-arch-1.0.34/src/edmpy/db.py` & `edm-arch-1.0.35/src/edmpy/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,7 +113,10 @@
     def get_link_fields(self, name = None, value = None):
         if name is not None and value is not None and self.db is not None:
             q = Query()
             r = self.db.table(name).search(q[name].matches('^' + value + '$', re.IGNORECASE))
             if r != []:
                 return r[0]
         return None
+
+    def get_doc_ids(self, table_name):
+        return sorted([r.doc_id for r in self.db.table(table_name).all()] if self.db is not None else [])
```

### Comparing `edm-arch-1.0.34/src/edmpy/edm.kv` & `edm-arch-1.0.35/src/edmpy/edm.kv`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.34/src/edmpy/edm.py` & `edm-arch-1.0.35/src/edmpy/edm.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,28 +45,41 @@
 
 Changes for Version 1.0.33
   Fixed installation issues
 
 Changes for Version 1.0.34
   Yet more fixes for Windows/PyPi installations
 
-  Bugs/To Do
+Changes for Version 1.0.35
+  Bug in file import fixed
+  Bug in CFG when no field type is specified fixed as well
+  Bug in Filter records that crashed program is fixed
+  Importing CSV now takes seconds rather than many many minutes (tested on import of 3996 records)
+  Saving a point is now faster when record count is high
+  Reworked a number of features because JSON files are not in doc_id order
+  Add a "SIMULATION mode on" warning to maing screen when simulating points
+  Suffix values on import csv are retained as integers
+  Tried to improve open CFG so that if a non-EDM CFG is opened, it is not also trashed
+  Fixed important bugs in station setup when using Manual XYZ or Manual VHD options
+  Error trap continuation shot on an empty data file
+
+Bugs/To Do
   could make menus work better with keyboard (at least with tab)
   there is no error checking on duplicates in datagrid edits
   Do unitchecking after doing an offset shot on suffix 0 points
-  On import, integers (like Suffix) are being converted to float values
   Good way to get random hash IDs
   Offer to change Z when prism changes in datagrid edit cases
   Thoroughly test unit checking
   Thoroughly test setups (with and without prism)
   Add home/end page up/page down and control home/control end to datagrid movement
   *** Keeping checking edit/save issues
   *** Program asks for save record in all points even when having saved already
   Add move to top or bottom in Help JSON and others (like Log file)
   Check what gets logged
+  Deal more nicely with aftermath of a non-valid CFG being opened
 """
 
 
 from kivy.config import Config
 from kivy.core.clipboard import Clipboard
 from kivy.graphics import Color, Rectangle
 from kivy.app import App
@@ -139,15 +152,15 @@
 """
 try:
     import win32timezone
     win32timezone.TimeZoneInfo.local()
 except ModuleNotFoundError:
     pass
 
-VERSION = '1.0.34'
+VERSION = '1.0.35'
 PRODUCTION_DATE = 'May, 2023'
 __DEFAULT_FIELDS__ = ['X', 'Y', 'Z', 'SLOPED', 'VANGLE', 'HANGLE', 'STATIONX', 'STATIONY', 'STATIONZ', 'LOCALX', 'LOCALY', 'LOCALZ', 'DATE', 'PRISM', 'ID']
 __BUTTONS__ = 13
 __LASTCOMPORT__ = 16
 MAX_SCREEN_WIDTH = 400
 
 
@@ -409,22 +422,30 @@
     def message_open_cfg_first(self):
         message = '\nBefore you can do this, you need to open a CFG file (see option under File menu).  Opening a CFG file will also open your database. '
         message += 'If you do not have a CFG file already, you can use a default one (see option under File menu).  Later you can alter the default CFG to '
         message += 'add additional options specific to your work.'
         return e5_MessageBox('EDM', message)
 
     def ready_to_use(self):
-        return self.cfg is not None and self.data.filename != ''
+        return self.cfg is not None and self.data.filename != '' and self.data.filename is not None
 
     def take_shot(self, instance):
         if not self.ready_to_use() and instance.id != 'measure':
             self.popup = self.message_open_cfg_first()
             self.popup.open()
             return
 
+        if instance.id == 'continue' and len(self.data.db.table(self.data.table)) == 0:
+            message = 'Continue works only after you have saved at least one point.  Continue repeats the last point changing only the Suffix field '
+            message += 'and the new measured values.  All other values, such as layer, excavator, and so forth, carry over.  Continue is an easy '
+            message += 'way to link a series of measures to a single object or into one set of points.'
+            self.popup = e5_MessageBox('EDM', message)
+            self.popup.open()
+            return
+
         self.station.shot_type = instance.id
         self.station.clear_xyz()
         if self.station.make == 'Microscribe':
             self.popup = DataGridTextBox(title = 'EDM', text = '<Microscribe>',
                                             label = 'Waiting on...',
                                             button_text = ['Cancel', 'Next'],
                                             call_back = self.have_shot,
@@ -447,17 +468,17 @@
             p = self.station.text_to_point(f'{self.popup.xcoord.textbox.text},{self.popup.ycoord.textbox.text},{self.popup.zcoord.textbox.text}')
             if p:
                 self.station.xyz = p
                 self.station.make_global()
                 self.station.vhd_from_xyz()
         elif self.popup.hangle and self.popup.vangle and self.popup.sloped:
             try:
-                self.station.hangle = float(self.popup.hangle.text)
-                self.station.vangle = float(self.popup.vangle.text)
-                self.station.sloped = float(self.popup.sloped.text)
+                self.station.hangle = float(self.popup.hangle.textbox.text)
+                self.station.vangle = float(self.popup.vangle.textbox.text)
+                self.station.sloped = float(self.popup.sloped.textbox.text)
             except ValueError:
                 self.station.xyz = point()
             self.station.vhd_to_xyz()
             self.station.make_global()
         self.station.pnt = None
         self.popup.dismiss()
         if self.station.xyz.x is None or self.station.xyz.y is None or self.station.xyz.z is None:
@@ -608,61 +629,65 @@
         self.make_backup()
         self.check_for_duplicate_xyz()
         return []
 
     def log_the_shot(self):
         logger = logging.getLogger(__name__)
         logger.info(f'{self.get_last_squid()} {self.station.vhd_to_sexa_pretty_compact()} with prism height {self.station.prism.height} '
-                        'from {self.station.location} ')
+                        f'from {self.station.location} ')
 
     def on_cancel(self):
         if self.data.db is not None:
-            last_record = self.data.db.table(self.data.table).all()[-1]
-            if last_record != []:
-                self.data.db.table(self.data.table).remove(doc_ids = [last_record.doc_id])
+            doc_ids = self.data.get_doc_ids(self.data.table)
+            if doc_ids is not None:
+                self.data.db.table(self.data.table).remove(doc_ids = [doc_ids[-1]])
 
     def get_last_squid(self):
         unit = self.get_last_value('UNIT')
         idno = self.get_last_value('ID')
         suffix = self.get_last_value('SUFFIX')
         return f'{unit}-{idno}({suffix})' if all(item is not None for item in [unit, idno, suffix]) else ''
 
     def update_info_label(self):
         last_squid = self.get_last_squid()
         self.info.text = last_squid if last_squid else 'EDM'
+        if self.station.make in ['Simulate']:
+            self.info.text += " - SIMULATION mode on"
 
-    def same_coordinates(record1, record2):
+    def same_coordinates(self, record1, record2):
         return record1['X'] == record2['X'] and record1['Y'] == record2['Y'] and record1['Z'] == record2['Z']
 
     def check_for_duplicate_xyz(self):
-        if self.station.make == 'Microscribe' and self.data.db is not None:
+        if self.data.db is not None:
             if len(self.data.db.table(self.data.table)) > 1:
-                last_record = self.data.db.table(self.data.table).all()[-1]
-                next_to_last_record = self.data.db.table(self.data.table).all()[-2]
+                doc_ids = self.data.get_doc_ids(self.data.table)
+                last_record = self.data.db.table(self.data.table).get(doc_id = doc_ids[-1])
+                next_to_last_record = self.data.db.table(self.data.table).get(doc_id = doc_ids[-2])
                 if all(field in last_record.keys() for field in ['X', 'Y', 'Z']):
                     if self.same_coordinates(last_record, next_to_last_record):
-                        self.popup = e5_MessageBox(title = 'Warning',
-                                                    message = "\nThe last two recorded points have the exact same XYZ "
-                                                        f"coordinates ({last_record['X']}, {last_record['Y']}, {last_record['Z']}).  "
-                                                        "Verify that the Microscribe is still properly recording points (green light is on).  "
-                                                        "If the red light is on, you need to re-initialize (Setup - Initialize Station) and "
-                                                        "re-shoot the last two points.")
+                        message = "\nThe last two recorded points have the exact same XYZ coordinates "
+                        message += f"({last_record['X']}, {last_record['Y']}, {last_record['Z']}).  "
+                        if self.station.make == 'Microscribe':
+                            message += "Verify that the Microscribe is still properly recording points (green light is on).  "
+                            message += "If the red light is on, you need to re-initialize (Setup - Initialize Station) and "
+                            message += "re-shoot the last two points."
+                        self.popup = e5_MessageBox(title = 'Warning', message=message)
                         self.popup.open()
 
     def close_popup(self, instance):
         self.popup.dismiss()
 
     def save_default_cfg(self):
-        content = e5_SaveDialog(filename = '',
-                                start_path = self.cfg.path,
-                                save = self.save_default,
-                                cancel = self.dismiss_popup)
-        self.popup = Popup(title = "Create a new default CFG file",
-                            content = content,
-                            size_hint = (0.9, 0.9))
+        content = e5_SaveDialog(filename='',
+                                start_path=self.cfg.path,
+                                save=self.save_default,
+                                cancel=self.dismiss_popup)
+        self.popup = Popup(title="Create a new default CFG file",
+                            content=content,
+                            size_hint=(0.9, 0.9))
         self.popup.open()
         self.popup_open = True
 
     def save_default(self, *args):
         path = self.popup.content.filesaver.path
         filename = self.popup.content.filename
         if '.cfg' not in filename.lower():
@@ -706,20 +731,23 @@
                             size_hint = (0.9, 0.9))
         self.popup.open()
 
     def load_cfg(self, path, filename):
         warnings, errors = [], []
         self.data.close()
         self.dismiss_popup()
-        self.cfg.load(os.path.join(path, filename[0]))
-        if self.cfg.filename:
-            warnings, errors = self.open_db()
-            if errors == []:
-                self.set_new_data_to_true()
-        self.ini.update(self.colors, self.cfg)
+        has_errors, errors = self.cfg.load(os.path.join(path, filename[0]))
+        if not has_errors:
+            if self.cfg.filename:
+                warnings, errors = self.open_db()
+                if errors == []:
+                    self.set_new_data_to_true()
+            self.ini.update(self.colors, self.cfg)
+        else:
+            self.cfg = CFG()
         self.build_mainscreen()
         self.reset_screens()
         if warnings or errors:
             self.popup = self.warnings_and_errors_popup(warnings, errors)
             self.popup.open()
 
     def reset_screen_defaults(self):
@@ -762,28 +790,37 @@
         self.popup.dismiss()
         start_path = self.cfg.path if self.cfg.path else self.app_paths.app_data_path
         content = e5_LoadDialog(load = self.load_csv,
                                 cancel = self.dismiss_popup,
                                 start_path = start_path,
                                 button_color = self.colors.button_color,
                                 button_background = self.colors.button_background,
-                                filters = ['*.csv', '*.CSV', '*.txt', '*.TXT', '*.json', '*.JSON'])
+                                filters = ['*.csv', '*.CSV', '*.txt', '*.TXT', '*.json', '*.JSON'],
+                                font_size = self.colors.button_font_size)
         self.popup = Popup(title = "Select CSV or JSON file to import from",
                             content = content,
                             size_hint = (0.9, 0.9))
         self.popup.open()
 
+    def fix_suffix(self, data):
+        for record in data:
+            if 'SUFFIX' in record:
+                try:
+                    record['SUFFIX'] = int(record['SUFFIX'])
+                except ValueError:
+                    pass
+        return data
+
     def read_csv_file(self, full_filename):
         data = []
         with open(full_filename, newline='') as csvfile:
             reader = csv.DictReader(csvfile, quoting = csv.QUOTE_NONNUMERIC)
             for row in reader:
                 data.append(row)
-        fields = [field.upper() for field in reader.fieldnames]
-        return fields, data
+        return [field.upper() for field in reader.fieldnames], self.fix_suffix(data)
 
     def read_json_table(self, full_filename, data_type):
         data = []
         if data_type.upper() in ['DATUMS', 'UNITS', 'PRISMS']:
             data = TinyDB(full_filename).table(data_type.lower()).all()
         fields = data[0].keys() if data else []
         return fields, data
@@ -847,43 +884,62 @@
     def build_hash_unique_ids(self):
         hash = {}
         if self.data.db is not None:
             for record in self.data.db.table(self.data.table):
                 hash[self.get_unique_key(record)] = record.doc_id
         return hash
 
+    def fix_date_time(self, date, time):
+        if " " in date:
+            new_date = date[:date.find(' ')]
+        else:
+            new_date = date
+        if " " in time:
+            new_time = time[time.find(" "):]
+        else:
+            new_time = time
+        return new_date + new_time
+
     def import_these(self, data):
         record_count = 0
         replacements = 0
-        hash_unique_ids = self.build_hash_unique_ids()
         if self.data.db is not None:
+            hash_unique_ids = self.build_hash_unique_ids()
+            data_to_insert = []
             for item in data:
                 insert_record = {}
                 for key, value in item.items():
                     if key.upper() == "UNIT" and self.csv_data_type == "Units":
                         insert_record['NAME'] = value
-                    elif key.upper() == "DATE" and "TIME" in item:
-                        insert_record['DATE'] = value + " " + item['TIME']
+                    elif (key.upper() == "DATE" or key.upper() == "DAY") and "TIME" in item:
+                        insert_record['DATE'] = self.fix_date_time(value, item['TIME'])
+                    elif (key.upper() == "DATE" or key.upper() == "DAY") and "time" in item:
+                        insert_record['DATE'] = self.fix_date_time(value, item['time'])
                     else:
                         insert_record[key.upper()] = value
                 if self.csv_data_type in ['Datums', 'Prisms', 'Units']:
                     if insert_record['NAME'].strip():
                         if len(self.data.get_by_name(self.csv_data_type.lower(), insert_record['NAME'])) > 0:
                             self.data.delete_by_name(self.csv_data_type.lower(), insert_record['NAME'])
                             replacements += 1
-                        self.data.db.table(self.csv_data_type.lower()).insert(insert_record)
+                        data_to_insert.append(insert_record)
                 if self.csv_data_type == 'Points':
-                    new_docid = self.data.db.table(self.data.table).insert(insert_record)
+                    # new_docid = self.data.db.table(self.data.table).insert(insert_record)
                     hash_key = self.get_unique_key(insert_record)
                     if hash_key in hash_unique_ids:
                         duplicate_doc_id = hash_unique_ids[hash_key]
                         self.data.db.table(self.data.table).remove(doc_ids = [duplicate_doc_id])
                         replacements += 1
-                    hash_unique_ids[hash_key] = new_docid
+                    # hash_unique_ids[hash_key] = new_docid
+                    data_to_insert.append(insert_record)
                 record_count += 1
+            if self.csv_data_type == 'Points':
+                self.data.db.table(self.data.table).insert_multiple(data_to_insert)
+            else:
+                self.data.db.table(self.csv_data_type.lower()).insert_multiple(data_to_insert)
         return (record_count, replacements)
 
     def load_csv(self, path, filename):
         # TODO This routine does not properly import Units.  The unitfields need to be put into a separate table
         # TODO Need to write the routine to import actual data
         full_filename = os.path.join(path, filename[0])
         self.dismiss_popup()
@@ -913,20 +969,20 @@
         self.open_popup()
         return errors
 
     def add_point_record(self):
         new_record = {}
         new_record = self.fill_default_fields(new_record)
         if self.station.shot_type != 'continue':
+            new_record = self.fill_button_defaults(new_record)
             new_record = self.find_unit_and_fill_fields(new_record)
             new_record = self.fill_carry_fields(new_record)
             new_record = self.fill_link_fields(new_record)
             new_record = self.do_increments(new_record)
             new_record['SUFFIX'] = 0
-            new_record = self.fill_button_defaults(new_record)
         else:
             new_record = self.fill_empty_with_last(new_record)
             new_record['SUFFIX'] = int(self.get_last_value('SUFFIX')) + 1
 
         self.data.db.table(self.data.table).insert(new_record)
 
     def fill_empty_with_last(self, new_record):
@@ -1015,24 +1071,27 @@
             if field == 'DATE':
                 new_record['DATE'] = f'{datetime.now().replace(microsecond=0)}'
         return new_record
 
     def get_last_value(self, field_name):
         if self.data.db is not None:
             if len(self.data.db.table(self.data.table)) > 0:
-                last_record = self.data.db.table(self.data.table).all()[-1]
+                doc_ids = self.data.get_doc_ids(self.data.table)
+                last_record = self.data.db.table(self.data.table).get(doc_id = doc_ids[-1])
                 if last_record != []:
                     if field_name in last_record.keys():
                         return last_record[field_name]
         return None
 
     def get_last_numeric_value(self, field_name):
         if self.data.db is not None:
             if len(self.data.db.table(self.data.table)) > 0:
-                for record in reversed(self.data.db.table(self.data.table).all()):
+                doc_ids = self.data.get_doc_ids(self.data.table)
+                for doc_id in reversed(doc_ids):
+                    record = self.data.db.table(self.data.table).get(doc_id = doc_id)
                     if record != []:
                         if field_name in record.keys():
                             if self.is_numeric(record[field_name]):
                                 return record[field_name]
         return None
 
     def is_numeric(self, value):
@@ -1368,14 +1427,21 @@
         self.on_record = on_record
         self.datum1 = datum1
         self.datum2 = datum2
         self.datum3 = datum3
         self.data = data
         self.default_prism = prism()
 
+    def is_numeric(self, value):
+        try:
+            float(value)
+            return True
+        except ValueError:
+            return False
+
     def record_datum(self, instance):
         self.set_angle()
 
     def get_angle(self):
         if self.id == 'datum1':
             if self.setup_type == 'Over a datum + Record a datum':
                 if self.datum1.datum.is_none() or self.datum2.datum.is_none():
@@ -1389,15 +1455,15 @@
 
     def set_angle(self):
         angle = self.get_angle()
         if angle is not None:
             if self.station.make in ['Manual XYZ', 'Manual VHD']:
                 self.popup = e5_MessageBox('Set horizonal angle',
                                             f'\nAim at {self.datum1.datum.name} and set the horizontal angle '
-                                                'to {self.station.decimal_degrees_to_sexastr(angle)}.',
+                                                f'to {self.station.decimal_degrees_to_sexa_pretty(angle)}.',
                                             call_back = self.now_take_shot, colors = self.colors)
                 self.popup.open()
             elif self.station.make in ['Leica', 'Wild', 'Leica GeoCom', 'Sokkia', 'Topcon']:
                 self.popup = self.get_prism_height()
                 self.popup.open()
                 self.station.set_horizontal_angle(self.station.decimal_degrees_to_dddmmss(angle))
                 self.station.take_shot()
@@ -1419,31 +1485,36 @@
             # self.popup = DataGridTextBox(title = self.text + '.  Waiting on Microscribe...', button_text = ['Cancel', 'Next'], call_back = self.microscribe)
             self.popup = DataGridTextBox(title = 'EDM',
                                             label = self.text + '.  Waiting on...',
                                             text = '<Microscribe>',
                                             button_text = ['Cancel', 'Next'],
                                             call_back = self.microscribe,
                                             colors = self.colors)
-            self.popup.open()
+            self.popup.open()   
         elif self.station.make in ['Manual XYZ', 'Manual VHD']:
-            self.popup = edm_manual(call_back = self.have_shot_manual, colors = self.colors)
+            self.popup = edm_manual(type = self.station.make, call_back = self.have_shot_manual, colors = self.colors)
             self.popup.open()
 
     def have_shot_manual(self, instance):
-        # check that next was pressed and get values
-        p = self.station.text_to_point(f'{self.popup.xcoord.text},{self.popup.ycoord.text},{self.popup.zcoord.text}')
-        if p:
-            self.station.xyz = p
-            self.station.make_global()
-            self.station.vhd_from_xyz()
+        if self.station.make in ['Manual XYZ']:
+            if self.popup.valid_data():
+                p = self.station.text_to_point(f'{self.popup.xcoord.textbox.text},{self.popup.ycoord.textbox.text},{self.popup.zcoord.textbox.text}')
+                self.station.xyz = p
+                self.station.make_global()
+                self.station.vhd_from_xyz()
+            else:
+                self.station.xyz = point()
         else:
-            self.station.hangle = self.popup.hangle.text if isinstance(self.popup.hangle.text, int) or isinstance(self.popup.hangle.text, float) else ''
-            self.station.vangle = self.popup.vangle.text if isinstance(self.popup.vangle.text, int) or isinstance(self.popup.vangle.text, float) else ''
-            self.station.sloped = self.popup.sloped.text if isinstance(self.popup.sloped.text, int) or isinstance(self.popup.sloped.text, float) else ''
-            self.station.vhd_to_xyz()
+            if self.popup.valid_data():
+                self.station.hangle = self.station.dms_to_decdeg(self.popup.hangle.textbox.text)
+                self.station.vangle = self.station.dms_to_decdeg(self.popup.vangle.textbox.text)
+                self.station.sloped = float(self.popup.sloped.textbox.text)
+                self.station.vhd_to_xyz()
+            else:
+                self.station.xyz = point()
         self.popup.dismiss()
         self.popup = self.get_prism_height()
         self.popup.open()
 
     def get_prism_height(self):
         prism_names = self.data.names('prisms') if self.data else []
         if len(prism_names) > 0:
@@ -1500,22 +1571,22 @@
         # except ValueError:
         #    self.station.prism = prism(None, 0.0, None)
         self.default_prism = self.station.prism
 
         self.event = Clock.schedule_interval(self.check_for_station_response, .1)
 
     def check_for_station_response(self, dt):
-        if self.station.data_waiting():
+        if self.station.data_waiting() or self.station.make in ['Manual XYZ', 'Manual VHD']:
             if self.station.make in ['Leica']:
                 self.station.fetch_point()
             elif self.station.make in ['Leica GeoCom']:
                 self.station.fetch_point_leica_geocom()
             elif self.station.make in ['Topcon']:
                 self.station.fetch_point_topcon()
-            if self.station.response:
+            if self.station.response or self.station.make in ['Manual XYZ', 'Manual VHD']:
                 self.station.prism_adjust()
                 if self.station.xyz.x is not None and self.station.xyz.y is not None and self.station.xyz.z is not None:
                     self.station.make_global()
                     if self.setup_type == 'verify' or self.setup_type == 'record_new':
                         self.result_label.text = self.station.point_pretty(self.station.xyz_global)
                     else:
                         self.result_label.text = self.station.point_pretty(self.station.xyz)
@@ -1584,42 +1655,39 @@
         self.spacing = 10
         self.cols = 2
         self.colors = colors
         self.data = data
         self.datum = default_datum
         self.call_back = call_back
         self.size_hint_y = None
-        self.add_widget(e5_button(text = text,
-                                    selected = True,
-                                    call_back = self.show_select_datum,
-                                    colors = self.colors))
-        if not self.datum.is_none():
-            self.result = e5_label(f'Datum: {self.datum.name}\nX: {self.datum.x}\nY: {self.datum.y}\nZ: {self.datum.z}',
-                                    colors = self.colors, label_height = 100)
-        else:
-            self.result = e5_label('Datum:\nX:\nY:\nZ:', colors = self.colors)
+        self.add_widget(e5_button(text=text,
+                                    selected=True,
+                                    call_back=self.show_select_datum,
+                                    colors=self.colors))
+        label = f'Datum: {self.datum.name}\nX: {self.datum.x}\nY: {self.datum.y}\nZ: {self.datum.z}' if not self.datum.is_none() else 'Datum:\nX:\nY:\nZ:'
+        self.result = e5_label(label, colors=self.colors, label_height=100)
         self.add_widget(self.result)
 
     def show_select_datum(self, instance):
-        self.popup = DataGridMenuList(title = "Datum",
-                                        menu_list = self.data.names('datums'),
-                                        menu_selected = '',
-                                        call_back = self.datum_selected,
-                                        colors = self.colors)
+        self.popup = DataGridMenuList(title="Datum",
+                                        menu_list=self.data.names('datums'),
+                                        menu_selected='',
+                                        call_back=self.datum_selected,
+                                        colors=self.colors)
         self.popup.open()
 
     def datum_selected(self, instance):
         self.popup.dismiss()
         self.datum = self.data.get_datum(instance.text)
-        if not self.datum.is_none():
-            self.result.text = f'Datum: {self.datum.name}\nX: {self.datum.x}\nY: {self.datum.y}\nZ: {self.datum.z}'
-            if self.call_back:
-                self.call_back(self)
-        else:
+        if self.datum.is_none():
             self.result.text = 'Search error'
+            return
+        self.result.text = f'Datum: {self.datum.name}\nX: {self.datum.x}\nY: {self.datum.y}\nZ: {self.datum.z}'
+        if self.call_back:
+            self.call_back(self)
 
 
 class setups(ScrollView):
 
     id = ObjectProperty(None)
     popup = ObjectProperty(None)
     popup_open = False
@@ -1788,23 +1856,23 @@
                 Color(0.8, 0.8, 0.8, 1)
                 Rectangle(size=self.size, pos=self.pos)
 
         # self.bind(size = draw_background)
         # self.bind(pos = draw_background)
 
     def datum1_selected(self, instance):
-        self.recorder[0].children[1].text = 'Record ' + instance.datum.name
+        self.recorder[0].children[1].text = 'Record\n' + instance.datum.name
         self.recorder[0].children[1].datum_name = instance.datum.name
 
     def datum2_selected(self, instance):
-        self.recorder[1].children[1].text = 'Record ' + instance.datum.name
+        self.recorder[1].children[1].text = 'Record\n' + instance.datum.name
         self.recorder[1].children[1].datum_name = instance.datum.name
 
     def datum3_selected(self, instance):
-        self.recorder[2].children[1].text = 'Record ' + instance.datum.name
+        self.recorder[2].children[1].text = 'Record\n' + instance.datum.name
         self.recorder[2].children[1].datum_name = instance.datum.name
 
     def set_hangle(self, instance):
         if self.hangle:
             self.station.set_horizontal_angle(self.hangle.text)
             logger = logging.getLogger(__name__)
             logger.info(f'Horizontal angle set to {self.hangle.text}')
```

### Comparing `edm-arch-1.0.34/src/edmpy/geo.py` & `edm-arch-1.0.35/src/edmpy/geo.py`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.34/src/edmpy/ini.py` & `edm-arch-1.0.35/src/edmpy/ini.py`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.34/src/edmpy/lib/blockdata.py` & `edm-arch-1.0.35/src/edmpy/lib/blockdata.py`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.34/src/edmpy/lib/colorscheme.py` & `edm-arch-1.0.35/src/edmpy/lib/colorscheme.py`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.34/src/edmpy/lib/constants.py` & `edm-arch-1.0.35/src/edmpy/lib/constants.py`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.34/src/edmpy/lib/dbs.py` & `edm-arch-1.0.35/src/edmpy/lib/dbs.py`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.34/src/edmpy/lib/e5_widgets.py` & `edm-arch-1.0.35/src/edmpy/lib/e5_widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,29 @@
                                             colors = colors)
         self.call_back = call_back
         pop_content.add_widget(buttons)
         self.content = pop_content
         self.title = 'Manual Input'
         self.size_hint = (.9, height_calculator(280))
         self.auto_dismiss = True
+        self.type = type
 
+    def is_numeric(self, value):
+        try:
+            float(value)
+            return True
+        except ValueError:
+            return False
+
+    def valid_data(self):
+        if self.type == 'Manual XYZ':
+            return all([self.is_numeric(txt) for txt in [self.xcoord.textbox.text, self.ycoord.textbox.text, self.zcoord.textbox.text]])
+        elif self.type == 'Manual VHD':
+            return all([self.is_numeric(txt) for txt in [self.hangle.textbox.text, self.vangle.textbox.text, self.sloped.textbox.text]])
+        
     def on_open(self):
         if self.xcoord is not None:
             self.xcoord.focus = True
         elif self.hangle is not None:
             self.hangle.focus = True
 
     def next_field(self, instance):
@@ -1082,18 +1096,23 @@
 
     def __init__(self, data = None, **kwargs):
         super(e5_JSONScreen, self).__init__(**kwargs)
         self.data = data
 
     def on_pre_enter(self):
         self.content.text = 'The last 150 lines:\n\n'
-        with open(self.data.filename, 'r') as f:
-            content = f.readlines()
-        # self.content.text += ''.join(list(reversed(content))[0:150])
-        self.content.text += ''.join(list(content)[-150:])
+        try:
+            with open(self.data.filename, 'r') as f:
+                content = f.readlines()
+            # self.content.text += ''.join(list(reversed(content))[0:150])
+            self.content.text += ''.join(list(content)[-150:])
+        except TypeError:
+            self.content.text = "\nA database file has not yet been opened."
+        except OSError:
+            self.content.text = "\nAn error occurred when reading the data file '%s'." % (self.data.filename)
         self.content.color = self.colors.text_color
         self.back_button.background_color = self.colors.button_background
         self.back_button.color = self.colors.button_color
 
 
 class e5_LogScreen(e5_InfoScreen):
 
@@ -1286,15 +1305,15 @@
         self.filter_field = 'Unit-ID'
         self.loading = True
 
     def on_pre_enter(self):
         self.loading = True
         if self.data.table is not None and self.e5_cfg is not None:
             self.reset_doc_ids()
-            self.doc_id = self.doc_ids[-1] if self.doc_ids else None
+            self.doc_id = max(self.doc_ids) if self.doc_ids else None
         else:
             self.doc_ids = []
             self.doc_id = None
         self.put_data_in_frame()
 
     def on_enter(self):
         if self.first_field_widget:
@@ -1305,15 +1324,16 @@
     def on_leave(self):
         # This helps insure that saving on lost focus works properly
         # There is an issue this addresses with building the screens
         # at startup.
         self.loading = True
 
     def reset_doc_ids(self):
-        self.doc_ids = [r.doc_id for r in self.data.db.table(self.data.table).all()] if self.data.db is not None else []
+        print('reset ids')
+        self.doc_ids = sorted([r.doc_id for r in self.data.db.table(self.data.table).all()] if self.data.db is not None else [])
 
     def filter(self, instance):
         if instance.text == 'Clear Filter':
             instance.text = 'Filter'
             self.reset_doc_ids()
             self.last_record(None)
             # self.update_record_counter_label()
@@ -1329,21 +1349,22 @@
         elif filter_field == 'Unit-ID':
             for record in self.data.db.table(self.data.table):
                 if "UNIT" in record.keys() and "ID" in record.keys():
                     if f"{str(record['UNIT']).lower()}-{str(record['ID']).lower()}" == filter_value.lower():
                         matches.append(record.doc_id)
         else:
             for record in self.data.db.table(self.data.table):
-                if str(record[filter_field]).lower() == filter_value.lower():
-                    matches.append(record.doc_id)
+                if filter_field in record:
+                    if str(record[filter_field]).lower() == filter_value.lower():
+                        matches.append(record.doc_id)
         return matches
 
     def apply_filter(self, instance):
         self.filter_field = self.popup.fields_dropdown.text
-        filter_value = self.popup.value_input.text
+        filter_value = self.popup.value_input.textbox.text
         if filter_value and self.filter_field:
             self.doc_ids = self.get_matching_doc_ids(self.filter_field, filter_value)
             if self.doc_ids:
                 self.first_record(None)
             else:
                 self.clear_the_frame()
                 self.doc_id = None
@@ -1503,15 +1524,17 @@
         if self.doc_id and self.data.table and self.e5_cfg and self.can_update_data_table:
             update = {}
             for field in self.e5_cfg.fields():
                 for widget in self.layout.walk():
                     if hasattr(widget, 'id'):
                         if widget.id == field:
                             if self.e5_cfg.save_as_numeric_field(field):
-                                if '.' in widget.text:
+                                if widget.text == '':
+                                    update[widget.id] = 0
+                                elif '.' in widget.text:
                                     update[widget.id] = float(widget.text)
                                 else:
                                     update[widget.id] = int(widget.text)
                             else:
                                 update[widget.id] = widget.text
                             break
             self.data.db.table(self.data.table).update(update, doc_ids = [self.doc_id])
@@ -1561,22 +1584,30 @@
         for field in self.e5_cfg.unique_together:
             unique_key.append("%s" % data_record[field] if field in data_record else '')
         return ",".join(unique_key)
 
     def check_unique_together(self):
         save_errors = []
         if self.e5_cfg.unique_together and len(self.data.db.table(self.data.table)) > 1:
-            doc_ids = self.data.doc_ids()
+            # doc_ids = self.data.doc_ids()
             unique_key = self.get_unique_key(self.convert_widgets_to_record())
-            for doc_id in doc_ids[0:-1]:
-                if unique_key == self.get_unique_key(self.data.db.table(self.data.table).get(doc_id = doc_id)):
-                    save_errors.append("Based on the unique together field(s) %s, this record's unique key of %s duplicates the record with a doc_id of %s." %
-                                        (",".join(self.e5_cfg.unique_together), unique_key, doc_id))
-                    break
-        return save_errors
+            hits = []
+            for item in self.data.db.table(self.data.table).all():
+                if self.get_unique_key(item) == unique_key:
+                    hits.append(item)
+                    if len(hits) > 1:
+                        save_errors.append("Based on the unique together field(s) %s, this record's unique key of %s duplicates an existing record." %
+                                            (",".join(self.e5_cfg.unique_together), unique_key))
+                        return save_errors
+            if len(hits) == 1:
+                if hits[0] != self.data.db.table(self.data.table).get(doc_id = self.doc_id):
+                    save_errors.append("Based on the unique together field(s) %s, this record's unique key of %s duplicates an existing record." %
+                                        (",".join(self.e5_cfg.unique_together), unique_key))
+                    return save_errors
+        return []
 
     def check_numeric_fields(self):
         save_errors = []
         for field_name in self.e5_cfg.fields():
             field = self.e5_cfg.get(field_name)
             if field.inputtype in ['NUMERIC', 'INSTRUMENT']:
                 for widget in self.layout.walk():
@@ -3503,16 +3534,16 @@
     def check_unique_together(self, current_doc_id, new_record):
         unique_error = ''
         if self.cfg.unique_together and len(self.data) > 1:
             unique_key = self.get_unique_key(new_record)
             for record in self.data.all():
                 if record.doc_id != current_doc_id:
                     if unique_key == self.get_unique_key(record):
-                        unique_error = f'Based on the unique together field(s) {",".join(self.cfg.unique_together)}, '\
-                                        f'this record\'s unique key of {unique_key} duplicates another record.  This is not allowed.'
+                        unique_error = f'Based on the unique together field(s) {",".join(self.cfg.unique_together)}, '
+                        unique_error += f'this record\'s unique key of {unique_key} duplicates another record.  This is not allowed.'
                         break
         return unique_error
 
     def update_datagrid_record(self, doc_id, new_record):
         datatable = self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable')
         for record in datatable.data:
             if record['key'] == doc_id and record['field'] in new_record.keys():
```

### Comparing `edm-arch-1.0.34/src/edmpy/lib/misc.py` & `edm-arch-1.0.35/src/edmpy/lib/misc.py`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.34/src/edmpy/totalstation.py` & `edm-arch-1.0.35/src/edmpy/totalstation.py`

 * *Files 0% similar despite different names*

```diff
@@ -507,15 +507,15 @@
         self.serialcom.write_timeout = 5
         try:
             self.serialcom.open()
             self.clear_io()
             self.initialize()
         except OSError as err:
             self.error_code = 1
-            self.error_message = str(err)
+            self.error_message = str(err) + '\n\n'
         return self.error_message
 
     def settings_pretty(self):
         if self.baudrate and self.comport and self.parity and self.databits and self.stopbits:
             return f"{self.comport}:{self.baudrate},{self.parity},{self.databits},{self.stopbits}"
         else:
             return "Incomplete Settings"
```

