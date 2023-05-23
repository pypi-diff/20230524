# Comparing `tmp/PyHP3478A-0.3.tar.gz` & `tmp/PyHP3478A-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyHP3478A-0.3.tar", last modified: Wed May  3 19:03:43 2023, max compression
+gzip compressed data, was "PyHP3478A-0.4.tar", last modified: Tue May 23 22:42:00 2023, max compression
```

## Comparing `PyHP3478A-0.3.tar` & `PyHP3478A-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 19:03:43.796014 PyHP3478A-0.3/
--rw-rw-rw-   0        0        0     1091 2023-01-16 20:41:41.000000 PyHP3478A-0.3/LICENSE
--rw-rw-rw-   0        0        0      326 2023-05-03 19:03:43.795013 PyHP3478A-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 19:03:43.764041 PyHP3478A-0.3/PyHP3478A/
--rw-rw-rw-   0        0        0     6932 2023-05-03 19:03:13.000000 PyHP3478A-0.3/PyHP3478A/HP3478A.py
--rw-rw-rw-   0        0        0       28 2023-05-02 17:49:03.000000 PyHP3478A-0.3/PyHP3478A/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 19:03:43.793013 PyHP3478A-0.3/PyHP3478A.egg-info/
--rw-rw-rw-   0        0        0      326 2023-05-03 19:03:43.000000 PyHP3478A-0.3/PyHP3478A.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-05-03 19:03:43.000000 PyHP3478A-0.3/PyHP3478A.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 19:03:43.000000 PyHP3478A-0.3/PyHP3478A.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-03 19:03:43.000000 PyHP3478A-0.3/PyHP3478A.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-03 19:03:43.000000 PyHP3478A-0.3/PyHP3478A.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      128 2023-04-25 18:04:12.000000 PyHP3478A-0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-03 19:03:43.796014 PyHP3478A-0.3/setup.cfg
--rw-rw-rw-   0        0        0      849 2023-05-02 17:28:04.000000 PyHP3478A-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 22:42:00.690962 PyHP3478A-0.4/
+-rw-rw-rw-   0        0        0     1091 2023-01-16 20:41:41.000000 PyHP3478A-0.4/LICENSE
+-rw-rw-rw-   0        0        0      335 2023-05-23 22:42:00.690962 PyHP3478A-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-23 22:42:00.675957 PyHP3478A-0.4/PyHP3478A/
+-rw-rw-rw-   0        0        0     6932 2023-05-03 19:05:17.000000 PyHP3478A-0.4/PyHP3478A/HP3478A.py
+-rw-rw-rw-   0        0        0       28 2023-05-03 19:05:17.000000 PyHP3478A-0.4/PyHP3478A/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 22:42:00.689961 PyHP3478A-0.4/PyHP3478A.egg-info/
+-rw-rw-rw-   0        0        0      335 2023-05-23 22:42:00.000000 PyHP3478A-0.4/PyHP3478A.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-05-23 22:42:00.000000 PyHP3478A-0.4/PyHP3478A.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 22:42:00.000000 PyHP3478A-0.4/PyHP3478A.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-23 22:42:00.000000 PyHP3478A-0.4/PyHP3478A.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-23 22:42:00.000000 PyHP3478A-0.4/PyHP3478A.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      128 2023-05-03 19:14:02.000000 PyHP3478A-0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-23 22:42:00.690962 PyHP3478A-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      886 2023-05-23 22:41:36.000000 PyHP3478A-0.4/setup.py
```

### Comparing `PyHP3478A-0.3/LICENSE` & `PyHP3478A-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyHP3478A-0.3/PyHP3478A/HP3478A.py` & `PyHP3478A-0.4/PyHP3478A/HP3478A.py`

 * *Files identical despite different names*

### Comparing `PyHP3478A-0.3/setup.py` & `PyHP3478A-0.4/setup.py`

 * *Files 10% similar despite different names*

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
+    url=f"https://github.com/Minu-IU3IRR/{project_name}",
+    bugtrack_url = f'https://github.com/Minu-IU3IRR/{project_name}/issues',
     license='MIT',
     author='Manuel Minutello',
     description='HP3478A python interface',
     long_description=open('README.md').read(),
     install_requires=['PyAR488'],
     python_requeres = '>=3.6'
 )
```

