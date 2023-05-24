# Comparing `tmp/srsinst.rga-0.2.9.tar.gz` & `tmp/srsinst.rga-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\instrument_library\rga100\dist\.tmp-j3yq1dge\srsinst.rga-0.2.9.tar", last modified: Tue Apr 11 18:35:49 2023, max compression
+gzip compressed data, was "C:\PyPI\instrument drivers to GIT\rga100\dist\.tmp-ejzn8mjc\srsinst.rga-0.3.0.tar", last modified: Wed May 24 20:43:46 2023, max compression
```

## Comparing `srsinst.rga-0.2.9.tar` & `srsinst.rga-0.3.0.tar`

### file list

```diff
@@ -1,50 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 18:35:49.806633 srsinst.rga-0.2.9/
--rw-rw-rw-   0        0        0     1107 2022-11-01 00:07:51.000000 srsinst.rga-0.2.9/LICENSE.txt
--rw-rw-rw-   0        0        0       58 2022-12-12 16:43:23.000000 srsinst.rga-0.2.9/MANIFEST.in
--rw-rw-rw-   0        0        0     5877 2023-04-11 18:35:49.806633 srsinst.rga-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     5071 2023-02-09 19:05:11.000000 srsinst.rga-0.2.9/README.md
--rw-rw-rw-   0        0        0       42 2023-04-11 18:35:49.806633 srsinst.rga-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     2148 2023-04-07 00:41:50.000000 srsinst.rga-0.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 18:35:49.564245 srsinst.rga-0.2.9/srsinst/
-drwxrwxrwx   0        0        0        0 2023-04-11 18:35:49.654178 srsinst.rga-0.2.9/srsinst/rga/
--rw-rw-rw-   0        0        0      345 2023-04-11 18:35:07.000000 srsinst.rga-0.2.9/srsinst/rga/__init__.py
--rw-rw-rw-   0        0        0      483 2023-04-07 00:54:15.000000 srsinst.rga-0.2.9/srsinst/rga/__main__.py
--rw-rw-rw-   0        0        0    10602 2023-01-31 00:04:05.000000 srsinst.rga-0.2.9/srsinst/rga/gaslib.dat
-drwxrwxrwx   0        0        0        0 2023-04-11 18:35:49.654178 srsinst.rga-0.2.9/srsinst/rga/instruments/
--rw-rw-rw-   0        0        0       38 2023-03-16 16:49:16.000000 srsinst.rga-0.2.9/srsinst/rga/instruments/__init__.py
--rw-rw-rw-   0        0        0      729 2023-04-06 22:14:12.000000 srsinst.rga-0.2.9/srsinst/rga/instruments/get_instruments.py
-drwxrwxrwx   0        0        0        0 2023-04-11 18:35:49.674125 srsinst.rga-0.2.9/srsinst/rga/instruments/rga100/
--rw-rw-rw-   0        0        0        0 2022-12-02 00:09:02.000000 srsinst.rga-0.2.9/srsinst/rga/instruments/rga100/__init__.py
--rw-rw-rw-   0        0        0     3966 2023-04-05 21:37:14.000000 srsinst.rga-0.2.9/srsinst/rga/instruments/rga100/commands.py
--rw-rw-rw-   0        0        0     6316 2023-04-07 00:33:39.000000 srsinst.rga-0.2.9/srsinst/rga/instruments/rga100/components.py
--rw-rw-rw-   0        0        0     4391 2022-12-02 00:09:02.000000 srsinst.rga-0.2.9/srsinst/rga/instruments/rga100/errors.py
--rw-rw-rw-   0        0        0     8005 2023-04-06 22:55:39.000000 srsinst.rga-0.2.9/srsinst/rga/instruments/rga100/rga.py
--rw-rw-rw-   0        0        0    10815 2023-04-05 21:37:14.000000 srsinst.rga-0.2.9/srsinst/rga/instruments/rga100/scans.py
--rw-rw-rw-   0        0        0     9751 2023-03-23 22:12:18.000000 srsinst.rga-0.2.9/srsinst/rga/instruments/rga100/sicp.py
-drwxrwxrwx   0        0        0        0 2023-04-11 18:35:49.710541 srsinst.rga-0.2.9/srsinst/rga/plots/
--rw-rw-rw-   0        0        0        0 2023-01-24 22:29:13.000000 srsinst.rga-0.2.9/srsinst/rga/plots/__init__.py
--rw-rw-rw-   0        0        0     3490 2023-04-06 22:14:36.000000 srsinst.rga-0.2.9/srsinst/rga/plots/analogscanplot.py
--rw-rw-rw-   0        0        0     2093 2023-01-30 21:23:01.000000 srsinst.rga-0.2.9/srsinst/rga/plots/analysis.py
--rw-rw-rw-   0        0        0     3115 2023-04-06 22:16:35.000000 srsinst.rga-0.2.9/srsinst/rga/plots/basescanplot.py
--rw-rw-rw-   0        0        0     3160 2023-04-06 22:17:17.000000 srsinst.rga-0.2.9/srsinst/rga/plots/histogramscanplot.py
--rw-rw-rw-   0        0        0     7982 2023-04-06 22:17:27.000000 srsinst.rga-0.2.9/srsinst/rga/plots/timeplot.py
--rw-rw-rw-   0        0        0     2180 2023-04-05 16:04:47.000000 srsinst.rga-0.2.9/srsinst/rga/rga.taskconfig
-drwxrwxrwx   0        0        0        0 2023-04-11 18:35:49.806633 srsinst.rga-0.2.9/srsinst/rga/tasks/
--rw-rw-rw-   0        0        0        0 2022-12-02 00:09:02.000000 srsinst.rga-0.2.9/srsinst/rga/tasks/__init__.py
--rw-rw-rw-   0        0        0     3870 2023-04-11 00:37:02.000000 srsinst.rga-0.2.9/srsinst/rga/tasks/analogscantask.py
--rw-rw-rw-   0        0        0     2436 2023-04-06 22:17:56.000000 srsinst.rga-0.2.9/srsinst/rga/tasks/cemcontroltask.py
--rw-rw-rw-   0        0        0     8541 2023-04-06 22:18:09.000000 srsinst.rga-0.2.9/srsinst/rga/tasks/cemgaintask.py
--rw-rw-rw-   0        0        0     9453 2023-04-11 00:37:45.000000 srsinst.rga-0.2.9/srsinst/rga/tasks/compositionanalysistask.py
--rw-rw-rw-   0        0        0     5104 2023-04-11 00:38:06.000000 srsinst.rga-0.2.9/srsinst/rga/tasks/derivedpvstscantask.py
--rw-rw-rw-   0        0        0     2632 2023-04-06 22:18:58.000000 srsinst.rga-0.2.9/srsinst/rga/tasks/filamentcontroltask.py
--rw-rw-rw-   0        0        0     3642 2023-04-11 00:38:30.000000 srsinst.rga-0.2.9/srsinst/rga/tasks/histogramscantask.py
--rw-rw-rw-   0        0        0    11350 2023-04-11 00:39:33.000000 srsinst.rga-0.2.9/srsinst/rga/tasks/peaktuningtask.py
--rw-rw-rw-   0        0        0     2438 2023-04-11 00:39:52.000000 srsinst.rga-0.2.9/srsinst/rga/tasks/pvstscantask.py
--rw-rw-rw-   0        0        0     1968 2023-04-06 22:19:58.000000 srsinst.rga-0.2.9/srsinst/rga/tasks/searchlan.py
-drwxrwxrwx   0        0        0        0 2023-04-11 18:35:49.634140 srsinst.rga-0.2.9/srsinst.rga.egg-info/
--rw-rw-rw-   0        0        0     5877 2023-04-11 18:35:49.000000 srsinst.rga-0.2.9/srsinst.rga.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1331 2023-04-11 18:35:49.000000 srsinst.rga-0.2.9/srsinst.rga.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 18:35:49.000000 srsinst.rga-0.2.9/srsinst.rga.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-11 18:35:49.000000 srsinst.rga-0.2.9/srsinst.rga.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-04-11 18:35:49.000000 srsinst.rga-0.2.9/srsinst.rga.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 18:35:49.000000 srsinst.rga-0.2.9/srsinst.rga.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 20:43:46.766221 srsinst.rga-0.3.0/
+-rw-rw-rw-   0        0        0     1356 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/.gitignore
+-rw-rw-rw-   0        0        0     1113 2023-05-19 17:56:22.000000 srsinst.rga-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     6402 2023-05-24 20:43:46.766221 srsinst.rga-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5623 2023-05-19 18:09:46.000000 srsinst.rga-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 20:43:46.702127 srsinst.rga-0.3.0/docs/
+drwxrwxrwx   0        0        0        0 2023-05-24 20:43:46.702127 srsinst.rga-0.3.0/docs/_static/
+drwxrwxrwx   0        0        0        0 2023-05-24 20:43:46.736271 srsinst.rga-0.3.0/docs/_static/image/
+-rw-rw-rw-   0        0        0   115947 2023-05-19 17:56:22.000000 srsinst.rga-0.3.0/docs/_static/image/derived-pvst-plot-screenshot.png
+-rw-rw-rw-   0        0        0     1164 2023-05-16 00:38:30.000000 srsinst.rga-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 20:43:46.766221 srsinst.rga-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-05-19 17:56:22.000000 srsinst.rga-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 20:43:46.712095 srsinst.rga-0.3.0/srsinst/
+drwxrwxrwx   0        0        0        0 2023-05-24 20:43:46.746266 srsinst.rga-0.3.0/srsinst/rga/
+-rw-rw-rw-   0        0        0      345 2023-05-24 20:36:23.000000 srsinst.rga-0.3.0/srsinst/rga/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-05-19 21:11:26.000000 srsinst.rga-0.3.0/srsinst/rga/__main__.py
+-rw-rw-rw-   0        0        0    10600 2023-05-19 21:11:26.000000 srsinst.rga-0.3.0/srsinst/rga/gaslib.dat
+drwxrwxrwx   0        0        0        0 2023-05-24 20:43:46.746266 srsinst.rga-0.3.0/srsinst/rga/instruments/
+-rw-rw-rw-   0        0        0       38 2023-05-19 21:11:26.000000 srsinst.rga-0.3.0/srsinst/rga/instruments/__init__.py
+-rw-rw-rw-   0        0        0      872 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/instruments/get_instruments.py
+drwxrwxrwx   0        0        0        0 2023-05-24 20:43:46.756254 srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/
+-rw-rw-rw-   0        0        0        0 2023-05-19 21:11:26.000000 srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/__init__.py
+-rw-rw-rw-   0        0        0     5249 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/commands.py
+-rw-rw-rw-   0        0        0     7009 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/components.py
+-rw-rw-rw-   0        0        0     4510 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/errors.py
+-rw-rw-rw-   0        0        0     8589 2023-05-23 22:01:40.000000 srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/rga.py
+-rw-rw-rw-   0        0        0    18656 2023-05-19 21:11:26.000000 srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/rga_commands.json
+-rw-rw-rw-   0        0        0    11501 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/scans.py
+-rw-rw-rw-   0        0        0     9872 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/sicp.py
+drwxrwxrwx   0        0        0        0 2023-05-24 20:43:46.756254 srsinst.rga-0.3.0/srsinst/rga/plots/
+-rw-rw-rw-   0        0        0        0 2023-05-19 21:11:26.000000 srsinst.rga-0.3.0/srsinst/rga/plots/__init__.py
+-rw-rw-rw-   0        0        0     3611 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/plots/analogscanplot.py
+-rw-rw-rw-   0        0        0     3443 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/plots/analysis.py
+-rw-rw-rw-   0        0        0     3234 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/plots/basescanplot.py
+-rw-rw-rw-   0        0        0     3279 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/plots/histogramscanplot.py
+-rw-rw-rw-   0        0        0     8102 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/plots/timeplot.py
+-rw-rw-rw-   0        0        0     2228 2023-05-22 17:53:19.000000 srsinst.rga-0.3.0/srsinst/rga/rga.taskconfig
+drwxrwxrwx   0        0        0        0 2023-05-24 20:43:46.766221 srsinst.rga-0.3.0/srsinst/rga/tasks/
+-rw-rw-rw-   0        0        0        0 2023-05-19 21:11:26.000000 srsinst.rga-0.3.0/srsinst/rga/tasks/__init__.py
+-rw-rw-rw-   0        0        0     3999 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/tasks/analogscantask.py
+-rw-rw-rw-   0        0        0     2543 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/tasks/cemcontroltask.py
+-rw-rw-rw-   0        0        0     9319 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/tasks/cemgaintask.py
+-rw-rw-rw-   0        0        0     9586 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/tasks/compositionanalysistask.py
+-rw-rw-rw-   0        0        0     5243 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/tasks/derivedpvstscantask.py
+-rw-rw-rw-   0        0        0     2751 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/tasks/filamentcontroltask.py
+-rw-rw-rw-   0        0        0     3685 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/tasks/histogramscantask.py
+-rw-rw-rw-   0        0        0    11440 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/tasks/peaktuningtask.py
+-rw-rw-rw-   0        0        0     2557 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/tasks/pvstscantask.py
+-rw-rw-rw-   0        0        0     2087 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/tasks/searchlan.py
+drwxrwxrwx   0        0        0        0 2023-05-24 20:43:46.746266 srsinst.rga-0.3.0/srsinst.rga.egg-info/
+-rw-rw-rw-   0        0        0     6402 2023-05-24 20:43:46.000000 srsinst.rga-0.3.0/srsinst.rga.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1432 2023-05-24 20:43:46.000000 srsinst.rga-0.3.0/srsinst.rga.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 20:43:46.000000 srsinst.rga-0.3.0/srsinst.rga.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-24 20:43:46.000000 srsinst.rga-0.3.0/srsinst.rga.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       68 2023-05-24 20:43:46.000000 srsinst.rga-0.3.0/srsinst.rga.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-24 20:43:46.000000 srsinst.rga-0.3.0/srsinst.rga.egg-info/top_level.txt
```

### Comparing `srsinst.rga-0.2.9/LICENSE.txt` & `srsinst.rga-0.3.0/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-
 The MIT License
 
-Copyright (c) 2022 Stanford Research Systems
+Copyright (c) 2022, 2023 Stanford Research Systems
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-of the Software, and to permit persons to whom the Software is furnished to do
-so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `srsinst.rga-0.2.9/PKG-INFO` & `srsinst.rga-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 Metadata-Version: 2.1
 Name: srsinst.rga
-Version: 0.2.9
-Summary: Instrument library and GUI application for SRS RGA
+Version: 0.3.0
+Summary: Instrument driver package for Residual Gas Analyzers (RGA) from Stanford Research Systems
 Author: Chulhoon Kim
 License: MIT license
 Keywords: RGA,residual gas analyzer,SRS,Stanford Research Systems
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Chemistry
-Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: full
-License-File: LICENSE.txt
+License-File: LICENSE
 
 # `srsinst.rga`
 
-`srsinst.rga` is a Python GUI application to control and acquire mass spectra from 
+`srsinst.rga` provides Python instrument classes to control and acquire mass spectra from 
 [Stanford Research Systems (SRS) Residual Gas Analyzers (RGA)](https://thinksrs.com/products/rga.html).
-To use this package safely, you need to be familiar with SRS RGA. You can download the
-[manual](https://thinksrs.com/downloads/pdfs/manuals/RGAm.pdf) for your reference.
+It also provides tasks running in GUI environment based on 
+[srsgui](https://thinksrs.github.io/srsgui/).  
+To operate SRS RGA with this package safely, you need to be familiar with SRS RGA. 
+For detailed information, refer to the 
+[manual](https://thinksrs.com/downloads/pdfs/manuals/RGAm.pdf).
+
+![screenshot](https://github.com/thinkSRS/srsinst.rga/blob/main/docs/_static/image/derived-pvst-plot-screenshot.png " ")
 
 ## Installation
-You should have a working Python with `pip` (Python package installer) installed. If you don't,
+You need a working Python with `pip` (Python package installer) installed. If you don't,
 [install Python 3](https://realpython.com/installing-python/) to your system.
 
-To install `srsinst.rga` as an instrument driver , use Python package installer `pip` from the command line.
+To install `srsinst.rga` as an instrument driver only, use Python package installer `pip` 
+from the command line.
 
     python -m pip install srsinst.rga
 
-To use its full GUI application, create a virtual environment and install:
+To use its full GUI application, create a virtual environment, if necessary,
+and install with *[full]* option:
+
+    # To create a simple virtual environment (Optional)
+    python -m venv venv
+    venv\scripts\activate
 
+    # To install full GUI application 
     python -m pip install srsinst.rga[full]
 
 
 ## Run `srsinst.rga` as GUI application
 If the Python Scripts directory is in PATH environment variable,
 Start the application by typing from the command line:
 
@@ -51,38 +62,39 @@
 
 It will start the GUI application.
 
 Connect to an RGA from the Instruments menu.
 Select a task from the Task menu.
 Press the green arrow to run the selected task. 
 
-You can write your own task or modify an existing one and run it from the application, too.
+You can write your own task or modify an existing one and run it from the application.
+Refer to [srsgui](https://thinksrs.github.io/srsgui/) documentation for details.
 
 ## Use `srsinst.rga` as instrument driver
 * Start the Python program, or an editor of your choice to write a Python script.
-* import the **RGA** class from `rga` package.
-* Instantiate **RGA** to connect to an SRS RGA.
+* import the **RGA100** class from `srsinst.rga` package.
+* Instantiate **RGA100** to connect to an SRS RGA.
 
-        from srsinst.rga import RGA100 as RGA
+        from srsinst.rga import RGA100
 
         # for TCPIP communication
         ip_address = '192.168.1.100'
         user_id = 'admin'
         password = 'admin'
 
-        rga1 = RGA('tcpip', ip_address, user_id, password)
+        rga1 = RGA100('tcpip', ip_address, user_id, password)
 
         # for serial communication
         # Baud rate for RGA100 is fixed to 28800
         # rga2 = RGA('serial', /dev/ttyUSB0', 28800)  # for Linux serial communication
 
         rga2 = RGA('serial', 'COM3', 28800)  # for Windows serial communication
 
-        # or initialize a Rga instance without connection, then connect.
-        rga3 = RGA()
+        # or initialize a RGA100 instance without connection, then connect.
+        rga3 = RGA100()
         rga3.connect('tcpip', ip_address, user_id, password)
 
 * Control ionizer parameters.
 
         # Set ionizer values
         rga1.ionizer.electron_energy = 70
         rga1.ionizer.ion_energy = 12
@@ -100,23 +112,23 @@
         # or
         a, b, c = rga1.ionizer.get_parameters()
 
 
         # Set the filament emsission current.
 
         rga1.ionizer.emission_current = 1.0  # in the unit of mA
-        rga1.ionizer.emission_current = 0.0  # It will turn off the filament
+        rga1.ionizer.emission_current = 0.0  # It will turn off the filament.
 
         # or
 
-        rga1.filament.turn_on(1.0)  # emission cureent in the unit of mA
+        rga1.filament.turn_on()  # Turn on with the default emission cureent of 1 mA.
         rga1.filament.turn_off()
 
 
-        # Get the emission current to check
+        # Read back the emission current
         a = rga1.ionizer.emission_current
 
 * Control detector parameters.
 
         # Set CEM voltage to the calibrated CEM voltage, or 0 to turn off
         rga1.cem.voltage = rga1.cem.stored_voltage
         rga1.cem.voltage = 0
@@ -143,15 +155,15 @@
         mi, mf, nf, sa = rga1.scan.get_parameters()
 
 * Run an analog scan.
 
         analog_spectrum  = rga1.scan.get_analog_scan()
         spectrum_in_torr = rga1.scan.get_partial_pressure_corrected_spectrum(analog_spectrum)
 
-        # Get the mathing mass axis with the spectrum
+        # Get the matching mass axis with the spectrum
         analog_mass_axis = rga1.scan.get_mass_axis(True)  # is it for analog scan? Yes.
 
 * Run a histogram scan.
 
         histogram_spectrum  = rga1.scan.get_histogram_scan()
 
         # Get the matching mass axis with the spectrum
```

### Comparing `srsinst.rga-0.2.9/README.md` & `srsinst.rga-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 # `srsinst.rga`
 
-`srsinst.rga` is a Python GUI application to control and acquire mass spectra from 
+`srsinst.rga` provides Python instrument classes to control and acquire mass spectra from 
 [Stanford Research Systems (SRS) Residual Gas Analyzers (RGA)](https://thinksrs.com/products/rga.html).
-To use this package safely, you need to be familiar with SRS RGA. You can download the
-[manual](https://thinksrs.com/downloads/pdfs/manuals/RGAm.pdf) for your reference.
+It also provides tasks running in GUI environment based on 
+[srsgui](https://thinksrs.github.io/srsgui/).  
+To operate SRS RGA with this package safely, you need to be familiar with SRS RGA. 
+For detailed information, refer to the 
+[manual](https://thinksrs.com/downloads/pdfs/manuals/RGAm.pdf).
+
+![screenshot](https://github.com/thinkSRS/srsinst.rga/blob/main/docs/_static/image/derived-pvst-plot-screenshot.png " ")
 
 ## Installation
-You should have a working Python with `pip` (Python package installer) installed. If you don't,
+You need a working Python with `pip` (Python package installer) installed. If you don't,
 [install Python 3](https://realpython.com/installing-python/) to your system.
 
-To install `srsinst.rga` as an instrument driver , use Python package installer `pip` from the command line.
+To install `srsinst.rga` as an instrument driver only, use Python package installer `pip` 
+from the command line.
 
     python -m pip install srsinst.rga
 
-To use its full GUI application, create a virtual environment and install:
+To use its full GUI application, create a virtual environment, if necessary,
+and install with *[full]* option:
+
+    # To create a simple virtual environment (Optional)
+    python -m venv venv
+    venv\scripts\activate
 
+    # To install full GUI application 
     python -m pip install srsinst.rga[full]
 
 
 ## Run `srsinst.rga` as GUI application
 If the Python Scripts directory is in PATH environment variable,
 Start the application by typing from the command line:
 
@@ -30,38 +42,39 @@
 
 It will start the GUI application.
 
 Connect to an RGA from the Instruments menu.
 Select a task from the Task menu.
 Press the green arrow to run the selected task. 
 
-You can write your own task or modify an existing one and run it from the application, too.
+You can write your own task or modify an existing one and run it from the application.
+Refer to [srsgui](https://thinksrs.github.io/srsgui/) documentation for details.
 
 ## Use `srsinst.rga` as instrument driver
 * Start the Python program, or an editor of your choice to write a Python script.
-* import the **RGA** class from `rga` package.
-* Instantiate **RGA** to connect to an SRS RGA.
+* import the **RGA100** class from `srsinst.rga` package.
+* Instantiate **RGA100** to connect to an SRS RGA.
 
-        from srsinst.rga import RGA100 as RGA
+        from srsinst.rga import RGA100
 
         # for TCPIP communication
         ip_address = '192.168.1.100'
         user_id = 'admin'
         password = 'admin'
 
-        rga1 = RGA('tcpip', ip_address, user_id, password)
+        rga1 = RGA100('tcpip', ip_address, user_id, password)
 
         # for serial communication
         # Baud rate for RGA100 is fixed to 28800
         # rga2 = RGA('serial', /dev/ttyUSB0', 28800)  # for Linux serial communication
 
         rga2 = RGA('serial', 'COM3', 28800)  # for Windows serial communication
 
-        # or initialize a Rga instance without connection, then connect.
-        rga3 = RGA()
+        # or initialize a RGA100 instance without connection, then connect.
+        rga3 = RGA100()
         rga3.connect('tcpip', ip_address, user_id, password)
 
 * Control ionizer parameters.
 
         # Set ionizer values
         rga1.ionizer.electron_energy = 70
         rga1.ionizer.ion_energy = 12
@@ -79,23 +92,23 @@
         # or
         a, b, c = rga1.ionizer.get_parameters()
 
 
         # Set the filament emsission current.
 
         rga1.ionizer.emission_current = 1.0  # in the unit of mA
-        rga1.ionizer.emission_current = 0.0  # It will turn off the filament
+        rga1.ionizer.emission_current = 0.0  # It will turn off the filament.
 
         # or
 
-        rga1.filament.turn_on(1.0)  # emission cureent in the unit of mA
+        rga1.filament.turn_on()  # Turn on with the default emission cureent of 1 mA.
         rga1.filament.turn_off()
 
 
-        # Get the emission current to check
+        # Read back the emission current
         a = rga1.ionizer.emission_current
 
 * Control detector parameters.
 
         # Set CEM voltage to the calibrated CEM voltage, or 0 to turn off
         rga1.cem.voltage = rga1.cem.stored_voltage
         rga1.cem.voltage = 0
@@ -122,15 +135,15 @@
         mi, mf, nf, sa = rga1.scan.get_parameters()
 
 * Run an analog scan.
 
         analog_spectrum  = rga1.scan.get_analog_scan()
         spectrum_in_torr = rga1.scan.get_partial_pressure_corrected_spectrum(analog_spectrum)
 
-        # Get the mathing mass axis with the spectrum
+        # Get the matching mass axis with the spectrum
         analog_mass_axis = rga1.scan.get_mass_axis(True)  # is it for analog scan? Yes.
 
 * Run a histogram scan.
 
         histogram_spectrum  = rga1.scan.get_histogram_scan()
 
         # Get the matching mass axis with the spectrum
```

### Comparing `srsinst.rga-0.2.9/srsinst/rga/gaslib.dat` & `srsinst.rga-0.3.0/srsinst/rga/gaslib.dat`

 * *Files 1% similar despite different names*

```diff
@@ -223,27 +223,27 @@
  20	22	21	0	0	0	0	0	0	0	
  100.0	9.7	0.3	0.0	0.0	0.0	0.0	0.0	0.0	0.0
 "Nitrobenzene"  1.0   1.0
  77	51	123	50	93	65	30	28	39	74	
  100.0	85.0	39.0	31.0	16.0	16.0	9.2	9.2	7.8	7.8
 "Nitrogen"  1.0   1.0
  28	14	29	0	0	0	0	0	0	0	
- 100.0	9.0	0.8	0.0	0.0	0.0	0.0	0.0	0.0	0.0
+ 100.0	6.0	0.8	0.0	0.0	0.0	0.0	0.0	0.0	0.0
 "o-Xylene"  1.0   1.0
  91	106	39	105	51	77	27	65	78	79	
  100.0	40.0	20.5	17.5	17.0	14.5	11.5	10.0	8.5	8.5
 "o-Cresol"  1.0   1.0
  108	107	77	79	39	90	51	27	0	0	
  100.0	75.0	34.0	33.0	28.0	25.0	21.0	20.0	0.0	0.0
 "Octane"  1.0   1.0
  43	57	85	41	71	29	56	42	0	0	
  100.0	30.0	25.0	25.0	19.0	17.0	14.0	10.0	0.0	0.0
 "Oxygen"  1.0   1.0
  32	16	34	33	0	0	0	0	0	0	
- 100.0	11.4	0.4	0.1	0.0	0.0	0.0	0.0	0.0	0.0
+ 100.0	7.0	0.4	0.1	0.0	0.0	0.0	0.0	0.0	0.0
 "p-Xylene"  1.0   1.0
  91	106	105	39	51	77	27	50	0	0	
  100.0	62.0	30.0	16.0	16.0	13.0	11.0	7.0	0.0	0.0
 "p-Cresol"  1.0   1.0
  107	108	77	79	51	39	27	53	50	52	
  100.0	91.0	28.0	21.0	19.0	17.0	17.0	15.0	12.0	10.0
 "Pentane"  1.0   1.0
@@ -295,11 +295,11 @@
  91	92	39	65	51	63	50	27	93	90	
  100.0	69.0	20.0	15.0	11.0	10.0	7.5	6.5	5.5	5.0
 "Turbopump Oil"  1.0   1.0
  43	57	41	55	71	69	0	0	0	0	
  100.0	88.0	76.0	73.0	52.0	49.0	0.0	0.0	0.0	0.0
 "Water"  1.0   1.0
  18	17	16	20	19	0	0	0	0	0	
- 100.0	32.0	19.0	0.3	0.1	0.0	0.0	0.0	0.0	0.0
+ 100.0	24.0	2.0	0.3	0.1	0.0	0.0	0.0	0.0	0.0
 "Xenon"  1.0   1.0
  132	129	131	134	136	130	128	124	126	66	
  100.0	98.3	78.8	38.8	33.0	15.2	7.1	0.4	0.3	15.0
```

### Comparing `srsinst.rga-0.2.9/srsinst/rga/instruments/get_instruments.py` & `srsinst.rga-0.3.0/srsinst/rga/instruments/get_instruments.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,27 @@
+##! 
+##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
+
 import logging
 from srsgui import Task
 from srsinst.rga.instruments.rga100.rga import RGA100
 
 logger = logging.getLogger(__name__)
 
 
 def get_rga(task: Task, name=None) -> RGA100:
     """
-    Instead of using task.get_instrument() directly in a Task subclass,
-    Defining a wrapper function with a instrument return type will help
-    a context-sensitive editors display  attributes available
-    for the instrument class.
+    Instead of using Task.get_instrument() in a Task subclass directly,
+    Defining a wrapper function that returns an instrument of
+    a specific class will help a context-sensitive editors
+    to display  attributes available for the instrument class.
     """
+
     if name is None:
         inst = list(task.inst_dict.values())[0]
     else:
         inst = task.get_instrument(name)
 
     if issubclass(type(inst), RGA100):
         return inst
```

### Comparing `srsinst.rga-0.2.9/srsinst/rga/instruments/rga100/commands.py` & `srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/commands.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,26 @@
+##! 
+##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
+
+"""
+RGA100 remote commands allow no space between a set command and the following parameter.
+Following NSCommand (no space command) classes are derived from
+`Command classes <https://thinksrs.github.io/srsgui/srsgui.inst.html#module-srsgui.inst.commands>`_
+in `srsgui <https://thinksrs.github.io/srsgui/index.html>`_
+to meet the requirement.
+"""
 
 from srsgui.inst.exceptions import InstCommunicationError, InstSetError, InstQueryError
 
 from srsgui.inst.commands import IntCommand, IntGetCommand, FloatCommand, \
                                  BoolSetCommand
 
-# RGA100 does not allow space between a set command and the following parameter.
+# Set command format with no space between a command and the following parameter.
 SetCommandFormat = '{}{}'
 
 
 class IntNSCommand(IntCommand):
     _set_command_format = SetCommandFormat
 
 
@@ -44,36 +56,56 @@
         except InstCommunicationError:
             raise InstSetError('Error during setting: CMD:{} '.format(set_string))
         except ValueError:
             raise InstSetError('Error during conversion: CMD: {}'
                                .format(set_string))
 
 
-class RgaFloatCommand(RgaIntCommand):
+class RgaFloatCommand(FloatNSCommand):
     """
     Descriptor for an RGA100 remote command to
     **set** and **query** a **float** value.
     Setting a value returns a status byte, which is stored as last_set_status
     """
 
-    def __init__(self, remote_command_name):
-        super().__init__(remote_command_name)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self._get_convert_function = float
         self._set_convert_function = float
 
+    def __set__(self, instance, value):
+        if instance is None:
+            return
+
+        set_string = self.remote_command
+        try:
+
+            if callable(self._set_convert_function):
+                converted_value = self._set_convert_function(value)
+            else:
+                converted_value = value
+            set_string = self._set_command_format.format(self.remote_command, converted_value)
+            reply = int(instance.comm.query_text_with_long_timeout(set_string))
+            instance.last_set_status = reply
+        except InstCommunicationError:
+            raise InstSetError('Error during setting: CMD:{} '.format(set_string))
+        except ValueError:
+            raise InstSetError('Error during conversion: CMD: {}'
+                               .format(set_string))
+
 
 class RgaIonEnergyCommand(RgaIntCommand):
     """
     Descriptor for a RGA100 remote command
     to  **set**  and **query** ion energy. only 8 and 12 eV are allowed.
     Setting a value returns a status byte, which is stored as last_set_status
    """
 
-    def __init__(self, remote_command_name):
-        super().__init__(remote_command_name)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self._get_convert_function = lambda a: 12 if int(a) != 0 else 8
         self._set_convert_function = lambda a: 1 if a >= 12 else 0
 
 
 class RgaTotalPressureCommand(IntGetCommand):
     """
     Descriptor for a RGA100 remote command to **query** total pressure value
@@ -100,11 +132,11 @@
     """
     Descriptor for a RGA100 remote command
     to  **set**  and **query** Cem gain stored.
     The raw data is stored as the gain divided by 1000.
     And the descriptor converts back to the original value
    """
 
-    def __init__(self, remote_command_name):
-        super().__init__(remote_command_name)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self._get_convert_function = lambda a: float(a) * 1000.0
         self._set_convert_function = lambda a: float(a) / 1000.0
```

### Comparing `srsinst.rga-0.2.9/srsinst/rga/instruments/rga100/components.py` & `srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/components.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,37 @@
+##! 
+##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
 
 from srsgui import InstException
 from srsgui import Component
 from srsgui import GetCommand, IntGetCommand
 
 from .commands import FloatNSCommand, BoolSetNSCommand,\
                       RgaIntCommand, RgaFloatCommand, \
                       RgaIonEnergyCommand, RgaTotalPressureCommand, \
                       RgaStoredCEMGainCommand
 from .errors import query_errors, fetch_error_descriptions
 
 
 class Ionizer(Component):
-    electron_energy = RgaIntCommand('EE')
-    ion_energy = RgaIonEnergyCommand('IE')
-    focus_voltage = RgaIntCommand('VF')
-    emission_current = RgaFloatCommand('FL')
+    electron_energy = RgaIntCommand('EE', 'eV', 25, 105, 1, 70)
+    ion_energy = RgaIonEnergyCommand('IE', 'eV', 8, 12, 4, 12)
+    focus_voltage = RgaIntCommand('VF', 'V', 0, 150, 1, 90)
+    emission_current = RgaFloatCommand('FL', 'mA', 0.0, 3.5, 0.01, 2, 1.0)
     """
     For typical operation, set emission current to 1 (mA).
     When the emission current is set to 0, the filament will be turned off
     """
 
     last_set_status = 0
     """
     RgaCommand returns status byte with set operations
-    heck this value after ionizer set commands 
+    Check this variable after ionizer set commands 
     """
 
     def get_parameters(self):
         """
         Get electron energy, ion energy, focus voltage setting values
 
         Returns
@@ -63,23 +67,17 @@
         return self.last_set_status
 
 
 class Filament(Component):
     last_set_status = 0
     """
     RgaCommand returns status byte with set operations
-    heck this value after ionizer set commands 
+    Check this value after ionizer set commands 
     """
 
-    def start_degas(self, degas_minute=3):
-        """
-        Start degas. Subsequent commands are blocked until the degas is over for RGA100.
-        """
-        self.comm.query_text_with_long_timeout('DG{}'.format(degas_minute), degas_minute * 65)
-
     def turn_on(self, target_emission_current=1.0):
         """
         Turn on filament to the target emission current
 
         Parameters
         -----------
             target_emission_current : int, optional
@@ -96,81 +94,97 @@
     def turn_off(self):
         """
         Turn off the filament
         """
         self._parent.ionizer.emission_current = 0.0
         return self.last_set_status
 
+    def start_degas(self, degas_minute=3):
+        """
+        Start degas. Subsequent commands are blocked until the degas is over for RGA100.
+        """
+        print('Degas starting')
+        self.comm.query_text_with_long_timeout('DG{}'.format(degas_minute), degas_minute * 65)
+        print('Degas finished')
+
+    allow_run_button = [turn_on, turn_off]
+
 
 class CEM(Component):
-    stored_gain = RgaStoredCEMGainCommand('MG')
+    voltage = RgaIntCommand('HV', 'V', 0, 2290, 1, 0)
+    stored_voltage = FloatNSCommand('MV', 'V', 0, 2290, 1, 0)
+
+    stored_gain = RgaStoredCEMGainCommand('MG', '', 0, 2000000, 1, 3, 0)
     """ 
     Stored CEM gain. Underlying remote command 'MG' returns 
     the gain divided by 1000. This descriptor generates
     the original value,  1000 times of the raw remote command value.    
      """
 
-    stored_voltage = FloatNSCommand('MV')
-    voltage = RgaIntCommand('HV')
-
     def turn_on(self):
         """
         Set CEM HV to the stored CEM voltage
         """
         self.voltage = self.stored_voltage
 
     def turn_off(self):
         """
         Set CEM HV to the stored CEM voltage
         """
         self.voltage = 0
 
+    allow_run_button = [turn_on, turn_off]
+
 
 class Pressure(Component):
-    partial_pressure_sensitivity = FloatNSCommand('SP')
+    partial_pressure_sensitivity = FloatNSCommand('SP', 'mA/Torr', 0.0, 10.0, 0.001, 2, 0.1)
     """
     Partial pressure sensitivity is used to convert a spectrum 
     in current unit to partial pressure unit. 
     The partial pressure sensitivity in the unit of mA/Torr        
     """
 
-    total_pressure_sensitivity = FloatNSCommand('ST')
+    total_pressure_sensitivity = FloatNSCommand('ST', 'mA/Torr', 0.0, 100.0, 0.001, 2, 0.01)
     """
     Total pressure sensitivity is used to convert total pressure measured   
     in current unit to pressure unit. 
     The total pressure sensitivity in the unit of mA/Torr
     """
 
     total_pressure_enable = BoolSetNSCommand('TP')
-    total_pressure = RgaTotalPressureCommand('TP')
+    total_pressure = RgaTotalPressureCommand('TP', 'x 10^-16 A')
     """
     Total pressure measured in  ion current in 0.1 fA 
     """
 
     def get_total_pressure_in_torr(self):
         factor = 1e-13 / self.total_pressure_sensitivity
         if self._parent.cem.voltage > 10:
             factor /= self._parent.cem.stored_gain
         return self.total_pressure * factor
 
     def get_partial_pressure_sensitivity_in_torr(self):
+        """
+        Sensitivity factor is multiplied to a raw ion current value (in 1e-16 A unit)
+        to calculate the partial pressure in Torr
+        """
         factor = 1e-13 / self.partial_pressure_sensitivity
         if self._parent.cem.voltage > 10:
             factor /= self._parent.cem.stored_gain
         return factor
 
 
 class QMF(Component):
     class RF(Component):
-        offset = FloatNSCommand('RI')
         slope = FloatNSCommand('RS')
+        offset = FloatNSCommand('RI')
 
     class DC(Component):
-        offset = FloatNSCommand('DI')
         slope = FloatNSCommand('DS')
+        offset = FloatNSCommand('DI')
 
     def __init__(self, parent):
         super().__init__(parent)
         self.rf = QMF.RF(self)
         self.dc = QMF.DC(self)
```

### Comparing `srsinst.rga-0.2.9/srsinst/rga/instruments/rga100/errors.py` & `srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+##! 
+##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
 
 """
 Module to handle RGA100 error status
 """
 
 BIT7 = 1 << 7
 BIT6 = 1 << 6
```

### Comparing `srsinst.rga-0.2.9/srsinst/rga/instruments/rga100/rga.py` & `srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/rga.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,501 +1,537 @@
-00000000: 0d0a 230d 0a23 203a 636f 7079 7269 6768  ..#..# :copyrigh
-00000010: 743a 2032 3032 3220 2053 7461 6e66 6f72  t: 2022  Stanfor
-00000020: 6420 5265 7365 6172 6368 2053 7973 7465  d Research Syste
-00000030: 6d73 2e0d 0a23 203a 6c69 6365 6e73 653a  ms...# :license:
-00000040: 204d 4954 2c20 7365 6520 4c49 4345 4e53   MIT, see LICENS
-00000050: 4520 666f 7220 6d6f 7265 2064 6574 6169  E for more detai
-00000060: 6c73 2e0d 0a23 0d0a 0d0a 2222 220d 0a4d  ls...#...."""..M
-00000070: 6f64 756c 6520 636f 6e74 6169 6e73 2074  odule contains t
-00000080: 6865 206d 6169 6e20 636c 6173 7320 666f  he main class fo
-00000090: 7220 6f70 6572 6174 696f 6e20 6f66 2053  r operation of S
-000000a0: 5253 2052 4741 3130 3020 7365 7269 6573  RS RGA100 series
-000000b0: 0d0a 2222 220d 0a0d 0a66 726f 6d20 7372  .."""....from sr
-000000c0: 7367 7569 2069 6d70 6f72 7420 496e 7374  sgui import Inst
-000000d0: 7275 6d65 6e74 0d0a 6672 6f6d 2073 7273  rument..from srs
-000000e0: 6775 6920 696d 706f 7274 2049 6e73 7443  gui import InstC
-000000f0: 6f6d 6d75 6e69 6361 7469 6f6e 4572 726f  ommunicationErro
-00000100: 722c 205c 0d0a 2020 2020 2020 2020 2020  r, \..          
-00000110: 2020 2020 2020 2020 2049 6e73 744c 6f67           InstLog
-00000120: 696e 4661 696c 7572 6545 7272 6f72 2c20  inFailureError, 
-00000130: 496e 7374 4964 4572 726f 720d 0a0d 0a66  InstIdError....f
-00000140: 726f 6d20 7372 7367 7569 2069 6d70 6f72  rom srsgui impor
-00000150: 7420 5365 7269 616c 496e 7465 7266 6163  t SerialInterfac
-00000160: 652c 2054 6370 6970 496e 7465 7266 6163  e, TcpipInterfac
-00000170: 650d 0a66 726f 6d20 7372 7367 7569 2069  e..from srsgui i
-00000180: 6d70 6f72 7420 4669 6e64 4c69 7374 496e  mport FindListIn
-00000190: 7075 742c 2049 7034 496e 7075 742c 2053  put, Ip4Input, S
-000001a0: 7472 696e 6749 6e70 7574 2c20 5061 7373  tringInput, Pass
-000001b0: 776f 7264 496e 7075 742c 2049 6e74 6567  wordInput, Integ
-000001c0: 6572 496e 7075 740d 0a0d 0a66 726f 6d20  erInput....from 
-000001d0: 2e73 6361 6e73 2069 6d70 6f72 7420 5363  .scans import Sc
-000001e0: 616e 730d 0a66 726f 6d20 2e63 6f6d 706f  ans..from .compo
-000001f0: 6e65 6e74 7320 696d 706f 7274 2051 4d46  nents import QMF
-00000200: 2c20 496f 6e69 7a65 722c 2046 696c 616d  , Ionizer, Filam
-00000210: 656e 742c 2043 454d 2c20 5072 6573 7375  ent, CEM, Pressu
-00000220: 7265 2c20 5374 6174 7573 0d0a 0d0a 0d0a  re, Status......
-00000230: 636c 6173 7320 4465 6661 756c 7473 3a0d  class Defaults:.
-00000240: 0a20 2020 2022 2222 0d0a 2020 2020 5352  .    """..    SR
-00000250: 5320 5247 4120 6465 6661 756c 7420 7661  S RGA default va
-00000260: 6c75 6573 2061 6674 6572 2072 6573 6574  lues after reset
-00000270: 0d0a 2020 2020 2222 220d 0a20 2020 2045  ..    """..    E
-00000280: 6c65 6374 726f 6e45 6e65 7267 7920 3d20  lectronEnergy = 
-00000290: 3730 0d0a 2020 2020 496f 6e45 6e65 7267  70..    IonEnerg
-000002a0: 7920 3d20 3132 0d0a 2020 2020 466f 6375  y = 12..    Focu
-000002b0: 7356 6f6c 7461 6765 203d 2039 300d 0a20  sVoltage = 90.. 
-000002c0: 2020 2049 6e69 7469 616c 4d61 7373 203d     InitialMass =
-000002d0: 2031 0d0a 2020 2020 5363 616e 5370 6565   1..    ScanSpee
-000002e0: 6420 3d20 340d 0a20 2020 2053 7465 7073  d = 4..    Steps
-000002f0: 5065 7241 6d75 203d 2031 300d 0a0d 0a0d  PerAmu = 10.....
-00000300: 0a63 6c61 7373 2052 4741 3130 3028 496e  .class RGA100(In
-00000310: 7374 7275 6d65 6e74 293a 0d0a 2020 2020  strument):..    
-00000320: 2222 220d 0a20 2020 2043 6c61 7373 2074  """..    Class t
-00000330: 6f20 636f 6e74 726f 6c20 616e 6420 6163  o control and ac
-00000340: 7175 6972 6520 6461 7461 2077 6974 680d  quire data with.
-00000350: 0a20 2020 2060 5352 5320 5247 4131 3030  .    `SRS RGA100
-00000360: 2c20 3230 302c 2033 3030 2073 6572 6965  , 200, 300 serie
-00000370: 7320 3c68 7474 7073 3a2f 2f77 7777 2e74  s <https://www.t
-00000380: 6869 6e6b 7372 732e 636f 6d2f 7072 6f64  hinksrs.com/prod
-00000390: 7563 7473 2f72 6761 2e68 746d 6c3e 605f  ucts/rga.html>`_
-000003a0: 2e0d 0a0d 0a20 2020 2041 206e 6174 6976  .....    A nativ
-000003b0: 6520 5352 5320 5247 4120 6861 7320 6120  e SRS RGA has a 
-000003c0: 5253 3233 3220 7365 7269 616c 2070 6f72  RS232 serial por
-000003d0: 7420 7468 6174 2063 6f6e 6e65 6374 7320  t that connects 
-000003e0: 7769 7468 0d0a 2020 2020 6261 7564 2072  with..    baud r
-000003f0: 6174 6520 6f66 2032 3838 3030 2c20 6f6e  ate of 28800, on
-00000400: 6520 7374 6f70 2062 6974 2c20 6e6f 2070  e stop bit, no p
-00000410: 6172 6974 792c 2077 6974 6820 5254 532f  arity, with RTS/
-00000420: 4354 5320 666c 6f77 2063 6f6e 7472 6f6c  CTS flow control
-00000430: 2e0d 0a0d 0a20 2020 2054 6865 7265 2069  .....    There i
-00000440: 7320 616e 206f 7074 696f 6e20 746f 2061  s an option to a
-00000450: 6464 2045 7468 6572 6e65 7420 636f 6d6d  dd Ethernet comm
-00000460: 756e 6963 6174 696f 6e20 7573 696e 670d  unication using.
-00000470: 0a20 2020 2060 5247 4120 6574 6865 726e  .    `RGA ethern
-00000480: 6574 2061 6461 7074 6572 203c 6874 7470  et adapter <http
-00000490: 733a 2f2f 7468 696e 6b73 7273 2e63 6f6d  s://thinksrs.com
-000004a0: 2f64 6f77 6e6c 6f61 6473 2f70 6466 732f  /downloads/pdfs/
-000004b0: 6d61 6e75 616c 732f 5245 416d 2e70 6466  manuals/REAm.pdf
-000004c0: 3e60 5f0d 0a0d 0a20 2020 2052 4741 3130  >`_....    RGA10
-000004d0: 3020 636c 6173 7320 7072 6f76 6964 6573  0 class provides
-000004e0: 206d 6574 686f 6473 2066 6f72 2065 7374   methods for est
-000004f0: 6162 6c69 7368 696e 6720 636f 6d6d 756e  ablishing commun
-00000500: 6963 6174 696f 6e2c 0d0a 2020 2020 6261  ication,..    ba
-00000510: 7369 6320 6f70 6572 6174 696f 6e20 616e  sic operation an
-00000520: 6420 7363 616e 7320 746f 2061 6371 7569  d scans to acqui
-00000530: 7265 206d 6173 7320 7370 6563 7472 612e  re mass spectra.
-00000540: 0d0a 0d0a 2020 2020 4578 616d 706c 650d  ....    Example.
-00000550: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 0d0a  .    ---------..
-00000560: 2020 2020 2e2e 2063 6f64 652d 626c 6f63      .. code-bloc
-00000570: 6b3a 3a20 7079 7468 6f6e 0d0a 0d0a 2020  k:: python....  
-00000580: 2020 2020 2020 6672 6f6d 2073 7273 696e        from srsin
-00000590: 7374 2e72 6761 2069 6d70 6f72 7420 5247  st.rga import RG
-000005a0: 4131 3030 0d0a 2020 2020 2020 2020 7231  A100..        r1
-000005b0: 203d 2052 4741 3130 3028 2773 6572 6961   = RGA100('seria
-000005c0: 6c27 2c20 2743 4f4d 3327 2c20 3238 3830  l', 'COM3', 2880
-000005d0: 3029 0d0a 0d0a 2020 2020 2020 2020 2320  0)....        # 
-000005e0: 6966 2045 7468 6572 6e65 7420 636f 6e6e  if Ethernet conn
-000005f0: 6563 7469 6f6e 2069 7320 7573 6564 2c0d  ection is used,.
-00000600: 0a20 2020 2020 2020 2023 2072 3120 3d20  .        # r1 = 
-00000610: 5247 4131 3030 2827 7463 7069 7027 2c20  RGA100('tcpip', 
-00000620: 2731 3932 2e31 3638 2e31 2e31 3030 272c  '192.168.1.100',
-00000630: 2027 7573 6572 6964 272c 2027 7061 7373   'userid', 'pass
-00000640: 776f 7264 2729 0d0a 0d0a 2020 2020 2020  word')....      
-00000650: 2020 7231 2e73 6574 5f65 6d69 7373 696f    r1.set_emissio
-00000660: 6e5f 6375 7272 656e 7428 312e 3029 0d0a  n_current(1.0)..
-00000670: 2020 2020 2020 2020 7231 2e73 6574 5f73          r1.set_s
-00000680: 6361 6e5f 7061 7261 6d65 7465 7273 2829  can_parameters()
-00000690: 0d0a 0d0a 2020 2020 2020 2020 7873 203d  ....        xs =
-000006a0: 2072 312e 6765 745f 6d61 7373 5f61 7869   r1.get_mass_axi
-000006b0: 7328 290d 0a20 2020 2020 2020 2079 7320  s()..        ys 
-000006c0: 3d20 7231 2e67 6574 5f61 6e61 6c6f 675f  = r1.get_analog_
-000006d0: 7363 616e 2829 0d0a 0d0a 2020 2020 2020  scan()....      
-000006e0: 2020 666f 7220 782c 2079 2069 6e20 7a69    for x, y in zi
-000006f0: 7028 7873 2c20 7973 293a 0d0a 2020 2020  p(xs, ys):..    
-00000700: 2020 2020 2020 2020 7072 696e 7428 782c          print(x,
-00000710: 2079 290d 0a0d 0a20 2020 2020 2020 2072   y)....        r
-00000720: 312e 7365 745f 656d 6973 7369 6f6e 5f63  1.set_emission_c
-00000730: 7572 7265 6e74 2830 2e30 290d 0a20 2020  urrent(0.0)..   
-00000740: 2020 2020 2072 312e 6469 7363 6f6e 6e65       r1.disconne
-00000750: 6374 2829 0d0a 0d0a 2020 2020 2222 220d  ct()....    """.
-00000760: 0a0d 0a20 2020 205f 4964 5374 7269 6e67  ...    _IdString
-00000770: 203d 2027 5352 5352 4741 270d 0a20 2020   = 'SRSRGA'..   
-00000780: 205f 7465 726d 5f63 6861 7220 3d20 6227   _term_char = b'
-00000790: 5c72 270d 0a20 2020 200d 0a20 2020 2061  \r'..    ..    a
-000007a0: 7661 696c 6162 6c65 5f69 6e74 6572 6661  vailable_interfa
-000007b0: 6365 7320 3d20 5b0d 0a20 2020 2020 2020  ces = [..       
-000007c0: 205b 2020 2053 6572 6961 6c49 6e74 6572   [   SerialInter
-000007d0: 6661 6365 2c0d 0a20 2020 2020 2020 2020  face,..         
-000007e0: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-000007f0: 2020 2020 2020 2770 6f72 7427 3a20 4669        'port': Fi
-00000800: 6e64 4c69 7374 496e 7075 7428 292c 0d0a  ndListInput(),..
-00000810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000820: 2762 6175 645f 7261 7465 273a 2032 3838  'baud_rate': 288
-00000830: 3030 2c0d 0a20 2020 2020 2020 2020 2020  00,..           
-00000840: 2020 2020 2027 6861 7264 7761 7265 5f66       'hardware_f
-00000850: 6c6f 775f 636f 6e74 726f 6c27 3a20 5472  low_control': Tr
-00000860: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
-00000870: 7d0d 0a20 2020 2020 2020 205d 2c0d 0a20  }..        ],.. 
-00000880: 2020 2020 2020 205b 2020 2054 6370 6970         [   Tcpip
-00000890: 496e 7465 7266 6163 652c 0d0a 2020 2020  Interface,..    
-000008a0: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
-000008b0: 2020 2020 2020 2020 2020 2027 6970 5f61             'ip_a
-000008c0: 6464 7265 7373 273a 2049 7034 496e 7075  ddress': Ip4Inpu
-000008d0: 7428 2731 3932 2e31 3638 2e31 2e31 3027  t('192.168.1.10'
-000008e0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-000008f0: 2020 2020 2775 7365 725f 6964 273a 2053      'user_id': S
-00000900: 7472 696e 6749 6e70 7574 2827 6164 6d69  tringInput('admi
-00000910: 6e27 292c 0d0a 2020 2020 2020 2020 2020  n'),..          
-00000920: 2020 2020 2020 2770 6173 7377 6f72 6427        'password'
-00000930: 3a20 5061 7373 776f 7264 496e 7075 7428  : PasswordInput(
-00000940: 2761 646d 696e 2729 2c0d 0a20 2020 2020  'admin'),..     
-00000950: 2020 2020 2020 2020 2020 2027 706f 7274             'port
-00000960: 273a 2038 3138 0d0a 2020 2020 2020 2020  ': 818..        
-00000970: 2020 2020 7d0d 0a20 2020 2020 2020 205d      }..        ]
-00000980: 2c0d 0a20 2020 205d 0d0a 0d0a 2020 2020  ,..    ]....    
-00000990: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-000009a0: 662c 2069 6e74 6572 6661 6365 5f74 7970  f, interface_typ
-000009b0: 653d 4e6f 6e65 2c20 2a61 7267 7329 3a0d  e=None, *args):.
-000009c0: 0a0d 0a20 2020 2020 2020 2073 7570 6572  ...        super
-000009d0: 2829 2e5f 5f69 6e69 745f 5f28 696e 7465  ().__init__(inte
-000009e0: 7266 6163 655f 7479 7065 2c20 2a61 7267  rface_type, *arg
-000009f0: 7329 0d0a 2020 2020 2020 2020 7365 6c66  s)..        self
-00000a00: 2e73 6574 5f74 6572 6d5f 6368 6172 2862  .set_term_char(b
-00000a10: 275c 7227 290d 0a20 2020 2020 2020 2073  '\r')..        s
-00000a20: 656c 662e 5f6d 5f6d 6178 203d 2031 3030  elf._m_max = 100
-00000a30: 0d0a 0d0a 2020 2020 2020 2020 2320 4164  ....        # Ad
-00000a40: 6420 636f 6d70 6f6e 656e 7473 0d0a 2020  d components..  
-00000a50: 2020 2020 2020 7365 6c66 2e73 6361 6e20        self.scan 
-00000a60: 3d20 5363 616e 7328 7365 6c66 290d 0a20  = Scans(self).. 
-00000a70: 2020 2020 2020 2073 656c 662e 696f 6e69         self.ioni
-00000a80: 7a65 7220 3d20 496f 6e69 7a65 7228 7365  zer = Ionizer(se
-00000a90: 6c66 290d 0a20 2020 2020 2020 2073 656c  lf)..        sel
-00000aa0: 662e 6669 6c61 6d65 6e74 203d 2046 696c  f.filament = Fil
-00000ab0: 616d 656e 7428 7365 6c66 290d 0a20 2020  ament(self)..   
-00000ac0: 2020 2020 2073 656c 662e 6365 6d20 3d20       self.cem = 
-00000ad0: 4345 4d28 7365 6c66 290d 0a20 2020 2020  CEM(self)..     
-00000ae0: 2020 2073 656c 662e 716d 6620 3d20 514d     self.qmf = QM
-00000af0: 4628 7365 6c66 290d 0a20 2020 2020 2020  F(self)..       
-00000b00: 2073 656c 662e 7072 6573 7375 7265 203d   self.pressure =
-00000b10: 2050 7265 7373 7572 6528 7365 6c66 290d   Pressure(self).
-00000b20: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-00000b30: 6174 7573 203d 2053 7461 7475 7328 7365  atus = Status(se
-00000b40: 6c66 290d 0a0d 0a20 2020 2064 6566 2063  lf)....    def c
-00000b50: 6f6e 6e65 6374 2873 656c 662c 2069 6e74  onnect(self, int
-00000b60: 6572 6661 6365 5f74 7970 652c 202a 6172  erface_type, *ar
-00000b70: 6773 293a 0d0a 2020 2020 2020 2020 2222  gs):..        ""
-00000b80: 220d 0a20 2020 2020 2020 2043 6f6e 6e65  "..        Conne
-00000b90: 6374 2074 6f20 616e 2069 6e73 7472 756d  ct to an instrum
-00000ba0: 656e 7420 6f76 6572 2074 6865 2073 7065  ent over the spe
-00000bb0: 6369 6669 6564 2063 6f6d 6d75 6e69 6361  cified communica
-00000bc0: 7469 6f6e 2069 6e74 6572 6661 6365 0d0a  tion interface..
-00000bd0: 0d0a 2020 2020 2020 2020 4966 2069 6e74  ..        If int
-00000be0: 6572 6661 6365 5f74 7970 6520 6973 2027  erface_type is '
-00000bf0: 7365 7269 616c 272c 0d0a 0d0a 2020 2020  serial',....    
-00000c00: 2020 2020 5061 7261 6d65 7465 7273 0d0a      Parameters..
-00000c10: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00000c20: 2d2d 2d0d 0a20 2020 2020 2020 2020 2020  ---..           
-00000c30: 2069 6e74 6572 6661 6365 5f74 7970 653a   interface_type:
-00000c40: 2073 7472 0d0a 2020 2020 2020 2020 2020   str..          
-00000c50: 2020 2020 2020 5573 6520 2a2a 2773 6572        Use **'ser
-00000c60: 6961 6c27 2a2a 2066 6f72 2073 6572 6961  ial'** for seria
-00000c70: 6c20 636f 6d6d 756e 6963 6174 696f 6e0d  l communication.
-00000c80: 0a20 2020 2020 2020 2020 2020 2070 6f72  .            por
-00000c90: 7420 3a20 7374 7269 6e67 0d0a 2020 2020  t : string..    
-00000ca0: 2020 2020 2020 2020 2020 2020 7365 7269              seri
-00000cb0: 616c 2070 6f72 742c 2020 7375 6368 2061  al port,  such a
-00000cc0: 7320 2743 4f4d 3327 206f 7220 272f 6465  s 'COM3' or '/de
-00000cd0: 762f 7474 7955 5342 3027 0d0a 2020 2020  v/ttyUSB0'..    
-00000ce0: 2020 2020 2020 2020 6261 7564 5f72 6174          baud_rat
-00000cf0: 6520 3a20 696e 742c 206f 7074 696f 6e61  e : int, optiona
-00000d00: 6c0d 0a20 2020 2020 2020 2020 2020 2020  l..             
-00000d10: 2020 2062 6175 6420 7261 7465 206f 6620     baud rate of 
-00000d20: 7468 6520 7365 7269 616c 2070 6f72 742c  the serial port,
-00000d30: 2064 6566 6175 6c74 2069 7320 3131 3432   default is 1142
-00000d40: 3030 2c20 616e 6420 5352 5320 5247 4120  00, and SRS RGA 
-00000d50: 7573 6573 2032 3838 3030 2e0d 0a20 2020  uses 28800...   
-00000d60: 2020 2020 2020 2020 2068 6172 6477 6172           hardwar
-00000d70: 655f 666c 6f77 5f63 6f6e 7472 6f6c 3a20  e_flow_control: 
-00000d80: 626f 6f6c 2c20 6f70 7469 6f6e 616c 0d0a  bool, optional..
-00000d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000da0: 5254 532f 4354 5320 7365 7474 696e 672e  RTS/CTS setting.
-00000db0: 2054 6865 2064 6566 6175 6c74 2069 7320   The default is 
-00000dc0: 4661 6c73 652c 2053 5253 2052 4741 2072  False, SRS RGA r
-00000dd0: 6571 7569 7265 7320 2a2a 5472 7565 2a2a  equires **True**
-00000de0: 2e0d 0a0d 0a20 2020 2020 2020 2049 6620  .....        If 
-00000df0: 696e 7465 7266 6163 655f 7479 7065 2069  interface_type i
-00000e00: 7320 2774 6370 6970 272c 0d0a 0d0a 2020  s 'tcpip',....  
-00000e10: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00000e20: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
-00000e30: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2020  -----..         
-00000e40: 2020 2069 6e74 6572 6661 6365 5f74 7970     interface_typ
-00000e50: 653a 2073 7472 0d0a 2020 2020 2020 2020  e: str..        
-00000e60: 2020 2020 2020 2020 5573 6520 2a2a 2774          Use **'t
-00000e70: 6370 6970 272a 2a20 666f 7220 4574 6865  cpip'** for Ethe
-00000e80: 726e 6574 2063 6f6d 6d75 6e69 6361 7469  rnet communicati
-00000e90: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
-00000ea0: 6970 5f61 6464 7265 7373 3a20 7374 720d  ip_address: str.
-00000eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000ec0: 2049 5020 6164 6472 6573 7320 6f66 2061   IP address of a
-00000ed0: 2069 6e73 7472 756d 656e 740d 0a20 2020   instrument..   
-00000ee0: 2020 2020 2020 2020 2075 7365 725f 6964           user_id
-00000ef0: 3a20 7374 720d 0a20 2020 2020 2020 2020  : str..         
-00000f00: 2020 2020 2020 2075 7365 7220 6e61 6d65         user name
-00000f10: 2066 6f72 206c 6f67 696e 2e0d 0a20 2020   for login...   
-00000f20: 2020 2020 2020 2020 2070 6173 7377 6f72           passwor
-00000f30: 6420 3a20 7374 720d 0a20 2020 2020 2020  d : str..       
-00000f40: 2020 2020 2020 2020 2070 6173 7377 6f72           passwor
-00000f50: 6420 666f 7220 6c6f 6769 6e2e 0d0a 2020  d for login...  
-00000f60: 2020 2020 2020 2020 2020 706f 7274 203a            port :
-00000f70: 2069 6e74 2c20 6f70 7469 6f6e 616c 0d0a   int, optional..
-00000f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f90: 5443 5020 706f 7274 206e 756d 6265 722e  TCP port number.
-00000fa0: 2054 6865 2064 6566 6175 6c74 2069 7320   The default is 
-00000fb0: 3831 382c 2077 6869 6368 2053 5253 2052  818, which SRS R
-00000fc0: 4741 2075 7365 730d 0a0d 0a20 2020 2020  GA uses....     
-00000fd0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00000fe0: 7375 7065 7228 292e 636f 6e6e 6563 7428  super().connect(
-00000ff0: 696e 7465 7266 6163 655f 7479 7065 2c20  interface_type, 
-00001000: 2a61 7267 7329 0d0a 2020 2020 2020 2020  *args)..        
-00001010: 6966 2074 7970 6528 7365 6c66 2e63 6f6d  if type(self.com
-00001020: 6d29 203d 3d20 5365 7269 616c 496e 7465  m) == SerialInte
-00001030: 7266 6163 653a 0d0a 2020 2020 2020 2020  rface:..        
-00001040: 2020 2020 2320 4d61 6b65 2073 7572 6520      # Make sure 
-00001050: 7468 6520 6861 7264 7761 7265 2066 6c6f  the hardware flo
-00001060: 7720 636f 6e74 726f 6c20 6973 2073 6574  w control is set
-00001070: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00001080: 6c66 2e63 6f6d 6d2e 5f73 6572 6961 6c2e  lf.comm._serial.
-00001090: 7274 7363 7473 203d 2054 7275 650d 0a0d  rtscts = True...
-000010a0: 0a20 2020 2064 6566 2063 6865 636b 5f69  .    def check_i
-000010b0: 6428 7365 6c66 293a 0d0a 0d0a 2020 2020  d(self):....    
-000010c0: 2020 2020 7365 6c66 2e5f 6d5f 6d61 7820      self._m_max 
-000010d0: 3d20 3130 300d 0a20 2020 2020 2020 2069  = 100..        i
-000010e0: 6620 6e6f 7420 7365 6c66 2e69 735f 636f  f not self.is_co
-000010f0: 6e6e 6563 7465 6428 293a 0d0a 2020 2020  nnected():..    
-00001100: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-00001110: 6f6e 652c 204e 6f6e 652c 204e 6f6e 650d  one, None, None.
-00001120: 0a0d 0a20 2020 2020 2020 2072 6570 6c79  ...        reply
-00001130: 203d 2073 656c 662e 7175 6572 795f 7465   = self.query_te
-00001140: 7874 2827 4944 3f27 292e 7374 7269 7028  xt('ID?').strip(
-00001150: 290d 0a0d 0a20 2020 2020 2020 2069 6620  )....        if 
-00001160: 6c65 6e28 7265 706c 7929 203c 2032 303a  len(reply) < 20:
-00001170: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00001180: 7475 726e 204e 6f6e 652c 204e 6f6e 652c  turn None, None,
-00001190: 204e 6f6e 650d 0a0d 0a20 2020 2020 2020   None....       
-000011a0: 206d 6f64 656c 5f6e 616d 6520 3d20 7265   model_name = re
-000011b0: 706c 795b 303a 395d 0d0a 2020 2020 2020  ply[0:9]..      
-000011c0: 2020 6669 726d 7761 7265 5f76 6572 7369    firmware_versi
-000011d0: 6f6e 203d 2072 6570 6c79 5b31 323a 3136  on = reply[12:16
-000011e0: 5d0d 0a20 2020 2020 2020 2073 6572 6961  ]..        seria
-000011f0: 6c5f 6e75 6d62 6572 203d 2072 6570 6c79  l_number = reply
-00001200: 5b31 383a 5d0d 0a0d 0a20 2020 2020 2020  [18:]....       
-00001210: 2069 6620 7365 6c66 2e5f 4964 5374 7269   if self._IdStri
-00001220: 6e67 206e 6f74 2069 6e20 7265 706c 793a  ng not in reply:
-00001230: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
-00001240: 6973 6520 496e 7374 4964 4572 726f 7228  ise InstIdError(
-00001250: 2249 6e76 616c 6964 2069 6e73 7472 756d  "Invalid instrum
-00001260: 656e 743a 207b 7d20 6e6f 7420 696e 207b  ent: {} not in {
-00001270: 7d22 0d0a 2020 2020 2020 2020 2020 2020  }"..            
-00001280: 2020 2020 2020 2e66 6f72 6d61 7428 7365        .format(se
-00001290: 6c66 2e5f 4964 5374 7269 6e67 2c20 6d6f  lf._IdString, mo
-000012a0: 6465 6c5f 6e61 6d65 2929 0d0a 2020 2020  del_name))..    
-000012b0: 2020 2020 7365 6c66 2e5f 6964 5f73 7472      self._id_str
-000012c0: 696e 6720 3d20 7265 706c 790d 0a0d 0a20  ing = reply.... 
-000012d0: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
-000012e0: 2020 2020 2020 2020 2073 656c 662e 5f6d           self._m
-000012f0: 5f6d 6178 203d 2069 6e74 2872 6570 6c79  _max = int(reply
-00001300: 5b36 3a39 5d29 2020 2320 756e 696e 6974  [6:9])  # uninit
-00001310: 6961 6c69 7a65 6420 756e 6974 2068 6173  ialized unit has
-00001320: 2027 3f3f 3f27 0d0a 2020 2020 2020 2020   '???'..        
-00001330: 6578 6365 7074 2056 616c 7565 4572 726f  except ValueErro
-00001340: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
-00001350: 7365 6c66 2e5f 6d5f 6d61 7820 3d20 3130  self._m_max = 10
-00001360: 300d 0a0d 0a20 2020 2020 2020 2073 656c  0....        sel
-00001370: 662e 5f6d 6f64 656c 5f6e 616d 6520 3d20  f._model_name = 
-00001380: 6d6f 6465 6c5f 6e61 6d65 0d0a 2020 2020  model_name..    
-00001390: 2020 2020 7365 6c66 2e5f 7365 7269 616c      self._serial
-000013a0: 5f6e 756d 6265 7220 3d20 7365 7269 616c  _number = serial
-000013b0: 5f6e 756d 6265 720d 0a20 2020 2020 2020  _number..       
-000013c0: 2073 656c 662e 5f66 6972 6d77 6172 655f   self._firmware_
-000013d0: 7665 7273 696f 6e20 3d20 6669 726d 7761  version = firmwa
-000013e0: 7265 5f76 6572 7369 6f6e 0d0a 2020 2020  re_version..    
-000013f0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00001400: 5f6d 6f64 656c 5f6e 616d 652c 2073 656c  _model_name, sel
-00001410: 662e 5f73 6572 6961 6c5f 6e75 6d62 6572  f._serial_number
-00001420: 2c20 7365 6c66 2e5f 6669 726d 7761 7265  , self._firmware
-00001430: 5f76 6572 7369 6f6e 0d0a 0d0a 2020 2020  _version....    
-00001440: 6465 6620 6765 745f 7374 6174 7573 2873  def get_status(s
-00001450: 656c 6629 3a0d 0a20 2020 2020 2020 2073  elf):..        s
-00001460: 7461 7475 735f 7374 7269 6e67 203d 2027  tatus_string = '
-00001470: 456d 6973 7369 6f6e 2063 7572 7265 6e74  Emission current
-00001480: 3a20 7b3a 2e32 667d 206d 415c 6e27 2e66  : {:.2f} mA\n'.f
-00001490: 6f72 6d61 7428 7365 6c66 2e69 6f6e 697a  ormat(self.ioniz
-000014a0: 6572 2e65 6d69 7373 696f 6e5f 6375 7272  er.emission_curr
-000014b0: 656e 7429 0d0a 2020 2020 2020 2020 7374  ent)..        st
-000014c0: 6174 7573 5f73 7472 696e 6720 2b3d 2027  atus_string += '
-000014d0: 4345 4d20 4856 3a20 7b3a 2e30 667d 2056  CEM HV: {:.0f} V
-000014e0: 5c6e 272e 666f 726d 6174 2873 656c 662e  \n'.format(self.
-000014f0: 6365 6d2e 766f 6c74 6167 6529 0d0a 2020  cem.voltage)..  
-00001500: 2020 2020 2020 7374 6174 7573 5f73 7472        status_str
-00001510: 696e 6720 2b3d 2073 656c 662e 7374 6174  ing += self.stat
-00001520: 7573 2e67 6574 5f65 7272 6f72 5f74 6578  us.get_error_tex
-00001530: 7428 290d 0a20 2020 2020 2020 2072 6574  t()..        ret
-00001540: 7572 6e20 7374 6174 7573 5f73 7472 696e  urn status_strin
-00001550: 670d 0a0d 0a20 2020 2064 6566 2068 616e  g....    def han
-00001560: 646c 655f 636f 6d6d 616e 6428 7365 6c66  dle_command(self
-00001570: 2c20 636d 645f 7374 7269 6e67 3a20 7374  , cmd_string: st
-00001580: 7229 3a0d 0a20 2020 2020 2020 2063 6d64  r):..        cmd
-00001590: 203d 2063 6d64 5f73 7472 696e 672e 7570   = cmd_string.up
-000015a0: 7065 7228 290d 0a20 2020 2020 2020 2072  per()..        r
-000015b0: 6570 6c79 203d 2027 270d 0a20 2020 2020  eply = ''..     
-000015c0: 2020 2069 6620 273f 2720 696e 2063 6d64     if '?' in cmd
-000015d0: 206f 7220 636d 642e 7374 6172 7473 7769   or cmd.startswi
-000015e0: 7468 2822 464c 2229 206f 7220 636d 642e  th("FL") or cmd.
-000015f0: 7374 6172 7473 7769 7468 2822 4856 2229  startswith("HV")
-00001600: 206f 7220 5c0d 0a20 2020 2020 2020 2020   or \..         
-00001610: 2020 2020 2020 2063 6d64 2e73 7461 7274         cmd.start
-00001620: 7377 6974 6828 2256 4622 2920 6f72 2063  swith("VF") or c
-00001630: 6d64 2e73 7461 7274 7377 6974 6828 2245  md.startswith("E
-00001640: 4522 295c 0d0a 2020 2020 2020 2020 2020  E")\..          
-00001650: 2020 2020 2020 6f72 2063 6d64 2e73 7461        or cmd.sta
-00001660: 7274 7377 6974 6828 2249 4522 2920 6f72  rtswith("IE") or
-00001670: 2063 6d64 2e73 7461 7274 7377 6974 6828   cmd.startswith(
-00001680: 2249 4e22 293a 0d0a 2020 2020 2020 2020  "IN"):..        
-00001690: 2020 2020 7265 706c 7920 3d20 7365 6c66      reply = self
-000016a0: 2e71 7565 7279 5f74 6578 7428 636d 6429  .query_text(cmd)
-000016b0: 2e73 7472 6970 2829 0d0a 2020 2020 2020  .strip()..      
-000016c0: 2020 656c 6966 2063 6d64 2e73 7461 7274    elif cmd.start
-000016d0: 7377 6974 6828 224d 5222 293a 0d0a 2020  swith("MR"):..  
-000016e0: 2020 2020 2020 2020 2020 2320 7365 6c66            # self
-000016f0: 2e73 656e 6428 636d 6429 0d0a 2020 2020  .send(cmd)..    
-00001700: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-00001710: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-00001720: 7373 203d 2069 6e74 2863 6d64 5b32 3a5d  ss = int(cmd[2:]
-00001730: 2e73 7472 6970 2829 290d 0a20 2020 2020  .strip())..     
-00001740: 2020 2020 2020 2020 2020 2069 6e74 656e             inten
-00001750: 7369 7479 203d 2073 656c 662e 7363 616e  sity = self.scan
-00001760: 2e67 6574 5f73 696e 676c 655f 6d61 7373  .get_single_mass
-00001770: 5f73 6361 6e28 6d61 7373 2920 2023 2072  _scan(mass)  # r
-00001780: 6561 645f 6c6f 6e67 2829 0d0a 2020 2020  ead_long()..    
-00001790: 2020 2020 2020 2020 2020 2020 7265 706c              repl
-000017a0: 7920 3d20 7374 7228 696e 7465 6e73 6974  y = str(intensit
-000017b0: 7929 0d0a 2020 2020 2020 2020 2020 2020  y)..            
-000017c0: 6578 6365 7074 3a0d 0a20 2020 2020 2020  except:..       
-000017d0: 2020 2020 2020 2020 2070 6173 730d 0a20           pass.. 
-000017e0: 2020 2020 2020 2065 6c69 6620 636d 642e         elif cmd.
-000017f0: 7374 6172 7473 7769 7468 2822 5343 2229  startswith("SC")
-00001800: 2061 6e64 206c 656e 2863 6d64 2920 3c20   and len(cmd) < 
-00001810: 3130 3a0d 0a20 2020 2020 2020 2020 2020  10:..           
-00001820: 2073 656c 662e 7363 616e 2e67 6574 5f61   self.scan.get_a
-00001830: 6e61 6c6f 675f 7363 616e 2829 0d0a 2020  nalog_scan()..  
-00001840: 2020 2020 2020 2020 2020 7265 706c 7920            reply 
-00001850: 3d20 2253 6361 6e20 436f 6d70 6c65 7465  = "Scan Complete
-00001860: 6422 0d0a 2020 2020 2020 2020 656c 6966  d"..        elif
-00001870: 2063 6d64 2e73 7461 7274 7377 6974 6828   cmd.startswith(
-00001880: 2248 5322 293a 0d0a 2020 2020 2020 2020  "HS"):..        
-00001890: 2020 2020 7365 6c66 2e73 6361 6e2e 6765      self.scan.ge
-000018a0: 745f 6869 7374 6f67 7261 6d5f 7363 616e  t_histogram_scan
-000018b0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-000018c0: 7265 706c 7920 3d20 2253 6361 6e20 436f  reply = "Scan Co
-000018d0: 6d70 6c65 7465 6422 0d0a 2020 2020 2020  mpleted"..      
-000018e0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-000018f0: 2020 2020 2073 656c 662e 7365 6e64 2863       self.send(c
-00001900: 6d64 290d 0a20 2020 2020 2020 2072 6574  md)..        ret
-00001910: 7572 6e20 7265 706c 790d 0a0d 0a20 2020  urn reply....   
-00001920: 2064 6566 2072 6573 6574 2873 656c 6629   def reset(self)
-00001930: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
-00001940: 7175 6572 795f 7465 7874 2822 494e 3222  query_text("IN2"
-00001950: 290d 0a0d 0a20 2020 2023 2046 6f72 2052  )....    # For R
-00001960: 4741 3130 302c 2020 5253 3233 3220 4453  GA100,  RS232 DS
-00001970: 5220 6c69 6e65 2073 686f 756c 6420 6265  R line should be
-00001980: 2068 6967 6820 6966 2052 5332 3332 2063   high if RS232 c
-00001990: 6162 6c65 2069 7320 636f 6e6e 6563 7465  able is connecte
-000019a0: 640d 0a20 2020 2064 6566 2063 6865 636b  d..    def check
-000019b0: 5f68 6561 645f 6f6e 6c69 6e65 2873 656c  _head_online(sel
-000019c0: 6629 3a0d 0a20 2020 2020 2020 2022 2222  f):..        """
-000019d0: 0d0a 2020 2020 2020 2020 4368 6563 6b20  ..        Check 
-000019e0: 6966 2053 5253 2052 4741 2069 7320 636f  if SRS RGA is co
-000019f0: 6e6e 6563 7465 6420 746f 2061 2063 6f6d  nnected to a com
-00001a00: 6d75 6e69 6361 7469 6f6e 2069 6e73 7465  munication inste
-00001a10: 7266 6163 650d 0a0d 0a20 2020 2020 2020  rface....       
-00001a20: 2046 6f72 2073 6572 6961 6c20 636f 6d6d   For serial comm
-00001a30: 756e 6963 6174 696f 6e2c 2069 7420 6368  unication, it ch
-00001a40: 6563 6b20 666f 7220 4453 5220 6c69 6e65  eck for DSR line
-00001a50: 2066 726f 6d20 5352 5320 5247 4120 6973   from SRS RGA is
-00001a60: 2073 6574 2068 6967 682e 0d0a 2020 2020   set high...    
-00001a70: 2020 2020 466f 7220 4574 6865 726e 6574      For Ethernet
-00001a80: 2063 6f6d 6d75 6e69 6361 7469 6f6e 2c20   communication, 
-00001a90: 6974 2063 6865 636b 2069 6620 7468 6520  it check if the 
-00001aa0: 5443 5020 736f 636b 6574 2069 7320 6f70  TCP socket is op
-00001ab0: 656e 2e0d 0a20 2020 2020 2020 2022 2222  en...        """
-00001ac0: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-00001ad0: 662e 636f 6d6d 2e74 7970 6520 3d3d 2049  f.comm.type == I
-00001ae0: 6e74 6572 6661 6365 2e53 4552 4941 4c3a  nterface.SERIAL:
-00001af0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00001b00: 7475 726e 2073 656c 662e 636f 6d6d 2e5f  turn self.comm._
-00001b10: 7365 7269 616c 2e64 7372 0d0a 2020 2020  serial.dsr..    
-00001b20: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00001b30: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00001b40: 6c66 2e69 735f 636f 6e6e 6563 7465 6428  lf.is_connected(
-00001b50: 290d 0a0d 0a20 2020 2064 6566 2067 6574  )....    def get
-00001b60: 5f6d 6178 5f6d 6173 7328 7365 6c66 293a  _max_mass(self):
-00001b70: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00001b80: 2020 2020 2020 2047 6574 206d 6178 696d         Get maxim
-00001b90: 756d 206d 6173 7320 7468 6174 2063 616e  um mass that can
-00001ba0: 2062 6520 7573 6564 2066 6f72 2061 2073   be used for a s
-00001bb0: 6361 6e0d 0a0d 0a20 2020 2020 2020 2053  can....        S
-00001bc0: 5253 2052 4741 3130 3020 6d6f 6465 6c20  RS RGA100 model 
-00001bd0: 6861 7320 7468 6520 6d61 7869 6d75 6d20  has the maximum 
-00001be0: 6d61 7373 206f 6620 3130 3020 414d 553b  mass of 100 AMU;
-00001bf0: 0d0a 2020 2020 2020 2020 5352 5320 5247  ..        SRS RG
-00001c00: 4132 3030 2c20 3230 3020 414d 553b 2061  A200, 200 AMU; a
-00001c10: 6e64 2053 5253 2052 4741 3330 302c 2033  nd SRS RGA300, 3
-00001c20: 3030 2041 4d55 2e0d 0a0d 0a20 2020 2020  00 AMU.....     
-00001c30: 2020 2052 6574 7572 6e73 0d0a 2020 2020     Returns..    
-00001c40: 2020 2020 2d2d 2d2d 2d2d 2d2d 0d0a 2020      --------..  
-00001c50: 2020 2020 2020 2020 2020 696e 740d 0a20            int.. 
-00001c60: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00001c70: 6178 696d 756d 206d 6173 730d 0a20 2020  aximum mass..   
-00001c80: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00001c90: 2020 7265 7475 726e 2073 656c 662e 5f6d    return self._m
-00001ca0: 5f6d 6178 0d0a 0d0a 2020 2020 6465 6620  _max....    def 
-00001cb0: 6361 6c69 6272 6174 655f 616c 6c28 7365  calibrate_all(se
-00001cc0: 6c66 293a 0d0a 2020 2020 2020 2020 2222  lf):..        ""
-00001cd0: 220d 0a20 2020 2020 2020 2043 616c 6962  "..        Calib
-00001ce0: 7261 7465 2061 6c6c 0d0a 0d0a 2020 2020  rate all....    
-00001cf0: 2020 2020 7265 7475 726e 730d 0a20 2020      returns..   
-00001d00: 2020 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20       --------.. 
-00001d10: 2020 2020 2020 2020 2020 2069 6e74 0d0a             int..
-00001d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d30: 4572 726f 7220 7374 6174 7573 2062 7974  Error status byt
-00001d40: 6520 6166 7465 7220 6361 6c69 6272 6174  e after calibrat
-00001d50: 696f 6e0d 0a20 2020 2020 2020 2022 2222  ion..        """
-00001d60: 0d0a 2020 2020 2020 2020 7265 706c 7920  ..        reply 
-00001d70: 3d20 7365 6c66 2e63 6f6d 6d2e 7175 6572  = self.comm.quer
-00001d80: 795f 7465 7874 5f77 6974 685f 6c6f 6e67  y_text_with_long
-00001d90: 5f74 696d 656f 7574 2822 4341 222c 2031  _timeout("CA", 1
-00001da0: 3230 290d 0a20 2020 2020 2020 2065 7272  20)..        err
-00001db0: 6f72 5f73 7461 7475 7320 3d20 696e 7428  or_status = int(
-00001dc0: 7265 706c 7929 0d0a 2020 2020 2020 2020  reply)..        
-00001dd0: 7265 7475 726e 2065 7272 6f72 5f73 7461  return error_sta
-00001de0: 7475 730d 0a0d 0a20 2020 2064 6566 2063  tus....    def c
-00001df0: 616c 6962 7261 7465 5f65 6c65 6374 726f  alibrate_electro
-00001e00: 6d65 7465 7228 7365 6c66 293a 0d0a 2020  meter(self):..  
-00001e10: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00001e20: 2020 2043 616c 6962 7261 7465 2065 6c65     Calibrate ele
-00001e30: 6374 726f 6d65 7465 7227 7320 492d 5620  ctrometer's I-V 
-00001e40: 7265 7370 6f6e 7365 0d0a 0d0a 2020 2020  response....    
-00001e50: 2020 2020 7265 7475 726e 730d 0a20 2020      returns..   
-00001e60: 2020 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20       --------.. 
-00001e70: 2020 2020 2020 2020 2020 2069 6e74 0d0a             int..
-00001e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e90: 4572 726f 7220 7374 6174 7573 2062 7974  Error status byt
-00001ea0: 6520 6166 7465 7220 6361 6c69 6272 6174  e after calibrat
-00001eb0: 696f 6e0d 0a20 2020 2020 2020 2022 2222  ion..        """
-00001ec0: 0d0a 2020 2020 2020 2020 7265 706c 7920  ..        reply 
-00001ed0: 3d20 7365 6c66 2e63 6f6d 6d2e 7175 6572  = self.comm.quer
-00001ee0: 795f 7465 7874 5f77 6974 685f 6c6f 6e67  y_text_with_long
-00001ef0: 5f74 696d 656f 7574 2822 434c 222c 2031  _timeout("CL", 1
-00001f00: 3230 290d 0a20 2020 2020 2020 2065 7272  20)..        err
-00001f10: 6f72 5f73 7461 7475 7320 3d20 696e 7428  or_status = int(
-00001f20: 7265 706c 7929 0d0a 2020 2020 2020 2020  reply)..        
-00001f30: 7265 7475 726e 2065 7272 6f72 5f73 7461  return error_sta
-00001f40: 7475 730d 0a                             tus..
+00000000: 2323 2120 0d0a 2323 2120 436f 7074 7269  ##! ..##! Coptri
+00000010: 6768 7428 6329 2032 3032 322c 2032 3032  ght(c) 2022, 202
+00000020: 3320 5374 616e 666f 7264 2052 6573 6561  3 Stanford Resea
+00000030: 7263 6820 5379 7374 656d 732c 2041 6c6c  rch Systems, All
+00000040: 2072 6967 6874 2072 6573 6572 7665 640d   right reserved.
+00000050: 0a23 2321 2053 7562 6a65 6374 2074 6f20  .##! Subject to 
+00000060: 7468 6520 4d49 5420 4c69 6365 6e73 650d  the MIT License.
+00000070: 0a23 2321 200d 0a0d 0a0d 0a22 2222 0d0a  .##! ......"""..
+00000080: 4d6f 6475 6c65 2063 6f6e 7461 696e 7320  Module contains 
+00000090: 7468 6520 6d61 696e 2063 6c61 7373 2066  the main class f
+000000a0: 6f72 206f 7065 7261 7469 6f6e 206f 6620  or operation of 
+000000b0: 5352 5320 5247 4131 3030 2073 6572 6965  SRS RGA100 serie
+000000c0: 730d 0a22 2222 0d0a 0d0a 6672 6f6d 2073  s.."""....from s
+000000d0: 7273 6775 6920 696d 706f 7274 2049 6e73  rsgui import Ins
+000000e0: 7472 756d 656e 740d 0a66 726f 6d20 7372  trument..from sr
+000000f0: 7367 7569 2069 6d70 6f72 7420 496e 7374  sgui import Inst
+00000100: 436f 6d6d 756e 6963 6174 696f 6e45 7272  CommunicationErr
+00000110: 6f72 2c20 5c0d 0a20 2020 2020 2020 2020  or, \..         
+00000120: 2020 2020 2020 2020 2020 496e 7374 4c6f            InstLo
+00000130: 6769 6e46 6169 6c75 7265 4572 726f 722c  ginFailureError,
+00000140: 2049 6e73 7449 6445 7272 6f72 0d0a 0d0a   InstIdError....
+00000150: 6672 6f6d 2073 7273 6775 6920 696d 706f  from srsgui impo
+00000160: 7274 2053 6572 6961 6c49 6e74 6572 6661  rt SerialInterfa
+00000170: 6365 2c20 5463 7069 7049 6e74 6572 6661  ce, TcpipInterfa
+00000180: 6365 0d0a 6672 6f6d 2073 7273 6775 6920  ce..from srsgui 
+00000190: 696d 706f 7274 2046 696e 644c 6973 7449  import FindListI
+000001a0: 6e70 7574 2c20 4970 3449 6e70 7574 2c20  nput, Ip4Input, 
+000001b0: 5374 7269 6e67 496e 7075 742c 2050 6173  StringInput, Pas
+000001c0: 7377 6f72 6449 6e70 7574 2c20 496e 7465  swordInput, Inte
+000001d0: 6765 7249 6e70 7574 0d0a 0d0a 6672 6f6d  gerInput....from
+000001e0: 202e 7363 616e 7320 696d 706f 7274 2053   .scans import S
+000001f0: 6361 6e73 2c20 5363 616e 7332 3030 2c20  cans, Scans200, 
+00000200: 5363 616e 7333 3030 0d0a 6672 6f6d 202e  Scans300..from .
+00000210: 636f 6d70 6f6e 656e 7473 2069 6d70 6f72  components impor
+00000220: 7420 514d 462c 2049 6f6e 697a 6572 2c20  t QMF, Ionizer, 
+00000230: 4669 6c61 6d65 6e74 2c20 4345 4d2c 2050  Filament, CEM, P
+00000240: 7265 7373 7572 652c 2053 7461 7475 730d  ressure, Status.
+00000250: 0a0d 0a0d 0a63 6c61 7373 2044 6566 6175  .....class Defau
+00000260: 6c74 733a 0d0a 2020 2020 2222 220d 0a20  lts:..    """.. 
+00000270: 2020 2053 5253 2052 4741 2064 6566 6175     SRS RGA defau
+00000280: 6c74 2076 616c 7565 7320 6166 7465 7220  lt values after 
+00000290: 7265 7365 740d 0a20 2020 2022 2222 0d0a  reset..    """..
+000002a0: 2020 2020 456c 6563 7472 6f6e 456e 6572      ElectronEner
+000002b0: 6779 203d 2037 300d 0a20 2020 2049 6f6e  gy = 70..    Ion
+000002c0: 456e 6572 6779 203d 2031 320d 0a20 2020  Energy = 12..   
+000002d0: 2046 6f63 7573 566f 6c74 6167 6520 3d20   FocusVoltage = 
+000002e0: 3930 0d0a 2020 2020 496e 6974 6961 6c4d  90..    InitialM
+000002f0: 6173 7320 3d20 310d 0a20 2020 2053 6361  ass = 1..    Sca
+00000300: 6e53 7065 6564 203d 2034 0d0a 2020 2020  nSpeed = 4..    
+00000310: 5374 6570 7350 6572 416d 7520 3d20 3130  StepsPerAmu = 10
+00000320: 0d0a 0d0a 0d0a 636c 6173 7320 5247 4131  ......class RGA1
+00000330: 3030 2849 6e73 7472 756d 656e 7429 3a0d  00(Instrument):.
+00000340: 0a20 2020 2022 2222 0d0a 2020 2020 436c  .    """..    Cl
+00000350: 6173 7320 746f 2063 6f6e 7472 6f6c 2061  ass to control a
+00000360: 6e64 2061 6371 7569 7265 2064 6174 6120  nd acquire data 
+00000370: 7769 7468 0d0a 2020 2020 6053 5253 2052  with..    `SRS R
+00000380: 4741 3130 302c 2032 3030 2c20 3330 3020  GA100, 200, 300 
+00000390: 7365 7269 6573 203c 6874 7470 733a 2f2f  series <https://
+000003a0: 7777 772e 7468 696e 6b73 7273 2e63 6f6d  www.thinksrs.com
+000003b0: 2f70 726f 6475 6374 732f 7267 612e 6874  /products/rga.ht
+000003c0: 6d6c 3e60 5f2e 0d0a 0d0a 2020 2020 4120  ml>`_.....    A 
+000003d0: 6e61 7469 7665 2053 5253 2052 4741 2068  native SRS RGA h
+000003e0: 6173 2061 2052 5332 3332 2073 6572 6961  as a RS232 seria
+000003f0: 6c20 706f 7274 2074 6861 7420 636f 6e6e  l port that conn
+00000400: 6563 7473 2077 6974 680d 0a20 2020 2062  ects with..    b
+00000410: 6175 6420 7261 7465 206f 6620 3238 3830  aud rate of 2880
+00000420: 302c 206f 6e65 2073 746f 7020 6269 742c  0, one stop bit,
+00000430: 206e 6f20 7061 7269 7479 2c20 7769 7468   no parity, with
+00000440: 2052 5453 2f43 5453 2066 6c6f 7720 636f   RTS/CTS flow co
+00000450: 6e74 726f 6c2e 0d0a 0d0a 2020 2020 5468  ntrol.....    Th
+00000460: 6572 6520 6973 2061 6e20 6f70 7469 6f6e  ere is an option
+00000470: 2074 6f20 6164 6420 4574 6865 726e 6574   to add Ethernet
+00000480: 2063 6f6d 6d75 6e69 6361 7469 6f6e 2075   communication u
+00000490: 7369 6e67 0d0a 2020 2020 6052 4741 2065  sing..    `RGA e
+000004a0: 7468 6572 6e65 7420 6164 6170 7465 7220  thernet adapter 
+000004b0: 3c68 7474 7073 3a2f 2f74 6869 6e6b 7372  <https://thinksr
+000004c0: 732e 636f 6d2f 646f 776e 6c6f 6164 732f  s.com/downloads/
+000004d0: 7064 6673 2f6d 616e 7561 6c73 2f52 4541  pdfs/manuals/REA
+000004e0: 6d2e 7064 663e 605f 0d0a 0d0a 2020 2020  m.pdf>`_....    
+000004f0: 5247 4131 3030 2063 6c61 7373 2070 726f  RGA100 class pro
+00000500: 7669 6465 7320 6d65 7468 6f64 7320 666f  vides methods fo
+00000510: 7220 6573 7461 626c 6973 6869 6e67 2063  r establishing c
+00000520: 6f6d 6d75 6e69 6361 7469 6f6e 2c0d 0a20  ommunication,.. 
+00000530: 2020 2062 6173 6963 206f 7065 7261 7469     basic operati
+00000540: 6f6e 2061 6e64 2073 6361 6e73 2074 6f20  on and scans to 
+00000550: 6163 7175 6972 6520 6d61 7373 2073 7065  acquire mass spe
+00000560: 6374 7261 2e0d 0a0d 0a20 2020 2045 7861  ctra.....    Exa
+00000570: 6d70 6c65 0d0a 2020 2020 2d2d 2d2d 2d2d  mple..    ------
+00000580: 2d2d 2d0d 0a20 2020 202e 2e20 636f 6465  ---..    .. code
+00000590: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0d  -block:: python.
+000005a0: 0a0d 0a20 2020 2020 2020 2066 726f 6d20  ...        from 
+000005b0: 7372 7369 6e73 742e 7267 6120 696d 706f  srsinst.rga impo
+000005c0: 7274 2052 4741 3130 300d 0a20 2020 2020  rt RGA100..     
+000005d0: 2020 2072 3120 3d20 5247 4131 3030 2827     r1 = RGA100('
+000005e0: 7365 7269 616c 272c 2027 434f 4d33 272c  serial', 'COM3',
+000005f0: 2032 3838 3030 290d 0a0d 0a20 2020 2020   28800)....     
+00000600: 2020 2023 2069 6620 4574 6865 726e 6574     # if Ethernet
+00000610: 2063 6f6e 6e65 6374 696f 6e20 6973 2075   connection is u
+00000620: 7365 642c 0d0a 2020 2020 2020 2020 2320  sed,..        # 
+00000630: 7231 203d 2052 4741 3130 3028 2774 6370  r1 = RGA100('tcp
+00000640: 6970 272c 2027 3139 322e 3136 382e 312e  ip', '192.168.1.
+00000650: 3130 3027 2c20 2775 7365 7269 6427 2c20  100', 'userid', 
+00000660: 2770 6173 7377 6f72 6427 290d 0a0d 0a20  'password').... 
+00000670: 2020 2020 2020 2072 312e 7365 745f 656d         r1.set_em
+00000680: 6973 7369 6f6e 5f63 7572 7265 6e74 2831  ission_current(1
+00000690: 2e30 290d 0a20 2020 2020 2020 2072 312e  .0)..        r1.
+000006a0: 7365 745f 7363 616e 5f70 6172 616d 6574  set_scan_paramet
+000006b0: 6572 7328 290d 0a0d 0a20 2020 2020 2020  ers()....       
+000006c0: 2078 7320 3d20 7231 2e67 6574 5f6d 6173   xs = r1.get_mas
+000006d0: 735f 6178 6973 2829 0d0a 2020 2020 2020  s_axis()..      
+000006e0: 2020 7973 203d 2072 312e 6765 745f 616e    ys = r1.get_an
+000006f0: 616c 6f67 5f73 6361 6e28 290d 0a0d 0a20  alog_scan().... 
+00000700: 2020 2020 2020 2066 6f72 2078 2c20 7920         for x, y 
+00000710: 696e 207a 6970 2878 732c 2079 7329 3a0d  in zip(xs, ys):.
+00000720: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00000730: 6e74 2878 2c20 7929 0d0a 0d0a 2020 2020  nt(x, y)....    
+00000740: 2020 2020 7231 2e73 6574 5f65 6d69 7373      r1.set_emiss
+00000750: 696f 6e5f 6375 7272 656e 7428 302e 3029  ion_current(0.0)
+00000760: 0d0a 2020 2020 2020 2020 7231 2e64 6973  ..        r1.dis
+00000770: 636f 6e6e 6563 7428 290d 0a0d 0a20 2020  connect()....   
+00000780: 2022 2222 0d0a 0d0a 2020 2020 5f49 6453   """....    _IdS
+00000790: 7472 696e 6720 3d20 2753 5253 5247 4127  tring = 'SRSRGA'
+000007a0: 0d0a 2020 2020 5f74 6572 6d5f 6368 6172  ..    _term_char
+000007b0: 203d 2062 275c 7227 0d0a 0d0a 2020 2020   = b'\r'....    
+000007c0: 6176 6169 6c61 626c 655f 696e 7465 7266  available_interf
+000007d0: 6163 6573 203d 205b 0d0a 2020 2020 2020  aces = [..      
+000007e0: 2020 5b53 6572 6961 6c49 6e74 6572 6661    [SerialInterfa
+000007f0: 6365 2c0d 0a20 2020 2020 2020 2020 2020  ce,..           
+00000800: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00000810: 2020 2020 2770 6f72 7427 3a20 4669 6e64      'port': Find
+00000820: 4c69 7374 496e 7075 7428 292c 0d0a 2020  ListInput(),..  
+00000830: 2020 2020 2020 2020 2020 2020 2020 2762                'b
+00000840: 6175 645f 7261 7465 273a 2032 3838 3030  aud_rate': 28800
+00000850: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000860: 2020 2027 6861 7264 7761 7265 5f66 6c6f     'hardware_flo
+00000870: 775f 636f 6e74 726f 6c27 3a20 5472 7565  w_control': True
+00000880: 0d0a 2020 2020 2020 2020 2020 2020 7d0d  ..            }.
+00000890: 0a20 2020 2020 2020 205d 2c0d 0a20 2020  .        ],..   
+000008a0: 2020 2020 205b 5463 7069 7049 6e74 6572       [TcpipInter
+000008b0: 6661 6365 2c0d 0a20 2020 2020 2020 2020  face,..         
+000008c0: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
+000008d0: 2020 2020 2020 2769 705f 6164 6472 6573        'ip_addres
+000008e0: 7327 3a20 4970 3449 6e70 7574 2827 3139  s': Ip4Input('19
+000008f0: 322e 3136 382e 312e 3130 2729 2c0d 0a20  2.168.1.10'),.. 
+00000900: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00000910: 7573 6572 5f69 6427 3a20 5374 7269 6e67  user_id': String
+00000920: 496e 7075 7428 2761 646d 696e 2729 2c0d  Input('admin'),.
+00000930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000940: 2027 7061 7373 776f 7264 273a 2050 6173   'password': Pas
+00000950: 7377 6f72 6449 6e70 7574 2827 6164 6d69  swordInput('admi
+00000960: 6e27 292c 0d0a 2020 2020 2020 2020 2020  n'),..          
+00000970: 2020 2020 2020 2770 6f72 7427 3a20 3831        'port': 81
+00000980: 380d 0a20 2020 2020 2020 2020 2020 207d  8..            }
+00000990: 0d0a 2020 2020 2020 2020 5d2c 0d0a 2020  ..        ],..  
+000009a0: 2020 5d0d 0a0d 0a20 2020 2064 6566 205f    ]....    def _
+000009b0: 5f69 6e69 745f 5f28 7365 6c66 2c20 696e  _init__(self, in
+000009c0: 7465 7266 6163 655f 7479 7065 3d4e 6f6e  terface_type=Non
+000009d0: 652c 202a 6172 6773 293a 0d0a 0d0a 2020  e, *args):....  
+000009e0: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
+000009f0: 696e 6974 5f5f 2869 6e74 6572 6661 6365  init__(interface
+00000a00: 5f74 7970 652c 202a 6172 6773 290d 0a20  _type, *args).. 
+00000a10: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
+00000a20: 7465 726d 5f63 6861 7228 6227 5c72 2729  term_char(b'\r')
+00000a30: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00000a40: 6d5f 6d61 7820 3d20 5363 616e 732e 4d61  m_max = Scans.Ma
+00000a50: 784d 6173 730d 0a0d 0a20 2020 2020 2020  xMass....       
+00000a60: 2023 2041 6464 2063 6f6d 706f 6e65 6e74   # Add component
+00000a70: 730d 0a20 2020 2020 2020 2073 656c 662e  s..        self.
+00000a80: 696f 6e69 7a65 7220 3d20 496f 6e69 7a65  ionizer = Ionize
+00000a90: 7228 7365 6c66 290d 0a20 2020 2020 2020  r(self)..       
+00000aa0: 2073 656c 662e 6669 6c61 6d65 6e74 203d   self.filament =
+00000ab0: 2046 696c 616d 656e 7428 7365 6c66 290d   Filament(self).
+00000ac0: 0a20 2020 2020 2020 2073 656c 662e 6365  .        self.ce
+00000ad0: 6d20 3d20 4345 4d28 7365 6c66 290d 0a20  m = CEM(self).. 
+00000ae0: 2020 2020 2020 2073 656c 662e 7363 616e         self.scan
+00000af0: 203d 2053 6361 6e73 2873 656c 6629 0d0a   = Scans(self)..
+00000b00: 2020 2020 2020 2020 7365 6c66 2e71 6d66          self.qmf
+00000b10: 203d 2051 4d46 2873 656c 6629 0d0a 2020   = QMF(self)..  
+00000b20: 2020 2020 2020 7365 6c66 2e70 7265 7373        self.press
+00000b30: 7572 6520 3d20 5072 6573 7375 7265 2873  ure = Pressure(s
+00000b40: 656c 6629 0d0a 2020 2020 2020 2020 7365  elf)..        se
+00000b50: 6c66 2e73 7461 7475 7320 3d20 5374 6174  lf.status = Stat
+00000b60: 7573 2873 656c 6629 0d0a 0d0a 2020 2020  us(self)....    
+00000b70: 6465 6620 636f 6e6e 6563 7428 7365 6c66  def connect(self
+00000b80: 2c20 696e 7465 7266 6163 655f 7479 7065  , interface_type
+00000b90: 2c20 2a61 7267 7329 3a0d 0a20 2020 2020  , *args):..     
+00000ba0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00000bb0: 436f 6e6e 6563 7420 746f 2061 6e20 696e  Connect to an in
+00000bc0: 7374 7275 6d65 6e74 206f 7665 7220 7468  strument over th
+00000bd0: 6520 7370 6563 6966 6965 6420 636f 6d6d  e specified comm
+00000be0: 756e 6963 6174 696f 6e20 696e 7465 7266  unication interf
+00000bf0: 6163 650d 0a0d 0a20 2020 2020 2020 2049  ace....        I
+00000c00: 6620 696e 7465 7266 6163 655f 7479 7065  f interface_type
+00000c10: 2069 7320 2773 6572 6961 6c27 2c0d 0a0d   is 'serial',...
+00000c20: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00000c30: 6572 730d 0a20 2020 2020 2020 202d 2d2d  ers..        ---
+00000c40: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
+00000c50: 2020 2020 2020 696e 7465 7266 6163 655f        interface_
+00000c60: 7479 7065 3a20 7374 720d 0a20 2020 2020  type: str..     
+00000c70: 2020 2020 2020 2020 2020 2055 7365 202a             Use *
+00000c80: 2a27 7365 7269 616c 272a 2a20 666f 7220  *'serial'** for 
+00000c90: 7365 7269 616c 2063 6f6d 6d75 6e69 6361  serial communica
+00000ca0: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
+00000cb0: 2020 706f 7274 203a 2073 7472 696e 670d    port : string.
+00000cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000cd0: 2073 6572 6961 6c20 706f 7274 2c20 2073   serial port,  s
+00000ce0: 7563 6820 6173 2027 434f 4d33 2720 6f72  uch as 'COM3' or
+00000cf0: 2027 2f64 6576 2f74 7479 5553 4230 270d   '/dev/ttyUSB0'.
+00000d00: 0a20 2020 2020 2020 2020 2020 2062 6175  .            bau
+00000d10: 645f 7261 7465 203a 2069 6e74 2c20 6f70  d_rate : int, op
+00000d20: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+00000d30: 2020 2020 2020 2020 6261 7564 2072 6174          baud rat
+00000d40: 6520 6f66 2074 6865 2073 6572 6961 6c20  e of the serial 
+00000d50: 706f 7274 2c20 6465 6661 756c 7420 6973  port, default is
+00000d60: 2031 3134 3230 302c 2061 6e64 2053 5253   114200, and SRS
+00000d70: 2052 4741 2075 7365 7320 3238 3830 302e   RGA uses 28800.
+00000d80: 0d0a 2020 2020 2020 2020 2020 2020 6861  ..            ha
+00000d90: 7264 7761 7265 5f66 6c6f 775f 636f 6e74  rdware_flow_cont
+00000da0: 726f 6c3a 2062 6f6f 6c2c 206f 7074 696f  rol: bool, optio
+00000db0: 6e61 6c0d 0a20 2020 2020 2020 2020 2020  nal..           
+00000dc0: 2020 2020 2052 5453 2f43 5453 2073 6574       RTS/CTS set
+00000dd0: 7469 6e67 2e20 5468 6520 6465 6661 756c  ting. The defaul
+00000de0: 7420 6973 2046 616c 7365 2c20 5352 5320  t is False, SRS 
+00000df0: 5247 4120 7265 7175 6972 6573 202a 2a54  RGA requires **T
+00000e00: 7275 652a 2a2e 0d0a 0d0a 2020 2020 2020  rue**.....      
+00000e10: 2020 4966 2069 6e74 6572 6661 6365 5f74    If interface_t
+00000e20: 7970 6520 6973 2027 7463 7069 7027 2c0d  ype is 'tcpip',.
+00000e30: 0a0d 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00000e40: 6574 6572 730d 0a20 2020 2020 2020 202d  eters..        -
+00000e50: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020  ----------..    
+00000e60: 2020 2020 2020 2020 696e 7465 7266 6163          interfac
+00000e70: 655f 7479 7065 3a20 7374 720d 0a20 2020  e_type: str..   
+00000e80: 2020 2020 2020 2020 2020 2020 2055 7365               Use
+00000e90: 202a 2a27 7463 7069 7027 2a2a 2066 6f72   **'tcpip'** for
+00000ea0: 2045 7468 6572 6e65 7420 636f 6d6d 756e   Ethernet commun
+00000eb0: 6963 6174 696f 6e0d 0a20 2020 2020 2020  ication..       
+00000ec0: 2020 2020 2069 705f 6164 6472 6573 733a       ip_address:
+00000ed0: 2073 7472 0d0a 2020 2020 2020 2020 2020   str..          
+00000ee0: 2020 2020 2020 4950 2061 6464 7265 7373        IP address
+00000ef0: 206f 6620 6120 696e 7374 7275 6d65 6e74   of a instrument
+00000f00: 0d0a 2020 2020 2020 2020 2020 2020 7573  ..            us
+00000f10: 6572 5f69 643a 2073 7472 0d0a 2020 2020  er_id: str..    
+00000f20: 2020 2020 2020 2020 2020 2020 7573 6572              user
+00000f30: 206e 616d 6520 666f 7220 6c6f 6769 6e2e   name for login.
+00000f40: 0d0a 2020 2020 2020 2020 2020 2020 7061  ..            pa
+00000f50: 7373 776f 7264 203a 2073 7472 0d0a 2020  ssword : str..  
+00000f60: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00000f70: 7373 776f 7264 2066 6f72 206c 6f67 696e  ssword for login
+00000f80: 2e0d 0a20 2020 2020 2020 2020 2020 2070  ...            p
+00000f90: 6f72 7420 3a20 696e 742c 206f 7074 696f  ort : int, optio
+00000fa0: 6e61 6c0d 0a20 2020 2020 2020 2020 2020  nal..           
+00000fb0: 2020 2020 2054 4350 2070 6f72 7420 6e75       TCP port nu
+00000fc0: 6d62 6572 2e20 5468 6520 6465 6661 756c  mber. The defaul
+00000fd0: 7420 6973 2038 3138 2c20 7768 6963 6820  t is 818, which 
+00000fe0: 5352 5320 5247 4120 7573 6573 0d0a 0d0a  SRS RGA uses....
+00000ff0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00001000: 2020 2020 2073 7570 6572 2829 2e63 6f6e       super().con
+00001010: 6e65 6374 2869 6e74 6572 6661 6365 5f74  nect(interface_t
+00001020: 7970 652c 202a 6172 6773 290d 0a20 2020  ype, *args)..   
+00001030: 2020 2020 2069 6620 7479 7065 2873 656c       if type(sel
+00001040: 662e 636f 6d6d 2920 3d3d 2053 6572 6961  f.comm) == Seria
+00001050: 6c49 6e74 6572 6661 6365 3a0d 0a20 2020  lInterface:..   
+00001060: 2020 2020 2020 2020 2023 204d 616b 6520           # Make 
+00001070: 7375 7265 2074 6865 2068 6172 6477 6172  sure the hardwar
+00001080: 6520 666c 6f77 2063 6f6e 7472 6f6c 2069  e flow control i
+00001090: 7320 7365 740d 0a20 2020 2020 2020 2020  s set..         
+000010a0: 2020 2073 656c 662e 636f 6d6d 2e5f 7365     self.comm._se
+000010b0: 7269 616c 2e72 7473 6374 7320 3d20 5472  rial.rtscts = Tr
+000010c0: 7565 0d0a 0d0a 2020 2020 6465 6620 6368  ue....    def ch
+000010d0: 6563 6b5f 6964 2873 656c 6629 3a0d 0a0d  eck_id(self):...
+000010e0: 0a20 2020 2020 2020 2073 656c 662e 5f6d  .        self._m
+000010f0: 5f6d 6178 203d 2031 3030 0d0a 2020 2020  _max = 100..    
+00001100: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+00001110: 6973 5f63 6f6e 6e65 6374 6564 2829 3a0d  is_connected():.
+00001120: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00001130: 7572 6e20 4e6f 6e65 2c20 4e6f 6e65 2c20  urn None, None, 
+00001140: 4e6f 6e65 0d0a 0d0a 2020 2020 2020 2020  None....        
+00001150: 7265 706c 7920 3d20 7365 6c66 2e71 7565  reply = self.que
+00001160: 7279 5f74 6578 7428 2749 443f 2729 2e73  ry_text('ID?').s
+00001170: 7472 6970 2829 0d0a 0d0a 2020 2020 2020  trip()....      
+00001180: 2020 6966 206c 656e 2872 6570 6c79 2920    if len(reply) 
+00001190: 3c20 3230 3a0d 0a20 2020 2020 2020 2020  < 20:..         
+000011a0: 2020 2072 6574 7572 6e20 4e6f 6e65 2c20     return None, 
+000011b0: 4e6f 6e65 2c20 4e6f 6e65 0d0a 0d0a 2020  None, None....  
+000011c0: 2020 2020 2020 6d6f 6465 6c5f 6e61 6d65        model_name
+000011d0: 203d 2072 6570 6c79 5b30 3a39 5d0d 0a20   = reply[0:9].. 
+000011e0: 2020 2020 2020 2066 6972 6d77 6172 655f         firmware_
+000011f0: 7665 7273 696f 6e20 3d20 7265 706c 795b  version = reply[
+00001200: 3132 3a31 365d 0d0a 2020 2020 2020 2020  12:16]..        
+00001210: 7365 7269 616c 5f6e 756d 6265 7220 3d20  serial_number = 
+00001220: 7265 706c 795b 3138 3a5d 0d0a 0d0a 2020  reply[18:]....  
+00001230: 2020 2020 2020 6966 2073 656c 662e 5f49        if self._I
+00001240: 6453 7472 696e 6720 6e6f 7420 696e 2072  dString not in r
+00001250: 6570 6c79 3a0d 0a20 2020 2020 2020 2020  eply:..         
+00001260: 2020 2072 6169 7365 2049 6e73 7449 6445     raise InstIdE
+00001270: 7272 6f72 2822 496e 7661 6c69 6420 696e  rror("Invalid in
+00001280: 7374 7275 6d65 6e74 3a20 7b7d 206e 6f74  strument: {} not
+00001290: 2069 6e20 7b7d 220d 0a20 2020 2020 2020   in {}"..       
+000012a0: 2020 2020 2020 2020 2020 202e 666f 726d             .form
+000012b0: 6174 2873 656c 662e 5f49 6453 7472 696e  at(self._IdStrin
+000012c0: 672c 206d 6f64 656c 5f6e 616d 6529 290d  g, model_name)).
+000012d0: 0a20 2020 2020 2020 2073 656c 662e 5f69  .        self._i
+000012e0: 645f 7374 7269 6e67 203d 2072 6570 6c79  d_string = reply
+000012f0: 0d0a 0d0a 2020 2020 2020 2020 7472 793a  ....        try:
+00001300: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00001310: 6c66 2e5f 6d5f 6d61 7820 3d20 696e 7428  lf._m_max = int(
+00001320: 7265 706c 795b 363a 395d 2920 2023 2075  reply[6:9])  # u
+00001330: 6e69 6e69 7469 616c 697a 6564 2075 6e69  ninitialized uni
+00001340: 7420 6861 7320 273f 3f3f 270d 0a20 2020  t has '???'..   
+00001350: 2020 2020 2065 7863 6570 7420 5661 6c75       except Valu
+00001360: 6545 7272 6f72 3a0d 0a20 2020 2020 2020  eError:..       
+00001370: 2020 2020 2073 656c 662e 5f6d 5f6d 6178       self._m_max
+00001380: 203d 2031 3030 0d0a 0d0a 2020 2020 2020   = 100....      
+00001390: 2020 7365 6c66 2e5f 6d6f 6465 6c5f 6e61    self._model_na
+000013a0: 6d65 203d 206d 6f64 656c 5f6e 616d 650d  me = model_name.
+000013b0: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
+000013c0: 6572 6961 6c5f 6e75 6d62 6572 203d 2073  erial_number = s
+000013d0: 6572 6961 6c5f 6e75 6d62 6572 0d0a 2020  erial_number..  
+000013e0: 2020 2020 2020 7365 6c66 2e5f 6669 726d        self._firm
+000013f0: 7761 7265 5f76 6572 7369 6f6e 203d 2066  ware_version = f
+00001400: 6972 6d77 6172 655f 7665 7273 696f 6e0d  irmware_version.
+00001410: 0a0d 0a20 2020 2020 2020 2069 6620 7365  ...        if se
+00001420: 6c66 2e5f 6d5f 6d61 7820 3e3d 2033 3030  lf._m_max >= 300
+00001430: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00001440: 656c 662e 5f6d 5f6d 6178 203d 2033 3030  elf._m_max = 300
+00001450: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00001460: 2074 7970 6528 7365 6c66 2e73 6361 6e29   type(self.scan)
+00001470: 2069 7320 6e6f 7420 5363 616e 7333 3030   is not Scans300
+00001480: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00001490: 2020 2073 656c 662e 7363 616e 203d 2053     self.scan = S
+000014a0: 6361 6e73 3330 3028 7365 6c66 290d 0a20  cans300(self).. 
+000014b0: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
+000014c0: 2e5f 6d5f 6d61 7820 3e3d 2032 3030 3a0d  ._m_max >= 200:.
+000014d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000014e0: 662e 5f6d 5f6d 6178 203d 2032 3030 0d0a  f._m_max = 200..
+000014f0: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+00001500: 7970 6528 7365 6c66 2e73 6361 6e29 2069  ype(self.scan) i
+00001510: 7320 6e6f 7420 5363 616e 7332 3030 3a0d  s not Scans200:.
+00001520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001530: 2073 656c 662e 7363 616e 203d 2053 6361   self.scan = Sca
+00001540: 6e73 3230 3028 7365 6c66 290d 0a20 2020  ns200(self)..   
+00001550: 2020 2020 2065 6c69 6620 7365 6c66 2e5f       elif self._
+00001560: 6d5f 6d61 7820 3e3d 2031 3030 3a0d 0a20  m_max >= 100:.. 
+00001570: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00001580: 5f6d 5f6d 6178 203d 2031 3030 0d0a 2020  _m_max = 100..  
+00001590: 2020 2020 2020 2020 2020 6966 2074 7970            if typ
+000015a0: 6528 7365 6c66 2e73 6361 6e29 2069 7320  e(self.scan) is 
+000015b0: 6e6f 7420 5363 616e 733a 0d0a 2020 2020  not Scans:..    
+000015c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000015d0: 2e73 6361 6e20 3d20 5363 616e 7328 7365  .scan = Scans(se
+000015e0: 6c66 290d 0a20 2020 2020 2020 2072 6574  lf)..        ret
+000015f0: 7572 6e20 7365 6c66 2e5f 6d6f 6465 6c5f  urn self._model_
+00001600: 6e61 6d65 2c20 7365 6c66 2e5f 7365 7269  name, self._seri
+00001610: 616c 5f6e 756d 6265 722c 2073 656c 662e  al_number, self.
+00001620: 5f66 6972 6d77 6172 655f 7665 7273 696f  _firmware_versio
+00001630: 6e0d 0a0d 0a20 2020 2064 6566 2067 6574  n....    def get
+00001640: 5f73 7461 7475 7328 7365 6c66 293a 0d0a  _status(self):..
+00001650: 2020 2020 2020 2020 7374 6174 7573 5f73          status_s
+00001660: 7472 696e 6720 3d20 2745 6d69 7373 696f  tring = 'Emissio
+00001670: 6e20 6375 7272 656e 743a 207b 3a2e 3266  n current: {:.2f
+00001680: 7d20 6d41 5c6e 272e 666f 726d 6174 2873  } mA\n'.format(s
+00001690: 656c 662e 696f 6e69 7a65 722e 656d 6973  elf.ionizer.emis
+000016a0: 7369 6f6e 5f63 7572 7265 6e74 290d 0a20  sion_current).. 
+000016b0: 2020 2020 2020 2073 7461 7475 735f 7374         status_st
+000016c0: 7269 6e67 202b 3d20 2743 454d 2048 563a  ring += 'CEM HV:
+000016d0: 207b 3a2e 3066 7d20 565c 6e27 2e66 6f72   {:.0f} V\n'.for
+000016e0: 6d61 7428 7365 6c66 2e63 656d 2e76 6f6c  mat(self.cem.vol
+000016f0: 7461 6765 290d 0a20 2020 2020 2020 2073  tage)..        s
+00001700: 7461 7475 735f 7374 7269 6e67 202b 3d20  tatus_string += 
+00001710: 7365 6c66 2e73 7461 7475 732e 6765 745f  self.status.get_
+00001720: 6572 726f 725f 7465 7874 2829 0d0a 2020  error_text()..  
+00001730: 2020 2020 2020 7265 7475 726e 2073 7461        return sta
+00001740: 7475 735f 7374 7269 6e67 0d0a 0d0a 2020  tus_string....  
+00001750: 2020 6465 6620 6861 6e64 6c65 5f63 6f6d    def handle_com
+00001760: 6d61 6e64 2873 656c 662c 2063 6d64 5f73  mand(self, cmd_s
+00001770: 7472 696e 673a 2073 7472 293a 0d0a 2020  tring: str):..  
+00001780: 2020 2020 2020 636d 6420 3d20 636d 645f        cmd = cmd_
+00001790: 7374 7269 6e67 2e75 7070 6572 2829 0d0a  string.upper()..
+000017a0: 2020 2020 2020 2020 7265 706c 7920 3d20          reply = 
+000017b0: 2727 0d0a 2020 2020 2020 2020 6966 2027  ''..        if '
+000017c0: 3f27 2069 6e20 636d 6420 6f72 2063 6d64  ?' in cmd or cmd
+000017d0: 2e73 7461 7274 7377 6974 6828 2246 4c22  .startswith("FL"
+000017e0: 2920 6f72 2063 6d64 2e73 7461 7274 7377  ) or cmd.startsw
+000017f0: 6974 6828 2248 5622 2920 6f72 205c 0d0a  ith("HV") or \..
+00001800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001810: 636d 642e 7374 6172 7473 7769 7468 2822  cmd.startswith("
+00001820: 5646 2229 206f 7220 636d 642e 7374 6172  VF") or cmd.star
+00001830: 7473 7769 7468 2822 4545 2229 5c0d 0a20  tswith("EE")\.. 
+00001840: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00001850: 7220 636d 642e 7374 6172 7473 7769 7468  r cmd.startswith
+00001860: 2822 4945 2229 206f 7220 636d 642e 7374  ("IE") or cmd.st
+00001870: 6172 7473 7769 7468 2822 494e 2229 3a0d  artswith("IN"):.
+00001880: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
+00001890: 6c79 203d 2073 656c 662e 7175 6572 795f  ly = self.query_
+000018a0: 7465 7874 2863 6d64 292e 7374 7269 7028  text(cmd).strip(
+000018b0: 290d 0a20 2020 2020 2020 2065 6c69 6620  )..        elif 
+000018c0: 636d 642e 7374 6172 7473 7769 7468 2822  cmd.startswith("
+000018d0: 4d52 2229 3a0d 0a20 2020 2020 2020 2020  MR"):..         
+000018e0: 2020 2023 2073 656c 662e 7365 6e64 2863     # self.send(c
+000018f0: 6d64 290d 0a20 2020 2020 2020 2020 2020  md)..           
+00001900: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
+00001910: 2020 2020 2020 206d 6173 7320 3d20 696e         mass = in
+00001920: 7428 636d 645b 323a 5d2e 7374 7269 7028  t(cmd[2:].strip(
+00001930: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00001940: 2020 2020 696e 7465 6e73 6974 7920 3d20      intensity = 
+00001950: 7365 6c66 2e73 6361 6e2e 6765 745f 7369  self.scan.get_si
+00001960: 6e67 6c65 5f6d 6173 735f 7363 616e 286d  ngle_mass_scan(m
+00001970: 6173 7329 2020 2320 7265 6164 5f6c 6f6e  ass)  # read_lon
+00001980: 6728 290d 0a20 2020 2020 2020 2020 2020  g()..           
+00001990: 2020 2020 2072 6570 6c79 203d 2073 7472       reply = str
+000019a0: 2869 6e74 656e 7369 7479 290d 0a20 2020  (intensity)..   
+000019b0: 2020 2020 2020 2020 2065 7863 6570 743a           except:
+000019c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000019d0: 2020 7061 7373 0d0a 2020 2020 2020 2020    pass..        
+000019e0: 656c 6966 2063 6d64 2e73 7461 7274 7377  elif cmd.startsw
+000019f0: 6974 6828 2253 4322 2920 616e 6420 6c65  ith("SC") and le
+00001a00: 6e28 636d 6429 203c 2031 303a 0d0a 2020  n(cmd) < 10:..  
+00001a10: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00001a20: 6361 6e2e 6765 745f 616e 616c 6f67 5f73  can.get_analog_s
+00001a30: 6361 6e28 290d 0a20 2020 2020 2020 2020  can()..         
+00001a40: 2020 2072 6570 6c79 203d 2022 5363 616e     reply = "Scan
+00001a50: 2043 6f6d 706c 6574 6564 220d 0a20 2020   Completed"..   
+00001a60: 2020 2020 2065 6c69 6620 636d 642e 7374       elif cmd.st
+00001a70: 6172 7473 7769 7468 2822 4853 2229 3a0d  artswith("HS"):.
+00001a80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00001a90: 662e 7363 616e 2e67 6574 5f68 6973 746f  f.scan.get_histo
+00001aa0: 6772 616d 5f73 6361 6e28 290d 0a20 2020  gram_scan()..   
+00001ab0: 2020 2020 2020 2020 2072 6570 6c79 203d           reply =
+00001ac0: 2022 5363 616e 2043 6f6d 706c 6574 6564   "Scan Completed
+00001ad0: 220d 0a20 2020 2020 2020 2065 6c73 653a  "..        else:
+00001ae0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00001af0: 6c66 2e73 656e 6428 636d 6429 0d0a 2020  lf.send(cmd)..  
+00001b00: 2020 2020 2020 7265 7475 726e 2072 6570        return rep
+00001b10: 6c79 0d0a 0d0a 2020 2020 6465 6620 7265  ly....    def re
+00001b20: 7365 7428 7365 6c66 293a 0d0a 2020 2020  set(self):..    
+00001b30: 2020 2020 7365 6c66 2e71 7565 7279 5f74      self.query_t
+00001b40: 6578 7428 2249 4e32 2229 0d0a 0d0a 2020  ext("IN2")....  
+00001b50: 2020 2320 466f 7220 5247 4131 3030 2c20    # For RGA100, 
+00001b60: 2052 5332 3332 2044 5352 206c 696e 6520   RS232 DSR line 
+00001b70: 7368 6f75 6c64 2062 6520 6869 6768 2069  should be high i
+00001b80: 6620 5253 3233 3220 6361 626c 6520 6973  f RS232 cable is
+00001b90: 2063 6f6e 6e65 6374 6564 0d0a 2020 2020   connected..    
+00001ba0: 6465 6620 6368 6563 6b5f 6865 6164 5f6f  def check_head_o
+00001bb0: 6e6c 696e 6528 7365 6c66 293a 0d0a 2020  nline(self):..  
+00001bc0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00001bd0: 2020 2043 6865 636b 2069 6620 5352 5320     Check if SRS 
+00001be0: 5247 4120 6973 2063 6f6e 6e65 6374 6564  RGA is connected
+00001bf0: 2074 6f20 6120 636f 6d6d 756e 6963 6174   to a communicat
+00001c00: 696f 6e20 696e 7374 6572 6661 6365 0d0a  ion insterface..
+00001c10: 0d0a 2020 2020 2020 2020 466f 7220 7365  ..        For se
+00001c20: 7269 616c 2063 6f6d 6d75 6e69 6361 7469  rial communicati
+00001c30: 6f6e 2c20 6974 2063 6865 636b 2066 6f72  on, it check for
+00001c40: 2044 5352 206c 696e 6520 6672 6f6d 2053   DSR line from S
+00001c50: 5253 2052 4741 2069 7320 7365 7420 6869  RS RGA is set hi
+00001c60: 6768 2e0d 0a20 2020 2020 2020 2046 6f72  gh...        For
+00001c70: 2045 7468 6572 6e65 7420 636f 6d6d 756e   Ethernet commun
+00001c80: 6963 6174 696f 6e2c 2069 7420 6368 6563  ication, it chec
+00001c90: 6b20 6966 2074 6865 2054 4350 2073 6f63  k if the TCP soc
+00001ca0: 6b65 7420 6973 206f 7065 6e2e 0d0a 2020  ket is open...  
+00001cb0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00001cc0: 2020 2069 6620 7365 6c66 2e63 6f6d 6d2e     if self.comm.
+00001cd0: 7479 7065 203d 3d20 5365 7269 616c 496e  type == SerialIn
+00001ce0: 7465 7266 6163 652e 4e41 4d45 3a0d 0a20  terface.NAME:.. 
+00001cf0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00001d00: 6e20 7365 6c66 2e63 6f6d 6d2e 5f73 6572  n self.comm._ser
+00001d10: 6961 6c2e 6473 720d 0a20 2020 2020 2020  ial.dsr..       
+00001d20: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00001d30: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00001d40: 6973 5f63 6f6e 6e65 6374 6564 2829 0d0a  is_connected()..
+00001d50: 0d0a 2020 2020 6465 6620 6765 745f 6d61  ..    def get_ma
+00001d60: 785f 6d61 7373 2873 656c 6629 3a0d 0a20  x_mass(self):.. 
+00001d70: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00001d80: 2020 2020 4765 7420 6d61 7869 6d75 6d20      Get maximum 
+00001d90: 6d61 7373 2074 6861 7420 6361 6e20 6265  mass that can be
+00001da0: 2075 7365 6420 666f 7220 6120 7363 616e   used for a scan
+00001db0: 0d0a 0d0a 2020 2020 2020 2020 5352 5320  ....        SRS 
+00001dc0: 5247 4131 3030 206d 6f64 656c 2068 6173  RGA100 model has
+00001dd0: 2074 6865 206d 6178 696d 756d 206d 6173   the maximum mas
+00001de0: 7320 6f66 2031 3030 2041 4d55 3b0d 0a20  s of 100 AMU;.. 
+00001df0: 2020 2020 2020 2053 5253 2052 4741 3230         SRS RGA20
+00001e00: 302c 2032 3030 2041 4d55 3b20 616e 6420  0, 200 AMU; and 
+00001e10: 5352 5320 5247 4133 3030 2c20 3330 3020  SRS RGA300, 300 
+00001e20: 414d 552e 0d0a 0d0a 2020 2020 2020 2020  AMU.....        
+00001e30: 5265 7475 726e 730d 0a20 2020 2020 2020  Returns..       
+00001e40: 202d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020   --------..     
+00001e50: 2020 2020 2020 2069 6e74 0d0a 2020 2020         int..    
+00001e60: 2020 2020 2020 2020 2020 2020 6d61 7869              maxi
+00001e70: 6d75 6d20 6d61 7373 0d0a 2020 2020 2020  mum mass..      
+00001e80: 2020 2222 220d 0a20 2020 2020 2020 2072    """..        r
+00001e90: 6574 7572 6e20 7365 6c66 2e5f 6d5f 6d61  eturn self._m_ma
+00001ea0: 780d 0a0d 0a20 2020 2064 6566 2063 616c  x....    def cal
+00001eb0: 6962 7261 7465 5f61 6c6c 2873 656c 6629  ibrate_all(self)
+00001ec0: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00001ed0: 2020 2020 2020 2020 4361 6c69 6272 6174          Calibrat
+00001ee0: 6520 616c 6c0d 0a0d 0a20 2020 2020 2020  e all....       
+00001ef0: 2072 6574 7572 6e73 0d0a 2020 2020 2020   returns..      
+00001f00: 2020 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020    --------..    
+00001f10: 2020 2020 2020 2020 696e 740d 0a20 2020          int..   
+00001f20: 2020 2020 2020 2020 2020 2020 2045 7272               Err
+00001f30: 6f72 2073 7461 7475 7320 6279 7465 2061  or status byte a
+00001f40: 6674 6572 2063 616c 6962 7261 7469 6f6e  fter calibration
+00001f50: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00001f60: 2020 2020 2020 2072 6570 6c79 203d 2073         reply = s
+00001f70: 656c 662e 636f 6d6d 2e71 7565 7279 5f74  elf.comm.query_t
+00001f80: 6578 745f 7769 7468 5f6c 6f6e 675f 7469  ext_with_long_ti
+00001f90: 6d65 6f75 7428 2243 4122 2c20 3132 3029  meout("CA", 120)
+00001fa0: 0d0a 2020 2020 2020 2020 6572 726f 725f  ..        error_
+00001fb0: 7374 6174 7573 203d 2069 6e74 2872 6570  status = int(rep
+00001fc0: 6c79 290d 0a20 2020 2020 2020 2072 6574  ly)..        ret
+00001fd0: 7572 6e20 6572 726f 725f 7374 6174 7573  urn error_status
+00001fe0: 0d0a 0d0a 2020 2020 6465 6620 6361 6c69  ....    def cali
+00001ff0: 6272 6174 655f 656c 6563 7472 6f6d 6574  brate_electromet
+00002000: 6572 2873 656c 6629 3a0d 0a20 2020 2020  er(self):..     
+00002010: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00002020: 4361 6c69 6272 6174 6520 656c 6563 7472  Calibrate electr
+00002030: 6f6d 6574 6572 2773 2049 2d56 2072 6573  ometer's I-V res
+00002040: 706f 6e73 650d 0a0d 0a20 2020 2020 2020  ponse....       
+00002050: 2072 6574 7572 6e73 0d0a 2020 2020 2020   returns..      
+00002060: 2020 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020    --------..    
+00002070: 2020 2020 2020 2020 696e 740d 0a20 2020          int..   
+00002080: 2020 2020 2020 2020 2020 2020 2045 7272               Err
+00002090: 6f72 2073 7461 7475 7320 6279 7465 2061  or status byte a
+000020a0: 6674 6572 2063 616c 6962 7261 7469 6f6e  fter calibration
+000020b0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+000020c0: 2020 2020 2020 2072 6570 6c79 203d 2073         reply = s
+000020d0: 656c 662e 636f 6d6d 2e71 7565 7279 5f74  elf.comm.query_t
+000020e0: 6578 745f 7769 7468 5f6c 6f6e 675f 7469  ext_with_long_ti
+000020f0: 6d65 6f75 7428 2243 4c22 2c20 3132 3029  meout("CL", 120)
+00002100: 0d0a 2020 2020 2020 2020 6572 726f 725f  ..        error_
+00002110: 7374 6174 7573 203d 2069 6e74 2872 6570  status = int(rep
+00002120: 6c79 290d 0a20 2020 2020 2020 2072 6574  ly)..        ret
+00002130: 7572 6e20 6572 726f 725f 7374 6174 7573  urn error_status
+00002140: 0d0a 0d0a 2020 2020 616c 6c6f 775f 7275  ....    allow_ru
+00002150: 6e5f 6275 7474 6f6e 203d 205b 7265 7365  n_button = [rese
+00002160: 742c 2063 616c 6962 7261 7465 5f61 6c6c  t, calibrate_all
+00002170: 2c20 6361 6c69 6272 6174 655f 656c 6563  , calibrate_elec
+00002180: 7472 6f6d 6574 6572 5d0d 0a0d 0a         trometer]....
```

### Comparing `srsinst.rga-0.2.9/srsinst/rga/instruments/rga100/scans.py` & `srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/scans.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,34 @@
+##! 
+##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
 
 import time
 import numpy as np
 
 from srsgui.inst.communications import Interface, SerialInterface, TcpipInterface
 from srsgui.inst.component import Component
 from srsgui.inst.commands import IntGetCommand
 
 from .commands import IntNSCommand
 
+
 class Scans(Component):
+    MaxMass = 100
     """
-    It contains implementation of setup and data acquisition from SRS RGAs
+    Component for scan setup and data acquisition from SRS RGAs
     """
 
-    initial_mass = IntNSCommand('MI')
-    final_mass = IntNSCommand('MF')
-    speed = IntNSCommand('NF')
-    resolution = IntNSCommand('SA')
-    total_points_analog = IntGetCommand('AP')
-    total_points_histogram = IntGetCommand('HP')
+    initial_mass = IntNSCommand('MI', 'AMU', 1, MaxMass, 1, 1)
+    final_mass = IntNSCommand('MF', 'AMU', 1, MaxMass, 1, MaxMass)
+    speed = IntNSCommand('NF', '', 0, 7, 1, 4)
+    resolution = IntNSCommand('SA', 'points/AMU', 10, 25, 1, 10)
+    total_points_analog = IntGetCommand('AP', 'points')
+    total_points_histogram = IntGetCommand('HP', 'points')
 
     def __init__(self, parent):
         super().__init__(parent)
 
         self.scan_type = None
 
         self.mass_axis = np.array([], dtype=np.double)
@@ -295,7 +301,24 @@
         c = np.polyfit(x1, y1, 2)  # fit the points around the max
         roots = np.roots(c)
         pp = (roots[0] + roots[1]) / 2.0  # peak position
         pp = pp.real
         pi = np.polyval(c, pp)  # c[0] + c[1] * pp + c[2] * pp ** 2  # peak intensity
         return pi
 
+
+class Scans200(Scans):
+    MaxMass = 200
+    """
+    Scans for RGA200
+    """
+    initial_mass = IntNSCommand('MI', 'AMU', 1, MaxMass, 1, 1)
+    final_mass = IntNSCommand('MF', 'AMU', 1, MaxMass, 1, MaxMass)
+
+
+class Scans300(Scans):
+    MaxMass = 300
+    """
+    Scans for RGA200
+    """
+    initial_mass = IntNSCommand('MI', 'AMU', 1, MaxMass, 1, 1)
+    final_mass = IntNSCommand('MF', 'AMU', 1, MaxMass, 1, MaxMass)
```

### Comparing `srsinst.rga-0.2.9/srsinst/rga/instruments/rga100/sicp.py` & `srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/sicp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+##! 
+##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
+
 """
 SRS Internet Configuration Protocol (SICP) class
 
 The RGA120 series and RGA Ethernet Adapter (REA) use the IP configuration over UDP broadcasting, SRS IP Configuration protocol (SICP). When a search
 packet is broadcasted, all SICP enabled devices on the Local Area Network (LAN)
 will respond with a packet. From those packets, you can find available devices
 on the network.
```

### Comparing `srsinst.rga-0.2.9/srsinst/rga/plots/analogscanplot.py` & `srsinst.rga-0.3.0/srsinst/rga/plots/analogscanplot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+##! 
+##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
+
 import time
 import logging
 from matplotlib.axes import Axes
 from srsgui import Task
 from srsinst.rga.plots.basescanplot import BaseScanPlot
 from srsinst.rga.plots.analysis import calculate_baseline
 from srsinst.rga.instruments.rga100.scans import Scans
```

### Comparing `srsinst.rga-0.2.9/srsinst/rga/plots/analysis.py` & `srsinst.rga-0.3.0/srsinst/rga/plots/analysis.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+##! 
+##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
 
 import numpy as np
 from numpy.linalg import norm
 
 from scipy import sparse
 from scipy.sparse import linalg
 
@@ -10,16 +14,39 @@
     """
     Calculate baseline of a spectrum based on
     Asymmetrically reweighted penalized least square (ARPLS)
 
     Original paper:
     https://pubs.rsc.org/en/content/articlelanding/2015/AN/C4AN01061B#!divAbstract
 
-    Python implementation
+    Python implementation:
     https://stackoverflow.com/questions/29156532/python-baseline-correction-library
+
+    Parameters
+    -----------
+        y: Numpy array
+            Intensity array
+        ratio: float
+            improvement ratio to reach before stopping iteration
+        lam: float
+            fit parameter lambda
+        niter: int
+            maximum iteration
+        full_output: bool, optional
+            generate detailed output
+
+    Returns
+    --------
+        Numpy array
+            baseline array, if full_output == False
+        tuple
+            (baseline array, baseline-subtracted intensity array,
+            termination information in dict format),
+            if full_output == True
+
     """
     L = len(y)
 
     diag = np.ones(L - 2)
     D = sparse.spdiags([diag, -2 * diag, diag], [0, -1, -2], L, L - 2)
 
     H = lam * D.dot(D.T)  # The transposes are flipped w.r.t the Algorithm on pg. 252
@@ -54,21 +81,42 @@
         info = {'num_iter': count, 'stop_criterion': crit}
         return z, d, info
     else:
         return z
 
 
 def get_peak_from_analog_scan(x, y, mass, fit=False):
+    """
+    Calculate a peak intensity from an analog scan spectrum
+
+    Parameters
+    -----------
+        x: Numpy array
+            mass axis values
+        y: Numpy array
+            intensity array
+        mass: float
+            peak position within the range of x
+        fit: bool, optional
+            The default is False, if False, return the maximum value around mass.
+            If True , it fits the data around x with a parabola, and calculate
+            the maximum of the parabola.
+    Returns
+    --------
+        float
+            peak intensity
+    """
     distance = 0.5
     m = np.where((x > mass - distance) & (x < mass + distance))[0]
     if len(m) < 5:
         return 0.0
     p = np.max(y[m])
     if not fit:
         return p
+
     arg = m[0] + np.argmax(y[m])
     x1 = x[arg - 2:arg + 4]
     y1 = y[arg - 2:arg + 4]
     c = np.polyfit(x1, y1, 2)  # fit the points around the max
     roots = np.roots(c)
     pp = (roots[0] + roots[1]) / 2.0  # peak position
     pp = pp.real
```

### Comparing `srsinst.rga-0.2.9/srsinst/rga/plots/basescanplot.py` & `srsinst.rga-0.3.0/srsinst/rga/plots/basescanplot.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+##! 
+##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
 
 import time
 import logging
 from matplotlib.axes import Axes
 from srsgui import Task
 
 logger = logging.getLogger(__name__)
```

### Comparing `srsinst.rga-0.2.9/srsinst/rga/plots/histogramscanplot.py` & `srsinst.rga-0.3.0/srsinst/rga/plots/histogramscanplot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+##! 
+##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
 
 import logging
 import numpy
 from matplotlib.axes import Axes
 from srsgui import Task
 from srsinst.rga.plots.basescanplot import BaseScanPlot
```

### Comparing `srsinst.rga-0.2.9/srsinst/rga/plots/timeplot.py` & `srsinst.rga-0.3.0/srsinst/rga/plots/timeplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+##! 
+##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
 
 import time
 import logging
 import numpy as np
 from datetime import datetime, timedelta
 from matplotlib.axes import Axes
 from srsgui import Task
@@ -43,15 +47,15 @@
         self.lines = {}
 
         self._data_buffer_size = 1000000  # Maximum data points per line
         self.data_points = 0  # Current data points in data buffer
         self.max_points_in_plot = 10000  # Maximum point to plot
 
         if self.use_datetime:
-            self.time = np.zeros(self._data_buffer_size).astype('datetime64[s]')
+            self.time = np.zeros(self._data_buffer_size).astype('datetime64[ms]')
         else:
             self.time = np.zeros(self._data_buffer_size, dtype=np.float64)
 
         for key in self.data_keys:
             self.data[key] = np.zeros(self._data_buffer_size)
             self.lines[key], = self.ax.plot([1.0], [1.0], label=key)
```

### Comparing `srsinst.rga-0.2.9/srsinst/rga/rga.taskconfig` & `srsinst.rga-0.3.0/srsinst/rga/rga.taskconfig`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 # Line that starts with '#' is a comment line
-# MyRGA Task list for srsgui
+# RGA Task list for srsgui
 
 # The name is used for the main window title
 
-Name: My RGA Tasks
+Name: RGA Tasks
 
 
 # Specify Instruments used in the task suite
-# A line that starts with 'inst' adds an instrument to be used in the following tasks
-# an instrument is a subclass derived from Instrument class in 'rga' package
-# The second column is the Python module or package that contains the instrument class.
+# A line that starts with 'inst' adds an instrument to be used in the following tasks.
+# An instrument is a subclass derived from Instrument class in 'srsgui' package
+# The second column is the name of the Python module or package that contains the instrument class.
 # The third column is a instrument class in the module
 # The fourth column is connection parameters.
-# if given, the instrument will be connected using the parameters when the config file is loaded.
+# If the fourth item is given, the instrument will be connected using the parameters 
+# when the config file is loaded.
 
 inst: rga,      srsinst.rga,    RGA100
 # inst: rga2,   srsinst.rga,    RGA100,    tcpip:172.25.40.37:admin:admin:818
 # inst: rga3,   srsinst.rga,    RGA100,    serial:com3:28800:True
 
 
-# A line that starts with 'task: ' adds a task to the task config file.
+# A line that starts with 'task: ' adds a task to the srsgui application.
 # The first column is the task name that will be used as a dictionary key
-# of the task, displayed in GUI Tak menu for selection, and used in task result data file.
-# The Second column is the Python module that contains the task class with relative path from the Task config file.
-# The third column is a task class  that is a Task subclass in the module.
+# of the task, displayed in GUI Tasks menu for selection, and used in task result data file.
+# The Second column is the name of the Python module that contains the task class 
+# with relative path from the Task config file.
+# The third column is the name of a Task subclass in the module.
 
 task: Search LAN for RGAs,         srsinst.rga.tasks.searchlan,                   SearchLanTask
 task: Filament Control,            srsinst.rga.tasks.filamentcontroltask,         FilamentControlTask
 task: CEM Control,                 srsinst.rga.tasks.cemcontroltask,              CEMControlTask
+task: CEM Gain Tuning,             srsinst.rga.tasks.cemgaintask,                 CEMGainTask
 task: Analog Scan,                 srsinst.rga.tasks.analogscantask,              AnalogScanTask
 task: Histogram Scan,              srsinst.rga.tasks.histogramscantask,           HistogramScanTask
 task: Pressure vs. Time Scan,      srsinst.rga.tasks.pvstscantask,                PvsTScanTask
 task: Derived P vs. T Scan,        srsinst.rga.tasks.derivedpvstscantask,         DerivedPvsTScanTask
 task: Composition analysis scan,   srsinst.rga.tasks.compositionanalysistask,     CompositionAnalysisTask
-task: CEM Gain Tuning,             srsinst.rga.tasks.cemgaintask,                 CEMGainTask
+
+
```

### Comparing `srsinst.rga-0.2.9/srsinst/rga/tasks/analogscantask.py` & `srsinst.rga-0.3.0/srsinst/rga/tasks/analogscantask.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,25 @@
+##! 
+##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
 
 from srsgui import Task
-from srsgui.task.inputs import ListInput, IntegerInput, InstrumentInput
-
-from srsinst.rga.plots.analogscanplot import AnalogScanPlot
+from srsgui import ListInput, IntegerInput, InstrumentInput
+from srsinst.rga import AnalogScanPlot
 
 # get_rga is imported from the path relative to the .taskconfig file
 from instruments import get_rga
 
 
 class AnalogScanTask(Task):
-    """Task to run analog scans.
     """
+    Task to run analog scans.
+    """
+
     InstrumentName = 'instrument to control'
     StartMass = 'start mass'
     StopMass = 'stop mass'
     ScanSpeed = 'scan speed'
     StepSize = 'step per AMU'
     IntensityUnit = 'intensity unit'
 
@@ -33,29 +38,30 @@
         self.params = self.get_all_input_parameters()
 
         # Get logger to use
         self.logger = self.get_logger(__name__)
 
         self.init_scan()
 
-        # Set up an analog scan plot for the test
+        # Set up an analog scan plot
         self.ax = self.get_figure().add_subplot(111)
         self.plot = AnalogScanPlot(self, self.ax, self.rga.scan, 'Analog Scan')
 
         if self.params[self.IntensityUnit] == 0:
             self.conversion_factor = 0.1
             self.plot.set_conversion_factor(self.conversion_factor, 'fA')
         else:
             self.conversion_factor = self.rga.pressure.get_partial_pressure_sensitivity_in_torr()
             self.plot.set_conversion_factor(self.conversion_factor, 'Torr')
 
     def init_scan(self):
         # Get the instrument to use
         self.rga = get_rga(self, self.params[self.InstrumentName])
         self.id_string = self.rga.status.id_string
+
         emission_current = self.rga.ionizer.emission_current
         cem_voltage = self.rga.cem.voltage
 
         self.logger.info('Emission current: {:.2f} mA CEM HV: {} V'.format(emission_current, cem_voltage))
         self.rga.scan.set_parameters(self.params[self.StartMass],
                                      self.params[self.StopMass],
                                      self.params[self.ScanSpeed],
@@ -67,21 +73,21 @@
 
         while self.is_running():
             try:
                 self.rga.scan.get_analog_scan()
             except Exception as e:
                 self.set_task_passed(False)
                 self.logger.error('{}: {}'.format(e.__class__.__name__, e))
-                if not self.rga.is_connected():
+                if not self.rga.is_connected():  # Check if RGA is connected.
                     self.logger.error('"{}" is disconnected'.format(self.params[self.InstrumentName]))
                     break
 
     def cleanup(self):
         self.logger.info('Task finished')
-        self.plot.cleanup() # Detach callback functions
+        self.plot.cleanup()  # Detach callback functions used in the plot
 
 
 if __name__ == '__main__':
     import time
     import logging
 
     from srsinst.rga import RGA100 as Rga
```

### Comparing `srsinst.rga-0.2.9/srsinst/rga/tasks/cemcontroltask.py` & `srsinst.rga-0.3.0/srsinst/rga/tasks/cemcontroltask.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+##! 
+##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
 
 from srsgui import Task
-from srsgui.task.inputs import ListInput, InstrumentInput
+from srsgui import ListInput, InstrumentInput
 
 # get_rga is imported from the path relative to the .taskconfig file
 from instruments import get_rga
 
 
 class CEMControlTask(Task):
     """Task to set CEM voltage
```

### Comparing `srsinst.rga-0.2.9/srsinst/rga/tasks/cemgaintask.py` & `srsinst.rga-0.3.0/srsinst/rga/tasks/cemgaintask.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+##! 
+##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
+
 import sys
 import math
 import time
 import math
 import numpy as np
 
 from srsgui import Task
-from srsgui.task.inputs import FloatInput, IntegerInput, InstrumentInput
+from srsgui import IntegerInput, InstrumentInput
 
 # get_rga is imported from the path relative to the .taskconfig file
 from instruments import get_rga
 
 
 class CEMGainTask(Task):
     """Task to measure CEM gain at different CEM voltage
@@ -43,21 +48,27 @@
 
         self.data_dict['t'] = []  # time
         self.data_dict['i'] = []  # intensity
 
         # Get value to use for test from input_parameters
         self.params = self.get_all_input_parameters()
         self.mass_to_measure_value = self.get_input_parameter(self.MassToMeasure)
+        self.wait_time_value = self.get_input_parameter(self.WaitTime)
+
+        # minimum Faraday cup ion current to run calibration
+        self.minimum_intensity = 200.0  # fA
+
         self.start_voltage_value = 800
         self.stop_voltage_value = 2000
         self.step_voltage_value = 160
 
-        self.wait_time_value = self.get_input_parameter(self.WaitTime)
+        self.init_plot()
+        self.init_rga()
 
-        # initialize Plot
+    def init_plot(self):
         self.ax1 = self.figure.add_subplot(121)
         self.ax1.set_title(self.__class__.__name__)
         self.ax1.set_xlabel("CEM HV (V)")
         self.ax1.set_ylabel('Gain')
 
         self.line1, = self.ax1.plot(self.data_dict['x'], self.data_dict['y'])
         self.ax1.set_xlim(self.start_voltage_value, self.stop_voltage_value, auto=False)
@@ -65,50 +76,51 @@
         self.ax1.set_yscale('log')
 
         self.ax2 = self.figure.add_subplot(122)
         self.ax2.set_title('Ion current measurement')
         self.ax2.set_xlabel("Time (s)")
         self.ax2.set_ylabel('Intensity (0.1fA)')
         self.line2, = self.ax2.plot(self.data_dict['t'], self.data_dict['i'])
-        self.ax2.set_xlim(0, 5)
+        self.ax2.set_xlim(0, self.wait_time_value * 1.2)
         self.ax2.set_ylim(10, 1e9)
         self.ax2.set_yscale('log')
 
-        # Initialize RGA
+    def init_rga(self):
         self.rga = get_rga(self, self.params[self.InstrumentName])
         print(self.rga.status.id_string)
         self.id_string = self.rga.status.id_string
         self.old_speed = self.rga.scan.speed
         self.old_hv = self.rga.cem.voltage
 
     def test(self):
         self.rga.scan.speed = self.params[self.ScanSpeed]
         self.rga.cem.voltage = 0
 
+        # Measure Faraday cup ion current as a reference
         rep = 4
-        minimum_intensity = 200.0  # fA
         total = self.measure_intensity_with_delay(self.params[self.WaitTime])
-
         for i in range(rep):
             total += self.measure_intensity_with_delay(0.0)
         fc_intensity = total / (rep + 1)
 
-        if fc_intensity < minimum_intensity:  # if smaller than minimum_intensity 
-            raise ValueError('FC reading {:.2f} is smaller than {} fA. Need more intensity to calibrate'.format(
-                fc_intensity, minimum_intensity))
+        if fc_intensity < self.minimum_intensity:  # if smaller than minimum_intensity
+            raise ValueError('FC reading {:.2f} fA is smaller than {} fA. Need more intensity to calibrate'.format(
+                fc_intensity, self.minimum_intensity))
 
-        self.logger.info('FC reading is {} fA at {} AMU and NF= {}'.format(
+        self.logger.info('FC reading is {:.2f} fA at {} AMU and NF= {}'.format(
             fc_intensity, self.mass_to_measure_value, self.params[self.ScanSpeed]
         ))
 
-        current_voltage = self.start_voltage_value
-        gain = 0
-
+        # Create a table to save data
         table_name = 'Gain vs. HV'
         self.create_table(table_name, 'CEM HV (V)', 'Gain')
+
+        # Loop to measure CEM gains
+        current_voltage = self.start_voltage_value
+        gain = 0
         while (current_voltage <= self.stop_voltage_value) and \
               (gain < self.params[self.GainToSet]):
             if not self.is_running():
                 break
             start_time = time.time()
             elapsed_time = 0
             self.data_dict['t'] = []
@@ -121,62 +133,70 @@
                 elapsed_time = time.time() - start_time
                 intensity = self.rga.scan.get_single_mass_scan(self.mass_to_measure_value) / 10.0
                 self.data_dict['t'].append(elapsed_time)
                 self.data_dict['i'].append(intensity)
                 self.notify_data_available(self.data_dict)
 
             gain = self.data_dict['i'][-1] / fc_intensity
+            gain_ratio = self.params[self.GainToSet] / gain
+
             self.data_dict['x'].append(current_voltage)
             self.data_dict['y'].append(gain)
 
             self.notify_data_available(self.data_dict)
 
-            gain_ratio = self.params[self.GainToSet] / gain
+            self.add_data_to_table(table_name, round(current_voltage, 0), round(gain, 1))
+            self.logger.info(f'CEM voltage: {current_voltage} Gain: {gain:.1f} Gain ratio: {gain_ratio:.1f}')
 
+            # Calculate the next CEM voltage
             if gain_ratio > 20 or gain < 0:
                 voltage_ratio = 1.16
             elif gain_ratio > 5:
                 voltage_ratio = 1.08
             elif gain_ratio > 2.5:
                 voltage_ratio = 1.04
             else:
                 voltage_ratio = 1.02
-
-            self.add_data_to_table(table_name, round(current_voltage, 0), round(gain, 1))
-            self.logger.info(f'CEM voltage: {current_voltage} Gain: {gain:.1f} Gain ratio: {gain_ratio:.1f}')
             current_voltage = int(current_voltage * voltage_ratio)
 
+        # Interpolate the CEM voltage from of measured data
         log_gain = math.log10(self.params[self.GainToSet])
         self.data_dict['log_y'] = [math.log10(a) if a > 0 else 0.001 for a in self.data_dict['y']]
         hv_to_set = int(np.interp(log_gain, self.data_dict['log_y'], self.data_dict['x']))
         self.logger.info(f'HV for gain {self.params[self.GainToSet]} : {hv_to_set:.0f}')
 
+        # Measure the gain at the calculated CEM voltage
         measured_gain = self.measure_gain_at_voltage(hv_to_set)
         self.logger.info(f'Measured gain at HV {hv_to_set:.0f} V : {measured_gain:.0f}')
 
+        # If the gain error is larger than 10 %, set it to fail
         error = abs(measured_gain - self.params[self.GainToSet]) / self.params[self.GainToSet]
         if error <= 0.10:
             self.rga.cem.voltage = hv_to_set
             self.rga.cem.stored_gain = round(measured_gain, 1)
             self.set_task_passed(True)
             self.add_details(f'Gain at {hv_to_set:.0f} V : {measured_gain:.0f}')
         else:
             self.set_task_passed(False)
 
     def update(self, data_dict):
+        """
+        Override Task.update.
+        It will run when self.notify_data_available() is called.
+        """
         try:
-            if data_dict['t'] == []:
+            if not data_dict['t']:
                 self.line2, = self.ax2.plot([], [])
             else:
                 self.line1.set_xdata(data_dict['x'])
                 self.line1.set_ydata(data_dict['y'])
 
                 self.line2.set_xdata(data_dict['t'])
                 self.line2.set_ydata(data_dict['i'])
-            self.figure.canvas.draw_idle()
+            self.request_figure_update()
 
         except Exception as e:
             self.logger.error('update error: {}'.format(e))
 
     def cleanup(self):
         self.rga.scan.speed = self.old_speed
         self.rga.cem.voltage = self.old_hv
@@ -191,15 +211,16 @@
         time.sleep(2.0)
         cem_intensity = self.measure_intensity_with_delay(self.params[self.WaitTime])
         return cem_intensity / fc_intensity
 
     def measure_intensity_with_delay(self, delay):
         start_time = time.time()
         elapsed_time = 0
-        while elapsed_time <= delay:
+        d = 0.0 if delay < 0.0 else delay
+        while elapsed_time <= d:
             elapsed_time = time.time() - start_time
             intensity = self.rga.scan.get_single_mass_scan(self.mass_to_measure_value) / 10.0
         return intensity
 
 
 if __name__ == '__main__':
     import logging
```

### Comparing `srsinst.rga-0.2.9/srsinst/rga/tasks/compositionanalysistask.py` & `srsinst.rga-0.3.0/srsinst/rga/tasks/compositionanalysistask.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+##! 
+##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
 
 from srsgui import Task
 from srsgui.task.inputs import StringInput, IntegerInput, InstrumentInput
 
 from srsinst.rga.plots.analysis import get_peak_from_analog_scan
 from srsinst.rga.plots.analogscanplot import AnalogScanPlot
 from srsinst.rga.plots.timeplot import TimePlot
@@ -42,14 +46,15 @@
     
     def setup(self):
         # Get values to use for task  from input_parameters in GUI
         self.params = self.get_all_input_parameters()
         gas_list = self.params[self.GasList].split(',')
         self.gas_list = [gas.strip().lower() for gas in gas_list]
         print(self.gas_list)
+
         # Get logger to use
         self.logger = self.get_logger(__name__)
 
         self.init_scan()
 
         self.lib = self.read_gas_library()
         self.mat = self.build_coeff_matrix(self.lib, self.params[self.StartMass], 
@@ -70,15 +75,15 @@
         self.ax_comp.set_xlim(self.params[self.StartMass], self.params[self.StopMass])
         self.ax_comp.set_ylim(1e-12, 1e-7)
         self.bar_x = np.arange(self.params[self.StartMass], self.params[self.StopMass] + 1)
         self.bar_y = np.zeros_like(self.bar_x)
 
         self.rect_dict = {}
         for gas in self.gas_list:
-            self.rect_dict[gas] = self.ax_comp.bar(self.bar_x, self.bar_y, label=gas)
+            self.rect_dict[gas] = self.ax_comp.bar(self.bar_x, self.bar_y, label=gas, alpha=0.6)
 
         # Setup patch-toggling legend
         self.legend = self.ax_comp.legend()
         self.patchd = {}
         for legpatch, patch_container in zip(self.legend.get_patches(), self.rect_dict.values()):
             legpatch.set_picker(True)
             self.patchd[legpatch] = patch_container
@@ -202,15 +207,15 @@
         self.logger.info('Number of gas read from {}: {}'.format(file_name, count//3))
         return d
 
     def build_coeff_matrix(self, gas_library, start_mass=1, stop_mass=50, 
                            gas_name_list=('Water', 'Nitrogen', 'Oxygen', 'Carbon dioxide')):
         """
         Build a least square fit coefficient matrix based on mass range  and 
-        refeence gas hsitogram spectra.
+        reference gas histogram spectra.
         """
         mat = np.array([np.zeros(stop_mass - start_mass + 1)])
         for gas in gas_name_list:
             gas_vector = np.array([np.zeros(stop_mass - start_mass + 1)])
             first_sens = gas_library[gas][0]
             second_sens = gas_library[gas][1] / 100.0
             total_sens = first_sens * second_sens
```

### Comparing `srsinst.rga-0.2.9/srsinst/rga/tasks/derivedpvstscantask.py` & `srsinst.rga-0.3.0/srsinst/rga/tasks/derivedpvstscantask.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+##! 
+##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
 
 from srsgui import Task
 from srsgui.task.inputs import ListInput, IntegerInput, StringInput, InstrumentInput
 
 from srsinst.rga.plots.timeplot import TimePlot
 from srsinst.rga.plots.analogscanplot import AnalogScanPlot
 
@@ -39,23 +43,23 @@
 
         self.mass_list = list(map(int, self.params[self.MassesToMeasure].split(',')))
 
         self.rga = get_rga(self, self.params[self.InstrumentName])
         self.id_string = self.rga.status.id_string
 
         margin = 5
-        init_mass = min(self.mass_list) - margin if min(self.mass_list) > margin else 1
-        fin_mass = max(self.mass_list) + margin if max(self.mass_list) < self.rga.scan.get_max_mass() \
+        initial_mass = min(self.mass_list) - margin if min(self.mass_list) > margin else 1
+        final_mass = max(self.mass_list) + margin if max(self.mass_list) < self.rga.scan.get_max_mass() \
             else self.rga.scan.get_max_mass()
 
         self.rga.scan.speed = self.params[self.ScanSpeed]
         self.rga.scan.resolution = 10
-        self.rga.scan.set_parameters(init_mass, fin_mass, self.params[self.ScanSpeed], self.rga.scan.resolution)
+        self.rga.scan.set_parameters(initial_mass, final_mass, self.params[self.ScanSpeed], self.rga.scan.resolution)
         self.logger.info('Scan initial mass: {}, final mass: {}, scan speed: {}, steps per AMU: {}'
-                         .format(init_mass, fin_mass, self.params[self.ScanSpeed], self.rga.scan.resolution))
+                         .format(initial_mass, final_mass, self.params[self.ScanSpeed], self.rga.scan.resolution))
 
         emission_current = self.rga.ionizer.emission_current
         cem_voltage = self.rga.cem.voltage
         self.logger.info('Emission current: {:.2f} mA CEM HV: {} V'.format(emission_current, cem_voltage))
 
         # Set up an derived P vs T plot
         self.ax_pvst = self.get_figure(self.DerivedPvsTPlot).add_subplot(111)
@@ -74,15 +78,15 @@
         else:
             self.conversion_factor = self.rga.pressure.get_partial_pressure_sensitivity_in_torr()
             self.plot_analog.set_conversion_factor(self.conversion_factor, 'Torr')
             self.pvst_plot.set_conversion_factor(self.conversion_factor, 'Torr')
 
         # Set up a log plot for the last full analog scan
         self.ax_log = self.get_figure(self.LogPlot).add_subplot(111)
-        self.ax_log.set_xlim(init_mass, fin_mass)
+        self.ax_log.set_xlim(initial_mass, final_mass)
         self.ax_log.set_xlabel("Mass (AMU)")
         self.ax_log.set_ylabel('Intensity')
         self.line_log, = self.ax_log.plot([1], [1])
         self.ax_log.set_yscale('log')
 
     def test(self):
         self.set_task_passed(True)
```

### Comparing `srsinst.rga-0.2.9/srsinst/rga/tasks/filamentcontroltask.py` & `srsinst.rga-0.3.0/srsinst/rga/tasks/filamentcontroltask.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+##! 
+##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
 
 from srsgui import Task
 from srsgui.task.inputs import FloatInput, InstrumentInput
 
 # get_rga is imported from the path relative to the .taskconfig file
 from instruments import get_rga
```

### Comparing `srsinst.rga-0.2.9/srsinst/rga/tasks/histogramscantask.py` & `srsinst.rga-0.3.0/srsinst/rga/tasks/histogramscantask.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+##! 
+##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
 
-import numpy
-from datetime import datetime
+import time
 
 from srsgui import Task
-from srsgui.task.inputs import ListInput, IntegerInput, InstrumentInput
-from srsinst.rga.plots.histogramscanplot import HistogramScanPlot
+from srsgui import ListInput, IntegerInput, InstrumentInput
+from srsinst.rga import HistogramScanPlot
 
 # get_rga is imported from the path relative to the .taskconfig file
 from instruments import get_rga
 
 
 class HistogramScanTask(Task):
     """Task to run histogram scans.
@@ -38,15 +41,14 @@
         # Get logger to use
         self.logger = self.get_logger(__name__)
 
         self.init_scan()
 
         # Set up an analog scan plot for the test
         self.ax = self.get_figure().add_subplot(111)
-
         self.plot = HistogramScanPlot(self, self.ax, self.rga.scan, 'Histogram')
 
         if self.params[self.IntensityUnit] == 0:
             self.conversion_factor = 0.1
             self.plot.set_conversion_factor(self.conversion_factor, 'fA')
         else:
             self.conversion_factor = self.rga.pressure.get_partial_pressure_sensitivity_in_torr()
@@ -94,14 +96,15 @@
     rga = Rga('serial', 'COM3', 115200, True)
     rga.comm.set_callbacks(logging.info, logging.info)
     task.inst_dict = {'dut': rga}
 
     task.figure = plt.figure()
     task.figure_dict = {'plot': task.figure}
 
-    task.set_input_parameter(task.Reps, 1)
     task.set_input_parameter(task.InstrumentName, 'dut')
 
     task.start()
+    time.sleep(1.0)
+    task.stop()
     task.wait()
     plt.show()
```

### Comparing `srsinst.rga-0.2.9/srsinst/rga/tasks/peaktuningtask.py` & `srsinst.rga-0.3.0/srsinst/rga/tasks/peaktuningtask.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+##! 
+##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
 
 import math
 import time
 import copy
 import numpy as np
 from scipy.signal import ricker, find_peaks, find_peaks_cwt, peak_widths, butter, filtfilt
 
@@ -26,18 +30,18 @@
     MassList = 'Masses used for tuning'
     PeakWidth = 'Peak width'
 
     # input_parameters values can be changed interactively from GUI
     input_parameters = {
         MassList: StringInput('14, 28, 32, 44'),
         PeakWidth: FloatInput(0.6, " AMU", 0.3, 1.2, .1),
-        RFSlope: FloatInput(0.5775, "", 0.1, 2000, .01),
-        RFIntercept: FloatInput(-0.5, " V", -30, 30, 0.001),
-        DCSlope: FloatInput(0.0951, "", -1, 1, .0001),
-        DCIntercept: FloatInput(-0.43, " V", -127, 127, 1.0),
+        RFSlope: FloatInput(1000, "", 600, 1600, .01),
+        RFIntercept: FloatInput(-0.5, " V", -86, 86, 0.001),
+        DCSlope: FloatInput(0.0951, "", -0.85, 0.85, .0001),
+        DCIntercept: FloatInput(125, " V", 0, 255, 1.0),
         PeakThreshold: FloatInput(1e4, "", 10, 1000000, 1),
     }
 
     def setup(self):
         self.logger = self.get_logger(__name__)
 
         # deepcopy need to have separate items  for multi-instances
@@ -246,21 +250,20 @@
             ymin, ymax = self.ax[1][0].get_ylim()
             self.ax[1][0].clear()
             self.ax[1][0].set_xlabel("Mass (AMU)")
             self.ax[1][0].set_ylabel('Ion Current(0.1 fA)')
             self.ax[1][0].set_yscale('log')
             self.ax[1][0].set_ylim(ymin, ymax)
             # self.ax[1][0].plot(self.data_dict['prev_x'], self.data_dict['prev_y'],
-            self.ax[1][0].plot(x, y,
-                               color="#808020", linewidth=1)
+            self.ax[1][0].plot(x, y, color="#808020", linewidth=1)
             self.ax[1][0].plot(peak_positions, y[peaks], "bx")
             self.ax[1][0].plot(peaks_cwt / sa + mi, y[peaks_cwt], "r.")
             self.ax[1][0].hlines(width_heights, width_x_min, width_x_max, color="red")
             self.ax[1][0].hlines(properties['width_heights'], properties['left_ips'] / sa + mi,
                                  properties['right_ips'] / sa + mi, color="blue")
 
             self.notify_data_available(self.data_dict)
         except Exception as e:
             self.logger.error('update_on_scan_finished error: {}'.format(e))
 
     def cleanup(self):
-        self.logger.info('Test Done')
+        self.logger.info('Task finished')
```

### Comparing `srsinst.rga-0.2.9/srsinst/rga/tasks/pvstscantask.py` & `srsinst.rga-0.3.0/srsinst/rga/tasks/pvstscantask.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+##! 
+##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
 
 from srsgui import Task
 from srsgui.task.inputs import ListInput, IntegerInput, StringInput, InstrumentInput
 
 from srsinst.rga.plots.timeplot import TimePlot
 
 # get_rga is imported from the path relative to the .taskconfig file
```

### Comparing `srsinst.rga-0.2.9/srsinst/rga/tasks/searchlan.py` & `srsinst.rga-0.3.0/srsinst/rga/tasks/searchlan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+##! 
+##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Subject to the MIT License
+##! 
 
 from srsgui import Task
 from srsgui.task.inputs import ListInput
 from srsinst.rga import SICP
 
 
 class SearchLanTask(Task):
```

### Comparing `srsinst.rga-0.2.9/srsinst.rga.egg-info/PKG-INFO` & `srsinst.rga-0.3.0/srsinst.rga.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 Metadata-Version: 2.1
 Name: srsinst.rga
-Version: 0.2.9
-Summary: Instrument library and GUI application for SRS RGA
+Version: 0.3.0
+Summary: Instrument driver package for Residual Gas Analyzers (RGA) from Stanford Research Systems
 Author: Chulhoon Kim
 License: MIT license
 Keywords: RGA,residual gas analyzer,SRS,Stanford Research Systems
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Chemistry
-Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: full
-License-File: LICENSE.txt
+License-File: LICENSE
 
 # `srsinst.rga`
 
-`srsinst.rga` is a Python GUI application to control and acquire mass spectra from 
+`srsinst.rga` provides Python instrument classes to control and acquire mass spectra from 
 [Stanford Research Systems (SRS) Residual Gas Analyzers (RGA)](https://thinksrs.com/products/rga.html).
-To use this package safely, you need to be familiar with SRS RGA. You can download the
-[manual](https://thinksrs.com/downloads/pdfs/manuals/RGAm.pdf) for your reference.
+It also provides tasks running in GUI environment based on 
+[srsgui](https://thinksrs.github.io/srsgui/).  
+To operate SRS RGA with this package safely, you need to be familiar with SRS RGA. 
+For detailed information, refer to the 
+[manual](https://thinksrs.com/downloads/pdfs/manuals/RGAm.pdf).
+
+![screenshot](https://github.com/thinkSRS/srsinst.rga/blob/main/docs/_static/image/derived-pvst-plot-screenshot.png " ")
 
 ## Installation
-You should have a working Python with `pip` (Python package installer) installed. If you don't,
+You need a working Python with `pip` (Python package installer) installed. If you don't,
 [install Python 3](https://realpython.com/installing-python/) to your system.
 
-To install `srsinst.rga` as an instrument driver , use Python package installer `pip` from the command line.
+To install `srsinst.rga` as an instrument driver only, use Python package installer `pip` 
+from the command line.
 
     python -m pip install srsinst.rga
 
-To use its full GUI application, create a virtual environment and install:
+To use its full GUI application, create a virtual environment, if necessary,
+and install with *[full]* option:
+
+    # To create a simple virtual environment (Optional)
+    python -m venv venv
+    venv\scripts\activate
 
+    # To install full GUI application 
     python -m pip install srsinst.rga[full]
 
 
 ## Run `srsinst.rga` as GUI application
 If the Python Scripts directory is in PATH environment variable,
 Start the application by typing from the command line:
 
@@ -51,38 +62,39 @@
 
 It will start the GUI application.
 
 Connect to an RGA from the Instruments menu.
 Select a task from the Task menu.
 Press the green arrow to run the selected task. 
 
-You can write your own task or modify an existing one and run it from the application, too.
+You can write your own task or modify an existing one and run it from the application.
+Refer to [srsgui](https://thinksrs.github.io/srsgui/) documentation for details.
 
 ## Use `srsinst.rga` as instrument driver
 * Start the Python program, or an editor of your choice to write a Python script.
-* import the **RGA** class from `rga` package.
-* Instantiate **RGA** to connect to an SRS RGA.
+* import the **RGA100** class from `srsinst.rga` package.
+* Instantiate **RGA100** to connect to an SRS RGA.
 
-        from srsinst.rga import RGA100 as RGA
+        from srsinst.rga import RGA100
 
         # for TCPIP communication
         ip_address = '192.168.1.100'
         user_id = 'admin'
         password = 'admin'
 
-        rga1 = RGA('tcpip', ip_address, user_id, password)
+        rga1 = RGA100('tcpip', ip_address, user_id, password)
 
         # for serial communication
         # Baud rate for RGA100 is fixed to 28800
         # rga2 = RGA('serial', /dev/ttyUSB0', 28800)  # for Linux serial communication
 
         rga2 = RGA('serial', 'COM3', 28800)  # for Windows serial communication
 
-        # or initialize a Rga instance without connection, then connect.
-        rga3 = RGA()
+        # or initialize a RGA100 instance without connection, then connect.
+        rga3 = RGA100()
         rga3.connect('tcpip', ip_address, user_id, password)
 
 * Control ionizer parameters.
 
         # Set ionizer values
         rga1.ionizer.electron_energy = 70
         rga1.ionizer.ion_energy = 12
@@ -100,23 +112,23 @@
         # or
         a, b, c = rga1.ionizer.get_parameters()
 
 
         # Set the filament emsission current.
 
         rga1.ionizer.emission_current = 1.0  # in the unit of mA
-        rga1.ionizer.emission_current = 0.0  # It will turn off the filament
+        rga1.ionizer.emission_current = 0.0  # It will turn off the filament.
 
         # or
 
-        rga1.filament.turn_on(1.0)  # emission cureent in the unit of mA
+        rga1.filament.turn_on()  # Turn on with the default emission cureent of 1 mA.
         rga1.filament.turn_off()
 
 
-        # Get the emission current to check
+        # Read back the emission current
         a = rga1.ionizer.emission_current
 
 * Control detector parameters.
 
         # Set CEM voltage to the calibrated CEM voltage, or 0 to turn off
         rga1.cem.voltage = rga1.cem.stored_voltage
         rga1.cem.voltage = 0
@@ -143,15 +155,15 @@
         mi, mf, nf, sa = rga1.scan.get_parameters()
 
 * Run an analog scan.
 
         analog_spectrum  = rga1.scan.get_analog_scan()
         spectrum_in_torr = rga1.scan.get_partial_pressure_corrected_spectrum(analog_spectrum)
 
-        # Get the mathing mass axis with the spectrum
+        # Get the matching mass axis with the spectrum
         analog_mass_axis = rga1.scan.get_mass_axis(True)  # is it for analog scan? Yes.
 
 * Run a histogram scan.
 
         histogram_spectrum  = rga1.scan.get_histogram_scan()
 
         # Get the matching mass axis with the spectrum
```

### Comparing `srsinst.rga-0.2.9/srsinst.rga.egg-info/SOURCES.txt` & `srsinst.rga-0.3.0/srsinst.rga.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-LICENSE.txt
-MANIFEST.in
+.gitignore
+LICENSE
 README.md
-readme.md
+pyproject.toml
 setup.py
+docs/_static/image/derived-pvst-plot-screenshot.png
 srsinst.rga.egg-info/PKG-INFO
 srsinst.rga.egg-info/SOURCES.txt
 srsinst.rga.egg-info/dependency_links.txt
 srsinst.rga.egg-info/entry_points.txt
 srsinst.rga.egg-info/requires.txt
 srsinst.rga.egg-info/top_level.txt
 srsinst/rga/__init__.py
@@ -16,14 +17,15 @@
 srsinst/rga/instruments/__init__.py
 srsinst/rga/instruments/get_instruments.py
 srsinst/rga/instruments/rga100/__init__.py
 srsinst/rga/instruments/rga100/commands.py
 srsinst/rga/instruments/rga100/components.py
 srsinst/rga/instruments/rga100/errors.py
 srsinst/rga/instruments/rga100/rga.py
+srsinst/rga/instruments/rga100/rga_commands.json
 srsinst/rga/instruments/rga100/scans.py
 srsinst/rga/instruments/rga100/sicp.py
 srsinst/rga/plots/__init__.py
 srsinst/rga/plots/analogscanplot.py
 srsinst/rga/plots/analysis.py
 srsinst/rga/plots/basescanplot.py
 srsinst/rga/plots/histogramscanplot.py
```

