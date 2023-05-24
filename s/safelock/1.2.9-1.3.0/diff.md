# Comparing `tmp/safelock-1.2.9.tar.gz` & `tmp/safelock-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safelock-1.2.9.tar", last modified: Tue Jan 25 09:50:28 2022, max compression
+gzip compressed data, was "safelock-1.3.0.tar", last modified: Sun Nov 27 11:24:55 2022, max compression
```

## Comparing `safelock-1.2.9.tar` & `safelock-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2022-01-25 09:50:28.911280 safelock-1.2.9/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1052 2020-10-15 12:51:39.000000 safelock-1.2.9/LICENSE
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)       34 2020-12-20 14:39:00.000000 safelock-1.2.9/MANIFEST.in
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2003 2022-01-25 09:50:28.911280 safelock-1.2.9/PKG-INFO
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      639 2022-01-25 09:50:19.000000 safelock-1.2.9/README.md
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2022-01-25 09:50:28.911280 safelock-1.2.9/safelock.egg-info/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2003 2022-01-25 09:50:28.000000 safelock-1.2.9/safelock.egg-info/PKG-INFO
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      211 2022-01-25 09:50:28.000000 safelock-1.2.9/safelock.egg-info/SOURCES.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)        1 2022-01-25 09:50:28.000000 safelock-1.2.9/safelock.egg-info/dependency_links.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)       15 2022-01-25 09:50:28.000000 safelock-1.2.9/safelock.egg-info/requires.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)        9 2022-01-25 09:50:28.000000 safelock-1.2.9/safelock.egg-info/top_level.txt
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2022-01-25 09:50:28.911280 safelock-1.2.9/sbin/
--rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)     7291 2022-01-25 07:48:11.000000 safelock-1.2.9/sbin/safelock
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)       38 2022-01-25 09:50:28.911280 safelock-1.2.9/setup.cfg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1888 2022-01-25 09:50:28.000000 safelock-1.2.9/setup.py
+drwxr-sr-x   0 ramblin   (1000) ramblin   (1000)        0 2022-11-27 11:24:55.581075 safelock-1.3.0/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1052 2022-04-23 12:12:52.000000 safelock-1.3.0/LICENSE
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)       34 2022-04-23 12:12:52.000000 safelock-1.3.0/MANIFEST.in
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1858 2022-11-27 11:24:55.581075 safelock-1.3.0/PKG-INFO
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      639 2022-11-27 11:24:40.000000 safelock-1.3.0/README.md
+drwxr-sr-x   0 ramblin   (1000) ramblin   (1000)        0 2022-11-27 11:24:55.581075 safelock-1.3.0/safelock.egg-info/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1858 2022-11-27 11:24:55.000000 safelock-1.3.0/safelock.egg-info/PKG-INFO
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      211 2022-11-27 11:24:55.000000 safelock-1.3.0/safelock.egg-info/SOURCES.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)        1 2022-11-27 11:24:55.000000 safelock-1.3.0/safelock.egg-info/dependency_links.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)       15 2022-11-27 11:24:55.000000 safelock-1.3.0/safelock.egg-info/requires.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)        9 2022-11-27 11:24:55.000000 safelock-1.3.0/safelock.egg-info/top_level.txt
+drwxr-sr-x   0 ramblin   (1000) ramblin   (1000)        0 2022-11-27 11:24:55.581075 safelock-1.3.0/sbin/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     7291 2022-11-27 11:24:55.000000 safelock-1.3.0/sbin/safelock
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)       38 2022-11-27 11:24:55.581075 safelock-1.3.0/setup.cfg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1888 2022-11-27 11:24:55.000000 safelock-1.3.0/setup.py
```

### Comparing `safelock-1.2.9/LICENSE` & `safelock-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safelock-1.2.9/PKG-INFO` & `safelock-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: safelock
-Version: 1.2.9
+Version: 1.3.0
 Summary: Safelock gives you simple systemwide multithread, multiprocess, multiprogram locks.
 Home-page: https://denova.com/open/safelock/
+Download-URL: https://github.com/denova-com/safelock/
 Author: denova.com
 Author-email: support@denova.com
 Maintainer: denova.com
 Maintainer-email: support@denova.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/denova-com/safelock/
 Project-URL: Documentation, https://denova.com/open/safelock/
 Project-URL: Source Code, https://github.com/denova-com/safelock/
-Description: 
-        DeNova Safelock
-        ---------------
-        
-        Mutually exclusive locks are usually the simplest way to get safe concurrent access to a shared resource.
-        But implementing the locks is a bear to get right.
-        Get simple systemwide multithread, multiprocess, and multiprogram safe locks.
-        
-        
-        Full Description
-        ----------------
-        
-        Learn more about [DeNova Safelock](https://denova.com/open/safelock/)
-        
-        Install Safelock's systemd [service file](https://denova.com/open/safelock/get_app/safelock.service)
-        to ensure your python apps can easily and safely be locked. If you are installing
-        Safelock from github, be sure to also install the "safelog" package from PyPI.
-        
 Keywords: locks multiprocess multithread multiinstance
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
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+DeNova Safelock
+---------------
+
+Mutually exclusive locks are usually the simplest way to get safe concurrent access to a shared resource.
+But implementing the locks is a bear to get right.
+Get simple systemwide multithread, multiprocess, and multiprogram safe locks.
+
+
+Full Description
+----------------
+
+Learn more about [DeNova Safelock](https://denova.com/open/safelock/)
+
+Install Safelock's systemd [service file](https://denova.com/open/safelock/get_app/safelock.service)
+to ensure your python apps can easily and safely be locked. If you are installing
+Safelock from github, be sure to also install the "safelog" package from PyPI.
```

### Comparing `safelock-1.2.9/README.md` & `safelock-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `safelock-1.2.9/safelock.egg-info/PKG-INFO` & `safelock-1.3.0/safelock.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: safelock
-Version: 1.2.9
+Version: 1.3.0
 Summary: Safelock gives you simple systemwide multithread, multiprocess, multiprogram locks.
 Home-page: https://denova.com/open/safelock/
+Download-URL: https://github.com/denova-com/safelock/
 Author: denova.com
 Author-email: support@denova.com
 Maintainer: denova.com
 Maintainer-email: support@denova.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/denova-com/safelock/
 Project-URL: Documentation, https://denova.com/open/safelock/
 Project-URL: Source Code, https://github.com/denova-com/safelock/
-Description: 
-        DeNova Safelock
-        ---------------
-        
-        Mutually exclusive locks are usually the simplest way to get safe concurrent access to a shared resource.
-        But implementing the locks is a bear to get right.
-        Get simple systemwide multithread, multiprocess, and multiprogram safe locks.
-        
-        
-        Full Description
-        ----------------
-        
-        Learn more about [DeNova Safelock](https://denova.com/open/safelock/)
-        
-        Install Safelock's systemd [service file](https://denova.com/open/safelock/get_app/safelock.service)
-        to ensure your python apps can easily and safely be locked. If you are installing
-        Safelock from github, be sure to also install the "safelog" package from PyPI.
-        
 Keywords: locks multiprocess multithread multiinstance
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
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+DeNova Safelock
+---------------
+
+Mutually exclusive locks are usually the simplest way to get safe concurrent access to a shared resource.
+But implementing the locks is a bear to get right.
+Get simple systemwide multithread, multiprocess, and multiprogram safe locks.
+
+
+Full Description
+----------------
+
+Learn more about [DeNova Safelock](https://denova.com/open/safelock/)
+
+Install Safelock's systemd [service file](https://denova.com/open/safelock/get_app/safelock.service)
+to ensure your python apps can easily and safely be locked. If you are installing
+Safelock from github, be sure to also install the "safelog" package from PyPI.
```

### Comparing `safelock-1.2.9/sbin/safelock` & `safelock-1.3.0/sbin/safelock`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     Server for Multiprocess-safe locks.
     Client side is denova.os.lock.
 
     When you install "safelock" from PyPI, all the dependencies, including the
     client side, are automatically installed.
 
     Copyright 2019-2022 DeNova
-    Last modified: 2022-01-25
+    Last modified: 2022-11-21
 
     Written because none of the standard python locking mechanisms work reliably.
 
     To do: Drop privs
 
     This file is open source, licensed under GPLv3 <http://www.gnu.org/licenses/>.
 '''
@@ -26,15 +26,15 @@
 from denova.os import lock
 from denova.os.process import is_pid_active, is_program_running
 from denova.os.user import require_user
 from denova.python.log import Log
 from denova.python.times import timestamp
 
 
-CURRENT_VERSION = '1.2.9'
+CURRENT_VERSION = '1.3.0'
 COPYRIGHT = 'Copyright 2019-2022 DeNova'
 LICENSE = 'GPLv3'
 
 # globals so they aren't initialized on every connection
 locks = {}
 count = 0
 log = Log()
```

### Comparing `safelock-1.2.9/setup.py` & `safelock-1.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 '''
     Set up for safelock
 
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
     name="safelock",
-    version="1.2.9",
+    version="1.3.0",
     author="denova.com",
     author_email="support@denova.com",
     maintainer="denova.com",
     maintainer_email="support@denova.com",
     description="Safelock gives you simple systemwide multithread, multiprocess, multiprogram locks.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

