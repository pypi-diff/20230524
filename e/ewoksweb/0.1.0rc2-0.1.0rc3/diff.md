# Comparing `tmp/ewoksweb-0.1.0rc2.tar.gz` & `tmp/ewoksweb-0.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ewoksweb-0.1.0rc2.tar", last modified: Tue May 23 16:08:30 2023, max compression
+gzip compressed data, was "ewoksweb-0.1.0rc3.tar", last modified: Wed May 24 08:24:21 2023, max compression
```

## Comparing `ewoksweb-0.1.0rc2.tar` & `ewoksweb-0.1.0rc3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:08:30.109697 ewoksweb-0.1.0rc2/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-05-23 05:03:43.000000 ewoksweb-0.1.0rc2/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     1736 2023-05-23 16:08:30.109697 ewoksweb-0.1.0rc2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1021 2023-05-23 05:03:43.000000 ewoksweb-0.1.0rc2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-23 05:03:44.000000 ewoksweb-0.1.0rc2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:08:30.093697 ewoksweb-0.1.0rc2/pysrc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:08:30.097697 ewoksweb-0.1.0rc2/pysrc/ewoksweb/
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-05-23 16:05:05.000000 ewoksweb-0.1.0rc2/pysrc/ewoksweb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-05-23 05:03:44.000000 ewoksweb-0.1.0rc2/pysrc/ewoksweb/serverutils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:08:30.097697 ewoksweb-0.1.0rc2/pysrc/ewoksweb/static/
--rw-r--r--   0 root         (0) root         (0)      457 2023-05-23 16:08:29.000000 ewoksweb-0.1.0rc2/pysrc/ewoksweb/static/asset-manifest.json
--rw-r--r--   0 root         (0) root         (0)     3870 2023-05-23 16:08:29.000000 ewoksweb-0.1.0rc2/pysrc/ewoksweb/static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)      635 2023-05-23 16:08:29.000000 ewoksweb-0.1.0rc2/pysrc/ewoksweb/static/index.html
--rw-r--r--   0 root         (0) root         (0)       67 2023-05-23 16:08:29.000000 ewoksweb-0.1.0rc2/pysrc/ewoksweb/static/robots.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:08:30.093697 ewoksweb-0.1.0rc2/pysrc/ewoksweb/static/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:08:30.097697 ewoksweb-0.1.0rc2/pysrc/ewoksweb/static/static/css/
--rw-r--r--   0 root         (0) root         (0)    13629 2023-05-23 16:08:29.000000 ewoksweb-0.1.0rc2/pysrc/ewoksweb/static/static/css/main.fa9245a4.css
--rw-r--r--   0 root         (0) root         (0)    28831 2023-05-23 16:08:29.000000 ewoksweb-0.1.0rc2/pysrc/ewoksweb/static/static/css/main.fa9245a4.css.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:08:30.101697 ewoksweb-0.1.0rc2/pysrc/ewoksweb/static/static/js/
--rw-r--r--   0 root         (0) root         (0)  1056065 2023-05-23 16:08:29.000000 ewoksweb-0.1.0rc2/pysrc/ewoksweb/static/static/js/main.573f7e67.js
--rw-r--r--   0 root         (0) root         (0)     3267 2023-05-23 16:08:29.000000 ewoksweb-0.1.0rc2/pysrc/ewoksweb/static/static/js/main.573f7e67.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)  4896448 2023-05-23 16:08:29.000000 ewoksweb-0.1.0rc2/pysrc/ewoksweb/static/static/js/main.573f7e67.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:08:30.105697 ewoksweb-0.1.0rc2/pysrc/ewoksweb/static/static/media/
--rw-r--r--   0 root         (0) root         (0)   157151 2023-05-23 16:08:29.000000 ewoksweb-0.1.0rc2/pysrc/ewoksweb/static/static/media/ewoksUI.27496ca19b6f9d2adad4.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:08:30.097697 ewoksweb-0.1.0rc2/pysrc/ewoksweb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1736 2023-05-23 16:08:30.000000 ewoksweb-0.1.0rc2/pysrc/ewoksweb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      779 2023-05-23 16:08:30.000000 ewoksweb-0.1.0rc2/pysrc/ewoksweb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 16:08:30.000000 ewoksweb-0.1.0rc2/pysrc/ewoksweb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-23 16:08:30.000000 ewoksweb-0.1.0rc2/pysrc/ewoksweb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-23 16:08:30.000000 ewoksweb-0.1.0rc2/pysrc/ewoksweb.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1026 2023-05-23 16:08:30.109697 ewoksweb-0.1.0rc2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      319 2023-05-23 05:03:44.000000 ewoksweb-0.1.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:24:21.188395 ewoksweb-0.1.0rc3/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-05-24 05:03:42.000000 ewoksweb-0.1.0rc3/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-05-24 08:24:21.188395 ewoksweb-0.1.0rc3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1021 2023-05-24 05:03:42.000000 ewoksweb-0.1.0rc3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-24 05:03:42.000000 ewoksweb-0.1.0rc3/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:24:21.172395 ewoksweb-0.1.0rc3/pysrc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:24:21.176395 ewoksweb-0.1.0rc3/pysrc/ewoksweb/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-05-24 08:10:04.000000 ewoksweb-0.1.0rc3/pysrc/ewoksweb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-05-24 05:03:42.000000 ewoksweb-0.1.0rc3/pysrc/ewoksweb/serverutils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:24:21.180395 ewoksweb-0.1.0rc3/pysrc/ewoksweb/static/
+-rw-r--r--   0 root         (0) root         (0)      457 2023-05-24 08:24:20.000000 ewoksweb-0.1.0rc3/pysrc/ewoksweb/static/asset-manifest.json
+-rw-r--r--   0 root         (0) root         (0)     3870 2023-05-24 08:24:20.000000 ewoksweb-0.1.0rc3/pysrc/ewoksweb/static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)      635 2023-05-24 08:24:20.000000 ewoksweb-0.1.0rc3/pysrc/ewoksweb/static/index.html
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-24 08:24:20.000000 ewoksweb-0.1.0rc3/pysrc/ewoksweb/static/robots.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:24:21.172395 ewoksweb-0.1.0rc3/pysrc/ewoksweb/static/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:24:21.180395 ewoksweb-0.1.0rc3/pysrc/ewoksweb/static/static/css/
+-rw-r--r--   0 root         (0) root         (0)    13629 2023-05-24 08:24:20.000000 ewoksweb-0.1.0rc3/pysrc/ewoksweb/static/static/css/main.fa9245a4.css
+-rw-r--r--   0 root         (0) root         (0)    28831 2023-05-24 08:24:20.000000 ewoksweb-0.1.0rc3/pysrc/ewoksweb/static/static/css/main.fa9245a4.css.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:24:21.180395 ewoksweb-0.1.0rc3/pysrc/ewoksweb/static/static/js/
+-rw-r--r--   0 root         (0) root         (0)  1056065 2023-05-24 08:24:20.000000 ewoksweb-0.1.0rc3/pysrc/ewoksweb/static/static/js/main.573f7e67.js
+-rw-r--r--   0 root         (0) root         (0)     3267 2023-05-24 08:24:20.000000 ewoksweb-0.1.0rc3/pysrc/ewoksweb/static/static/js/main.573f7e67.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)  4896448 2023-05-24 08:24:20.000000 ewoksweb-0.1.0rc3/pysrc/ewoksweb/static/static/js/main.573f7e67.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:24:21.188395 ewoksweb-0.1.0rc3/pysrc/ewoksweb/static/static/media/
+-rw-r--r--   0 root         (0) root         (0)   157151 2023-05-24 08:24:20.000000 ewoksweb-0.1.0rc3/pysrc/ewoksweb/static/static/media/ewoksUI.27496ca19b6f9d2adad4.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:24:21.176395 ewoksweb-0.1.0rc3/pysrc/ewoksweb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-05-24 08:24:21.000000 ewoksweb-0.1.0rc3/pysrc/ewoksweb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      779 2023-05-24 08:24:21.000000 ewoksweb-0.1.0rc3/pysrc/ewoksweb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 08:24:21.000000 ewoksweb-0.1.0rc3/pysrc/ewoksweb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-24 08:24:21.000000 ewoksweb-0.1.0rc3/pysrc/ewoksweb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-24 08:24:21.000000 ewoksweb-0.1.0rc3/pysrc/ewoksweb.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2023-05-24 08:24:21.188395 ewoksweb-0.1.0rc3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      319 2023-05-24 05:03:42.000000 ewoksweb-0.1.0rc3/setup.py
```

### Comparing `ewoksweb-0.1.0rc2/LICENSE.md` & `ewoksweb-0.1.0rc3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksweb-0.1.0rc2/PKG-INFO` & `ewoksweb-0.1.0rc3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksweb
-Version: 0.1.0rc2
+Version: 0.1.0rc3
 Summary: Web frontend for ewoks
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksweb
 Author: ESRF
 Author-email: giannis.koumoutsos@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksweb
 Project-URL: Documentation, https://workflow.gitlab-pages.esrf.fr/ewoks/ewoksweb
```

### Comparing `ewoksweb-0.1.0rc2/README.md` & `ewoksweb-0.1.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `ewoksweb-0.1.0rc2/pysrc/ewoksweb/static/favicon.ico` & `ewoksweb-0.1.0rc3/pysrc/ewoksweb/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ewoksweb-0.1.0rc2/pysrc/ewoksweb/static/index.html` & `ewoksweb-0.1.0rc3/pysrc/ewoksweb/static/index.html`

 * *Files identical despite different names*

### Comparing `ewoksweb-0.1.0rc2/pysrc/ewoksweb/static/static/css/main.fa9245a4.css` & `ewoksweb-0.1.0rc3/pysrc/ewoksweb/static/static/css/main.fa9245a4.css`

 * *Files identical despite different names*

### Comparing `ewoksweb-0.1.0rc2/pysrc/ewoksweb/static/static/css/main.fa9245a4.css.map` & `ewoksweb-0.1.0rc3/pysrc/ewoksweb/static/static/css/main.fa9245a4.css.map`

 * *Files identical despite different names*

### Comparing `ewoksweb-0.1.0rc2/pysrc/ewoksweb/static/static/js/main.573f7e67.js` & `ewoksweb-0.1.0rc3/pysrc/ewoksweb/static/static/js/main.573f7e67.js`

 * *Files identical despite different names*

### Comparing `ewoksweb-0.1.0rc2/pysrc/ewoksweb/static/static/js/main.573f7e67.js.LICENSE.txt` & `ewoksweb-0.1.0rc3/pysrc/ewoksweb/static/static/js/main.573f7e67.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ewoksweb-0.1.0rc2/pysrc/ewoksweb/static/static/js/main.573f7e67.js.map` & `ewoksweb-0.1.0rc3/pysrc/ewoksweb/static/static/js/main.573f7e67.js.map`

 * *Files identical despite different names*

### Comparing `ewoksweb-0.1.0rc2/pysrc/ewoksweb/static/static/media/ewoksUI.27496ca19b6f9d2adad4.png` & `ewoksweb-0.1.0rc3/pysrc/ewoksweb/static/static/media/ewoksUI.27496ca19b6f9d2adad4.png`

 * *Files identical despite different names*

### Comparing `ewoksweb-0.1.0rc2/pysrc/ewoksweb.egg-info/PKG-INFO` & `ewoksweb-0.1.0rc3/pysrc/ewoksweb.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksweb
-Version: 0.1.0rc2
+Version: 0.1.0rc3
 Summary: Web frontend for ewoks
 Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksweb
 Author: ESRF
 Author-email: giannis.koumoutsos@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksweb
 Project-URL: Documentation, https://workflow.gitlab-pages.esrf.fr/ewoks/ewoksweb
```

### Comparing `ewoksweb-0.1.0rc2/pysrc/ewoksweb.egg-info/SOURCES.txt` & `ewoksweb-0.1.0rc3/pysrc/ewoksweb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ewoksweb-0.1.0rc2/setup.cfg` & `ewoksweb-0.1.0rc3/setup.cfg`

 * *Files identical despite different names*

