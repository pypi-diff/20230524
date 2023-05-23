# Comparing `tmp/nriapp-1.1.18.tar.gz` & `tmp/nriapp-1.1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nriapp-1.1.18.tar", last modified: Tue May 16 13:48:03 2023, max compression
+gzip compressed data, was "nriapp-1.1.19.tar", last modified: Tue May 23 23:27:00 2023, max compression
```

## Comparing `nriapp-1.1.18.tar` & `nriapp-1.1.19.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 13:48:03.774419 nriapp-1.1.18/
--rw-rw-rw-   0        0        0     1084 2023-02-12 09:09:41.000000 nriapp-1.1.18/LICENSE
--rw-rw-rw-   0        0        0       57 2023-03-02 17:29:56.000000 nriapp-1.1.18/MANIFEST.in
--rw-rw-rw-   0        0        0      273 2023-05-16 13:48:03.774419 nriapp-1.1.18/PKG-INFO
--rw-rw-rw-   0        0        0        7 2023-02-12 09:19:02.000000 nriapp-1.1.18/README
--rw-rw-rw-   0        0        0      344 2023-05-06 05:28:38.000000 nriapp-1.1.18/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-05-16 13:48:03.774419 nriapp-1.1.18/setup.cfg
--rw-rw-rw-   0        0        0     1108 2023-05-16 13:47:53.000000 nriapp-1.1.18/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:48:03.493619 nriapp-1.1.18/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 13:48:03.618419 nriapp-1.1.18/src/nriapp/
--rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.18/src/nriapp/__init__.py
--rw-rw-rw-   0        0        0     3672 2023-02-02 00:29:38.000000 nriapp-1.1.18/src/nriapp/changelog.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 13:48:03.649619 nriapp-1.1.18/src/nriapp/config/
--rw-rw-rw-   0        0        0        2 2023-03-02 07:59:35.000000 nriapp-1.1.18/src/nriapp/config/__init__.py
--rw-rw-rw-   0        0        0       55 2023-03-02 07:59:35.000000 nriapp-1.1.18/src/nriapp/config/config.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:48:03.680819 nriapp-1.1.18/src/nriapp/core/
--rw-rw-rw-   0        0        0        0 2023-04-19 13:47:32.000000 nriapp-1.1.18/src/nriapp/core/__init__.py
--rw-rw-rw-   0        0        0     1520 2023-04-19 13:47:32.000000 nriapp-1.1.18/src/nriapp/core/abuseipdbapi.py
--rw-rw-rw-   0        0        0    20524 2023-05-16 04:22:17.000000 nriapp-1.1.18/src/nriapp/core/dataexplorer.py
--rw-rw-rw-   0        0        0    30935 2023-05-02 03:08:50.000000 nriapp-1.1.18/src/nriapp/core/msgraphapi.py
--rw-rw-rw-   0        0        0   104956 2023-05-16 05:49:17.000000 nriapp-1.1.18/src/nriapp/core/mssentinelapi.py
--rw-rw-rw-   0        0        0     6076 2023-04-19 13:47:32.000000 nriapp-1.1.18/src/nriapp/core/multifactor.py
--rw-rw-rw-   0        0        0      640 2023-04-19 13:47:32.000000 nriapp-1.1.18/src/nriapp/core/vtquery.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:48:03.712019 nriapp-1.1.18/src/nriapp/helper/
--rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.18/src/nriapp/helper/__init__.py
--rw-rw-rw-   0        0        0     5696 2023-04-19 13:47:32.000000 nriapp-1.1.18/src/nriapp/helper/doc.py
--rw-rw-rw-   0        0        0      246 2023-04-19 13:47:32.000000 nriapp-1.1.18/src/nriapp/helper/excel.py
--rw-rw-rw-   0        0        0     8397 2023-04-29 03:04:07.000000 nriapp-1.1.18/src/nriapp/helper/login.py
--rw-rw-rw-   0        0        0     2443 2023-04-19 13:47:32.000000 nriapp-1.1.18/src/nriapp/helper/pylog.py
--rw-rw-rw-   0        0        0     1247 2023-04-19 13:47:32.000000 nriapp-1.1.18/src/nriapp/helper/requestheader.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:48:03.618419 nriapp-1.1.18/src/nriapp/nriapp.egg-info/
--rw-rw-rw-   0        0        0      273 2023-05-16 13:48:02.000000 nriapp-1.1.18/src/nriapp/nriapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      989 2023-05-16 13:48:02.000000 nriapp-1.1.18/src/nriapp/nriapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 13:48:02.000000 nriapp-1.1.18/src/nriapp/nriapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-16 13:48:02.000000 nriapp-1.1.18/src/nriapp/nriapp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-05-16 13:48:02.000000 nriapp-1.1.18/src/nriapp/nriapp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    38168 2023-05-16 13:46:09.000000 nriapp-1.1.18/src/nriapp/nriapp.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:27:00.766621 nriapp-1.1.19/
+-rw-rw-rw-   0        0        0     1084 2023-02-12 09:09:41.000000 nriapp-1.1.19/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-03-02 17:29:56.000000 nriapp-1.1.19/MANIFEST.in
+-rw-rw-rw-   0        0        0      273 2023-05-23 23:27:00.766621 nriapp-1.1.19/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2023-02-12 09:19:02.000000 nriapp-1.1.19/README
+-rw-rw-rw-   0        0        0      344 2023-05-06 05:28:38.000000 nriapp-1.1.19/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-05-23 23:27:00.766621 nriapp-1.1.19/setup.cfg
+-rw-rw-rw-   0        0        0     1108 2023-05-23 23:26:42.000000 nriapp-1.1.19/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:27:00.657421 nriapp-1.1.19/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 23:27:00.735421 nriapp-1.1.19/src/nriapp/
+-rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.19/src/nriapp/__init__.py
+-rw-rw-rw-   0        0        0     3672 2023-02-02 00:29:38.000000 nriapp-1.1.19/src/nriapp/changelog.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 23:27:00.735421 nriapp-1.1.19/src/nriapp/config/
+-rw-rw-rw-   0        0        0        2 2023-03-02 07:59:35.000000 nriapp-1.1.19/src/nriapp/config/__init__.py
+-rw-rw-rw-   0        0        0       55 2023-03-02 07:59:35.000000 nriapp-1.1.19/src/nriapp/config/config.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:27:00.751021 nriapp-1.1.19/src/nriapp/core/
+-rw-rw-rw-   0        0        0        0 2023-04-19 13:47:32.000000 nriapp-1.1.19/src/nriapp/core/__init__.py
+-rw-rw-rw-   0        0        0     1520 2023-04-19 13:47:32.000000 nriapp-1.1.19/src/nriapp/core/abuseipdbapi.py
+-rw-rw-rw-   0        0        0    20524 2023-05-16 04:22:17.000000 nriapp-1.1.19/src/nriapp/core/dataexplorer.py
+-rw-rw-rw-   0        0        0    30935 2023-05-02 03:08:50.000000 nriapp-1.1.19/src/nriapp/core/msgraphapi.py
+-rw-rw-rw-   0        0        0   105457 2023-05-23 23:18:48.000000 nriapp-1.1.19/src/nriapp/core/mssentinelapi.py
+-rw-rw-rw-   0        0        0     6076 2023-04-19 13:47:32.000000 nriapp-1.1.19/src/nriapp/core/multifactor.py
+-rw-rw-rw-   0        0        0      640 2023-04-19 13:47:32.000000 nriapp-1.1.19/src/nriapp/core/vtquery.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:27:00.766621 nriapp-1.1.19/src/nriapp/helper/
+-rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.19/src/nriapp/helper/__init__.py
+-rw-rw-rw-   0        0        0     5696 2023-04-19 13:47:32.000000 nriapp-1.1.19/src/nriapp/helper/doc.py
+-rw-rw-rw-   0        0        0      246 2023-04-19 13:47:32.000000 nriapp-1.1.19/src/nriapp/helper/excel.py
+-rw-rw-rw-   0        0        0     8397 2023-04-29 03:04:07.000000 nriapp-1.1.19/src/nriapp/helper/login.py
+-rw-rw-rw-   0        0        0     2443 2023-04-19 13:47:32.000000 nriapp-1.1.19/src/nriapp/helper/pylog.py
+-rw-rw-rw-   0        0        0     1247 2023-04-19 13:47:32.000000 nriapp-1.1.19/src/nriapp/helper/requestheader.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:27:00.719821 nriapp-1.1.19/src/nriapp/nriapp.egg-info/
+-rw-rw-rw-   0        0        0      273 2023-05-23 23:26:59.000000 nriapp-1.1.19/src/nriapp/nriapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      989 2023-05-23 23:26:59.000000 nriapp-1.1.19/src/nriapp/nriapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 23:26:59.000000 nriapp-1.1.19/src/nriapp/nriapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-23 23:26:59.000000 nriapp-1.1.19/src/nriapp/nriapp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-05-23 23:26:59.000000 nriapp-1.1.19/src/nriapp/nriapp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    38168 2023-05-16 13:46:09.000000 nriapp-1.1.19/src/nriapp/nriapp.py
```

### Comparing `nriapp-1.1.18/LICENSE` & `nriapp-1.1.19/LICENSE`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.18/setup.py` & `nriapp-1.1.19/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 #with open('requirements.txt') as f:
 #    requirements = f.read().splitlines()
 
 
 setup(
    name='nriapp',
-   version='1.1.18',
+   version='1.1.19',
    description='This is an internal tool for crawling MS 365 Defender web with NRI',
     license='MIT',
    author='Llallum Victoria',
    author_email='llallumvictoria@gmail.com',
 #   packages=find_packages('src'),
    package_dir = {'':'src/nriapp'},
```

### Comparing `nriapp-1.1.18/src/nriapp/changelog.txt` & `nriapp-1.1.19/src/nriapp/changelog.txt`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.18/src/nriapp/core/abuseipdbapi.py` & `nriapp-1.1.19/src/nriapp/core/abuseipdbapi.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.18/src/nriapp/core/dataexplorer.py` & `nriapp-1.1.19/src/nriapp/core/dataexplorer.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.18/src/nriapp/core/msgraphapi.py` & `nriapp-1.1.19/src/nriapp/core/msgraphapi.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.18/src/nriapp/core/mssentinelapi.py` & `nriapp-1.1.19/src/nriapp/core/mssentinelapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1856,14 +1856,32 @@
         if len(hash) != 40:
             info.update({"sha256" : hash.lower()})
         else:
             info.update({"sha1" : hash.lower()})
         
         return info
 
+    def get_device_info(self, senseMachineId):
+
+        machine_info = "https://security.microsoft.com/apiproxy/mtp/getMachine/machines"
+
+        params = {
+            "machineId"         : senseMachineId,
+            "idType"            : "SenseMachineId",
+            "readFromCache"     : "true",
+            "lookingBackIndays" : 180
+            }
+
+        response = self.tryrequest(machine_info, params=params)
+
+        info = json.loads(response.text)
+
+        return info
+
+
     def get_device_inventory(self, pageIndex=1):
 
         device_totals = "https://security.microsoft.com/apiproxy/mtp/k8s/machines"
 
         params = {
             "lookingBackIndays" : 30,
             "deviceCategories"  : "IoT,Unknown,Endpoint,NetworkDevice",
```

### Comparing `nriapp-1.1.18/src/nriapp/core/multifactor.py` & `nriapp-1.1.19/src/nriapp/core/multifactor.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.18/src/nriapp/core/vtquery.py` & `nriapp-1.1.19/src/nriapp/core/vtquery.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.18/src/nriapp/helper/doc.py` & `nriapp-1.1.19/src/nriapp/helper/doc.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.18/src/nriapp/helper/login.py` & `nriapp-1.1.19/src/nriapp/helper/login.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.18/src/nriapp/helper/pylog.py` & `nriapp-1.1.19/src/nriapp/helper/pylog.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.18/src/nriapp/helper/requestheader.py` & `nriapp-1.1.19/src/nriapp/helper/requestheader.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.18/src/nriapp/nriapp.egg-info/SOURCES.txt` & `nriapp-1.1.19/src/nriapp/nriapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.18/src/nriapp/nriapp.py` & `nriapp-1.1.19/src/nriapp/nriapp.py`

 * *Files identical despite different names*

