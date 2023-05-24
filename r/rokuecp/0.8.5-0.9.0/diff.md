# Comparing `tmp/rokuecp-0.8.5.tar.gz` & `tmp/rokuecp-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rokuecp-0.8.5.tar", last modified: Tue Nov 23 20:41:42 2021, max compression
+gzip compressed data, was "rokuecp-0.9.0.tar", last modified: Sun Jan  2 20:33:05 2022, max compression
```

## Comparing `rokuecp-0.8.5.tar` & `rokuecp-0.9.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 20:41:42.512028 rokuecp-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2021-11-23 20:41:33.000000 rokuecp-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      102 2021-11-23 20:41:33.000000 rokuecp-0.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2021-11-23 20:41:42.512028 rokuecp-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      630 2021-11-23 20:41:33.000000 rokuecp-0.8.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       45 2021-11-23 20:41:33.000000 rokuecp-0.8.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 20:41:42.508027 rokuecp-0.8.5/rokuecp/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2021-11-23 20:41:33.000000 rokuecp-0.8.5/rokuecp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-11-23 20:41:33.000000 rokuecp-0.8.5/rokuecp/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3679 2021-11-23 20:41:33.000000 rokuecp-0.8.5/rokuecp/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2021-11-23 20:41:33.000000 rokuecp-0.8.5/rokuecp/const.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2021-11-23 20:41:33.000000 rokuecp-0.8.5/rokuecp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      844 2021-11-23 20:41:33.000000 rokuecp-0.8.5/rokuecp/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     7064 2021-11-23 20:41:33.000000 rokuecp-0.8.5/rokuecp/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2021-11-23 20:41:33.000000 rokuecp-0.8.5/rokuecp/resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)     7304 2021-11-23 20:41:33.000000 rokuecp-0.8.5/rokuecp/rokuecp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-23 20:41:42.512028 rokuecp-0.8.5/rokuecp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2021-11-23 20:41:42.000000 rokuecp-0.8.5/rokuecp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      415 2021-11-23 20:41:42.000000 rokuecp-0.8.5/rokuecp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-23 20:41:42.000000 rokuecp-0.8.5/rokuecp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-23 20:41:42.000000 rokuecp-0.8.5/rokuecp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       45 2021-11-23 20:41:42.000000 rokuecp-0.8.5/rokuecp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-11-23 20:41:42.000000 rokuecp-0.8.5/rokuecp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-23 20:41:42.512028 rokuecp-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1713 2021-11-23 20:41:33.000000 rokuecp-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:33:05.402109 rokuecp-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-01-02 20:32:54.000000 rokuecp-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-01-02 20:32:54.000000 rokuecp-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1426 2022-01-02 20:33:05.402109 rokuecp-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      630 2022-01-02 20:32:54.000000 rokuecp-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-01-02 20:32:54.000000 rokuecp-0.9.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:33:05.402109 rokuecp-0.9.0/rokuecp/
+-rw-r--r--   0 runner    (1001) docker     (121)      140 2022-01-02 20:32:54.000000 rokuecp-0.9.0/rokuecp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-01-02 20:32:54.000000 rokuecp-0.9.0/rokuecp/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-01-02 20:32:54.000000 rokuecp-0.9.0/rokuecp/const.py
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-01-02 20:32:54.000000 rokuecp-0.9.0/rokuecp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      844 2022-01-02 20:32:54.000000 rokuecp-0.9.0/rokuecp/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7380 2022-01-02 20:32:54.000000 rokuecp-0.9.0/rokuecp/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-01-02 20:32:54.000000 rokuecp-0.9.0/rokuecp/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10225 2022-01-02 20:32:54.000000 rokuecp-0.9.0/rokuecp/rokuecp.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:33:05.402109 rokuecp-0.9.0/rokuecp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1426 2022-01-02 20:33:05.000000 rokuecp-0.9.0/rokuecp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2022-01-02 20:33:05.000000 rokuecp-0.9.0/rokuecp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-02 20:33:05.000000 rokuecp-0.9.0/rokuecp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-02 20:33:05.000000 rokuecp-0.9.0/rokuecp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-01-02 20:33:05.000000 rokuecp-0.9.0/rokuecp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-01-02 20:33:05.000000 rokuecp-0.9.0/rokuecp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-02 20:33:05.402109 rokuecp-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-01-02 20:32:54.000000 rokuecp-0.9.0/setup.py
```

### Comparing `rokuecp-0.8.5/LICENSE` & `rokuecp-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rokuecp-0.8.5/PKG-INFO` & `rokuecp-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: rokuecp
-Version: 0.8.5
+Version: 0.9.0
 Summary: Asynchronous Python client for Roku (ECP).
 Home-page: https://github.com/ctalkington/python-rokuecp
 Author: Chris Talkington
 Author-email: chris@talkingtontech.com
 License: MIT license
 Keywords: roku,api,async,client,ecp
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python: Roku (ECP) Client
```

### Comparing `rokuecp-0.8.5/README.md` & `rokuecp-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `rokuecp-0.8.5/rokuecp/const.py` & `rokuecp-0.9.0/rokuecp/const.py`

 * *Files identical despite different names*

### Comparing `rokuecp-0.8.5/rokuecp/helpers.py` & `rokuecp-0.9.0/rokuecp/helpers.py`

 * *Files identical despite different names*

### Comparing `rokuecp-0.8.5/rokuecp/models.py` & `rokuecp-0.9.0/rokuecp/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,27 +55,31 @@
     serial_number: str
     version: str
     network_type: Optional[str] = None
     network_name: Optional[str] = None
     ethernet_support: Optional[bool] = None
     ethernet_mac: Optional[str] = None
     wifi_mac: Optional[str] = None
+    supports_airplay: Optional[bool] = None
+    supports_find_remote: Optional[bool] = None
     supports_private_listening: Optional[bool] = None
     headphones_connected: Optional[bool] = None
 
     @staticmethod
     def from_dict(data: dict):
         """Return Info object from Roku API response."""
         device_type = "box"
 
         if data.get("is-tv", "false") == "true":
             device_type = "tv"
         elif data.get("is-stick", "false") == "true":
             device_type = "stick"
 
+        airplay = data.get("supports-airplay", "false") == "true"
+        find_remote = data.get("supports-find-remote", "false") == "true"
         private_listening = data.get("supports-private-listening", "false") == "true"
 
         return Info(
             name=data.get("user-device-name", None),
             brand=data.get("vendor-name", "Roku"),
             device_type=device_type,
             device_location=data.get("user-device-location", None),
@@ -84,14 +88,16 @@
             network_type=data.get("network-type", None),
             network_name=data.get("network-name", None),
             serial_number=data.get("serial-number", None),
             version=data.get("software-version", None),
             ethernet_support=data.get("supports-ethernet", "false") == "true",
             ethernet_mac=data.get("ethernet-mac", None),
             wifi_mac=data.get("wifi-mac", None),
+            supports_airplay=airplay,
+            supports_find_remote=find_remote,
             supports_private_listening=private_listening,
             headphones_connected=data.get("headphones-connected", "false") == "true",
         )
 
 
 @dataclass(frozen=True)
 class Channel:
```

### Comparing `rokuecp-0.8.5/rokuecp/resolver.py` & `rokuecp-0.9.0/rokuecp/resolver.py`

 * *Files identical despite different names*

### Comparing `rokuecp-0.8.5/rokuecp.egg-info/PKG-INFO` & `rokuecp-0.9.0/rokuecp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: rokuecp
-Version: 0.8.5
+Version: 0.9.0
 Summary: Asynchronous Python client for Roku (ECP).
 Home-page: https://github.com/ctalkington/python-rokuecp
 Author: Chris Talkington
 Author-email: chris@talkingtontech.com
 License: MIT license
 Keywords: roku,api,async,client,ecp
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python: Roku (ECP) Client
```

### Comparing `rokuecp-0.8.5/setup.py` & `rokuecp-0.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,38 +14,43 @@
     return re.search(regex, read(*path)).group("version")
 
 
 def read(*parts):
     """Read file."""
     filename = os.path.join(os.path.abspath(os.path.dirname(__file__)), *parts)
     sys.stdout.write(filename)
-    with open(filename, encoding="utf-8", mode="rt") as fp:
+    with open(filename, encoding="utf-8") as fp:
         return fp.read()
 
 
-with open("README.md") as readme_file:
+with open("README.md", encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 setup(
     author="Chris Talkington",
     author_email="chris@talkingtontech.com",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Framework :: AsyncIO",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     description="Asynchronous Python client for Roku (ECP).",
     include_package_data=True,
-    install_requires=list(val.strip() for val in open("requirements.txt")),
+    install_requires=list(
+        val.strip()
+        for val in open(  # pylint: disable=consider-using-with
+            "requirements.txt", encoding="utf-8"
+        )
+    ),
     keywords=["roku", "api", "async", "client", "ecp"],
     license="MIT license",
     long_description_content_type="text/markdown",
     long_description=readme,
     name="rokuecp",
     packages=find_packages(include=["rokuecp"]),
     test_suite="tests",
```

