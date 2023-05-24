# Comparing `tmp/django-mermaid-0.0.4.tar.gz` & `tmp/django-mermaid-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mermaid-0.0.4.tar", last modified: Tue Mar 14 16:07:57 2023, max compression
+gzip compressed data, was "django-mermaid-0.0.5.tar", last modified: Mon May  1 12:52:25 2023, max compression
```

## Comparing `django-mermaid-0.0.4.tar` & `django-mermaid-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:07:57.343546 django-mermaid-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-14 16:07:47.000000 django-mermaid-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-03-14 16:07:57.343546 django-mermaid-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-03-14 16:07:47.000000 django-mermaid-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-14 16:07:47.000000 django-mermaid-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-03-14 16:07:57.343546 django-mermaid-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-14 16:07:47.000000 django-mermaid-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:07:57.339546 django-mermaid-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:07:57.339546 django-mermaid-0.0.4/src/django_mermaid/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-14 16:07:47.000000 django-mermaid-0.0.4/src/django_mermaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-14 16:07:47.000000 django-mermaid-0.0.4/src/django_mermaid/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:07:57.343546 django-mermaid-0.0.4/src/django_mermaid/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-14 16:07:47.000000 django-mermaid-0.0.4/src/django_mermaid/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-14 16:07:47.000000 django-mermaid-0.0.4/src/django_mermaid/templatetags/mermaid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:07:57.343546 django-mermaid-0.0.4/src/django_mermaid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-03-14 16:07:57.000000 django-mermaid-0.0.4/src/django_mermaid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-14 16:07:57.000000 django-mermaid-0.0.4/src/django_mermaid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 16:07:57.000000 django-mermaid-0.0.4/src/django_mermaid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 16:07:57.000000 django-mermaid-0.0.4/src/django_mermaid.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-14 16:07:57.000000 django-mermaid-0.0.4/src/django_mermaid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-14 16:07:57.000000 django-mermaid-0.0.4/src/django_mermaid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:52:25.492858 django-mermaid-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-01 12:52:12.000000 django-mermaid-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-01 12:52:25.492858 django-mermaid-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-01 12:52:12.000000 django-mermaid-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-01 12:52:12.000000 django-mermaid-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-01 12:52:25.492858 django-mermaid-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-01 12:52:12.000000 django-mermaid-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:52:25.488858 django-mermaid-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:52:25.488858 django-mermaid-0.0.5/src/django_mermaid/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 12:52:12.000000 django-mermaid-0.0.5/src/django_mermaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-01 12:52:12.000000 django-mermaid-0.0.5/src/django_mermaid/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:52:25.492858 django-mermaid-0.0.5/src/django_mermaid/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-01 12:52:12.000000 django-mermaid-0.0.5/src/django_mermaid/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-01 12:52:12.000000 django-mermaid-0.0.5/src/django_mermaid/templatetags/mermaid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:52:25.492858 django-mermaid-0.0.5/src/django_mermaid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-01 12:52:25.000000 django-mermaid-0.0.5/src/django_mermaid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-01 12:52:25.000000 django-mermaid-0.0.5/src/django_mermaid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 12:52:25.000000 django-mermaid-0.0.5/src/django_mermaid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 12:52:25.000000 django-mermaid-0.0.5/src/django_mermaid.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-01 12:52:25.000000 django-mermaid-0.0.5/src/django_mermaid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-01 12:52:25.000000 django-mermaid-0.0.5/src/django_mermaid.egg-info/top_level.txt
```

### Comparing `django-mermaid-0.0.4/LICENSE` & `django-mermaid-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mermaid-0.0.4/PKG-INFO` & `django-mermaid-0.0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,12 @@
-Metadata-Version: 2.1
-Name: django-mermaid
-Version: 0.0.4
-Summary: Django template tag for rendering mermaid diagrams
-Home-page: https://github.com/ArtyomVancyan/django-mermaid
-Author: Artyom Vancyan
-Author-email: artyom@pysnippet.org
-License: MIT
-Keywords: python,django,mermaid,mermaid-diagrams,django-templatetag
-Platform: unix
-Platform: linux
-Platform: osx
-Platform: win32
-Classifier: Framework :: Django
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Django Mermaid
 
-Django template tag for rendering mermaid diagrams.
-
 [![PyPI](https://img.shields.io/pypi/v/django-mermaid.svg)](https://pypi.org/project/django-mermaid/)
+[![Python](https://img.shields.io/pypi/pyversions/django-mermaid.svg?logoColor=white)](https://pypi.org/project/django-mermaid/)
+[![Django](https://img.shields.io/badge/django-1.11%20|%202.0%20|%203.0%20|%204.0%20|%204.2-0C4B33)](https://pypi.org/project/django-mermaid/)
 [![License](https://img.shields.io/pypi/l/django-mermaid.svg)](https://github.com/ArtyomVancyan/django-mermaid/blob/master/LICENSE)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://makeapullrequest.com)
 [![Tests](https://github.com/ArtyomVancyan/django-mermaid/actions/workflows/tests.yml/badge.svg)](https://github.com/ArtyomVancyan/django-mermaid/actions/workflows/tests.yml)
 
 ## Install
 
 ```shell
```

### Comparing `django-mermaid-0.0.4/src/django_mermaid/apps.py` & `django-mermaid-0.0.5/src/django_mermaid/apps.py`

 * *Files identical despite different names*

### Comparing `django-mermaid-0.0.4/src/django_mermaid/templatetags/mermaid.py` & `django-mermaid-0.0.5/src/django_mermaid/templatetags/mermaid.py`

 * *Files identical despite different names*

### Comparing `django-mermaid-0.0.4/src/django_mermaid.egg-info/PKG-INFO` & `django-mermaid-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,50 @@
 Metadata-Version: 2.1
 Name: django-mermaid
-Version: 0.0.4
-Summary: Django template tag for rendering mermaid diagrams
+Version: 0.0.5
+Summary: Django template tag for rendering mermaid diagrams.
 Home-page: https://github.com/ArtyomVancyan/django-mermaid
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: MIT
-Keywords: python,django,mermaid,mermaid-diagrams,django-templatetag
+Keywords: python,django,mermaid,tag,graph,jinja,diagram,template
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: win32
-Classifier: Framework :: Django
 Classifier: Operating System :: OS Independent
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 1.11
+Classifier: Framework :: Django :: 2.0
+Classifier: Framework :: Django :: 2.1
+Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Mermaid
 
-Django template tag for rendering mermaid diagrams.
-
 [![PyPI](https://img.shields.io/pypi/v/django-mermaid.svg)](https://pypi.org/project/django-mermaid/)
+[![Python](https://img.shields.io/pypi/pyversions/django-mermaid.svg?logoColor=white)](https://pypi.org/project/django-mermaid/)
+[![Django](https://img.shields.io/badge/django-1.11%20|%202.0%20|%203.0%20|%204.0%20|%204.2-0C4B33)](https://pypi.org/project/django-mermaid/)
 [![License](https://img.shields.io/pypi/l/django-mermaid.svg)](https://github.com/ArtyomVancyan/django-mermaid/blob/master/LICENSE)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://makeapullrequest.com)
 [![Tests](https://github.com/ArtyomVancyan/django-mermaid/actions/workflows/tests.yml/badge.svg)](https://github.com/ArtyomVancyan/django-mermaid/actions/workflows/tests.yml)
 
 ## Install
 
 ```shell
```

