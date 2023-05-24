# Comparing `tmp/os2ds-rules-0.0.7.tar.gz` & `tmp/os2ds-rules-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os2ds-rules-0.0.7.tar", last modified: Wed May 24 09:47:04 2023, max compression
+gzip compressed data, was "os2ds-rules-0.0.8.tar", last modified: Wed May 24 11:10:23 2023, max compression
```

## Comparing `os2ds-rules-0.0.7.tar` & `os2ds-rules-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:47:04.872522 os2ds-rules-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-24 09:46:55.000000 os2ds-rules-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-24 09:46:55.000000 os2ds-rules-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-05-24 09:47:04.872522 os2ds-rules-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-05-24 09:46:55.000000 os2ds-rules-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:47:04.872522 os2ds-rules-0.0.7/include/
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-24 09:46:55.000000 os2ds-rules-0.0.7/include/cpr-detector.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:47:04.872522 os2ds-rules-0.0.7/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-05-24 09:46:55.000000 os2ds-rules-0.0.7/lib/address_rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-05-24 09:46:55.000000 os2ds-rules-0.0.7/lib/cpr-detector.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-24 09:46:55.000000 os2ds-rules-0.0.7/lib/name_rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-24 09:46:55.000000 os2ds-rules-0.0.7/lib/wordlist_rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-24 09:46:55.000000 os2ds-rules-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 09:47:04.872522 os2ds-rules-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-24 09:46:55.000000 os2ds-rules-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:47:04.872522 os2ds-rules-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:47:04.872522 os2ds-rules-0.0.7/src/os2ds_rules/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-24 09:46:55.000000 os2ds-rules-0.0.7/src/os2ds_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-24 09:46:55.000000 os2ds-rules-0.0.7/src/os2ds_rules/address_rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-24 09:46:55.000000 os2ds-rules-0.0.7/src/os2ds_rules/cpr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-24 09:46:55.000000 os2ds-rules-0.0.7/src/os2ds_rules/name_rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-05-24 09:46:55.000000 os2ds-rules-0.0.7/src/os2ds_rules/wordlist_rule.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:47:04.872522 os2ds-rules-0.0.7/src/os2ds_rules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-05-24 09:47:04.000000 os2ds-rules-0.0.7/src/os2ds_rules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-24 09:47:04.000000 os2ds-rules-0.0.7/src/os2ds_rules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:47:04.000000 os2ds-rules-0.0.7/src/os2ds_rules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 09:47:04.000000 os2ds-rules-0.0.7/src/os2ds_rules.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:10:23.614684 os2ds-rules-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-05-24 11:10:23.614684 os2ds-rules-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:10:23.610684 os2ds-rules-0.0.8/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/include/cpr-detector.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:10:23.610684 os2ds-rules-0.0.8/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/lib/address_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/lib/cpr-detector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/lib/name_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/lib/wordlist_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 11:10:23.614684 os2ds-rules-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:10:23.610684 os2ds-rules-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:10:23.610684 os2ds-rules-0.0.8/src/os2ds_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/src/os2ds_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/src/os2ds_rules/address_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/src/os2ds_rules/cpr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/src/os2ds_rules/name_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/src/os2ds_rules/wordlist_rule.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:10:23.614684 os2ds-rules-0.0.8/src/os2ds_rules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-05-24 11:10:23.000000 os2ds-rules-0.0.8/src/os2ds_rules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-24 11:10:23.000000 os2ds-rules-0.0.8/src/os2ds_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 11:10:23.000000 os2ds-rules-0.0.8/src/os2ds_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 11:10:23.000000 os2ds-rules-0.0.8/src/os2ds_rules.egg-info/top_level.txt
```

### Comparing `os2ds-rules-0.0.7/LICENSE` & `os2ds-rules-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.7/PKG-INFO` & `os2ds-rules-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os2ds-rules
-Version: 0.0.7
+Version: 0.0.8
 Summary: Text processing tool for detecting Danish CPR-numbers.
 Author-email: HackTheOxidation <tomas.hagenau@protonmail.ch>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

### Comparing `os2ds-rules-0.0.7/README.md` & `os2ds-rules-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.7/include/cpr-detector.hpp` & `os2ds-rules-0.0.8/include/cpr-detector.hpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.7/lib/address_rule.cpp` & `os2ds-rules-0.0.8/lib/address_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.7/lib/cpr-detector.cpp` & `os2ds-rules-0.0.8/lib/cpr-detector.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #include <algorithm>
 #include <array>
 #include <cstddef>
+#include <cctype>
 #include <iterator>
 #include <numeric>
 #include <string_view>
 
 #include <cpr-detector.hpp>
 #include <data_structures.hpp>
 
@@ -31,14 +32,16 @@
       auto begin = indices[j];
       auto end = indices[i] - begin;
 
       if (end > content.size())
 	end = content.size() - begin - 1;
 
       std::string target = content.substr(begin, end);
+      std::transform(target.begin(), target.end(), target.begin(),
+                     [](unsigned char c) { return std::tolower(c); });
 
       if (blacklist_words_set.contains(target))
 	return true;
     }
   }
 
   return false;
```

### Comparing `os2ds-rules-0.0.7/lib/name_rule.cpp` & `os2ds-rules-0.0.8/lib/name_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.7/lib/wordlist_rule.cpp` & `os2ds-rules-0.0.8/lib/wordlist_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.7/pyproject.toml` & `os2ds-rules-0.0.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "os2ds-rules"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="HackTheOxidation", email="tomas.hagenau@protonmail.ch" },
 ]
 description = "Text processing tool for detecting Danish CPR-numbers."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `os2ds-rules-0.0.7/setup.py` & `os2ds-rules-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.7/src/os2ds_rules/__init__.py` & `os2ds-rules-0.0.8/src/os2ds_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.7/src/os2ds_rules/address_rule.cpp` & `os2ds-rules-0.0.8/src/os2ds_rules/address_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.7/src/os2ds_rules/cpr.cpp` & `os2ds-rules-0.0.8/src/os2ds_rules/cpr.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.7/src/os2ds_rules/name_rule.cpp` & `os2ds-rules-0.0.8/src/os2ds_rules/name_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.7/src/os2ds_rules/wordlist_rule.cpp` & `os2ds-rules-0.0.8/src/os2ds_rules/wordlist_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.7/src/os2ds_rules.egg-info/PKG-INFO` & `os2ds-rules-0.0.8/src/os2ds_rules.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os2ds-rules
-Version: 0.0.7
+Version: 0.0.8
 Summary: Text processing tool for detecting Danish CPR-numbers.
 Author-email: HackTheOxidation <tomas.hagenau@protonmail.ch>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

