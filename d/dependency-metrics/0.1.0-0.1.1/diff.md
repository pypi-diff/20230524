# Comparing `tmp/dependency-metrics-0.1.0.tar.gz` & `tmp/dependency-metrics-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dependency-metrics-0.1.0.tar", last modified: Wed May 17 08:30:30 2023, max compression
+gzip compressed data, was "dependency-metrics-0.1.1.tar", last modified: Wed May 24 19:29:16 2023, max compression
```

## Comparing `dependency-metrics-0.1.0.tar` & `dependency-metrics-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 grahamherceg   (501) staff       (20)        0 2023-05-17 08:30:30.576119 dependency-metrics-0.1.0/
--rw-r--r--   0 grahamherceg   (501) staff       (20)     1508 2023-05-01 19:34:19.000000 dependency-metrics-0.1.0/LICENSE
--rw-r--r--   0 grahamherceg   (501) staff       (20)     4556 2023-05-17 08:30:30.575408 dependency-metrics-0.1.0/PKG-INFO
--rw-r--r--   0 grahamherceg   (501) staff       (20)     2268 2023-05-03 19:26:00.000000 dependency-metrics-0.1.0/README.md
-drwxr-xr-x   0 grahamherceg   (501) staff       (20)        0 2023-05-17 08:30:30.558359 dependency-metrics-0.1.0/dependency_metrics/
--rw-r--r--   0 grahamherceg   (501) staff       (20)      308 2023-05-17 08:04:35.000000 dependency-metrics-0.1.0/dependency_metrics/constants.py
--rw-r--r--   0 grahamherceg   (501) staff       (20)     2653 2023-05-17 08:04:35.000000 dependency-metrics-0.1.0/dependency_metrics/datadog_utils.py
--rw-r--r--   0 grahamherceg   (501) staff       (20)       57 2023-05-01 19:34:19.000000 dependency-metrics-0.1.0/dependency_metrics/exceptions.py
--rw-r--r--   0 grahamherceg   (501) staff       (20)     3239 2023-05-01 19:34:19.000000 dependency-metrics-0.1.0/dependency_metrics/metrics.py
-drwxr-xr-x   0 grahamherceg   (501) staff       (20)        0 2023-05-17 08:30:30.568035 dependency-metrics-0.1.0/dependency_metrics/package_managers/
--rw-r--r--   0 grahamherceg   (501) staff       (20)        0 2023-05-01 19:34:19.000000 dependency-metrics-0.1.0/dependency_metrics/package_managers/__init__.py
--rw-r--r--   0 grahamherceg   (501) staff       (20)      562 2023-05-02 18:45:11.000000 dependency-metrics-0.1.0/dependency_metrics/package_managers/pip.py
--rw-r--r--   0 grahamherceg   (501) staff       (20)     1052 2023-05-01 19:34:19.000000 dependency-metrics-0.1.0/dependency_metrics/package_managers/utils.py
--rw-r--r--   0 grahamherceg   (501) staff       (20)     3517 2023-05-17 08:04:35.000000 dependency-metrics-0.1.0/dependency_metrics/package_managers/yarn.py
--rw-r--r--   0 grahamherceg   (501) staff       (20)      960 2023-05-01 19:34:19.000000 dependency-metrics-0.1.0/dependency_metrics/parsing_utils.py
-drwxr-xr-x   0 grahamherceg   (501) staff       (20)        0 2023-05-17 08:30:30.564940 dependency-metrics-0.1.0/dependency_metrics.egg-info/
--rw-r--r--   0 grahamherceg   (501) staff       (20)     4556 2023-05-17 08:30:30.000000 dependency-metrics-0.1.0/dependency_metrics.egg-info/PKG-INFO
--rw-r--r--   0 grahamherceg   (501) staff       (20)      711 2023-05-17 08:30:30.000000 dependency-metrics-0.1.0/dependency_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 grahamherceg   (501) staff       (20)        1 2023-05-17 08:30:30.000000 dependency-metrics-0.1.0/dependency_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 grahamherceg   (501) staff       (20)       60 2023-05-17 08:30:30.000000 dependency-metrics-0.1.0/dependency_metrics.egg-info/entry_points.txt
--rw-r--r--   0 grahamherceg   (501) staff       (20)       43 2023-05-17 08:30:30.000000 dependency-metrics-0.1.0/dependency_metrics.egg-info/requires.txt
--rw-r--r--   0 grahamherceg   (501) staff       (20)       19 2023-05-17 08:30:30.000000 dependency-metrics-0.1.0/dependency_metrics.egg-info/top_level.txt
--rw-r--r--   0 grahamherceg   (501) staff       (20)      932 2023-05-17 08:28:43.000000 dependency-metrics-0.1.0/pyproject.toml
--rw-r--r--   0 grahamherceg   (501) staff       (20)       38 2023-05-17 08:30:30.576523 dependency-metrics-0.1.0/setup.cfg
-drwxr-xr-x   0 grahamherceg   (501) staff       (20)        0 2023-05-17 08:30:30.574051 dependency-metrics-0.1.0/tests/
--rw-r--r--   0 grahamherceg   (501) staff       (20)     3493 2023-05-17 08:04:35.000000 dependency-metrics-0.1.0/tests/test_datadog_utils.py
--rw-r--r--   0 grahamherceg   (501) staff       (20)     2569 2023-05-01 19:34:19.000000 dependency-metrics-0.1.0/tests/test_metrics.py
--rw-r--r--   0 grahamherceg   (501) staff       (20)     2475 2023-05-01 19:34:19.000000 dependency-metrics-0.1.0/tests/test_parsing_utils.py
+drwxr-xr-x   0 grahamherceg   (501) staff       (20)        0 2023-05-24 19:29:16.454564 dependency-metrics-0.1.1/
+-rw-r--r--   0 grahamherceg   (501) staff       (20)     1508 2023-05-01 19:34:19.000000 dependency-metrics-0.1.1/LICENSE
+-rw-r--r--   0 grahamherceg   (501) staff       (20)     4565 2023-05-24 19:29:16.454235 dependency-metrics-0.1.1/PKG-INFO
+-rw-r--r--   0 grahamherceg   (501) staff       (20)     2278 2023-05-24 19:13:45.000000 dependency-metrics-0.1.1/README.md
+drwxr-xr-x   0 grahamherceg   (501) staff       (20)        0 2023-05-24 19:29:16.444975 dependency-metrics-0.1.1/dependency_metrics/
+-rw-r--r--   0 grahamherceg   (501) staff       (20)      308 2023-05-17 08:04:35.000000 dependency-metrics-0.1.1/dependency_metrics/constants.py
+-rw-r--r--   0 grahamherceg   (501) staff       (20)     2679 2023-05-24 19:13:45.000000 dependency-metrics-0.1.1/dependency_metrics/datadog_utils.py
+-rw-r--r--   0 grahamherceg   (501) staff       (20)       57 2023-05-01 19:34:19.000000 dependency-metrics-0.1.1/dependency_metrics/exceptions.py
+-rw-r--r--   0 grahamherceg   (501) staff       (20)     3880 2023-05-24 19:13:45.000000 dependency-metrics-0.1.1/dependency_metrics/metrics.py
+drwxr-xr-x   0 grahamherceg   (501) staff       (20)        0 2023-05-24 19:29:16.451673 dependency-metrics-0.1.1/dependency_metrics/package_managers/
+-rw-r--r--   0 grahamherceg   (501) staff       (20)        0 2023-05-01 19:34:19.000000 dependency-metrics-0.1.1/dependency_metrics/package_managers/__init__.py
+-rw-r--r--   0 grahamherceg   (501) staff       (20)      830 2023-05-24 19:13:45.000000 dependency-metrics-0.1.1/dependency_metrics/package_managers/pip.py
+-rw-r--r--   0 grahamherceg   (501) staff       (20)     1638 2023-05-24 19:13:45.000000 dependency-metrics-0.1.1/dependency_metrics/package_managers/utils.py
+-rw-r--r--   0 grahamherceg   (501) staff       (20)     3660 2023-05-24 19:13:45.000000 dependency-metrics-0.1.1/dependency_metrics/package_managers/yarn.py
+-rw-r--r--   0 grahamherceg   (501) staff       (20)      960 2023-05-01 19:34:19.000000 dependency-metrics-0.1.1/dependency_metrics/parsing_utils.py
+drwxr-xr-x   0 grahamherceg   (501) staff       (20)        0 2023-05-24 19:29:16.449065 dependency-metrics-0.1.1/dependency_metrics.egg-info/
+-rw-r--r--   0 grahamherceg   (501) staff       (20)     4565 2023-05-24 19:29:16.000000 dependency-metrics-0.1.1/dependency_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 grahamherceg   (501) staff       (20)      711 2023-05-24 19:29:16.000000 dependency-metrics-0.1.1/dependency_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 grahamherceg   (501) staff       (20)        1 2023-05-24 19:29:16.000000 dependency-metrics-0.1.1/dependency_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 grahamherceg   (501) staff       (20)       60 2023-05-24 19:29:16.000000 dependency-metrics-0.1.1/dependency_metrics.egg-info/entry_points.txt
+-rw-r--r--   0 grahamherceg   (501) staff       (20)       43 2023-05-24 19:29:16.000000 dependency-metrics-0.1.1/dependency_metrics.egg-info/requires.txt
+-rw-r--r--   0 grahamherceg   (501) staff       (20)       19 2023-05-24 19:29:16.000000 dependency-metrics-0.1.1/dependency_metrics.egg-info/top_level.txt
+-rw-r--r--   0 grahamherceg   (501) staff       (20)      932 2023-05-24 19:29:02.000000 dependency-metrics-0.1.1/pyproject.toml
+-rw-r--r--   0 grahamherceg   (501) staff       (20)       38 2023-05-24 19:29:16.454661 dependency-metrics-0.1.1/setup.cfg
+drwxr-xr-x   0 grahamherceg   (501) staff       (20)        0 2023-05-24 19:29:16.453564 dependency-metrics-0.1.1/tests/
+-rw-r--r--   0 grahamherceg   (501) staff       (20)     3493 2023-05-17 08:04:35.000000 dependency-metrics-0.1.1/tests/test_datadog_utils.py
+-rw-r--r--   0 grahamherceg   (501) staff       (20)     2673 2023-05-24 19:13:45.000000 dependency-metrics-0.1.1/tests/test_metrics.py
+-rw-r--r--   0 grahamherceg   (501) staff       (20)     2475 2023-05-01 19:34:19.000000 dependency-metrics-0.1.1/tests/test_parsing_utils.py
```

### Comparing `dependency-metrics-0.1.0/LICENSE` & `dependency-metrics-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dependency-metrics-0.1.0/PKG-INFO` & `dependency-metrics-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dependency-metrics
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python tool to track outdated dependencies.
 Author-email: Dimagi <dev@dimagi.com>
 Maintainer-email: Dimagi <dev@dimagi.com>
 License: Copyright (c) 2023, Dimagi Inc., and individual contributors.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -70,14 +70,15 @@
 
 #### --stats option
 
 Use the `--stats` option to generate a simple dictionary that displays the total number of outdated dependencies, as well as a breakdown detailing the number of outdated dependencies for each version type.
 
 ```commandline
 $ metrics pip --stats
+Total: 5
 Outdated: 2
 Multi-Major: 1
 Major: 0
 Minor: 1
 Patch: 0
 Unknown: 0
 ```
```

### Comparing `dependency-metrics-0.1.0/README.md` & `dependency-metrics-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 #### --stats option
 
 Use the `--stats` option to generate a simple dictionary that displays the total number of outdated dependencies, as well as a breakdown detailing the number of outdated dependencies for each version type.
 
 ```commandline
 $ metrics pip --stats
+Total: 5
 Outdated: 2
 Multi-Major: 1
 Major: 0
 Minor: 1
 Patch: 0
 Unknown: 0
 ```
```

### Comparing `dependency-metrics-0.1.0/dependency_metrics/datadog_utils.py` & `dependency-metrics-0.1.1/dependency_metrics/datadog_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
         YARN: "js",
     }
     return metric_name_map[key]
 
 
 def get_metric_name_for_stats_key(key):
     metric_name_map = {
+        "Total": "total",
         "Outdated": "outdated",
         "Multi-Major": "multi_major_outdated",
         "Major": "major_outdated",
         "Minor": "minor_outdated",
         "Patch": "patch_outdated",
         "Unknown": "unknown"
     }
```

### Comparing `dependency-metrics-0.1.0/dependency_metrics/metrics.py` & `dependency-metrics-0.1.1/dependency_metrics/metrics.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 import argparse
 
 from dependency_metrics.constants import PIP, YARN
 from dependency_metrics.datadog_utils import send_stats_to_datadog
-from dependency_metrics.package_managers.utils import iter_packages
+from dependency_metrics.package_managers.utils import (get_total_package_count,
+                                                       iter_outdated_packages)
+
+
+def print_packages_table(package_manager):
+    outdated_packages = iter_outdated_packages(package_manager)
+    for row in build_packages_table(outdated_packages):
+        print(row)
 
 
 def build_packages_table(packages):
     """ Builds a table representing how out of date dependencies are
     Example:
     Behind   Package                      Latest       Version
     n/a      At.js                        exotic       1.5.3
@@ -27,15 +34,26 @@
         else:
             behind = "n/a"
         rows.append(build_row(behind, name, current, latest))
 
     return rows
 
 
-def get_package_stats(packages):
+def get_package_stats(package_manager):
+    """
+    Adds a total count to the dictionary returned by get_outdated_package_stats
+    """
+    outdated_packages = iter_outdated_packages(package_manager)
+    outdated_stats = get_outdated_package_stats(outdated_packages)
+    total_stats = {"Total": get_total_package_count(package_manager)}
+    # overcomplicated to ensure the Total key is first in the dictionary
+    return {**total_stats, **outdated_stats}
+
+
+def get_outdated_package_stats(packages):
     """Displays a count for each version category of out of date dependencies"""
     stats = {
         "Outdated": 0,
         "Multi-Major": 0,
         "Major": 0,
         "Minor": 0,
         "Patch": 0,
@@ -83,26 +101,23 @@
         "--send",
         help="generate statistics and send to datadog",
         default=False,
         action="store_true"
     )
     args = parser.parse_args()
 
-    packages = iter_packages(args.package_manager)
     if args.stats or args.send:
-        stats = get_package_stats(packages)
+        stats = get_package_stats(args.package_manager)
         if args.stats:
             # NOTE: subtle detail: we're depending on Python 3's ordered dict to
             # maintain deterministic ordering here
             for key, value in stats.items():
                 print(f"{key}: {value}")
         elif args.send:
             send_stats_to_datadog(stats, args.package_manager)
 
     else:
-        package_table = build_packages_table(packages)
-        for row in package_table:
-            print(row)
+        print_packages_table(args.package_manager)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dependency-metrics-0.1.0/dependency_metrics/package_managers/yarn.py` & `dependency-metrics-0.1.1/dependency_metrics/package_managers/yarn.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,29 +27,36 @@
 
 If new information is found that clearly states yarn package names are 
 case-insensitive, then the behavior can change to retry package names that fail 
 with a lower cased version of the name.
 """
 
 
-def get_yarn_packages():
+def get_outdated_yarn_packages():
     version = Yarn.version()
     if not version.startswith("1."):
         raise Crash(f"Yarn Classic (v1.x) is required, found {version}")
 
     outdated_packages = []
     for package in parse_yarn_list():
         latest_version = pull_latest_version(package["name"])
         if package["version"] != latest_version:
             # only care if it is actually outdated
             package["latest_version"] = latest_version
             outdated_packages.append(package)
     return outdated_packages
 
 
+def get_total_count_for_yarn():
+    """
+    Return total number of installed dependencies
+    """
+    return len(parse_yarn_list())
+
+
 def pull_latest_version(package_name):
     """
     Attempts to pull latest version of package from yarn
     :param package_name: name of javascript package
     :returns: returns version as string, or UNKNOWN_VERSION if not found
     """
     string_output = Yarn.latest_version(package_name)
```

### Comparing `dependency-metrics-0.1.0/dependency_metrics/parsing_utils.py` & `dependency-metrics-0.1.1/dependency_metrics/parsing_utils.py`

 * *Files identical despite different names*

### Comparing `dependency-metrics-0.1.0/dependency_metrics.egg-info/PKG-INFO` & `dependency-metrics-0.1.1/dependency_metrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dependency-metrics
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python tool to track outdated dependencies.
 Author-email: Dimagi <dev@dimagi.com>
 Maintainer-email: Dimagi <dev@dimagi.com>
 License: Copyright (c) 2023, Dimagi Inc., and individual contributors.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -70,14 +70,15 @@
 
 #### --stats option
 
 Use the `--stats` option to generate a simple dictionary that displays the total number of outdated dependencies, as well as a breakdown detailing the number of outdated dependencies for each version type.
 
 ```commandline
 $ metrics pip --stats
+Total: 5
 Outdated: 2
 Multi-Major: 1
 Major: 0
 Minor: 1
 Patch: 0
 Unknown: 0
 ```
```

### Comparing `dependency-metrics-0.1.0/dependency_metrics.egg-info/SOURCES.txt` & `dependency-metrics-0.1.1/dependency_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dependency-metrics-0.1.0/pyproject.toml` & `dependency-metrics-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools"]
 
 [project]
 name = "dependency-metrics"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.md"
 description = "Python tool to track outdated dependencies."
 authors = [
     {name = "Dimagi", email = "dev@dimagi.com"},
 ]
 maintainers = [
     {name = "Dimagi", email = "dev@dimagi.com"}
```

### Comparing `dependency-metrics-0.1.0/tests/test_datadog_utils.py` & `dependency-metrics-0.1.1/tests/test_datadog_utils.py`

 * *Files identical despite different names*

### Comparing `dependency-metrics-0.1.0/tests/test_metrics.py` & `dependency-metrics-0.1.1/tests/test_metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from unittest import TestCase
 
-from dependency_metrics.metrics import build_packages_table, get_package_stats
+from dependency_metrics.metrics import (build_packages_table,
+                                        get_outdated_package_stats)
 
 
 class BuildPackagesTableTests(TestCase):
 
     def test_header_row(self):
         packages = []
         rows = build_packages_table(packages)
@@ -17,67 +18,67 @@
 
     def test_row_with_no_delta(self):
         packages = [([0, 0, 0], 'test', '1.0', '1.0')]
         rows = build_packages_table(packages)
         self.assertEqual(rows[1], "0.0.0    test                         1.0          1.0")
 
 
-class GetPackageStatsTests(TestCase):
+class GetOutdatedPackageStatsTests(TestCase):
 
     def test_outdated_multi_major_package(self):
         packages = [([2, 0, 0], 'test', '3.1', '1.0')]
-        stats = get_package_stats(packages)
+        stats = get_outdated_package_stats(packages)
         self.assertEqual(stats, {
             "Outdated": 1,
             "Multi-Major": 1,
             "Major": 0,
             "Minor": 0,
             "Patch": 0,
             "Unknown": 0,
         })
 
     def test_outdated_major_package(self):
         packages = [([1, 0, 0], 'test', '2.5', '1.0')]
-        stats = get_package_stats(packages)
+        stats = get_outdated_package_stats(packages)
         self.assertEqual(stats, {
             "Outdated": 1,
             "Multi-Major": 0,
             "Major": 1,
             "Minor": 0,
             "Patch": 0,
             "Unknown": 0,
         })
 
     def test_outdated_minor_package(self):
         packages = [([0, 5, 0], 'test', '2.5', '2.0')]
-        stats = get_package_stats(packages)
+        stats = get_outdated_package_stats(packages)
         self.assertEqual(stats, {
             "Outdated": 1,
             "Multi-Major": 0,
             "Major": 0,
             "Minor": 1,
             "Patch": 0,
             "Unknown": 0,
         })
 
     def test_outdated_patch_package(self):
         packages = [([0, 0, 3], 'test', '2.5.4', '2.5.1')]
-        stats = get_package_stats(packages)
+        stats = get_outdated_package_stats(packages)
         self.assertEqual(stats, {
             "Outdated": 1,
             "Multi-Major": 0,
             "Major": 0,
             "Minor": 0,
             "Patch": 1,
             "Unknown": 0,
         })
 
     def test_unknown_package(self):
         packages = [(None, 'test', 'unknown', '2.5.1')]
-        stats = get_package_stats(packages)
+        stats = get_outdated_package_stats(packages)
         self.assertEqual(stats, {
             "Outdated": 1,
             "Multi-Major": 0,
             "Major": 0,
             "Minor": 0,
             "Patch": 0,
             "Unknown": 1,
```

### Comparing `dependency-metrics-0.1.0/tests/test_parsing_utils.py` & `dependency-metrics-0.1.1/tests/test_parsing_utils.py`

 * *Files identical despite different names*

