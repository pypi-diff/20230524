# Comparing `tmp/divio_docs_gen-0.2.1.tar.gz` & `tmp/divio_docs_gen-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "divio_docs_gen-0.2.1.tar", last modified: Tue May  9 07:05:56 2023, max compression
+gzip compressed data, was "divio_docs_gen-0.2.2.tar", last modified: Wed May 24 15:42:13 2023, max compression
```

## Comparing `divio_docs_gen-0.2.1.tar` & `divio_docs_gen-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 07:05:56.266177 divio_docs_gen-0.2.1/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6069 2023-05-09 07:05:56.266177 divio_docs_gen-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5275 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/README.md
--rw-r--r--   0 root         (0) root         (0)      907 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 07:05:56.266177 divio_docs_gen-0.2.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 07:05:56.266177 divio_docs_gen-0.2.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 07:05:56.266177 divio_docs_gen-0.2.1/src/divio_docs_gen/
--rw-r--r--   0 root         (0) root         (0)     7711 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/src/divio_docs_gen/Args.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 07:05:56.266177 divio_docs_gen-0.2.1/src/divio_docs_gen/Repo/
--rw-r--r--   0 root         (0) root         (0)     3135 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/src/divio_docs_gen/Repo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1754 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/src/divio_docs_gen/Repo/files.py
--rw-r--r--   0 root         (0) root         (0)      876 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/src/divio_docs_gen/Repo/sections.py
--rw-r--r--   0 root         (0) root         (0)     5428 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/src/divio_docs_gen/Section.py
--rw-r--r--   0 root         (0) root         (0)      191 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/src/divio_docs_gen/__init__.py
--rw-r--r--   0 root         (0) root         (0)      113 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/src/divio_docs_gen/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1772 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/src/divio_docs_gen/index.py
--rw-r--r--   0 root         (0) root         (0)     1441 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/src/divio_docs_gen/markdown_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 07:05:56.266177 divio_docs_gen-0.2.1/src/divio_docs_gen/write_to_disk/
--rw-r--r--   0 root         (0) root         (0)     1732 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/src/divio_docs_gen/write_to_disk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3312 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/src/divio_docs_gen/write_to_disk/nav.py
--rw-r--r--   0 root         (0) root         (0)      611 2023-05-09 07:05:46.000000 divio_docs_gen-0.2.1/src/divio_docs_gen/write_to_disk/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 07:05:56.266177 divio_docs_gen-0.2.1/src/divio_docs_gen.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6069 2023-05-09 07:05:56.000000 divio_docs_gen-0.2.1/src/divio_docs_gen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      662 2023-05-09 07:05:56.000000 divio_docs_gen-0.2.1/src/divio_docs_gen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 07:05:56.000000 divio_docs_gen-0.2.1/src/divio_docs_gen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-09 07:05:56.000000 divio_docs_gen-0.2.1/src/divio_docs_gen.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-09 07:05:56.000000 divio_docs_gen-0.2.1/src/divio_docs_gen.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:42:13.189439 divio_docs_gen-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-05-24 15:42:02.000000 divio_docs_gen-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6069 2023-05-24 15:42:13.189439 divio_docs_gen-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5275 2023-05-24 15:42:02.000000 divio_docs_gen-0.2.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      907 2023-05-24 15:42:02.000000 divio_docs_gen-0.2.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 15:42:13.189439 divio_docs_gen-0.2.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:42:13.185439 divio_docs_gen-0.2.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:42:13.185439 divio_docs_gen-0.2.2/src/divio_docs_gen/
+-rw-r--r--   0 root         (0) root         (0)     7711 2023-05-24 15:42:02.000000 divio_docs_gen-0.2.2/src/divio_docs_gen/Args.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:42:13.189439 divio_docs_gen-0.2.2/src/divio_docs_gen/Repo/
+-rw-r--r--   0 root         (0) root         (0)     3135 2023-05-24 15:42:02.000000 divio_docs_gen-0.2.2/src/divio_docs_gen/Repo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1754 2023-05-24 15:42:02.000000 divio_docs_gen-0.2.2/src/divio_docs_gen/Repo/files.py
+-rw-r--r--   0 root         (0) root         (0)      876 2023-05-24 15:42:02.000000 divio_docs_gen-0.2.2/src/divio_docs_gen/Repo/sections.py
+-rw-r--r--   0 root         (0) root         (0)     5428 2023-05-24 15:42:02.000000 divio_docs_gen-0.2.2/src/divio_docs_gen/Section.py
+-rw-r--r--   0 root         (0) root         (0)      191 2023-05-24 15:42:02.000000 divio_docs_gen-0.2.2/src/divio_docs_gen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      113 2023-05-24 15:42:02.000000 divio_docs_gen-0.2.2/src/divio_docs_gen/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-05-24 15:42:02.000000 divio_docs_gen-0.2.2/src/divio_docs_gen/index.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2023-05-24 15:42:02.000000 divio_docs_gen-0.2.2/src/divio_docs_gen/markdown_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:42:13.189439 divio_docs_gen-0.2.2/src/divio_docs_gen/write_to_disk/
+-rw-r--r--   0 root         (0) root         (0)     1732 2023-05-24 15:42:02.000000 divio_docs_gen-0.2.2/src/divio_docs_gen/write_to_disk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3312 2023-05-24 15:42:02.000000 divio_docs_gen-0.2.2/src/divio_docs_gen/write_to_disk/nav.py
+-rw-r--r--   0 root         (0) root         (0)      611 2023-05-24 15:42:02.000000 divio_docs_gen-0.2.2/src/divio_docs_gen/write_to_disk/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:42:13.189439 divio_docs_gen-0.2.2/src/divio_docs_gen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6069 2023-05-24 15:42:13.000000 divio_docs_gen-0.2.2/src/divio_docs_gen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      662 2023-05-24 15:42:13.000000 divio_docs_gen-0.2.2/src/divio_docs_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 15:42:13.000000 divio_docs_gen-0.2.2/src/divio_docs_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-24 15:42:13.000000 divio_docs_gen-0.2.2/src/divio_docs_gen.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-24 15:42:13.000000 divio_docs_gen-0.2.2/src/divio_docs_gen.egg-info/top_level.txt
```

### Comparing `divio_docs_gen-0.2.1/LICENSE` & `divio_docs_gen-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.1/PKG-INFO` & `divio_docs_gen-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: divio_docs_gen
-Version: 0.2.1
+Version: 0.2.2
 Summary: Turn all the markdown files in your repos into one big, divio structrured documentation
 Author-email: Denperidge <denperidge@gmail.com>
 Project-URL: Homepage, https://github.com/Denperidge-Redpencil/divio-docs-gen
 Project-URL: Bug Tracker, https://github.com/Denperidge-Redpencil/divio-docs-gen/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Documentation
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Divio Docs Generator
 
 Automatically collect, aggregate and structure all your [divio-style documentation](https://documentation.divio.com/) into a tree of .md files.
 ```
```

### Comparing `divio_docs_gen-0.2.1/README.md` & `divio_docs_gen-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.1/pyproject.toml` & `divio_docs_gen-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "divio_docs_gen"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
     { name="Denperidge", email="denperidge@gmail.com" },
 ]
 description = "Turn all the markdown files in your repos into one big, divio structrured documentation"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.6"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Information Technology",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
```

### Comparing `divio_docs_gen-0.2.1/src/divio_docs_gen/Args.py` & `divio_docs_gen-0.2.2/src/divio_docs_gen/Args.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.1/src/divio_docs_gen/Repo/__init__.py` & `divio_docs_gen-0.2.2/src/divio_docs_gen/Repo/__init__.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.1/src/divio_docs_gen/Repo/files.py` & `divio_docs_gen-0.2.2/src/divio_docs_gen/Repo/files.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.1/src/divio_docs_gen/Repo/sections.py` & `divio_docs_gen-0.2.2/src/divio_docs_gen/Repo/sections.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.1/src/divio_docs_gen/Section.py` & `divio_docs_gen-0.2.2/src/divio_docs_gen/Section.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.1/src/divio_docs_gen/index.py` & `divio_docs_gen-0.2.2/src/divio_docs_gen/index.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.1/src/divio_docs_gen/markdown_parser.py` & `divio_docs_gen-0.2.2/src/divio_docs_gen/markdown_parser.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.1/src/divio_docs_gen/write_to_disk/__init__.py` & `divio_docs_gen-0.2.2/src/divio_docs_gen/write_to_disk/__init__.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.1/src/divio_docs_gen/write_to_disk/nav.py` & `divio_docs_gen-0.2.2/src/divio_docs_gen/write_to_disk/nav.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.1/src/divio_docs_gen/write_to_disk/utils.py` & `divio_docs_gen-0.2.2/src/divio_docs_gen/write_to_disk/utils.py`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.2.1/src/divio_docs_gen.egg-info/PKG-INFO` & `divio_docs_gen-0.2.2/src/divio_docs_gen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: divio-docs-gen
-Version: 0.2.1
+Version: 0.2.2
 Summary: Turn all the markdown files in your repos into one big, divio structrured documentation
 Author-email: Denperidge <denperidge@gmail.com>
 Project-URL: Homepage, https://github.com/Denperidge-Redpencil/divio-docs-gen
 Project-URL: Bug Tracker, https://github.com/Denperidge-Redpencil/divio-docs-gen/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Documentation
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Divio Docs Generator
 
 Automatically collect, aggregate and structure all your [divio-style documentation](https://documentation.divio.com/) into a tree of .md files.
 ```
```

### Comparing `divio_docs_gen-0.2.1/src/divio_docs_gen.egg-info/SOURCES.txt` & `divio_docs_gen-0.2.2/src/divio_docs_gen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

