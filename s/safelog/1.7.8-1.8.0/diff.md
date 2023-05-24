# Comparing `tmp/safelog-1.7.8.tar.gz` & `tmp/safelog-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safelog-1.7.8.tar", last modified: Tue Jan 25 09:50:36 2022, max compression
+gzip compressed data, was "safelog-1.8.0.tar", last modified: Sun Nov 27 11:24:56 2022, max compression
```

## Comparing `safelog-1.7.8.tar` & `safelog-1.8.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2022-01-25 09:50:36.315477 safelog-1.7.8/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)       32 2020-12-20 14:39:06.000000 safelog-1.7.8/MANIFEST.in
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1858 2022-01-25 09:50:36.315477 safelog-1.7.8/PKG-INFO
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      551 2022-01-25 09:50:19.000000 safelog-1.7.8/README.md
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2022-01-25 09:50:36.315477 safelog-1.7.8/safelog.egg-info/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1858 2022-01-25 09:50:36.000000 safelog-1.7.8/safelog.egg-info/PKG-INFO
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      197 2022-01-25 09:50:36.000000 safelog-1.7.8/safelog.egg-info/SOURCES.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)        1 2022-01-25 09:50:36.000000 safelog-1.7.8/safelog.egg-info/dependency_links.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)        7 2022-01-25 09:50:36.000000 safelog-1.7.8/safelog.egg-info/requires.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)        8 2022-01-25 09:50:36.000000 safelog-1.7.8/safelog.egg-info/top_level.txt
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2022-01-25 09:50:36.315477 safelog-1.7.8/sbin/
--rwxr--r--   0 ramblin   (1000) ramblin   (1000)    10638 2022-01-25 07:50:24.000000 safelog-1.7.8/sbin/safelog
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)       38 2022-01-25 09:50:36.315477 safelog-1.7.8/setup.cfg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1825 2022-01-25 09:50:29.000000 safelog-1.7.8/setup.py
+drwxr-sr-x   0 ramblin   (1000) ramblin   (1000)        0 2022-11-27 11:24:56.377075 safelog-1.8.0/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      594 2022-04-23 12:12:52.000000 safelog-1.8.0/LICENSE
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)       32 2022-04-23 12:12:52.000000 safelog-1.8.0/MANIFEST.in
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1721 2022-11-27 11:24:56.377075 safelog-1.8.0/PKG-INFO
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      551 2022-11-27 11:24:40.000000 safelog-1.8.0/README.md
+drwxr-sr-x   0 ramblin   (1000) ramblin   (1000)        0 2022-11-27 11:24:56.377075 safelog-1.8.0/safelog.egg-info/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1721 2022-11-27 11:24:56.000000 safelog-1.8.0/safelog.egg-info/PKG-INFO
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      205 2022-11-27 11:24:56.000000 safelog-1.8.0/safelog.egg-info/SOURCES.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)        1 2022-11-27 11:24:56.000000 safelog-1.8.0/safelog.egg-info/dependency_links.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)        7 2022-11-27 11:24:56.000000 safelog-1.8.0/safelog.egg-info/requires.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)        8 2022-11-27 11:24:56.000000 safelog-1.8.0/safelog.egg-info/top_level.txt
+drwxr-sr-x   0 ramblin   (1000) ramblin   (1000)        0 2022-11-27 11:24:56.377075 safelog-1.8.0/sbin/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    10638 2022-11-27 11:24:55.000000 safelog-1.8.0/sbin/safelog
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)       38 2022-11-27 11:24:56.377075 safelog-1.8.0/setup.cfg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1825 2022-11-27 11:24:55.000000 safelog-1.8.0/setup.py
```

### Comparing `safelog-1.7.8/PKG-INFO` & `safelog-1.8.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: safelog
-Version: 1.7.8
+Version: 1.8.0
 Summary: Safelog is a multithread, multiprocess, multiinstance logging package.
 Home-page: https://denova.com/open/safelog/
+Download-URL: https://github.com/denova-com/safelog/
 Author: denova.com
 Author-email: support@denova.com
 Maintainer: denova.com
 Maintainer-email: support@denova.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/denova-com/safelog/
 Project-URL: Documentation, https://denova.com/open/safelog/
 Project-URL: Source Code, https://github.com/denova-com/safelog/
-Description: 
-        DeNova Safelog
-        --------------
-        
-        Get instant multithread, multiprocess, and multiprogram safe logs. Safelog also
-        has a much simpler and more powerful api than standard python logging.
-        
-        
-        Full Description
-        ----------------
-        
-        Learn more about [DeNova Safelog](https://denova.com/open/safelog/)
-        
-        Install Safelog's systemd [service file](https://denova.com/open/safelog/get_app/safelog.service)
-        to make sure "safelog" is available for all of your python apps. If you are installing
-        Safelog from github, be sure to also install the "denova" package from PyPI.
-        
 Keywords: logging multiprocess multithread multi-instance
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: System :: Logging
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+DeNova Safelog
+--------------
+
+Get instant multithread, multiprocess, and multiprogram safe logs. Safelog also
+has a much simpler and more powerful api than standard python logging.
+
+
+Full Description
+----------------
+
+Learn more about [DeNova Safelog](https://denova.com/open/safelog/)
+
+Install Safelog's systemd [service file](https://denova.com/open/safelog/get_app/safelog.service)
+to make sure "safelog" is available for all of your python apps. If you are installing
+Safelog from github, be sure to also install the "denova" package from PyPI.
```

### Comparing `safelog-1.7.8/README.md` & `safelog-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `safelog-1.7.8/safelog.egg-info/PKG-INFO` & `safelog-1.8.0/safelog.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: safelog
-Version: 1.7.8
+Version: 1.8.0
 Summary: Safelog is a multithread, multiprocess, multiinstance logging package.
 Home-page: https://denova.com/open/safelog/
+Download-URL: https://github.com/denova-com/safelog/
 Author: denova.com
 Author-email: support@denova.com
 Maintainer: denova.com
 Maintainer-email: support@denova.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/denova-com/safelog/
 Project-URL: Documentation, https://denova.com/open/safelog/
 Project-URL: Source Code, https://github.com/denova-com/safelog/
-Description: 
-        DeNova Safelog
-        --------------
-        
-        Get instant multithread, multiprocess, and multiprogram safe logs. Safelog also
-        has a much simpler and more powerful api than standard python logging.
-        
-        
-        Full Description
-        ----------------
-        
-        Learn more about [DeNova Safelog](https://denova.com/open/safelog/)
-        
-        Install Safelog's systemd [service file](https://denova.com/open/safelog/get_app/safelog.service)
-        to make sure "safelog" is available for all of your python apps. If you are installing
-        Safelog from github, be sure to also install the "denova" package from PyPI.
-        
 Keywords: logging multiprocess multithread multi-instance
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: System :: Logging
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+DeNova Safelog
+--------------
+
+Get instant multithread, multiprocess, and multiprogram safe logs. Safelog also
+has a much simpler and more powerful api than standard python logging.
+
+
+Full Description
+----------------
+
+Learn more about [DeNova Safelog](https://denova.com/open/safelog/)
+
+Install Safelog's systemd [service file](https://denova.com/open/safelog/get_app/safelog.service)
+to make sure "safelog" is available for all of your python apps. If you are installing
+Safelog from github, be sure to also install the "denova" package from PyPI.
```

### Comparing `safelog-1.7.8/sbin/safelog` & `safelog-1.8.0/sbin/safelog`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
     When you install "safelog" from PyPI, all the dependencies, including the
     client side, are automatically installed.
 
     Get instant multithread, multiprocess, and multiprogram safe logs.
 
     Copyright 2019-2022 DeNova
-    Last modified: 2022-01-25
+    Last modified: 2022-11-21
 
     To do: Drop privs. Create a user with write permission to log files.
 
     This file is open source, licensed under GPLv3 <http://www.gnu.org/licenses/>.
 '''
 
 import os
@@ -34,15 +34,15 @@
 # in denova.python.log so they can be imported easily by tools
 from denova.python.log import SAFELOG_HOST, SAFELOG_PORT, FIELD_SEPARATOR
 # safelog itself uses the alternative logging in denova.python._log
 from denova.python._log import log as tmp_log
 from denova.python.times import timestamp
 
 
-CURRENT_VERSION = '1.7.8'
+CURRENT_VERSION = '1.8.0'
 COPYRIGHT = 'Copyright 2019-2022 DeNova'
 LICENSE = 'GPLv3'
 
 # must be distinct from denova.python.log.FIELD_SEPARATOR
 NEWLINE_SUBSTITUTE = '\x02'
 
 # analogous to /var/log
```

### Comparing `safelog-1.7.8/setup.py` & `safelog-1.8.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 '''
     Set up for safelog
 
     Copyright 2018-2022 DeNova
-    Last modified: 2022-01-25
+    Last modified: 2022-11-27
 '''
 
 import os.path
 import setuptools
 
 # read long description
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="safelog",
-    version="1.7.8",
+    version="1.8.0",
     author="denova.com",
     author_email="support@denova.com",
     maintainer="denova.com",
     maintainer_email="support@denova.com",
     description="Safelog is a multithread, multiprocess, multiinstance logging package.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

