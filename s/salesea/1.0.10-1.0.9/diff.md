# Comparing `tmp/salesea-1.0.10.tar.gz` & `tmp/salesea-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salesea-1.0.10.tar", last modified: Wed May 24 02:22:32 2023, max compression
+gzip compressed data, was "salesea-1.0.9.tar", last modified: Tue May 23 07:38:20 2023, max compression
```

## Comparing `salesea-1.0.10.tar` & `salesea-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 02:22:32.346042 salesea-1.0.10/
--rw-rw-rw-   0        0        0     2588 2023-05-24 02:22:32.346042 salesea-1.0.10/PKG-INFO
--rw-rw-rw-   0        0        0     1613 2023-05-22 09:08:17.000000 salesea-1.0.10/README.md
--rw-rw-rw-   0        0        0      111 2023-05-24 02:22:32.347036 salesea-1.0.10/setup.cfg
--rw-rw-rw-   0        0        0     2300 2023-05-24 02:21:52.000000 salesea-1.0.10/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 02:22:32.326035 salesea-1.0.10/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 02:22:32.339035 salesea-1.0.10/src/salesea/
--rw-rw-rw-   0        0        0       25 2023-05-18 07:08:55.000000 salesea-1.0.10/src/salesea/__init__.py
--rw-rw-rw-   0        0        0     1916 2023-05-18 08:27:21.000000 salesea-1.0.10/src/salesea/__main__.py
--rw-rw-rw-   0        0        0     7111 2023-05-23 07:51:49.000000 salesea-1.0.10/src/salesea/app.py
--rw-rw-rw-   0        0        0     3509 2023-05-18 08:19:26.000000 salesea-1.0.10/src/salesea/config.py
--rw-rw-rw-   0        0        0     1214 2023-05-22 05:27:18.000000 salesea-1.0.10/src/salesea/log.py
--rw-rw-rw-   0        0        0     7716 2023-05-22 03:01:08.000000 salesea-1.0.10/src/salesea/nginx.py
--rw-rw-rw-   0        0        0      936 2023-05-18 09:22:59.000000 salesea-1.0.10/src/salesea/solution.py
--rw-rw-rw-   0        0        0      134 2023-05-18 07:39:33.000000 salesea-1.0.10/src/salesea/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-24 02:22:32.345064 salesea-1.0.10/src/salesea.egg-info/
--rw-rw-rw-   0        0        0     2588 2023-05-24 02:22:32.000000 salesea-1.0.10/src/salesea.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      414 2023-05-24 02:22:32.000000 salesea-1.0.10/src/salesea.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 02:22:32.000000 salesea-1.0.10/src/salesea.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-24 02:22:32.000000 salesea-1.0.10/src/salesea.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-05-24 02:22:32.000000 salesea-1.0.10/src/salesea.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-24 02:22:32.000000 salesea-1.0.10/src/salesea.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 07:38:20.782057 salesea-1.0.9/
+-rw-rw-rw-   0        0        0     2587 2023-05-23 07:38:20.782057 salesea-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1613 2023-05-22 09:08:17.000000 salesea-1.0.9/README.md
+-rw-rw-rw-   0        0        0      111 2023-05-23 07:38:20.783057 salesea-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2298 2023-05-23 07:16:05.000000 salesea-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:38:20.757001 salesea-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 07:38:20.775057 salesea-1.0.9/src/salesea/
+-rw-rw-rw-   0        0        0       25 2023-05-18 07:08:55.000000 salesea-1.0.9/src/salesea/__init__.py
+-rw-rw-rw-   0        0        0     1916 2023-05-18 08:27:21.000000 salesea-1.0.9/src/salesea/__main__.py
+-rw-rw-rw-   0        0        0     7119 2023-05-23 07:18:06.000000 salesea-1.0.9/src/salesea/app.py
+-rw-rw-rw-   0        0        0     3509 2023-05-18 08:19:26.000000 salesea-1.0.9/src/salesea/config.py
+-rw-rw-rw-   0        0        0     1214 2023-05-22 05:27:18.000000 salesea-1.0.9/src/salesea/log.py
+-rw-rw-rw-   0        0        0     7716 2023-05-22 03:01:08.000000 salesea-1.0.9/src/salesea/nginx.py
+-rw-rw-rw-   0        0        0      936 2023-05-18 09:22:59.000000 salesea-1.0.9/src/salesea/solution.py
+-rw-rw-rw-   0        0        0      134 2023-05-18 07:39:33.000000 salesea-1.0.9/src/salesea/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:38:20.781057 salesea-1.0.9/src/salesea.egg-info/
+-rw-rw-rw-   0        0        0     2587 2023-05-23 07:38:20.000000 salesea-1.0.9/src/salesea.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2023-05-23 07:38:20.000000 salesea-1.0.9/src/salesea.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 07:38:20.000000 salesea-1.0.9/src/salesea.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-23 07:38:20.000000 salesea-1.0.9/src/salesea.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-05-23 07:38:20.000000 salesea-1.0.9/src/salesea.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-23 07:38:20.000000 salesea-1.0.9/src/salesea.egg-info/top_level.txt
```

### Comparing `salesea-1.0.10/PKG-INFO` & `salesea-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesea
-Version: 1.0.10
+Version: 1.0.9
 Summary: This is an Nginx log collection tool.
 Author: howard
 Author-email: 18071131140telephone@gmail.com
 Keywords: nginx,logs,collection
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `salesea-1.0.10/README.md` & `salesea-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `salesea-1.0.10/setup.py` & `salesea-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #     print(requires.splitlines())
 # ------------------------------------------------------------------------------- #
 
 setup(
     name='salesea',
     author='howard',
     author_email='18071131140telephone@gmail.com',
-    version='1.0.10',
+    version='1.0.9',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     description='This is an Nginx log collection tool.',
     long_description=readme,
     long_description_content_type='text/markdown',
     keywords=[
         'nginx',
@@ -34,15 +34,15 @@
     #                   'attrs>=21.4.0',
     #                   'charset-normalizer>=2.0.7',
     #                   'frozenlist>=1.2.0',
     #                   'idna>=3.3',
     #                   'multidict>=5.2.0',
     #                   'yarl>=1.7.2'],
     install_requires=[
-        'requests>=2.18.4',
+        'requests>=2.26.0'
     ],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.0',
         'Programming Language :: Python :: 3.1',
         'Programming Language :: Python :: 3.2',
```

### Comparing `salesea-1.0.10/src/salesea/__main__.py` & `salesea-1.0.9/src/salesea/__main__.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.10/src/salesea/app.py` & `salesea-1.0.9/src/salesea/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 
     try:
         from .config import NGINX_PATH, SERVER_NAME, CHECK_INTERVAL, REQUEST_CONCURRENCY, VISIT_APIKEY, LOG_FORMAT
 
         try:
             nginx = Nginx(Path(NGINX_PATH) if NGINX_PATH else None)
         except NginxException as e:
-            logger.error(f"{e}")
+            logger.error(f"[nginx] {e}")
             exit(1)
 
         #############################################################################
         #####Print Config############################################################
         logger.debug(f"#" * 65)
         logger.debug(f"# nginx_path: {nginx.nginx_path}")
         logger.debug(f"# server_name: {SERVER_NAME}")
```

### Comparing `salesea-1.0.10/src/salesea/config.py` & `salesea-1.0.9/src/salesea/config.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.10/src/salesea/log.py` & `salesea-1.0.9/src/salesea/log.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.10/src/salesea/nginx.py` & `salesea-1.0.9/src/salesea/nginx.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.10/src/salesea/solution.py` & `salesea-1.0.9/src/salesea/solution.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.10/src/salesea.egg-info/PKG-INFO` & `salesea-1.0.9/src/salesea.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesea
-Version: 1.0.10
+Version: 1.0.9
 Summary: This is an Nginx log collection tool.
 Author: howard
 Author-email: 18071131140telephone@gmail.com
 Keywords: nginx,logs,collection
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.0
```

