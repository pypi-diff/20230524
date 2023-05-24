# Comparing `tmp/trodesnetwork-0.0.8.tar.gz` & `tmp/trodesnetwork-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trodesnetwork-0.0.8.tar", last modified: Sun Oct 10 19:51:41 2021, max compression
+gzip compressed data, was "trodesnetwork-0.0.9.tar", last modified: Mon Oct 11 16:23:49 2021, max compression
```

## Comparing `trodesnetwork-0.0.8.tar` & `trodesnetwork-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 trevortknguyen  (1000) trevortknguyen  (1000)        0 2021-10-10 19:51:41.256087 trodesnetwork-0.0.8/
--rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)        0 2021-03-15 22:37:32.000000 trodesnetwork-0.0.8/LICENSE
--rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)      198 2021-10-10 19:51:41.256087 trodesnetwork-0.0.8/PKG-INFO
--rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)      415 2021-05-31 20:02:00.000000 trodesnetwork-0.0.8/README.md
--rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)       38 2021-10-10 19:51:41.256087 trodesnetwork-0.0.8/setup.cfg
--rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)      289 2021-10-10 19:43:46.000000 trodesnetwork-0.0.8/setup.py
-drwxrwxr-x   0 trevortknguyen  (1000) trevortknguyen  (1000)        0 2021-10-10 19:51:41.252087 trodesnetwork-0.0.8/trodesnetwork/
--rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)       70 2021-07-16 21:28:14.000000 trodesnetwork-0.0.8/trodesnetwork/__init__.py
--rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)     3988 2021-07-03 03:41:50.000000 trodesnetwork-0.0.8/trodesnetwork/socket.py
-drwxrwxr-x   0 trevortknguyen  (1000) trevortknguyen  (1000)        0 2021-10-10 19:51:41.256087 trodesnetwork-0.0.8/trodesnetwork/trodes/
--rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)      368 2021-10-02 13:33:43.000000 trodesnetwork-0.0.8/trodesnetwork/trodes/__init__.py
--rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)     1669 2021-10-02 13:33:43.000000 trodesnetwork-0.0.8/trodesnetwork/trodes/acquisition.py
--rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)     2474 2021-10-02 13:33:43.000000 trodesnetwork-0.0.8/trodesnetwork/trodes/analog.py
--rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)     2339 2021-10-02 13:33:43.000000 trodesnetwork-0.0.8/trodesnetwork/trodes/digital.py
--rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)     2330 2021-10-02 13:33:43.000000 trodesnetwork-0.0.8/trodesnetwork/trodes/events.py
--rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)     2337 2021-10-02 13:33:43.000000 trodesnetwork-0.0.8/trodesnetwork/trodes/hardware_channel_map.py
--rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)      557 2021-10-02 13:33:43.000000 trodesnetwork-0.0.8/trodesnetwork/trodes/info_client.py
--rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)     8783 2021-10-02 13:33:43.000000 trodesnetwork-0.0.8/trodesnetwork/trodes/trodes.py
--rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)      225 2021-10-02 13:33:43.000000 trodesnetwork-0.0.8/trodesnetwork/trodes/trodes_client.py
-drwxrwxr-x   0 trevortknguyen  (1000) trevortknguyen  (1000)        0 2021-10-10 19:51:41.252087 trodesnetwork-0.0.8/trodesnetwork.egg-info/
--rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)      198 2021-10-10 19:51:41.000000 trodesnetwork-0.0.8/trodesnetwork.egg-info/PKG-INFO
--rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)      573 2021-10-10 19:51:41.000000 trodesnetwork-0.0.8/trodesnetwork.egg-info/SOURCES.txt
--rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)        1 2021-10-10 19:51:41.000000 trodesnetwork-0.0.8/trodesnetwork.egg-info/dependency_links.txt
--rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)       30 2021-10-10 19:51:41.000000 trodesnetwork-0.0.8/trodesnetwork.egg-info/requires.txt
--rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)       14 2021-10-10 19:51:41.000000 trodesnetwork-0.0.8/trodesnetwork.egg-info/top_level.txt
+drwxrwxr-x   0 trevortknguyen  (1000) trevortknguyen  (1000)        0 2021-10-11 16:23:49.681004 trodesnetwork-0.0.9/
+-rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)        0 2021-03-15 22:37:32.000000 trodesnetwork-0.0.9/LICENSE
+-rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)      198 2021-10-11 16:23:49.681004 trodesnetwork-0.0.9/PKG-INFO
+-rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)      415 2021-05-31 20:02:00.000000 trodesnetwork-0.0.9/README.md
+-rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)       38 2021-10-11 16:23:49.681004 trodesnetwork-0.0.9/setup.cfg
+-rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)      289 2021-10-11 15:14:38.000000 trodesnetwork-0.0.9/setup.py
+drwxrwxr-x   0 trevortknguyen  (1000) trevortknguyen  (1000)        0 2021-10-11 16:23:49.681004 trodesnetwork-0.0.9/trodesnetwork/
+-rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)       70 2021-07-16 21:28:14.000000 trodesnetwork-0.0.9/trodesnetwork/__init__.py
+-rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)     3988 2021-07-03 03:41:50.000000 trodesnetwork-0.0.9/trodesnetwork/socket.py
+drwxrwxr-x   0 trevortknguyen  (1000) trevortknguyen  (1000)        0 2021-10-11 16:23:49.681004 trodesnetwork-0.0.9/trodesnetwork/trodes/
+-rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)      408 2021-10-11 15:14:38.000000 trodesnetwork-0.0.9/trodesnetwork/trodes/__init__.py
+-rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)     1669 2021-10-02 13:33:43.000000 trodesnetwork-0.0.9/trodesnetwork/trodes/acquisition.py
+-rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)     2474 2021-10-10 20:01:07.000000 trodesnetwork-0.0.9/trodesnetwork/trodes/analog.py
+-rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)     2339 2021-10-02 13:33:43.000000 trodesnetwork-0.0.9/trodesnetwork/trodes/digital.py
+-rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)     2330 2021-10-02 13:33:43.000000 trodesnetwork-0.0.9/trodesnetwork/trodes/events.py
+-rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)     1373 2021-10-11 15:14:38.000000 trodesnetwork-0.0.9/trodesnetwork/trodes/file.py
+-rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)     2337 2021-10-02 13:33:43.000000 trodesnetwork-0.0.9/trodesnetwork/trodes/hardware_channel_map.py
+-rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)      557 2021-10-02 13:33:43.000000 trodesnetwork-0.0.9/trodesnetwork/trodes/info_client.py
+-rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)     8783 2021-10-02 13:33:43.000000 trodesnetwork-0.0.9/trodesnetwork/trodes/trodes.py
+-rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)      225 2021-10-02 13:33:43.000000 trodesnetwork-0.0.9/trodesnetwork/trodes/trodes_client.py
+drwxrwxr-x   0 trevortknguyen  (1000) trevortknguyen  (1000)        0 2021-10-11 16:23:49.681004 trodesnetwork-0.0.9/trodesnetwork.egg-info/
+-rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)      198 2021-10-11 16:23:49.000000 trodesnetwork-0.0.9/trodesnetwork.egg-info/PKG-INFO
+-rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)      602 2021-10-11 16:23:49.000000 trodesnetwork-0.0.9/trodesnetwork.egg-info/SOURCES.txt
+-rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)        1 2021-10-11 16:23:49.000000 trodesnetwork-0.0.9/trodesnetwork.egg-info/dependency_links.txt
+-rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)       30 2021-10-11 16:23:49.000000 trodesnetwork-0.0.9/trodesnetwork.egg-info/requires.txt
+-rw-rw-r--   0 trevortknguyen  (1000) trevortknguyen  (1000)       14 2021-10-11 16:23:49.000000 trodesnetwork-0.0.9/trodesnetwork.egg-info/top_level.txt
```

### Comparing `trodesnetwork-0.0.8/trodesnetwork/socket.py` & `trodesnetwork-0.0.9/trodesnetwork/socket.py`

 * *Files identical despite different names*

### Comparing `trodesnetwork-0.0.8/trodesnetwork/trodes/acquisition.py` & `trodesnetwork-0.0.9/trodesnetwork/trodes/acquisition.py`

 * *Files identical despite different names*

### Comparing `trodesnetwork-0.0.8/trodesnetwork/trodes/analog.py` & `trodesnetwork-0.0.9/trodesnetwork/trodes/analog.py`

 * *Files identical despite different names*

### Comparing `trodesnetwork-0.0.8/trodesnetwork/trodes/digital.py` & `trodesnetwork-0.0.9/trodesnetwork/trodes/digital.py`

 * *Files identical despite different names*

### Comparing `trodesnetwork-0.0.8/trodesnetwork/trodes/events.py` & `trodesnetwork-0.0.9/trodesnetwork/trodes/events.py`

 * *Files identical despite different names*

### Comparing `trodesnetwork-0.0.8/trodesnetwork/trodes/hardware_channel_map.py` & `trodesnetwork-0.0.9/trodesnetwork/trodes/hardware_channel_map.py`

 * *Files identical despite different names*

### Comparing `trodesnetwork-0.0.8/trodesnetwork/trodes/info_client.py` & `trodesnetwork-0.0.9/trodesnetwork/trodes/info_client.py`

 * *Files identical despite different names*

### Comparing `trodesnetwork-0.0.8/trodesnetwork/trodes/trodes.py` & `trodesnetwork-0.0.9/trodesnetwork/trodes/trodes.py`

 * *Files identical despite different names*

### Comparing `trodesnetwork-0.0.8/trodesnetwork.egg-info/SOURCES.txt` & `trodesnetwork-0.0.9/trodesnetwork.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -9,11 +9,12 @@
 trodesnetwork.egg-info/requires.txt
 trodesnetwork.egg-info/top_level.txt
 trodesnetwork/trodes/__init__.py
 trodesnetwork/trodes/acquisition.py
 trodesnetwork/trodes/analog.py
 trodesnetwork/trodes/digital.py
 trodesnetwork/trodes/events.py
+trodesnetwork/trodes/file.py
 trodesnetwork/trodes/hardware_channel_map.py
 trodesnetwork/trodes/info_client.py
 trodesnetwork/trodes/trodes.py
 trodesnetwork/trodes/trodes_client.py
```

