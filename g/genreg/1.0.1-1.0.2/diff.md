# Comparing `tmp/genreg-1.0.1.tar.gz` & `tmp/genreg-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/andras.aszodi/VBCF/biocomp/PROJECTS/training/pytraining/lang/scripts/dev/full/dist/tmpeo9njyqa/genreg-1.0.1.tar", last modified: Wed Jul 14 14:18:09 2021, max compression
+gzip compressed data, was "genreg-1.0.2.tar", last modified: Thu Aug 18 13:12:40 2022, max compression
```

## Comparing `genreg-1.0.1.tar` & `genreg-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 andras.aszodi (50818)     2048        0 2021-07-14 14:18:09.000000 genreg-1.0.1/
--rw-r--r--   0 andras.aszodi (50818)     2048     1236 2021-07-13 10:47:16.000000 genreg-1.0.1/LICENSE
--rw-r--r--   0 andras.aszodi (50818)     2048      800 2021-07-14 14:18:09.000000 genreg-1.0.1/PKG-INFO
--rw-r--r--   0 andras.aszodi (50818)     2048      305 2021-07-13 10:46:01.000000 genreg-1.0.1/README.md
-drwxr-xr-x   0 andras.aszodi (50818)     2048        0 2021-07-14 14:18:09.000000 genreg-1.0.1/genreg/
--rw-r--r--   0 andras.aszodi (50818)     2048        0 2021-07-09 13:41:11.000000 genreg-1.0.1/genreg/__init__.py
--rw-r--r--   0 andras.aszodi (50818)     2048     7946 2021-07-13 10:23:44.000000 genreg-1.0.1/genreg/region.py
-drwxr-xr-x   0 andras.aszodi (50818)     2048        0 2021-07-14 14:18:09.000000 genreg-1.0.1/genreg/tests/
--rw-r--r--   0 andras.aszodi (50818)     2048        0 2021-07-09 13:41:11.000000 genreg-1.0.1/genreg/tests/__init__.py
--rw-r--r--   0 andras.aszodi (50818)     2048     5555 2021-07-13 10:24:36.000000 genreg-1.0.1/genreg/tests/testregion.py
-drwxr-xr-x   0 andras.aszodi (50818)     2048        0 2021-07-14 14:18:09.000000 genreg-1.0.1/genreg.egg-info/
--rw-r--r--   0 andras.aszodi (50818)     2048      800 2021-07-14 14:18:09.000000 genreg-1.0.1/genreg.egg-info/PKG-INFO
--rw-r--r--   0 andras.aszodi (50818)     2048      250 2021-07-14 14:18:09.000000 genreg-1.0.1/genreg.egg-info/SOURCES.txt
--rw-r--r--   0 andras.aszodi (50818)     2048        1 2021-07-14 14:18:09.000000 genreg-1.0.1/genreg.egg-info/dependency_links.txt
--rw-r--r--   0 andras.aszodi (50818)     2048        7 2021-07-14 14:18:09.000000 genreg-1.0.1/genreg.egg-info/top_level.txt
--rw-r--r--   0 andras.aszodi (50818)     2048      103 2021-07-13 10:49:12.000000 genreg-1.0.1/pyproject.toml
--rw-r--r--   0 andras.aszodi (50818)     2048      554 2021-07-14 14:18:09.000000 genreg-1.0.1/setup.cfg
+drwxr-xr-x   0 andras.aszodi   (504) staff       (20)        0 2022-08-18 13:12:40.819854 genreg-1.0.2/
+-rw-r--r--   0 andras.aszodi   (504) staff       (20)     1236 2022-02-08 16:00:16.000000 genreg-1.0.2/LICENSE
+-rw-r--r--   0 andras.aszodi   (504) staff       (20)     2192 2022-08-18 13:12:40.819371 genreg-1.0.2/PKG-INFO
+-rw-r--r--   0 andras.aszodi   (504) staff       (20)      305 2022-02-08 16:00:16.000000 genreg-1.0.2/README.md
+drwxr-xr-x   0 andras.aszodi   (504) staff       (20)        0 2022-08-18 13:12:40.816195 genreg-1.0.2/genreg/
+-rw-r--r--   0 andras.aszodi   (504) staff       (20)        0 2022-02-08 16:00:16.000000 genreg-1.0.2/genreg/__init__.py
+-rw-r--r--   0 andras.aszodi   (504) staff       (20)     7947 2022-08-18 12:23:20.000000 genreg-1.0.2/genreg/region.py
+drwxr-xr-x   0 andras.aszodi   (504) staff       (20)        0 2022-08-18 13:12:40.818628 genreg-1.0.2/genreg/tests/
+-rw-r--r--   0 andras.aszodi   (504) staff       (20)        0 2022-02-08 16:00:16.000000 genreg-1.0.2/genreg/tests/__init__.py
+-rw-r--r--   0 andras.aszodi   (504) staff       (20)     5555 2022-02-08 16:00:16.000000 genreg-1.0.2/genreg/tests/testregion.py
+drwxr-xr-x   0 andras.aszodi   (504) staff       (20)        0 2022-08-18 13:12:40.817940 genreg-1.0.2/genreg.egg-info/
+-rw-r--r--   0 andras.aszodi   (504) staff       (20)     2192 2022-08-18 13:12:40.000000 genreg-1.0.2/genreg.egg-info/PKG-INFO
+-rw-r--r--   0 andras.aszodi   (504) staff       (20)      240 2022-08-18 13:12:40.000000 genreg-1.0.2/genreg.egg-info/SOURCES.txt
+-rw-r--r--   0 andras.aszodi   (504) staff       (20)        1 2022-08-18 13:12:40.000000 genreg-1.0.2/genreg.egg-info/dependency_links.txt
+-rw-r--r--   0 andras.aszodi   (504) staff       (20)        7 2022-08-18 13:12:40.000000 genreg-1.0.2/genreg.egg-info/top_level.txt
+-rw-r--r--   0 andras.aszodi   (504) staff       (20)      594 2022-08-18 13:11:52.000000 genreg-1.0.2/pyproject.toml
+-rw-r--r--   0 andras.aszodi   (504) staff       (20)       38 2022-08-18 13:12:40.819978 genreg-1.0.2/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `genreg-1.0.1/LICENSE` & `genreg-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `genreg-1.0.1/genreg/region.py` & `genreg-1.0.2/genreg/region.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,10 +205,10 @@
     # 3A-2. Detects "empty" lines to be ignored by the input methods.
     def _ignore_line(self, line):
         """
         :param line: A string containing a line, possibly read from a BED or GFF file.
         :return: True if `line` is empty or all-whitespace or a comment.
         """
         return len(line) == 0 or \
-            re.match(r"[ \t]*$", line) or \
+            re.match(r"^[ \t]*$", line) or \
             line[0] == '#'
```

### Comparing `genreg-1.0.1/genreg/tests/testregion.py` & `genreg-1.0.2/genreg/tests/testregion.py`

 * *Files identical despite different names*

