# Comparing `tmp/stringtokenizer-1.1.3.tar.gz` & `tmp/stringtokenizer-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stringtokenizer-1.1.3.tar", last modified: Mon May 22 08:49:04 2023, max compression
+gzip compressed data, was "stringtokenizer-1.1.4.tar", last modified: Wed May 24 16:25:47 2023, max compression
```

## Comparing `stringtokenizer-1.1.3.tar` & `stringtokenizer-1.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-22 08:49:04.304425 stringtokenizer-1.1.3/
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1500 2023-05-22 08:49:04.303981 stringtokenizer-1.1.3/PKG-INFO
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      953 2023-05-21 05:54:17.000000 stringtokenizer-1.1.3/README.md
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       38 2023-05-22 08:49:04.304525 stringtokenizer-1.1.3/setup.cfg
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      513 2023-05-22 08:48:40.000000 stringtokenizer-1.1.3/setup.py
-drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-22 08:49:04.301788 stringtokenizer-1.1.3/stringtokenizer/
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       46 2023-05-17 18:44:19.000000 stringtokenizer-1.1.3/stringtokenizer/__init__.py
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1595 2023-05-21 05:49:54.000000 stringtokenizer-1.1.3/stringtokenizer/stringtokenizer.py
-drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-22 08:49:04.303464 stringtokenizer-1.1.3/stringtokenizer.egg-info/
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1500 2023-05-22 08:49:04.000000 stringtokenizer-1.1.3/stringtokenizer.egg-info/PKG-INFO
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      237 2023-05-22 08:49:04.000000 stringtokenizer-1.1.3/stringtokenizer.egg-info/SOURCES.txt
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        1 2023-05-22 08:49:04.000000 stringtokenizer-1.1.3/stringtokenizer.egg-info/dependency_links.txt
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       16 2023-05-22 08:49:04.000000 stringtokenizer-1.1.3/stringtokenizer.egg-info/top_level.txt
+drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-24 16:25:47.696097 stringtokenizer-1.1.4/
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1500 2023-05-24 16:25:47.695793 stringtokenizer-1.1.4/PKG-INFO
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      953 2023-05-21 05:54:17.000000 stringtokenizer-1.1.4/README.md
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       38 2023-05-24 16:25:47.696191 stringtokenizer-1.1.4/setup.cfg
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      513 2023-05-24 16:25:36.000000 stringtokenizer-1.1.4/setup.py
+drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-24 16:25:47.693164 stringtokenizer-1.1.4/stringtokenizer/
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       46 2023-05-17 18:44:19.000000 stringtokenizer-1.1.4/stringtokenizer/__init__.py
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     2034 2023-05-24 16:23:46.000000 stringtokenizer-1.1.4/stringtokenizer/stringtokenizer.py
+drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-24 16:25:47.695277 stringtokenizer-1.1.4/stringtokenizer.egg-info/
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1500 2023-05-24 16:25:47.000000 stringtokenizer-1.1.4/stringtokenizer.egg-info/PKG-INFO
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      237 2023-05-24 16:25:47.000000 stringtokenizer-1.1.4/stringtokenizer.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        1 2023-05-24 16:25:47.000000 stringtokenizer-1.1.4/stringtokenizer.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       16 2023-05-24 16:25:47.000000 stringtokenizer-1.1.4/stringtokenizer.egg-info/top_level.txt
```

### Comparing `stringtokenizer-1.1.3/PKG-INFO` & `stringtokenizer-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stringtokenizer
-Version: 1.1.3
+Version: 1.1.4
 Summary: A string tokenizer implementation
 Home-page: UNKNOWN
 Author: Tanmay Mandal
 Author-email: tanmay.mandal@zohomail.in
 License: MIT
 Description: **This project is a python implementation of the StringTokenizer class present in java**
```

### Comparing `stringtokenizer-1.1.3/README.md` & `stringtokenizer-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `stringtokenizer-1.1.3/setup.py` & `stringtokenizer-1.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(
     name='stringtokenizer',
-    version='1.1.3',
+    version='1.1.4',
     license='MIT',
     description='A string tokenizer implementation',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Tanmay Mandal',
     author_email='tanmay.mandal@zohomail.in',
     packages=['stringtokenizer'],
```

### Comparing `stringtokenizer-1.1.3/stringtokenizer/stringtokenizer.py` & `stringtokenizer-1.1.4/stringtokenizer/stringtokenizer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 class StringTokenizer:
     def __init__(self,st,delim=' \t\n\r\f',retdelim=False):
         if type(retdelim)!=bool:
             raise TypeError("Expected <class 'bool'> received "+str(type(retdelim)))
         self.__tokens=list(st)
-        self.__delim=tuple(delim)
+        try:
+            self.__delim=tuple(__flatten__(delim))
+        except Exception:
+            raise TypeError('Invalid Delimeter Group')
         self.__retdelim=retdelim
     def nextToken(self,delim=None):
         if delim==None:
             delim=self.__delim
         else:
-            delim=tuple(delim)
+            try:
+                delim=tuple(__flatten__(delim))
+            except Exception:
+                raise TypeError('Invalid Delimeter Group')
             self.__delim=delim
         temp=''
         while len(self.__tokens)>0:
             if temp=='' and self.__tokens[0] in delim:
                 if self.__retdelim:
                     temp=self.__tokens[0]
                     del self.__tokens[0]
@@ -47,7 +53,18 @@
             while True:
                 self.nextToken()
                 c+=1
         except Exception:
             pass
         self.__tokens=temp
         return c
+    def __flatten__(d):
+    	d=list(d)
+    	nd=[]
+    	for i in d:
+    		if len(i)==0:
+    			...
+    		elif type(i)!=str:
+    			nd.extend(flatten(i))
+    		else:
+    			nd.extend(list(i))
+    	return nd
```

### Comparing `stringtokenizer-1.1.3/stringtokenizer.egg-info/PKG-INFO` & `stringtokenizer-1.1.4/stringtokenizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stringtokenizer
-Version: 1.1.3
+Version: 1.1.4
 Summary: A string tokenizer implementation
 Home-page: UNKNOWN
 Author: Tanmay Mandal
 Author-email: tanmay.mandal@zohomail.in
 License: MIT
 Description: **This project is a python implementation of the StringTokenizer class present in java**
```

