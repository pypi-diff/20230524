# Comparing `tmp/FCSAPIAccessSDK-1.1.1.tar.gz` & `tmp/FCSAPIAccessSDK-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FCSAPIAccessSDK-1.1.1.tar", last modified: Wed May 24 14:10:06 2023, max compression
+gzip compressed data, was "FCSAPIAccessSDK-1.1.2.tar", last modified: Wed May 24 14:21:21 2023, max compression
```

## Comparing `FCSAPIAccessSDK-1.1.1.tar` & `FCSAPIAccessSDK-1.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 14:10:06.259603 FCSAPIAccessSDK-1.1.1/
-drwxrwxrwx   0        0        0        0 2023-05-24 14:10:06.234500 FCSAPIAccessSDK-1.1.1/FCSAPIAccess/
--rw-rw-rw-   0        0        0      127 2022-03-16 06:17:23.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccess/__init__.py
--rw-rw-rw-   0        0        0     5049 2023-05-24 13:53:43.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccess/api_access.py
--rw-rw-rw-   0        0        0     9757 2023-05-24 13:43:59.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccess/exceptions.py
--rw-rw-rw-   0        0        0     6169 2023-05-24 14:08:06.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccess/fcs_monitoring.py
--rw-rw-rw-   0        0        0     9535 2023-05-24 14:08:07.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccess/fcs_notification.py
--rw-rw-rw-   0        0        0    68100 2023-05-24 14:08:06.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccess/fcs_project.py
--rw-rw-rw-   0        0        0     6073 2023-05-24 14:08:07.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccess/fcs_translation.py
--rw-rw-rw-   0        0        0     5071 2023-05-19 20:26:24.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccess/scope.py
-drwxrwxrwx   0        0        0        0 2023-05-24 14:10:06.256609 FCSAPIAccessSDK-1.1.1/FCSAPIAccessSDK.egg-info/
--rw-rw-rw-   0        0        0     1887 2023-05-24 14:10:06.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccessSDK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      474 2023-05-24 14:10:06.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccessSDK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 14:10:06.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccessSDK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-24 14:10:06.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccessSDK.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-24 14:10:06.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccessSDK.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2022-03-16 05:36:31.000000 FCSAPIAccessSDK-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     1887 2023-05-24 14:10:06.260604 FCSAPIAccessSDK-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      765 2022-04-14 20:12:51.000000 FCSAPIAccessSDK-1.1.1/README.md
--rw-rw-rw-   0        0        0       86 2023-05-24 14:10:06.267410 FCSAPIAccessSDK-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1453 2023-05-24 14:09:46.000000 FCSAPIAccessSDK-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 14:10:06.257609 FCSAPIAccessSDK-1.1.1/tests/
--rw-rw-rw-   0        0        0     1203 2022-04-14 20:07:43.000000 FCSAPIAccessSDK-1.1.1/tests/test_auth.py
+drwxrwxrwx   0        0        0        0 2023-05-24 14:21:21.112034 FCSAPIAccessSDK-1.1.2/
+drwxrwxrwx   0        0        0        0 2023-05-24 14:21:21.089764 FCSAPIAccessSDK-1.1.2/FCSAPIAccess/
+-rw-rw-rw-   0        0        0      127 2022-03-16 06:17:23.000000 FCSAPIAccessSDK-1.1.2/FCSAPIAccess/__init__.py
+-rw-rw-rw-   0        0        0     5265 2023-05-24 14:20:05.000000 FCSAPIAccessSDK-1.1.2/FCSAPIAccess/api_access.py
+-rw-rw-rw-   0        0        0     9818 2023-05-24 14:19:50.000000 FCSAPIAccessSDK-1.1.2/FCSAPIAccess/exceptions.py
+-rw-rw-rw-   0        0        0     6169 2023-05-24 14:12:53.000000 FCSAPIAccessSDK-1.1.2/FCSAPIAccess/fcs_monitoring.py
+-rw-rw-rw-   0        0        0     9535 2023-05-24 14:12:53.000000 FCSAPIAccessSDK-1.1.2/FCSAPIAccess/fcs_notification.py
+-rw-rw-rw-   0        0        0    68112 2023-05-24 14:12:53.000000 FCSAPIAccessSDK-1.1.2/FCSAPIAccess/fcs_project.py
+-rw-rw-rw-   0        0        0     6073 2023-05-24 14:12:53.000000 FCSAPIAccessSDK-1.1.2/FCSAPIAccess/fcs_translation.py
+-rw-rw-rw-   0        0        0     5071 2023-05-19 20:26:24.000000 FCSAPIAccessSDK-1.1.2/FCSAPIAccess/scope.py
+drwxrwxrwx   0        0        0        0 2023-05-24 14:21:21.107720 FCSAPIAccessSDK-1.1.2/FCSAPIAccessSDK.egg-info/
+-rw-rw-rw-   0        0        0     1887 2023-05-24 14:21:21.000000 FCSAPIAccessSDK-1.1.2/FCSAPIAccessSDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2023-05-24 14:21:21.000000 FCSAPIAccessSDK-1.1.2/FCSAPIAccessSDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 14:21:21.000000 FCSAPIAccessSDK-1.1.2/FCSAPIAccessSDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-24 14:21:21.000000 FCSAPIAccessSDK-1.1.2/FCSAPIAccessSDK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-24 14:21:21.000000 FCSAPIAccessSDK-1.1.2/FCSAPIAccessSDK.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2022-03-16 05:36:31.000000 FCSAPIAccessSDK-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1887 2023-05-24 14:21:21.112034 FCSAPIAccessSDK-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      765 2022-04-14 20:12:51.000000 FCSAPIAccessSDK-1.1.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-24 14:21:21.118024 FCSAPIAccessSDK-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1453 2023-05-24 14:20:18.000000 FCSAPIAccessSDK-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 14:21:21.109714 FCSAPIAccessSDK-1.1.2/tests/
+-rw-rw-rw-   0        0        0     1188 2023-05-24 14:11:21.000000 FCSAPIAccessSDK-1.1.2/tests/test_auth.py
```

### Comparing `FCSAPIAccessSDK-1.1.1/FCSAPIAccess/api_access.py` & `FCSAPIAccessSDK-1.1.2/FCSAPIAccess/api_access.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,20 @@
         if r.status_code == 400:
             if r.json()["error"] == "invalid_grant":
                 raise exceptions.InvalidGrantException(
                     "The provided client_id and client_secret do not match an active application"
                 )
 
         approved_scope: str = r.json()["scope"]
-        self._scope = [scopes.Scope(s) for s in approved_scope.split(" ")]
+
+        if len(approved_scope) == 0:
+            self._scope = []
+
+        else:
+            self._scope = [scopes.Scope(s) for s in approved_scope.split(" ")]
 
         return r.json()["access_token"], r.json()["refresh_token"]
 
     def custom_request(
             self, endpoint: str, method: str, args: dict = None, json: dict = None, additional_headers: dict = None,
             api_version: str = "v1"
     ) -> dict:
@@ -85,14 +90,17 @@
     def refresh_token(self) -> typing.Tuple[str, str]:
         r = requests.post(self.url_base + "/project/oauth2", json={
             "grant_type": "refresh_token",
             "client_id": self._client_id,
             "access_token": self._access_token,
             "refresh_token": self._refresh_token
         })
+        if r.status_code == 401:
+            raise exceptions.InvalidCredentialsException(r.json()["error_description"])
+
         return r.json()["access_token"], r.json()["refresh_token"]
 
     def get_scope_string(self) -> str:
         return " ".join(s.value for s in self._scope)
 
     def set_access_token(self, access_token: str, refresh_token: str = None):
         self._access_token = access_token
```

### Comparing `FCSAPIAccessSDK-1.1.1/FCSAPIAccess/exceptions.py` & `FCSAPIAccessSDK-1.1.2/FCSAPIAccess/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 class InvalidGrantException(Exception):
     pass
 
 
+class InvalidCredentialsException(Exception):
+    pass
+
+
 class ClientError(Exception):
     pass
 
 
 class ServerError(Exception):
     pass
```

### Comparing `FCSAPIAccessSDK-1.1.1/FCSAPIAccess/fcs_monitoring.py` & `FCSAPIAccessSDK-1.1.2/FCSAPIAccess/fcs_monitoring.py`

 * *Files identical despite different names*

### Comparing `FCSAPIAccessSDK-1.1.1/FCSAPIAccess/fcs_notification.py` & `FCSAPIAccessSDK-1.1.2/FCSAPIAccess/fcs_notification.py`

 * *Files identical despite different names*

### Comparing `FCSAPIAccessSDK-1.1.1/FCSAPIAccess/fcs_project.py` & `FCSAPIAccessSDK-1.1.2/FCSAPIAccess/fcs_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -747,26 +747,26 @@
                 "privacy_policy": privacy_policy,
                 "terms_of_service": terms_of_service
             }
         )
         
         return self._check_status(r, lambda: self.change_settings(**local_vars))
         
-    def copy_settings(self, from) -> dict:
+    def copy_settings(self, from_id) -> dict:
         """
         
-        :param from: 
+        :param from_id: 
         """
         local_vars = locals()
         if 'self' in local_vars: del local_vars['self']
 
         headers = self.headers.copy()
         r = requests.request(
             "PUT", 
-            "https://fangcloudservices.pythonanywhere.com/api/v1/project/import?from={}".format(self._url_encode(from)), 
+            "https://fangcloudservices.pythonanywhere.com/api/v1/project/import?from_id={}".format(self._url_encode(from_id)), 
             headers=headers
         )
         
         return self._check_status(r, lambda: self.copy_settings(**local_vars))
         
     def get_scopes(self) -> dict:
         """
```

### Comparing `FCSAPIAccessSDK-1.1.1/FCSAPIAccess/fcs_translation.py` & `FCSAPIAccessSDK-1.1.2/FCSAPIAccess/fcs_translation.py`

 * *Files identical despite different names*

### Comparing `FCSAPIAccessSDK-1.1.1/FCSAPIAccess/scope.py` & `FCSAPIAccessSDK-1.1.2/FCSAPIAccess/scope.py`

 * *Files identical despite different names*

### Comparing `FCSAPIAccessSDK-1.1.1/FCSAPIAccessSDK.egg-info/PKG-INFO` & `FCSAPIAccessSDK-1.1.2/FCSAPIAccessSDK.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FCSAPIAccessSDK
-Version: 1.1.1
+Version: 1.1.2
 Summary: The SDK for project-level access to your FangCloudServices account
 Home-page: https://github.com/CPSuperstore/FangCloudServicesAPIAccessSDK
 Author: CPSuperstore
 Author-email: cpsuperstoreinc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/CPSuperstore/FangCloudServicesAPIAccessSDK/issues
 Keywords: FANG,CLOUD,SERVICES,FCS,SDK,USER,MANAGEMENT,OAUTH2,SECURITY
```

### Comparing `FCSAPIAccessSDK-1.1.1/LICENSE` & `FCSAPIAccessSDK-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FCSAPIAccessSDK-1.1.1/PKG-INFO` & `FCSAPIAccessSDK-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FCSAPIAccessSDK
-Version: 1.1.1
+Version: 1.1.2
 Summary: The SDK for project-level access to your FangCloudServices account
 Home-page: https://github.com/CPSuperstore/FangCloudServicesAPIAccessSDK
 Author: CPSuperstore
 Author-email: cpsuperstoreinc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/CPSuperstore/FangCloudServicesAPIAccessSDK/issues
 Keywords: FANG,CLOUD,SERVICES,FCS,SDK,USER,MANAGEMENT,OAUTH2,SECURITY
```

### Comparing `FCSAPIAccessSDK-1.1.1/README.md` & `FCSAPIAccessSDK-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `FCSAPIAccessSDK-1.1.1/setup.py` & `FCSAPIAccessSDK-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='FCSAPIAccessSDK',
-    version='1.1.1',
+    version='1.1.2',
     packages=['FCSAPIAccess'],
     url='https://github.com/CPSuperstore/FangCloudServicesAPIAccessSDK',
     license='Apache License 2.0',
     author='CPSuperstore',
     author_email='cpsuperstoreinc@gmail.com',
     description='The SDK for project-level access to your FangCloudServices account',
     long_description=long_description,
```

### Comparing `FCSAPIAccessSDK-1.1.1/tests/test_auth.py` & `FCSAPIAccessSDK-1.1.2/tests/test_auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     credentials = json.load(f)
 
 
 class TestCaseComparisons(unittest.TestCase):
     def test_correct_credentials(self):
         FCSAPIAccess(
             credentials["client_id"], credentials["client_secret"],
-            Scope.FULL_ACCESS
+            []
         )
 
     def test_expired_access_token(self):
         access = FCSAPIAccess(
             credentials["client_id"], credentials["client_secret"],
             Scope.FULL_ACCESS
         )
```

