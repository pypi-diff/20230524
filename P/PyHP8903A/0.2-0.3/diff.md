# Comparing `tmp/PyHP8903A-0.2.tar.gz` & `tmp/PyHP8903A-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyHP8903A-0.2.tar", last modified: Tue Apr 25 18:02:21 2023, max compression
+gzip compressed data, was "PyHP8903A-0.3.tar", last modified: Tue May 23 22:39:03 2023, max compression
```

## Comparing `PyHP8903A-0.2.tar` & `PyHP8903A-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 18:02:21.853497 PyHP8903A-0.2/
--rw-rw-rw-   0        0        0     1091 2023-01-16 20:41:41.000000 PyHP8903A-0.2/LICENSE
--rw-rw-rw-   0        0        0      326 2023-04-25 18:02:21.852496 PyHP8903A-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-25 18:02:21.837960 PyHP8903A-0.2/PyHP8903A/
--rw-rw-rw-   0        0        0    12181 2023-04-25 18:02:13.000000 PyHP8903A-0.2/PyHP8903A/PyHP8903A.py
--rw-rw-rw-   0        0        0       30 2023-04-25 17:20:45.000000 PyHP8903A-0.2/PyHP8903A/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 18:02:21.851497 PyHP8903A-0.2/PyHP8903A.egg-info/
--rw-rw-rw-   0        0        0      326 2023-04-25 18:02:21.000000 PyHP8903A-0.2/PyHP8903A.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-04-25 18:02:21.000000 PyHP8903A-0.2/PyHP8903A.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 18:02:21.000000 PyHP8903A-0.2/PyHP8903A.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-25 18:02:21.000000 PyHP8903A-0.2/PyHP8903A.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-25 18:02:21.000000 PyHP8903A-0.2/PyHP8903A.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      128 2023-04-25 17:24:00.000000 PyHP8903A-0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-25 18:02:21.853497 PyHP8903A-0.2/setup.cfg
--rw-rw-rw-   0        0        0      849 2023-04-25 17:45:43.000000 PyHP8903A-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 22:39:03.297772 PyHP8903A-0.3/
+-rw-rw-rw-   0        0        0     1091 2023-01-16 20:41:41.000000 PyHP8903A-0.3/LICENSE
+-rw-rw-rw-   0        0        0      335 2023-05-23 22:39:03.297772 PyHP8903A-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-23 22:39:03.279923 PyHP8903A-0.3/PyHP8903A/
+-rw-rw-rw-   0        0        0    12181 2023-04-25 18:02:13.000000 PyHP8903A-0.3/PyHP8903A/PyHP8903A.py
+-rw-rw-rw-   0        0        0       30 2023-04-25 17:20:45.000000 PyHP8903A-0.3/PyHP8903A/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 22:39:03.296270 PyHP8903A-0.3/PyHP8903A.egg-info/
+-rw-rw-rw-   0        0        0      335 2023-05-23 22:39:03.000000 PyHP8903A-0.3/PyHP8903A.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-05-23 22:39:03.000000 PyHP8903A-0.3/PyHP8903A.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 22:39:03.000000 PyHP8903A-0.3/PyHP8903A.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-23 22:39:03.000000 PyHP8903A-0.3/PyHP8903A.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-23 22:39:03.000000 PyHP8903A-0.3/PyHP8903A.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      128 2023-04-25 17:24:00.000000 PyHP8903A-0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-23 22:39:03.298774 PyHP8903A-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      864 2023-05-23 22:38:45.000000 PyHP8903A-0.3/setup.py
```

### Comparing `PyHP8903A-0.2/LICENSE` & `PyHP8903A-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyHP8903A-0.2/PyHP8903A/PyHP8903A.py` & `PyHP8903A-0.3/PyHP8903A/PyHP8903A.py`

 * *Files identical despite different names*

### Comparing `PyHP8903A-0.2/setup.py` & `PyHP8903A-0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 setup(
     name=project_name,
     version=local_build_version,
     packages=find_packages(exclude=('_INTERNAL_build.py',
                                     '_INTERNAL_version.json',
                                     '.gitignore',
                                     'workspace.code-workspace')),
-    url="https://github.com/Minu-IU3IRR/",
-    bugtrack_url = 'https://github.com/Minu-IU3IRR/',
+    url="https://github.com/Minu-IU3IRR/PyHP8903A",
+    bugtrack_url = 'https://github.com/Minu-IU3IRR/issues',
     license='MIT',
     author='Manuel Minutello',
     description='HP8903A python interface',
     long_description=open('README.md').read(),
     install_requires=['PyAR488'],
     python_requeres = '>=3.6'
 )
```

