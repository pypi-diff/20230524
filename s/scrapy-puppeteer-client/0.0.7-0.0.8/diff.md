# Comparing `tmp/scrapy-puppeteer-client-0.0.7.tar.gz` & `tmp/scrapy-puppeteer-client-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy-puppeteer-client-0.0.7.tar", last modified: Tue May  2 09:27:56 2023, max compression
+gzip compressed data, was "scrapy-puppeteer-client-0.0.8.tar", last modified: Wed May 24 13:35:46 2023, max compression
```

## Comparing `scrapy-puppeteer-client-0.0.7.tar` & `scrapy-puppeteer-client-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:27:56.176780 scrapy-puppeteer-client-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-02 09:27:46.000000 scrapy-puppeteer-client-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-05-02 09:27:56.176780 scrapy-puppeteer-client-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-05-02 09:27:46.000000 scrapy-puppeteer-client-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:27:56.172780 scrapy-puppeteer-client-0.0.7/scrapy_puppeteer_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-05-02 09:27:56.000000 scrapy-puppeteer-client-0.0.7/scrapy_puppeteer_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-02 09:27:56.000000 scrapy-puppeteer-client-0.0.7/scrapy_puppeteer_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:27:56.000000 scrapy-puppeteer-client-0.0.7/scrapy_puppeteer_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 09:27:56.000000 scrapy-puppeteer-client-0.0.7/scrapy_puppeteer_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:27:56.176780 scrapy-puppeteer-client-0.0.7/scrapypuppeteer/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-02 09:27:46.000000 scrapy-puppeteer-client-0.0.7/scrapypuppeteer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-05-02 09:27:46.000000 scrapy-puppeteer-client-0.0.7/scrapypuppeteer/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-02 09:27:46.000000 scrapy-puppeteer-client-0.0.7/scrapypuppeteer/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-02 09:27:46.000000 scrapy-puppeteer-client-0.0.7/scrapypuppeteer/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-02 09:27:46.000000 scrapy-puppeteer-client-0.0.7/scrapypuppeteer/response.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 09:27:56.176780 scrapy-puppeteer-client-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-02 09:27:46.000000 scrapy-puppeteer-client-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:35:46.904196 scrapy-puppeteer-client-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-24 13:35:33.000000 scrapy-puppeteer-client-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-05-24 13:35:46.904196 scrapy-puppeteer-client-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-05-24 13:35:33.000000 scrapy-puppeteer-client-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:35:46.904196 scrapy-puppeteer-client-0.0.8/scrapy_puppeteer_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-05-24 13:35:46.000000 scrapy-puppeteer-client-0.0.8/scrapy_puppeteer_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-24 13:35:46.000000 scrapy-puppeteer-client-0.0.8/scrapy_puppeteer_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:35:46.000000 scrapy-puppeteer-client-0.0.8/scrapy_puppeteer_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-24 13:35:46.000000 scrapy-puppeteer-client-0.0.8/scrapy_puppeteer_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:35:46.904196 scrapy-puppeteer-client-0.0.8/scrapypuppeteer/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-24 13:35:33.000000 scrapy-puppeteer-client-0.0.8/scrapypuppeteer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-05-24 13:35:33.000000 scrapy-puppeteer-client-0.0.8/scrapypuppeteer/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-05-24 13:35:33.000000 scrapy-puppeteer-client-0.0.8/scrapypuppeteer/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-24 13:35:33.000000 scrapy-puppeteer-client-0.0.8/scrapypuppeteer/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-24 13:35:33.000000 scrapy-puppeteer-client-0.0.8/scrapypuppeteer/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 13:35:46.904196 scrapy-puppeteer-client-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-24 13:35:33.000000 scrapy-puppeteer-client-0.0.8/setup.py
```

### Comparing `scrapy-puppeteer-client-0.0.7/LICENSE` & `scrapy-puppeteer-client-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy-puppeteer-client-0.0.7/PKG-INFO` & `scrapy-puppeteer-client-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-puppeteer-client
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library to use Puppeteer-managed browser in Scrapy spiders
 Home-page: https://github.com/ispras/scrapy-puppeteer
 Author: MODIS @ ISP RAS
 Maintainer: Maksim Varlamov
 Maintainer-email: varlamov@ispras.ru
 License: BSD
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `scrapy-puppeteer-client-0.0.7/README.md` & `scrapy-puppeteer-client-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `scrapy-puppeteer-client-0.0.7/scrapy_puppeteer_client.egg-info/PKG-INFO` & `scrapy-puppeteer-client-0.0.8/scrapy_puppeteer_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-puppeteer-client
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library to use Puppeteer-managed browser in Scrapy spiders
 Home-page: https://github.com/ispras/scrapy-puppeteer
 Author: MODIS @ ISP RAS
 Maintainer: Maksim Varlamov
 Maintainer-email: varlamov@ispras.ru
 License: BSD
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `scrapy-puppeteer-client-0.0.7/scrapypuppeteer/actions.py` & `scrapy-puppeteer-client-0.0.8/scrapypuppeteer/actions.py`

 * *Files identical despite different names*

### Comparing `scrapy-puppeteer-client-0.0.7/scrapypuppeteer/middleware.py` & `scrapy-puppeteer-client-0.0.8/scrapypuppeteer/middleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             proxy = request.meta.get('proxy')
             if proxy:
                 payload['proxy'] = proxy
             include_headers = self.include_headers if request.include_headers is None else request.include_headers
             if include_headers:
                 headers = request.headers.to_unicode_dict()
                 if isinstance(include_headers, list):
-                    headers = {h: headers[h] for h in include_headers if h in headers}
+                    headers = {h.lower(): headers[h] for h in include_headers if h in headers}
                 payload['headers'] = headers
             return json.dumps(payload)
         return str(payload)
 
     def process_response(self, request, response, spider):
         if not isinstance(response, TextResponse):
             return response
```

### Comparing `scrapy-puppeteer-client-0.0.7/scrapypuppeteer/request.py` & `scrapy-puppeteer-client-0.0.8/scrapypuppeteer/request.py`

 * *Files identical despite different names*

### Comparing `scrapy-puppeteer-client-0.0.7/scrapypuppeteer/response.py` & `scrapy-puppeteer-client-0.0.8/scrapypuppeteer/response.py`

 * *Files identical despite different names*

### Comparing `scrapy-puppeteer-client-0.0.7/setup.py` & `scrapy-puppeteer-client-0.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
 setup(
     name='scrapy-puppeteer-client',
-    version='0.0.7',
+    version='0.0.8',
     description='A library to use Puppeteer-managed browser in Scrapy spiders',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/ispras/scrapy-puppeteer',
     author='MODIS @ ISP RAS',
     maintainer='Maksim Varlamov',
     maintainer_email='varlamov@ispras.ru',
```

