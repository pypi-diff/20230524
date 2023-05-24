# Comparing `tmp/attm-0.0.3-py3-none-win_amd64.whl.zip` & `tmp/attm-0.0.4-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 60058 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat      718 b- defN 23-May-24 01:20 attm/__init__.py
+Zip file size: 59985 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat      781 b- defN 23-May-24 01:40 attm/__init__.py
 -rw-rw-rw-  2.0 fat      270 b- defN 23-May-23 23:24 attm/config.py
 -rw-rw-rw-  2.0 fat     5529 b- defN 23-May-24 00:53 attm/main.py
--rw-rw-rw-  2.0 fat     4967 b- defN 23-May-24 01:20 attm/utils.py
+-rw-rw-rw-  2.0 fat     4455 b- defN 23-May-24 01:38 attm/utils.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-23 23:24 attm/res/__init__.py
 -rw-rw-rw-  2.0 fat       12 b- defN 23-May-23 23:24 attm/res/holiday.txt
 -rw-rw-rw-  2.0 fat    10319 b- defN 23-May-23 23:24 attm/res/icon.ico
 -rw-rw-rw-  2.0 fat    42402 b- defN 23-May-23 23:24 attm/res/icon.png
--rw-rw-rw-  2.0 fat     1087 b- defN 23-May-24 01:23 attm-0.0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3206 b- defN 23-May-24 01:23 attm-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       98 b- defN 23-May-24 01:23 attm-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       41 b- defN 23-May-24 01:23 attm-0.0.3.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        5 b- defN 23-May-24 01:23 attm-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1042 b- defN 23-May-24 01:23 attm-0.0.3.dist-info/RECORD
-14 files, 69696 bytes uncompressed, 58352 bytes compressed:  16.3%
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-May-24 01:40 attm-0.0.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3206 b- defN 23-May-24 01:40 attm-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       98 b- defN 23-May-24 01:40 attm-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       41 b- defN 23-May-24 01:40 attm-0.0.4.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        5 b- defN 23-May-24 01:40 attm-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1042 b- defN 23-May-24 01:40 attm-0.0.4.dist-info/RECORD
+14 files, 69247 bytes uncompressed, 58279 bytes compressed:  15.8%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: attm/res/icon.ico
 Comment: 
 
 Filename: attm/res/icon.png
 Comment: 
 
-Filename: attm-0.0.3.dist-info/LICENSE
+Filename: attm-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: attm-0.0.3.dist-info/METADATA
+Filename: attm-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: attm-0.0.3.dist-info/WHEEL
+Filename: attm-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: attm-0.0.3.dist-info/entry_points.txt
+Filename: attm-0.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: attm-0.0.3.dist-info/top_level.txt
+Filename: attm-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: attm-0.0.3.dist-info/RECORD
+Filename: attm-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## attm/__init__.py

```diff
@@ -1,17 +1,20 @@
 import argparse
 import pathlib
 import shutil
 
 import attm.utils
 
+VERSION = '0.0.4'
+
+# Path
 PACKAGE = pathlib.Path(attm.__path__[0]).resolve()
 VENV = PACKAGE.parent.parent.parent
 ROOT = VENV.parent
-VERSION = '0.0.3'
+ACTIVATE = VENV.joinpath("Scripts", "activate.bat")
 
 
 def entrypoint():
     parser = argparse.ArgumentParser()
     parser.add_argument('task', type=str, help='Perform initial setup. (init, start)')
     args = parser.parse_args()
```

## attm/utils.py

```diff
@@ -40,16 +40,16 @@
     account = cryptography.fernet.Fernet(privkey).decrypt(token)
     account = json.loads(account)
     return account
 
 
 def create_lnk_file():
     subprocess.run(
-        f'{attm.VENV.joinpath("Scripts", "activate.bat")} && '
-        f'pylnk3 create {attm.ROOT.joinpath("Scripts", "pythonw.exe")} '
+        f'{attm.ACTIVATE} && '
+        f'pylnk3 create {attm.VENV.joinpath("Scripts", "pythonw.exe")} '
         f'"근태 관리자.lnk" '
         f'--arguments main.py '
         f'--icon {attm.PACKAGE.joinpath("res", "icon.ico")} '
         f'--workdir {attm.PACKAGE}',
         shell=True, check=True
     )
     startup_path = pathlib.Path('~').expanduser().joinpath(
@@ -78,40 +78,32 @@
 
 def update(icon: pystray.Icon) -> None:
     try:
         logging.info('업데이트 확인...')
         icon.notify('업데이트 확인...')
         updated = False
 
-        # 코드 업데이트
-        stdout = subprocess.run('git reset --hard && git pull -p -t',
-                                shell=True, capture_output=True, check=True, encoding='utf-8').stdout
-        if stdout.find('Already up to date.') == -1:
-            updated = True
-            logging.info('코드를 업데이트했습니다.')
-            icon.notify('코드를 업데이트했습니다.')
-
         # 패키지 업데이트
         stdout = subprocess.run(
-            'venv\\Scripts\\activate.bat && pip list --disable-pip-version-check --outdated --format json',
+            f'{attm.ACTIVATE} && pip list --disable-pip-version-check --outdated --format json',
             shell=True, capture_output=True, check=True, encoding='utf-8').stdout
         outdated_packages = [i['name'] for i in json.loads(stdout)]
         if len(outdated_packages) > 0:
-            subprocess.run('venv\\Scripts\\activate.bat && python -m pip install -U ' + ' '.join(outdated_packages),
+            subprocess.run(f'{attm.ACTIVATE} && python -m pip install -U ' + ' '.join(outdated_packages),
                            shell=True, check=True)
             updated = True
             logging.info(f'다음 패키지를 업데이트했습니다: {outdated_packages}')
             icon.notify(f'다음 패키지를 업데이트했습니다: {outdated_packages}')
 
         # 업데이트한 경우 재시작, 최신인 경우 알림
         if updated:
             restart(icon)
         else:
-            logging.info('코드와 패키지 모두 최신입니다.')
-            icon.notify('코드와 패키지 모두 최신입니다.')
+            logging.info('최신 버전입니다.')
+            icon.notify('최신 버전입니다.')
     except subprocess.CalledProcessError as e:
         logging.error(traceback.format_exc())
         icon.notify(f'오류 발생: {e}\n자세한 내용은 로그를 참조하세요.')
 
 
 def open_code_dir() -> None:
     subprocess.Popen('start .', shell=True)
```

## Comparing `attm-0.0.3.dist-info/LICENSE` & `attm-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `attm-0.0.3.dist-info/METADATA` & `attm-0.0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attm
-Version: 0.0.3
+Version: 0.0.4
 Summary: Attendance Manager (근태 관리자)
 Home-page: https://github.com/syshin-cubox-ai/attm
 Author: synml
 Author-email: kistssy@gmail.com
 License: MIT
 Platform: Windows
 Requires-Python: >=3.9
```

