# Comparing `tmp/attm-0.0.9-py3-none-win_amd64.whl.zip` & `tmp/attm-0.1.0-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 59942 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat      934 b- defN 23-May-24 04:25 attm/__init__.py
--rw-rw-rw-  2.0 fat      270 b- defN 23-May-24 02:23 attm/config.py
--rw-rw-rw-  2.0 fat     5529 b- defN 23-May-24 01:55 attm/main.py
--rw-rw-rw-  2.0 fat     4141 b- defN 23-May-24 04:26 attm/utils.py
+Zip file size: 59961 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat     1011 b- defN 23-May-24 06:54 attm/__init__.py
+-rw-rw-rw-  2.0 fat     5613 b- defN 23-May-24 07:01 attm/main.py
+-rw-rw-rw-  2.0 fat     4184 b- defN 23-May-24 06:56 attm/utils.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-23 23:24 attm/res/__init__.py
--rw-rw-rw-  2.0 fat       12 b- defN 23-May-23 23:24 attm/res/holiday.txt
+-rw-rw-rw-  2.0 fat      188 b- defN 23-May-24 07:00 attm/res/config.yaml
+-rw-rw-rw-  2.0 fat       12 b- defN 23-May-24 06:49 attm/res/holiday.txt
 -rw-rw-rw-  2.0 fat    10319 b- defN 23-May-23 23:24 attm/res/icon.ico
 -rw-rw-rw-  2.0 fat    42402 b- defN 23-May-23 23:24 attm/res/icon.png
--rw-rw-rw-  2.0 fat     1087 b- defN 23-May-24 04:28 attm-0.0.9.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3206 b- defN 23-May-24 04:28 attm-0.0.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       98 b- defN 23-May-24 04:28 attm-0.0.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       41 b- defN 23-May-24 04:28 attm-0.0.9.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        5 b- defN 23-May-24 04:28 attm-0.0.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1042 b- defN 23-May-24 04:28 attm-0.0.9.dist-info/RECORD
-14 files, 69086 bytes uncompressed, 58236 bytes compressed:  15.7%
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-May-24 07:20 attm-0.1.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3229 b- defN 23-May-24 07:20 attm-0.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       98 b- defN 23-May-24 07:20 attm-0.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       41 b- defN 23-May-24 07:20 attm-0.1.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        5 b- defN 23-May-24 07:20 attm-0.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1049 b- defN 23-May-24 07:20 attm-0.1.0.dist-info/RECORD
+14 files, 69238 bytes uncompressed, 58243 bytes compressed:  15.9%
```

## zipnote {}

```diff
@@ -1,43 +1,43 @@
 Filename: attm/__init__.py
 Comment: 
 
-Filename: attm/config.py
-Comment: 
-
 Filename: attm/main.py
 Comment: 
 
 Filename: attm/utils.py
 Comment: 
 
 Filename: attm/res/__init__.py
 Comment: 
 
+Filename: attm/res/config.yaml
+Comment: 
+
 Filename: attm/res/holiday.txt
 Comment: 
 
 Filename: attm/res/icon.ico
 Comment: 
 
 Filename: attm/res/icon.png
 Comment: 
 
-Filename: attm-0.0.9.dist-info/LICENSE
+Filename: attm-0.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: attm-0.0.9.dist-info/METADATA
+Filename: attm-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: attm-0.0.9.dist-info/WHEEL
+Filename: attm-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: attm-0.0.9.dist-info/entry_points.txt
+Filename: attm-0.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: attm-0.0.9.dist-info/top_level.txt
+Filename: attm-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: attm-0.0.9.dist-info/RECORD
+Filename: attm-0.1.0.dist-info/RECORD
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
 
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 
 # Path
 PACKAGE = pathlib.Path(attm.__path__[0]).resolve()
 VENV = PACKAGE.parent.parent.parent
 ROOT = VENV.parent
 ACTIVATE = VENV.joinpath("Scripts", "activate.bat")
 STARTUP = pathlib.Path('~').expanduser().joinpath(
@@ -20,14 +20,15 @@
 def entrypoint():
     parser = argparse.ArgumentParser()
     parser.add_argument('task', type=str, help='Perform initial setup. (init, start)')
     args = parser.parse_args()
 
     if args.task == 'init':
         attm.utils.create_lnk_file()
+        shutil.copy(attm.PACKAGE.joinpath('res', 'config.yaml'), attm.ROOT)
         shutil.copy(attm.PACKAGE.joinpath('res', 'holiday.txt'), attm.ROOT)
         attm.utils.save_account_info()
     else:
         raise ValueError(f'해당 명령은 정의되지 않았습니다: {args.task}')
 
 
 if __name__ == '__main__':
```

## attm/main.py

```diff
@@ -1,28 +1,26 @@
 import datetime
 import logging
 import os
 import random
 import time
 import traceback
 
+import attm
+import attm.utils
 import holidays
 import pystray
 import schedule
 import selenium.common.exceptions
 import selenium.webdriver
 import selenium.webdriver.support.expected_conditions as ec
 from PIL import Image
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 
-import attm
-import config
-import utils
-
 
 def except_attendance() -> bool:
     today = datetime.datetime.today()
 
     if today.weekday() in [5, 6]:
         logging.info('주말 기록 제외')
         return True
@@ -51,18 +49,18 @@
             secs = random.randint(0, 540)
             scheduled_time = datetime.datetime.now() + datetime.timedelta(seconds=secs)
             logging.info(f'기록 예정 시각: {scheduled_time.strftime("%H:%M:%S")}')
             icon.notify(f'기록 예정 시각: {scheduled_time.strftime("%H:%M:%S")}')
             time.sleep(secs)
 
         # 크롬 드라이버 인스턴스 생성
-        driver = utils.create_chrome_instance('https://cubox.daouoffice.com/app/ehr', headless)
+        driver = attm.utils.create_chrome_instance('https://cubox.daouoffice.com/app/ehr', headless)
 
         # 로그인
-        account = utils.load_account_info()
+        account = attm.utils.load_account_info()
         driver.find_element(By.ID, 'username').send_keys(account['username'])
         driver.find_element(By.ID, 'password').send_keys(account['password'])
         driver.execute_script('arguments[0].click();', driver.find_element(By.ID, 'login_submit'))
         del account
 
         # 공지 제거
         try:
@@ -95,46 +93,48 @@
         icon.notify(f'오류 발생: {e}\n자세한 내용은 로그를 참조하세요.')
 
 
 def setup(icon: pystray.Icon) -> None:
     icon.visible = True
 
     # 스케줄 등록
-    schedule.every().day.at(config.schedule_work_in).do(record_commute, icon, work_in=True)
-    schedule.every().day.at(config.schedule_work_out).do(record_commute, icon, work_out=True)
-    schedule.every().day.at(config.schedule_update).do(utils.update, icon)
+    schedule.every().day.at(config['schedule_work_in']).do(record_commute, icon, work_in=True)
+    schedule.every().day.at(config['schedule_work_out']).do(record_commute, icon, work_out=True)
+    schedule.every().day.at(config['schedule_update']).do(attm.utils.update, icon)
 
     # 시작 알림
-    time.sleep(config.start_delay_secs)
+    time.sleep(1)
     logging.info('출퇴근 자동 기록 시작')
     icon.notify('출퇴근 자동 기록 시작')
 
     # 실행 상태 유지
     while icon.visible:
         schedule.run_pending()
         time.sleep(1)
 
 
 def main():
-    logging.basicConfig(filename=attm.ROOT.joinpath('attm.log'), filemode='w', format='%(asctime)s:%(levelname)s:%(message)s',
+    logging.basicConfig(filename=attm.ROOT.joinpath('attm.log'), filemode='w',
+                        format='%(asctime)s:%(levelname)s:%(message)s',
                         encoding='utf-8', level=logging.INFO)
     logging.info('프로그램 시작')
 
     icon = pystray.Icon(
         'attendance_manager',
         Image.open(os.path.join('res', 'icon.png')),
         '근태 관리자',
         pystray.Menu(
-            pystray.MenuItem('업데이트 확인', lambda icon, item: utils.update(icon)),
-            pystray.MenuItem('설치 폴더 열기', lambda icon, item: utils.open_root_dir()),
-            pystray.MenuItem('로그 표시', lambda icon, item: utils.show_log()),
-            pystray.MenuItem('정보', lambda icon, item: icon.notify(utils.info())),
+            pystray.MenuItem('업데이트 확인', lambda icon, item: attm.utils.update(icon)),
+            pystray.MenuItem('설치 폴더 열기', lambda icon, item: attm.utils.open_root_dir()),
+            pystray.MenuItem('로그 표시', lambda icon, item: attm.utils.show_log()),
+            pystray.MenuItem('정보', lambda icon, item: icon.notify(attm.utils.info())),
             pystray.Menu.SEPARATOR,
-            pystray.MenuItem('재시작', lambda icon, item: utils.restart(icon)),
-            pystray.MenuItem('종료', lambda icon, item: utils.exit_action(icon)),
+            pystray.MenuItem('재시작', lambda icon, item: attm.utils.restart(icon)),
+            pystray.MenuItem('종료', lambda icon, item: attm.utils.exit_action(icon)),
         )
     )
     icon.run(setup)
 
 
 if __name__ == '__main__':
+    config = attm.utils.load_config()
     main()
```

## attm/utils.py

```diff
@@ -1,129 +1,136 @@
-import datetime
-import json
-import logging
-import os
-import platform
-import shutil
-import subprocess
-import sys
-import traceback
-
-import chromedriver_autoinstaller
-import cryptography.fernet
-import pystray
-import selenium.common.exceptions
-import selenium.webdriver
-from selenium.webdriver.chrome.webdriver import WebDriver
-
-import attm
-
-
-def save_account_info() -> None:
-    print('다우오피스 로그인 계정 정보를 입력해주세요.')
-    print('계정 정보는 암호화되며, 개발자도 복호화할 수 없습니다.')
-    data = f'{{"username": "{input("사용자 이름: ")}", "password": "{input("비밀번호: ")}"}}'.encode()
-    privkey = cryptography.fernet.Fernet.generate_key()
-    token = cryptography.fernet.Fernet(privkey).encrypt(data)
-    del data
-
-    with open(attm.ROOT.joinpath('account.bin'), 'wb') as f:
-        f.writelines((privkey, b'\n', token))
-    os.system('cls')
-    print('계정 정보가 저장되었습니다.')
-
-
-def load_account_info() -> dict:
-    with open(attm.ROOT.joinpath('account.bin'), 'rb') as f:
-        privkey, token = [i.strip() for i in f.readlines()]
-
-    account = cryptography.fernet.Fernet(privkey).decrypt(token)
-    account = json.loads(account)
-    return account
-
-
-def create_lnk_file():
-    subprocess.run(
-        f'{attm.ACTIVATE} && '
-        f'pylnk3 create {attm.VENV.joinpath("Scripts", "pythonw.exe")} '
-        f'"근태 관리자.lnk" '
-        f'--arguments main.py '
-        f'--icon {attm.PACKAGE.joinpath("res", "icon.ico")} '
-        f'--workdir {attm.PACKAGE}',
-        shell=True, check=True
-    )
-    shutil.copy('근태 관리자.lnk', attm.STARTUP)
-    shutil.copy('근태 관리자.lnk', attm.START_MENU)
-    os.remove('근태 관리자.lnk')
-
-
-def create_chrome_instance(url: str, headless: bool) -> WebDriver:
-    chromedriver_autoinstaller.install(cwd=True)
-
-    options = selenium.webdriver.ChromeOptions()
-    if headless:
-        options.add_argument('headless')
-        options.add_argument('disable-gpu')
-    options.add_argument('disable-dev-shm-usage')
-
-    driver = selenium.webdriver.Chrome(options=options)
-    driver.get(url)
-    driver.set_window_size(1400, 900)
-    return driver
-
-
-def update(icon: pystray.Icon) -> None:
-    try:
-        logging.info('업데이트 확인...')
-        icon.notify('업데이트 확인...')
-
-        # 패키지 업데이트 확인
-        stdout = subprocess.run(
-            f'{attm.ACTIVATE} && pip list --disable-pip-version-check --outdated --format json',
-            shell=True, capture_output=True, check=True, encoding='utf-8').stdout
-        outdated_packages = [i['name'] for i in json.loads(stdout)]
-
-        # 패키지 업데이트 수행
-        if len(outdated_packages) == 0:
-            logging.info('최신 버전입니다.')
-            icon.notify('최신 버전입니다.')
-        else:
-            subprocess.Popen(
-                f'timeout 3 > nul && '
-                f'{attm.ACTIVATE} && '
-                f'python -m pip install -U {" ".join(outdated_packages)} && '
-                f'{attm.STARTUP.joinpath("근태 관리자.lnk")}',
-                shell=True)
-            exit_action(icon)
-
-    except subprocess.CalledProcessError as e:
-        logging.error(traceback.format_exc())
-        icon.notify(f'오류 발생: {e}\n자세한 내용은 로그를 참조하세요.')
-
-
-def open_root_dir() -> None:
-    subprocess.Popen(f'start {attm.ROOT}', shell=True)
-
-
-def show_log() -> None:
-    subprocess.Popen(f'notepad {attm.ROOT.joinpath("attm.log")}', shell=True)
-
-
-def info() -> str:
-    return f"""
-버전: {attm.VERSION}
-OS: {platform.platform()}
-Copyright ⓒ {datetime.datetime.now().year}. Seokyong Shin
-""".strip()
-
-
-def restart(icon: pystray.Icon) -> None:
-    logging.info('프로그램 재시작')
-    icon.visible = False
-    os.execl(sys.executable, sys.executable, *sys.argv)
-    icon.stop()
-
-
-def exit_action(icon: pystray.Icon) -> None:
-    logging.info('프로그램 종료')
-    icon.visible = False
-    icon.stop()
+import datetime
+import json
+import logging
+import os
+import platform
+import shutil
+import subprocess
+import sys
+import traceback
+
+import attm
+import chromedriver_autoinstaller
+import cryptography.fernet
+import pystray
+import selenium.common.exceptions
+import selenium.webdriver
+import yaml
+from selenium.webdriver.chrome.webdriver import WebDriver
+
+
+def load_config():
+    with open(attm.ROOT.joinpath('config.yaml'), 'r', encoding='utf-8') as f:
+        config = yaml.safe_load(f)
+    return config
+
+
+def save_account_info() -> None:
+    print('다우오피스 로그인 계정 정보를 입력해주세요.')
+    print('계정 정보는 암호화되며, 개발자도 복호화할 수 없습니다.')
+    data = f'{{"username": "{input("사용자 이름: ")}", "password": "{input("비밀번호: ")}"}}'.encode()
+    privkey = cryptography.fernet.Fernet.generate_key()
+    token = cryptography.fernet.Fernet(privkey).encrypt(data)
+    del data
+
+    with open(attm.ROOT.joinpath('account.bin'), 'wb') as f:
+        f.writelines((privkey, b'\n', token))
+    os.system('cls')
+    print('계정 정보가 저장되었습니다.')
+
+
+def load_account_info() -> dict:
+    with open(attm.ROOT.joinpath('account.bin'), 'rb') as f:
+        privkey, token = [i.strip() for i in f.readlines()]
+
+    account = cryptography.fernet.Fernet(privkey).decrypt(token)
+    account = json.loads(account)
+    return account
+
+
+def create_lnk_file():
+    subprocess.run(
+        f'{attm.ACTIVATE} && '
+        f'pylnk3 create {attm.VENV.joinpath("Scripts", "pythonw.exe")} '
+        f'"근태 관리자.lnk" '
+        f'--arguments main.py '
+        f'--icon {attm.PACKAGE.joinpath("res", "icon.ico")} '
+        f'--workdir {attm.PACKAGE}',
+        shell=True, check=True
+    )
+    shutil.copy('근태 관리자.lnk', attm.STARTUP)
+    shutil.copy('근태 관리자.lnk', attm.START_MENU)
+    os.remove('근태 관리자.lnk')
+
+
+def create_chrome_instance(url: str, headless: bool) -> WebDriver:
+    chromedriver_autoinstaller.install(cwd=True)
+
+    options = selenium.webdriver.ChromeOptions()
+    if headless:
+        options.add_argument('headless')
+        options.add_argument('disable-gpu')
+    options.add_argument('disable-dev-shm-usage')
+
+    driver = selenium.webdriver.Chrome(options=options)
+    driver.get(url)
+    driver.set_window_size(1400, 900)
+    return driver
+
+
+def update(icon: pystray.Icon) -> None:
+    try:
+        logging.info('업데이트 확인...')
+        icon.notify('업데이트 확인...')
+
+        # 패키지 업데이트 확인
+        stdout = subprocess.run(
+            f'{attm.ACTIVATE} && pip list --disable-pip-version-check --outdated --format json',
+            shell=True, capture_output=True, check=True, encoding='utf-8').stdout
+        outdated_packages = [i['name'] for i in json.loads(stdout)]
+
+        # 패키지 업데이트 수행
+        if len(outdated_packages) == 0:
+            logging.info('최신 버전입니다.')
+            icon.notify('최신 버전입니다.')
+        else:
+            subprocess.Popen(
+                f'timeout 4 > nul && '
+                f'{attm.ACTIVATE} && '
+                f'python -m pip install -U {" ".join(outdated_packages)} && '
+                f'"{attm.STARTUP.joinpath("근태 관리자.lnk")}"',
+                shell=True
+            )
+            exit_action(icon)
+
+    except subprocess.CalledProcessError as e:
+        logging.error(traceback.format_exc())
+        icon.notify(f'오류 발생: {e}\n자세한 내용은 로그를 참조하세요.')
+
+
+def open_root_dir() -> None:
+    subprocess.Popen(f'start {attm.ROOT}', shell=True)
+
+
+def show_log() -> None:
+    subprocess.Popen(f'notepad {attm.ROOT.joinpath("attm.log")}', shell=True)
+
+
+def info() -> str:
+    return f"""
+버전: {attm.VERSION}
+OS: {platform.platform()}
+Copyright ⓒ {datetime.datetime.now().year}. Seokyong Shin
+""".strip()
+
+
+def restart(icon: pystray.Icon) -> None:
+    logging.info('프로그램 재시작')
+    icon.visible = False
+    subprocess.Popen([sys.executable, *sys.argv])
+    icon.stop()
+
+
+def exit_action(icon: pystray.Icon) -> None:
+    logging.info('프로그램 종료')
+    icon.visible = False
+    icon.stop()
```

## Comparing `attm-0.0.9.dist-info/LICENSE` & `attm-0.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `attm-0.0.9.dist-info/METADATA` & `attm-0.1.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: attm
-Version: 0.0.9
+Version: 0.1.0
 Summary: Attendance Manager (근태 관리자)
 Home-page: https://github.com/syshin-cubox-ai/attm
 Author: synml
 Author-email: kistssy@gmail.com
 License: MIT
 Platform: Windows
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: chromedriver-autoinstaller
 Requires-Dist: cryptography
 Requires-Dist: holidays
 Requires-Dist: pylnk3
 Requires-Dist: pystray
+Requires-Dist: pyyaml
 Requires-Dist: schedule
 Requires-Dist: selenium
 
 # Attendance Manager (근태 관리자)
 
 ## 요구사항
 - Windows 10 또는 11
```

