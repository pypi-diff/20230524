# Comparing `tmp/divio_docs_gen-0.2.4.tar.gz` & `tmp/divio_docs_gen-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "divio_docs_gen-0.2.4.tar", last modified: Wed May 24 16:49:46 2023, max compression
+gzip compressed data, was "divio_docs_gen-0.2.5.tar", last modified: Wed May 24 16:55:48 2023, max compression
```

## Comparing `divio_docs_gen-0.2.4.tar` & `divio_docs_gen-0.2.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 16:49:46.812734 divio_docs_gen-0.2.4/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6069 2023-05-24 16:49:46.812734 divio_docs_gen-0.2.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5275 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/README.md
--rw-r--r--   0 root         (0) root         (0)     1031 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 16:49:46.812734 divio_docs_gen-0.2.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 16:49:46.808734 divio_docs_gen-0.2.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 16:49:46.808734 divio_docs_gen-0.2.4/src/divio_docs_gen/
--rw-r--r--   0 root         (0) root         (0)     7711 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/src/divio_docs_gen/Args.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 16:49:46.812734 divio_docs_gen-0.2.4/src/divio_docs_gen/Repo/
--rw-r--r--   0 root         (0) root         (0)     3135 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/src/divio_docs_gen/Repo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1754 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/src/divio_docs_gen/Repo/files.py
--rw-r--r--   0 root         (0) root         (0)      876 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/src/divio_docs_gen/Repo/sections.py
--rw-r--r--   0 root         (0) root         (0)     5428 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/src/divio_docs_gen/Section.py
--rw-r--r--   0 root         (0) root         (0)      191 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/src/divio_docs_gen/__init__.py
--rw-r--r--   0 root         (0) root         (0)      113 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/src/divio_docs_gen/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1772 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/src/divio_docs_gen/index.py
--rw-r--r--   0 root         (0) root         (0)     1441 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/src/divio_docs_gen/markdown_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 16:49:46.812734 divio_docs_gen-0.2.4/src/divio_docs_gen/write_to_disk/
--rw-r--r--   0 root         (0) root         (0)     1732 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/src/divio_docs_gen/write_to_disk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3312 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/src/divio_docs_gen/write_to_disk/nav.py
--rw-r--r--   0 root         (0) root         (0)      611 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/src/divio_docs_gen/write_to_disk/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 16:49:46.808734 divio_docs_gen-0.2.4/src/divio_docs_gen.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6069 2023-05-24 16:49:46.000000 divio_docs_gen-0.2.4/src/divio_docs_gen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      703 2023-05-24 16:49:46.000000 divio_docs_gen-0.2.4/src/divio_docs_gen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 16:49:46.000000 divio_docs_gen-0.2.4/src/divio_docs_gen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-24 16:49:46.000000 divio_docs_gen-0.2.4/src/divio_docs_gen.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-05-24 16:49:46.000000 divio_docs_gen-0.2.4/src/divio_docs_gen.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-24 16:49:46.000000 divio_docs_gen-0.2.4/src/divio_docs_gen.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 16:55:48.805453 divio_docs_gen-0.2.5/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-05-24 16:55:39.000000 divio_docs_gen-0.2.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6069 2023-05-24 16:55:48.805453 divio_docs_gen-0.2.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5275 2023-05-24 16:55:39.000000 divio_docs_gen-0.2.5/README.md
+-rw-r--r--   0 root         (0) root         (0)      965 2023-05-24 16:55:39.000000 divio_docs_gen-0.2.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 16:55:48.805453 divio_docs_gen-0.2.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 16:55:48.801453 divio_docs_gen-0.2.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 16:55:48.805453 divio_docs_gen-0.2.5/src/divio_docs_gen/
+-rw-r--r--   0 root         (0) root         (0)     7711 2023-05-24 16:55:39.000000 divio_docs_gen-0.2.5/src/divio_docs_gen/Args.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 16:55:48.805453 divio_docs_gen-0.2.5/src/divio_docs_gen/Repo/
+-rw-r--r--   0 root         (0) root         (0)     3135 2023-05-24 16:55:39.000000 divio_docs_gen-0.2.5/src/divio_docs_gen/Repo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1754 2023-05-24 16:55:39.000000 divio_docs_gen-0.2.5/src/divio_docs_gen/Repo/files.py
+-rw-r--r--   0 root         (0) root         (0)      876 2023-05-24 16:55:39.000000 divio_docs_gen-0.2.5/src/divio_docs_gen/Repo/sections.py
+-rw-r--r--   0 root         (0) root         (0)     5428 2023-05-24 16:55:39.000000 divio_docs_gen-0.2.5/src/divio_docs_gen/Section.py
+-rw-r--r--   0 root         (0) root         (0)      191 2023-05-24 16:55:39.000000 divio_docs_gen-0.2.5/src/divio_docs_gen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      113 2023-05-24 16:55:39.000000 divio_docs_gen-0.2.5/src/divio_docs_gen/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-05-24 16:55:39.000000 divio_docs_gen-0.2.5/src/divio_docs_gen/index.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2023-05-24 16:55:39.000000 divio_docs_gen-0.2.5/src/divio_docs_gen/markdown_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 16:55:48.805453 divio_docs_gen-0.2.5/src/divio_docs_gen/write_to_disk/
+-rw-r--r--   0 root         (0) root         (0)     1732 2023-05-24 16:55:39.000000 divio_docs_gen-0.2.5/src/divio_docs_gen/write_to_disk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3312 2023-05-24 16:55:39.000000 divio_docs_gen-0.2.5/src/divio_docs_gen/write_to_disk/nav.py
+-rw-r--r--   0 root         (0) root         (0)      611 2023-05-24 16:55:39.000000 divio_docs_gen-0.2.5/src/divio_docs_gen/write_to_disk/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 16:55:48.805453 divio_docs_gen-0.2.5/src/divio_docs_gen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6069 2023-05-24 16:55:48.000000 divio_docs_gen-0.2.5/src/divio_docs_gen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      703 2023-05-24 16:55:48.000000 divio_docs_gen-0.2.5/src/divio_docs_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 16:55:48.000000 divio_docs_gen-0.2.5/src/divio_docs_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-24 16:55:48.000000 divio_docs_gen-0.2.5/src/divio_docs_gen.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-05-24 16:55:48.000000 divio_docs_gen-0.2.5/src/divio_docs_gen.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-24 16:55:48.000000 divio_docs_gen-0.2.5/src/divio_docs_gen.egg-info/top_level.txt
```

### Comparing `divio_docs_gen-0.2.4/LICENSE` & `divio_docs_gen-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.4/PKG-INFO` & `divio_docs_gen-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: divio_docs_gen
-Version: 0.2.4
+Version: 0.2.5
 Summary: Turn all the markdown files in your repos into one big, divio structrured documentation
 Author-email: Denperidge <denperidge@gmail.com>
 Project-URL: Homepage, https://github.com/Denperidge-Redpencil/divio-docs-gen
 Project-URL: Bug Tracker, https://github.com/Denperidge-Redpencil/divio-docs-gen/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
```

### Comparing `divio_docs_gen-0.2.4/README.md` & `divio_docs_gen-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.4/src/divio_docs_gen/Args.py` & `divio_docs_gen-0.2.5/src/divio_docs_gen/Args.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.4/src/divio_docs_gen/Repo/__init__.py` & `divio_docs_gen-0.2.5/src/divio_docs_gen/Repo/__init__.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.4/src/divio_docs_gen/Repo/files.py` & `divio_docs_gen-0.2.5/src/divio_docs_gen/Repo/files.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.4/src/divio_docs_gen/Repo/sections.py` & `divio_docs_gen-0.2.5/src/divio_docs_gen/Repo/sections.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.4/src/divio_docs_gen/Section.py` & `divio_docs_gen-0.2.5/src/divio_docs_gen/Section.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.4/src/divio_docs_gen/index.py` & `divio_docs_gen-0.2.5/src/divio_docs_gen/index.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.4/src/divio_docs_gen/markdown_parser.py` & `divio_docs_gen-0.2.5/src/divio_docs_gen/markdown_parser.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.4/src/divio_docs_gen/write_to_disk/__init__.py` & `divio_docs_gen-0.2.5/src/divio_docs_gen/write_to_disk/__init__.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.4/src/divio_docs_gen/write_to_disk/nav.py` & `divio_docs_gen-0.2.5/src/divio_docs_gen/write_to_disk/nav.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.4/src/divio_docs_gen/write_to_disk/utils.py` & `divio_docs_gen-0.2.5/src/divio_docs_gen/write_to_disk/utils.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.4/src/divio_docs_gen.egg-info/PKG-INFO` & `divio_docs_gen-0.2.5/src/divio_docs_gen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: divio-docs-gen
-Version: 0.2.4
+Version: 0.2.5
 Summary: Turn all the markdown files in your repos into one big, divio structrured documentation
 Author-email: Denperidge <denperidge@gmail.com>
 Project-URL: Homepage, https://github.com/Denperidge-Redpencil/divio-docs-gen
 Project-URL: Bug Tracker, https://github.com/Denperidge-Redpencil/divio-docs-gen/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
```

### Comparing `divio_docs_gen-0.2.4/src/divio_docs_gen.egg-info/SOURCES.txt` & `divio_docs_gen-0.2.5/src/divio_docs_gen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

