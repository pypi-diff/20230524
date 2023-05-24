# Comparing `tmp/divio_docs_gen-0.2.3.tar.gz` & `tmp/divio_docs_gen-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "divio_docs_gen-0.2.3.tar", last modified: Wed May 24 16:46:52 2023, max compression
+gzip compressed data, was "divio_docs_gen-0.2.4.tar", last modified: Wed May 24 16:49:46 2023, max compression
```

## Comparing `divio_docs_gen-0.2.3.tar` & `divio_docs_gen-0.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 16:46:52.386319 divio_docs_gen-0.2.3/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-05-24 16:46:42.000000 divio_docs_gen-0.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6069 2023-05-24 16:46:52.386319 divio_docs_gen-0.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5275 2023-05-24 16:46:42.000000 divio_docs_gen-0.2.3/README.md
--rw-r--r--   0 root         (0) root         (0)     1031 2023-05-24 16:46:42.000000 divio_docs_gen-0.2.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 16:46:52.386319 divio_docs_gen-0.2.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 16:46:52.382319 divio_docs_gen-0.2.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 16:46:52.386319 divio_docs_gen-0.2.3/src/divio_docs_gen/
--rw-r--r--   0 root         (0) root         (0)     7711 2023-05-24 16:46:42.000000 divio_docs_gen-0.2.3/src/divio_docs_gen/Args.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 16:46:52.386319 divio_docs_gen-0.2.3/src/divio_docs_gen/Repo/
--rw-r--r--   0 root         (0) root         (0)     3135 2023-05-24 16:46:42.000000 divio_docs_gen-0.2.3/src/divio_docs_gen/Repo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1754 2023-05-24 16:46:42.000000 divio_docs_gen-0.2.3/src/divio_docs_gen/Repo/files.py
--rw-r--r--   0 root         (0) root         (0)      876 2023-05-24 16:46:42.000000 divio_docs_gen-0.2.3/src/divio_docs_gen/Repo/sections.py
--rw-r--r--   0 root         (0) root         (0)     5428 2023-05-24 16:46:42.000000 divio_docs_gen-0.2.3/src/divio_docs_gen/Section.py
--rw-r--r--   0 root         (0) root         (0)      191 2023-05-24 16:46:42.000000 divio_docs_gen-0.2.3/src/divio_docs_gen/__init__.py
--rw-r--r--   0 root         (0) root         (0)      113 2023-05-24 16:46:42.000000 divio_docs_gen-0.2.3/src/divio_docs_gen/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1772 2023-05-24 16:46:42.000000 divio_docs_gen-0.2.3/src/divio_docs_gen/index.py
--rw-r--r--   0 root         (0) root         (0)     1441 2023-05-24 16:46:42.000000 divio_docs_gen-0.2.3/src/divio_docs_gen/markdown_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 16:46:52.386319 divio_docs_gen-0.2.3/src/divio_docs_gen/write_to_disk/
--rw-r--r--   0 root         (0) root         (0)     1732 2023-05-24 16:46:42.000000 divio_docs_gen-0.2.3/src/divio_docs_gen/write_to_disk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3312 2023-05-24 16:46:42.000000 divio_docs_gen-0.2.3/src/divio_docs_gen/write_to_disk/nav.py
--rw-r--r--   0 root         (0) root         (0)      611 2023-05-24 16:46:42.000000 divio_docs_gen-0.2.3/src/divio_docs_gen/write_to_disk/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 16:46:52.386319 divio_docs_gen-0.2.3/src/divio_docs_gen.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6069 2023-05-24 16:46:52.000000 divio_docs_gen-0.2.3/src/divio_docs_gen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      703 2023-05-24 16:46:52.000000 divio_docs_gen-0.2.3/src/divio_docs_gen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 16:46:52.000000 divio_docs_gen-0.2.3/src/divio_docs_gen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-24 16:46:52.000000 divio_docs_gen-0.2.3/src/divio_docs_gen.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-05-24 16:46:52.000000 divio_docs_gen-0.2.3/src/divio_docs_gen.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-24 16:46:52.000000 divio_docs_gen-0.2.3/src/divio_docs_gen.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 16:49:46.812734 divio_docs_gen-0.2.4/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6069 2023-05-24 16:49:46.812734 divio_docs_gen-0.2.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5275 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/README.md
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 16:49:46.812734 divio_docs_gen-0.2.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 16:49:46.808734 divio_docs_gen-0.2.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 16:49:46.808734 divio_docs_gen-0.2.4/src/divio_docs_gen/
+-rw-r--r--   0 root         (0) root         (0)     7711 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/src/divio_docs_gen/Args.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 16:49:46.812734 divio_docs_gen-0.2.4/src/divio_docs_gen/Repo/
+-rw-r--r--   0 root         (0) root         (0)     3135 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/src/divio_docs_gen/Repo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1754 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/src/divio_docs_gen/Repo/files.py
+-rw-r--r--   0 root         (0) root         (0)      876 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/src/divio_docs_gen/Repo/sections.py
+-rw-r--r--   0 root         (0) root         (0)     5428 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/src/divio_docs_gen/Section.py
+-rw-r--r--   0 root         (0) root         (0)      191 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/src/divio_docs_gen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      113 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/src/divio_docs_gen/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/src/divio_docs_gen/index.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/src/divio_docs_gen/markdown_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 16:49:46.812734 divio_docs_gen-0.2.4/src/divio_docs_gen/write_to_disk/
+-rw-r--r--   0 root         (0) root         (0)     1732 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/src/divio_docs_gen/write_to_disk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3312 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/src/divio_docs_gen/write_to_disk/nav.py
+-rw-r--r--   0 root         (0) root         (0)      611 2023-05-24 16:49:37.000000 divio_docs_gen-0.2.4/src/divio_docs_gen/write_to_disk/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 16:49:46.808734 divio_docs_gen-0.2.4/src/divio_docs_gen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6069 2023-05-24 16:49:46.000000 divio_docs_gen-0.2.4/src/divio_docs_gen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      703 2023-05-24 16:49:46.000000 divio_docs_gen-0.2.4/src/divio_docs_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 16:49:46.000000 divio_docs_gen-0.2.4/src/divio_docs_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-24 16:49:46.000000 divio_docs_gen-0.2.4/src/divio_docs_gen.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2023-05-24 16:49:46.000000 divio_docs_gen-0.2.4/src/divio_docs_gen.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-24 16:49:46.000000 divio_docs_gen-0.2.4/src/divio_docs_gen.egg-info/top_level.txt
```

### Comparing `divio_docs_gen-0.2.3/LICENSE` & `divio_docs_gen-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.3/PKG-INFO` & `divio_docs_gen-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: divio_docs_gen
-Version: 0.2.3
+Version: 0.2.4
 Summary: Turn all the markdown files in your repos into one big, divio structrured documentation
 Author-email: Denperidge <denperidge@gmail.com>
 Project-URL: Homepage, https://github.com/Denperidge-Redpencil/divio-docs-gen
 Project-URL: Bug Tracker, https://github.com/Denperidge-Redpencil/divio-docs-gen/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
```

### Comparing `divio_docs_gen-0.2.3/README.md` & `divio_docs_gen-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.3/pyproject.toml` & `divio_docs_gen-0.2.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "divio_docs_gen"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
     { name="Denperidge", email="denperidge@gmail.com" },
 ]
 description = "Turn all the markdown files in your repos into one big, divio structrured documentation"
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies = [
     "GitPython",
-    "python-slugify; python_version<'3.6'",
-    "unicode-slugify; python_version>'3.7'"
+    "python-slugify; python_version>'3.6'",
+    "unicode-slugify; python_version<'3.7'"
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Information Technology",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `divio_docs_gen-0.2.3/src/divio_docs_gen/Args.py` & `divio_docs_gen-0.2.4/src/divio_docs_gen/Args.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.3/src/divio_docs_gen/Repo/__init__.py` & `divio_docs_gen-0.2.4/src/divio_docs_gen/Repo/__init__.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.3/src/divio_docs_gen/Repo/files.py` & `divio_docs_gen-0.2.4/src/divio_docs_gen/Repo/files.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.3/src/divio_docs_gen/Repo/sections.py` & `divio_docs_gen-0.2.4/src/divio_docs_gen/Repo/sections.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.3/src/divio_docs_gen/Section.py` & `divio_docs_gen-0.2.4/src/divio_docs_gen/Section.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.3/src/divio_docs_gen/index.py` & `divio_docs_gen-0.2.4/src/divio_docs_gen/index.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.3/src/divio_docs_gen/markdown_parser.py` & `divio_docs_gen-0.2.4/src/divio_docs_gen/markdown_parser.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.3/src/divio_docs_gen/write_to_disk/__init__.py` & `divio_docs_gen-0.2.4/src/divio_docs_gen/write_to_disk/__init__.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.3/src/divio_docs_gen/write_to_disk/nav.py` & `divio_docs_gen-0.2.4/src/divio_docs_gen/write_to_disk/nav.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.3/src/divio_docs_gen/write_to_disk/utils.py` & `divio_docs_gen-0.2.4/src/divio_docs_gen/write_to_disk/utils.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.3/src/divio_docs_gen.egg-info/PKG-INFO` & `divio_docs_gen-0.2.4/src/divio_docs_gen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: divio-docs-gen
-Version: 0.2.3
+Version: 0.2.4
 Summary: Turn all the markdown files in your repos into one big, divio structrured documentation
 Author-email: Denperidge <denperidge@gmail.com>
 Project-URL: Homepage, https://github.com/Denperidge-Redpencil/divio-docs-gen
 Project-URL: Bug Tracker, https://github.com/Denperidge-Redpencil/divio-docs-gen/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
```

### Comparing `divio_docs_gen-0.2.3/src/divio_docs_gen.egg-info/SOURCES.txt` & `divio_docs_gen-0.2.4/src/divio_docs_gen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

