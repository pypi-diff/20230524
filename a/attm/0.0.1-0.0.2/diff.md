# Comparing `tmp/attm-0.0.1-py3-none-win_amd64.whl.zip` & `tmp/attm-0.0.2-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 60056 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat      723 b- defN 23-May-23 23:24 attm/__init__.py
+Zip file size: 60061 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat      743 b- defN 23-May-24 00:57 attm/__init__.py
 -rw-rw-rw-  2.0 fat      270 b- defN 23-May-23 23:24 attm/config.py
--rw-rw-rw-  2.0 fat     5514 b- defN 23-May-23 23:24 attm/main.py
--rw-rw-rw-  2.0 fat     4997 b- defN 23-May-23 23:56 attm/utils.py
+-rw-rw-rw-  2.0 fat     5529 b- defN 23-May-24 00:53 attm/main.py
+-rw-rw-rw-  2.0 fat     4977 b- defN 23-May-24 00:50 attm/utils.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-23 23:24 attm/res/__init__.py
 -rw-rw-rw-  2.0 fat       12 b- defN 23-May-23 23:24 attm/res/holiday.txt
 -rw-rw-rw-  2.0 fat    10319 b- defN 23-May-23 23:24 attm/res/icon.ico
 -rw-rw-rw-  2.0 fat    42402 b- defN 23-May-23 23:24 attm/res/icon.png
--rw-rw-rw-  2.0 fat     1087 b- defN 23-May-24 00:31 attm-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3206 b- defN 23-May-24 00:31 attm-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       98 b- defN 23-May-24 00:31 attm-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       41 b- defN 23-May-24 00:31 attm-0.0.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        5 b- defN 23-May-24 00:31 attm-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1042 b- defN 23-May-24 00:31 attm-0.0.1.dist-info/RECORD
-14 files, 69716 bytes uncompressed, 58350 bytes compressed:  16.3%
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-May-24 01:05 attm-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3206 b- defN 23-May-24 01:05 attm-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       98 b- defN 23-May-24 01:05 attm-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       41 b- defN 23-May-24 01:05 attm-0.0.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        5 b- defN 23-May-24 01:05 attm-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1042 b- defN 23-May-24 01:05 attm-0.0.2.dist-info/RECORD
+14 files, 69731 bytes uncompressed, 58355 bytes compressed:  16.3%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: attm/res/icon.ico
 Comment: 
 
 Filename: attm/res/icon.png
 Comment: 
 
-Filename: attm-0.0.1.dist-info/LICENSE
+Filename: attm-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: attm-0.0.1.dist-info/METADATA
+Filename: attm-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: attm-0.0.1.dist-info/WHEEL
+Filename: attm-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: attm-0.0.1.dist-info/entry_points.txt
+Filename: attm-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: attm-0.0.1.dist-info/top_level.txt
+Filename: attm-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: attm-0.0.1.dist-info/RECORD
+Filename: attm-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## attm/__init__.py

```diff
@@ -2,25 +2,26 @@
 import pathlib
 import shutil
 
 import attm.utils
 
 PACKAGE_PATH = pathlib.Path(attm.__path__[0]).resolve()
 VENV_PATH = PACKAGE_PATH.parent.parent.parent
-VERSION = '0.0.1'
+ROOT = VENV_PATH.parent
+VERSION = '0.0.2'
 
 
 def entrypoint():
     parser = argparse.ArgumentParser()
     parser.add_argument('task', type=str, help='Perform initial setup. (init, start)')
     args = parser.parse_args()
 
     if args.task == 'init':
         attm.utils.create_lnk_file()
-        shutil.copy(attm.PACKAGE_PATH.joinpath('res', 'holiday.txt'), attm.VENV_PATH)
+        shutil.copy(attm.PACKAGE_PATH.joinpath('res', 'holiday.txt'), attm.ROOT)
         attm.utils.save_account_info()
     else:
         raise ValueError(f'해당 명령은 정의되지 않았습니다: {args.task}')
 
 
 if __name__ == '__main__':
     entrypoint()
```

## attm/main.py

```diff
@@ -27,15 +27,15 @@
         logging.info('주말 기록 제외')
         return True
 
     if today in holidays.KR():
         logging.info('공휴일 기록 제외')
         return True
 
-    with open(attm.VENV_PATH.joinpath('holiday.txt'), 'r', encoding='utf-8') as f:
+    with open(attm.ROOT.joinpath('holiday.txt'), 'r', encoding='utf-8') as f:
         holiday = [i.strip() for i in f.readlines()]
     if today.strftime('%Y-%m-%d') in holiday:
         logging.info('연차 기록 제외')
         return True
 
     return False
 
@@ -111,15 +111,15 @@
     # 실행 상태 유지
     while icon.visible:
         schedule.run_pending()
         time.sleep(1)
 
 
 def main():
-    logging.basicConfig(filename='attm.log', filemode='w', format='%(asctime)s:%(levelname)s:%(message)s',
+    logging.basicConfig(filename=attm.ROOT.joinpath('attm.log'), filemode='w', format='%(asctime)s:%(levelname)s:%(message)s',
                         encoding='utf-8', level=logging.INFO)
     logging.info('프로그램 시작')
 
     icon = pystray.Icon(
         'attendance_manager',
         Image.open(os.path.join('res', 'icon.png')),
         '근태 관리자',
```

## attm/utils.py

```diff
@@ -23,33 +23,33 @@
     print('다우오피스 로그인 계정 정보를 입력해주세요.')
     print('계정 정보는 암호화되며, 개발자도 복호화할 수 없습니다.')
     data = f'{{"username": "{input("사용자 이름: ")}", "password": "{input("비밀번호: ")}"}}'.encode()
     privkey = cryptography.fernet.Fernet.generate_key()
     token = cryptography.fernet.Fernet(privkey).encrypt(data)
     del data
 
-    with open(attm.VENV_PATH.joinpath('account.bin'), 'wb') as f:
+    with open(attm.ROOT.joinpath('account.bin'), 'wb') as f:
         f.writelines((privkey, b'\n', token))
     os.system('cls')
     print('계정 정보가 저장되었습니다.')
 
 
 def load_account_info() -> dict:
-    with open(attm.VENV_PATH.joinpath('account.bin'), 'rb') as f:
+    with open(attm.ROOT.joinpath('account.bin'), 'rb') as f:
         privkey, token = [i.strip() for i in f.readlines()]
 
     account = cryptography.fernet.Fernet(privkey).decrypt(token)
     account = json.loads(account)
     return account
 
 
 def create_lnk_file():
     subprocess.run(
-        f'{attm.VENV_PATH.joinpath("Scripts", "activate.bat")} && '
-        f'pylnk3 create {attm.VENV_PATH.joinpath("Scripts", "pythonw.exe")} '
+        f'{attm.ROOT.joinpath("Scripts", "activate.bat")} && '
+        f'pylnk3 create {attm.ROOT.joinpath("Scripts", "pythonw.exe")} '
         f'"근태 관리자.lnk" '
         f'--arguments main.py '
         f'--icon {attm.PACKAGE_PATH.joinpath("res", "icon.ico")} '
         f'--workdir {attm.PACKAGE_PATH}',
         shell=True, check=True
     )
     startup_path = pathlib.Path('~').expanduser().joinpath(
```

## Comparing `attm-0.0.1.dist-info/LICENSE` & `attm-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `attm-0.0.1.dist-info/METADATA` & `attm-0.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attm
-Version: 0.0.1
+Version: 0.0.2
 Summary: Attendance Manager (근태 관리자)
 Home-page: https://github.com/syshin-cubox-ai/attm
 Author: synml
 Author-email: kistssy@gmail.com
 License: MIT
 Platform: Windows
 Requires-Python: >=3.9
```

