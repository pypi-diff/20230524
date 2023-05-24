# Comparing `tmp/djangoldp_application-1.1.7.tar.gz` & `tmp/djangoldp_application-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_application-1.1.7.tar", last modified: Tue May 23 12:41:36 2023, max compression
+gzip compressed data, was "dist/djangoldp_application-1.1.8.tar", last modified: Wed May 24 05:14:26 2023, max compression
```

## Comparing `djangoldp_application-1.1.7.tar` & `djangoldp_application-1.1.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:41:36.000000 djangoldp_application-1.1.7/
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-05-23 12:41:18.000000 djangoldp_application-1.1.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-23 12:41:18.000000 djangoldp_application-1.1.7/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      641 2023-05-23 12:41:36.000000 djangoldp_application-1.1.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-23 12:41:36.000000 djangoldp_application-1.1.7/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:41:36.000000 djangoldp_application-1.1.7/djangoldp_application.egg-info/
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-23 12:41:35.000000 djangoldp_application-1.1.7/djangoldp_application.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 12:41:35.000000 djangoldp_application-1.1.7/djangoldp_application.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1348 2023-05-23 12:41:35.000000 djangoldp_application-1.1.7/djangoldp_application.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-23 12:41:35.000000 djangoldp_application-1.1.7/djangoldp_application.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-23 12:41:35.000000 djangoldp_application-1.1.7/djangoldp_application.egg-info/requires.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:41:36.000000 djangoldp_application-1.1.7/djangoldp_application/
--rw-rw-rw-   0 root         (0) root         (0)    17495 2023-05-23 12:41:18.000000 djangoldp_application-1.1.7/djangoldp_application/views.py
--rw-rw-rw-   0 root         (0) root         (0)    19301 2023-05-23 12:41:18.000000 djangoldp_application-1.1.7/djangoldp_application/models.py
--rw-rw-rw-   0 root         (0) root         (0)     5488 2023-05-23 12:41:18.000000 djangoldp_application-1.1.7/djangoldp_application/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-05-23 12:41:18.000000 djangoldp_application-1.1.7/djangoldp_application/djangoldp_urls.py
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-05-23 12:41:33.000000 djangoldp_application-1.1.7/djangoldp_application/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-23 12:41:18.000000 djangoldp_application-1.1.7/djangoldp_application/apps.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-23 12:41:18.000000 djangoldp_application-1.1.7/djangoldp_application/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:41:36.000000 djangoldp_application-1.1.7/djangoldp_application/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2264 2023-05-23 12:41:18.000000 djangoldp_application-1.1.7/djangoldp_application/migrations/0009_applicationgraphics.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-05-23 12:41:18.000000 djangoldp_application-1.1.7/djangoldp_application/migrations/0014_auto_20230512_1613.py
--rw-rw-rw-   0 root         (0) root         (0)    22281 2023-05-23 12:41:18.000000 djangoldp_application-1.1.7/djangoldp_application/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-05-23 12:41:18.000000 djangoldp_application-1.1.7/djangoldp_application/migrations/0011_auto_20230512_1555.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-05-23 12:41:18.000000 djangoldp_application-1.1.7/djangoldp_application/migrations/0010_auto_20230331_0921.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 12:41:18.000000 djangoldp_application-1.1.7/djangoldp_application/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-05-23 12:41:18.000000 djangoldp_application-1.1.7/djangoldp_application/migrations/0013_auto_20230512_1608.py
--rw-rw-rw-   0 root         (0) root         (0)      549 2023-05-23 12:41:18.000000 djangoldp_application-1.1.7/djangoldp_application/migrations/0012_auto_20230512_1556.py
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-05-23 12:41:18.000000 djangoldp_application-1.1.7/djangoldp_application/migrations/0003_application_api_url.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2023-05-23 12:41:18.000000 djangoldp_application-1.1.7/djangoldp_application/migrations/0005_auto_20230331_0850.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-05-23 12:41:18.000000 djangoldp_application-1.1.7/djangoldp_application/migrations/0007_auto_20230331_0857.py
--rw-rw-rw-   0 root         (0) root         (0)     2157 2023-05-23 12:41:18.000000 djangoldp_application-1.1.7/djangoldp_application/migrations/0008_applicationnpm.py
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-05-23 12:41:18.000000 djangoldp_application-1.1.7/djangoldp_application/migrations/0004_auto_20230328_1657.py
--rw-rw-rw-   0 root         (0) root         (0)     2271 2023-05-23 12:41:18.000000 djangoldp_application-1.1.7/djangoldp_application/migrations/0002_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)     2283 2023-05-23 12:41:18.000000 djangoldp_application-1.1.7/djangoldp_application/migrations/0006_applicationservice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 05:14:26.000000 djangoldp_application-1.1.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-05-24 05:14:08.000000 djangoldp_application-1.1.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-24 05:14:08.000000 djangoldp_application-1.1.8/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-05-24 05:14:26.000000 djangoldp_application-1.1.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-24 05:14:26.000000 djangoldp_application-1.1.8/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 05:14:26.000000 djangoldp_application-1.1.8/djangoldp_application.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-24 05:14:26.000000 djangoldp_application-1.1.8/djangoldp_application.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 05:14:26.000000 djangoldp_application-1.1.8/djangoldp_application.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1348 2023-05-24 05:14:26.000000 djangoldp_application-1.1.8/djangoldp_application.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 05:14:26.000000 djangoldp_application-1.1.8/djangoldp_application.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-24 05:14:26.000000 djangoldp_application-1.1.8/djangoldp_application.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 05:14:26.000000 djangoldp_application-1.1.8/djangoldp_application/
+-rw-rw-rw-   0 root         (0) root         (0)    17495 2023-05-24 05:14:08.000000 djangoldp_application-1.1.8/djangoldp_application/views.py
+-rw-rw-rw-   0 root         (0) root         (0)    19328 2023-05-24 05:14:08.000000 djangoldp_application-1.1.8/djangoldp_application/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     5488 2023-05-24 05:14:08.000000 djangoldp_application-1.1.8/djangoldp_application/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-05-24 05:14:08.000000 djangoldp_application-1.1.8/djangoldp_application/djangoldp_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-05-24 05:14:24.000000 djangoldp_application-1.1.8/djangoldp_application/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-24 05:14:08.000000 djangoldp_application-1.1.8/djangoldp_application/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-24 05:14:08.000000 djangoldp_application-1.1.8/djangoldp_application/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 05:14:26.000000 djangoldp_application-1.1.8/djangoldp_application/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-05-24 05:14:08.000000 djangoldp_application-1.1.8/djangoldp_application/migrations/0009_applicationgraphics.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-05-24 05:14:08.000000 djangoldp_application-1.1.8/djangoldp_application/migrations/0014_auto_20230512_1613.py
+-rw-rw-rw-   0 root         (0) root         (0)    22281 2023-05-24 05:14:08.000000 djangoldp_application-1.1.8/djangoldp_application/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-05-24 05:14:08.000000 djangoldp_application-1.1.8/djangoldp_application/migrations/0011_auto_20230512_1555.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-05-24 05:14:08.000000 djangoldp_application-1.1.8/djangoldp_application/migrations/0010_auto_20230331_0921.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 05:14:08.000000 djangoldp_application-1.1.8/djangoldp_application/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-05-24 05:14:08.000000 djangoldp_application-1.1.8/djangoldp_application/migrations/0013_auto_20230512_1608.py
+-rw-rw-rw-   0 root         (0) root         (0)      549 2023-05-24 05:14:08.000000 djangoldp_application-1.1.8/djangoldp_application/migrations/0012_auto_20230512_1556.py
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-05-24 05:14:08.000000 djangoldp_application-1.1.8/djangoldp_application/migrations/0003_application_api_url.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2023-05-24 05:14:08.000000 djangoldp_application-1.1.8/djangoldp_application/migrations/0005_auto_20230331_0850.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-05-24 05:14:08.000000 djangoldp_application-1.1.8/djangoldp_application/migrations/0007_auto_20230331_0857.py
+-rw-rw-rw-   0 root         (0) root         (0)     2157 2023-05-24 05:14:08.000000 djangoldp_application-1.1.8/djangoldp_application/migrations/0008_applicationnpm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-05-24 05:14:08.000000 djangoldp_application-1.1.8/djangoldp_application/migrations/0004_auto_20230328_1657.py
+-rw-rw-rw-   0 root         (0) root         (0)     2271 2023-05-24 05:14:08.000000 djangoldp_application-1.1.8/djangoldp_application/migrations/0002_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)     2283 2023-05-24 05:14:08.000000 djangoldp_application-1.1.8/djangoldp_application/migrations/0006_applicationservice.py
```

### Comparing `djangoldp_application-1.1.7/README.md` & `djangoldp_application-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.7/setup.cfg` & `djangoldp_application-1.1.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.7/djangoldp_application.egg-info/SOURCES.txt` & `djangoldp_application-1.1.8/djangoldp_application.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.7/djangoldp_application/views.py` & `djangoldp_application-1.1.8/djangoldp_application/views.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.7/djangoldp_application/models.py` & `djangoldp_application-1.1.8/djangoldp_application/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,14 +71,15 @@
             "application_title",
             "application_logo",
             "components",
             "packages",
             "graphics",
             "services",
             "federation",
+            "deployments",
         ]
         superuser_perms = ["view"]
         verbose_name = _("application")
         verbose_name_plural = _("applications")
 
 
 STATUS_CHOICES = [
```

### Comparing `djangoldp_application-1.1.7/djangoldp_application/admin.py` & `djangoldp_application-1.1.8/djangoldp_application/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.7/djangoldp_application/djangoldp_urls.py` & `djangoldp_application-1.1.8/djangoldp_application/djangoldp_urls.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.7/djangoldp_application/migrations/0009_applicationgraphics.py` & `djangoldp_application-1.1.8/djangoldp_application/migrations/0009_applicationgraphics.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.7/djangoldp_application/migrations/0014_auto_20230512_1613.py` & `djangoldp_application-1.1.8/djangoldp_application/migrations/0014_auto_20230512_1613.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.7/djangoldp_application/migrations/0001_initial.py` & `djangoldp_application-1.1.8/djangoldp_application/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.7/djangoldp_application/migrations/0011_auto_20230512_1555.py` & `djangoldp_application-1.1.8/djangoldp_application/migrations/0011_auto_20230512_1555.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.7/djangoldp_application/migrations/0010_auto_20230331_0921.py` & `djangoldp_application-1.1.8/djangoldp_application/migrations/0010_auto_20230331_0921.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.7/djangoldp_application/migrations/0013_auto_20230512_1608.py` & `djangoldp_application-1.1.8/djangoldp_application/migrations/0013_auto_20230512_1608.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.7/djangoldp_application/migrations/0012_auto_20230512_1556.py` & `djangoldp_application-1.1.8/djangoldp_application/migrations/0012_auto_20230512_1556.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.7/djangoldp_application/migrations/0005_auto_20230331_0850.py` & `djangoldp_application-1.1.8/djangoldp_application/migrations/0005_auto_20230331_0850.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.7/djangoldp_application/migrations/0008_applicationnpm.py` & `djangoldp_application-1.1.8/djangoldp_application/migrations/0008_applicationnpm.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.7/djangoldp_application/migrations/0004_auto_20230328_1657.py` & `djangoldp_application-1.1.8/djangoldp_application/migrations/0004_auto_20230328_1657.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.7/djangoldp_application/migrations/0002_deployment.py` & `djangoldp_application-1.1.8/djangoldp_application/migrations/0002_deployment.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.7/djangoldp_application/migrations/0006_applicationservice.py` & `djangoldp_application-1.1.8/djangoldp_application/migrations/0006_applicationservice.py`

 * *Files identical despite different names*

