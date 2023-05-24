# Comparing `tmp/flirimageextractor-1.5.2.tar.gz` & `tmp/flirimageextractor-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flirimageextractor-1.5.2.tar", max compression
+gzip compressed data, was "flirimageextractor-1.5.3.tar", max compression
```

## Comparing `flirimageextractor-1.5.2.tar` & `flirimageextractor-1.5.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-05-22 00:44:41.960662 flirimageextractor-1.5.2/LICENSE
--rw-r--r--   0        0        0     3520 2023-05-22 00:44:41.960662 flirimageextractor-1.5.2/README.md
--rw-r--r--   0        0        0      114 2023-05-22 00:44:41.984663 flirimageextractor-1.5.2/flirimageextractor/__init__.py
--rw-r--r--   0        0        0     3604 2023-05-22 00:44:41.984663 flirimageextractor-1.5.2/flirimageextractor/__main__.py
--rw-r--r--   0        0        0     2135 2023-05-22 00:44:41.984663 flirimageextractor-1.5.2/flirimageextractor/dialogs.py
--rw-r--r--   0        0        0    16918 2023-05-22 00:44:41.984663 flirimageextractor-1.5.2/flirimageextractor/flir_image_extractor.py
--rw-r--r--   0        0        0     9492 2023-05-22 00:44:41.984663 flirimageextractor-1.5.2/flirimageextractor/flyr_unpack.py
--rw-r--r--   0        0        0     4140 2023-05-22 00:44:41.984663 flirimageextractor-1.5.2/flirimageextractor/processing.py
--rw-r--r--   0        0        0    42181 2023-05-22 00:44:41.988663 flirimageextractor-1.5.2/flirimageextractor/thermal_base.py
--rw-r--r--   0        0        0     9341 2023-05-22 00:44:41.988663 flirimageextractor-1.5.2/flirimageextractor/utils.py
--rw-r--r--   0        0        0     1568 2023-05-22 00:44:41.988663 flirimageextractor-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     5031 1970-01-01 00:00:00.000000 flirimageextractor-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-24 06:51:01.362078 flirimageextractor-1.5.3/LICENSE
+-rw-r--r--   0        0        0     3573 2023-05-24 06:51:01.362078 flirimageextractor-1.5.3/README.md
+-rw-r--r--   0        0        0      114 2023-05-24 06:51:01.382079 flirimageextractor-1.5.3/flirimageextractor/__init__.py
+-rw-r--r--   0        0        0     3604 2023-05-24 06:51:01.382079 flirimageextractor-1.5.3/flirimageextractor/__main__.py
+-rw-r--r--   0        0        0     2135 2023-05-24 06:51:01.382079 flirimageextractor-1.5.3/flirimageextractor/dialogs.py
+-rw-r--r--   0        0        0    16918 2023-05-24 06:51:01.382079 flirimageextractor-1.5.3/flirimageextractor/flir_image_extractor.py
+-rw-r--r--   0        0        0     9492 2023-05-24 06:51:01.382079 flirimageextractor-1.5.3/flirimageextractor/flyr_unpack.py
+-rw-r--r--   0        0        0     4140 2023-05-24 06:51:01.382079 flirimageextractor-1.5.3/flirimageextractor/processing.py
+-rw-r--r--   0        0        0    42181 2023-05-24 06:51:01.382079 flirimageextractor-1.5.3/flirimageextractor/thermal_base.py
+-rw-r--r--   0        0        0     9341 2023-05-24 06:51:01.382079 flirimageextractor-1.5.3/flirimageextractor/utils.py
+-rw-r--r--   0        0        0     1723 2023-05-24 06:51:01.382079 flirimageextractor-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     5050 1970-01-01 00:00:00.000000 flirimageextractor-1.5.3/PKG-INFO
```

### Comparing `flirimageextractor-1.5.2/LICENSE` & `flirimageextractor-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.5.2/README.md` & `flirimageextractor-1.5.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 
 ## Development
 Install the required packages using [Pipenv](https://pipenv.kennethreitz.org/en/latest/). Then run `pre-commit install` to install the pre-commit hooks. Note that this tool is intended to work on Windows as well as Unix operating systems so use os.path functions to manipulate file paths instead of string manipulation.
 
 ## Build Command for Dev (uses poetry or twine)
 - python -m build --sdist --wheel
 - poetry build
+- poetry add "packagename" --group=extras --optional
 - sphinx-build -b html docs/source docs/build (To Generate Docs)
 
 ## Credits
 
 This CLi was developed using this repos:
 - https://github.com/Nervengift/read_thermal.py
 - https://github.com/detecttechnologies/thermal_base/
```

### Comparing `flirimageextractor-1.5.2/flirimageextractor/__main__.py` & `flirimageextractor-1.5.3/flirimageextractor/__main__.py`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.5.2/flirimageextractor/dialogs.py` & `flirimageextractor-1.5.3/flirimageextractor/dialogs.py`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.5.2/flirimageextractor/flir_image_extractor.py` & `flirimageextractor-1.5.3/flirimageextractor/flir_image_extractor.py`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.5.2/flirimageextractor/flyr_unpack.py` & `flirimageextractor-1.5.3/flirimageextractor/flyr_unpack.py`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.5.2/flirimageextractor/processing.py` & `flirimageextractor-1.5.3/flirimageextractor/processing.py`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.5.2/flirimageextractor/thermal_base.py` & `flirimageextractor-1.5.3/flirimageextractor/thermal_base.py`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.5.2/flirimageextractor/utils.py` & `flirimageextractor-1.5.3/flirimageextractor/utils.py`

 * *Files identical despite different names*

### Comparing `flirimageextractor-1.5.2/pyproject.toml` & `flirimageextractor-1.5.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flirimageextractor"
-version = "1.5.2"
+version = "1.5.3"
 description = "A small tool/lib to read temperatures and original photos from FLIR® thermal camera images."
 authors = [
     "National Drones <development@nationaldrones.com>",
     "olawale williams <olawalewilliams9438@gmail.com>",
 ]
 readme = "README.md"
 maintainers = [
@@ -21,22 +21,22 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
     "Topic :: Multimedia :: Graphics :: Capture :: Digital Camera",
 ]
 
 [tool.poetry.dependencies]
+# These packages are mandatory and form the core of this package’s distribution.
 python = "^3.7"
 pillow = "9.5.0"
 matplotlib = "3.5.3"
 numpy = "1.21.1"
 sphinx = "5.3.0"
 keyring = "23.13.1"
 loguru = "0.7.0"
-wxpython = "4.2.0"
 logzero = "1.7.0"
 opencv-python = "4.5.1.48"
 requests = "2.28.2"
 tqdm = "4.65.0"
 m2r = "0.3.1"
 
 
@@ -49,10 +49,14 @@
 flir-image-extractor = 'flirimageextractor.__main__:main'
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 black = "23.3.0"
 pre-commit = "2.21.0"
 
+
+[tool.poetry.group.extras.dependencies]
+wxpython = {version = "^4.2.0", optional = true}
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `flirimageextractor-1.5.2/PKG-INFO` & `flirimageextractor-1.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flirimageextractor
-Version: 1.5.2
+Version: 1.5.3
 Summary: A small tool/lib to read temperatures and original photos from FLIR® thermal camera images.
 Home-page: https://github.com/nationaldronesau/FlirImageExtractor
 License: MIT
 Keywords: extract-images,flir,thermal,flirtools
 Author: National Drones
 Author-email: development@nationaldrones.com
 Maintainer: olawale williams
@@ -27,15 +27,14 @@
 Requires-Dist: matplotlib (==3.5.3)
 Requires-Dist: numpy (==1.21.1)
 Requires-Dist: opencv-python (==4.5.1.48)
 Requires-Dist: pillow (==9.5.0)
 Requires-Dist: requests (==2.28.2)
 Requires-Dist: sphinx (==5.3.0)
 Requires-Dist: tqdm (==4.65.0)
-Requires-Dist: wxpython (==4.2.0)
 Project-URL: Repository, https://github.com/nationaldronesau/FlirImageExtractor
 Description-Content-Type: text/markdown
 
 # Flir Image Extractor CLI
 
 The email address attached to this on PyPi may not be monitored, open issues on the [GitHub repo](https://github.com/nationaldronesau/FlirImageExtractor) to ensure a response
 
@@ -97,14 +96,15 @@
 
 ## Development
 Install the required packages using [Pipenv](https://pipenv.kennethreitz.org/en/latest/). Then run `pre-commit install` to install the pre-commit hooks. Note that this tool is intended to work on Windows as well as Unix operating systems so use os.path functions to manipulate file paths instead of string manipulation.
 
 ## Build Command for Dev (uses poetry or twine)
 - python -m build --sdist --wheel
 - poetry build
+- poetry add "packagename" --group=extras --optional
 - sphinx-build -b html docs/source docs/build (To Generate Docs)
 
 ## Credits
 
 This CLi was developed using this repos:
 - https://github.com/Nervengift/read_thermal.py
 - https://github.com/detecttechnologies/thermal_base/
```

