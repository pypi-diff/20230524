# Comparing `tmp/jutility-0.0.8.tar.gz` & `tmp/jutility-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Jake\Documents\Programming\jutility\dist\.tmp-jbhsok19\jutility-0.0.8.tar", last modified: Sun May 14 19:12:30 2023, max compression
+gzip compressed data, was "C:\Users\Jake\Documents\Programming\jutility\dist\.tmp-jj4bkh5j\jutility-0.0.9.tar", last modified: Mon May 15 13:45:32 2023, max compression
```

## Comparing `jutility-0.0.8.tar` & `jutility-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 19:12:30.000000 jutility-0.0.8/
--rw-rw-rw-   0        0        0     1087 2023-05-13 21:09:33.000000 jutility-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     2993 2023-05-14 19:12:30.000000 jutility-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2333 2023-05-14 19:09:35.000000 jutility-0.0.8/README.md
--rw-rw-rw-   0        0        0       90 2023-05-14 18:37:23.000000 jutility-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      760 2023-05-14 19:12:30.000000 jutility-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-14 19:12:30.000000 jutility-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-14 19:12:30.000000 jutility-0.0.8/src/jutility/
--rw-rw-rw-   0        0        0        0 2023-05-13 20:59:58.000000 jutility-0.0.8/src/jutility/__init__.py
--rw-rw-rw-   0        0        0    16333 2023-05-14 17:11:46.000000 jutility-0.0.8/src/jutility/plotting.py
--rw-rw-rw-   0        0        0    10048 2023-05-13 21:30:51.000000 jutility-0.0.8/src/jutility/sweep.py
--rw-rw-rw-   0        0        0    13209 2023-05-14 15:33:41.000000 jutility-0.0.8/src/jutility/util.py
-drwxrwxrwx   0        0        0        0 2023-05-14 19:12:30.000000 jutility-0.0.8/src/jutility.egg-info/
--rw-rw-rw-   0        0        0     2993 2023-05-14 19:12:30.000000 jutility-0.0.8/src/jutility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-05-14 19:12:30.000000 jutility-0.0.8/src/jutility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 19:12:30.000000 jutility-0.0.8/src/jutility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-14 19:12:30.000000 jutility-0.0.8/src/jutility.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-14 19:12:30.000000 jutility-0.0.8/src/jutility.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-14 19:12:30.000000 jutility-0.0.8/tests/
--rw-rw-rw-   0        0        0     9100 2023-05-14 15:22:52.000000 jutility-0.0.8/tests/test_plotting.py
--rw-rw-rw-   0        0        0     9206 2023-05-13 21:45:28.000000 jutility-0.0.8/tests/test_sweep.py
--rw-rw-rw-   0        0        0    12140 2023-05-14 15:40:12.000000 jutility-0.0.8/tests/test_util.py
+drwxrwxrwx   0        0        0        0 2023-05-15 13:45:32.000000 jutility-0.0.9/
+-rw-rw-rw-   0        0        0     1087 2023-05-13 21:09:33.000000 jutility-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     2985 2023-05-15 13:45:32.000000 jutility-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2324 2023-05-15 13:40:15.000000 jutility-0.0.9/README.md
+-rw-rw-rw-   0        0        0       90 2023-05-14 18:37:23.000000 jutility-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      761 2023-05-15 13:45:32.000000 jutility-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-15 13:45:32.000000 jutility-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-15 13:45:32.000000 jutility-0.0.9/src/jutility/
+-rw-rw-rw-   0        0        0        0 2023-05-13 20:59:58.000000 jutility-0.0.9/src/jutility/__init__.py
+-rw-rw-rw-   0        0        0    16779 2023-05-15 11:03:39.000000 jutility-0.0.9/src/jutility/plotting.py
+-rw-rw-rw-   0        0        0    10048 2023-05-13 21:30:51.000000 jutility-0.0.9/src/jutility/sweep.py
+-rw-rw-rw-   0        0        0    13351 2023-05-15 11:47:34.000000 jutility-0.0.9/src/jutility/util.py
+drwxrwxrwx   0        0        0        0 2023-05-15 13:45:32.000000 jutility-0.0.9/src/jutility.egg-info/
+-rw-rw-rw-   0        0        0     2985 2023-05-15 13:45:32.000000 jutility-0.0.9/src/jutility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-05-15 13:45:32.000000 jutility-0.0.9/src/jutility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 13:45:32.000000 jutility-0.0.9/src/jutility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-15 13:45:32.000000 jutility-0.0.9/src/jutility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-15 13:45:32.000000 jutility-0.0.9/src/jutility.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 13:45:32.000000 jutility-0.0.9/tests/
+-rw-rw-rw-   0        0        0     9100 2023-05-14 15:22:52.000000 jutility-0.0.9/tests/test_plotting.py
+-rw-rw-rw-   0        0        0     9206 2023-05-13 21:45:28.000000 jutility-0.0.9/tests/test_sweep.py
+-rw-rw-rw-   0        0        0    12140 2023-05-14 15:40:12.000000 jutility-0.0.9/tests/test_util.py
```

### Comparing `jutility-0.0.8/LICENSE` & `jutility-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jutility-0.0.8/PKG-INFO` & `jutility-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: jutility
-Version: 0.0.8
-Summary: Collection of Python utilities intended to be useful for machine learning research and experiments
+Version: 0.0.9
+Summary: Collection of Python utilities intended to be useful for machine learning research and experiments.
 Home-page: https://github.com/jakelevi1996/jutility
 Author: Jake Levi
 Author-email: jakelevi@hotmail.co.uk
 License: MIT License
 Project-URL: Documentation, https://github.com/jakelevi1996/jutility
 Project-URL: Source Code, https://github.com/jakelevi1996/jutility
 Project-URL: Bug Tracker, https://github.com/jakelevi1996/jutility/issues
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # jutility
 
 Collection of Python utilities intended to be useful for machine learning research and experiments.
 
-![](https://raw.githubusercontent.com/jakelevi1996/jutility/main/images/logo.png)
+![](https://raw.githubusercontent.com/jakelevi1996/jutility/main/images/logo_black.png)
 
 ## Contents
 
 - [jutility](#jutility)
   - [Contents](#contents)
   - [Install with `pip`](#install-with-pip)
   - [Usage examples](#usage-examples)
@@ -42,15 +42,15 @@
 
 *Coming soon*
 
 (in the meantime, see [`scripts/make_logo.py`](scripts/make_logo.py) which made the logo above, and [unit tests](tests/) for [`util`](tests/test_util.py), [`plotting`](tests/test_plotting.py), and [`sweep`](tests/test_sweep.py))
 
 ## Unit tests
 
-To run unit all unit tests, install [`pytest`](https://pypi.org/project/pytest/) (these tests have previously been run with `pytest` version 5.4.1), and run the following command (at the time of writing, this takes about 17 seconds to run 42 unit tests, because several unit tests involve saving images or GIFs to disk):
+To run all unit tests, install [`pytest`](https://pypi.org/project/pytest/) (these tests have previously been run with `pytest` version 5.4.1), and run the following command (at the time of writing, this takes about 17 seconds to run 42 unit tests, because several unit tests involve saving images or GIFs to disk):
 
 ```
 pytest
 ```
 
 ## Build package locally
 
@@ -61,15 +61,15 @@
 python -m pip install --force-reinstall --no-deps dist/$WHEEL_NAME
 ```
 
 ## Updating package on PyPI
 
 This package was uploaded to PyPI following [the Packaging Python Projects tutorial in the official Python documentation](https://packaging.python.org/en/latest/tutorials/packaging-projects/).
 
-To update PyPI with a newer version, update the `version` tag in [pyproject.toml](pyproject.toml), and then use the following commands:
+To update PyPI with a newer version, update the `version` tag in [setup.cfg](setup.cfg), and then use the following commands:
 
 ```
 rm -rf dist/*
 python -m build
 python -m twine upload dist/*
 ```
```

### Comparing `jutility-0.0.8/README.md` & `jutility-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # jutility
 
 Collection of Python utilities intended to be useful for machine learning research and experiments.
 
-![](https://raw.githubusercontent.com/jakelevi1996/jutility/main/images/logo.png)
+![](https://raw.githubusercontent.com/jakelevi1996/jutility/main/images/logo_black.png)
 
 ## Contents
 
 - [jutility](#jutility)
   - [Contents](#contents)
   - [Install with `pip`](#install-with-pip)
   - [Usage examples](#usage-examples)
@@ -27,15 +27,15 @@
 
 *Coming soon*
 
 (in the meantime, see [`scripts/make_logo.py`](scripts/make_logo.py) which made the logo above, and [unit tests](tests/) for [`util`](tests/test_util.py), [`plotting`](tests/test_plotting.py), and [`sweep`](tests/test_sweep.py))
 
 ## Unit tests
 
-To run unit all unit tests, install [`pytest`](https://pypi.org/project/pytest/) (these tests have previously been run with `pytest` version 5.4.1), and run the following command (at the time of writing, this takes about 17 seconds to run 42 unit tests, because several unit tests involve saving images or GIFs to disk):
+To run all unit tests, install [`pytest`](https://pypi.org/project/pytest/) (these tests have previously been run with `pytest` version 5.4.1), and run the following command (at the time of writing, this takes about 17 seconds to run 42 unit tests, because several unit tests involve saving images or GIFs to disk):
 
 ```
 pytest
 ```
 
 ## Build package locally
 
@@ -46,15 +46,15 @@
 python -m pip install --force-reinstall --no-deps dist/$WHEEL_NAME
 ```
 
 ## Updating package on PyPI
 
 This package was uploaded to PyPI following [the Packaging Python Projects tutorial in the official Python documentation](https://packaging.python.org/en/latest/tutorials/packaging-projects/).
 
-To update PyPI with a newer version, update the `version` tag in [pyproject.toml](pyproject.toml), and then use the following commands:
+To update PyPI with a newer version, update the `version` tag in [setup.cfg](setup.cfg), and then use the following commands:
 
 ```
 rm -rf dist/*
 python -m build
 python -m twine upload dist/*
 ```
```

### Comparing `jutility-0.0.8/setup.cfg` & `jutility-0.0.9/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206a 7574 696c 6974 790d 0a76 6572   = jutility..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e38 0d0a 6175  sion = 0.0.8..au
+00000020: 7369 6f6e 203d 2030 2e30 2e39 0d0a 6175  sion = 0.0.9..au
 00000030: 7468 6f72 203d 204a 616b 6520 4c65 7669  thor = Jake Levi
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 206a 616b 656c 6576 6940 686f 746d 6169   jakelevi@hotmai
 00000060: 6c2e 636f 2e75 6b0d 0a64 6573 6372 6970  l.co.uk..descrip
 00000070: 7469 6f6e 203d 2043 6f6c 6c65 6374 696f  tion = Collectio
 00000080: 6e20 6f66 2050 7974 686f 6e20 7574 696c  n of Python util
 00000090: 6974 6965 7320 696e 7465 6e64 6564 2074  ities intended t
 000000a0: 6f20 6265 2075 7365 6675 6c20 666f 7220  o be useful for 
 000000b0: 6d61 6368 696e 6520 6c65 6172 6e69 6e67  machine learning
 000000c0: 2072 6573 6561 7263 6820 616e 6420 6578   research and ex
-000000d0: 7065 7269 6d65 6e74 730d 0a6c 6f6e 675f  periments..long_
-000000e0: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
-000000f0: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
-00000100: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
-00000110: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
-00000120: 6578 742f 6d61 726b 646f 776e 0d0a 6c69  ext/markdown..li
-00000130: 6365 6e73 6520 3d20 4d49 5420 4c69 6365  cense = MIT Lice
-00000140: 6e73 650d 0a6c 6963 656e 7365 5f66 696c  nse..license_fil
-00000150: 6573 203d 204c 4943 454e 5345 0d0a 7572  es = LICENSE..ur
-00000160: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
-00000170: 7562 2e63 6f6d 2f6a 616b 656c 6576 6931  ub.com/jakelevi1
-00000180: 3939 362f 6a75 7469 6c69 7479 0d0a 7072  996/jutility..pr
-00000190: 6f6a 6563 745f 7572 6c73 203d 200d 0a09  oject_urls = ...
-000001a0: 446f 6375 6d65 6e74 6174 696f 6e20 2020  Documentation   
-000001b0: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
-000001c0: 2e63 6f6d 2f6a 616b 656c 6576 6931 3939  .com/jakelevi199
-000001d0: 362f 6a75 7469 6c69 7479 0d0a 0953 6f75  6/jutility...Sou
-000001e0: 7263 6520 436f 6465 2020 2020 203d 2068  rce Code     = h
-000001f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000200: 6d2f 6a61 6b65 6c65 7669 3139 3936 2f6a  m/jakelevi1996/j
-00000210: 7574 696c 6974 790d 0a09 4275 6720 5472  utility...Bug Tr
-00000220: 6163 6b65 7220 2020 2020 3d20 6874 7470  acker     = http
-00000230: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-00000240: 616b 656c 6576 6931 3939 362f 6a75 7469  akelevi1996/juti
-00000250: 6c69 7479 2f69 7373 7565 730d 0a0d 0a5b  lity/issues....[
-00000260: 6f70 7469 6f6e 735d 0d0a 7079 7468 6f6e  options]..python
-00000270: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
-00000280: 370d 0a69 6e73 7461 6c6c 5f72 6571 7569  7..install_requi
-00000290: 7265 7320 3d20 0d0a 096d 6174 706c 6f74  res = ...matplot
-000002a0: 6c69 623e 3d33 2e35 2e33 0d0a 096e 756d  lib>=3.5.3...num
-000002b0: 7079 3e3d 312e 3231 2e36 0d0a 0950 696c  py>=1.21.6...Pil
-000002c0: 6c6f 773e 3d39 2e35 2e30 0d0a 0d0a 5b65  low>=9.5.0....[e
-000002d0: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-000002e0: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-000002f0: 203d 2030 0d0a 0d0a                       = 0....
+000000d0: 7065 7269 6d65 6e74 732e 0d0a 6c6f 6e67  periments...long
+000000e0: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
+000000f0: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
+00000100: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+00000110: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
+00000120: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a6c  text/markdown..l
+00000130: 6963 656e 7365 203d 204d 4954 204c 6963  icense = MIT Lic
+00000140: 656e 7365 0d0a 6c69 6365 6e73 655f 6669  ense..license_fi
+00000150: 6c65 7320 3d20 4c49 4345 4e53 450d 0a75  les = LICENSE..u
+00000160: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
+00000170: 6875 622e 636f 6d2f 6a61 6b65 6c65 7669  hub.com/jakelevi
+00000180: 3139 3936 2f6a 7574 696c 6974 790d 0a70  1996/jutility..p
+00000190: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
+000001a0: 0944 6f63 756d 656e 7461 7469 6f6e 2020  .Documentation  
+000001b0: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
+000001c0: 622e 636f 6d2f 6a61 6b65 6c65 7669 3139  b.com/jakelevi19
+000001d0: 3936 2f6a 7574 696c 6974 790d 0a09 536f  96/jutility...So
+000001e0: 7572 6365 2043 6f64 6520 2020 2020 3d20  urce Code     = 
+000001f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000200: 6f6d 2f6a 616b 656c 6576 6931 3939 362f  om/jakelevi1996/
+00000210: 6a75 7469 6c69 7479 0d0a 0942 7567 2054  jutility...Bug T
+00000220: 7261 636b 6572 2020 2020 203d 2068 7474  racker     = htt
+00000230: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000240: 6a61 6b65 6c65 7669 3139 3936 2f6a 7574  jakelevi1996/jut
+00000250: 696c 6974 792f 6973 7375 6573 0d0a 0d0a  ility/issues....
+00000260: 5b6f 7074 696f 6e73 5d0d 0a70 7974 686f  [options]..pytho
+00000270: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
+00000280: 2e37 0d0a 696e 7374 616c 6c5f 7265 7175  .7..install_requ
+00000290: 6972 6573 203d 200d 0a09 6d61 7470 6c6f  ires = ...matplo
+000002a0: 746c 6962 3e3d 332e 352e 330d 0a09 6e75  tlib>=3.5.3...nu
+000002b0: 6d70 793e 3d31 2e32 312e 360d 0a09 5069  mpy>=1.21.6...Pi
+000002c0: 6c6c 6f77 3e3d 392e 352e 300d 0a0d 0a5b  llow>=9.5.0....[
+000002d0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+000002e0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+000002f0: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `jutility-0.0.8/src/jutility/plotting.py` & `jutility-0.0.9/src/jutility/plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -250,26 +250,28 @@
         log_xscale=False,
         log_yscale=False,
         rotate_xticklabels=False,
         axis_equal=False,
         axis_off=False,
         grid=True,
         title=None,
+        colour=None,
     ):
         self._xlabel = xlabel
         self._ylabel = ylabel
         self._xlim = xlim
         self._ylim = ylim
         self._log_xscale = log_xscale
         self._log_yscale = log_yscale
         self._rotate_xticklabels = rotate_xticklabels
         self._axis_equal = axis_equal
         self._axis_off = axis_off
         self._grid = grid
         self._title = title
+        self._colour = colour
 
     def set_title(self, title):
         self._title = title
 
     def apply(self, axis):
         if self._xlabel is not None:
             axis.set_xlabel(self._xlabel)
@@ -290,40 +292,46 @@
         if self._grid:
             axis.grid(True, which="both")
         if self._rotate_xticklabels:
             for xtl in axis.get_xticklabels():
                 xtl.set(rotation=-45, ha="left")
         if self._title is not None:
             axis.set_title(wrap(self._title))
+        if self._colour is not None:
+            axis.set_facecolor(self._colour)
 
 class FigureProperties:
     def __init__(
         self,
         num_rows=None,
         num_cols=None,
         figsize=None,
         sharex=False,
         sharey=False,
         width_ratios=None,
         height_ratios=None,
         tight_layout=True,
+        colour=None,
         title=None,
         title_font_size=25,
+        title_colour=None,
         top_space=None,
     ):
         self._num_rows = num_rows
         self._num_cols = num_cols
         self._figsize = figsize
         self._sharex = sharex
         self._sharey = sharey
         self._width_ratios = width_ratios
         self._height_ratios = height_ratios
         self._tight_layout = tight_layout
+        self._colour = colour
         self._title = title
         self._title_font_size = title_font_size
+        self._title_colour = title_colour
         self._top_space = top_space
 
     def get_figure_and_axes(self, num_subplots):
         if self._num_rows is None:
             if self._num_cols is None:
                 self._num_cols = math.ceil(math.sqrt(num_subplots))
             self._num_rows = math.ceil(num_subplots / self._num_cols)
@@ -347,16 +355,22 @@
             squeeze=False,
         )
         return figure, axes.flat
 
     def apply(self, figure):
         if self._tight_layout:
             figure.tight_layout()
+        if self._colour is not None:
+            figure.patch.set_facecolor(self._colour)
         if self._title is not None:
-            figure.suptitle(wrap(self._title), fontsize=self._title_font_size)
+            figure.suptitle(
+                wrap(self._title),
+                fontsize=self._title_font_size,
+                color=self._title_colour,
+            )
         if self._top_space is not None:
             figure.subplots_adjust(top=(1 - self._top_space))
 
 class Subplot:
     def __init__(self, *lines, axis_properties=None):
         self._lines = lines
         if axis_properties is None:
```

### Comparing `jutility-0.0.8/src/jutility/sweep.py` & `jutility-0.0.9/src/jutility/sweep.py`

 * *Files identical despite different names*

### Comparing `jutility-0.0.8/src/jutility/util.py` & `jutility-0.0.9/src/jutility/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -379,47 +379,51 @@
 
     if file_ext is not None:
         filename = "%s.%s" % (filename, file_ext)
 
     full_path = os.path.join(dir_name, filename)
     return full_path
 
-def save_pickle(data, filename, dir_name=None):
+def save_pickle(data, filename, dir_name=None, verbose=True):
     full_path = get_full_path(
         filename,
         dir_name,
         for_saving=True,
         file_ext="pkl",
     )
-    print("Saving pickle in \"%s\"" % full_path)
+    if verbose:
+        print("Saving pickle in \"%s\"" % full_path)
     with open(full_path, "wb") as f:
         pickle.dump(data, f)
 
-def load_pickle(filename, dir_name=None):
+def load_pickle(filename, dir_name=None, verbose=False):
     full_path = get_full_path(filename, dir_name)
-    print("Loading pickle from \"%s\"" % full_path)
+    if verbose:
+        print("Loading pickle from \"%s\"" % full_path)
     with open(full_path, "rb") as f:
         data = pickle.load(f)
 
     return data
 
-def save_json(data, filename, dir_name=None):
+def save_json(data, filename, dir_name=None, verbose=True):
     full_path = get_full_path(
         filename,
         dir_name,
         for_saving=True,
         file_ext="json",
     )
-    print("Saving JSON in \"%s\"" % full_path)
+    if verbose:
+        print("Saving JSON in \"%s\"" % full_path)
     with open(full_path, "w") as f:
         json.dump(data, f)
 
-def load_json(filename, dir_name=None):
+def load_json(filename, dir_name=None, verbose=False):
     full_path = get_full_path(filename, dir_name)
-    print("Loading JSON from \"%s\"" % full_path)
+    if verbose:
+        print("Loading JSON from \"%s\"" % full_path)
     with open(full_path, "r") as f:
         data = json.load(f)
 
     return data
 
 def is_numeric(x):
     return any(isinstance(x, t) for t in [int, float, np.number])
```

### Comparing `jutility-0.0.8/src/jutility.egg-info/PKG-INFO` & `jutility-0.0.9/src/jutility.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: jutility
-Version: 0.0.8
-Summary: Collection of Python utilities intended to be useful for machine learning research and experiments
+Version: 0.0.9
+Summary: Collection of Python utilities intended to be useful for machine learning research and experiments.
 Home-page: https://github.com/jakelevi1996/jutility
 Author: Jake Levi
 Author-email: jakelevi@hotmail.co.uk
 License: MIT License
 Project-URL: Documentation, https://github.com/jakelevi1996/jutility
 Project-URL: Source Code, https://github.com/jakelevi1996/jutility
 Project-URL: Bug Tracker, https://github.com/jakelevi1996/jutility/issues
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # jutility
 
 Collection of Python utilities intended to be useful for machine learning research and experiments.
 
-![](https://raw.githubusercontent.com/jakelevi1996/jutility/main/images/logo.png)
+![](https://raw.githubusercontent.com/jakelevi1996/jutility/main/images/logo_black.png)
 
 ## Contents
 
 - [jutility](#jutility)
   - [Contents](#contents)
   - [Install with `pip`](#install-with-pip)
   - [Usage examples](#usage-examples)
@@ -42,15 +42,15 @@
 
 *Coming soon*
 
 (in the meantime, see [`scripts/make_logo.py`](scripts/make_logo.py) which made the logo above, and [unit tests](tests/) for [`util`](tests/test_util.py), [`plotting`](tests/test_plotting.py), and [`sweep`](tests/test_sweep.py))
 
 ## Unit tests
 
-To run unit all unit tests, install [`pytest`](https://pypi.org/project/pytest/) (these tests have previously been run with `pytest` version 5.4.1), and run the following command (at the time of writing, this takes about 17 seconds to run 42 unit tests, because several unit tests involve saving images or GIFs to disk):
+To run all unit tests, install [`pytest`](https://pypi.org/project/pytest/) (these tests have previously been run with `pytest` version 5.4.1), and run the following command (at the time of writing, this takes about 17 seconds to run 42 unit tests, because several unit tests involve saving images or GIFs to disk):
 
 ```
 pytest
 ```
 
 ## Build package locally
 
@@ -61,15 +61,15 @@
 python -m pip install --force-reinstall --no-deps dist/$WHEEL_NAME
 ```
 
 ## Updating package on PyPI
 
 This package was uploaded to PyPI following [the Packaging Python Projects tutorial in the official Python documentation](https://packaging.python.org/en/latest/tutorials/packaging-projects/).
 
-To update PyPI with a newer version, update the `version` tag in [pyproject.toml](pyproject.toml), and then use the following commands:
+To update PyPI with a newer version, update the `version` tag in [setup.cfg](setup.cfg), and then use the following commands:
 
 ```
 rm -rf dist/*
 python -m build
 python -m twine upload dist/*
 ```
```

### Comparing `jutility-0.0.8/tests/test_plotting.py` & `jutility-0.0.9/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `jutility-0.0.8/tests/test_sweep.py` & `jutility-0.0.9/tests/test_sweep.py`

 * *Files identical despite different names*

### Comparing `jutility-0.0.8/tests/test_util.py` & `jutility-0.0.9/tests/test_util.py`

 * *Files identical despite different names*

