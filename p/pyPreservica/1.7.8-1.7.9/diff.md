# Comparing `tmp/pyPreservica-1.7.8.tar.gz` & `tmp/pyPreservica-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPreservica-1.7.8.tar", last modified: Tue May 16 13:55:41 2023, max compression
+gzip compressed data, was "pyPreservica-1.7.9.tar", last modified: Wed May 24 09:28:40 2023, max compression
```

## Comparing `pyPreservica-1.7.8.tar` & `pyPreservica-1.7.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 13:55:41.164294 pyPreservica-1.7.8/
--rw-rw-rw-   0        0        0    11558 2020-08-17 10:38:19.000000 pyPreservica-1.7.8/LICENSE.txt
--rw-rw-rw-   0        0        0     2581 2023-05-16 13:55:41.162182 pyPreservica-1.7.8/PKG-INFO
--rw-rw-rw-   0        0        0     1602 2022-03-16 17:04:00.000000 pyPreservica-1.7.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 13:55:41.111426 pyPreservica-1.7.8/pyPreservica/
--rw-rw-rw-   0        0        0     1037 2023-05-16 13:21:35.000000 pyPreservica-1.7.8/pyPreservica/__init__.py
--rw-rw-rw-   0        0        0    37685 2023-05-03 10:58:47.000000 pyPreservica-1.7.8/pyPreservica/adminAPI.py
--rw-rw-rw-   0        0        0    32269 2023-05-03 10:51:09.000000 pyPreservica-1.7.8/pyPreservica/common.py
--rw-rw-rw-   0        0        0    16189 2023-03-01 16:04:47.000000 pyPreservica-1.7.8/pyPreservica/contentAPI.py
--rw-rw-rw-   0        0        0   105659 2023-03-01 16:04:03.000000 pyPreservica-1.7.8/pyPreservica/entityAPI.py
--rw-rw-rw-   0        0        0     6258 2023-05-16 11:37:54.000000 pyPreservica-1.7.8/pyPreservica/monitorAPI.py
--rw-rw-rw-   0        0        0     4875 2022-04-21 08:22:10.000000 pyPreservica-1.7.8/pyPreservica/opex.py
--rw-rw-rw-   0        0        0    10522 2021-11-17 14:16:50.000000 pyPreservica-1.7.8/pyPreservica/parAPI.py
--rw-rw-rw-   0        0        0    23541 2023-04-17 14:03:38.000000 pyPreservica-1.7.8/pyPreservica/retentionAPI.py
--rw-rw-rw-   0        0        0    92445 2023-05-16 11:37:54.000000 pyPreservica-1.7.8/pyPreservica/uploadAPI.py
--rw-rw-rw-   0        0        0       99 2023-05-15 14:18:19.000000 pyPreservica-1.7.8/pyPreservica/vocabularyAPI.py
--rw-rw-rw-   0        0        0     6383 2023-05-16 13:25:15.000000 pyPreservica-1.7.8/pyPreservica/webHooksAPI.py
--rw-rw-rw-   0        0        0    17812 2023-03-01 16:08:31.000000 pyPreservica-1.7.8/pyPreservica/workflowAPI.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:55:41.151978 pyPreservica-1.7.8/pyPreservica.egg-info/
--rw-rw-rw-   0        0        0     2581 2023-05-16 13:55:39.000000 pyPreservica-1.7.8/pyPreservica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2023-05-16 13:55:39.000000 pyPreservica-1.7.8/pyPreservica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 13:55:39.000000 pyPreservica-1.7.8/pyPreservica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-05-16 13:55:39.000000 pyPreservica-1.7.8/pyPreservica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-16 13:55:39.000000 pyPreservica-1.7.8/pyPreservica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 13:55:41.168356 pyPreservica-1.7.8/setup.cfg
--rw-rw-rw-   0        0        0     1645 2023-05-16 12:42:45.000000 pyPreservica-1.7.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:28:40.245142 pyPreservica-1.7.9/
+-rw-rw-rw-   0        0        0    11558 2020-08-17 10:38:19.000000 pyPreservica-1.7.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     2581 2023-05-24 09:28:40.245142 pyPreservica-1.7.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1602 2022-03-16 17:04:00.000000 pyPreservica-1.7.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 09:28:40.198273 pyPreservica-1.7.9/pyPreservica/
+-rw-rw-rw-   0        0        0     1096 2023-05-24 08:23:27.000000 pyPreservica-1.7.9/pyPreservica/__init__.py
+-rw-rw-rw-   0        0        0    37685 2023-05-03 10:58:47.000000 pyPreservica-1.7.9/pyPreservica/adminAPI.py
+-rw-rw-rw-   0        0        0    32269 2023-05-03 10:51:09.000000 pyPreservica-1.7.9/pyPreservica/common.py
+-rw-rw-rw-   0        0        0    16189 2023-03-01 16:04:47.000000 pyPreservica-1.7.9/pyPreservica/contentAPI.py
+-rw-rw-rw-   0        0        0   105699 2023-05-24 08:44:58.000000 pyPreservica-1.7.9/pyPreservica/entityAPI.py
+-rw-rw-rw-   0        0        0     6258 2023-05-16 11:37:54.000000 pyPreservica-1.7.9/pyPreservica/monitorAPI.py
+-rw-rw-rw-   0        0        0     4875 2022-04-21 08:22:10.000000 pyPreservica-1.7.9/pyPreservica/opex.py
+-rw-rw-rw-   0        0        0    10522 2021-11-17 14:16:50.000000 pyPreservica-1.7.9/pyPreservica/parAPI.py
+-rw-rw-rw-   0        0        0    23544 2023-05-16 16:46:33.000000 pyPreservica-1.7.9/pyPreservica/retentionAPI.py
+-rw-rw-rw-   0        0        0    92445 2023-05-16 11:37:54.000000 pyPreservica-1.7.9/pyPreservica/uploadAPI.py
+-rw-rw-rw-   0        0        0     5496 2023-05-17 12:28:12.000000 pyPreservica-1.7.9/pyPreservica/vocabularyAPI.py
+-rw-rw-rw-   0        0        0     6736 2023-05-24 08:15:02.000000 pyPreservica-1.7.9/pyPreservica/webHooksAPI.py
+-rw-rw-rw-   0        0        0    17812 2023-03-01 16:08:31.000000 pyPreservica-1.7.9/pyPreservica/workflowAPI.py
+drwxrwxrwx   0        0        0        0 2023-05-24 09:28:40.229520 pyPreservica-1.7.9/pyPreservica.egg-info/
+-rw-rw-rw-   0        0        0     2581 2023-05-24 09:28:38.000000 pyPreservica-1.7.9/pyPreservica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-05-24 09:28:38.000000 pyPreservica-1.7.9/pyPreservica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 09:28:38.000000 pyPreservica-1.7.9/pyPreservica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-05-24 09:28:38.000000 pyPreservica-1.7.9/pyPreservica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-24 09:28:38.000000 pyPreservica-1.7.9/pyPreservica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 09:28:40.245142 pyPreservica-1.7.9/setup.cfg
+-rw-rw-rw-   0        0        0     1645 2023-05-24 08:23:27.000000 pyPreservica-1.7.9/setup.py
```

### Comparing `pyPreservica-1.7.8/LICENSE.txt` & `pyPreservica-1.7.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.8/PKG-INFO` & `pyPreservica-1.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPreservica
-Version: 1.7.8
+Version: 1.7.9
 Summary: Python library for the Preservica API
 Home-page: https://pypreservica.readthedocs.io/
 Author: James Carr
 Author-email: drjamescarr@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pypreservica.readthedocs.io
 Project-URL: Source, https://github.com/carj/pyPreservica
```

### Comparing `pyPreservica-1.7.8/README.md` & `pyPreservica-1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.8/pyPreservica/__init__.py` & `pyPreservica-1.7.9/pyPreservica/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,16 @@
                     cvs_to_cmis_xslt, csv_to_search_xml, generic_asset_package, upload_config, multi_asset_package
 from .workflowAPI import WorkflowAPI, WorkflowContext, WorkflowInstance
 from .retentionAPI import RetentionAPI, RetentionAssignment, RetentionPolicy
 from .parAPI import PreservationActionRegistry
 from .adminAPI import AdminAPI
 from .monitorAPI import MonitorAPI, MonitorCategory, MonitorStatus, MessageStatus
 from .webHooksAPI import WebHooksAPI, TriggerType, WebHookHandler
+from .vocabularyAPI import ControlledVocabularyAPI, Table
 
 
 __author__ = "James Carr (drjamescarr@gmail.com)"
 
 # Version of the Preservica API package
-__version__ = "1.7.8"
+__version__ = "1.7.9"
 
 __license__ = "Apache License Version 2.0"
```

### Comparing `pyPreservica-1.7.8/pyPreservica/adminAPI.py` & `pyPreservica-1.7.9/pyPreservica/adminAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.8/pyPreservica/common.py` & `pyPreservica-1.7.9/pyPreservica/common.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.8/pyPreservica/contentAPI.py` & `pyPreservica-1.7.9/pyPreservica/contentAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.8/pyPreservica/entityAPI.py` & `pyPreservica-1.7.9/pyPreservica/entityAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 licence:    Apache License 2.0
 
 """
 import uuid
 import xml.etree.ElementTree
 from datetime import datetime, timedelta, timezone
 from time import sleep
-from typing import Any, Generator, Tuple, Iterable
+from typing import Any, Generator, Tuple, Iterable, Union
 
 from pyPreservica.common import *
 
 logger = logging.getLogger(__name__)
 
 
 class EntityAPI(AuthenticatedAPI):
@@ -27,15 +27,15 @@
 
             The EntityAPI allows users to interact with the Preservica repository
 
 
     """
 
     def __init__(self, username: str = None, password: str = None, tenant: str = None, server: str = None,
-                 use_shared_secret: bool = False,  protocol: str = "https"):
+                 use_shared_secret: bool = False, protocol: str = "https") -> object:
         super().__init__(username, password, tenant, server, use_shared_secret, protocol)
         xml.etree.ElementTree.register_namespace("oai_dc", "http://www.openarchives.org/OAI/2.0/oai_dc/")
         xml.etree.ElementTree.register_namespace("ead", "urn:isbn:1-931666-22-9")
 
     def user_security_tags(self, with_permissions: bool = False) -> dict:
         """
              Return  security tags available for the  current user
@@ -1694,25 +1694,25 @@
          """
         self.token = self.__token__()
         for entity in self.descendants(folder=folder):
             yield entity
             if entity.entity_type == EntityType.FOLDER:
                 yield from self.all_descendants(folder=entity)
 
-    def descendants(self, folder: Folder = None) -> Generator:
+    def descendants(self, folder: Union[str, Folder] = None) -> Generator:
         maximum = 100
         paged_set = self.children(folder, maximum=maximum, next_page=None)
         for entity in paged_set.results:
             yield entity
         while paged_set.has_more:
             paged_set = self.children(folder, maximum=maximum, next_page=paged_set.next_page)
             for entity in paged_set.results:
                 yield entity
 
-    def children(self, folder: Folder = None, maximum: int = 100, next_page: str = None) -> PagedSet:
+    def children(self, folder: Union[str, Folder] = None, maximum: int = 100, next_page: str = None) -> PagedSet:
         headers = {HEADER_TOKEN: self.token}
         data = {'start': str(0), 'max': str(maximum)}
         folder_reference = folder
         if next_page is None:
             if folder_reference is None:
                 request = self.session.get(f'{self.protocol}://{self.server}/api/entity/root/children', params=data,
                                            headers=headers)
```

### Comparing `pyPreservica-1.7.8/pyPreservica/monitorAPI.py` & `pyPreservica-1.7.9/pyPreservica/monitorAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.8/pyPreservica/opex.py` & `pyPreservica-1.7.9/pyPreservica/opex.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.8/pyPreservica/parAPI.py` & `pyPreservica-1.7.9/pyPreservica/parAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.8/pyPreservica/retentionAPI.py` & `pyPreservica-1.7.9/pyPreservica/retentionAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-pyPreservica EntityAPI module definition
+pyPreservica RetentionAPI module definition
 
 A client library for the Preservica Repository web services Entity API
 https://us.preservica.com/api/entity/documentation.html
 
 author:     James Carr
 licence:    Apache License 2.0
```

### Comparing `pyPreservica-1.7.8/pyPreservica/uploadAPI.py` & `pyPreservica-1.7.9/pyPreservica/uploadAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.8/pyPreservica/webHooksAPI.py` & `pyPreservica-1.7.9/pyPreservica/webHooksAPI.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
-pyPreservica EntityAPI module definition
+pyPreservica WebHooksAPI module definition
 
 A client library for the Preservica Repository web services Webhook API
 https://us.preservica.com/api/webhook/documentation.html
 
 author:     James Carr
 licence:    Apache License 2.0
 
 """
+import json
 from http.server import BaseHTTPRequestHandler
 from urllib.parse import urlparse, parse_qs
 import hmac
 from pyPreservica.common import *
 
 logger = logging.getLogger(__name__)
 
@@ -23,29 +24,30 @@
     A sample web hook web server which provides handshake verification
     The shared secret key is passed in via the HTTPServer
 
     Extend the class and implement do_WORK() method
     The JSON document is passed into do_WORK()
 
     """
+
     def hmac(self, key, message):
         return hmac.new(key=bytes(key, 'latin-1'), msg=bytes(message, 'latin-1'), digestmod=hashlib.sha256).hexdigest()
 
     def do_POST(self):
         result = urlparse(self.path)
         q = parse_qs(result.query)
         if 'challengeCode' in q:
             code = q['challengeCode'][0]
             signature = self.hmac(self.server.secret_key, code)
             response = f'{{ "challengeCode": "{code}",     "challengeResponse": "{signature}" }}'
             self.send_response(200)
             self.send_header("Content-type", "application/json")
             self.end_headers()
             self.wfile.write(bytes(response.encode('utf-8')))
-            self.log_message("Handshake Completed.")
+            self.log_message(f"Handshake Completed. {response.encode('utf-8')}")
         else:
             verif_sig = self.headers.get("Preservica-Signature", None)
             if "chunked" in self.headers.get("Transfer-Encoding", "") and (verif_sig is not None):
                 payload = ""
                 while True:
                     line = self.rfile.readline().strip()
                     chunk_length = int(line, 16)
@@ -77,15 +79,15 @@
     """
     Class to register new webhook endpoints
 
     """
 
     def subscriptions(self):
         """
-        Return all the current active web hook subscriptions
+        Return all the current active web hook subscriptions as a json document
 
         :return: list of web hooks
         """
         self._check_if_user_has_manager_role()
         headers = {HEADER_TOKEN: self.token}
         response = self.session.get(f'{self.protocol}://{self.server}{BASE_ENDPOINT}/subscriptions', headers=headers)
         if response.status_code == requests.codes.unauthorized:
@@ -97,35 +99,45 @@
             return doc
         else:
             exception = HTTPException("", response.status_code, response.url, "subscriptions",
                                       response.content.decode('utf-8'))
             logger.error(exception)
             raise exception
 
-    def un_subscribe(self, subscription_id: str):
+    def unsubscribe_all(self):
+        """
+        Unsubscribe from all webhooks.
+        :return:
+        """
+        self._check_if_user_has_manager_role()
+        subscriptions = self.subscriptions()
+        for sub in subscriptions:
+            self.unsubscribe(sub['id'])
+
+    def unsubscribe(self, subscription_id: str):
         """
-        Unsubscribe from provided webhook.
+        Unsubscribe from the provided webhook.
 
         :param subscription_id:
         :return:
         """
         self._check_if_user_has_manager_role()
         headers = {HEADER_TOKEN: self.token}
         response = self.session.delete(
             f'{self.protocol}://{self.server}{BASE_ENDPOINT}/subscriptions/{subscription_id}',
             headers=headers)
         if response.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
-            return self.un_subscribe(subscription_id)
+            return self.unsubscribe(subscription_id)
         if response.status_code == requests.codes.no_content:
             json_response = str(response.content.decode('utf-8'))
             logger.debug(json_response)
             return json_response
         else:
-            exception = HTTPException(str(subscription_id), response.status_code, response.url, "un_subscribe",
+            exception = HTTPException(str(subscription_id), response.status_code, response.url, "unsubscribe",
                                       response.content.decode('utf-8'))
             logger.error(exception)
             raise exception
 
     def subscribe(self, url: str, triggerType: TriggerType, secret: str):
         """
         Subscribe to a new web hook
```

### Comparing `pyPreservica-1.7.8/pyPreservica/workflowAPI.py` & `pyPreservica-1.7.9/pyPreservica/workflowAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.8/pyPreservica.egg-info/PKG-INFO` & `pyPreservica-1.7.9/pyPreservica.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPreservica
-Version: 1.7.8
+Version: 1.7.9
 Summary: Python library for the Preservica API
 Home-page: https://pypreservica.readthedocs.io/
 Author: James Carr
 Author-email: drjamescarr@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pypreservica.readthedocs.io
 Project-URL: Source, https://github.com/carj/pyPreservica
```

### Comparing `pyPreservica-1.7.8/pyPreservica.egg-info/SOURCES.txt` & `pyPreservica-1.7.9/pyPreservica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.8/setup.py` & `pyPreservica-1.7.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     os.system('twine upload dist/*')
     sys.exit()
 
 
 # This call to setup() does all the work
 setup(
     name=PKG,
-    version="1.7.8",
+    version="1.7.9",
     description="Python library for the Preservica API",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://pypreservica.readthedocs.io/",
     author="James Carr",
     author_email="drjamescarr@gmail.com",
     license="Apache License 2.0",
```

