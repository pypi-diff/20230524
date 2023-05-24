# Comparing `tmp/safecopy-1.2.8.tar.gz` & `tmp/safecopy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safecopy-1.2.8.tar", last modified: Thu Jan 27 17:37:02 2022, max compression
+gzip compressed data, was "safecopy-1.3.0.tar", last modified: Sun Nov 27 11:24:54 2022, max compression
```

## Comparing `safecopy-1.2.8.tar` & `safecopy-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2022-01-27 17:37:02.196022 safecopy-1.2.8/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      594 2019-09-14 15:30:43.000000 safecopy-1.2.8/LICENSE
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)       30 2020-12-05 12:16:49.000000 safecopy-1.2.8/MANIFEST.in
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1702 2022-01-27 17:37:02.196022 safecopy-1.2.8/PKG-INFO
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      340 2022-01-27 17:37:00.000000 safecopy-1.2.8/README.md
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2022-01-27 17:37:02.192021 safecopy-1.2.8/bin/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    43878 2022-01-27 17:37:00.000000 safecopy-1.2.8/bin/safecopy
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2022-01-27 17:37:02.192021 safecopy-1.2.8/safecopy.egg-info/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1702 2022-01-27 17:37:01.000000 safecopy-1.2.8/safecopy.egg-info/PKG-INFO
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      210 2022-01-27 17:37:02.000000 safecopy-1.2.8/safecopy.egg-info/SOURCES.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)        1 2022-01-27 17:37:01.000000 safecopy-1.2.8/safecopy.egg-info/dependency_links.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)       24 2022-01-27 17:37:01.000000 safecopy-1.2.8/safecopy.egg-info/requires.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)        9 2022-01-27 17:37:01.000000 safecopy-1.2.8/safecopy.egg-info/top_level.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)       38 2022-01-27 17:37:02.196022 safecopy-1.2.8/setup.cfg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1892 2022-01-27 17:37:00.000000 safecopy-1.2.8/setup.py
+drwxr-sr-x   0 ramblin   (1000) ramblin   (1000)        0 2022-11-27 11:24:54.173075 safecopy-1.3.0/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      594 2022-04-23 12:12:52.000000 safecopy-1.3.0/LICENSE
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)       30 2022-04-23 12:12:52.000000 safecopy-1.3.0/MANIFEST.in
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1573 2022-11-27 11:24:54.173075 safecopy-1.3.0/PKG-INFO
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      340 2022-11-27 11:24:40.000000 safecopy-1.3.0/README.md
+drwxr-sr-x   0 ramblin   (1000) ramblin   (1000)        0 2022-11-27 11:24:54.173075 safecopy-1.3.0/bin/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    43997 2022-11-27 11:24:53.000000 safecopy-1.3.0/bin/safecopy
+drwxr-sr-x   0 ramblin   (1000) ramblin   (1000)        0 2022-11-27 11:24:54.173075 safecopy-1.3.0/safecopy.egg-info/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1573 2022-11-27 11:24:54.000000 safecopy-1.3.0/safecopy.egg-info/PKG-INFO
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      210 2022-11-27 11:24:54.000000 safecopy-1.3.0/safecopy.egg-info/SOURCES.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)        1 2022-11-27 11:24:54.000000 safecopy-1.3.0/safecopy.egg-info/dependency_links.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)       24 2022-11-27 11:24:54.000000 safecopy-1.3.0/safecopy.egg-info/requires.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)        9 2022-11-27 11:24:54.000000 safecopy-1.3.0/safecopy.egg-info/top_level.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)       38 2022-11-27 11:24:54.173075 safecopy-1.3.0/setup.cfg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1892 2022-11-27 11:24:53.000000 safecopy-1.3.0/setup.py
```

### Comparing `safecopy-1.2.8/LICENSE` & `safecopy-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safecopy-1.2.8/PKG-INFO` & `safecopy-1.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: safecopy
-Version: 1.2.8
+Version: 1.3.0
 Summary: Simple secure file copy. Alternative to rsync.
 Home-page: https://denova.com/open/safecopy/
+Download-URL: https://github.com/denova-com/safecopy/
 Author: denova.com
 Author-email: support@denova.com
 Maintainer: denova.com
 Maintainer-email: support@denova.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/denova-com/safecopy/
 Project-URL: Documentation, https://denova.com/open/safecopy/
 Project-URL: Source Code, https://github.com/denova-com/safecopy/
-Description: 
-        DeNova Safecopy
-        ---------------
-        
-        Safecopy syncronizes drives and directories very carefully.
-        Like rsync, without rsync's insecure default metadata check.
-        Securely copies to and from remote filesystems through sshfs.
-        
-        
-        Full Description
-        ----------------
-        
-        Learn more about the denova python package at:
-        
-            https://denova.com/open/safecopy/
-        
 Keywords: rsync file-copy
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop 
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System :: Filesystems
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+DeNova Safecopy
+---------------
+
+Safecopy syncronizes drives and directories very carefully.
+Like rsync, without rsync's insecure default metadata check.
+Securely copies to and from remote filesystems through sshfs.
+
+
+Full Description
+----------------
+
+Learn more about the denova python package at:
+
+    https://denova.com/open/safecopy/
```

### Comparing `safecopy-1.2.8/bin/safecopy` & `safecopy-1.3.0/bin/safecopy`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
     When you install "safecopy" from PyPI, all the dependencies, including the
     client side, are automatically installed.
 
     See docs at https://denova.com/open/safecopy/
 
     Copyright 2018-2022 DeNova
-    Last modified: 2022-01-27
+    Last modified: 2022-11-21
 '''
 
 import argparse
 import doctest
 import filecmp
 import os
 import platform
@@ -32,15 +32,15 @@
 from denova.python.elapsed_time import LogElapsedTime
 from denova.python.log import Log, get_log_path
 from denova.os.command import run_verbose
 from denova.os.fs import why_file_permission_denied
 
 DEBUG = True
 
-CURRENT_VERSION = '1.2.8'
+CURRENT_VERSION = '1.3.0'
 COPYRIGHT = 'Copyright 2018-2022 DeNova'
 LICENSE = 'GPLv3'
 
 # do not change the format of the following line without updating blockchain-backup
 COPYING_FILE = 'copying "{}" to "{}"'
 
 UID_GID_MASK = stat.S_ISUID | stat.S_ISGID
@@ -129,16 +129,16 @@
             error_exit('need one or more source paths and the destination path')
 
 def show_version():
     ''' Show safecopy's name and version.
 
         >>> show_version()
         <BLANKLINE>
-        Safecopy 1.2.6
-        Copyright 2018-2021 DeNova
+        Safecopy 1.2.8
+        Copyright 2018-2022 DeNova
         License: GPLv3
         <BLANKLINE>
         <BLANKLINE>
     '''
 
     details = f'\nSafecopy {CURRENT_VERSION}\n{COPYRIGHT}\nLicense: {LICENSE}\n\n'
 
@@ -508,15 +508,15 @@
     if args.verbose:
         log_message(msg)
 
 def warn(msg):
     ''' Print and log warning message '''
 
     if args and not args.nowarn:
-        msg = 'Warning: ' + msg
+        msg = 'Warning: ' + str(msg)
         print(msg)
         sys.stdout.flush()
         log_message(msg)
 
 def log_message(message):
     ''' Log a message if the denova package is available. '''
 
@@ -698,18 +698,20 @@
                             # verbose_log('read from_file')
                             from_bytes = from_file.read(buffer_size)
                             # verbose_log('read to_file')
                             to_bytes = to_file.read(buffer_size)
 
                             delay()
 
-                        verbose_log('count last partial buffer')
-                        last_buffer_size = min(len(from_bytes),
-                                               len(to_bytes))
+                        last_buffer_size = min(len(from_bytes), len(to_bytes))
                         index = 0
+                        if ((index < last_buffer_size) and
+                               (from_bytes[index] == to_bytes[index])):
+                            verbose_log(f'including last partial buffer: {last_buffer_size}')
+
                         while ((index < last_buffer_size) and
                                (from_bytes[index] == to_bytes[index])):
                             self.count = self.count + 1
                             index = index + 1
 
         verbose_log(f'{self.count} equal bytes')
```

### Comparing `safecopy-1.2.8/safecopy.egg-info/PKG-INFO` & `safecopy-1.3.0/safecopy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: safecopy
-Version: 1.2.8
+Version: 1.3.0
 Summary: Simple secure file copy. Alternative to rsync.
 Home-page: https://denova.com/open/safecopy/
+Download-URL: https://github.com/denova-com/safecopy/
 Author: denova.com
 Author-email: support@denova.com
 Maintainer: denova.com
 Maintainer-email: support@denova.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/denova-com/safecopy/
 Project-URL: Documentation, https://denova.com/open/safecopy/
 Project-URL: Source Code, https://github.com/denova-com/safecopy/
-Description: 
-        DeNova Safecopy
-        ---------------
-        
-        Safecopy syncronizes drives and directories very carefully.
-        Like rsync, without rsync's insecure default metadata check.
-        Securely copies to and from remote filesystems through sshfs.
-        
-        
-        Full Description
-        ----------------
-        
-        Learn more about the denova python package at:
-        
-            https://denova.com/open/safecopy/
-        
 Keywords: rsync file-copy
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop 
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System :: Filesystems
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+DeNova Safecopy
+---------------
+
+Safecopy syncronizes drives and directories very carefully.
+Like rsync, without rsync's insecure default metadata check.
+Securely copies to and from remote filesystems through sshfs.
+
+
+Full Description
+----------------
+
+Learn more about the denova python package at:
+
+    https://denova.com/open/safecopy/
```

### Comparing `safecopy-1.2.8/setup.py` & `safecopy-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 '''
     Set up for safecopy
 
     Copyright 2018-2021 DeNova
-    Last modified: 2022-01-27
+    Last modified: 2022-11-27
 '''
 
 import os.path
 import setuptools
 
 # read long description
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="safecopy",
-    version="1.2.8",
+    version="1.3.0",
     author="denova.com",
     author_email="support@denova.com",
     maintainer="denova.com",
     maintainer_email="support@denova.com",
     description="Simple secure file copy. Alternative to rsync.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

