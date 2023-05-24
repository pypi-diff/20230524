# Comparing `tmp/secret_message-0.5.tar.gz` & `tmp/secret_message-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secret_message-0.5.tar", last modified: Tue May 23 06:46:59 2023, max compression
+gzip compressed data, was "secret_message-0.6.tar", last modified: Wed May 24 17:40:20 2023, max compression
```

## Comparing `secret_message-0.5.tar` & `secret_message-0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-23 06:46:59.099506 secret_message-0.5/
--rw-rw----   0 root         (0) everybody  (9997)     1065 2023-05-22 13:17:48.000000 secret_message-0.5/LICENSE.txt
--rw-rw----   0 root         (0) everybody  (9997)     2713 2023-05-23 06:46:59.099506 secret_message-0.5/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     2335 2023-05-23 06:45:28.000000 secret_message-0.5/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-23 06:46:59.019507 secret_message-0.5/secret_message/
--rw-rw----   0 root         (0) everybody  (9997)     1762 2023-05-22 19:05:19.000000 secret_message-0.5/secret_message/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-23 06:46:59.069507 secret_message-0.5/secret_message.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     2713 2023-05-23 06:46:58.000000 secret_message-0.5/secret_message.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      209 2023-05-23 06:46:58.000000 secret_message-0.5/secret_message.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-23 06:46:58.000000 secret_message-0.5/secret_message.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       15 2023-05-23 06:46:58.000000 secret_message-0.5/secret_message.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-23 06:46:59.099506 secret_message-0.5/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     2881 2023-05-23 06:46:27.000000 secret_message-0.5/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-24 17:40:20.278383 secret_message-0.6/
+-rw-rw----   0 root         (0) everybody  (9997)     1065 2023-05-22 13:17:48.000000 secret_message-0.6/LICENSE.txt
+-rw-rw----   0 root         (0) everybody  (9997)     2713 2023-05-24 17:40:20.268383 secret_message-0.6/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     2335 2023-05-23 06:45:28.000000 secret_message-0.6/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-24 17:40:20.198383 secret_message-0.6/secret_message/
+-rw-rw----   0 root         (0) everybody  (9997)     1947 2023-05-24 17:39:22.000000 secret_message-0.6/secret_message/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-24 17:40:20.258383 secret_message-0.6/secret_message.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     2713 2023-05-24 17:40:19.000000 secret_message-0.6/secret_message.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      209 2023-05-24 17:40:19.000000 secret_message-0.6/secret_message.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-24 17:40:19.000000 secret_message-0.6/secret_message.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       15 2023-05-24 17:40:19.000000 secret_message-0.6/secret_message.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-24 17:40:20.278383 secret_message-0.6/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     2881 2023-05-24 17:39:45.000000 secret_message-0.6/setup.py
```

### Comparing `secret_message-0.5/LICENSE.txt` & `secret_message-0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `secret_message-0.5/PKG-INFO` & `secret_message-0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secret_message
-Version: 0.5
+Version: 0.6
 Summary: Create and share a Message Secretly.
 Author: E Lusifa Taehyung
 Author-email: purplebird7613@gmail.com
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `secret_message-0.5/README.md` & `secret_message-0.6/README.md`

 * *Files identical despite different names*

### Comparing `secret_message-0.5/secret_message/__init__.py` & `secret_message-0.6/secret_message/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 	print("Creating Message.....")	
 	response = requests.post(url,headers = headers,data = data)
 	os.system("clear")
 	
 	obj = json.loads(response.text)
 	print(json.dumps(obj,indent = 3,ensure_ascii = False))
 	
+	return json.dumps(obj,indent = 3,ensure_ascii = False)
+	
 # =====[] Showing Message ======
 def show(username,msg_url,msg_pass):
 	url = msg_url
 	
 	print(f"Connecting {username}.....")
 	User = user(username)
 	os.system("clear")
@@ -57,14 +59,16 @@
 	
 	print("Getting The Message......")	
 	response = requests.post(url,headers = headers,data = data)
 	os.system("clear")
 	
 	obj = json.loads(response.text)
 	print(json.dumps(obj["Message"],indent = 3,ensure_ascii = False))
+	
+	return json.dumps(obj["Message"],indent = 3,ensure_ascii = False)
 
 # ====== Message History ======
 def history(username):
 	url = f"{host}/api/message-history/"
 	
 	print(f"Connecting {username}.....")
 	User = user(username)
@@ -76,8 +80,10 @@
 	
 	print("Getting Message History.....")	
 	response = requests.get(url,headers = headers)
 	os.system("clear")
 	
 	obj = json.loads(response.text)
 	print(json.dumps(obj,indent = 3,ensure_ascii = False))
+	
+	return json.dumps(obj,indent = 3,ensure_ascii = False)
```

### Comparing `secret_message-0.5/secret_message.egg-info/PKG-INFO` & `secret_message-0.6/secret_message.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secret-message
-Version: 0.5
+Version: 0.6
 Summary: Create and share a Message Secretly.
 Author: E Lusifa Taehyung
 Author-email: purplebird7613@gmail.com
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `secret_message-0.5/setup.py` & `secret_message-0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 """          
 
 setuptools.setup(
 
 	name = 'secret_message', 
 
-	version = '0.5',
+	version = '0.6',
 
 	author = "E Lusifa Taehyung",
 
 	author_email = "purplebird7613@gmail.com",
 
 	description = "Create and share a Message Secretly.",
```

