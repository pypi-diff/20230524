# Comparing `tmp/attm-0.0.8-py3-none-win_amd64.whl.zip` & `tmp/attm-0.0.9-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 59954 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat      781 b- defN 23-May-24 02:23 attm/__init__.py
+Zip file size: 59942 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat      934 b- defN 23-May-24 04:25 attm/__init__.py
 -rw-rw-rw-  2.0 fat      270 b- defN 23-May-24 02:23 attm/config.py
 -rw-rw-rw-  2.0 fat     5529 b- defN 23-May-24 01:55 attm/main.py
--rw-rw-rw-  2.0 fat     4399 b- defN 23-May-24 02:01 attm/utils.py
+-rw-rw-rw-  2.0 fat     4141 b- defN 23-May-24 04:26 attm/utils.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-23 23:24 attm/res/__init__.py
 -rw-rw-rw-  2.0 fat       12 b- defN 23-May-23 23:24 attm/res/holiday.txt
 -rw-rw-rw-  2.0 fat    10319 b- defN 23-May-23 23:24 attm/res/icon.ico
 -rw-rw-rw-  2.0 fat    42402 b- defN 23-May-23 23:24 attm/res/icon.png
--rw-rw-rw-  2.0 fat     1087 b- defN 23-May-24 02:23 attm-0.0.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3206 b- defN 23-May-24 02:23 attm-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       98 b- defN 23-May-24 02:23 attm-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       41 b- defN 23-May-24 02:23 attm-0.0.8.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        5 b- defN 23-May-24 02:23 attm-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1042 b- defN 23-May-24 02:23 attm-0.0.8.dist-info/RECORD
-14 files, 69191 bytes uncompressed, 58248 bytes compressed:  15.8%
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-May-24 04:28 attm-0.0.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3206 b- defN 23-May-24 04:28 attm-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       98 b- defN 23-May-24 04:28 attm-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       41 b- defN 23-May-24 04:28 attm-0.0.9.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        5 b- defN 23-May-24 04:28 attm-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1042 b- defN 23-May-24 04:28 attm-0.0.9.dist-info/RECORD
+14 files, 69086 bytes uncompressed, 58236 bytes compressed:  15.7%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: attm/res/icon.ico
 Comment: 
 
 Filename: attm/res/icon.png
 Comment: 
 
-Filename: attm-0.0.8.dist-info/LICENSE
+Filename: attm-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: attm-0.0.8.dist-info/METADATA
+Filename: attm-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: attm-0.0.8.dist-info/WHEEL
+Filename: attm-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: attm-0.0.8.dist-info/entry_points.txt
+Filename: attm-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: attm-0.0.8.dist-info/top_level.txt
+Filename: attm-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: attm-0.0.8.dist-info/RECORD
+Filename: attm-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## attm/__init__.py

```diff
@@ -1,20 +1,24 @@
 import argparse
 import pathlib
 import shutil
 
 import attm.utils
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 
 # Path
 PACKAGE = pathlib.Path(attm.__path__[0]).resolve()
 VENV = PACKAGE.parent.parent.parent
 ROOT = VENV.parent
 ACTIVATE = VENV.joinpath("Scripts", "activate.bat")
+STARTUP = pathlib.Path('~').expanduser().joinpath(
+    'AppData/Roaming/Microsoft/Windows/Start Menu/Programs/Startup'
+)
+START_MENU = STARTUP.parent
 
 
 def entrypoint():
     parser = argparse.ArgumentParser()
     parser.add_argument('task', type=str, help='Perform initial setup. (init, start)')
     args = parser.parse_args()
```

## attm/utils.py

```diff
@@ -1,12 +1,11 @@
 import datetime
 import json
 import logging
 import os
-import pathlib
 import platform
 import shutil
 import subprocess
 import sys
 import traceback
 
 import chromedriver_autoinstaller
@@ -48,20 +47,16 @@
         f'pylnk3 create {attm.VENV.joinpath("Scripts", "pythonw.exe")} '
         f'"근태 관리자.lnk" '
         f'--arguments main.py '
         f'--icon {attm.PACKAGE.joinpath("res", "icon.ico")} '
         f'--workdir {attm.PACKAGE}',
         shell=True, check=True
     )
-    startup_path = pathlib.Path('~').expanduser().joinpath(
-        'AppData/Roaming/Microsoft/Windows/Start Menu/Programs/Startup'
-    )
-    start_menu_path = startup_path.parent
-    shutil.copy('근태 관리자.lnk', startup_path)
-    shutil.copy('근태 관리자.lnk', start_menu_path)
+    shutil.copy('근태 관리자.lnk', attm.STARTUP)
+    shutil.copy('근태 관리자.lnk', attm.START_MENU)
     os.remove('근태 관리자.lnk')
 
 
 def create_chrome_instance(url: str, headless: bool) -> WebDriver:
     chromedriver_autoinstaller.install(cwd=True)
 
     options = selenium.webdriver.ChromeOptions()
@@ -88,19 +83,21 @@
         outdated_packages = [i['name'] for i in json.loads(stdout)]
 
         # 패키지 업데이트 수행
         if len(outdated_packages) == 0:
             logging.info('최신 버전입니다.')
             icon.notify('최신 버전입니다.')
         else:
-            subprocess.run(f'{attm.ACTIVATE} && python -m pip install -U ' + ' '.join(outdated_packages),
-                           shell=True, check=True)
-            logging.info(f'다음 패키지를 업데이트했습니다: {outdated_packages}')
-            icon.notify(f'다음 패키지를 업데이트했습니다: {outdated_packages}')
-            restart(icon)
+            subprocess.Popen(
+                f'timeout 3 > nul && '
+                f'{attm.ACTIVATE} && '
+                f'python -m pip install -U {" ".join(outdated_packages)} && '
+                f'{attm.STARTUP.joinpath("근태 관리자.lnk")}',
+                shell=True)
+            exit_action(icon)
 
     except subprocess.CalledProcessError as e:
         logging.error(traceback.format_exc())
         icon.notify(f'오류 발생: {e}\n자세한 내용은 로그를 참조하세요.')
 
 
 def open_root_dir() -> None:
```

## Comparing `attm-0.0.8.dist-info/LICENSE` & `attm-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `attm-0.0.8.dist-info/METADATA` & `attm-0.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attm
-Version: 0.0.8
+Version: 0.0.9
 Summary: Attendance Manager (근태 관리자)
 Home-page: https://github.com/syshin-cubox-ai/attm
 Author: synml
 Author-email: kistssy@gmail.com
 License: MIT
 Platform: Windows
 Requires-Python: >=3.9
```

## Comparing `attm-0.0.8.dist-info/RECORD` & `attm-0.0.9.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-attm/__init__.py,sha256=PhhpkrT2u5VcfD4edLXFrySlvXtG1hoYPoV09aJ51Cc,781
+attm/__init__.py,sha256=QhIVsmVZcLixRxrsRFYbqr4XCzXONOi-qLB40rqt9Bc,934
 attm/config.py,sha256=WUlSOjY4uOYiMzeX1CGVriAERzyk8v2nHJzJcpon59Q,270
 attm/main.py,sha256=rcy6QVbuHUZ0u7Sx1KhBSXBObwkmvGDmLaecv0qRmnw,5529
-attm/utils.py,sha256=kQWQsVgR9tXy6CP2bcWbLYmDK5yOPEbUONVnGf_y808,4399
+attm/utils.py,sha256=aSftHc0H7Tg4iSc12yOW1vC8sun6Wh37Z5B4jF9rvAM,4141
 attm/res/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 attm/res/holiday.txt,sha256=YsBJe_keJKkWXKO4VKsr4SYHtyZ_2ljyFu56jNWSVPA,12
 attm/res/icon.ico,sha256=MbVMT8FDlWKnACScVY6rSqd7VqGaBIdWacEPVr9hlMo,10319
 attm/res/icon.png,sha256=cTDQURXYUYT589rJFCjtXE1VKg1awFggf98yufC5l9I,42402
-attm-0.0.8.dist-info/LICENSE,sha256=xuOueRZ-vxAHBM2drSHAqA2erzepHIKYnsTtTswGW9w,1087
-attm-0.0.8.dist-info/METADATA,sha256=P8p4D8n0lr6mjRbb_JTbOB-_4J5c6MeyvW8x1T9cWNk,3206
-attm-0.0.8.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
-attm-0.0.8.dist-info/entry_points.txt,sha256=aJks8Y8rsYdDWz5kIZsMjPGhvhUDKj846hu-hVSVciM,41
-attm-0.0.8.dist-info/top_level.txt,sha256=qIstk_4xcvIgjsAC4OIWbMmJ2-q5qhP-9JL8YyGMezg,5
-attm-0.0.8.dist-info/RECORD,,
+attm-0.0.9.dist-info/LICENSE,sha256=xuOueRZ-vxAHBM2drSHAqA2erzepHIKYnsTtTswGW9w,1087
+attm-0.0.9.dist-info/METADATA,sha256=wEaRliLCRsdziO_A7fekGy-gLDmHJ77qB-nANr2wlL8,3206
+attm-0.0.9.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
+attm-0.0.9.dist-info/entry_points.txt,sha256=aJks8Y8rsYdDWz5kIZsMjPGhvhUDKj846hu-hVSVciM,41
+attm-0.0.9.dist-info/top_level.txt,sha256=qIstk_4xcvIgjsAC4OIWbMmJ2-q5qhP-9JL8YyGMezg,5
+attm-0.0.9.dist-info/RECORD,,
```

