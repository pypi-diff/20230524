# Comparing `tmp/mystring-0.0.9.tar.gz` & `tmp/mystring-0.0.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mystring-0.0.9.tar", last modified: Sun Mar  5 22:54:59 2023, max compression
+gzip compressed data, was "mystring-0.0.90.tar", last modified: Wed May 24 02:00:25 2023, max compression
```

## Comparing `mystring-0.0.9.tar` & `mystring-0.0.90.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:54:59.363714 mystring-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-05 22:54:55.000000 mystring-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-05 22:54:59.363714 mystring-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-05 22:54:55.000000 mystring-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:54:59.363714 mystring-0.0.9/mystring/
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-03-05 22:54:55.000000 mystring-0.0.9/mystring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:54:59.363714 mystring-0.0.9/mystring.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-05 22:54:59.000000 mystring-0.0.9/mystring.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-05 22:54:59.000000 mystring-0.0.9/mystring.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 22:54:59.000000 mystring-0.0.9/mystring.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-05 22:54:59.000000 mystring-0.0.9/mystring.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-05 22:54:59.363714 mystring-0.0.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3409 2023-03-05 22:54:55.000000 mystring-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:00:25.078575 mystring-0.0.90/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-24 02:00:20.000000 mystring-0.0.90/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-24 02:00:25.078575 mystring-0.0.90/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-24 02:00:20.000000 mystring-0.0.90/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:00:25.078575 mystring-0.0.90/mystring/
+-rw-r--r--   0 runner    (1001) docker     (123)    17681 2023-05-24 02:00:20.000000 mystring-0.0.90/mystring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:00:25.078575 mystring-0.0.90/mystring.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-24 02:00:25.000000 mystring-0.0.90/mystring.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-24 02:00:25.000000 mystring-0.0.90/mystring.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 02:00:25.000000 mystring-0.0.90/mystring.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-24 02:00:25.000000 mystring-0.0.90/mystring.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-24 02:00:25.000000 mystring-0.0.90/mystring.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 02:00:25.078575 mystring-0.0.90/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3460 2023-05-24 02:00:20.000000 mystring-0.0.90/setup.py
```

### Comparing `mystring-0.0.9/LICENSE` & `mystring-0.0.90/LICENSE`

 * *Files identical despite different names*

### Comparing `mystring-0.0.9/setup.py` & `mystring-0.0.90/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.9"
+VERSION = "0.0.90"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
@@ -116,14 +116,18 @@
 	python_requires=REQUIRES_PYTHON,
 	url=URL,
 	packages=find_packages(
 		exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
 	entry_points={
 	},
 	install_requires=[
+		"pandas",
+		"seaborn",
+		"ephfile",
+		"pydbhub"
 	],
 	include_package_data=True,
 	classifiers=[
 		'Programming Language :: Python',
 		'Programming Language :: Python :: 3',
 		'Programming Language :: Python :: 3.8',
 	],
```

