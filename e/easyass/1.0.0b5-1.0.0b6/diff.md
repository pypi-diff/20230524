# Comparing `tmp/easyass-1.0.0b5.tar.gz` & `tmp/easyass-1.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyass-1.0.0b5.tar", last modified: Wed May 24 15:49:50 2023, max compression
+gzip compressed data, was "easyass-1.0.0b6.tar", last modified: Wed May 24 15:54:18 2023, max compression
```

## Comparing `easyass-1.0.0b5.tar` & `easyass-1.0.0b6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 15:49:50.802709 easyass-1.0.0b5/
--rw-rw-rw-   0        0        0     1098 2023-05-22 16:23:51.000000 easyass-1.0.0b5/LICENSE
--rw-rw-rw-   0        0        0     2310 2023-05-24 15:49:50.801705 easyass-1.0.0b5/PKG-INFO
--rw-rw-rw-   0        0        0     1825 2023-05-23 16:01:07.000000 easyass-1.0.0b5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 15:49:50.794673 easyass-1.0.0b5/easyass/
--rw-rw-rw-   0        0        0      138 2023-05-24 15:39:18.000000 easyass-1.0.0b5/easyass/__init__.py
--rw-rw-rw-   0        0        0     3763 2023-05-21 16:01:10.000000 easyass-1.0.0b5/easyass/ass_types.py
--rw-rw-rw-   0        0        0      906 2023-05-21 16:01:10.000000 easyass-1.0.0b5/easyass/base.py
-drwxrwxrwx   0        0        0        0 2023-05-24 15:49:50.797096 easyass-1.0.0b5/easyass/easyass.egg-info/
--rw-rw-rw-   0        0        0     2310 2023-05-24 15:49:50.000000 easyass-1.0.0b5/easyass/easyass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      467 2023-05-24 15:49:50.000000 easyass-1.0.0b5/easyass/easyass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 15:49:50.000000 easyass-1.0.0b5/easyass/easyass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-05-24 15:49:50.000000 easyass-1.0.0b5/easyass/easyass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1710 2023-05-24 15:44:05.000000 easyass-1.0.0b5/easyass/easyass.py
--rw-rw-rw-   0        0        0      415 2023-05-21 16:01:10.000000 easyass-1.0.0b5/easyass/errors.py
-drwxrwxrwx   0        0        0        0 2023-05-24 15:49:50.799698 easyass-1.0.0b5/easyass/events/
--rw-rw-rw-   0        0        0       44 2023-05-21 16:01:10.000000 easyass-1.0.0b5/easyass/events/__init__.py
--rw-rw-rw-   0        0        0     5694 2023-05-22 15:05:36.000000 easyass-1.0.0b5/easyass/events/events.py
--rw-rw-rw-   0        0        0    18140 2023-05-22 15:05:36.000000 easyass-1.0.0b5/easyass/events/text.py
-drwxrwxrwx   0        0        0        0 2023-05-24 15:49:50.800702 easyass-1.0.0b5/easyass/scriptinfo/
--rw-rw-rw-   0        0        0       27 2023-05-21 16:01:10.000000 easyass-1.0.0b5/easyass/scriptinfo/__init__.py
--rw-rw-rw-   0        0        0     3439 2023-05-22 15:05:36.000000 easyass-1.0.0b5/easyass/scriptinfo/scriptinfo.py
-drwxrwxrwx   0        0        0        0 2023-05-24 15:49:50.801705 easyass-1.0.0b5/easyass/styles/
--rw-rw-rw-   0        0        0       23 2023-05-21 16:01:10.000000 easyass-1.0.0b5/easyass/styles/__init__.py
--rw-rw-rw-   0        0        0     6443 2023-05-22 15:05:36.000000 easyass-1.0.0b5/easyass/styles/styles.py
--rw-rw-rw-   0        0        0       42 2023-05-24 15:49:50.802709 easyass-1.0.0b5/setup.cfg
--rw-rw-rw-   0        0        0      806 2023-05-24 15:49:21.000000 easyass-1.0.0b5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:54:18.616797 easyass-1.0.0b6/
+-rw-rw-rw-   0        0        0     1098 2023-05-22 16:23:51.000000 easyass-1.0.0b6/LICENSE
+-rw-rw-rw-   0        0        0     2310 2023-05-24 15:54:18.616797 easyass-1.0.0b6/PKG-INFO
+-rw-rw-rw-   0        0        0     1825 2023-05-23 16:01:07.000000 easyass-1.0.0b6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 15:54:18.609313 easyass-1.0.0b6/easyass/
+-rw-rw-rw-   0        0        0      138 2023-05-24 15:39:18.000000 easyass-1.0.0b6/easyass/__init__.py
+-rw-rw-rw-   0        0        0     3763 2023-05-21 16:01:10.000000 easyass-1.0.0b6/easyass/ass_types.py
+-rw-rw-rw-   0        0        0      906 2023-05-21 16:01:10.000000 easyass-1.0.0b6/easyass/base.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:54:18.611313 easyass-1.0.0b6/easyass/easyass.egg-info/
+-rw-rw-rw-   0        0        0     2310 2023-05-24 15:54:18.000000 easyass-1.0.0b6/easyass/easyass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      467 2023-05-24 15:54:18.000000 easyass-1.0.0b6/easyass/easyass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 15:54:18.000000 easyass-1.0.0b6/easyass/easyass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-05-24 15:54:18.000000 easyass-1.0.0b6/easyass/easyass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1710 2023-05-24 15:44:05.000000 easyass-1.0.0b6/easyass/easyass.py
+-rw-rw-rw-   0        0        0      415 2023-05-21 16:01:10.000000 easyass-1.0.0b6/easyass/errors.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:54:18.613328 easyass-1.0.0b6/easyass/events/
+-rw-rw-rw-   0        0        0       44 2023-05-21 16:01:10.000000 easyass-1.0.0b6/easyass/events/__init__.py
+-rw-rw-rw-   0        0        0     5678 2023-05-24 15:53:18.000000 easyass-1.0.0b6/easyass/events/events.py
+-rw-rw-rw-   0        0        0    18132 2023-05-24 15:53:22.000000 easyass-1.0.0b6/easyass/events/text.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:54:18.614316 easyass-1.0.0b6/easyass/scriptinfo/
+-rw-rw-rw-   0        0        0       27 2023-05-21 16:01:10.000000 easyass-1.0.0b6/easyass/scriptinfo/__init__.py
+-rw-rw-rw-   0        0        0     3423 2023-05-24 15:52:57.000000 easyass-1.0.0b6/easyass/scriptinfo/scriptinfo.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:54:18.615315 easyass-1.0.0b6/easyass/styles/
+-rw-rw-rw-   0        0        0       23 2023-05-21 16:01:10.000000 easyass-1.0.0b6/easyass/styles/__init__.py
+-rw-rw-rw-   0        0        0     6419 2023-05-24 15:53:29.000000 easyass-1.0.0b6/easyass/styles/styles.py
+-rw-rw-rw-   0        0        0       42 2023-05-24 15:54:18.616797 easyass-1.0.0b6/setup.cfg
+-rw-rw-rw-   0        0        0      806 2023-05-24 15:53:58.000000 easyass-1.0.0b6/setup.py
```

### Comparing `easyass-1.0.0b5/LICENSE` & `easyass-1.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `easyass-1.0.0b5/PKG-INFO` & `easyass-1.0.0b6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyass
-Version: 1.0.0b5
+Version: 1.0.0b6
 Summary: An ass subtitle parsing library
 Home-page: https://github.com/hihkm/easyAss
 Author: tikm
 Author-email: hkm@tikm.org
 License: MIT Licence
 Keywords: ass,subtitle
 Platform: all
```

### Comparing `easyass-1.0.0b5/README.md` & `easyass-1.0.0b6/README.md`

 * *Files identical despite different names*

### Comparing `easyass-1.0.0b5/easyass/ass_types.py` & `easyass-1.0.0b6/easyass/ass_types.py`

 * *Files identical despite different names*

### Comparing `easyass-1.0.0b5/easyass/base.py` & `easyass-1.0.0b6/easyass/base.py`

 * *Files identical despite different names*

### Comparing `easyass-1.0.0b5/easyass/easyass.egg-info/PKG-INFO` & `easyass-1.0.0b6/easyass/easyass.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyass
-Version: 1.0.0b5
+Version: 1.0.0b6
 Summary: An ass subtitle parsing library
 Home-page: https://github.com/hihkm/easyAss
 Author: tikm
 Author-email: hkm@tikm.org
 License: MIT Licence
 Keywords: ass,subtitle
 Platform: all
```

### Comparing `easyass-1.0.0b5/easyass/easyass.py` & `easyass-1.0.0b6/easyass/easyass.py`

 * *Files identical despite different names*

### Comparing `easyass-1.0.0b5/easyass/events/events.py` & `easyass-1.0.0b6/easyass/events/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum
 from .text import Text
 
-from easyass.ass_types import AssTime
-from easyass.errors import Errors
+from ass_types import AssTime
+from errors import Errors
 
 
 class Events(list):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.event_format: EventFormat = ...
```

### Comparing `easyass-1.0.0b5/easyass/events/text.py` & `easyass-1.0.0b6/easyass/events/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 import inspect
 import re
 
-from easyass.ass_types import AssColor
+from ass_types import AssColor
 
 
 class TextBase:
     _prefix = ''
     _with_bracket = True
     _arg_mapper: dict[str, dict] = ...
     """
```

### Comparing `easyass-1.0.0b5/easyass/scriptinfo/scriptinfo.py` & `easyass-1.0.0b6/easyass/scriptinfo/scriptinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from easyass.errors import Errors
-from easyass.base import AssAttr
+from errors import Errors
+from base import AssAttr
 
 
 class ScriptInfo:
     def __init__(self):
         self.script_info_attrs = {attr_name: None
                                   for attr_name in SCRIPT_INFO_ATTR_DEF.keys()}
         self.script_info_attrs.update({
```

### Comparing `easyass-1.0.0b5/easyass/styles/styles.py` & `easyass-1.0.0b6/easyass/styles/styles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from easyass.errors import Errors
-from easyass.base import AssAttr
-from easyass.ass_types import AssColor
+from errors import Errors
+from base import AssAttr
+from ass_types import AssColor
 
 
 class Styles(list):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.style_format: StyleFormat = StyleFormat()
```

### Comparing `easyass-1.0.0b5/setup.py` & `easyass-1.0.0b6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open(r'README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(
     name='easyass',
-    version='1.0.0b5',
+    version='1.0.0b6',
     keywords=['ass', 'subtitle'],
     description='An ass subtitle parsing library',
     license='MIT Licence',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     url='https://github.com/hihkm/easyAss',
```

