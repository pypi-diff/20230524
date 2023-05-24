# Comparing `tmp/zdaemon-4.4.tar.gz` & `tmp/zdaemon-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zdaemon-4.4.tar", last modified: Fri Dec  2 07:34:50 2022, max compression
+gzip compressed data, was "zdaemon-5.0.tar", last modified: Wed May 24 06:09:28 2023, max compression
```

## Comparing `zdaemon-4.4.tar` & `zdaemon-5.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-12-02 07:34:50.815906 zdaemon-4.4/
--rw-r--r--   0 mac        (513) staff       (20)      598 2022-12-02 07:34:47.000000 zdaemon-4.4/.coveragerc
--rw-r--r--   0 mac        (513) staff       (20)     8740 2022-12-02 07:34:47.000000 zdaemon-4.4/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      808 2022-12-02 07:34:47.000000 zdaemon-4.4/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2022-12-02 07:34:47.000000 zdaemon-4.4/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2022-12-02 07:34:47.000000 zdaemon-4.4/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      305 2022-12-02 07:34:47.000000 zdaemon-4.4/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)    25442 2022-12-02 07:34:50.816177 zdaemon-4.4/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      298 2022-12-02 07:34:47.000000 zdaemon-4.4/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      453 2022-12-02 07:34:50.817475 zdaemon-4.4/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     2649 2022-12-02 07:34:47.000000 zdaemon-4.4/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-12-02 07:34:50.795870 zdaemon-4.4/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-12-02 07:34:50.805610 zdaemon-4.4/src/zdaemon/
--rw-r--r--   0 mac        (513) staff       (20)    15160 2022-12-02 07:34:47.000000 zdaemon-4.4/src/zdaemon/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      701 2022-12-02 07:34:47.000000 zdaemon-4.4/src/zdaemon/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)       40 2022-12-02 07:34:47.000000 zdaemon-4.4/src/zdaemon/__main__.py
--rw-r--r--   0 mac        (513) staff       (20)    12245 2022-12-02 07:34:47.000000 zdaemon-4.4/src/zdaemon/component.xml
--rw-r--r--   0 mac        (513) staff       (20)      437 2022-12-02 07:34:47.000000 zdaemon-4.4/src/zdaemon/sample.conf
--rw-r--r--   0 mac        (513) staff       (20)     1010 2022-12-02 07:34:47.000000 zdaemon-4.4/src/zdaemon/schema.xml
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-12-02 07:34:50.815291 zdaemon-4.4/src/zdaemon/tests/
--rw-r--r--   0 mac        (513) staff       (20)       46 2022-12-02 07:34:47.000000 zdaemon-4.4/src/zdaemon/tests/__init__.py
--rwxr-xr-x   0 mac        (513) staff       (20)      118 2022-12-02 07:34:47.000000 zdaemon-4.4/src/zdaemon/tests/nokill.py
--rw-r--r--   0 mac        (513) staff       (20)     1563 2022-12-02 07:34:47.000000 zdaemon-4.4/src/zdaemon/tests/parent.py
--rw-r--r--   0 mac        (513) staff       (20)    12131 2022-12-02 07:34:47.000000 zdaemon-4.4/src/zdaemon/tests/tests.py
--rw-r--r--   0 mac        (513) staff       (20)     4036 2022-12-02 07:34:47.000000 zdaemon-4.4/src/zdaemon/tests/testuser.py
--rw-r--r--   0 mac        (513) staff       (20)     2459 2022-12-02 07:34:47.000000 zdaemon-4.4/src/zdaemon/tests/testzdctl.py
--rw-r--r--   0 mac        (513) staff       (20)    18141 2022-12-02 07:34:47.000000 zdaemon-4.4/src/zdaemon/tests/testzdoptions.py
--rw-r--r--   0 mac        (513) staff       (20)    15816 2022-12-02 07:34:47.000000 zdaemon-4.4/src/zdaemon/tests/testzdrun.py
--rwxr-xr-x   0 mac        (513) staff       (20)    21598 2022-12-02 07:34:47.000000 zdaemon-4.4/src/zdaemon/zdctl.py
--rw-r--r--   0 mac        (513) staff       (20)    18887 2022-12-02 07:34:47.000000 zdaemon-4.4/src/zdaemon/zdoptions.py
--rwxr-xr-x   0 mac        (513) staff       (20)    25475 2022-12-02 07:34:47.000000 zdaemon-4.4/src/zdaemon/zdrun.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-12-02 07:34:50.808621 zdaemon-4.4/src/zdaemon.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)    25442 2022-12-02 07:34:49.000000 zdaemon-4.4/src/zdaemon.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      812 2022-12-02 07:34:50.000000 zdaemon-4.4/src/zdaemon.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-12-02 07:34:50.000000 zdaemon-4.4/src/zdaemon.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)       47 2022-12-02 07:34:50.000000 zdaemon-4.4/src/zdaemon.egg-info/entry_points.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-12-02 07:34:49.000000 zdaemon-4.4/src/zdaemon.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)       86 2022-12-02 07:34:50.000000 zdaemon-4.4/src/zdaemon.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        8 2022-12-02 07:34:50.000000 zdaemon-4.4/src/zdaemon.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1217 2022-12-02 07:34:47.000000 zdaemon-4.4/tox.ini
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-24 06:09:28.797851 zdaemon-5.0/
+-rw-r--r--   0 mac        (513) staff       (20)      564 2023-05-24 06:09:28.000000 zdaemon-5.0/.coveragerc
+-rw-r--r--   0 mac        (513) staff       (20)     8818 2023-05-24 06:09:28.000000 zdaemon-5.0/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)      808 2023-05-24 06:09:28.000000 zdaemon-5.0/CONTRIBUTING.md
+-rw-r--r--   0 mac        (513) staff       (20)       32 2023-05-24 06:09:28.000000 zdaemon-5.0/COPYRIGHT.txt
+-rw-r--r--   0 mac        (513) staff       (20)     2070 2023-05-24 06:09:28.000000 zdaemon-5.0/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)      305 2023-05-24 06:09:28.000000 zdaemon-5.0/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)    25325 2023-05-24 06:09:28.798005 zdaemon-5.0/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      298 2023-05-24 06:09:28.000000 zdaemon-5.0/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)      454 2023-05-24 06:09:28.798541 zdaemon-5.0/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     2484 2023-05-24 06:09:28.000000 zdaemon-5.0/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-24 06:09:28.785110 zdaemon-5.0/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-24 06:09:28.792288 zdaemon-5.0/src/zdaemon/
+-rw-r--r--   0 mac        (513) staff       (20)    15160 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)      701 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)       40 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/__main__.py
+-rw-r--r--   0 mac        (513) staff       (20)    12245 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/component.xml
+-rw-r--r--   0 mac        (513) staff       (20)      437 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/sample.conf
+-rw-r--r--   0 mac        (513) staff       (20)     1010 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/schema.xml
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-24 06:09:28.797584 zdaemon-5.0/src/zdaemon/tests/
+-rw-r--r--   0 mac        (513) staff       (20)       46 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/tests/__init__.py
+-rwxr-xr-x   0 mac        (513) staff       (20)      118 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/tests/nokill.py
+-rw-r--r--   0 mac        (513) staff       (20)     1563 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/tests/parent.py
+-rw-r--r--   0 mac        (513) staff       (20)    12093 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/tests/tests.py
+-rw-r--r--   0 mac        (513) staff       (20)     4050 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/tests/testuser.py
+-rw-r--r--   0 mac        (513) staff       (20)     2459 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/tests/testzdctl.py
+-rw-r--r--   0 mac        (513) staff       (20)    18007 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/tests/testzdoptions.py
+-rw-r--r--   0 mac        (513) staff       (20)    15741 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/tests/testzdrun.py
+-rwxr-xr-x   0 mac        (513) staff       (20)    21550 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/zdctl.py
+-rw-r--r--   0 mac        (513) staff       (20)    18841 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/zdoptions.py
+-rwxr-xr-x   0 mac        (513) staff       (20)    25450 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon/zdrun.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-24 06:09:28.794869 zdaemon-5.0/src/zdaemon.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)    25325 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      812 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)       47 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon.egg-info/entry_points.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)       86 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        8 2023-05-24 06:09:28.000000 zdaemon-5.0/src/zdaemon.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)     1173 2023-05-24 06:09:28.000000 zdaemon-5.0/tox.ini
```

### Comparing `zdaemon-4.4/.coveragerc` & `zdaemon-5.0/.coveragerc`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/buildout-recipe
 [run]
 source = zdaemon
-plugins = coverage_python_version
 branch = true
 parallel = true
 data_file = $COVERAGE_HOME.coverage
 omit = */__main__.py
 
 [paths]
 source =
```

### Comparing `zdaemon-4.4/CHANGES.rst` & `zdaemon-5.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 ==========
 Change log
 ==========
 
+5.0 (2023-05-24)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
 4.4 (2022-12-02)
 ================
 
 - Add support for Python 3.8, 3.9, 3.10, 3.11.
 
 - Drop support for Python 3.4.
```

### Comparing `zdaemon-4.4/CONTRIBUTING.md` & `zdaemon-5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zdaemon-4.4/LICENSE.txt` & `zdaemon-5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zdaemon-4.4/PKG-INFO` & `zdaemon-5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 Metadata-Version: 2.1
 Name: zdaemon
-Version: 4.4
+Version: 5.0
 Summary: Daemon process control library and tools for Unix-based systems
 Home-page: https://github.com/zopefoundation/zdaemon
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Utilities
+Requires-Python: >=3.7
 Provides-Extra: test
 License-File: LICENSE.txt
 
 *****************************************************
 ``zdaemon`` process controller for Unix-based systems
 *****************************************************
 
@@ -564,14 +560,20 @@
 Log output from zdaemon usually isn't very interesting but can be
 handy for debugging.
 
 ==========
 Change log
 ==========
 
+5.0 (2023-05-24)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
 4.4 (2022-12-02)
 ================
 
 - Add support for Python 3.8, 3.9, 3.10, 3.11.
 
 - Drop support for Python 3.4.
 
@@ -903,9 +905,7 @@
 - Document/demonstrate some important features, such as:
 
   - working directory
 
 Bugs:
 
 - help command
-
-
```

### Comparing `zdaemon-4.4/setup.py` & `zdaemon-5.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -33,20 +33,20 @@
 
 def read(*rnames):
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
 
 setup(
     name="zdaemon",
-    version='4.4',
+    version='5.0',
     url="https://github.com/zopefoundation/zdaemon",
     license="ZPL 2.1",
     description="Daemon process control library and tools for Unix-based systems",  # noqa: E501 line too long
     author="Zope Foundation and Contributors",
-    author_email="zope-dev@zope.org",
+    author_email="zope-dev@zope.dev",
     long_description=(
         read('README.rst') +
         '\n' +
         read('src/zdaemon/README.rst') +
         '\n' +
         read('CHANGES.rst')),
     packages=[
@@ -55,31 +55,28 @@
     package_dir={
         "": "src"},
     classifiers=[
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'License :: OSI Approved :: Zope Public License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Operating System :: POSIX',
         'Topic :: Utilities',
     ],
     zip_safe=False,
     entry_points=entry_points,
     include_package_data=True,
+    python_requires='>=3.7',
     install_requires=[
         "ZConfig",
         "setuptools"
     ],
     extras_require=dict(test=tests_require),
 )
```

### Comparing `zdaemon-4.4/src/zdaemon/README.rst` & `zdaemon-5.0/src/zdaemon/README.rst`

 * *Files identical despite different names*

### Comparing `zdaemon-4.4/src/zdaemon/__init__.py` & `zdaemon-5.0/src/zdaemon/__init__.py`

 * *Files identical despite different names*

### Comparing `zdaemon-4.4/src/zdaemon/component.xml` & `zdaemon-5.0/src/zdaemon/component.xml`

 * *Files identical despite different names*

### Comparing `zdaemon-4.4/src/zdaemon/schema.xml` & `zdaemon-5.0/src/zdaemon/schema.xml`

 * *Files identical despite different names*

### Comparing `zdaemon-4.4/src/zdaemon/tests/parent.py` & `zdaemon-5.0/src/zdaemon/tests/parent.py`

 * *Files identical despite different names*

### Comparing `zdaemon-4.4/src/zdaemon/tests/tests.py` & `zdaemon-5.0/src/zdaemon/tests/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 # Version 2.0 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
-from __future__ import print_function
 
 import doctest
 import glob
 import os
 import re
 import shutil
 import signal
```

### Comparing `zdaemon-4.4/src/zdaemon/tests/testuser.py` & `zdaemon-5.0/src/zdaemon/tests/testuser.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 ##############################################################################
 
 # Test user and groups options
 
 import doctest
 import os
 import sys
+from unittest import mock
 
-import mock
 from zope.testing import setupstack
 
 import zdaemon.zdctl
 
 
 def write(name, text):
     with open(name, 'w') as f:
```

### Comparing `zdaemon-4.4/src/zdaemon/tests/testzdctl.py` & `zdaemon-5.0/src/zdaemon/tests/testzdctl.py`

 * *Files identical despite different names*

### Comparing `zdaemon-4.4/src/zdaemon/tests/testzdoptions.py` & `zdaemon-5.0/src/zdaemon/tests/testzdoptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,32 +16,26 @@
 
 import doctest
 import os
 import shutil
 import sys
 import tempfile
 import unittest
+from io import StringIO
 
 import ZConfig
 
 import zdaemon
 from zdaemon.zdoptions import RunnerOptions
 from zdaemon.zdoptions import ZDOptions
 from zdaemon.zdoptions import existing_parent_directory
 from zdaemon.zdoptions import existing_parent_dirpath
 from zdaemon.zdoptions import list_of_ints
 
 
-try:
-    from StringIO import StringIO
-except ImportError:
-    # PY3 support.
-    from io import StringIO
-
-
 class ZDOptionsTestBase(unittest.TestCase):
 
     OptionsClass = ZDOptions
 
     def save_streams(self):
         self.save_stdout = sys.stdout
         self.save_stderr = sys.stderr
@@ -434,21 +428,21 @@
 
 
 class TestRunnerDirectory(ZDOptionsTestBase):
 
     OptionsClass = RunnerOptions
 
     def setUp(self):
-        super(TestRunnerDirectory, self).setUp()
+        super().setUp()
         # Create temporary directory to work in
         self.root = tempfile.mkdtemp()
 
     def tearDown(self):
         shutil.rmtree(self.root)
-        super(TestRunnerDirectory, self).tearDown()
+        super().tearDown()
 
     def test_not_existing_directory(self):
         options = self.OptionsClass()
         path = os.path.join(self.root, 'does-not-exist', 'really-not')
         self.check_exit_code(options, ["-z", path])
         socket = os.path.join(path, 'socket')
         self.check_exit_code(options, ["-s", socket])
```

### Comparing `zdaemon-4.4/src/zdaemon/tests/testzdrun.py` & `zdaemon-5.0/src/zdaemon/tests/testzdrun.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,18 @@
 """Test suite for zdrun.py."""
-from __future__ import print_function
 
 import os
 import shutil
 import signal
 import socket
 import sys
 import tempfile
 import time
 import unittest
-
-
-try:
-    from StringIO import StringIO
-except ImportError:
-    # PY3 support.
-    from io import StringIO
+from io import StringIO
 
 import ZConfig
 
 from zdaemon import zdctl
 from zdaemon import zdrun
 
 
@@ -292,15 +285,15 @@
             if os.path.exists(path):
                 os.remove(path)
 
 
 class TestRunnerDirectory(unittest.TestCase):
 
     def setUp(self):
-        super(TestRunnerDirectory, self).setUp()
+        super().setUp()
         self.root = tempfile.mkdtemp()
         self.save_stdout = sys.stdout
         self.save_stderr = sys.stdout
         sys.stdout = StringIO()
         sys.stderr = StringIO()
         self.expect = ''
         self.cmd = "/bin/true"
@@ -312,15 +305,15 @@
         got = sys.stdout.getvalue()
         err = sys.stderr.getvalue()
         sys.stdout = self.save_stdout
         sys.stderr = self.save_stderr
         if err:
             print(err, end='', file=sys.stderr)
         self.assertEqual(self.expect, got)
-        super(TestRunnerDirectory, self).tearDown()
+        super().tearDown()
 
     def run_ctl(self, opts):
         options = zdctl.ZDCtlOptions()
         options.realize(opts + ['fg'])
         self.expect = self.cmd + '\n'
         proc = zdctl.ZDCmd(options)
         proc.onecmd(" ".join(options.args))
@@ -434,15 +427,15 @@
         while True:
             data = sock.recv(1000)
             if not data:
                 break
             response += data
         sock.close()
         return response
-    except socket.error as msg:
+    except OSError as msg:
         if str(msg) == 'AF_UNIX path too long':
             # MacOS has apparent small limits on the length of a UNIX
             # domain socket filename, we want to make MacOS users aware
             # of the actual problem
             raise
         if raise_on_error:
             raise
@@ -450,10 +443,12 @@
     finally:
         sock.close()
 
 
 def test_suite():
     suite = unittest.TestSuite()
     if os.name == "posix":
-        suite.addTest(unittest.makeSuite(ZDaemonTests))
-        suite.addTest(unittest.makeSuite(TestRunnerDirectory))
+        loadTestsFromTestCase = (
+            unittest.defaultTestLoader.loadTestsFromTestCase)
+        suite.addTest(loadTestsFromTestCase(ZDaemonTests))
+        suite.addTest(loadTestsFromTestCase(TestRunnerDirectory))
     return suite
```

### Comparing `zdaemon-4.4/src/zdaemon/zdctl.py` & `zdaemon-5.0/src/zdaemon/zdctl.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 --version -- print zdaemon version and exit
 -z/--directory DIRECTORY -- directory to chdir to when using -d (default off)
 action [arguments] -- see below
 
 Actions are commands like "start", "stop" and "status".  Use the
 action "help" to find out about available actions.
 """
-from __future__ import print_function
 
 import cmd
 import os
 import os.path
 import re
 import signal
 import socket
@@ -228,15 +227,15 @@
             response = b""
             while True:
                 data = sock.recv(1000)
                 if not data:
                     break
                 response += data
             return response.decode()
-        except socket.error:
+        except OSError:
             return None
         finally:
             sock.close()
 
     zd_testing = 0
 
     def get_status(self):
@@ -525,15 +524,15 @@
                 print("No default log file specified; use logtail <logfile>")
                 return
         try:
             helper = TailHelper(arg)
             helper.tailf()
         except KeyboardInterrupt:
             print()
-        except IOError as msg:
+        except OSError as msg:
             print(msg)
         except OSError as msg:
             print(msg)
 
     def help_logtail(self):
         print("logtail [logfile] -- Run tail -f on the given logfile.")
         print("                     A default file may exist.")
@@ -571,15 +570,15 @@
 
 
 class TailHelper:
 
     MAX_BUFFSIZE = 1024
 
     def __init__(self, fname):
-        self.f = open(fname, 'r')
+        self.f = open(fname)
 
     def tailf(self):
         sz, lines = self.tail(10)
         for line in lines:
             sys.stdout.write(line)
             sys.stdout.flush()
         while True:
```

### Comparing `zdaemon-4.4/src/zdaemon/zdoptions.py` & `zdaemon-5.0/src/zdaemon/zdoptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Option processing for zdaemon and related code."""
-from __future__ import print_function
 
 import getopt
 import os
 import signal
 import sys
 
 import pkg_resources
@@ -173,16 +172,16 @@
                 raise ValueError("flag= requires a command line flag")
 
             def handler(arg, flag=flag):
                 return flag
 
         if short and long:
             if short.endswith(":") != long.endswith("="):
-                raise ValueError("inconsistent short/long options: %r %r" % (
-                    short, long))
+                raise ValueError(
+                    f"inconsistent short/long options: {short!r} {long!r}")
 
         if short:
             if short[0] == "-":
                 raise ValueError("short option should not start with '-'")
             key, rest = short[:1], short[1:]
             if rest not in ("", ":"):
                 raise ValueError("short option should be 'x' or 'x:'")
@@ -258,15 +257,15 @@
         # Process options returned by getopt
         for opt, arg in self.options:
             name, handler = self.options_map[opt]
             if handler is not None:
                 try:
                     arg = handler(arg)
                 except ValueError as msg:
-                    self.usage("invalid value for %s %r: %s" % (opt, arg, msg))
+                    self.usage(f"invalid value for {opt} {arg!r}: {msg}")
             if name and arg is not None:
                 if getattr(self, name) is not None:
                     if getattr(self, name) == arg:
                         # Repeated option, but we don't mind because it
                         # just reinforces what we have.
                         continue
                     self.usage("conflicting command line option %r" % opt)
```

### Comparing `zdaemon-4.4/src/zdaemon/zdrun.py` & `zdaemon-5.0/src/zdaemon/zdrun.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,15 +293,15 @@
     def checkopen(self):
         s = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
         try:
             s.connect(self.options.sockname)
             s.send(b"status\n")
             data = s.recv(1000).decode()
             s.close()
-        except socket.error:
+        except OSError:
             pass
         else:
             data = data.rstrip("\n")
             msg = ("Another zrdun is already up using socket %r:\n%s" %
                    (self.options.sockname, data))
             sys.stderr.write(msg + "\n")
             sys.stderr.flush()  # just in case
@@ -412,31 +412,31 @@
                 if timeout <= 0:
                     self.delay = 0
                     if self.killing and self.proc.pid:
                         self.proc.kill(signal.SIGKILL)
                         self.delay = time.time() + self.options.backofflimit
             try:
                 r, w, x = select.select(r, w, x, timeout)
-            except select.error as err:
+            except OSError as err:
                 if err.args[0] != errno.EINTR:
                     raise
                 r = w = x = []
             if self.waitstatus:
                 self.reportstatus()
             if self.commandsocket and self.commandsocket in r:
                 try:
                     self.dorecv()
-                except socket.error as msg:
+                except OSError as msg:
                     self.logger.exception("socket.error in dorecv(): %s"
                                           % str(msg))
                     self.commandsocket = None
             if self.mastersocket in r:
                 try:
                     self.doaccept()
-                except socket.error as msg:
+                except OSError as msg:
                     self.logger.exception("socket.error in doaccept(): %s"
                                           % str(msg))
                     self.commandsocket = None
             if sig_r in r:
                 os.read(sig_r, 1)  # don't let the buffer fill up
         self.logger.info("Exiting")
         sys.exit(0)
@@ -618,15 +618,15 @@
             if hasattr(self.commandsocket, "sendall"):
                 self.commandsocket.sendall(msg)
             else:  # pragma: nocover
                 # This is quadratic, but msg is rarely more than 100 bytes :-)
                 while msg:
                     sent = self.commandsocket.send(msg)
                     msg = msg[sent:]
-        except socket.error as msg:
+        except OSError as msg:
             self.logger.warn("Error sending reply: %s" % str(msg))
 
 
 class Transcript:
 
     def __init__(self, filename):
         self.read_from, w = os.pipe()
```

### Comparing `zdaemon-4.4/src/zdaemon.egg-info/PKG-INFO` & `zdaemon-5.0/src/zdaemon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 Metadata-Version: 2.1
 Name: zdaemon
-Version: 4.4
+Version: 5.0
 Summary: Daemon process control library and tools for Unix-based systems
 Home-page: https://github.com/zopefoundation/zdaemon
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Utilities
+Requires-Python: >=3.7
 Provides-Extra: test
 License-File: LICENSE.txt
 
 *****************************************************
 ``zdaemon`` process controller for Unix-based systems
 *****************************************************
 
@@ -564,14 +560,20 @@
 Log output from zdaemon usually isn't very interesting but can be
 handy for debugging.
 
 ==========
 Change log
 ==========
 
+5.0 (2023-05-24)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
 4.4 (2022-12-02)
 ================
 
 - Add support for Python 3.8, 3.9, 3.10, 3.11.
 
 - Drop support for Python 3.4.
 
@@ -903,9 +905,7 @@
 - Document/demonstrate some important features, such as:
 
   - working directory
 
 Bugs:
 
 - help command
-
-
```

### Comparing `zdaemon-4.4/src/zdaemon.egg-info/SOURCES.txt` & `zdaemon-5.0/src/zdaemon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zdaemon-4.4/tox.ini` & `zdaemon-5.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/buildout-recipe
 [tox]
 minversion = 3.18
 envlist =
     lint
-    py27
-    py35
-    py36
     py37
     py38
     py39
     py310
     py311
-    pypy
     pypy3
     coverage
 
 [testenv]
 usedevelop = true
 deps =
 commands =
@@ -37,14 +33,15 @@
     check-python-versions >= 0.19.1
     wheel
     flake8
     isort
 
 [testenv:isort-apply]
 basepython = python3
+skip_install = true
 commands_pre =
 deps =
     isort
 commands =
     isort {toxinidir}/src {toxinidir}/setup.py []
 
 [testenv:coverage]
@@ -52,15 +49,14 @@
 allowlist_externals =
     mkdir
 setenv =
     COVERAGE_PROCESS_START={toxinidir}/.coveragerc
     COVERAGE_HOME={toxinidir}/
 deps =
     coverage
-    coverage-python-version
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage erase
     coverage run -m zope.testrunner --test-path=src {posargs:-vc}
     coverage combine
     coverage html
     coverage report -m --fail-under=79
```

