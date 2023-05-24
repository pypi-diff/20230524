# Comparing `tmp/dingtalk-stream-0.2.1.tar.gz` & `tmp/dingtalk-stream-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingtalk-stream-0.2.1.tar", last modified: Mon May 22 05:04:44 2023, max compression
+gzip compressed data, was "dingtalk-stream-0.2.2.tar", last modified: Wed May 24 11:59:12 2023, max compression
```

## Comparing `dingtalk-stream-0.2.1.tar` & `dingtalk-stream-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 05:04:44.620638 dingtalk-stream-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-22 05:04:42.000000 dingtalk-stream-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-22 05:04:44.616638 dingtalk-stream-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-22 05:04:42.000000 dingtalk-stream-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 05:04:44.616638 dingtalk-stream-0.2.1/dingtalk_stream/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-22 05:04:42.000000 dingtalk-stream-0.2.1/dingtalk_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-05-22 05:04:42.000000 dingtalk-stream-0.2.1/dingtalk_stream/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-22 05:04:42.000000 dingtalk-stream-0.2.1/dingtalk_stream/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-05-22 05:04:42.000000 dingtalk-stream-0.2.1/dingtalk_stream/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-22 05:04:42.000000 dingtalk-stream-0.2.1/dingtalk_stream/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-22 05:04:42.000000 dingtalk-stream-0.2.1/dingtalk_stream/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-05-22 05:04:42.000000 dingtalk-stream-0.2.1/dingtalk_stream/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 05:04:44.616638 dingtalk-stream-0.2.1/dingtalk_stream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-22 05:04:44.000000 dingtalk-stream-0.2.1/dingtalk_stream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-22 05:04:44.000000 dingtalk-stream-0.2.1/dingtalk_stream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 05:04:44.000000 dingtalk-stream-0.2.1/dingtalk_stream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-22 05:04:44.000000 dingtalk-stream-0.2.1/dingtalk_stream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-22 05:04:44.000000 dingtalk-stream-0.2.1/dingtalk_stream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 05:04:44.620638 dingtalk-stream-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-22 05:04:42.000000 dingtalk-stream-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:59:12.641217 dingtalk-stream-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-24 11:59:11.000000 dingtalk-stream-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-24 11:59:12.641217 dingtalk-stream-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-24 11:59:11.000000 dingtalk-stream-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:59:12.641217 dingtalk-stream-0.2.2/dingtalk_stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-24 11:59:11.000000 dingtalk-stream-0.2.2/dingtalk_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-05-24 11:59:11.000000 dingtalk-stream-0.2.2/dingtalk_stream/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-24 11:59:11.000000 dingtalk-stream-0.2.2/dingtalk_stream/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-05-24 11:59:11.000000 dingtalk-stream-0.2.2/dingtalk_stream/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-24 11:59:11.000000 dingtalk-stream-0.2.2/dingtalk_stream/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-24 11:59:11.000000 dingtalk-stream-0.2.2/dingtalk_stream/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-05-24 11:59:11.000000 dingtalk-stream-0.2.2/dingtalk_stream/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:59:12.641217 dingtalk-stream-0.2.2/dingtalk_stream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-24 11:59:12.000000 dingtalk-stream-0.2.2/dingtalk_stream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-24 11:59:12.000000 dingtalk-stream-0.2.2/dingtalk_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 11:59:12.000000 dingtalk-stream-0.2.2/dingtalk_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-24 11:59:12.000000 dingtalk-stream-0.2.2/dingtalk_stream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-24 11:59:12.000000 dingtalk-stream-0.2.2/dingtalk_stream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 11:59:12.641217 dingtalk-stream-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-24 11:59:11.000000 dingtalk-stream-0.2.2/setup.py
```

### Comparing `dingtalk-stream-0.2.1/LICENSE` & `dingtalk-stream-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.2.1/PKG-INFO` & `dingtalk-stream-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.2.1/README.md` & `dingtalk-stream-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.2.1/dingtalk_stream/chatbot.py` & `dingtalk-stream-0.2.2/dingtalk_stream/chatbot.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.2.1/dingtalk_stream/frames.py` & `dingtalk-stream-0.2.2/dingtalk_stream/frames.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.2.1/dingtalk_stream/handlers.py` & `dingtalk-stream-0.2.2/dingtalk_stream/handlers.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.2.1/dingtalk_stream/stream.py` & `dingtalk-stream-0.2.2/dingtalk_stream/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,17 +143,18 @@
             'subscriptions': topics,
         }).encode('utf-8')
 
         try:
             response = requests.post(DingTalkStreamClient.OPEN_CONNECTION_API,
                                      headers=request_headers,
                                      data=request_body)
+            http_body = response.json()
             response.raise_for_status()
         except Exception as e:
-            self.logger.error("open connection failed, error=%s", e)
+            self.logger.error("open connection failed, error=%s, response.body=%s", e, http_body)
             return None
         return response.json()
 
     def reset_access_token(self):
         """ reset token if open api return 401 """
         self._access_token = {}
```

### Comparing `dingtalk-stream-0.2.1/dingtalk_stream.egg-info/PKG-INFO` & `dingtalk-stream-0.2.2/dingtalk_stream.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.2.1/setup.py` & `dingtalk-stream-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='dingtalk-stream',
-    version='0.2.1',
+    version='0.2.2',
     description='A Python library for sending messages to DingTalk chatbot',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/open-dingtalk/dingtalk-stream-sdk-python',
     author='Ke Jie',
     author_email='jinxi.kj@alibaba-inc.com',
     license='MIT',
```

