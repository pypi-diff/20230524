# Comparing `tmp/PrSpiders-0.5.1.tar.gz` & `tmp/PrSpiders-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrSpiders-0.5.1.tar", last modified: Wed May 24 01:39:13 2023, max compression
+gzip compressed data, was "PrSpiders-0.5.2.tar", last modified: Wed May 24 05:19:31 2023, max compression
```

## Comparing `PrSpiders-0.5.1.tar` & `PrSpiders-0.5.2.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 01:39:13.194158 PrSpiders-0.5.1/
--rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.5.1/LICENSE.txt
--rw-rw-rw-   0        0        0     5678 2023-05-24 01:39:13.176156 PrSpiders-0.5.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-24 01:39:12.954159 PrSpiders-0.5.1/PrSpider/
--rw-rw-rw-   0        0        0    12780 2023-05-24 01:37:19.000000 PrSpiders-0.5.1/PrSpider/PrSpiders.py
--rw-rw-rw-   0        0        0       98 2023-05-23 06:27:42.000000 PrSpiders-0.5.1/PrSpider/__init__.py
--rw-rw-rw-   0        0        0    11257 2023-05-24 01:36:58.000000 PrSpiders-0.5.1/PrSpider/pxpath.py
--rw-rw-rw-   0        0        0     3193 2023-05-23 07:08:35.000000 PrSpiders-0.5.1/PrSpider/pyconn.py
--rw-rw-rw-   0        0        0     4560 2023-05-23 06:28:17.000000 PrSpiders-0.5.1/PrSpider/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.1/PrSpider/useragent.py
-drwxrwxrwx   0        0        0        0 2023-05-24 01:39:13.042163 PrSpiders-0.5.1/PrSpiders.egg-info/
--rw-rw-rw-   0        0        0     5678 2023-05-24 01:39:12.000000 PrSpiders-0.5.1/PrSpiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      582 2023-05-24 01:39:12.000000 PrSpiders-0.5.1/PrSpiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 01:39:12.000000 PrSpiders-0.5.1/PrSpiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-05-24 01:39:12.000000 PrSpiders-0.5.1/PrSpiders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2023-05-24 01:39:12.000000 PrSpiders-0.5.1/PrSpiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-05-24 01:39:12.000000 PrSpiders-0.5.1/PrSpiders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5166 2023-04-23 08:22:29.000000 PrSpiders-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 01:39:13.057159 PrSpiders-0.5.1/pkg/
--rw-rw-rw-   0        0        0       23 2023-05-24 01:39:05.000000 PrSpiders-0.5.1/pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 01:39:13.110159 PrSpiders-0.5.1/pkg/prspider/
--rw-rw-rw-   0        0        0     1212 2023-04-20 09:13:43.000000 PrSpiders-0.5.1/pkg/prspider/PrSpider_CMD.py
--rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.5.1/pkg/prspider/PrSpider_run.py
--rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.5.1/pkg/prspider/__init__.py
--rw-rw-rw-   0        0        0      833 2023-04-23 03:22:54.000000 PrSpiders-0.5.1/pkg/prspider/start.py
-drwxrwxrwx   0        0        0        0 2023-05-24 01:39:13.162156 PrSpiders-0.5.1/requestXpath/
--rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.5.1/requestXpath/__init__.py
--rw-rw-rw-   0        0        0     8642 2023-04-18 08:44:05.000000 PrSpiders-0.5.1/requestXpath/pxpath.py
--rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.5.1/requestXpath/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.1/requestXpath/useragent.py
--rw-rw-rw-   0        0        0       42 2023-05-24 01:39:13.197159 PrSpiders-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1032 2023-05-24 01:38:46.000000 PrSpiders-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:19:31.496300 PrSpiders-0.5.2/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.5.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     5678 2023-05-24 05:19:31.317298 PrSpiders-0.5.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-24 05:19:30.465300 PrSpiders-0.5.2/PrSpider/
+-rw-rw-rw-   0        0        0    10667 2023-05-24 05:19:03.000000 PrSpiders-0.5.2/PrSpider/PrSpiders.py
+-rw-rw-rw-   0        0        0       98 2023-05-23 06:27:42.000000 PrSpiders-0.5.2/PrSpider/__init__.py
+-rw-rw-rw-   0        0        0     2392 2023-05-24 05:18:39.000000 PrSpiders-0.5.2/PrSpider/log.py
+-rw-rw-rw-   0        0        0    11257 2023-05-24 01:36:58.000000 PrSpiders-0.5.2/PrSpider/pxpath.py
+-rw-rw-rw-   0        0        0     3193 2023-05-23 07:08:35.000000 PrSpiders-0.5.2/PrSpider/pyconn.py
+-rw-rw-rw-   0        0        0     4560 2023-05-23 06:28:17.000000 PrSpiders-0.5.2/PrSpider/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.2/PrSpider/useragent.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:19:30.523298 PrSpiders-0.5.2/PrSpiders.egg-info/
+-rw-rw-rw-   0        0        0     5678 2023-05-24 05:19:29.000000 PrSpiders-0.5.2/PrSpiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      598 2023-05-24 05:19:30.000000 PrSpiders-0.5.2/PrSpiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 05:19:29.000000 PrSpiders-0.5.2/PrSpiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-05-24 05:19:29.000000 PrSpiders-0.5.2/PrSpiders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2023-05-24 05:19:29.000000 PrSpiders-0.5.2/PrSpiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-05-24 05:19:29.000000 PrSpiders-0.5.2/PrSpiders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5166 2023-04-23 08:22:29.000000 PrSpiders-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 05:19:30.536301 PrSpiders-0.5.2/pkg/
+-rw-rw-rw-   0        0        0       23 2023-05-24 01:39:05.000000 PrSpiders-0.5.2/pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:19:30.714298 PrSpiders-0.5.2/pkg/prspider/
+-rw-rw-rw-   0        0        0     1212 2023-04-20 09:13:43.000000 PrSpiders-0.5.2/pkg/prspider/PrSpider_CMD.py
+-rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.5.2/pkg/prspider/PrSpider_run.py
+-rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.5.2/pkg/prspider/__init__.py
+-rw-rw-rw-   0        0        0      833 2023-04-23 03:22:54.000000 PrSpiders-0.5.2/pkg/prspider/start.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:19:30.950298 PrSpiders-0.5.2/requestXpath/
+-rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.5.2/requestXpath/__init__.py
+-rw-rw-rw-   0        0        0     8642 2023-04-18 08:44:05.000000 PrSpiders-0.5.2/requestXpath/pxpath.py
+-rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.5.2/requestXpath/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.2/requestXpath/useragent.py
+-rw-rw-rw-   0        0        0       42 2023-05-24 05:19:31.496300 PrSpiders-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1032 2023-05-24 05:19:27.000000 PrSpiders-0.5.2/setup.py
```

### Comparing `PrSpiders-0.5.1/LICENSE.txt` & `PrSpiders-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.1/PKG-INFO` & `PrSpiders-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.5.1
+Version: 0.5.2
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.5.1/PrSpider/PrSpiders.py` & `PrSpiders-0.5.2/PrSpider/PrSpiders.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import os
-import re
-import sys
 import time
 from typing import Optional
 from loguru import logger as loguer
 from .requestXpath import prequest
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from .pyconn import PrMysql
-
-
+from .log import *
 
 
 class settions(object):
     workers: Optional[int] = 10000
     request_num: Optional[int] = 0
     retry_num: Optional[int] = 0
     success_num: Optional[int] = 0
@@ -22,34 +19,37 @@
     executor: Optional[object] = None
     retry: Optional[bool] = True
     pid: Optional[int] = os.getppid()
     start_time: Optional[int] = time.time()
     download_delay: Optional[int] = 0
     download_num: Optional[int] = 5
     logger: Optional[bool or str] = False
-    log_level: Optional[str] = "info"
+    log_level: Optional[str] = 'info'
     log_stdout: Optional[bool] = False
     futures: Optional[list] = set()
+    init: Optional[int] = 0
 
 
 class PrSpiders(settions):
     def __init__(self, **kwargs) -> None:
+        settions.init += 1
+        if settions.init <= 1:
+            Log(self.log_stdout, self.log_level, self.logger).loggering()
         settions.request_num = self.request_num
         settions.success_num = self.success_num
         settions.false_num = self.false_num
         settions.retry = self.retry
         settions.futures = self.futures
         settions.workers = self.workers
         settions.download_delay = self.download_delay
         settions.executor = ThreadPoolExecutor(settions.workers)
         settions.download_num = self.download_num
         settions.logger = self.logger
         settions.log_stdout = self.log_stdout
         settions.log_level = self.log_level
-        self.loguer = self.loggering(self.logger, self.log_level)
         loguer.warning(
             "\033[31m~~~ @PrSpider Start  @Workers %s  @Retry %s  @Pid %s @Download_Delay %s @Download_Num %s @LOG_LEVEL %s ~~~\033[0m"
             % (
                 self.workers,
                 self.retry,
                 self.pid,
                 self.download_delay,
@@ -237,64 +237,14 @@
         )
 
     def process_timestamp(self, t):
         timeArray = time.localtime(int(t))
         formatTime = time.strftime("%Y-%m-%d %H:%M:%S", timeArray)
         return formatTime
 
-    def loggering(self, file_log, level="info"):
-        """
-        打日志
-        :param file_log: 日志文件名，类型string；
-        """
-        # 创建一个loggger，并设置日志级别
-        level_dict = {
-            "warn": 'WARNING',
-            "info": 'INFO',
-            "debug": 'DEBUG',
-            "error": 'ERROR',
-            "critical": 'CRITICAL',
-        }
-        level_stdout = {
-            "critical": ['Print', 'CRITICAL'],
-            "error": ['Print', 'ERROR', 'CRITICAL', ],
-            "warn": ['Print', 'WARNING', 'ERROR', 'CRITICAL'],
-            "info": ['Print', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'],
-            "debug": ['Print', 'DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'],
-        }
-        levels = level_dict.get(level.lower())
-        slevel = level_stdout.get(level.lower())
-        loguer.level("TRACE", color="<blue>")
-        loguer.level("DEBUG", color="<green>")
-        loguer.level("INFO", color="<cyan>")
-        loguer.level("SUCCESS", color="<light-green>")
-        loguer.level("WARNING", color="<yellow>")
-        loguer.level("ERROR", color="<red>")
-        loguer.level("CRITICAL", color="<red>")
-        stdout_handler = {
-            "sink": sys.stdout,
-            "filter": lambda record: record["level"].name in slevel,
-            "format": "<light-green><b>{time:YYYY-MM-DD HH:mm:ss.SSS}</b></light-green> | <b><level>{level: ^8}</level></b> | <b>{message}</b>"
-        }
-        loguer.configure(handlers=[stdout_handler])
-        if self.log_stdout:
-            loguer.level("Print", no=60, color="<green>")
-            sys.stdout = InterceptHandler()
-        if file_log:
-            file_log = os.path.basename(__file__) if file_log is True else file_log
-            file_log = (
-                re.sub("\..*", ".log", file_log)
-                if "." in file_log
-                else file_log + ".log"
-            )
-            filename = f"./{file_log}"
-            loguer.add(filename, level=levels)
-
-        return loguer
-
     @classmethod
     def PrMysql(self, **kwargs):
         return PrMysql(loguer=loguer, **kwargs)
 
     def __del__(self):
         end_time = time.time()
         spend_time = end_time - self.start_time
@@ -326,16 +276,8 @@
             self.retry_num,
             self.process_timestamp(self.start_time),
             self.process_timestamp(end_time),
             spend_time,
             average_time,
         )
         loguer.info(m)
-
-
-class InterceptHandler():
-    def write(self, message):
-        if message.strip():
-            loguer.log("Print", message.strip())
-
-    def flush(self):
-        pass
+        self.executor.shutdown(wait=True)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `PrSpiders-0.5.1/PrSpider/pxpath.py` & `PrSpiders-0.5.2/PrSpider/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.1/PrSpider/pyconn.py` & `PrSpiders-0.5.2/PrSpider/pyconn.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.1/PrSpider/requestXpath.py` & `PrSpiders-0.5.2/PrSpider/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.1/PrSpider/useragent.py` & `PrSpiders-0.5.2/PrSpider/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.1/PrSpiders.egg-info/PKG-INFO` & `PrSpiders-0.5.2/PrSpiders.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.5.1
+Version: 0.5.2
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.5.1/PrSpiders.egg-info/SOURCES.txt` & `PrSpiders-0.5.2/PrSpiders.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE.txt
 README.md
 setup.py
 PrSpider/PrSpiders.py
 PrSpider/__init__.py
+PrSpider/log.py
 PrSpider/pxpath.py
 PrSpider/pyconn.py
 PrSpider/requestXpath.py
 PrSpider/useragent.py
 PrSpiders.egg-info/PKG-INFO
 PrSpiders.egg-info/SOURCES.txt
 PrSpiders.egg-info/dependency_links.txt
```

### Comparing `PrSpiders-0.5.1/README.md` & `PrSpiders-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.1/pkg/prspider/PrSpider_CMD.py` & `PrSpiders-0.5.2/pkg/prspider/PrSpider_CMD.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.1/pkg/prspider/start.py` & `PrSpiders-0.5.2/pkg/prspider/start.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.1/requestXpath/__init__.py` & `PrSpiders-0.5.2/requestXpath/__init__.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.1/requestXpath/pxpath.py` & `PrSpiders-0.5.2/requestXpath/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.1/requestXpath/requestXpath.py` & `PrSpiders-0.5.2/requestXpath/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.1/requestXpath/useragent.py` & `PrSpiders-0.5.2/requestXpath/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.1/setup.py` & `PrSpiders-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!python
 # -*- coding:utf-8 -*-
 from __future__ import print_function
 from setuptools import setup, find_packages
 
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PrSpiders",
     version=__version__,
```

