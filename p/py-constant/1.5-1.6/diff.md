# Comparing `tmp/py_constant-1.5.tar.gz` & `tmp/py_constant-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py_constant-1.5.tar", last modified: Wed Feb 27 11:34:08 2019, max compression
+gzip compressed data, was "py_constant-1.6.tar", last modified: Wed May 24 14:52:12 2023, max compression
```

## Comparing `py_constant-1.5.tar` & `py_constant-1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxr-xr-x   0 mihagrgicjelen   (502) staff       (20)        0 2019-02-27 11:34:08.000000 py_constant-1.5/
--rw-r--r--   0 mihagrgicjelen   (502) staff       (20)      382 2019-02-27 11:34:08.000000 py_constant-1.5/PKG-INFO
--rw-r--r--   0 mihagrgicjelen   (502) staff       (20)       65 2019-02-05 11:05:52.000000 py_constant-1.5/README.txt
-drwxr-xr-x   0 mihagrgicjelen   (502) staff       (20)        0 2019-02-27 11:34:08.000000 py_constant-1.5/py_constant/
--rw-r--r--   0 mihagrgicjelen   (502) staff       (20)       27 2019-02-27 11:32:40.000000 py_constant-1.5/py_constant/__init__.py
--rw-r--r--   0 mihagrgicjelen   (502) staff       (20)     3486 2019-02-06 09:58:58.000000 py_constant-1.5/py_constant/py_constant.py
--rw-r--r--   0 mihagrgicjelen   (502) staff       (20)      381 2019-02-27 11:34:07.000000 py_constant-1.5/setup.py
+drwxr-xr-x   0 mihagrgicjelen   (501) staff       (20)        0 2023-05-24 14:52:12.795871 py_constant-1.6/
+-rw-r--r--   0 mihagrgicjelen   (501) staff       (20)      382 2023-05-24 14:52:12.795918 py_constant-1.6/PKG-INFO
+-rw-r--r--   0 mihagrgicjelen   (501) staff       (20)       65 2023-05-24 14:46:57.035310 py_constant-1.6/README.txt
+drwxr-xr-x   0 mihagrgicjelen   (501) staff       (20)        0 2023-05-24 14:52:12.795843 py_constant-1.6/py_constant/
+-rw-r--r--   0 mihagrgicjelen   (501) staff       (20)       27 2023-05-24 14:46:57.036132 py_constant-1.6/py_constant/__init__.py
+-rw-r--r--   0 mihagrgicjelen   (501) staff       (20)     3791 2023-05-24 14:51:46.398558 py_constant-1.6/py_constant/py_constant.py
+-rw-r--r--   0 mihagrgicjelen   (501) staff       (20)      381 2023-05-24 14:51:00.120600 py_constant-1.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `py_constant-1.5/py_constant/py_constant.py` & `py_constant-1.6/py_constant/py_constant.py`

 * *Files 16% similar despite different names*

```diff
@@ -113,7 +113,17 @@
             return opts
 
         except AttributeError as e:
 
             raise Exception(
                 'Probably no get_all() or get_title() '
                 'implemented for %s (%s)' % (cls, e))
+
+    @classmethod
+    def to_django_choices(cls):
+        try:
+            return [(x, cls.get_title(x)) for x in cls.get_all()]
+
+        except AttributeError as e:
+            raise Exception(
+                'Probably no get_all() or get_title() '
+                'implemented for %s (%s)' % (cls, e))
```

