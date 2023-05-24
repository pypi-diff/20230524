# Comparing `tmp/rzpipe-0.4.0.tar.gz` & `tmp/rzpipe-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rzpipe-0.4.0.tar", last modified: Tue Jun 28 08:35:48 2022, max compression
+gzip compressed data, was "rzpipe-0.5.0.tar", last modified: Wed May 24 16:30:56 2023, max compression
```

## Comparing `rzpipe-0.4.0.tar` & `rzpipe-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 08:35:48.447302 rzpipe-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-06-28 08:30:42.000000 rzpipe-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-06-28 08:30:42.000000 rzpipe-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-06-28 08:35:48.447302 rzpipe-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-06-28 08:30:42.000000 rzpipe-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 08:35:48.447302 rzpipe-0.4.0/rzpipe/
--rw-r--r--   0 runner    (1001) docker     (121)     4613 2022-06-28 08:30:42.000000 rzpipe-0.4.0/rzpipe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3473 2022-06-28 08:30:42.000000 rzpipe-0.4.0/rzpipe/native.py
--rw-r--r--   0 runner    (1001) docker     (121)     7076 2022-06-28 08:30:42.000000 rzpipe-0.4.0/rzpipe/open_async.py
--rw-r--r--   0 runner    (1001) docker     (121)     9439 2022-06-28 08:30:42.000000 rzpipe-0.4.0/rzpipe/open_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4872 2022-06-28 08:30:42.000000 rzpipe-0.4.0/rzpipe/open_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 08:35:48.447302 rzpipe-0.4.0/rzpipe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-06-28 08:35:48.000000 rzpipe-0.4.0/rzpipe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-06-28 08:35:48.000000 rzpipe-0.4.0/rzpipe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-28 08:35:48.000000 rzpipe-0.4.0/rzpipe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-06-28 08:35:48.000000 rzpipe-0.4.0/rzpipe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-28 08:35:48.447302 rzpipe-0.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      876 2022-06-28 08:30:42.000000 rzpipe-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:30:56.270512 rzpipe-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-05-24 16:23:58.000000 rzpipe-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-24 16:23:58.000000 rzpipe-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-05-24 16:30:56.270512 rzpipe-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      506 2023-05-24 16:23:58.000000 rzpipe-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:30:56.270512 rzpipe-0.5.0/rzpipe/
+-rw-r--r--   0 runner    (1001) docker     (122)     4613 2023-05-24 16:23:58.000000 rzpipe-0.5.0/rzpipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3473 2023-05-24 16:23:58.000000 rzpipe-0.5.0/rzpipe/native.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7096 2023-05-24 16:23:58.000000 rzpipe-0.5.0/rzpipe/open_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10191 2023-05-24 16:23:58.000000 rzpipe-0.5.0/rzpipe/open_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4892 2023-05-24 16:23:58.000000 rzpipe-0.5.0/rzpipe/open_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:30:56.270512 rzpipe-0.5.0/rzpipe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-05-24 16:30:56.000000 rzpipe-0.5.0/rzpipe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-24 16:30:56.000000 rzpipe-0.5.0/rzpipe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 16:30:56.000000 rzpipe-0.5.0/rzpipe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-24 16:30:56.000000 rzpipe-0.5.0/rzpipe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-24 16:30:56.270512 rzpipe-0.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)      876 2023-05-24 16:23:58.000000 rzpipe-0.5.0/setup.py
```

### Comparing `rzpipe-0.4.0/LICENSE` & `rzpipe-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rzpipe-0.4.0/PKG-INFO` & `rzpipe-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rzpipe
-Version: 0.4.0
+Version: 0.5.0
 Summary: Pipe interface for rizin
 Home-page: https://rizin.re
 Author: rizinorg
 Author-email: info@rizin.re
 License: MIT
 Description: # rzpipe for Python
```

### Comparing `rzpipe-0.4.0/rzpipe/__init__.py` & `rzpipe-0.5.0/rzpipe/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import time
 
 try:
     import rzlang
 except ImportError:
     rzlang = None
 
-VERSION = "0.4.0"
+VERSION = "0.5.0"
 
 from .open_sync import open
 from shutil import which
 
 
 def version():
     """Return string with the version of the rzpipe library"""
```

### Comparing `rzpipe-0.4.0/rzpipe/native.py` & `rzpipe-0.5.0/rzpipe/native.py`

 * *Files identical despite different names*

### Comparing `rzpipe-0.4.0/rzpipe/open_async.py` & `rzpipe-0.5.0/rzpipe/open_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 
     def close(self):
         if self._loop.is_running():
             self._loop.stop()
         if not self._loop.is_closed():
             self._loop.close()
 
-    def __init__(self, filename="", flags=None, rz_home=None):
-        super(open, self).__init__(filename, flags)
+    def __init__(self, filename="", flags=None, rz_home=None, **kwargs):
+        super(open, self).__init__(filename, flags, **kwargs)
 
         if flags is None:
             flags = []
 
         self.rz_home = rz_home
 
         if os.name == "nt":
```

### Comparing `rzpipe-0.4.0/rzpipe/open_base.py` & `rzpipe-0.5.0/rzpipe/open_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 """
 
 import json
 import os
 import platform
 import sys
+import signal
+import functools
+from contextlib import contextmanager
 from shutil import which
 from subprocess import Popen, PIPE
 
 try:
     import rzlang
 except ImportError:
     rzlang = None
@@ -74,22 +77,31 @@
             bin_file = "/usr/bin/rizin"
 
         if os.path.isfile(bin_file):
             return bin_file
         else:
             raise IOError("rizin can't be found in your system")
 
+@contextmanager
+def timeout_callback(timeout_s, callback):
+    signal.signal(signal.SIGALRM, callback)
+
+    try:
+        signal.alarm(timeout_s)
+        yield
+    finally:
+        signal.alarm(0)
 
 class OpenBase(object):
     """
     Class representing an rzpipe connection with a running rizin instance
     Class body derived from __init__.py "open" class.
     """
 
-    def __init__(self, filename="", flags=None):
+    def __init__(self, filename="", flags=None, cmd_timeout_s=-1):
         """
         Open a new rizin pipe
         The 'filename' can be one of the following:
 
         * absolute or relative path to file
         * http://<host>:<port> to connect to an rizin webserver
         * tcp://<host>:<port> to connect to an rizin tcp server
@@ -101,14 +113,16 @@
                 ("-wdn") or separated by commas ("-w","-d","-n")
         Returns:
             Returns an object with methods to interact with rizin via commands
         """
         if not flags:
             flags = []
 
+        self.cmd_timeout_s = cmd_timeout_s
+
         self._async = False
 
         # Set cmd native as default
         self.uri = filename
         self._cmd = self._cmd_native
 
         if not filename and has_rzlang():
@@ -157,14 +171,19 @@
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         self.quit()
 
+    def _handle_killswitch_timeout(self, context, *args):
+        self._quit_process()
+
+        raise TimeoutError(f"Timeout of {self.cmd_timeout_s} seconds reached on '{context}'")
+
     def _cmd_pipe(self, cmd):
         out = b""
         cmd = cmd.strip().replace("\n", ";")
         if os.name == "nt":
             cmd = cmd.encode("utf-8")
             windll.kernel32.WriteFile(
                 self.pipe[1], cmd, len(cmd), byref(cbWritten), None
@@ -203,14 +222,17 @@
 
     def _cmd_rzlang(self, cmd):
         return rzlang.cmd(cmd)
 
     def quit(self):
         """Quit current rzpipe session and kill"""
         self.cmd("q")
+        self._quit_process()
+
+    def _quit_process(self):
         if hasattr(self, "process"):
             import subprocess
 
             is_async = not isinstance(self.process, subprocess.Popen)
             if not is_async:
                 for f in [self.process.stdin, self.process.stdout]:
                     if f is not None:
@@ -237,20 +259,24 @@
 
         res = self._cmd(cmd)
         if res is not None:
             return res.strip()
         return None
         """
 
-        res = self._cmd(cmd, **kwargs)
-        if res is not None:
-            if os.name == "nt":
-                res = res.replace("\r\n", "\n")
-            return res
-        return None
+        with timeout_callback(
+            self.cmd_timeout_s,
+            functools.partial(self._handle_killswitch_timeout, f"rzpipe.cmd: {cmd}")
+        ):
+            res = self._cmd(cmd, **kwargs)
+            if res is not None:
+                if os.name == "nt":
+                    res = res.replace("\r\n", "\n")
+                return res
+            return None
 
     def cmdj(self, cmd, **kwargs):
         """Same as cmd() but evaluates JSONs and returns an object
         Args:
             cmdj (str): rizin command
         Returns:
             Returns a JSON object respresenting the parsed JSON
```

### Comparing `rzpipe-0.4.0/rzpipe/open_sync.py` & `rzpipe-0.5.0/rzpipe/open_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 try:
     import fcntl
 except ImportError:
     fcntl = None
 
 
 class open(OpenBase):
-    def __init__(self, filename="", flags=None, rizin_home=None):
-        super(open, self).__init__(filename, flags)
+    def __init__(self, filename="", flags=None, rizin_home=None, **kwargs):
+        super(open, self).__init__(filename, flags, **kwargs)
         if flags is None:
             flags = []
         if filename.startswith("http://"):
             self._cmd = self._cmd_http
             self.uri = filename + "/cmd"
         elif filename.startswith("ccall://"):
             self._cmd = self._cmd_native
```

### Comparing `rzpipe-0.4.0/rzpipe.egg-info/PKG-INFO` & `rzpipe-0.5.0/rzpipe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rzpipe
-Version: 0.4.0
+Version: 0.5.0
 Summary: Pipe interface for rizin
 Home-page: https://rizin.re
 Author: rizinorg
 Author-email: info@rizin.re
 License: MIT
 Description: # rzpipe for Python
```

### Comparing `rzpipe-0.4.0/setup.py` & `rzpipe-0.5.0/setup.py`

 * *Files identical despite different names*

