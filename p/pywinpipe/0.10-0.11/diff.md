# Comparing `tmp/pywinpipe-0.10.tar.gz` & `tmp/pywinpipe-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywinpipe-0.10.tar", last modified: Mon May 22 00:53:22 2023, max compression
+gzip compressed data, was "pywinpipe-0.11.tar", last modified: Wed May 24 00:35:32 2023, max compression
```

## Comparing `pywinpipe-0.10.tar` & `pywinpipe-0.11.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 00:53:22.485859 pywinpipe-0.10/
--rw-rw-rw-   0        0        0     1148 2023-05-22 00:53:16.000000 pywinpipe-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0       98 2023-05-22 00:53:16.000000 pywinpipe-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     4368 2023-05-22 00:53:22.485859 pywinpipe-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     3714 2023-05-22 00:52:21.000000 pywinpipe-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 00:53:22.453651 pywinpipe-0.10/pywinpipe/
--rw-rw-rw-   0        0        0     3714 2023-05-22 00:52:21.000000 pywinpipe-0.10/pywinpipe/README.md
--rw-rw-rw-   0        0        0     7310 2023-05-22 00:50:33.000000 pywinpipe-0.10/pywinpipe/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-22 00:53:21.000000 pywinpipe-0.10/pywinpipe/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-05-22 00:53:21.000000 pywinpipe-0.10/pywinpipe/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-05-22 00:53:22.481957 pywinpipe-0.10/pywinpipe.egg-info/
--rw-rw-rw-   0        0        0     4368 2023-05-22 00:53:22.000000 pywinpipe-0.10/pywinpipe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-05-22 00:53:22.000000 pywinpipe-0.10/pywinpipe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 00:53:22.000000 pywinpipe-0.10/pywinpipe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-22 00:53:22.000000 pywinpipe-0.10/pywinpipe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-05-22 00:53:22.487811 pywinpipe-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1319 2023-05-22 00:53:21.000000 pywinpipe-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 00:35:32.083503 pywinpipe-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-05-24 00:35:26.000000 pywinpipe-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0       98 2023-05-24 00:35:25.000000 pywinpipe-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     4368 2023-05-24 00:35:32.083503 pywinpipe-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     3714 2023-05-22 01:05:16.000000 pywinpipe-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 00:35:32.081551 pywinpipe-0.11/pywinpipe/
+-rw-rw-rw-   0        0        0     3714 2023-05-22 01:05:16.000000 pywinpipe-0.11/pywinpipe/README.md
+-rw-rw-rw-   0        0        0     7475 2023-05-24 00:33:06.000000 pywinpipe-0.11/pywinpipe/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 00:35:31.000000 pywinpipe-0.11/pywinpipe/requirements.txt
+-rw-rw-rw-   0        0        0        2 2023-05-24 00:35:31.000000 pywinpipe-0.11/pywinpipe/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-05-24 00:35:32.083503 pywinpipe-0.11/pywinpipe.egg-info/
+-rw-rw-rw-   0        0        0     4368 2023-05-24 00:35:31.000000 pywinpipe-0.11/pywinpipe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-05-24 00:35:31.000000 pywinpipe-0.11/pywinpipe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 00:35:31.000000 pywinpipe-0.11/pywinpipe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-24 00:35:31.000000 pywinpipe-0.11/pywinpipe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-05-24 00:35:32.084479 pywinpipe-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1319 2023-05-24 00:35:31.000000 pywinpipe-0.11/setup.py
```

### Comparing `pywinpipe-0.10/LICENSE.rst` & `pywinpipe-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pywinpipe-0.10/PKG-INFO` & `pywinpipe-0.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywinpipe
-Version: 0.10
+Version: 0.11
 Summary: pywinpipe - Fast data exchange between 2 processes (Windows only)
 Home-page: https://github.com/hansalemaos/pywinpipe
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: pipes,windows,named pipes,share,data
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pywinpipe-0.10/README.md` & `pywinpipe-0.11/README.md`

 * *Files identical despite different names*

### Comparing `pywinpipe-0.10/pywinpipe/README.md` & `pywinpipe-0.11/pywinpipe/README.md`

 * *Files identical despite different names*

### Comparing `pywinpipe-0.10/pywinpipe/__init__.py` & `pywinpipe-0.11/pywinpipe/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,36 +27,38 @@
     def __init__(
         self,
         pipename=r"\\.\pipe\example",
         nMaxInstances=1,
         nOutBufferSize=65536,
         nInBufferSize=65536,
         timeout=0,
+            block_or_nonblock='block',
     ):
         r"""
         Initializes the Write2Pipe instance and creates a named pipe.
 
         Args:
         - pipename (str): The name of the named pipe to be created. Defaults to "\\.\pipe\example".
         - nMaxInstances (int): The maximum number of instances that can connect to the named pipe. Defaults to 1.
         - nOutBufferSize (int): The size of the output buffer for the named pipe. Defaults to 65536.
         - nInBufferSize (int): The size of the input buffer for the named pipe. Defaults to 65536.
         - timeout (int): The timeout value for waiting on the named pipe connection. Defaults to 0 (no timeout).
+        - block_or_nonblock (str): valid options block/unblock Defaults to block.
 
         Note: The nMaxInstances, nOutBufferSize, and nInBufferSize parameters should match the corresponding values used when creating the named pipe.
         """
         self.nMaxInstances = nMaxInstances
         self.nOutBufferSize = nOutBufferSize
         self.nInBufferSize = nInBufferSize
         self.pipename = pipename
         self.timeout = timeout
         self.pipe = kernel32.CreateNamedPipeW(
             self.pipename,
             PIPE_ACCESS_DUPLEX,
-            PIPE_TYPE_MESSAGE | PIPE_READMODE_MESSAGE | PIPE_WAIT,
+            PIPE_TYPE_MESSAGE | PIPE_READMODE_MESSAGE | 0x00000001 if block_or_nonblock=='unblock' else 0x00000000,
             self.nMaxInstances,
             self.nOutBufferSize,
             self.nInBufferSize,
             0,
             None,
         )
         print("Waiting for client[s]")
@@ -135,15 +137,15 @@
                     ),  # GENERIC_READ | GENERIC_WRITE
                     0,
                     None,
                     ctypes.c_ulong(3),  # OPEN_EXISTING
                     0,
                     None,
                 )
-                self.mode = ctypes.c_ulong(PIPE_READMODE_MESSAGE)
+                self.mode = ctypes.c_ulong(PIPE_READMODE_MESSAGE )
                 self.res = ctypes.windll.kernel32.SetNamedPipeHandleState(
                     self.handle, ctypes.byref(self.mode), None, None
                 )
                 break
             except Exception as fe:
                 print(fe)
                 continue
@@ -187,15 +189,15 @@
         while True:
             try:
                 resp = (ctypes.c_char * buffer_size)()
                 bytes_read = ctypes.c_ulong(0)
                 ctypes.windll.kernel32.ReadFile(
                     self.handle,
                     resp,
-                    ctypes.sizeof(resp),
+                    buffer_size,
                     ctypes.byref(bytes_read),
                     None,
                 )
                 yield resp.value, bytes_read.value # value, and len of values read
             except Exception as e:
                 print("Pipe not found, waiting ...")
                 sleep(sleep_when_error)
```

### Comparing `pywinpipe-0.10/pywinpipe.egg-info/PKG-INFO` & `pywinpipe-0.11/pywinpipe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywinpipe
-Version: 0.10
+Version: 0.11
 Summary: pywinpipe - Fast data exchange between 2 processes (Windows only)
 Home-page: https://github.com/hansalemaos/pywinpipe
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: pipes,windows,named pipes,share,data
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pywinpipe-0.10/setup.py` & `pywinpipe-0.11/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''pywinpipe - Fast data exchange between 2 processes (Windows only)'''
 
 # Setting up
 setup(
     name="pywinpipe",
     version=VERSION,
     license='MIT',
```

