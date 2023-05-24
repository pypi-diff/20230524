# Comparing `tmp/PrSpiders-0.5.0.tar.gz` & `tmp/PrSpiders-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrSpiders-0.5.0.tar", last modified: Tue May 23 07:08:50 2023, max compression
+gzip compressed data, was "PrSpiders-0.5.1.tar", last modified: Wed May 24 01:39:13 2023, max compression
```

## Comparing `PrSpiders-0.5.0.tar` & `PrSpiders-0.5.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 07:08:50.759925 PrSpiders-0.5.0/
--rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.5.0/LICENSE.txt
--rw-rw-rw-   0        0        0     5678 2023-05-23 07:08:50.744922 PrSpiders-0.5.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-23 07:08:49.734926 PrSpiders-0.5.0/PrSpider/
--rw-rw-rw-   0        0        0    12780 2023-05-23 06:27:19.000000 PrSpiders-0.5.0/PrSpider/PrSpiders.py
--rw-rw-rw-   0        0        0       98 2023-05-23 06:27:42.000000 PrSpiders-0.5.0/PrSpider/__init__.py
--rw-rw-rw-   0        0        0    11047 2023-05-23 06:28:34.000000 PrSpiders-0.5.0/PrSpider/pxpath.py
--rw-rw-rw-   0        0        0     3193 2023-05-23 07:08:35.000000 PrSpiders-0.5.0/PrSpider/pyconn.py
--rw-rw-rw-   0        0        0     4560 2023-05-23 06:28:17.000000 PrSpiders-0.5.0/PrSpider/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.0/PrSpider/useragent.py
-drwxrwxrwx   0        0        0        0 2023-05-23 07:08:50.091923 PrSpiders-0.5.0/PrSpiders.egg-info/
--rw-rw-rw-   0        0        0     5678 2023-05-23 07:08:48.000000 PrSpiders-0.5.0/PrSpiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      582 2023-05-23 07:08:48.000000 PrSpiders-0.5.0/PrSpiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 07:08:48.000000 PrSpiders-0.5.0/PrSpiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-05-23 07:08:48.000000 PrSpiders-0.5.0/PrSpiders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2023-05-23 07:08:48.000000 PrSpiders-0.5.0/PrSpiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-05-23 07:08:48.000000 PrSpiders-0.5.0/PrSpiders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5166 2023-04-23 08:22:29.000000 PrSpiders-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 07:08:50.108923 PrSpiders-0.5.0/pkg/
--rw-rw-rw-   0        0        0       23 2023-04-23 03:23:07.000000 PrSpiders-0.5.0/pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 07:08:50.442923 PrSpiders-0.5.0/pkg/prspider/
--rw-rw-rw-   0        0        0     1212 2023-04-20 09:13:43.000000 PrSpiders-0.5.0/pkg/prspider/PrSpider_CMD.py
--rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.5.0/pkg/prspider/PrSpider_run.py
--rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.5.0/pkg/prspider/__init__.py
--rw-rw-rw-   0        0        0      833 2023-04-23 03:22:54.000000 PrSpiders-0.5.0/pkg/prspider/start.py
-drwxrwxrwx   0        0        0        0 2023-05-23 07:08:50.705929 PrSpiders-0.5.0/requestXpath/
--rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.5.0/requestXpath/__init__.py
--rw-rw-rw-   0        0        0     8642 2023-04-18 08:44:05.000000 PrSpiders-0.5.0/requestXpath/pxpath.py
--rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.5.0/requestXpath/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.0/requestXpath/useragent.py
--rw-rw-rw-   0        0        0       42 2023-05-23 07:08:50.761920 PrSpiders-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1032 2023-05-23 07:08:42.000000 PrSpiders-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 01:39:13.194158 PrSpiders-0.5.1/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.5.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     5678 2023-05-24 01:39:13.176156 PrSpiders-0.5.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-24 01:39:12.954159 PrSpiders-0.5.1/PrSpider/
+-rw-rw-rw-   0        0        0    12780 2023-05-24 01:37:19.000000 PrSpiders-0.5.1/PrSpider/PrSpiders.py
+-rw-rw-rw-   0        0        0       98 2023-05-23 06:27:42.000000 PrSpiders-0.5.1/PrSpider/__init__.py
+-rw-rw-rw-   0        0        0    11257 2023-05-24 01:36:58.000000 PrSpiders-0.5.1/PrSpider/pxpath.py
+-rw-rw-rw-   0        0        0     3193 2023-05-23 07:08:35.000000 PrSpiders-0.5.1/PrSpider/pyconn.py
+-rw-rw-rw-   0        0        0     4560 2023-05-23 06:28:17.000000 PrSpiders-0.5.1/PrSpider/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.1/PrSpider/useragent.py
+drwxrwxrwx   0        0        0        0 2023-05-24 01:39:13.042163 PrSpiders-0.5.1/PrSpiders.egg-info/
+-rw-rw-rw-   0        0        0     5678 2023-05-24 01:39:12.000000 PrSpiders-0.5.1/PrSpiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      582 2023-05-24 01:39:12.000000 PrSpiders-0.5.1/PrSpiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 01:39:12.000000 PrSpiders-0.5.1/PrSpiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-05-24 01:39:12.000000 PrSpiders-0.5.1/PrSpiders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2023-05-24 01:39:12.000000 PrSpiders-0.5.1/PrSpiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-05-24 01:39:12.000000 PrSpiders-0.5.1/PrSpiders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5166 2023-04-23 08:22:29.000000 PrSpiders-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 01:39:13.057159 PrSpiders-0.5.1/pkg/
+-rw-rw-rw-   0        0        0       23 2023-05-24 01:39:05.000000 PrSpiders-0.5.1/pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 01:39:13.110159 PrSpiders-0.5.1/pkg/prspider/
+-rw-rw-rw-   0        0        0     1212 2023-04-20 09:13:43.000000 PrSpiders-0.5.1/pkg/prspider/PrSpider_CMD.py
+-rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.5.1/pkg/prspider/PrSpider_run.py
+-rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.5.1/pkg/prspider/__init__.py
+-rw-rw-rw-   0        0        0      833 2023-04-23 03:22:54.000000 PrSpiders-0.5.1/pkg/prspider/start.py
+drwxrwxrwx   0        0        0        0 2023-05-24 01:39:13.162156 PrSpiders-0.5.1/requestXpath/
+-rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.5.1/requestXpath/__init__.py
+-rw-rw-rw-   0        0        0     8642 2023-04-18 08:44:05.000000 PrSpiders-0.5.1/requestXpath/pxpath.py
+-rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.5.1/requestXpath/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.1/requestXpath/useragent.py
+-rw-rw-rw-   0        0        0       42 2023-05-24 01:39:13.197159 PrSpiders-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1032 2023-05-24 01:38:46.000000 PrSpiders-0.5.1/setup.py
```

### Comparing `PrSpiders-0.5.0/LICENSE.txt` & `PrSpiders-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.0/PKG-INFO` & `PrSpiders-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.5.0
+Version: 0.5.1
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.5.0/PrSpider/PrSpiders.py` & `PrSpiders-0.5.1/PrSpider/PrSpiders.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.0/PrSpider/pxpath.py` & `PrSpiders-0.5.1/PrSpider/pxpath.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from urllib.parse import urljoin
 import re, time, copy
 from lxml import etree
 from datetime import timedelta, datetime
 import unicodedata
 from PrSpider.PrSpiders import loguer
 
+
 class Xpath(object):
     def __init__(self, response, encoding="utf-8"):
         if isinstance(response, str):
             self.res = etree.HTML(response)
         else:
             response.encoding = encoding
             self.res = etree.HTML(response.text)
@@ -188,15 +189,15 @@
         if data is None or len(data) == 0:
             return None
         data = self.parse_txt(data)
         try:
             result = self.parse_time(data)
             return result
         except Exception as e:
-            loguer.error(e)
+            loguer.error('@Date时间处理错误 | [%s] | %s' % (data, e))
             return None
 
     @classmethod
     def repl_date(self, l: list):
         if len(l) > 1:
             raise ValueError("匹配时间数量超过一个 <str>%s</str>" % l)
         res = "".join(l).strip()
@@ -230,26 +231,32 @@
             days = re.findall("(\d+)天前", s_time)[0]
             result_time = (datetime.now() - timedelta(days=int(days))).strftime(
                 "%Y-%m-%d %H:%M:%S"
             )
 
         # 昨天 18:03
         elif "昨天" in s_time:
-            last_time = re.findall(r".*?(\d{1,2}:\d{1,2})", s_time)[0]
+            try:
+                last_time = re.findall(r".*?(\d{1,2}:\d{1,2})", s_time)[0]
+            except:
+                last_time = '00:00'
             days_ago = datetime.now() - timedelta(days=int(1))
             y_m_d = (
                     str(days_ago.year) + "-" + str(days_ago.month) + "-" + str(days_ago.day)
             )
             _time = y_m_d + " " + last_time
             result_time = time.strftime(
                 "%Y-%m-%d %H:%M:%S", time.strptime(_time, "%Y-%m-%d %H:%M")
             )
 
         elif "前天" in s_time:
-            last_time = re.findall(r".*?(\d{1,2}:\d{1,2})", s_time)[0]
+            try:
+                last_time = re.findall(r".*?(\d{1,2}:\d{1,2})", s_time)[0]
+            except:
+                last_time = '00:00'
             days_ago = datetime.now() - timedelta(days=int(2))
             y_m_d = (
                     str(days_ago.year) + "-" + str(days_ago.month) + "-" + str(days_ago.day)
             )
             _time = y_m_d + " " + last_time
             result_time = time.strftime(
                 "%Y-%m-%d %H:%M:%S", time.strptime(_time, "%Y-%m-%d %H:%M")
```

### Comparing `PrSpiders-0.5.0/PrSpider/pyconn.py` & `PrSpiders-0.5.1/PrSpider/pyconn.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.0/PrSpider/requestXpath.py` & `PrSpiders-0.5.1/PrSpider/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.0/PrSpider/useragent.py` & `PrSpiders-0.5.1/PrSpider/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.0/PrSpiders.egg-info/PKG-INFO` & `PrSpiders-0.5.1/PrSpiders.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.5.0
+Version: 0.5.1
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.5.0/PrSpiders.egg-info/SOURCES.txt` & `PrSpiders-0.5.1/PrSpiders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.0/README.md` & `PrSpiders-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.0/pkg/prspider/PrSpider_CMD.py` & `PrSpiders-0.5.1/pkg/prspider/PrSpider_CMD.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.0/pkg/prspider/start.py` & `PrSpiders-0.5.1/pkg/prspider/start.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.0/requestXpath/__init__.py` & `PrSpiders-0.5.1/requestXpath/__init__.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.0/requestXpath/pxpath.py` & `PrSpiders-0.5.1/requestXpath/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.0/requestXpath/requestXpath.py` & `PrSpiders-0.5.1/requestXpath/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.0/requestXpath/useragent.py` & `PrSpiders-0.5.1/requestXpath/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.0/setup.py` & `PrSpiders-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!python
 # -*- coding:utf-8 -*-
 from __future__ import print_function
 from setuptools import setup, find_packages
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PrSpiders",
     version=__version__,
```

