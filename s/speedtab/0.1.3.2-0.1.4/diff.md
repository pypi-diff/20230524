# Comparing `tmp/speedtab-0.1.3.2.tar.gz` & `tmp/speedtab-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtab-0.1.3.2.tar", max compression
+gzip compressed data, was "speedtab-0.1.4.tar", max compression
```

## Comparing `speedtab-0.1.3.2.tar` & `speedtab-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      567 2023-05-22 10:27:03.691219 speedtab-0.1.3.2/pyproject.toml
--rw-r--r--   0        0        0      352 2022-09-07 08:00:08.177672 speedtab-0.1.3.2/speedtab/__init__.py
--rw-r--r--   0        0        0    45532 2023-05-22 10:26:29.269245 speedtab-0.1.3.2/speedtab/client.py
--rw-r--r--   0        0        0     6192 2023-05-19 11:01:11.239027 speedtab-0.1.3.2/speedtab/enums.py
--rw-r--r--   0        0        0     1730 2023-05-19 11:23:08.076916 speedtab-0.1.3.2/speedtab/formats.py
--rw-r--r--   0        0        0      783 2023-05-22 10:27:24.043638 speedtab-0.1.3.2/setup.py
--rw-r--r--   0        0        0      808 2023-05-22 10:27:24.043638 speedtab-0.1.3.2/PKG-INFO
+-rw-r--r--   0        0        0      565 2023-05-24 14:59:45.962392 speedtab-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      352 2022-09-07 08:00:08.177672 speedtab-0.1.4/speedtab/__init__.py
+-rw-r--r--   0        0        0    49953 2023-05-24 14:57:04.407916 speedtab-0.1.4/speedtab/client.py
+-rw-r--r--   0        0        0     6192 2023-05-19 11:01:11.239027 speedtab-0.1.4/speedtab/enums.py
+-rw-r--r--   0        0        0     1730 2023-05-19 11:23:08.076916 speedtab-0.1.4/speedtab/formats.py
+-rw-r--r--   0        0        0      781 2023-05-24 14:59:58.215209 speedtab-0.1.4/setup.py
+-rw-r--r--   0        0        0      806 2023-05-24 14:59:58.215209 speedtab-0.1.4/PKG-INFO
```

### Comparing `speedtab-0.1.3.2/pyproject.toml` & `speedtab-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speedtab"
-version = "0.1.3.2"
+version = "0.1.4"
 description = "Convenient wrapper for working with Google Spreadsheets"
 authors = ["Bogdan Gergel <bogger147@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/BoggerSancho/SpeedTab-beta"
 repository = "https://github.com/BoggerSancho/SpeedTab-beta"
 
 [tool.poetry.dependencies]
```

### Comparing `speedtab-0.1.3.2/speedtab/client.py` & `speedtab-0.1.4/speedtab/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+import io
 import re
 from collections.abc import Iterable
 from datetime import datetime, date
 from itertools import zip_longest
 from typing import Union
 
 import numpy as np
 import pandas as pd
 from google.oauth2.credentials import Credentials
 from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.discovery import build
+from googleapiclient.errors import HttpError
+from googleapiclient.http import MediaIoBaseDownload
 
 from speedtab.enums import MergeType, BorderStyle, HorizontalAlignment, VerticalAlignment, WrapStrategy, ShareRole, \
     ChartType, StackedType, LegendPosition, AxisPosition, BooleanConditionTypes, BorderSides
 from speedtab.formats import Color, Border, Number, BaseNumberFormat
 
 SCOPES = ['https://www.googleapis.com/auth/spreadsheets', 'https://www.googleapis.com/auth/drive', 'https://www.googleapis.com/auth/drive.file']
 SHIFT_DIM = {
@@ -123,19 +126,20 @@
         self.position = position
         self.sheetId = sheetId
         self.task = task
         self.work_zone = work_zone
 
 
 class SpreedSheet:
-    def __init__(self, spreadsheet_id, token_path, credentials, connect):
+    def __init__(self, spreadsheet_id, token_path, credentials, connect_v4, connect_v3):
         self.spreadsheet_id = spreadsheet_id
         self.token_path = token_path
         self.credentials = credentials
-        self.connect_v4 = connect
+        self.connect_v4 = connect_v4
+        self.connect_v3 = connect_v3
         self._get_metadata()
         self._task_queue = []
 
     def _regroup_tasks(self):
         groups = []
         for id in [x.get('sheetId') for x in self.sheets.values()]:
             current_id_tasks = [x for x in self._task_queue if x.sheetId == id]
@@ -156,14 +160,15 @@
 
             groups.append(merged_group)
 
         full_groups = [sorted(sum(x, []), key=lambda x: (TYPE_ORDER[x.task_type], x.position)) for x in zip_longest(*groups, fillvalue=[])]
 
         curr_size = {}
         new_size = {}
+        delete_group = []
         for sheet in self.sheets.values():
             curr_size[sheet.get('sheetId')] = [sheet.get('max_row'), sheet.get('max_column')]
             new_size[sheet.get('sheetId')] = [sheet.get('max_row'), sheet.get('max_column')]
 
         for group in full_groups:
             for task in group:
                 if task.task_type == 'clear' and 'updateSheetProperties' in task.task.keys():
@@ -182,16 +187,20 @@
                             task.work_zone.get('endRowIndex', 0) if task.work_zone.get('endRowIndex', 0) is not None else 0
                             ),
                         max(new_size[task.sheetId][1],
                             task.work_zone.get('startColumnIndex', 0) if task.work_zone.get('startColumnIndex', 0) is not None else 0,
                             task.work_zone.get('endColumnIndex', 0) if task.work_zone.get('endColumnIndex', 0) is not None else 0
                             )
                     ]
-            for key, (rows, columns) in curr_size.items():
-                self._set_sheet_size(rows, columns, key, group)
+                if task.task_type == 'format' and 'deleteSheet' in task.task.keys():
+                    delete_group.append(task.sheetId)
+
+            for key, (rows, columns) in new_size.items():
+                if new_size[key] != curr_size[key] and key not in delete_group:
+                    self._set_sheet_size(rows, columns, key, group)
 
         return [sorted(group, key=lambda x: (TYPE_ORDER[x.task_type], x.position)) for group in full_groups]
 
     def _set_sheet_size(self, rows: int, columns: int, sheet_id, group):
         group.append(Task('format', len(self._task_queue), sheet_id, {
             'updateSheetProperties': {
                 'properties': {
@@ -203,20 +212,21 @@
                 },
                 'fields': 'gridProperties.rowCount, gridProperties.columnCount',
             }}, None))
 
     def _get_metadata(self):
         metadata = self.connect_v4.spreadsheets().get(spreadsheetId=self.spreadsheet_id).execute()
         self.sheets = dict(
-            [(prop.get('title'), {
-                'max_column': prop.get('gridProperties').get('columnCount'),
-                'max_row': prop.get('gridProperties').get('rowCount'),
-                'sheetId': prop.get('sheetId'),
-                'position': prop.get('index'),
-            }) for prop in [sheet.get('properties') for sheet in metadata.get('sheets')]]
+            [(properties.get('title'), {
+                'max_column': properties.get('gridProperties').get('columnCount'),
+                'max_row': properties.get('gridProperties').get('rowCount'),
+                'sheetId': properties.get('sheetId'),
+                'position': properties.get('index'),
+                'charts': [chart.get('chartId') for chart in charts],
+            }) for properties, charts in [(sheet.get('properties'), sheet.get('charts', [])) for sheet in metadata.get('sheets')]]
         )
 
     def sheets_list(self):
         return list(self.sheets.keys())
 
     def exec(self):
         batch_update_chart_list = []
@@ -268,20 +278,95 @@
         self._get_metadata()
         return self
 
     def delete_sheets(self, sheets):
         for sheet in sheets:
             self._task_queue.append(Task('format', len(self._task_queue), self.sheets.get(sheet).get('sheetId'), {
                 'deleteSheet': {
-                    'sheetId': self.sheets.get(sheet).get('sheetId')}}, self.work_zone))
+                    'sheetId': self.sheets.get(sheet).get('sheetId')}}, (0, 0, 0, 0)))
         return self
 
     def sheet(self, sheet_name):
         return Sheet(sheet_name, self.sheets.get(sheet_name).get('sheetId'), self._task_queue, self.sheets, self)
 
+    def export_as_zip(self, output: str):
+        try:
+            request = self.connect_v3.files().export_media(fileId=self.spreadsheet_id, mimeType='application/zip')
+
+            fh = io.FileIO(output, mode='w')
+
+            downloader = MediaIoBaseDownload(fh, request)
+            done = False
+            while done is False:
+                status, done = downloader.next_chunk()
+                print("Download %d%%." % int(status.progress() * 100))
+
+        except HttpError as error:
+            print(F'An error occurred: {error}')
+
+    def export_as_excel(self, output: str):
+        try:
+            request = self.connect_v3.files().export_media(fileId=self.spreadsheet_id, mimeType='application/vnd.openxmlformats-officedocument.spreadsheetml.sheet')
+
+            fh = io.FileIO(output, mode='w')
+
+            downloader = MediaIoBaseDownload(fh, request)
+            done = False
+            while done is False:
+                status, done = downloader.next_chunk()
+                print("Download %d%%." % int(status.progress() * 100))
+
+        except HttpError as error:
+            print(F'An error occurred: {error}')
+
+    def export_as_open_document(self, output: str):
+        try:
+            request = self.connect_v3.files().export_media(fileId=self.spreadsheet_id, mimeType='application/x-vnd.oasis.opendocument.spreadsheet')
+
+            fh = io.FileIO(output, mode='w')
+
+            downloader = MediaIoBaseDownload(fh, request)
+            done = False
+            while done is False:
+                status, done = downloader.next_chunk()
+                print("Download %d%%." % int(status.progress() * 100))
+
+        except HttpError as error:
+            print(F'An error occurred: {error}')
+
+    def export_as_pdf(self, output: str):
+        try:
+            request = self.connect_v3.files().export_media(fileId=self.spreadsheet_id, mimeType='application/pdf')
+
+            fh = io.FileIO(output, mode='w')
+
+            downloader = MediaIoBaseDownload(fh, request)
+            done = False
+            while done is False:
+                status, done = downloader.next_chunk()
+                print("Download %d%%." % int(status.progress() * 100))
+
+        except HttpError as error:
+            print(F'An error occurred: {error}')
+
+    def export_as_csv(self, output: str):
+        try:
+            request = self.connect_v3.files().export_media(fileId=self.spreadsheet_id, mimeType='text/csv')
+
+            fh = io.FileIO(output, mode='w')
+
+            downloader = MediaIoBaseDownload(fh, request)
+            done = False
+            while done is False:
+                status, done = downloader.next_chunk()
+                print("Download %d%%." % int(status.progress() * 100))
+
+        except HttpError as error:
+            print(F'An error occurred: {error}')
+
 
 class Range:
     def __init__(self, sheet_id, _task_queue, work_zone, start_data_cell, base, data_cell):
         self.sheet_id = sheet_id
         self._task_queue = _task_queue
         self.work_zone = work_zone
         self.start_data_cell = start_data_cell
@@ -591,14 +676,25 @@
                     'sheetId': self.sheet_id,
                     'dimension': 'ROWS',
                     'length': rows,
                 }}, self.work_zone))
 
         return self
 
+    def hide_sheet(self, hide=True):
+        self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
+            'updateSheetProperties': {
+                'properties': {
+                    'sheetId': self.sheet_id,
+                    'hidden': hide
+                },
+                'fields': 'hidden'
+            }}, self.work_zone))
+        return self
+
     def hide_grid_lines(self, hide_grid=True):
         self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
             'updateSheetProperties': {
                 'properties': {
                     'sheetId': self.sheet_id,
                     'gridProperties': {
                         'hideGridlines': hide_grid,
@@ -844,15 +940,14 @@
                 'values': values,
                 'majorDimension': DIMENSION.get(axis.upper() if isinstance(axis, str) else axis),
               }, self.work_zone))
 
         return self
 
 
-
 class Sheet(Range):
     def __init__(self, sheet_name, sheet_id, task_query, sheets, base, cells=(0, 0, None, None)):
         self.base = base
         self.sheet_name = sheet_name
         self.sheet_id = sheet_id
         self._task_queue = task_query
         self.sheets = sheets
@@ -869,14 +964,23 @@
 
     def sheet(self, sheet_name):
         return Sheet(sheet_name, self.sheet_id, self._task_queue, self.sheets, self.base)
 
     def cell_range(self, input_range):
         return Sheet(self.sheet_name, self.sheet_id, self._task_queue, self.sheets, self.base, input_range)
 
+    def delete_all_charts(self):
+        for chart_id in self.sheets.get(self.sheet_name).get('charts'):
+            self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
+                    'deleteEmbeddedObject': {
+                        'objectId': chart_id
+                    }}, self.work_zone))
+
+        return self
+
 
 class Client:
     def __init__(self, token_path='token.json'):
         self.token_path = token_path
         self.credentials = Credentials.from_authorized_user_file(self.token_path, SCOPES)
         self.list_of_spreadsheets = []
         self.connect_v4 = self._connect_v4()
@@ -902,15 +1006,15 @@
                          .create(fields='spreadsheetId',
                                  body={
                                      'properties': {'title': title},
                                      'sheets': [{'properties': {'title': sheet_name,
                                                                 'gridProperties': {'hideGridlines': grid}}}
                                                 for sheet_name, grid in zip(sheets, hide_grid_lines)]})
                          .execute().get('spreadsheetId'), token_path=self.token_path,
-                         credentials=self.credentials, connect=self.connect_v4)
+                         credentials=self.credentials, connect_v4=self.connect_v4, connect_v3=self.connect_v3)
         self.list_of_spreadsheets.append(ss)
         return ss
 
     def create_folder(self, folder_name: str, parent_id: str = None):
         return self.connect_v3.files().create(body={
             'name': folder_name,
             'mimeType': "application/vnd.google-apps.folder",
@@ -944,20 +1048,23 @@
         return files
 
     def search_folder(self, folder_name, current_folder: str = None, mkdir: bool = False):
         folders = [file for file in self.search_files(current_folder) if
                    file.get('file_type') == 'folder' and file.get('name') == folder_name]
 
         if folders:
-            return folders[0].get('id')
+            return (folder.get('id') for folder in folders)
         elif mkdir:
             return self.create_folder(folder_name, current_folder)
         else:
             return None
 
+    def delete_file(self, file_id: str):
+        self.connect_v3.files().delete(fileId=file_id).execute()
+
     def move_spreadsheet_to_folder(self, ss: SpreedSheet, real_folder_id: str):
         previous_parents = ','.join(self.connect_v3.files().get(fileId=ss.spreadsheet_id, fields='parents').execute().get('parents'))
         self.connect_v3.files().update(fileId=ss.spreadsheet_id, addParents=real_folder_id,
                                        removeParents=previous_parents, fields='id, parents').execute()
 
     def share_spreadsheet_with_domain(self, ss: SpreedSheet, domain: str, role: ShareRole):
         self.connect_v3.permissions().create(**{
@@ -980,15 +1087,16 @@
                 'emailAddress': user,
             },
             'fields': 'id',
         }).execute()
 
     def get_spreadsheet(self, spreadsheet_id):
         ss = SpreedSheet(spreadsheet_id=spreadsheet_id, token_path=self.token_path,
-                         credentials=self.credentials, connect=self.connect_v4)
+                         credentials=self.credentials, connect_v4=self.connect_v4,
+                         connect_v3=self.connect_v3)
         self.list_of_spreadsheets.append(ss)
         return ss
 
     def _connect_v4(self):
         return build('sheets', 'v4', credentials=self.credentials)
 
     def _connect_v3(self):
```

### Comparing `speedtab-0.1.3.2/speedtab/enums.py` & `speedtab-0.1.4/speedtab/enums.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.3.2/speedtab/formats.py` & `speedtab-0.1.4/speedtab/formats.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.3.2/setup.py` & `speedtab-0.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['google-api-python-client>=2.58.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.2,<0.6.0']
 
 setup_kwargs = {
     'name': 'speedtab',
-    'version': '0.1.3.2',
+    'version': '0.1.4',
     'description': 'Convenient wrapper for working with Google Spreadsheets',
     'long_description': None,
     'author': 'Bogdan Gergel',
     'author_email': 'bogger147@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/BoggerSancho/SpeedTab-beta',
```

### Comparing `speedtab-0.1.3.2/PKG-INFO` & `speedtab-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtab
-Version: 0.1.3.2
+Version: 0.1.4
 Summary: Convenient wrapper for working with Google Spreadsheets
 Home-page: https://github.com/BoggerSancho/SpeedTab-beta
 License: MIT
 Author: Bogdan Gergel
 Author-email: bogger147@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

