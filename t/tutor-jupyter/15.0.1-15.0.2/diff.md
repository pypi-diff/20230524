# Comparing `tmp/tutor-jupyter-15.0.1.tar.gz` & `tmp/tutor-jupyter-15.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tutor-jupyter-15.0.1.tar", last modified: Mon May 22 07:45:20 2023, max compression
+gzip compressed data, was "dist/tutor-jupyter-15.0.2.tar", last modified: Wed May 24 21:11:35 2023, max compression
```

## Comparing `tutor-jupyter-15.0.1.tar` & `tutor-jupyter-15.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/
--rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/LICENSE.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       84 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     6018 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     5117 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/pyproject.toml
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     1774 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutor_jupyter.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     6018 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutor_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     1149 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutor_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutor_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       48 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutor_jupyter.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       48 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutor_jupyter.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       13 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutor_jupyter.egg-info/top_level.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutorjupyter/
--rw-r--r--   0 ci        (1000) ci        (1000)       23 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutorjupyter/patches/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/patches/.gitignore
--rw-r--r--   0 ci        (1000) ci        (1000)       78 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/patches/caddyfile
--rw-r--r--   0 ci        (1000) ci        (1000)       84 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/patches/dev-docker-compose-services
--rw-r--r--   0 ci        (1000) ci        (1000)      297 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/patches/local-docker-compose-jobs-services
--rw-r--r--   0 ci        (1000) ci        (1000)      464 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/patches/local-docker-compose-services
--rw-r--r--   0 ci        (1000) ci        (1000)      193 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/patches/openedx-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      176 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/patches/openedx-dockerfile-post-python-requirements
--rw-r--r--   0 ci        (1000) ci        (1000)     4145 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/plugin.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/apps/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/apps/.gitignore
--rw-r--r--   0 ci        (1000) ci        (1000)     4185 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/apps/jupyterhub_config.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/build/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/build/.gitignore
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/build/hub/
--rw-r--r--   0 ci        (1000) ci        (1000)      606 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/build/hub/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/build/lab/
--rw-r--r--   0 ci        (1000) ci        (1000)      838 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/build/lab/Dockerfile
--rw-r--r--   0 ci        (1000) ci        (1000)      295 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/build/lab/config.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/jobs/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/jobs/init/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/jobs/init/.gitignore
--rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/jobs/init/jupyterhub.sh
--rw-r--r--   0 ci        (1000) ci        (1000)      862 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/jobs/init/mysql.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/
+-rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/LICENSE.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       84 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     6018 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     5117 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/pyproject.toml
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     1774 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutor_jupyter.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     6018 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutor_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     1149 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutor_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutor_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       48 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutor_jupyter.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       48 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutor_jupyter.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       13 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutor_jupyter.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutorjupyter/
+-rw-r--r--   0 ci        (1000) ci        (1000)       23 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutorjupyter/patches/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/patches/.gitignore
+-rw-r--r--   0 ci        (1000) ci        (1000)       78 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/patches/caddyfile
+-rw-r--r--   0 ci        (1000) ci        (1000)       84 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/patches/dev-docker-compose-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      297 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      464 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/patches/local-docker-compose-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      193 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/patches/openedx-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)      176 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/patches/openedx-dockerfile-post-python-requirements
+-rw-r--r--   0 ci        (1000) ci        (1000)     4145 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/plugin.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/apps/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/apps/.gitignore
+-rw-r--r--   0 ci        (1000) ci        (1000)     4185 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/apps/jupyterhub_config.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/build/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/build/.gitignore
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/build/hub/
+-rw-r--r--   0 ci        (1000) ci        (1000)      410 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/build/hub/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/build/lab/
+-rw-r--r--   0 ci        (1000) ci        (1000)      838 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/build/lab/Dockerfile
+-rw-r--r--   0 ci        (1000) ci        (1000)      295 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/build/lab/config.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/jobs/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:35.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/jobs/init/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/jobs/init/.gitignore
+-rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/jobs/init/jupyterhub.sh
+-rw-r--r--   0 ci        (1000) ci        (1000)      862 2023-05-24 21:11:27.000000 tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/jobs/init/mysql.sh
```

### Comparing `tutor-jupyter-15.0.1/LICENSE.txt` & `tutor-jupyter-15.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-15.0.1/PKG-INFO` & `tutor-jupyter-15.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-jupyter
-Version: 15.0.1
+Version: 15.0.2
 Summary: Jupyter Notebook plugin for Tutor
 Home-page: https://github.com/overhangio/tutor-jupyter
 Author: Overhang.IO
 Maintainer: Régis Behmo
 Maintainer-email: regis@overhang.io
 License: AGPLv3
 Project-URL: Code, https://github.com/overhangio/tutor-jupyter
```

### Comparing `tutor-jupyter-15.0.1/README.rst` & `tutor-jupyter-15.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-15.0.1/setup.py` & `tutor-jupyter-15.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-15.0.1/tutor_jupyter.egg-info/PKG-INFO` & `tutor-jupyter-15.0.2/tutor_jupyter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-jupyter
-Version: 15.0.1
+Version: 15.0.2
 Summary: Jupyter Notebook plugin for Tutor
 Home-page: https://github.com/overhangio/tutor-jupyter
 Author: Overhang.IO
 Maintainer: Régis Behmo
 Maintainer-email: regis@overhang.io
 License: AGPLv3
 Project-URL: Code, https://github.com/overhangio/tutor-jupyter
```

### Comparing `tutor-jupyter-15.0.1/tutor_jupyter.egg-info/SOURCES.txt` & `tutor-jupyter-15.0.2/tutor_jupyter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-15.0.1/tutorjupyter/plugin.py` & `tutor-jupyter-15.0.2/tutorjupyter/plugin.py`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/apps/jupyterhub_config.py` & `tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/apps/jupyterhub_config.py`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/build/lab/Dockerfile` & `tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/build/lab/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/jobs/init/mysql.sh` & `tutor-jupyter-15.0.2/tutorjupyter/templates/jupyter/jobs/init/mysql.sh`

 * *Files identical despite different names*

