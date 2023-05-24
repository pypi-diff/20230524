# Comparing `tmp/django-forbid-0.0.6.tar.gz` & `tmp/django-forbid-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-forbid-0.0.6.tar", last modified: Mon Apr 17 15:36:39 2023, max compression
+gzip compressed data, was "django-forbid-0.0.7.tar", last modified: Tue May 16 18:13:36 2023, max compression
```

## Comparing `django-forbid-0.0.6.tar` & `django-forbid-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:36:39.547046 django-forbid-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-17 15:36:29.000000 django-forbid-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-04-17 15:36:39.547046 django-forbid-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-17 15:36:29.000000 django-forbid-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-17 15:36:29.000000 django-forbid-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-17 15:36:39.547046 django-forbid-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 15:36:29.000000 django-forbid-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:36:39.543046 django-forbid-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:36:39.543046 django-forbid-0.0.6/src/django_forbid/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 15:36:29.000000 django-forbid-0.0.6/src/django_forbid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-17 15:36:29.000000 django-forbid-0.0.6/src/django_forbid/access.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-17 15:36:29.000000 django-forbid-0.0.6/src/django_forbid/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-17 15:36:29.000000 django-forbid-0.0.6/src/django_forbid/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-17 15:36:29.000000 django-forbid-0.0.6/src/django_forbid/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-17 15:36:29.000000 django-forbid-0.0.6/src/django_forbid/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-17 15:36:29.000000 django-forbid-0.0.6/src/django_forbid/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:36:39.543046 django-forbid-0.0.6/src/django_forbid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-04-17 15:36:39.000000 django-forbid-0.0.6/src/django_forbid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-17 15:36:39.000000 django-forbid-0.0.6/src/django_forbid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:36:39.000000 django-forbid-0.0.6/src/django_forbid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:36:39.000000 django-forbid-0.0.6/src/django_forbid.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-17 15:36:39.000000 django-forbid-0.0.6/src/django_forbid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-17 15:36:39.000000 django-forbid-0.0.6/src/django_forbid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:13:36.357143 django-forbid-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 18:13:23.000000 django-forbid-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-05-16 18:13:36.357143 django-forbid-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-16 18:13:23.000000 django-forbid-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-16 18:13:23.000000 django-forbid-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-16 18:13:36.357143 django-forbid-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 18:13:23.000000 django-forbid-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:13:36.357143 django-forbid-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:13:36.357143 django-forbid-0.0.7/src/django_forbid/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 18:13:23.000000 django-forbid-0.0.7/src/django_forbid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-16 18:13:23.000000 django-forbid-0.0.7/src/django_forbid/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-16 18:13:23.000000 django-forbid-0.0.7/src/django_forbid/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-16 18:13:23.000000 django-forbid-0.0.7/src/django_forbid/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:13:36.357143 django-forbid-0.0.7/src/django_forbid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-05-16 18:13:36.000000 django-forbid-0.0.7/src/django_forbid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-16 18:13:36.000000 django-forbid-0.0.7/src/django_forbid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:13:36.000000 django-forbid-0.0.7/src/django_forbid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:13:36.000000 django-forbid-0.0.7/src/django_forbid.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-16 18:13:36.000000 django-forbid-0.0.7/src/django_forbid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 18:13:36.000000 django-forbid-0.0.7/src/django_forbid.egg-info/top_level.txt
```

### Comparing `django-forbid-0.0.6/LICENSE` & `django-forbid-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-forbid-0.0.6/PKG-INFO` & `django-forbid-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-forbid
-Version: 0.0.6
+Version: 0.0.7
 Summary: Secure your Django app by controlling the access - grant or deny user access based on device and location, including VPN detection.
 Home-page: https://github.com/pysnippet/django-forbid
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: MIT
 Keywords: python,django,permit,forbid,access,device,secure,country,control,security,location,territory,vpn,detection,django-forbid
 Platform: unix
@@ -29,23 +29,24 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Forbid <img src="https://github.com/pysnippet.png" align="right" height="64" />
 
-Secure your Django app by controlling the access - grant or deny user access based on device and location, including VPN
-detection.
-
 [![PyPI](https://img.shields.io/pypi/v/django-forbid.svg)](https://pypi.org/project/django-forbid/)
 [![Python](https://img.shields.io/pypi/pyversions/django-forbid.svg?logoColor=white)](https://pypi.org/project/django-forbid/)
 [![Django](https://img.shields.io/pypi/djversions/django-forbid.svg?color=0C4B33&label=django)](https://pypi.org/project/django-forbid/)
 [![License](https://img.shields.io/pypi/l/django-forbid.svg)](https://github.com/pysnippet/django-forbid/blob/master/LICENSE)
 [![Tests](https://github.com/pysnippet/django-forbid/actions/workflows/tests.yml/badge.svg)](https://github.com/pysnippet/django-forbid/actions/workflows/tests.yml)
 
+Django Forbid aims to make website access managed and secure for the maintainers. It provides a middleware to grant or
+deny user access based on device and/or location. It also supports VPN detection for banning users who want to lie about
+their country and geolocation. Also, users can use only the VPN detection feature or disable it.
+
 ## Install
 
 ```shell
 python -m pip install django-forbid
 ```
 
 ## Configuration
```

### Comparing `django-forbid-0.0.6/README.md` & `django-forbid-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Django Forbid <img src="https://github.com/pysnippet.png" align="right" height="64" />
 
-Secure your Django app by controlling the access - grant or deny user access based on device and location, including VPN
-detection.
-
 [![PyPI](https://img.shields.io/pypi/v/django-forbid.svg)](https://pypi.org/project/django-forbid/)
 [![Python](https://img.shields.io/pypi/pyversions/django-forbid.svg?logoColor=white)](https://pypi.org/project/django-forbid/)
 [![Django](https://img.shields.io/pypi/djversions/django-forbid.svg?color=0C4B33&label=django)](https://pypi.org/project/django-forbid/)
 [![License](https://img.shields.io/pypi/l/django-forbid.svg)](https://github.com/pysnippet/django-forbid/blob/master/LICENSE)
 [![Tests](https://github.com/pysnippet/django-forbid/actions/workflows/tests.yml/badge.svg)](https://github.com/pysnippet/django-forbid/actions/workflows/tests.yml)
 
+Django Forbid aims to make website access managed and secure for the maintainers. It provides a middleware to grant or
+deny user access based on device and/or location. It also supports VPN detection for banning users who want to lie about
+their country and geolocation. Also, users can use only the VPN detection feature or disable it.
+
 ## Install
 
 ```shell
 python -m pip install django-forbid
 ```
 
 ## Configuration
```

### Comparing `django-forbid-0.0.6/setup.cfg` & `django-forbid-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-forbid-0.0.6/src/django_forbid/config.py` & `django-forbid-0.0.7/src/django_forbid/config.py`

 * *Files identical despite different names*

### Comparing `django-forbid-0.0.6/src/django_forbid.egg-info/PKG-INFO` & `django-forbid-0.0.7/src/django_forbid.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-forbid
-Version: 0.0.6
+Version: 0.0.7
 Summary: Secure your Django app by controlling the access - grant or deny user access based on device and location, including VPN detection.
 Home-page: https://github.com/pysnippet/django-forbid
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: MIT
 Keywords: python,django,permit,forbid,access,device,secure,country,control,security,location,territory,vpn,detection,django-forbid
 Platform: unix
@@ -29,23 +29,24 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Forbid <img src="https://github.com/pysnippet.png" align="right" height="64" />
 
-Secure your Django app by controlling the access - grant or deny user access based on device and location, including VPN
-detection.
-
 [![PyPI](https://img.shields.io/pypi/v/django-forbid.svg)](https://pypi.org/project/django-forbid/)
 [![Python](https://img.shields.io/pypi/pyversions/django-forbid.svg?logoColor=white)](https://pypi.org/project/django-forbid/)
 [![Django](https://img.shields.io/pypi/djversions/django-forbid.svg?color=0C4B33&label=django)](https://pypi.org/project/django-forbid/)
 [![License](https://img.shields.io/pypi/l/django-forbid.svg)](https://github.com/pysnippet/django-forbid/blob/master/LICENSE)
 [![Tests](https://github.com/pysnippet/django-forbid/actions/workflows/tests.yml/badge.svg)](https://github.com/pysnippet/django-forbid/actions/workflows/tests.yml)
 
+Django Forbid aims to make website access managed and secure for the maintainers. It provides a middleware to grant or
+deny user access based on device and/or location. It also supports VPN detection for banning users who want to lie about
+their country and geolocation. Also, users can use only the VPN detection feature or disable it.
+
 ## Install
 
 ```shell
 python -m pip install django-forbid
 ```
 
 ## Configuration
```

