# Comparing `tmp/aepp-0.2.9.tar.gz` & `tmp/aepp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aepp-0.2.9.tar", last modified: Tue Apr  4 09:30:10 2023, max compression
+gzip compressed data, was "aepp-0.3.0.tar", last modified: Wed May 24 21:35:55 2023, max compression
```

## Comparing `aepp-0.2.9.tar` & `aepp-0.3.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 09:30:10.865281 aepp-0.2.9/
--rw-rw-rw-   0        0        0    10337 2021-10-20 19:48:57.000000 aepp-0.2.9/LICENSE
--rw-rw-rw-   0        0        0       16 2021-10-20 19:48:57.000000 aepp-0.2.9/MANIFEST.in
--rw-rw-rw-   0        0        0     3916 2023-04-04 09:30:10.864284 aepp-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     3253 2023-04-04 08:33:58.000000 aepp-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 09:30:10.822395 aepp-0.2.9/aepp/
--rw-rw-rw-   0        0        0     4601 2022-11-04 20:05:49.000000 aepp-0.2.9/aepp/__init__.py
--rw-rw-rw-   0        0        0       21 2023-04-04 08:48:21.000000 aepp-0.2.9/aepp/__version__.py
--rw-rw-rw-   0        0        0     4272 2023-02-04 09:19:40.000000 aepp-0.2.9/aepp/accesscontrol.py
--rw-rw-rw-   0        0        0    33405 2023-04-04 08:52:22.000000 aepp-0.2.9/aepp/catalog.py
--rw-rw-rw-   0        0        0     1836 2023-04-04 08:33:58.000000 aepp-0.2.9/aepp/config.py
--rw-rw-rw-   0        0        0    12808 2023-03-12 19:07:29.000000 aepp-0.2.9/aepp/configs.py
--rw-rw-rw-   0        0        0    23296 2023-04-04 08:43:31.000000 aepp-0.2.9/aepp/connector.py
--rw-rw-rw-   0        0        0    37405 2023-02-04 09:20:35.000000 aepp-0.2.9/aepp/customerprofile.py
--rw-rw-rw-   0        0        0    13212 2023-02-04 09:22:21.000000 aepp-0.2.9/aepp/dataaccess.py
--rw-rw-rw-   0        0        0    26369 2023-02-04 09:24:20.000000 aepp-0.2.9/aepp/dataprep.py
--rw-rw-rw-   0        0        0     7742 2023-03-12 19:07:12.000000 aepp-0.2.9/aepp/datasets.py
--rw-rw-rw-   0        0        0    23348 2023-02-04 09:31:59.000000 aepp-0.2.9/aepp/destination.py
--rw-rw-rw-   0        0        0     4251 2023-04-04 08:33:58.000000 aepp-0.2.9/aepp/destinationinstanceservice.py
--rw-rw-rw-   0        0        0    71154 2023-04-04 08:47:18.000000 aepp-0.2.9/aepp/flowservice.py
--rw-rw-rw-   0        0        0    18994 2023-02-04 09:30:09.000000 aepp-0.2.9/aepp/identity.py
--rw-rw-rw-   0        0        0    20359 2023-03-12 19:25:32.000000 aepp-0.2.9/aepp/ingestion.py
--rw-rw-rw-   0        0        0     8905 2023-02-04 09:35:43.000000 aepp-0.2.9/aepp/observability.py
--rw-rw-rw-   0        0        0    15229 2023-02-04 09:37:12.000000 aepp-0.2.9/aepp/policy.py
--rw-rw-rw-   0        0        0     7746 2023-02-04 09:39:18.000000 aepp-0.2.9/aepp/privacyservice.py
--rw-rw-rw-   0        0        0    51377 2023-02-09 17:51:38.000000 aepp-0.2.9/aepp/queryservice.py
--rw-rw-rw-   0        0        0     7186 2023-03-12 19:07:29.000000 aepp-0.2.9/aepp/sandboxes.py
--rw-rw-rw-   0        0        0   144959 2023-04-04 09:26:16.000000 aepp-0.2.9/aepp/schema.py
--rw-rw-rw-   0        0        0    37429 2023-02-04 09:44:52.000000 aepp-0.2.9/aepp/segmentation.py
--rw-rw-rw-   0        0        0     7145 2023-02-04 09:46:19.000000 aepp-0.2.9/aepp/sensei.py
-drwxrwxrwx   0        0        0        0 2023-04-04 09:30:10.838353 aepp-0.2.9/aepp.egg-info/
--rw-rw-rw-   0        0        0     3916 2023-04-04 09:30:10.000000 aepp-0.2.9/aepp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      814 2023-04-04 09:30:10.000000 aepp-0.2.9/aepp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 09:30:10.000000 aepp-0.2.9/aepp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-04-04 09:30:10.000000 aepp-0.2.9/aepp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-04 09:30:10.000000 aepp-0.2.9/aepp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-04 09:30:10.866278 aepp-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1584 2022-11-15 13:03:17.000000 aepp-0.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-04 09:30:10.860294 aepp-0.2.9/tests/
--rw-rw-rw-   0        0        0        0 2023-03-12 19:07:12.000000 aepp-0.2.9/tests/__init__.py
--rw-rw-rw-   0        0        0     1623 2023-03-12 19:07:12.000000 aepp-0.2.9/tests/catalog_test.py
--rw-rw-rw-   0        0        0      615 2023-03-12 19:07:12.000000 aepp-0.2.9/tests/dataaccess_test.py
--rw-rw-rw-   0        0        0      470 2023-03-12 19:07:12.000000 aepp-0.2.9/tests/datasets_test.py
--rw-rw-rw-   0        0        0     1482 2023-04-04 08:33:58.000000 aepp-0.2.9/tests/destinationinstanceservice_test.py
--rw-rw-rw-   0        0        0     3585 2023-03-12 19:07:12.000000 aepp-0.2.9/tests/flowservice_test.py
--rw-rw-rw-   0        0        0     2151 2023-03-12 19:07:12.000000 aepp-0.2.9/tests/schema_test.py
+drwxrwxrwx   0        0        0        0 2023-05-24 21:35:55.969395 aepp-0.3.0/
+-rw-rw-rw-   0        0        0    10337 2023-05-10 18:38:24.000000 aepp-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-05-10 18:38:24.000000 aepp-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3941 2023-05-24 21:35:55.968398 aepp-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3280 2023-05-12 08:07:02.000000 aepp-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 21:35:55.905567 aepp-0.3.0/aepp/
+-rw-rw-rw-   0        0        0     5224 2023-05-10 18:04:54.000000 aepp-0.3.0/aepp/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-05-24 21:31:23.000000 aepp-0.3.0/aepp/__version__.py
+-rw-rw-rw-   0        0        0     4888 2023-05-10 18:04:54.000000 aepp-0.3.0/aepp/accesscontrol.py
+-rw-rw-rw-   0        0        0    53530 2023-05-10 18:04:54.000000 aepp-0.3.0/aepp/catalog.py
+-rw-rw-rw-   0        0        0     2491 2023-05-24 21:26:52.000000 aepp-0.3.0/aepp/config.py
+-rw-rw-rw-   0        0        0    15338 2023-05-24 21:26:52.000000 aepp-0.3.0/aepp/configs.py
+-rw-rw-rw-   0        0        0    25957 2023-05-24 21:26:52.000000 aepp-0.3.0/aepp/connector.py
+-rw-rw-rw-   0        0        0    38021 2023-05-10 18:04:54.000000 aepp-0.3.0/aepp/customerprofile.py
+-rw-rw-rw-   0        0        0    13828 2023-05-10 18:04:54.000000 aepp-0.3.0/aepp/dataaccess.py
+-rw-rw-rw-   0        0        0    26985 2023-05-10 18:04:54.000000 aepp-0.3.0/aepp/dataprep.py
+-rw-rw-rw-   0        0        0     8358 2023-05-10 18:04:54.000000 aepp-0.3.0/aepp/datasets.py
+-rw-rw-rw-   0        0        0    23964 2023-05-10 18:04:54.000000 aepp-0.3.0/aepp/destination.py
+-rw-rw-rw-   0        0        0     4924 2023-05-23 14:25:29.000000 aepp-0.3.0/aepp/destinationinstanceservice.py
+-rw-rw-rw-   0        0        0    74612 2023-05-10 18:04:54.000000 aepp-0.3.0/aepp/flowservice.py
+-rw-rw-rw-   0        0        0    19610 2023-05-10 18:04:54.000000 aepp-0.3.0/aepp/identity.py
+-rw-rw-rw-   0        0        0    21043 2023-05-10 18:04:54.000000 aepp-0.3.0/aepp/ingestion.py
+-rw-rw-rw-   0        0        0     9521 2023-05-10 18:04:54.000000 aepp-0.3.0/aepp/observability.py
+-rw-rw-rw-   0        0        0    15845 2023-05-10 18:04:54.000000 aepp-0.3.0/aepp/policy.py
+-rw-rw-rw-   0        0        0     8362 2023-05-10 18:04:54.000000 aepp-0.3.0/aepp/privacyservice.py
+-rw-rw-rw-   0        0        0    51993 2023-05-10 18:04:54.000000 aepp-0.3.0/aepp/queryservice.py
+-rw-rw-rw-   0        0        0     7827 2023-05-10 18:04:54.000000 aepp-0.3.0/aepp/sandboxes.py
+-rw-rw-rw-   0        0        0   149385 2023-05-10 18:04:54.000000 aepp-0.3.0/aepp/schema.py
+-rw-rw-rw-   0        0        0    38045 2023-05-10 18:04:54.000000 aepp-0.3.0/aepp/segmentation.py
+-rw-rw-rw-   0        0        0     7761 2023-05-10 18:04:54.000000 aepp-0.3.0/aepp/sensei.py
+drwxrwxrwx   0        0        0        0 2023-05-24 21:35:55.929504 aepp-0.3.0/aepp.egg-info/
+-rw-rw-rw-   0        0        0     3941 2023-05-24 21:35:55.000000 aepp-0.3.0/aepp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      814 2023-05-24 21:35:55.000000 aepp-0.3.0/aepp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 21:35:55.000000 aepp-0.3.0/aepp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-24 21:35:55.000000 aepp-0.3.0/aepp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-24 21:35:55.000000 aepp-0.3.0/aepp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 21:35:55.970393 aepp-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2205 2023-05-10 18:04:54.000000 aepp-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 21:35:55.962414 aepp-0.3.0/tests/
+-rw-rw-rw-   0        0        0      623 2023-05-10 18:04:54.000000 aepp-0.3.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     2246 2023-05-10 18:04:54.000000 aepp-0.3.0/tests/catalog_test.py
+-rw-rw-rw-   0        0        0     1238 2023-05-10 18:04:54.000000 aepp-0.3.0/tests/dataaccess_test.py
+-rw-rw-rw-   0        0        0     1093 2023-05-10 18:04:54.000000 aepp-0.3.0/tests/datasets_test.py
+-rw-rw-rw-   0        0        0     2105 2023-05-23 14:25:29.000000 aepp-0.3.0/tests/destinationinstanceservice_test.py
+-rw-rw-rw-   0        0        0     4208 2023-05-10 18:04:54.000000 aepp-0.3.0/tests/flowservice_test.py
+-rw-rw-rw-   0        0        0     2774 2023-05-10 18:04:54.000000 aepp-0.3.0/tests/schema_test.py
```

### Comparing `aepp-0.2.9/LICENSE` & `aepp-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aepp-0.2.9/PKG-INFO` & `aepp-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: aepp
-Version: 0.2.9
+Version: 0.3.0
 Summary: Package to manage AEP API endpoint and some helper functions
-Home-page: https://github.com/pitchmuc/aep
+Home-page: https://github.com/adobe/aepp
 Author: Julien Piccini
 Author-email: piccini.julien@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Utilities
 Classifier: Topic :: Internet
@@ -71,15 +71,15 @@
 * [flowservice](./docs/flowservice.md)
 * [policy](./docs/policy.md)
 * [datasets](./docs/datasets.md)
 * [ingestion](./docs/ingestion.md)
 * [destination Authoring](./docs/destination.md)
 * [destination Instance](./docs/destinationinstanceservice.md)
 * [observability](./docs/observability.md)
-* accesscontrol
+* [accesscontrol](./docs/accesscontrol.md)
 * sensei
 * [privacyservice](./docs/privacyservice.md) (see 2nd note below)
 
 Last but not least, the core methods are described here: [main](./docs/main.md)
 
 ## queryservice module
```

### Comparing `aepp-0.2.9/README.md` & `aepp-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 * [flowservice](./docs/flowservice.md)
 * [policy](./docs/policy.md)
 * [datasets](./docs/datasets.md)
 * [ingestion](./docs/ingestion.md)
 * [destination Authoring](./docs/destination.md)
 * [destination Instance](./docs/destinationinstanceservice.md)
 * [observability](./docs/observability.md)
-* accesscontrol
+* [accesscontrol](./docs/accesscontrol.md)
 * sensei
 * [privacyservice](./docs/privacyservice.md) (see 2nd note below)
 
 Last but not least, the core methods are described here: [main](./docs/main.md)
 
 ## queryservice module
```

### Comparing `aepp-0.2.9/aepp/__init__.py` & `aepp-0.3.0/aepp/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+#  Copyright 2023 Adobe. All rights reserved.
+#  This file is licensed to you under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License. You may obtain a copy
+#  of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software distributed under
+#  the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
+#  OF ANY KIND, either express or implied. See the License for the specific language
+#  governing permissions and limitations under the License.
+
 # Internal Library
 from aepp import config
 from aepp import connector
 from .configs import *
 from .__version__ import __version__
 from typing import Union
```

### Comparing `aepp-0.2.9/aepp/accesscontrol.py` & `aepp-0.3.0/aepp/destinationinstanceservice.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,43 @@
+#  Copyright 2023 Adobe. All rights reserved.
+#  This file is licensed to you under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License. You may obtain a copy
+#  of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software distributed under
+#  the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
+#  OF ANY KIND, either express or implied. See the License for the specific language
+#  governing permissions and limitations under the License.
+
+# Internal Library
 import aepp
 from aepp import connector
+from typing import Union
 import logging
 from .configs import ConnectObject
-from typing import Union
-
-class AccessControl:
-    """
-    Access Control API endpoints.
-    Complete documentation is available:
-    https://www.adobe.io/apis/experienceplatform/home/api-reference.html#!acpdr/swagger-specs/access-control.yaml
-    """
 
-    ## logging capability
+class DestinationInstanceService:
     loggingEnabled = False
     logger = None
-
-    def __init__(
-        self,
+    """
+    This class is referring to Destination Instance Service capability for AEP.
+    """
+    def __init__(self,
         config: Union[dict,ConnectObject] = aepp.config.config_object,
-        header: dict =aepp.config.header,
+        header: dict = aepp.config.header,
         loggingObject: dict = None,
-        **kwargs,
-    ) -> None:
+        **kwargs,):
         """
-        Instantiate the access controle API wrapper.
+        Instantiating the class for destination instance service
+
         Arguments:
-            config : OPTIONAL : config object in the config module. (DO NOT MODIFY)
-            header : OPTIONAL : header object  in the config module. (DO NOT MODIFY)
             loggingObject : OPTIONAL : logging object to log messages.
-        kwargs :
-            header options
+            config : OPTIONAL : config object in the config module.
+            header : OPTIONAL : header object  in the config module.
+        possible kwargs:
         """
         if loggingObject is not None and sorted(
             ["level", "stream", "format", "filename", "file"]
         ) == sorted(list(loggingObject.keys())):
             self.loggingEnabled = True
             self.logger = logging.getLogger(f"{__name__}")
             self.logger.setLevel(loggingObject["level"])
@@ -51,50 +55,46 @@
                 self.logger.addHandler(streamHandler)
         if type(config) == dict: ## Supporting either default setup or passing a ConnectObject
             config = config
         elif type(config) == ConnectObject:
             header = config.getConfigHeader()
             config = config.getConfigObject()
         self.connector = connector.AdobeRequest(
-            config_object=config,
+            config=config,
             header=header,
             loggingEnabled=self.loggingEnabled,
             logger=self.logger,
         )
-        if kwargs.get('sandbox',None) is not None: ## supporting sandbox setup on class instanciation
+        self.header = self.connector.header
+        # self.header.update({"Accept": "application/json"})
+        self.header.update(**kwargs)
+        if kwargs.get('sandbox',None) is not None: ## supporting sandbox setup on class instantiation
             self.sandbox = kwargs.get('sandbox')
             self.connector.config["sandbox"] = kwargs.get('sandbox')
             self.header.update({"x-sandbox-name":kwargs.get('sandbox')})
             self.connector.header.update({"x-sandbox-name":kwargs.get('sandbox')})
         else:
             self.sandbox = self.connector.config["sandbox"]
-        self.header = self.connector.header
-        self.header.update(**kwargs)
-        self.endpoint = (
-            aepp.config.endpoints["global"] + aepp.config.endpoints["access"]
-        )
-
-    def getReferences(self) -> dict:
-        """
-        List all available permission names and resource types.
+        self.endpoint = aepp.config.endpoints["global"] + aepp.config.endpoints["destinationInstance"]
+        
+        
+    def createAdHocDatasetExport(self, flowIdToDatasetIds: dict = None)->dict:
         """
-        if self.loggingEnabled:
-            self.logger.debug(f"Starting getReferences")
-        path = "/acl/reference"
-        res = self.connector.getData(self.endpoint + path, headers=self.header)
-        return res
-
-    def postEffectivePolicies(self, listElements: list = None):
-        """
-        List all effective policies for a user on given resources within a sandbox.
+        Create an Adhoc Request based on the flowId and the datasetId passed in argument.
         Arguments:
-            listElements : REQUIRED : List of resource urls. Example url : /resource-types/{resourceName} or /permissions/{highLevelPermissionName}
+            flowIdToDatasetIds : REQUIRED :  dict containing the definition of flowId to datasetIds
         """
-        if type(listElements) != list:
-            raise TypeError("listElements should be a list of elements")
         if self.loggingEnabled:
-            self.logger.debug(f"Starting postEffectivePolicies")
-        path = "/acl/effective-policies"
-        res = self.connector.postData(
-            self.endpoint + path, data=listElements, headers=self.header
-        )
+            self.logger.debug(f"Starting creating adhoc dataset export")
+        if flowIdToDatasetIds is None or type(flowIdToDatasetIds) != dict:
+            raise Exception("Require a dict for defining the flowId to datasetIds mapping")
+        activationInfo = {'activationInfo': {'destinations': []}};
+        for flowId, datasetIds in flowIdToDatasetIds.items():
+            destination = {'flowId': flowId, 'datasets': []}
+            for datasetId in datasetIds:
+                dataset = {'id': datasetId}
+                destination['datasets'].append(dataset)
+            activationInfo['activationInfo']['destinations'].append(destination)
+        self.header.update({"Accept":"application/vnd.adobe.adhoc.activation+json; version=3"})
+        path = "/adhocrun"
+        res = self.connector.postData(self.endpoint + path, data=activationInfo)
         return res
```

### Comparing `aepp-0.2.9/aepp/configs.py` & `aepp-0.3.0/aepp/configs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+#  Copyright 2023 Adobe. All rights reserved.
+#  This file is licensed to you under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License. You may obtain a copy
+#  of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software distributed under
+#  the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
+#  OF ANY KIND, either express or implied. See the License for the specific language
+#  governing permissions and limitations under the License.
+
 import json
 import os
 from pathlib import Path
 from typing import Optional
 import json
 
 # Non standard libraries
@@ -28,62 +38,65 @@
 
 
 def createConfigFile(
     destination: str = "config_aep_template.json",
     sandbox: str = "prod",
     environment: str = "prod",
     verbose: object = False,
-    auth_type: str = "jwt",
+    auth_type: str = "oauthV2",
     **kwargs,
 ) -> None:
     """
     This function will create a 'config_admin.json' file where you can store your access data.
     Arguments:
         destination : OPTIONAL : if you wish to save the file at a specific location.
         sandbox : OPTIONAL : You can directly set your sandbox name in this parameter.
         verbose : OPTIONAL : set to true, gives you a print stateent where is the location.
-        auth_type : OPTIONAL : type of authentication, either "jwt" or "oauth"
+        auth_type : OPTIONAL : type of authentication, either "jwt" or "oauthV2" or "oauthV1". Default is oauthV2
     """
     json_data: dict = {
         "org_id": "<orgID>",
         "client_id": "<client_id>",
         "secret": "<YourSecret>",
         "sandbox-name": sandbox,
         "environment": environment
     }
     if auth_type == "jwt":
         json_data["tech_id"] = "<something>@techacct.adobe.com"
         json_data["pathToKey"] = "<path/to/your/privatekey.key>"
-    elif auth_type == "oauth":
+    elif auth_type == "oauthV2":
+        json_data["scopes"] = "<scopes>"
+    elif auth_type == "oauthV1":
         json_data["auth_code"] = "<auth_code>"
     else:
-        raise ValueError("unsupported authentication type, currently only jwt and oauth are supported")
-
+        raise ValueError("unsupported authentication type, currently only jwt, oauthV1 and oauthV2 are supported")
     if ".json" not in destination:
         destination: str = f"{destination}.json"
     with open(destination, "w") as cf:
         cf.write(json.dumps(json_data, indent=4))
     if verbose:
         print(
-            f" file created at this location : {os.getcwd()}{os.sep}config_analytics.json"
+            f" file created at this location : {os.getcwd()}{os.sep}{destination}.json"
         )
 
 
 def importConfigFile(
     path: str = None,
     connectInstance: bool = False,
-    auth_type: str = "jwt"
+    auth_type: str = None,
+    sandbox:str = None,
 ):
     """Reads the file denoted by the supplied `path` and retrieves the configuration information
     from it.
 
     Arguments:
         path: REQUIRED : path to the configuration file. Can be either a fully-qualified or relative.
         connectInstance : OPTIONAL : If you want to return an instance of the ConnectObject class
-        auth_type : OPTIONAL : type of authentication, either "jwt" or "oauth"
+        auth_type : OPTIONAL : type of authentication, either "jwt" or "oauthV1" or "oauthV2". Detected based on keys present in config file.
+        sandbox : OPTIONAL : The sandbox to connect it.
 
     Example of path value.
     "config.json"
     "./config.json"
     "/my-folder/config.json"
     """
     if path is None:
@@ -92,42 +105,50 @@
     config_file_path: Optional[Path] = find_path(path)
     if config_file_path is None:
         raise FileNotFoundError(
             f"Unable to find the configuration file under path `{path}`."
         )
     with open(config_file_path, "r") as file:
         provided_config = json.load(file)
-        provided_keys = provided_config.keys()
+        provided_keys = list(provided_config.keys())
         if "api_key" in provided_keys:
             ## old naming for client_id
             client_id = provided_config["api_key"]
         elif "client_id" in provided_keys:
             client_id = provided_config["client_id"]
         else:
             raise RuntimeError(
                 f"Either an `api_key` or a `client_id` should be provided."
             )
-
+        if auth_type is None:
+            if 'scopes' in provided_keys:
+                auth_type = 'oauthV2'
+            elif 'tech_id' in provided_keys and "pathToKey" in provided_keys:
+                auth_type = 'jwt'
+            elif 'auth_code' in provided_keys:
+                auth_type = 'oauthV1'
         args = {
             "org_id": provided_config["org_id"],
             "client_id": client_id,
             "secret": provided_config["secret"],
             "sandbox": provided_config.get("sandbox-name", "prod"),
             "environment": provided_config.get("environment", "prod"),
             "connectInstance": connectInstance
         }
-
+        if sandbox is not None: ## overriding sandbox from parameter
+            args["sandbox"] = sandbox
         if auth_type == "jwt":
             args["tech_id"] = provided_config["tech_id"]
             args["path_to_key"] = provided_config["pathToKey"]
-        elif auth_type == "oauth":
+        elif auth_type == "oauthV2":
+            args["scopes"] = provided_config["scopes"].replace(' ','')
+        elif auth_type == "oauthV1":
             args["auth_code"] = provided_config["auth_code"]
         else:
             raise ValueError("unsupported authentication type, currently only jwt and oauth are supported")
-
         myInstance = configure(**args)
 
     if connectInstance:
         return myInstance
 
 
 def configure(
@@ -136,74 +157,79 @@
     secret: str = None,
     client_id: str = None,
     path_to_key: str = None,
     private_key: str = None,
     sandbox: str = "prod",
     connectInstance: bool = False,
     environment: str = "prod",
-    auth_code: str = None
+    scopes: str = None,
+    auth_code:str=None
 ):
     """Performs programmatic configuration of the API using provided values.
     Arguments:
         org_id : REQUIRED : Organization ID
         tech_id : OPTIONAL : Technical Account ID
         secret : REQUIRED : secret generated for your connection
         client_id : REQUIRED : The client_id (old api_key) provided by the JWT connection.
         path_to_key : REQUIRED : If you have a file containing your private key value.
         private_key : REQUIRED : If you do not use a file but pass a variable directly.
         sandbox : OPTIONAL : If not provided, default to prod
         connectInstance : OPTIONAL : If you want to return an instance of the ConnectObject class
         environment : OPTIONAL : If not provided, default to prod
-        auth_code : OPTIONAL : If an authorization code is used directly instead of generating via JWT
+        scopes : OPTIONAL : The scope define in your project for your API connection. Oauth V2, for clients and customers.
+        auth_code : OPTIONAL : If an authorization code is used directly instead of generating via JWT. Oauth V1 only, for adobe internal services.
     """
     if not org_id:
         raise ValueError("`org_id` must be specified in the configuration.")
     if not client_id:
         raise ValueError("`client_id` must be specified in the configuration.")
     if not secret:
         raise ValueError("`secret` must be specified in the configuration.")
-    if (auth_code is not None and (path_to_key is not None or private_key is not None)) \
-            or (auth_code is None and path_to_key is None and private_key is None):
-        raise ValueError("either `auth_code` needs to be specified or one of `private_key` or `path_to_key`")
+    if (scopes is not None and (path_to_key is not None or private_key is not None) and auth_code is not None) \
+            or (scopes is None and path_to_key is None and private_key is None and auth_code is None):
+        raise ValueError("either `scopes` needs to be specified or one of `private_key` or `path_to_key` or an `auth_code`")
     config_object["org_id"] = org_id
     header["x-gw-ims-org-id"] = org_id
     config_object["client_id"] = client_id
     header["x-api-key"] = client_id
     config_object["tech_id"] = tech_id
     config_object["secret"] = secret
     config_object["pathToKey"] = path_to_key
     config_object["private_key"] = private_key
+    config_object["scopes"] = scopes
     config_object["auth_code"] = auth_code
     config_object["sandbox"] = sandbox
     header["x-sandbox-name"] = sandbox
 
     # ensure we refer to the right environment endpoints
     config_object["environment"] = environment
     if environment == "prod":
         endpoints["global"] = "https://platform.adobe.io"
         config_object["imsEndpoint"] = "https://ims-na1.adobelogin.com"
     else:
         endpoints["global"] = f"https://platform-{environment}.adobe.io"
         config_object["imsEndpoint"] = "https://ims-na1-stg1.adobelogin.com"
     endpoints["streaming"]["inlet"] = f"{endpoints['global']}/data/core/edge"
     config_object["jwtTokenEndpoint"] = f"{config_object['imsEndpoint']}/ims/exchange/jwt"
-    config_object["oauthTokenEndpoint"] = f"{config_object['imsEndpoint']}/ims/token/v1"
-
+    config_object["oauthTokenEndpointV1"] = f"{config_object['imsEndpoint']}/ims/token/v1"
+    config_object["oauthTokenEndpointV2"] = f"{config_object['imsEndpoint']}/ims/token/v2"
     # ensure the reset of the state by overwriting possible values from previous import.
     config_object["date_limit"] = 0
     config_object["token"] = ""
     if connectInstance:
         myInstance = ConnectObject(
             org_id=org_id,
             tech_id=tech_id,
             secret=secret,
             client_id=client_id,
             path_to_key = path_to_key,
             private_key = private_key,
-            sandbox=sandbox
+            sandbox=sandbox,
+            scopes=scopes,
+            auth_code=auth_code
         )
         return myInstance
 
 
 def get_private_key_from_config(config: dict) -> str:
     """
     Returns the private key directly or read a file to return the private key.
@@ -255,16 +281,18 @@
     def __init__(self,
             org_id: str = None,
             tech_id: str = None,
             secret: str = None,
             client_id: str = None,
             path_to_key: str = None,
             private_key: str = None,
+            scopes:str=None,
             sandbox: str = "prod",
             environment: str = "prod",
+            auth_code:str=None,
             **kwargs)->None:
         """
         Take a config object and save the configuration directly in the instance of the class.
         """
         self.header = {"Accept": "application/json",
           "Content-Type": "application/json",
           "Authorization": "",
@@ -277,49 +305,65 @@
             self.globalEndpoint = "https://platform.adobe.io"
             self.imsEndpoint = "https://ims-na1.adobelogin.com"
         else:
             self.globalEndpoint = f"https://platform-{environment}.adobe.io"
             self.imsEndpoint = "https://ims-na1-stg1.adobelogin.com"
         self.streamInletEndpoint = f"{self.globalEndpoint}/data/core/edge"
         self.jwtEndpoint = f"{self.imsEndpoint}/ims/exchange/jwt"
-        self.oathEndpoint = f"{self.imsEndpoint}/ims/token/v1"
+        self.oauthEndpointV1 = f"{self.imsEndpoint}/ims/token/v1"
+        self.oauthEndpointV2 = f"{self.imsEndpoint}/ims/token/v2"
         self.org_id = org_id
         self.tech_id = tech_id
         self.client_id = client_id
         self.secret = secret
         self.pathToKey = path_to_key
         self.privateKey = private_key
         self.sandbox = sandbox
+        self.scopes = scopes
         self.token = ""
         self.__configObject__ = {
             "org_id": self.org_id,
             "client_id": self.client_id,
             "tech_id": self.tech_id,
             "pathToKey": self.pathToKey,
             "private_key": self.privateKey,
             "secret": self.secret,
             "date_limit" : 0,
             "sandbox": self.sandbox,
             "token": "",
             "imsEndpoint" : self.imsEndpoint,
             "jwtTokenEndpoint" : self.jwtEndpoint,
-            "oathTokenEndpoint" : self.oathEndpoint 
+            "oauthTokenEndpointV1" : self.oauthEndpointV1,
+            "oauthTokenEndpointV2" : self.oauthEndpointV2,
+            "scopes": self.scopes
         }
     
     def connect(self)->None:
         """
         Generate a token and provide a connector instance in that class.
         """
         self.connector = connector.AdobeRequest(self.__configObject__,self.header)
         self.token = self.connector.token
+        self.header['Authorization'] = 'bearer '+self.token
     
     def getConfigObject(self)->dict:
         """
         Return the config object expected.
         """
         return self.__configObject__
     
     def getConfigHeader(self)->dict:
         """
         Return the default header
         """
-        return self.header
+        return self.header
+
+    def setSandbox(self,sandbox:str=None)->dict:
+        """
+        Update the sandbox used
+        """
+        if sandbox is None:
+            return None
+        self.sandbox = sandbox
+        self.header["x-sandbox-name"] = sandbox
+        self.__configObject__["sandbox"] = sandbox
+        return self.getConfigObject()
```

### Comparing `aepp-0.2.9/aepp/connector.py` & `aepp-0.3.0/aepp/connector.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+#  Copyright 2023 Adobe. All rights reserved.
+#  This file is licensed to you under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License. You may obtain a copy
+#  of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software distributed under
+#  the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
+#  OF ANY KIND, either express or implied. See the License for the specific language
+#  governing permissions and limitations under the License.
+
 ## Internal modules
 from aepp import config, configs
 
 ## External module
 import json
 import os
 from dataclasses import dataclass
@@ -59,36 +69,48 @@
             )
         self.config = deepcopy(config)
         self.header = deepcopy(header)
         self.endpoints = deepcopy(endpoints)
         self.loggingEnabled = loggingEnabled
         self.logger = logger
         self.retry = retry
+        requests.packages.urllib3.disable_warnings()
         if self.config["token"] == "" or time.time() > self.config["date_limit"]:
             if self.config["private_key"] is not None or self.config["pathToKey"] is not None:
+                self.connectionType = 'jwt'
                 token_info = self.get_jwt_token_and_expiry_for_config(
                     config=self.config,
                     verbose=verbose,
                     aepScope=kwargs.get("aepScope"),
                     privacyScope=kwargs.get("privacyScope"),
                 )
+            elif self.config["scopes"] is not None:
+                self.connectionType = 'oauthV2'
+                token_info = self.get_oauth_token_and_expiry_for_config(
+                    config=self.config,
+                    verbose=verbose
+                )
             else:
+                self.connectionType = 'oauthV1'
                 token_info = self.get_oauth_token_and_expiry_for_config(
                     config=self.config,
                     verbose=verbose
                 )
             self.token = token_info.token
             self.config["token"] = self.token
+            if self.connectionType == 'jwt':
+                timeScale = 1000 ## jwt returns milliseconds expiry
+            elif self.connectionType == 'oauthV1' or self.connectionType == 'oauthV2':
+                timeScale = 1 ## oauth returns seconds expiry
             self.config["date_limit"] = (
-                time.time() + token_info.expiry / 1000 - 500
+                time.time() + token_info.expiry / timeScale - 500
             )
             self.header.update({"Authorization": f"Bearer {self.token}"})
-
         # x-sandbox-id is required when using non-user token, but forbidden for user token
-        if self.config["auth_code"] is not None and "x-sandbox-id" not in self.header:
+        if self.connectionType == 'oauthV1' and "x-sandbox-id" not in self.header:
             self.update_sandbox_id(self.config["sandbox"])
 
     def _find_path(self, path: str) -> Optional[Path]:
         """Checks if the file denoted by the specified `path` exists and returns the Path object
         for the file.
 
         If the file under the `path` does not exist and the path denotes an absolute path, tries
@@ -117,23 +139,34 @@
         Arguments :
             config : REQUIRED : Configuration object.
             verbose : OPTIONAL : Default False. If set to True, print information.
             save : OPTIONAL : Default False. If set to True, save the toke in the .
         """
         if type(config)!= dict:
             config = config.getConfigObject()
-        oauth_payload = {
-            "grant_type": "authorization_code",
-            "client_id": config["client_id"],
-            "client_secret": config["secret"],
-            "code": config["auth_code"]
-        }
-        response = requests.post(
-            config["oauthTokenEndpoint"], data=oauth_payload
-        )
+        if self.connectionType == 'oauthV1':
+            oauth_payload = {
+                "grant_type": "authorization_code",
+                "client_id": config["client_id"],
+                "client_secret": config["secret"],
+                "code": config["auth_code"]
+            }
+            response = requests.post(
+                config["oauthTokenEndpointV1"], data=oauth_payload, verify=False
+            )
+        elif self.connectionType == 'oauthV2':
+            oauth_payload = {
+                "grant_type": "client_credentials",
+                "client_id": config["client_id"],
+                "client_secret": config["secret"],
+                "scope": config["scopes"]
+            }
+            response = requests.post(
+                config["oauthTokenEndpointV2"], data=oauth_payload, verify=False
+            )
         return self._token_postprocess(response=response, verbose=verbose, save=save)
 
     def get_jwt_token_and_expiry_for_config(
         self,
         config: Union[dict,configs.ConnectObject],
         verbose: bool = False,
         save: bool = False,
@@ -171,15 +204,15 @@
 
         payload = {
             "client_id": config["client_id"],
             "client_secret": config["secret"],
             "jwt_token": encoded_jwt,
         }
         response = requests.post(
-            config["jwtTokenEndpoint"], headers=header_jwt, data=payload
+            config["jwtTokenEndpoint"], headers=header_jwt, data=payload, verify=False
         )
         return self._token_postprocess(response=response, verbose=verbose, save=save)
 
     def _token_postprocess(
         self,
         response: Response,
         verbose: bool = False,
@@ -195,26 +228,26 @@
         json_response = response.json()
         try:
             self.token = json_response["access_token"]
             self.config["token"] = self.token
         except KeyError:
             print("Issue retrieving token")
             print(json_response)
-        expiry = json_response["expires_in"] - 500
+        expiry = json_response["expires_in"]
         if save:
             with open("token.txt", "w") as f:
                 f.write(self.token)
             print(f"token has been saved here: {os.getcwd()}{os.sep}token.txt")
         if self.loggingEnabled:
             self.logger.debug(f"token retrieved: {self.token}")
         if verbose:
-            print("token valid till : " + time.ctime(time.time() + expiry / 1000))
+            print("token valid till : " + time.ctime(time.time() + expiry))
         if self.loggingEnabled:
             self.logger.debug(
-                f"token valid till : {time.ctime(time.time() + expiry / 1000)}"
+                f"token valid till : {time.ctime(time.time() + expiry)}"
             )
         return TokenInfo(token=self.token, expiry=expiry)
 
     def _get_jwt(self, payload: dict, private_key: str) -> str:
         """
         Ensure that jwt enconding return the same type (str) as versions < 2.0.0 returned bytes and >2.0.0 return strings.
         """
@@ -227,22 +260,29 @@
         """
         Checking if the token is still valid
         """
         now = time.time()
         if now > self.config["date_limit"]:
             if self.loggingEnabled:
                 self.logger.warning("token expired. Trying to retrieve a new token")
-            token_with_expiry = self.get_jwt_token_and_expiry_for_config(config=self.config)
+            if self.connectionType == 'jwt':
+                token_with_expiry = self.get_jwt_token_and_expiry_for_config(config=self.config)
+            elif self.connectionType == 'oauthV1' or self.connectionType == 'oauthV2':
+                token_with_expiry = self.get_oauth_token_and_expiry_for_config(config=self.config)
             self.token = token_with_expiry["token"]
             self.config["token"] = self.token
             if self.loggingEnabled:
                 self.logger.info("new token retrieved : {self.token}")
             self.header.update({"Authorization": f"Bearer {self.token}"})
+            if self.connectionType == 'jwt':
+                timeScale = 1000 ## jwt returns milliseconds expiry
+            elif self.connectionType == 'oauthV1' or self.connectionType == 'oauthV2':
+                timeScale = 1 ## oauth returns seconds expiry
             self.config["date_limit"] = (
-                time.time() + token_with_expiry["expiry"] / 1000 - 500
+                time.time() + token_with_expiry["expiry"] / timeScale - 500
             )
 
     def updateSandbox(self, sandbox: str) -> None:
         """
         Update the sandbox used for the request
         Arguments:
             sandbox : REQUIRED : the sandbox to use for the requests
@@ -250,15 +290,15 @@
         if not sandbox:
             raise Exception("require a sandbox")
         self.header["x-sandbox-name"] = sandbox
 
     def update_sandbox_id(self, sandbox: str) -> None:
         """
         Update the sandbox ID used for the request.
-        This is required when using non-user credentials.
+        This is required when using non-user credentials. Only internal adobe tools and oauth V1 can access this.
         Arguments:
             sandbox : REQUIRED : the sandbox name to use for the requests
         """
         if not sandbox:
             raise Exception("require a sandbox")
         endpoint = f"{self.endpoints['global']}{self.endpoints['sandboxes']}/sandboxes/{sandbox}"
         res = self.getData(endpoint)
@@ -283,28 +323,28 @@
         if headers is None:
             headers = self.header
         if self.loggingEnabled:
             self.logger.debug(
                 f"Start GET request to {endpoint} with header: {json.dumps(headers)}"
             )
         if params is None and data is None:
-            res = requests.get(endpoint, headers=headers)
+            res = requests.get(endpoint, headers=headers, verify=False)
         elif params is not None and data is None:
             if self.loggingEnabled:
                 self.logger.debug(f"params: {json.dumps(params)}")
-            res = requests.get(endpoint, headers=headers, params=params)
+            res = requests.get(endpoint, headers=headers, params=params, verify=False)
         elif params is None and data is not None:
             if self.loggingEnabled:
                 self.logger.debug(f"data: {json.dumps(data)}")
-            res = requests.get(endpoint, headers=headers, data=data)
+            res = requests.get(endpoint, headers=headers, data=data, verify=False)
         elif params is not None and data is not None:
             if self.loggingEnabled:
                 self.logger.debug(f"params: {json.dumps(params)}")
                 self.logger.debug(f"data: {json.dumps(data)}")
-            res = requests.get(endpoint, headers=headers, params=params, data=data)
+            res = requests.get(endpoint, headers=headers, params=params, data=data, verify=False)
         if self.loggingEnabled:
             self.logger.debug(f"endpoint used: {res.request.url}")
             self.logger.debug(f"params used: {params}")
         try:
             if kwargs.get("format", "json") == "json":
                 res_json = res.json()
             if kwargs.get("format", "json") == "txt":
@@ -355,17 +395,17 @@
         if headers is None:
             headers = self.header
         if self.loggingEnabled:
             self.logger.debug(
                 f"Start GET request to {endpoint} with header: {json.dumps(headers)}"
             )
         if params is None:
-            res = requests.head(endpoint, headers=headers)
+            res = requests.head(endpoint, headers=headers, verify=False)
         if params is not None:
-            res = requests.head(endpoint, headers=headers, params=params)
+            res = requests.head(endpoint, headers=headers, params=params, verify=False)
         try:
             res_header = res.headers()
         except:
             if kwargs.get("verbose", False):
                 print("error generating the JSON response")
                 print(f"status: {res.status_code}")
                 print(res.text)
@@ -392,35 +432,35 @@
         if headers is None:
             headers = self.header
         if self.loggingEnabled:
             self.logger.debug(
                 f"Start POST request to {endpoint} with header: {json.dumps(headers)}"
             )
         if params is None and data is None:
-            res = requests.post(endpoint, headers=headers)
+            res = requests.post(endpoint, headers=headers, verify=False)
         elif params is not None and data is None:
             if self.loggingEnabled:
                 self.logger.debug(f"params: {json.dumps(params)}")
-            res = requests.post(endpoint, headers=headers, params=params)
+            res = requests.post(endpoint, headers=headers, params=params, verify=False)
         elif params is None and data is not None:
             if self.loggingEnabled:
                 self.logger.debug(f"data: {json.dumps(data)}")
-            res = requests.post(endpoint, headers=headers, data=json.dumps(data))
+            res = requests.post(endpoint, headers=headers, data=json.dumps(data), verify=False)
         elif params is not None and data is not None:
             if self.loggingEnabled:
                 self.logger.debug(f"params: {json.dumps(params)}")
                 self.logger.debug(f"data: {json.dumps(data)}")
             res = requests.post(
-                endpoint, headers=headers, params=params, data=json.dumps(data)
+                endpoint, headers=headers, params=params, data=json.dumps(data), verify=False
             )
         elif bytesData is not None:
             if self.loggingEnabled:
                 self.logger.debug(f"bytes data used")
             res = requests.post(
-                endpoint, headers=headers, params=params, data=bytesData
+                endpoint, headers=headers, params=params, data=bytesData, verify=False
             )
         try:
             formatUse = kwargs.get("format", "json")
             if self.loggingEnabled:
                 self.logger.debug(f"format used: {formatUse}")
             if formatUse == "json":
                 res_json = res.json()
@@ -467,25 +507,25 @@
         if self.loggingEnabled:
             self.logger.debug(
                 f"Start PATCH request to {endpoint} with header: {json.dumps(headers)}"
             )
         if params is not None and data is None:
             if self.loggingEnabled:
                 self.logger.debug(f"params: {json.dumps(params)}")
-            res = requests.patch(endpoint, headers=headers, params=params)
+            res = requests.patch(endpoint, headers=headers, params=params, verify=False)
         elif params is None and data is not None:
             if self.loggingEnabled:
                 self.logger.debug(f"data: {json.dumps(data)}")
-            res = requests.patch(endpoint, headers=headers, data=json.dumps(data))
+            res = requests.patch(endpoint, headers=headers, data=json.dumps(data), verify=False)
         elif params is not None and data is not None:
             if self.loggingEnabled:
                 self.logger.debug(f"params: {json.dumps(params)}")
                 self.logger.debug(f"data: {json.dumps(data)}")
             res = requests.patch(
-                endpoint, headers=headers, params=params, data=json.dumps(data)
+                endpoint, headers=headers, params=params, data=json.dumps(data), verify=False
             )
         try:
             res_json = res.json()
         except:
             if kwargs.get("verbose", False):
                 print("error generating the JSON response")
                 print(f"status: {res.status_code}")
@@ -521,25 +561,25 @@
         if self.loggingEnabled:
             self.logger.debug(
                 f"Start PUT request to {endpoint} with header: {json.dumps(headers)}"
             )
         if params is not None and data is None:
             if self.loggingEnabled:
                 self.logger.debug(f"params: {json.dumps(params)}")
-            res = requests.put(endpoint, headers=headers, params=params)
+            res = requests.put(endpoint, headers=headers, params=params, verify=False)
         elif params is None and data is not None:
             if self.loggingEnabled:
                 self.logger.debug(f"data: {json.dumps(data)}")
-            res = requests.put(endpoint, headers=headers, data=json.dumps(data))
+            res = requests.put(endpoint, headers=headers, data=json.dumps(data), verify=False)
         elif params is not None and data is not None:
             if self.loggingEnabled:
                 self.logger.debug(f"params: {json.dumps(params)}")
                 self.logger.debug(f"data: {json.dumps(data)}")
             res = requests.put(
-                endpoint, headers=headers, params=params, data=json.dumps(data)
+                endpoint, headers=headers, params=params, data=json.dumps(data), verify=False
             )
         try:
             res_json = res.json()
         except:
             if kwargs.get("verbose", False):
                 print("error generating the JSON response")
                 print(f"status: {res.status_code}")
@@ -564,17 +604,17 @@
         if headers is None:
             headers = self.header
         if self.loggingEnabled:
             self.logger.debug(
                 f"Start PUT request to {endpoint} with header: {json.dumps(headers)}"
             )
         if params is None:
-            res = requests.delete(endpoint, headers=headers)
+            res = requests.delete(endpoint, headers=headers, verify=False)
         elif params is not None:
-            res = requests.delete(endpoint, headers=headers, params=params)
+            res = requests.delete(endpoint, headers=headers, params=params, verify=False)
         try:
             status_code = res.status_code
             if status_code >= 400:
                 if self.loggingEnabled:
                     self.logger.error(
                         f"error with the response {res.status_code}: {res.text}"
                     )
```

### Comparing `aepp-0.2.9/aepp/customerprofile.py` & `aepp-0.3.0/aepp/customerprofile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+#  Copyright 2023 Adobe. All rights reserved.
+#  This file is licensed to you under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License. You may obtain a copy
+#  of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software distributed under
+#  the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
+#  OF ANY KIND, either express or implied. See the License for the specific language
+#  governing permissions and limitations under the License.
+
 # Internal Library
 import aepp
 from aepp import connector
 from copy import deepcopy
 import pandas as pd
 import logging
 from typing import Union
@@ -55,15 +65,15 @@
                 self.logger.addHandler(streamHandler)
         if type(config) == dict: ## Supporting either default setup or passing a ConnectObject
             config = config
         elif type(config) == ConnectObject:
             header = config.getConfigHeader()
             config = config.getConfigObject()
         self.connector = connector.AdobeRequest(
-            config_object=config,
+            config=config,
             header=header,
             loggingEnabled=self.loggingEnabled,
             logger=self.logger,
         )
         self.header = self.connector.header
         self.header["Accept"] = "application/vnd.adobe.xdm+json"
         self.header.update(**kwargs)
```

### Comparing `aepp-0.2.9/aepp/dataaccess.py` & `aepp-0.3.0/aepp/dataaccess.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+#  Copyright 2023 Adobe. All rights reserved.
+#  This file is licensed to you under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License. You may obtain a copy
+#  of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software distributed under
+#  the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
+#  OF ANY KIND, either express or implied. See the License for the specific language
+#  governing permissions and limitations under the License.
+
 import aepp
 from aepp import connector
 import logging
 import time
 import io
 from typing import Union
 from .configs import ConnectObject
@@ -51,15 +61,15 @@
                 self.logger.addHandler(streamHandler)
         if type(config) == dict: ## Supporting either default setup or passing a ConnectObject
             config = config
         elif type(config) == ConnectObject:
             header = config.getConfigHeader()
             config = config.getConfigObject()
         self.connector = connector.AdobeRequest(
-            config_object=config,
+            config=config,
             header=header,
             loggingEnabled=self.loggingEnabled,
             loggingObject=self.logger,
         )
         self.header = self.connector.header
         self.header.update(**kwargs)
         if kwargs.get('sandbox',None) is not None: ## supporting sandbox setup on class instanciation
```

### Comparing `aepp-0.2.9/aepp/dataprep.py` & `aepp-0.3.0/aepp/dataprep.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+#  Copyright 2023 Adobe. All rights reserved.
+#  This file is licensed to you under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License. You may obtain a copy
+#  of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software distributed under
+#  the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
+#  OF ANY KIND, either express or implied. See the License for the specific language
+#  governing permissions and limitations under the License.
+
 import aepp
 from aepp import connector
 from copy import deepcopy
 import pandas as pd
 from typing import Union
 import re
 import logging
@@ -56,15 +66,15 @@
                 self.logger.addHandler(streamHandler)
         if type(config) == dict: ## Supporting either default setup or passing a ConnectObject
             config = config
         elif type(config) == ConnectObject:
             header = config.getConfigHeader()
             config = config.getConfigObject()
         self.connector = connector.AdobeRequest(
-            config_object=config,
+            config=config,
             header=header,
             loggingEnabled=self.loggingEnabled,
             logger=self.logger,
         )
         self.header = self.connector.header
         self.header.update(**kwargs)
         if kwargs.get('sandbox',None) is not None: ## supporting sandbox setup on class instanciation
```

### Comparing `aepp-0.2.9/aepp/datasets.py` & `aepp-0.3.0/aepp/datasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+#  Copyright 2023 Adobe. All rights reserved.
+#  This file is licensed to you under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License. You may obtain a copy
+#  of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software distributed under
+#  the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
+#  OF ANY KIND, either express or implied. See the License for the specific language
+#  governing permissions and limitations under the License.
+
 import aepp
 from aepp import connector
 from copy import deepcopy
 import logging
 from typing import Union
 from .configs import ConnectObject
 
@@ -66,15 +76,15 @@
                 self.logger.addHandler(streamHandler)
         if type(config) == dict: ## Supporting either default setup or passing a ConnectObject
             config = config
         elif type(config) == ConnectObject:
             header = config.getConfigHeader()
             config = config.getConfigObject()
         self.connector = connector.AdobeRequest(
-            config_object=config,
+            config=config,
             header=header,
             loggingEnabled=self.loggingEnabled,
             logger=self.logger,
         )
         self.header = self.connector.header
         self.header.update(**kwargs)
         if kwargs.get('sandbox',None) is not None: ## supporting sandbox setup on class instanciation
```

### Comparing `aepp-0.2.9/aepp/destination.py` & `aepp-0.3.0/aepp/destination.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+#  Copyright 2023 Adobe. All rights reserved.
+#  This file is licensed to you under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License. You may obtain a copy
+#  of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software distributed under
+#  the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
+#  OF ANY KIND, either express or implied. See the License for the specific language
+#  governing permissions and limitations under the License.
+
 # Internal Library
 import aepp
 from aepp import connector
 from aepp import config
 from copy import deepcopy
 from typing import Union
 import time
@@ -49,15 +59,15 @@
                 self.logger.addHandler(streamHandler)
         if type(config) == dict: ## Supporting either default setup or passing a ConnectObject
             config = config
         elif type(config) == ConnectObject:
             header = config.getConfigHeader()
             config = config.getConfigObject()
         self.connector = connector.AdobeRequest(
-            config_object=config,
+            config=config,
             header=header,
             loggingEnabled=self.loggingEnabled,
             logger=self.logger,
         )
         self.header = self.connector.header
         # self.header.update({"Accept": "application/json"})
         self.header.update(**kwargs)
```

### Comparing `aepp-0.2.9/aepp/flowservice.py` & `aepp-0.3.0/aepp/flowservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+#  Copyright 2023 Adobe. All rights reserved.
+#  This file is licensed to you under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License. You may obtain a copy
+#  of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software distributed under
+#  the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
+#  OF ANY KIND, either express or implied. See the License for the specific language
+#  governing permissions and limitations under the License.
+
 import aepp
 from aepp import connector
 from copy import deepcopy
 import time,json
 import logging
 from dataclasses import dataclass
 from typing import Union
@@ -71,15 +81,15 @@
                 self.logger.addHandler(streamHandler)
         if type(config) == dict: ## Supporting either default setup or passing a ConnectObject
             config = config
         elif type(config) == ConnectObject:
             header = config.getConfigHeader()
             config = config.getConfigObject()
         self.connector = connector.AdobeRequest(
-            config_object=config,
+            config=config,
             header=header,
             loggingEnabled=self.loggingEnabled,
             logger=self.logger,
         )
         self.header = self.connector.header
         self.header.update(**kwargs)
         if kwargs.get('sandbox',None) is not None: ## supporting sandbox setup on class instanciation
@@ -1378,24 +1388,34 @@
                 header=aepp.config.header)->None:
         """
         Instantiate a Flow Manager Instance based on the flow ID.
         Arguments:
             flowId : REQUIRED : A flow ID
         """
         from aepp import schema, catalog,dataprep,flowservice
-        self.schemaAPI = schema.Schema()
-        self.catalogAPI = catalog.Catalog()
-        self.mapperAPI = dataprep.DataPrep()
-        self.flowAPI = flowservice.FlowService()
+        self.schemaAPI = schema.Schema(config=config)
+        self.catalogAPI = catalog.Catalog(config=config)
+        self.mapperAPI = dataprep.DataPrep(config=config)
+        self.flowAPI = flowservice.FlowService(config=config)
         self.flowData = self.flowAPI.getFlow(flowId)
         self.__setAttributes__(self.flowData)
         self.flowMapping = None
+        self.datasetId = None
         self.flowSpec = {'id' : self.flowData.get('flowSpec',{}).get('id')}
         self.flowSourceConnection = {'id' : self.flowData.get('sourceConnectionIds',[None])[0]}
         self.flowTargetConnection = {'id' : self.flowData.get('targetConnectionIds',[None])[0]}
+        sourceConnections:list = self.flowData.get('inheritedAttributes',{}).get('sourceConnections',[{}])
+        self.connectionInfo = {}
+        for element in sourceConnections:
+            if 'typeInfo' in element.keys():
+                self.connectionInfo = {'id':element.get('id'),'name':element.get('typeInfo',{}).get('id')}
+            if 'baseConnection' in element.keys():
+                self.connectionInfo = {'id':element.get('baseConnection',{}).get('id'),'name':None}
+        if self.connectionInfo.get('id',None) is not None and self.connectionInfo.get('name',None) is None:
+            self.connectionInfo['name'] = self.flowAPI.getConnection(self.connectionInfo['id']).get('items',[{}])[0].get('name')
         for trans in self.flowData.get('transformations',[{}]):
             if trans.get('name') == 'Mapping':
                 self.flowMapping = {'id':trans.get('params',{}).get('mappingId')}
         ## Flow Spec part
         if self.flowSpec['id'] is not None:
             flowSpecData = self.flowAPI.getFlowSpec(self.flowSpec['id'])
             self.flowSpec['name'] = flowSpecData['name']
@@ -1405,32 +1425,48 @@
             sourceConnData = self.flowAPI.getSourceConnection(self.flowSourceConnection['id'])
             self.flowSourceConnection['data'] = sourceConnData.get('data')
             self.flowSourceConnection['params'] = sourceConnData.get('params')
             self.flowSourceConnection['connectionSpec'] = sourceConnData.get('connectionSpec')
             if self.flowSourceConnection['connectionSpec'].get('id') is not None:
                 connSpec = self.flowAPI.getConnectionSpec(self.flowSourceConnection['connectionSpec'].get('id'))
                 self.flowSourceConnection['connectionSpec']['name'] = connSpec.get('name')
+            if connSpec.get('sourceSpec',{}).get('attributes',{}).get('uiAttributes',{}).get('isSource',False):
+                self.connectionType = 'source'
+            elif  connSpec.get('attributes',{}).get('isDestination',False):
+                self.connectionType = 'destination'
+            self.frequency = connSpec.get('sourceSpec',{}).get('attributes',{}).get('uiAttributes',{}).get('frequency',{}).get('key','unknown')
         ## Target Connection part
         if self.flowTargetConnection['id'] is not None:
             targetConnData = self.flowAPI.getTargetConnection(self.flowTargetConnection['id'])
-            self.flowTargetConnection['name'] = targetConnData.get('name')
-            self.flowTargetConnection['data'] = targetConnData.get('data')
-            self.flowTargetConnection['params'] = targetConnData.get('params')
-            self.flowTargetConnection['connectionSpec'] = targetConnData.get('connectionSpec')
-            if self.flowTargetConnection['connectionSpec'].get('id') is not None:
+            self.flowTargetConnection['name']:str = targetConnData.get('name')
+            self.flowTargetConnection['data']:dict = targetConnData.get('data',{})
+            self.flowTargetConnection['params']:dict = targetConnData.get('params',{})
+            for key, value in self.flowTargetConnection['params'].items():
+                if key == 'datasetId':
+                    self.datasetId = value
+            self.flowTargetConnection['connectionSpec']:dict = targetConnData.get('connectionSpec',{})
+            if self.flowTargetConnection['connectionSpec'].get('id',None) is not None:
                 connSpec = self.flowAPI.getConnectionSpec(self.flowSourceConnection['connectionSpec'].get('id'))
                 self.flowTargetConnection['connectionSpec']['name'] = connSpec.get('name')
         ## Catalog part
         if 'dataSetId' in self.flowTargetConnection['params'].keys():
             datasetInfo = self.catalogAPI.getDataSet(self.flowTargetConnection['params']['dataSetId'])
-            self.flowTargetConnection['params']['datasetName'] = datasetInfo[list(datasetInfo.keys())[0]].get('name')
+            if 'status' in datasetInfo.keys():
+                if datasetInfo['status'] == 404:
+                    self.flowTargetConnection['params']['datasetName'] = 'DELETED'
+            else:
+                self.flowTargetConnection['params']['datasetName'] = datasetInfo[list(datasetInfo.keys())[0]].get('name')
         ## Schema part
-        if 'schema' in self.flowTargetConnection['data'].keys():
-            schemaInfo = self.schemaAPI.getSchema(self.flowTargetConnection['data']['schema']['id'],full=False)
-            self.flowTargetConnection['data']['schema']['name'] = schemaInfo.get('title')
+        if 'schema' in self.flowTargetConnection.get('data',{}).keys():
+            if self.flowTargetConnection.get('data',{}).get('schema',None) is not None:
+                ## handling inconsistency in the response
+                schemaId = self.flowTargetConnection['data']['schema'].get('id',self.flowTargetConnection['data']['schema'].get('schemaId',None))
+                if schemaId is not None:
+                    schemaInfo = self.schemaAPI.getSchema(schemaId,full=False)
+                    self.flowTargetConnection['data']['schema']['name'] = schemaInfo.get('title')
         ## Mapping
         if self.flowMapping is not None:
             mappingInfo = self.mapperAPI.getMappingSet(self.flowMapping['id'])
             self.flowMapping['createdDate'] = time.ctime(mappingInfo.get('createdDate')/1000)
             self.flowMapping['createdDateTS'] = mappingInfo.get('createdDate')
             self.flowMapping['updatedAtTS'] = mappingInfo.get('updatedAt',None)
             if self.flowMapping['updatedAtTS'] is None:
@@ -1444,42 +1480,62 @@
         Set the attributes
         """
         self.id = flowData.get('id')
         self.etag = flowData.get('etag')
         self.sandbox = flowData.get('sandboxName')
         self.name = flowData.get('name')
         self.version = flowData.get('version')
+        self.state = flowData.get('state')
 
 
     def __repr__(self)->str:
         data = {
                 "id" : self.id,
                 "name": self.name,
                 "version":self.version,
+                "connectionName" : self.connectionInfo.get('name','unknown'),
+                "frequency" : self.frequency,
                 "flowSpecs": self.flowSpec,
                 "sourceConnection": self.flowSourceConnection,
                 "targetConnection": self.flowTargetConnection,
             }
         if self.flowMapping is not None:
             data['mapping'] = self.flowMapping
         return json.dumps(data,indent=2)
     
     def __str__(self)->str:
         data = {
                 "id" : self.id,
                 "name": self.name,
                 "version":self.version,
+                "connectionName" : self.connectionInfo.get('name','unknown'),
+                "frequency" : self.frequency,
                 "flowSpecs": self.flowSpec,
                 "sourceConnection": self.flowSourceConnection,
                 "targetConnection": self.flowTargetConnection,
             }
         if self.flowMapping is not None:
             data['mapping'] = self.flowMapping
         return json.dumps(data,indent=2)
 
+    def summary(self):
+        data = {
+                "id" : self.id,
+                "name": self.name,
+                "version":self.version,
+                "connectionName" : self.connectionInfo.get('name','unknown'),
+                "frequency" : self.frequency,
+                "flowSpecs": self.flowSpec,
+                "sourceConnection": self.flowSourceConnection,
+                "targetConnection": self.flowTargetConnection,
+            }
+        if self.flowMapping is not None:
+            data['mapping'] = self.flowMapping
+        return data
+
     def getFlowSpec(self)->dict:
         """
         Return a dictionary of the flow Spec.
         """
         if self.flowSpec['id'] is not None:
             flowSpecData = self.flowAPI.getFlowSpec(self.flowSpec['id'])
             return flowSpecData
```

### Comparing `aepp-0.2.9/aepp/identity.py` & `aepp-0.3.0/aepp/identity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+#  Copyright 2023 Adobe. All rights reserved.
+#  This file is licensed to you under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License. You may obtain a copy
+#  of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software distributed under
+#  the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
+#  OF ANY KIND, either express or implied. See the License for the specific language
+#  governing permissions and limitations under the License.
+
 import aepp
 from aepp import connector
 from copy import deepcopy
 import logging
 from typing import Union
 from .configs import ConnectObject
 
@@ -55,15 +65,15 @@
                 self.logger.addHandler(streamHandler)
         if type(config) == dict: ## Supporting either default setup or passing a ConnectObject
             config = config
         elif type(config) == ConnectObject:
             header = config.getConfigHeader()
             config = config.getConfigObject()
         self.connector = connector.AdobeRequest(
-            config_object=config,
+            config=config,
             header=header,
             loggingEnabled=self.loggingEnabled,
             logger=self.logger,
         )
         self.header = self.connector.header
         self.header.update(**kwargs)
         if kwargs.get('sandbox',None) is not None: ## supporting sandbox setup on class instanciation
```

### Comparing `aepp-0.2.9/aepp/ingestion.py` & `aepp-0.3.0/aepp/ingestion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+#  Copyright 2023 Adobe. All rights reserved.
+#  This file is licensed to you under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License. You may obtain a copy
+#  of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software distributed under
+#  the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
+#  OF ANY KIND, either express or implied. See the License for the specific language
+#  governing permissions and limitations under the License.
+
 import aepp
 from aepp import connector
 from copy import deepcopy
 import requests
 from typing import Union
 import logging
 import json
@@ -27,14 +37,15 @@
         """
         Instantiate the DataAccess class.
         Arguments:
             config : OPTIONAL : config object in the config module.
             header : OPTIONAL : header object  in the config module.
         Additional kwargs will update the header.
         """
+        requests.packages.urllib3.disable_warnings()
         if loggingObject is not None and sorted(
             ["level", "stream", "format", "filename", "file"]
         ) == sorted(list(loggingObject.keys())):
             self.loggingEnabled = True
             self.logger = logging.getLogger(f"{__name__}")
             self.logger.setLevel(loggingObject["level"])
             if type(loggingObject["format"]) == str:
@@ -51,15 +62,15 @@
                 self.logger.addHandler(streamHandler)
         if type(config) == dict: ## Supporting either default setup or passing a ConnectObject
             config = config
         elif type(config) == ConnectObject:
             header = config.getConfigHeader()
             config = config.getConfigObject()
         self.connector = connector.AdobeRequest(
-            config_object=config, 
+            config=config, 
             header=header,
             logger=self.logger,
             loggingEnabled=self.loggingEnabled)
         self.header = self.connector.header
         self.header.update(**kwargs)
         if kwargs.get('sandbox',None) is not None: ## supporting sandbox setup on class instanciation
             self.sandbox = kwargs.get('sandbox')
@@ -316,15 +327,15 @@
             raise Exception("require the content range to be passed")
         privateHeader = deepcopy(self.header)
         privateHeader["Content-Type"] = "application/octet-stream"
         privateHeader["Content-Range"] = contentRange
         if self.loggingEnabled:
             self.logger.debug(f"Uploading large part for batch ID: ({batchId})")
         path = f"/batches/{batchId}/datasets/{datasetId}/files/{filePath}"
-        res = requests.patch(self.endpoint + path, data=data, headers=privateHeader)
+        res = requests.patch(self.endpoint + path, data=data, headers=privateHeader, verify=False)
         res_json = res.json()
         return res_json
 
     def headFileStatus(
         self, batchId: str = None, datasetId: str = None, filePath: str = None
     ) -> dict:
         """
```

### Comparing `aepp-0.2.9/aepp/observability.py` & `aepp-0.3.0/aepp/sandboxes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,49 @@
+#  Copyright 2023 Adobe. All rights reserved.
+#  This file is licensed to you under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License. You may obtain a copy
+#  of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software distributed under
+#  the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
+#  OF ANY KIND, either express or implied. See the License for the specific language
+#  governing permissions and limitations under the License.
+
 import aepp
 from aepp import connector
-import pandas as pd
 import logging
 from typing import Union
 from .configs import ConnectObject
 
-class Observability:
+
+class Sandboxes:
     """
-    A class that presents the different methods available on the Observability API from AEP.
-    A complete documentation of the methods can be found here:
-    https://www.adobe.io/apis/experienceplatform/home/api-reference.html#!acpdr/swagger-specs/observability-insights.yaml
+    A collection of methods to realize actions on the sandboxes.
+    It comes from the sandbox API:
+    https://www.adobe.io/apis/experienceplatform/home/api-reference.html#!acpdr/swagger-specs/sandbox-api.yaml
     """
 
     ## logging capability
     loggingEnabled = False
     logger = None
 
     def __init__(
         self,
         config: Union[dict,ConnectObject] = aepp.config.config_object,
         header: dict = aepp.config.header,
         loggingObject: dict = None,
         **kwargs,
-    ) -> None:
+    ):
         """
-        Instanciate the observability API methods class.
+        Instantiate the sandbox class.
         Arguments:
-            loggingObject : OPTIONAL : logging object to log messages.
             config : OPTIONAL : config object in the config module. (DO NOT MODIFY)
             header : OPTIONAL : header object  in the config module. (DO NOT MODIFY)
+            loggingObject : OPTIONAL : logging object to log messages.
+        Additional kwargs will update the header.
         """
         if loggingObject is not None and sorted(
             ["level", "stream", "format", "filename", "file"]
         ) == sorted(list(loggingObject.keys())):
             self.loggingEnabled = True
             self.logger = logging.getLogger(f"{__name__}")
             self.logger.setLevel(loggingObject["level"])
@@ -50,150 +61,132 @@
                 self.logger.addHandler(streamHandler)
         if type(config) == dict: ## Supporting either default setup or passing a ConnectObject
             config = config
         elif type(config) == ConnectObject:
             header = config.getConfigHeader()
             config = config.getConfigObject()
         self.connector = connector.AdobeRequest(
-            config_object=config,
+            config=config,
             header=header,
             loggingEnabled=self.loggingEnabled,
-            logger=self.logger,
+            loggingObject=self.logger,
         )
         self.header = self.connector.header
         self.header.update(**kwargs)
         if kwargs.get('sandbox',None) is not None: ## supporting sandbox setup on class instanciation
             self.sandbox = kwargs.get('sandbox')
             self.connector.config["sandbox"] = kwargs.get('sandbox')
             self.header.update({"x-sandbox-name":kwargs.get('sandbox')})
             self.connector.header.update({"x-sandbox-name":kwargs.get('sandbox')})
         else:
             self.sandbox = self.connector.config["sandbox"]
         self.endpoint = (
-            aepp.config.endpoints["global"] + aepp.config.endpoints["observability"]
+            aepp.config.endpoints["global"] + aepp.config.endpoints["sandboxes"]
         )
-        self.POST_METRICS = {
-            "start": "2020-07-14T00:00:00.000Z",
-            "end": "2020-07-22T00:00:00.000Z",
-            "granularity": "day",
-            "metrics": [
-                {
-                    "name": "timeseries.ingestion.dataset.recordsuccess.count",
-                    "filters": [
-                        {
-                            "name": "dataSetId",
-                            "value": "5edcfb2fbb642119194c7d94|5eddb21420f516191b7a8dad",
-                            "groupBy": True,
-                        }
-                    ],
-                    "aggregator": "sum",
-                    "downsample": "sum",
-                },
-                {
-                    "name": "timeseries.ingestion.dataset.dailysize",
-                    "filters": [
-                        {
-                            "name": "dataSetId",
-                            "value": "5eddb21420f516191b7a8dad",
-                            "groupBy": False,
-                        }
-                    ],
-                    "aggregator": "sum",
-                    "downsample": "sum",
-                },
-            ],
-        }
-        self._loadREFERENCES()
-
-    def _loadREFERENCES(self):
-        """
-        Load document as attributes if possible
-        """
-        if self.loggingEnabled:
-            self.logger.debug(f"Loading references")
-        try:
-            import importlib.resources as pkg_resources
-
-            pathIdentity = pkg_resources.path("aepp", "observability_identity.pickle")
-            pathIngestion = pkg_resources.path("aepp", "observability_ingestion.pickle")
-            pathGDPR = pkg_resources.path("aepp", "observability_gdpr.pickle")
-            pathQS = pkg_resources.path("aepp", "observability_queryService.pickle")
-            pathRLTime = pkg_resources.path("aepp", "observability_realTime.pickle")
-        except ImportError:
-            # Try backported to PY<37 with pkg_resources.
-            if self.loggingEnabled:
-                self.logger.debug(f"Loading references - ImportError - 2nd try")
-            try:
-                import pkg_resources
-
-                pathIdentity = pkg_resources.resource_filename(
-                    "aepp", "observability_identity.pickle"
-                )
-                pathIngestion = pkg_resources.resource_filename(
-                    "aepp", "observability_ingestion.pickle"
-                )
-                pathGDPR = pkg_resources.resource_filename(
-                    "aepp", "observability_gdpr.pickle"
-                )
-                pathQS = pkg_resources.resource_filename(
-                    "aepp", "observability_queryService.pickle"
-                )
-                pathRLTime = pkg_resources.resource_filename(
-                    "aepp", "observability_realTime.pickle"
-                )
-            except:
-                print("no supported files")
-                if self.loggingEnabled:
-                    self.logger.debug(f"Failed loading references")
-        try:
-            with pathIdentity as f:
-                self.REFERENCE_IDENTITY = pd.read_pickle(f)
-                self.REFERENCE_IDENTITY = self.REFERENCE_IDENTITY.style.set_properties(
-                    subset=["Insights metric"], **{"width": "100px"}
-                )
-            with pathIngestion as f:
-                self.REFERENCE_INGESTION = pd.read_pickle(f)
-                self.REFERENCE_INGESTION = (
-                    self.REFERENCE_INGESTION.style.set_properties(
-                        subset=["Insights metric"], **{"width": "100px"}
-                    )
-                )
-            with pathGDPR as f:
-                self.REFERENCE_GDPR = pd.read_pickle(f)
-                self.REFERENCE_GDPR = self.REFERENCE_GDPR.style.set_properties(
-                    subset=["Insights metric"], **{"width": "100px"}
-                )
-            with pathRLTime as f:
-                self.REFERENCE_REALTIME = pd.read_pickle(f)
-                self.REFERENCE_REALTIME = self.REFERENCE_REALTIME.style.set_properties(
-                    subset=["Insights metric"], **{"width": "100px"}
-                )
-            with pathQS as f:
-                self.REFERENCE_QUERYSERVICE = pd.read_pickle(f)
-                self.REFERENCE_QUERYSERVICE = (
-                    self.REFERENCE_QUERYSERVICE.style.set_properties(
-                        subset=["Insights metric"], **{"width": "100px"}
-                    )
-                )
-        except:
-            if self.loggingEnabled:
-                self.logger.debug(f"Failed loading references - backup to None")
-            self.REFERENCE_IDENTITY = None
-            self.REFERENCE_INGESTION = None
-            self.REFERENCE_QUERYSERVICE = None
-            self.REFERENCE_GDPR = None
-            self.REFERENCE_REALTIME = None
-
-    def createMetricsReport(self, data: dict = None) -> dict:
-        """
-        Using the POST method to retrieve metrics specified in the data dictionary.
-        Please use the different REFERENCES attributes to know which metrics are supported.
-        You have a template for the data dictionary on the POST_METRICS attribute.
+
+    def getSandboxes(self) -> list:
+        """
+        Return the list of all the sandboxes
+        """
+        if self.loggingEnabled:
+            self.logger.debug(f"Starting getSandboxes")
+        path = self.endpoint + "/sandboxes"
+        res = self.connector.getData(path)
+        data = res["sandboxes"]
+        return data
+
+    def getSandboxTypes(self) -> list:
+        """
+        Return the list of all the sandboxes types.
+        """
+        if self.loggingEnabled:
+            self.logger.debug(f"Starting getSandboxTyoes")
+        path = self.endpoint + "/sandboxTypes"
+        res = self.connector.getData(path)
+        data = res["sandboxTypes"]
+        return data
+
+    def createSandbox(
+        self, name: str = None, title: str = None, type_sandbox: str = "development"
+    ) -> dict:
+        """
+        Create a new sandbox in your AEP instance.
+        Arguments:
+            name : REQUIRED : name of your sandbox
+            title : REQUIRED : display name of your sandbox
+            type_sandbox : OPTIONAL : type of your sandbox. default : development.
+        """
+        if name is None or title is None:
+            raise Exception("name and title cannot be empty")
+        if self.loggingEnabled:
+            self.logger.debug(f"Starting createSandbox")
+        path = self.endpoint + "/sandboxes"
+        data = {"name": name, "title": title, "type": type_sandbox}
+        res = self.connector.postData(path, data=data)
+        return res
+
+    def getSandbox(self, name: str) -> dict:
+        """
+        retrieve a Sandbox information by name
+        Argument:
+            name : REQUIRED : name of Sandbox
+        """
+        if name is None:
+            raise Exception("Expected a name as parameter")
+        if self.loggingEnabled:
+            self.logger.debug(f"Starting getSandbox")
+        path = self.endpoint + f"/sandboxes/{name}"
+        res = self.connector.getData(path)
+        return res
+
+    def getSandboxId(self, name: str) -> str:
+        """
+        Retrieve the ID of a sandbox by name.
+        Argument:
+            name : REQUIRED : name of Sandbox
+        """
+        return self.getSandbox(name)["id"]
+
+    def deleteSandbox(self, name: str) -> dict:
+        """
+        Delete a sandbox by its name.
+        Arguments:
+            name : REQUIRED : sandbox to be deleted.
+        """
+        if name is None:
+            raise Exception("Expected a name as parameter")
+        if self.loggingEnabled:
+            self.logger.debug(f"Starting deleteSandbox")
+        path = self.endpoint + f"/sandboxes/{name}"
+        res = self.connector.deleteData(path)
+        return res
+
+    def resetSandbox(self, name: str) -> dict:
+        """
+        Reset a sandbox by its name. Sandbox will be empty.
+        Arguments:
+            name : REQUIRED : sandbox name to be deleted.
+        """
+        if name is None:
+            raise Exception("Expected a sandbox name as parameter")
+        if self.loggingEnabled:
+            self.logger.debug(f"Starting resetSandbox")
+        path = self.endpoint + f"/sandboxes/{name}"
+        res = self.connector.putData(path, data={'action':'reset'})
+        return res
+
+    def updateSandbox(self, name: str, action: dict = None) -> dict:
+        """
+        Update the Sandbox with the action provided.
         Arguments:
-            data : REQUIRED : The metrics requested in the report creation.
-                You can use the POST_METRICS attribute to see a template.
+            name : REQUIRED : sandbox name to be updated.
+            action : REQUIRED : dictionary defining the action to realize on that sandbox.
         """
+        if name is None:
+            raise Exception("Expected a sandbox name as parameter")
+        if action is None or type(action) != dict:
+            raise Exception("Expected a dictionary to pass the action")
         if self.loggingEnabled:
-            self.logger.debug(f"Starting createMetricsReport")
-        path = "/metrics"
-        res = self.connector.postData(self.endpoint + path, data=data)
+            self.logger.debug(f"Starting updateSandboxes")
+        path = self.endpoint + f"/sandboxes/{name}"
+        res = self.connector.patchData(path, data=action)
         return res
```

### Comparing `aepp-0.2.9/aepp/policy.py` & `aepp-0.3.0/aepp/policy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+#  Copyright 2023 Adobe. All rights reserved.
+#  This file is licensed to you under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License. You may obtain a copy
+#  of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software distributed under
+#  the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
+#  OF ANY KIND, either express or implied. See the License for the specific language
+#  governing permissions and limitations under the License.
+
 import aepp
 import typing
 from aepp import connector
 import logging
 from .configs import ConnectObject
 
 class Policy:
@@ -48,15 +58,15 @@
                 self.logger.addHandler(streamHandler)
         if type(config) == dict: ## Supporting either default setup or passing a ConnectObject
             config = config
         elif type(config) == ConnectObject:
             header = config.getConfigHeader()
             config = config.getConfigObject()
         self.connector = connector.AdobeRequest(
-            config_object=config,
+            config=config,
             header=header,
             loggingEnabled=self.loggingEnabled,
             loggingObject=self.logger,
         )
         self.header = self.connector.header
         self.header.update(**kwargs)
         if kwargs.get('sandbox',None) is not None: ## supporting sandbox setup on class instanciation
```

### Comparing `aepp-0.2.9/aepp/privacyservice.py` & `aepp-0.3.0/aepp/privacyservice.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+#  Copyright 2023 Adobe. All rights reserved.
+#  This file is licensed to you under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License. You may obtain a copy
+#  of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software distributed under
+#  the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
+#  OF ANY KIND, either express or implied. See the License for the specific language
+#  governing permissions and limitations under the License.
+
 import aepp
 from aepp import connector
 import logging
 from typing import Union
 from .configs import ConnectObject
 
 class Privacy:
@@ -96,15 +106,15 @@
                 self.logger.addHandler(streamHandler)
         if type(config) == dict: ## Supporting either default setup or passing a ConnectObject
             config = config
         elif type(config) == ConnectObject:
             header = config.getConfigHeader()
             config = config.getConfigObject()
         self.connector = connector.AdobeRequest(
-            config_object=config,
+            config=config,
             header=header,
             aepScope=aepScope,
             privacyScope=privacyScope,
             loggingEnabled=self.loggingEnabled,
             logger=self.logger,
         )
         self.header = self.connector.header
```

### Comparing `aepp-0.2.9/aepp/queryservice.py` & `aepp-0.3.0/aepp/queryservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+#  Copyright 2023 Adobe. All rights reserved.
+#  This file is licensed to you under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License. You may obtain a copy
+#  of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software distributed under
+#  the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
+#  OF ANY KIND, either express or implied. See the License for the specific language
+#  governing permissions and limitations under the License.
+
 # Internal Library
 from aepp import connector
 import pandas as pd
 from typing import Union
 import re
 import aepp
 import time
@@ -95,15 +105,15 @@
                 self.logger.addHandler(streamHandler)
         if type(config) == dict: ## Supporting either default setup or passing a ConnectObject
             config = config
         elif type(config) == ConnectObject:
             header = config.getConfigHeader()
             config = config.getConfigObject()
         self.connector = connector.AdobeRequest(
-            config_object=config,
+            config=config,
             header=header,
             loggingEnabled=self.loggingEnabled,
             logger=self.logger,
         )
         self.header = self.connector.header
         # self.header.update({"Accept": "application/json"})
         self.header.update(**kwargs)
```

### Comparing `aepp-0.2.9/aepp/schema.py` & `aepp-0.3.0/aepp/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+#  Copyright 2023 Adobe. All rights reserved.
+#  This file is licensed to you under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License. You may obtain a copy
+#  of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software distributed under
+#  the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
+#  OF ANY KIND, either express or implied. See the License for the specific language
+#  governing permissions and limitations under the License.
+
 # Internal Library
 import aepp
 from dataclasses import dataclass
 from aepp import connector
 from copy import deepcopy
 from typing import Union
 import time
@@ -94,15 +104,15 @@
                 self.logger.addHandler(streamHandler)
         if type(config) == dict: ## Supporting either default setup or passing a ConnectObject
             config = config
         elif type(config) == ConnectObject:
             header = config.getConfigHeader()
             config = config.getConfigObject()
         self.connector = connector.AdobeRequest(
-            config_object=config,
+            config=config,
             header=header,
             loggingEnabled=self.loggingEnabled,
             logger=self.logger,
         )
         self.header = self.connector.header
         self.header["Accept"] = "application/vnd.adobe.xed+json"
         self.connector.header['Accept'] = "application/vnd.adobe.xed+json"
@@ -1950,32 +1960,48 @@
                 If you pass the $id or altId, you should pass the schemaAPI instance or have uploaded a configuration file.
             title : OPTIONAL : If you want to name the field group.
             fg_class : OPTIONAL : the class that will support this field group.
                 by default events and profile, possible value : "record"
             schemaAPI : OPTIONAL : The instance of the Schema class. Provide a way to connect to the API.
             config : OPTIONAL : The config object in case you want to override the configuration.
         """
-        
+        self.EDITABLE = False
         self.fieldGroup = {}
-        if schemaAPI is not None:
+        if schemaAPI is not None and type(schemaAPI) == 'Schema':
             self.schemaAPI = schemaAPI
         else:
             self.schemaAPI = Schema(config=config)
         self.tenantId = f"_{self.schemaAPI.getTenantId()}"
         if fieldGroup is not None:
             if type(fieldGroup) == dict:
                 if fieldGroup.get("meta:resourceType",None) == "mixins":
-                    self.fieldGroup = fieldGroup
+                    if fieldGroup.get('definitions',None) is not None:
+                        if 'mixins' in fieldGroup.get('$id'):
+                            self.EDITABLE = True
+                            self.fieldGroup = self.schemaAPI.getFieldGroup(fieldGroup['$id'],full=False)
+                        else:
+                            tmp_def = self.schemaAPI.getFieldGroup(fieldGroup['$id'],full=True) ## handling default mixins
+                            tmp_def['definitions'] = tmp_def['properties']
+                            self.fieldGroup = tmp_def
+                    else:
+                        self.fieldGroup = self.schemaAPI.getFieldGroup(fieldGroup['$id'],full=False)
             elif type(fieldGroup) == str and (fieldGroup.startswith('https:') or fieldGroup.startswith(f'{self.tenantId}.')):
                 if self.schemaAPI is None:
                     raise Exception("You try to retrieve the fieldGroup definition from the id, but no API has been passed in the schemaAPI parameter.")
-                self.fieldGroup = self.schemaAPI.getFieldGroup(fieldGroup,full=False)
+                if 'mixins' in fieldGroup:
+                    self.EDITABLE = True
+                    self.fieldGroup = self.schemaAPI.getFieldGroup(fieldGroup,full=False)
+                else: ## handling default mixins
+                    tmp_def = self.schemaAPI.getFieldGroup(fieldGroup,full=True) ## handling default mixins
+                    tmp_def['definitions'] = tmp_def['properties']
+                    self.fieldGroup = tmp_def
             else:
                 raise ValueError("the element pass is not a field group definition")
         else:
+            self.EDITABLE = True
             self.fieldGroup = {
                 "title" : "",
                 "meta:resourceType":"mixins",
                 "description" : "",
                 "type": "object",
                 "definitions":{
                     "customFields":{
@@ -2013,14 +2039,20 @@
                 for cls in fg_class:
                     if 'experienceevent' in cls or "https://ns.adobe.com/xdm/context/experienceevent" ==cls:
                         self.fieldGroup["meta:intendedToExtend"].append("https://ns.adobe.com/xdm/context/experienceevent")
                     elif "profile" in cls or "https://ns.adobe.com/xdm/context/profile" == cls:
                         self.fieldGroup["meta:intendedToExtend"].append("https://ns.adobe.com/xdm/context/profile")
                     elif "record" in cls or "https://ns.adobe.com/xdm/data/record" == cls:
                         self.fieldGroup["meta:intendedToExtend"].append("https://ns.adobe.com/xdm/context/profile")
+        if len(self.fieldGroup.get('allOf',[]))>1:
+            ### handling the custom field group based on existing ootb field groups
+            for element in self.fieldGroup.get('allOf'):
+                if element.get('$ref') != '#/definitions/customFields' and element.get('$ref') != '#/definitions/property':
+                    additionalDefinition = self.schemaAPI.getFieldGroup(element.get('$ref'),full=True)
+                    self.fieldGroup['definitions'] = self.__simpleDeepMerge__(self.fieldGroup['definitions'],additionalDefinition.get('properties'))
         self.__setAttributes__(self.fieldGroup)
         if title is not None:
             self.fieldGroup['title'] = title
             self.title = title
         
     
     def __setAttributes__(self,fieldGroup:dict)->None:
@@ -2295,15 +2327,15 @@
                 dictionary['querypath'] = []
             if description:
                 dictionary['description'] = []
         else:
             dictionary = dictionary
         for key in mydict:
             if type(mydict[key]) == dict:
-                if mydict[key].get('type') == 'object':
+                if mydict[key].get('type') == 'object' or 'properties' in mydict[key].keys():
                     if path is None:
                         if key != "property" and key != "customFields":
                             tmp_path = key
                         else:
                             tmp_path = None
                     else:
                         tmp_path = f"{path}.{key}"
@@ -2598,15 +2630,14 @@
 
     def addField(self,path:str,dataType:str=None,title:str=None,objectComponents:dict=None,array:bool=False,enumValues:dict=None,**kwargs)->dict:
         """
         Add the field to the existing fieldgroup definition.
         Returns False when the field could not be inserted.
         Arguments:
             path : REQUIRED : path with dot notation where you want to create that new field. New field name should be included.
-                In case of array of objects, use the "[*]" notation
             dataType : REQUIRED : the field type you want to create
                 A type can be any of the following: "string","boolean","double","long","integer","short","byte","date","dateTime","boolean","object","array"
                 NOTE : "array" type is to be used for array of objects. If the type is string array, use the boolean "array" parameter.
             title : OPTIONAL : if you want to have a custom title.
             objectComponents: OPTIONAL : A dictionary with the name of the fields contain in the "object" or "array of objects" specify, with their typed.
                 Example : {'field1:'string','field2':'double'}
             array : OPTIONAL : Boolean. If the element to create is an array. False by default.
@@ -2728,36 +2759,56 @@
             operation : REQUIRED : The list of operation to realise
         """
         if operations is None or type(operations) != list:
             raise ValueError('Require a list of operations')
         if self.schemaAPI is None:
             Exception('Require a schema API connection. Pass the instance of a Schema class or import a configuration file.')
         res = self.schemaAPI.patchFieldGroup(self.id,operations)
+        if 'status' in res.keys():
+            if res['status'] >= 400:
+                print(res['title'])
+                return res
+            else:
+                return res
         self.fieldGroup = res
         self.__setAttributes__(self.fieldGroup)
         return res
     
     def updateFieldGroup(self)->dict:
         """
         Use the PUT method to push the current field group representation to AEP via API request.
         """
         if self.schemaAPI is None:
             Exception('Require a schema API connection. Pass the instance of a Schema class or import a configuration file.')
         res = self.schemaAPI.putFieldGroup(self.id,self.to_xdm())
+        if 'status' in res.keys():
+            if res['status'] >= 400:
+                print(res['title'])
+                return res
+            else:
+                return res
         self.fieldGroup = res
         self.__setAttributes__(self.fieldGroup)
         return res
     
     def createFieldGroup(self)->dict:
         """
         Use the POST method to create the field group in the organization.
         """
         if self.schemaAPI is None:
             Exception('Require a schema API connection. Pass the instance of a Schema class or import a configuration file.')
         res = self.schemaAPI.createFieldGroup(self.to_xdm())
+        if 'status' in res.keys():
+            if res['status'] >= 400:
+                print(res['title'])
+                return res
+            else:
+                return res
+        self.fieldGroup = res
+        self.__setAttributes__(self.fieldGroup)
         return res
 
 
 class SchemaManager:
     """
     A class to handle the schema management.
     """
@@ -2803,14 +2854,15 @@
                 Warning("No schema instance has been passed or config file imported.\n Aborting the creation of field Group Manager")
             else:
                 for ref in self.fieldGroupIds:
                     if '/mixins/' in ref:
                         definition = self.schemaAPI.getFieldGroup(ref,full=False)
                     else:
                         definition = self.schemaAPI.getFieldGroup(ref,full=True)
+                        definition['definitions'] = definition['properties']
                     self.fieldGroupsManagers.append(FieldGroupManager(fieldGroup=definition))
         elif type(schema) == str:
             if self.schemaAPI is None:
                 Warning("No schema instance has been passed or config file imported.\n Aborting the retrieveal of the Schema Definition")
             else:
                 self.schema = self.schemaAPI.getSchema(schema,full=False)
                 self.__setAttributes__(self.schema)
@@ -2820,14 +2872,15 @@
                     Warning("fgManager is set to True but no schema instance has been passed.\n Aborting the creation of field Group Manager")
                 else:
                     for ref in self.fieldGroupIds:
                         if '/mixins/' in ref:
                             definition = self.schemaAPI.getFieldGroup(ref,full=False)
                         else:
                             definition = self.schemaAPI.getFieldGroup(ref,full=True)
+                            definition['definitions'] = definition['properties']
                         self.fieldGroupsManagers.append(FieldGroupManager(fieldGroup=definition))
         elif schema is None:
             self.schema = {
                     "title": None,
                     "description": "power by aepp",
                     "allOf": [
                             {
@@ -3031,14 +3084,20 @@
     def updateSchema(self)->dict:
         """
         Use the PUT method to replace the existing schema with the new definition.
         """
         if self.schemaAPI is None:
             raise Exception("Require a Schema instance to connect to the API")
         res = self.schemaAPI.putSchema(self.id,self.schema)
+        if 'status' in res.keys():
+            if res['status'] == 400:
+                print(res['title'])
+                return res
+            else:
+                return res
         self.schema = res
         self.__setAttributes__(self.schema)
         return res
     
     def createDescriptorOperation(self,descType:str=None,
                                 completePath:str=None,
                                 identityNSCode:str=None,
@@ -3052,14 +3111,15 @@
         Create a descriptor object to be used in the createDescriptor.
         You can see the type of descriptor available in the DESCRIPTOR_TYPES attribute and also on the official documentation:
         https://experienceleague.adobe.com/docs/experience-platform/xdm/api/descriptors.html?lang=en#appendix
         Arguments:
             descType : REQUIRED : The type to be used.
                 it can only be one of the following value: "xdm:descriptorIdentity","xdm:alternateDisplayInfo","xdm:descriptorOneToOne","xdm:descriptorReferenceIdentity","xdm:descriptorDeprecated"
             completePath : REQUIRED : the complete path of the field you want to attach a descriptor.
+                Example: '/definitions/customFields/properties/_tenant/properties/tenantObject/properties/field'
             identityNSCode : OPTIONAL : if the descriptor is identity related, the namespace CODE  used.
             identityPrimary : OPTIONAL : If the primary descriptor added is the primary identity.
             alternateTitle : OPTIONAL : if the descriptor is alternateDisplay, the alternate title to be used.
             alternateDescription : OPTIONAL if you wish to add a new description.
             lookupSchema : OPTIONAL : The schema ID for the lookup if the descriptor is for lookup setup
             targetCompletePath : OPTIONAL : if you have the complete path for the field in the target lookup schema.
         """
@@ -3126,8 +3186,24 @@
         Create a descriptor attached to that class bsaed on the creatorDescriptor operation provided. 
         Arguments:
             descriptor : REQUIRED : The operation to add a descriptor to the schema.
         """
         if descriptor is None:
             raise ValueError('Require an operation to be used')
         res = self.schemaAPI.createDescriptor(descriptor)
-        return res
+        return res
+
+    def compareObservableSchema(self,observableSchemaManager:'ObservableSchemaManager'=None)->pd.DataFrame:
+        """
+        A method to compare the existing schema with the observable schema and find out the difference in them.
+        It output a dataframe with all of the path, the field group, the type (if provided) and the part availability (in that dataset)
+        Arguments:
+            observableSchemaManager : REQUIRED : the ObservableSchemaManager class instance.
+        """
+        df_schema = self.to_dataframe()
+        df_obs = observableSchemaManager.to_dataframe()
+        df_merge = df_schema.merge(df_obs,left_on='path',right_on='path',how='left',indicator=True)
+        df_merge = df_merge.rename(columns={"_merge": "availability",'type_x':'type'})
+        df_merge = df_merge.drop("type_y",axis=1)
+        df_merge['availability'] = df_merge['availability'].str.replace('left_only','schema_only')
+        df_merge['availability'] = df_merge['availability'].str.replace('both','schema_dataset')
+        return df_merge
```

### Comparing `aepp-0.2.9/aepp/segmentation.py` & `aepp-0.3.0/aepp/segmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+#  Copyright 2023 Adobe. All rights reserved.
+#  This file is licensed to you under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License. You may obtain a copy
+#  of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software distributed under
+#  the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
+#  OF ANY KIND, either express or implied. See the License for the specific language
+#  governing permissions and limitations under the License.
+
 # Internal Library
 import aepp
 from aepp import connector
 import time
 from concurrent import futures
 import logging
 from typing import Union
@@ -91,15 +101,15 @@
                 self.logger.addHandler(streamHandler)
         if type(config) == dict: ## Supporting either default setup or passing a ConnectObject
             config = config
         elif type(config) == ConnectObject:
             header = config.getConfigHeader()
             config = config.getConfigObject()
         self.connector = connector.AdobeRequest(
-            config_object=config,
+            config=config,
             header=header,
             loggingEnabled=self.loggingEnabled,
             logger=self.logger,
         )
         self.header = self.connector.header
         self.header.update(**kwargs)
         if kwargs.get('sandbox',None) is not None: ## supporting sandbox setup on class instanciation
```

### Comparing `aepp-0.2.9/aepp/sensei.py` & `aepp-0.3.0/aepp/sensei.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+#  Copyright 2023 Adobe. All rights reserved.
+#  This file is licensed to you under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License. You may obtain a copy
+#  of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software distributed under
+#  the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
+#  OF ANY KIND, either express or implied. See the License for the specific language
+#  governing permissions and limitations under the License.
+
 # internal library
 import aepp
 from aepp import connector
 import logging
 from copy import deepcopy
 from typing import Union
 from .configs import ConnectObject
@@ -52,15 +62,15 @@
                 self.logger.addHandler(streamHandler)
         if type(config) == dict: ## Supporting either default setup or passing a ConnectObject
             config = config
         elif type(config) == ConnectObject:
             header = config.getConfigHeader()
             config = config.getConfigObject()
         self.connector = connector.AdobeRequest(
-            config_object=config,
+            config=config,
             header=header,
             loggingEnabled=self.loggingEnabled,
             logger=self.logger,
         )
         self.header = self.connector.header
         self.header[
             "Accept"
```

### Comparing `aepp-0.2.9/aepp.egg-info/PKG-INFO` & `aepp-0.3.0/aepp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: aepp
-Version: 0.2.9
+Version: 0.3.0
 Summary: Package to manage AEP API endpoint and some helper functions
-Home-page: https://github.com/pitchmuc/aep
+Home-page: https://github.com/adobe/aepp
 Author: Julien Piccini
 Author-email: piccini.julien@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Utilities
 Classifier: Topic :: Internet
@@ -71,15 +71,15 @@
 * [flowservice](./docs/flowservice.md)
 * [policy](./docs/policy.md)
 * [datasets](./docs/datasets.md)
 * [ingestion](./docs/ingestion.md)
 * [destination Authoring](./docs/destination.md)
 * [destination Instance](./docs/destinationinstanceservice.md)
 * [observability](./docs/observability.md)
-* accesscontrol
+* [accesscontrol](./docs/accesscontrol.md)
 * sensei
 * [privacyservice](./docs/privacyservice.md) (see 2nd note below)
 
 Last but not least, the core methods are described here: [main](./docs/main.md)
 
 ## queryservice module
```

### Comparing `aepp-0.2.9/aepp.egg-info/SOURCES.txt` & `aepp-0.3.0/aepp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aepp-0.2.9/tests/catalog_test.py` & `aepp-0.3.0/tests/catalog_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+#  Copyright 2023 Adobe. All rights reserved.
+#  This file is licensed to you under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License. You may obtain a copy
+#  of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software distributed under
+#  the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
+#  OF ANY KIND, either express or implied. See the License for the specific language
+#  governing permissions and limitations under the License.
+
 from aepp.schema import Schema
 import unittest
 from unittest.mock import patch, MagicMock
 
 
 class CatalogTest(unittest.TestCase):
```

### Comparing `aepp-0.2.9/tests/destinationinstanceservice_test.py` & `aepp-0.3.0/tests/destinationinstanceservice_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+#  Copyright 2023 Adobe. All rights reserved.
+#  This file is licensed to you under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License. You may obtain a copy
+#  of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software distributed under
+#  the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
+#  OF ANY KIND, either express or implied. See the License for the specific language
+#  governing permissions and limitations under the License.
+
 from aepp.destinationinstanceservice import DestinationInstanceService
 import unittest
 from unittest.mock import patch, MagicMock, ANY
 
 
 class DestinationInstanceServiceTest(unittest.TestCase):
     ADHOC_INPUT = {"flow1": ["dataset1"], "flow2": ["dataset2", "dataset3"]}
```

