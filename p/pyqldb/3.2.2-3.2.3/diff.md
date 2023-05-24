# Comparing `tmp/pyqldb-3.2.2.tar.gz` & `tmp/pyqldb-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqldb-3.2.2.tar", last modified: Thu Oct 28 18:27:04 2021, max compression
+gzip compressed data, was "pyqldb-3.2.3.tar", last modified: Wed May 24 11:38:18 2023, max compression
```

## Comparing `pyqldb-3.2.2.tar` & `pyqldb-3.2.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 guyilin  (1142257502) staff       (20)        0 2021-10-28 18:27:04.772288 pyqldb-3.2.2/
--rw-r--r--   0 guyilin  (1142257502) staff       (20)    10141 2021-10-28 18:15:58.000000 pyqldb-3.2.2/LICENSE
--rw-r--r--   0 guyilin  (1142257502) staff       (20)       72 2021-10-28 18:15:58.000000 pyqldb-3.2.2/NOTICE
--rw-r--r--   0 guyilin  (1142257502) staff       (20)     6491 2021-10-28 18:27:04.771889 pyqldb-3.2.2/PKG-INFO
--rw-r--r--   0 guyilin  (1142257502) staff       (20)     5923 2021-10-28 18:15:58.000000 pyqldb-3.2.2/README.md
-drwxr-xr-x   0 guyilin  (1142257502) staff       (20)        0 2021-10-28 18:27:04.754570 pyqldb-3.2.2/pyqldb/
--rw-r--r--   0 guyilin  (1142257502) staff       (20)      590 2021-10-28 18:15:58.000000 pyqldb-3.2.2/pyqldb/__init__.py
-drwxr-xr-x   0 guyilin  (1142257502) staff       (20)        0 2021-10-28 18:27:04.757531 pyqldb-3.2.2/pyqldb/communication/
--rw-r--r--   0 guyilin  (1142257502) staff       (20)      567 2021-10-28 18:15:58.000000 pyqldb-3.2.2/pyqldb/communication/__init__.py
--rw-r--r--   0 guyilin  (1142257502) staff       (20)     8261 2021-10-28 18:15:58.000000 pyqldb-3.2.2/pyqldb/communication/session_client.py
-drwxr-xr-x   0 guyilin  (1142257502) staff       (20)        0 2021-10-28 18:27:04.759500 pyqldb-3.2.2/pyqldb/config/
--rw-r--r--   0 guyilin  (1142257502) staff       (20)      562 2021-10-28 18:15:58.000000 pyqldb-3.2.2/pyqldb/config/__init__.py
--rw-r--r--   0 guyilin  (1142257502) staff       (20)     3123 2021-10-28 18:15:58.000000 pyqldb-3.2.2/pyqldb/config/retry_config.py
-drwxr-xr-x   0 guyilin  (1142257502) staff       (20)        0 2021-10-28 18:27:04.765013 pyqldb-3.2.2/pyqldb/cursor/
--rw-r--r--   0 guyilin  (1142257502) staff       (20)      567 2021-10-28 18:15:58.000000 pyqldb-3.2.2/pyqldb/cursor/__init__.py
--rw-r--r--   0 guyilin  (1142257502) staff       (20)     2326 2021-10-28 18:15:58.000000 pyqldb-3.2.2/pyqldb/cursor/buffered_cursor.py
--rw-r--r--   0 guyilin  (1142257502) staff       (20)     4147 2021-10-28 18:15:58.000000 pyqldb-3.2.2/pyqldb/cursor/read_ahead_cursor.py
--rw-r--r--   0 guyilin  (1142257502) staff       (20)     5825 2021-10-28 18:15:58.000000 pyqldb-3.2.2/pyqldb/cursor/stream_cursor.py
-drwxr-xr-x   0 guyilin  (1142257502) staff       (20)        0 2021-10-28 18:27:04.765859 pyqldb-3.2.2/pyqldb/driver/
--rw-r--r--   0 guyilin  (1142257502) staff       (20)      567 2021-10-28 18:15:58.000000 pyqldb-3.2.2/pyqldb/driver/__init__.py
--rw-r--r--   0 guyilin  (1142257502) staff       (20)    16772 2021-10-28 18:15:58.000000 pyqldb-3.2.2/pyqldb/driver/qldb_driver.py
-drwxr-xr-x   0 guyilin  (1142257502) staff       (20)        0 2021-10-28 18:27:04.766375 pyqldb-3.2.2/pyqldb/errors/
--rw-r--r--   0 guyilin  (1142257502) staff       (20)     5561 2021-10-28 18:15:58.000000 pyqldb-3.2.2/pyqldb/errors/__init__.py
-drwxr-xr-x   0 guyilin  (1142257502) staff       (20)        0 2021-10-28 18:27:04.767714 pyqldb-3.2.2/pyqldb/execution/
--rw-r--r--   0 guyilin  (1142257502) staff       (20)      562 2021-10-28 18:15:58.000000 pyqldb-3.2.2/pyqldb/execution/__init__.py
--rw-r--r--   0 guyilin  (1142257502) staff       (20)     1409 2021-10-28 18:15:58.000000 pyqldb-3.2.2/pyqldb/execution/executable.py
--rw-r--r--   0 guyilin  (1142257502) staff       (20)     2154 2021-10-28 18:15:58.000000 pyqldb-3.2.2/pyqldb/execution/executor.py
-drwxr-xr-x   0 guyilin  (1142257502) staff       (20)        0 2021-10-28 18:27:04.768627 pyqldb-3.2.2/pyqldb/session/
--rw-r--r--   0 guyilin  (1142257502) staff       (20)      567 2021-10-28 18:15:58.000000 pyqldb-3.2.2/pyqldb/session/__init__.py
--rw-r--r--   0 guyilin  (1142257502) staff       (20)     6383 2021-10-28 18:15:58.000000 pyqldb-3.2.2/pyqldb/session/qldb_session.py
-drwxr-xr-x   0 guyilin  (1142257502) staff       (20)        0 2021-10-28 18:27:04.769552 pyqldb-3.2.2/pyqldb/transaction/
--rw-r--r--   0 guyilin  (1142257502) staff       (20)      567 2021-10-28 18:15:58.000000 pyqldb-3.2.2/pyqldb/transaction/__init__.py
--rw-r--r--   0 guyilin  (1142257502) staff       (20)     5620 2021-10-28 18:15:58.000000 pyqldb-3.2.2/pyqldb/transaction/transaction.py
-drwxr-xr-x   0 guyilin  (1142257502) staff       (20)        0 2021-10-28 18:27:04.771138 pyqldb-3.2.2/pyqldb/util/
--rw-r--r--   0 guyilin  (1142257502) staff       (20)      567 2021-10-28 18:15:58.000000 pyqldb-3.2.2/pyqldb/util/__init__.py
--rw-r--r--   0 guyilin  (1142257502) staff       (20)     1495 2021-10-28 18:15:58.000000 pyqldb-3.2.2/pyqldb/util/atomic_integer.py
--rw-r--r--   0 guyilin  (1142257502) staff       (20)     3790 2021-10-28 18:15:58.000000 pyqldb-3.2.2/pyqldb/util/qldb_hash.py
--rw-r--r--   0 guyilin  (1142257502) staff       (20)     1503 2021-10-28 18:15:58.000000 pyqldb-3.2.2/pyqldb/util/retry.py
-drwxr-xr-x   0 guyilin  (1142257502) staff       (20)        0 2021-10-28 18:27:04.756534 pyqldb-3.2.2/pyqldb.egg-info/
--rw-r--r--   0 guyilin  (1142257502) staff       (20)     6491 2021-10-28 18:27:04.000000 pyqldb-3.2.2/pyqldb.egg-info/PKG-INFO
--rw-r--r--   0 guyilin  (1142257502) staff       (20)      847 2021-10-28 18:27:04.000000 pyqldb-3.2.2/pyqldb.egg-info/SOURCES.txt
--rw-r--r--   0 guyilin  (1142257502) staff       (20)        1 2021-10-28 18:27:04.000000 pyqldb-3.2.2/pyqldb.egg-info/dependency_links.txt
--rw-r--r--   0 guyilin  (1142257502) staff       (20)       76 2021-10-28 18:27:04.000000 pyqldb-3.2.2/pyqldb.egg-info/requires.txt
--rw-r--r--   0 guyilin  (1142257502) staff       (20)        7 2021-10-28 18:27:04.000000 pyqldb-3.2.2/pyqldb.egg-info/top_level.txt
--rw-r--r--   0 guyilin  (1142257502) staff       (20)       38 2021-10-28 18:27:04.772412 pyqldb-3.2.2/setup.cfg
--rw-r--r--   0 guyilin  (1142257502) staff       (20)     1665 2021-10-28 18:15:58.000000 pyqldb-3.2.2/setup.py
+drwxr-xr-x   0 batteson   (504) staff       (20)        0 2023-05-24 11:38:18.993319 pyqldb-3.2.3/
+-rw-r--r--   0 batteson   (504) staff       (20)    10141 2022-11-24 12:16:35.000000 pyqldb-3.2.3/LICENSE
+-rw-r--r--   0 batteson   (504) staff       (20)       72 2022-11-24 12:16:35.000000 pyqldb-3.2.3/NOTICE
+-rw-r--r--   0 batteson   (504) staff       (20)     6629 2023-05-24 11:38:18.993175 pyqldb-3.2.3/PKG-INFO
+-rw-r--r--   0 batteson   (504) staff       (20)     6100 2023-03-24 09:43:15.000000 pyqldb-3.2.3/README.md
+drwxr-xr-x   0 batteson   (504) staff       (20)        0 2023-05-24 11:38:18.989116 pyqldb-3.2.3/pyqldb/
+-rw-r--r--   0 batteson   (504) staff       (20)      590 2023-05-24 11:32:41.000000 pyqldb-3.2.3/pyqldb/__init__.py
+drwxr-xr-x   0 batteson   (504) staff       (20)        0 2023-05-24 11:38:18.990038 pyqldb-3.2.3/pyqldb/communication/
+-rw-r--r--   0 batteson   (504) staff       (20)      567 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/communication/__init__.py
+-rw-r--r--   0 batteson   (504) staff       (20)     8261 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/communication/session_client.py
+drwxr-xr-x   0 batteson   (504) staff       (20)        0 2023-05-24 11:38:18.990300 pyqldb-3.2.3/pyqldb/config/
+-rw-r--r--   0 batteson   (504) staff       (20)      562 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/config/__init__.py
+-rw-r--r--   0 batteson   (504) staff       (20)     3123 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/config/retry_config.py
+drwxr-xr-x   0 batteson   (504) staff       (20)        0 2023-05-24 11:38:18.990834 pyqldb-3.2.3/pyqldb/cursor/
+-rw-r--r--   0 batteson   (504) staff       (20)      567 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/cursor/__init__.py
+-rw-r--r--   0 batteson   (504) staff       (20)     2326 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/cursor/buffered_cursor.py
+-rw-r--r--   0 batteson   (504) staff       (20)     4147 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/cursor/read_ahead_cursor.py
+-rw-r--r--   0 batteson   (504) staff       (20)     5825 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/cursor/stream_cursor.py
+drwxr-xr-x   0 batteson   (504) staff       (20)        0 2023-05-24 11:38:18.991090 pyqldb-3.2.3/pyqldb/driver/
+-rw-r--r--   0 batteson   (504) staff       (20)      567 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/driver/__init__.py
+-rw-r--r--   0 batteson   (504) staff       (20)    16772 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/driver/qldb_driver.py
+drwxr-xr-x   0 batteson   (504) staff       (20)        0 2023-05-24 11:38:18.991266 pyqldb-3.2.3/pyqldb/errors/
+-rw-r--r--   0 batteson   (504) staff       (20)     5561 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/errors/__init__.py
+drwxr-xr-x   0 batteson   (504) staff       (20)        0 2023-05-24 11:38:18.991702 pyqldb-3.2.3/pyqldb/execution/
+-rw-r--r--   0 batteson   (504) staff       (20)      562 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/execution/__init__.py
+-rw-r--r--   0 batteson   (504) staff       (20)     1409 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/execution/executable.py
+-rw-r--r--   0 batteson   (504) staff       (20)     2154 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/execution/executor.py
+drwxr-xr-x   0 batteson   (504) staff       (20)        0 2023-05-24 11:38:18.992135 pyqldb-3.2.3/pyqldb/session/
+-rw-r--r--   0 batteson   (504) staff       (20)      567 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/session/__init__.py
+-rw-r--r--   0 batteson   (504) staff       (20)     6383 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/session/qldb_session.py
+drwxr-xr-x   0 batteson   (504) staff       (20)        0 2023-05-24 11:38:18.992415 pyqldb-3.2.3/pyqldb/transaction/
+-rw-r--r--   0 batteson   (504) staff       (20)      567 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/transaction/__init__.py
+-rw-r--r--   0 batteson   (504) staff       (20)     5620 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/transaction/transaction.py
+drwxr-xr-x   0 batteson   (504) staff       (20)        0 2023-05-24 11:38:18.992972 pyqldb-3.2.3/pyqldb/util/
+-rw-r--r--   0 batteson   (504) staff       (20)      567 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/util/__init__.py
+-rw-r--r--   0 batteson   (504) staff       (20)     1495 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/util/atomic_integer.py
+-rw-r--r--   0 batteson   (504) staff       (20)     3790 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/util/qldb_hash.py
+-rw-r--r--   0 batteson   (504) staff       (20)     1503 2022-11-24 12:16:35.000000 pyqldb-3.2.3/pyqldb/util/retry.py
+drwxr-xr-x   0 batteson   (504) staff       (20)        0 2023-05-24 11:38:18.989782 pyqldb-3.2.3/pyqldb.egg-info/
+-rw-r--r--   0 batteson   (504) staff       (20)     6629 2023-05-24 11:38:18.000000 pyqldb-3.2.3/pyqldb.egg-info/PKG-INFO
+-rw-r--r--   0 batteson   (504) staff       (20)      847 2023-05-24 11:38:18.000000 pyqldb-3.2.3/pyqldb.egg-info/SOURCES.txt
+-rw-r--r--   0 batteson   (504) staff       (20)        1 2023-05-24 11:38:18.000000 pyqldb-3.2.3/pyqldb.egg-info/dependency_links.txt
+-rw-r--r--   0 batteson   (504) staff       (20)       81 2023-05-24 11:38:18.000000 pyqldb-3.2.3/pyqldb.egg-info/requires.txt
+-rw-r--r--   0 batteson   (504) staff       (20)        7 2023-05-24 11:38:18.000000 pyqldb-3.2.3/pyqldb.egg-info/top_level.txt
+-rw-r--r--   0 batteson   (504) staff       (20)       38 2023-05-24 11:38:18.993358 pyqldb-3.2.3/setup.cfg
+-rw-r--r--   0 batteson   (504) staff       (20)     1670 2023-05-24 11:26:56.000000 pyqldb-3.2.3/setup.py
```

### Comparing `pyqldb-3.2.2/LICENSE` & `pyqldb-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.2/PKG-INFO` & `pyqldb-3.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 Metadata-Version: 2.1
 Name: pyqldb
-Version: 3.2.2
+Version: 3.2.3
 Summary: Python driver for Amazon QLDB
-Home-page: UNKNOWN
 Author: Amazon Web Services
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # Amazon QLDB Python Driver
 
-This is the Python driver for [Amazon Quantum Ledger Database (QLDB)](https://aws.amazon.com/qldb/), which allows Python developers
-to write software that makes use of AmazonQLDB.
-
 [![Latest Version](https://img.shields.io/pypi/v/pyqldb.svg)](https://pypi.python.org/pypi/pyqldb)
 [![Documentation Status](https://readthedocs.org/projects/amazon-qldb-driver-python/badge/?version=latest)](https://amazon-qldb-driver-python.readthedocs.io/en/latest/?badge=latest)
 [![Build Status](https://github.com/awslabs/amazon-qldb-driver-python/workflows/Python%20application/badge.svg)](https://github.com/awslabs/amazon-qldb-driver-python/actions?query=workflow%3A%22Python+application%22)
 [![license](https://img.shields.io/badge/license-Apache%202.0-blue)](https://github.com/awslabs/amazon-qldb-driver-python/blob/master/LICENSE)
 [![AWS Provider](https://img.shields.io/badge/provider-AWS-orange?logo=amazon-aws&color=ff9900)](https://aws.amazon.com/qldb/)
 
-For our tutorial, see [Python and Amazon QLDB](https://docs.aws.amazon.com/qldb/latest/developerguide/getting-started.python.html).
+This is the Python driver for [Amazon Quantum Ledger Database (QLDB)](https://aws.amazon.com/qldb/), which allows Python developers
+to write software that makes use of Amazon QLDB.
 
+For getting started with the driver, see [Python and Amazon QLDB](https://docs.aws.amazon.com/qldb/latest/developerguide/getting-started.python.html).
 ## Requirements
 
 ### Basic Configuration
 
 See [Accessing Amazon QLDB](https://docs.aws.amazon.com/qldb/latest/developerguide/accessing.html) for information on connecting to AWS.
 
 ### Required Python versions
@@ -43,14 +40,16 @@
 
 Please see the link below for more detail to install Python:
 
 * [Python Installation](https://www.python.org/downloads/)
 
 ## Getting Started
 
+Please see the [Quickstart guide for the Amazon QLDB Driver for Python](https://docs.aws.amazon.com/qldb/latest/developerguide/driver-quickstart-python.html).
+
 First, install the driver using pip:
 
 ```pip install pyqldb```
 
 
 Then from a Python interpreter, call the driver and specify the ledger name:
 
@@ -99,37 +98,35 @@
 ```
 
 You can run the integration tests with this command:
 ```
 $ pytest tests/integration
 ```
 
+### Documentation 
+
+Sphinx is used for documentation. You can generate HTML locally with the following:
+
+```
+$ pip install -r requirements-docs.txt
+$ pip install -e .
+$ cd docs
+$ make html
+```
+
 ## Getting Help
 
 Please use these community resources for getting help.
 * Ask a question on StackOverflow and tag it with the [amazon-qldb](https://stackoverflow.com/questions/tagged/amazon-qldb) tag.
 * Open a support ticket with [AWS Support](http://docs.aws.amazon.com/awssupport/latest/user/getting-started.html).
 * Make a new thread at [AWS QLDB Forum](https://forums.aws.amazon.com/forum.jspa?forumID=353&start=0).
 * If you think you may have found a bug, please open an [issue](https://github.com/awslabs/amazon-qldb-driver-python/issues/new).
 
 ## Opening Issues
 
-If you encounter a bug with the Amazon QLDB Python Driver, we would like to hear about it. Please search the [existing issues](https://github.com/awslabs/amazon-qldb-driver-python/issues) and see if others are also experiencing the issue before opening a new issue. When opening a new issue, we will need the version of Amazon QLDB Python Driver, Python language version, and OS you’re using. Please also include reproduction case for the issue when appropriate.
+If you encounter a bug with the Amazon QLDB Python Driver, we would like to hear about it. Please search the [existing issues](https://github.com/awslabs/amazon-qldb-driver-python/issues) and see if others are also experiencing the issue before opening a new issue. When opening a new issue, we will need the version of Amazon QLDB Python Driver, Python language version, and OS you're using. Please also include reproduction case for the issue when appropriate.
 
 The GitHub issues are intended for bug reports and feature requests. For help and questions with using Amazon QLDB Python Driver, please make use of the resources listed in the [Getting Help](https://github.com/awslabs/amazon-qldb-driver-python#getting-help) section. Keeping the list of open issues lean will help us respond in a timely manner.
 
-### Documentation 
-
-Sphinx is used for documentation. You can generate HTML locally with the following:
-
-```
-$ pip install -r requirements-docs.txt
-$ pip install -e .
-$ cd docs
-$ make html
-```
-
 ## License
 
 This library is licensed under the Apache 2.0 License.
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyqldb-3.2.2/README.md` & `pyqldb-3.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # Amazon QLDB Python Driver
 
-This is the Python driver for [Amazon Quantum Ledger Database (QLDB)](https://aws.amazon.com/qldb/), which allows Python developers
-to write software that makes use of AmazonQLDB.
-
 [![Latest Version](https://img.shields.io/pypi/v/pyqldb.svg)](https://pypi.python.org/pypi/pyqldb)
 [![Documentation Status](https://readthedocs.org/projects/amazon-qldb-driver-python/badge/?version=latest)](https://amazon-qldb-driver-python.readthedocs.io/en/latest/?badge=latest)
 [![Build Status](https://github.com/awslabs/amazon-qldb-driver-python/workflows/Python%20application/badge.svg)](https://github.com/awslabs/amazon-qldb-driver-python/actions?query=workflow%3A%22Python+application%22)
 [![license](https://img.shields.io/badge/license-Apache%202.0-blue)](https://github.com/awslabs/amazon-qldb-driver-python/blob/master/LICENSE)
 [![AWS Provider](https://img.shields.io/badge/provider-AWS-orange?logo=amazon-aws&color=ff9900)](https://aws.amazon.com/qldb/)
 
-For our tutorial, see [Python and Amazon QLDB](https://docs.aws.amazon.com/qldb/latest/developerguide/getting-started.python.html).
+This is the Python driver for [Amazon Quantum Ledger Database (QLDB)](https://aws.amazon.com/qldb/), which allows Python developers
+to write software that makes use of Amazon QLDB.
 
+For getting started with the driver, see [Python and Amazon QLDB](https://docs.aws.amazon.com/qldb/latest/developerguide/getting-started.python.html).
 ## Requirements
 
 ### Basic Configuration
 
 See [Accessing Amazon QLDB](https://docs.aws.amazon.com/qldb/latest/developerguide/accessing.html) for information on connecting to AWS.
 
 ### Required Python versions
@@ -25,14 +24,16 @@
 
 Please see the link below for more detail to install Python:
 
 * [Python Installation](https://www.python.org/downloads/)
 
 ## Getting Started
 
+Please see the [Quickstart guide for the Amazon QLDB Driver for Python](https://docs.aws.amazon.com/qldb/latest/developerguide/driver-quickstart-python.html).
+
 First, install the driver using pip:
 
 ```pip install pyqldb```
 
 
 Then from a Python interpreter, call the driver and specify the ledger name:
 
@@ -81,35 +82,35 @@
 ```
 
 You can run the integration tests with this command:
 ```
 $ pytest tests/integration
 ```
 
+### Documentation 
+
+Sphinx is used for documentation. You can generate HTML locally with the following:
+
+```
+$ pip install -r requirements-docs.txt
+$ pip install -e .
+$ cd docs
+$ make html
+```
+
 ## Getting Help
 
 Please use these community resources for getting help.
 * Ask a question on StackOverflow and tag it with the [amazon-qldb](https://stackoverflow.com/questions/tagged/amazon-qldb) tag.
 * Open a support ticket with [AWS Support](http://docs.aws.amazon.com/awssupport/latest/user/getting-started.html).
 * Make a new thread at [AWS QLDB Forum](https://forums.aws.amazon.com/forum.jspa?forumID=353&start=0).
 * If you think you may have found a bug, please open an [issue](https://github.com/awslabs/amazon-qldb-driver-python/issues/new).
 
 ## Opening Issues
 
-If you encounter a bug with the Amazon QLDB Python Driver, we would like to hear about it. Please search the [existing issues](https://github.com/awslabs/amazon-qldb-driver-python/issues) and see if others are also experiencing the issue before opening a new issue. When opening a new issue, we will need the version of Amazon QLDB Python Driver, Python language version, and OS you’re using. Please also include reproduction case for the issue when appropriate.
+If you encounter a bug with the Amazon QLDB Python Driver, we would like to hear about it. Please search the [existing issues](https://github.com/awslabs/amazon-qldb-driver-python/issues) and see if others are also experiencing the issue before opening a new issue. When opening a new issue, we will need the version of Amazon QLDB Python Driver, Python language version, and OS you're using. Please also include reproduction case for the issue when appropriate.
 
 The GitHub issues are intended for bug reports and feature requests. For help and questions with using Amazon QLDB Python Driver, please make use of the resources listed in the [Getting Help](https://github.com/awslabs/amazon-qldb-driver-python#getting-help) section. Keeping the list of open issues lean will help us respond in a timely manner.
 
-### Documentation 
-
-Sphinx is used for documentation. You can generate HTML locally with the following:
-
-```
-$ pip install -r requirements-docs.txt
-$ pip install -e .
-$ cd docs
-$ make html
-```
-
 ## License
 
 This library is licensed under the Apache 2.0 License.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyqldb-3.2.2/pyqldb/__init__.py` & `pyqldb-3.2.3/pyqldb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
 # CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions
 # and limitations under the License.
 
-__version__ = '3.2.2'
+__version__ = '3.2.3'
```

### Comparing `pyqldb-3.2.2/pyqldb/communication/__init__.py` & `pyqldb-3.2.3/pyqldb/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.2/pyqldb/communication/session_client.py` & `pyqldb-3.2.3/pyqldb/communication/session_client.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.2/pyqldb/config/__init__.py` & `pyqldb-3.2.3/pyqldb/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.2/pyqldb/config/retry_config.py` & `pyqldb-3.2.3/pyqldb/config/retry_config.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.2/pyqldb/cursor/__init__.py` & `pyqldb-3.2.3/pyqldb/cursor/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.2/pyqldb/cursor/buffered_cursor.py` & `pyqldb-3.2.3/pyqldb/cursor/buffered_cursor.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.2/pyqldb/cursor/read_ahead_cursor.py` & `pyqldb-3.2.3/pyqldb/cursor/read_ahead_cursor.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.2/pyqldb/cursor/stream_cursor.py` & `pyqldb-3.2.3/pyqldb/cursor/stream_cursor.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.2/pyqldb/driver/__init__.py` & `pyqldb-3.2.3/pyqldb/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.2/pyqldb/driver/qldb_driver.py` & `pyqldb-3.2.3/pyqldb/driver/qldb_driver.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.2/pyqldb/errors/__init__.py` & `pyqldb-3.2.3/pyqldb/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.2/pyqldb/execution/__init__.py` & `pyqldb-3.2.3/pyqldb/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.2/pyqldb/execution/executable.py` & `pyqldb-3.2.3/pyqldb/execution/executable.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.2/pyqldb/execution/executor.py` & `pyqldb-3.2.3/pyqldb/execution/executor.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.2/pyqldb/session/__init__.py` & `pyqldb-3.2.3/pyqldb/session/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.2/pyqldb/session/qldb_session.py` & `pyqldb-3.2.3/pyqldb/session/qldb_session.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.2/pyqldb/transaction/__init__.py` & `pyqldb-3.2.3/pyqldb/transaction/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.2/pyqldb/transaction/transaction.py` & `pyqldb-3.2.3/pyqldb/transaction/transaction.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.2/pyqldb/util/__init__.py` & `pyqldb-3.2.3/pyqldb/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.2/pyqldb/util/atomic_integer.py` & `pyqldb-3.2.3/pyqldb/util/atomic_integer.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.2/pyqldb/util/qldb_hash.py` & `pyqldb-3.2.3/pyqldb/util/qldb_hash.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.2/pyqldb/util/retry.py` & `pyqldb-3.2.3/pyqldb/util/retry.py`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.2/pyqldb.egg-info/PKG-INFO` & `pyqldb-3.2.3/pyqldb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 Metadata-Version: 2.1
 Name: pyqldb
-Version: 3.2.2
+Version: 3.2.3
 Summary: Python driver for Amazon QLDB
-Home-page: UNKNOWN
 Author: Amazon Web Services
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # Amazon QLDB Python Driver
 
-This is the Python driver for [Amazon Quantum Ledger Database (QLDB)](https://aws.amazon.com/qldb/), which allows Python developers
-to write software that makes use of AmazonQLDB.
-
 [![Latest Version](https://img.shields.io/pypi/v/pyqldb.svg)](https://pypi.python.org/pypi/pyqldb)
 [![Documentation Status](https://readthedocs.org/projects/amazon-qldb-driver-python/badge/?version=latest)](https://amazon-qldb-driver-python.readthedocs.io/en/latest/?badge=latest)
 [![Build Status](https://github.com/awslabs/amazon-qldb-driver-python/workflows/Python%20application/badge.svg)](https://github.com/awslabs/amazon-qldb-driver-python/actions?query=workflow%3A%22Python+application%22)
 [![license](https://img.shields.io/badge/license-Apache%202.0-blue)](https://github.com/awslabs/amazon-qldb-driver-python/blob/master/LICENSE)
 [![AWS Provider](https://img.shields.io/badge/provider-AWS-orange?logo=amazon-aws&color=ff9900)](https://aws.amazon.com/qldb/)
 
-For our tutorial, see [Python and Amazon QLDB](https://docs.aws.amazon.com/qldb/latest/developerguide/getting-started.python.html).
+This is the Python driver for [Amazon Quantum Ledger Database (QLDB)](https://aws.amazon.com/qldb/), which allows Python developers
+to write software that makes use of Amazon QLDB.
 
+For getting started with the driver, see [Python and Amazon QLDB](https://docs.aws.amazon.com/qldb/latest/developerguide/getting-started.python.html).
 ## Requirements
 
 ### Basic Configuration
 
 See [Accessing Amazon QLDB](https://docs.aws.amazon.com/qldb/latest/developerguide/accessing.html) for information on connecting to AWS.
 
 ### Required Python versions
@@ -43,14 +40,16 @@
 
 Please see the link below for more detail to install Python:
 
 * [Python Installation](https://www.python.org/downloads/)
 
 ## Getting Started
 
+Please see the [Quickstart guide for the Amazon QLDB Driver for Python](https://docs.aws.amazon.com/qldb/latest/developerguide/driver-quickstart-python.html).
+
 First, install the driver using pip:
 
 ```pip install pyqldb```
 
 
 Then from a Python interpreter, call the driver and specify the ledger name:
 
@@ -99,37 +98,35 @@
 ```
 
 You can run the integration tests with this command:
 ```
 $ pytest tests/integration
 ```
 
+### Documentation 
+
+Sphinx is used for documentation. You can generate HTML locally with the following:
+
+```
+$ pip install -r requirements-docs.txt
+$ pip install -e .
+$ cd docs
+$ make html
+```
+
 ## Getting Help
 
 Please use these community resources for getting help.
 * Ask a question on StackOverflow and tag it with the [amazon-qldb](https://stackoverflow.com/questions/tagged/amazon-qldb) tag.
 * Open a support ticket with [AWS Support](http://docs.aws.amazon.com/awssupport/latest/user/getting-started.html).
 * Make a new thread at [AWS QLDB Forum](https://forums.aws.amazon.com/forum.jspa?forumID=353&start=0).
 * If you think you may have found a bug, please open an [issue](https://github.com/awslabs/amazon-qldb-driver-python/issues/new).
 
 ## Opening Issues
 
-If you encounter a bug with the Amazon QLDB Python Driver, we would like to hear about it. Please search the [existing issues](https://github.com/awslabs/amazon-qldb-driver-python/issues) and see if others are also experiencing the issue before opening a new issue. When opening a new issue, we will need the version of Amazon QLDB Python Driver, Python language version, and OS you’re using. Please also include reproduction case for the issue when appropriate.
+If you encounter a bug with the Amazon QLDB Python Driver, we would like to hear about it. Please search the [existing issues](https://github.com/awslabs/amazon-qldb-driver-python/issues) and see if others are also experiencing the issue before opening a new issue. When opening a new issue, we will need the version of Amazon QLDB Python Driver, Python language version, and OS you're using. Please also include reproduction case for the issue when appropriate.
 
 The GitHub issues are intended for bug reports and feature requests. For help and questions with using Amazon QLDB Python Driver, please make use of the resources listed in the [Getting Help](https://github.com/awslabs/amazon-qldb-driver-python#getting-help) section. Keeping the list of open issues lean will help us respond in a timely manner.
 
-### Documentation 
-
-Sphinx is used for documentation. You can generate HTML locally with the following:
-
-```
-$ pip install -r requirements-docs.txt
-$ pip install -e .
-$ cd docs
-$ make html
-```
-
 ## License
 
 This library is licensed under the Apache 2.0 License.
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyqldb-3.2.2/pyqldb.egg-info/SOURCES.txt` & `pyqldb-3.2.3/pyqldb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyqldb-3.2.2/setup.py` & `pyqldb-3.2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # and limitations under the License.
 import os
 import re
 import setuptools
 
 ROOT = os.path.join(os.path.dirname(__file__), 'pyqldb')
 VERSION_RE = re.compile(r'''__version__ = ['"]([0-9.a-z\-]+)['"]''')
-requires = ['amazon.ion>=0.7.0,<1',
+requires = ['amazon.ion>=0.7.0,<=0.9.3',
             'boto3>=1.17.5,<2',
             'botocore>=1.20.5,<2',
             'ionhash>=1.2.1,<2']
 
 
 def get_version():
     init = open(os.path.join(ROOT, '__init__.py')).read()
```

