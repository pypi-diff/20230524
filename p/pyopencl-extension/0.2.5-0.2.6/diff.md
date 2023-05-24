# Comparing `tmp/pyopencl-extension-0.2.5.tar.gz` & `tmp/pyopencl-extension-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopencl-extension-0.2.5.tar", last modified: Thu Mar 23 13:03:57 2023, max compression
+gzip compressed data, was "pyopencl-extension-0.2.6.tar", last modified: Wed May 24 12:32:27 2023, max compression
```

## Comparing `pyopencl-extension-0.2.5.tar` & `pyopencl-extension-0.2.6.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 13:03:57.305140 pyopencl-extension-0.2.5/
--rw-rw-rw-   0        0        0     1994 2021-02-20 16:14:08.000000 pyopencl-extension-0.2.5/.gitignore
--rw-rw-rw-   0        0        0     1084 2022-10-04 15:29:34.000000 pyopencl-extension-0.2.5/LICENSE
--rw-rw-rw-   0        0        0     3333 2023-03-23 13:03:57.305140 pyopencl-extension-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     2583 2022-10-04 15:29:34.000000 pyopencl-extension-0.2.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-23 13:03:57.236107 pyopencl-extension-0.2.5/examples/
--rw-rw-rw-   0        0        0        0 2021-02-04 18:19:20.000000 pyopencl-extension-0.2.5/examples/__init__.py
--rw-rw-rw-   0        0        0      515 2021-11-16 11:51:09.000000 pyopencl-extension-0.2.5/examples/minimal.py
-drwxrwxrwx   0        0        0        0 2023-03-23 13:03:57.251780 pyopencl-extension-0.2.5/pyopencl_extension/
--rw-rw-rw-   0        0        0     1252 2023-02-26 16:33:31.000000 pyopencl-extension-0.2.5/pyopencl_extension/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-23 13:03:57.258289 pyopencl-extension-0.2.5/pyopencl_extension/components/
--rw-rw-rw-   0        0        0        0 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.5/pyopencl_extension/components/__init__.py
--rw-rw-rw-   0        0        0    13458 2023-01-16 12:36:15.000000 pyopencl-extension-0.2.5/pyopencl_extension/components/copy_array_region.py
--rw-rw-rw-   0        0        0    23764 2022-10-04 15:30:53.000000 pyopencl-extension-0.2.5/pyopencl_extension/components/fft.py
--rw-rw-rw-   0        0        0       61 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.5/pyopencl_extension/components/pytest.ini
--rw-rw-rw-   0        0        0     4241 2022-10-04 15:30:53.000000 pyopencl-extension-0.2.5/pyopencl_extension/components/sumalongaxis.py
--rw-rw-rw-   0        0        0     3893 2022-10-04 15:30:53.000000 pyopencl-extension-0.2.5/pyopencl_extension/components/transpose.py
--rw-rw-rw-   0        0        0    40168 2023-03-23 11:16:57.000000 pyopencl-extension-0.2.5/pyopencl_extension/emulation.py
--rw-rw-rw-   0        0        0    42315 2023-03-02 10:19:10.000000 pyopencl-extension-0.2.5/pyopencl_extension/framework.py
-drwxrwxrwx   0        0        0        0 2023-03-23 13:03:57.273908 pyopencl-extension-0.2.5/pyopencl_extension/helpers/
--rw-rw-rw-   0        0        0        0 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.5/pyopencl_extension/helpers/__init__.py
--rw-rw-rw-   0        0        0     1048 2022-10-04 15:30:53.000000 pyopencl-extension-0.2.5/pyopencl_extension/helpers/general.py
--rw-rw-rw-   0        0        0      605 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.5/pyopencl_extension/helpers/setup_pyopencl.py
-drwxrwxrwx   0        0        0        0 2023-03-23 13:03:57.273908 pyopencl-extension-0.2.5/pyopencl_extension/modifications_pyopencl/
--rw-rw-rw-   0        0        0        0 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.5/pyopencl_extension/modifications_pyopencl/__init__.py
--rw-rw-rw-   0        0        0     2737 2022-06-22 15:19:37.000000 pyopencl-extension-0.2.5/pyopencl_extension/modifications_pyopencl/array.py
--rw-rw-rw-   0        0        0     4862 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.5/pyopencl_extension/modifications_pyopencl/cltypes.py
--rw-rw-rw-   0        0        0     9240 2022-05-25 11:16:39.000000 pyopencl-extension-0.2.5/pyopencl_extension/modifications_pyopencl/command_queue.py
--rw-rw-rw-   0        0        0     1378 2022-02-18 12:09:00.000000 pyopencl-extension-0.2.5/pyopencl_extension/modifications_pyopencl/context.py
-drwxrwxrwx   0        0        0        0 2023-03-23 13:03:57.289529 pyopencl-extension-0.2.5/pyopencl_extension/types/
--rw-rw-rw-   0        0        0        0 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.5/pyopencl_extension/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-23 13:03:57.289529 pyopencl-extension-0.2.5/pyopencl_extension/types/auto_gen/
--rw-rw-rw-   0        0        0        0 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.5/pyopencl_extension/types/auto_gen/__init__.py
--rw-rw-rw-   0        0        0     3155 2023-02-12 21:05:55.000000 pyopencl-extension-0.2.5/pyopencl_extension/types/auto_gen/cl_types.py
--rw-rw-rw-   0        0        0     1399 2023-02-12 21:05:55.000000 pyopencl-extension-0.2.5/pyopencl_extension/types/auto_gen/cl_types_import.py
--rw-rw-rw-   0        0        0     3706 2023-02-12 21:05:53.000000 pyopencl-extension-0.2.5/pyopencl_extension/types/auto_gen/generate_files.py
--rw-rw-rw-   0        0        0     2014 2023-02-12 21:05:55.000000 pyopencl-extension-0.2.5/pyopencl_extension/types/auto_gen/types_for_emulation.py
--rw-rw-rw-   0        0        0     5159 2022-06-01 11:28:11.000000 pyopencl-extension-0.2.5/pyopencl_extension/types/funcs_for_emulation.py
--rw-rw-rw-   0        0        0    12075 2021-11-17 18:50:32.000000 pyopencl-extension-0.2.5/pyopencl_extension/types/type_handler.py
--rw-rw-rw-   0        0        0     7414 2022-10-04 15:30:53.000000 pyopencl-extension-0.2.5/pyopencl_extension/types/utilities_np_cl.py
-drwxrwxrwx   0        0        0        0 2023-03-23 13:03:57.258289 pyopencl-extension-0.2.5/pyopencl_extension.egg-info/
--rw-rw-rw-   0        0        0     3333 2023-03-23 13:03:56.000000 pyopencl-extension-0.2.5/pyopencl_extension.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1750 2023-03-23 13:03:57.000000 pyopencl-extension-0.2.5/pyopencl_extension.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-23 13:03:56.000000 pyopencl-extension-0.2.5/pyopencl_extension.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-03-23 13:03:56.000000 pyopencl-extension-0.2.5/pyopencl_extension.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-03-23 13:03:56.000000 pyopencl-extension-0.2.5/pyopencl_extension.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-23 13:03:57.305140 pyopencl-extension-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     5529 2023-03-23 13:00:38.000000 pyopencl-extension-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-23 13:03:57.289529 pyopencl-extension-0.2.5/tests/
--rw-rw-rw-   0        0        0        0 2020-04-20 11:14:23.000000 pyopencl-extension-0.2.5/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2021-11-16 10:28:59.000000 pyopencl-extension-0.2.5/tests/conftest.py
--rw-rw-rw-   0        0        0       77 2022-07-25 11:40:17.000000 pyopencl-extension-0.2.5/tests/pytest.ini
-drwxrwxrwx   0        0        0        0 2023-03-23 13:03:57.305140 pyopencl-extension-0.2.5/tests/test_components/
--rw-rw-rw-   0        0        0        0 2021-02-04 17:45:00.000000 pyopencl-extension-0.2.5/tests/test_components/__init__.py
--rw-rw-rw-   0        0        0     2532 2021-11-16 11:30:31.000000 pyopencl-extension-0.2.5/tests/test_components/test_copy_array_region.py
--rw-rw-rw-   0        0        0     4597 2021-11-16 11:33:33.000000 pyopencl-extension-0.2.5/tests/test_components/test_fft.py
--rw-rw-rw-   0        0        0      807 2021-11-16 11:35:44.000000 pyopencl-extension-0.2.5/tests/test_components/test_sum.py
--rw-rw-rw-   0        0        0     1368 2021-11-16 11:36:28.000000 pyopencl-extension-0.2.5/tests/test_components/test_transpose.py
--rw-rw-rw-   0        0        0    21012 2023-03-23 11:16:32.000000 pyopencl-extension-0.2.5/tests/test_emulation.py
--rw-rw-rw-   0        0        0    13024 2023-02-26 19:40:12.000000 pyopencl-extension-0.2.5/tests/test_framework.py
+drwxrwxrwx   0        0        0        0 2023-05-24 12:32:27.897037 pyopencl-extension-0.2.6/
+-rw-rw-rw-   0        0        0     1994 2021-02-20 16:14:08.000000 pyopencl-extension-0.2.6/.gitignore
+-rw-rw-rw-   0        0        0     1084 2022-10-04 15:29:34.000000 pyopencl-extension-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0     3333 2023-05-24 12:32:27.896040 pyopencl-extension-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2583 2022-10-04 15:29:34.000000 pyopencl-extension-0.2.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-24 12:32:27.817225 pyopencl-extension-0.2.6/examples/
+-rw-rw-rw-   0        0        0        0 2021-02-04 18:19:20.000000 pyopencl-extension-0.2.6/examples/__init__.py
+-rw-rw-rw-   0        0        0      515 2021-11-16 11:51:09.000000 pyopencl-extension-0.2.6/examples/minimal.py
+drwxrwxrwx   0        0        0        0 2023-05-24 12:32:27.824256 pyopencl-extension-0.2.6/pyopencl_extension/
+-rw-rw-rw-   0        0        0     1252 2023-02-26 16:33:31.000000 pyopencl-extension-0.2.6/pyopencl_extension/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 12:32:27.845224 pyopencl-extension-0.2.6/pyopencl_extension/components/
+-rw-rw-rw-   0        0        0        0 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.6/pyopencl_extension/components/__init__.py
+-rw-rw-rw-   0        0        0    13458 2023-01-16 12:36:15.000000 pyopencl-extension-0.2.6/pyopencl_extension/components/copy_array_region.py
+-rw-rw-rw-   0        0        0    23764 2022-10-04 15:30:53.000000 pyopencl-extension-0.2.6/pyopencl_extension/components/fft.py
+-rw-rw-rw-   0        0        0       61 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.6/pyopencl_extension/components/pytest.ini
+-rw-rw-rw-   0        0        0     4241 2022-10-04 15:30:53.000000 pyopencl-extension-0.2.6/pyopencl_extension/components/sumalongaxis.py
+-rw-rw-rw-   0        0        0     3893 2022-10-04 15:30:53.000000 pyopencl-extension-0.2.6/pyopencl_extension/components/transpose.py
+-rw-rw-rw-   0        0        0    40168 2023-03-23 11:16:57.000000 pyopencl-extension-0.2.6/pyopencl_extension/emulation.py
+-rw-rw-rw-   0        0        0    42315 2023-03-02 10:19:10.000000 pyopencl-extension-0.2.6/pyopencl_extension/framework.py
+drwxrwxrwx   0        0        0        0 2023-05-24 12:32:27.849346 pyopencl-extension-0.2.6/pyopencl_extension/helpers/
+-rw-rw-rw-   0        0        0        0 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.6/pyopencl_extension/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1048 2022-10-04 15:30:53.000000 pyopencl-extension-0.2.6/pyopencl_extension/helpers/general.py
+-rw-rw-rw-   0        0        0      605 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.6/pyopencl_extension/helpers/setup_pyopencl.py
+drwxrwxrwx   0        0        0        0 2023-05-24 12:32:27.859128 pyopencl-extension-0.2.6/pyopencl_extension/modifications_pyopencl/
+-rw-rw-rw-   0        0        0        0 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.6/pyopencl_extension/modifications_pyopencl/__init__.py
+-rw-rw-rw-   0        0        0     2737 2022-06-22 15:19:37.000000 pyopencl-extension-0.2.6/pyopencl_extension/modifications_pyopencl/array.py
+-rw-rw-rw-   0        0        0     4862 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.6/pyopencl_extension/modifications_pyopencl/cltypes.py
+-rw-rw-rw-   0        0        0     9483 2023-05-24 12:07:46.000000 pyopencl-extension-0.2.6/pyopencl_extension/modifications_pyopencl/command_queue.py
+-rw-rw-rw-   0        0        0     1378 2022-02-18 12:09:00.000000 pyopencl-extension-0.2.6/pyopencl_extension/modifications_pyopencl/context.py
+drwxrwxrwx   0        0        0        0 2023-05-24 12:32:27.865112 pyopencl-extension-0.2.6/pyopencl_extension/types/
+-rw-rw-rw-   0        0        0        0 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.6/pyopencl_extension/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 12:32:27.876109 pyopencl-extension-0.2.6/pyopencl_extension/types/auto_gen/
+-rw-rw-rw-   0        0        0        0 2021-03-31 13:30:36.000000 pyopencl-extension-0.2.6/pyopencl_extension/types/auto_gen/__init__.py
+-rw-rw-rw-   0        0        0     3155 2023-02-12 21:05:55.000000 pyopencl-extension-0.2.6/pyopencl_extension/types/auto_gen/cl_types.py
+-rw-rw-rw-   0        0        0     1399 2023-02-12 21:05:55.000000 pyopencl-extension-0.2.6/pyopencl_extension/types/auto_gen/cl_types_import.py
+-rw-rw-rw-   0        0        0     3706 2023-02-12 21:05:53.000000 pyopencl-extension-0.2.6/pyopencl_extension/types/auto_gen/generate_files.py
+-rw-rw-rw-   0        0        0     2014 2023-02-12 21:05:55.000000 pyopencl-extension-0.2.6/pyopencl_extension/types/auto_gen/types_for_emulation.py
+-rw-rw-rw-   0        0        0     5159 2022-06-01 11:28:11.000000 pyopencl-extension-0.2.6/pyopencl_extension/types/funcs_for_emulation.py
+-rw-rw-rw-   0        0        0    12075 2021-11-17 18:50:32.000000 pyopencl-extension-0.2.6/pyopencl_extension/types/type_handler.py
+-rw-rw-rw-   0        0        0     7414 2022-10-04 15:30:53.000000 pyopencl-extension-0.2.6/pyopencl_extension/types/utilities_np_cl.py
+drwxrwxrwx   0        0        0        0 2023-05-24 12:32:27.834619 pyopencl-extension-0.2.6/pyopencl_extension.egg-info/
+-rw-rw-rw-   0        0        0     3333 2023-05-24 12:32:27.000000 pyopencl-extension-0.2.6/pyopencl_extension.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1750 2023-05-24 12:32:27.000000 pyopencl-extension-0.2.6/pyopencl_extension.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 12:32:27.000000 pyopencl-extension-0.2.6/pyopencl_extension.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2023-05-24 12:32:27.000000 pyopencl-extension-0.2.6/pyopencl_extension.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-24 12:32:27.000000 pyopencl-extension-0.2.6/pyopencl_extension.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 12:32:27.897037 pyopencl-extension-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     5529 2023-05-24 12:09:15.000000 pyopencl-extension-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 12:32:27.884094 pyopencl-extension-0.2.6/tests/
+-rw-rw-rw-   0        0        0        0 2020-04-20 11:14:23.000000 pyopencl-extension-0.2.6/tests/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-11-16 10:28:59.000000 pyopencl-extension-0.2.6/tests/conftest.py
+-rw-rw-rw-   0        0        0       77 2022-07-25 11:40:17.000000 pyopencl-extension-0.2.6/tests/pytest.ini
+drwxrwxrwx   0        0        0        0 2023-05-24 12:32:27.894051 pyopencl-extension-0.2.6/tests/test_components/
+-rw-rw-rw-   0        0        0        0 2021-02-04 17:45:00.000000 pyopencl-extension-0.2.6/tests/test_components/__init__.py
+-rw-rw-rw-   0        0        0     2532 2021-11-16 11:30:31.000000 pyopencl-extension-0.2.6/tests/test_components/test_copy_array_region.py
+-rw-rw-rw-   0        0        0     4597 2021-11-16 11:33:33.000000 pyopencl-extension-0.2.6/tests/test_components/test_fft.py
+-rw-rw-rw-   0        0        0      807 2021-11-16 11:35:44.000000 pyopencl-extension-0.2.6/tests/test_components/test_sum.py
+-rw-rw-rw-   0        0        0     1368 2021-11-16 11:36:28.000000 pyopencl-extension-0.2.6/tests/test_components/test_transpose.py
+-rw-rw-rw-   0        0        0    21012 2023-03-23 11:16:32.000000 pyopencl-extension-0.2.6/tests/test_emulation.py
+-rw-rw-rw-   0        0        0    13024 2023-02-26 19:40:12.000000 pyopencl-extension-0.2.6/tests/test_framework.py
```

### Comparing `pyopencl-extension-0.2.5/.gitignore` & `pyopencl-extension-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/LICENSE` & `pyopencl-extension-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/PKG-INFO` & `pyopencl-extension-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopencl-extension
-Version: 0.2.5
+Version: 0.2.6
 Summary: This package extends PyOpenCl by providing an object-oriented kernel programming framework and debugging capabilities.
 Home-page: https://github.com/philipp-mohr/pyopencl-extension
 Author: P.Mohr
 Author-email: philipp.mohr@tuhh.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyopencl-extension-0.2.5/README.rst` & `pyopencl-extension-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/examples/minimal.py` & `pyopencl-extension-0.2.6/examples/minimal.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/pyopencl_extension/__init__.py` & `pyopencl-extension-0.2.6/pyopencl_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/pyopencl_extension/components/copy_array_region.py` & `pyopencl-extension-0.2.6/pyopencl_extension/components/copy_array_region.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/pyopencl_extension/components/fft.py` & `pyopencl-extension-0.2.6/pyopencl_extension/components/fft.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/pyopencl_extension/components/sumalongaxis.py` & `pyopencl-extension-0.2.6/pyopencl_extension/components/sumalongaxis.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/pyopencl_extension/components/transpose.py` & `pyopencl-extension-0.2.6/pyopencl_extension/components/transpose.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/pyopencl_extension/emulation.py` & `pyopencl-extension-0.2.6/pyopencl_extension/emulation.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/pyopencl_extension/framework.py` & `pyopencl-extension-0.2.6/pyopencl_extension/framework.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/pyopencl_extension/helpers/general.py` & `pyopencl-extension-0.2.6/pyopencl_extension/helpers/general.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/pyopencl_extension/helpers/setup_pyopencl.py` & `pyopencl-extension-0.2.6/pyopencl_extension/helpers/setup_pyopencl.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/pyopencl_extension/modifications_pyopencl/array.py` & `pyopencl-extension-0.2.6/pyopencl_extension/modifications_pyopencl/array.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/pyopencl_extension/modifications_pyopencl/cltypes.py` & `pyopencl-extension-0.2.6/pyopencl_extension/modifications_pyopencl/cltypes.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/pyopencl_extension/modifications_pyopencl/command_queue.py` & `pyopencl-extension-0.2.6/pyopencl_extension/modifications_pyopencl/command_queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,14 @@
         self.profiling_enabled = True if self.properties == cl.command_queue_properties.PROFILING_ENABLE else False
         self.t_ns = TimingsQueue(profiling_enabled=self.profiling_enabled)
 
     @property
     def context(self) -> Context:
         return self._context
 
-
     def get_profiler(self) -> 'Profiling':
         self.t_ns.profiling_finished = time.perf_counter_ns()
         self.t_ns.compilation = self.context.time_compilation_ns
         return Profiling(self)
 
     def add_event(self, event, name):
         if self.profiling_enabled:
@@ -231,7 +230,14 @@
         _current_queue = create_queue(_default_device, *args, **kwargs)
     return _current_queue
 
 
 def get_device(device_id: int) -> cl.Device:
     return get_devices()[device_id]
 
+
+def activate_profiling(**kwargs):
+    set_current_queue(create_queue(queue_properties=QueueProperties.PROFILING_ENABLE, **kwargs))
+
+
+def evaluate_profiling():
+    get_current_queue().get_profiler().show_histogram_cumulative_kernel_times()
```

### Comparing `pyopencl-extension-0.2.5/pyopencl_extension/modifications_pyopencl/context.py` & `pyopencl-extension-0.2.6/pyopencl_extension/modifications_pyopencl/context.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/pyopencl_extension/types/auto_gen/cl_types.py` & `pyopencl-extension-0.2.6/pyopencl_extension/types/auto_gen/cl_types.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/pyopencl_extension/types/auto_gen/cl_types_import.py` & `pyopencl-extension-0.2.6/pyopencl_extension/types/auto_gen/cl_types_import.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/pyopencl_extension/types/auto_gen/generate_files.py` & `pyopencl-extension-0.2.6/pyopencl_extension/types/auto_gen/generate_files.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/pyopencl_extension/types/auto_gen/types_for_emulation.py` & `pyopencl-extension-0.2.6/pyopencl_extension/types/auto_gen/types_for_emulation.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/pyopencl_extension/types/funcs_for_emulation.py` & `pyopencl-extension-0.2.6/pyopencl_extension/types/funcs_for_emulation.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/pyopencl_extension/types/type_handler.py` & `pyopencl-extension-0.2.6/pyopencl_extension/types/type_handler.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/pyopencl_extension/types/utilities_np_cl.py` & `pyopencl-extension-0.2.6/pyopencl_extension/types/utilities_np_cl.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/pyopencl_extension.egg-info/PKG-INFO` & `pyopencl-extension-0.2.6/pyopencl_extension.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopencl-extension
-Version: 0.2.5
+Version: 0.2.6
 Summary: This package extends PyOpenCl by providing an object-oriented kernel programming framework and debugging capabilities.
 Home-page: https://github.com/philipp-mohr/pyopencl-extension
 Author: P.Mohr
 Author-email: philipp.mohr@tuhh.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyopencl-extension-0.2.5/pyopencl_extension.egg-info/SOURCES.txt` & `pyopencl-extension-0.2.6/pyopencl_extension.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/setup.py` & `pyopencl-extension-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 NAME = 'pyopencl-extension'
 DESCRIPTION = 'This package extends PyOpenCl by providing an object-oriented kernel programming framework and ' \
               'debugging capabilities.'
 URL = 'https://github.com/philipp-mohr/pyopencl-extension'
 EMAIL = 'philipp.mohr@tuhh.de'
 AUTHOR = 'P.Mohr'
 REQUIRES_PYTHON = '>=3.10.0'
-VERSION = '0.2.5'
+VERSION = '0.2.6'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'numpy', 'pyopencl', 'mako', 'pycparser', 'pycparserext', 'pyastyle'  # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

### Comparing `pyopencl-extension-0.2.5/tests/test_components/test_copy_array_region.py` & `pyopencl-extension-0.2.6/tests/test_components/test_copy_array_region.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/tests/test_components/test_fft.py` & `pyopencl-extension-0.2.6/tests/test_components/test_fft.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/tests/test_components/test_sum.py` & `pyopencl-extension-0.2.6/tests/test_components/test_sum.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/tests/test_components/test_transpose.py` & `pyopencl-extension-0.2.6/tests/test_components/test_transpose.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/tests/test_emulation.py` & `pyopencl-extension-0.2.6/tests/test_emulation.py`

 * *Files identical despite different names*

### Comparing `pyopencl-extension-0.2.5/tests/test_framework.py` & `pyopencl-extension-0.2.6/tests/test_framework.py`

 * *Files identical despite different names*

