# Comparing `tmp/enc_tool-1.1.0.tar.gz` & `tmp/enc_tool-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enc_tool-1.1.0.tar", last modified: Fri May 19 09:28:26 2023, max compression
+gzip compressed data, was "enc_tool-1.1.2.tar", last modified: Wed May 24 11:13:18 2023, max compression
```

## Comparing `enc_tool-1.1.0.tar` & `enc_tool-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxr-x   0 night-error  (1000) night-error  (1000)        0 2023-05-19 09:28:26.035150 enc_tool-1.1.0/
--rw-rw-r--   0 night-error  (1000) night-error  (1000)     1623 2023-05-19 09:28:26.035150 enc_tool-1.1.0/PKG-INFO
--rw-rw-r--   0 night-error  (1000) night-error  (1000)     1419 2023-05-19 09:17:51.000000 enc_tool-1.1.0/README.md
-drwxrwxr-x   0 night-error  (1000) night-error  (1000)        0 2023-05-19 09:28:26.027150 enc_tool-1.1.0/enc_tool.egg-info/
--rw-rw-r--   0 night-error  (1000) night-error  (1000)     1623 2023-05-19 09:28:25.000000 enc_tool-1.1.0/enc_tool.egg-info/PKG-INFO
--rw-rw-r--   0 night-error  (1000) night-error  (1000)      332 2023-05-19 09:28:26.000000 enc_tool-1.1.0/enc_tool.egg-info/SOURCES.txt
--rw-rw-r--   0 night-error  (1000) night-error  (1000)        1 2023-05-19 09:28:25.000000 enc_tool-1.1.0/enc_tool.egg-info/dependency_links.txt
--rw-rw-r--   0 night-error  (1000) night-error  (1000)       54 2023-05-19 09:28:25.000000 enc_tool-1.1.0/enc_tool.egg-info/entry_points.txt
--rw-rw-r--   0 night-error  (1000) night-error  (1000)       22 2023-05-19 09:28:25.000000 enc_tool-1.1.0/enc_tool.egg-info/requires.txt
--rw-rw-r--   0 night-error  (1000) night-error  (1000)       20 2023-05-19 09:28:25.000000 enc_tool-1.1.0/enc_tool.egg-info/top_level.txt
-drwxrwxr-x   0 night-error  (1000) night-error  (1000)        0 2023-05-19 09:28:26.031150 enc_tool-1.1.0/encrypter_decrypter/
--rw-rw-r--   0 night-error  (1000) night-error  (1000)        0 2023-05-19 08:07:57.000000 enc_tool-1.1.0/encrypter_decrypter/__init__.py
--rw-rw-r--   0 night-error  (1000) night-error  (1000)     2292 2023-05-19 08:49:47.000000 enc_tool-1.1.0/encrypter_decrypter/enc_tool.py
--rw-rw-r--   0 night-error  (1000) night-error  (1000)     3565 2023-05-19 09:18:22.000000 enc_tool-1.1.0/encrypter_decrypter/main.py
--rw-rw-r--   0 night-error  (1000) night-error  (1000)      101 2023-05-19 09:07:41.000000 enc_tool-1.1.0/encrypter_decrypter/test.py
--rw-rw-r--   0 night-error  (1000) night-error  (1000)       38 2023-05-19 09:28:26.035150 enc_tool-1.1.0/setup.cfg
--rw-rw-r--   0 night-error  (1000) night-error  (1000)      860 2023-05-19 09:12:43.000000 enc_tool-1.1.0/setup.py
+drwxrwxr-x   0 night-error  (1000) night-error  (1000)        0 2023-05-24 11:13:18.030509 enc_tool-1.1.2/
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)     1669 2023-05-24 11:13:18.030509 enc_tool-1.1.2/PKG-INFO
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)     1419 2023-05-19 09:17:51.000000 enc_tool-1.1.2/README.md
+drwxrwxr-x   0 night-error  (1000) night-error  (1000)        0 2023-05-24 11:13:18.026509 enc_tool-1.1.2/enc_tool.egg-info/
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)     1669 2023-05-24 11:13:17.000000 enc_tool-1.1.2/enc_tool.egg-info/PKG-INFO
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)      408 2023-05-24 11:13:17.000000 enc_tool-1.1.2/enc_tool.egg-info/SOURCES.txt
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)        1 2023-05-24 11:13:17.000000 enc_tool-1.1.2/enc_tool.egg-info/dependency_links.txt
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)       54 2023-05-24 11:13:17.000000 enc_tool-1.1.2/enc_tool.egg-info/entry_points.txt
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)       22 2023-05-24 11:13:17.000000 enc_tool-1.1.2/enc_tool.egg-info/requires.txt
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)       20 2023-05-24 11:13:17.000000 enc_tool-1.1.2/enc_tool.egg-info/top_level.txt
+drwxrwxr-x   0 night-error  (1000) night-error  (1000)        0 2023-05-24 11:13:18.030509 enc_tool-1.1.2/encrypter_decrypter/
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)        0 2023-05-19 08:07:57.000000 enc_tool-1.1.2/encrypter_decrypter/__init__.py
+drwxrwxr-x   0 night-error  (1000) night-error  (1000)        0 2023-05-24 11:13:18.030509 enc_tool-1.1.2/encrypter_decrypter/config/
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)        0 2023-05-19 09:52:29.000000 enc_tool-1.1.2/encrypter_decrypter/config/__init__.py
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)      140 2023-05-24 09:44:04.000000 enc_tool-1.1.2/encrypter_decrypter/config/config.py
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)     2596 2023-05-24 09:42:41.000000 enc_tool-1.1.2/encrypter_decrypter/enc_tool.py
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)     3499 2023-05-19 10:00:21.000000 enc_tool-1.1.2/encrypter_decrypter/main.py
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)       15 2023-05-24 11:06:08.000000 enc_tool-1.1.2/encrypter_decrypter/test.py
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)       38 2023-05-24 11:13:18.030509 enc_tool-1.1.2/setup.cfg
+-rw-rw-r--   0 night-error  (1000) night-error  (1000)      736 2023-05-19 09:55:10.000000 enc_tool-1.1.2/setup.py
```

### Comparing `enc_tool-1.1.0/PKG-INFO` & `enc_tool-1.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: enc_tool
-Version: 1.1.0
-Summary: A tool to encrypt and decrypt your data! 
+Version: 1.1.2
+Summary: A tool to encrypt and decrypt your data! Use it to make your messages and files safe...
 Author: Night Error
 Author-email: night.error.go@gmail.com
 Description-Content-Type: text/markdown
 
 # ENC Tool
 A Python command-line too encrypt and decrypt your data securely.
 <br><br>
```

### Comparing `enc_tool-1.1.0/README.md` & `enc_tool-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `enc_tool-1.1.0/enc_tool.egg-info/PKG-INFO` & `enc_tool-1.1.2/enc_tool.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: enc-tool
-Version: 1.1.0
-Summary: A tool to encrypt and decrypt your data! 
+Version: 1.1.2
+Summary: A tool to encrypt and decrypt your data! Use it to make your messages and files safe...
 Author: Night Error
 Author-email: night.error.go@gmail.com
 Description-Content-Type: text/markdown
 
 # ENC Tool
 A Python command-line too encrypt and decrypt your data securely.
 <br><br>
```

### Comparing `enc_tool-1.1.0/encrypter_decrypter/enc_tool.py` & `enc_tool-1.1.2/encrypter_decrypter/enc_tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,18 +36,26 @@
         sys.exit()
 
     # return encrypted data
     return encrypted_message.decode()
 
 
 def save_data(data, path):
-
-    with open(path, 'w') as file:
+    try:
+        with open(path, 'w') as file:
             file.write(data)
-    return path
+        return path
+    except IsADirectoryError:
+        print(Fore.RED + "Error: Please enter a valid path to save your encrypted data!")
+        sys.exit()
+    except FileNotFoundError:
+        print(Fore.RED + "Error: Please enter a valid path to save your encrypted data!")
+        sys.exit()
+
+        
 
 
 def read_data(path):
     try:
         with open(path, 'r', encoding='utf-8') as file:
             data = file.read()
         return data
```

### Comparing `enc_tool-1.1.0/encrypter_decrypter/main.py` & `enc_tool-1.1.2/encrypter_decrypter/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from encrypter_decrypter import enc_tool as enc
 import argparse
 import json
+from encrypter_decrypter.config import config
 # Just styles
 from colorama import Fore, Style, init
 init(autoreset=True)
 
-# read data from config file
-with open("encrypter_decrypter/config/config.json", "r") as file:
-    config = json.load(file)
+
 
 
 def main():
-    parser = argparse.ArgumentParser(prog= config['name'], 
-                                    description= config['description'])
+    parser = argparse.ArgumentParser(prog= config.NAME + config.VERSION, 
+                                    description= config.DESCRIPTION)
     parser.add_argument('data', nargs='?', help="The message you want to encrypt.")
     parser.add_argument('-p', '--password', help="Password to encrypt or decrypt your data.", required=True)
     parser.add_argument('-d', '--decrypt', help="Add this for decryption", action="store_true")
     parser.add_argument('-s', '--save', help="Path to file that encrypted / decrypted data will be saved in.")
     parser.add_argument('-f', '--file', help="Path to file that you want encrypt / decrypt data in it.")
     args = parser.parse_args()
```

### Comparing `enc_tool-1.1.0/setup.py` & `enc_tool-1.1.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 from setuptools import setup, find_packages
 import os
-import json
+from encrypter_decrypter.config import config
 
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-# read data from config file
-with open(os.path.join(directory, "encrypter_decrypter/config/config.json"), "r") as file:
-    config = json.load(file)
-
 setup(
-    name=config['name'],
-    version= config['version'],
+    name=config.NAME,
+    version= config.VERSION,
     packages=find_packages(),
-    description= config['description'],
+    description= config.DESCRIPTION,
     long_description= long_description,
     long_description_content_type="text/markdown",
-    author= config['author'],
-    author_email= config['author_email'],
+    author= "Night Error",
+    author_email= "night.error.go@gmail.com",
 
     entry_points={
         'console_scripts': [
             'enc = encrypter_decrypter.main:main',
         ],
     },
     install_requires=[
```

