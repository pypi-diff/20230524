# Comparing `tmp/FCSAPIAccessSDK-1.1.0.tar.gz` & `tmp/FCSAPIAccessSDK-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FCSAPIAccessSDK-1.1.0.tar", last modified: Fri May 19 20:59:01 2023, max compression
+gzip compressed data, was "FCSAPIAccessSDK-1.1.1.tar", last modified: Wed May 24 14:10:06 2023, max compression
```

## Comparing `FCSAPIAccessSDK-1.1.0.tar` & `FCSAPIAccessSDK-1.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 20:59:01.800546 FCSAPIAccessSDK-1.1.0/
-drwxrwxrwx   0        0        0        0 2023-05-19 20:59:01.725288 FCSAPIAccessSDK-1.1.0/FCSAPIAccess/
--rw-rw-rw-   0        0        0      127 2022-03-16 06:17:23.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccess/__init__.py
--rw-rw-rw-   0        0        0     3915 2022-04-26 02:36:49.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccess/api_access.py
--rw-rw-rw-   0        0        0      102 2022-04-14 20:02:56.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccess/exceptions.py
--rw-rw-rw-   0        0        0     6023 2023-05-19 20:53:50.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccess/fcs_monitoring.py
--rw-rw-rw-   0        0        0     9389 2023-05-19 20:53:50.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccess/fcs_notification.py
--rw-rw-rw-   0        0        0    66135 2023-05-19 20:53:50.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccess/fcs_project.py
--rw-rw-rw-   0        0        0     5927 2023-05-19 20:53:50.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccess/fcs_translation.py
--rw-rw-rw-   0        0        0     5071 2023-05-19 20:26:24.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccess/scope.py
-drwxrwxrwx   0        0        0        0 2023-05-19 20:59:01.745318 FCSAPIAccessSDK-1.1.0/FCSAPIAccessSDK.egg-info/
--rw-rw-rw-   0        0        0     1887 2023-05-19 20:59:01.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccessSDK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      474 2023-05-19 20:59:01.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccessSDK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 20:59:01.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccessSDK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-19 20:59:01.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccessSDK.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-19 20:59:01.000000 FCSAPIAccessSDK-1.1.0/FCSAPIAccessSDK.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2022-03-16 05:36:31.000000 FCSAPIAccessSDK-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     1887 2023-05-19 20:59:01.800546 FCSAPIAccessSDK-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      765 2022-04-14 20:12:51.000000 FCSAPIAccessSDK-1.1.0/README.md
--rw-rw-rw-   0        0        0       86 2023-05-19 20:59:01.807529 FCSAPIAccessSDK-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1453 2023-05-19 20:56:56.000000 FCSAPIAccessSDK-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 20:59:01.797551 FCSAPIAccessSDK-1.1.0/tests/
--rw-rw-rw-   0        0        0     1203 2022-04-14 20:07:43.000000 FCSAPIAccessSDK-1.1.0/tests/test_auth.py
+drwxrwxrwx   0        0        0        0 2023-05-24 14:10:06.259603 FCSAPIAccessSDK-1.1.1/
+drwxrwxrwx   0        0        0        0 2023-05-24 14:10:06.234500 FCSAPIAccessSDK-1.1.1/FCSAPIAccess/
+-rw-rw-rw-   0        0        0      127 2022-03-16 06:17:23.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccess/__init__.py
+-rw-rw-rw-   0        0        0     5049 2023-05-24 13:53:43.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccess/api_access.py
+-rw-rw-rw-   0        0        0     9757 2023-05-24 13:43:59.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccess/exceptions.py
+-rw-rw-rw-   0        0        0     6169 2023-05-24 14:08:06.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccess/fcs_monitoring.py
+-rw-rw-rw-   0        0        0     9535 2023-05-24 14:08:07.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccess/fcs_notification.py
+-rw-rw-rw-   0        0        0    68100 2023-05-24 14:08:06.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccess/fcs_project.py
+-rw-rw-rw-   0        0        0     6073 2023-05-24 14:08:07.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccess/fcs_translation.py
+-rw-rw-rw-   0        0        0     5071 2023-05-19 20:26:24.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccess/scope.py
+drwxrwxrwx   0        0        0        0 2023-05-24 14:10:06.256609 FCSAPIAccessSDK-1.1.1/FCSAPIAccessSDK.egg-info/
+-rw-rw-rw-   0        0        0     1887 2023-05-24 14:10:06.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccessSDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2023-05-24 14:10:06.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccessSDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 14:10:06.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccessSDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-24 14:10:06.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccessSDK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-24 14:10:06.000000 FCSAPIAccessSDK-1.1.1/FCSAPIAccessSDK.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2022-03-16 05:36:31.000000 FCSAPIAccessSDK-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1887 2023-05-24 14:10:06.260604 FCSAPIAccessSDK-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      765 2022-04-14 20:12:51.000000 FCSAPIAccessSDK-1.1.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-24 14:10:06.267410 FCSAPIAccessSDK-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1453 2023-05-24 14:09:46.000000 FCSAPIAccessSDK-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 14:10:06.257609 FCSAPIAccessSDK-1.1.1/tests/
+-rw-rw-rw-   0        0        0     1203 2022-04-14 20:07:43.000000 FCSAPIAccessSDK-1.1.1/tests/test_auth.py
```

### Comparing `FCSAPIAccessSDK-1.1.0/FCSAPIAccess/api_access.py` & `FCSAPIAccessSDK-1.1.1/FCSAPIAccess/api_access.py`

 * *Files 22% similar despite different names*

```diff
@@ -56,14 +56,36 @@
                 )
 
         approved_scope: str = r.json()["scope"]
         self._scope = [scopes.Scope(s) for s in approved_scope.split(" ")]
 
         return r.json()["access_token"], r.json()["refresh_token"]
 
+    def custom_request(
+            self, endpoint: str, method: str, args: dict = None, json: dict = None, additional_headers: dict = None,
+            api_version: str = "v1"
+    ) -> dict:
+
+        local_vars = locals()
+        if 'self' in local_vars: del local_vars['self']
+
+        additional_headers = {} if additional_headers is None else additional_headers
+
+        headers = {'Authorization': 'Bearer {}'.format(self._access_token)}
+        headers.update(additional_headers)
+
+        r = requests.request(
+            method,
+            "https://fangcloudservices.pythonanywhere.com/api/" + api_version + endpoint,
+            headers=headers,
+            params=args, json=json
+        )
+
+        return self._check_status(r, lambda: self.custom_request(**local_vars))
+
     def refresh_token(self) -> typing.Tuple[str, str]:
         r = requests.post(self.url_base + "/project/oauth2", json={
             "grant_type": "refresh_token",
             "client_id": self._client_id,
             "access_token": self._access_token,
             "refresh_token": self._refresh_token
         })
@@ -93,13 +115,22 @@
 
             if "error" in response:
                 if response["error"] == "expired_code":
                     self.set_access_token(*self.refresh_token())
                     return retry()
 
         if r.status_code == 500:
-            try:
-                raise exceptions.APIErrorException(r.json()["message"])
-            except KeyError:
-                raise exceptions.APIErrorException(
-                    "An unknown server has occurred. Please contact support for more info"
-                )
+            response = r.json()
+            if "message" in response:
+                raise exceptions.HTTP500InternalServerError(response["message"])
+
+            raise exceptions.HTTP500InternalServerError(
+                "An unknown server has occurred. Please contact support for more info"
+            )
+
+        if r.status_code == 404:
+            raise exceptions.HTTP404NotFound(
+                "The resource or endpoint you have requested either does not exist, "
+                "or you do not have permission to access"
+            )
+
+        exceptions.raise_exception(r.status_code)
```

### Comparing `FCSAPIAccessSDK-1.1.0/FCSAPIAccess/fcs_monitoring.py` & `FCSAPIAccessSDK-1.1.1/FCSAPIAccess/fcs_monitoring.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,21 @@
     def __init__(self, access_token):
         self.headers = {'Authorization': 'Bearer {}'.format(access_token)}
         self._status_check = lambda x, y: None
 
     def _check_status(self, r: requests.Response, retry: callable):
         check = self._status_check(r, retry)
         
-        return r.json() if check is None else check
+        if "json" in r.headers['content-type']:
+            result = r.json()
+            
+        else:
+            result = r.text
+        
+        return result if check is None else check
         
     def _url_encode(self, text: str) -> str:
         return urllib.parse.quote_plus(str(text))
     
     def get_urls(self) -> dict:
         """
         This endpoint retrieves the URLs you are monitoring
```

### Comparing `FCSAPIAccessSDK-1.1.0/FCSAPIAccess/fcs_notification.py` & `FCSAPIAccessSDK-1.1.1/FCSAPIAccess/fcs_notification.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,21 @@
     def __init__(self, access_token):
         self.headers = {'Authorization': 'Bearer {}'.format(access_token)}
         self._status_check = lambda x, y: None
 
     def _check_status(self, r: requests.Response, retry: callable):
         check = self._status_check(r, retry)
         
-        return r.json() if check is None else check
+        if "json" in r.headers['content-type']:
+            result = r.json()
+            
+        else:
+            result = r.text
+        
+        return result if check is None else check
         
     def _url_encode(self, text: str) -> str:
         return urllib.parse.quote_plus(str(text))
     
     def get_channels(self) -> dict:
         """
         Retrieves a list of existing channels
```

### Comparing `FCSAPIAccessSDK-1.1.0/FCSAPIAccess/fcs_project.py` & `FCSAPIAccessSDK-1.1.1/FCSAPIAccess/fcs_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,21 @@
     def __init__(self, access_token):
         self.headers = {'Authorization': 'Bearer {}'.format(access_token)}
         self._status_check = lambda x, y: None
 
     def _check_status(self, r: requests.Response, retry: callable):
         check = self._status_check(r, retry)
         
-        return r.json() if check is None else check
+        if "json" in r.headers['content-type']:
+            result = r.json()
+            
+        else:
+            result = r.text
+        
+        return result if check is None else check
         
     def _url_encode(self, text: str) -> str:
         return urllib.parse.quote_plus(str(text))
     
     def get_all_email_addresses(self, user) -> dict:
         """
         Retrieves the email addresses linked to a specified user.
@@ -277,14 +283,38 @@
             "GET", 
             "https://fangcloudservices.pythonanywhere.com/api/v1/project/user?id={}".format(self._url_encode(id)), 
             headers=headers
         )
         
         return self._check_status(r, lambda: self.get_user(**local_vars))
         
+    def search_users(self, username, display_name, email, primary_email, password_reset, reset_password_on_login, user_role, active) -> dict:
+        """
+        This endpoint retrieves a single user who has the specified ID.
+        :param username: 
+        :param display_name: 
+        :param email: 
+        :param primary_email: 
+        :param password_reset: 
+        :param reset_password_on_login: 
+        :param user_role: 
+        :param active: 
+        """
+        local_vars = locals()
+        if 'self' in local_vars: del local_vars['self']
+
+        headers = self.headers.copy()
+        r = requests.request(
+            "GET", 
+            "https://fangcloudservices.pythonanywhere.com/api/v1/project/user/search?username={}&display_name={}&email={}&primary_email={}&password_reset={}&reset_password_on_login={}&user_role={}&active={}".format(self._url_encode(username), self._url_encode(display_name), self._url_encode(email), self._url_encode(primary_email), self._url_encode(password_reset), self._url_encode(reset_password_on_login), self._url_encode(user_role), self._url_encode(active)), 
+            headers=headers
+        )
+        
+        return self._check_status(r, lambda: self.search_users(**local_vars))
+        
     def create_user(self, data, username, email, user_role, password, mailing_lists, dob, favourite_color) -> dict:
         """
         StartFragment
         
         Sets the properties of a new user.
         
         If the requested `user_role` or `mailing_list` IDs do not correspond to an existing user role or mailing list, you will receive a 404 error and the update will not be made.
@@ -717,14 +747,31 @@
                 "privacy_policy": privacy_policy,
                 "terms_of_service": terms_of_service
             }
         )
         
         return self._check_status(r, lambda: self.change_settings(**local_vars))
         
+    def copy_settings(self, from) -> dict:
+        """
+        
+        :param from: 
+        """
+        local_vars = locals()
+        if 'self' in local_vars: del local_vars['self']
+
+        headers = self.headers.copy()
+        r = requests.request(
+            "PUT", 
+            "https://fangcloudservices.pythonanywhere.com/api/v1/project/import?from={}".format(self._url_encode(from)), 
+            headers=headers
+        )
+        
+        return self._check_status(r, lambda: self.copy_settings(**local_vars))
+        
     def get_scopes(self) -> dict:
         """
         Retrieves the full list of scopes available to your account.
         """
         local_vars = locals()
         if 'self' in local_vars: del local_vars['self']
```

### Comparing `FCSAPIAccessSDK-1.1.0/FCSAPIAccess/fcs_translation.py` & `FCSAPIAccessSDK-1.1.1/FCSAPIAccess/fcs_translation.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,21 @@
     def __init__(self, access_token):
         self.headers = {'Authorization': 'Bearer {}'.format(access_token)}
         self._status_check = lambda x, y: None
 
     def _check_status(self, r: requests.Response, retry: callable):
         check = self._status_check(r, retry)
         
-        return r.json() if check is None else check
+        if "json" in r.headers['content-type']:
+            result = r.json()
+            
+        else:
+            result = r.text
+        
+        return result if check is None else check
         
     def _url_encode(self, text: str) -> str:
         return urllib.parse.quote_plus(str(text))
     
     def poll_translation(self, id) -> dict:
         """
         Polls the status of an ongoing translation job.
```

### Comparing `FCSAPIAccessSDK-1.1.0/FCSAPIAccess/scope.py` & `FCSAPIAccessSDK-1.1.1/FCSAPIAccess/scope.py`

 * *Files identical despite different names*

### Comparing `FCSAPIAccessSDK-1.1.0/FCSAPIAccessSDK.egg-info/PKG-INFO` & `FCSAPIAccessSDK-1.1.1/FCSAPIAccessSDK.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FCSAPIAccessSDK
-Version: 1.1.0
+Version: 1.1.1
 Summary: The SDK for project-level access to your FangCloudServices account
 Home-page: https://github.com/CPSuperstore/FangCloudServicesAPIAccessSDK
 Author: CPSuperstore
 Author-email: cpsuperstoreinc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/CPSuperstore/FangCloudServicesAPIAccessSDK/issues
 Keywords: FANG,CLOUD,SERVICES,FCS,SDK,USER,MANAGEMENT,OAUTH2,SECURITY
```

### Comparing `FCSAPIAccessSDK-1.1.0/LICENSE` & `FCSAPIAccessSDK-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FCSAPIAccessSDK-1.1.0/PKG-INFO` & `FCSAPIAccessSDK-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FCSAPIAccessSDK
-Version: 1.1.0
+Version: 1.1.1
 Summary: The SDK for project-level access to your FangCloudServices account
 Home-page: https://github.com/CPSuperstore/FangCloudServicesAPIAccessSDK
 Author: CPSuperstore
 Author-email: cpsuperstoreinc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/CPSuperstore/FangCloudServicesAPIAccessSDK/issues
 Keywords: FANG,CLOUD,SERVICES,FCS,SDK,USER,MANAGEMENT,OAUTH2,SECURITY
```

### Comparing `FCSAPIAccessSDK-1.1.0/README.md` & `FCSAPIAccessSDK-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `FCSAPIAccessSDK-1.1.0/setup.py` & `FCSAPIAccessSDK-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='FCSAPIAccessSDK',
-    version='1.1.0',
+    version='1.1.1',
     packages=['FCSAPIAccess'],
     url='https://github.com/CPSuperstore/FangCloudServicesAPIAccessSDK',
     license='Apache License 2.0',
     author='CPSuperstore',
     author_email='cpsuperstoreinc@gmail.com',
     description='The SDK for project-level access to your FangCloudServices account',
     long_description=long_description,
```

### Comparing `FCSAPIAccessSDK-1.1.0/tests/test_auth.py` & `FCSAPIAccessSDK-1.1.1/tests/test_auth.py`

 * *Files identical despite different names*

