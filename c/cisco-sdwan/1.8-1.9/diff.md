# Comparing `tmp/cisco-sdwan-1.8.tar.gz` & `tmp/cisco-sdwan-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cisco-sdwan-1.8.tar", last modified: Fri Oct  9 19:31:48 2020, max compression
+gzip compressed data, was "dist/cisco-sdwan-1.9.tar", last modified: Wed Oct 14 02:34:58 2020, max compression
```

## Comparing `cisco-sdwan-1.8.tar` & `cisco-sdwan-1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 mareis     (502) staff       (20)        0 2020-10-09 19:31:48.096962 cisco-sdwan-1.8/
--rw-r--r--   0 mareis     (502) staff       (20)    49488 2020-10-09 19:31:48.096644 cisco-sdwan-1.8/PKG-INFO
--rw-r--r--   0 mareis     (502) staff       (20)    43092 2020-10-09 19:23:34.000000 cisco-sdwan-1.8/README.md
-drwxr-xr-x   0 mareis     (502) staff       (20)        0 2020-10-09 19:31:48.082896 cisco-sdwan-1.8/cisco_sdwan/
--rw-r--r--   0 mareis     (502) staff       (20)      155 2019-12-05 17:59:52.000000 cisco-sdwan-1.8/cisco_sdwan/__init__.py
--rw-r--r--   0 mareis     (502) staff       (20)      314 2020-10-09 18:50:54.000000 cisco-sdwan-1.8/cisco_sdwan/__version__.py
-drwxr-xr-x   0 mareis     (502) staff       (20)        0 2020-10-09 19:31:48.089718 cisco-sdwan-1.8/cisco_sdwan/base/
--rw-r--r--   0 mareis     (502) staff       (20)        0 2019-05-20 15:35:05.000000 cisco-sdwan-1.8/cisco_sdwan/base/__init__.py
--rw-r--r--   0 mareis     (502) staff       (20)     8455 2020-09-02 05:17:14.000000 cisco-sdwan-1.8/cisco_sdwan/base/catalog.py
--rw-r--r--   0 mareis     (502) staff       (20)    24290 2020-09-03 03:51:45.000000 cisco-sdwan-1.8/cisco_sdwan/base/models_base.py
--rw-r--r--   0 mareis     (502) staff       (20)    50142 2020-10-09 18:28:56.000000 cisco-sdwan-1.8/cisco_sdwan/base/models_vmanage.py
--rw-r--r--   0 mareis     (502) staff       (20)     2825 2020-06-22 22:40:33.000000 cisco-sdwan-1.8/cisco_sdwan/base/processor.py
--rw-r--r--   0 mareis     (502) staff       (20)     5529 2020-08-12 18:25:49.000000 cisco-sdwan-1.8/cisco_sdwan/base/rest_api.py
--rw-r--r--   0 mareis     (502) staff       (20)     6293 2020-10-09 18:29:54.000000 cisco-sdwan-1.8/cisco_sdwan/cmd.py
-drwxr-xr-x   0 mareis     (502) staff       (20)        0 2020-10-09 19:31:48.092470 cisco-sdwan-1.8/cisco_sdwan/migration/
--rw-r--r--   0 mareis     (502) staff       (20)     1057 2020-06-22 22:40:33.000000 cisco-sdwan-1.8/cisco_sdwan/migration/__init__.py
--rw-r--r--   0 mareis     (502) staff       (20)     6621 2020-06-22 22:40:33.000000 cisco-sdwan-1.8/cisco_sdwan/migration/device_migration.py
--rw-r--r--   0 mareis     (502) staff       (20)     1529 2020-06-22 22:40:33.000000 cisco-sdwan-1.8/cisco_sdwan/migration/device_template_recipes.json
--rw-r--r--   0 mareis     (502) staff       (20)     9086 2020-06-22 22:40:33.000000 cisco-sdwan-1.8/cisco_sdwan/migration/feature_migration.py
--rw-r--r--   0 mareis     (502) staff       (20)    34075 2020-06-22 22:40:33.000000 cisco-sdwan-1.8/cisco_sdwan/migration/feature_template_recipes.json
-drwxr-xr-x   0 mareis     (502) staff       (20)        0 2020-10-09 19:31:48.093570 cisco-sdwan-1.8/cisco_sdwan/migration/feature_templates/
--rw-r--r--   0 mareis     (502) staff       (20)     5992 2020-06-22 22:40:33.000000 cisco-sdwan-1.8/cisco_sdwan/migration/feature_templates/Factory_Default_AAA_CISCO_Template.json
--rw-r--r--   0 mareis     (502) staff       (20)     3130 2020-06-22 22:40:33.000000 cisco-sdwan-1.8/cisco_sdwan/migration/feature_templates/Factory_Default_Global_CISCO_Template.json
-drwxr-xr-x   0 mareis     (502) staff       (20)        0 2020-10-09 19:31:48.095733 cisco-sdwan-1.8/cisco_sdwan/tasks/
--rw-r--r--   0 mareis     (502) staff       (20)        0 2019-12-04 22:25:08.000000 cisco-sdwan-1.8/cisco_sdwan/tasks/__init__.py
--rw-r--r--   0 mareis     (502) staff       (20)    20018 2020-10-09 18:17:27.000000 cisco-sdwan-1.8/cisco_sdwan/tasks/common.py
--rw-r--r--   0 mareis     (502) staff       (20)    36034 2020-10-09 19:00:47.000000 cisco-sdwan-1.8/cisco_sdwan/tasks/implementation.py
--rw-r--r--   0 mareis     (502) staff       (20)     6858 2020-10-09 18:28:56.000000 cisco-sdwan-1.8/cisco_sdwan/tasks/utils.py
-drwxr-xr-x   0 mareis     (502) staff       (20)        0 2020-10-09 19:31:48.085440 cisco-sdwan-1.8/cisco_sdwan.egg-info/
--rw-r--r--   0 mareis     (502) staff       (20)    49488 2020-10-09 19:31:47.000000 cisco-sdwan-1.8/cisco_sdwan.egg-info/PKG-INFO
--rw-r--r--   0 mareis     (502) staff       (20)      989 2020-10-09 19:31:47.000000 cisco-sdwan-1.8/cisco_sdwan.egg-info/SOURCES.txt
--rw-r--r--   0 mareis     (502) staff       (20)        1 2020-10-09 19:31:47.000000 cisco-sdwan-1.8/cisco_sdwan.egg-info/dependency_links.txt
--rw-r--r--   0 mareis     (502) staff       (20)       78 2020-10-09 19:31:47.000000 cisco-sdwan-1.8/cisco_sdwan.egg-info/entry_points.txt
--rw-r--r--   0 mareis     (502) staff       (20)        9 2020-10-09 19:31:47.000000 cisco-sdwan-1.8/cisco_sdwan.egg-info/requires.txt
--rw-r--r--   0 mareis     (502) staff       (20)       12 2020-10-09 19:31:47.000000 cisco-sdwan-1.8/cisco_sdwan.egg-info/top_level.txt
--rw-r--r--   0 mareis     (502) staff       (20)       38 2020-10-09 19:31:48.097100 cisco-sdwan-1.8/setup.cfg
--rw-r--r--   0 mareis     (502) staff       (20)     1038 2020-06-23 00:58:46.000000 cisco-sdwan-1.8/setup.py
+drwxr-xr-x   0 mareis     (502) staff       (20)        0 2020-10-14 02:34:58.549413 cisco-sdwan-1.9/
+-rw-r--r--   0 mareis     (502) staff       (20)    49488 2020-10-14 02:34:58.549162 cisco-sdwan-1.9/PKG-INFO
+-rw-r--r--   0 mareis     (502) staff       (20)    43092 2020-10-09 19:23:34.000000 cisco-sdwan-1.9/README.md
+drwxr-xr-x   0 mareis     (502) staff       (20)        0 2020-10-14 02:34:58.537938 cisco-sdwan-1.9/cisco_sdwan/
+-rw-r--r--   0 mareis     (502) staff       (20)      155 2019-12-05 17:59:52.000000 cisco-sdwan-1.9/cisco_sdwan/__init__.py
+-rw-r--r--   0 mareis     (502) staff       (20)      314 2020-10-14 02:28:30.000000 cisco-sdwan-1.9/cisco_sdwan/__version__.py
+drwxr-xr-x   0 mareis     (502) staff       (20)        0 2020-10-14 02:34:58.543041 cisco-sdwan-1.9/cisco_sdwan/base/
+-rw-r--r--   0 mareis     (502) staff       (20)        0 2019-05-20 15:35:05.000000 cisco-sdwan-1.9/cisco_sdwan/base/__init__.py
+-rw-r--r--   0 mareis     (502) staff       (20)     8455 2020-09-02 05:17:14.000000 cisco-sdwan-1.9/cisco_sdwan/base/catalog.py
+-rw-r--r--   0 mareis     (502) staff       (20)    24290 2020-09-03 03:51:45.000000 cisco-sdwan-1.9/cisco_sdwan/base/models_base.py
+-rw-r--r--   0 mareis     (502) staff       (20)    50596 2020-10-14 02:28:30.000000 cisco-sdwan-1.9/cisco_sdwan/base/models_vmanage.py
+-rw-r--r--   0 mareis     (502) staff       (20)     2825 2020-06-22 22:40:33.000000 cisco-sdwan-1.9/cisco_sdwan/base/processor.py
+-rw-r--r--   0 mareis     (502) staff       (20)     5529 2020-08-12 18:25:49.000000 cisco-sdwan-1.9/cisco_sdwan/base/rest_api.py
+-rw-r--r--   0 mareis     (502) staff       (20)     6293 2020-10-09 18:29:54.000000 cisco-sdwan-1.9/cisco_sdwan/cmd.py
+drwxr-xr-x   0 mareis     (502) staff       (20)        0 2020-10-14 02:34:58.545264 cisco-sdwan-1.9/cisco_sdwan/migration/
+-rw-r--r--   0 mareis     (502) staff       (20)     1057 2020-06-22 22:40:33.000000 cisco-sdwan-1.9/cisco_sdwan/migration/__init__.py
+-rw-r--r--   0 mareis     (502) staff       (20)     6621 2020-06-22 22:40:33.000000 cisco-sdwan-1.9/cisco_sdwan/migration/device_migration.py
+-rw-r--r--   0 mareis     (502) staff       (20)     1529 2020-06-22 22:40:33.000000 cisco-sdwan-1.9/cisco_sdwan/migration/device_template_recipes.json
+-rw-r--r--   0 mareis     (502) staff       (20)     9086 2020-06-22 22:40:33.000000 cisco-sdwan-1.9/cisco_sdwan/migration/feature_migration.py
+-rw-r--r--   0 mareis     (502) staff       (20)    34075 2020-06-22 22:40:33.000000 cisco-sdwan-1.9/cisco_sdwan/migration/feature_template_recipes.json
+drwxr-xr-x   0 mareis     (502) staff       (20)        0 2020-10-14 02:34:58.546217 cisco-sdwan-1.9/cisco_sdwan/migration/feature_templates/
+-rw-r--r--   0 mareis     (502) staff       (20)     5992 2020-06-22 22:40:33.000000 cisco-sdwan-1.9/cisco_sdwan/migration/feature_templates/Factory_Default_AAA_CISCO_Template.json
+-rw-r--r--   0 mareis     (502) staff       (20)     3130 2020-06-22 22:40:33.000000 cisco-sdwan-1.9/cisco_sdwan/migration/feature_templates/Factory_Default_Global_CISCO_Template.json
+drwxr-xr-x   0 mareis     (502) staff       (20)        0 2020-10-14 02:34:58.548255 cisco-sdwan-1.9/cisco_sdwan/tasks/
+-rw-r--r--   0 mareis     (502) staff       (20)        0 2019-12-04 22:25:08.000000 cisco-sdwan-1.9/cisco_sdwan/tasks/__init__.py
+-rw-r--r--   0 mareis     (502) staff       (20)    20018 2020-10-09 18:17:27.000000 cisco-sdwan-1.9/cisco_sdwan/tasks/common.py
+-rw-r--r--   0 mareis     (502) staff       (20)    36034 2020-10-09 19:00:47.000000 cisco-sdwan-1.9/cisco_sdwan/tasks/implementation.py
+-rw-r--r--   0 mareis     (502) staff       (20)     6858 2020-10-09 18:28:56.000000 cisco-sdwan-1.9/cisco_sdwan/tasks/utils.py
+drwxr-xr-x   0 mareis     (502) staff       (20)        0 2020-10-14 02:34:58.540222 cisco-sdwan-1.9/cisco_sdwan.egg-info/
+-rw-r--r--   0 mareis     (502) staff       (20)    49488 2020-10-14 02:34:58.000000 cisco-sdwan-1.9/cisco_sdwan.egg-info/PKG-INFO
+-rw-r--r--   0 mareis     (502) staff       (20)      989 2020-10-14 02:34:58.000000 cisco-sdwan-1.9/cisco_sdwan.egg-info/SOURCES.txt
+-rw-r--r--   0 mareis     (502) staff       (20)        1 2020-10-14 02:34:58.000000 cisco-sdwan-1.9/cisco_sdwan.egg-info/dependency_links.txt
+-rw-r--r--   0 mareis     (502) staff       (20)       78 2020-10-14 02:34:58.000000 cisco-sdwan-1.9/cisco_sdwan.egg-info/entry_points.txt
+-rw-r--r--   0 mareis     (502) staff       (20)        9 2020-10-14 02:34:58.000000 cisco-sdwan-1.9/cisco_sdwan.egg-info/requires.txt
+-rw-r--r--   0 mareis     (502) staff       (20)       12 2020-10-14 02:34:58.000000 cisco-sdwan-1.9/cisco_sdwan.egg-info/top_level.txt
+-rw-r--r--   0 mareis     (502) staff       (20)       38 2020-10-14 02:34:58.549518 cisco-sdwan-1.9/setup.cfg
+-rw-r--r--   0 mareis     (502) staff       (20)     1038 2020-06-23 00:58:46.000000 cisco-sdwan-1.9/setup.py
```

### Comparing `cisco-sdwan-1.8/PKG-INFO` & `cisco-sdwan-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cisco-sdwan
-Version: 1.8
+Version: 1.9
 Summary: Automation Tools for Cisco SD-WAN Powered by Viptela
 Home-page: https://github.com/CiscoDevNet/sastre
 Author: Marcelo Reis
 Author-email: mareis@cisco.com
 License: UNKNOWN
 Description: [![published](https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-published.svg)](https://developer.cisco.com/codeexchange/github/repo/reismarcelo/sastre)
```

### Comparing `cisco-sdwan-1.8/README.md` & `cisco-sdwan-1.9/README.md`

 * *Files identical despite different names*

### Comparing `cisco-sdwan-1.8/cisco_sdwan/base/catalog.py` & `cisco-sdwan-1.9/cisco_sdwan/base/catalog.py`

 * *Files identical despite different names*

### Comparing `cisco-sdwan-1.8/cisco_sdwan/base/models_base.py` & `cisco-sdwan-1.9/cisco_sdwan/base/models_base.py`

 * *Files identical despite different names*

### Comparing `cisco-sdwan-1.8/cisco_sdwan/base/models_vmanage.py` & `cisco-sdwan-1.9/cisco_sdwan/base/models_vmanage.py`

 * *Files 1% similar despite different names*

```diff
@@ -516,14 +516,23 @@
     api_path = ApiPath('template/policy/customapp')
     store_path = ('policy_templates', 'CustomApp')
     store_file = '{item_name}.json'
     name_tag = 'appName'
     id_tag = 'appId'
     skip_cmp_tag_set = {'lastUpdated', }
 
+    def __init__(self, data):
+        """
+        :param data: dict containing the information to be associated with this API item.
+        """
+        # In 20.3.1 the payload returned by vManage contains a 'data' key with the policy definition in it. This is
+        # different than on previous versions or other ConfigItems. Overwriting the default __init__ in order to
+        # handle both options.
+        super().__init__(data.get('data', data))
+
 
 @register('policy_customapp', 'custom application policy', PolicyCustomApp, min_version='20.1')
 class PolicyCustomAppIndex(IndexConfigItem):
     api_path = ApiPath('template/policy/customapp', None, None, None)
     store_file = 'policy_templates_customapp.json'
     iter_fields = IdName('appId', 'appName')
```

### Comparing `cisco-sdwan-1.8/cisco_sdwan/base/processor.py` & `cisco-sdwan-1.9/cisco_sdwan/base/processor.py`

 * *Files identical despite different names*

### Comparing `cisco-sdwan-1.8/cisco_sdwan/base/rest_api.py` & `cisco-sdwan-1.9/cisco_sdwan/base/rest_api.py`

 * *Files identical despite different names*

### Comparing `cisco-sdwan-1.8/cisco_sdwan/cmd.py` & `cisco-sdwan-1.9/cisco_sdwan/cmd.py`

 * *Files identical despite different names*

### Comparing `cisco-sdwan-1.8/cisco_sdwan/migration/__init__.py` & `cisco-sdwan-1.9/cisco_sdwan/migration/__init__.py`

 * *Files identical despite different names*

### Comparing `cisco-sdwan-1.8/cisco_sdwan/migration/device_migration.py` & `cisco-sdwan-1.9/cisco_sdwan/migration/device_migration.py`

 * *Files identical despite different names*

### Comparing `cisco-sdwan-1.8/cisco_sdwan/migration/device_template_recipes.json` & `cisco-sdwan-1.9/cisco_sdwan/migration/device_template_recipes.json`

 * *Files identical despite different names*

### Comparing `cisco-sdwan-1.8/cisco_sdwan/migration/feature_migration.py` & `cisco-sdwan-1.9/cisco_sdwan/migration/feature_migration.py`

 * *Files identical despite different names*

### Comparing `cisco-sdwan-1.8/cisco_sdwan/migration/feature_template_recipes.json` & `cisco-sdwan-1.9/cisco_sdwan/migration/feature_template_recipes.json`

 * *Files identical despite different names*

### Comparing `cisco-sdwan-1.8/cisco_sdwan/migration/feature_templates/Factory_Default_AAA_CISCO_Template.json` & `cisco-sdwan-1.9/cisco_sdwan/migration/feature_templates/Factory_Default_AAA_CISCO_Template.json`

 * *Files identical despite different names*

### Comparing `cisco-sdwan-1.8/cisco_sdwan/migration/feature_templates/Factory_Default_Global_CISCO_Template.json` & `cisco-sdwan-1.9/cisco_sdwan/migration/feature_templates/Factory_Default_Global_CISCO_Template.json`

 * *Files identical despite different names*

### Comparing `cisco-sdwan-1.8/cisco_sdwan/tasks/common.py` & `cisco-sdwan-1.9/cisco_sdwan/tasks/common.py`

 * *Files identical despite different names*

### Comparing `cisco-sdwan-1.8/cisco_sdwan/tasks/implementation.py` & `cisco-sdwan-1.9/cisco_sdwan/tasks/implementation.py`

 * *Files identical despite different names*

### Comparing `cisco-sdwan-1.8/cisco_sdwan/tasks/utils.py` & `cisco-sdwan-1.9/cisco_sdwan/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `cisco-sdwan-1.8/cisco_sdwan.egg-info/PKG-INFO` & `cisco-sdwan-1.9/cisco_sdwan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cisco-sdwan
-Version: 1.8
+Version: 1.9
 Summary: Automation Tools for Cisco SD-WAN Powered by Viptela
 Home-page: https://github.com/CiscoDevNet/sastre
 Author: Marcelo Reis
 Author-email: mareis@cisco.com
 License: UNKNOWN
 Description: [![published](https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-published.svg)](https://developer.cisco.com/codeexchange/github/repo/reismarcelo/sastre)
```

### Comparing `cisco-sdwan-1.8/cisco_sdwan.egg-info/SOURCES.txt` & `cisco-sdwan-1.9/cisco_sdwan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cisco-sdwan-1.8/setup.py` & `cisco-sdwan-1.9/setup.py`

 * *Files identical despite different names*

