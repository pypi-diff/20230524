# Comparing `tmp/google-sheet-downloader-1.0.6.tar.gz` & `tmp/google-sheet-downloader-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-sheet-downloader-1.0.6.tar", last modified: Sat May 13 02:34:51 2023, max compression
+gzip compressed data, was "google-sheet-downloader-1.0.7.tar", last modified: Wed May 24 06:36:34 2023, max compression
```

## Comparing `google-sheet-downloader-1.0.6.tar` & `google-sheet-downloader-1.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-13 02:34:51.657940 google-sheet-downloader-1.0.6/
--rw-r--r--   0 chiubowen   (501) staff       (20)     4694 2023-05-13 02:34:51.657832 google-sheet-downloader-1.0.6/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     4513 2023-05-13 02:34:51.000000 google-sheet-downloader-1.0.6/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-13 02:34:51.657652 google-sheet-downloader-1.0.6/google_sheet_downloader.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     4694 2023-05-13 02:34:51.000000 google-sheet-downloader-1.0.6/google_sheet_downloader.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      329 2023-05-13 02:34:51.000000 google-sheet-downloader-1.0.6/google_sheet_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-13 02:34:51.000000 google-sheet-downloader-1.0.6/google_sheet_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       74 2023-05-13 02:34:51.000000 google-sheet-downloader-1.0.6/google_sheet_downloader.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       75 2023-05-13 02:34:51.000000 google-sheet-downloader-1.0.6/google_sheet_downloader.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       24 2023-05-13 02:34:51.000000 google-sheet-downloader-1.0.6/google_sheet_downloader.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     3133 2023-05-13 02:34:51.000000 google-sheet-downloader-1.0.6/google_sheet_downloader.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-13 02:34:51.657977 google-sheet-downloader-1.0.6/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      556 2023-05-13 02:34:51.000000 google-sheet-downloader-1.0.6/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-24 06:36:34.620302 google-sheet-downloader-1.0.7/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4670 2023-05-24 06:36:34.620167 google-sheet-downloader-1.0.7/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4489 2023-05-24 06:36:34.000000 google-sheet-downloader-1.0.7/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-24 06:36:34.619937 google-sheet-downloader-1.0.7/google_sheet_downloader.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4670 2023-05-24 06:36:34.000000 google-sheet-downloader-1.0.7/google_sheet_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      329 2023-05-24 06:36:34.000000 google-sheet-downloader-1.0.7/google_sheet_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-24 06:36:34.000000 google-sheet-downloader-1.0.7/google_sheet_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       74 2023-05-24 06:36:34.000000 google-sheet-downloader-1.0.7/google_sheet_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       75 2023-05-24 06:36:34.000000 google-sheet-downloader-1.0.7/google_sheet_downloader.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       24 2023-05-24 06:36:34.000000 google-sheet-downloader-1.0.7/google_sheet_downloader.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     3206 2023-05-24 06:36:34.000000 google-sheet-downloader-1.0.7/google_sheet_downloader.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-24 06:36:34.620350 google-sheet-downloader-1.0.7/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      556 2023-05-24 06:36:34.000000 google-sheet-downloader-1.0.7/setup.py
```

### Comparing `google-sheet-downloader-1.0.6/PKG-INFO` & `google-sheet-downloader-1.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: google-sheet-downloader
-Version: 1.0.6
+Version: 1.0.7
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
-# 積木塊：Google Sheets 下載器 v1.0.4 by Bowen Chiu 2023-05-12 15:32
+# 積木塊：Google Sheets 下載器 by Bowen Chiu
 這是一個能夠下載 Google Sheets 試算表的小工具。使用者可以輸入 Google 服務帳戶金鑰、試算表 ID、輸出資料夾路徑等資訊，程式會利用 Google Sheets API 下載資料並存成 CSV 檔案。
 
 ## 使用說明
 特色:
 - 支援快取功能，曾經下載過的 google sheet document id 就不會再下載，飛快
 - 支援多個檔案下載
 - 支援一個 spreadsheet 當中所有的 worksheet 下載轉換為多個 .csv 檔案
```

### Comparing `google-sheet-downloader-1.0.6/README.md` & `google-sheet-downloader-1.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# 積木塊：Google Sheets 下載器 v1.0.4 by Bowen Chiu 2023-05-12 15:32
+# 積木塊：Google Sheets 下載器 by Bowen Chiu
 這是一個能夠下載 Google Sheets 試算表的小工具。使用者可以輸入 Google 服務帳戶金鑰、試算表 ID、輸出資料夾路徑等資訊，程式會利用 Google Sheets API 下載資料並存成 CSV 檔案。
 
 ## 使用說明
 特色:
 - 支援快取功能，曾經下載過的 google sheet document id 就不會再下載，飛快
 - 支援多個檔案下載
 - 支援一個 spreadsheet 當中所有的 worksheet 下載轉換為多個 .csv 檔案
```

### Comparing `google-sheet-downloader-1.0.6/google_sheet_downloader.egg-info/PKG-INFO` & `google-sheet-downloader-1.0.7/google_sheet_downloader.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: google-sheet-downloader
-Version: 1.0.6
+Version: 1.0.7
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
-# 積木塊：Google Sheets 下載器 v1.0.4 by Bowen Chiu 2023-05-12 15:32
+# 積木塊：Google Sheets 下載器 by Bowen Chiu
 這是一個能夠下載 Google Sheets 試算表的小工具。使用者可以輸入 Google 服務帳戶金鑰、試算表 ID、輸出資料夾路徑等資訊，程式會利用 Google Sheets API 下載資料並存成 CSV 檔案。
 
 ## 使用說明
 特色:
 - 支援快取功能，曾經下載過的 google sheet document id 就不會再下載，飛快
 - 支援多個檔案下載
 - 支援一個 spreadsheet 當中所有的 worksheet 下載轉換為多個 .csv 檔案
```

### Comparing `google-sheet-downloader-1.0.6/google_sheet_downloader.py` & `google-sheet-downloader-1.0.7/google_sheet_downloader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # google_sheet_downloader.py
 import argparse
 import csv
 import glob
+import hashlib
 import json
 import os
 
 import gspread
 from google.oauth2.service_account import Credentials
 
 
@@ -38,16 +39,17 @@
     matching_files = glob.glob(pattern)
 
     return len(matching_files) > 0
 
 
 def save_to_csv(data, output_folder, sheet_name, worksheet_name, sheet_id):
     os.makedirs(output_folder, exist_ok=True)
+    sha256_digest = hashlib.sha256(f"{sheet_name}_{worksheet_name}".encode()).hexdigest()
     output_file = os.path.join(output_folder,
-                               f"doc-id_{sheet_id}_spreadsheet_{sheet_name}_worksheet_{worksheet_name}.csv")
+                               f"doc-id_{sheet_id}_sha_{sha256_digest}.csv")
     with open(output_file, 'w', newline='', encoding='utf-8') as f:
         writer = csv.writer(f)
         writer.writerows(data)
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser(description="Google Sheet Downloader")
```

### Comparing `google-sheet-downloader-1.0.6/setup.py` & `google-sheet-downloader-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="google-sheet-downloader",
-    version="1.0.6",
+    version="1.0.7",
     packages=find_packages(),
     py_modules=['google_sheet_downloader'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'google_sheet_downloader = google_sheet_downloader:main',
         ],
```

