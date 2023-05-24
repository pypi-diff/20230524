# Comparing `tmp/bossman-0.8.0.tar.gz` & `tmp/bossman-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bossman-0.8.0.tar", last modified: Wed Sep  9 20:15:42 2020, max compression
+gzip compressed data, was "dist/bossman-0.9.0.tar", last modified: Fri Sep 11 16:01:12 2020, max compression
```

## Comparing `bossman-0.8.0.tar` & `bossman-0.9.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 ahogg      (503)      600        0 2020-09-09 20:15:42.000000 bossman-0.8.0/
--rw-r--r--   0 ahogg      (503)      600     4579 2020-09-09 20:15:42.000000 bossman-0.8.0/PKG-INFO
--rw-r--r--   0 ahogg      (503)      600     3200 2020-09-07 20:04:51.000000 bossman-0.8.0/README.md
-drwxr-xr-x   0 ahogg      (503)      600        0 2020-09-09 20:15:42.000000 bossman-0.8.0/bossman/
--rw-r--r--   0 ahogg      (503)      600     2205 2020-09-09 18:19:27.000000 bossman-0.8.0/bossman/__init__.py
-drwxr-xr-x   0 ahogg      (503)      600        0 2020-09-09 20:15:42.000000 bossman-0.8.0/bossman/abc/
--rw-r--r--   0 ahogg      (503)      600        0 2020-09-07 11:06:50.000000 bossman-0.8.0/bossman/abc/__init__.py
--rw-r--r--   0 ahogg      (503)      600      526 2020-09-07 16:30:51.000000 bossman-0.8.0/bossman/abc/resource.py
--rw-r--r--   0 ahogg      (503)      600     2086 2020-09-09 16:36:07.000000 bossman-0.8.0/bossman/abc/resource_type.py
-drwxr-xr-x   0 ahogg      (503)      600        0 2020-09-09 20:15:42.000000 bossman-0.8.0/bossman/cli/
--rw-r--r--   0 ahogg      (503)      600     1695 2020-09-09 18:18:08.000000 bossman-0.8.0/bossman/cli/__init__.py
--rw-r--r--   0 ahogg      (503)      600     1468 2020-09-09 18:51:30.000000 bossman-0.8.0/bossman/cli/apply_cmd.py
--rw-r--r--   0 ahogg      (503)      600      710 2020-09-09 17:06:43.000000 bossman-0.8.0/bossman/cli/log_cmd.py
--rw-r--r--   0 ahogg      (503)      600     1901 2020-09-09 18:24:45.000000 bossman-0.8.0/bossman/cli/status_cmd.py
--rw-r--r--   0 ahogg      (503)      600     1389 2020-09-07 09:35:29.000000 bossman-0.8.0/bossman/config.py
--rw-r--r--   0 ahogg      (503)      600      566 2020-09-09 18:12:15.000000 bossman-0.8.0/bossman/errors.py
--rw-r--r--   0 ahogg      (503)      600     1001 2020-09-06 09:52:35.000000 bossman-0.8.0/bossman/git.py
--rw-r--r--   0 ahogg      (503)      600      397 2020-09-05 23:32:07.000000 bossman-0.8.0/bossman/logging.py
-drwxr-xr-x   0 ahogg      (503)      600        0 2020-09-09 20:15:42.000000 bossman-0.8.0/bossman/plugins/
--rw-r--r--   0 ahogg      (503)      600        0 2020-09-07 09:13:40.000000 bossman-0.8.0/bossman/plugins/__init__.py
-drwxr-xr-x   0 ahogg      (503)      600        0 2020-09-09 20:15:42.000000 bossman-0.8.0/bossman/plugins/akamai/
--rw-r--r--   0 ahogg      (503)      600        0 2020-09-05 18:51:27.000000 bossman-0.8.0/bossman/plugins/akamai/__init__.py
-drwxr-xr-x   0 ahogg      (503)      600        0 2020-09-09 20:15:42.000000 bossman-0.8.0/bossman/plugins/akamai/lib/
--rw-r--r--   0 ahogg      (503)      600        0 2020-09-08 20:24:16.000000 bossman-0.8.0/bossman/plugins/akamai/lib/__init__.py
--rw-r--r--   0 ahogg      (503)      600     1100 2020-09-08 20:24:16.000000 bossman-0.8.0/bossman/plugins/akamai/lib/edgegrid.py
--rw-r--r--   0 ahogg      (503)      600     4335 2020-09-09 19:51:45.000000 bossman-0.8.0/bossman/plugins/akamai/lib/papi.py
--rw-r--r--   0 ahogg      (503)      600     5423 2020-09-09 19:41:56.000000 bossman-0.8.0/bossman/plugins/akamai/property.py
--rw-r--r--   0 ahogg      (503)      600     5664 2020-09-09 18:39:15.000000 bossman-0.8.0/bossman/repo.py
--rw-r--r--   0 ahogg      (503)      600     1683 2020-09-09 17:08:31.000000 bossman-0.8.0/bossman/resources.py
-drwxr-xr-x   0 ahogg      (503)      600        0 2020-09-09 20:15:42.000000 bossman-0.8.0/bossman.egg-info/
--rw-r--r--   0 ahogg      (503)      600     4579 2020-09-09 20:15:42.000000 bossman-0.8.0/bossman.egg-info/PKG-INFO
--rw-r--r--   0 ahogg      (503)      600      759 2020-09-09 20:15:42.000000 bossman-0.8.0/bossman.egg-info/SOURCES.txt
--rw-r--r--   0 ahogg      (503)      600        1 2020-09-09 20:15:42.000000 bossman-0.8.0/bossman.egg-info/dependency_links.txt
--rw-r--r--   0 ahogg      (503)      600       46 2020-09-09 20:15:42.000000 bossman-0.8.0/bossman.egg-info/entry_points.txt
--rw-r--r--   0 ahogg      (503)      600        1 2020-09-07 19:19:42.000000 bossman-0.8.0/bossman.egg-info/not-zip-safe
--rw-r--r--   0 ahogg      (503)      600       70 2020-09-09 20:15:42.000000 bossman-0.8.0/bossman.egg-info/requires.txt
--rw-r--r--   0 ahogg      (503)      600        8 2020-09-09 20:15:42.000000 bossman-0.8.0/bossman.egg-info/top_level.txt
--rw-r--r--   0 ahogg      (503)      600       79 2020-09-09 20:15:42.000000 bossman-0.8.0/setup.cfg
--rw-r--r--   0 ahogg      (503)      600     1014 2020-09-07 20:45:11.000000 bossman-0.8.0/setup.py
+drwxr-xr-x   0 ahogg      (503)      600        0 2020-09-11 16:01:12.000000 bossman-0.9.0/
+-rw-r--r--   0 ahogg      (503)      600     4579 2020-09-11 16:01:12.000000 bossman-0.9.0/PKG-INFO
+-rw-r--r--   0 ahogg      (503)      600     3200 2020-09-07 20:04:51.000000 bossman-0.9.0/README.md
+drwxr-xr-x   0 ahogg      (503)      600        0 2020-09-11 16:01:12.000000 bossman-0.9.0/bossman/
+-rw-r--r--   0 ahogg      (503)      600     2205 2020-09-09 18:19:27.000000 bossman-0.9.0/bossman/__init__.py
+drwxr-xr-x   0 ahogg      (503)      600        0 2020-09-11 16:01:12.000000 bossman-0.9.0/bossman/abc/
+-rw-r--r--   0 ahogg      (503)      600        0 2020-09-07 11:06:50.000000 bossman-0.9.0/bossman/abc/__init__.py
+-rw-r--r--   0 ahogg      (503)      600      526 2020-09-07 16:30:51.000000 bossman-0.9.0/bossman/abc/resource.py
+-rw-r--r--   0 ahogg      (503)      600     2086 2020-09-09 16:36:07.000000 bossman-0.9.0/bossman/abc/resource_type.py
+drwxr-xr-x   0 ahogg      (503)      600        0 2020-09-11 16:01:12.000000 bossman-0.9.0/bossman/cli/
+-rw-r--r--   0 ahogg      (503)      600     1695 2020-09-09 18:18:08.000000 bossman-0.9.0/bossman/cli/__init__.py
+-rw-r--r--   0 ahogg      (503)      600     1468 2020-09-09 18:51:30.000000 bossman-0.9.0/bossman/cli/apply_cmd.py
+-rw-r--r--   0 ahogg      (503)      600      710 2020-09-09 17:06:43.000000 bossman-0.9.0/bossman/cli/log_cmd.py
+-rw-r--r--   0 ahogg      (503)      600     1901 2020-09-09 18:24:45.000000 bossman-0.9.0/bossman/cli/status_cmd.py
+-rw-r--r--   0 ahogg      (503)      600     1389 2020-09-07 09:35:29.000000 bossman-0.9.0/bossman/config.py
+-rw-r--r--   0 ahogg      (503)      600      566 2020-09-09 18:12:15.000000 bossman-0.9.0/bossman/errors.py
+-rw-r--r--   0 ahogg      (503)      600     1001 2020-09-06 09:52:35.000000 bossman-0.9.0/bossman/git.py
+-rw-r--r--   0 ahogg      (503)      600      397 2020-09-05 23:32:07.000000 bossman-0.9.0/bossman/logging.py
+drwxr-xr-x   0 ahogg      (503)      600        0 2020-09-11 16:01:12.000000 bossman-0.9.0/bossman/plugins/
+-rw-r--r--   0 ahogg      (503)      600        0 2020-09-07 09:13:40.000000 bossman-0.9.0/bossman/plugins/__init__.py
+drwxr-xr-x   0 ahogg      (503)      600        0 2020-09-11 16:01:12.000000 bossman-0.9.0/bossman/plugins/akamai/
+-rw-r--r--   0 ahogg      (503)      600        0 2020-09-05 18:51:27.000000 bossman-0.9.0/bossman/plugins/akamai/__init__.py
+drwxr-xr-x   0 ahogg      (503)      600        0 2020-09-11 16:01:12.000000 bossman-0.9.0/bossman/plugins/akamai/lib/
+-rw-r--r--   0 ahogg      (503)      600        0 2020-09-08 20:24:16.000000 bossman-0.9.0/bossman/plugins/akamai/lib/__init__.py
+-rw-r--r--   0 ahogg      (503)      600     1100 2020-09-08 20:24:16.000000 bossman-0.9.0/bossman/plugins/akamai/lib/edgegrid.py
+-rw-r--r--   0 ahogg      (503)      600     4615 2020-09-11 12:10:02.000000 bossman-0.9.0/bossman/plugins/akamai/lib/papi.py
+-rw-r--r--   0 ahogg      (503)      600     5896 2020-09-11 12:22:11.000000 bossman-0.9.0/bossman/plugins/akamai/property.py
+-rw-r--r--   0 ahogg      (503)      600     5664 2020-09-09 18:39:15.000000 bossman-0.9.0/bossman/repo.py
+-rw-r--r--   0 ahogg      (503)      600     1683 2020-09-09 17:08:31.000000 bossman-0.9.0/bossman/resources.py
+drwxr-xr-x   0 ahogg      (503)      600        0 2020-09-11 16:01:12.000000 bossman-0.9.0/bossman.egg-info/
+-rw-r--r--   0 ahogg      (503)      600     4579 2020-09-11 16:01:11.000000 bossman-0.9.0/bossman.egg-info/PKG-INFO
+-rw-r--r--   0 ahogg      (503)      600      759 2020-09-11 16:01:11.000000 bossman-0.9.0/bossman.egg-info/SOURCES.txt
+-rw-r--r--   0 ahogg      (503)      600        1 2020-09-11 16:01:11.000000 bossman-0.9.0/bossman.egg-info/dependency_links.txt
+-rw-r--r--   0 ahogg      (503)      600       46 2020-09-11 16:01:11.000000 bossman-0.9.0/bossman.egg-info/entry_points.txt
+-rw-r--r--   0 ahogg      (503)      600        1 2020-09-07 19:19:42.000000 bossman-0.9.0/bossman.egg-info/not-zip-safe
+-rw-r--r--   0 ahogg      (503)      600       70 2020-09-11 16:01:11.000000 bossman-0.9.0/bossman.egg-info/requires.txt
+-rw-r--r--   0 ahogg      (503)      600        8 2020-09-11 16:01:11.000000 bossman-0.9.0/bossman.egg-info/top_level.txt
+-rw-r--r--   0 ahogg      (503)      600       79 2020-09-11 16:01:12.000000 bossman-0.9.0/setup.cfg
+-rw-r--r--   0 ahogg      (503)      600     1014 2020-09-07 20:45:11.000000 bossman-0.9.0/setup.py
```

### Comparing `bossman-0.8.0/PKG-INFO` & `bossman-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bossman
-Version: 0.8.0
+Version: 0.9.0
 Summary: Automation framework
 Home-page: https://github.com/ynohat/bossman
 Author: Anthony Hogg
 Author-email: anthony@hogg.fr
 License: UNKNOWN
 Description: # Bossman
```

### Comparing `bossman-0.8.0/README.md` & `bossman-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `bossman-0.8.0/bossman/__init__.py` & `bossman-0.9.0/bossman/__init__.py`

 * *Files identical despite different names*

### Comparing `bossman-0.8.0/bossman/abc/resource.py` & `bossman-0.9.0/bossman/abc/resource.py`

 * *Files identical despite different names*

### Comparing `bossman-0.8.0/bossman/abc/resource_type.py` & `bossman-0.9.0/bossman/abc/resource_type.py`

 * *Files identical despite different names*

### Comparing `bossman-0.8.0/bossman/cli/__init__.py` & `bossman-0.9.0/bossman/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `bossman-0.8.0/bossman/cli/apply_cmd.py` & `bossman-0.9.0/bossman/cli/apply_cmd.py`

 * *Files identical despite different names*

### Comparing `bossman-0.8.0/bossman/cli/log_cmd.py` & `bossman-0.9.0/bossman/cli/log_cmd.py`

 * *Files identical despite different names*

### Comparing `bossman-0.8.0/bossman/cli/status_cmd.py` & `bossman-0.9.0/bossman/cli/status_cmd.py`

 * *Files identical despite different names*

### Comparing `bossman-0.8.0/bossman/config.py` & `bossman-0.9.0/bossman/config.py`

 * *Files identical despite different names*

### Comparing `bossman-0.8.0/bossman/errors.py` & `bossman-0.9.0/bossman/errors.py`

 * *Files identical despite different names*

### Comparing `bossman-0.8.0/bossman/git.py` & `bossman-0.9.0/bossman/git.py`

 * *Files identical despite different names*

### Comparing `bossman-0.8.0/bossman/plugins/akamai/lib/edgegrid.py` & `bossman-0.9.0/bossman/plugins/akamai/lib/edgegrid.py`

 * *Files identical despite different names*

### Comparing `bossman-0.8.0/bossman/plugins/akamai/lib/papi.py` & `bossman-0.9.0/bossman/plugins/akamai/lib/papi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import json
 from functools import lru_cache
 from bossman.plugins.akamai.lib.edgegrid import Session
 from bossman.logging import get_class_logger
+from bossman.cache import cache
+
+_cache = cache.key(__name__)
 
 class PAPIClient:
   def __init__(self, edgerc, section, switch_key=None, **kwargs):
     self.logger = get_class_logger(self)
     self.session = Session(edgerc, section, switch_key=switch_key, **kwargs)
 
   @lru_cache(maxsize=1000)
@@ -14,16 +17,22 @@
     response = self.session.post("/papi/v1/search/find-by-value", json={"propertyName": propertyName})
     self.logger.debug("find_by_property_name response={response}".format(response=response.content))
     versions = response.json().get("versions").get("items")
     return versions
 
   def get_property_id(self, propertyName):
     self.logger.debug("get_property_id propertyName={propertyName}".format(propertyName=propertyName))
-    versions = self.find_by_property_name(propertyName)
-    return versions[0].get("propertyId")
+    cache = _cache.key("property_id", propertyName)
+    property_id = cache.get_str()
+    if property_id is None:
+      versions = self.find_by_property_name(propertyName)
+      if len(versions) == 1:
+        property_id = str(versions[0].get("propertyId"))
+        cache.update(property_id)
+    return property_id
 
   def get_latest_property_version(self, propertyId, network=None):
     self.logger.debug("get_latest_property_version propertyId={propertyId} network={network}".format(propertyId=propertyId, network=network))
     params = dict()
     if not network is None:
       params["activatedOn"] = network
     url = "/papi/v1/properties/{propertyId}/versions/latest".format(propertyId=propertyId)
```

### Comparing `bossman-0.8.0/bossman/plugins/akamai/property.py` & `bossman-0.9.0/bossman/plugins/akamai/property.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import re
 import json
 from os import getenv
 from os.path import expanduser, basename, dirname, join
 
+from bossman.cache import cache
 from bossman.errors import BossmanError
 from bossman.abc.resource_type import ResourceTypeABC
 from bossman.abc.resource import ResourceABC
 from bossman.repo import Revision
 from bossman.plugins.akamai.lib.papi import PAPIClient
 from bossman.resources import RemoteRev
 
 RE_COMMIT = re.compile("^commit: ([a-z0-9]*)", re.MULTILINE)
 
+_cache = cache.key(__name__)
+
 class PropertyError(BossmanError):
   def __rich__(self):
     return "{}: {}".format(self.__class__.__name__, " ".join(self.args))
 
 class PropertyResource(ResourceABC):
   def __init__(self, path, **kwargs):
     super(PropertyResource, self).__init__(path)
@@ -48,22 +51,27 @@
 
   def create_resource(self, path: str, **kwargs):
     return PropertyResource(path, **kwargs)
 
   def get_remote_rev(self, resource: PropertyResource) -> str:
     local_rev, remote_rev = None, None
     property_id = self.papi.get_property_id(resource.name)
-    property_version = self.papi.find_latest_property_version(
-      property_id,
-      lambda v: RE_COMMIT.search(v.get("note", ""))
-    )
-    self.logger.info("get_remote_rev {property_name} -> {property_version}".format(property_name=resource.name, property_version=property_version))
-    if property_version:
-      remote_rev = property_version.get("propertyVersion")
-      local_rev = RE_COMMIT.search(property_version.get("note")).group(1)
+    cache = _cache.key("remote_version", property_id)
+    remote_version = cache.get_json()
+    if remote_version is None:
+      remote_version = self.papi.find_latest_property_version(
+        property_id,
+        lambda v: RE_COMMIT.search(v.get("note", ""))
+      )
+      self.logger.info("get_remote_rev {property_name} -> {property_version}".format(property_name=resource.name, property_version=remote_version))
+      if remote_version:
+        cache.update_json(remote_version)
+    if remote_version:
+      remote_rev = remote_version.get("propertyVersion")
+      local_rev = RE_COMMIT.search(remote_version.get("note")).group(1)
     return RemoteRev(local_rev=local_rev, remote_rev=remote_rev)
 
   def is_dirty(self, resource: PropertyResource) -> bool:
     """
     An Akamai property is dirty if its latest version does not refer to a
     revision in its notes.
     """
@@ -119,11 +127,16 @@
       self.papi.update_property_hostnames(property_id, next_version.get("propertyVersion"), hostnames_json)
     # then, regardless of whether there was a change to the rule tree, we need to update it with
     # the commit message and id, otherwise we will get a dirty status
     rules_json.update(comments="{}\n\ncommit: {}".format(revision.message.strip(), revision.id))
     self.papi.update_property_rule_tree(property_id, next_version.get("propertyVersion"), rules_json)
 
   def get_property_version_for_revision_id(self, property_id, revision_id):
-    search = r'commit: {}'.format(revision_id)
-    predicate = lambda v: search in v.get("note", "")
-    property_version = self.papi.find_latest_property_version(property_id, predicate)
+    cache = _cache.key("property_version", property_id, revision_id)
+    property_version = cache.get_str()
+    if property_version is None:
+      search = r'commit: {}'.format(revision_id)
+      predicate = lambda v: search in v.get("note", "")
+      property_version = self.papi.find_latest_property_version(property_id, predicate)
+      if property_version != None:
+        cache.update(property_version)
     return property_version
```

### Comparing `bossman-0.8.0/bossman/repo.py` & `bossman-0.9.0/bossman/repo.py`

 * *Files identical despite different names*

### Comparing `bossman-0.8.0/bossman/resources.py` & `bossman-0.9.0/bossman/resources.py`

 * *Files identical despite different names*

### Comparing `bossman-0.8.0/bossman.egg-info/PKG-INFO` & `bossman-0.9.0/bossman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bossman
-Version: 0.8.0
+Version: 0.9.0
 Summary: Automation framework
 Home-page: https://github.com/ynohat/bossman
 Author: Anthony Hogg
 Author-email: anthony@hogg.fr
 License: UNKNOWN
 Description: # Bossman
```

### Comparing `bossman-0.8.0/bossman.egg-info/SOURCES.txt` & `bossman-0.9.0/bossman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bossman-0.8.0/setup.py` & `bossman-0.9.0/setup.py`

 * *Files identical despite different names*

