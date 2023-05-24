# Comparing `tmp/snbtlib-0.0.7.tar.gz` & `tmp/snbtlib-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snbtlib-0.0.7.tar", last modified: Tue Apr 18 02:15:02 2023, max compression
+gzip compressed data, was "snbtlib-0.1.0.tar", last modified: Wed May 24 01:39:48 2023, max compression
```

## Comparing `snbtlib-0.0.7.tar` & `snbtlib-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 02:15:02.762783 snbtlib-0.0.7/
--rw-rw-rw-   0        0        0     1085 2023-02-07 06:40:54.000000 snbtlib-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      716 2023-04-18 02:15:02.762783 snbtlib-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      425 2023-03-08 06:57:28.000000 snbtlib-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-04-18 02:15:02.763784 snbtlib-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      558 2023-04-18 02:13:31.000000 snbtlib-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:15:02.758783 snbtlib-0.0.7/snbtlib/
--rw-rw-rw-   0        0        0      302 2023-04-18 02:12:57.000000 snbtlib-0.0.7/snbtlib/__init__.py
--rw-rw-rw-   0        0        0     6952 2023-04-18 02:12:47.000000 snbtlib-0.0.7/snbtlib/formatter.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:15:02.761783 snbtlib-0.0.7/snbtlib.egg-info/
--rw-rw-rw-   0        0        0      716 2023-04-18 02:15:02.000000 snbtlib-0.0.7/snbtlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-04-18 02:15:02.000000 snbtlib-0.0.7/snbtlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 02:15:02.000000 snbtlib-0.0.7/snbtlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-18 02:15:02.000000 snbtlib-0.0.7/snbtlib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-18 02:15:02.761783 snbtlib-0.0.7/test/
--rw-rw-rw-   0        0        0      190 2023-03-15 08:59:09.000000 snbtlib-0.0.7/test/test.py
+drwxrwxrwx   0        0        0        0 2023-05-24 01:39:48.035952 snbtlib-0.1.0/
+-rw-rw-rw-   0        0        0     1085 2023-02-07 06:40:54.000000 snbtlib-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      716 2023-05-24 01:39:48.035952 snbtlib-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-03-08 06:57:28.000000 snbtlib-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-24 01:39:48.036951 snbtlib-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      558 2023-05-24 01:39:29.000000 snbtlib-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 01:39:48.032951 snbtlib-0.1.0/snbtlib/
+-rw-rw-rw-   0        0        0      302 2023-04-18 02:12:57.000000 snbtlib-0.1.0/snbtlib/__init__.py
+-rw-rw-rw-   0        0        0     7388 2023-05-24 01:38:42.000000 snbtlib-0.1.0/snbtlib/formatter.py
+drwxrwxrwx   0        0        0        0 2023-05-24 01:39:48.034953 snbtlib-0.1.0/snbtlib.egg-info/
+-rw-rw-rw-   0        0        0      716 2023-05-24 01:39:48.000000 snbtlib-0.1.0/snbtlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-05-24 01:39:48.000000 snbtlib-0.1.0/snbtlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 01:39:48.000000 snbtlib-0.1.0/snbtlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-24 01:39:48.000000 snbtlib-0.1.0/snbtlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 01:39:48.035952 snbtlib-0.1.0/test/
+-rw-rw-rw-   0        0        0      197 2023-04-18 02:16:35.000000 snbtlib-0.1.0/test/test.py
```

### Comparing `snbtlib-0.0.7/LICENSE` & `snbtlib-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snbtlib-0.0.7/PKG-INFO` & `snbtlib-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snbtlib
-Version: 0.0.7
+Version: 0.1.0
 Summary: a formatter for snbt from minecraft
 Home-page: 
 Author: Tryanks
 Author-email: tryanks@outlook.com
 License: MIT License
 Keywords: minecraft
 Platform: any
```

### Comparing `snbtlib-0.0.7/setup.py` & `snbtlib-0.1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='snbtlib',
-    version='0.0.7',
+    version='0.1.0',
     keywords='minecraft',
     description='a formatter for snbt from minecraft',
     long_description=long_description,
     license='MIT License',
     url='',
     author='Tryanks',
     author_email='tryanks@outlook.com',
```

### Comparing `snbtlib-0.0.7/snbtlib/formatter.py` & `snbtlib-0.1.0/snbtlib/formatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -169,16 +169,21 @@
         if i == '{':
             token.type = Token.BEGIN_DICT
             token.value = '{'
         elif i == '[':
             token.type = Token.BEGIN_LIST
             token.value = '['
         elif i in '-0123456789':
-            token.type = Token.NUMBER
-            token.value = NumberBuilder(reader)
+            if reader.snext() == ':':
+                reader.last()
+                token = KeyBuilder(token, reader)
+            else:
+                reader.last()
+                token.type = Token.NUMBER
+                token.value = NumberBuilder(reader)
         elif i == ']':
             token.type = Token.END_LIST
             token.value = ']'
         elif i == '}':
             token.type = Token.END_DICT
             token.value = '}'
         elif i in ',\n':
@@ -190,15 +195,15 @@
     return token_list
 
 
 def NumberBuilder(r):
     s = StringIO()
     s.write(r.get_point())
     while i := r.next():
-        if i in '},\n' or i.isspace():
+        if i in '},\n:' or i.isspace():
             r.last()
             break
         s.write(i)
     return '$number$' + s.getvalue()
 
 
 def StringBuilder(r):
@@ -213,16 +218,20 @@
         s.write(i)
     return s.getvalue()
 
 
 def KeyBuilder(token, r):
     s = ''
     stringStatus = False
+    numberStatus = False
     if r.get_point() == '"':
         stringStatus = True
+    elif r.get_point() in '0123456789':
+        r.last()
+        numberStatus = True
     else:
         s += r.get_point()
     token.type = Token.KEY
     while i := r.snext():
         if stringStatus:
             if i == '\\':
                 s += '\\'
@@ -238,14 +247,19 @@
                         s += '\\'
                         s += r.get_point()
                         continue
                     else:
                         r.last()
                         token.type = Token.STRING
                         break
+        if numberStatus:
+            if i in '0123456789':
+                s += i
+            if r.snext() == ':':
+                break
         if i == ':' and not stringStatus:
             break
         s += i
         if s in ('true', 'false'):
             token.type = Token.BOOL
             s = True if s == 'true' else False
             break
```

### Comparing `snbtlib-0.0.7/snbtlib.egg-info/PKG-INFO` & `snbtlib-0.1.0/snbtlib.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snbtlib
-Version: 0.0.7
+Version: 0.1.0
 Summary: a formatter for snbt from minecraft
 Home-page: 
 Author: Tryanks
 Author-email: tryanks@outlook.com
 License: MIT License
 Keywords: minecraft
 Platform: any
```

