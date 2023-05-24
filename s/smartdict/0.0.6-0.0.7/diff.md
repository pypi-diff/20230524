# Comparing `tmp/smartdict-0.0.6.tar.gz` & `tmp/smartdict-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartdict-0.0.6.tar", last modified: Sun May 21 15:01:21 2023, max compression
+gzip compressed data, was "smartdict-0.0.7.tar", last modified: Wed May 24 05:15:30 2023, max compression
```

## Comparing `smartdict-0.0.6.tar` & `smartdict-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-05-21 15:01:21.966395 smartdict-0.0.6/
--rw-r--r--   0 jyonnliu   (501) staff       (20)     2556 2023-05-21 15:01:21.966298 smartdict-0.0.6/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)     2284 2022-11-02 06:20:42.000000 smartdict-0.0.6/README.md
--rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2023-05-21 15:01:21.966423 smartdict-0.0.6/setup.cfg
--rw-r--r--   0 jyonnliu   (501) staff       (20)      591 2023-05-21 15:01:08.000000 smartdict-0.0.6/setup.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-05-21 15:01:21.965734 smartdict-0.0.6/smartdict/
--rw-r--r--   0 jyonnliu   (501) staff       (20)       89 2022-10-20 00:56:59.000000 smartdict-0.0.6/smartdict/__init__.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     4606 2023-05-21 15:01:03.000000 smartdict-0.0.6/smartdict/dict_compiler.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-05-21 15:01:21.966148 smartdict-0.0.6/smartdict.egg-info/
--rw-r--r--   0 jyonnliu   (501) staff       (20)     2556 2023-05-21 15:01:21.000000 smartdict-0.0.6/smartdict.egg-info/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)      199 2023-05-21 15:01:21.000000 smartdict-0.0.6/smartdict.egg-info/SOURCES.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2023-05-21 15:01:21.000000 smartdict-0.0.6/smartdict.egg-info/dependency_links.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)       10 2023-05-21 15:01:21.000000 smartdict-0.0.6/smartdict.egg-info/top_level.txt
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-05-24 05:15:30.509644 smartdict-0.0.7/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     2556 2023-05-24 05:15:30.509541 smartdict-0.0.7/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     2284 2022-11-02 06:20:42.000000 smartdict-0.0.7/README.md
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2023-05-24 05:15:30.509673 smartdict-0.0.7/setup.cfg
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      591 2023-05-24 05:15:17.000000 smartdict-0.0.7/setup.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-05-24 05:15:30.508979 smartdict-0.0.7/smartdict/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       89 2022-10-20 00:56:59.000000 smartdict-0.0.7/smartdict/__init__.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     4776 2023-05-24 05:14:51.000000 smartdict-0.0.7/smartdict/dict_compiler.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-05-24 05:15:30.509393 smartdict-0.0.7/smartdict.egg-info/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     2556 2023-05-24 05:15:30.000000 smartdict-0.0.7/smartdict.egg-info/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      199 2023-05-24 05:15:30.000000 smartdict-0.0.7/smartdict.egg-info/SOURCES.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2023-05-24 05:15:30.000000 smartdict-0.0.7/smartdict.egg-info/dependency_links.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       10 2023-05-24 05:15:30.000000 smartdict-0.0.7/smartdict.egg-info/top_level.txt
```

### Comparing `smartdict-0.0.6/PKG-INFO` & `smartdict-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartdict
-Version: 0.0.6
+Version: 0.0.7
 Summary: a string-based refdict
 Home-page: https://github.com/Jyonn/SmartDict
 Author: Jyonn Liu
 Author-email: i@6-79.cn
 License: MIT Licence
 Keywords: dict,refer
 Platform: any
```

### Comparing `smartdict-0.0.6/README.md` & `smartdict-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `smartdict-0.0.6/setup.py` & `smartdict-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='smartdict',
-    version='0.0.6',
+    version='0.0.7',
     keywords=['dict', 'refer'],
     description='a string-based refdict',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT Licence',
     url='https://github.com/Jyonn/SmartDict',
     author='Jyonn Liu',
```

### Comparing `smartdict-0.0.6/smartdict/dict_compiler.py` & `smartdict-0.0.7/smartdict/dict_compiler.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 
     def __setitem__(self, key, value):
         self.d[key] = value
 
     def __contains__(self, item):
         return item in self.d
 
+    def keys(self):
+        return self.d.keys()
+
 
 class DictCompiler:
     p = re.compile('\\${(.*?)}')
     pf = re.compile('\\${(.*?)}\\$')
 
     class InCircle:
         pass
@@ -87,28 +90,35 @@
 
     def _process_full_ref(self, path: str, s: str):
         match = self.pf.fullmatch(s)
         if not match:
             return self.NotFound
 
         full_ref = match.group(1)
+
+        if path in self.circle:
+            v = self.circle[path]
+            if isinstance(v, self.InCircle):
+                raise ValueError(f'Dict references are in circle, circle = {self.circle.keys()}')
+            return v
+
         self.circle[path] = self.InCircle()
         value = self._get_value(full_ref)
-        value = self._process(path.split('.'), value)
+        value = self._process([], value)
         self.circle[path] = value
         return value
 
     def _process_item(self, path: str, s: str):
         if not isinstance(s, str):
             return s
 
         if path in self.circle:
             v = self.circle[path]
             if isinstance(v, self.InCircle):
-                raise ValueError(f'Dict references are in circle, path = {path}')
+                raise ValueError(f'Dict references are in circle, circle = {self.circle.keys()}')
             return v
 
         full_value = self._process_full_ref(path, s)
         if full_value is not self.NotFound:
             return full_value
 
         refs = self._get_refs(s)
@@ -146,19 +156,14 @@
 def parse(d: dict):
     compiler = DictCompiler(d)
     return compiler.parse()
 
 
 if __name__ == '__main__':
     d = dict(
-        a='${b.v.1}+1',
-        b='${c}$',
-        c=dict(
-            __l=23,
-            v=('sorry', 'good', 'ok'),
-            m='${c.__l}'
-        )
+        a='${b}$',
+        b='${a}$',
     )
     # d = [1,2,'${0}$']
 
     rd = DictCompiler(d)
     print(rd.parse())
```

### Comparing `smartdict-0.0.6/smartdict.egg-info/PKG-INFO` & `smartdict-0.0.7/smartdict.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartdict
-Version: 0.0.6
+Version: 0.0.7
 Summary: a string-based refdict
 Home-page: https://github.com/Jyonn/SmartDict
 Author: Jyonn Liu
 Author-email: i@6-79.cn
 License: MIT Licence
 Keywords: dict,refer
 Platform: any
```

