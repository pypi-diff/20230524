# Comparing `tmp/scrappo-1.1.0.tar.gz` & `tmp/scrappo-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrappo-1.1.0.tar", last modified: Thu Apr 27 23:26:57 2023, max compression
+gzip compressed data, was "scrappo-1.1.1.tar", last modified: Wed May 24 07:14:45 2023, max compression
```

## Comparing `scrappo-1.1.0.tar` & `scrappo-1.1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:26:57.667125 scrappo-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-27 23:26:42.000000 scrappo-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-04-27 23:26:57.667125 scrappo-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-27 23:26:42.000000 scrappo-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:26:57.663125 scrappo-1.1.0/scrappo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/movies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:26:57.663125 scrappo-1.1.0/scrappo/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/settings/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/url_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:26:57.667125 scrappo-1.1.0/scrappo/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/utils/bytes_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/utils/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/utils/reflection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/utils/split_string.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:26:57.667125 scrappo-1.1.0/scrappo/version/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/version/progsettings.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/version/progsettings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:26:57.663125 scrappo-1.1.0/scrappo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-04-27 23:26:57.000000 scrappo-1.1.0/scrappo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-27 23:26:57.000000 scrappo-1.1.0/scrappo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 23:26:57.000000 scrappo-1.1.0/scrappo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-27 23:26:57.000000 scrappo-1.1.0/scrappo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-27 23:26:57.000000 scrappo-1.1.0/scrappo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 23:26:57.000000 scrappo-1.1.0/scrappo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 23:26:57.667125 scrappo-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-27 23:26:42.000000 scrappo-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:14:45.106809 scrappo-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-24 07:14:29.000000 scrappo-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-05-24 07:14:45.106809 scrappo-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-05-24 07:14:29.000000 scrappo-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:14:45.102808 scrappo-1.1.1/scrappo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:14:29.000000 scrappo-1.1.1/scrappo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-24 07:14:29.000000 scrappo-1.1.1/scrappo/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-24 07:14:29.000000 scrappo-1.1.1/scrappo/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-24 07:14:29.000000 scrappo-1.1.1/scrappo/movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-24 07:14:29.000000 scrappo-1.1.1/scrappo/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-24 07:14:29.000000 scrappo-1.1.1/scrappo/series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:14:45.102808 scrappo-1.1.1/scrappo/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:14:29.000000 scrappo-1.1.1/scrappo/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-24 07:14:29.000000 scrappo-1.1.1/scrappo/settings/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-05-24 07:14:29.000000 scrappo-1.1.1/scrappo/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-24 07:14:29.000000 scrappo-1.1.1/scrappo/url_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:14:45.106809 scrappo-1.1.1/scrappo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:14:29.000000 scrappo-1.1.1/scrappo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-24 07:14:29.000000 scrappo-1.1.1/scrappo/utils/bytes_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-24 07:14:29.000000 scrappo-1.1.1/scrappo/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-24 07:14:29.000000 scrappo-1.1.1/scrappo/utils/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-24 07:14:29.000000 scrappo-1.1.1/scrappo/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-24 07:14:29.000000 scrappo-1.1.1/scrappo/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-24 07:14:29.000000 scrappo-1.1.1/scrappo/utils/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-24 07:14:29.000000 scrappo-1.1.1/scrappo/utils/split_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-24 07:14:29.000000 scrappo-1.1.1/scrappo/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:14:45.106809 scrappo-1.1.1/scrappo/version/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:14:29.000000 scrappo-1.1.1/scrappo/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-24 07:14:29.000000 scrappo-1.1.1/scrappo/version/progsettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-24 07:14:29.000000 scrappo-1.1.1/scrappo/version/progsettings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-24 07:14:29.000000 scrappo-1.1.1/scrappo/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:14:45.102808 scrappo-1.1.1/scrappo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-05-24 07:14:45.000000 scrappo-1.1.1/scrappo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-24 07:14:45.000000 scrappo-1.1.1/scrappo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 07:14:45.000000 scrappo-1.1.1/scrappo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-24 07:14:45.000000 scrappo-1.1.1/scrappo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-24 07:14:45.000000 scrappo-1.1.1/scrappo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 07:14:45.000000 scrappo-1.1.1/scrappo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 07:14:45.106809 scrappo-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-24 07:14:29.000000 scrappo-1.1.1/setup.py
```

### Comparing `scrappo-1.1.0/LICENSE` & `scrappo-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scrappo-1.1.0/PKG-INFO` & `scrappo-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrappo
-Version: 1.1.0
+Version: 1.1.1
 Summary: Download any video from a specific URL.
 Home-page: https://github.com/zaytiri/scrappo
 Author: zaytiri
 Project-URL: GitHub, https://github.com/zaytiri/scrappo
 Project-URL: Changelog, https://github.com/zaytiri/scrappo/blob/main/CHANGELOG.md
 Keywords: video,download,tool,scrapping,scrap,cli,url python
 Classifier: Environment :: Console
```

### Comparing `scrappo-1.1.0/README.md` & `scrappo-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `scrappo-1.1.0/scrappo/downloader.py` & `scrappo-1.1.1/scrappo/downloader.py`

 * *Files identical despite different names*

### Comparing `scrappo-1.1.0/scrappo/movies.py` & `scrappo-1.1.1/scrappo/movies.py`

 * *Files identical despite different names*

### Comparing `scrappo-1.1.0/scrappo/processor.py` & `scrappo-1.1.1/scrappo/processor.py`

 * *Files identical despite different names*

### Comparing `scrappo-1.1.0/scrappo/series.py` & `scrappo-1.1.1/scrappo/series.py`

 * *Files identical despite different names*

### Comparing `scrappo-1.1.0/scrappo/settings/manager.py` & `scrappo-1.1.1/scrappo/settings/manager.py`

 * *Files identical despite different names*

### Comparing `scrappo-1.1.0/scrappo/settings/settings.py` & `scrappo-1.1.1/scrappo/settings/settings.py`

 * *Files identical despite different names*

### Comparing `scrappo-1.1.0/scrappo/url_parser.py` & `scrappo-1.1.1/scrappo/url_parser.py`

 * *Files identical despite different names*

### Comparing `scrappo-1.1.0/scrappo/utils/bytes_conversion.py` & `scrappo-1.1.1/scrappo/utils/bytes_conversion.py`

 * *Files identical despite different names*

### Comparing `scrappo-1.1.0/scrappo/utils/date.py` & `scrappo-1.1.1/scrappo/utils/date.py`

 * *Files identical despite different names*

### Comparing `scrappo-1.1.0/scrappo/utils/directory.py` & `scrappo-1.1.1/scrappo/utils/directory.py`

 * *Files identical despite different names*

### Comparing `scrappo-1.1.0/scrappo/utils/file.py` & `scrappo-1.1.1/scrappo/utils/file.py`

 * *Files identical despite different names*

### Comparing `scrappo-1.1.0/scrappo/utils/split_string.py` & `scrappo-1.1.1/scrappo/utils/split_string.py`

 * *Files identical despite different names*

### Comparing `scrappo-1.1.0/scrappo/video.py` & `scrappo-1.1.1/scrappo/video.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         if not os.path.isdir(parent_path):
             os.mkdir(parent_path)
         return parent_path
 
     @staticmethod
     def file_exists(path):
         if os.path.isfile(path):
-            show('Skipping existing video...')
+            show('Skipping existing video...\n')
             return True
         return False
 
     def add_errors(self, successful, path, url):
         if not successful:
             error = {'path': path, 'url': url}
             self.errors.append(error)
```

### Comparing `scrappo-1.1.0/scrappo.egg-info/PKG-INFO` & `scrappo-1.1.1/scrappo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrappo
-Version: 1.1.0
+Version: 1.1.1
 Summary: Download any video from a specific URL.
 Home-page: https://github.com/zaytiri/scrappo
 Author: zaytiri
 Project-URL: GitHub, https://github.com/zaytiri/scrappo
 Project-URL: Changelog, https://github.com/zaytiri/scrappo/blob/main/CHANGELOG.md
 Keywords: video,download,tool,scrapping,scrap,cli,url python
 Classifier: Environment :: Console
```

### Comparing `scrappo-1.1.0/scrappo.egg-info/SOURCES.txt` & `scrappo-1.1.1/scrappo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scrappo-1.1.0/setup.py` & `scrappo-1.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     keywords="video, download, tool, scrapping, scrap, cli, url python",
     package_data={'scrappo': ['version/progsettings.yaml']},
     packages=["scrappo", "scrappo.utils", "scrappo.version", "scrappo.settings"],
     python_requires=">=3.10.6",
     install_requires=[
         "PyYAML~=6.0",
         "margument>=1.1.1",
-        "requests~=2.28.2",
+        "requests>=2.31.0",
         "progress~=1.6",
     ],
     entry_points={
         "console_scripts": [
             "scrappo=scrappo:app.main",
         ],
     }
-)
+)
```

