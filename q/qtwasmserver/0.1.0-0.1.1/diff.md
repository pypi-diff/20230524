# Comparing `tmp/qtwasmserver-0.1.0.tar.gz` & `tmp/qtwasmserver-0.1.1.tar.gz`

## Comparing `qtwasmserver-0.1.0.tar` & `qtwasmserver-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 qtwasmserver-0.1.0/build
--rwxr-xr-x   0        0        0     9805 2020-02-02 00:00:00.000000 qtwasmserver-0.1.0/src/qtwasmserver/qtwasmserver.py
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 qtwasmserver-0.1.0/src/qtwasmserver/setup.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 qtwasmserver-0.1.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 qtwasmserver-0.1.0/LICENSE
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 qtwasmserver-0.1.0/README.md
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 qtwasmserver-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 qtwasmserver-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 qtwasmserver-0.1.1/build
+-rwxr-xr-x   0        0        0     9805 2020-02-02 00:00:00.000000 qtwasmserver-0.1.1/src/qtwasmserver/qtwasmserver.py
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 qtwasmserver-0.1.1/src/qtwasmserver/setup.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 qtwasmserver-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 qtwasmserver-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 qtwasmserver-0.1.1/README.md
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 qtwasmserver-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 qtwasmserver-0.1.1/PKG-INFO
```

### Comparing `qtwasmserver-0.1.0/src/qtwasmserver/qtwasmserver.py` & `qtwasmserver-0.1.1/src/qtwasmserver/qtwasmserver.py`

 * *Files identical despite different names*

### Comparing `qtwasmserver-0.1.0/LICENSE` & `qtwasmserver-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qtwasmserver-0.1.0/README.md` & `qtwasmserver-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 pip install qtwasmserver
 
 Usage exmaples:
 
     qtwasmserver                            # Start server on localhost, serve $CWD
     qtwasmserver /path/to/wasm/builds       # Specify web root path
-    qtwasmserver -p 1080                    # Start server(s) on a spesific port
+    qtwasmserver -p 1080                    # Start server(s) on custom port
     qtwasmserver --all-interfaces           # Start server(s) on all network interfaces
     qtwasmserver -a 10.0.0.2                # Start server on specific address, in addition to localhost
     qtwasmserver --cross-origin-isolation   # Enable cross-origin isolation mode for multithreading
     qtwasmserver -h                         # Show help
 
 # Using mkcert
```

### Comparing `qtwasmserver-0.1.0/pyproject.toml` & `qtwasmserver-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "qtwasmserver"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Morten Sørvig", email="msorvig@gmail.com" },
 ]
 description = "Development Web Server for Qt for Webassembly"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qtwasmserver-0.1.0/PKG-INFO` & `qtwasmserver-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtwasmserver
-Version: 0.1.0
+Version: 0.1.1
 Summary: Development Web Server for Qt for Webassembly
 Project-URL: Homepage, https://github.com/msorvig/qtwasmserver
 Project-URL: Bug Tracker, https://github.com/msorvig/qtwasmserver/issues
 Author-email: Morten Sørvig <msorvig@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -53,15 +53,15 @@
 
 pip install qtwasmserver
 
 Usage exmaples:
 
     qtwasmserver                            # Start server on localhost, serve $CWD
     qtwasmserver /path/to/wasm/builds       # Specify web root path
-    qtwasmserver -p 1080                    # Start server(s) on a spesific port
+    qtwasmserver -p 1080                    # Start server(s) on custom port
     qtwasmserver --all-interfaces           # Start server(s) on all network interfaces
     qtwasmserver -a 10.0.0.2                # Start server on specific address, in addition to localhost
     qtwasmserver --cross-origin-isolation   # Enable cross-origin isolation mode for multithreading
     qtwasmserver -h                         # Show help
 
 # Using mkcert
```

