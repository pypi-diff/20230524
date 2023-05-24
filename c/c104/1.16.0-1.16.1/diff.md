# Comparing `tmp/c104-1.16.0-cp39-cp39-win_amd64.whl.zip` & `tmp/c104-1.16.1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 389352 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat   925184 b- defN 23-May-15 10:52 c104.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    35149 b- defN 23-May-15 10:52 c104-1.16.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6282 b- defN 23-May-15 10:52 c104-1.16.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-15 10:52 c104-1.16.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-May-15 10:52 c104-1.16.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      459 b- defN 23-May-15 10:52 c104-1.16.0.dist-info/RECORD
-6 files, 967179 bytes uncompressed, 388530 bytes compressed:  59.8%
+Zip file size: 389198 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat   925184 b- defN 23-May-24 13:33 c104.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    35149 b- defN 23-May-24 13:33 c104-1.16.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6097 b- defN 23-May-24 13:33 c104-1.16.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-24 13:33 c104-1.16.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-May-24 13:33 c104-1.16.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      459 b- defN 23-May-24 13:33 c104-1.16.1.dist-info/RECORD
+6 files, 966994 bytes uncompressed, 388376 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: c104.cp39-win_amd64.pyd
 Comment: 
 
-Filename: c104-1.16.0.dist-info/LICENSE
+Filename: c104-1.16.1.dist-info/LICENSE
 Comment: 
 
-Filename: c104-1.16.0.dist-info/METADATA
+Filename: c104-1.16.1.dist-info/METADATA
 Comment: 
 
-Filename: c104-1.16.0.dist-info/WHEEL
+Filename: c104-1.16.1.dist-info/WHEEL
 Comment: 
 
-Filename: c104-1.16.0.dist-info/top_level.txt
+Filename: c104-1.16.1.dist-info/top_level.txt
 Comment: 
 
-Filename: c104-1.16.0.dist-info/RECORD
+Filename: c104-1.16.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `c104-1.16.0.dist-info/LICENSE` & `c104-1.16.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `c104-1.16.0.dist-info/METADATA` & `c104-1.16.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c104
-Version: 1.16.0
+Version: 1.16.1
 Summary: iec104-python
 Home-page: https://github.com/fraunhofer-fit-dien/iec104-python
 Author: Martin Unkel, Fraunhofer FIT
 Author-email: martin.unkel@fit.fraunhofer.de
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -111,53 +111,38 @@
 [&raquo; Documentation](https://github.com/catchorg/Catch2/blob/devel/docs/Readme.md)
 
 
 ## System requirements
 
 ### Operating systems
 
-* Debian/Ubuntu (x64): YES
+* Debian/Ubuntu (x64): YES >= 20.04
 * Raspbian (arm32v7): YES
 * Windows (x64): YES
 * Raspbian (aarch64): Not yet
 
 ### Python versions
 * python >= 3.6, < 3.11
 
 ## Installation
+Please adjust the version number to the latest version or use a specific version according to your needs.
 
-### Package distribution
-
-#### Install from pypi package (comming soon)
+### Install from pypi.org
 ```bash
 python3 -m pip install c104~=1.16.0
 ```
 
-#### Add to requirements.txt
-```
-c104~=1.16.0
-```
-
-### Source distribution
-
-#### Install from source
-
+### Install from git
 ```bash
-sudo apt-get install build-essential python3-dev python3-pip
 python3 -m pip install c104@git+https://github.com/fraunhofer-fit-dien/iec104-python.git@v1.16.0
 ```
 
-#### Add to requirements.txt
-```
-c104 @ git+https://github.com/fraunhofer-fit-dien/iec104-python.git@v1.16.0
-```
-
 ## Wiki
 
-Read more about the **Classes** and their **Properties** in our [project Wiki](https://iec104-python.readthedocs.io/).
+Read more about the **Classes** and their **Properties** in our [project Wiki](https://iec104-python.readthedocs.io/python/index.html).
 
 ## Contribution
 
 ### How to contribute
 
 1. Add feature requests and report bugs using GitHub's issues
```

