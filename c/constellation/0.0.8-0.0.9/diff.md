# Comparing `tmp/constellation-0.0.8.tar.gz` & `tmp/constellation-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constellation-0.0.8.tar", last modified: Fri Jan  7 16:39:44 2022, max compression
+gzip compressed data, was "constellation-0.0.9.tar", last modified: Mon Jan 10 14:22:52 2022, max compression
```

## Comparing `constellation-0.0.8.tar` & `constellation-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-01-07 16:39:44.956952 constellation-0.0.8/
--rw-rw-r--   0 rob       (1000) rob       (1000)     1096 2022-01-07 16:39:18.000000 constellation-0.0.8/LICENSE
--rw-rw-r--   0 rob       (1000) rob       (1000)      960 2022-01-07 16:39:44.956952 constellation-0.0.8/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      481 2022-01-07 16:39:18.000000 constellation-0.0.8/README.md
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-01-07 16:39:44.956952 constellation-0.0.8/constellation/
--rw-rw-r--   0 rob       (1000) rob       (1000)      337 2022-01-07 16:39:18.000000 constellation-0.0.8/constellation/__init__.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     4146 2022-01-07 16:39:18.000000 constellation-0.0.8/constellation/config.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    10116 2022-01-07 16:39:18.000000 constellation-0.0.8/constellation/constellation.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     6866 2022-01-07 16:39:18.000000 constellation-0.0.8/constellation/docker_util.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1460 2022-01-07 16:39:18.000000 constellation-0.0.8/constellation/notifier.py
--rw-rw-r--   0 rob       (1000) rob       (1000)      536 2022-01-07 16:39:18.000000 constellation-0.0.8/constellation/util.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     3264 2022-01-07 16:39:18.000000 constellation-0.0.8/constellation/vault.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-01-07 16:39:44.956952 constellation-0.0.8/constellation.egg-info/
--rw-rw-r--   0 rob       (1000) rob       (1000)      960 2022-01-07 16:39:44.000000 constellation-0.0.8/constellation.egg-info/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      566 2022-01-07 16:39:44.000000 constellation-0.0.8/constellation.egg-info/SOURCES.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-01-07 16:39:44.000000 constellation-0.0.8/constellation.egg-info/dependency_links.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-01-07 16:39:44.000000 constellation-0.0.8/constellation.egg-info/not-zip-safe
--rw-rw-r--   0 rob       (1000) rob       (1000)       36 2022-01-07 16:39:44.000000 constellation-0.0.8/constellation.egg-info/requires.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       14 2022-01-07 16:39:44.000000 constellation-0.0.8/constellation.egg-info/top_level.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       63 2022-01-07 16:39:44.960952 constellation-0.0.8/setup.cfg
--rw-rw-r--   0 rob       (1000) rob       (1000)     1007 2022-01-07 16:39:18.000000 constellation-0.0.8/setup.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-01-07 16:39:44.956952 constellation-0.0.8/test/
--rw-rw-r--   0 rob       (1000) rob       (1000)     5948 2022-01-07 16:39:18.000000 constellation-0.0.8/test/test_config.py
--rw-rw-r--   0 rob       (1000) rob       (1000)    12357 2022-01-07 16:39:18.000000 constellation-0.0.8/test/test_constellation.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     7595 2022-01-07 16:39:18.000000 constellation-0.0.8/test/test_docker_util.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1805 2022-01-07 16:39:18.000000 constellation-0.0.8/test/test_notify.py
--rw-rw-r--   0 rob       (1000) rob       (1000)      398 2022-01-07 16:39:18.000000 constellation-0.0.8/test/test_util.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     6405 2022-01-07 16:39:18.000000 constellation-0.0.8/test/test_vault.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-01-10 14:22:52.180755 constellation-0.0.9/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1096 2022-01-10 14:22:23.000000 constellation-0.0.9/LICENSE
+-rw-rw-r--   0 rob       (1000) rob       (1000)      960 2022-01-10 14:22:52.180755 constellation-0.0.9/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      481 2022-01-10 14:22:23.000000 constellation-0.0.9/README.md
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-01-10 14:22:52.180755 constellation-0.0.9/constellation/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      337 2022-01-10 14:22:23.000000 constellation-0.0.9/constellation/__init__.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     4451 2022-01-10 14:22:23.000000 constellation-0.0.9/constellation/config.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    10116 2022-01-10 14:22:23.000000 constellation-0.0.9/constellation/constellation.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     6866 2022-01-10 14:22:23.000000 constellation-0.0.9/constellation/docker_util.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1460 2022-01-10 14:22:23.000000 constellation-0.0.9/constellation/notifier.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)      536 2022-01-10 14:22:23.000000 constellation-0.0.9/constellation/util.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2737 2022-01-10 14:22:23.000000 constellation-0.0.9/constellation/vault.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-01-10 14:22:52.180755 constellation-0.0.9/constellation.egg-info/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      960 2022-01-10 14:22:52.000000 constellation-0.0.9/constellation.egg-info/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      566 2022-01-10 14:22:52.000000 constellation-0.0.9/constellation.egg-info/SOURCES.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-01-10 14:22:52.000000 constellation-0.0.9/constellation.egg-info/dependency_links.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-01-10 14:22:52.000000 constellation-0.0.9/constellation.egg-info/not-zip-safe
+-rw-rw-r--   0 rob       (1000) rob       (1000)       36 2022-01-10 14:22:52.000000 constellation-0.0.9/constellation.egg-info/requires.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       14 2022-01-10 14:22:52.000000 constellation-0.0.9/constellation.egg-info/top_level.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       63 2022-01-10 14:22:52.180755 constellation-0.0.9/setup.cfg
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1007 2022-01-10 14:22:23.000000 constellation-0.0.9/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-01-10 14:22:52.180755 constellation-0.0.9/test/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     6286 2022-01-10 14:22:23.000000 constellation-0.0.9/test/test_config.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    12357 2022-01-10 14:22:23.000000 constellation-0.0.9/test/test_constellation.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     7595 2022-01-10 14:22:23.000000 constellation-0.0.9/test/test_docker_util.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1805 2022-01-10 14:22:23.000000 constellation-0.0.9/test/test_notify.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)      398 2022-01-10 14:22:23.000000 constellation-0.0.9/test/test_util.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     4892 2022-01-10 14:22:23.000000 constellation-0.0.9/test/test_vault.py
```

### Comparing `constellation-0.0.8/LICENSE` & `constellation-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `constellation-0.0.8/PKG-INFO` & `constellation-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constellation
-Version: 0.0.8
+Version: 0.0.9
 Summary: Deploy scripts for constellations of docker containers
 Home-page: https://github.com/reside-ic/constellation
 Author: Rich FitzJohn
 Author-email: r.fitzjohn@imperial.ac.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `constellation-0.0.8/constellation/config.py` & `constellation-0.0.9/constellation/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import copy
 import tempfile
 import yaml
+import re
+import os
 
 import constellation.vault as vault
 from constellation.util import ImageReference
 
 
 def read_yaml(filename):
     with open(filename, "r") as f:
@@ -32,14 +34,16 @@
     if type(path) is str:
         path = [path]
     for i, p in enumerate(path):
         try:
             data = data[p]
             if data is None:
                 raise KeyError()
+            if isinstance(data, str) and re.search("^\\$[0-9A-Z_]+$", data):
+                data = get_envvar(data[1:])
         except KeyError as e:
             if is_optional:
                 return default
             e.args = (":".join(path[:(i + 1)]),)
             raise e
 
     expected = {"string": str,
@@ -126,7 +130,15 @@
 def collapse(options):
     """Combine a list of dictionaries recursively, combining from left to
 right so that later dictionaries override values in earlier ones"""
     ret = {}
     for o in options:
         combine(ret, o)
     return ret
+
+
+def get_envvar(name):
+    try:
+        return os.environ[name]
+    except KeyError:
+        raise KeyError("Did not find env var '{}'".format(
+            name))
```

### Comparing `constellation-0.0.8/constellation/constellation.py` & `constellation-0.0.9/constellation/constellation.py`

 * *Files identical despite different names*

### Comparing `constellation-0.0.8/constellation/docker_util.py` & `constellation-0.0.9/constellation/docker_util.py`

 * *Files identical despite different names*

### Comparing `constellation-0.0.8/constellation/notifier.py` & `constellation-0.0.9/constellation/notifier.py`

 * *Files identical despite different names*

### Comparing `constellation-0.0.8/constellation/util.py` & `constellation-0.0.9/constellation/util.py`

 * *Files identical despite different names*

### Comparing `constellation-0.0.8/constellation/vault.py` & `constellation-0.0.9/constellation/vault.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,27 +66,19 @@
         if self.auth_method == "token":
             cl = hvac.Client(url=self.url, token=self.auth_args["token"])
         else:
             cl = hvac.Client(url=self.url)
             print("Authenticating with the vault using '{}'".format(
                 self.auth_method))
 
-            if not self.auth_args:
-                self.auth_args = {}
-
             if self.auth_method == "github":
+                if not self.auth_args:
+                    self.auth_args = {}
                 if "token" not in self.auth_args:
                     self.auth_args["token"] = get_github_token()
-            elif self.auth_method == "approle":
-                if "role_id" not in self.auth_args:
-                    self.auth_args["role_id"] = get_envvar(
-                        "VAULT_AUTH_ROLE_ID")
-                if "secret_id" not in self.auth_args:
-                    self.auth_args["secret_id"] = get_envvar(
-                        "VAULT_AUTH_SECRET_ID")
 
             getattr(cl.auth, self.auth_method).login(**self.auth_args)
         return cl
 
 
 class vault_not_enabled:
     def __getattr__(self, name):
@@ -96,18 +88,10 @@
 def get_github_token():
     try:
         return os.environ["VAULT_AUTH_GITHUB_TOKEN"]
     except KeyError:
         return input("Enter GitHub token for vault: ").strip()
 
 
-def get_envvar(name):
-    try:
-        return os.environ[name]
-    except KeyError:
-        raise KeyError("Did not find env var '{}'".format(
-            name))
-
-
 def drop_envvar(name):
     if name in os.environ:
         del os.environ[name]
```

### Comparing `constellation-0.0.8/constellation.egg-info/PKG-INFO` & `constellation-0.0.9/constellation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constellation
-Version: 0.0.8
+Version: 0.0.9
 Summary: Deploy scripts for constellations of docker containers
 Home-page: https://github.com/reside-ic/constellation
 Author: Rich FitzJohn
 Author-email: r.fitzjohn@imperial.ac.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `constellation-0.0.8/constellation.egg-info/SOURCES.txt` & `constellation-0.0.9/constellation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `constellation-0.0.8/setup.py` & `constellation-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "docker",
     "hvac",
     "pytest",
     "pyyaml",
     "vault_dev"]
 
 setup(name="constellation",
-      version="0.0.8",
+      version="0.0.9",
       description="Deploy scripts for constellations of docker containers",
       long_description=long_description,
       classifiers=[
           "Programming Language :: Python :: 3",
           "License :: OSI Approved :: MIT License",
           "Operating System :: OS Independent",
       ],
```

### Comparing `constellation-0.0.8/test/test_config.py` & `constellation-0.0.9/test/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+import os
 import pytest
 
+from unittest import mock
+
 from constellation.config import *
 
 sample_data = {"a": "value1", "b": {"x": "value2"}, "c": 1, "d": True,
-               "e": None}
+               "e": None, "f": "$EXAMPLE_ENV_VAR"}
 
 
 def test_config_string_reads_simple_values():
     assert config_string(sample_data, "a") == "value1"
     assert config_string(sample_data, ["a"]) == "value1"
 
 
@@ -182,10 +185,20 @@
         msg = "'container_prefix' may not be modified"
         with pytest.raises(Exception, match=msg):
             config_build(path, data, "options")
         with pytest.raises(Exception, match=msg):
             config_build(path, data, None, options)
 
 
+def test_config_read_env_var():
+    with mock.patch.dict(os.environ, {"EXAMPLE_ENV_VAR": "value1"}):
+        assert config_string(sample_data, "f") == "value1"
+
+
+def test_config_read_env_var_error():
+    with pytest.raises(KeyError):
+        config_string(sample_data, "f")
+
+
 def write_file(contents, path):
     with open(path, "w") as f:
         f.write(contents)
```

### Comparing `constellation-0.0.8/test/test_constellation.py` & `constellation-0.0.9/test/test_constellation.py`

 * *Files identical despite different names*

### Comparing `constellation-0.0.8/test/test_docker_util.py` & `constellation-0.0.9/test/test_docker_util.py`

 * *Files identical despite different names*

### Comparing `constellation-0.0.8/test/test_notify.py` & `constellation-0.0.9/test/test_notify.py`

 * *Files identical despite different names*

### Comparing `constellation-0.0.8/test/test_vault.py` & `constellation-0.0.9/test/test_vault.py`

 * *Files 23% similar despite different names*

```diff
@@ -120,58 +120,14 @@
         url = "http://localhost:{}".format(s.port)
         token = os.environ["VAULT_TEST_GITHUB_PAT"]
         with mock.patch.dict(os.environ, {"VAULT_AUTH_GITHUB_TOKEN": token}):
             cfg = vault_config(url, "github", None)
             assert cfg.client().is_authenticated()
 
 
-def test_vault_config_approle_login():
-    with vault_dev.server() as s:
-        cl = s.client()
-        cl.sys.enable_auth_method(method_type="approle")
-        cl.auth.approle.create_or_update_approle(
-            role_name="test-role"
-        )
-
-        url = "http://localhost:{}".format(s.port)
-        role_id = cl.auth.approle.read_role_id(
-            role_name="test-role"
-        )["data"]["role_id"]
-        secret_id = cl.auth.approle.generate_secret_id(
-            role_name="test-role"
-        )["data"]["secret_id"]
-        with mock.patch.dict(os.environ, {
-            "VAULT_AUTH_ROLE_ID": role_id,
-            "VAULT_AUTH_SECRET_ID": secret_id
-        }):
-            cfg = vault_config(url, "approle", None)
-            assert cfg.client().is_authenticated()
-
-
-def test_vault_config_approle_no_args():
-    with vault_dev.server() as s:
-        cl = s.client()
-        cl.sys.enable_auth_method(method_type="approle")
-        cl.auth.approle.create_or_update_approle(
-            role_name="test-role"
-        )
-
-        url = "http://localhost:{}".format(s.port)
-        role_id = cl.auth.approle.read_role_id(
-            role_name="test-role"
-        )["data"]["role_id"]
-        with mock.patch.dict(os.environ, {
-            "VAULT_AUTH_ROLE_ID": role_id
-        }):
-            cfg = vault_config(url, "approle", None)
-            msg = "Did not find env var 'VAULT_AUTH_SECRET_ID'"
-            with pytest.raises(Exception, match=msg):
-                cfg.client().is_authenticated()
-
-
 # Utility required to work around https://github.com/hvac/hvac/issues/421
 def test_drop_envvar_removes_envvar():
     name = "VAULT_DEV_TEST_VAR"
     os.environ[name] = "x"
     drop_envvar(name)
     assert name not in os.environ
```

