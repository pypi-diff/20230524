# Comparing `tmp/ubicquia-0.1.4.tar.gz` & `tmp/ubicquia-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubicquia-0.1.4.tar", last modified: Tue Dec 13 00:04:11 2022, max compression
+gzip compressed data, was "ubicquia-0.2.0.tar", last modified: Wed May 17 03:00:15 2023, max compression
```

## Comparing `ubicquia-0.1.4.tar` & `ubicquia-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 rod       (1000) rod       (1000)        0 2022-12-13 00:04:11.524758 ubicquia-0.1.4/
--rw-rw-r--   0 rod       (1000) rod       (1000)    35128 2022-09-01 20:30:21.000000 ubicquia-0.1.4/LICENSE.txt
--rw-rw-r--   0 rod       (1000) rod       (1000)      519 2022-12-13 00:04:11.524758 ubicquia-0.1.4/PKG-INFO
--rw-rw-r--   0 rod       (1000) rod       (1000)     1551 2022-09-09 04:04:15.000000 ubicquia-0.1.4/README.md
--rw-rw-r--   0 rod       (1000) rod       (1000)       38 2022-12-13 00:04:11.524758 ubicquia-0.1.4/setup.cfg
--rw-rw-r--   0 rod       (1000) rod       (1000)      627 2022-12-12 23:54:40.000000 ubicquia-0.1.4/setup.py
-drwxrwxr-x   0 rod       (1000) rod       (1000)        0 2022-12-13 00:04:11.524758 ubicquia-0.1.4/ubicquia/
--rw-rw-r--   0 rod       (1000) rod       (1000)      382 2022-12-13 00:02:44.000000 ubicquia-0.1.4/ubicquia/__init__.py
--rw-rw-r--   0 rod       (1000) rod       (1000)     8678 2022-12-01 18:05:28.000000 ubicquia-0.1.4/ubicquia/base.py
--rw-rw-r--   0 rod       (1000) rod       (1000)     1080 2022-09-09 03:58:10.000000 ubicquia-0.1.4/ubicquia/base_models.py
--rw-rw-r--   0 rod       (1000) rod       (1000)      764 2022-12-12 23:32:29.000000 ubicquia-0.1.4/ubicquia/client.py
--rw-rw-r--   0 rod       (1000) rod       (1000)     3313 2022-12-01 18:04:56.000000 ubicquia-0.1.4/ubicquia/light_control.py
--rw-rw-r--   0 rod       (1000) rod       (1000)     2043 2022-09-09 00:07:54.000000 ubicquia-0.1.4/ubicquia/light_control_models.py
--rw-rw-r--   0 rod       (1000) rod       (1000)     3350 2022-11-07 18:04:47.000000 ubicquia-0.1.4/ubicquia/nodes.py
--rw-rw-r--   0 rod       (1000) rod       (1000)     4455 2022-11-07 17:56:19.000000 ubicquia-0.1.4/ubicquia/nodes_models.py
--rw-rw-r--   0 rod       (1000) rod       (1000)     1925 2022-07-06 20:02:26.000000 ubicquia-0.1.4/ubicquia/public_safety.py
--rw-rw-r--   0 rod       (1000) rod       (1000)     1706 2022-12-12 23:53:00.000000 ubicquia-0.1.4/ubicquia/reports.py
--rw-rw-r--   0 rod       (1000) rod       (1000)     1576 2022-08-03 17:39:50.000000 ubicquia-0.1.4/ubicquia/setup_logger.py
--rw-rw-r--   0 rod       (1000) rod       (1000)      790 2022-07-15 23:00:34.000000 ubicquia-0.1.4/ubicquia/shortcuts.py
--rw-rw-r--   0 rod       (1000) rod       (1000)     2480 2022-11-09 02:30:16.000000 ubicquia-0.1.4/ubicquia/traffic_mobility.py
--rw-rw-r--   0 rod       (1000) rod       (1000)      753 2022-11-09 02:47:22.000000 ubicquia-0.1.4/ubicquia/traffic_mobility_models.py
--rw-rw-r--   0 rod       (1000) rod       (1000)     1574 2022-07-08 22:12:43.000000 ubicquia-0.1.4/ubicquia/utils.py
--rw-rw-r--   0 rod       (1000) rod       (1000)     8446 2022-07-15 23:00:34.000000 ubicquia-0.1.4/ubicquia/wifi.py
--rw-rw-r--   0 rod       (1000) rod       (1000)     5585 2022-07-15 23:00:34.000000 ubicquia-0.1.4/ubicquia/wifi_captive_portal.py
-drwxrwxr-x   0 rod       (1000) rod       (1000)        0 2022-12-13 00:04:11.524758 ubicquia-0.1.4/ubicquia.egg-info/
--rw-rw-r--   0 rod       (1000) rod       (1000)      519 2022-12-13 00:04:11.000000 ubicquia-0.1.4/ubicquia.egg-info/PKG-INFO
--rw-rw-r--   0 rod       (1000) rod       (1000)      597 2022-12-13 00:04:11.000000 ubicquia-0.1.4/ubicquia.egg-info/SOURCES.txt
--rw-rw-r--   0 rod       (1000) rod       (1000)        1 2022-12-13 00:04:11.000000 ubicquia-0.1.4/ubicquia.egg-info/dependency_links.txt
--rw-rw-r--   0 rod       (1000) rod       (1000)       63 2022-12-13 00:04:11.000000 ubicquia-0.1.4/ubicquia.egg-info/requires.txt
--rw-rw-r--   0 rod       (1000) rod       (1000)        9 2022-12-13 00:04:11.000000 ubicquia-0.1.4/ubicquia.egg-info/top_level.txt
+drwxrwxr-x   0 rod       (1000) rod       (1000)        0 2023-05-17 03:00:15.210446 ubicquia-0.2.0/
+-rw-rw-r--   0 rod       (1000) rod       (1000)    35128 2022-09-01 20:30:21.000000 ubicquia-0.2.0/LICENSE.txt
+-rw-rw-r--   0 rod       (1000) rod       (1000)      562 2023-05-17 03:00:15.210446 ubicquia-0.2.0/PKG-INFO
+-rw-rw-r--   0 rod       (1000) rod       (1000)     1673 2023-05-17 02:51:45.000000 ubicquia-0.2.0/README.md
+-rw-rw-r--   0 rod       (1000) rod       (1000)       38 2023-05-17 03:00:15.210446 ubicquia-0.2.0/setup.cfg
+-rw-rw-r--   0 rod       (1000) rod       (1000)      600 2023-05-17 02:51:45.000000 ubicquia-0.2.0/setup.py
+drwxrwxr-x   0 rod       (1000) rod       (1000)        0 2023-05-17 03:00:15.206446 ubicquia-0.2.0/ubicquia/
+-rw-rw-r--   0 rod       (1000) rod       (1000)      382 2023-05-17 02:51:45.000000 ubicquia-0.2.0/ubicquia/__init__.py
+-rw-rw-r--   0 rod       (1000) rod       (1000)     9085 2023-05-17 02:51:45.000000 ubicquia-0.2.0/ubicquia/base.py
+-rw-rw-r--   0 rod       (1000) rod       (1000)     1080 2022-09-09 03:58:10.000000 ubicquia-0.2.0/ubicquia/base_models.py
+-rw-rw-r--   0 rod       (1000) rod       (1000)     1493 2023-01-07 00:59:58.000000 ubicquia-0.2.0/ubicquia/client.py
+-rw-rw-r--   0 rod       (1000) rod       (1000)     3313 2022-12-01 18:04:56.000000 ubicquia-0.2.0/ubicquia/light_control.py
+-rw-rw-r--   0 rod       (1000) rod       (1000)     2043 2022-09-09 00:07:54.000000 ubicquia-0.2.0/ubicquia/light_control_models.py
+-rw-rw-r--   0 rod       (1000) rod       (1000)     4222 2023-01-13 19:04:34.000000 ubicquia-0.2.0/ubicquia/nodes.py
+-rw-rw-r--   0 rod       (1000) rod       (1000)     4943 2023-01-13 19:05:47.000000 ubicquia-0.2.0/ubicquia/nodes_models.py
+-rw-rw-r--   0 rod       (1000) rod       (1000)     1925 2022-07-06 20:02:26.000000 ubicquia-0.2.0/ubicquia/public_safety.py
+-rw-rw-r--   0 rod       (1000) rod       (1000)     1874 2023-05-17 02:51:45.000000 ubicquia-0.2.0/ubicquia/reports.py
+-rw-rw-r--   0 rod       (1000) rod       (1000)     1576 2022-08-03 17:39:50.000000 ubicquia-0.2.0/ubicquia/setup_logger.py
+-rw-rw-r--   0 rod       (1000) rod       (1000)     1564 2023-05-17 02:51:45.000000 ubicquia-0.2.0/ubicquia/shortcuts.py
+-rw-rw-r--   0 rod       (1000) rod       (1000)     2480 2022-11-09 02:30:16.000000 ubicquia-0.2.0/ubicquia/traffic_mobility.py
+-rw-rw-r--   0 rod       (1000) rod       (1000)      753 2022-11-09 02:47:22.000000 ubicquia-0.2.0/ubicquia/traffic_mobility_models.py
+-rw-rw-r--   0 rod       (1000) rod       (1000)     1574 2022-07-08 22:12:43.000000 ubicquia-0.2.0/ubicquia/utils.py
+-rw-rw-r--   0 rod       (1000) rod       (1000)     8446 2022-07-15 23:00:34.000000 ubicquia-0.2.0/ubicquia/wifi.py
+-rw-rw-r--   0 rod       (1000) rod       (1000)     5585 2022-07-15 23:00:34.000000 ubicquia-0.2.0/ubicquia/wifi_captive_portal.py
+drwxrwxr-x   0 rod       (1000) rod       (1000)        0 2023-05-17 03:00:15.206446 ubicquia-0.2.0/ubicquia.egg-info/
+-rw-rw-r--   0 rod       (1000) rod       (1000)      562 2023-05-17 03:00:15.000000 ubicquia-0.2.0/ubicquia.egg-info/PKG-INFO
+-rw-rw-r--   0 rod       (1000) rod       (1000)      597 2023-05-17 03:00:15.000000 ubicquia-0.2.0/ubicquia.egg-info/SOURCES.txt
+-rw-rw-r--   0 rod       (1000) rod       (1000)        1 2023-05-17 03:00:15.000000 ubicquia-0.2.0/ubicquia.egg-info/dependency_links.txt
+-rw-rw-r--   0 rod       (1000) rod       (1000)       47 2023-05-17 03:00:15.000000 ubicquia-0.2.0/ubicquia.egg-info/requires.txt
+-rw-rw-r--   0 rod       (1000) rod       (1000)        9 2023-05-17 03:00:15.000000 ubicquia-0.2.0/ubicquia.egg-info/top_level.txt
```

### Comparing `ubicquia-0.1.4/LICENSE.txt` & `ubicquia-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ubicquia-0.1.4/PKG-INFO` & `ubicquia-0.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubicquia
-Version: 0.1.4
+Version: 0.2.0
 Summary: Ubicquia API Client Library
 Author: CiberC Dev
 License: GPLv3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Ubicquia API client
@@ -18,14 +18,18 @@
 
 session = UbicquiaSession(..., )
 ubicquia = Ubicquia(session)
 ```
 
 ## Changes
 
-v012
+v020
 
-- Add node method current_node_state
+- Remove python-decouple dependency
 
 v014
 
 - New reports (energy usage and energy usage chart)
+
+v012
+
+- Add node method current_node_state
```

### Comparing `ubicquia-0.1.4/README.md` & `ubicquia-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 
 Python package library for accessing the Ubicquia API. Following 12-factor app principles, the library is external dependency from the applications that requires it. This project will store in Azure but a distribuible lib is public in PyPI.
 
 A public MD `README_PUB.md` created for descritpion in PyPI.
 
 Create `.env` to configure project read the `.example.env` to configure.
 
+## Version
+
+Use editor to replace and set the version:
+
+v0.2.0
+
 ## Build a dist
 
 ```bash
 rm -rf dist/*
 python setup.py sdist bdist_wheel
 twine upload dist/*
 pip install ubicquia
@@ -29,14 +35,18 @@
 2. Crear VLAN
 3. Crear Captive Portal y configurarlo
 4. Definir radio profile (2.4Ghz, 5Ghz)
 5. Crear Venue y asociar los elementos anteriores.
 
 ## Changes
 
+2023-05-16
+
+- Remove dependency for env: python-decouple
+
 2022-09-08
 
 - Change Pydantic base config to extra = allow instead of forbird
 - Add light control module with set light status and dim
 
 ## Ref
```

### Comparing `ubicquia-0.1.4/setup.py` & `ubicquia-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 with open('README_PUB.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="ubicquia",
     packages=find_packages(include=["ubicquia"]),
     # packages=["ubicquia"],
-    version="0.1.4",
+    version="0.2.0",
     description="Ubicquia API Client Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # url="https://<site>.readthedocs.io/",
     license="GPLv3",
     author="CiberC Dev",
     install_requires=[
         'requests>=2.28',
         'requests-oauthlib',
-        'python-decouple',
         'pydantic>=1.9'
     ],
 )
```

### Comparing `ubicquia-0.1.4/ubicquia/base.py` & `ubicquia-0.2.0/ubicquia/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """Base
 
 - AUTH_URL: URL for authentication based on default or env.
 - BASE_URL: URL for API requests.
 """
+import os
 from abc import ABC, abstractmethod
 import json
 import logging
 from pathlib import Path
 from time import time
 from typing import TypedDict
 
-from decouple import config
 from requests_oauthlib import OAuth2Session
 from requests.auth import HTTPBasicAuth
-from requests import Session
+from requests import Session, Response
 from requests.exceptions import HTTPError
 from oauthlib.oauth2 import LegacyApplicationClient
 from oauthlib.oauth2.rfc6749.errors import InvalidGrantError
 
 logger = logging.getLogger(__name__)
 
-AUTH_URL = config(
+AUTH_URL = os.getenv(
     'UBICQUIA_AUTH_URL',
     'https://auth.ubihub.ubicquia.com'
     '/auth/realms/ubivu-prd/protocol/openid-connect/token'
 )
 
-BASE_URL = config('UBICQUIA_BASE_URL', 'https://api.ubicquia.com/api')
+BASE_URL = os.getenv('UBICQUIA_BASE_URL', 'https://api.ubicquia.com/api')
 
 
 class TokenUpdate(ABC):
     """Define implementation interface for Store Token.
 
     Define a way to save and obtains token from external storage systems.
     """
@@ -191,14 +191,29 @@
         # Standard:
         self.client.headers.update({'Accept': 'application/json'})
         # Ubicquia API Docs show:
         # self.client.headers.update({'accept': 'application/json'})
         # print(f'self.client.headers {self.client.headers}')
         # import pdb; pdb.set_trace()
 
+    def raw_req(self, *args, **kwargs) -> Response:
+        """Returns a Respose object from requests.
+
+        Args:
+            *args, **kwargs: parameters passed to requests.request
+
+        Return:
+            Response object from requests module.
+
+        Raises:
+            HTTP Errors from requests.
+        """
+        self.obtain_token_session()
+        return self.client.request(*args, **kwargs)
+
     def req(self, *args, **kwargs) -> dict:
         """Make a HTTP request to server.
 
         Wrapper for requests. Use this method as it were
 
         .. code:: python
```

### Comparing `ubicquia-0.1.4/ubicquia/base_models.py` & `ubicquia-0.2.0/ubicquia/base_models.py`

 * *Files identical despite different names*

### Comparing `ubicquia-0.1.4/ubicquia/light_control.py` & `ubicquia-0.2.0/ubicquia/light_control.py`

 * *Files identical despite different names*

### Comparing `ubicquia-0.1.4/ubicquia/light_control_models.py` & `ubicquia-0.2.0/ubicquia/light_control_models.py`

 * *Files identical despite different names*

### Comparing `ubicquia-0.1.4/ubicquia/nodes.py` & `ubicquia-0.2.0/ubicquia/nodes.py`

 * *Files 22% similar despite different names*

```diff
@@ -96,7 +96,38 @@
         url = self.base_url + '/currentnodestate'
 
         if is_active not in [0, 1]:
             raise ValueError('Invalid value')
         params = {'isActive': is_active}
         d = self.session.req('get', url, params=params)
         return models.NodeListResponse(**d)
+
+    def discover_devices(self) -> models.DiscoverDevices:
+        """Discover all ubicells for a customer.
+
+        This endpoint method is not offically documented. Example of part of the
+        data:
+
+         .. code:: python
+
+            {"data": [
+                {
+                    "LPState": -2,
+                    "dali": "No",
+                    "dali_status": "",
+                    "dev_eui": "...",
+                    "id": 1,
+                    "latitude": "...",
+                    "longitude": "...",
+                    "updatedDateTime": "2022-11-25 13:18:10"
+                }],
+            ...}
+
+        Returns:
+            Devices and their states.
+
+        Raises:
+            HTTP Errors.
+        """
+        url = self.base_url_v2 + '/map/nodes/light'
+        d = self.session.req('post', url)
+        return models.DiscoverDevices(**d)
```

### Comparing `ubicquia-0.1.4/ubicquia/nodes_models.py` & `ubicquia-0.2.0/ubicquia/nodes_models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Optional  # , Union
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 from .base_models import Link, ResponseModel, Base, Meta
 
 
 class GenericStatus(Base):
     color: Optional[str]
     status: Optional[str]
     type: Optional[str]
@@ -158,7 +158,29 @@
     data: List[Node]
     links: Optional[Link]
     meta: Optional[Meta]
 
 
 class NodeResponse(ResponseModel):
     data: Node
+
+
+class DiscoverDeviceData(BaseModel):
+    lp_state: int = Field(..., alias='LPState')
+    dali: str
+    dali_status: str
+    dev_eui: str
+    id: int
+    latitude: Optional[str]
+    longitude: Optional[str]
+    updated_date_time: str = Field(..., alias='updatedDateTime')
+
+
+class DiscoverDeviceMeta(BaseModel):
+    all_count: int
+    filter_count: int
+
+
+class DiscoverDevices(ResponseModel):
+    data: List[DiscoverDeviceData] = []
+    meta: DiscoverDeviceMeta
+    timestamp: str
```

### Comparing `ubicquia-0.1.4/ubicquia/public_safety.py` & `ubicquia-0.2.0/ubicquia/public_safety.py`

 * *Files identical despite different names*

### Comparing `ubicquia-0.1.4/ubicquia/reports.py` & `ubicquia-0.2.0/ubicquia/reports.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,7 +66,12 @@
             date: format yyyy-mm-dd
             report_type: only ReportType values
         """
         url = self.base_url + '/energyusageChart'
         params = {'report_type': report_type, 'date': date}
         d = self.session.req('get', url, params=params)
         return ReportChartResponse(**d)
+
+    def kilowatt_hour(self, start_date: str, end_date: str, **pagination):
+        raise NotImplementedError
+        # url = self.base_url + '/kwhLoad'
+        return
```

### Comparing `ubicquia-0.1.4/ubicquia/setup_logger.py` & `ubicquia-0.2.0/ubicquia/setup_logger.py`

 * *Files identical despite different names*

### Comparing `ubicquia-0.1.4/ubicquia/traffic_mobility.py` & `ubicquia-0.2.0/ubicquia/traffic_mobility.py`

 * *Files identical despite different names*

### Comparing `ubicquia-0.1.4/ubicquia/traffic_mobility_models.py` & `ubicquia-0.2.0/ubicquia/traffic_mobility_models.py`

 * *Files identical despite different names*

### Comparing `ubicquia-0.1.4/ubicquia/utils.py` & `ubicquia-0.2.0/ubicquia/utils.py`

 * *Files identical despite different names*

### Comparing `ubicquia-0.1.4/ubicquia/wifi.py` & `ubicquia-0.2.0/ubicquia/wifi.py`

 * *Files identical despite different names*

### Comparing `ubicquia-0.1.4/ubicquia/wifi_captive_portal.py` & `ubicquia-0.2.0/ubicquia/wifi_captive_portal.py`

 * *Files identical despite different names*

### Comparing `ubicquia-0.1.4/ubicquia.egg-info/PKG-INFO` & `ubicquia-0.2.0/ubicquia.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubicquia
-Version: 0.1.4
+Version: 0.2.0
 Summary: Ubicquia API Client Library
 Author: CiberC Dev
 License: GPLv3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Ubicquia API client
@@ -18,14 +18,18 @@
 
 session = UbicquiaSession(..., )
 ubicquia = Ubicquia(session)
 ```
 
 ## Changes
 
-v012
+v020
 
-- Add node method current_node_state
+- Remove python-decouple dependency
 
 v014
 
 - New reports (energy usage and energy usage chart)
+
+v012
+
+- Add node method current_node_state
```

### Comparing `ubicquia-0.1.4/ubicquia.egg-info/SOURCES.txt` & `ubicquia-0.2.0/ubicquia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

