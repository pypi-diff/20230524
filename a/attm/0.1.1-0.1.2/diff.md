# Comparing `tmp/attm-0.1.1-py3-none-win_amd64.whl.zip` & `tmp/attm-0.1.2-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 59957 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat     1011 b- defN 23-May-24 07:31 attm/__init__.py
+Zip file size: 59960 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat     1011 b- defN 23-May-24 07:32 attm/__init__.py
 -rw-rw-rw-  2.0 fat     5613 b- defN 23-May-24 07:01 attm/main.py
 -rw-rw-rw-  2.0 fat     4333 b- defN 23-May-24 07:28 attm/utils.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-23 23:24 attm/res/__init__.py
 -rw-rw-rw-  2.0 fat      188 b- defN 23-May-24 07:00 attm/res/config.yaml
 -rw-rw-rw-  2.0 fat       12 b- defN 23-May-24 06:49 attm/res/holiday.txt
 -rw-rw-rw-  2.0 fat    10319 b- defN 23-May-23 23:24 attm/res/icon.ico
 -rw-rw-rw-  2.0 fat    42402 b- defN 23-May-23 23:24 attm/res/icon.png
--rw-rw-rw-  2.0 fat     1087 b- defN 23-May-24 07:31 attm-0.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3229 b- defN 23-May-24 07:31 attm-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       98 b- defN 23-May-24 07:31 attm-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       41 b- defN 23-May-24 07:31 attm-0.1.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        5 b- defN 23-May-24 07:31 attm-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1049 b- defN 23-May-24 07:31 attm-0.1.1.dist-info/RECORD
-14 files, 69387 bytes uncompressed, 58239 bytes compressed:  16.1%
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-May-24 07:32 attm-0.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3229 b- defN 23-May-24 07:32 attm-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       98 b- defN 23-May-24 07:32 attm-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       41 b- defN 23-May-24 07:32 attm-0.1.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        5 b- defN 23-May-24 07:32 attm-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1049 b- defN 23-May-24 07:32 attm-0.1.2.dist-info/RECORD
+14 files, 69387 bytes uncompressed, 58242 bytes compressed:  16.1%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: attm/res/icon.ico
 Comment: 
 
 Filename: attm/res/icon.png
 Comment: 
 
-Filename: attm-0.1.1.dist-info/LICENSE
+Filename: attm-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: attm-0.1.1.dist-info/METADATA
+Filename: attm-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: attm-0.1.1.dist-info/WHEEL
+Filename: attm-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: attm-0.1.1.dist-info/entry_points.txt
+Filename: attm-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: attm-0.1.1.dist-info/top_level.txt
+Filename: attm-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: attm-0.1.1.dist-info/RECORD
+Filename: attm-0.1.2.dist-info/RECORD
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
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 
 # Path
 PACKAGE = pathlib.Path(attm.__path__[0]).resolve()
 VENV = PACKAGE.parent.parent.parent
 ROOT = VENV.parent
 ACTIVATE = VENV.joinpath("Scripts", "activate.bat")
 STARTUP = pathlib.Path('~').expanduser().joinpath(
```

## Comparing `attm-0.1.1.dist-info/LICENSE` & `attm-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `attm-0.1.1.dist-info/METADATA` & `attm-0.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attm
-Version: 0.1.1
+Version: 0.1.2
 Summary: Attendance Manager (근태 관리자)
 Home-page: https://github.com/syshin-cubox-ai/attm
 Author: synml
 Author-email: kistssy@gmail.com
 License: MIT
 Platform: Windows
 Requires-Python: >=3.9
```

## Comparing `attm-0.1.1.dist-info/RECORD` & `attm-0.1.2.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-attm/__init__.py,sha256=EPorWNgnnMk1Fd76gjfxtn5S1bfi-lQyJ6uMBQexSiM,1011
+attm/__init__.py,sha256=8ugncnrf16H4qFKsyMLbwpgac4AD5kgmmolf02nH8qc,1011
 attm/main.py,sha256=hZ0tzDQy-5yLfwOj0ZAipcCim8LyRBPZAGMr8EL4CVM,5613
 attm/utils.py,sha256=vxc83sEQdod1M4w0Tg7id0zjxFHCQfRNOC2cWw_UmdE,4333
 attm/res/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 attm/res/config.yaml,sha256=wZqCXakTZovK35VpIdR4UC-TzDlnj0Lr-VU3v7ubDLo,188
 attm/res/holiday.txt,sha256=YsBJe_keJKkWXKO4VKsr4SYHtyZ_2ljyFu56jNWSVPA,12
 attm/res/icon.ico,sha256=MbVMT8FDlWKnACScVY6rSqd7VqGaBIdWacEPVr9hlMo,10319
 attm/res/icon.png,sha256=cTDQURXYUYT589rJFCjtXE1VKg1awFggf98yufC5l9I,42402
-attm-0.1.1.dist-info/LICENSE,sha256=xuOueRZ-vxAHBM2drSHAqA2erzepHIKYnsTtTswGW9w,1087
-attm-0.1.1.dist-info/METADATA,sha256=r8NphOLz-HOG9q-y6tr-F9zHUsk-GyE-jT4fA83FCFA,3229
-attm-0.1.1.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
-attm-0.1.1.dist-info/entry_points.txt,sha256=aJks8Y8rsYdDWz5kIZsMjPGhvhUDKj846hu-hVSVciM,41
-attm-0.1.1.dist-info/top_level.txt,sha256=qIstk_4xcvIgjsAC4OIWbMmJ2-q5qhP-9JL8YyGMezg,5
-attm-0.1.1.dist-info/RECORD,,
+attm-0.1.2.dist-info/LICENSE,sha256=xuOueRZ-vxAHBM2drSHAqA2erzepHIKYnsTtTswGW9w,1087
+attm-0.1.2.dist-info/METADATA,sha256=vsLw00UosakKLbpgnFw-lnKqy_aWFPUYJGbZZGEOREg,3229
+attm-0.1.2.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
+attm-0.1.2.dist-info/entry_points.txt,sha256=aJks8Y8rsYdDWz5kIZsMjPGhvhUDKj846hu-hVSVciM,41
+attm-0.1.2.dist-info/top_level.txt,sha256=qIstk_4xcvIgjsAC4OIWbMmJ2-q5qhP-9JL8YyGMezg,5
+attm-0.1.2.dist-info/RECORD,,
```

