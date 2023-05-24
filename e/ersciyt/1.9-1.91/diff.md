# Comparing `tmp/ersciyt-1.9.tar.gz` & `tmp/ersciyt-1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ersciyt-1.9.tar", last modified: Tue May 23 15:17:48 2023, max compression
+gzip compressed data, was "ersciyt-1.91.tar", last modified: Tue May 23 15:49:39 2023, max compression
```

## Comparing `ersciyt-1.9.tar` & `ersciyt-1.91.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:17:48.640834 ersciyt-1.9/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-05-23 15:17:40.000000 ersciyt-1.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-23 15:17:40.000000 ersciyt-1.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      631 2023-05-23 15:17:48.640834 ersciyt-1.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      365 2023-05-23 15:17:40.000000 ersciyt-1.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:17:48.638834 ersciyt-1.9/ersciyt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 15:17:40.000000 ersciyt-1.9/ersciyt/__init__.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-23 15:17:40.000000 ersciyt-1.9/ersciyt/admin.py
--rw-r--r--   0 root         (0) root         (0)      146 2023-05-23 15:17:40.000000 ersciyt-1.9/ersciyt/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:17:48.639834 ersciyt-1.9/ersciyt/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 15:17:40.000000 ersciyt-1.9/ersciyt/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2023-05-23 15:17:40.000000 ersciyt-1.9/ersciyt/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:17:48.639834 ersciyt-1.9/ersciyt/static/
--rw-r--r--   0 root         (0) root         (0)    11852 2023-05-23 15:17:40.000000 ersciyt-1.9/ersciyt/static/ersci_viddown_tab2.xpi
--rw-r--r--   0 root         (0) root         (0)        2 2023-05-23 15:17:40.000000 ersciyt-1.9/ersciyt/static/ytvid.mp4
--rw-r--r--   0 root         (0) root         (0)       60 2023-05-23 15:17:40.000000 ersciyt-1.9/ersciyt/tests.py
--rw-r--r--   0 root         (0) root         (0)      573 2023-05-23 15:17:40.000000 ersciyt-1.9/ersciyt/urls.py
--rw-r--r--   0 root         (0) root         (0)     8711 2023-05-23 15:17:40.000000 ersciyt-1.9/ersciyt/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:17:48.639834 ersciyt-1.9/ersciyt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      631 2023-05-23 15:17:48.000000 ersciyt-1.9/ersciyt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      417 2023-05-23 15:17:48.000000 ersciyt-1.9/ersciyt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 15:17:48.000000 ersciyt-1.9/ersciyt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-23 15:17:48.000000 ersciyt-1.9/ersciyt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-23 15:17:48.000000 ersciyt-1.9/ersciyt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      664 2023-05-23 15:17:48.640834 ersciyt-1.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-23 15:17:40.000000 ersciyt-1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:49:39.075537 ersciyt-1.91/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-05-23 15:49:29.000000 ersciyt-1.91/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-23 15:49:29.000000 ersciyt-1.91/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      632 2023-05-23 15:49:39.075537 ersciyt-1.91/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      365 2023-05-23 15:49:29.000000 ersciyt-1.91/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:49:39.073536 ersciyt-1.91/ersciyt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 15:49:29.000000 ersciyt-1.91/ersciyt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-23 15:49:29.000000 ersciyt-1.91/ersciyt/admin.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-05-23 15:49:29.000000 ersciyt-1.91/ersciyt/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:49:39.074536 ersciyt-1.91/ersciyt/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 15:49:29.000000 ersciyt-1.91/ersciyt/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-23 15:49:29.000000 ersciyt-1.91/ersciyt/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:49:39.075537 ersciyt-1.91/ersciyt/static/
+-rw-r--r--   0 root         (0) root         (0)    11852 2023-05-23 15:49:29.000000 ersciyt-1.91/ersciyt/static/ersci_viddown_tab2.xpi
+-rw-r--r--   0 root         (0) root         (0)        2 2023-05-23 15:49:29.000000 ersciyt-1.91/ersciyt/static/ytvid.mp4
+-rw-r--r--   0 root         (0) root         (0)       60 2023-05-23 15:49:29.000000 ersciyt-1.91/ersciyt/tests.py
+-rw-r--r--   0 root         (0) root         (0)      573 2023-05-23 15:49:29.000000 ersciyt-1.91/ersciyt/urls.py
+-rw-r--r--   0 root         (0) root         (0)     8712 2023-05-23 15:49:29.000000 ersciyt-1.91/ersciyt/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:49:39.074536 ersciyt-1.91/ersciyt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      632 2023-05-23 15:49:38.000000 ersciyt-1.91/ersciyt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      417 2023-05-23 15:49:38.000000 ersciyt-1.91/ersciyt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 15:49:38.000000 ersciyt-1.91/ersciyt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-23 15:49:38.000000 ersciyt-1.91/ersciyt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-23 15:49:38.000000 ersciyt-1.91/ersciyt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      665 2023-05-23 15:49:39.076537 ersciyt-1.91/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-23 15:49:29.000000 ersciyt-1.91/setup.py
```

### Comparing `ersciyt-1.9/LICENSE` & `ersciyt-1.91/LICENSE`

 * *Files identical despite different names*

### Comparing `ersciyt-1.9/PKG-INFO` & `ersciyt-1.91/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.9
+Version: 1.91
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ersciyt-1.9/ersciyt/static/ersci_viddown_tab2.xpi` & `ersciyt-1.91/ersciyt/static/ersci_viddown_tab2.xpi`

 * *Files identical despite different names*

### Comparing `ersciyt-1.9/ersciyt/urls.py` & `ersciyt-1.91/ersciyt/urls.py`

 * *Files identical despite different names*

### Comparing `ersciyt-1.9/ersciyt/views.py` & `ersciyt-1.91/ersciyt/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
     except:
         return HttpResponse ('Youtube Url Is Mistake!')
 
 def yt2mp4(request,link):
     try:        
         vidpath = finders.find('ytvid.mp4')        
         if os.path.isfile(vidpath):
-            os.remove(vipath)
+            os.remove(vidpath)
         os.system('yt-dlp  -f 18 -o {} https://www.youtube.com/watch?v={}'.format(vidpath,link)) 
         return redirect("/static/ytvid.mp4")
     except:
         return HttpResponse ('Youtube Url Is Mistake!')
 
 def shqr(request):
     try:
```

### Comparing `ersciyt-1.9/ersciyt.egg-info/PKG-INFO` & `ersciyt-1.91/ersciyt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.9
+Version: 1.91
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ersciyt-1.9/setup.cfg` & `ersciyt-1.91/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ersciyt
-version = 1.9
+version = 1.91
 description = Youtube Downloader
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/epg900/yt.git
 author = epg
 author_email = epg900@gmail.com
 license = GNU GENERAL PUBLIC LICENSE
```

