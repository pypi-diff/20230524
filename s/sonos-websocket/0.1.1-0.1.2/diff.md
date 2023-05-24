# Comparing `tmp/sonos-websocket-0.1.1.tar.gz` & `tmp/sonos-websocket-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonos-websocket-0.1.1.tar", last modified: Tue May  9 02:34:08 2023, max compression
+gzip compressed data, was "sonos-websocket-0.1.2.tar", last modified: Wed May 24 03:00:29 2023, max compression
```

## Comparing `sonos-websocket-0.1.1.tar` & `sonos-websocket-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:34:08.403478 sonos-websocket-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-09 02:34:08.403478 sonos-websocket-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-09 02:33:57.000000 sonos-websocket-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-09 02:33:57.000000 sonos-websocket-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 02:33:57.000000 sonos-websocket-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 02:34:08.403478 sonos-websocket-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:34:08.399478 sonos-websocket-0.1.1/sonos_websocket/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-09 02:33:57.000000 sonos-websocket-0.1.1/sonos_websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-09 02:33:57.000000 sonos-websocket-0.1.1/sonos_websocket/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-09 02:33:57.000000 sonos-websocket-0.1.1/sonos_websocket/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-09 02:33:57.000000 sonos-websocket-0.1.1/sonos_websocket/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-05-09 02:33:57.000000 sonos-websocket-0.1.1/sonos_websocket/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:34:08.403478 sonos-websocket-0.1.1/sonos_websocket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-09 02:34:08.000000 sonos-websocket-0.1.1/sonos_websocket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-09 02:34:08.000000 sonos-websocket-0.1.1/sonos_websocket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 02:34:08.000000 sonos-websocket-0.1.1/sonos_websocket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-09 02:34:08.000000 sonos-websocket-0.1.1/sonos_websocket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 02:34:08.000000 sonos-websocket-0.1.1/sonos_websocket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:00:29.667031 sonos-websocket-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-24 03:00:29.667031 sonos-websocket-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-24 03:00:17.000000 sonos-websocket-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-24 03:00:17.000000 sonos-websocket-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-24 03:00:17.000000 sonos-websocket-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 03:00:29.667031 sonos-websocket-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:00:29.667031 sonos-websocket-0.1.2/sonos_websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-24 03:00:17.000000 sonos-websocket-0.1.2/sonos_websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-24 03:00:17.000000 sonos-websocket-0.1.2/sonos_websocket/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-24 03:00:17.000000 sonos-websocket-0.1.2/sonos_websocket/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-24 03:00:17.000000 sonos-websocket-0.1.2/sonos_websocket/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-05-24 03:00:17.000000 sonos-websocket-0.1.2/sonos_websocket/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:00:29.667031 sonos-websocket-0.1.2/sonos_websocket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-24 03:00:29.000000 sonos-websocket-0.1.2/sonos_websocket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-24 03:00:29.000000 sonos-websocket-0.1.2/sonos_websocket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 03:00:29.000000 sonos-websocket-0.1.2/sonos_websocket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 03:00:29.000000 sonos-websocket-0.1.2/sonos_websocket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-24 03:00:29.000000 sonos-websocket-0.1.2/sonos_websocket.egg-info/top_level.txt
```

### Comparing `sonos-websocket-0.1.1/PKG-INFO` & `sonos-websocket-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonos-websocket
-Version: 0.1.1
+Version: 0.1.2
 Summary: An asynchronous Python library to communicate with Sonos devices over websockets.
 Author-email: Jason Lawrence <jjlawren@users.noreply.github.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/jjlawren/sonos-websocket
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sonos-websocket-0.1.1/README.md` & `sonos-websocket-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sonos-websocket-0.1.1/pyproject.toml` & `sonos-websocket-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sonos-websocket-0.1.1/sonos_websocket/__main__.py` & `sonos-websocket-0.1.2/sonos_websocket/__main__.py`

 * *Files identical despite different names*

### Comparing `sonos-websocket-0.1.1/sonos_websocket/websocket.py` & `sonos-websocket-0.1.2/sonos_websocket/websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,16 @@
             try:
                 async with asyncio_timeout(3):
                     await self.ws.send_json(payload)
                     msg = await self.ws.receive()
             except asyncio.TimeoutError:
                 _LOGGER.error("Command timed out")
             except ConnectionResetError:
+                # Websocket closing
+                self.ws = None
                 _LOGGER.debug("Websocket connection reset, will try again")
             else:
                 if msg.type in (WSMsgType.CLOSE, WSMsgType.CLOSED, WSMsgType.CLOSING):
                     _LOGGER.debug("Websocket closed, will try again")
                 elif msg.type != WSMsgType.TEXT:
                     _LOGGER.error("Received non-text message: %s", msg.type.name)
                 else:
```

### Comparing `sonos-websocket-0.1.1/sonos_websocket.egg-info/PKG-INFO` & `sonos-websocket-0.1.2/sonos_websocket.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonos-websocket
-Version: 0.1.1
+Version: 0.1.2
 Summary: An asynchronous Python library to communicate with Sonos devices over websockets.
 Author-email: Jason Lawrence <jjlawren@users.noreply.github.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/jjlawren/sonos-websocket
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

