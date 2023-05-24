# Comparing `tmp/pxgrid-api-0.2.3.tar.gz` & `tmp/pxgrid-api-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pxgrid-api-0.2.3.tar", last modified: Tue May 16 03:55:36 2023, max compression
+gzip compressed data, was "pxgrid-api-0.2.4.tar", last modified: Wed May 24 16:12:44 2023, max compression
```

## Comparing `pxgrid-api-0.2.3.tar` & `pxgrid-api-0.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-16 03:55:36.390559 pxgrid-api-0.2.3/
--rw-r--r--   0 vibobrov   (503) staff       (20)    11357 2023-05-10 01:50:25.000000 pxgrid-api-0.2.3/LICENSE
--rw-r--r--   0 vibobrov   (503) staff       (20)       24 2023-05-13 01:43:48.000000 pxgrid-api-0.2.3/MANIFEST.in
--rw-r--r--   0 vibobrov   (503) staff       (20)    29667 2023-05-16 03:55:36.390104 pxgrid-api-0.2.3/PKG-INFO
--rw-r--r--   0 vibobrov   (503) staff       (20)    16165 2023-05-16 03:25:57.000000 pxgrid-api-0.2.3/README.rst
--rw-r--r--   0 vibobrov   (503) staff       (20)      766 2023-05-16 03:54:47.000000 pxgrid-api-0.2.3/pyproject.toml
--rw-r--r--   0 vibobrov   (503) staff       (20)       38 2023-05-16 03:55:36.390679 pxgrid-api-0.2.3/setup.cfg
-drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-16 03:55:36.379358 pxgrid-api-0.2.3/src/
-drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-16 03:55:36.384460 pxgrid-api-0.2.3/src/pxapi/
--rw-r--r--   0 vibobrov   (503) staff       (20)       82 2023-05-16 03:54:52.000000 pxgrid-api-0.2.3/src/pxapi/__init__.py
--rwxr-xr-x   0 vibobrov   (503) staff       (20)    20351 2023-05-16 03:54:31.000000 pxgrid-api-0.2.3/src/pxapi/__main__.py
--rw-r--r--   0 vibobrov   (503) staff       (20)    29194 2023-05-16 03:48:27.000000 pxgrid-api-0.2.3/src/pxapi/pxapi.py
--rw-r--r--   0 vibobrov   (503) staff       (20)     1488 2023-05-16 03:15:00.000000 pxgrid-api-0.2.3/src/pxapi/stompframe.py
-drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-16 03:55:36.389059 pxgrid-api-0.2.3/src/pxgrid_api.egg-info/
--rw-r--r--   0 vibobrov   (503) staff       (20)    29667 2023-05-16 03:55:36.000000 pxgrid-api-0.2.3/src/pxgrid_api.egg-info/PKG-INFO
--rw-r--r--   0 vibobrov   (503) staff       (20)      362 2023-05-16 03:55:36.000000 pxgrid-api-0.2.3/src/pxgrid_api.egg-info/SOURCES.txt
--rw-r--r--   0 vibobrov   (503) staff       (20)        1 2023-05-16 03:55:36.000000 pxgrid-api-0.2.3/src/pxgrid_api.egg-info/dependency_links.txt
--rw-r--r--   0 vibobrov   (503) staff       (20)       48 2023-05-16 03:55:36.000000 pxgrid-api-0.2.3/src/pxgrid_api.egg-info/entry_points.txt
--rw-r--r--   0 vibobrov   (503) staff       (20)       42 2023-05-16 03:55:36.000000 pxgrid-api-0.2.3/src/pxgrid_api.egg-info/requires.txt
--rw-r--r--   0 vibobrov   (503) staff       (20)       14 2023-05-16 03:55:36.000000 pxgrid-api-0.2.3/src/pxgrid_api.egg-info/top_level.txt
+drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-24 16:12:44.636604 pxgrid-api-0.2.4/
+-rw-r--r--   0 vibobrov   (503) staff       (20)    11357 2023-05-10 01:50:25.000000 pxgrid-api-0.2.4/LICENSE
+-rw-r--r--   0 vibobrov   (503) staff       (20)       24 2023-05-13 01:43:48.000000 pxgrid-api-0.2.4/MANIFEST.in
+-rw-r--r--   0 vibobrov   (503) staff       (20)    29738 2023-05-24 16:12:44.636133 pxgrid-api-0.2.4/PKG-INFO
+-rw-r--r--   0 vibobrov   (503) staff       (20)    16236 2023-05-19 19:04:16.000000 pxgrid-api-0.2.4/README.rst
+-rw-r--r--   0 vibobrov   (503) staff       (20)      766 2023-05-24 16:12:35.000000 pxgrid-api-0.2.4/pyproject.toml
+-rw-r--r--   0 vibobrov   (503) staff       (20)       38 2023-05-24 16:12:44.636758 pxgrid-api-0.2.4/setup.cfg
+drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-24 16:12:44.623376 pxgrid-api-0.2.4/src/
+drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-24 16:12:44.631039 pxgrid-api-0.2.4/src/pxapi/
+-rw-r--r--   0 vibobrov   (503) staff       (20)      149 2023-05-24 16:10:42.000000 pxgrid-api-0.2.4/src/pxapi/__init__.py
+-rwxr-xr-x   0 vibobrov   (503) staff       (20)    20351 2023-05-16 03:54:31.000000 pxgrid-api-0.2.4/src/pxapi/__main__.py
+-rw-r--r--   0 vibobrov   (503) staff       (20)    29250 2023-05-24 16:09:22.000000 pxgrid-api-0.2.4/src/pxapi/pxapi.py
+-rw-r--r--   0 vibobrov   (503) staff       (20)     1555 2023-05-16 13:17:07.000000 pxgrid-api-0.2.4/src/pxapi/stompframe.py
+drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-24 16:12:44.635150 pxgrid-api-0.2.4/src/pxgrid_api.egg-info/
+-rw-r--r--   0 vibobrov   (503) staff       (20)    29738 2023-05-24 16:12:44.000000 pxgrid-api-0.2.4/src/pxgrid_api.egg-info/PKG-INFO
+-rw-r--r--   0 vibobrov   (503) staff       (20)      362 2023-05-24 16:12:44.000000 pxgrid-api-0.2.4/src/pxgrid_api.egg-info/SOURCES.txt
+-rw-r--r--   0 vibobrov   (503) staff       (20)        1 2023-05-24 16:12:44.000000 pxgrid-api-0.2.4/src/pxgrid_api.egg-info/dependency_links.txt
+-rw-r--r--   0 vibobrov   (503) staff       (20)       48 2023-05-24 16:12:44.000000 pxgrid-api-0.2.4/src/pxgrid_api.egg-info/entry_points.txt
+-rw-r--r--   0 vibobrov   (503) staff       (20)       42 2023-05-24 16:12:44.000000 pxgrid-api-0.2.4/src/pxgrid_api.egg-info/requires.txt
+-rw-r--r--   0 vibobrov   (503) staff       (20)       14 2023-05-24 16:12:44.000000 pxgrid-api-0.2.4/src/pxgrid_api.egg-info/top_level.txt
```

### Comparing `pxgrid-api-0.2.3/LICENSE` & `pxgrid-api-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pxgrid-api-0.2.3/PKG-INFO` & `pxgrid-api-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pxgrid-api
-Version: 0.2.3
+Version: 0.2.4
 Summary: pxGrid API library and command line tool
 Author-email: Viktor Bobrov <vibobrov@cisco.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -221,14 +221,16 @@
 
 This repo includes two components:
 - A python API library making it easier to interact with pxGrid services on ISE
 - Interactive CLI utility to interface with pxGrid without writing any code
 
 pxGrid requires FQDNs of all the nodes to be resolvable. It is not possible to use the library or the CLI utility to connect to ISE via IP address, even if there's just one node. Hosts record will work as well.
 
+Full API documention is available at https://pxgrid-api.readthedocs.io/
+
 Features
 --------
 
 - Support for both certificate and password authentication when connecting to pxGrid nodes
 - Commands and methods to interact with most pxGrid services
 - Websocket support for subscribing to topics.
 - Debug capabilities to show all low level interactions with pxGrid
@@ -371,15 +373,15 @@
 
   # Install the module
   pip install pxgrid-api
 
 Usage
 -----
 
-All commands are document and help can be retrived using help &lt;command&gt;
+All commands are document and help can be retrived using **help <command>**
 
 .. code-block:: console
 
   $ pxshell
   pxshell> help
 
   Documented commands (type help <topic>):
```

### Comparing `pxgrid-api-0.2.3/README.rst` & `pxgrid-api-0.2.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 This repo includes two components:
 - A python API library making it easier to interact with pxGrid services on ISE
 - Interactive CLI utility to interface with pxGrid without writing any code
 
 pxGrid requires FQDNs of all the nodes to be resolvable. It is not possible to use the library or the CLI utility to connect to ISE via IP address, even if there's just one node. Hosts record will work as well.
 
+Full API documention is available at https://pxgrid-api.readthedocs.io/
+
 Features
 --------
 
 - Support for both certificate and password authentication when connecting to pxGrid nodes
 - Commands and methods to interact with most pxGrid services
 - Websocket support for subscribing to topics.
 - Debug capabilities to show all low level interactions with pxGrid
@@ -154,15 +156,15 @@
 
   # Install the module
   pip install pxgrid-api
 
 Usage
 -----
 
-All commands are document and help can be retrived using help &lt;command&gt;
+All commands are document and help can be retrived using **help <command>**
 
 .. code-block:: console
 
   $ pxshell
   pxshell> help
 
   Documented commands (type help <topic>):
```

### Comparing `pxgrid-api-0.2.3/pyproject.toml` & `pxgrid-api-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires=["setuptools","wheel"]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "pxgrid-api"
-version = "0.2.3"
+version = "0.2.4"
 description = "pxGrid API library and command line tool"
 readme = "README.rst"
 authors = [{ name = "Viktor Bobrov", email = "vibobrov@cisco.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

### Comparing `pxgrid-api-0.2.3/src/pxapi/__main__.py` & `pxgrid-api-0.2.4/src/pxapi/__main__.py`

 * *Files identical despite different names*

### Comparing `pxgrid-api-0.2.3/src/pxapi/pxapi.py` & `pxgrid-api-0.2.4/src/pxapi/pxapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,15 +292,15 @@
         """Retrieve active session by MAC Address\n
         Reference: https://github.com/cisco-pxgrid/pxgrid-rest-ws/wiki/Session-Directory#post-restbaseurlgetsessionbymacaddress
 
         :param mac: endpoint MAC Address
         :return: dict containing all sessions for the MAC Address
         """
         self.__check_mac(mac)
-        return(self.__send_px_api(self.SERVICE_SESSION,"getSessionByMacAddress",{"mac":mac}))
+        return(self.__send_px_api(self.SERVICE_SESSION,"getSessionByMacAddress",{"macAddress":mac}))
 
     def get_user_groups(self):
         """Retrieve all user to group assignments\n
         Reference: https://github.com/cisco-pxgrid/pxgrid-rest-ws/wiki/Session-Directory#post-restbaseurlgetusergroups
 
         :return: dict of all user groups
         """
@@ -365,15 +365,15 @@
         """Retrieve ANC Policy assignment by MAC Address\n
         Reference https://github.com/cisco-pxgrid/pxgrid-rest-ws/wiki/ANC-configuration#post-restbaseurlgetendpointbymacaddress
 
         :param mac: MAC Address of the endpoint
         :return: dict of ANC Policy assigned to MAC Address
         """
         self.__check_mac(mac)
-        return(self.__send_px_api(self.SERVICE_ANC,"getEndpointByMacAddress",{"mac":mac}))
+        return(self.__send_px_api(self.SERVICE_ANC,"getEndpointByMacAddress",{"macAddress":mac}))
     
     
     def anc_get_endpoint_policies(self):
         """Retrieves endpoint to ANC Policy assignments based on MAC Address and NAS-IP-Address\n
         Reference: https://github.com/cisco-pxgrid/pxgrid-rest-ws/wiki/ANC-configuration#post-restbaseurlgetendpointpolicies-since-ise-26p7-27p2-30
 
         :return: dict with ANC Policy assigned to a MAC Address and NAS-IP-Address
@@ -386,25 +386,25 @@
         
         :param mac: endpoint MAC Address
         :param nas_ip: device IP Address
         :return: dict with ANC Policy assigned to a MAC Address and NAS-IP-Address
         """
         self.__check_mac(mac)
         self.__check_ip(nas_ip)
-        return(self.__send_px_api(self.SERVICE_ANC,"getEndpointByNasIpAddress",{"mac":mac,"nasIpAddress":nas_ip}))
+        return(self.__send_px_api(self.SERVICE_ANC,"getEndpointByNasIpAddress",{"macAddress":mac,"nasIpAddress":nas_ip}))
 
     def anc_apply_endpoint_by_mac_address(self,policy,mac):
         """Apply ANC Policy by MAC Address. Endpoint does not need to be online.\n
         Reference: https://github.com/cisco-pxgrid/pxgrid-rest-ws/wiki/ANC-configuration#post-restbaseurlapplyendpointbymacaddress
         
         :param policy: name of ANC Policy
         :param mac: MAC Address of endpoint
         """
         self.__check_mac(mac)
-        return(self.__send_px_api(self.SERVICE_ANC,"applyEndpointByMacAddress",{"policyName":policy,"mac":mac}))
+        return(self.__send_px_api(self.SERVICE_ANC,"applyEndpointByMacAddress",{"policyName":policy,"macAddress":mac}))
 
     def anc_apply_endpoint_by_ip_address(self,policy,ip):
         """Apply ANC Policy by IP Address. Requires that the endpoint is connected to the network.\n
         Reference: https://github.com/cisco-pxgrid/pxgrid-rest-ws/wiki/ANC-configuration#post-restbaseurlapplyendpointbyipaddress
 
         :param policyName: name of ANC Policy
         :param ip: IP Address of endpoint
@@ -418,35 +418,35 @@
 
         :param policy: name of ANC Policy
         :param mac: MAC Address of endpoint
         :param nas_ip: device IP Address
         """
         self.__check_mac(mac)
         self.__check_ip(nas_ip)
-        return(self.__send_px_api(self.SERVICE_ANC,"applyEndpointPolicy",{"policyName":policy,"mac":mac,"nasIpAddress":nas_ip}))
+        return(self.__send_px_api(self.SERVICE_ANC,"applyEndpointPolicy",{"policyName":policy,"macAddress":mac,"nasIpAddress":nas_ip}))
 
     def anc_clear_endpoint_by_mac_address(self,mac):
         """Clear ANC Policy from endpoint by MAC Address\n
         Reference: https://github.com/cisco-pxgrid/pxgrid-rest-ws/wiki/ANC-configuration#post-restbaseurlclearendpointbymacaddress
 
         :param mac: MAC Address of endpoint
         """
         self.__check_mac(mac)
-        return(self.__send_px_api(self.SERVICE_ANC,"clearEndpointByMacAddress",{"mac":mac}))
+        return(self.__send_px_api(self.SERVICE_ANC,"clearEndpointByMacAddress",{"macAddress":mac}))
     
     def anc_clear_endpoint_policy(self,mac,nas_ip):
         """Clear ANC Policy from endpoint by MAC Address and NAS-IP-Address\n
         Reference: https://github.com/cisco-pxgrid/pxgrid-rest-ws/wiki/ANC-configuration#post-restbaseurlclearendpointpolicy-since-ise-26p7-27p2-30
 
         :param mac: MAC Address of endpoint
         :param nas_ip: device IP Address
         """
         self.__check_mac(mac)
         self.__check_ip(nas_ip)
-        return(self.__send_px_api(self.SERVICE_ANC,"clearEndpointPolicy",{"mac":mac,"nasIpAddress":nas_ip}))
+        return(self.__send_px_api(self.SERVICE_ANC,"clearEndpointPolicy",{"macAddress":mac,"nasIpAddress":nas_ip}))
 
     def anc_get_operation_status(self,operation_id):
         """Get status of an ongoing ANC operation\n
         Reference: https://github.com/cisco-pxgrid/pxgrid-rest-ws/wiki/ANC-configuration#post-restbaseurlgetoperationstatus
 
         :param operation_id: Operation ID to look up
         :return: dict containing operation status
@@ -465,15 +465,15 @@
         """Retrieve MDM status of an endpoint based on MAC Address\n
         Reference: https://github.com/cisco-pxgrid/pxgrid-rest-ws/wiki/MDM#post-restbaseurlgetendpointbymacaddress
 
         :param mac: MAC Address of endpoint
         :return: dict with MDM attributes of the specified MAC Address
         """
         self.__check_mac(mac)
-        return(self.__send_px_api(self.SERVICE_MDM,"getEndpointByMacAddress",{"mac":mac}))
+        return(self.__send_px_api(self.SERVICE_MDM,"getEndpointByMacAddress",{"macAddress":mac}))
     
     def mdm_get_endpoints_by_type(self,mdm_type):
         """Retrive MDM endpoints by type\n
         Reference: https://github.com/cisco-pxgrid/pxgrid-rest-ws/wiki/MDM#post-restbaseurlgetendpointsbytype
 
         :param mdm_type: Valid options are NON_COMPLIANT, REGISTERED or DISCONNECTED
         :return: dict with MDM endpoints for the specified type
```

### Comparing `pxgrid-api-0.2.3/src/pxapi/stompframe.py` & `pxgrid-api-0.2.4/src/pxapi/stompframe.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#
+# Copyright (c) 2023 Cisco Systems, Inc. and/or its affiliates
+#
 import json
 
 class StompFrame:
     def __init__(self,command,headers,data=""):
         """Initializes class
 
         :param command: STOMP command
```

### Comparing `pxgrid-api-0.2.3/src/pxgrid_api.egg-info/PKG-INFO` & `pxgrid-api-0.2.4/src/pxgrid_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pxgrid-api
-Version: 0.2.3
+Version: 0.2.4
 Summary: pxGrid API library and command line tool
 Author-email: Viktor Bobrov <vibobrov@cisco.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -221,14 +221,16 @@
 
 This repo includes two components:
 - A python API library making it easier to interact with pxGrid services on ISE
 - Interactive CLI utility to interface with pxGrid without writing any code
 
 pxGrid requires FQDNs of all the nodes to be resolvable. It is not possible to use the library or the CLI utility to connect to ISE via IP address, even if there's just one node. Hosts record will work as well.
 
+Full API documention is available at https://pxgrid-api.readthedocs.io/
+
 Features
 --------
 
 - Support for both certificate and password authentication when connecting to pxGrid nodes
 - Commands and methods to interact with most pxGrid services
 - Websocket support for subscribing to topics.
 - Debug capabilities to show all low level interactions with pxGrid
@@ -371,15 +373,15 @@
 
   # Install the module
   pip install pxgrid-api
 
 Usage
 -----
 
-All commands are document and help can be retrived using help &lt;command&gt;
+All commands are document and help can be retrived using **help <command>**
 
 .. code-block:: console
 
   $ pxshell
   pxshell> help
 
   Documented commands (type help <topic>):
```

