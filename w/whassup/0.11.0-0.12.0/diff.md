# Comparing `tmp/whassup-0.11.0.tar.gz` & `tmp/whassup-0.12.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whassup-0.11.0.tar", last modified: Sun Jan 29 21:15:47 2023, max compression
+gzip compressed data, was "whassup-0.12.0.tar", last modified: Wed May 24 08:52:23 2023, max compression
```

## Comparing `whassup-0.11.0.tar` & `whassup-0.12.0.tar`

### file list

```diff
@@ -1,16 +1,25 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-01-29 21:15:47.462482 whassup-0.11.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1061 2023-01-29 19:37:36.000000 whassup-0.11.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      768 2023-01-29 21:15:47.462482 whassup-0.11.0/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-01-29 21:15:47.462482 whassup-0.11.0/scripts/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       54 2023-01-29 19:32:32.000000 whassup-0.11.0/scripts/whassup
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-01-29 21:15:47.462482 whassup-0.11.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      964 2023-01-29 19:42:58.000000 whassup-0.11.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-01-29 21:15:47.462482 whassup-0.11.0/whassup/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5092 2023-01-29 21:02:34.000000 whassup-0.11.0/whassup/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1136 2023-01-29 21:04:37.000000 whassup-0.11.0/whassup/exceptions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-01-29 21:15:47.462482 whassup-0.11.0/whassup.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      768 2023-01-29 21:15:47.000000 whassup-0.11.0/whassup.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2023-01-29 21:15:47.000000 whassup-0.11.0/whassup.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-01-29 21:15:47.000000 whassup-0.11.0/whassup.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-01-29 21:15:47.000000 whassup-0.11.0/whassup.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-01-29 21:15:47.000000 whassup-0.11.0/whassup.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 08:52:23.804626 whassup-0.12.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1061 2023-05-24 07:55:03.000000 whassup-0.12.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      768 2023-05-24 08:52:23.804626 whassup-0.12.0/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 08:52:23.804626 whassup-0.12.0/scripts/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       54 2023-05-24 07:55:03.000000 whassup-0.12.0/scripts/whassup
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-24 08:52:23.804626 whassup-0.12.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      964 2023-05-24 08:52:00.000000 whassup-0.12.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 08:52:23.804626 whassup-0.12.0/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1299 2023-05-24 07:55:03.000000 whassup-0.12.0/tests/test_check.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      511 2023-05-24 07:55:03.000000 whassup-0.12.0/tests/test_check_status.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      660 2023-05-24 07:55:03.000000 whassup-0.12.0/tests/test_check_timestamp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1513 2023-05-24 08:43:55.000000 whassup-0.12.0/tests/test_cli.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      686 2023-05-24 07:55:03.000000 whassup-0.12.0/tests/test_dictionary_from_response.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1595 2023-05-24 07:55:03.000000 whassup-0.12.0/tests/test_remote_data_from_dictionary.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4263 2023-05-24 07:55:03.000000 whassup-0.12.0/tests/test_response_from_url.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3085 2023-05-24 08:43:55.000000 whassup-0.12.0/tests/test_warning_tolerant_check.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 08:52:23.804626 whassup-0.12.0/whassup/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5145 2023-05-24 08:43:55.000000 whassup-0.12.0/whassup/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1170 2023-05-24 08:43:55.000000 whassup-0.12.0/whassup/exceptions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 08:52:23.804626 whassup-0.12.0/whassup.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      768 2023-05-24 08:52:23.000000 whassup-0.12.0/whassup.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      473 2023-05-24 08:52:23.000000 whassup-0.12.0/whassup.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-24 08:52:23.000000 whassup-0.12.0/whassup.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-05-24 08:52:23.000000 whassup-0.12.0/whassup.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-05-24 08:52:23.000000 whassup-0.12.0/whassup.egg-info/top_level.txt
```

### Comparing `whassup-0.11.0/LICENSE` & `whassup-0.12.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whassup-0.11.0/PKG-INFO` & `whassup-0.12.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: whassup
-Version: 0.11.0
+Version: 0.12.0
 Summary: Minimalist health-check for stayinalive
 Home-page: https://zebr0.io/projects/whassup
-Download-URL: https://github.com/zebr0/whassup
+Download-URL: https://gitlab.com/zebr0/whassup
 Author: Thomas JOUANNOT
 Author-email: mazerty@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `whassup-0.11.0/setup.py` & `whassup-0.12.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
 setuptools.setup(
     name="whassup",
-    version="0.11.0",
+    version="0.12.0",
     description="Minimalist health-check for stayinalive",
     long_description="TODO",
     long_description_content_type="text/markdown",
     author="Thomas JOUANNOT",
     author_email="mazerty@gmail.com",
     url="https://zebr0.io/projects/whassup",
-    download_url="https://github.com/zebr0/whassup",
+    download_url="https://gitlab.com/zebr0/whassup",
     packages=["whassup"],
     scripts=["scripts/whassup"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
```

### Comparing `whassup-0.11.0/whassup/__init__.py` & `whassup-0.12.0/whassup/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import threading
 import time
 from datetime import datetime, timedelta, timezone
 from typing import Optional, List
 
 import requests
 
-from .exceptions import CheckWarning, UrlWarning, ResponseWarning, TimestampWarning, StatusWarning, ExpectedModeWarning, DictionaryError, StatusError, WarningTimeoutError
+from .exceptions import CheckWarning, UrlWarning, ResponseWarning, TimestampWarning, StatusWarning, ExpectedModesWarning, DictionaryError, StatusError, WarningTimeoutError
 
 REQUEST_TIMEOUT_DEFAULT: float = 3.05  # see https://docs.python-requests.org/en/master/user/advanced/#timeouts
 STAYINALIVE_TIMEOUT_DEFAULT: float = 15
 WARNING_TIMEOUT_DEFAULT: float = 600  # 10 minutes
 DELAY_DEFAULT: float = 3
 
 
@@ -73,15 +73,15 @@
     _check_timestamp(remote_data.timestamp, stayinalive_timeout)
 
     return remote_data
 
 
 def warning_tolerant_check(url: str,
                            event: threading.Event = None,
-                           expected_mode: str = None,
+                           expected_modes: List[str] = None,
                            delay: float = DELAY_DEFAULT,
                            warning_timeout: float = WARNING_TIMEOUT_DEFAULT,
                            request_timeout: float = REQUEST_TIMEOUT_DEFAULT,
                            stayinalive_timeout: float = STAYINALIVE_TIMEOUT_DEFAULT,
                            ignore_tls: bool = False) -> RemoteData:
     if not event:
         event = threading.Event()
@@ -89,36 +89,36 @@
     timer = threading.Timer(warning_timeout, lambda: event.set())
     timer.start()
 
     try:
         while True:
             try:
                 remote_data = check(url, request_timeout, stayinalive_timeout, ignore_tls)
-                if not expected_mode or remote_data.mode == expected_mode:
+                if not expected_modes or remote_data.mode in expected_modes:
                     return remote_data
                 else:
-                    raise ExpectedModeWarning(expected_mode)
+                    raise ExpectedModesWarning(expected_modes)
             except CheckWarning as warning:
                 event.wait(delay)
                 if event.is_set():
                     raise WarningTimeoutError(warning)
     finally:
         timer.cancel()
 
 
 def main(args: Optional[List[str]] = None) -> None:
     argparser = argparse.ArgumentParser(description="")
     argparser.add_argument("url", help="", metavar="<url>")
-    argparser.add_argument("-m", "--expected-mode", help="", metavar="<mode>")
+    argparser.add_argument("-m", "--expected-mode", action="append", dest="expected_modes", help="", metavar="<mode>")
     argparser.add_argument("-d", "--delay", type=float, default=DELAY_DEFAULT, help="", metavar="<duration>")
     argparser.add_argument("-w", "--warning-timeout", type=float, default=WARNING_TIMEOUT_DEFAULT, help="", metavar="<duration>")
     argparser.add_argument("-r", "--request-timeout", type=float, default=REQUEST_TIMEOUT_DEFAULT, help="", metavar="<duration>")
     argparser.add_argument("-t", "--stayinalive-timeout", type=float, default=STAYINALIVE_TIMEOUT_DEFAULT, help="", metavar="<duration>")
     argparser.add_argument("-i", "--ignore-tls", action="store_true", help="")
     args = argparser.parse_args(args)
 
     # turning SIGINT and SIGTERM into an event
     event = threading.Event()
     for sig in [signal.SIGINT, signal.SIGTERM]:
         signal.signal(sig, lambda signum, frame: event.set())
 
-    print(warning_tolerant_check(args.url, event, args.expected_mode, args.delay, args.warning_timeout, args.request_timeout, args.stayinalive_timeout, args.ignore_tls).to_json())
+    print(warning_tolerant_check(args.url, event, args.expected_modes, args.delay, args.warning_timeout, args.request_timeout, args.stayinalive_timeout, args.ignore_tls).to_json())
```

### Comparing `whassup-0.11.0/whassup/exceptions.py` & `whassup-0.12.0/whassup/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import datetime
+from typing import List
 
 
 class CheckWarning(Exception):
     pass
 
 
 class UrlWarning(CheckWarning):
@@ -23,17 +24,17 @@
         self.now = now
 
 
 class StatusWarning(CheckWarning):
     pass
 
 
-class ExpectedModeWarning(CheckWarning):
-    def __init__(self, expected_mode: str):
-        self.expected_mode = expected_mode
+class ExpectedModesWarning(CheckWarning):
+    def __init__(self, expected_modes: List[str]):
+        self.expected_modes = expected_modes
 
 
 class CheckError(Exception):
     pass
 
 
 class DictionaryError(CheckError):
```

### Comparing `whassup-0.11.0/whassup.egg-info/PKG-INFO` & `whassup-0.12.0/whassup.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: whassup
-Version: 0.11.0
+Version: 0.12.0
 Summary: Minimalist health-check for stayinalive
 Home-page: https://zebr0.io/projects/whassup
-Download-URL: https://github.com/zebr0/whassup
+Download-URL: https://gitlab.com/zebr0/whassup
 Author: Thomas JOUANNOT
 Author-email: mazerty@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

