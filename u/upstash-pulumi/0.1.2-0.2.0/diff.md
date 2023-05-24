# Comparing `tmp/upstash_pulumi-0.1.2.tar.gz` & `tmp/upstash_pulumi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_pulumi-0.1.2.tar", last modified: Fri Feb 17 02:42:49 2023, max compression
+gzip compressed data, was "upstash_pulumi-0.2.0.tar", last modified: Wed May 24 10:33:40 2023, max compression
```

## Comparing `upstash_pulumi-0.1.2.tar` & `upstash_pulumi-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 02:42:49.272950 upstash_pulumi-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-02-17 02:42:49.272950 upstash_pulumi-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 02:42:49.272950 upstash_pulumi-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 02:42:49.268950 upstash_pulumi-0.1.2/upstash_pulumi/
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 02:42:49.272950 upstash_pulumi-0.1.2/upstash_pulumi/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi/get_kafka_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi/get_kafka_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi/get_kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi/get_q_stash_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi/get_q_stash_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi/get_q_stash_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi/get_redis_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi/get_team.py
--rw-r--r--   0 runner    (1001) docker     (123)    24159 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi/kafka_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    18654 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi/kafka_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    28859 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi/kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi/q_stash_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    27903 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi/q_stash_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi/q_stash_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)    35522 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi/redis_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi/team.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 02:42:49.268950 upstash_pulumi-0.1.2/upstash_pulumi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-17 02:42:49.000000 upstash_pulumi-0.1.2/upstash_pulumi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:33:40.720572 upstash_pulumi-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-24 10:33:40.720572 upstash_pulumi-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 10:33:40.720572 upstash_pulumi-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:33:40.720572 upstash_pulumi-0.2.0/upstash_pulumi/
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:33:40.720572 upstash_pulumi-0.2.0/upstash_pulumi/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/get_kafka_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/get_kafka_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/get_kafka_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/get_kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/get_q_stash_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/get_q_stash_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/get_q_stash_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/get_redis_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24159 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/kafka_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16506 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/kafka_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19196 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/kafka_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28859 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/q_stash_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28533 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/q_stash_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/q_stash_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47596 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/redis_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi/team.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:33:40.720572 upstash_pulumi-0.2.0/upstash_pulumi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 10:33:40.000000 upstash_pulumi-0.2.0/upstash_pulumi.egg-info/top_level.txt
```

### Comparing `upstash_pulumi-0.1.2/PKG-INFO` & `upstash_pulumi-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upstash_pulumi
-Version: 0.1.2
+Version: 0.2.0
 Summary: A Pulumi package for creating and managing upstash cloud resources.
 Home-page: https://www.upstash.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/upstash/pulumi-upstash
 Keywords: pulumi upstash category/cloud
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `upstash_pulumi-0.1.2/README.md` & `upstash_pulumi-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `upstash_pulumi-0.1.2/setup.py` & `upstash_pulumi-0.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.1.2"
-PLUGIN_VERSION = "0.1.2"
+VERSION = "0.2.0"
+PLUGIN_VERSION = "0.2.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
-            check_call(['pulumi', 'plugin', 'install', 'resource', 'upstash', PLUGIN_VERSION, '--server', 'https://github.com/upstash/pulumi-upstash/releases/download/v${VERSION}'])
+            check_call(['pulumi', 'plugin', 'install', 'resource', 'upstash', PLUGIN_VERSION, '--server', 'github://api.github.com/upstash/pulumi-upstash'])
         except OSError as error:
             if error.errno == errno.ENOENT:
                 print(f"""
                 There was an error installing the upstash resource provider plugin.
                 It looks like `pulumi` is not installed on your system.
                 Please visit https://pulumi.com/ to install the Pulumi CLI.
                 You may try manually installing the plugin by running
```

### Comparing `upstash_pulumi-0.1.2/upstash_pulumi/__init__.py` & `upstash_pulumi-0.2.0/upstash_pulumi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from .get_kafka_cluster import *
+from .get_kafka_connector import *
 from .get_kafka_credential import *
 from .get_kafka_topic import *
 from .get_q_stash_endpoint import *
 from .get_q_stash_schedule import *
 from .get_q_stash_topic import *
 from .get_redis_database import *
 from .get_team import *
 from .kafka_cluster import *
+from .kafka_connector import *
 from .kafka_credential import *
 from .kafka_topic import *
 from .provider import *
 from .q_stash_endpoint import *
 from .q_stash_schedule import *
 from .q_stash_topic import *
 from .redis_database import *
@@ -39,14 +41,22 @@
   "fqn": "upstash_pulumi",
   "classes": {
    "upstash:index/kafkaCluster:KafkaCluster": "KafkaCluster"
   }
  },
  {
   "pkg": "upstash",
+  "mod": "index/kafkaConnector",
+  "fqn": "upstash_pulumi",
+  "classes": {
+   "upstash:index/kafkaConnector:KafkaConnector": "KafkaConnector"
+  }
+ },
+ {
+  "pkg": "upstash",
   "mod": "index/kafkaCredential",
   "fqn": "upstash_pulumi",
   "classes": {
    "upstash:index/kafkaCredential:KafkaCredential": "KafkaCredential"
   }
  },
  {
```

### Comparing `upstash_pulumi-0.1.2/upstash_pulumi/_utilities.py` & `upstash_pulumi-0.2.0/upstash_pulumi/_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,8 +232,8 @@
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
 
 def get_plugin_download_url():
-	return "https://github.com/upstash/pulumi-upstash/releases/download/v${VERSION}"
+	return "github://api.github.com/upstash/pulumi-upstash"
```

### Comparing `upstash_pulumi-0.1.2/upstash_pulumi/config/vars.py` & `upstash_pulumi-0.2.0/upstash_pulumi/config/vars.py`

 * *Files identical despite different names*

### Comparing `upstash_pulumi-0.1.2/upstash_pulumi/get_kafka_cluster.py` & `upstash_pulumi-0.2.0/upstash_pulumi/get_kafka_cluster.py`

 * *Files identical despite different names*

### Comparing `upstash_pulumi-0.1.2/upstash_pulumi/get_kafka_credential.py` & `upstash_pulumi-0.2.0/upstash_pulumi/get_kafka_credential.py`

 * *Files identical despite different names*

### Comparing `upstash_pulumi-0.1.2/upstash_pulumi/get_kafka_topic.py` & `upstash_pulumi-0.2.0/upstash_pulumi/get_kafka_topic.py`

 * *Files identical despite different names*

### Comparing `upstash_pulumi-0.1.2/upstash_pulumi/get_q_stash_endpoint.py` & `upstash_pulumi-0.2.0/upstash_pulumi/get_q_stash_endpoint.py`

 * *Files identical despite different names*

### Comparing `upstash_pulumi-0.1.2/upstash_pulumi/get_q_stash_schedule.py` & `upstash_pulumi-0.2.0/upstash_pulumi/get_q_stash_schedule.py`

 * *Files identical despite different names*

### Comparing `upstash_pulumi-0.1.2/upstash_pulumi/get_q_stash_topic.py` & `upstash_pulumi-0.2.0/upstash_pulumi/get_q_stash_topic.py`

 * *Files identical despite different names*

### Comparing `upstash_pulumi-0.1.2/upstash_pulumi/get_redis_database.py` & `upstash_pulumi-0.2.0/upstash_pulumi/get_redis_database.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,18 @@
 ]
 
 @pulumi.output_type
 class GetRedisDatabaseResult:
     """
     A collection of values returned by getRedisDatabase.
     """
-    def __init__(__self__, consistent=None, creation_time=None, database_id=None, database_name=None, database_type=None, db_daily_bandwidth_limit=None, db_disk_threshold=None, db_max_clients=None, db_max_commands_per_second=None, db_max_entry_size=None, db_max_request_size=None, db_memory_threshold=None, endpoint=None, id=None, multizone=None, password=None, port=None, read_only_rest_token=None, region=None, rest_token=None, state=None, tls=None, user_email=None):
+    def __init__(__self__, auto_scale=None, consistent=None, creation_time=None, database_id=None, database_name=None, database_type=None, db_daily_bandwidth_limit=None, db_disk_threshold=None, db_max_clients=None, db_max_commands_per_second=None, db_max_entry_size=None, db_max_request_size=None, db_memory_threshold=None, endpoint=None, eviction=None, id=None, multizone=None, password=None, port=None, primary_region=None, read_only_rest_token=None, read_regions=None, region=None, rest_token=None, state=None, tls=None, user_email=None):
+        if auto_scale and not isinstance(auto_scale, bool):
+            raise TypeError("Expected argument 'auto_scale' to be a bool")
+        pulumi.set(__self__, "auto_scale", auto_scale)
         if consistent and not isinstance(consistent, bool):
             raise TypeError("Expected argument 'consistent' to be a bool")
         if consistent is not None:
             warnings.warn("""Consistent option is deprecated.""", DeprecationWarning)
             pulumi.log.warn("""consistent is deprecated: Consistent option is deprecated.""")
 
         pulumi.set(__self__, "consistent", consistent)
@@ -60,29 +63,42 @@
         pulumi.set(__self__, "db_max_request_size", db_max_request_size)
         if db_memory_threshold and not isinstance(db_memory_threshold, int):
             raise TypeError("Expected argument 'db_memory_threshold' to be a int")
         pulumi.set(__self__, "db_memory_threshold", db_memory_threshold)
         if endpoint and not isinstance(endpoint, str):
             raise TypeError("Expected argument 'endpoint' to be a str")
         pulumi.set(__self__, "endpoint", endpoint)
+        if eviction and not isinstance(eviction, bool):
+            raise TypeError("Expected argument 'eviction' to be a bool")
+        pulumi.set(__self__, "eviction", eviction)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if multizone and not isinstance(multizone, bool):
             raise TypeError("Expected argument 'multizone' to be a bool")
+        if multizone is not None:
+            warnings.warn("""Multizone option is deprecated. It is enabled by default for paid databases.""", DeprecationWarning)
+            pulumi.log.warn("""multizone is deprecated: Multizone option is deprecated. It is enabled by default for paid databases.""")
+
         pulumi.set(__self__, "multizone", multizone)
         if password and not isinstance(password, str):
             raise TypeError("Expected argument 'password' to be a str")
         pulumi.set(__self__, "password", password)
         if port and not isinstance(port, int):
             raise TypeError("Expected argument 'port' to be a int")
         pulumi.set(__self__, "port", port)
+        if primary_region and not isinstance(primary_region, str):
+            raise TypeError("Expected argument 'primary_region' to be a str")
+        pulumi.set(__self__, "primary_region", primary_region)
         if read_only_rest_token and not isinstance(read_only_rest_token, str):
             raise TypeError("Expected argument 'read_only_rest_token' to be a str")
         pulumi.set(__self__, "read_only_rest_token", read_only_rest_token)
+        if read_regions and not isinstance(read_regions, list):
+            raise TypeError("Expected argument 'read_regions' to be a list")
+        pulumi.set(__self__, "read_regions", read_regions)
         if region and not isinstance(region, str):
             raise TypeError("Expected argument 'region' to be a str")
         pulumi.set(__self__, "region", region)
         if rest_token and not isinstance(rest_token, str):
             raise TypeError("Expected argument 'rest_token' to be a str")
         pulumi.set(__self__, "rest_token", rest_token)
         if state and not isinstance(state, str):
@@ -92,14 +108,19 @@
             raise TypeError("Expected argument 'tls' to be a bool")
         pulumi.set(__self__, "tls", tls)
         if user_email and not isinstance(user_email, str):
             raise TypeError("Expected argument 'user_email' to be a str")
         pulumi.set(__self__, "user_email", user_email)
 
     @property
+    @pulumi.getter(name="autoScale")
+    def auto_scale(self) -> bool:
+        return pulumi.get(self, "auto_scale")
+
+    @property
     @pulumi.getter
     def consistent(self) -> bool:
         return pulumi.get(self, "consistent")
 
     @property
     @pulumi.getter(name="creationTime")
     def creation_time(self) -> int:
@@ -158,14 +179,19 @@
     @property
     @pulumi.getter
     def endpoint(self) -> str:
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter
+    def eviction(self) -> bool:
+        return pulumi.get(self, "eviction")
+
+    @property
+    @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
@@ -180,19 +206,29 @@
 
     @property
     @pulumi.getter
     def port(self) -> int:
         return pulumi.get(self, "port")
 
     @property
+    @pulumi.getter(name="primaryRegion")
+    def primary_region(self) -> str:
+        return pulumi.get(self, "primary_region")
+
+    @property
     @pulumi.getter(name="readOnlyRestToken")
     def read_only_rest_token(self) -> str:
         return pulumi.get(self, "read_only_rest_token")
 
     @property
+    @pulumi.getter(name="readRegions")
+    def read_regions(self) -> Sequence[str]:
+        return pulumi.get(self, "read_regions")
+
+    @property
     @pulumi.getter
     def region(self) -> str:
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="restToken")
     def rest_token(self) -> str:
@@ -216,32 +252,36 @@
 
 class AwaitableGetRedisDatabaseResult(GetRedisDatabaseResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetRedisDatabaseResult(
+            auto_scale=self.auto_scale,
             consistent=self.consistent,
             creation_time=self.creation_time,
             database_id=self.database_id,
             database_name=self.database_name,
             database_type=self.database_type,
             db_daily_bandwidth_limit=self.db_daily_bandwidth_limit,
             db_disk_threshold=self.db_disk_threshold,
             db_max_clients=self.db_max_clients,
             db_max_commands_per_second=self.db_max_commands_per_second,
             db_max_entry_size=self.db_max_entry_size,
             db_max_request_size=self.db_max_request_size,
             db_memory_threshold=self.db_memory_threshold,
             endpoint=self.endpoint,
+            eviction=self.eviction,
             id=self.id,
             multizone=self.multizone,
             password=self.password,
             port=self.port,
+            primary_region=self.primary_region,
             read_only_rest_token=self.read_only_rest_token,
+            read_regions=self.read_regions,
             region=self.region,
             rest_token=self.rest_token,
             state=self.state,
             tls=self.tls,
             user_email=self.user_email)
 
 
@@ -264,32 +304,36 @@
     if opts.version is None:
         opts.version = _utilities.get_version()
         if opts.plugin_download_url is None:
             opts.plugin_download_url = _utilities.get_plugin_download_url()
     __ret__ = pulumi.runtime.invoke('upstash:index/getRedisDatabase:getRedisDatabase', __args__, opts=opts, typ=GetRedisDatabaseResult).value
 
     return AwaitableGetRedisDatabaseResult(
+        auto_scale=__ret__.auto_scale,
         consistent=__ret__.consistent,
         creation_time=__ret__.creation_time,
         database_id=__ret__.database_id,
         database_name=__ret__.database_name,
         database_type=__ret__.database_type,
         db_daily_bandwidth_limit=__ret__.db_daily_bandwidth_limit,
         db_disk_threshold=__ret__.db_disk_threshold,
         db_max_clients=__ret__.db_max_clients,
         db_max_commands_per_second=__ret__.db_max_commands_per_second,
         db_max_entry_size=__ret__.db_max_entry_size,
         db_max_request_size=__ret__.db_max_request_size,
         db_memory_threshold=__ret__.db_memory_threshold,
         endpoint=__ret__.endpoint,
+        eviction=__ret__.eviction,
         id=__ret__.id,
         multizone=__ret__.multizone,
         password=__ret__.password,
         port=__ret__.port,
+        primary_region=__ret__.primary_region,
         read_only_rest_token=__ret__.read_only_rest_token,
+        read_regions=__ret__.read_regions,
         region=__ret__.region,
         rest_token=__ret__.rest_token,
         state=__ret__.state,
         tls=__ret__.tls,
         user_email=__ret__.user_email)
```

### Comparing `upstash_pulumi-0.1.2/upstash_pulumi/get_team.py` & `upstash_pulumi-0.2.0/upstash_pulumi/get_team.py`

 * *Files identical despite different names*

### Comparing `upstash_pulumi-0.1.2/upstash_pulumi/kafka_cluster.py` & `upstash_pulumi-0.2.0/upstash_pulumi/kafka_cluster.py`

 * *Files identical despite different names*

### Comparing `upstash_pulumi-0.1.2/upstash_pulumi/kafka_credential.py` & `upstash_pulumi-0.2.0/upstash_pulumi/kafka_credential.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,14 +260,19 @@
             cleanup_policy=var["cleanup_policy"],
             cluster_id=resource["upstash_kafka_cluster"]["exampleKafkaCluster"]["cluster_id"])
         example_kafka_credential = upstash.KafkaCredential("exampleKafkaCredential",
             cluster_id=example_kafka_cluster.cluster_id,
             credential_name="credentialFromTerraform",
             topic=example_kafka_topic.topic_name,
             permissions="ALL")
+        example_kafka_credential_all_topics = upstash.KafkaCredential("exampleKafkaCredentialAllTopics",
+            cluster_id=example_kafka_cluster.cluster_id,
+            credential_name="credentialFromTerraform",
+            topic="*",
+            permissions="ALL")
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cluster_id: ID of the kafka cluster
         :param pulumi.Input[str] credential_name: Name of the kafka credential
         :param pulumi.Input[str] permissions: Permission scope given to the kafka credential
@@ -299,14 +304,19 @@
             cleanup_policy=var["cleanup_policy"],
             cluster_id=resource["upstash_kafka_cluster"]["exampleKafkaCluster"]["cluster_id"])
         example_kafka_credential = upstash.KafkaCredential("exampleKafkaCredential",
             cluster_id=example_kafka_cluster.cluster_id,
             credential_name="credentialFromTerraform",
             topic=example_kafka_topic.topic_name,
             permissions="ALL")
+        example_kafka_credential_all_topics = upstash.KafkaCredential("exampleKafkaCredentialAllTopics",
+            cluster_id=example_kafka_cluster.cluster_id,
+            credential_name="credentialFromTerraform",
+            topic="*",
+            permissions="ALL")
         ```
 
         :param str resource_name: The name of the resource.
         :param KafkaCredentialArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `upstash_pulumi-0.1.2/upstash_pulumi/kafka_topic.py` & `upstash_pulumi-0.2.0/upstash_pulumi/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `upstash_pulumi-0.1.2/upstash_pulumi/provider.py` & `upstash_pulumi-0.2.0/upstash_pulumi/provider.py`

 * *Files identical despite different names*

### Comparing `upstash_pulumi-0.1.2/upstash_pulumi/q_stash_endpoint.py` & `upstash_pulumi-0.2.0/upstash_pulumi/q_stash_endpoint.py`

 * *Files identical despite different names*

### Comparing `upstash_pulumi-0.1.2/upstash_pulumi/q_stash_schedule.py` & `upstash_pulumi-0.2.0/upstash_pulumi/q_stash_schedule.py`

 * *Files 2% similar despite different names*

```diff
@@ -422,15 +422,27 @@
                  delay: Optional[pulumi.Input[str]] = None,
                  destination: Optional[pulumi.Input[str]] = None,
                  forward_headers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  not_before: Optional[pulumi.Input[int]] = None,
                  retries: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
-        Create a QStashSchedule resource with the given unique name, props, and options.
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import upstash_pulumi as upstash
+
+        example_qstash_schedule = upstash.QStashSchedule("exampleQstashSchedule",
+            destination=resource["upstash_qstash_topic"]["exampleQstashTopic"]["topic_id"],
+            cron="* * * * */2")
+        # or simply provide a link
+        # destination = "https://***.***"
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] body: Body to send for the POST request in string format. Needs escaping (\) double quotes.
         :param pulumi.Input[str] callback: Callback URL for Qstash Schedule.
         :param pulumi.Input[bool] content_based_deduplication: Content Based Deduplication (bool) for Qstash Scheduling.
         :param pulumi.Input[str] content_type: Content type for Qstash Scheduling.
         :param pulumi.Input[str] cron: Cron string for Qstash Schedule
@@ -444,15 +456,27 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: QStashScheduleArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a QStashSchedule resource with the given unique name, props, and options.
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import upstash_pulumi as upstash
+
+        example_qstash_schedule = upstash.QStashSchedule("exampleQstashSchedule",
+            destination=resource["upstash_qstash_topic"]["exampleQstashTopic"]["topic_id"],
+            cron="* * * * */2")
+        # or simply provide a link
+        # destination = "https://***.***"
+        ```
+
         :param str resource_name: The name of the resource.
         :param QStashScheduleArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(QStashScheduleArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `upstash_pulumi-0.1.2/upstash_pulumi/q_stash_topic.py` & `upstash_pulumi-0.2.0/upstash_pulumi/q_stash_topic.py`

 * *Files identical despite different names*

### Comparing `upstash_pulumi-0.1.2/upstash_pulumi/redis_database.py` & `upstash_pulumi-0.2.0/upstash_pulumi/redis_database.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,37 +11,59 @@
 __all__ = ['RedisDatabaseArgs', 'RedisDatabase']
 
 @pulumi.input_type
 class RedisDatabaseArgs:
     def __init__(__self__, *,
                  database_name: pulumi.Input[str],
                  region: pulumi.Input[str],
+                 auto_scale: Optional[pulumi.Input[bool]] = None,
                  consistent: Optional[pulumi.Input[bool]] = None,
+                 eviction: Optional[pulumi.Input[bool]] = None,
                  multizone: Optional[pulumi.Input[bool]] = None,
+                 primary_region: Optional[pulumi.Input[str]] = None,
+                 read_regions: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tls: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a RedisDatabase resource.
         :param pulumi.Input[str] database_name: Name of the database
         :param pulumi.Input[str] region: region of the database. Possible values are: "global", "eu-west-1", "us-east-1", "us-west-1", "ap-northeast-1" ,
                "eu-central1"
+        :param pulumi.Input[bool] auto_scale: Upgrade to higher plans automatically when it hits quotas
         :param pulumi.Input[bool] consistent: When enabled, all writes are synchronously persisted to the disk.
+        :param pulumi.Input[bool] eviction: Enable eviction, to evict keys when your database reaches the max size
         :param pulumi.Input[bool] multizone: When enabled, database becomes highly available and is deployed in multiple zones. (If changed to false from true,
                results in deletion and recreation of the resource)
+        :param pulumi.Input[str] primary_region: Primary region for the database (Only works if region='global'. Can be one of [us-east-1, us-west-1, us-west-2,
+               eu-central-1, eu-west-1, sa-east-1, ap-southeast-1, ap-southeast-2])
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] read_regions: Read regions for the database (Only works if region='global' and primary_region is set. Can be any combination of
+               [us-east-1, us-west-1, us-west-2, eu-central-1, eu-west-1, sa-east-1, ap-southeast-1, ap-southeast-2], excluding the one
+               given as primary.)
         :param pulumi.Input[bool] tls: When enabled, data is encrypted in transit. (If changed to false from true, results in deletion and recreation of the
                resource)
         """
         pulumi.set(__self__, "database_name", database_name)
         pulumi.set(__self__, "region", region)
+        if auto_scale is not None:
+            pulumi.set(__self__, "auto_scale", auto_scale)
         if consistent is not None:
             warnings.warn("""Consistent option is deprecated.""", DeprecationWarning)
             pulumi.log.warn("""consistent is deprecated: Consistent option is deprecated.""")
         if consistent is not None:
             pulumi.set(__self__, "consistent", consistent)
+        if eviction is not None:
+            pulumi.set(__self__, "eviction", eviction)
+        if multizone is not None:
+            warnings.warn("""Multizone option is deprecated. It is enabled by default for paid databases.""", DeprecationWarning)
+            pulumi.log.warn("""multizone is deprecated: Multizone option is deprecated. It is enabled by default for paid databases.""")
         if multizone is not None:
             pulumi.set(__self__, "multizone", multizone)
+        if primary_region is not None:
+            pulumi.set(__self__, "primary_region", primary_region)
+        if read_regions is not None:
+            pulumi.set(__self__, "read_regions", read_regions)
         if tls is not None:
             pulumi.set(__self__, "tls", tls)
 
     @property
     @pulumi.getter(name="databaseName")
     def database_name(self) -> pulumi.Input[str]:
         """
@@ -63,39 +85,90 @@
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: pulumi.Input[str]):
         pulumi.set(self, "region", value)
 
     @property
+    @pulumi.getter(name="autoScale")
+    def auto_scale(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Upgrade to higher plans automatically when it hits quotas
+        """
+        return pulumi.get(self, "auto_scale")
+
+    @auto_scale.setter
+    def auto_scale(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "auto_scale", value)
+
+    @property
     @pulumi.getter
     def consistent(self) -> Optional[pulumi.Input[bool]]:
         """
         When enabled, all writes are synchronously persisted to the disk.
         """
         return pulumi.get(self, "consistent")
 
     @consistent.setter
     def consistent(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "consistent", value)
 
     @property
     @pulumi.getter
+    def eviction(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Enable eviction, to evict keys when your database reaches the max size
+        """
+        return pulumi.get(self, "eviction")
+
+    @eviction.setter
+    def eviction(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "eviction", value)
+
+    @property
+    @pulumi.getter
     def multizone(self) -> Optional[pulumi.Input[bool]]:
         """
         When enabled, database becomes highly available and is deployed in multiple zones. (If changed to false from true,
         results in deletion and recreation of the resource)
         """
         return pulumi.get(self, "multizone")
 
     @multizone.setter
     def multizone(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "multizone", value)
 
     @property
+    @pulumi.getter(name="primaryRegion")
+    def primary_region(self) -> Optional[pulumi.Input[str]]:
+        """
+        Primary region for the database (Only works if region='global'. Can be one of [us-east-1, us-west-1, us-west-2,
+        eu-central-1, eu-west-1, sa-east-1, ap-southeast-1, ap-southeast-2])
+        """
+        return pulumi.get(self, "primary_region")
+
+    @primary_region.setter
+    def primary_region(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "primary_region", value)
+
+    @property
+    @pulumi.getter(name="readRegions")
+    def read_regions(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Read regions for the database (Only works if region='global' and primary_region is set. Can be any combination of
+        [us-east-1, us-west-1, us-west-2, eu-central-1, eu-west-1, sa-east-1, ap-southeast-1, ap-southeast-2], excluding the one
+        given as primary.)
+        """
+        return pulumi.get(self, "read_regions")
+
+    @read_regions.setter
+    def read_regions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "read_regions", value)
+
+    @property
     @pulumi.getter
     def tls(self) -> Optional[pulumi.Input[bool]]:
         """
         When enabled, data is encrypted in transit. (If changed to false from true, results in deletion and recreation of the
         resource)
         """
         return pulumi.get(self, "tls")
@@ -104,64 +177,77 @@
     def tls(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "tls", value)
 
 
 @pulumi.input_type
 class _RedisDatabaseState:
     def __init__(__self__, *,
+                 auto_scale: Optional[pulumi.Input[bool]] = None,
                  consistent: Optional[pulumi.Input[bool]] = None,
                  creation_time: Optional[pulumi.Input[int]] = None,
                  database_id: Optional[pulumi.Input[str]] = None,
                  database_name: Optional[pulumi.Input[str]] = None,
                  database_type: Optional[pulumi.Input[str]] = None,
                  db_daily_bandwidth_limit: Optional[pulumi.Input[int]] = None,
                  db_disk_threshold: Optional[pulumi.Input[int]] = None,
                  db_max_clients: Optional[pulumi.Input[int]] = None,
                  db_max_commands_per_second: Optional[pulumi.Input[int]] = None,
                  db_max_entry_size: Optional[pulumi.Input[int]] = None,
                  db_max_request_size: Optional[pulumi.Input[int]] = None,
                  db_memory_threshold: Optional[pulumi.Input[int]] = None,
                  endpoint: Optional[pulumi.Input[str]] = None,
+                 eviction: Optional[pulumi.Input[bool]] = None,
                  multizone: Optional[pulumi.Input[bool]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  port: Optional[pulumi.Input[int]] = None,
+                 primary_region: Optional[pulumi.Input[str]] = None,
                  read_only_rest_token: Optional[pulumi.Input[str]] = None,
+                 read_regions: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  rest_token: Optional[pulumi.Input[str]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  tls: Optional[pulumi.Input[bool]] = None,
                  user_email: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering RedisDatabase resources.
+        :param pulumi.Input[bool] auto_scale: Upgrade to higher plans automatically when it hits quotas
         :param pulumi.Input[bool] consistent: When enabled, all writes are synchronously persisted to the disk.
         :param pulumi.Input[int] creation_time: Creation time of the database
         :param pulumi.Input[str] database_id: Unique Database ID for created database
         :param pulumi.Input[str] database_name: Name of the database
         :param pulumi.Input[str] database_type: Type of the database
         :param pulumi.Input[int] db_daily_bandwidth_limit: Daily bandwidth limit for the database
         :param pulumi.Input[int] db_disk_threshold: Disk threshold for the database
         :param pulumi.Input[int] db_max_clients: Max clients for the database
         :param pulumi.Input[int] db_max_commands_per_second: Max commands per second for the database
         :param pulumi.Input[int] db_max_entry_size: Max entry size for the database
         :param pulumi.Input[int] db_max_request_size: Max request size for the database
         :param pulumi.Input[int] db_memory_threshold: Memory threshold for the database
         :param pulumi.Input[str] endpoint: Database URL for connection
+        :param pulumi.Input[bool] eviction: Enable eviction, to evict keys when your database reaches the max size
         :param pulumi.Input[bool] multizone: When enabled, database becomes highly available and is deployed in multiple zones. (If changed to false from true,
                results in deletion and recreation of the resource)
         :param pulumi.Input[str] password: Password of the database
         :param pulumi.Input[int] port: Port of the endpoint
+        :param pulumi.Input[str] primary_region: Primary region for the database (Only works if region='global'. Can be one of [us-east-1, us-west-1, us-west-2,
+               eu-central-1, eu-west-1, sa-east-1, ap-southeast-1, ap-southeast-2])
         :param pulumi.Input[str] read_only_rest_token: Rest Token for the database.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] read_regions: Read regions for the database (Only works if region='global' and primary_region is set. Can be any combination of
+               [us-east-1, us-west-1, us-west-2, eu-central-1, eu-west-1, sa-east-1, ap-southeast-1, ap-southeast-2], excluding the one
+               given as primary.)
         :param pulumi.Input[str] region: region of the database. Possible values are: "global", "eu-west-1", "us-east-1", "us-west-1", "ap-northeast-1" ,
                "eu-central1"
         :param pulumi.Input[str] rest_token: Rest Token for the database.
         :param pulumi.Input[str] state: State of the database
         :param pulumi.Input[bool] tls: When enabled, data is encrypted in transit. (If changed to false from true, results in deletion and recreation of the
                resource)
         :param pulumi.Input[str] user_email: User email for the database
         """
+        if auto_scale is not None:
+            pulumi.set(__self__, "auto_scale", auto_scale)
         if consistent is not None:
             warnings.warn("""Consistent option is deprecated.""", DeprecationWarning)
             pulumi.log.warn("""consistent is deprecated: Consistent option is deprecated.""")
         if consistent is not None:
             pulumi.set(__self__, "consistent", consistent)
         if creation_time is not None:
             pulumi.set(__self__, "creation_time", creation_time)
@@ -183,34 +269,55 @@
             pulumi.set(__self__, "db_max_entry_size", db_max_entry_size)
         if db_max_request_size is not None:
             pulumi.set(__self__, "db_max_request_size", db_max_request_size)
         if db_memory_threshold is not None:
             pulumi.set(__self__, "db_memory_threshold", db_memory_threshold)
         if endpoint is not None:
             pulumi.set(__self__, "endpoint", endpoint)
+        if eviction is not None:
+            pulumi.set(__self__, "eviction", eviction)
+        if multizone is not None:
+            warnings.warn("""Multizone option is deprecated. It is enabled by default for paid databases.""", DeprecationWarning)
+            pulumi.log.warn("""multizone is deprecated: Multizone option is deprecated. It is enabled by default for paid databases.""")
         if multizone is not None:
             pulumi.set(__self__, "multizone", multizone)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
+        if primary_region is not None:
+            pulumi.set(__self__, "primary_region", primary_region)
         if read_only_rest_token is not None:
             pulumi.set(__self__, "read_only_rest_token", read_only_rest_token)
+        if read_regions is not None:
+            pulumi.set(__self__, "read_regions", read_regions)
         if region is not None:
             pulumi.set(__self__, "region", region)
         if rest_token is not None:
             pulumi.set(__self__, "rest_token", rest_token)
         if state is not None:
             pulumi.set(__self__, "state", state)
         if tls is not None:
             pulumi.set(__self__, "tls", tls)
         if user_email is not None:
             pulumi.set(__self__, "user_email", user_email)
 
     @property
+    @pulumi.getter(name="autoScale")
+    def auto_scale(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Upgrade to higher plans automatically when it hits quotas
+        """
+        return pulumi.get(self, "auto_scale")
+
+    @auto_scale.setter
+    def auto_scale(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "auto_scale", value)
+
+    @property
     @pulumi.getter
     def consistent(self) -> Optional[pulumi.Input[bool]]:
         """
         When enabled, all writes are synchronously persisted to the disk.
         """
         return pulumi.get(self, "consistent")
 
@@ -360,14 +467,26 @@
 
     @endpoint.setter
     def endpoint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "endpoint", value)
 
     @property
     @pulumi.getter
+    def eviction(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Enable eviction, to evict keys when your database reaches the max size
+        """
+        return pulumi.get(self, "eviction")
+
+    @eviction.setter
+    def eviction(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "eviction", value)
+
+    @property
+    @pulumi.getter
     def multizone(self) -> Optional[pulumi.Input[bool]]:
         """
         When enabled, database becomes highly available and is deployed in multiple zones. (If changed to false from true,
         results in deletion and recreation of the resource)
         """
         return pulumi.get(self, "multizone")
 
@@ -396,26 +515,53 @@
         return pulumi.get(self, "port")
 
     @port.setter
     def port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "port", value)
 
     @property
+    @pulumi.getter(name="primaryRegion")
+    def primary_region(self) -> Optional[pulumi.Input[str]]:
+        """
+        Primary region for the database (Only works if region='global'. Can be one of [us-east-1, us-west-1, us-west-2,
+        eu-central-1, eu-west-1, sa-east-1, ap-southeast-1, ap-southeast-2])
+        """
+        return pulumi.get(self, "primary_region")
+
+    @primary_region.setter
+    def primary_region(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "primary_region", value)
+
+    @property
     @pulumi.getter(name="readOnlyRestToken")
     def read_only_rest_token(self) -> Optional[pulumi.Input[str]]:
         """
         Rest Token for the database.
         """
         return pulumi.get(self, "read_only_rest_token")
 
     @read_only_rest_token.setter
     def read_only_rest_token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "read_only_rest_token", value)
 
     @property
+    @pulumi.getter(name="readRegions")
+    def read_regions(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Read regions for the database (Only works if region='global' and primary_region is set. Can be any combination of
+        [us-east-1, us-west-1, us-west-2, eu-central-1, eu-west-1, sa-east-1, ap-southeast-1, ap-southeast-2], excluding the one
+        given as primary.)
+        """
+        return pulumi.get(self, "read_regions")
+
+    @read_regions.setter
+    def read_regions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "read_regions", value)
+
+    @property
     @pulumi.getter
     def region(self) -> Optional[pulumi.Input[str]]:
         """
         region of the database. Possible values are: "global", "eu-west-1", "us-east-1", "us-west-1", "ap-northeast-1" ,
         "eu-central1"
         """
         return pulumi.get(self, "region")
@@ -475,17 +621,21 @@
 
 
 class RedisDatabase(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 auto_scale: Optional[pulumi.Input[bool]] = None,
                  consistent: Optional[pulumi.Input[bool]] = None,
                  database_name: Optional[pulumi.Input[str]] = None,
+                 eviction: Optional[pulumi.Input[bool]] = None,
                  multizone: Optional[pulumi.Input[bool]] = None,
+                 primary_region: Optional[pulumi.Input[str]] = None,
+                 read_regions: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tls: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         ## Example Usage
 
         ```python
@@ -497,18 +647,25 @@
             multizone=True,
             region="eu-west-1",
             tls=True)
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[bool] auto_scale: Upgrade to higher plans automatically when it hits quotas
         :param pulumi.Input[bool] consistent: When enabled, all writes are synchronously persisted to the disk.
         :param pulumi.Input[str] database_name: Name of the database
+        :param pulumi.Input[bool] eviction: Enable eviction, to evict keys when your database reaches the max size
         :param pulumi.Input[bool] multizone: When enabled, database becomes highly available and is deployed in multiple zones. (If changed to false from true,
                results in deletion and recreation of the resource)
+        :param pulumi.Input[str] primary_region: Primary region for the database (Only works if region='global'. Can be one of [us-east-1, us-west-1, us-west-2,
+               eu-central-1, eu-west-1, sa-east-1, ap-southeast-1, ap-southeast-2])
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] read_regions: Read regions for the database (Only works if region='global' and primary_region is set. Can be any combination of
+               [us-east-1, us-west-1, us-west-2, eu-central-1, eu-west-1, sa-east-1, ap-southeast-1, ap-southeast-2], excluding the one
+               given as primary.)
         :param pulumi.Input[str] region: region of the database. Possible values are: "global", "eu-west-1", "us-east-1", "us-west-1", "ap-northeast-1" ,
                "eu-central1"
         :param pulumi.Input[bool] tls: When enabled, data is encrypted in transit. (If changed to false from true, results in deletion and recreation of the
                resource)
         """
         ...
     @overload
@@ -541,17 +698,21 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 auto_scale: Optional[pulumi.Input[bool]] = None,
                  consistent: Optional[pulumi.Input[bool]] = None,
                  database_name: Optional[pulumi.Input[str]] = None,
+                 eviction: Optional[pulumi.Input[bool]] = None,
                  multizone: Optional[pulumi.Input[bool]] = None,
+                 primary_region: Optional[pulumi.Input[str]] = None,
+                 read_regions: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tls: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
@@ -560,22 +721,29 @@
         if opts.plugin_download_url is None:
             opts.plugin_download_url = _utilities.get_plugin_download_url()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RedisDatabaseArgs.__new__(RedisDatabaseArgs)
 
+            __props__.__dict__["auto_scale"] = auto_scale
             if consistent is not None and not opts.urn:
                 warnings.warn("""Consistent option is deprecated.""", DeprecationWarning)
                 pulumi.log.warn("""consistent is deprecated: Consistent option is deprecated.""")
             __props__.__dict__["consistent"] = consistent
             if database_name is None and not opts.urn:
                 raise TypeError("Missing required property 'database_name'")
             __props__.__dict__["database_name"] = database_name
+            __props__.__dict__["eviction"] = eviction
+            if multizone is not None and not opts.urn:
+                warnings.warn("""Multizone option is deprecated. It is enabled by default for paid databases.""", DeprecationWarning)
+                pulumi.log.warn("""multizone is deprecated: Multizone option is deprecated. It is enabled by default for paid databases.""")
             __props__.__dict__["multizone"] = multizone
+            __props__.__dict__["primary_region"] = primary_region
+            __props__.__dict__["read_regions"] = read_regions
             if region is None and not opts.urn:
                 raise TypeError("Missing required property 'region'")
             __props__.__dict__["region"] = region
             __props__.__dict__["tls"] = tls
             __props__.__dict__["creation_time"] = None
             __props__.__dict__["database_id"] = None
             __props__.__dict__["database_type"] = None
@@ -601,98 +769,121 @@
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
+            auto_scale: Optional[pulumi.Input[bool]] = None,
             consistent: Optional[pulumi.Input[bool]] = None,
             creation_time: Optional[pulumi.Input[int]] = None,
             database_id: Optional[pulumi.Input[str]] = None,
             database_name: Optional[pulumi.Input[str]] = None,
             database_type: Optional[pulumi.Input[str]] = None,
             db_daily_bandwidth_limit: Optional[pulumi.Input[int]] = None,
             db_disk_threshold: Optional[pulumi.Input[int]] = None,
             db_max_clients: Optional[pulumi.Input[int]] = None,
             db_max_commands_per_second: Optional[pulumi.Input[int]] = None,
             db_max_entry_size: Optional[pulumi.Input[int]] = None,
             db_max_request_size: Optional[pulumi.Input[int]] = None,
             db_memory_threshold: Optional[pulumi.Input[int]] = None,
             endpoint: Optional[pulumi.Input[str]] = None,
+            eviction: Optional[pulumi.Input[bool]] = None,
             multizone: Optional[pulumi.Input[bool]] = None,
             password: Optional[pulumi.Input[str]] = None,
             port: Optional[pulumi.Input[int]] = None,
+            primary_region: Optional[pulumi.Input[str]] = None,
             read_only_rest_token: Optional[pulumi.Input[str]] = None,
+            read_regions: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             region: Optional[pulumi.Input[str]] = None,
             rest_token: Optional[pulumi.Input[str]] = None,
             state: Optional[pulumi.Input[str]] = None,
             tls: Optional[pulumi.Input[bool]] = None,
             user_email: Optional[pulumi.Input[str]] = None) -> 'RedisDatabase':
         """
         Get an existing RedisDatabase resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[bool] auto_scale: Upgrade to higher plans automatically when it hits quotas
         :param pulumi.Input[bool] consistent: When enabled, all writes are synchronously persisted to the disk.
         :param pulumi.Input[int] creation_time: Creation time of the database
         :param pulumi.Input[str] database_id: Unique Database ID for created database
         :param pulumi.Input[str] database_name: Name of the database
         :param pulumi.Input[str] database_type: Type of the database
         :param pulumi.Input[int] db_daily_bandwidth_limit: Daily bandwidth limit for the database
         :param pulumi.Input[int] db_disk_threshold: Disk threshold for the database
         :param pulumi.Input[int] db_max_clients: Max clients for the database
         :param pulumi.Input[int] db_max_commands_per_second: Max commands per second for the database
         :param pulumi.Input[int] db_max_entry_size: Max entry size for the database
         :param pulumi.Input[int] db_max_request_size: Max request size for the database
         :param pulumi.Input[int] db_memory_threshold: Memory threshold for the database
         :param pulumi.Input[str] endpoint: Database URL for connection
+        :param pulumi.Input[bool] eviction: Enable eviction, to evict keys when your database reaches the max size
         :param pulumi.Input[bool] multizone: When enabled, database becomes highly available and is deployed in multiple zones. (If changed to false from true,
                results in deletion and recreation of the resource)
         :param pulumi.Input[str] password: Password of the database
         :param pulumi.Input[int] port: Port of the endpoint
+        :param pulumi.Input[str] primary_region: Primary region for the database (Only works if region='global'. Can be one of [us-east-1, us-west-1, us-west-2,
+               eu-central-1, eu-west-1, sa-east-1, ap-southeast-1, ap-southeast-2])
         :param pulumi.Input[str] read_only_rest_token: Rest Token for the database.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] read_regions: Read regions for the database (Only works if region='global' and primary_region is set. Can be any combination of
+               [us-east-1, us-west-1, us-west-2, eu-central-1, eu-west-1, sa-east-1, ap-southeast-1, ap-southeast-2], excluding the one
+               given as primary.)
         :param pulumi.Input[str] region: region of the database. Possible values are: "global", "eu-west-1", "us-east-1", "us-west-1", "ap-northeast-1" ,
                "eu-central1"
         :param pulumi.Input[str] rest_token: Rest Token for the database.
         :param pulumi.Input[str] state: State of the database
         :param pulumi.Input[bool] tls: When enabled, data is encrypted in transit. (If changed to false from true, results in deletion and recreation of the
                resource)
         :param pulumi.Input[str] user_email: User email for the database
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _RedisDatabaseState.__new__(_RedisDatabaseState)
 
+        __props__.__dict__["auto_scale"] = auto_scale
         __props__.__dict__["consistent"] = consistent
         __props__.__dict__["creation_time"] = creation_time
         __props__.__dict__["database_id"] = database_id
         __props__.__dict__["database_name"] = database_name
         __props__.__dict__["database_type"] = database_type
         __props__.__dict__["db_daily_bandwidth_limit"] = db_daily_bandwidth_limit
         __props__.__dict__["db_disk_threshold"] = db_disk_threshold
         __props__.__dict__["db_max_clients"] = db_max_clients
         __props__.__dict__["db_max_commands_per_second"] = db_max_commands_per_second
         __props__.__dict__["db_max_entry_size"] = db_max_entry_size
         __props__.__dict__["db_max_request_size"] = db_max_request_size
         __props__.__dict__["db_memory_threshold"] = db_memory_threshold
         __props__.__dict__["endpoint"] = endpoint
+        __props__.__dict__["eviction"] = eviction
         __props__.__dict__["multizone"] = multizone
         __props__.__dict__["password"] = password
         __props__.__dict__["port"] = port
+        __props__.__dict__["primary_region"] = primary_region
         __props__.__dict__["read_only_rest_token"] = read_only_rest_token
+        __props__.__dict__["read_regions"] = read_regions
         __props__.__dict__["region"] = region
         __props__.__dict__["rest_token"] = rest_token
         __props__.__dict__["state"] = state
         __props__.__dict__["tls"] = tls
         __props__.__dict__["user_email"] = user_email
         return RedisDatabase(resource_name, opts=opts, __props__=__props__)
 
     @property
+    @pulumi.getter(name="autoScale")
+    def auto_scale(self) -> pulumi.Output[Optional[bool]]:
+        """
+        Upgrade to higher plans automatically when it hits quotas
+        """
+        return pulumi.get(self, "auto_scale")
+
+    @property
     @pulumi.getter
     def consistent(self) -> pulumi.Output[Optional[bool]]:
         """
         When enabled, all writes are synchronously persisted to the disk.
         """
         return pulumi.get(self, "consistent")
 
@@ -790,14 +981,22 @@
         """
         Database URL for connection
         """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter
+    def eviction(self) -> pulumi.Output[Optional[bool]]:
+        """
+        Enable eviction, to evict keys when your database reaches the max size
+        """
+        return pulumi.get(self, "eviction")
+
+    @property
+    @pulumi.getter
     def multizone(self) -> pulumi.Output[Optional[bool]]:
         """
         When enabled, database becomes highly available and is deployed in multiple zones. (If changed to false from true,
         results in deletion and recreation of the resource)
         """
         return pulumi.get(self, "multizone")
 
@@ -814,22 +1013,41 @@
     def port(self) -> pulumi.Output[int]:
         """
         Port of the endpoint
         """
         return pulumi.get(self, "port")
 
     @property
+    @pulumi.getter(name="primaryRegion")
+    def primary_region(self) -> pulumi.Output[Optional[str]]:
+        """
+        Primary region for the database (Only works if region='global'. Can be one of [us-east-1, us-west-1, us-west-2,
+        eu-central-1, eu-west-1, sa-east-1, ap-southeast-1, ap-southeast-2])
+        """
+        return pulumi.get(self, "primary_region")
+
+    @property
     @pulumi.getter(name="readOnlyRestToken")
     def read_only_rest_token(self) -> pulumi.Output[str]:
         """
         Rest Token for the database.
         """
         return pulumi.get(self, "read_only_rest_token")
 
     @property
+    @pulumi.getter(name="readRegions")
+    def read_regions(self) -> pulumi.Output[Optional[Sequence[str]]]:
+        """
+        Read regions for the database (Only works if region='global' and primary_region is set. Can be any combination of
+        [us-east-1, us-west-1, us-west-2, eu-central-1, eu-west-1, sa-east-1, ap-southeast-1, ap-southeast-2], excluding the one
+        given as primary.)
+        """
+        return pulumi.get(self, "read_regions")
+
+    @property
     @pulumi.getter
     def region(self) -> pulumi.Output[str]:
         """
         region of the database. Possible values are: "global", "eu-west-1", "us-east-1", "us-west-1", "ap-northeast-1" ,
         "eu-central1"
         """
         return pulumi.get(self, "region")
```

### Comparing `upstash_pulumi-0.1.2/upstash_pulumi/team.py` & `upstash_pulumi-0.2.0/upstash_pulumi/team.py`

 * *Files identical despite different names*

### Comparing `upstash_pulumi-0.1.2/upstash_pulumi.egg-info/PKG-INFO` & `upstash_pulumi-0.2.0/upstash_pulumi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upstash-pulumi
-Version: 0.1.2
+Version: 0.2.0
 Summary: A Pulumi package for creating and managing upstash cloud resources.
 Home-page: https://www.upstash.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/upstash/pulumi-upstash
 Keywords: pulumi upstash category/cloud
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `upstash_pulumi-0.1.2/upstash_pulumi.egg-info/SOURCES.txt` & `upstash_pulumi-0.2.0/upstash_pulumi.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 README.md
 setup.py
 upstash_pulumi/__init__.py
 upstash_pulumi/_utilities.py
 upstash_pulumi/get_kafka_cluster.py
+upstash_pulumi/get_kafka_connector.py
 upstash_pulumi/get_kafka_credential.py
 upstash_pulumi/get_kafka_topic.py
 upstash_pulumi/get_q_stash_endpoint.py
 upstash_pulumi/get_q_stash_schedule.py
 upstash_pulumi/get_q_stash_topic.py
 upstash_pulumi/get_redis_database.py
 upstash_pulumi/get_team.py
 upstash_pulumi/kafka_cluster.py
+upstash_pulumi/kafka_connector.py
 upstash_pulumi/kafka_credential.py
 upstash_pulumi/kafka_topic.py
 upstash_pulumi/provider.py
 upstash_pulumi/pulumi-plugin.json
 upstash_pulumi/py.typed
 upstash_pulumi/q_stash_endpoint.py
 upstash_pulumi/q_stash_schedule.py
```

