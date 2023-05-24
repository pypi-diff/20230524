# Comparing `tmp/NamasteiG-0.3.0.tar.gz` & `tmp/NamasteiG-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NamasteiG-0.3.0.tar", last modified: Mon May  8 08:33:00 2023, max compression
+gzip compressed data, was "NamasteiG-0.3.1.tar", last modified: Wed May 24 18:45:36 2023, max compression
```

## Comparing `NamasteiG-0.3.0.tar` & `NamasteiG-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 08:33:00.391506 NamasteiG-0.3.0/
--rw-rw-rw-   0        0        0     1077 2022-12-10 14:24:59.000000 NamasteiG-0.3.0/LICENSE
--rw-rw-rw-   0        0        0      838 2023-05-08 08:33:00.391506 NamasteiG-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      326 2022-12-14 19:04:09.000000 NamasteiG-0.3.0/README.md
--rw-rw-rw-   0        0        0      593 2023-05-08 08:32:44.000000 NamasteiG-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 08:33:00.393010 NamasteiG-0.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-08 08:33:00.376439 NamasteiG-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-08 08:33:00.383986 NamasteiG-0.3.0/src/NamasteiG/
--rw-rw-rw-   0        0        0     8405 2023-04-16 13:01:55.000000 NamasteiG-0.3.0/src/NamasteiG/VerifyData.py
--rw-rw-rw-   0        0        0    27983 2023-05-08 08:32:23.000000 NamasteiG-0.3.0/src/NamasteiG/__init__.py
--rw-rw-rw-   0        0        0      501 2023-04-21 14:30:38.000000 NamasteiG-0.3.0/src/NamasteiG/example.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:33:00.390409 NamasteiG-0.3.0/src/NamasteiG.egg-info/
--rw-rw-rw-   0        0        0      838 2023-05-08 08:33:00.000000 NamasteiG-0.3.0/src/NamasteiG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-05-08 08:33:00.000000 NamasteiG-0.3.0/src/NamasteiG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 08:33:00.000000 NamasteiG-0.3.0/src/NamasteiG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-08 08:33:00.000000 NamasteiG-0.3.0/src/NamasteiG.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 18:45:36.660772 NamasteiG-0.3.1/
+-rw-rw-rw-   0        0        0     1077 2022-12-10 14:24:59.000000 NamasteiG-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0      838 2023-05-24 18:45:36.659315 NamasteiG-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2022-12-14 19:04:09.000000 NamasteiG-0.3.1/README.md
+-rw-rw-rw-   0        0        0      593 2023-05-24 18:45:26.000000 NamasteiG-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 18:45:36.660772 NamasteiG-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 18:45:36.650115 NamasteiG-0.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 18:45:36.655624 NamasteiG-0.3.1/src/NamasteiG/
+-rw-rw-rw-   0        0        0     8405 2023-04-16 13:01:55.000000 NamasteiG-0.3.1/src/NamasteiG/VerifyData.py
+-rw-rw-rw-   0        0        0    27983 2023-05-24 18:42:53.000000 NamasteiG-0.3.1/src/NamasteiG/__init__.py
+-rw-rw-rw-   0        0        0      501 2023-04-21 14:30:38.000000 NamasteiG-0.3.1/src/NamasteiG/example.py
+drwxrwxrwx   0        0        0        0 2023-05-24 18:45:36.659315 NamasteiG-0.3.1/src/NamasteiG.egg-info/
+-rw-rw-rw-   0        0        0      838 2023-05-24 18:45:36.000000 NamasteiG-0.3.1/src/NamasteiG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-05-24 18:45:36.000000 NamasteiG-0.3.1/src/NamasteiG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 18:45:36.000000 NamasteiG-0.3.1/src/NamasteiG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-24 18:45:36.000000 NamasteiG-0.3.1/src/NamasteiG.egg-info/top_level.txt
```

### Comparing `NamasteiG-0.3.0/LICENSE` & `NamasteiG-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `NamasteiG-0.3.0/PKG-INFO` & `NamasteiG-0.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NamasteiG
-Version: 0.3.0
+Version: 0.3.1
 Summary: Most PowerFull Instagram Library
 Author-email: Abhinav Bhardwaj <abhinav.bhardwaj.56614@gmail.com>
 Project-URL: Homepage, https://t.me/namastelibrary
 Project-URL: Bug Tracker, https://t.me/namastehackers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NamasteiG-0.3.0/pyproject.toml` & `NamasteiG-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NamasteiG"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Abhinav Bhardwaj", email="abhinav.bhardwaj.56614@gmail.com" },
 ]
 description = "Most PowerFull Instagram Library"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `NamasteiG-0.3.0/src/NamasteiG/VerifyData.py` & `NamasteiG-0.3.1/src/NamasteiG/VerifyData.py`

 * *Files identical despite different names*

### Comparing `NamasteiG-0.3.0/src/NamasteiG/__init__.py` & `NamasteiG-0.3.1/src/NamasteiG/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,16 +53,16 @@
         self.PigeonSession = f'UFS-{str(uuid.uuid4())}-0'
         self.IgDeviceId = uuid.uuid4()
         self.IgFamilyDeviceId = uuid.uuid4()
         self.AndroidID = f'android-{secrets.token_hex(8)}'
         self.Waterfall= uuid.uuid4()
         self.Qpl=uuid.uuid4()
         rnd=str(random.randint(150, 999))
-        self.UserAgent = "Instagram 281.0.0.19.105 Android (" + ["23/6.0", "24/7.0", "25/7.1.1", "26/8.0", "27/8.1", "28/9.0"][random.randint(0, 5)] + "; " + str(random.randint(100, 1300)) + "dpi; " + str(random.randint(200, 2000)) + "x" + str(random.randint(200, 2000)) + "; " + ["SAMSUNG", "HUAWEI", "LGE/lge", "HTC", "ASUS", "ZTE", "ONEPLUS", "XIAOMI", "OPPO", "VIVO", "SONY", "REALME"][random.randint(0, 11)] + "; SM-T" + rnd + "; SM-T" + rnd + "; qcom; en_US; 470774561)"
-        self.Blockversion = 'c0a45b461eed836c64d795e59fde36963cf2dd6a6d58c06a50d936bd9f62180d'
+        self.UserAgent = "Instagram 283.0.0.20.105 Android (" + ["23/6.0", "24/7.0", "25/7.1.1", "26/8.0", "27/8.1", "28/9.0"][random.randint(0, 5)] + "; " + str(random.randint(100, 1300)) + "dpi; " + str(random.randint(200, 2000)) + "x" + str(random.randint(200, 2000)) + "; " + ["SAMSUNG", "HUAWEI", "LGE/lge", "HTC", "ASUS", "ZTE", "ONEPLUS", "XIAOMI", "OPPO", "VIVO", "SONY", "REALME"][random.randint(0, 11)] + "; SM-T" + rnd + "; SM-T" + rnd + "; qcom; en_US; 475221265)"
+        self.Blockversion = 'f5fbf62cc3c51dc0e6f4ffd3a79e0c5929ae0b8af58c54acd1e186871a92fb27'
         self.proxy = Proxy
 
     def generate_jazoest(self,symbols):
         amount = sum(ord(s) for s in symbols)
         return f'2{amount}'
 
     def GetMid(self):
```

### Comparing `NamasteiG-0.3.0/src/NamasteiG.egg-info/PKG-INFO` & `NamasteiG-0.3.1/src/NamasteiG.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NamasteiG
-Version: 0.3.0
+Version: 0.3.1
 Summary: Most PowerFull Instagram Library
 Author-email: Abhinav Bhardwaj <abhinav.bhardwaj.56614@gmail.com>
 Project-URL: Homepage, https://t.me/namastelibrary
 Project-URL: Bug Tracker, https://t.me/namastehackers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

