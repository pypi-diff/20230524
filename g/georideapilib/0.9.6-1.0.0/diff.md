# Comparing `tmp/georideapilib-0.9.6.tar.gz` & `tmp/georideapilib-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "georideapilib-0.9.6.tar", last modified: Fri Mar 24 22:13:50 2023, max compression
+gzip compressed data, was "georideapilib-1.0.0.tar", last modified: Wed May 24 10:36:37 2023, max compression
```

## Comparing `georideapilib-0.9.6.tar` & `georideapilib-1.0.0.tar`

### file list

```diff
@@ -1,35 +1,28 @@
-drwxr-xr-x   0 mduval    (1000) mduval    (1000)        0 2023-03-24 22:13:50.097935 georideapilib-0.9.6/
--rw-r--r--   0 mduval    (1000) mduval    (1000)       84 2022-03-04 14:44:43.000000 georideapilib-0.9.6/.gitignore
--rw-r--r--   0 mduval    (1000) mduval    (1000)      208 2019-10-25 20:05:24.000000 georideapilib-0.9.6/.travis.yml
--rw-r--r--   0 mduval    (1000) mduval    (1000)    35149 2019-10-26 23:46:45.000000 georideapilib-0.9.6/LICENSE
--rw-r--r--   0 mduval    (1000) mduval    (1000)      374 2023-03-24 22:13:50.097935 georideapilib-0.9.6/PKG-INFO
--rw-r--r--   0 mduval    (1000) mduval    (1000)     1087 2022-03-04 09:30:13.000000 georideapilib-0.9.6/README.md
-drwxr-xr-x   0 mduval    (1000) mduval    (1000)        0 2023-03-24 22:13:50.095935 georideapilib-0.9.6/examples/
--rw-r--r--   0 mduval    (1000) mduval    (1000)     5106 2023-03-24 21:59:16.000000 georideapilib-0.9.6/examples/example.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)    12381 2019-10-25 19:51:47.000000 georideapilib-0.9.6/georide-logo.png
-drwxr-xr-x   0 mduval    (1000) mduval    (1000)        0 2023-03-24 22:13:50.096935 georideapilib-0.9.6/georideapilib/
--rw-r--r--   0 mduval    (1000) mduval    (1000)    10753 2023-03-24 21:59:16.000000 georideapilib-0.9.6/georideapilib/api.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)      633 2021-04-11 15:41:10.000000 georideapilib-0.9.6/georideapilib/exception.py
-drwxr-xr-x   0 mduval    (1000) mduval    (1000)        0 2023-03-24 22:13:50.097935 georideapilib-0.9.6/georideapilib/objects/
--rw-r--r--   0 mduval    (1000) mduval    (1000)     1218 2023-03-24 21:59:55.000000 georideapilib-0.9.6/georideapilib/objects/GeoRideAccount.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)      728 2023-03-24 21:59:16.000000 georideapilib-0.9.6/georideapilib/objects/GeoRideSharedTrip.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)     3170 2023-03-24 21:59:16.000000 georideapilib-0.9.6/georideapilib/objects/GeoRideSubscription.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)     1084 2023-03-24 21:59:16.000000 georideapilib-0.9.6/georideapilib/objects/GeoRideSubscription_CardInfo.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)    21877 2023-03-24 22:13:01.000000 georideapilib-0.9.6/georideapilib/objects/GeoRideTracker.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)     3527 2023-03-24 21:59:16.000000 georideapilib-0.9.6/georideapilib/objects/GeoRideTrackerBeacon.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)     1460 2023-03-24 21:59:16.000000 georideapilib-0.9.6/georideapilib/objects/GeoRideTrackerPosition.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)     3605 2023-03-24 21:59:16.000000 georideapilib-0.9.6/georideapilib/objects/GeoRideTrackerTrip.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)     1935 2023-03-24 21:59:16.000000 georideapilib-0.9.6/georideapilib/objects/GeoRideUser.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)      360 2023-03-24 21:59:16.000000 georideapilib-0.9.6/georideapilib/objects/JsonMgtMetaClass.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)      351 2023-03-24 21:59:16.000000 georideapilib-0.9.6/georideapilib/objects/__init__.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)     3929 2022-03-19 20:43:23.000000 georideapilib-0.9.6/georideapilib/socket.py
-drwxr-xr-x   0 mduval    (1000) mduval    (1000)        0 2023-03-24 22:13:50.096935 georideapilib-0.9.6/georideapilib.egg-info/
--rw-r--r--   0 mduval    (1000) mduval    (1000)      374 2023-03-24 22:13:50.000000 georideapilib-0.9.6/georideapilib.egg-info/PKG-INFO
--rw-r--r--   0 mduval    (1000) mduval    (1000)      860 2023-03-24 22:13:50.000000 georideapilib-0.9.6/georideapilib.egg-info/SOURCES.txt
--rw-r--r--   0 mduval    (1000) mduval    (1000)        1 2023-03-24 22:13:50.000000 georideapilib-0.9.6/georideapilib.egg-info/dependency_links.txt
--rw-r--r--   0 mduval    (1000) mduval    (1000)       31 2023-03-24 22:13:50.000000 georideapilib-0.9.6/georideapilib.egg-info/requires.txt
--rw-r--r--   0 mduval    (1000) mduval    (1000)       14 2023-03-24 22:13:50.000000 georideapilib-0.9.6/georideapilib.egg-info/top_level.txt
--rw-r--r--   0 mduval    (1000) mduval    (1000)      528 2022-03-04 09:30:13.000000 georideapilib-0.9.6/logging.conf
--rw-r--r--   0 mduval    (1000) mduval    (1000)       79 2023-03-24 22:13:50.097935 georideapilib-0.9.6/setup.cfg
--rw-r--r--   0 mduval    (1000) mduval    (1000)     1217 2023-03-24 22:13:01.000000 georideapilib-0.9.6/setup.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)       72 2019-10-25 20:06:10.000000 georideapilib-0.9.6/test_requirements.txt
+drwxr-xr-x   0 mduval    (1000) mduval    (1000)        0 2023-05-24 10:36:37.530752 georideapilib-1.0.0/
+-rw-r--r--   0 mduval    (1000) mduval    (1000)    35149 2023-02-27 17:50:53.000000 georideapilib-1.0.0/LICENSE
+-rw-r--r--   0 mduval    (1000) mduval    (1000)      374 2023-05-24 10:36:37.534085 georideapilib-1.0.0/PKG-INFO
+-rw-r--r--   0 mduval    (1000) mduval    (1000)     1087 2023-02-27 17:50:53.000000 georideapilib-1.0.0/README.md
+drwxr-xr-x   0 mduval    (1000) mduval    (1000)        0 2023-05-24 10:36:37.517419 georideapilib-1.0.0/georideapilib/
+-rw-r--r--   0 mduval    (1000) mduval    (1000)    10805 2023-05-24 10:34:47.000000 georideapilib-1.0.0/georideapilib/api.py
+-rw-r--r--   0 mduval    (1000) mduval    (1000)      633 2023-02-27 17:50:53.000000 georideapilib-1.0.0/georideapilib/exception.py
+drwxr-xr-x   0 mduval    (1000) mduval    (1000)        0 2023-05-24 10:36:37.530752 georideapilib-1.0.0/georideapilib/objects/
+-rw-r--r--   0 mduval    (1000) mduval    (1000)     1218 2023-02-27 19:06:34.000000 georideapilib-1.0.0/georideapilib/objects/GeoRideAccount.py
+-rw-r--r--   0 mduval    (1000) mduval    (1000)      728 2023-02-27 17:54:17.000000 georideapilib-1.0.0/georideapilib/objects/GeoRideSharedTrip.py
+-rw-r--r--   0 mduval    (1000) mduval    (1000)     3170 2023-02-27 17:54:17.000000 georideapilib-1.0.0/georideapilib/objects/GeoRideSubscription.py
+-rw-r--r--   0 mduval    (1000) mduval    (1000)     1084 2023-02-27 17:54:17.000000 georideapilib-1.0.0/georideapilib/objects/GeoRideSubscription_CardInfo.py
+-rw-r--r--   0 mduval    (1000) mduval    (1000)    21877 2023-05-24 10:32:51.000000 georideapilib-1.0.0/georideapilib/objects/GeoRideTracker.py
+-rw-r--r--   0 mduval    (1000) mduval    (1000)     3527 2023-02-27 17:54:17.000000 georideapilib-1.0.0/georideapilib/objects/GeoRideTrackerBeacon.py
+-rw-r--r--   0 mduval    (1000) mduval    (1000)     1460 2023-02-27 17:54:17.000000 georideapilib-1.0.0/georideapilib/objects/GeoRideTrackerPosition.py
+-rw-r--r--   0 mduval    (1000) mduval    (1000)     3605 2023-02-27 17:54:17.000000 georideapilib-1.0.0/georideapilib/objects/GeoRideTrackerTrip.py
+-rw-r--r--   0 mduval    (1000) mduval    (1000)     1935 2023-02-27 17:54:17.000000 georideapilib-1.0.0/georideapilib/objects/GeoRideUser.py
+-rw-r--r--   0 mduval    (1000) mduval    (1000)      360 2023-02-27 17:54:17.000000 georideapilib-1.0.0/georideapilib/objects/JsonMgtMetaClass.py
+-rw-r--r--   0 mduval    (1000) mduval    (1000)      351 2023-02-27 17:54:17.000000 georideapilib-1.0.0/georideapilib/objects/__init__.py
+-rw-r--r--   0 mduval    (1000) mduval    (1000)     3935 2023-05-24 10:34:47.000000 georideapilib-1.0.0/georideapilib/socket.py
+drwxr-xr-x   0 mduval    (1000) mduval    (1000)        0 2023-05-24 10:36:37.520752 georideapilib-1.0.0/georideapilib.egg-info/
+-rw-r--r--   0 mduval    (1000) mduval    (1000)      374 2023-05-24 10:36:37.000000 georideapilib-1.0.0/georideapilib.egg-info/PKG-INFO
+-rw-r--r--   0 mduval    (1000) mduval    (1000)      765 2023-05-24 10:36:37.000000 georideapilib-1.0.0/georideapilib.egg-info/SOURCES.txt
+-rw-r--r--   0 mduval    (1000) mduval    (1000)        1 2023-05-24 10:36:37.000000 georideapilib-1.0.0/georideapilib.egg-info/dependency_links.txt
+-rw-r--r--   0 mduval    (1000) mduval    (1000)       31 2023-05-24 10:36:37.000000 georideapilib-1.0.0/georideapilib.egg-info/requires.txt
+-rw-r--r--   0 mduval    (1000) mduval    (1000)       14 2023-05-24 10:36:37.000000 georideapilib-1.0.0/georideapilib.egg-info/top_level.txt
+-rw-r--r--   0 mduval    (1000) mduval    (1000)       79 2023-05-24 10:36:37.534085 georideapilib-1.0.0/setup.cfg
+-rw-r--r--   0 mduval    (1000) mduval    (1000)     1217 2023-05-24 10:34:47.000000 georideapilib-1.0.0/setup.py
```

### Comparing `georideapilib-0.9.6/LICENSE` & `georideapilib-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `georideapilib-0.9.6/README.md` & `georideapilib-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `georideapilib-0.9.6/georideapilib/api.py` & `georideapilib-1.0.0/georideapilib/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 
 from georideapilib.exception import (
     LoginException,
     SeverException,
     UnauthorizedException
 )
 
-GEORIDE_API_HOST = "https://api.georide.fr"
+GEORIDE_API_HOST = "https://api.georide.com"
+GEORIDE_SOCKET_HOST = "https://socket.georide.com"
 GEORIDE_API_ENDPOINT_LOGIN = "/user/login"
 GEORIDE_API_ENDPOINT_NEW_TOKEN = "/user/new-token"
 GEORIDE_API_ENDPOINT_LOGOUT = "/user/logout"
 GEORIDE_API_ENDPOINT_USER = "/user"
 GEORIDE_API_ENDPOINT_TRACKERS = "/user/trackers"
 GEORIDE_API_ENDPOINT_TRIPS = "/tracker/{trackerId}/trips"
 GEORIDE_API_ENDPOINT_LOCK = "/tracker/{trackerId}/lock"
```

### Comparing `georideapilib-0.9.6/georideapilib/exception.py` & `georideapilib-1.0.0/georideapilib/exception.py`

 * *Files identical despite different names*

### Comparing `georideapilib-0.9.6/georideapilib/objects/GeoRideAccount.py` & `georideapilib-1.0.0/georideapilib/objects/GeoRideAccount.py`

 * *Files identical despite different names*

### Comparing `georideapilib-0.9.6/georideapilib/objects/GeoRideSharedTrip.py` & `georideapilib-1.0.0/georideapilib/objects/GeoRideSharedTrip.py`

 * *Files identical despite different names*

### Comparing `georideapilib-0.9.6/georideapilib/objects/GeoRideSubscription.py` & `georideapilib-1.0.0/georideapilib/objects/GeoRideSubscription.py`

 * *Files identical despite different names*

### Comparing `georideapilib-0.9.6/georideapilib/objects/GeoRideSubscription_CardInfo.py` & `georideapilib-1.0.0/georideapilib/objects/GeoRideSubscription_CardInfo.py`

 * *Files identical despite different names*

### Comparing `georideapilib-0.9.6/georideapilib/objects/GeoRideTracker.py` & `georideapilib-1.0.0/georideapilib/objects/GeoRideTracker.py`

 * *Files identical despite different names*

### Comparing `georideapilib-0.9.6/georideapilib/objects/GeoRideTrackerBeacon.py` & `georideapilib-1.0.0/georideapilib/objects/GeoRideTrackerBeacon.py`

 * *Files identical despite different names*

### Comparing `georideapilib-0.9.6/georideapilib/objects/GeoRideTrackerPosition.py` & `georideapilib-1.0.0/georideapilib/objects/GeoRideTrackerPosition.py`

 * *Files identical despite different names*

### Comparing `georideapilib-0.9.6/georideapilib/objects/GeoRideTrackerTrip.py` & `georideapilib-1.0.0/georideapilib/objects/GeoRideTrackerTrip.py`

 * *Files identical despite different names*

### Comparing `georideapilib-0.9.6/georideapilib/objects/GeoRideUser.py` & `georideapilib-1.0.0/georideapilib/objects/GeoRideUser.py`

 * *Files identical despite different names*

### Comparing `georideapilib-0.9.6/georideapilib/socket.py` & `georideapilib-1.0.0/georideapilib/socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ GeoRide socket-io implementation """
 import logging
 import socketio
 
-from georideapilib.api import GEORIDE_API_HOST
+from georideapilib.api import GEORIDE_SOCKET_HOST
 
 _LOGGER = logging.getLogger(__name__)
 
 sio = socketio.Client(reconnection=True) # pylint: disable=C0103
 
 @sio.on('connect')
 def on_connect():
@@ -100,15 +100,15 @@
             if self._on_locked_callback is not None:
                 self._on_locked_callback(data)        
         self._initialised = True
 
     def connect(self, auth_token):
         """ connect to the georide socket"""
         if self._initialised is not False:
-            sio.connect(GEORIDE_API_HOST, headers={'token': auth_token})
+            sio.connect(GEORIDE_SOCKET_HOST, headers={'token': auth_token})
             sio.wait()
         else:
             _LOGGER.error("Please call init() before")
         
     def disconnect(self):
         """disconnect from the georide socket"""
         sio.disconnect()
```

### Comparing `georideapilib-0.9.6/georideapilib.egg-info/SOURCES.txt` & `georideapilib-1.0.0/georideapilib.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,11 @@
-.gitignore
-.travis.yml
 LICENSE
 README.md
-georide-logo.png
-logging.conf
 setup.cfg
 setup.py
-test_requirements.txt
-examples/example.py
 georideapilib/api.py
 georideapilib/exception.py
 georideapilib/socket.py
 georideapilib.egg-info/PKG-INFO
 georideapilib.egg-info/SOURCES.txt
 georideapilib.egg-info/dependency_links.txt
 georideapilib.egg-info/requires.txt
```

### Comparing `georideapilib-0.9.6/setup.py` & `georideapilib-1.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 # make pythonpack
 # python setup.py register sdist upload
 # and be sure to test it firstly using
 # "python setup.py register sdist upload -r pypitest"
 setup(
     name='georideapilib',
     packages=['georideapilib', 'georideapilib.objects'],  # this must be the same as the name above
-    version='0.9.6',
+    version='1.0.0',
     description='Lib to control GeoRide tracker devices with theire rest api',
     author='Matthieu DUVAL',
     author_email='georideapilib@duval-dev.fr',
     # use the URL to the github repo
     url='https://github.com/hacf/georide-api',
-    download_url='https://codeload.github.com/hacf/georide-api/tar.gz/0.9.3',
+    download_url='https://codeload.github.com/hacf/georide-api/tar.gz/1.0.0',
     keywords=['rest', 'georide', 'api', 'grutier', 'GeoRide'],  # arbitrary keywords
     classifiers=[],
-    install_requires=["python-socketio[client]==4.6.1"],
+    install_requires=["python-socketio[client]==5.8.0"],
     tests_require=[
         'pytest>=3.7',
         'pytest-pep8',  
         'pytest-cov',
         'python-coveralls',
         'pylint',
         'coverage>=4.4'
```

