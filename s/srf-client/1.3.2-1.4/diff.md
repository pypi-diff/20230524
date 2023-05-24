# Comparing `tmp/srf-client-1.3.2.tar.gz` & `tmp/srf-client-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/srf-client-1.3.2.tar", last modified: Wed Nov 30 11:46:36 2022, max compression
+gzip compressed data, was "dist/srf-client-1.4.tar", last modified: Wed May 24 13:22:09 2023, max compression
```

## Comparing `srf-client-1.3.2.tar` & `srf-client-1.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0     1000     1004        0 2022-11-30 11:46:36.000000 srf-client-1.3.2/
--rw-r--r--   0     1000     1004     1067 2022-09-02 16:05:39.000000 srf-client-1.3.2/LICENSE
--rw-r--r--   0     1000     1004     1271 2022-11-30 11:46:36.000000 srf-client-1.3.2/PKG-INFO
--rw-r--r--   0     1000     1004      439 2022-11-30 11:46:36.000000 srf-client-1.3.2/setup.cfg
--rwxr-xr-x   0     1000     1004     2291 2022-11-30 11:45:30.000000 srf-client-1.3.2/setup.py
-drwxr-xr-x   0     1000     1004        0 2022-11-30 11:46:36.000000 srf-client-1.3.2/srf_client/
--rw-r--r--   0     1000     1004     2337 2022-09-02 16:05:39.000000 srf-client-1.3.2/srf_client/__init__.py
--rw-r--r--   0     1000     1004     5941 2022-09-02 16:05:39.000000 srf-client-1.3.2/srf_client/client.py
--rw-r--r--   0     1000     1004     2221 2022-11-08 17:40:49.000000 srf-client-1.3.2/srf_client/filter.py
--rw-r--r--   0     1000     1004     1805 2022-09-02 16:05:39.000000 srf-client-1.3.2/srf_client/fleets.py
--rw-r--r--   0     1000     1004     4222 2022-09-02 16:05:39.000000 srf-client-1.3.2/srf_client/legs.py
--rw-r--r--   0     1000     1004     1018 2022-09-02 16:05:39.000000 srf-client-1.3.2/srf_client/locations.py
--rw-r--r--   0     1000     1004    20431 2022-09-02 16:05:39.000000 srf-client-1.3.2/srf_client/model.py
--rw-r--r--   0     1000     1004    10202 2022-09-02 16:05:39.000000 srf-client-1.3.2/srf_client/oauth.py
--rw-r--r--   0     1000     1004     2052 2022-09-02 16:05:39.000000 srf-client-1.3.2/srf_client/orders.py
--rw-r--r--   0     1000     1004      883 2022-09-02 16:05:39.000000 srf-client-1.3.2/srf_client/organisations.py
--rw-r--r--   0     1000     1004     3985 2022-09-02 16:05:39.000000 srf-client-1.3.2/srf_client/paging.py
--rw-r--r--   0     1000     1004     3604 2022-09-02 16:05:39.000000 srf-client-1.3.2/srf_client/pandas.py
--rw-r--r--   0     1000     1004     2649 2022-09-02 16:05:39.000000 srf-client-1.3.2/srf_client/routes.py
--rw-r--r--   0     1000     1004      832 2022-09-02 16:05:39.000000 srf-client-1.3.2/srf_client/sort.py
--rw-r--r--   0     1000     1004     1167 2022-09-02 16:05:39.000000 srf-client-1.3.2/srf_client/trailers.py
--rw-r--r--   0     1000     1004      907 2022-09-02 16:05:39.000000 srf-client-1.3.2/srf_client/trials.py
--rw-r--r--   0     1000     1004     2695 2022-09-02 16:05:39.000000 srf-client-1.3.2/srf_client/trips.py
--rw-r--r--   0     1000     1004      789 2022-09-02 16:05:39.000000 srf-client-1.3.2/srf_client/util.py
--rw-r--r--   0     1000     1004     2610 2022-09-02 16:05:39.000000 srf-client-1.3.2/srf_client/vehicle_classes.py
--rw-r--r--   0     1000     1004     1675 2022-09-02 16:05:39.000000 srf-client-1.3.2/srf_client/vehicles.py
-drwxr-xr-x   0     1000     1004        0 2022-11-30 11:46:36.000000 srf-client-1.3.2/srf_client.egg-info/
--rw-r--r--   0     1000     1004     1271 2022-11-30 11:46:36.000000 srf-client-1.3.2/srf_client.egg-info/PKG-INFO
--rw-r--r--   0     1000     1004      631 2022-11-30 11:46:36.000000 srf-client-1.3.2/srf_client.egg-info/SOURCES.txt
--rw-r--r--   0     1000     1004        1 2022-11-30 11:46:36.000000 srf-client-1.3.2/srf_client.egg-info/dependency_links.txt
--rw-r--r--   0     1000     1004      183 2022-11-30 11:46:36.000000 srf-client-1.3.2/srf_client.egg-info/requires.txt
--rw-r--r--   0     1000     1004       11 2022-11-30 11:46:36.000000 srf-client-1.3.2/srf_client.egg-info/top_level.txt
+drwxr-xr-x   0     1000     1004        0 2023-05-24 13:22:09.000000 srf-client-1.4/
+-rw-r--r--   0     1000     1004     1067 2022-09-02 16:05:39.000000 srf-client-1.4/LICENSE
+-rw-r--r--   0     1000     1004     1269 2023-05-24 13:22:09.000000 srf-client-1.4/PKG-INFO
+-rw-r--r--   0     1000     1004      439 2023-05-24 13:22:09.000000 srf-client-1.4/setup.cfg
+-rwxr-xr-x   0     1000     1004     2289 2023-05-24 13:21:14.000000 srf-client-1.4/setup.py
+drwxr-xr-x   0     1000     1004        0 2023-05-24 13:22:09.000000 srf-client-1.4/srf_client/
+-rw-r--r--   0     1000     1004     2337 2022-09-02 16:05:39.000000 srf-client-1.4/srf_client/__init__.py
+-rw-r--r--   0     1000     1004     6321 2023-05-24 13:21:14.000000 srf-client-1.4/srf_client/client.py
+-rw-r--r--   0     1000     1004     2221 2022-11-08 17:40:49.000000 srf-client-1.4/srf_client/filter.py
+-rw-r--r--   0     1000     1004     1805 2022-09-02 16:05:39.000000 srf-client-1.4/srf_client/fleets.py
+-rw-r--r--   0     1000     1004     6045 2023-05-24 13:21:14.000000 srf-client-1.4/srf_client/legs.py
+-rw-r--r--   0     1000     1004     1018 2022-09-02 16:05:39.000000 srf-client-1.4/srf_client/locations.py
+-rw-r--r--   0     1000     1004    20815 2023-05-24 13:21:14.000000 srf-client-1.4/srf_client/model.py
+-rw-r--r--   0     1000     1004    10203 2023-05-24 13:21:14.000000 srf-client-1.4/srf_client/oauth.py
+-rw-r--r--   0     1000     1004     2052 2022-09-02 16:05:39.000000 srf-client-1.4/srf_client/orders.py
+-rw-r--r--   0     1000     1004      883 2022-09-02 16:05:39.000000 srf-client-1.4/srf_client/organisations.py
+-rw-r--r--   0     1000     1004     3985 2022-09-02 16:05:39.000000 srf-client-1.4/srf_client/paging.py
+-rw-r--r--   0     1000     1004     4159 2023-05-24 13:21:14.000000 srf-client-1.4/srf_client/pandas.py
+-rw-r--r--   0     1000     1004     2649 2022-09-02 16:05:39.000000 srf-client-1.4/srf_client/routes.py
+-rw-r--r--   0     1000     1004      832 2022-09-02 16:05:39.000000 srf-client-1.4/srf_client/sort.py
+-rw-r--r--   0     1000     1004     1167 2022-09-02 16:05:39.000000 srf-client-1.4/srf_client/trailers.py
+-rw-r--r--   0     1000     1004      907 2022-09-02 16:05:39.000000 srf-client-1.4/srf_client/trials.py
+-rw-r--r--   0     1000     1004     2695 2022-09-02 16:05:39.000000 srf-client-1.4/srf_client/trips.py
+-rw-r--r--   0     1000     1004      789 2022-09-02 16:05:39.000000 srf-client-1.4/srf_client/util.py
+-rw-r--r--   0     1000     1004     2610 2022-09-02 16:05:39.000000 srf-client-1.4/srf_client/vehicle_classes.py
+-rw-r--r--   0     1000     1004     1675 2022-09-02 16:05:39.000000 srf-client-1.4/srf_client/vehicles.py
+drwxr-xr-x   0     1000     1004        0 2023-05-24 13:22:09.000000 srf-client-1.4/srf_client.egg-info/
+-rw-r--r--   0     1000     1004     1269 2023-05-24 13:22:08.000000 srf-client-1.4/srf_client.egg-info/PKG-INFO
+-rw-r--r--   0     1000     1004      631 2023-05-24 13:22:08.000000 srf-client-1.4/srf_client.egg-info/SOURCES.txt
+-rw-r--r--   0     1000     1004        1 2023-05-24 13:22:08.000000 srf-client-1.4/srf_client.egg-info/dependency_links.txt
+-rw-r--r--   0     1000     1004      183 2023-05-24 13:22:08.000000 srf-client-1.4/srf_client.egg-info/requires.txt
+-rw-r--r--   0     1000     1004       11 2023-05-24 13:22:08.000000 srf-client-1.4/srf_client.egg-info/top_level.txt
```

### Comparing `srf-client-1.3.2/LICENSE` & `srf-client-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `srf-client-1.3.2/PKG-INFO` & `srf-client-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srf-client
-Version: 1.3.2
+Version: 1.4
 Summary: Centre for Sustainable Road Freight - Data Platform client
 Home-page: https://data.csrf.ac.uk
 Author: James Howe
 Author-email: jmh205@cam.ac.uk
 Maintainer: Centre for Sustainable Road Freight
 Maintainer-email: tech@csrf.ac.uk
 License: MIT
```

### Comparing `srf-client-1.3.2/setup.py` & `srf-client-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 import os
 
 from setuptools import find_packages, setup
 
-__version__ = '1.3.2'
+__version__ = '1.4'
 
 try:
     if os.environ['GIT_BRANCH'] == 'master':
         __version__ += '.dev' + os.environ['BUILD_NUMBER']
 except KeyError:
     pass
```

### Comparing `srf-client-1.3.2/srf_client/__init__.py` & `srf-client-1.4/srf_client/__init__.py`

 * *Files identical despite different names*

### Comparing `srf-client-1.3.2/srf_client/client.py` & `srf-client-1.4/srf_client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,14 +106,24 @@
 
         :param url: Request URL. Will be resolved relative to the API root.
         :param kwargs: Additional options for request
         """
         url, kwargs = self._prepare_request(url, kwargs)
         return self._session.get(url=url, **kwargs)
 
+    def post(self, url, **kwargs) -> Response:
+        """
+        Perform a raw POST request. Probably requires write scope.
+
+        :param url: Request URL. Will be resolved relative to the API root.
+        :param kwargs: Additional options for request
+        """
+        url, kwargs = self._prepare_request(url, kwargs)
+        return self._session.post(url=url, **kwargs)
+
     def ping(self, timeout=2) -> bool:
         """
         Check whether the service is reachable.
 
         May fail due to server-side errors, invalid authentication,
         or incorrect configuration.
```

### Comparing `srf-client-1.3.2/srf_client/filter.py` & `srf-client-1.4/srf_client/filter.py`

 * *Files identical despite different names*

### Comparing `srf-client-1.3.2/srf_client/fleets.py` & `srf-client-1.4/srf_client/fleets.py`

 * *Files identical despite different names*

### Comparing `srf-client-1.3.2/srf_client/locations.py` & `srf-client-1.4/srf_client/locations.py`

 * *Files identical despite different names*

### Comparing `srf-client-1.3.2/srf_client/model.py` & `srf-client-1.4/srf_client/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,26 +322,36 @@
     def calibration(self) -> 'Calibration':  # noqa: D102
         return self._client.legs.get_calibration(self)
 
     def get_data(self, include=None) -> Iterable['Measurement']:
         """
         Return available measurements.
 
-        :param include: Data types to include. By default all are included.
+        :param include: Data types to include. By default, all are included.
         """
         return self._client.legs.get_data(self, include=include)
 
     def get_raw_data(self, include=None) -> Iterable['Measurement']:
         """
         Return the raw measurements.
 
-        :param include: Data types to include. By default all are included.
+        :param include: Data types to include. By default, all are included.
         """
         return self._client.legs.get_raw_data(self, include=include)
 
+    def get_gradient(self, **kwargs) -> Iterable['Measurement']:
+        """
+        Return computed gradient data for the leg.
+
+        :param leg: Parent leg object
+        :param generate: Request and wait for generation if not available
+        :param timeout: How long to wait if requesting generation
+        """
+        return self._client.legs.get_gradient(self, **kwargs)
+
 
 @attr.s(frozen=True, slots=True, auto_attribs=True, kw_only=True)
 class Calibration:
     """
     Leg calibration data for vehicle dynamics.
 
     :param forward: Unit vector pointing in the direction of forward travel
```

### Comparing `srf-client-1.3.2/srf_client/oauth.py` & `srf-client-1.4/srf_client/oauth.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,35 +89,35 @@
 
     srf = SRFDataOAuth(client_id='...', client_secret='...', scope=('CLIENT',))
     srf.login_with_client()
     srf.ping()
 
 """
 
-from typing import Callable, Mapping, Sequence
-from urllib.parse import urljoin
 from oauthlib.oauth2 import BackendApplicationClient, OAuth2Error, \
     WebApplicationClient
 from requests import RequestException
 from requests_oauthlib import OAuth2Session
+from typing import Callable, Mapping, Sequence
+from urllib.parse import urljoin
 
 from .client import SRFData
 
 __all__ = ['SRFDataOAuth']
 
 
 def make_urls(server_root):
     """
     Build keyword arguments for a non-standard server root.
 
     Useful for testing:
 
     .. code:: python
 
-        srf = SRFDataOAuth(client_id='TEST', client_secret='TEST,
+        srf = SRFDataOAuth(client_id='TEST', client_secret='TEST',
                            **make_urls('https://localhost:8443')
 
     """
     return {'root': urljoin(server_root, 'api'),
             'redirect_uri': urljoin(server_root, 'oauth/callback'),
             'auth_endpoint': urljoin(server_root, 'oauth/authorize'),
             'token_endpoint': urljoin(server_root, 'oauth/token'),
```

### Comparing `srf-client-1.3.2/srf_client/orders.py` & `srf-client-1.4/srf_client/orders.py`

 * *Files identical despite different names*

### Comparing `srf-client-1.3.2/srf_client/organisations.py` & `srf-client-1.4/srf_client/organisations.py`

 * *Files identical despite different names*

### Comparing `srf-client-1.3.2/srf_client/paging.py` & `srf-client-1.4/srf_client/paging.py`

 * *Files identical despite different names*

### Comparing `srf-client-1.3.2/srf_client/pandas.py` & `srf-client-1.4/srf_client/pandas.py`

 * *Files 12% similar despite different names*

```diff
@@ -90,9 +90,27 @@
     collected = [df for df in collected if not df.empty]
     if not collected:
         return pd.DataFrame()
     else:
         return reduce(pd.DataFrame.join, collected)
 
 
+def get_gradient_frame(self: Leg, **kwargs) -> pd.DataFrame:
+    type_defs = self._client.get_types()
+    columns = ['9 ' + field.name for field in type_defs['9'].fields]
+
+    data = self.get_gradient(**kwargs)
+    if not data:
+        return pd.DataFrame()
+
+    df = pd.DataFrame.from_records(
+        ((pd.to_datetime(m.timestamp, unit='ms'), *(
+            pd.to_numeric(v) for v in m.data.split(','))) for m in data),
+        index='timestamp',
+        columns=['timestamp', *columns]
+    )
+    return df
+
+
 Leg.get_data_frame = get_data_frame
 Trip.get_data_frame = get_data_frame
+Leg.get_gradient_frame = get_gradient_frame
```

### Comparing `srf-client-1.3.2/srf_client/routes.py` & `srf-client-1.4/srf_client/routes.py`

 * *Files identical despite different names*

### Comparing `srf-client-1.3.2/srf_client/sort.py` & `srf-client-1.4/srf_client/sort.py`

 * *Files identical despite different names*

### Comparing `srf-client-1.3.2/srf_client/trailers.py` & `srf-client-1.4/srf_client/trailers.py`

 * *Files identical despite different names*

### Comparing `srf-client-1.3.2/srf_client/trials.py` & `srf-client-1.4/srf_client/trials.py`

 * *Files identical despite different names*

### Comparing `srf-client-1.3.2/srf_client/trips.py` & `srf-client-1.4/srf_client/trips.py`

 * *Files identical despite different names*

### Comparing `srf-client-1.3.2/srf_client/util.py` & `srf-client-1.4/srf_client/util.py`

 * *Files identical despite different names*

### Comparing `srf-client-1.3.2/srf_client/vehicle_classes.py` & `srf-client-1.4/srf_client/vehicle_classes.py`

 * *Files identical despite different names*

### Comparing `srf-client-1.3.2/srf_client/vehicles.py` & `srf-client-1.4/srf_client/vehicles.py`

 * *Files identical despite different names*

### Comparing `srf-client-1.3.2/srf_client.egg-info/PKG-INFO` & `srf-client-1.4/srf_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srf-client
-Version: 1.3.2
+Version: 1.4
 Summary: Centre for Sustainable Road Freight - Data Platform client
 Home-page: https://data.csrf.ac.uk
 Author: James Howe
 Author-email: jmh205@cam.ac.uk
 Maintainer: Centre for Sustainable Road Freight
 Maintainer-email: tech@csrf.ac.uk
 License: MIT
```

### Comparing `srf-client-1.3.2/srf_client.egg-info/SOURCES.txt` & `srf-client-1.4/srf_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

