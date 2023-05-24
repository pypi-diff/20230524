# Comparing `tmp/stringtokenizer-1.1.7.tar.gz` & `tmp/stringtokenizer-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stringtokenizer-1.1.7.tar", last modified: Wed May 24 17:00:09 2023, max compression
+gzip compressed data, was "stringtokenizer-1.1.8.tar", last modified: Wed May 24 18:35:03 2023, max compression
```

## Comparing `stringtokenizer-1.1.7.tar` & `stringtokenizer-1.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-24 17:00:09.785741 stringtokenizer-1.1.7/
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1500 2023-05-24 17:00:09.784575 stringtokenizer-1.1.7/PKG-INFO
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      953 2023-05-21 05:54:17.000000 stringtokenizer-1.1.7/README.md
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       38 2023-05-24 17:00:09.786187 stringtokenizer-1.1.7/setup.cfg
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      513 2023-05-24 16:59:29.000000 stringtokenizer-1.1.7/setup.py
-drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-24 17:00:09.771535 stringtokenizer-1.1.7/stringtokenizer/
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       46 2023-05-17 18:44:19.000000 stringtokenizer-1.1.7/stringtokenizer/__init__.py
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     2058 2023-05-24 16:59:52.000000 stringtokenizer-1.1.7/stringtokenizer/stringtokenizer.py
-drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-24 17:00:09.781889 stringtokenizer-1.1.7/stringtokenizer.egg-info/
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1500 2023-05-24 17:00:09.000000 stringtokenizer-1.1.7/stringtokenizer.egg-info/PKG-INFO
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      237 2023-05-24 17:00:09.000000 stringtokenizer-1.1.7/stringtokenizer.egg-info/SOURCES.txt
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        1 2023-05-24 17:00:09.000000 stringtokenizer-1.1.7/stringtokenizer.egg-info/dependency_links.txt
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       16 2023-05-24 17:00:09.000000 stringtokenizer-1.1.7/stringtokenizer.egg-info/top_level.txt
+drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-24 18:35:03.225759 stringtokenizer-1.1.8/
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1500 2023-05-24 18:35:03.225246 stringtokenizer-1.1.8/PKG-INFO
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      953 2023-05-21 05:54:17.000000 stringtokenizer-1.1.8/README.md
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       38 2023-05-24 18:35:03.225957 stringtokenizer-1.1.8/setup.cfg
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      513 2023-05-24 18:34:50.000000 stringtokenizer-1.1.8/setup.py
+drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-24 18:35:03.218884 stringtokenizer-1.1.8/stringtokenizer/
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       46 2023-05-17 18:44:19.000000 stringtokenizer-1.1.8/stringtokenizer/__init__.py
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     2097 2023-05-24 18:33:40.000000 stringtokenizer-1.1.8/stringtokenizer/stringtokenizer.py
+drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-24 18:35:03.223937 stringtokenizer-1.1.8/stringtokenizer.egg-info/
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1500 2023-05-24 18:35:02.000000 stringtokenizer-1.1.8/stringtokenizer.egg-info/PKG-INFO
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      237 2023-05-24 18:35:02.000000 stringtokenizer-1.1.8/stringtokenizer.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        1 2023-05-24 18:35:02.000000 stringtokenizer-1.1.8/stringtokenizer.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       16 2023-05-24 18:35:02.000000 stringtokenizer-1.1.8/stringtokenizer.egg-info/top_level.txt
```

### Comparing `stringtokenizer-1.1.7/PKG-INFO` & `stringtokenizer-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stringtokenizer
-Version: 1.1.7
+Version: 1.1.8
 Summary: A string tokenizer implementation
 Home-page: UNKNOWN
 Author: Tanmay Mandal
 Author-email: tanmay.mandal@zohomail.in
 License: MIT
 Description: **This project is a python implementation of the StringTokenizer class present in java**
```

### Comparing `stringtokenizer-1.1.7/README.md` & `stringtokenizer-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `stringtokenizer-1.1.7/setup.py` & `stringtokenizer-1.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(
     name='stringtokenizer',
-    version='1.1.7',
+    version='1.1.8',
     license='MIT',
     description='A string tokenizer implementation',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Tanmay Mandal',
     author_email='tanmay.mandal@zohomail.in',
     packages=['stringtokenizer'],
```

### Comparing `stringtokenizer-1.1.7/stringtokenizer/stringtokenizer.py` & `stringtokenizer-1.1.8/stringtokenizer/stringtokenizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,17 +54,19 @@
                 self.nextToken()
                 c+=1
         except Exception:
             pass
         self.__tokens=temp
         return c
     def __flatten__(self,d):
-    	d=list(d)
+    	t=list(d)
+    	if type(d)==str
+    	    return t
     	nd=[]
-    	for i in d:
+    	for i in t:
     		if len(i)==0:
     			...
     		elif type(i)!=str:
     			nd.extend(self.__flatten__(i))
     		else:
     			nd.extend(list(i))
     	return nd
```

### Comparing `stringtokenizer-1.1.7/stringtokenizer.egg-info/PKG-INFO` & `stringtokenizer-1.1.8/stringtokenizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stringtokenizer
-Version: 1.1.7
+Version: 1.1.8
 Summary: A string tokenizer implementation
 Home-page: UNKNOWN
 Author: Tanmay Mandal
 Author-email: tanmay.mandal@zohomail.in
 License: MIT
 Description: **This project is a python implementation of the StringTokenizer class present in java**
```

