# Comparing `tmp/routingfilter-1.3.1.tar.gz` & `tmp/routingfilter-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routingfilter-1.3.1.tar", last modified: Fri Feb  4 16:06:17 2022, max compression
+gzip compressed data, was "routingfilter-1.3.2.tar", last modified: Mon Mar 14 13:41:00 2022, max compression
```

## Comparing `routingfilter-1.3.1.tar` & `routingfilter-1.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:06:17.223631 routingfilter-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-02-04 16:06:06.000000 routingfilter-1.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-04 16:06:06.000000 routingfilter-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-02-04 16:06:17.223631 routingfilter-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-02-04 16:06:06.000000 routingfilter-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-02-04 16:06:06.000000 routingfilter-1.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:06:17.223631 routingfilter-1.3.1/routingfilter/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:06:06.000000 routingfilter-1.3.1/routingfilter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8175 2022-02-04 16:06:06.000000 routingfilter-1.3.1/routingfilter/configfilter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2191 2022-02-04 16:06:06.000000 routingfilter-1.3.1/routingfilter/dictquery.py
--rw-r--r--   0 runner    (1001) docker     (121)     6982 2022-02-04 16:06:06.000000 routingfilter-1.3.1/routingfilter/routing.py
--rw-r--r--   0 runner    (1001) docker     (121)    11687 2022-02-04 16:06:06.000000 routingfilter-1.3.1/routingfilter/routing_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:06:17.223631 routingfilter-1.3.1/routingfilter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-02-04 16:06:17.000000 routingfilter-1.3.1/routingfilter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-02-04 16:06:17.000000 routingfilter-1.3.1/routingfilter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 16:06:17.000000 routingfilter-1.3.1/routingfilter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-02-04 16:06:17.000000 routingfilter-1.3.1/routingfilter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-02-04 16:06:17.000000 routingfilter-1.3.1/routingfilter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-04 16:06:17.223631 routingfilter-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      904 2022-02-04 16:06:06.000000 routingfilter-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 13:41:00.514457 routingfilter-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-03-14 13:40:46.000000 routingfilter-1.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-14 13:40:46.000000 routingfilter-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-03-14 13:41:00.514457 routingfilter-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      476 2022-03-14 13:40:46.000000 routingfilter-1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-03-14 13:40:46.000000 routingfilter-1.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 13:41:00.514457 routingfilter-1.3.2/routingfilter/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-14 13:40:46.000000 routingfilter-1.3.2/routingfilter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8279 2022-03-14 13:40:46.000000 routingfilter-1.3.2/routingfilter/configfilter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2191 2022-03-14 13:40:46.000000 routingfilter-1.3.2/routingfilter/dictquery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6982 2022-03-14 13:40:46.000000 routingfilter-1.3.2/routingfilter/routing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11640 2022-03-14 13:40:46.000000 routingfilter-1.3.2/routingfilter/routing_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 13:41:00.514457 routingfilter-1.3.2/routingfilter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-03-14 13:41:00.000000 routingfilter-1.3.2/routingfilter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      379 2022-03-14 13:41:00.000000 routingfilter-1.3.2/routingfilter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-14 13:41:00.000000 routingfilter-1.3.2/routingfilter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-03-14 13:41:00.000000 routingfilter-1.3.2/routingfilter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-03-14 13:41:00.000000 routingfilter-1.3.2/routingfilter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-14 13:41:00.514457 routingfilter-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      904 2022-03-14 13:40:46.000000 routingfilter-1.3.2/setup.py
```

### Comparing `routingfilter-1.3.1/LICENSE.txt` & `routingfilter-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `routingfilter-1.3.1/PKG-INFO` & `routingfilter-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routingfilter
-Version: 1.3.1
+Version: 1.3.2
 Summary: Generic Business Logic Implementation for Routing objects as python dictionaries
 Home-page: https://github.com/certego/RoutingFilter
 Author: Certego S.r.l.
 Author-email: support@certego.net
 License: GNU LGPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `routingfilter-1.3.1/routingfilter/configfilter.py` & `routingfilter-1.3.2/routingfilter/configfilter.py`

 * *Files 5% similar despite different names*

```diff
@@ -158,17 +158,17 @@
 
     def __check_network(self, target):
         for value in self.value:
             try:
                 if target in IP(value):
                     return True
             except ValueError:
-                raise ValueError(f"Invalid IP/network address: {value}")
+                self.logger.error(f"Unparsable IP/network address (malformed). Filter value: {value}; source field value: {target}")
             except TypeError:
-                self.logger.warning(f"Unparsable IP/network address (wrong type): {value}")
+                self.logger.warning(f"Unparsable IP/network address (wrong type). Filter value: {value}; source field value: {target}")
         return False
 
     def _filter_NOT_NETWORK(self, data):
         return not self._filter_NETWORK(data)
 
     def _filter_DOMAIN(self, data):
         for key in self.key:
```

### Comparing `routingfilter-1.3.1/routingfilter/dictquery.py` & `routingfilter-1.3.2/routingfilter/dictquery.py`

 * *Files identical despite different names*

### Comparing `routingfilter-1.3.1/routingfilter/routing.py` & `routingfilter-1.3.2/routingfilter/routing.py`

 * *Files identical despite different names*

### Comparing `routingfilter-1.3.1/routingfilter/routing_test.py` & `routingfilter-1.3.2/routingfilter/routing_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import unittest
 
 from routingfilter.routing import Routing
 
 
 def load_test_data(name):
     """Load a JSON test file from 'test_data' folder, given its name (extension excluded), and parse it into a dictionary."""
-    with open(os.path.join('routingfilter/test_data', name + '.json')) as file:
+    with open(os.path.join('test_data', name + '.json')) as file:
         data = json.load(file)
     return data
 
 
 class RoutingTestCase(unittest.TestCase):
     """Class to tests routing.py file. These tests loads sample events from JSON files in 'test_data' folder
     and test if the routing rules are working correctly."""
@@ -181,23 +181,21 @@
         self.assertFalse(self.routing.match(self.test_event_10))
 
     def test_single_filter_NETWORK_NOT_NETWORK(self):
         self.routing.load_from_dicts([load_test_data("test_rule_9_network")])  # NETWORK
         self.assertTrue(self.routing.match(self.test_event_4))
         self.assertFalse(self.routing.match(self.test_event_5))
         self.assertFalse(self.routing.match(self.test_event_9))
-        with self.assertRaises(ValueError):
-            self.routing.match(self.test_event_6)
+        self.assertFalse(self.routing.match(self.test_event_6))  # Unparsable
         self.routing.load_from_dicts([load_test_data("test_rule_10_not_network")])  # NOT_NETWORK
         self.assertFalse(self.routing.match(self.test_event_4))
         self.assertTrue(self.routing.match(self.test_event_5))
         self.assertFalse(self.routing.match(self.test_event_3))
         self.assertTrue(self.routing.match(self.test_event_9))
-        with self.assertRaises(ValueError):
-            self.routing.match(self.test_event_6)
+        self.assertTrue(self.routing.match(self.test_event_6))  # Unparsable
 
     def test_event_with_lists_as_fields(self):
         self.routing.load_from_dicts([load_test_data("test_rule_9_network")])  # NETWORK
         self.assertTrue(self.routing.match(self.test_event_with_list_1))
 
         self.routing.load_from_dicts([load_test_data("test_rule_1_equals")])
         self.assertTrue(self.routing.match(self.test_event_with_list_2))
```

### Comparing `routingfilter-1.3.1/routingfilter.egg-info/PKG-INFO` & `routingfilter-1.3.2/routingfilter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routingfilter
-Version: 1.3.1
+Version: 1.3.2
 Summary: Generic Business Logic Implementation for Routing objects as python dictionaries
 Home-page: https://github.com/certego/RoutingFilter
 Author: Certego S.r.l.
 Author-email: support@certego.net
 License: GNU LGPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `routingfilter-1.3.1/setup.py` & `routingfilter-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='routingfilter',
-    version='1.3.1',
+    version='1.3.2',
     packages=['routingfilter'],
     include_package_data=True,
     install_requires=["IPy"],
     url='https://github.com/certego/RoutingFilter',
     license='GNU LGPLv3',
     author='Certego S.r.l.',
     author_email='support@certego.net',
```

