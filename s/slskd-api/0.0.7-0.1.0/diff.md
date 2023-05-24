# Comparing `tmp/slskd-api-0.0.7.tar.gz` & `tmp/slskd-api-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slskd-api-0.0.7.tar", last modified: Sat May 20 08:17:15 2023, max compression
+gzip compressed data, was "slskd-api-0.1.0.tar", last modified: Wed May 24 18:52:25 2023, max compression
```

## Comparing `slskd-api-0.0.7.tar` & `slskd-api-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:17:15.831958 slskd-api-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    34260 2023-05-20 08:16:58.000000 slskd-api-0.0.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-20 08:17:15.831958 slskd-api-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-20 08:16:58.000000 slskd-api-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 08:17:15.831958 slskd-api-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-20 08:16:58.000000 slskd-api-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:17:15.827957 slskd-api-0.0.7/slskd_api/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:17:15.831958 slskd-api-0.0.7/slskd_api/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/application.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/conversations.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/public_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/relay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/rooms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/searches.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/shares.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/apis/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-20 08:16:58.000000 slskd-api-0.0.7/slskd_api/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:17:15.827957 slskd-api-0.0.7/slskd_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-20 08:17:15.000000 slskd-api-0.0.7/slskd_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-20 08:17:15.000000 slskd-api-0.0.7/slskd_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 08:17:15.000000 slskd-api-0.0.7/slskd_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-20 08:17:15.000000 slskd-api-0.0.7/slskd_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-20 08:17:15.000000 slskd-api-0.0.7/slskd_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:25.872889 slskd-api-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34260 2023-05-24 18:52:13.000000 slskd-api-0.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-24 18:52:25.868889 slskd-api-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-24 18:52:13.000000 slskd-api-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 18:52:25.872889 slskd-api-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-24 18:52:13.000000 slskd-api-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:25.864889 slskd-api-0.1.0/slskd_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-24 18:52:13.000000 slskd-api-0.1.0/slskd_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:25.868889 slskd-api-0.1.0/slskd_api/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-24 18:52:13.000000 slskd-api-0.1.0/slskd_api/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-24 18:52:13.000000 slskd-api-0.1.0/slskd_api/apis/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-24 18:52:13.000000 slskd-api-0.1.0/slskd_api/apis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-24 18:52:13.000000 slskd-api-0.1.0/slskd_api/apis/conversations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-24 18:52:13.000000 slskd-api-0.1.0/slskd_api/apis/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-24 18:52:13.000000 slskd-api-0.1.0/slskd_api/apis/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-24 18:52:13.000000 slskd-api-0.1.0/slskd_api/apis/public_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-24 18:52:13.000000 slskd-api-0.1.0/slskd_api/apis/relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-24 18:52:13.000000 slskd-api-0.1.0/slskd_api/apis/rooms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-05-24 18:52:13.000000 slskd-api-0.1.0/slskd_api/apis/searches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-24 18:52:13.000000 slskd-api-0.1.0/slskd_api/apis/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-24 18:52:13.000000 slskd-api-0.1.0/slskd_api/apis/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-24 18:52:13.000000 slskd-api-0.1.0/slskd_api/apis/shares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-24 18:52:13.000000 slskd-api-0.1.0/slskd_api/apis/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-24 18:52:13.000000 slskd-api-0.1.0/slskd_api/apis/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-24 18:52:13.000000 slskd-api-0.1.0/slskd_api/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:25.864889 slskd-api-0.1.0/slskd_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-24 18:52:25.000000 slskd-api-0.1.0/slskd_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-24 18:52:25.000000 slskd-api-0.1.0/slskd_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 18:52:25.000000 slskd-api-0.1.0/slskd_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-24 18:52:25.000000 slskd-api-0.1.0/slskd_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 18:52:25.000000 slskd-api-0.1.0/slskd_api.egg-info/top_level.txt
```

### Comparing `slskd-api-0.0.7/LICENSE.md` & `slskd-api-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.7/PKG-INFO` & `slskd-api-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slskd-api
-Version: 0.0.7
+Version: 0.1.0
 Summary: API Wrapper to interact with slskd
 Author: bigoulours
 License: GNU Affero General Public License v3.0
 Project-URL: Documentation, https://slskd-api.readthedocs.io
 Project-URL: Source, https://github.com/bigoulours/slskd-python-api
 Project-URL: Funding, https://liberapay.com/bigoulours/donate
 Requires-Python: >=3.7
```

### Comparing `slskd-api-0.0.7/README.md` & `slskd-api-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.7/setup.py` & `slskd-api-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `slskd-api-0.0.7/slskd_api/apis/application.py` & `slskd-api-0.1.0/slskd_api/apis/application.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+# Copyright (C) 2023 bigoulours
+# 
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as
+# published by the Free Software Foundation, either version 3 of the
+# License, or (at your option) any later version.
+# 
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+# 
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 from .base import *
 
 class ApplicationApi(BaseApi):
     """
     This class contains the methods to interact with the Application API.
     """
 
@@ -64,14 +79,13 @@
         :return: True if successful.
         """
         url = self.api_url + '/application/gc'
         response = requests.post(url, headers=self.header)
         return response.ok
     
     
-# Getting error 'Could not find file...':
+# Not supposed to be part of the external API
+# More info in the Github discussion: https://github.com/slskd/slskd/discussions/910
     # def dump(self):
-    #     """
-    #     """
     #     url = self.api_url + '/application/dump'
     #     response = requests.get(url, headers=self.header)
     #     return response.json()
```

### Comparing `slskd-api-0.0.7/slskd_api/apis/options.py` & `slskd-api-0.1.0/slskd_api/apis/shares.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,78 +1,78 @@
+# Copyright (C) 2023 bigoulours
+# 
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as
+# published by the Free Software Foundation, either version 3 of the
+# License, or (at your option) any later version.
+# 
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+# 
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 from .base import *
 
-class OptionsApi(BaseApi):
+class SharesApi(BaseApi):
     """
-    This class contains the methods to interact with the Options API.
+    This class contains the methods to interact with the Shares API.
     """
 
-    def get(self) -> dict:
+    def get_all(self) -> dict:
         """
-        Gets the current application options.
+        Gets the current list of shares.
         """
-        url = self.api_url + '/options'
+        url = self.api_url + '/shares'
         response = requests.get(url, headers=self.header)
         return response.json()
     
 
-    def get_startup(self) -> dict:
-        """
-        Gets the application options provided at startup.
+    def start_scan(self) -> bool:
         """
-        url = self.api_url + '/options/startup'
-        response = requests.get(url, headers=self.header)
-        return response.json()
+        Initiates a scan of the configured shares.
 
-  
-    def debug(self) -> str:
-        """
-        Gets the debug view of the current application options.
-        debug and remote_configuration must be set to true.
-        Only works with token (usr/pwd login). 'Unauthorized' with API-Key.
+        :return: True if successful.
         """
-        url = self.api_url + '/options/debug'
-        response = requests.get(url, headers=self.header)
-        return response.json()
-
+        url = self.api_url + '/shares'
+        response = requests.put(url, headers=self.header)
+        return response.ok
+    
 
-    def yaml_location(self) -> str:
+    def cancel_scan(self) -> bool:
         """
-        Gets the path of the yaml config file. remote_configuration must be set to true.
-        Only works with token (usr/pwd login). 'Unauthorized' with API-Key.
+        Cancels a share scan, if one is running.
+
+        :return: True if successful.
         """
-        url = self.api_url + '/options/yaml/location'
-        response = requests.get(url, headers=self.header)
-        return response.json()
+        url = self.api_url + '/shares'
+        response = requests.delete(url, headers=self.header)
+        return response.ok
     
 
-    def download_yaml(self) -> str:
+    def get(self, id: str) -> dict:
         """
-        Gets the content of the yaml config file as text. remote_configuration must be set to true.
-        Only works with token (usr/pwd login). 'Unauthorized' with API-Key.
+        Gets the share associated with the specified id.
         """
-        url = self.api_url + '/options/yaml'
+        url = self.api_url + f'/shares/{id}'
         response = requests.get(url, headers=self.header)
         return response.json()
     
 
-    def upload_yaml(self, yaml_content: str) -> bool:
+    def all_contents(self) -> list:
         """
-        Sets the content of the yaml config file. remote_configuration must be set to true.
-        Only works with token (usr/pwd login). 'Unauthorized' with API-Key.
-
-        :return: True if successful.
+        Returns a list of all shared directories and files.
         """
-        url = self.api_url + '/options/yaml'
-        response = requests.post(url, headers=self.header, json=yaml_content)
-        return response.ok
+        url = self.api_url + '/shares/contents'
+        response = requests.get(url, headers=self.header)
+        return response.json()
     
 
-    def validate_yaml(self, yaml_content: str) -> str:
+    def contents(self, id: str) -> list:
         """
-        Validates the provided yaml string. remote_configuration must be set to true.
-        Only works with token (usr/pwd login). 'Unauthorized' with API-Key.
-
-        :return: Empty string if validation successful. Error message otherwise.
+        Gets the contents of the share associated with the specified id.
         """
-        url = self.api_url + '/options/yaml/validate'
-        response = requests.post(url, headers=self.header, json=yaml_content)
-        return response.text
+        url = self.api_url + f'/shares/{id}/contents'
+        response = requests.get(url, headers=self.header)
+        return response.json()
```

### Comparing `slskd-api-0.0.7/slskd_api/apis/relay.py` & `slskd-api-0.1.0/slskd_api/apis/relay.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+# Copyright (C) 2023 bigoulours
+# 
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as
+# published by the Free Software Foundation, either version 3 of the
+# License, or (at your option) any later version.
+# 
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+# 
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 from .base import *
 
 class RelayApi(BaseApi):
     """
     [UNTESTED] This class contains the methods to interact with the Relay API.
     """
```

### Comparing `slskd-api-0.0.7/slskd_api/apis/server.py` & `slskd-api-0.1.0/slskd_api/apis/public_chat.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,42 @@
+# Copyright (C) 2023 bigoulours
+# 
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as
+# published by the Free Software Foundation, either version 3 of the
+# License, or (at your option) any later version.
+# 
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+# 
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 from .base import *
 
-class ServerApi(BaseApi):
+class PublicChatApi(BaseApi):
     """
-    This class contains the methods to interact with the Search API.
+    [UNTESTED] This class contains the methods to interact with the PublicChat API.
     """
 
-    def connect(self) -> bool:
+    def start(self) -> bool:
         """
-        Connects the client.
+        Starts public chat.
 
         :return: True if successful.
         """
-        url = self.api_url + '/server'
-        response = requests.put(url, headers=self.header)
+        url = self.api_url + '/publicchat'
+        response = requests.post(url, headers=self.header)
         return response.ok
     
 
-    def disconnect(self) -> bool:
+    def stop(self) -> bool:
         """
-        Disconnects the client.
+        Stops public chat.
 
         :return: True if successful.
         """
-        url = self.api_url + '/server'
-        response = requests.delete(url, headers=self.header, json='')
+        url = self.api_url + '/publicchat'
+        response = requests.delete(url, headers=self.header)
         return response.ok
-    
-
-    def state(self) -> dict:
-        """
-        Retrieves the current state of the server.
-        """
-        url = self.api_url + '/server'
-        response = requests.get(url, headers=self.header)
-        return response.json()
```

### Comparing `slskd-api-0.0.7/slskd_api/apis/transfers.py` & `slskd-api-0.1.0/slskd_api/apis/transfers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+# Copyright (C) 2023 bigoulours
+# 
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as
+# published by the Free Software Foundation, either version 3 of the
+# License, or (at your option) any later version.
+# 
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+# 
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 from .base import *
 from typing import Union
 
 class TransfersApi(BaseApi):
     """
     This class contains the methods to interact with the Transfers API.
     """
```

### Comparing `slskd-api-0.0.7/slskd_api/client.py` & `slskd-api-0.1.0/slskd_api/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+# Copyright (C) 2023 bigoulours
+# 
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as
+# published by the Free Software Foundation, either version 3 of the
+# License, or (at your option) any later version.
+# 
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+# 
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 API_VERSION = 'v0'
 
 import requests
 from urllib.parse import urljoin
 from functools import reduce
 from base64 import b64encode
 from slskd_api.apis import *
@@ -18,26 +33,29 @@
 
     def __init__(self,
                  host: str,
                  api_key: str = None,
                  url_base: str = '/',
                  username: str = None,
                  password: str = None,
+                 token: str = None,
     ):
         api_url = reduce(urljoin, [host, f'{url_base}/', f'api/{API_VERSION}'])
      
         header = {'accept': '*/*'}
 
         if api_key:
             header['X-API-Key'] = api_key
         elif username and password:
             header['Authorization'] = 'Bearer ' + \
                             SessionApi(api_url, header).login(username, password)['token']
+        elif token:
+            header['Authorization'] = 'Bearer ' + token
         else:
-            raise ValueError('Please provide an API-Key or a valid username/password pair.')
+            raise ValueError('Please provide an API-Key, a valid token or username/password.')
         
         base_args = (api_url, header)
         
         self.application = ApplicationApi(*base_args)
         self.conversations = ConversationsApi(*base_args)
         self.logs = LogsApi(*base_args)
         self.options = OptionsApi(*base_args)
```

### Comparing `slskd-api-0.0.7/slskd_api.egg-info/PKG-INFO` & `slskd-api-0.1.0/slskd_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slskd-api
-Version: 0.0.7
+Version: 0.1.0
 Summary: API Wrapper to interact with slskd
 Author: bigoulours
 License: GNU Affero General Public License v3.0
 Project-URL: Documentation, https://slskd-api.readthedocs.io
 Project-URL: Source, https://github.com/bigoulours/slskd-python-api
 Project-URL: Funding, https://liberapay.com/bigoulours/donate
 Requires-Python: >=3.7
```

### Comparing `slskd-api-0.0.7/slskd_api.egg-info/SOURCES.txt` & `slskd-api-0.1.0/slskd_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

