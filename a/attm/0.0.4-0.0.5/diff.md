# Comparing `tmp/attm-0.0.4-py3-none-win_amd64.whl.zip` & `tmp/attm-0.0.5-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 59985 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat      781 b- defN 23-May-24 01:40 attm/__init__.py
+Zip file size: 59995 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat      781 b- defN 23-May-24 01:46 attm/__init__.py
 -rw-rw-rw-  2.0 fat      270 b- defN 23-May-23 23:24 attm/config.py
 -rw-rw-rw-  2.0 fat     5529 b- defN 23-May-24 00:53 attm/main.py
--rw-rw-rw-  2.0 fat     4455 b- defN 23-May-24 01:38 attm/utils.py
+-rw-rw-rw-  2.0 fat     4480 b- defN 23-May-24 01:45 attm/utils.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-23 23:24 attm/res/__init__.py
 -rw-rw-rw-  2.0 fat       12 b- defN 23-May-23 23:24 attm/res/holiday.txt
 -rw-rw-rw-  2.0 fat    10319 b- defN 23-May-23 23:24 attm/res/icon.ico
 -rw-rw-rw-  2.0 fat    42402 b- defN 23-May-23 23:24 attm/res/icon.png
--rw-rw-rw-  2.0 fat     1087 b- defN 23-May-24 01:40 attm-0.0.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3206 b- defN 23-May-24 01:40 attm-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       98 b- defN 23-May-24 01:40 attm-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       41 b- defN 23-May-24 01:40 attm-0.0.4.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        5 b- defN 23-May-24 01:40 attm-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1042 b- defN 23-May-24 01:40 attm-0.0.4.dist-info/RECORD
-14 files, 69247 bytes uncompressed, 58279 bytes compressed:  15.8%
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-May-24 01:46 attm-0.0.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3206 b- defN 23-May-24 01:46 attm-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       98 b- defN 23-May-24 01:46 attm-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       41 b- defN 23-May-24 01:46 attm-0.0.5.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        5 b- defN 23-May-24 01:46 attm-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1042 b- defN 23-May-24 01:46 attm-0.0.5.dist-info/RECORD
+14 files, 69272 bytes uncompressed, 58289 bytes compressed:  15.9%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: attm/res/icon.ico
 Comment: 
 
 Filename: attm/res/icon.png
 Comment: 
 
-Filename: attm-0.0.4.dist-info/LICENSE
+Filename: attm-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: attm-0.0.4.dist-info/METADATA
+Filename: attm-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: attm-0.0.4.dist-info/WHEEL
+Filename: attm-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: attm-0.0.4.dist-info/entry_points.txt
+Filename: attm-0.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: attm-0.0.4.dist-info/top_level.txt
+Filename: attm-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: attm-0.0.4.dist-info/RECORD
+Filename: attm-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## attm/__init__.py

```diff
@@ -1,14 +1,14 @@
 import argparse
 import pathlib
 import shutil
 
 import attm.utils
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 
 # Path
 PACKAGE = pathlib.Path(attm.__path__[0]).resolve()
 VENV = PACKAGE.parent.parent.parent
 ROOT = VENV.parent
 ACTIVATE = VENV.joinpath("Scripts", "activate.bat")
```

## attm/utils.py

```diff
@@ -106,15 +106,15 @@
 
 
 def open_code_dir() -> None:
     subprocess.Popen('start .', shell=True)
 
 
 def show_log() -> None:
-    subprocess.Popen('notepad attm.log', shell=True)
+    subprocess.Popen(f'notepad {attm.ROOT.joinpath("attm.log")}', shell=True)
 
 
 def info() -> str:
     return f"""
 버전: {attm.VERSION}
 OS: {platform.platform()}
 Copyright ⓒ {datetime.datetime.now().year}. Seokyong Shin
```

## Comparing `attm-0.0.4.dist-info/LICENSE` & `attm-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `attm-0.0.4.dist-info/METADATA` & `attm-0.0.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attm
-Version: 0.0.4
+Version: 0.0.5
 Summary: Attendance Manager (근태 관리자)
 Home-page: https://github.com/syshin-cubox-ai/attm
 Author: synml
 Author-email: kistssy@gmail.com
 License: MIT
 Platform: Windows
 Requires-Python: >=3.9
```

