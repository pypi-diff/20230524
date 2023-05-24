# Comparing `tmp/mocksafe-0.4.1a0.tar.gz` & `tmp/mocksafe-0.5.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mocksafe-0.4.1a0.tar", last modified: Tue May 23 16:01:24 2023, max compression
+gzip compressed data, was "mocksafe-0.5.0a0.tar", last modified: Wed May 24 12:17:30 2023, max compression
```

## Comparing `mocksafe-0.4.1a0.tar` & `mocksafe-0.5.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-23 16:01:24.440817 mocksafe-0.4.1a0/
--rw-r--r--   0 danielmayo   (501) staff       (20)     1068 2023-05-08 16:33:22.000000 mocksafe-0.4.1a0/LICENSE
--rw-r--r--   0 danielmayo   (501) staff       (20)     4777 2023-05-23 16:01:24.440563 mocksafe-0.4.1a0/PKG-INFO
--rw-r--r--   0 danielmayo   (501) staff       (20)     2123 2023-05-23 15:56:21.000000 mocksafe-0.4.1a0/README.rst
-drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-23 16:01:24.430740 mocksafe-0.4.1a0/mocksafe/
--rw-r--r--   0 danielmayo   (501) staff       (20)      400 2023-05-23 15:56:21.000000 mocksafe-0.4.1a0/mocksafe/__init__.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     1165 2023-05-18 16:23:02.000000 mocksafe-0.4.1a0/mocksafe/call_matchers.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     6661 2023-05-23 15:54:53.000000 mocksafe-0.4.1a0/mocksafe/call_type_validator.py
--rw-r--r--   0 danielmayo   (501) staff       (20)      119 2023-05-16 16:52:33.000000 mocksafe-0.4.1a0/mocksafe/custom_types.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     5464 2023-05-23 15:54:53.000000 mocksafe-0.4.1a0/mocksafe/mock.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     1802 2023-05-23 15:54:53.000000 mocksafe-0.4.1a0/mocksafe/spy.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     3294 2023-05-23 15:54:53.000000 mocksafe-0.4.1a0/mocksafe/stub.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     4058 2023-05-18 16:23:02.000000 mocksafe-0.4.1a0/mocksafe/that.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     6464 2023-05-23 15:54:53.000000 mocksafe-0.4.1a0/mocksafe/when_then.py
-drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-23 16:01:24.439831 mocksafe-0.4.1a0/mocksafe.egg-info/
--rw-r--r--   0 danielmayo   (501) staff       (20)     4777 2023-05-23 16:01:24.000000 mocksafe-0.4.1a0/mocksafe.egg-info/PKG-INFO
--rw-r--r--   0 danielmayo   (501) staff       (20)      377 2023-05-23 16:01:24.000000 mocksafe-0.4.1a0/mocksafe.egg-info/SOURCES.txt
--rw-r--r--   0 danielmayo   (501) staff       (20)        1 2023-05-23 16:01:24.000000 mocksafe-0.4.1a0/mocksafe.egg-info/dependency_links.txt
--rw-r--r--   0 danielmayo   (501) staff       (20)        9 2023-05-23 16:01:24.000000 mocksafe-0.4.1a0/mocksafe.egg-info/top_level.txt
--rw-r--r--   0 danielmayo   (501) staff       (20)     1869 2023-05-23 15:56:21.000000 mocksafe-0.4.1a0/pyproject.toml
--rw-r--r--   0 danielmayo   (501) staff       (20)       38 2023-05-23 16:01:24.440875 mocksafe-0.4.1a0/setup.cfg
-drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-23 16:01:24.440194 mocksafe-0.4.1a0/tests/
--rw-r--r--   0 danielmayo   (501) staff       (20)     6118 2023-05-23 10:53:25.000000 mocksafe-0.4.1a0/tests/test_mocksafe.py
+drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-24 12:17:30.059701 mocksafe-0.5.0a0/
+-rw-r--r--   0 danielmayo   (501) staff       (20)     1068 2023-05-08 16:33:22.000000 mocksafe-0.5.0a0/LICENSE
+-rw-r--r--   0 danielmayo   (501) staff       (20)     4781 2023-05-24 12:17:30.059382 mocksafe-0.5.0a0/PKG-INFO
+-rw-r--r--   0 danielmayo   (501) staff       (20)     2119 2023-05-24 12:10:10.000000 mocksafe-0.5.0a0/README.rst
+drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-24 12:17:30.028707 mocksafe-0.5.0a0/mocksafe/
+-rw-r--r--   0 danielmayo   (501) staff       (20)      476 2023-05-24 12:06:58.000000 mocksafe-0.5.0a0/mocksafe/__init__.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     1165 2023-05-18 16:23:02.000000 mocksafe-0.5.0a0/mocksafe/call_matchers.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     6661 2023-05-23 15:54:53.000000 mocksafe-0.5.0a0/mocksafe/call_type_validator.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)      119 2023-05-16 16:52:33.000000 mocksafe-0.5.0a0/mocksafe/custom_types.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     7520 2023-05-24 12:05:28.000000 mocksafe-0.5.0a0/mocksafe/mock.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     1802 2023-05-23 15:54:53.000000 mocksafe-0.5.0a0/mocksafe/spy.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     3294 2023-05-24 05:50:09.000000 mocksafe-0.5.0a0/mocksafe/stub.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     4058 2023-05-18 16:23:02.000000 mocksafe-0.5.0a0/mocksafe/that.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     6464 2023-05-23 15:54:53.000000 mocksafe-0.5.0a0/mocksafe/when_then.py
+drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-24 12:17:30.057428 mocksafe-0.5.0a0/mocksafe.egg-info/
+-rw-r--r--   0 danielmayo   (501) staff       (20)     4781 2023-05-24 12:17:29.000000 mocksafe-0.5.0a0/mocksafe.egg-info/PKG-INFO
+-rw-r--r--   0 danielmayo   (501) staff       (20)      377 2023-05-24 12:17:29.000000 mocksafe-0.5.0a0/mocksafe.egg-info/SOURCES.txt
+-rw-r--r--   0 danielmayo   (501) staff       (20)        1 2023-05-24 12:17:29.000000 mocksafe-0.5.0a0/mocksafe.egg-info/dependency_links.txt
+-rw-r--r--   0 danielmayo   (501) staff       (20)        9 2023-05-24 12:17:29.000000 mocksafe-0.5.0a0/mocksafe.egg-info/top_level.txt
+-rw-r--r--   0 danielmayo   (501) staff       (20)     1877 2023-05-24 12:08:50.000000 mocksafe-0.5.0a0/pyproject.toml
+-rw-r--r--   0 danielmayo   (501) staff       (20)       38 2023-05-24 12:17:30.059771 mocksafe-0.5.0a0/setup.cfg
+drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-24 12:17:30.058924 mocksafe-0.5.0a0/tests/
+-rw-r--r--   0 danielmayo   (501) staff       (20)     6604 2023-05-24 12:05:28.000000 mocksafe-0.5.0a0/tests/test_mocksafe.py
```

### Comparing `mocksafe-0.4.1a0/LICENSE` & `mocksafe-0.5.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `mocksafe-0.4.1a0/PKG-INFO` & `mocksafe-0.5.0a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocksafe
-Version: 0.4.1a0
+Version: 0.5.0a0
 Summary: A mocking library developed to enable static and runtime type checking of your mocks to keep them in sync with production code.
 License: MIT License
         
         Copyright (c) 2023 Daniel Mayo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -20,15 +20,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Documentation, https://mocksafe.readthedocs.io
+Project-URL: Documentation, https://mocksafe.readthedocs.io/en/0.5/
 Project-URL: Source, https://github.com/dmayo3/mocksafe
 Keywords: mock,mocking,typed,typing,typesafe,testing,tests,mocks,magicmock,unittest,stubbing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -51,16 +51,16 @@
 License-File: LICENSE
 
 .. image:: https://github.com/dmayo3/mocksafe/actions/workflows/mocksafe.yml/badge.svg
     :target: https://github.com/dmayo3/mocksafe/actions/workflows/mocksafe.yml?query=branch%3Amain
     :alt: Github Actions Status
 .. image:: https://codecov.io/gh/dmayo3/mocksafe/branch/main/graph/badge.svg?token=S3JI6OOTGF 
     :target: https://codecov.io/gh/dmayo3/mocksafe
-.. image:: https://readthedocs.org/projects/mocksafe/badge/?version=latest
-    :target: https://mocksafe.readthedocs.io/en/latest/?badge=latest
+.. image:: https://readthedocs.org/projects/mocksafe/badge/?version=0.5
+    :target: https://mocksafe.readthedocs.io/en/0.5/?badge=0.5
     :alt: Documentation Status
 .. image:: https://badge.fury.io/py/mocksafe.svg
     :target: https://badge.fury.io/py/mocksafe
     :alt: PyPI Package
 .. image:: https://img.shields.io/pypi/pyversions/mocksafe.svg
     :target: https://pypi.org/project/mocksafe
     :alt: Supported versions
@@ -70,15 +70,15 @@
 .. image:: http://www.mypy-lang.org/static/mypy_badge.svg
     :target: http://mypy-lang.org/
     :alt: Type checked by mypy
 .. image:: https://img.shields.io/badge/License-MIT-green.svg
     :target: https://github.com/dmayo3/mocksafe/blob/main/LICENSE
     :alt: MIT License
 
-MockSafe v0.4.1-alpha
+MockSafe v0.5.0-alpha
 ---------------------
 
 A mocking library developed to enable static and runtime type checking of your mocks to help keep them up-to-date with your production code.
 
 It has a simple, fluent API and is designed to be used with Python's `assert` statement.
 
 Checkout the docs link below for more information.
@@ -86,18 +86,18 @@
 Install and quickstart
 ----------------------
 
 ::
 
     pip install mocksafe
 
-`Library Usage <https://mocksafe.readthedocs.io/en/latest/usage.html>`_
+`Library Usage <https://mocksafe.readthedocs.io/en/0.5/usage.html>`_
 
 Links
 ----------------------
 
 :Install: `PyPi <https://pypi.org/project/mocksafe>`_
-:Docs:    `Read The Docs <https://mocksafe.readthedocs.io>`_
+:Docs:    `Read The Docs <https://mocksafe.readthedocs.io/en/0.5/>`_
 :License: `MIT <https://github.com/dmayo3/mocksafe/blob/main/LICENSE>`_
 :Source:  `GitHub <https://github.com/dmayo3/mocksafe>`_
 :Issues:  `GitHub Issues <https://github.com/dmayo3/mocksafe/issues>`_
 :Discussion:  `Questions & Feedback <https://github.com/dmayo3/mocksafe/discussions>`_
```

### Comparing `mocksafe-0.4.1a0/README.rst` & `mocksafe-0.5.0a0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. image:: https://github.com/dmayo3/mocksafe/actions/workflows/mocksafe.yml/badge.svg
     :target: https://github.com/dmayo3/mocksafe/actions/workflows/mocksafe.yml?query=branch%3Amain
     :alt: Github Actions Status
 .. image:: https://codecov.io/gh/dmayo3/mocksafe/branch/main/graph/badge.svg?token=S3JI6OOTGF 
     :target: https://codecov.io/gh/dmayo3/mocksafe
-.. image:: https://readthedocs.org/projects/mocksafe/badge/?version=latest
-    :target: https://mocksafe.readthedocs.io/en/latest/?badge=latest
+.. image:: https://readthedocs.org/projects/mocksafe/badge/?version=0.5
+    :target: https://mocksafe.readthedocs.io/en/0.5/?badge=0.5
     :alt: Documentation Status
 .. image:: https://badge.fury.io/py/mocksafe.svg
     :target: https://badge.fury.io/py/mocksafe
     :alt: PyPI Package
 .. image:: https://img.shields.io/pypi/pyversions/mocksafe.svg
     :target: https://pypi.org/project/mocksafe
     :alt: Supported versions
@@ -18,15 +18,15 @@
 .. image:: http://www.mypy-lang.org/static/mypy_badge.svg
     :target: http://mypy-lang.org/
     :alt: Type checked by mypy
 .. image:: https://img.shields.io/badge/License-MIT-green.svg
     :target: https://github.com/dmayo3/mocksafe/blob/main/LICENSE
     :alt: MIT License
 
-MockSafe v0.4.1-alpha
+MockSafe v0.5.0-alpha
 ---------------------
 
 A mocking library developed to enable static and runtime type checking of your mocks to help keep them up-to-date with your production code.
 
 It has a simple, fluent API and is designed to be used with Python's `assert` statement.
 
 Checkout the docs link below for more information.
@@ -34,18 +34,18 @@
 Install and quickstart
 ----------------------
 
 ::
 
     pip install mocksafe
 
-`Library Usage <https://mocksafe.readthedocs.io/en/latest/usage.html>`_
+`Library Usage <https://mocksafe.readthedocs.io/en/0.5/usage.html>`_
 
 Links
 ----------------------
 
 :Install: `PyPi <https://pypi.org/project/mocksafe>`_
-:Docs:    `Read The Docs <https://mocksafe.readthedocs.io>`_
+:Docs:    `Read The Docs <https://mocksafe.readthedocs.io/en/0.5/>`_
 :License: `MIT <https://github.com/dmayo3/mocksafe/blob/main/LICENSE>`_
 :Source:  `GitHub <https://github.com/dmayo3/mocksafe>`_
 :Issues:  `GitHub Issues <https://github.com/dmayo3/mocksafe/issues>`_
 :Discussion:  `Questions & Feedback <https://github.com/dmayo3/mocksafe/discussions>`_
```

### Comparing `mocksafe-0.4.1a0/mocksafe/call_matchers.py` & `mocksafe-0.5.0a0/mocksafe/call_matchers.py`

 * *Files identical despite different names*

### Comparing `mocksafe-0.4.1a0/mocksafe/call_type_validator.py` & `mocksafe-0.5.0a0/mocksafe/call_type_validator.py`

 * *Files identical despite different names*

### Comparing `mocksafe-0.4.1a0/mocksafe/spy.py` & `mocksafe-0.5.0a0/mocksafe/spy.py`

 * *Files identical despite different names*

### Comparing `mocksafe-0.4.1a0/mocksafe/stub.py` & `mocksafe-0.5.0a0/mocksafe/stub.py`

 * *Files identical despite different names*

### Comparing `mocksafe-0.4.1a0/mocksafe/that.py` & `mocksafe-0.5.0a0/mocksafe/that.py`

 * *Files identical despite different names*

### Comparing `mocksafe-0.4.1a0/mocksafe/when_then.py` & `mocksafe-0.5.0a0/mocksafe/when_then.py`

 * *Files identical despite different names*

### Comparing `mocksafe-0.4.1a0/mocksafe.egg-info/PKG-INFO` & `mocksafe-0.5.0a0/mocksafe.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocksafe
-Version: 0.4.1a0
+Version: 0.5.0a0
 Summary: A mocking library developed to enable static and runtime type checking of your mocks to keep them in sync with production code.
 License: MIT License
         
         Copyright (c) 2023 Daniel Mayo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -20,15 +20,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Documentation, https://mocksafe.readthedocs.io
+Project-URL: Documentation, https://mocksafe.readthedocs.io/en/0.5/
 Project-URL: Source, https://github.com/dmayo3/mocksafe
 Keywords: mock,mocking,typed,typing,typesafe,testing,tests,mocks,magicmock,unittest,stubbing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -51,16 +51,16 @@
 License-File: LICENSE
 
 .. image:: https://github.com/dmayo3/mocksafe/actions/workflows/mocksafe.yml/badge.svg
     :target: https://github.com/dmayo3/mocksafe/actions/workflows/mocksafe.yml?query=branch%3Amain
     :alt: Github Actions Status
 .. image:: https://codecov.io/gh/dmayo3/mocksafe/branch/main/graph/badge.svg?token=S3JI6OOTGF 
     :target: https://codecov.io/gh/dmayo3/mocksafe
-.. image:: https://readthedocs.org/projects/mocksafe/badge/?version=latest
-    :target: https://mocksafe.readthedocs.io/en/latest/?badge=latest
+.. image:: https://readthedocs.org/projects/mocksafe/badge/?version=0.5
+    :target: https://mocksafe.readthedocs.io/en/0.5/?badge=0.5
     :alt: Documentation Status
 .. image:: https://badge.fury.io/py/mocksafe.svg
     :target: https://badge.fury.io/py/mocksafe
     :alt: PyPI Package
 .. image:: https://img.shields.io/pypi/pyversions/mocksafe.svg
     :target: https://pypi.org/project/mocksafe
     :alt: Supported versions
@@ -70,15 +70,15 @@
 .. image:: http://www.mypy-lang.org/static/mypy_badge.svg
     :target: http://mypy-lang.org/
     :alt: Type checked by mypy
 .. image:: https://img.shields.io/badge/License-MIT-green.svg
     :target: https://github.com/dmayo3/mocksafe/blob/main/LICENSE
     :alt: MIT License
 
-MockSafe v0.4.1-alpha
+MockSafe v0.5.0-alpha
 ---------------------
 
 A mocking library developed to enable static and runtime type checking of your mocks to help keep them up-to-date with your production code.
 
 It has a simple, fluent API and is designed to be used with Python's `assert` statement.
 
 Checkout the docs link below for more information.
@@ -86,18 +86,18 @@
 Install and quickstart
 ----------------------
 
 ::
 
     pip install mocksafe
 
-`Library Usage <https://mocksafe.readthedocs.io/en/latest/usage.html>`_
+`Library Usage <https://mocksafe.readthedocs.io/en/0.5/usage.html>`_
 
 Links
 ----------------------
 
 :Install: `PyPi <https://pypi.org/project/mocksafe>`_
-:Docs:    `Read The Docs <https://mocksafe.readthedocs.io>`_
+:Docs:    `Read The Docs <https://mocksafe.readthedocs.io/en/0.5/>`_
 :License: `MIT <https://github.com/dmayo3/mocksafe/blob/main/LICENSE>`_
 :Source:  `GitHub <https://github.com/dmayo3/mocksafe>`_
 :Issues:  `GitHub Issues <https://github.com/dmayo3/mocksafe/issues>`_
 :Discussion:  `Questions & Feedback <https://github.com/dmayo3/mocksafe/discussions>`_
```

### Comparing `mocksafe-0.4.1a0/pyproject.toml` & `mocksafe-0.5.0a0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mocksafe"
-version = "0.4.1-alpha"
+version = "0.5.0-alpha"
 
 description = "A mocking library developed to enable static and runtime type checking of your mocks to keep them in sync with production code."
 
 requires-python = ">= 3.9"
 readme = "README.rst"
 license = { file = "LICENSE" }
 classifiers = [
@@ -28,23 +28,23 @@
     "Framework :: Pytest",
     "Typing :: Typed",
 ]
 keywords = ["mock", "mocking", "typed", "typing", "typesafe", "testing", "tests", "mocks", "magicmock", "unittest", "stubbing"]
 dependencies = []
 
 [project.urls]
-Documentation = "https://mocksafe.readthedocs.io"
+Documentation = "https://mocksafe.readthedocs.io/en/0.5/"
 Source = "https://github.com/dmayo3/mocksafe"
 
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools", "wheel"]
 
 [tool.bumpver]
-current_version = "0.4.1-alpha"
+current_version = "0.5.0-alpha"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `mocksafe-0.4.1a0/tests/test_mocksafe.py` & `mocksafe-0.5.0a0/tests/test_mocksafe.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from random import Random
+import random
+from types import ModuleType
 from typing import Optional
 import pytest
-from mocksafe import mock, when, that, spy
+from mocksafe import mock, mock_module, when, that, spy
 
 
 class MyClass:
     def foo(self, bar: str, baz: int = 123) -> int:
         return baz + len(bar)
 
     def quux(self) -> Optional[str]:
@@ -229,12 +230,29 @@
     assert mock_object.foo("a") == 5
     assert mock_object.foo("b") == 10
     with pytest.raises(ValueError):
         mock_object.foo("c")
 
 
 def test_mock_random_class():
-    mock_random: Random = mock(Random)
+    mock_random: random.Random = mock(random.Random)
 
     when(mock_random.random).any_call().then_return(0.123)
 
     assert mock_random.random() == 0.123
+
+
+def test_mock_random_module():
+    mock_random = mock_module(random)
+
+    assert isinstance(mock_random, ModuleType)
+
+    when(mock_random.random).any_call().then_return(0.123)
+
+    assert mock_random.random() == 0.123
+
+    assert that(mock_random.random).was_called
+    assert that(mock_random.random).num_calls == 1
+    assert that(mock_random.random).last_call == ()
+
+    with pytest.raises(AttributeError):
+        mock_random.foobar()
```

