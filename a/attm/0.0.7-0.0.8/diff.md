# Comparing `tmp/attm-0.0.7-py3-none-win_amd64.whl.zip` & `tmp/attm-0.0.8-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 59953 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat      781 b- defN 23-May-24 02:15 attm/__init__.py
--rw-rw-rw-  2.0 fat      270 b- defN 23-May-23 23:24 attm/config.py
+Zip file size: 59954 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat      781 b- defN 23-May-24 02:23 attm/__init__.py
+-rw-rw-rw-  2.0 fat      270 b- defN 23-May-24 02:23 attm/config.py
 -rw-rw-rw-  2.0 fat     5529 b- defN 23-May-24 01:55 attm/main.py
 -rw-rw-rw-  2.0 fat     4399 b- defN 23-May-24 02:01 attm/utils.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-23 23:24 attm/res/__init__.py
 -rw-rw-rw-  2.0 fat       12 b- defN 23-May-23 23:24 attm/res/holiday.txt
 -rw-rw-rw-  2.0 fat    10319 b- defN 23-May-23 23:24 attm/res/icon.ico
 -rw-rw-rw-  2.0 fat    42402 b- defN 23-May-23 23:24 attm/res/icon.png
--rw-rw-rw-  2.0 fat     1087 b- defN 23-May-24 02:22 attm-0.0.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3206 b- defN 23-May-24 02:22 attm-0.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       98 b- defN 23-May-24 02:22 attm-0.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       41 b- defN 23-May-24 02:22 attm-0.0.7.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        5 b- defN 23-May-24 02:22 attm-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1042 b- defN 23-May-24 02:22 attm-0.0.7.dist-info/RECORD
-14 files, 69191 bytes uncompressed, 58247 bytes compressed:  15.8%
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-May-24 02:23 attm-0.0.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3206 b- defN 23-May-24 02:23 attm-0.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       98 b- defN 23-May-24 02:23 attm-0.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       41 b- defN 23-May-24 02:23 attm-0.0.8.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        5 b- defN 23-May-24 02:23 attm-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1042 b- defN 23-May-24 02:23 attm-0.0.8.dist-info/RECORD
+14 files, 69191 bytes uncompressed, 58248 bytes compressed:  15.8%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: attm/res/icon.ico
 Comment: 
 
 Filename: attm/res/icon.png
 Comment: 
 
-Filename: attm-0.0.7.dist-info/LICENSE
+Filename: attm-0.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: attm-0.0.7.dist-info/METADATA
+Filename: attm-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: attm-0.0.7.dist-info/WHEEL
+Filename: attm-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: attm-0.0.7.dist-info/entry_points.txt
+Filename: attm-0.0.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: attm-0.0.7.dist-info/top_level.txt
+Filename: attm-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: attm-0.0.7.dist-info/RECORD
+Filename: attm-0.0.8.dist-info/RECORD
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
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 
 # Path
 PACKAGE = pathlib.Path(attm.__path__[0]).resolve()
 VENV = PACKAGE.parent.parent.parent
 ROOT = VENV.parent
 ACTIVATE = VENV.joinpath("Scripts", "activate.bat")
```

## attm/config.py

```diff
@@ -1,10 +1,10 @@
 # 수정 후 프로그램을 재시작 해주세요!
 # 재시작해야 변경 사항이 반영됩니다.
 
 # 프로그램 설정
-start_delay_secs = 7
+start_delay_secs = 2
 
 # 내장 스케줄러 설정
 schedule_work_in = '08:49'
 schedule_work_out = '18:01'
 schedule_update = '12:00'
```

## Comparing `attm-0.0.7.dist-info/LICENSE` & `attm-0.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `attm-0.0.7.dist-info/METADATA` & `attm-0.0.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attm
-Version: 0.0.7
+Version: 0.0.8
 Summary: Attendance Manager (근태 관리자)
 Home-page: https://github.com/syshin-cubox-ai/attm
 Author: synml
 Author-email: kistssy@gmail.com
 License: MIT
 Platform: Windows
 Requires-Python: >=3.9
```

## Comparing `attm-0.0.7.dist-info/RECORD` & `attm-0.0.8.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-attm/__init__.py,sha256=OHRvtj_hckhnxkJx97jmZnr59caCwnorN6Idfa_qCWM,781
-attm/config.py,sha256=PrBh0oXGw0wfoO1yVsVysLxdU5shGd5znWvifDBQGvw,270
+attm/__init__.py,sha256=PhhpkrT2u5VcfD4edLXFrySlvXtG1hoYPoV09aJ51Cc,781
+attm/config.py,sha256=WUlSOjY4uOYiMzeX1CGVriAERzyk8v2nHJzJcpon59Q,270
 attm/main.py,sha256=rcy6QVbuHUZ0u7Sx1KhBSXBObwkmvGDmLaecv0qRmnw,5529
 attm/utils.py,sha256=kQWQsVgR9tXy6CP2bcWbLYmDK5yOPEbUONVnGf_y808,4399
 attm/res/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 attm/res/holiday.txt,sha256=YsBJe_keJKkWXKO4VKsr4SYHtyZ_2ljyFu56jNWSVPA,12
 attm/res/icon.ico,sha256=MbVMT8FDlWKnACScVY6rSqd7VqGaBIdWacEPVr9hlMo,10319
 attm/res/icon.png,sha256=cTDQURXYUYT589rJFCjtXE1VKg1awFggf98yufC5l9I,42402
-attm-0.0.7.dist-info/LICENSE,sha256=xuOueRZ-vxAHBM2drSHAqA2erzepHIKYnsTtTswGW9w,1087
-attm-0.0.7.dist-info/METADATA,sha256=LJfc4jX7MKUJVXnWVTYClQYnuixWUBeKy9sXoXn1HCQ,3206
-attm-0.0.7.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
-attm-0.0.7.dist-info/entry_points.txt,sha256=aJks8Y8rsYdDWz5kIZsMjPGhvhUDKj846hu-hVSVciM,41
-attm-0.0.7.dist-info/top_level.txt,sha256=qIstk_4xcvIgjsAC4OIWbMmJ2-q5qhP-9JL8YyGMezg,5
-attm-0.0.7.dist-info/RECORD,,
+attm-0.0.8.dist-info/LICENSE,sha256=xuOueRZ-vxAHBM2drSHAqA2erzepHIKYnsTtTswGW9w,1087
+attm-0.0.8.dist-info/METADATA,sha256=P8p4D8n0lr6mjRbb_JTbOB-_4J5c6MeyvW8x1T9cWNk,3206
+attm-0.0.8.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
+attm-0.0.8.dist-info/entry_points.txt,sha256=aJks8Y8rsYdDWz5kIZsMjPGhvhUDKj846hu-hVSVciM,41
+attm-0.0.8.dist-info/top_level.txt,sha256=qIstk_4xcvIgjsAC4OIWbMmJ2-q5qhP-9JL8YyGMezg,5
+attm-0.0.8.dist-info/RECORD,,
```

