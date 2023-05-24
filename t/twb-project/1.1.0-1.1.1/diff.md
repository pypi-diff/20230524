# Comparing `tmp/twb_project-1.1.0.tar.gz` & `tmp/twb_project-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twb_project-1.1.0.tar", max compression
+gzip compressed data, was "twb_project-1.1.1.tar", max compression
```

## Comparing `twb_project-1.1.0.tar` & `twb_project-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-1.1.0/LICENSE
--rw-r--r--   0        0        0     1547 2023-05-21 20:04:40.510524 twb_project-1.1.0/README.md
--rw-r--r--   0        0        0      789 2023-05-22 12:50:03.416126 twb_project-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      143 2023-05-07 20:45:45.325589 twb_project-1.1.0/twb/__init__.py
--rw-r--r--   0        0        0    17182 2023-05-21 22:12:03.290444 twb_project-1.1.0/twb/builder.py
--rw-r--r--   0        0        0      227 2023-05-03 04:36:18.661146 twb_project-1.1.0/twb/builder_helpers.py
--rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-1.1.0/twb/decompressor.py
--rw-r--r--   0        0        0     3794 2023-04-20 07:59:01.227219 twb_project-1.1.0/twb/logger.py
--rw-r--r--   0        0        0     1817 2023-05-04 17:42:59.712780 twb_project-1.1.0/twb/logger_init.py
--rw-r--r--   0        0        0    10603 2023-05-02 23:19:18.752689 twb_project-1.1.0/twb/modifier.py
--rw-r--r--   0        0        0     9161 2023-04-20 02:54:12.926181 twb_project-1.1.0/twb/parallelization.py
--rw-r--r--   0        0        0     5527 2023-05-02 04:49:02.953589 twb_project-1.1.0/twb/reader.py
--rw-r--r--   0        0        0     6171 2023-05-07 20:45:49.998705 twb_project-1.1.0/twb/utils.py
--rw-r--r--   0        0        0     3727 2023-05-22 12:48:38.539400 twb_project-1.1.0/twb/warehouse.py
--rw-r--r--   0        0        0     2569 1970-01-01 00:00:00.000000 twb_project-1.1.0/setup.py
--rw-r--r--   0        0        0     2572 1970-01-01 00:00:00.000000 twb_project-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1547 2023-05-21 20:04:40.510524 twb_project-1.1.1/README.md
+-rw-r--r--   0        0        0      789 2023-05-24 01:45:19.534352 twb_project-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      143 2023-05-07 20:45:45.325589 twb_project-1.1.1/twb/__init__.py
+-rw-r--r--   0        0        0    17371 2023-05-24 01:44:19.877508 twb_project-1.1.1/twb/builder.py
+-rw-r--r--   0        0        0      227 2023-05-03 04:36:18.661146 twb_project-1.1.1/twb/builder_helpers.py
+-rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-1.1.1/twb/decompressor.py
+-rw-r--r--   0        0        0     3794 2023-04-20 07:59:01.227219 twb_project-1.1.1/twb/logger.py
+-rw-r--r--   0        0        0     1817 2023-05-04 17:42:59.712780 twb_project-1.1.1/twb/logger_init.py
+-rw-r--r--   0        0        0    10603 2023-05-02 23:19:18.752689 twb_project-1.1.1/twb/modifier.py
+-rw-r--r--   0        0        0     9161 2023-04-20 02:54:12.926181 twb_project-1.1.1/twb/parallelization.py
+-rw-r--r--   0        0        0     5527 2023-05-02 04:49:02.953589 twb_project-1.1.1/twb/reader.py
+-rw-r--r--   0        0        0     6171 2023-05-07 20:45:49.998705 twb_project-1.1.1/twb/utils.py
+-rw-r--r--   0        0        0     3727 2023-05-22 12:48:38.539400 twb_project-1.1.1/twb/warehouse.py
+-rw-r--r--   0        0        0     2569 1970-01-01 00:00:00.000000 twb_project-1.1.1/setup.py
+-rw-r--r--   0        0        0     2572 1970-01-01 00:00:00.000000 twb_project-1.1.1/PKG-INFO
```

### Comparing `twb_project-1.1.0/LICENSE` & `twb_project-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twb_project-1.1.0/README.md` & `twb_project-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `twb_project-1.1.0/pyproject.toml` & `twb_project-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twb-project"
-version = "1.1.0"
+version = "1.1.1"
 description = "An unified tool for the research in extracting information from Wikipedia Edit History chunk."
 authors = ["Lingxi Li <hi@lingxi.li>"]
 license = "GNU GPL"
 readme = "README.md"
 packages = [
     { include = "twb" },
 ]
@@ -14,15 +14,15 @@
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 py7zr = "^0.20.5"
 xmltodict = "^0.13.0"
 jsonlines = "^3.1.0"
 zstandard = "^0.21.0"
 psutil = "^5.9.5"
-requests = "^2.30.0"
+requests = "^2.31.0"
 beautifulsoup4 = "^4.12.2"
 tqdm = "^4.65.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 
 [tool.poetry.scripts]
```

### Comparing `twb_project-1.1.0/twb/builder.py` & `twb_project-1.1.1/twb/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import logging
 import os
+import shutil
 from functools import partial
 import multiprocessing as mp
 from typing import List, Tuple, Optional, TextIO
 import time
 import uuid
 
 import xmltodict
@@ -229,14 +230,18 @@
         except Exception as e:
             logging.critical(f'Error occurred when processing the file [{xml_file}]: {e}')
 
         try:
             # Remove XML file.
             os.remove(xml_path)
 
+            # Remove the directory if it becomes empty.
+            if not get_file_list(os.path.dirname(xml_path)):
+                shutil.rmtree(os.path.dirname(xml_path))
+
         except:
             logging.error(f'Failed to remove the XML file [{xml_path}].')
 
         logging.debug(f'Processed (OK): count = {processed_count}')
 
         return full_warehouse_paths
```

### Comparing `twb_project-1.1.0/twb/decompressor.py` & `twb_project-1.1.1/twb/decompressor.py`

 * *Files identical despite different names*

### Comparing `twb_project-1.1.0/twb/logger.py` & `twb_project-1.1.1/twb/logger.py`

 * *Files identical despite different names*

### Comparing `twb_project-1.1.0/twb/logger_init.py` & `twb_project-1.1.1/twb/logger_init.py`

 * *Files identical despite different names*

### Comparing `twb_project-1.1.0/twb/modifier.py` & `twb_project-1.1.1/twb/modifier.py`

 * *Files identical despite different names*

### Comparing `twb_project-1.1.0/twb/parallelization.py` & `twb_project-1.1.1/twb/parallelization.py`

 * *Files identical despite different names*

### Comparing `twb_project-1.1.0/twb/reader.py` & `twb_project-1.1.1/twb/reader.py`

 * *Files identical despite different names*

### Comparing `twb_project-1.1.0/twb/utils.py` & `twb_project-1.1.1/twb/utils.py`

 * *Files identical despite different names*

### Comparing `twb_project-1.1.0/twb/warehouse.py` & `twb_project-1.1.1/twb/warehouse.py`

 * *Files identical despite different names*

### Comparing `twb_project-1.1.0/setup.py` & `twb_project-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 {'': ['*']}
 
 install_requires = \
 ['beautifulsoup4>=4.12.2,<5.0.0',
  'jsonlines>=3.1.0,<4.0.0',
  'psutil>=5.9.5,<6.0.0',
  'py7zr>=0.20.5,<0.21.0',
- 'requests>=2.30.0,<3.0.0',
+ 'requests>=2.31.0,<3.0.0',
  'tqdm>=4.65.0,<5.0.0',
  'xmltodict>=0.13.0,<0.14.0',
  'zstandard>=0.21.0,<0.22.0']
 
 entry_points = \
 {'console_scripts': ['benchmark = tests.benchmark:main']}
 
 setup_kwargs = {
     'name': 'twb-project',
-    'version': '1.1.0',
+    'version': '1.1.1',
     'description': 'An unified tool for the research in extracting information from Wikipedia Edit History chunk.',
     'long_description': '<img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/007bbe1a-fc2b-4135-e9a6-0d8784004c00/HD" alt="TWB" />\n\n# Temporal Wikipedia Blocks (TWB)\n\nTemporal Wikipedia Blocks (TWB) is a powerful Python package designed to process the extensive edit history of Wikipedia pages into easily manageable and memory-friendly blocks. The package is specifically developed to enable efficient parallelization and composition of these blocks to facilitate faster processing and analysis of large Wikipedia datasets. The original design of this package is to build other Wikipedia-oriented datasets on top of it.\n\nThe package works by dividing the Wikipedia edit history into temporal blocks, which are essentially subsets of the complete dataset that are based on time intervals. These blocks can then be easily processed and analyzed without the need to load the entire dataset into memory.\n\n## Installation\n\nThe package is available on PyPI and can be installed using pip:\n\n```bash\npip install twb-project\n```\n\n## Benefits\n\n- **Efficient**: The package is designed to be memory-friendly and can be easily parallelized to process large datasets.\n- **Fast**: The package is designed to be fast and can be easily optimized to process large datasets.\n- **Flexible**: The package is designed to be flexible and can be easily extended to support other types of blocks.\n- **Composable**: The package is designed to be composable and can be easily combined with other packages to build other datasets.\n\n## Specification\n\n- Default compression method: ZStandard.\n',
     'author': 'Lingxi Li',
     'author_email': 'hi@lingxi.li',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://twb.lingxi.li/',
```

### Comparing `twb_project-1.1.0/PKG-INFO` & `twb_project-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twb-project
-Version: 1.1.0
+Version: 1.1.1
 Summary: An unified tool for the research in extracting information from Wikipedia Edit History chunk.
 Home-page: https://twb.lingxi.li/
 License: GNU GPL
 Author: Lingxi Li
 Author-email: hi@lingxi.li
 Requires-Python: >=3.8,<4
 Classifier: License :: Other/Proprietary License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: jsonlines (>=3.1.0,<4.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: py7zr (>=0.20.5,<0.21.0)
-Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Requires-Dist: zstandard (>=0.21.0,<0.22.0)
 Project-URL: Repository, https://github.com/lilingxi01/twb-project
 Description-Content-Type: text/markdown
 
 <img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/007bbe1a-fc2b-4135-e9a6-0d8784004c00/HD" alt="TWB" />
```

