# Comparing `tmp/htcdaskgateway-0.1.6.tar.gz` & `tmp/htcdaskgateway-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htcdaskgateway-0.1.6.tar", last modified: Tue May 23 21:41:26 2023, max compression
+gzip compressed data, was "htcdaskgateway-0.1.7.tar", last modified: Tue May 23 21:56:38 2023, max compression
```

## Comparing `htcdaskgateway-0.1.6.tar` & `htcdaskgateway-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 macosta  (53128)     5063        0 2023-05-23 21:41:26.181128 htcdaskgateway-0.1.6/
--rw-r--r--   0 macosta  (53128)     5063     2673 2023-05-23 21:41:26.179128 htcdaskgateway-0.1.6/PKG-INFO
--rw-r--r--   0 macosta  (53128)     5063     2173 2022-11-02 21:00:56.000000 htcdaskgateway-0.1.6/README.md
--rw-r--r--   0 macosta  (53128)     5063       38 2023-05-23 21:41:26.181128 htcdaskgateway-0.1.6/setup.cfg
--rw-r--r--   0 macosta  (53128)     5063      786 2023-05-23 21:36:27.000000 htcdaskgateway-0.1.6/setup.py
-drwxr-xr-x   0 macosta  (53128)     5063        0 2023-05-23 21:41:26.170128 htcdaskgateway-0.1.6/src/
-drwxr-xr-x   0 macosta  (53128)     5063        0 2023-05-23 21:41:26.174128 htcdaskgateway-0.1.6/src/htcdaskgateway/
--rw-r--r--   0 macosta  (53128)     5063      153 2022-11-02 20:44:23.000000 htcdaskgateway-0.1.6/src/htcdaskgateway/__init__.py
--rw-r--r--   0 macosta  (53128)     5063     8750 2023-05-23 21:38:35.000000 htcdaskgateway-0.1.6/src/htcdaskgateway/cluster.py
--rw-r--r--   0 macosta  (53128)     5063     3286 2023-05-23 21:39:58.000000 htcdaskgateway-0.1.6/src/htcdaskgateway/gateway.py
-drwxr-xr-x   0 macosta  (53128)     5063        0 2023-05-23 21:41:26.178128 htcdaskgateway-0.1.6/src/htcdaskgateway.egg-info/
--rw-r--r--   0 macosta  (53128)     5063     2673 2023-05-23 21:41:25.000000 htcdaskgateway-0.1.6/src/htcdaskgateway.egg-info/PKG-INFO
--rw-r--r--   0 macosta  (53128)     5063      277 2023-05-23 21:41:25.000000 htcdaskgateway-0.1.6/src/htcdaskgateway.egg-info/SOURCES.txt
--rw-r--r--   0 macosta  (53128)     5063        1 2023-05-23 21:41:25.000000 htcdaskgateway-0.1.6/src/htcdaskgateway.egg-info/dependency_links.txt
--rw-r--r--   0 macosta  (53128)     5063       15 2023-05-23 21:41:25.000000 htcdaskgateway-0.1.6/src/htcdaskgateway.egg-info/top_level.txt
+drwxr-xr-x   0 macosta  (53128)     5063        0 2023-05-23 21:56:38.590211 htcdaskgateway-0.1.7/
+-rw-r--r--   0 macosta  (53128)     5063     2673 2023-05-23 21:56:38.588212 htcdaskgateway-0.1.7/PKG-INFO
+-rw-r--r--   0 macosta  (53128)     5063     2173 2022-11-02 21:00:56.000000 htcdaskgateway-0.1.7/README.md
+-rw-r--r--   0 macosta  (53128)     5063       38 2023-05-23 21:56:38.591211 htcdaskgateway-0.1.7/setup.cfg
+-rw-r--r--   0 macosta  (53128)     5063      786 2023-05-23 21:56:20.000000 htcdaskgateway-0.1.7/setup.py
+drwxr-xr-x   0 macosta  (53128)     5063        0 2023-05-23 21:56:38.559212 htcdaskgateway-0.1.7/src/
+drwxr-xr-x   0 macosta  (53128)     5063        0 2023-05-23 21:56:38.577211 htcdaskgateway-0.1.7/src/htcdaskgateway/
+-rw-r--r--   0 macosta  (53128)     5063      153 2022-11-02 20:44:23.000000 htcdaskgateway-0.1.7/src/htcdaskgateway/__init__.py
+-rw-r--r--   0 macosta  (53128)     5063     8750 2023-05-23 21:38:35.000000 htcdaskgateway-0.1.7/src/htcdaskgateway/cluster.py
+-rw-r--r--   0 macosta  (53128)     5063     3277 2023-05-23 21:56:09.000000 htcdaskgateway-0.1.7/src/htcdaskgateway/gateway.py
+drwxr-xr-x   0 macosta  (53128)     5063        0 2023-05-23 21:56:38.583212 htcdaskgateway-0.1.7/src/htcdaskgateway.egg-info/
+-rw-r--r--   0 macosta  (53128)     5063     2673 2023-05-23 21:56:38.000000 htcdaskgateway-0.1.7/src/htcdaskgateway.egg-info/PKG-INFO
+-rw-r--r--   0 macosta  (53128)     5063      277 2023-05-23 21:56:38.000000 htcdaskgateway-0.1.7/src/htcdaskgateway.egg-info/SOURCES.txt
+-rw-r--r--   0 macosta  (53128)     5063        1 2023-05-23 21:56:38.000000 htcdaskgateway-0.1.7/src/htcdaskgateway.egg-info/dependency_links.txt
+-rw-r--r--   0 macosta  (53128)     5063       15 2023-05-23 21:56:38.000000 htcdaskgateway-0.1.7/src/htcdaskgateway.egg-info/top_level.txt
```

### Comparing `htcdaskgateway-0.1.6/PKG-INFO` & `htcdaskgateway-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htcdaskgateway
-Version: 0.1.6
+Version: 0.1.7
 Summary: Launches a Dask Gateway cluster in K8s and joins HTCondor workers to it
 Home-page: https://github.com/mapsacosta/htcdaskgateway
 Author: Maria P. Acosta F./Fermilab EAF project
 Author-email: macosta@fnal.gov
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `htcdaskgateway-0.1.6/README.md` & `htcdaskgateway-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `htcdaskgateway-0.1.6/setup.py` & `htcdaskgateway-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="htcdaskgateway",
-    version="0.1.6",
+    version="0.1.7",
     author="Maria P. Acosta F./Fermilab EAF project",
     author_email="macosta@fnal.gov",
     description="Launches a Dask Gateway cluster in K8s and joins HTCondor workers to it",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache',
     url="https://github.com/mapsacosta/htcdaskgateway",
```

### Comparing `htcdaskgateway-0.1.6/src/htcdaskgateway/cluster.py` & `htcdaskgateway-0.1.7/src/htcdaskgateway/cluster.py`

 * *Files identical despite different names*

### Comparing `htcdaskgateway-0.1.6/src/htcdaskgateway/gateway.py` & `htcdaskgateway-0.1.7/src/htcdaskgateway/gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 logger = logging.getLogger("htcdaskgateway.HTCGateway")
 
 
 class HTCGateway(Gateway):
     
     def __init__(self, **kwargs):
         #address = kwargs.pop('address', 'http://172.30.92.196')
-        super().__init__(address, auth="jupyterhub", **kwargs)
+        super().__init__(auth="jupyterhub", **kwargs)
     
     def new_cluster(self, cluster_options=None, shutdown_on_close=True, **kwargs):
         """Submit a new cluster to the gateway, and wait for it to be started.
         Same as calling ``submit`` and ``connect`` in one go.
         Parameters
         ----------
         cluster_options : dask_gateway.options.Options, optional
```

### Comparing `htcdaskgateway-0.1.6/src/htcdaskgateway.egg-info/PKG-INFO` & `htcdaskgateway-0.1.7/src/htcdaskgateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htcdaskgateway
-Version: 0.1.6
+Version: 0.1.7
 Summary: Launches a Dask Gateway cluster in K8s and joins HTCondor workers to it
 Home-page: https://github.com/mapsacosta/htcdaskgateway
 Author: Maria P. Acosta F./Fermilab EAF project
 Author-email: macosta@fnal.gov
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

