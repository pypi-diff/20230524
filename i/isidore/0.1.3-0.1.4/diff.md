# Comparing `tmp/isidore-0.1.3.tar.gz` & `tmp/isidore-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/media/data/Documents/Programs/isidore/lib/dist/.tmp-gjmd_icc/isidore-0.1.3.tar", last modified: Mon May 22 18:47:57 2023, max compression
+gzip compressed data, was "/media/data/Documents/Programs/isidore/lib/dist/.tmp-gvw_81_m/isidore-0.1.4.tar", last modified: Wed May 24 17:38:01 2023, max compression
```

## Comparing `isidore-0.1.3.tar` & `isidore-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 18:47:57.000000 isidore-0.1.3/
--rw-r--r--   0 scott     (1000) scott     (1000)     1063 2023-05-06 12:39:48.000000 isidore-0.1.3/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     1002 2023-05-22 18:47:57.000000 isidore-0.1.3/PKG-INFO
--rw-r--r--   0 scott     (1000) scott     (1000)      245 2023-05-12 17:10:25.000000 isidore-0.1.3/README.md
--rw-r--r--   0 scott     (1000) scott     (1000)      880 2023-05-22 18:47:38.000000 isidore-0.1.3/pyproject.toml
--rw-r--r--   0 scott     (1000) scott     (1000)       38 2023-05-22 18:47:57.000000 isidore-0.1.3/setup.cfg
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 18:47:57.000000 isidore-0.1.3/src/
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 18:47:57.000000 isidore-0.1.3/src/isidore/
--rw-r--r--   0 scott     (1000) scott     (1000)        1 2023-05-12 12:18:21.000000 isidore-0.1.3/src/isidore/__init__.py
--rw-r--r--   0 scott     (1000) scott     (1000)    32541 2023-05-22 18:47:38.000000 isidore-0.1.3/src/isidore/libIsidore.py
--rw-r--r--   0 scott     (1000) scott     (1000)    37498 2023-05-22 18:47:38.000000 isidore-0.1.3/src/isidore/libIsidoreCmdline.py
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-22 18:47:57.000000 isidore-0.1.3/src/isidore.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     1002 2023-05-22 18:47:57.000000 isidore-0.1.3/src/isidore.egg-info/PKG-INFO
--rw-r--r--   0 scott     (1000) scott     (1000)      289 2023-05-22 18:47:57.000000 isidore-0.1.3/src/isidore.egg-info/SOURCES.txt
--rw-r--r--   0 scott     (1000) scott     (1000)        1 2023-05-22 18:47:57.000000 isidore-0.1.3/src/isidore.egg-info/dependency_links.txt
--rw-r--r--   0 scott     (1000) scott     (1000)       30 2023-05-22 18:47:57.000000 isidore-0.1.3/src/isidore.egg-info/requires.txt
--rw-r--r--   0 scott     (1000) scott     (1000)        8 2023-05-22 18:47:57.000000 isidore-0.1.3/src/isidore.egg-info/top_level.txt
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-24 17:38:01.000000 isidore-0.1.4/
+-rw-r--r--   0 scott     (1000) scott     (1000)     1063 2023-05-06 12:39:48.000000 isidore-0.1.4/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     1002 2023-05-24 17:38:01.000000 isidore-0.1.4/PKG-INFO
+-rw-r--r--   0 scott     (1000) scott     (1000)      245 2023-05-12 17:10:25.000000 isidore-0.1.4/README.md
+-rw-r--r--   0 scott     (1000) scott     (1000)      880 2023-05-24 17:37:13.000000 isidore-0.1.4/pyproject.toml
+-rw-r--r--   0 scott     (1000) scott     (1000)       38 2023-05-24 17:38:01.000000 isidore-0.1.4/setup.cfg
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-24 17:38:01.000000 isidore-0.1.4/src/
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-24 17:38:01.000000 isidore-0.1.4/src/isidore/
+-rw-r--r--   0 scott     (1000) scott     (1000)        1 2023-05-12 12:18:21.000000 isidore-0.1.4/src/isidore/__init__.py
+-rw-r--r--   0 scott     (1000) scott     (1000)    33953 2023-05-24 17:37:13.000000 isidore-0.1.4/src/isidore/libIsidore.py
+-rw-r--r--   0 scott     (1000) scott     (1000)    37675 2023-05-24 17:37:13.000000 isidore-0.1.4/src/isidore/libIsidoreCmdline.py
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-24 17:38:01.000000 isidore-0.1.4/src/isidore.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     1002 2023-05-24 17:38:01.000000 isidore-0.1.4/src/isidore.egg-info/PKG-INFO
+-rw-r--r--   0 scott     (1000) scott     (1000)      289 2023-05-24 17:38:01.000000 isidore-0.1.4/src/isidore.egg-info/SOURCES.txt
+-rw-r--r--   0 scott     (1000) scott     (1000)        1 2023-05-24 17:38:01.000000 isidore-0.1.4/src/isidore.egg-info/dependency_links.txt
+-rw-r--r--   0 scott     (1000) scott     (1000)       30 2023-05-24 17:38:01.000000 isidore-0.1.4/src/isidore.egg-info/requires.txt
+-rw-r--r--   0 scott     (1000) scott     (1000)        8 2023-05-24 17:38:01.000000 isidore-0.1.4/src/isidore.egg-info/top_level.txt
```

### Comparing `isidore-0.1.3/LICENSE` & `isidore-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `isidore-0.1.3/PKG-INFO` & `isidore-0.1.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isidore
-Version: 0.1.3
+Version: 0.1.4
 Summary: database, API, and CLI suite for managing Ansible inventories
 Author-email: Scott Court <Z5T1@Z5T1.com>
 Project-URL: Homepage, https://github.com/Z5T1/isidore
 Project-URL: Bug Tracker, https://github.com/Z5T1/isidore/issues
 Project-URL: Documentation, https://github.com/Z5T1/isidore/blob/master/doc/README.md
 Project-URL: Discord, https://discord.gg/c357N3JQFJ
 Project-URL: Source Code, https://github.com/Z5T1/isidore
```

### Comparing `isidore-0.1.3/pyproject.toml` & `isidore-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "isidore"
-version = "0.1.3"
+version = "0.1.4"
 keywords = [ "ansible", "inventory", "database", "isidore" ]
 authors = [
   { name="Scott Court", email="Z5T1@Z5T1.com" },
 ]
 description = "database, API, and CLI suite for managing Ansible inventories"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `isidore-0.1.3/src/isidore/libIsidore.py` & `isidore-0.1.4/src/isidore/libIsidore.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import yaml
 import json
 
 # Represents an Isidore database instance
 class Isidore:
 
     _conn = None
-    _version = '0.1.3'
+    _version = '0.1.4'
 
     # Connects to a MySQL database and creates a new Isidore object to interact
     # with it.
     # @param user       The MySQL username
     # @param password   The password for the MySQL user
     # @param host       The MySQL server to connect to
     # @param database   The name of the database to use
@@ -298,15 +298,49 @@
 
         return json.dumps(inv)
 
     # Builds an Ansible inventory in YAML format from all hosts
     # and tags in the database
     # @return       the Ansible YAML inventory as a string
     def getInventoryYaml(self):
-        return yaml.dump(self.getInventory(), default_flow_style=False)
+        # Any variables assigned to the 'all' tag require special treatment
+        # since it goes at the top of the YAML tree unlike all the other tags.
+        tag_all = self.getTag('all')
+        inv = {
+                'all': {
+                    'hosts': dict(),
+                    'children': dict(),
+                    'vars': dict() if tag_all == None
+                        else tag_all.getDetails()['all']['vars']
+                }
+        }
+
+        # Add all the hosts without a group to ensure every system is included,
+        # even those without any tags.
+        for host in self.getCommissionedHosts():
+            name = host.getHostname()
+            inv['all']['hosts'][name] = host.getDetails()[name]['vars']
+
+        # Add each tag and its hosts as a group
+        for tag in self.getTags(True):
+            name = tag.getName()
+            details = tag.getDetails()
+            # Skip the all tag since it requires special care and is handled
+            # above
+            if name == 'all':
+                continue
+            inv['all']['children'][name] = {
+                    'hosts': dict.fromkeys(details[name]['hosts'], dict()),
+                    'vars': details[name]['vars']
+            }
+
+        # Generate YAML output without any anchors/aliases
+        noalias_dumper = yaml.dumper.SafeDumper
+        noalias_dumper.ignore_aliases = lambda self, data: True
+        return yaml.dump(inv, default_flow_style=False, Dumper=noalias_dumper)
 
     # Gets a tag in the database
     # @param name       The name of the tag to get
     # @return           The Tag object, or None if the tag does
     #                   not exist.
     def getTag(self, name):
         cursor = self._conn.cursor()
```

### Comparing `isidore-0.1.3/src/isidore/libIsidoreCmdline.py` & `isidore-0.1.4/src/isidore/libIsidoreCmdline.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 from isidore.libIsidore import *
 
 # The Isidore command prompt
 class IsidoreCmdline:
 
     _isidore = None
-    _version = '0.1.3'
+    _version = '0.1.4'
 
     # Creates a new Isidore command prompt
     # @param isidore    The underlying Isidore instance for the command prompt
     #                   to connect to.
     def __init__(self, isidore):
         self._isidore = isidore
 
@@ -236,18 +236,21 @@
     def show_inventory(self, args):
         if len(args) == 2:
             print(self._isidore.getInventoryIni())
 
         elif args[2] == '?':
             print('''\
 ?           print this help message
+human       print the inventory in a human friendly format
 ini         print the inventory in INI format
 json        print the inventory in JSON format
 yaml        print the inventory in YAML format''')
 
+        elif args[2] == 'human':
+            print(yaml.dump(self._isidore.getInventory(), default_flow_style=False))
         elif args[2] == 'ini':
             print(self._isidore.getInventoryIni())
         elif args[2] == 'json':
             print(self._isidore.getInventoryJson())
         elif args[2] == 'yaml':
             print(self._isidore.getInventoryYaml())
         else:
```

### Comparing `isidore-0.1.3/src/isidore.egg-info/PKG-INFO` & `isidore-0.1.4/src/isidore.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isidore
-Version: 0.1.3
+Version: 0.1.4
 Summary: database, API, and CLI suite for managing Ansible inventories
 Author-email: Scott Court <Z5T1@Z5T1.com>
 Project-URL: Homepage, https://github.com/Z5T1/isidore
 Project-URL: Bug Tracker, https://github.com/Z5T1/isidore/issues
 Project-URL: Documentation, https://github.com/Z5T1/isidore/blob/master/doc/README.md
 Project-URL: Discord, https://discord.gg/c357N3JQFJ
 Project-URL: Source Code, https://github.com/Z5T1/isidore
```

