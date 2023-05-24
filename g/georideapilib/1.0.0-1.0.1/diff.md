# Comparing `tmp/georideapilib-1.0.0.tar.gz` & `tmp/georideapilib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "georideapilib-1.0.0.tar", last modified: Wed May 24 10:36:37 2023, max compression
+gzip compressed data, was "georideapilib-1.0.1.tar", last modified: Wed May 24 11:37:55 2023, max compression
```

## Comparing `georideapilib-1.0.0.tar` & `georideapilib-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mduval    (1000) mduval    (1000)        0 2023-05-24 10:36:37.530752 georideapilib-1.0.0/
--rw-r--r--   0 mduval    (1000) mduval    (1000)    35149 2023-02-27 17:50:53.000000 georideapilib-1.0.0/LICENSE
--rw-r--r--   0 mduval    (1000) mduval    (1000)      374 2023-05-24 10:36:37.534085 georideapilib-1.0.0/PKG-INFO
--rw-r--r--   0 mduval    (1000) mduval    (1000)     1087 2023-02-27 17:50:53.000000 georideapilib-1.0.0/README.md
-drwxr-xr-x   0 mduval    (1000) mduval    (1000)        0 2023-05-24 10:36:37.517419 georideapilib-1.0.0/georideapilib/
--rw-r--r--   0 mduval    (1000) mduval    (1000)    10805 2023-05-24 10:34:47.000000 georideapilib-1.0.0/georideapilib/api.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)      633 2023-02-27 17:50:53.000000 georideapilib-1.0.0/georideapilib/exception.py
-drwxr-xr-x   0 mduval    (1000) mduval    (1000)        0 2023-05-24 10:36:37.530752 georideapilib-1.0.0/georideapilib/objects/
--rw-r--r--   0 mduval    (1000) mduval    (1000)     1218 2023-02-27 19:06:34.000000 georideapilib-1.0.0/georideapilib/objects/GeoRideAccount.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)      728 2023-02-27 17:54:17.000000 georideapilib-1.0.0/georideapilib/objects/GeoRideSharedTrip.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)     3170 2023-02-27 17:54:17.000000 georideapilib-1.0.0/georideapilib/objects/GeoRideSubscription.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)     1084 2023-02-27 17:54:17.000000 georideapilib-1.0.0/georideapilib/objects/GeoRideSubscription_CardInfo.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)    21877 2023-05-24 10:32:51.000000 georideapilib-1.0.0/georideapilib/objects/GeoRideTracker.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)     3527 2023-02-27 17:54:17.000000 georideapilib-1.0.0/georideapilib/objects/GeoRideTrackerBeacon.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)     1460 2023-02-27 17:54:17.000000 georideapilib-1.0.0/georideapilib/objects/GeoRideTrackerPosition.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)     3605 2023-02-27 17:54:17.000000 georideapilib-1.0.0/georideapilib/objects/GeoRideTrackerTrip.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)     1935 2023-02-27 17:54:17.000000 georideapilib-1.0.0/georideapilib/objects/GeoRideUser.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)      360 2023-02-27 17:54:17.000000 georideapilib-1.0.0/georideapilib/objects/JsonMgtMetaClass.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)      351 2023-02-27 17:54:17.000000 georideapilib-1.0.0/georideapilib/objects/__init__.py
--rw-r--r--   0 mduval    (1000) mduval    (1000)     3935 2023-05-24 10:34:47.000000 georideapilib-1.0.0/georideapilib/socket.py
-drwxr-xr-x   0 mduval    (1000) mduval    (1000)        0 2023-05-24 10:36:37.520752 georideapilib-1.0.0/georideapilib.egg-info/
--rw-r--r--   0 mduval    (1000) mduval    (1000)      374 2023-05-24 10:36:37.000000 georideapilib-1.0.0/georideapilib.egg-info/PKG-INFO
--rw-r--r--   0 mduval    (1000) mduval    (1000)      765 2023-05-24 10:36:37.000000 georideapilib-1.0.0/georideapilib.egg-info/SOURCES.txt
--rw-r--r--   0 mduval    (1000) mduval    (1000)        1 2023-05-24 10:36:37.000000 georideapilib-1.0.0/georideapilib.egg-info/dependency_links.txt
--rw-r--r--   0 mduval    (1000) mduval    (1000)       31 2023-05-24 10:36:37.000000 georideapilib-1.0.0/georideapilib.egg-info/requires.txt
--rw-r--r--   0 mduval    (1000) mduval    (1000)       14 2023-05-24 10:36:37.000000 georideapilib-1.0.0/georideapilib.egg-info/top_level.txt
--rw-r--r--   0 mduval    (1000) mduval    (1000)       79 2023-05-24 10:36:37.534085 georideapilib-1.0.0/setup.cfg
--rw-r--r--   0 mduval    (1000) mduval    (1000)     1217 2023-05-24 10:34:47.000000 georideapilib-1.0.0/setup.py
+drwxr-xr-x   0 mduval    (1000) mduval    (1000)        0 2023-05-24 11:37:55.384147 georideapilib-1.0.1/
+-rw-r--r--   0 mduval    (1000) mduval    (1000)    35149 2023-02-27 17:50:53.000000 georideapilib-1.0.1/LICENSE
+-rw-r--r--   0 mduval    (1000) mduval    (1000)      374 2023-05-24 11:37:55.384147 georideapilib-1.0.1/PKG-INFO
+-rw-r--r--   0 mduval    (1000) mduval    (1000)     1087 2023-02-27 17:50:53.000000 georideapilib-1.0.1/README.md
+drwxr-xr-x   0 mduval    (1000) mduval    (1000)        0 2023-05-24 11:37:55.380814 georideapilib-1.0.1/georideapilib/
+-rw-r--r--   0 mduval    (1000) mduval    (1000)    10805 2023-05-24 10:34:47.000000 georideapilib-1.0.1/georideapilib/api.py
+-rw-r--r--   0 mduval    (1000) mduval    (1000)      633 2023-02-27 17:50:53.000000 georideapilib-1.0.1/georideapilib/exception.py
+drwxr-xr-x   0 mduval    (1000) mduval    (1000)        0 2023-05-24 11:37:55.384147 georideapilib-1.0.1/georideapilib/objects/
+-rw-r--r--   0 mduval    (1000) mduval    (1000)     1218 2023-02-27 19:06:34.000000 georideapilib-1.0.1/georideapilib/objects/GeoRideAccount.py
+-rw-r--r--   0 mduval    (1000) mduval    (1000)      728 2023-02-27 17:54:17.000000 georideapilib-1.0.1/georideapilib/objects/GeoRideSharedTrip.py
+-rw-r--r--   0 mduval    (1000) mduval    (1000)     3170 2023-02-27 17:54:17.000000 georideapilib-1.0.1/georideapilib/objects/GeoRideSubscription.py
+-rw-r--r--   0 mduval    (1000) mduval    (1000)     1084 2023-02-27 17:54:17.000000 georideapilib-1.0.1/georideapilib/objects/GeoRideSubscription_CardInfo.py
+-rw-r--r--   0 mduval    (1000) mduval    (1000)    21877 2023-05-24 10:32:51.000000 georideapilib-1.0.1/georideapilib/objects/GeoRideTracker.py
+-rw-r--r--   0 mduval    (1000) mduval    (1000)     3527 2023-02-27 17:54:17.000000 georideapilib-1.0.1/georideapilib/objects/GeoRideTrackerBeacon.py
+-rw-r--r--   0 mduval    (1000) mduval    (1000)     1460 2023-02-27 17:54:17.000000 georideapilib-1.0.1/georideapilib/objects/GeoRideTrackerPosition.py
+-rw-r--r--   0 mduval    (1000) mduval    (1000)     3605 2023-02-27 17:54:17.000000 georideapilib-1.0.1/georideapilib/objects/GeoRideTrackerTrip.py
+-rw-r--r--   0 mduval    (1000) mduval    (1000)     1935 2023-02-27 17:54:17.000000 georideapilib-1.0.1/georideapilib/objects/GeoRideUser.py
+-rw-r--r--   0 mduval    (1000) mduval    (1000)      360 2023-02-27 17:54:17.000000 georideapilib-1.0.1/georideapilib/objects/JsonMgtMetaClass.py
+-rw-r--r--   0 mduval    (1000) mduval    (1000)      351 2023-02-27 17:54:17.000000 georideapilib-1.0.1/georideapilib/objects/__init__.py
+-rw-r--r--   0 mduval    (1000) mduval    (1000)     3935 2023-05-24 10:34:47.000000 georideapilib-1.0.1/georideapilib/socket.py
+drwxr-xr-x   0 mduval    (1000) mduval    (1000)        0 2023-05-24 11:37:55.380814 georideapilib-1.0.1/georideapilib.egg-info/
+-rw-r--r--   0 mduval    (1000) mduval    (1000)      374 2023-05-24 11:37:55.000000 georideapilib-1.0.1/georideapilib.egg-info/PKG-INFO
+-rw-r--r--   0 mduval    (1000) mduval    (1000)      765 2023-05-24 11:37:55.000000 georideapilib-1.0.1/georideapilib.egg-info/SOURCES.txt
+-rw-r--r--   0 mduval    (1000) mduval    (1000)        1 2023-05-24 11:37:55.000000 georideapilib-1.0.1/georideapilib.egg-info/dependency_links.txt
+-rw-r--r--   0 mduval    (1000) mduval    (1000)       31 2023-05-24 11:37:55.000000 georideapilib-1.0.1/georideapilib.egg-info/requires.txt
+-rw-r--r--   0 mduval    (1000) mduval    (1000)       14 2023-05-24 11:37:55.000000 georideapilib-1.0.1/georideapilib.egg-info/top_level.txt
+-rw-r--r--   0 mduval    (1000) mduval    (1000)       79 2023-05-24 11:37:55.384147 georideapilib-1.0.1/setup.cfg
+-rw-r--r--   0 mduval    (1000) mduval    (1000)     1217 2023-05-24 11:37:24.000000 georideapilib-1.0.1/setup.py
```

### Comparing `georideapilib-1.0.0/LICENSE` & `georideapilib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `georideapilib-1.0.0/README.md` & `georideapilib-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `georideapilib-1.0.0/georideapilib/api.py` & `georideapilib-1.0.1/georideapilib/api.py`

 * *Files identical despite different names*

### Comparing `georideapilib-1.0.0/georideapilib/exception.py` & `georideapilib-1.0.1/georideapilib/exception.py`

 * *Files identical despite different names*

### Comparing `georideapilib-1.0.0/georideapilib/objects/GeoRideAccount.py` & `georideapilib-1.0.1/georideapilib/objects/GeoRideAccount.py`

 * *Files identical despite different names*

### Comparing `georideapilib-1.0.0/georideapilib/objects/GeoRideSharedTrip.py` & `georideapilib-1.0.1/georideapilib/objects/GeoRideSharedTrip.py`

 * *Files identical despite different names*

### Comparing `georideapilib-1.0.0/georideapilib/objects/GeoRideSubscription.py` & `georideapilib-1.0.1/georideapilib/objects/GeoRideSubscription.py`

 * *Files identical despite different names*

### Comparing `georideapilib-1.0.0/georideapilib/objects/GeoRideSubscription_CardInfo.py` & `georideapilib-1.0.1/georideapilib/objects/GeoRideSubscription_CardInfo.py`

 * *Files identical despite different names*

### Comparing `georideapilib-1.0.0/georideapilib/objects/GeoRideTracker.py` & `georideapilib-1.0.1/georideapilib/objects/GeoRideTracker.py`

 * *Files identical despite different names*

### Comparing `georideapilib-1.0.0/georideapilib/objects/GeoRideTrackerBeacon.py` & `georideapilib-1.0.1/georideapilib/objects/GeoRideTrackerBeacon.py`

 * *Files identical despite different names*

### Comparing `georideapilib-1.0.0/georideapilib/objects/GeoRideTrackerPosition.py` & `georideapilib-1.0.1/georideapilib/objects/GeoRideTrackerPosition.py`

 * *Files identical despite different names*

### Comparing `georideapilib-1.0.0/georideapilib/objects/GeoRideTrackerTrip.py` & `georideapilib-1.0.1/georideapilib/objects/GeoRideTrackerTrip.py`

 * *Files identical despite different names*

### Comparing `georideapilib-1.0.0/georideapilib/objects/GeoRideUser.py` & `georideapilib-1.0.1/georideapilib/objects/GeoRideUser.py`

 * *Files identical despite different names*

### Comparing `georideapilib-1.0.0/georideapilib/socket.py` & `georideapilib-1.0.1/georideapilib/socket.py`

 * *Files identical despite different names*

### Comparing `georideapilib-1.0.0/georideapilib.egg-info/SOURCES.txt` & `georideapilib-1.0.1/georideapilib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `georideapilib-1.0.0/setup.py` & `georideapilib-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 # make pythonpack
 # python setup.py register sdist upload
 # and be sure to test it firstly using
 # "python setup.py register sdist upload -r pypitest"
 setup(
     name='georideapilib',
     packages=['georideapilib', 'georideapilib.objects'],  # this must be the same as the name above
-    version='1.0.0',
+    version='1.0.1',
     description='Lib to control GeoRide tracker devices with theire rest api',
     author='Matthieu DUVAL',
     author_email='georideapilib@duval-dev.fr',
     # use the URL to the github repo
     url='https://github.com/hacf/georide-api',
     download_url='https://codeload.github.com/hacf/georide-api/tar.gz/1.0.0',
     keywords=['rest', 'georide', 'api', 'grutier', 'GeoRide'],  # arbitrary keywords
     classifiers=[],
-    install_requires=["python-socketio[client]==5.8.0"],
+    install_requires=["python-socketio[client]==4.6.1"],
     tests_require=[
         'pytest>=3.7',
         'pytest-pep8',  
         'pytest-cov',
         'python-coveralls',
         'pylint',
         'coverage>=4.4'
```

