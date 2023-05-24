# Comparing `tmp/htcdaskgateway-0.1.8.tar.gz` & `tmp/htcdaskgateway-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htcdaskgateway-0.1.8.tar", last modified: Tue May 23 22:30:41 2023, max compression
+gzip compressed data, was "htcdaskgateway-0.1.9.tar", last modified: Wed May 24 01:27:06 2023, max compression
```

## Comparing `htcdaskgateway-0.1.8.tar` & `htcdaskgateway-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 macosta  (53128)     5063        0 2023-05-23 22:30:41.232503 htcdaskgateway-0.1.8/
--rw-r--r--   0 macosta  (53128)     5063     2673 2023-05-23 22:30:41.125503 htcdaskgateway-0.1.8/PKG-INFO
--rw-r--r--   0 macosta  (53128)     5063     2173 2022-11-02 21:00:56.000000 htcdaskgateway-0.1.8/README.md
--rw-r--r--   0 macosta  (53128)     5063       38 2023-05-23 22:30:41.234502 htcdaskgateway-0.1.8/setup.cfg
--rw-r--r--   0 macosta  (53128)     5063      786 2023-05-23 22:30:14.000000 htcdaskgateway-0.1.8/setup.py
-drwxr-xr-x   0 macosta  (53128)     5063        0 2023-05-23 22:30:41.006503 htcdaskgateway-0.1.8/src/
-drwxr-xr-x   0 macosta  (53128)     5063        0 2023-05-23 22:30:41.068503 htcdaskgateway-0.1.8/src/htcdaskgateway/
--rw-r--r--   0 macosta  (53128)     5063      153 2022-11-02 20:44:23.000000 htcdaskgateway-0.1.8/src/htcdaskgateway/__init__.py
--rw-r--r--   0 macosta  (53128)     5063     8750 2023-05-23 22:30:02.000000 htcdaskgateway-0.1.8/src/htcdaskgateway/cluster.py
--rw-r--r--   0 macosta  (53128)     5063     3285 2023-05-23 22:29:59.000000 htcdaskgateway-0.1.8/src/htcdaskgateway/gateway.py
-drwxr-xr-x   0 macosta  (53128)     5063        0 2023-05-23 22:30:41.123503 htcdaskgateway-0.1.8/src/htcdaskgateway.egg-info/
--rw-r--r--   0 macosta  (53128)     5063     2673 2023-05-23 22:30:38.000000 htcdaskgateway-0.1.8/src/htcdaskgateway.egg-info/PKG-INFO
--rw-r--r--   0 macosta  (53128)     5063      277 2023-05-23 22:30:39.000000 htcdaskgateway-0.1.8/src/htcdaskgateway.egg-info/SOURCES.txt
--rw-r--r--   0 macosta  (53128)     5063        1 2023-05-23 22:30:38.000000 htcdaskgateway-0.1.8/src/htcdaskgateway.egg-info/dependency_links.txt
--rw-r--r--   0 macosta  (53128)     5063       15 2023-05-23 22:30:39.000000 htcdaskgateway-0.1.8/src/htcdaskgateway.egg-info/top_level.txt
+drwxr-xr-x   0 macosta  (53128)     5063        0 2023-05-24 01:27:06.818981 htcdaskgateway-0.1.9/
+-rw-r--r--   0 macosta  (53128)     5063     2673 2023-05-24 01:27:06.817981 htcdaskgateway-0.1.9/PKG-INFO
+-rw-r--r--   0 macosta  (53128)     5063     2173 2022-11-02 21:00:56.000000 htcdaskgateway-0.1.9/README.md
+-rw-r--r--   0 macosta  (53128)     5063       38 2023-05-24 01:27:06.818981 htcdaskgateway-0.1.9/setup.cfg
+-rw-r--r--   0 macosta  (53128)     5063      786 2023-05-24 01:26:57.000000 htcdaskgateway-0.1.9/setup.py
+drwxr-xr-x   0 macosta  (53128)     5063        0 2023-05-24 01:27:06.805981 htcdaskgateway-0.1.9/src/
+drwxr-xr-x   0 macosta  (53128)     5063        0 2023-05-24 01:27:06.812981 htcdaskgateway-0.1.9/src/htcdaskgateway/
+-rw-r--r--   0 macosta  (53128)     5063      153 2022-11-02 20:44:23.000000 htcdaskgateway-0.1.9/src/htcdaskgateway/__init__.py
+-rw-r--r--   0 macosta  (53128)     5063     8750 2023-05-24 01:26:18.000000 htcdaskgateway-0.1.9/src/htcdaskgateway/cluster.py
+-rw-r--r--   0 macosta  (53128)     5063     3319 2023-05-24 01:26:45.000000 htcdaskgateway-0.1.9/src/htcdaskgateway/gateway.py
+drwxr-xr-x   0 macosta  (53128)     5063        0 2023-05-24 01:27:06.815981 htcdaskgateway-0.1.9/src/htcdaskgateway.egg-info/
+-rw-r--r--   0 macosta  (53128)     5063     2673 2023-05-24 01:27:06.000000 htcdaskgateway-0.1.9/src/htcdaskgateway.egg-info/PKG-INFO
+-rw-r--r--   0 macosta  (53128)     5063      277 2023-05-24 01:27:06.000000 htcdaskgateway-0.1.9/src/htcdaskgateway.egg-info/SOURCES.txt
+-rw-r--r--   0 macosta  (53128)     5063        1 2023-05-24 01:27:06.000000 htcdaskgateway-0.1.9/src/htcdaskgateway.egg-info/dependency_links.txt
+-rw-r--r--   0 macosta  (53128)     5063       15 2023-05-24 01:27:06.000000 htcdaskgateway-0.1.9/src/htcdaskgateway.egg-info/top_level.txt
```

### Comparing `htcdaskgateway-0.1.8/PKG-INFO` & `htcdaskgateway-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htcdaskgateway
-Version: 0.1.8
+Version: 0.1.9
 Summary: Launches a Dask Gateway cluster in K8s and joins HTCondor workers to it
 Home-page: https://github.com/mapsacosta/htcdaskgateway
 Author: Maria P. Acosta F./Fermilab EAF project
 Author-email: macosta@fnal.gov
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `htcdaskgateway-0.1.8/README.md` & `htcdaskgateway-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `htcdaskgateway-0.1.8/setup.py` & `htcdaskgateway-0.1.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="htcdaskgateway",
-    version="0.1.8",
+    version="0.1.9",
     author="Maria P. Acosta F./Fermilab EAF project",
     author_email="macosta@fnal.gov",
     description="Launches a Dask Gateway cluster in K8s and joins HTCondor workers to it",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache',
     url="https://github.com/mapsacosta/htcdaskgateway",
```

### Comparing `htcdaskgateway-0.1.8/src/htcdaskgateway/cluster.py` & `htcdaskgateway-0.1.9/src/htcdaskgateway/cluster.py`

 * *Files identical despite different names*

### Comparing `htcdaskgateway-0.1.8/src/htcdaskgateway/gateway.py` & `htcdaskgateway-0.1.9/src/htcdaskgateway/gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
             ``cluster_options`` for more information.
         Returns
         -------
         cluster : GatewayCluster
         """
         logger.info(" Creating HTCGatewayCluster ")
         return HTCGatewayCluster(
+            address=self.address,
             proxy_address=self.proxy_address,
             public_address=self._public_address,
             auth=self.auth,
             asynchronous=self.asynchronous,
             loop=self.loop,
             cluster_options=cluster_options,
             shutdown_on_close=shutdown_on_close,
```

### Comparing `htcdaskgateway-0.1.8/src/htcdaskgateway.egg-info/PKG-INFO` & `htcdaskgateway-0.1.9/src/htcdaskgateway.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htcdaskgateway
-Version: 0.1.8
+Version: 0.1.9
 Summary: Launches a Dask Gateway cluster in K8s and joins HTCondor workers to it
 Home-page: https://github.com/mapsacosta/htcdaskgateway
 Author: Maria P. Acosta F./Fermilab EAF project
 Author-email: macosta@fnal.gov
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

