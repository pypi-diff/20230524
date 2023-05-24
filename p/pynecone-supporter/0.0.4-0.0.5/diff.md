# Comparing `tmp/pynecone-supporter-0.0.4.tar.gz` & `tmp/pynecone-supporter-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynecone-supporter-0.0.4.tar", last modified: Thu Mar 16 11:32:05 2023, max compression
+gzip compressed data, was "pynecone-supporter-0.0.5.tar", last modified: Wed May 24 08:14:28 2023, max compression
```

## Comparing `pynecone-supporter-0.0.4.tar` & `pynecone-supporter-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 11:32:05.907724 pynecone-supporter-0.0.4/
--rw-r--r--   0 root         (0) root         (0)     1421 2023-03-16 11:32:05.906725 pynecone-supporter-0.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1139 2023-03-16 11:32:05.000000 pynecone-supporter-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 11:32:05.904724 pynecone-supporter-0.0.4/pynecone_supporter/
--rw-r--r--   0 root         (0) root         (0)       76 2023-03-16 11:32:05.000000 pynecone-supporter-0.0.4/pynecone_supporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 11:32:05.906725 pynecone-supporter-0.0.4/pynecone_supporter/components/
--rw-r--r--   0 root         (0) root         (0)      238 2023-03-16 11:32:05.000000 pynecone-supporter-0.0.4/pynecone_supporter/components/__init__.py
--rw-r--r--   0 root         (0) root         (0)      484 2023-03-16 11:32:05.000000 pynecone-supporter-0.0.4/pynecone_supporter/components/color_picker.py
--rw-r--r--   0 root         (0) root         (0)      491 2023-03-16 11:32:05.000000 pynecone-supporter-0.0.4/pynecone_supporter/components/json_editor.py
--rw-r--r--   0 root         (0) root         (0)      509 2023-03-16 11:32:05.000000 pynecone-supporter-0.0.4/pynecone_supporter/components/jumo_button.py
--rw-r--r--   0 root         (0) root         (0)      250 2023-03-16 11:32:05.000000 pynecone-supporter-0.0.4/pynecone_supporter/components/webcam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 11:32:05.905724 pynecone-supporter-0.0.4/pynecone_supporter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1421 2023-03-16 11:32:05.000000 pynecone-supporter-0.0.4/pynecone_supporter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      517 2023-03-16 11:32:05.000000 pynecone-supporter-0.0.4/pynecone_supporter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-16 11:32:05.000000 pynecone-supporter-0.0.4/pynecone_supporter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-16 11:32:05.000000 pynecone-supporter-0.0.4/pynecone_supporter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-16 11:32:05.000000 pynecone-supporter-0.0.4/pynecone_supporter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-03-16 11:32:05.000000 pynecone-supporter-0.0.4/pynecone_supporter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-16 11:32:05.907724 pynecone-supporter-0.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      606 2023-03-16 11:32:05.000000 pynecone-supporter-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:14:28.813272 pynecone-supporter-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)     1403 2023-05-24 08:14:28.813272 pynecone-supporter-0.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-05-24 08:14:27.000000 pynecone-supporter-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:14:28.810272 pynecone-supporter-0.0.5/pynecone_supporter/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-05-24 08:14:27.000000 pynecone-supporter-0.0.5/pynecone_supporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:14:28.813272 pynecone-supporter-0.0.5/pynecone_supporter/components/
+-rw-r--r--   0 root         (0) root         (0)      242 2023-05-24 08:14:27.000000 pynecone-supporter-0.0.5/pynecone_supporter/components/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      489 2023-05-24 08:14:27.000000 pynecone-supporter-0.0.5/pynecone_supporter/components/color_picker.py
+-rw-r--r--   0 root         (0) root         (0)      496 2023-05-24 08:14:27.000000 pynecone-supporter-0.0.5/pynecone_supporter/components/json_editor.py
+-rw-r--r--   0 root         (0) root         (0)      514 2023-05-24 08:14:27.000000 pynecone-supporter-0.0.5/pynecone_supporter/components/jumo_button.py
+-rw-r--r--   0 root         (0) root         (0)      250 2023-05-24 08:14:27.000000 pynecone-supporter-0.0.5/pynecone_supporter/components/webcam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:14:28.811272 pynecone-supporter-0.0.5/pynecone_supporter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1403 2023-05-24 08:14:28.000000 pynecone-supporter-0.0.5/pynecone_supporter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      517 2023-05-24 08:14:28.000000 pynecone-supporter-0.0.5/pynecone_supporter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 08:14:28.000000 pynecone-supporter-0.0.5/pynecone_supporter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 08:14:28.000000 pynecone-supporter-0.0.5/pynecone_supporter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-24 08:14:28.000000 pynecone-supporter-0.0.5/pynecone_supporter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-24 08:14:28.000000 pynecone-supporter-0.0.5/pynecone_supporter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 08:14:28.814272 pynecone-supporter-0.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      606 2023-05-24 08:14:27.000000 pynecone-supporter-0.0.5/setup.py
```

### Comparing `pynecone-supporter-0.0.4/PKG-INFO` & `pynecone-supporter-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pynecone-supporter
-Version: 0.0.4
+Version: 0.0.5
 Summary: Pynecone supporter
 Home-page: https://github.com/automatethem/pynecone-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # pynecone-supporter
 
 https://pypi.org/project/pynecone-supporter
 <pre>
 pip install pynecone-supporter
```

### Comparing `pynecone-supporter-0.0.4/README.md` & `pynecone-supporter-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pynecone-supporter-0.0.4/pynecone_supporter.egg-info/PKG-INFO` & `pynecone-supporter-0.0.5/pynecone_supporter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pynecone-supporter
-Version: 0.0.4
+Version: 0.0.5
 Summary: Pynecone supporter
 Home-page: https://github.com/automatethem/pynecone-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # pynecone-supporter
 
 https://pypi.org/project/pynecone-supporter
 <pre>
 pip install pynecone-supporter
```

### Comparing `pynecone-supporter-0.0.4/pynecone_supporter.egg-info/SOURCES.txt` & `pynecone-supporter-0.0.5/pynecone_supporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynecone-supporter-0.0.4/setup.py` & `pynecone-supporter-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 setuptools.setup(
 	name='pynecone-supporter',
-	version='0.0.4',
+	version='0.0.5',
 	description='Pynecone supporter',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	author='Sang Ki Kwon',
 	url='https://github.com/automatethem/pynecone-supporter',
 	install_requires=requirements(),
 	author_email='automatethem@gmail.com',
```

