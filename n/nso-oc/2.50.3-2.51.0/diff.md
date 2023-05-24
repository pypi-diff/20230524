# Comparing `tmp/nso-oc-2.50.3.tar.gz` & `tmp/nso-oc-2.51.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nso-oc-2.50.3.tar", last modified: Thu May 18 18:55:46 2023, max compression
+gzip compressed data, was "nso-oc-2.51.0.tar", last modified: Wed May 24 13:45:16 2023, max compression
```

## Comparing `nso-oc-2.50.3.tar` & `nso-oc-2.51.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:55:46.296969 nso-oc-2.50.3/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-18 18:55:09.000000 nso-oc-2.50.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-18 18:55:09.000000 nso-oc-2.50.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-18 18:55:46.296969 nso-oc-2.50.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-18 18:55:09.000000 nso-oc-2.50.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:55:46.288969 nso-oc-2.50.3/nso_oc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-18 18:55:46.000000 nso-oc-2.50.3/nso_oc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-18 18:55:46.000000 nso-oc-2.50.3/nso_oc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:55:46.000000 nso-oc-2.50.3/nso_oc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-18 18:55:46.000000 nso-oc-2.50.3/nso_oc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 18:55:46.000000 nso-oc-2.50.3/nso_oc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-18 18:55:46.000000 nso-oc-2.50.3/nso_oc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:55:46.292969 nso-oc-2.50.3/package_nso_to_oc/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-18 18:55:09.000000 nso-oc-2.50.3/package_nso_to_oc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-18 18:55:09.000000 nso-oc-2.50.3/package_nso_to_oc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-18 18:55:09.000000 nso-oc-2.50.3/package_nso_to_oc/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-05-18 18:55:09.000000 nso-oc-2.50.3/package_nso_to_oc/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:55:46.292969 nso-oc-2.50.3/package_nso_to_oc/xe/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-18 18:55:09.000000 nso-oc-2.50.3/package_nso_to_oc/xe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-05-18 18:55:09.000000 nso-oc-2.50.3/package_nso_to_oc/xe/common_xe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-18 18:55:09.000000 nso-oc-2.50.3/package_nso_to_oc/xe/main_xe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30058 2023-05-18 18:55:09.000000 nso-oc-2.50.3/package_nso_to_oc/xe/xe_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-05-18 18:55:09.000000 nso-oc-2.50.3/package_nso_to_oc/xe/xe_bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    63537 2023-05-18 18:55:09.000000 nso-oc-2.50.3/package_nso_to_oc/xe/xe_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    42084 2023-05-18 18:55:09.000000 nso-oc-2.50.3/package_nso_to_oc/xe/xe_network_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    39884 2023-05-18 18:55:09.000000 nso-oc-2.50.3/package_nso_to_oc/xe/xe_ospfv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-05-18 18:55:09.000000 nso-oc-2.50.3/package_nso_to_oc/xe/xe_routing_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-05-18 18:55:09.000000 nso-oc-2.50.3/package_nso_to_oc/xe/xe_static_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-05-18 18:55:09.000000 nso-oc-2.50.3/package_nso_to_oc/xe/xe_stp.py
--rw-r--r--   0 runner    (1001) docker     (123)    93881 2023-05-18 18:55:09.000000 nso-oc-2.50.3/package_nso_to_oc/xe/xe_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-18 18:55:09.000000 nso-oc-2.50.3/package_nso_to_oc/xe/xe_vlans.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:55:46.296969 nso-oc-2.50.3/package_nso_to_oc/xr/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-18 18:55:09.000000 nso-oc-2.50.3/package_nso_to_oc/xr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-18 18:55:09.000000 nso-oc-2.50.3/package_nso_to_oc/xr/common_xr.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-18 18:55:09.000000 nso-oc-2.50.3/package_nso_to_oc/xr/main_xr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-05-18 18:55:09.000000 nso-oc-2.50.3/package_nso_to_oc/xr/xr_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-05-18 18:55:09.000000 nso-oc-2.50.3/package_nso_to_oc/xr/xr_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-18 18:55:09.000000 nso-oc-2.50.3/package_nso_to_oc/xr/xr_system.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-18 18:55:09.000000 nso-oc-2.50.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-18 18:55:46.296969 nso-oc-2.50.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-18 18:55:09.000000 nso-oc-2.50.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:45:16.520041 nso-oc-2.51.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-24 13:44:48.000000 nso-oc-2.51.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-24 13:44:48.000000 nso-oc-2.51.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-24 13:45:16.520041 nso-oc-2.51.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-24 13:44:48.000000 nso-oc-2.51.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:45:16.516041 nso-oc-2.51.0/nso_oc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-24 13:45:16.000000 nso-oc-2.51.0/nso_oc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-24 13:45:16.000000 nso-oc-2.51.0/nso_oc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:45:16.000000 nso-oc-2.51.0/nso_oc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-24 13:45:16.000000 nso-oc-2.51.0/nso_oc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 13:45:16.000000 nso-oc-2.51.0/nso_oc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 13:45:16.000000 nso-oc-2.51.0/nso_oc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:45:16.516041 nso-oc-2.51.0/package_nso_to_oc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-24 13:44:48.000000 nso-oc-2.51.0/package_nso_to_oc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 13:44:48.000000 nso-oc-2.51.0/package_nso_to_oc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-24 13:44:48.000000 nso-oc-2.51.0/package_nso_to_oc/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-05-24 13:44:48.000000 nso-oc-2.51.0/package_nso_to_oc/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:45:16.520041 nso-oc-2.51.0/package_nso_to_oc/xe/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-24 13:44:48.000000 nso-oc-2.51.0/package_nso_to_oc/xe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-05-24 13:44:48.000000 nso-oc-2.51.0/package_nso_to_oc/xe/common_xe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-24 13:44:48.000000 nso-oc-2.51.0/package_nso_to_oc/xe/main_xe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30058 2023-05-24 13:44:48.000000 nso-oc-2.51.0/package_nso_to_oc/xe/xe_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-05-24 13:44:48.000000 nso-oc-2.51.0/package_nso_to_oc/xe/xe_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63537 2023-05-24 13:44:48.000000 nso-oc-2.51.0/package_nso_to_oc/xe/xe_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42084 2023-05-24 13:44:48.000000 nso-oc-2.51.0/package_nso_to_oc/xe/xe_network_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39884 2023-05-24 13:44:48.000000 nso-oc-2.51.0/package_nso_to_oc/xe/xe_ospfv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-05-24 13:44:48.000000 nso-oc-2.51.0/package_nso_to_oc/xe/xe_routing_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-05-24 13:44:48.000000 nso-oc-2.51.0/package_nso_to_oc/xe/xe_static_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-05-24 13:44:48.000000 nso-oc-2.51.0/package_nso_to_oc/xe/xe_stp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104722 2023-05-24 13:44:48.000000 nso-oc-2.51.0/package_nso_to_oc/xe/xe_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-24 13:44:48.000000 nso-oc-2.51.0/package_nso_to_oc/xe/xe_vlans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:45:16.520041 nso-oc-2.51.0/package_nso_to_oc/xr/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-24 13:44:48.000000 nso-oc-2.51.0/package_nso_to_oc/xr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-24 13:44:48.000000 nso-oc-2.51.0/package_nso_to_oc/xr/common_xr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-24 13:44:48.000000 nso-oc-2.51.0/package_nso_to_oc/xr/main_xr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-05-24 13:44:48.000000 nso-oc-2.51.0/package_nso_to_oc/xr/xr_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-05-24 13:44:48.000000 nso-oc-2.51.0/package_nso_to_oc/xr/xr_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-24 13:44:48.000000 nso-oc-2.51.0/package_nso_to_oc/xr/xr_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-24 13:44:48.000000 nso-oc-2.51.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-24 13:45:16.520041 nso-oc-2.51.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-24 13:44:48.000000 nso-oc-2.51.0/setup.py
```

### Comparing `nso-oc-2.50.3/LICENSE` & `nso-oc-2.51.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.3/PKG-INFO` & `nso-oc-2.51.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.50.3
+Version: 2.51.0
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.50.3/README.md` & `nso-oc-2.51.0/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.3/nso_oc.egg-info/PKG-INFO` & `nso-oc-2.51.0/nso_oc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.50.3
+Version: 2.51.0
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.50.3/nso_oc.egg-info/SOURCES.txt` & `nso-oc-2.51.0/nso_oc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.3/package_nso_to_oc/README.md` & `nso-oc-2.51.0/package_nso_to_oc/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.3/package_nso_to_oc/common.py` & `nso-oc-2.51.0/package_nso_to_oc/common.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.3/package_nso_to_oc/main.py` & `nso-oc-2.51.0/package_nso_to_oc/main.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.3/package_nso_to_oc/xe/common_xe.py` & `nso-oc-2.51.0/package_nso_to_oc/xe/common_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.3/package_nso_to_oc/xe/main_xe.py` & `nso-oc-2.51.0/package_nso_to_oc/xe/main_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.3/package_nso_to_oc/xe/xe_acls.py` & `nso-oc-2.51.0/package_nso_to_oc/xe/xe_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.3/package_nso_to_oc/xe/xe_bgp.py` & `nso-oc-2.51.0/package_nso_to_oc/xe/xe_bgp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.3/package_nso_to_oc/xe/xe_interfaces.py` & `nso-oc-2.51.0/package_nso_to_oc/xe/xe_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.3/package_nso_to_oc/xe/xe_network_instances.py` & `nso-oc-2.51.0/package_nso_to_oc/xe/xe_network_instances.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.3/package_nso_to_oc/xe/xe_ospfv2.py` & `nso-oc-2.51.0/package_nso_to_oc/xe/xe_ospfv2.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.3/package_nso_to_oc/xe/xe_routing_policy.py` & `nso-oc-2.51.0/package_nso_to_oc/xe/xe_routing_policy.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.3/package_nso_to_oc/xe/xe_static_route.py` & `nso-oc-2.51.0/package_nso_to_oc/xe/xe_static_route.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.3/package_nso_to_oc/xe/xe_stp.py` & `nso-oc-2.51.0/package_nso_to_oc/xe/xe_stp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.3/package_nso_to_oc/xe/xe_system.py` & `nso-oc-2.51.0/package_nso_to_oc/xe/xe_system.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,14 +70,17 @@
                 "openconfig-system-ext:config": {},
                 "openconfig-system-ext:block-for": {"openconfig-system-ext:config": {}}
             },
             "openconfig-system-ext:object-tracking": {
                 "openconfig-system-ext:config": {"openconfig-system-ext:timer": {}},
                 "openconfig-system-ext:object-track": []
             },
+            "openconfig-system-ext:key-chains": {
+                "openconfig-system-ext:key-chain": []
+            },
             "openconfig-system-ext:boot-network": {
                 "openconfig-system-ext:config": {},
             },
             "openconfig-system-ext:nat": {
                 "openconfig-system-ext:pools": {"openconfig-system-ext:pool": []},
                 "openconfig-system-ext:inside": {"openconfig-system-ext:source": {}
                 }
@@ -129,14 +132,17 @@
         del config_leftover["tailf-ned-cisco-ios:login"]["block-for"]["within"]
     # track-object
     if config_before.get("tailf-ned-cisco-ios:track", {}).get("timer", {}).get("interface", {}).get("seconds"):
         openconfig_system_services["openconfig-system-ext:object-tracking"]["openconfig-system-ext:config"]["openconfig-system-ext:timer"]["openconfig-system-ext:interface-timer"] = config_before.get("tailf-ned-cisco-ios:track", {}).get("timer", {}).get("interface", {}).get("seconds")
         del config_leftover["tailf-ned-cisco-ios:track"]["timer"]
     if type(config_before.get("tailf-ned-cisco-ios:track", {}).get("track-object", '')) is list:
         xe_system_object_track(config_before, config_leftover)
+    # key-chains
+    if type(config_before.get("tailf-ned-cisco-ios:key", {}).get("chain", '')) is list or type(config_before.get("tailf-ned-cisco-ios:key", {}).get("tcp", {}).get("chain", '')) is list:
+        xe_system_key_chain(config_before, config_leftover)
     # Archive Logging
     if type(config_before.get("tailf-ned-cisco-ios:archive", {}).get("log", {}).get("config", {}).get("logging", {}).get("enable", '')) is list:
         openconfig_system_services["openconfig-system-ext:config"]["openconfig-system-ext:archive-logging"] = True
         del config_leftover["tailf-ned-cisco-ios:archive"]["log"]["config"]["logging"]["enable"]
     else:
         openconfig_system_services["openconfig-system-ext:config"]["openconfig-system-ext:archive-logging"] = False
     # boot network
@@ -343,14 +349,186 @@
             else:
                 print("Invalid track_object data structure")
         openconfig_system["openconfig-system:system"]["openconfig-system-ext:services"]["openconfig-system-ext:object-tracking"]["openconfig-system-ext:object-track"].append(tmp_track_object)
     if config_leftover["tailf-ned-cisco-ios:track"]["track-object"]:
         del config_leftover["tailf-ned-cisco-ios:track"]["track-object"]
 
 
+def xe_system_key_chain(config_before: dict, config_leftover: dict) -> None:
+    """
+    Translates NSO XE NED to MDD OpenConfig System Key Chain
+    """
+    key_chain = {
+        "openconfig-system-ext:name": "",
+        "openconfig-system-ext:type": "",
+        "openconfig-system-ext:keys": []
+    }
+    key = {
+        "openconfig-system-ext:id": None,
+        "openconfig-system-ext:config": {
+            "openconfig-system-ext:id": None,
+            "openconfig-system-ext:key-string": "",
+            "openconfig-system-ext:cryptographic-algorithm": "",
+            "openconfig-system-ext:accept-lifetime": {},
+            "openconfig-system-ext:send-lifetime": {},
+        }
+    }
+    key_tcp = {
+        "openconfig-system-ext:id": None,
+        "openconfig-system-ext:config": {
+            "openconfig-system-ext:id": None,
+            "openconfig-system-ext:key-string": "",
+            "openconfig-system-ext:cryptographic-algorithm-tcp": "",
+            "openconfig-system-ext:send-id": None,
+            "openconfig-system-ext:recv-id": None,
+            "openconfig-system-ext:accept-lifetime": {},
+            "openconfig-system-ext:send-lifetime": {},
+        }
+    }
+    # NA key chain
+    for key_chain_index, key_chain_list in enumerate(config_before.get("tailf-ned-cisco-ios:key", {}).get("chain", '')):
+        tmp_key_chain = copy.deepcopy(key_chain)
+        tmp_key_chain["openconfig-system-ext:type"] = "NOT_APPLICABLE"
+        for k, v in key_chain_list.items():
+            if "name" in k:
+                tmp_key_chain["openconfig-system-ext:name"] = v
+            elif "key" in k:
+                for keydata in v:
+                    tmp_key = copy.deepcopy(key)
+                    accept_lifetime_global = True
+                    send_lifetime_global = True
+                    for keydata_k, keydata_v in keydata.items():
+                        if keydata_k == "id":
+                            tmp_key["openconfig-system-ext:id"] = keydata_v
+                            tmp_key["openconfig-system-ext:config"]["openconfig-system-ext:id"] = keydata_v
+                        elif keydata_k == "cryptographic-algorithm":
+                            tmp_key["openconfig-system-ext:config"]["openconfig-system-ext:cryptographic-algorithm"] = str(keydata_v)
+                        elif keydata_k == "key-string":
+                            for ks_k, ks_v in keydata_v.items():
+                                if "type" in ks_k:
+                                    keystring_type = ks_v
+                                elif "secret" in ks_k:
+                                    tmp_key["openconfig-system-ext:config"]["openconfig-system-ext:key-string"] = str(ks_v)
+                        elif keydata_k == "accept-lifetime":
+                            for al_k, al_v in keydata_v.items():
+                                if "local" in al_k:
+                                    accept_lifetime_global = False
+                                    tmp_lt = xe_parse_keychain_lifetime(al_v)
+                                    tmp_key["openconfig-system-ext:config"]["openconfig-system-ext:accept-lifetime"].update({"openconfig-system-ext:local": {}})
+                                    tmp_key["openconfig-system-ext:config"]["openconfig-system-ext:accept-lifetime"]["openconfig-system-ext:local"] = tmp_lt
+                            if accept_lifetime_global == True:
+                                tmp_lt = xe_parse_keychain_lifetime(keydata_v)
+                                tmp_key["openconfig-system-ext:config"]["openconfig-system-ext:accept-lifetime"] = tmp_lt
+                        elif keydata_k == "send-lifetime":
+                            for sl_k, sl_v in keydata_v.items():
+                                if "local" in sl_k:
+                                    send_lifetime_global = False
+                                    tmp_lt = xe_parse_keychain_lifetime(sl_v)
+                                    tmp_key["openconfig-system-ext:config"]["openconfig-system-ext:send-lifetime"].update({"openconfig-system-ext:local": {}})
+                                    tmp_key["openconfig-system-ext:config"]["openconfig-system-ext:send-lifetime"]["openconfig-system-ext:local"] = tmp_lt
+                            if send_lifetime_global == True:
+                                tmp_lt = xe_parse_keychain_lifetime(keydata_v)
+                                tmp_key["openconfig-system-ext:config"]["openconfig-system-ext:send-lifetime"] = tmp_lt
+                    tmp_key_chain["openconfig-system-ext:keys"].append(tmp_key)
+
+        openconfig_system["openconfig-system:system"]["openconfig-system-ext:services"]["openconfig-system-ext:key-chains"]["openconfig-system-ext:key-chain"].append(tmp_key_chain)
+    if config_leftover.get("tailf-ned-cisco-ios:key", {}).get("chain"):
+        del config_leftover["tailf-ned-cisco-ios:key"]["chain"]
+
+    # TCP key chain
+    for key_chain_index, key_chain_list in enumerate(config_before.get("tailf-ned-cisco-ios:key", {}).get("tcp", {}).get("chain", '')):
+        tmp_key_chain = copy.deepcopy(key_chain)
+        tmp_key_chain["openconfig-system-ext:type"] = "TCP"
+        for k, v in key_chain_list.items():
+            if "name" in k:
+                tmp_key_chain["openconfig-system-ext:name"] = v
+            elif "key" in k:
+                for keydata in v:
+                    tmp_key_tcp = copy.deepcopy(key_tcp)
+                    accept_lifetime_global = True
+                    send_lifetime_global = True
+                    for keydata_k, keydata_v in keydata.items():
+                        if keydata_k == "id":
+                            tmp_key_tcp["openconfig-system-ext:id"] = keydata_v
+                            tmp_key_tcp["openconfig-system-ext:config"]["openconfig-system-ext:id"] = keydata_v
+                        elif keydata_k == "send-id":
+                            tmp_key_tcp["openconfig-system-ext:config"]["openconfig-system-ext:send-id"] = keydata_v
+                        elif keydata_k == "recv-id":
+                            tmp_key_tcp["openconfig-system-ext:config"]["openconfig-system-ext:recv-id"] = keydata_v
+                        elif "cryptographic-algorithm" in keydata_k:
+                            tmp_key_tcp["openconfig-system-ext:config"]["openconfig-system-ext:cryptographic-algorithm-tcp"] = str(keydata_v)
+                        elif keydata_k == "key-string":
+                            for ks_k, ks_v in keydata_v.items():
+                                if "type" in ks_k:
+                                    keystring_type = ks_v
+                                elif "secret" in ks_k:
+                                    tmp_key_tcp["openconfig-system-ext:config"]["openconfig-system-ext:key-string"] = str(ks_v)
+                        elif keydata_k == "accept-lifetime":
+                            for al_k, al_v in keydata_v.items():
+                                if "local" in al_k:
+                                    accept_lifetime_global = False
+                                    tmp_lt = xe_parse_keychain_lifetime(al_v)
+                                    tmp_key_tcp["openconfig-system-ext:config"]["openconfig-system-ext:accept-lifetime"].update({"openconfig-system-ext:local": {}})
+                                    tmp_key_tcp["openconfig-system-ext:config"]["openconfig-system-ext:accept-lifetime"]["openconfig-system-ext:local"] = tmp_lt
+                            if accept_lifetime_global == True:
+                                tmp_lt = xe_parse_keychain_lifetime(keydata_v)
+                                tmp_key_tcp["openconfig-system-ext:config"]["openconfig-system-ext:accept-lifetime"] = tmp_lt
+                        elif keydata_k == "send-lifetime":
+                            for sl_k, sl_v in keydata_v.items():
+                                if "local" in sl_k:
+                                    send_lifetime_global = False
+                                    tmp_lt = xe_parse_keychain_lifetime(sl_v)
+                                    tmp_key_tcp["openconfig-system-ext:config"]["openconfig-system-ext:send-lifetime"].update({"openconfig-system-ext:local": {}})
+                                    tmp_key_tcp["openconfig-system-ext:config"]["openconfig-system-ext:send-lifetime"]["openconfig-system-ext:local"] = tmp_lt
+                            if send_lifetime_global == True:
+                                tmp_lt = xe_parse_keychain_lifetime(keydata_v)
+                                tmp_key_tcp["openconfig-system-ext:config"]["openconfig-system-ext:send-lifetime"] = tmp_lt
+                    tmp_key_chain["openconfig-system-ext:keys"].append(tmp_key_tcp)
+
+        openconfig_system["openconfig-system:system"]["openconfig-system-ext:services"]["openconfig-system-ext:key-chains"]["openconfig-system-ext:key-chain"].append(tmp_key_chain)
+    if config_leftover.get("tailf-ned-cisco-ios:key", {}).get("tcp"):
+        del config_leftover["tailf-ned-cisco-ios:key"]["tcp"]
+
+def xe_parse_keychain_lifetime(lifetime_dict: dict):
+    """
+    Parse the keychain lifetime dataset.
+    Returns: lifetime dict
+    """
+    lifetime = {
+        "openconfig-system-ext:start-time": "",
+        "openconfig-system-ext:start-date": None,
+        "openconfig-system-ext:start-month": "",
+        "openconfig-system-ext:start-year": None
+    }
+
+    tmp_lifetime = copy.deepcopy(lifetime)
+    for k, v in lifetime_dict.items():
+        if "start-time" in k:
+            tmp_lifetime["openconfig-system-ext:start-time"] = str(v)
+        elif "start-date" in k:
+            tmp_lifetime["openconfig-system-ext:start-date"] = v
+        elif "start-month" in k:
+            tmp_lifetime["openconfig-system-ext:start-month"] = str(v)
+        elif "start-year" in k:
+            tmp_lifetime["openconfig-system-ext:start-year"] = v
+        elif "infinite" in k:
+            tmp_lifetime["openconfig-system-ext:infinite"] = True
+        elif "duration" in k:
+            tmp_lifetime["openconfig-system-ext:duration"] = v
+        elif "stop-time" in k:
+            tmp_lifetime["openconfig-system-ext:stop-time"] = str(v)
+        elif "stop-date" in k:
+            tmp_lifetime["openconfig-system-ext:stop-date"] = str(v)
+        elif "stop-month" in k:
+            tmp_lifetime["openconfig-system-ext:stop-month"] = str(v)
+        elif "stop-year" in k:
+            tmp_lifetime["openconfig-system-ext:stop-year"] = str(v)
+    return(tmp_lifetime)
+
+
 def xe_system_ssh_server(config_before: dict, config_leftover: dict) -> None:
     """
     Translates NSO XE NED to MDD OpenConfig System SSH Server
     """
     openconfig_system_ssh_server_config = openconfig_system["openconfig-system:system"]["openconfig-system:ssh-server"]["openconfig-system:config"]
     openconfig_system_ssh_server_alg_config = openconfig_system["openconfig-system:system"]["openconfig-system:ssh-server"]["openconfig-system-ext:algorithm"]["openconfig-system-ext:config"]
```

### Comparing `nso-oc-2.50.3/package_nso_to_oc/xe/xe_vlans.py` & `nso-oc-2.51.0/package_nso_to_oc/xe/xe_vlans.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.3/package_nso_to_oc/xr/common_xr.py` & `nso-oc-2.51.0/package_nso_to_oc/xr/common_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.3/package_nso_to_oc/xr/main_xr.py` & `nso-oc-2.51.0/package_nso_to_oc/xr/main_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.3/package_nso_to_oc/xr/xr_acls.py` & `nso-oc-2.51.0/package_nso_to_oc/xr/xr_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.3/package_nso_to_oc/xr/xr_interfaces.py` & `nso-oc-2.51.0/package_nso_to_oc/xr/xr_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.3/package_nso_to_oc/xr/xr_system.py` & `nso-oc-2.51.0/package_nso_to_oc/xr/xr_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.3/setup.py` & `nso-oc-2.51.0/setup.py`

 * *Files identical despite different names*

