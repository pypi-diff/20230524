# Comparing `tmp/mkdocs-exclude-unused-files-1.1.0.tar.gz` & `tmp/mkdocs_exclude_unused_files-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-exclude-unused-files-1.1.0.tar", last modified: Wed Mar 29 13:51:18 2023, max compression
+gzip compressed data, was "mkdocs_exclude_unused_files-1.2.0.tar", max compression
```

## Comparing `mkdocs-exclude-unused-files-1.1.0.tar` & `mkdocs_exclude_unused_files-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,6 @@
-drwxr-xr-x   0 kadse      (501) staff       (20)        0 2023-03-29 13:51:18.595379 mkdocs-exclude-unused-files-1.1.0/
--rw-r--r--   0 kadse      (501) staff       (20)     1082 2023-02-26 19:18:51.000000 mkdocs-exclude-unused-files-1.1.0/LICENSE.md
--rw-r--r--   0 kadse      (501) staff       (20)     5175 2023-03-29 13:51:18.595245 mkdocs-exclude-unused-files-1.1.0/PKG-INFO
--rw-r--r--   0 kadse      (501) staff       (20)     4710 2023-03-29 13:44:46.000000 mkdocs-exclude-unused-files-1.1.0/README.md
-drwxr-xr-x   0 kadse      (501) staff       (20)        0 2023-03-29 13:51:18.594240 mkdocs-exclude-unused-files-1.1.0/mkdocs_exclude_unused_files/
--rw-r--r--   0 kadse      (501) staff       (20)        0 2023-02-26 16:32:41.000000 mkdocs-exclude-unused-files-1.1.0/mkdocs_exclude_unused_files/__init__.py
--rw-r--r--   0 kadse      (501) staff       (20)     4159 2023-03-29 13:44:46.000000 mkdocs-exclude-unused-files-1.1.0/mkdocs_exclude_unused_files/plugin.py
-drwxr-xr-x   0 kadse      (501) staff       (20)        0 2023-03-29 13:51:18.595068 mkdocs-exclude-unused-files-1.1.0/mkdocs_exclude_unused_files.egg-info/
--rw-r--r--   0 kadse      (501) staff       (20)     5175 2023-03-29 13:51:18.000000 mkdocs-exclude-unused-files-1.1.0/mkdocs_exclude_unused_files.egg-info/PKG-INFO
--rw-r--r--   0 kadse      (501) staff       (20)      415 2023-03-29 13:51:18.000000 mkdocs-exclude-unused-files-1.1.0/mkdocs_exclude_unused_files.egg-info/SOURCES.txt
--rw-r--r--   0 kadse      (501) staff       (20)        1 2023-03-29 13:51:18.000000 mkdocs-exclude-unused-files-1.1.0/mkdocs_exclude_unused_files.egg-info/dependency_links.txt
--rw-r--r--   0 kadse      (501) staff       (20)      107 2023-03-29 13:51:18.000000 mkdocs-exclude-unused-files-1.1.0/mkdocs_exclude_unused_files.egg-info/entry_points.txt
--rw-r--r--   0 kadse      (501) staff       (20)       22 2023-03-29 13:51:18.000000 mkdocs-exclude-unused-files-1.1.0/mkdocs_exclude_unused_files.egg-info/requires.txt
--rw-r--r--   0 kadse      (501) staff       (20)       28 2023-03-29 13:51:18.000000 mkdocs-exclude-unused-files-1.1.0/mkdocs_exclude_unused_files.egg-info/top_level.txt
--rw-r--r--   0 kadse      (501) staff       (20)       38 2023-03-29 13:51:18.595417 mkdocs-exclude-unused-files-1.1.0/setup.cfg
--rw-r--r--   0 kadse      (501) staff       (20)      915 2023-03-29 13:46:56.000000 mkdocs-exclude-unused-files-1.1.0/setup.py
+-rw-r--r--   0        0        0     1099 2023-05-21 20:35:27.085092 mkdocs_exclude_unused_files-1.2.0/LICENSE.md
+-rw-r--r--   0        0        0     4013 2023-05-21 20:35:27.085372 mkdocs_exclude_unused_files-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-02-26 16:32:41.145666 mkdocs_exclude_unused_files-1.2.0/mkdocs_exclude_unused_files/__init__.py
+-rw-r--r--   0        0        0     7209 2023-05-21 20:35:27.085685 mkdocs_exclude_unused_files-1.2.0/mkdocs_exclude_unused_files/plugin.py
+-rw-r--r--   0        0        0     2647 2023-05-24 16:08:35.623263 mkdocs_exclude_unused_files-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5206 1970-01-01 00:00:00.000000 mkdocs_exclude_unused_files-1.2.0/PKG-INFO
```

### Comparing `mkdocs-exclude-unused-files-1.1.0/LICENSE.md` & `mkdocs_exclude_unused_files-1.2.0/LICENSE.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
-Copyright 2023-* Jonas Lorenz <jonas@jonasdoesthings.com>
+# MIT License
+
+Copyright (c) 2023 Jonas Lorenz <jonas@jonasdoesthings.com>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

