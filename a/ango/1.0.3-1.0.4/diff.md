# Comparing `tmp/ango-1.0.3.tar.gz` & `tmp/ango-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ango-1.0.3.tar", last modified: Wed May 17 14:28:39 2023, max compression
+gzip compressed data, was "ango-1.0.4.tar", last modified: Wed May 24 08:30:56 2023, max compression
```

## Comparing `ango-1.0.3.tar` & `ango-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-17 14:28:39.297436 ango-1.0.3/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-17 14:28:39.297436 ango-1.0.3/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 ango-1.0.3/README.md
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-17 14:28:39.297436 ango-1.0.3/ango/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.3/ango/__init__.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-17 14:28:39.297436 ango-1.0.3/ango/models/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.3/ango/models/__init__.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-03-08 06:39:17.000000 ango-1.0.3/ango/models/enums.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5421 2023-01-23 13:16:24.000000 ango-1.0.3/ango/models/label_category.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-02-08 11:40:21.000000 ango-1.0.3/ango/plugin_logger.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5337 2023-05-17 13:09:55.000000 ango-1.0.3/ango/plugins.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)    14425 2023-05-17 14:28:05.000000 ango-1.0.3/ango/sdk.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-17 14:28:39.297436 ango-1.0.3/ango.egg-info/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-17 14:28:39.000000 ango-1.0.3/ango.egg-info/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      299 2023-05-17 14:28:39.000000 ango-1.0.3/ango.egg-info/SOURCES.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-05-17 14:28:39.000000 ango-1.0.3/ango.egg-info/dependency_links.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      130 2023-05-17 14:28:39.000000 ango-1.0.3/ango.egg-info/requires.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        5 2023-05-17 14:28:39.000000 ango-1.0.3/ango.egg-info/top_level.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-05-17 14:28:39.297436 ango-1.0.3/setup.cfg
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      864 2023-05-17 12:30:01.000000 ango-1.0.3/setup.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-24 08:30:56.446047 ango-1.0.4/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-24 08:30:56.446047 ango-1.0.4/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 ango-1.0.4/README.md
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-24 08:30:56.446047 ango-1.0.4/ango/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.4/ango/__init__.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-24 08:30:56.446047 ango-1.0.4/ango/models/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.4/ango/models/__init__.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-03-08 06:39:17.000000 ango-1.0.4/ango/models/enums.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5421 2023-01-23 13:16:24.000000 ango-1.0.4/ango/models/label_category.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-02-08 11:40:21.000000 ango-1.0.4/ango/plugin_logger.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5433 2023-05-24 08:30:39.000000 ango-1.0.4/ango/plugins.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)    14425 2023-05-17 14:28:05.000000 ango-1.0.4/ango/sdk.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-24 08:30:56.446047 ango-1.0.4/ango.egg-info/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-24 08:30:56.000000 ango-1.0.4/ango.egg-info/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      299 2023-05-24 08:30:56.000000 ango-1.0.4/ango.egg-info/SOURCES.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-05-24 08:30:56.000000 ango-1.0.4/ango.egg-info/dependency_links.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      130 2023-05-24 08:30:56.000000 ango-1.0.4/ango.egg-info/requires.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        5 2023-05-24 08:30:56.000000 ango-1.0.4/ango.egg-info/top_level.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-05-24 08:30:56.446047 ango-1.0.4/setup.cfg
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      864 2023-05-24 08:30:39.000000 ango-1.0.4/setup.py
```

### Comparing `ango-1.0.3/PKG-INFO` & `ango-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 1.0.3
+Version: 1.0.4
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ango-1.0.3/README.md` & `ango-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ango-1.0.3/ango/models/label_category.py` & `ango-1.0.4/ango/models/label_category.py`

 * *Files identical despite different names*

### Comparing `ango-1.0.3/ango/plugin_logger.py` & `ango-1.0.4/ango/plugin_logger.py`

 * *Files identical despite different names*

### Comparing `ango-1.0.3/ango/plugins.py` & `ango-1.0.4/ango/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,16 @@
         super().__init__(id, secret, callback)
         self.host = host
 
     def on_plugin(self, data):
         workflow = data.get('workflow')
         if not workflow:
             return super().on_plugin(data)
+        #data["logger"] = self._get_logger(data)
+        data["batches"] = data.get('tags', [])
         api_key = data.get('apiKey')
         task_id = data.get('labeltask').get('_id')
         sdk = SDK(api_key=api_key, host=self.host)
         answer = self.callback(**data)
         annotation = {
             "tools": answer.get("answer").get("objects") + data.get('labeltask').get("answer").get("tools"),
             "classifications": answer.get("answer").get("classifications") + data.get('labeltask').get("answer").get("classifications"),
```

### Comparing `ango-1.0.3/ango/sdk.py` & `ango-1.0.4/ango/sdk.py`

 * *Files identical despite different names*

### Comparing `ango-1.0.3/ango.egg-info/PKG-INFO` & `ango-1.0.4/ango.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 1.0.3
+Version: 1.0.4
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ango-1.0.3/setup.py` & `ango-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="ango",
-    version="1.0.3",
+    version="1.0.4",
     author="Faruk Karakaya",
     author_email="<faruk@ango.ai>",
     description="Ango-Hub SDK",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
-        "python-socketio~=5.5.2",
+        "python-socketio~=5.8.0",
         "APScheduler~=3.9.1",
         "websocket-client",
         "flask-socketio",
         "requests~=2.27.1",
         "tqdm",
         "validators~=0.20.0",
         "boto3~=1.26.30",
```

