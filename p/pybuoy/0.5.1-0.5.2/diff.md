# Comparing `tmp/pybuoy-0.5.1.tar.gz` & `tmp/pybuoy-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybuoy-0.5.1.tar", max compression
+gzip compressed data, was "pybuoy-0.5.2.tar", max compression
```

## Comparing `pybuoy-0.5.1.tar` & `pybuoy-0.5.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35149 2022-07-04 22:21:34.001272 pybuoy-0.5.1/LICENSE
--rw-r--r--   0        0        0     1906 2023-03-04 16:06:52.788019 pybuoy-0.5.1/README.rst
--rw-r--r--   0        0        0      102 2022-08-29 13:43:09.385251 pybuoy-0.5.1/pybuoy/__init__.py
--rw-r--r--   0        0        0      508 2023-03-04 15:16:32.461138 pybuoy-0.5.1/pybuoy/api/base.py
--rw-r--r--   0        0        0     4258 2023-03-26 18:14:57.217230 pybuoy-0.5.1/pybuoy/api/forecasts.py
--rw-r--r--   0        0        0     2067 2022-09-18 14:36:45.095868 pybuoy-0.5.1/pybuoy/api/realtime.py
--rw-r--r--   0        0        0      315 2022-08-12 04:44:53.835216 pybuoy-0.5.1/pybuoy/api/stations.py
--rw-r--r--   0        0        0     1031 2023-03-04 15:16:32.461771 pybuoy-0.5.1/pybuoy/buoy.py
--rw-r--r--   0        0        0      645 2023-03-26 18:15:16.697403 pybuoy-0.5.1/pybuoy/const.py
--rw-r--r--   0        0        0      380 2023-03-04 15:16:32.462189 pybuoy-0.5.1/pybuoy/endpoints.py
--rw-r--r--   0        0        0      473 2023-03-04 15:16:32.462365 pybuoy-0.5.1/pybuoy/exceptions.py
--rw-r--r--   0        0        0    20984 2023-03-04 15:16:32.462528 pybuoy-0.5.1/pybuoy/mixins/noaa.xsl
--rw-r--r--   0        0        0     5646 2023-03-04 15:16:32.462882 pybuoy-0.5.1/pybuoy/mixins/parser.py
--rw-r--r--   0        0        0      468 2023-03-04 15:16:32.463026 pybuoy-0.5.1/pybuoy/observation/__init__.py
--rw-r--r--   0        0        0     1745 2022-09-01 01:42:14.442217 pybuoy-0.5.1/pybuoy/observation/meta.py
--rw-r--r--   0        0        0     9314 2023-03-04 15:16:32.463159 pybuoy-0.5.1/pybuoy/observation/observation.py
--rw-r--r--   0        0        0     2205 2022-09-11 21:25:14.182775 pybuoy-0.5.1/pybuoy/observation/observation_datum.py
--rw-r--r--   0        0        0     2362 2023-03-04 15:16:32.463288 pybuoy-0.5.1/pybuoy/observation/observations.py
--rw-r--r--   0        0        0        0 2022-08-12 04:45:40.068525 pybuoy-0.5.1/pybuoy/py.typed
--rw-r--r--   0        0        0     3937 2023-03-04 15:16:32.463486 pybuoy-0.5.1/pybuoy/unit_mappings.py
--rw-r--r--   0        0        0     1554 2023-03-26 18:15:16.697611 pybuoy-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2770 1970-01-01 00:00:00.000000 pybuoy-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-07-04 22:21:34.001272 pybuoy-0.5.2/LICENSE
+-rw-r--r--   0        0        0     1906 2023-03-04 16:06:52.788019 pybuoy-0.5.2/README.rst
+-rw-r--r--   0        0        0      102 2022-08-29 13:43:09.385251 pybuoy-0.5.2/pybuoy/__init__.py
+-rw-r--r--   0        0        0      508 2023-03-04 15:16:32.461138 pybuoy-0.5.2/pybuoy/api/base.py
+-rw-r--r--   0        0        0     4258 2023-03-26 18:14:57.217230 pybuoy-0.5.2/pybuoy/api/forecasts.py
+-rw-r--r--   0        0        0     2067 2022-09-18 14:36:45.095868 pybuoy-0.5.2/pybuoy/api/realtime.py
+-rw-r--r--   0        0        0      315 2022-08-12 04:44:53.835216 pybuoy-0.5.2/pybuoy/api/stations.py
+-rw-r--r--   0        0        0     1031 2023-03-04 15:16:32.461771 pybuoy-0.5.2/pybuoy/buoy.py
+-rw-r--r--   0        0        0      645 2023-05-24 12:55:17.478911 pybuoy-0.5.2/pybuoy/const.py
+-rw-r--r--   0        0        0      380 2023-03-04 15:16:32.462189 pybuoy-0.5.2/pybuoy/endpoints.py
+-rw-r--r--   0        0        0      473 2023-03-04 15:16:32.462365 pybuoy-0.5.2/pybuoy/exceptions.py
+-rw-r--r--   0        0        0    20984 2023-03-04 15:16:32.462528 pybuoy-0.5.2/pybuoy/mixins/noaa.xsl
+-rw-r--r--   0        0        0     5646 2023-03-04 15:16:32.462882 pybuoy-0.5.2/pybuoy/mixins/parser.py
+-rw-r--r--   0        0        0      468 2023-03-04 15:16:32.463026 pybuoy-0.5.2/pybuoy/observation/__init__.py
+-rw-r--r--   0        0        0     1745 2022-09-01 01:42:14.442217 pybuoy-0.5.2/pybuoy/observation/meta.py
+-rw-r--r--   0        0        0     9314 2023-03-04 15:16:32.463159 pybuoy-0.5.2/pybuoy/observation/observation.py
+-rw-r--r--   0        0        0     2205 2022-09-11 21:25:14.182775 pybuoy-0.5.2/pybuoy/observation/observation_datum.py
+-rw-r--r--   0        0        0     2362 2023-03-04 15:16:32.463288 pybuoy-0.5.2/pybuoy/observation/observations.py
+-rw-r--r--   0        0        0        0 2022-08-12 04:45:40.068525 pybuoy-0.5.2/pybuoy/py.typed
+-rw-r--r--   0        0        0     3937 2023-03-04 15:16:32.463486 pybuoy-0.5.2/pybuoy/unit_mappings.py
+-rw-r--r--   0        0        0     1553 2023-05-24 12:55:07.776108 pybuoy-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2719 1970-01-01 00:00:00.000000 pybuoy-0.5.2/PKG-INFO
```

### Comparing `pybuoy-0.5.1/LICENSE` & `pybuoy-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybuoy-0.5.1/README.rst` & `pybuoy-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `pybuoy-0.5.1/pybuoy/api/forecasts.py` & `pybuoy-0.5.2/pybuoy/api/forecasts.py`

 * *Files identical despite different names*

### Comparing `pybuoy-0.5.1/pybuoy/api/realtime.py` & `pybuoy-0.5.2/pybuoy/api/realtime.py`

 * *Files identical despite different names*

### Comparing `pybuoy-0.5.1/pybuoy/buoy.py` & `pybuoy-0.5.2/pybuoy/buoy.py`

 * *Files identical despite different names*

### Comparing `pybuoy-0.5.1/pybuoy/const.py` & `pybuoy-0.5.2/pybuoy/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,8 +31,8 @@
     "swdir",
     "swdir2",
     "swr1",
     "swr2",
     "txt",
 ]
 
-__version__ = "0.5.1"
+__version__ = "0.5.2"
```

### Comparing `pybuoy-0.5.1/pybuoy/mixins/noaa.xsl` & `pybuoy-0.5.2/pybuoy/mixins/noaa.xsl`

 * *Files identical despite different names*

### Comparing `pybuoy-0.5.1/pybuoy/mixins/parser.py` & `pybuoy-0.5.2/pybuoy/mixins/parser.py`

 * *Files identical despite different names*

### Comparing `pybuoy-0.5.1/pybuoy/observation/meta.py` & `pybuoy-0.5.2/pybuoy/observation/meta.py`

 * *Files identical despite different names*

### Comparing `pybuoy-0.5.1/pybuoy/observation/observation.py` & `pybuoy-0.5.2/pybuoy/observation/observation.py`

 * *Files identical despite different names*

### Comparing `pybuoy-0.5.1/pybuoy/observation/observation_datum.py` & `pybuoy-0.5.2/pybuoy/observation/observation_datum.py`

 * *Files identical despite different names*

### Comparing `pybuoy-0.5.1/pybuoy/observation/observations.py` & `pybuoy-0.5.2/pybuoy/observation/observations.py`

 * *Files identical despite different names*

### Comparing `pybuoy-0.5.1/pybuoy/unit_mappings.py` & `pybuoy-0.5.2/pybuoy/unit_mappings.py`

 * *Files identical despite different names*

### Comparing `pybuoy-0.5.1/pyproject.toml` & `pybuoy-0.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybuoy"
-version = "0.5.1"
+version = "0.5.2"
 authors = ["Kyle J. Burda <kylejbdev@gmail.com>"]
 classifiers=[
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3.11",
 ]
 description = "Python wrapper for NOAA and NDBC REST web services."
 documentation = "https://pybuoy.readthedocs.io"
@@ -14,33 +14,33 @@
 readme = "README.rst"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/clairBuoyant/pybuoy"
 "Bug Tracker" = "https://github.com/clairBuoyant/pybuoy/issues"
 
 [tool.poetry.dependencies]
-python = "^3.11"
-requests = "^2.28.2"
 lxml = "^4.9.2"
+python = "^3.11"
+requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.1.0"
+black = "^23.3.0"
 flake8 = "^6.0.0"
-isort = { version = "^5.11.5", extras = ["pyproject"]}
-mypy = "^1.0.1"
-pytest = "^7.2.1"
-pre-commit = "^3.0.4"
-types-requests = "^2.28.11"
+isort = { version = "^5.12.0", extras = ["pyproject"]}
+mypy = "^1.3.0"
+pre-commit = "^3.3.2"
+pytest = "^7.3.1"
+types-requests = "^2.31.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-Sphinx = "^6.1.3"
 furo = "^2022.12.7"
+Sphinx = "^6.1.3"
 
 [tool.black]
 line-length = 88
 target_version = ['py310']
 exclude = '''
 (
   /(
```

### Comparing `pybuoy-0.5.1/PKG-INFO` & `pybuoy-0.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: pybuoy
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python wrapper for NOAA and NDBC REST web services.
 License: GPL-3.0-or-later
 Keywords: NDBC,NOAA,api,buoy,weather,wrapper
 Author: Kyle J. Burda
 Author-email: kylejbdev@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/clairBuoyant/pybuoy/issues
 Project-URL: Documentation, https://pybuoy.readthedocs.io
 Project-URL: Source Code, https://github.com/clairBuoyant/pybuoy
 Description-Content-Type: text/x-rst
 
 =====================================
 pybuoy - Python NOAA/NDBC API Wrapper
```

