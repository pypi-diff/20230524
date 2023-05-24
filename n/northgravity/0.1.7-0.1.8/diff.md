# Comparing `tmp/northgravity-0.1.7.tar.gz` & `tmp/northgravity-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "northgravity-0.1.7.tar", last modified: Tue May 23 13:57:31 2023, max compression
+gzip compressed data, was "northgravity-0.1.8.tar", last modified: Tue May 23 15:51:06 2023, max compression
```

## Comparing `northgravity-0.1.7.tar` & `northgravity-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:57:31.444412 northgravity-0.1.7/
--rw-rw-r--   0 root         (0) root         (0)     1055 2023-04-18 12:31:14.000000 northgravity-0.1.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)    29830 2023-05-23 13:57:31.444412 northgravity-0.1.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    29397 2023-05-23 13:57:31.000000 northgravity-0.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:57:31.444412 northgravity-0.1.7/northgravity/
--rw-rw-r--   0 root         (0) root         (0)     1327 2023-05-18 09:33:33.000000 northgravity-0.1.7/northgravity/Authenticator.py
--rw-rw-r--   0 root         (0) root         (0)     9912 2023-05-23 13:44:00.000000 northgravity-0.1.7/northgravity/DatalakeHandler.py
--rw-rw-r--   0 root         (0) root         (0)      309 2023-04-18 12:31:14.000000 northgravity-0.1.7/northgravity/ExceptionHandler.py
--rw-rw-r--   0 root         (0) root         (0)     6567 2023-04-18 12:31:14.000000 northgravity-0.1.7/northgravity/HTTPCalller.py
--rw-rw-r--   0 root         (0) root         (0)     1792 2023-04-18 12:31:14.000000 northgravity-0.1.7/northgravity/StatusHandler.py
--rw-rw-r--   0 root         (0) root         (0)    10261 2023-04-18 12:31:14.000000 northgravity-0.1.7/northgravity/TaskHandler.py
--rw-rw-r--   0 root         (0) root         (0)    13042 2023-04-18 12:31:14.000000 northgravity-0.1.7/northgravity/Timeseries.py
--rw-rw-r--   0 root         (0) root         (0)      567 2023-04-18 12:31:14.000000 northgravity-0.1.7/northgravity/__init__.py
--rw-r--r--   0 root         (0) root         (0)      122 2023-05-23 13:57:31.000000 northgravity-0.1.7/northgravity/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:57:31.444412 northgravity-0.1.7/northgravity.egg-info/
--rw-r--r--   0 root         (0) root         (0)    29830 2023-05-23 13:57:31.000000 northgravity-0.1.7/northgravity.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      464 2023-05-23 13:57:31.000000 northgravity-0.1.7/northgravity.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 13:57:31.000000 northgravity-0.1.7/northgravity.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-05-23 13:57:31.000000 northgravity-0.1.7/northgravity.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 13:57:31.000000 northgravity-0.1.7/northgravity.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 13:57:31.444412 northgravity-0.1.7/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      829 2023-04-18 12:31:14.000000 northgravity-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:51:06.645182 northgravity-0.1.8/
+-rw-rw-r--   0 root         (0) root         (0)     1055 2023-04-18 12:31:14.000000 northgravity-0.1.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    29830 2023-05-23 15:51:06.645182 northgravity-0.1.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    29397 2023-05-23 15:51:06.000000 northgravity-0.1.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:51:06.645182 northgravity-0.1.8/northgravity/
+-rw-rw-r--   0 root         (0) root         (0)     1327 2023-05-18 09:33:33.000000 northgravity-0.1.8/northgravity/Authenticator.py
+-rw-rw-r--   0 root         (0) root         (0)    10526 2023-05-23 15:34:39.000000 northgravity-0.1.8/northgravity/DatalakeHandler.py
+-rw-rw-r--   0 root         (0) root         (0)      309 2023-04-18 12:31:14.000000 northgravity-0.1.8/northgravity/ExceptionHandler.py
+-rw-rw-r--   0 root         (0) root         (0)     6567 2023-04-18 12:31:14.000000 northgravity-0.1.8/northgravity/HTTPCalller.py
+-rw-rw-r--   0 root         (0) root         (0)     1792 2023-04-18 12:31:14.000000 northgravity-0.1.8/northgravity/StatusHandler.py
+-rw-rw-r--   0 root         (0) root         (0)    10261 2023-04-18 12:31:14.000000 northgravity-0.1.8/northgravity/TaskHandler.py
+-rw-rw-r--   0 root         (0) root         (0)    13042 2023-04-18 12:31:14.000000 northgravity-0.1.8/northgravity/Timeseries.py
+-rw-rw-r--   0 root         (0) root         (0)      567 2023-04-18 12:31:14.000000 northgravity-0.1.8/northgravity/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      122 2023-05-23 15:51:06.000000 northgravity-0.1.8/northgravity/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:51:06.645182 northgravity-0.1.8/northgravity.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    29830 2023-05-23 15:51:06.000000 northgravity-0.1.8/northgravity.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      464 2023-05-23 15:51:06.000000 northgravity-0.1.8/northgravity.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 15:51:06.000000 northgravity-0.1.8/northgravity.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-05-23 15:51:06.000000 northgravity-0.1.8/northgravity.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 15:51:06.000000 northgravity-0.1.8/northgravity.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 15:51:06.645182 northgravity-0.1.8/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      829 2023-04-18 12:31:14.000000 northgravity-0.1.8/setup.py
```

### Comparing `northgravity-0.1.7/LICENSE` & `northgravity-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.7/PKG-INFO` & `northgravity-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: northgravity
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python SDK for NorthGravity platform
 Home-page: https://www.northgravity.com/
 Author: NorthGravity
 Author-email: info@northgravity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -40,19 +40,19 @@
 - **Time Series Handler** - retrieves data directly from the time series database
 
 
 
 ## How to install and set the package: 
 ### Install
 ```text
-pip3 install northgravity==0.1.7
+pip3 install northgravity==0.1.8
 ```
 As the library is available from pip, it can be installed as a specific version within a Python Task from within requirements.txt just by adding:
 ```text
-northgravity==0.1.7
+northgravity==0.1.8
 ```
 The package relies on the requests library so, in the project, the user must install this library in the requirements.txt file.
 ```text
 pip3 install requests==2.25.1
 ```
```

### Comparing `northgravity-0.1.7/README.md` & `northgravity-0.1.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -26,19 +26,19 @@
 - **Time Series Handler** - retrieves data directly from the time series database
 
 
 
 ## How to install and set the package: 
 ### Install
 ```text
-pip3 install northgravity==0.1.7
+pip3 install northgravity==0.1.8
 ```
 As the library is available from pip, it can be installed as a specific version within a Python Task from within requirements.txt just by adding:
 ```text
-northgravity==0.1.7
+northgravity==0.1.8
 ```
 The package relies on the requests library so, in the project, the user must install this library in the requirements.txt file.
 ```text
 pip3 install requests==2.25.1
 ```
```

### Comparing `northgravity-0.1.7/northgravity/Authenticator.py` & `northgravity-0.1.8/northgravity/Authenticator.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.7/northgravity/DatalakeHandler.py` & `northgravity-0.1.8/northgravity/DatalakeHandler.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         :return: the file matches on the datalake and their attributes
         '''
         if metadata_field not in ['', None]:
             assert metadata_value not in ['', None], 'If metadata_field is passed, the metadata_value should also exist. Please add metadata_value parameter'
         if metadata_value not in ['', None]:
             assert metadata_field not in ['', None], 'If metadata_field is passed, the metadata_value should also exist. Please add metadata_field parameter'
 
-        metadata_field = 'fields.'+ metadata_field
+            metadata_field = 'fields.'+ metadata_field
         log.debug(f'Search file: {file_name} of type {file_type} on group {group_name}')
 
         # Prepare query parameters
         init_query = {"name": file_name, "type": file_type, "uuid": None, "groupName": group_name, metadata_field:metadata_value}
         query = format_query(init_query)
 
         path = f'/file/search?size={size}&from={from_page}&query={query}'
@@ -164,42 +164,50 @@
                 'No file {} found on group {} with type {}: {}'.format(file_name, group_name, file_type, query))
 
         else:
             # Download by ID of the found file
             fid = query['items'][0]['fid']
             return self.download_by_id(file_id=fid, dest_file_name=dest_file_name, save=save, unzip=unzip)
 
-    def upload_file(self, file, group_name, file_upload_name=None, file_type='SOURCE', partial_update=False):
+    def upload_file(self, file, group_name, file_upload_name=None, file_type='SOURCE', partial_update=False, metadata_field=None, metadata_value=None):
         '''
         Upload the file to the datalake group with the given type (SOURCE as default)
 
         :param: file: either the path on the disk of the file to upload either the object directly
         :param: group_name: the name of the datalake group. if None, goes to the group where the pipeline is saved
         :param: file_upload_name: if not None, upload the file on the datalake with a different name
         :param: file_type: file type to save the file in the lake - SOURCE (default), NCSV ...
 
         :return: file unique ID on the datalake & the name on the datalake
         '''
 
         # Raise an error if the passed file is an object in RAM & no upload name was given
         if (not isinstance(file, str)) and (file_upload_name is None):
             raise ValueError('If uploading a file from RAM the file_upload_name must be given')
+        
+        if metadata_field not in ['', None]:
+            assert metadata_value not in ['', None], 'If metadata_field is passed, the metadata_value should also exist. Please add metadata_value parameter'
+        if metadata_value not in ['', None]:
+            assert metadata_field not in ['', None], 'If metadata_field is passed, the metadata_value should also exist. Please add metadata_field parameter'
 
         # Get the uploaded file name from path (original name) if none was passed
         file_name = file.split('/')[-1] if (file_upload_name is None) and isinstance(file, str) else file_upload_name
 
         log.info(f'Upload File with Name: {file_name} of type {file_type} to group {group_name}')
 
-        p_u = [{"name":"PARTIAL_UPDATE","value":"true"}] if partial_update is True else []
+        metadata_fields = [{"name":"PARTIAL_UPDATE","value":"true"}] if partial_update is True else []
+
+        if metadata_field not in ['', None]:
+            metadata_fields.append({"name":metadata_field,"value":metadata_value})
 
         # PAYLOAD for the upload of the file
         payload = {"groupName": group_name,
                    "fileName": file_name,
                    "fileType": file_type,
-                   "fields": p_u}
+                   "fields": metadata_fields}
 
         log.debug(f'Payload: {payload}')
 
         return self.caller.file_uploader(payload, file), file_name
 
 
 # ---------------------
```

### Comparing `northgravity-0.1.7/northgravity/HTTPCalller.py` & `northgravity-0.1.8/northgravity/HTTPCalller.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.7/northgravity/StatusHandler.py` & `northgravity-0.1.8/northgravity/StatusHandler.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.7/northgravity/TaskHandler.py` & `northgravity-0.1.8/northgravity/TaskHandler.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.7/northgravity/Timeseries.py` & `northgravity-0.1.8/northgravity/Timeseries.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.7/northgravity/__init__.py` & `northgravity-0.1.8/northgravity/__init__.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.7/northgravity.egg-info/PKG-INFO` & `northgravity-0.1.8/northgravity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: northgravity
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python SDK for NorthGravity platform
 Home-page: https://www.northgravity.com/
 Author: NorthGravity
 Author-email: info@northgravity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -40,19 +40,19 @@
 - **Time Series Handler** - retrieves data directly from the time series database
 
 
 
 ## How to install and set the package: 
 ### Install
 ```text
-pip3 install northgravity==0.1.7
+pip3 install northgravity==0.1.8
 ```
 As the library is available from pip, it can be installed as a specific version within a Python Task from within requirements.txt just by adding:
 ```text
-northgravity==0.1.7
+northgravity==0.1.8
 ```
 The package relies on the requests library so, in the project, the user must install this library in the requirements.txt file.
 ```text
 pip3 install requests==2.25.1
 ```
```

### Comparing `northgravity-0.1.7/setup.py` & `northgravity-0.1.8/setup.py`

 * *Files identical despite different names*

