# Comparing `tmp/eo-learn-1.4.1.tar.gz` & `tmp/eo-learn-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eo-learn-1.4.1.tar", last modified: Tue Mar 14 10:33:50 2023, max compression
+gzip compressed data, was "eo-learn-1.4.2.tar", last modified: Wed May 24 10:47:26 2023, max compression
```

## Comparing `eo-learn-1.4.1.tar` & `eo-learn-1.4.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:50.384002 eo-learn-1.4.1/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1745 2022-05-03 09:13:51.000000 eo-learn-1.4.1/LICENSE
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       61 2021-07-28 10:08:20.000000 eo-learn-1.4.1/MANIFEST.in
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    16023 2023-03-14 10:33:50.380002 eo-learn-1.4.1/PKG-INFO
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    13047 2023-03-14 10:22:12.000000 eo-learn-1.4.1/README.md
-drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-03-14 10:33:50.380002 eo-learn-1.4.1/eo_learn.egg-info/
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    16023 2023-03-14 10:33:50.000000 eo-learn-1.4.1/eo_learn.egg-info/PKG-INFO
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      286 2023-03-14 10:33:50.000000 eo-learn-1.4.1/eo_learn.egg-info/SOURCES.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2023-03-14 10:33:50.000000 eo-learn-1.4.1/eo_learn.egg-info/dependency_links.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2021-06-22 10:10:41.000000 eo-learn-1.4.1/eo_learn.egg-info/not-zip-safe
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      353 2023-03-14 10:33:50.000000 eo-learn-1.4.1/eo_learn.egg-info/requires.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2023-03-14 10:33:50.000000 eo-learn-1.4.1/eo_learn.egg-info/top_level.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1708 2023-03-14 10:22:12.000000 eo-learn-1.4.1/pyproject.toml
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      149 2023-03-14 10:22:12.000000 eo-learn-1.4.1/requirements-dev.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      168 2023-03-14 10:22:12.000000 eo-learn-1.4.1/requirements-docs.txt
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       38 2023-03-14 10:33:50.384002 eo-learn-1.4.1/setup.cfg
--rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2610 2023-03-14 10:22:12.000000 eo-learn-1.4.1/setup.py
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-05-24 10:47:25.998046 eo-learn-1.4.2/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1404 2023-05-24 10:35:48.000000 eo-learn-1.4.2/CREDITS.md
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     1745 2023-05-03 06:34:57.000000 eo-learn-1.4.2/LICENSE
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       80 2023-05-24 10:35:48.000000 eo-learn-1.4.2/MANIFEST.in
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    16107 2023-05-24 10:47:25.998046 eo-learn-1.4.2/PKG-INFO
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    13130 2023-05-24 10:35:48.000000 eo-learn-1.4.2/README.md
+drwxrwxr-x   0 zluksic   (1000) zluksic   (1000)        0 2023-05-24 10:47:25.994046 eo-learn-1.4.2/eo_learn.egg-info/
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)    16107 2023-05-24 10:47:25.000000 eo-learn-1.4.2/eo_learn.egg-info/PKG-INFO
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      297 2023-05-24 10:47:25.000000 eo-learn-1.4.2/eo_learn.egg-info/SOURCES.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2023-05-24 10:47:25.000000 eo-learn-1.4.2/eo_learn.egg-info/dependency_links.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2021-06-22 10:10:41.000000 eo-learn-1.4.2/eo_learn.egg-info/not-zip-safe
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      345 2023-05-24 10:47:25.000000 eo-learn-1.4.2/eo_learn.egg-info/requires.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)        1 2023-05-24 10:47:25.000000 eo-learn-1.4.2/eo_learn.egg-info/top_level.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     4129 2023-05-24 10:35:48.000000 eo-learn-1.4.2/pyproject.toml
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      141 2023-05-24 10:35:48.000000 eo-learn-1.4.2/requirements-dev.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)      168 2023-05-03 06:39:37.000000 eo-learn-1.4.2/requirements-docs.txt
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)       38 2023-05-24 10:47:25.998046 eo-learn-1.4.2/setup.cfg
+-rw-rw-r--   0 zluksic   (1000) zluksic   (1000)     2611 2023-05-24 10:35:48.000000 eo-learn-1.4.2/setup.py
```

### Comparing `eo-learn-1.4.1/LICENSE` & `eo-learn-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eo-learn-1.4.1/PKG-INFO` & `eo-learn-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eo-learn
-Version: 1.4.1
+Version: 1.4.2
 Summary: Earth observation processing framework for machine learning in Python
 Home-page: https://github.com/sentinel-hub/eo-learn
 Author: Sinergise EO research team
 Author-email: eoresearch@sinergise.com
 License: MIT
 Project-URL: Documentation, https://eo-learn.readthedocs.io
 Project-URL: Source Code, https://github.com/sentinel-hub/eo-learn
@@ -59,15 +59,15 @@
         - **`eo-learn-ml-tools`** - Various tools that can be used before or after the machine learning process.
         - **`eo-learn-visualization`** - Visualization tools for core elements of eo-learn.
         
         ## Installation
         
         ### PyPi distribution
         
-        The package requires Python version **>=3.7** . It can be installed with:
+        The package requires Python version **>=3.8** . It can be installed with:
         
         ```bash
         pip install eo-learn
         ```
         
         In order to avoid heavy package dependencies it is possible to install each subpackage separately:
         
@@ -99,15 +99,15 @@
         
         One of dependencies of `eo-learn-mask` subpackage is `lightgbm` package. On Windows it requires 64 bit Python distribution. If having problems during installation please check [LightGBM installation guide](https://lightgbm.readthedocs.io/en/latest/Installation-Guide.html).
         
         Some subpackages contain extension modules under `extra` subfolder. Those modules typically require additional package dependencies which don't get installed by default.
         
         ### Conda Forge distribution
         
-        The package requires a Python environment **>=3.7**.
+        The package requires a Python environment **>=3.8**.
         
         Thanks to the maintainers of the conda forge feedstock (@benhuff, @dcunn, @mwilson8, @oblute, @rluria14), `eo-learn` can
         be installed using `conda-forge` as follows:
         
         ```bash
         conda config --add channels conda-forge
         
@@ -156,15 +156,15 @@
         
         ## More Examples
         
         Examples and introductions to the package can be found [here](https://github.com/sentinel-hub/eo-learn/tree/master/examples). A large collection of examples is available at the [`eo-learn-examples`](https://github.com/sentinel-hub/eo-learn-examples) repository. While the examples there are not always up-to-date they can be a great source of ideas.
         
         ## Contributions
         
-        If you would like to contribute to `eo-learn`, check out our [contribution guidelines](./CONTRIBUTING.md).
+        The list of all `eo-learn` contributors can be found [here](./CONTRIBUTING.md). If you would like to contribute to `eo-learn`, please check our [contribution guidelines](./CONTRIBUTING.md).
         
         ## Blog posts and papers
         
         - [Introducing eo-learn](https://medium.com/sentinel-hub/introducing-eo-learn-ab37f2869f5c) (by Devis Peressutti)
         - [Land Cover Classification with eo-learn: Part 1 - Mastering Satellite Image Data in an Open-Source Python Environment](https://medium.com/sentinel-hub/land-cover-classification-with-eo-learn-part-1-2471e8098195) (by Matic Lubej)
         - [Land Cover Classification with eo-learn: Part 2 - Going from Data to Predictions in the Comfort of Your Laptop](https://medium.com/sentinel-hub/land-cover-classification-with-eo-learn-part-2-bd9aa86f8500) (by Matic Lubej)
         - [Land Cover Classification with eo-learn: Part 3 - Pushing Beyond the Point of “Good Enough”](https://medium.com/sentinel-hub/land-cover-classification-with-eo-learn-part-3-c62ed9ecd405) (by Matic Lubej)
@@ -218,17 +218,17 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: DEV
```

### Comparing `eo-learn-1.4.1/README.md` & `eo-learn-1.4.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 - **`eo-learn-ml-tools`** - Various tools that can be used before or after the machine learning process.
 - **`eo-learn-visualization`** - Visualization tools for core elements of eo-learn.
 
 ## Installation
 
 ### PyPi distribution
 
-The package requires Python version **>=3.7** . It can be installed with:
+The package requires Python version **>=3.8** . It can be installed with:
 
 ```bash
 pip install eo-learn
 ```
 
 In order to avoid heavy package dependencies it is possible to install each subpackage separately:
 
@@ -88,15 +88,15 @@
 
 One of dependencies of `eo-learn-mask` subpackage is `lightgbm` package. On Windows it requires 64 bit Python distribution. If having problems during installation please check [LightGBM installation guide](https://lightgbm.readthedocs.io/en/latest/Installation-Guide.html).
 
 Some subpackages contain extension modules under `extra` subfolder. Those modules typically require additional package dependencies which don't get installed by default.
 
 ### Conda Forge distribution
 
-The package requires a Python environment **>=3.7**.
+The package requires a Python environment **>=3.8**.
 
 Thanks to the maintainers of the conda forge feedstock (@benhuff, @dcunn, @mwilson8, @oblute, @rluria14), `eo-learn` can
 be installed using `conda-forge` as follows:
 
 ```bash
 conda config --add channels conda-forge
 
@@ -145,15 +145,15 @@
 
 ## More Examples
 
 Examples and introductions to the package can be found [here](https://github.com/sentinel-hub/eo-learn/tree/master/examples). A large collection of examples is available at the [`eo-learn-examples`](https://github.com/sentinel-hub/eo-learn-examples) repository. While the examples there are not always up-to-date they can be a great source of ideas.
 
 ## Contributions
 
-If you would like to contribute to `eo-learn`, check out our [contribution guidelines](./CONTRIBUTING.md).
+The list of all `eo-learn` contributors can be found [here](./CONTRIBUTING.md). If you would like to contribute to `eo-learn`, please check our [contribution guidelines](./CONTRIBUTING.md).
 
 ## Blog posts and papers
 
 - [Introducing eo-learn](https://medium.com/sentinel-hub/introducing-eo-learn-ab37f2869f5c) (by Devis Peressutti)
 - [Land Cover Classification with eo-learn: Part 1 - Mastering Satellite Image Data in an Open-Source Python Environment](https://medium.com/sentinel-hub/land-cover-classification-with-eo-learn-part-1-2471e8098195) (by Matic Lubej)
 - [Land Cover Classification with eo-learn: Part 2 - Going from Data to Predictions in the Comfort of Your Laptop](https://medium.com/sentinel-hub/land-cover-classification-with-eo-learn-part-2-bd9aa86f8500) (by Matic Lubej)
 - [Land Cover Classification with eo-learn: Part 3 - Pushing Beyond the Point of “Good Enough”](https://medium.com/sentinel-hub/land-cover-classification-with-eo-learn-part-3-c62ed9ecd405) (by Matic Lubej)
```

### Comparing `eo-learn-1.4.1/eo_learn.egg-info/PKG-INFO` & `eo-learn-1.4.2/eo_learn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eo-learn
-Version: 1.4.1
+Version: 1.4.2
 Summary: Earth observation processing framework for machine learning in Python
 Home-page: https://github.com/sentinel-hub/eo-learn
 Author: Sinergise EO research team
 Author-email: eoresearch@sinergise.com
 License: MIT
 Project-URL: Documentation, https://eo-learn.readthedocs.io
 Project-URL: Source Code, https://github.com/sentinel-hub/eo-learn
@@ -59,15 +59,15 @@
         - **`eo-learn-ml-tools`** - Various tools that can be used before or after the machine learning process.
         - **`eo-learn-visualization`** - Visualization tools for core elements of eo-learn.
         
         ## Installation
         
         ### PyPi distribution
         
-        The package requires Python version **>=3.7** . It can be installed with:
+        The package requires Python version **>=3.8** . It can be installed with:
         
         ```bash
         pip install eo-learn
         ```
         
         In order to avoid heavy package dependencies it is possible to install each subpackage separately:
         
@@ -99,15 +99,15 @@
         
         One of dependencies of `eo-learn-mask` subpackage is `lightgbm` package. On Windows it requires 64 bit Python distribution. If having problems during installation please check [LightGBM installation guide](https://lightgbm.readthedocs.io/en/latest/Installation-Guide.html).
         
         Some subpackages contain extension modules under `extra` subfolder. Those modules typically require additional package dependencies which don't get installed by default.
         
         ### Conda Forge distribution
         
-        The package requires a Python environment **>=3.7**.
+        The package requires a Python environment **>=3.8**.
         
         Thanks to the maintainers of the conda forge feedstock (@benhuff, @dcunn, @mwilson8, @oblute, @rluria14), `eo-learn` can
         be installed using `conda-forge` as follows:
         
         ```bash
         conda config --add channels conda-forge
         
@@ -156,15 +156,15 @@
         
         ## More Examples
         
         Examples and introductions to the package can be found [here](https://github.com/sentinel-hub/eo-learn/tree/master/examples). A large collection of examples is available at the [`eo-learn-examples`](https://github.com/sentinel-hub/eo-learn-examples) repository. While the examples there are not always up-to-date they can be a great source of ideas.
         
         ## Contributions
         
-        If you would like to contribute to `eo-learn`, check out our [contribution guidelines](./CONTRIBUTING.md).
+        The list of all `eo-learn` contributors can be found [here](./CONTRIBUTING.md). If you would like to contribute to `eo-learn`, please check our [contribution guidelines](./CONTRIBUTING.md).
         
         ## Blog posts and papers
         
         - [Introducing eo-learn](https://medium.com/sentinel-hub/introducing-eo-learn-ab37f2869f5c) (by Devis Peressutti)
         - [Land Cover Classification with eo-learn: Part 1 - Mastering Satellite Image Data in an Open-Source Python Environment](https://medium.com/sentinel-hub/land-cover-classification-with-eo-learn-part-1-2471e8098195) (by Matic Lubej)
         - [Land Cover Classification with eo-learn: Part 2 - Going from Data to Predictions in the Comfort of Your Laptop](https://medium.com/sentinel-hub/land-cover-classification-with-eo-learn-part-2-bd9aa86f8500) (by Matic Lubej)
         - [Land Cover Classification with eo-learn: Part 3 - Pushing Beyond the Point of “Good Enough”](https://medium.com/sentinel-hub/land-cover-classification-with-eo-learn-part-3-c62ed9ecd405) (by Matic Lubej)
@@ -218,17 +218,17 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: DEV
```

### Comparing `eo-learn-1.4.1/setup.py` & `eo-learn-1.4.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 def parse_requirements(file):
     with open(os.path.join(os.path.dirname(__file__), file)) as requirements_file:
         return sorted({line.partition("#")[0].strip() for line in requirements_file} - set(""))
 
 
 setup(
     name="eo-learn",
-    python_requires=">=3.7",
-    version="1.4.1",
+    python_requires=">=3.8",
+    version="1.4.2",
     description="Earth observation processing framework for machine learning in Python",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/sentinel-hub/eo-learn",
     project_urls={
         "Documentation": "https://eo-learn.readthedocs.io",
         "Source Code": "https://github.com/sentinel-hub/eo-learn",
@@ -34,38 +34,38 @@
     },
     author="Sinergise EO research team",
     author_email="eoresearch@sinergise.com",
     license="MIT",
     packages=[],
     include_package_data=True,
     install_requires=[
-        "eo-learn-core==1.4.1",
-        "eo-learn-coregistration==1.4.1",
-        "eo-learn-features==1.4.1",
-        "eo-learn-geometry==1.4.1",
-        "eo-learn-io==1.4.1",
-        "eo-learn-mask==1.4.1",
-        "eo-learn-ml-tools==1.4.1",
-        "eo-learn-visualization==1.4.1",
+        "eo-learn-core==1.4.2",
+        "eo-learn-coregistration==1.4.2",
+        "eo-learn-features==1.4.2",
+        "eo-learn-geometry==1.4.2",
+        "eo-learn-io==1.4.2",
+        "eo-learn-mask==1.4.2",
+        "eo-learn-ml-tools==1.4.2",
+        "eo-learn-visualization==1.4.2",
     ],
     extras_require={"DEV": parse_requirements("requirements-dev.txt")},
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Operating System :: MacOS",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: Unix",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: GIS",
         "Topic :: Scientific/Engineering :: Image Processing",
     ],
 )
```

