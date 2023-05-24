# Comparing `tmp/PrSpiders-0.4.9.tar.gz` & `tmp/PrSpiders-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrSpiders-0.4.9.tar", last modified: Tue May 23 06:30:14 2023, max compression
+gzip compressed data, was "PrSpiders-0.5.0.tar", last modified: Tue May 23 07:08:50 2023, max compression
```

## Comparing `PrSpiders-0.4.9.tar` & `PrSpiders-0.5.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 06:30:14.477264 PrSpiders-0.4.9/
--rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.4.9/LICENSE.txt
--rw-rw-rw-   0        0        0     5678 2023-05-23 06:30:14.451264 PrSpiders-0.4.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-23 06:30:14.232270 PrSpiders-0.4.9/PrSpider/
--rw-rw-rw-   0        0        0    12780 2023-05-23 06:27:19.000000 PrSpiders-0.4.9/PrSpider/PrSpiders.py
--rw-rw-rw-   0        0        0       98 2023-05-23 06:27:42.000000 PrSpiders-0.4.9/PrSpider/__init__.py
--rw-rw-rw-   0        0        0    11047 2023-05-23 06:28:34.000000 PrSpiders-0.4.9/PrSpider/pxpath.py
--rw-rw-rw-   0        0        0     2675 2023-05-23 06:26:59.000000 PrSpiders-0.4.9/PrSpider/pyconn.py
--rw-rw-rw-   0        0        0     4560 2023-05-23 06:28:17.000000 PrSpiders-0.4.9/PrSpider/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.4.9/PrSpider/useragent.py
-drwxrwxrwx   0        0        0        0 2023-05-23 06:30:14.334265 PrSpiders-0.4.9/PrSpiders.egg-info/
--rw-rw-rw-   0        0        0     5678 2023-05-23 06:30:13.000000 PrSpiders-0.4.9/PrSpiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      582 2023-05-23 06:30:13.000000 PrSpiders-0.4.9/PrSpiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 06:30:13.000000 PrSpiders-0.4.9/PrSpiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-05-23 06:30:13.000000 PrSpiders-0.4.9/PrSpiders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2023-05-23 06:30:13.000000 PrSpiders-0.4.9/PrSpiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-05-23 06:30:13.000000 PrSpiders-0.4.9/PrSpiders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5166 2023-04-23 08:22:29.000000 PrSpiders-0.4.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 06:30:14.348269 PrSpiders-0.4.9/pkg/
--rw-rw-rw-   0        0        0       23 2023-04-23 03:23:07.000000 PrSpiders-0.4.9/pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 06:30:14.393265 PrSpiders-0.4.9/pkg/prspider/
--rw-rw-rw-   0        0        0     1212 2023-04-20 09:13:43.000000 PrSpiders-0.4.9/pkg/prspider/PrSpider_CMD.py
--rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.4.9/pkg/prspider/PrSpider_run.py
--rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.4.9/pkg/prspider/__init__.py
--rw-rw-rw-   0        0        0      833 2023-04-23 03:22:54.000000 PrSpiders-0.4.9/pkg/prspider/start.py
-drwxrwxrwx   0        0        0        0 2023-05-23 06:30:14.438271 PrSpiders-0.4.9/requestXpath/
--rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.4.9/requestXpath/__init__.py
--rw-rw-rw-   0        0        0     8642 2023-04-18 08:44:05.000000 PrSpiders-0.4.9/requestXpath/pxpath.py
--rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.4.9/requestXpath/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.4.9/requestXpath/useragent.py
--rw-rw-rw-   0        0        0       42 2023-05-23 06:30:14.483267 PrSpiders-0.4.9/setup.cfg
--rw-rw-rw-   0        0        0     1032 2023-05-23 06:28:54.000000 PrSpiders-0.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:08:50.759925 PrSpiders-0.5.0/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.5.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     5678 2023-05-23 07:08:50.744922 PrSpiders-0.5.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-23 07:08:49.734926 PrSpiders-0.5.0/PrSpider/
+-rw-rw-rw-   0        0        0    12780 2023-05-23 06:27:19.000000 PrSpiders-0.5.0/PrSpider/PrSpiders.py
+-rw-rw-rw-   0        0        0       98 2023-05-23 06:27:42.000000 PrSpiders-0.5.0/PrSpider/__init__.py
+-rw-rw-rw-   0        0        0    11047 2023-05-23 06:28:34.000000 PrSpiders-0.5.0/PrSpider/pxpath.py
+-rw-rw-rw-   0        0        0     3193 2023-05-23 07:08:35.000000 PrSpiders-0.5.0/PrSpider/pyconn.py
+-rw-rw-rw-   0        0        0     4560 2023-05-23 06:28:17.000000 PrSpiders-0.5.0/PrSpider/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.0/PrSpider/useragent.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:08:50.091923 PrSpiders-0.5.0/PrSpiders.egg-info/
+-rw-rw-rw-   0        0        0     5678 2023-05-23 07:08:48.000000 PrSpiders-0.5.0/PrSpiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      582 2023-05-23 07:08:48.000000 PrSpiders-0.5.0/PrSpiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 07:08:48.000000 PrSpiders-0.5.0/PrSpiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-05-23 07:08:48.000000 PrSpiders-0.5.0/PrSpiders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2023-05-23 07:08:48.000000 PrSpiders-0.5.0/PrSpiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-05-23 07:08:48.000000 PrSpiders-0.5.0/PrSpiders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5166 2023-04-23 08:22:29.000000 PrSpiders-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 07:08:50.108923 PrSpiders-0.5.0/pkg/
+-rw-rw-rw-   0        0        0       23 2023-04-23 03:23:07.000000 PrSpiders-0.5.0/pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:08:50.442923 PrSpiders-0.5.0/pkg/prspider/
+-rw-rw-rw-   0        0        0     1212 2023-04-20 09:13:43.000000 PrSpiders-0.5.0/pkg/prspider/PrSpider_CMD.py
+-rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.5.0/pkg/prspider/PrSpider_run.py
+-rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.5.0/pkg/prspider/__init__.py
+-rw-rw-rw-   0        0        0      833 2023-04-23 03:22:54.000000 PrSpiders-0.5.0/pkg/prspider/start.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:08:50.705929 PrSpiders-0.5.0/requestXpath/
+-rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.5.0/requestXpath/__init__.py
+-rw-rw-rw-   0        0        0     8642 2023-04-18 08:44:05.000000 PrSpiders-0.5.0/requestXpath/pxpath.py
+-rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.5.0/requestXpath/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.0/requestXpath/useragent.py
+-rw-rw-rw-   0        0        0       42 2023-05-23 07:08:50.761920 PrSpiders-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1032 2023-05-23 07:08:42.000000 PrSpiders-0.5.0/setup.py
```

### Comparing `PrSpiders-0.4.9/LICENSE.txt` & `PrSpiders-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.9/PKG-INFO` & `PrSpiders-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.4.9
+Version: 0.5.0
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.4.9/PrSpider/PrSpiders.py` & `PrSpiders-0.5.0/PrSpider/PrSpiders.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.9/PrSpider/pxpath.py` & `PrSpiders-0.5.0/PrSpider/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.9/PrSpider/pyconn.py` & `PrSpiders-0.5.0/PrSpider/pyconn.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from PrSpiders import loguer
+import pymysql
+from .PrSpiders import loguer
+
 
 def ErrorTip(func):
     def wrapper(*args, **kwargs):
         try:
             return func(*args, **kwargs)
         except Exception as e:
             loguer.error(e)
@@ -15,59 +17,75 @@
     数据存储
     """
 
     def __init__(
             self, host='localhost', port=3306, user=None,
             password=None, db=None, charset=None, tb=None, tip=False, loguer=loguer
             , **kwargs):
-        import pymysql
         """
         创建连接
         """
+        self.host = host
+        self.port = port
+        self.user = user
+        self.password = password
+        self.db = db
+        self.charset = charset
+        self.tip = tip
+        self.kwargs = kwargs
         self.pyconn = pymysql.connect(host=host, port=port, user=user, password=password,
                                       database=db, charset=charset, **kwargs)
         self.tip = tip
         self.loguer = loguer
         self.table = tb
         self.login('[%s]数据库成功连接' % db)
 
     @property
     @ErrorTip
+    def conn(self):
+        pyconn = pymysql.connect(host=self.host, port=self.port, user=self.user, password=self.password,
+                                 database=self.db, charset=self.charset, **self.kwargs)
+        return pyconn
+
+    @property
+    @ErrorTip
     def cursor(self):
-        import copy
-        cursor = copy.copy(self.pyconn.cursor())
+        pyconn = self.conn
+        cursor = pyconn.cursor()
         return cursor
 
     @ErrorTip
     def insert(self, sql):
-        self.cursor.execute(sql)
-        insert_id = self.pyconn.insert_id()
+        pyconn = self.conn
+        cursor = pyconn.cursor()
+        cursor.execute(sql)
+        insert_id = pyconn.insert_id()
         self.login('数据成功插入: %s' % insert_id)
-        self.pyconn.commit()
+        pyconn.commit()
         return insert_id
 
     @ErrorTip
     def execute(self, sql):
         return self.cursor.execute(sql)
 
     @ErrorTip
     def fetchone(self, sql):
-        cursor = self.pyconn.cursor()
+        cursor = self.conn.cursor()
         cursor.execute(sql)
         return cursor.fetchone()
 
     @ErrorTip
     def fetchall(self, sql):
-        cursor = self.pyconn.cursor()
+        cursor = self.conn.cursor()
         cursor.execute(sql)
         return cursor.fetchall()
 
     @ErrorTip
     def fetchmany(self, sql):
-        cursor = self.pyconn.cursor()
+        cursor = self.conn.cursor()
         cursor.execute(sql)
         return cursor.fetchmany()
 
     @ErrorTip
     def executemany(self, sql):
         return self.cursor.executemany(sql)
```

### Comparing `PrSpiders-0.4.9/PrSpider/requestXpath.py` & `PrSpiders-0.5.0/PrSpider/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.9/PrSpider/useragent.py` & `PrSpiders-0.5.0/PrSpider/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.9/PrSpiders.egg-info/PKG-INFO` & `PrSpiders-0.5.0/PrSpiders.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.4.9
+Version: 0.5.0
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.4.9/PrSpiders.egg-info/SOURCES.txt` & `PrSpiders-0.5.0/PrSpiders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.9/README.md` & `PrSpiders-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.9/pkg/prspider/PrSpider_CMD.py` & `PrSpiders-0.5.0/pkg/prspider/PrSpider_CMD.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.9/pkg/prspider/start.py` & `PrSpiders-0.5.0/pkg/prspider/start.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.9/requestXpath/__init__.py` & `PrSpiders-0.5.0/requestXpath/__init__.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.9/requestXpath/pxpath.py` & `PrSpiders-0.5.0/requestXpath/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.9/requestXpath/requestXpath.py` & `PrSpiders-0.5.0/requestXpath/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.9/requestXpath/useragent.py` & `PrSpiders-0.5.0/requestXpath/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.9/setup.py` & `PrSpiders-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!python
 # -*- coding:utf-8 -*-
 from __future__ import print_function
 from setuptools import setup, find_packages
 
-__version__ = "0.4.9"
+__version__ = "0.5.0"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PrSpiders",
     version=__version__,
```

