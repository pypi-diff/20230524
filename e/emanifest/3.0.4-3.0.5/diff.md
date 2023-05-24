# Comparing `tmp/emanifest-3.0.4.tar.gz` & `tmp/emanifest-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emanifest-3.0.4.tar", last modified: Tue May  9 19:45:32 2023, max compression
+gzip compressed data, was "emanifest-3.0.5.tar", last modified: Wed May 24 15:20:33 2023, max compression
```

## Comparing `emanifest-3.0.4.tar` & `emanifest-3.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:45:32.757695 emanifest-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-09 19:45:14.000000 emanifest-3.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-05-09 19:45:32.757695 emanifest-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-05-09 19:45:14.000000 emanifest-3.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-09 19:45:14.000000 emanifest-3.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 19:45:32.757695 emanifest-3.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:45:32.757695 emanifest-3.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:45:32.757695 emanifest-3.0.4/src/emanifest/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-09 19:45:14.000000 emanifest-3.0.4/src/emanifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37641 2023-05-09 19:45:14.000000 emanifest-3.0.4/src/emanifest/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-05-09 19:45:14.000000 emanifest-3.0.4/src/emanifest/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:45:32.757695 emanifest-3.0.4/src/emanifest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-05-09 19:45:32.000000 emanifest-3.0.4/src/emanifest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-09 19:45:32.000000 emanifest-3.0.4/src/emanifest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:45:32.000000 emanifest-3.0.4/src/emanifest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-09 19:45:32.000000 emanifest-3.0.4/src/emanifest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 19:45:32.000000 emanifest-3.0.4/src/emanifest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:20:32.999691 emanifest-3.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-24 15:20:13.000000 emanifest-3.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-05-24 15:20:32.999691 emanifest-3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-05-24 15:20:13.000000 emanifest-3.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-24 15:20:13.000000 emanifest-3.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 15:20:32.999691 emanifest-3.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:20:32.995690 emanifest-3.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:20:32.999691 emanifest-3.0.5/src/emanifest/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-24 15:20:13.000000 emanifest-3.0.5/src/emanifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37641 2023-05-24 15:20:13.000000 emanifest-3.0.5/src/emanifest/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-05-24 15:20:13.000000 emanifest-3.0.5/src/emanifest/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:20:32.999691 emanifest-3.0.5/src/emanifest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-05-24 15:20:32.000000 emanifest-3.0.5/src/emanifest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-24 15:20:32.000000 emanifest-3.0.5/src/emanifest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:20:32.000000 emanifest-3.0.5/src/emanifest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-24 15:20:32.000000 emanifest-3.0.5/src/emanifest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 15:20:32.000000 emanifest-3.0.5/src/emanifest.egg-info/top_level.txt
```

### Comparing `emanifest-3.0.4/LICENSE.txt` & `emanifest-3.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `emanifest-3.0.4/PKG-INFO` & `emanifest-3.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emanifest
-Version: 3.0.4
+Version: 3.0.5
 Summary: An API utility wrapper for accessing the e-Manifest hazardous waste tracking system maintained by the US Environmental Protection Agency
 Author-email: William Nicholas  <nicholas.william@epa.gov>, David Graham <graham.david@epa.gov>
 Maintainer-email: William Nicholas <nicholas.william@epa.gov>, David Graham <graham.david@epa.gov>, Scott Christian <christian.scott@epa.gov>
 License: CCO 1.0
 Project-URL: issues, https://github.com/USEPA/e-Manifest/issues
 Project-URL: documentation, https://github.com/USEPA/e-Manifest/emanifest-py
 Project-URL: homepage, https://github.com/USEPA/e-Manifest
```

### Comparing `emanifest-3.0.4/README.md` & `emanifest-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `emanifest-3.0.4/pyproject.toml` & `emanifest-3.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "emanifest"
-version = "3.0.4"
+version = "3.0.5"
 description = "An API utility wrapper for accessing the e-Manifest hazardous waste tracking system maintained by the US Environmental Protection Agency"
 readme = "README.md"
 authors = [
     { name = "William Nicholas ", email = "nicholas.william@epa.gov" },
     { name = "David Graham", email = "graham.david@epa.gov" },
 ]
 maintainers = [
@@ -12,20 +12,20 @@
     { name = "David Graham", email = "graham.david@epa.gov" },
     { name = "Scott Christian", email = "christian.scott@epa.gov" },
 ]
 
 license = { text = "CCO 1.0" }
 requires-python = ">=3.7"
 dependencies = [
-    "requests==2.28.1",
-    "certifi==2022.12.7",
-    "requests-toolbelt==0.10.1",
-    "charset-normalizer==2.1.1",
+    "requests==2.31.0",
+    "certifi==2023.5.7",
+    "requests-toolbelt==1.0.0",
+    "charset-normalizer==3.1.0",
     "idna==3.4",
-    "urllib3==1.26.13"
+    "urllib3==2.0.2"
 ]
 
 [project.urls]
 issues = "https://github.com/USEPA/e-Manifest/issues"
 documentation = "https://github.com/USEPA/e-Manifest/emanifest-py"
 homepage = "https://github.com/USEPA/e-Manifest"
 repository = "https://github.com/USEPA/e-Manifest"
```

### Comparing `emanifest-3.0.4/src/emanifest/client.py` & `emanifest-3.0.5/src/emanifest/client.py`

 * *Files identical despite different names*

### Comparing `emanifest-3.0.4/src/emanifest/test_client.py` & `emanifest-3.0.5/src/emanifest/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,23 +88,23 @@
         api_key_set_during_auth = my_subclass.retrieve_key()
         assert api_key_set_during_auth == self.MyClass.mock_api_key_from_external
 
 
 class TestAutoAuthentication:
     api_id = os.getenv('RCRAINFO_API_ID')
     api_key = os.getenv('RCRAINFO_API_KEY')
-    rcrainfo = RcrainfoClient('preprod', api_key=api_key, api_id=api_id)
 
     def test_automatically_authenticates(self):
         """
         RcrainfoClient will automatically authenticate once a request is made,
         (e.g., calling get_manifest(...) will do the equivalent of authenticate(...) first
         """
-        _resp = self.rcrainfo.get_manifest(TEST_GEN_MTN)
-        assert self.rcrainfo.is_authenticated
+        rcrainfo = RcrainfoClient('preprod', api_key=self.api_key, api_id=self.api_id)
+        _resp = rcrainfo.get_manifest(TEST_GEN_MTN)
+        assert rcrainfo.is_authenticated
 
     def test_does_not_authenticate_when_false(self):
         """
         emanifest(py) package will auto-authenticate (and re-authenticate) unless
         the auto_renew argument is set to False
         """
         rcrainfo = RcrainfoClient('preprod', api_key=self.api_key, api_id=self.api_id, auto_renew=False)
```

### Comparing `emanifest-3.0.4/src/emanifest.egg-info/PKG-INFO` & `emanifest-3.0.5/src/emanifest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emanifest
-Version: 3.0.4
+Version: 3.0.5
 Summary: An API utility wrapper for accessing the e-Manifest hazardous waste tracking system maintained by the US Environmental Protection Agency
 Author-email: William Nicholas  <nicholas.william@epa.gov>, David Graham <graham.david@epa.gov>
 Maintainer-email: William Nicholas <nicholas.william@epa.gov>, David Graham <graham.david@epa.gov>, Scott Christian <christian.scott@epa.gov>
 License: CCO 1.0
 Project-URL: issues, https://github.com/USEPA/e-Manifest/issues
 Project-URL: documentation, https://github.com/USEPA/e-Manifest/emanifest-py
 Project-URL: homepage, https://github.com/USEPA/e-Manifest
```

