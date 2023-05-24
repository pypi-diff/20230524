# Comparing `tmp/pulumiverse_astra-1.0.26.tar.gz` & `tmp/pulumiverse_astra-1.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_astra-1.0.26.tar", last modified: Sat Jul 16 20:03:04 2022, max compression
+gzip compressed data, was "pulumiverse_astra-1.0.37.tar", last modified: Wed May 24 17:53:00 2023, max compression
```

## Comparing `pulumiverse_astra-1.0.26.tar` & `pulumiverse_astra-1.0.37.tar`

### file list

```diff
@@ -1,42 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 20:03:04.512453 pulumiverse_astra-1.0.26/
--rw-r--r--   0 runner    (1001) docker     (121)     1780 2022-07-16 20:03:04.512453 pulumiverse_astra-1.0.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1412 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 20:03:04.512453 pulumiverse_astra-1.0.26/pulumiverse_astra/
--rw-r--r--   0 runner    (1001) docker     (121)     2684 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7782 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)    12404 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/access_list.py
--rw-r--r--   0 runner    (1001) docker     (121)    19174 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/cdc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 20:03:04.512453 pulumiverse_astra-1.0.26/pulumiverse_astra/config/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (121)    26216 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/database.py
--rw-r--r--   0 runner    (1001) docker     (121)     3912 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/get_access_list.py
--rw-r--r--   0 runner    (1001) docker     (121)    10161 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/get_astra_database.py
--rw-r--r--   0 runner    (1001) docker     (121)     3962 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/get_astra_databases.py
--rw-r--r--   0 runner    (1001) docker     (121)     2455 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/get_available_regions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3687 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/get_keyspace.py
--rw-r--r--   0 runner    (1001) docker     (121)     3489 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/get_keyspaces.py
--rw-r--r--   0 runner    (1001) docker     (121)     5378 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/get_private_link_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (121)     4349 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/get_private_links.py
--rw-r--r--   0 runner    (1001) docker     (121)     4761 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (121)     4203 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/get_secure_connect_bundle_url.py
--rw-r--r--   0 runner    (1001) docker     (121)     9595 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/keyspace.py
--rw-r--r--   0 runner    (1001) docker     (121)     9173 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    14353 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/private_link.py
--rw-r--r--   0 runner    (1001) docker     (121)    13839 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/private_link_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     4546 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    19844 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/role.py
--rw-r--r--   0 runner    (1001) docker     (121)    13789 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/streaming_tenant.py
--rw-r--r--   0 runner    (1001) docker     (121)     9847 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra/token.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-16 20:03:04.512453 pulumiverse_astra-1.0.26/pulumiverse_astra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1780 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/pulumiverse_astra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-16 20:03:04.512453 pulumiverse_astra-1.0.26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2212 2022-07-16 20:03:04.000000 pulumiverse_astra-1.0.26/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:53:00.260825 pulumiverse_astra-1.0.37/
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-24 17:53:00.260825 pulumiverse_astra-1.0.37/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:53:00.256825 pulumiverse_astra-1.0.37/pulumiverse_astra/
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/access_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18916 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/cdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:53:00.260825 pulumiverse_astra-1.0.37/pulumiverse_astra/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29495 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/get_access_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/get_astra_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/get_astra_databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/get_available_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/get_keyspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/get_keyspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/get_private_link_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/get_private_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/get_secure_connect_bundle_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/get_streaming_tenant_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/keyspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14181 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/private_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23699 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/private_link_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24482 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31108 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/streaming_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25385 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/streaming_tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16072 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/streaming_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22511 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/pulumiverse_astra/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:53:00.260825 pulumiverse_astra-1.0.37/pulumiverse_astra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-24 17:53:00.000000 pulumiverse_astra-1.0.37/pulumiverse_astra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-24 17:53:00.000000 pulumiverse_astra-1.0.37/pulumiverse_astra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 17:53:00.000000 pulumiverse_astra-1.0.37/pulumiverse_astra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 17:53:00.000000 pulumiverse_astra-1.0.37/pulumiverse_astra.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-24 17:53:00.000000 pulumiverse_astra-1.0.37/pulumiverse_astra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 17:53:00.000000 pulumiverse_astra-1.0.37/pulumiverse_astra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 17:53:00.260825 pulumiverse_astra-1.0.37/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-24 17:52:59.000000 pulumiverse_astra-1.0.37/setup.py
```

### Comparing `pulumiverse_astra-1.0.26/PKG-INFO` & `pulumiverse_astra-1.0.37/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_astra
-Version: 1.0.26
+Version: 1.0.37
 Summary: A Pulumi package for creating and managing astra cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-astra
 Keywords: pulumi astra category/cloud datastax
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumiverse_astra-1.0.26/README.md` & `pulumiverse_astra-1.0.37/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra/__init__.py` & `pulumiverse_astra-1.0.37/pulumiverse_astra/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,22 +12,28 @@
 from .get_astra_database import *
 from .get_astra_databases import *
 from .get_available_regions import *
 from .get_keyspace import *
 from .get_keyspaces import *
 from .get_private_link_endpoints import *
 from .get_private_links import *
+from .get_role import *
 from .get_roles import *
 from .get_secure_connect_bundle_url import *
+from .get_streaming_tenant_tokens import *
+from .get_users import *
 from .keyspace import *
 from .private_link import *
 from .private_link_endpoint import *
 from .provider import *
 from .role import *
+from .streaming_sink import *
 from .streaming_tenant import *
+from .streaming_topic import *
+from .table import *
 from .token import *
 from ._inputs import *
 from . import outputs
 
 # Make subpackages available:
 if typing.TYPE_CHECKING:
     import pulumiverse_astra.config as __config
@@ -92,22 +98,46 @@
   "fqn": "pulumiverse_astra",
   "classes": {
    "astra:index/role:Role": "Role"
   }
  },
  {
   "pkg": "astra",
+  "mod": "index/streamingSink",
+  "fqn": "pulumiverse_astra",
+  "classes": {
+   "astra:index/streamingSink:StreamingSink": "StreamingSink"
+  }
+ },
+ {
+  "pkg": "astra",
   "mod": "index/streamingTenant",
   "fqn": "pulumiverse_astra",
   "classes": {
    "astra:index/streamingTenant:StreamingTenant": "StreamingTenant"
   }
  },
  {
   "pkg": "astra",
+  "mod": "index/streamingTopic",
+  "fqn": "pulumiverse_astra",
+  "classes": {
+   "astra:index/streamingTopic:StreamingTopic": "StreamingTopic"
+  }
+ },
+ {
+  "pkg": "astra",
+  "mod": "index/table",
+  "fqn": "pulumiverse_astra",
+  "classes": {
+   "astra:index/table:Table": "Table"
+  }
+ },
+ {
+  "pkg": "astra",
   "mod": "index/token",
   "fqn": "pulumiverse_astra",
   "classes": {
    "astra:index/token:Token": "Token"
   }
  }
 ]
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra/_inputs.py` & `pulumiverse_astra-1.0.37/pulumiverse_astra/_inputs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
@@ -14,40 +15,54 @@
 
 @pulumi.input_type
 class AccessListAddressArgs:
     def __init__(__self__, *,
                  address: pulumi.Input[str],
                  enabled: pulumi.Input[bool],
                  description: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] address: IP Address/CIDR group that should have access
+        :param pulumi.Input[bool] enabled: Enable/disable this IP Address/CIDR group's access
+        :param pulumi.Input[str] description: Description for the IP Address/CIDR group
+        """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "enabled", enabled)
         if description is not None:
             pulumi.set(__self__, "description", description)
 
     @property
     @pulumi.getter
     def address(self) -> pulumi.Input[str]:
+        """
+        IP Address/CIDR group that should have access
+        """
         return pulumi.get(self, "address")
 
     @address.setter
     def address(self, value: pulumi.Input[str]):
         pulumi.set(self, "address", value)
 
     @property
     @pulumi.getter
     def enabled(self) -> pulumi.Input[bool]:
+        """
+        Enable/disable this IP Address/CIDR group's access
+        """
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: pulumi.Input[bool]):
         pulumi.set(self, "enabled", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
+        """
+        Description for the IP Address/CIDR group
+        """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra/_utilities.py` & `pulumiverse_astra-1.0.37/pulumiverse_astra/_utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,14 +94,25 @@
 _version = _get_semver_version()
 _version_str = str(_version)
 
 
 def get_version():
     return _version_str
 
+def get_resource_opts_defaults() -> pulumi.ResourceOptions:
+    return pulumi.ResourceOptions(
+        version=get_version(),
+        plugin_download_url=get_plugin_download_url(),
+    )
+
+def get_invoke_opts_defaults() -> pulumi.InvokeOptions:
+    return pulumi.InvokeOptions(
+        version=get_version(),
+        plugin_download_url=get_plugin_download_url(),
+    )
 
 def get_resource_args_opts(resource_args_type, resource_options_type, *args, **kwargs):
     """
     Return the resource args and options given the *args and **kwargs of a resource's
     __init__ method.
     """
 
@@ -232,8 +243,8 @@
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
 
 def get_plugin_download_url():
-	return "https://github.com/pulumiverse/pulumi-astra/releases/download/${VERSION}"
+	return "github://api.github.com/pulumiverse"
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra/access_list.py` & `pulumiverse_astra-1.0.37/pulumiverse_astra/access_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -230,22 +231,17 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  addresses: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['AccessListAddressArgs']]]]] = None,
                  database_id: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
-        if opts.plugin_download_url is None:
-            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AccessListArgs.__new__(AccessListArgs)
 
             if addresses is None and not opts.urn:
                 raise TypeError("Missing required property 'addresses'")
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra/cdc.py` & `pulumiverse_astra-1.0.37/pulumiverse_astra/cdc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['CdcArgs', 'Cdc']
@@ -19,15 +20,15 @@
                  table: pulumi.Input[str],
                  tenant_name: pulumi.Input[str],
                  topic_partitions: pulumi.Input[int]):
         """
         The set of arguments for constructing a Cdc resource.
         :param pulumi.Input[str] database_id: Astra database to create the keyspace.
         :param pulumi.Input[str] database_name: Astra database name.
-        :param pulumi.Input[str] keyspace: Initial keyspace name. For additional keyspaces, use the astra_keyspace resource.
+        :param pulumi.Input[str] keyspace: Initial keyspace name. For additional keyspaces, use the Keyspace resource.
         :param pulumi.Input[str] table: Astra database table.
         :param pulumi.Input[str] tenant_name: Streaming tenant name
         :param pulumi.Input[int] topic_partitions: Number of partitions in cdc topic.
         """
         pulumi.set(__self__, "database_id", database_id)
         pulumi.set(__self__, "database_name", database_name)
         pulumi.set(__self__, "keyspace", keyspace)
@@ -59,15 +60,15 @@
     def database_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "database_name", value)
 
     @property
     @pulumi.getter
     def keyspace(self) -> pulumi.Input[str]:
         """
-        Initial keyspace name. For additional keyspaces, use the astra_keyspace resource.
+        Initial keyspace name. For additional keyspaces, use the Keyspace resource.
         """
         return pulumi.get(self, "keyspace")
 
     @keyspace.setter
     def keyspace(self, value: pulumi.Input[str]):
         pulumi.set(self, "keyspace", value)
 
@@ -117,19 +118,19 @@
                  database_name: Optional[pulumi.Input[str]] = None,
                  keyspace: Optional[pulumi.Input[str]] = None,
                  table: Optional[pulumi.Input[str]] = None,
                  tenant_name: Optional[pulumi.Input[str]] = None,
                  topic_partitions: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering Cdc resources.
-        :param pulumi.Input[str] connector_status: Streaming tenant name
-        :param pulumi.Input[str] data_topic: Streaming tenant name
+        :param pulumi.Input[str] connector_status: Connector Status
+        :param pulumi.Input[str] data_topic: Data topic name
         :param pulumi.Input[str] database_id: Astra database to create the keyspace.
         :param pulumi.Input[str] database_name: Astra database name.
-        :param pulumi.Input[str] keyspace: Initial keyspace name. For additional keyspaces, use the astra_keyspace resource.
+        :param pulumi.Input[str] keyspace: Initial keyspace name. For additional keyspaces, use the Keyspace resource.
         :param pulumi.Input[str] table: Astra database table.
         :param pulumi.Input[str] tenant_name: Streaming tenant name
         :param pulumi.Input[int] topic_partitions: Number of partitions in cdc topic.
         """
         if connector_status is not None:
             pulumi.set(__self__, "connector_status", connector_status)
         if data_topic is not None:
@@ -147,27 +148,27 @@
         if topic_partitions is not None:
             pulumi.set(__self__, "topic_partitions", topic_partitions)
 
     @property
     @pulumi.getter(name="connectorStatus")
     def connector_status(self) -> Optional[pulumi.Input[str]]:
         """
-        Streaming tenant name
+        Connector Status
         """
         return pulumi.get(self, "connector_status")
 
     @connector_status.setter
     def connector_status(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "connector_status", value)
 
     @property
     @pulumi.getter(name="dataTopic")
     def data_topic(self) -> Optional[pulumi.Input[str]]:
         """
-        Streaming tenant name
+        Data topic name
         """
         return pulumi.get(self, "data_topic")
 
     @data_topic.setter
     def data_topic(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "data_topic", value)
 
@@ -195,15 +196,15 @@
     def database_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "database_name", value)
 
     @property
     @pulumi.getter
     def keyspace(self) -> Optional[pulumi.Input[str]]:
         """
-        Initial keyspace name. For additional keyspaces, use the astra_keyspace resource.
+        Initial keyspace name. For additional keyspaces, use the Keyspace resource.
         """
         return pulumi.get(self, "keyspace")
 
     @keyspace.setter
     def keyspace(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "keyspace", value)
 
@@ -287,15 +288,15 @@
          $ pulumi import astra:index/cdc:Cdc example databaseId/keyspace/table/tenantName
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] database_id: Astra database to create the keyspace.
         :param pulumi.Input[str] database_name: Astra database name.
-        :param pulumi.Input[str] keyspace: Initial keyspace name. For additional keyspaces, use the astra_keyspace resource.
+        :param pulumi.Input[str] keyspace: Initial keyspace name. For additional keyspaces, use the Keyspace resource.
         :param pulumi.Input[str] table: Astra database table.
         :param pulumi.Input[str] tenant_name: Streaming tenant name
         :param pulumi.Input[int] topic_partitions: Number of partitions in cdc topic.
         """
         ...
     @overload
     def __init__(__self__,
@@ -351,22 +352,17 @@
                  database_id: Optional[pulumi.Input[str]] = None,
                  database_name: Optional[pulumi.Input[str]] = None,
                  keyspace: Optional[pulumi.Input[str]] = None,
                  table: Optional[pulumi.Input[str]] = None,
                  tenant_name: Optional[pulumi.Input[str]] = None,
                  topic_partitions: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
-        if opts.plugin_download_url is None:
-            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = CdcArgs.__new__(CdcArgs)
 
             if database_id is None and not opts.urn:
                 raise TypeError("Missing required property 'database_id'")
@@ -409,19 +405,19 @@
         """
         Get an existing Cdc resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] connector_status: Streaming tenant name
-        :param pulumi.Input[str] data_topic: Streaming tenant name
+        :param pulumi.Input[str] connector_status: Connector Status
+        :param pulumi.Input[str] data_topic: Data topic name
         :param pulumi.Input[str] database_id: Astra database to create the keyspace.
         :param pulumi.Input[str] database_name: Astra database name.
-        :param pulumi.Input[str] keyspace: Initial keyspace name. For additional keyspaces, use the astra_keyspace resource.
+        :param pulumi.Input[str] keyspace: Initial keyspace name. For additional keyspaces, use the Keyspace resource.
         :param pulumi.Input[str] table: Astra database table.
         :param pulumi.Input[str] tenant_name: Streaming tenant name
         :param pulumi.Input[int] topic_partitions: Number of partitions in cdc topic.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _CdcState.__new__(_CdcState)
@@ -436,23 +432,23 @@
         __props__.__dict__["topic_partitions"] = topic_partitions
         return Cdc(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="connectorStatus")
     def connector_status(self) -> pulumi.Output[str]:
         """
-        Streaming tenant name
+        Connector Status
         """
         return pulumi.get(self, "connector_status")
 
     @property
     @pulumi.getter(name="dataTopic")
     def data_topic(self) -> pulumi.Output[str]:
         """
-        Streaming tenant name
+        Data topic name
         """
         return pulumi.get(self, "data_topic")
 
     @property
     @pulumi.getter(name="databaseId")
     def database_id(self) -> pulumi.Output[str]:
         """
@@ -468,15 +464,15 @@
         """
         return pulumi.get(self, "database_name")
 
     @property
     @pulumi.getter
     def keyspace(self) -> pulumi.Output[str]:
         """
-        Initial keyspace name. For additional keyspaces, use the astra_keyspace resource.
+        Initial keyspace name. For additional keyspaces, use the Keyspace resource.
         """
         return pulumi.get(self, "keyspace")
 
     @property
     @pulumi.getter
     def table(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra/config/vars.py` & `pulumiverse_astra-1.0.37/pulumiverse_astra/config/vars.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 import types
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra/database.py` & `pulumiverse_astra-1.0.37/pulumiverse_astra/database.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['DatabaseArgs', 'Database']
 
 @pulumi.input_type
 class DatabaseArgs:
     def __init__(__self__, *,
                  cloud_provider: pulumi.Input[str],
                  keyspace: pulumi.Input[str],
                  regions: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 deletion_protection: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Database resource.
         :param pulumi.Input[str] cloud_provider: The cloud provider to launch the database. (Currently supported: aws, azure, gcp)
-        :param pulumi.Input[str] keyspace: Initial keyspace name. For additional keyspaces, use the astra_keyspace resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] regions: Cloud regions to launch the database. (see https://docs.datastax.com/en/astra/docs/database-regions.html for supported
-               regions)
+        :param pulumi.Input[str] keyspace: Initial keyspace name. For additional keyspaces, use the Keyspace resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] regions: Cloud regions to launch the database. (see https://docs.datastax.com/en/astra/docs/database-regions.html for supported regions)
+        :param pulumi.Input[bool] deletion_protection: Whether or not to allow Terraform to destroy the instance. Unless this field is set to false in Terraform state, a
+               `terraform destroy` or `terraform apply` command that deletes the instance will fail. Defaults to `true`.
         :param pulumi.Input[str] name: Astra database name.
         """
         pulumi.set(__self__, "cloud_provider", cloud_provider)
         pulumi.set(__self__, "keyspace", keyspace)
         pulumi.set(__self__, "regions", regions)
+        if deletion_protection is not None:
+            pulumi.set(__self__, "deletion_protection", deletion_protection)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter(name="cloudProvider")
     def cloud_provider(self) -> pulumi.Input[str]:
         """
@@ -43,36 +48,48 @@
     def cloud_provider(self, value: pulumi.Input[str]):
         pulumi.set(self, "cloud_provider", value)
 
     @property
     @pulumi.getter
     def keyspace(self) -> pulumi.Input[str]:
         """
-        Initial keyspace name. For additional keyspaces, use the astra_keyspace resource.
+        Initial keyspace name. For additional keyspaces, use the Keyspace resource.
         """
         return pulumi.get(self, "keyspace")
 
     @keyspace.setter
     def keyspace(self, value: pulumi.Input[str]):
         pulumi.set(self, "keyspace", value)
 
     @property
     @pulumi.getter
     def regions(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        Cloud regions to launch the database. (see https://docs.datastax.com/en/astra/docs/database-regions.html for supported
-        regions)
+        Cloud regions to launch the database. (see https://docs.datastax.com/en/astra/docs/database-regions.html for supported regions)
         """
         return pulumi.get(self, "regions")
 
     @regions.setter
     def regions(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "regions", value)
 
     @property
+    @pulumi.getter(name="deletionProtection")
+    def deletion_protection(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether or not to allow Terraform to destroy the instance. Unless this field is set to false in Terraform state, a
+        `terraform destroy` or `terraform apply` command that deletes the instance will fail. Defaults to `true`.
+        """
+        return pulumi.get(self, "deletion_protection")
+
+    @deletion_protection.setter
+    def deletion_protection(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "deletion_protection", value)
+
+    @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         Astra database name.
         """
         return pulumi.get(self, "name")
 
@@ -85,14 +102,15 @@
 class _DatabaseState:
     def __init__(__self__, *,
                  additional_keyspaces: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  cloud_provider: Optional[pulumi.Input[str]] = None,
                  cqlsh_url: Optional[pulumi.Input[str]] = None,
                  data_endpoint_url: Optional[pulumi.Input[str]] = None,
                  datacenters: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 deletion_protection: Optional[pulumi.Input[bool]] = None,
                  grafana_url: Optional[pulumi.Input[str]] = None,
                  graphql_url: Optional[pulumi.Input[str]] = None,
                  keyspace: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  node_count: Optional[pulumi.Input[int]] = None,
                  organization_id: Optional[pulumi.Input[str]] = None,
                  owner_id: Optional[pulumi.Input[str]] = None,
@@ -101,39 +119,42 @@
                  status: Optional[pulumi.Input[str]] = None,
                  total_storage: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering Database resources.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] additional_keyspaces: Additional keyspaces
         :param pulumi.Input[str] cloud_provider: The cloud provider to launch the database. (Currently supported: aws, azure, gcp)
         :param pulumi.Input[str] cqlsh_url: The cqlsh_url
-        :param pulumi.Input[str] data_endpoint_url: The data_endpoint_url
+        :param pulumi.Input[str] data_endpoint_url: The data*endpoint*url
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] datacenters: Map of Datacenter IDs. The map key is "cloud_provider.region". Example: "GCP.us-east4".
+        :param pulumi.Input[bool] deletion_protection: Whether or not to allow Terraform to destroy the instance. Unless this field is set to false in Terraform state, a
+               `terraform destroy` or `terraform apply` command that deletes the instance will fail. Defaults to `true`.
         :param pulumi.Input[str] grafana_url: The grafana_url
         :param pulumi.Input[str] graphql_url: The graphql_url
-        :param pulumi.Input[str] keyspace: Initial keyspace name. For additional keyspaces, use the astra_keyspace resource.
+        :param pulumi.Input[str] keyspace: Initial keyspace name. For additional keyspaces, use the Keyspace resource.
         :param pulumi.Input[str] name: Astra database name.
         :param pulumi.Input[int] node_count: The node_count
         :param pulumi.Input[str] organization_id: The org id.
         :param pulumi.Input[str] owner_id: The owner id.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] regions: Cloud regions to launch the database. (see https://docs.datastax.com/en/astra/docs/database-regions.html for supported
-               regions)
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] regions: Cloud regions to launch the database. (see https://docs.datastax.com/en/astra/docs/database-regions.html for supported regions)
         :param pulumi.Input[int] replication_factor: The replication_factor
         :param pulumi.Input[str] status: The status
         :param pulumi.Input[int] total_storage: The total_storage
         """
         if additional_keyspaces is not None:
             pulumi.set(__self__, "additional_keyspaces", additional_keyspaces)
         if cloud_provider is not None:
             pulumi.set(__self__, "cloud_provider", cloud_provider)
         if cqlsh_url is not None:
             pulumi.set(__self__, "cqlsh_url", cqlsh_url)
         if data_endpoint_url is not None:
             pulumi.set(__self__, "data_endpoint_url", data_endpoint_url)
         if datacenters is not None:
             pulumi.set(__self__, "datacenters", datacenters)
+        if deletion_protection is not None:
+            pulumi.set(__self__, "deletion_protection", deletion_protection)
         if grafana_url is not None:
             pulumi.set(__self__, "grafana_url", grafana_url)
         if graphql_url is not None:
             pulumi.set(__self__, "graphql_url", graphql_url)
         if keyspace is not None:
             pulumi.set(__self__, "keyspace", keyspace)
         if name is not None:
@@ -189,15 +210,15 @@
     def cqlsh_url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cqlsh_url", value)
 
     @property
     @pulumi.getter(name="dataEndpointUrl")
     def data_endpoint_url(self) -> Optional[pulumi.Input[str]]:
         """
-        The data_endpoint_url
+        The data*endpoint*url
         """
         return pulumi.get(self, "data_endpoint_url")
 
     @data_endpoint_url.setter
     def data_endpoint_url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "data_endpoint_url", value)
 
@@ -210,14 +231,27 @@
         return pulumi.get(self, "datacenters")
 
     @datacenters.setter
     def datacenters(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "datacenters", value)
 
     @property
+    @pulumi.getter(name="deletionProtection")
+    def deletion_protection(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether or not to allow Terraform to destroy the instance. Unless this field is set to false in Terraform state, a
+        `terraform destroy` or `terraform apply` command that deletes the instance will fail. Defaults to `true`.
+        """
+        return pulumi.get(self, "deletion_protection")
+
+    @deletion_protection.setter
+    def deletion_protection(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "deletion_protection", value)
+
+    @property
     @pulumi.getter(name="grafanaUrl")
     def grafana_url(self) -> Optional[pulumi.Input[str]]:
         """
         The grafana_url
         """
         return pulumi.get(self, "grafana_url")
 
@@ -237,15 +271,15 @@
     def graphql_url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "graphql_url", value)
 
     @property
     @pulumi.getter
     def keyspace(self) -> Optional[pulumi.Input[str]]:
         """
-        Initial keyspace name. For additional keyspaces, use the astra_keyspace resource.
+        Initial keyspace name. For additional keyspaces, use the Keyspace resource.
         """
         return pulumi.get(self, "keyspace")
 
     @keyspace.setter
     def keyspace(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "keyspace", value)
 
@@ -297,16 +331,15 @@
     def owner_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "owner_id", value)
 
     @property
     @pulumi.getter
     def regions(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Cloud regions to launch the database. (see https://docs.datastax.com/en/astra/docs/database-regions.html for supported
-        regions)
+        Cloud regions to launch the database. (see https://docs.datastax.com/en/astra/docs/database-regions.html for supported regions)
         """
         return pulumi.get(self, "regions")
 
     @regions.setter
     def regions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "regions", value)
 
@@ -349,14 +382,15 @@
 
 class Database(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  cloud_provider: Optional[pulumi.Input[str]] = None,
+                 deletion_protection: Optional[pulumi.Input[bool]] = None,
                  keyspace: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  regions: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         ## Example Usage
 
@@ -375,18 +409,19 @@
         ```sh
          $ pulumi import astra:index/database:Database example 48bfc13b-c1a5-48db-b70f-b6ef9709872b
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cloud_provider: The cloud provider to launch the database. (Currently supported: aws, azure, gcp)
-        :param pulumi.Input[str] keyspace: Initial keyspace name. For additional keyspaces, use the astra_keyspace resource.
+        :param pulumi.Input[bool] deletion_protection: Whether or not to allow Terraform to destroy the instance. Unless this field is set to false in Terraform state, a
+               `terraform destroy` or `terraform apply` command that deletes the instance will fail. Defaults to `true`.
+        :param pulumi.Input[str] keyspace: Initial keyspace name. For additional keyspaces, use the Keyspace resource.
         :param pulumi.Input[str] name: Astra database name.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] regions: Cloud regions to launch the database. (see https://docs.datastax.com/en/astra/docs/database-regions.html for supported
-               regions)
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] regions: Cloud regions to launch the database. (see https://docs.datastax.com/en/astra/docs/database-regions.html for supported regions)
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: DatabaseArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -421,34 +456,31 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  cloud_provider: Optional[pulumi.Input[str]] = None,
+                 deletion_protection: Optional[pulumi.Input[bool]] = None,
                  keyspace: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  regions: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
-        if opts.plugin_download_url is None:
-            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DatabaseArgs.__new__(DatabaseArgs)
 
             if cloud_provider is None and not opts.urn:
                 raise TypeError("Missing required property 'cloud_provider'")
             __props__.__dict__["cloud_provider"] = cloud_provider
+            __props__.__dict__["deletion_protection"] = deletion_protection
             if keyspace is None and not opts.urn:
                 raise TypeError("Missing required property 'keyspace'")
             __props__.__dict__["keyspace"] = keyspace
             __props__.__dict__["name"] = name
             if regions is None and not opts.urn:
                 raise TypeError("Missing required property 'regions'")
             __props__.__dict__["regions"] = regions
@@ -475,14 +507,15 @@
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             additional_keyspaces: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             cloud_provider: Optional[pulumi.Input[str]] = None,
             cqlsh_url: Optional[pulumi.Input[str]] = None,
             data_endpoint_url: Optional[pulumi.Input[str]] = None,
             datacenters: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+            deletion_protection: Optional[pulumi.Input[bool]] = None,
             grafana_url: Optional[pulumi.Input[str]] = None,
             graphql_url: Optional[pulumi.Input[str]] = None,
             keyspace: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
             node_count: Optional[pulumi.Input[int]] = None,
             organization_id: Optional[pulumi.Input[str]] = None,
             owner_id: Optional[pulumi.Input[str]] = None,
@@ -496,38 +529,40 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] additional_keyspaces: Additional keyspaces
         :param pulumi.Input[str] cloud_provider: The cloud provider to launch the database. (Currently supported: aws, azure, gcp)
         :param pulumi.Input[str] cqlsh_url: The cqlsh_url
-        :param pulumi.Input[str] data_endpoint_url: The data_endpoint_url
+        :param pulumi.Input[str] data_endpoint_url: The data*endpoint*url
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] datacenters: Map of Datacenter IDs. The map key is "cloud_provider.region". Example: "GCP.us-east4".
+        :param pulumi.Input[bool] deletion_protection: Whether or not to allow Terraform to destroy the instance. Unless this field is set to false in Terraform state, a
+               `terraform destroy` or `terraform apply` command that deletes the instance will fail. Defaults to `true`.
         :param pulumi.Input[str] grafana_url: The grafana_url
         :param pulumi.Input[str] graphql_url: The graphql_url
-        :param pulumi.Input[str] keyspace: Initial keyspace name. For additional keyspaces, use the astra_keyspace resource.
+        :param pulumi.Input[str] keyspace: Initial keyspace name. For additional keyspaces, use the Keyspace resource.
         :param pulumi.Input[str] name: Astra database name.
         :param pulumi.Input[int] node_count: The node_count
         :param pulumi.Input[str] organization_id: The org id.
         :param pulumi.Input[str] owner_id: The owner id.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] regions: Cloud regions to launch the database. (see https://docs.datastax.com/en/astra/docs/database-regions.html for supported
-               regions)
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] regions: Cloud regions to launch the database. (see https://docs.datastax.com/en/astra/docs/database-regions.html for supported regions)
         :param pulumi.Input[int] replication_factor: The replication_factor
         :param pulumi.Input[str] status: The status
         :param pulumi.Input[int] total_storage: The total_storage
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _DatabaseState.__new__(_DatabaseState)
 
         __props__.__dict__["additional_keyspaces"] = additional_keyspaces
         __props__.__dict__["cloud_provider"] = cloud_provider
         __props__.__dict__["cqlsh_url"] = cqlsh_url
         __props__.__dict__["data_endpoint_url"] = data_endpoint_url
         __props__.__dict__["datacenters"] = datacenters
+        __props__.__dict__["deletion_protection"] = deletion_protection
         __props__.__dict__["grafana_url"] = grafana_url
         __props__.__dict__["graphql_url"] = graphql_url
         __props__.__dict__["keyspace"] = keyspace
         __props__.__dict__["name"] = name
         __props__.__dict__["node_count"] = node_count
         __props__.__dict__["organization_id"] = organization_id
         __props__.__dict__["owner_id"] = owner_id
@@ -561,27 +596,36 @@
         """
         return pulumi.get(self, "cqlsh_url")
 
     @property
     @pulumi.getter(name="dataEndpointUrl")
     def data_endpoint_url(self) -> pulumi.Output[str]:
         """
-        The data_endpoint_url
+        The data*endpoint*url
         """
         return pulumi.get(self, "data_endpoint_url")
 
     @property
     @pulumi.getter
     def datacenters(self) -> pulumi.Output[Mapping[str, str]]:
         """
         Map of Datacenter IDs. The map key is "cloud_provider.region". Example: "GCP.us-east4".
         """
         return pulumi.get(self, "datacenters")
 
     @property
+    @pulumi.getter(name="deletionProtection")
+    def deletion_protection(self) -> pulumi.Output[Optional[bool]]:
+        """
+        Whether or not to allow Terraform to destroy the instance. Unless this field is set to false in Terraform state, a
+        `terraform destroy` or `terraform apply` command that deletes the instance will fail. Defaults to `true`.
+        """
+        return pulumi.get(self, "deletion_protection")
+
+    @property
     @pulumi.getter(name="grafanaUrl")
     def grafana_url(self) -> pulumi.Output[str]:
         """
         The grafana_url
         """
         return pulumi.get(self, "grafana_url")
 
@@ -593,15 +637,15 @@
         """
         return pulumi.get(self, "graphql_url")
 
     @property
     @pulumi.getter
     def keyspace(self) -> pulumi.Output[str]:
         """
-        Initial keyspace name. For additional keyspaces, use the astra_keyspace resource.
+        Initial keyspace name. For additional keyspaces, use the Keyspace resource.
         """
         return pulumi.get(self, "keyspace")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
@@ -633,16 +677,15 @@
         """
         return pulumi.get(self, "owner_id")
 
     @property
     @pulumi.getter
     def regions(self) -> pulumi.Output[Sequence[str]]:
         """
-        Cloud regions to launch the database. (see https://docs.datastax.com/en/astra/docs/database-regions.html for supported
-        regions)
+        Cloud regions to launch the database. (see https://docs.datastax.com/en/astra/docs/database-regions.html for supported regions)
         """
         return pulumi.get(self, "regions")
 
     @property
     @pulumi.getter(name="replicationFactor")
     def replication_factor(self) -> pulumi.Output[int]:
         """
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra/get_access_list.py` & `pulumiverse_astra-1.0.37/pulumiverse_astra/get_access_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
@@ -34,24 +35,33 @@
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
 
     @property
     @pulumi.getter
     def addresses(self) -> Sequence['outputs.GetAccessListAddressResult']:
+        """
+        Addresses in the access list.
+        """
         return pulumi.get(self, "addresses")
 
     @property
     @pulumi.getter(name="databaseId")
     def database_id(self) -> str:
+        """
+        The ID of the Astra database.
+        """
         return pulumi.get(self, "database_id")
 
     @property
     @pulumi.getter
     def enabled(self) -> bool:
+        """
+        The Access list is enabled or disabled.
+        """
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
@@ -80,23 +90,21 @@
 
     ```python
     import pulumi
     import pulumi_astra as astra
 
     dev = astra.get_access_list(database_id="8d356587-73b3-430a-9c0e-d780332e2afb")
     ```
+
+
+    :param str database_id: The ID of the Astra database.
     """
     __args__ = dict()
     __args__['databaseId'] = database_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
-        if opts.plugin_download_url is None:
-            opts.plugin_download_url = _utilities.get_plugin_download_url()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('astra:index/getAccessList:getAccessList', __args__, opts=opts, typ=GetAccessListResult).value
 
     return AwaitableGetAccessListResult(
         addresses=__ret__.addresses,
         database_id=__ret__.database_id,
         enabled=__ret__.enabled,
         id=__ret__.id)
@@ -112,9 +120,12 @@
 
     ```python
     import pulumi
     import pulumi_astra as astra
 
     dev = astra.get_access_list(database_id="8d356587-73b3-430a-9c0e-d780332e2afb")
     ```
+
+
+    :param str database_id: The ID of the Astra database.
     """
     ...
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra/get_astra_database.py` & `pulumiverse_astra-1.0.37/pulumiverse_astra/get_astra_database.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
@@ -75,102 +76,153 @@
         if total_storage and not isinstance(total_storage, int):
             raise TypeError("Expected argument 'total_storage' to be a int")
         pulumi.set(__self__, "total_storage", total_storage)
 
     @property
     @pulumi.getter(name="additionalKeyspaces")
     def additional_keyspaces(self) -> Sequence[str]:
+        """
+        Additional keyspaces
+        """
         return pulumi.get(self, "additional_keyspaces")
 
     @property
     @pulumi.getter(name="cloudProvider")
     def cloud_provider(self) -> str:
+        """
+        Cloud provider (AWS, GCP, AZURE)
+        """
         return pulumi.get(self, "cloud_provider")
 
     @property
     @pulumi.getter(name="cqlshUrl")
     def cqlsh_url(self) -> str:
+        """
+        URL for cqlsh web
+        """
         return pulumi.get(self, "cqlsh_url")
 
     @property
     @pulumi.getter(name="dataEndpointUrl")
     def data_endpoint_url(self) -> str:
+        """
+        REST API URL
+        """
         return pulumi.get(self, "data_endpoint_url")
 
     @property
     @pulumi.getter(name="databaseId")
     def database_id(self) -> str:
+        """
+        Astra Database ID (system generated)
+        """
         return pulumi.get(self, "database_id")
 
     @property
     @pulumi.getter
     def datacenters(self) -> Mapping[str, str]:
+        """
+        Map of Datacenter IDs. The map key is "cloud_provider.region". Example: "GCP.us-east4".
+        """
         return pulumi.get(self, "datacenters")
 
     @property
     @pulumi.getter(name="grafanaUrl")
     def grafana_url(self) -> str:
+        """
+        URL for the grafana dashboard for this database
+        """
         return pulumi.get(self, "grafana_url")
 
     @property
     @pulumi.getter(name="graphqlUrl")
     def graphql_url(self) -> str:
+        """
+        Graphql URL
+        """
         return pulumi.get(self, "graphql_url")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def keyspace(self) -> str:
+        """
+        Initial keyspace
+        """
         return pulumi.get(self, "keyspace")
 
     @property
     @pulumi.getter
     def name(self) -> str:
+        """
+        Database name (user provided)
+        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="nodeCount")
     def node_count(self) -> int:
+        """
+        Node count (not relevant for serverless databases)
+        """
         return pulumi.get(self, "node_count")
 
     @property
     @pulumi.getter(name="organizationId")
     def organization_id(self) -> str:
+        """
+        Ordg id (system generated)
+        """
         return pulumi.get(self, "organization_id")
 
     @property
     @pulumi.getter(name="ownerId")
     def owner_id(self) -> str:
+        """
+        Owner id (system generated)
+        """
         return pulumi.get(self, "owner_id")
 
     @property
     @pulumi.getter
     def regions(self) -> Sequence[str]:
+        """
+        Cloud provider region. Get list of supported regions from regions data-source
+        """
         return pulumi.get(self, "regions")
 
     @property
     @pulumi.getter(name="replicationFactor")
     def replication_factor(self) -> int:
+        """
+        Replication Factor (not relevant for serverless databases)
+        """
         return pulumi.get(self, "replication_factor")
 
     @property
     @pulumi.getter
     def status(self) -> str:
+        """
+        Database status
+        """
         return pulumi.get(self, "status")
 
     @property
     @pulumi.getter(name="totalStorage")
     def total_storage(self) -> int:
+        """
+        Storage Capacity (not relevant for serverelss databases)
+        """
         return pulumi.get(self, "total_storage")
 
 
 class AwaitableGetAstraDatabaseResult(GetAstraDatabaseResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -205,23 +257,21 @@
 
     ```python
     import pulumi
     import pulumi_astra as astra
 
     db = astra.get_astra_database(database_id="8d356587-73b3-430a-9c0e-d780332e2afb")
     ```
+
+
+    :param str database_id: Astra Database ID (system generated)
     """
     __args__ = dict()
     __args__['databaseId'] = database_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
-        if opts.plugin_download_url is None:
-            opts.plugin_download_url = _utilities.get_plugin_download_url()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('astra:index/getAstraDatabase:getAstraDatabase', __args__, opts=opts, typ=GetAstraDatabaseResult).value
 
     return AwaitableGetAstraDatabaseResult(
         additional_keyspaces=__ret__.additional_keyspaces,
         cloud_provider=__ret__.cloud_provider,
         cqlsh_url=__ret__.cqlsh_url,
         data_endpoint_url=__ret__.data_endpoint_url,
@@ -251,9 +301,12 @@
 
     ```python
     import pulumi
     import pulumi_astra as astra
 
     db = astra.get_astra_database(database_id="8d356587-73b3-430a-9c0e-d780332e2afb")
     ```
+
+
+    :param str database_id: Astra Database ID (system generated)
     """
     ...
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra/get_astra_databases.py` & `pulumiverse_astra-1.0.37/pulumiverse_astra/get_astra_databases.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
@@ -34,32 +35,41 @@
         if status and not isinstance(status, str):
             raise TypeError("Expected argument 'status' to be a str")
         pulumi.set(__self__, "status", status)
 
     @property
     @pulumi.getter(name="cloudProvider")
     def cloud_provider(self) -> Optional[str]:
+        """
+        The cloud provider
+        """
         return pulumi.get(self, "cloud_provider")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def results(self) -> Sequence['outputs.GetAstraDatabasesResultResult']:
+        """
+        The list of Astra databases that match the search criteria.
+        """
         return pulumi.get(self, "results")
 
     @property
     @pulumi.getter
     def status(self) -> Optional[str]:
+        """
+        Status flter. Only return databases with matching status, if supplied. Otherwise return all databases matching other requirements
+        """
         return pulumi.get(self, "status")
 
 
 class AwaitableGetAstraDatabasesResult(GetAstraDatabasesResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -72,24 +82,23 @@
 
 
 def get_astra_databases(cloud_provider: Optional[str] = None,
                         status: Optional[str] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAstraDatabasesResult:
     """
     `get_astra_databases` provides a datasource for a list of Astra databases. This can be used to select databases within your Astra Organization.
+
+
+    :param str cloud_provider: The cloud provider
+    :param str status: Status flter. Only return databases with matching status, if supplied. Otherwise return all databases matching other requirements
     """
     __args__ = dict()
     __args__['cloudProvider'] = cloud_provider
     __args__['status'] = status
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
-        if opts.plugin_download_url is None:
-            opts.plugin_download_url = _utilities.get_plugin_download_url()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('astra:index/getAstraDatabases:getAstraDatabases', __args__, opts=opts, typ=GetAstraDatabasesResult).value
 
     return AwaitableGetAstraDatabasesResult(
         cloud_provider=__ret__.cloud_provider,
         id=__ret__.id,
         results=__ret__.results,
         status=__ret__.status)
@@ -97,9 +106,13 @@
 
 @_utilities.lift_output_func(get_astra_databases)
 def get_astra_databases_output(cloud_provider: Optional[pulumi.Input[Optional[str]]] = None,
                                status: Optional[pulumi.Input[Optional[str]]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAstraDatabasesResult]:
     """
     `get_astra_databases` provides a datasource for a list of Astra databases. This can be used to select databases within your Astra Organization.
+
+
+    :param str cloud_provider: The cloud provider
+    :param str status: Status flter. Only return databases with matching status, if supplied. Otherwise return all databases matching other requirements
     """
     ...
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra/get_available_regions.py` & `pulumiverse_astra-1.0.37/pulumiverse_astra/get_available_regions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
@@ -35,14 +36,17 @@
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def results(self) -> Sequence['outputs.GetAvailableRegionsResultResult']:
+        """
+        The list of supported Astra regions by cloud provider and tier.
+        """
         return pulumi.get(self, "results")
 
 
 class AwaitableGetAvailableRegionsResult(GetAvailableRegionsResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -62,18 +66,13 @@
     import pulumi
     import pulumi_astra as astra
 
     regions = astra.get_available_regions()
     ```
     """
     __args__ = dict()
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
-        if opts.plugin_download_url is None:
-            opts.plugin_download_url = _utilities.get_plugin_download_url()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('astra:index/getAvailableRegions:getAvailableRegions', __args__, opts=opts, typ=GetAvailableRegionsResult).value
 
     return AwaitableGetAvailableRegionsResult(
         id=__ret__.id,
         results=__ret__.results)
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra/get_keyspace.py` & `pulumiverse_astra-1.0.37/pulumiverse_astra/get_keyspace.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
@@ -30,27 +31,33 @@
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter(name="databaseId")
     def database_id(self) -> str:
+        """
+        The ID of the Astra database.
+        """
         return pulumi.get(self, "database_id")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> str:
+        """
+        The keyspace name.
+        """
         return pulumi.get(self, "name")
 
 
 class AwaitableGetKeyspaceResult(GetKeyspaceResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -72,24 +79,23 @@
     ```python
     import pulumi
     import pulumi_astra as astra
 
     dev = astra.get_keyspace(database_id="f9f4b1e0-4c05-451e-9bba-d631295a7f73",
         name="puppies")
     ```
+
+
+    :param str database_id: The ID of the Astra database.
+    :param str name: The keyspace name.
     """
     __args__ = dict()
     __args__['databaseId'] = database_id
     __args__['name'] = name
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
-        if opts.plugin_download_url is None:
-            opts.plugin_download_url = _utilities.get_plugin_download_url()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('astra:index/getKeyspace:getKeyspace', __args__, opts=opts, typ=GetKeyspaceResult).value
 
     return AwaitableGetKeyspaceResult(
         database_id=__ret__.database_id,
         id=__ret__.id,
         name=__ret__.name)
 
@@ -106,9 +112,13 @@
     ```python
     import pulumi
     import pulumi_astra as astra
 
     dev = astra.get_keyspace(database_id="f9f4b1e0-4c05-451e-9bba-d631295a7f73",
         name="puppies")
     ```
+
+
+    :param str database_id: The ID of the Astra database.
+    :param str name: The keyspace name.
     """
     ...
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra/get_keyspaces.py` & `pulumiverse_astra-1.0.37/pulumiverse_astra/get_keyspaces.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
@@ -31,27 +32,33 @@
         if results and not isinstance(results, list):
             raise TypeError("Expected argument 'results' to be a list")
         pulumi.set(__self__, "results", results)
 
     @property
     @pulumi.getter(name="databaseId")
     def database_id(self) -> str:
+        """
+        The ID of the Astra database.
+        """
         return pulumi.get(self, "database_id")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def results(self) -> Sequence['outputs.GetKeyspacesResultResult']:
+        """
+        The list of keyspaces that match the search criteria.
+        """
         return pulumi.get(self, "results")
 
 
 class AwaitableGetKeyspacesResult(GetKeyspacesResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -71,23 +78,21 @@
 
     ```python
     import pulumi
     import pulumi_astra as astra
 
     dev = astra.get_keyspaces(database_id="f9f4b1e0-4c05-451e-9bba-d631295a7f73")
     ```
+
+
+    :param str database_id: The ID of the Astra database.
     """
     __args__ = dict()
     __args__['databaseId'] = database_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
-        if opts.plugin_download_url is None:
-            opts.plugin_download_url = _utilities.get_plugin_download_url()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('astra:index/getKeyspaces:getKeyspaces', __args__, opts=opts, typ=GetKeyspacesResult).value
 
     return AwaitableGetKeyspacesResult(
         database_id=__ret__.database_id,
         id=__ret__.id,
         results=__ret__.results)
 
@@ -102,9 +107,12 @@
 
     ```python
     import pulumi
     import pulumi_astra as astra
 
     dev = astra.get_keyspaces(database_id="f9f4b1e0-4c05-451e-9bba-d631295a7f73")
     ```
+
+
+    :param str database_id: The ID of the Astra database.
     """
     ...
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra/get_private_link_endpoints.py` & `pulumiverse_astra-1.0.37/pulumiverse_astra/get_private_link_endpoints.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
@@ -37,37 +38,49 @@
         if results and not isinstance(results, list):
             raise TypeError("Expected argument 'results' to be a list")
         pulumi.set(__self__, "results", results)
 
     @property
     @pulumi.getter(name="databaseId")
     def database_id(self) -> str:
+        """
+        The ID of the Astra database.
+        """
         return pulumi.get(self, "database_id")
 
     @property
     @pulumi.getter(name="datacenterId")
     def datacenter_id(self) -> str:
+        """
+        The Datacenter ID of the Astra database.
+        """
         return pulumi.get(self, "datacenter_id")
 
     @property
     @pulumi.getter(name="endpointId")
     def endpoint_id(self) -> str:
+        """
+        Endpoint ID.
+        """
         return pulumi.get(self, "endpoint_id")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def results(self) -> Sequence['outputs.GetPrivateLinkEndpointsResultResult']:
+        """
+        The list of private links endpoint details that match the search criteria.
+        """
         return pulumi.get(self, "results")
 
 
 class AwaitableGetPrivateLinkEndpointsResult(GetPrivateLinkEndpointsResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -93,25 +106,25 @@
     import pulumi
     import pulumi_astra as astra
 
     dev = astra.get_private_link_endpoints(database_id="8d356587-73b3-430a-9c0e-d780332e2afb",
         datacenter_id="8d356587-73b3-430a-9c0e-d780332e2afb-1",
         endpoint_id="com.amazonaws.vpce.us-east-1.vpce-svc-03ac5a4b18ee480df")
     ```
+
+
+    :param str database_id: The ID of the Astra database.
+    :param str datacenter_id: The Datacenter ID of the Astra database.
+    :param str endpoint_id: Endpoint ID.
     """
     __args__ = dict()
     __args__['databaseId'] = database_id
     __args__['datacenterId'] = datacenter_id
     __args__['endpointId'] = endpoint_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
-        if opts.plugin_download_url is None:
-            opts.plugin_download_url = _utilities.get_plugin_download_url()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('astra:index/getPrivateLinkEndpoints:getPrivateLinkEndpoints', __args__, opts=opts, typ=GetPrivateLinkEndpointsResult).value
 
     return AwaitableGetPrivateLinkEndpointsResult(
         database_id=__ret__.database_id,
         datacenter_id=__ret__.datacenter_id,
         endpoint_id=__ret__.endpoint_id,
         id=__ret__.id,
@@ -132,9 +145,14 @@
     import pulumi
     import pulumi_astra as astra
 
     dev = astra.get_private_link_endpoints(database_id="8d356587-73b3-430a-9c0e-d780332e2afb",
         datacenter_id="8d356587-73b3-430a-9c0e-d780332e2afb-1",
         endpoint_id="com.amazonaws.vpce.us-east-1.vpce-svc-03ac5a4b18ee480df")
     ```
+
+
+    :param str database_id: The ID of the Astra database.
+    :param str datacenter_id: The Datacenter ID of the Astra database.
+    :param str endpoint_id: Endpoint ID.
     """
     ...
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra/get_private_links.py` & `pulumiverse_astra-1.0.37/pulumiverse_astra/get_private_links.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
@@ -34,32 +35,41 @@
         if results and not isinstance(results, list):
             raise TypeError("Expected argument 'results' to be a list")
         pulumi.set(__self__, "results", results)
 
     @property
     @pulumi.getter(name="databaseId")
     def database_id(self) -> str:
+        """
+        The ID of the Astra database.
+        """
         return pulumi.get(self, "database_id")
 
     @property
     @pulumi.getter(name="datacenterId")
     def datacenter_id(self) -> str:
+        """
+        The datacenter where of the Astra database.
+        """
         return pulumi.get(self, "datacenter_id")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def results(self) -> Sequence['outputs.GetPrivateLinksResultResult']:
+        """
+        The list of private links that match the search criteria.
+        """
         return pulumi.get(self, "results")
 
 
 class AwaitableGetPrivateLinksResult(GetPrivateLinksResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -82,24 +92,23 @@
     ```python
     import pulumi
     import pulumi_astra as astra
 
     dev = astra.get_private_links(database_id="a6bc9c26-e7ce-424f-84c7-0a00afb12588",
         datacenter_id="a6bc9c26-e7ce-424f-84c7-0a00afb12588-1")
     ```
+
+
+    :param str database_id: The ID of the Astra database.
+    :param str datacenter_id: The datacenter where of the Astra database.
     """
     __args__ = dict()
     __args__['databaseId'] = database_id
     __args__['datacenterId'] = datacenter_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
-        if opts.plugin_download_url is None:
-            opts.plugin_download_url = _utilities.get_plugin_download_url()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('astra:index/getPrivateLinks:getPrivateLinks', __args__, opts=opts, typ=GetPrivateLinksResult).value
 
     return AwaitableGetPrivateLinksResult(
         database_id=__ret__.database_id,
         datacenter_id=__ret__.datacenter_id,
         id=__ret__.id,
         results=__ret__.results)
@@ -117,9 +126,13 @@
     ```python
     import pulumi
     import pulumi_astra as astra
 
     dev = astra.get_private_links(database_id="a6bc9c26-e7ce-424f-84c7-0a00afb12588",
         datacenter_id="a6bc9c26-e7ce-424f-84c7-0a00afb12588-1")
     ```
+
+
+    :param str database_id: The ID of the Astra database.
+    :param str datacenter_id: The datacenter where of the Astra database.
     """
     ...
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra/get_roles.py` & `pulumiverse_astra-1.0.37/pulumiverse_astra/get_role.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetRolesResult',
-    'AwaitableGetRolesResult',
-    'get_roles',
-    'get_roles_output',
+    'GetRoleResult',
+    'AwaitableGetRoleResult',
+    'get_role',
+    'get_role_output',
 ]
 
 @pulumi.output_type
-class GetRolesResult:
+class GetRoleResult:
     """
-    A collection of values returned by getRoles.
+    A collection of values returned by getRole.
     """
     def __init__(__self__, description=None, effect=None, id=None, policies=None, resources=None, role_id=None, role_name=None):
         if description and not isinstance(description, str):
             raise TypeError("Expected argument 'description' to be a str")
         pulumi.set(__self__, "description", description)
         if effect and not isinstance(effect, str):
             raise TypeError("Expected argument 'effect' to be a str")
@@ -42,108 +43,127 @@
         if role_name and not isinstance(role_name, str):
             raise TypeError("Expected argument 'role_name' to be a str")
         pulumi.set(__self__, "role_name", role_name)
 
     @property
     @pulumi.getter
     def description(self) -> str:
+        """
+        Role description
+        """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def effect(self) -> str:
+        """
+        Role effect
+        """
         return pulumi.get(self, "effect")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def policies(self) -> Sequence[str]:
+        """
+        List of policies for the role. See https://docs.datastax.com/en/astra/docs/user-permissions.html#*operational*roles_detail for supported policies.
+        """
         return pulumi.get(self, "policies")
 
     @property
     @pulumi.getter
     def resources(self) -> Sequence[str]:
+        """
+        Resources for which role is applicable (format is "drn:astra:org:\\n\\n", followed by optional resource criteria. See example usage above).
+        """
         return pulumi.get(self, "resources")
 
     @property
     @pulumi.getter(name="roleId")
     def role_id(self) -> str:
+        """
+        Role ID, system generated
+        """
         return pulumi.get(self, "role_id")
 
     @property
     @pulumi.getter(name="roleName")
     def role_name(self) -> str:
+        """
+        Role name
+        """
         return pulumi.get(self, "role_name")
 
 
-class AwaitableGetRolesResult(GetRolesResult):
+class AwaitableGetRoleResult(GetRoleResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetRolesResult(
+        return GetRoleResult(
             description=self.description,
             effect=self.effect,
             id=self.id,
             policies=self.policies,
             resources=self.resources,
             role_id=self.role_id,
             role_name=self.role_name)
 
 
-def get_roles(role_id: Optional[str] = None,
-              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRolesResult:
+def get_role(role_id: Optional[str] = None,
+             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRoleResult:
     """
     `Role` provides a datasource that lists the custom roles for an org.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_astra as astra
 
-    dev = astra.get_roles(role_id="role-id-here")
+    dev = astra.get_role(role_id="role-id-here")
     ```
+
+
+    :param str role_id: Role ID, system generated
     """
     __args__ = dict()
     __args__['roleId'] = role_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
-        if opts.plugin_download_url is None:
-            opts.plugin_download_url = _utilities.get_plugin_download_url()
-    __ret__ = pulumi.runtime.invoke('astra:index/getRoles:getRoles', __args__, opts=opts, typ=GetRolesResult).value
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
+    __ret__ = pulumi.runtime.invoke('astra:index/getRole:getRole', __args__, opts=opts, typ=GetRoleResult).value
 
-    return AwaitableGetRolesResult(
+    return AwaitableGetRoleResult(
         description=__ret__.description,
         effect=__ret__.effect,
         id=__ret__.id,
         policies=__ret__.policies,
         resources=__ret__.resources,
         role_id=__ret__.role_id,
         role_name=__ret__.role_name)
 
 
-@_utilities.lift_output_func(get_roles)
-def get_roles_output(role_id: Optional[pulumi.Input[str]] = None,
-                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRolesResult]:
+@_utilities.lift_output_func(get_role)
+def get_role_output(role_id: Optional[pulumi.Input[str]] = None,
+                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRoleResult]:
     """
     `Role` provides a datasource that lists the custom roles for an org.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_astra as astra
 
-    dev = astra.get_roles(role_id="role-id-here")
+    dev = astra.get_role(role_id="role-id-here")
     ```
+
+
+    :param str role_id: Role ID, system generated
     """
     ...
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra/get_secure_connect_bundle_url.py` & `pulumiverse_astra-1.0.37/pulumiverse_astra/get_users.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,109 +1,131 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
+from . import outputs
 
 __all__ = [
-    'GetSecureConnectBundleUrlResult',
-    'AwaitableGetSecureConnectBundleUrlResult',
-    'get_secure_connect_bundle_url',
-    'get_secure_connect_bundle_url_output',
+    'GetUsersResult',
+    'AwaitableGetUsersResult',
+    'get_users',
+    'get_users_output',
 ]
 
 @pulumi.output_type
-class GetSecureConnectBundleUrlResult:
+class GetUsersResult:
     """
-    A collection of values returned by getSecureConnectBundleUrl.
+    A collection of values returned by getUsers.
     """
-    def __init__(__self__, database_id=None, id=None, url=None):
-        if database_id and not isinstance(database_id, str):
-            raise TypeError("Expected argument 'database_id' to be a str")
-        pulumi.set(__self__, "database_id", database_id)
+    def __init__(__self__, id=None, org_id=None, org_name=None, users=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if url and not isinstance(url, str):
-            raise TypeError("Expected argument 'url' to be a str")
-        pulumi.set(__self__, "url", url)
-
-    @property
-    @pulumi.getter(name="databaseId")
-    def database_id(self) -> str:
-        return pulumi.get(self, "database_id")
+        if org_id and not isinstance(org_id, str):
+            raise TypeError("Expected argument 'org_id' to be a str")
+        pulumi.set(__self__, "org_id", org_id)
+        if org_name and not isinstance(org_name, str):
+            raise TypeError("Expected argument 'org_name' to be a str")
+        pulumi.set(__self__, "org_name", org_name)
+        if users and not isinstance(users, list):
+            raise TypeError("Expected argument 'users' to be a list")
+        pulumi.set(__self__, "users", users)
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
+    @pulumi.getter(name="orgId")
+    def org_id(self) -> str:
+        """
+        Organization ID.
+        """
+        return pulumi.get(self, "org_id")
+
+    @property
+    @pulumi.getter(name="orgName")
+    def org_name(self) -> Optional[str]:
+        """
+        Organization Name.
+        """
+        return pulumi.get(self, "org_name")
+
+    @property
     @pulumi.getter
-    def url(self) -> str:
-        return pulumi.get(self, "url")
+    def users(self) -> Sequence['outputs.GetUsersUserResult']:
+        """
+        The list of Astra users.
+        """
+        return pulumi.get(self, "users")
 
 
-class AwaitableGetSecureConnectBundleUrlResult(GetSecureConnectBundleUrlResult):
+class AwaitableGetUsersResult(GetUsersResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetSecureConnectBundleUrlResult(
-            database_id=self.database_id,
+        return GetUsersResult(
             id=self.id,
-            url=self.url)
+            org_id=self.org_id,
+            org_name=self.org_name,
+            users=self.users)
 
 
-def get_secure_connect_bundle_url(database_id: Optional[str] = None,
-                                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSecureConnectBundleUrlResult:
+def get_users(org_name: Optional[str] = None,
+              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUsersResult:
     """
-    `get_secure_connect_bundle_url` provides a datasource that generates a temporary secure connect bundle URL. This URL lasts five minutes. Secure connect bundles are used to connect to Astra using cql cassandra drivers. See the [docs](https://docs.datastax.com/en/astra/docs/connecting-to-database.html) for more information on how to connect.
+    `get_users` provides a datasource for a list of Astra users. This can be used to select users within your Astra Organization.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_astra as astra
 
-    dev = astra.get_secure_connect_bundle_url(database_id="f9f4b1e0-4c05-451e-9bba-d631295a7f73")
+    dev = astra.get_users()
     ```
+
+
+    :param str org_name: Organization Name.
     """
     __args__ = dict()
-    __args__['databaseId'] = database_id
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
-        if opts.plugin_download_url is None:
-            opts.plugin_download_url = _utilities.get_plugin_download_url()
-    __ret__ = pulumi.runtime.invoke('astra:index/getSecureConnectBundleUrl:getSecureConnectBundleUrl', __args__, opts=opts, typ=GetSecureConnectBundleUrlResult).value
+    __args__['orgName'] = org_name
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
+    __ret__ = pulumi.runtime.invoke('astra:index/getUsers:getUsers', __args__, opts=opts, typ=GetUsersResult).value
 
-    return AwaitableGetSecureConnectBundleUrlResult(
-        database_id=__ret__.database_id,
+    return AwaitableGetUsersResult(
         id=__ret__.id,
-        url=__ret__.url)
+        org_id=__ret__.org_id,
+        org_name=__ret__.org_name,
+        users=__ret__.users)
 
 
-@_utilities.lift_output_func(get_secure_connect_bundle_url)
-def get_secure_connect_bundle_url_output(database_id: Optional[pulumi.Input[str]] = None,
-                                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSecureConnectBundleUrlResult]:
+@_utilities.lift_output_func(get_users)
+def get_users_output(org_name: Optional[pulumi.Input[Optional[str]]] = None,
+                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUsersResult]:
     """
-    `get_secure_connect_bundle_url` provides a datasource that generates a temporary secure connect bundle URL. This URL lasts five minutes. Secure connect bundles are used to connect to Astra using cql cassandra drivers. See the [docs](https://docs.datastax.com/en/astra/docs/connecting-to-database.html) for more information on how to connect.
+    `get_users` provides a datasource for a list of Astra users. This can be used to select users within your Astra Organization.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_astra as astra
 
-    dev = astra.get_secure_connect_bundle_url(database_id="f9f4b1e0-4c05-451e-9bba-d631295a7f73")
+    dev = astra.get_users()
     ```
+
+
+    :param str org_name: Organization Name.
     """
     ...
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra/keyspace.py` & `pulumiverse_astra-1.0.37/pulumiverse_astra/keyspace.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['KeyspaceArgs', 'Keyspace']
@@ -14,16 +15,15 @@
 class KeyspaceArgs:
     def __init__(__self__, *,
                  database_id: pulumi.Input[str],
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Keyspace resource.
         :param pulumi.Input[str] database_id: Astra database to create the keyspace.
-        :param pulumi.Input[str] name: Keyspace name can have up to 48 alpha-numeric characters and contain underscores; only letters and numbers are supported
-               as the first character.
+        :param pulumi.Input[str] name: Keyspace name can have up to 48 alpha-numeric characters and contain underscores; only letters and numbers are supported as the first character.
         """
         pulumi.set(__self__, "database_id", database_id)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter(name="databaseId")
@@ -37,16 +37,15 @@
     def database_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "database_id", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Keyspace name can have up to 48 alpha-numeric characters and contain underscores; only letters and numbers are supported
-        as the first character.
+        Keyspace name can have up to 48 alpha-numeric characters and contain underscores; only letters and numbers are supported as the first character.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -55,16 +54,15 @@
 class _KeyspaceState:
     def __init__(__self__, *,
                  database_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Keyspace resources.
         :param pulumi.Input[str] database_id: Astra database to create the keyspace.
-        :param pulumi.Input[str] name: Keyspace name can have up to 48 alpha-numeric characters and contain underscores; only letters and numbers are supported
-               as the first character.
+        :param pulumi.Input[str] name: Keyspace name can have up to 48 alpha-numeric characters and contain underscores; only letters and numbers are supported as the first character.
         """
         if database_id is not None:
             pulumi.set(__self__, "database_id", database_id)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
@@ -79,16 +77,15 @@
     def database_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "database_id", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Keyspace name can have up to 48 alpha-numeric characters and contain underscores; only letters and numbers are supported
-        as the first character.
+        Keyspace name can have up to 48 alpha-numeric characters and contain underscores; only letters and numbers are supported as the first character.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -120,16 +117,15 @@
         ```sh
          $ pulumi import astra:index/keyspace:Keyspace example 48bfc13b-c1a5-48db-b70f-b6ef9709872b/keyspace/example
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] database_id: Astra database to create the keyspace.
-        :param pulumi.Input[str] name: Keyspace name can have up to 48 alpha-numeric characters and contain underscores; only letters and numbers are supported
-               as the first character.
+        :param pulumi.Input[str] name: Keyspace name can have up to 48 alpha-numeric characters and contain underscores; only letters and numbers are supported as the first character.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: KeyspaceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -167,22 +163,17 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  database_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
-        if opts.plugin_download_url is None:
-            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = KeyspaceArgs.__new__(KeyspaceArgs)
 
             if database_id is None and not opts.urn:
                 raise TypeError("Missing required property 'database_id'")
@@ -204,16 +195,15 @@
         Get an existing Keyspace resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] database_id: Astra database to create the keyspace.
-        :param pulumi.Input[str] name: Keyspace name can have up to 48 alpha-numeric characters and contain underscores; only letters and numbers are supported
-               as the first character.
+        :param pulumi.Input[str] name: Keyspace name can have up to 48 alpha-numeric characters and contain underscores; only letters and numbers are supported as the first character.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _KeyspaceState.__new__(_KeyspaceState)
 
         __props__.__dict__["database_id"] = database_id
         __props__.__dict__["name"] = name
@@ -227,12 +217,11 @@
         """
         return pulumi.get(self, "database_id")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Keyspace name can have up to 48 alpha-numeric characters and contain underscores; only letters and numbers are supported
-        as the first character.
+        Keyspace name can have up to 48 alpha-numeric characters and contain underscores; only letters and numbers are supported as the first character.
         """
         return pulumi.get(self, "name")
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra/outputs.py` & `pulumiverse_astra-1.0.37/pulumiverse_astra/outputs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,73 +1,101 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
+from . import outputs
 
 __all__ = [
     'AccessListAddress',
     'GetAccessListAddressResult',
     'GetAstraDatabasesResultResult',
     'GetAvailableRegionsResultResult',
     'GetKeyspacesResultResult',
     'GetPrivateLinkEndpointsResultResult',
     'GetPrivateLinksResultResult',
+    'GetRolesResultResult',
+    'GetSecureConnectBundleUrlSecureBundleResult',
+    'GetSecureConnectBundleUrlSecureBundleCustomDomainBundleResult',
+    'GetStreamingTenantTokensTokenResult',
+    'GetUsersUserResult',
+    'GetUsersUserRoleResult',
 ]
 
 @pulumi.output_type
 class AccessListAddress(dict):
     def __init__(__self__, *,
                  address: str,
                  enabled: bool,
                  description: Optional[str] = None):
+        """
+        :param str address: IP Address/CIDR group that should have access
+        :param bool enabled: Enable/disable this IP Address/CIDR group's access
+        :param str description: Description for the IP Address/CIDR group
+        """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "enabled", enabled)
         if description is not None:
             pulumi.set(__self__, "description", description)
 
     @property
     @pulumi.getter
     def address(self) -> str:
+        """
+        IP Address/CIDR group that should have access
+        """
         return pulumi.get(self, "address")
 
     @property
     @pulumi.getter
     def enabled(self) -> bool:
+        """
+        Enable/disable this IP Address/CIDR group's access
+        """
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter
     def description(self) -> Optional[str]:
+        """
+        Description for the IP Address/CIDR group
+        """
         return pulumi.get(self, "description")
 
 
 @pulumi.output_type
 class GetAccessListAddressResult(dict):
     def __init__(__self__, *,
                  address: str,
                  enabled: bool,
                  description: Optional[str] = None):
+        """
+        :param bool enabled: The Access list is enabled or disabled.
+        """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "enabled", enabled)
         if description is not None:
             pulumi.set(__self__, "description", description)
 
     @property
     @pulumi.getter
     def address(self) -> str:
         return pulumi.get(self, "address")
 
     @property
     @pulumi.getter
     def enabled(self) -> bool:
+        """
+        The Access list is enabled or disabled.
+        """
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter
     def description(self) -> Optional[str]:
         return pulumi.get(self, "description")
 
@@ -88,14 +116,19 @@
                  node_count: int,
                  organization_id: str,
                  owner_id: str,
                  regions: Sequence[str],
                  replication_factor: int,
                  status: str,
                  total_storage: int):
+        """
+        :param str cloud_provider: The cloud provider
+        :param str id: The ID of this resource.
+        :param str status: Status flter. Only return databases with matching status, if supplied. Otherwise return all databases matching other requirements
+        """
         pulumi.set(__self__, "additional_keyspaces", additional_keyspaces)
         pulumi.set(__self__, "cloud_provider", cloud_provider)
         pulumi.set(__self__, "cqlsh_url", cqlsh_url)
         pulumi.set(__self__, "data_endpoint_url", data_endpoint_url)
         pulumi.set(__self__, "datacenters", datacenters)
         pulumi.set(__self__, "grafana_url", grafana_url)
         pulumi.set(__self__, "graphql_url", graphql_url)
@@ -114,14 +147,17 @@
     @pulumi.getter(name="additionalKeyspaces")
     def additional_keyspaces(self) -> Sequence[str]:
         return pulumi.get(self, "additional_keyspaces")
 
     @property
     @pulumi.getter(name="cloudProvider")
     def cloud_provider(self) -> str:
+        """
+        The cloud provider
+        """
         return pulumi.get(self, "cloud_provider")
 
     @property
     @pulumi.getter(name="cqlshUrl")
     def cqlsh_url(self) -> str:
         return pulumi.get(self, "cqlsh_url")
 
@@ -144,14 +180,17 @@
     @pulumi.getter(name="graphqlUrl")
     def graphql_url(self) -> str:
         return pulumi.get(self, "graphql_url")
 
     @property
     @pulumi.getter
     def id(self) -> str:
+        """
+        The ID of this resource.
+        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def keyspace(self) -> str:
         return pulumi.get(self, "keyspace")
 
@@ -184,14 +223,17 @@
     @pulumi.getter(name="replicationFactor")
     def replication_factor(self) -> int:
         return pulumi.get(self, "replication_factor")
 
     @property
     @pulumi.getter
     def status(self) -> str:
+        """
+        Status flter. Only return databases with matching status, if supplied. Otherwise return all databases matching other requirements
+        """
         return pulumi.get(self, "status")
 
     @property
     @pulumi.getter(name="totalStorage")
     def total_storage(self) -> int:
         return pulumi.get(self, "total_storage")
 
@@ -244,14 +286,17 @@
 @pulumi.output_type
 class GetPrivateLinkEndpointsResultResult(dict):
     def __init__(__self__, *,
                  create_time: str,
                  description: str,
                  endpoint_id: str,
                  status: str):
+        """
+        :param str endpoint_id: Endpoint ID.
+        """
         pulumi.set(__self__, "create_time", create_time)
         pulumi.set(__self__, "description", description)
         pulumi.set(__self__, "endpoint_id", endpoint_id)
         pulumi.set(__self__, "status", status)
 
     @property
     @pulumi.getter(name="createTime")
@@ -262,14 +307,17 @@
     @pulumi.getter
     def description(self) -> str:
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="endpointId")
     def endpoint_id(self) -> str:
+        """
+        Endpoint ID.
+        """
         return pulumi.get(self, "endpoint_id")
 
     @property
     @pulumi.getter
     def status(self) -> str:
         return pulumi.get(self, "status")
 
@@ -277,33 +325,264 @@
 @pulumi.output_type
 class GetPrivateLinksResultResult(dict):
     def __init__(__self__, *,
                  allowed_principals: Sequence[str],
                  datacenter_id: str,
                  endpoints: Sequence[str],
                  service_name: str):
+        """
+        :param str datacenter_id: The datacenter where of the Astra database.
+        """
         pulumi.set(__self__, "allowed_principals", allowed_principals)
         pulumi.set(__self__, "datacenter_id", datacenter_id)
         pulumi.set(__self__, "endpoints", endpoints)
         pulumi.set(__self__, "service_name", service_name)
 
     @property
     @pulumi.getter(name="allowedPrincipals")
     def allowed_principals(self) -> Sequence[str]:
         return pulumi.get(self, "allowed_principals")
 
     @property
     @pulumi.getter(name="datacenterId")
     def datacenter_id(self) -> str:
+        """
+        The datacenter where of the Astra database.
+        """
         return pulumi.get(self, "datacenter_id")
 
     @property
     @pulumi.getter
     def endpoints(self) -> Sequence[str]:
         return pulumi.get(self, "endpoints")
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> str:
         return pulumi.get(self, "service_name")
 
 
+@pulumi.output_type
+class GetRolesResultResult(dict):
+    def __init__(__self__, *,
+                 description: str,
+                 effect: str,
+                 policies: Sequence[str],
+                 resources: Sequence[str],
+                 role_id: str,
+                 role_name: str):
+        pulumi.set(__self__, "description", description)
+        pulumi.set(__self__, "effect", effect)
+        pulumi.set(__self__, "policies", policies)
+        pulumi.set(__self__, "resources", resources)
+        pulumi.set(__self__, "role_id", role_id)
+        pulumi.set(__self__, "role_name", role_name)
+
+    @property
+    @pulumi.getter
+    def description(self) -> str:
+        return pulumi.get(self, "description")
+
+    @property
+    @pulumi.getter
+    def effect(self) -> str:
+        return pulumi.get(self, "effect")
+
+    @property
+    @pulumi.getter
+    def policies(self) -> Sequence[str]:
+        return pulumi.get(self, "policies")
+
+    @property
+    @pulumi.getter
+    def resources(self) -> Sequence[str]:
+        return pulumi.get(self, "resources")
+
+    @property
+    @pulumi.getter(name="roleId")
+    def role_id(self) -> str:
+        return pulumi.get(self, "role_id")
+
+    @property
+    @pulumi.getter(name="roleName")
+    def role_name(self) -> str:
+        return pulumi.get(self, "role_name")
+
+
+@pulumi.output_type
+class GetSecureConnectBundleUrlSecureBundleResult(dict):
+    def __init__(__self__, *,
+                 custom_domain_bundles: Sequence['outputs.GetSecureConnectBundleUrlSecureBundleCustomDomainBundleResult'],
+                 datacenter_id: str,
+                 internal_migration_proxy_url: str,
+                 internal_url: str,
+                 migration_proxy_url: str,
+                 url: str):
+        """
+        :param str datacenter_id: The ID of the Astra datacenter. If omitted, all bundles will be fetched.
+        """
+        pulumi.set(__self__, "custom_domain_bundles", custom_domain_bundles)
+        pulumi.set(__self__, "datacenter_id", datacenter_id)
+        pulumi.set(__self__, "internal_migration_proxy_url", internal_migration_proxy_url)
+        pulumi.set(__self__, "internal_url", internal_url)
+        pulumi.set(__self__, "migration_proxy_url", migration_proxy_url)
+        pulumi.set(__self__, "url", url)
+
+    @property
+    @pulumi.getter(name="customDomainBundles")
+    def custom_domain_bundles(self) -> Sequence['outputs.GetSecureConnectBundleUrlSecureBundleCustomDomainBundleResult']:
+        return pulumi.get(self, "custom_domain_bundles")
+
+    @property
+    @pulumi.getter(name="datacenterId")
+    def datacenter_id(self) -> str:
+        """
+        The ID of the Astra datacenter. If omitted, all bundles will be fetched.
+        """
+        return pulumi.get(self, "datacenter_id")
+
+    @property
+    @pulumi.getter(name="internalMigrationProxyUrl")
+    def internal_migration_proxy_url(self) -> str:
+        return pulumi.get(self, "internal_migration_proxy_url")
+
+    @property
+    @pulumi.getter(name="internalUrl")
+    def internal_url(self) -> str:
+        return pulumi.get(self, "internal_url")
+
+    @property
+    @pulumi.getter(name="migrationProxyUrl")
+    def migration_proxy_url(self) -> str:
+        return pulumi.get(self, "migration_proxy_url")
+
+    @property
+    @pulumi.getter
+    def url(self) -> str:
+        return pulumi.get(self, "url")
+
+
+@pulumi.output_type
+class GetSecureConnectBundleUrlSecureBundleCustomDomainBundleResult(dict):
+    def __init__(__self__, *,
+                 api_fqdn: str,
+                 cql_fqdn: str,
+                 dashboard_fqdn: str,
+                 domain: str,
+                 url: str):
+        pulumi.set(__self__, "api_fqdn", api_fqdn)
+        pulumi.set(__self__, "cql_fqdn", cql_fqdn)
+        pulumi.set(__self__, "dashboard_fqdn", dashboard_fqdn)
+        pulumi.set(__self__, "domain", domain)
+        pulumi.set(__self__, "url", url)
+
+    @property
+    @pulumi.getter(name="apiFqdn")
+    def api_fqdn(self) -> str:
+        return pulumi.get(self, "api_fqdn")
+
+    @property
+    @pulumi.getter(name="cqlFqdn")
+    def cql_fqdn(self) -> str:
+        return pulumi.get(self, "cql_fqdn")
+
+    @property
+    @pulumi.getter(name="dashboardFqdn")
+    def dashboard_fqdn(self) -> str:
+        return pulumi.get(self, "dashboard_fqdn")
+
+    @property
+    @pulumi.getter
+    def domain(self) -> str:
+        return pulumi.get(self, "domain")
+
+    @property
+    @pulumi.getter
+    def url(self) -> str:
+        return pulumi.get(self, "url")
+
+
+@pulumi.output_type
+class GetStreamingTenantTokensTokenResult(dict):
+    def __init__(__self__, *,
+                 iat: int,
+                 iss: str,
+                 sub: str,
+                 token: str,
+                 token_id: str):
+        pulumi.set(__self__, "iat", iat)
+        pulumi.set(__self__, "iss", iss)
+        pulumi.set(__self__, "sub", sub)
+        pulumi.set(__self__, "token", token)
+        pulumi.set(__self__, "token_id", token_id)
+
+    @property
+    @pulumi.getter
+    def iat(self) -> int:
+        return pulumi.get(self, "iat")
+
+    @property
+    @pulumi.getter
+    def iss(self) -> str:
+        return pulumi.get(self, "iss")
+
+    @property
+    @pulumi.getter
+    def sub(self) -> str:
+        return pulumi.get(self, "sub")
+
+    @property
+    @pulumi.getter
+    def token(self) -> str:
+        return pulumi.get(self, "token")
+
+    @property
+    @pulumi.getter(name="tokenId")
+    def token_id(self) -> str:
+        return pulumi.get(self, "token_id")
+
+
+@pulumi.output_type
+class GetUsersUserResult(dict):
+    def __init__(__self__, *,
+                 email: str,
+                 roles: Sequence['outputs.GetUsersUserRoleResult'],
+                 status: str,
+                 user_id: str):
+        pulumi.set(__self__, "email", email)
+        pulumi.set(__self__, "roles", roles)
+        pulumi.set(__self__, "status", status)
+        pulumi.set(__self__, "user_id", user_id)
+
+    @property
+    @pulumi.getter
+    def email(self) -> str:
+        return pulumi.get(self, "email")
+
+    @property
+    @pulumi.getter
+    def roles(self) -> Sequence['outputs.GetUsersUserRoleResult']:
+        return pulumi.get(self, "roles")
+
+    @property
+    @pulumi.getter
+    def status(self) -> str:
+        return pulumi.get(self, "status")
+
+    @property
+    @pulumi.getter(name="userId")
+    def user_id(self) -> str:
+        return pulumi.get(self, "user_id")
+
+
+@pulumi.output_type
+class GetUsersUserRoleResult(dict):
+    def __init__(__self__, *,
+                 role_id: str):
+        pulumi.set(__self__, "role_id", role_id)
+
+    @property
+    @pulumi.getter(name="roleId")
+    def role_id(self) -> str:
+        return pulumi.get(self, "role_id")
+
+
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra/private_link.py` & `pulumiverse_astra-1.0.37/pulumiverse_astra/private_link.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['PrivateLinkArgs', 'PrivateLink']
@@ -213,22 +214,17 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  allowed_principals: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  database_id: Optional[pulumi.Input[str]] = None,
                  datacenter_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
-        if opts.plugin_download_url is None:
-            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PrivateLinkArgs.__new__(PrivateLinkArgs)
 
             if allowed_principals is None and not opts.urn:
                 raise TypeError("Missing required property 'allowed_principals'")
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra/provider.py` & `pulumiverse_astra-1.0.37/pulumiverse_astra/provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['ProviderArgs', 'Provider']
@@ -76,22 +77,17 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  token: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
-        if opts.plugin_download_url is None:
-            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
             __props__.__dict__["token"] = token
         super(Provider, __self__).__init__(
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra/role.py` & `pulumiverse_astra-1.0.37/pulumiverse_astra/role.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['RoleArgs', 'Role']
@@ -18,18 +19,16 @@
                  policies: pulumi.Input[Sequence[pulumi.Input[str]]],
                  resources: pulumi.Input[Sequence[pulumi.Input[str]]],
                  role_name: pulumi.Input[str]):
         """
         The set of arguments for constructing a Role resource.
         :param pulumi.Input[str] description: Role description
         :param pulumi.Input[str] effect: Role effect
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] policies: List of policies for the role. See
-               https://docs.datastax.com/en/astra/docs/user-permissions.html#_operational_roles_detail for supported policies.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] resources: Resources for which role is applicable (format is "drn:astra:org:<org UUID>", followed by optional resource criteria.
-               See example usage above).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] policies: List of policies for the role. See https://docs.datastax.com/en/astra/docs/user-permissions.html#*operational*roles_detail for supported policies.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] resources: Resources for which role is applicable (format is "drn:astra:org:\\n\\n", followed by optional resource criteria. See example usage above).
         :param pulumi.Input[str] role_name: Role name
         """
         pulumi.set(__self__, "description", description)
         pulumi.set(__self__, "effect", effect)
         pulumi.set(__self__, "policies", policies)
         pulumi.set(__self__, "resources", resources)
         pulumi.set(__self__, "role_name", role_name)
@@ -58,29 +57,27 @@
     def effect(self, value: pulumi.Input[str]):
         pulumi.set(self, "effect", value)
 
     @property
     @pulumi.getter
     def policies(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        List of policies for the role. See
-        https://docs.datastax.com/en/astra/docs/user-permissions.html#_operational_roles_detail for supported policies.
+        List of policies for the role. See https://docs.datastax.com/en/astra/docs/user-permissions.html#*operational*roles_detail for supported policies.
         """
         return pulumi.get(self, "policies")
 
     @policies.setter
     def policies(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "policies", value)
 
     @property
     @pulumi.getter
     def resources(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        Resources for which role is applicable (format is "drn:astra:org:<org UUID>", followed by optional resource criteria.
-        See example usage above).
+        Resources for which role is applicable (format is "drn:astra:org:\\n\\n", followed by optional resource criteria. See example usage above).
         """
         return pulumi.get(self, "resources")
 
     @resources.setter
     def resources(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "resources", value)
 
@@ -106,18 +103,16 @@
                  resources: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  role_id: Optional[pulumi.Input[str]] = None,
                  role_name: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Role resources.
         :param pulumi.Input[str] description: Role description
         :param pulumi.Input[str] effect: Role effect
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] policies: List of policies for the role. See
-               https://docs.datastax.com/en/astra/docs/user-permissions.html#_operational_roles_detail for supported policies.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] resources: Resources for which role is applicable (format is "drn:astra:org:<org UUID>", followed by optional resource criteria.
-               See example usage above).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] policies: List of policies for the role. See https://docs.datastax.com/en/astra/docs/user-permissions.html#*operational*roles_detail for supported policies.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] resources: Resources for which role is applicable (format is "drn:astra:org:\\n\\n", followed by optional resource criteria. See example usage above).
         :param pulumi.Input[str] role_id: Role ID, system generated
         :param pulumi.Input[str] role_name: Role name
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if effect is not None:
             pulumi.set(__self__, "effect", effect)
@@ -154,29 +149,27 @@
     def effect(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "effect", value)
 
     @property
     @pulumi.getter
     def policies(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of policies for the role. See
-        https://docs.datastax.com/en/astra/docs/user-permissions.html#_operational_roles_detail for supported policies.
+        List of policies for the role. See https://docs.datastax.com/en/astra/docs/user-permissions.html#*operational*roles_detail for supported policies.
         """
         return pulumi.get(self, "policies")
 
     @policies.setter
     def policies(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "policies", value)
 
     @property
     @pulumi.getter
     def resources(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Resources for which role is applicable (format is "drn:astra:org:<org UUID>", followed by optional resource criteria.
-        See example usage above).
+        Resources for which role is applicable (format is "drn:astra:org:\\n\\n", followed by optional resource criteria. See example usage above).
         """
         return pulumi.get(self, "resources")
 
     @resources.setter
     def resources(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "resources", value)
 
@@ -221,59 +214,97 @@
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumiverse_astra as astra
 
-        example = astra.Role("example",
-            description="test role",
-            effect="allow",
-            policies=["db-all-keyspace-create"],
-            resources=["drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73"],
-            role_name="puppies")
-        example2 = astra.Role("example2",
-            description="complex role",
+        # Example role that grants policy permissions to ALL Astra DBs in an organization
+        alldbsrole = astra.Role("alldbsrole",
+            role_name="alldbsrole",
+            description="Role that applies to all DBs in an org",
             effect="allow",
+            resources=[
+                "drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:*",
+                "drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:*:keyspace:*",
+                "drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:*:keyspace:*:table:*",
+            ],
             policies=[
-                "accesslist-read",
-                "db-all-keyspace-describe",
-                "db-keyspace-describe",
-                "db-table-select",
-                "db-table-describe",
-                "db-graphql",
-                "db-rest",
+                "org-db-view",
                 "db-cql",
-            ],
+                "db-table-alter",
+                "db-table-create",
+                "db-table-describe",
+                "db-table-modify",
+                "db-table-select",
+                "db-keyspace-alter",
+                "db-keyspace-describe",
+                "db-keyspace-modify",
+                "db-keyspace-authorize",
+                "db-keyspace-drop",
+                "db-keyspace-create",
+                "db-keyspace-grant",
+            ])
+        # Example resources for a more restricted role
+        # A Terraform managed Astra DB resource
+        exampledb = astra.Database("exampledb",
+            keyspace="primaryks",
+            cloud_provider="gcp",
+            regions=["us-east1"])
+        # Example application keyspaces
+        appks1 = astra.Keyspace("appks1", database_id=exampledb.id)
+        appks2 = astra.Keyspace("appks2", database_id=exampledb.id)
+        appks3 = astra.Keyspace("appks3", database_id=exampledb.id)
+        # Example role that grants policy permissions to specific keyspaces within a single Astra DB
+        singledbrole = astra.Role("singledbrole",
+            role_name="singledbrole",
+            description="Role that applies to specific keyspaces for a single Astra DB",
+            effect="allow",
             resources=[
-                "drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73",
-                "drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:5b70892f-e01a-4595-98e6-19ecc9985d50",
-                "drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:5b70892f-e01a-4595-98e6-19ecc9985d50:keyspace:system_schema:table:*",
-                "drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:5b70892f-e01a-4595-98e6-19ecc9985d50:keyspace:system:table:*",
-                "drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:5b70892f-e01a-4595-98e6-19ecc9985d50:keyspace:system_virtual_schema:table:*",
-                "drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:5b70892f-e01a-4595-98e6-19ecc9985d50:keyspace:*",
-                "drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:5b70892f-e01a-4595-98e6-19ecc9985d50:keyspace:*:table:*",
+                pulumi.Output.all(exampledb.id, exampledb.keyspace).apply(lambda id, keyspace: f"drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:{id}:keyspace:{keyspace}"),
+                pulumi.Output.all(exampledb.id, exampledb.keyspace).apply(lambda id, keyspace: f"drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:{id}:keyspace:{keyspace}:table:*"),
+                pulumi.Output.all(exampledb.id, appks1.name).apply(lambda id, name: f"drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:{id}:keyspace:{name}"),
+                pulumi.Output.all(exampledb.id, appks1.name).apply(lambda id, name: f"drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:{id}:keyspace:{name}:table:*"),
+                pulumi.Output.all(exampledb.id, appks2.name).apply(lambda id, name: f"drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:{id}:keyspace:{name}"),
+                pulumi.Output.all(exampledb.id, appks2.name).apply(lambda id, name: f"drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:{id}:keyspace:{name}:table:*"),
+                pulumi.Output.all(exampledb.id, appks3.name).apply(lambda id, name: f"drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:{id}:keyspace:{name}"),
+                pulumi.Output.all(exampledb.id, appks3.name).apply(lambda id, name: f"drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:{id}:keyspace:{name}:table:*"),
+                exampledb.id.apply(lambda id: f"drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:{id}:keyspace:futureks"),
+                exampledb.id.apply(lambda id: f"drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:{id}:keyspace:futureks:table:*"),
             ],
-            role_name="puppies")
+            policies=[
+                "org-db-view",
+                "db-cql",
+                "db-table-alter",
+                "db-table-create",
+                "db-table-describe",
+                "db-table-modify",
+                "db-table-select",
+                "db-keyspace-alter",
+                "db-keyspace-describe",
+                "db-keyspace-modify",
+                "db-keyspace-authorize",
+                "db-keyspace-drop",
+                "db-keyspace-create",
+                "db-keyspace-grant",
+            ])
         ```
 
         ## Import
 
         ```sh
          $ pulumi import astra:index/role:Role example role-id
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Role description
         :param pulumi.Input[str] effect: Role effect
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] policies: List of policies for the role. See
-               https://docs.datastax.com/en/astra/docs/user-permissions.html#_operational_roles_detail for supported policies.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] resources: Resources for which role is applicable (format is "drn:astra:org:<org UUID>", followed by optional resource criteria.
-               See example usage above).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] policies: List of policies for the role. See https://docs.datastax.com/en/astra/docs/user-permissions.html#*operational*roles_detail for supported policies.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] resources: Resources for which role is applicable (format is "drn:astra:org:\\n\\n", followed by optional resource criteria. See example usage above).
         :param pulumi.Input[str] role_name: Role name
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: RoleArgs,
@@ -283,43 +314,83 @@
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumiverse_astra as astra
 
-        example = astra.Role("example",
-            description="test role",
-            effect="allow",
-            policies=["db-all-keyspace-create"],
-            resources=["drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73"],
-            role_name="puppies")
-        example2 = astra.Role("example2",
-            description="complex role",
+        # Example role that grants policy permissions to ALL Astra DBs in an organization
+        alldbsrole = astra.Role("alldbsrole",
+            role_name="alldbsrole",
+            description="Role that applies to all DBs in an org",
             effect="allow",
+            resources=[
+                "drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:*",
+                "drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:*:keyspace:*",
+                "drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:*:keyspace:*:table:*",
+            ],
             policies=[
-                "accesslist-read",
-                "db-all-keyspace-describe",
-                "db-keyspace-describe",
-                "db-table-select",
-                "db-table-describe",
-                "db-graphql",
-                "db-rest",
+                "org-db-view",
                 "db-cql",
-            ],
+                "db-table-alter",
+                "db-table-create",
+                "db-table-describe",
+                "db-table-modify",
+                "db-table-select",
+                "db-keyspace-alter",
+                "db-keyspace-describe",
+                "db-keyspace-modify",
+                "db-keyspace-authorize",
+                "db-keyspace-drop",
+                "db-keyspace-create",
+                "db-keyspace-grant",
+            ])
+        # Example resources for a more restricted role
+        # A Terraform managed Astra DB resource
+        exampledb = astra.Database("exampledb",
+            keyspace="primaryks",
+            cloud_provider="gcp",
+            regions=["us-east1"])
+        # Example application keyspaces
+        appks1 = astra.Keyspace("appks1", database_id=exampledb.id)
+        appks2 = astra.Keyspace("appks2", database_id=exampledb.id)
+        appks3 = astra.Keyspace("appks3", database_id=exampledb.id)
+        # Example role that grants policy permissions to specific keyspaces within a single Astra DB
+        singledbrole = astra.Role("singledbrole",
+            role_name="singledbrole",
+            description="Role that applies to specific keyspaces for a single Astra DB",
+            effect="allow",
             resources=[
-                "drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73",
-                "drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:5b70892f-e01a-4595-98e6-19ecc9985d50",
-                "drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:5b70892f-e01a-4595-98e6-19ecc9985d50:keyspace:system_schema:table:*",
-                "drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:5b70892f-e01a-4595-98e6-19ecc9985d50:keyspace:system:table:*",
-                "drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:5b70892f-e01a-4595-98e6-19ecc9985d50:keyspace:system_virtual_schema:table:*",
-                "drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:5b70892f-e01a-4595-98e6-19ecc9985d50:keyspace:*",
-                "drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:5b70892f-e01a-4595-98e6-19ecc9985d50:keyspace:*:table:*",
+                pulumi.Output.all(exampledb.id, exampledb.keyspace).apply(lambda id, keyspace: f"drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:{id}:keyspace:{keyspace}"),
+                pulumi.Output.all(exampledb.id, exampledb.keyspace).apply(lambda id, keyspace: f"drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:{id}:keyspace:{keyspace}:table:*"),
+                pulumi.Output.all(exampledb.id, appks1.name).apply(lambda id, name: f"drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:{id}:keyspace:{name}"),
+                pulumi.Output.all(exampledb.id, appks1.name).apply(lambda id, name: f"drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:{id}:keyspace:{name}:table:*"),
+                pulumi.Output.all(exampledb.id, appks2.name).apply(lambda id, name: f"drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:{id}:keyspace:{name}"),
+                pulumi.Output.all(exampledb.id, appks2.name).apply(lambda id, name: f"drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:{id}:keyspace:{name}:table:*"),
+                pulumi.Output.all(exampledb.id, appks3.name).apply(lambda id, name: f"drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:{id}:keyspace:{name}"),
+                pulumi.Output.all(exampledb.id, appks3.name).apply(lambda id, name: f"drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:{id}:keyspace:{name}:table:*"),
+                exampledb.id.apply(lambda id: f"drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:{id}:keyspace:futureks"),
+                exampledb.id.apply(lambda id: f"drn:astra:org:f9f4b1e0-4c05-451e-9bba-d631295a7f73:db:{id}:keyspace:futureks:table:*"),
             ],
-            role_name="puppies")
+            policies=[
+                "org-db-view",
+                "db-cql",
+                "db-table-alter",
+                "db-table-create",
+                "db-table-describe",
+                "db-table-modify",
+                "db-table-select",
+                "db-keyspace-alter",
+                "db-keyspace-describe",
+                "db-keyspace-modify",
+                "db-keyspace-authorize",
+                "db-keyspace-drop",
+                "db-keyspace-create",
+                "db-keyspace-grant",
+            ])
         ```
 
         ## Import
 
         ```sh
          $ pulumi import astra:index/role:Role example role-id
         ```
@@ -341,22 +412,17 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  effect: Optional[pulumi.Input[str]] = None,
                  policies: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  resources: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  role_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
-        if opts.plugin_download_url is None:
-            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RoleArgs.__new__(RoleArgs)
 
             if description is None and not opts.urn:
                 raise TypeError("Missing required property 'description'")
@@ -395,18 +461,16 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Role description
         :param pulumi.Input[str] effect: Role effect
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] policies: List of policies for the role. See
-               https://docs.datastax.com/en/astra/docs/user-permissions.html#_operational_roles_detail for supported policies.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] resources: Resources for which role is applicable (format is "drn:astra:org:<org UUID>", followed by optional resource criteria.
-               See example usage above).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] policies: List of policies for the role. See https://docs.datastax.com/en/astra/docs/user-permissions.html#*operational*roles_detail for supported policies.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] resources: Resources for which role is applicable (format is "drn:astra:org:\\n\\n", followed by optional resource criteria. See example usage above).
         :param pulumi.Input[str] role_id: Role ID, system generated
         :param pulumi.Input[str] role_name: Role name
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _RoleState.__new__(_RoleState)
 
@@ -434,25 +498,23 @@
         """
         return pulumi.get(self, "effect")
 
     @property
     @pulumi.getter
     def policies(self) -> pulumi.Output[Sequence[str]]:
         """
-        List of policies for the role. See
-        https://docs.datastax.com/en/astra/docs/user-permissions.html#_operational_roles_detail for supported policies.
+        List of policies for the role. See https://docs.datastax.com/en/astra/docs/user-permissions.html#*operational*roles_detail for supported policies.
         """
         return pulumi.get(self, "policies")
 
     @property
     @pulumi.getter
     def resources(self) -> pulumi.Output[Sequence[str]]:
         """
-        Resources for which role is applicable (format is "drn:astra:org:<org UUID>", followed by optional resource criteria.
-        See example usage above).
+        Resources for which role is applicable (format is "drn:astra:org:\\n\\n", followed by optional resource criteria. See example usage above).
         """
         return pulumi.get(self, "resources")
 
     @property
     @pulumi.getter(name="roleId")
     def role_id(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra/streaming_tenant.py` & `pulumiverse_astra-1.0.37/pulumiverse_astra/streaming_topic.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['StreamingTenantArgs', 'StreamingTenant']
+__all__ = ['StreamingTopicArgs', 'StreamingTopic']
 
 @pulumi.input_type
-class StreamingTenantArgs:
+class StreamingTopicArgs:
     def __init__(__self__, *,
                  cloud_provider: pulumi.Input[str],
+                 namespace: pulumi.Input[str],
                  region: pulumi.Input[str],
                  tenant_name: pulumi.Input[str],
                  topic: pulumi.Input[str],
-                 user_email: pulumi.Input[str]):
+                 deletion_protection: Optional[pulumi.Input[bool]] = None):
         """
-        The set of arguments for constructing a StreamingTenant resource.
+        The set of arguments for constructing a StreamingTopic resource.
         :param pulumi.Input[str] cloud_provider: Cloud provider
+        :param pulumi.Input[str] namespace: Pulsar Namespace
         :param pulumi.Input[str] region: cloud region
         :param pulumi.Input[str] tenant_name: Streaming tenant name.
         :param pulumi.Input[str] topic: Streaming tenant topic.
-        :param pulumi.Input[str] user_email: User email for tenant.
+        :param pulumi.Input[bool] deletion_protection: Whether or not to allow Terraform to destroy this streaming topic. Unless this field is set to false in Terraform state,
+               a `terraform destroy` or `terraform apply` command that deletes the instance will fail. Defaults to `true`.
         """
         pulumi.set(__self__, "cloud_provider", cloud_provider)
+        pulumi.set(__self__, "namespace", namespace)
         pulumi.set(__self__, "region", region)
         pulumi.set(__self__, "tenant_name", tenant_name)
         pulumi.set(__self__, "topic", topic)
-        pulumi.set(__self__, "user_email", user_email)
+        if deletion_protection is not None:
+            pulumi.set(__self__, "deletion_protection", deletion_protection)
 
     @property
     @pulumi.getter(name="cloudProvider")
     def cloud_provider(self) -> pulumi.Input[str]:
         """
         Cloud provider
         """
@@ -42,14 +48,26 @@
 
     @cloud_provider.setter
     def cloud_provider(self, value: pulumi.Input[str]):
         pulumi.set(self, "cloud_provider", value)
 
     @property
     @pulumi.getter
+    def namespace(self) -> pulumi.Input[str]:
+        """
+        Pulsar Namespace
+        """
+        return pulumi.get(self, "namespace")
+
+    @namespace.setter
+    def namespace(self, value: pulumi.Input[str]):
+        pulumi.set(self, "namespace", value)
+
+    @property
+    @pulumi.getter
     def region(self) -> pulumi.Input[str]:
         """
         cloud region
         """
         return pulumi.get(self, "region")
 
     @region.setter
@@ -77,66 +95,97 @@
         return pulumi.get(self, "topic")
 
     @topic.setter
     def topic(self, value: pulumi.Input[str]):
         pulumi.set(self, "topic", value)
 
     @property
-    @pulumi.getter(name="userEmail")
-    def user_email(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="deletionProtection")
+    def deletion_protection(self) -> Optional[pulumi.Input[bool]]:
         """
-        User email for tenant.
+        Whether or not to allow Terraform to destroy this streaming topic. Unless this field is set to false in Terraform state,
+        a `terraform destroy` or `terraform apply` command that deletes the instance will fail. Defaults to `true`.
         """
-        return pulumi.get(self, "user_email")
+        return pulumi.get(self, "deletion_protection")
 
-    @user_email.setter
-    def user_email(self, value: pulumi.Input[str]):
-        pulumi.set(self, "user_email", value)
+    @deletion_protection.setter
+    def deletion_protection(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "deletion_protection", value)
 
 
 @pulumi.input_type
-class _StreamingTenantState:
+class _StreamingTopicState:
     def __init__(__self__, *,
                  cloud_provider: Optional[pulumi.Input[str]] = None,
+                 deletion_protection: Optional[pulumi.Input[bool]] = None,
+                 namespace: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tenant_name: Optional[pulumi.Input[str]] = None,
-                 topic: Optional[pulumi.Input[str]] = None,
-                 user_email: Optional[pulumi.Input[str]] = None):
+                 topic: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering StreamingTenant resources.
+        Input properties used for looking up and filtering StreamingTopic resources.
         :param pulumi.Input[str] cloud_provider: Cloud provider
+        :param pulumi.Input[bool] deletion_protection: Whether or not to allow Terraform to destroy this streaming topic. Unless this field is set to false in Terraform state,
+               a `terraform destroy` or `terraform apply` command that deletes the instance will fail. Defaults to `true`.
+        :param pulumi.Input[str] namespace: Pulsar Namespace
         :param pulumi.Input[str] region: cloud region
         :param pulumi.Input[str] tenant_name: Streaming tenant name.
         :param pulumi.Input[str] topic: Streaming tenant topic.
-        :param pulumi.Input[str] user_email: User email for tenant.
         """
         if cloud_provider is not None:
             pulumi.set(__self__, "cloud_provider", cloud_provider)
+        if deletion_protection is not None:
+            pulumi.set(__self__, "deletion_protection", deletion_protection)
+        if namespace is not None:
+            pulumi.set(__self__, "namespace", namespace)
         if region is not None:
             pulumi.set(__self__, "region", region)
         if tenant_name is not None:
             pulumi.set(__self__, "tenant_name", tenant_name)
         if topic is not None:
             pulumi.set(__self__, "topic", topic)
-        if user_email is not None:
-            pulumi.set(__self__, "user_email", user_email)
 
     @property
     @pulumi.getter(name="cloudProvider")
     def cloud_provider(self) -> Optional[pulumi.Input[str]]:
         """
         Cloud provider
         """
         return pulumi.get(self, "cloud_provider")
 
     @cloud_provider.setter
     def cloud_provider(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cloud_provider", value)
 
     @property
+    @pulumi.getter(name="deletionProtection")
+    def deletion_protection(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether or not to allow Terraform to destroy this streaming topic. Unless this field is set to false in Terraform state,
+        a `terraform destroy` or `terraform apply` command that deletes the instance will fail. Defaults to `true`.
+        """
+        return pulumi.get(self, "deletion_protection")
+
+    @deletion_protection.setter
+    def deletion_protection(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "deletion_protection", value)
+
+    @property
+    @pulumi.getter
+    def namespace(self) -> Optional[pulumi.Input[str]]:
+        """
+        Pulsar Namespace
+        """
+        return pulumi.get(self, "namespace")
+
+    @namespace.setter
+    def namespace(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "namespace", value)
+
+    @property
     @pulumi.getter
     def region(self) -> Optional[pulumi.Input[str]]:
         """
         cloud region
         """
         return pulumi.get(self, "region")
 
@@ -164,195 +213,164 @@
         """
         return pulumi.get(self, "topic")
 
     @topic.setter
     def topic(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "topic", value)
 
-    @property
-    @pulumi.getter(name="userEmail")
-    def user_email(self) -> Optional[pulumi.Input[str]]:
-        """
-        User email for tenant.
-        """
-        return pulumi.get(self, "user_email")
-
-    @user_email.setter
-    def user_email(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "user_email", value)
-
 
-class StreamingTenant(pulumi.CustomResource):
+class StreamingTopic(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  cloud_provider: Optional[pulumi.Input[str]] = None,
+                 deletion_protection: Optional[pulumi.Input[bool]] = None,
+                 namespace: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tenant_name: Optional[pulumi.Input[str]] = None,
                  topic: Optional[pulumi.Input[str]] = None,
-                 user_email: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        `StreamingTenant` creates an Astra Streaming tenant.
-
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumiverse_astra as astra
-
-        streaming_tenant_1 = astra.StreamingTenant("streamingTenant-1",
-            cloud_provider="gcp",
-            region="useast-4",
-            tenant_name="terraformtest",
-            topic="terraformtest",
-            user_email="seb@datastax.com")
-        ```
-
-        ## Import
-
-        ```sh
-         $ pulumi import astra:index/streamingTenant:StreamingTenant example tenant_name
-        ```
+        `StreamingTopic` creates an Astra Streaming topic.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cloud_provider: Cloud provider
+        :param pulumi.Input[bool] deletion_protection: Whether or not to allow Terraform to destroy this streaming topic. Unless this field is set to false in Terraform state,
+               a `terraform destroy` or `terraform apply` command that deletes the instance will fail. Defaults to `true`.
+        :param pulumi.Input[str] namespace: Pulsar Namespace
         :param pulumi.Input[str] region: cloud region
         :param pulumi.Input[str] tenant_name: Streaming tenant name.
         :param pulumi.Input[str] topic: Streaming tenant topic.
-        :param pulumi.Input[str] user_email: User email for tenant.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: StreamingTenantArgs,
+                 args: StreamingTopicArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        `StreamingTenant` creates an Astra Streaming tenant.
-
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumiverse_astra as astra
-
-        streaming_tenant_1 = astra.StreamingTenant("streamingTenant-1",
-            cloud_provider="gcp",
-            region="useast-4",
-            tenant_name="terraformtest",
-            topic="terraformtest",
-            user_email="seb@datastax.com")
-        ```
-
-        ## Import
-
-        ```sh
-         $ pulumi import astra:index/streamingTenant:StreamingTenant example tenant_name
-        ```
+        `StreamingTopic` creates an Astra Streaming topic.
 
         :param str resource_name: The name of the resource.
-        :param StreamingTenantArgs args: The arguments to use to populate this resource's properties.
+        :param StreamingTopicArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(StreamingTenantArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(StreamingTopicArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  cloud_provider: Optional[pulumi.Input[str]] = None,
+                 deletion_protection: Optional[pulumi.Input[bool]] = None,
+                 namespace: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tenant_name: Optional[pulumi.Input[str]] = None,
                  topic: Optional[pulumi.Input[str]] = None,
-                 user_email: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
-        if opts.plugin_download_url is None:
-            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = StreamingTenantArgs.__new__(StreamingTenantArgs)
+            __props__ = StreamingTopicArgs.__new__(StreamingTopicArgs)
 
             if cloud_provider is None and not opts.urn:
                 raise TypeError("Missing required property 'cloud_provider'")
             __props__.__dict__["cloud_provider"] = cloud_provider
+            __props__.__dict__["deletion_protection"] = deletion_protection
+            if namespace is None and not opts.urn:
+                raise TypeError("Missing required property 'namespace'")
+            __props__.__dict__["namespace"] = namespace
             if region is None and not opts.urn:
                 raise TypeError("Missing required property 'region'")
             __props__.__dict__["region"] = region
             if tenant_name is None and not opts.urn:
                 raise TypeError("Missing required property 'tenant_name'")
             __props__.__dict__["tenant_name"] = tenant_name
             if topic is None and not opts.urn:
                 raise TypeError("Missing required property 'topic'")
             __props__.__dict__["topic"] = topic
-            if user_email is None and not opts.urn:
-                raise TypeError("Missing required property 'user_email'")
-            __props__.__dict__["user_email"] = user_email
-        super(StreamingTenant, __self__).__init__(
-            'astra:index/streamingTenant:StreamingTenant',
+        super(StreamingTopic, __self__).__init__(
+            'astra:index/streamingTopic:StreamingTopic',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             cloud_provider: Optional[pulumi.Input[str]] = None,
+            deletion_protection: Optional[pulumi.Input[bool]] = None,
+            namespace: Optional[pulumi.Input[str]] = None,
             region: Optional[pulumi.Input[str]] = None,
             tenant_name: Optional[pulumi.Input[str]] = None,
-            topic: Optional[pulumi.Input[str]] = None,
-            user_email: Optional[pulumi.Input[str]] = None) -> 'StreamingTenant':
+            topic: Optional[pulumi.Input[str]] = None) -> 'StreamingTopic':
         """
-        Get an existing StreamingTenant resource's state with the given name, id, and optional extra
+        Get an existing StreamingTopic resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cloud_provider: Cloud provider
+        :param pulumi.Input[bool] deletion_protection: Whether or not to allow Terraform to destroy this streaming topic. Unless this field is set to false in Terraform state,
+               a `terraform destroy` or `terraform apply` command that deletes the instance will fail. Defaults to `true`.
+        :param pulumi.Input[str] namespace: Pulsar Namespace
         :param pulumi.Input[str] region: cloud region
         :param pulumi.Input[str] tenant_name: Streaming tenant name.
         :param pulumi.Input[str] topic: Streaming tenant topic.
-        :param pulumi.Input[str] user_email: User email for tenant.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _StreamingTenantState.__new__(_StreamingTenantState)
+        __props__ = _StreamingTopicState.__new__(_StreamingTopicState)
 
         __props__.__dict__["cloud_provider"] = cloud_provider
+        __props__.__dict__["deletion_protection"] = deletion_protection
+        __props__.__dict__["namespace"] = namespace
         __props__.__dict__["region"] = region
         __props__.__dict__["tenant_name"] = tenant_name
         __props__.__dict__["topic"] = topic
-        __props__.__dict__["user_email"] = user_email
-        return StreamingTenant(resource_name, opts=opts, __props__=__props__)
+        return StreamingTopic(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="cloudProvider")
     def cloud_provider(self) -> pulumi.Output[str]:
         """
         Cloud provider
         """
         return pulumi.get(self, "cloud_provider")
 
     @property
+    @pulumi.getter(name="deletionProtection")
+    def deletion_protection(self) -> pulumi.Output[Optional[bool]]:
+        """
+        Whether or not to allow Terraform to destroy this streaming topic. Unless this field is set to false in Terraform state,
+        a `terraform destroy` or `terraform apply` command that deletes the instance will fail. Defaults to `true`.
+        """
+        return pulumi.get(self, "deletion_protection")
+
+    @property
+    @pulumi.getter
+    def namespace(self) -> pulumi.Output[str]:
+        """
+        Pulsar Namespace
+        """
+        return pulumi.get(self, "namespace")
+
+    @property
     @pulumi.getter
     def region(self) -> pulumi.Output[str]:
         """
         cloud region
         """
         return pulumi.get(self, "region")
 
@@ -368,15 +386,7 @@
     @pulumi.getter
     def topic(self) -> pulumi.Output[str]:
         """
         Streaming tenant topic.
         """
         return pulumi.get(self, "topic")
 
-    @property
-    @pulumi.getter(name="userEmail")
-    def user_email(self) -> pulumi.Output[str]:
-        """
-        User email for tenant.
-        """
-        return pulumi.get(self, "user_email")
-
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra/token.py` & `pulumiverse_astra-1.0.37/pulumiverse_astra/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['TokenArgs', 'Token']
@@ -171,22 +172,17 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
-        if opts.plugin_download_url is None:
-            opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = TokenArgs.__new__(TokenArgs)
 
             if roles is None and not opts.urn:
                 raise TypeError("Missing required property 'roles'")
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra.egg-info/PKG-INFO` & `pulumiverse_astra-1.0.37/pulumiverse_astra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-astra
-Version: 1.0.26
+Version: 1.0.37
 Summary: A Pulumi package for creating and managing astra cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-astra
 Keywords: pulumi astra category/cloud datastax
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumiverse_astra-1.0.26/pulumiverse_astra.egg-info/SOURCES.txt` & `pulumiverse_astra-1.0.37/pulumiverse_astra.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,25 +10,31 @@
 pulumiverse_astra/get_astra_database.py
 pulumiverse_astra/get_astra_databases.py
 pulumiverse_astra/get_available_regions.py
 pulumiverse_astra/get_keyspace.py
 pulumiverse_astra/get_keyspaces.py
 pulumiverse_astra/get_private_link_endpoints.py
 pulumiverse_astra/get_private_links.py
+pulumiverse_astra/get_role.py
 pulumiverse_astra/get_roles.py
 pulumiverse_astra/get_secure_connect_bundle_url.py
+pulumiverse_astra/get_streaming_tenant_tokens.py
+pulumiverse_astra/get_users.py
 pulumiverse_astra/keyspace.py
 pulumiverse_astra/outputs.py
 pulumiverse_astra/private_link.py
 pulumiverse_astra/private_link_endpoint.py
 pulumiverse_astra/provider.py
 pulumiverse_astra/pulumi-plugin.json
 pulumiverse_astra/py.typed
 pulumiverse_astra/role.py
+pulumiverse_astra/streaming_sink.py
 pulumiverse_astra/streaming_tenant.py
+pulumiverse_astra/streaming_topic.py
+pulumiverse_astra/table.py
 pulumiverse_astra/token.py
 pulumiverse_astra.egg-info/PKG-INFO
 pulumiverse_astra.egg-info/SOURCES.txt
 pulumiverse_astra.egg-info/dependency_links.txt
 pulumiverse_astra.egg-info/not-zip-safe
 pulumiverse_astra.egg-info/requires.txt
 pulumiverse_astra.egg-info/top_level.txt
```

### Comparing `pulumiverse_astra-1.0.26/setup.py` & `pulumiverse_astra-1.0.37/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.0.26"
-PLUGIN_VERSION = "1.0.26"
+VERSION = "1.0.37"
+PLUGIN_VERSION = "1.0.37"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
-            check_call(['pulumi', 'plugin', 'install', 'resource', 'astra', PLUGIN_VERSION, '--server', 'https://github.com/pulumiverse/pulumi-astra/releases/download/${VERSION}'])
+            check_call(['pulumi', 'plugin', 'install', 'resource', 'astra', PLUGIN_VERSION, '--server', 'github://api.github.com/pulumiverse'])
         except OSError as error:
             if error.errno == errno.ENOENT:
                 print(f"""
                 There was an error installing the astra resource provider plugin.
                 It looks like `pulumi` is not installed on your system.
                 Please visit https://pulumi.com/ to install the Pulumi CLI.
                 You may try manually installing the plugin by running
```

