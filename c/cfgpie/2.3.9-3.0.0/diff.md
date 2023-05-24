# Comparing `tmp/cfgpie-2.3.9.tar.gz` & `tmp/cfgpie-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfgpie-2.3.9.tar", last modified: Thu Dec 29 12:42:45 2022, max compression
+gzip compressed data, was "cfgpie-3.0.0.tar", last modified: Wed May 24 15:26:51 2023, max compression
```

## Comparing `cfgpie-2.3.9.tar` & `cfgpie-3.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-12-29 12:42:45.958235 cfgpie-2.3.9/
--rw-rw-rw-   0        0        0     1090 2022-09-04 11:44:11.000000 cfgpie-2.3.9/LICENSE
--rw-rw-rw-   0        0        0       14 2022-10-24 07:53:37.000000 cfgpie-2.3.9/MANIFEST.in
--rw-rw-rw-   0        0        0     6191 2022-12-29 12:42:45.958235 cfgpie-2.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     5234 2022-12-29 12:36:33.000000 cfgpie-2.3.9/README.md
--rw-rw-rw-   0        0        0       93 2022-08-10 18:07:14.000000 cfgpie-2.3.9/pyproject.toml
--rw-rw-rw-   0        0        0     1084 2022-12-29 12:42:45.958235 cfgpie-2.3.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-12-29 12:42:45.938493 cfgpie-2.3.9/src/
-drwxrwxrwx   0        0        0        0 2022-12-29 12:42:45.947256 cfgpie-2.3.9/src/cfgpie/
--rw-rw-rw-   0        0        0      384 2022-12-29 12:07:25.000000 cfgpie-2.3.9/src/cfgpie/__init__.py
--rw-rw-rw-   0        0        0      546 2022-10-04 17:04:28.000000 cfgpie-2.3.9/src/cfgpie/constants.py
--rw-rw-rw-   0        0        0      225 2022-10-02 15:56:49.000000 cfgpie-2.3.9/src/cfgpie/exceptions.py
--rw-rw-rw-   0        0        0     5850 2022-12-29 12:11:38.000000 cfgpie-2.3.9/src/cfgpie/handlers.py
--rw-rw-rw-   0        0        0      946 2022-12-01 16:27:10.000000 cfgpie-2.3.9/src/cfgpie/utils.py
-drwxrwxrwx   0        0        0        0 2022-12-29 12:42:45.947256 cfgpie-2.3.9/src/cfgpie.egg-info/
--rw-rw-rw-   0        0        0     6191 2022-12-29 12:42:45.000000 cfgpie-2.3.9/src/cfgpie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2022-12-29 12:42:45.000000 cfgpie-2.3.9/src/cfgpie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-29 12:42:45.000000 cfgpie-2.3.9/src/cfgpie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-04 16:13:39.000000 cfgpie-2.3.9/src/cfgpie.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2022-12-29 12:42:45.000000 cfgpie-2.3.9/src/cfgpie.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 15:26:51.759187 cfgpie-3.0.0/
+-rw-rw-rw-   0        0        0     1090 2022-09-04 11:44:11.000000 cfgpie-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0       14 2022-10-24 07:53:37.000000 cfgpie-3.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5732 2023-05-24 15:26:51.759187 cfgpie-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4929 2023-05-24 15:13:32.000000 cfgpie-3.0.0/README.md
+-rw-rw-rw-   0        0        0       93 2022-08-10 18:07:14.000000 cfgpie-3.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      963 2023-05-24 15:26:51.760185 cfgpie-3.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 15:26:51.738489 cfgpie-3.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 15:26:51.754262 cfgpie-3.0.0/src/cfgpie/
+-rw-rw-rw-   0        0        0      145 2023-05-24 14:22:23.000000 cfgpie-3.0.0/src/cfgpie/__init__.py
+-rw-rw-rw-   0        0        0      719 2023-05-24 14:22:23.000000 cfgpie-3.0.0/src/cfgpie/constants.py
+-rw-rw-rw-   0        0        0      275 2023-05-24 14:16:08.000000 cfgpie-3.0.0/src/cfgpie/exceptions.py
+-rw-rw-rw-   0        0        0     7353 2023-05-24 14:22:23.000000 cfgpie-3.0.0/src/cfgpie/handlers.py
+-rw-rw-rw-   0        0        0     1270 2023-05-24 14:08:16.000000 cfgpie-3.0.0/src/cfgpie/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:26:51.758182 cfgpie-3.0.0/src/cfgpie.egg-info/
+-rw-rw-rw-   0        0        0     5732 2023-05-24 15:26:51.000000 cfgpie-3.0.0/src/cfgpie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-05-24 15:26:51.000000 cfgpie-3.0.0/src/cfgpie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 15:26:51.000000 cfgpie-3.0.0/src/cfgpie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-04 16:13:39.000000 cfgpie-3.0.0/src/cfgpie.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-05-24 15:26:51.000000 cfgpie-3.0.0/src/cfgpie.egg-info/top_level.txt
```

### Comparing `cfgpie-2.3.9/LICENSE` & `cfgpie-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cfgpie-2.3.9/PKG-INFO` & `cfgpie-3.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
 Name: cfgpie
-Version: 2.3.9
+Version: 3.0.0
 Summary: Simplified `ConfigParser` setup.
 Home-page: https://github.com/ClaudiuDrug/cfgpie
 Author: Claudiu DRUG
 Author-email: claudiu.drug@outlook.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/ClaudiuDrug/cfgpie/issues
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
@@ -37,133 +34,126 @@
 python -m pip install [--upgrade] cfgpie
 ```
 
 ---
 
 #### Usage:
 
-After installation, simply import the method `get_config` from `cfgpie` module:
+After installation, simply import the class `CfgParser` from `cfgpie` module:
+
 ```python
-from cfgpie import CfgParser, get_config
+from cfgpie import CfgParser
 ```
 
-By passing a name with the `name` param we can have multiple instances:
+By passing a name with the `name` param we can have multiple named instances:
+
 ```python
 # mymodule.py
 
-from cfgpie import CfgParser, get_config
+from cfgpie import CfgParser
 
-cfg: CfgParser = get_config(name="main")
-cfg2: CfgParser = get_config(name="main")
-other: CfgParser = get_config(name="other")
+cfg1: CfgParser = CfgParser(name="root")
+cfg2: CfgParser = CfgParser(name="root")
+cfg3: CfgParser = CfgParser(name="other")
 
 
 if __name__ == '__main__':
 
     print("*" * 80)
-    print("cfg:", cfg.name)
+    print("cfg1:", cfg1.name)
     print("cfg2:", cfg2.name)
-    print("other:", other.name)
+    print("cfg3:", cfg3.name)
 
     print("*" * 80)
-    print("cfg == other:", cfg == other)
-    print("cfg is other:", cfg is other)
+    print("cfg1 == cfg3:", cfg1 == cfg3)
+    print("cfg1 is cfg3:", cfg1 is cfg3)
 
     print("*" * 80)
-    print("cfg == cfg2:", cfg == cfg2)
-    print("cfg is cfg2:", cfg is cfg2)
+    print("cfg1 == cfg2:", cfg1 == cfg2)
+    print("cfg1 is cfg2:", cfg1 is cfg2)
 ```
 
 ```
 ********************************************************************************
-cfg: main.CfgParser
-cfg2: main.CfgParser
-other: other.CfgParser
+cfg1: root
+cfg2: root
+cfg3: other
 ********************************************************************************
-cfg == other: False
-cfg is other: False
+cfg1 == cfg3: False
+cfg1 is cfg3: False
 ********************************************************************************
-cfg == cfg2: True
-cfg is cfg2: True
+cfg1 == cfg2: True
+cfg1 is cfg2: True
 ```
 
-Setting up our config environment:
+Setting up our configuration:
 
 ```python
-# constants.py
+# -*- coding: UTF-8 -*-
 
-from os.path import join, dirname, realpath
+from os.path import dirname, realpath, join
 from sys import modules
 from types import ModuleType
 
-# main module:
+from cfgpie import CfgParser
+
+# main python module:
 MODULE: ModuleType = modules.get("__main__")
 
 # root directory:
 ROOT: str = dirname(realpath(MODULE.__file__))
 
-# default config file path:
+# config default file path:
 CONFIG: str = join(ROOT, "config", "config.ini")
 
-# backup config params:
 BACKUP: dict = {
     "FOLDERS": {
-        "logger": r"${DEFAULT:directory}\logs",
+        "logger": r"${DEFAULT:directory}\logs",  # extended interpolation
     },
     "TESTS": {
         "option_1": "some_value",
         "option_2": 23453,
         "option_3": True,
         "option_4": r"${DEFAULT:directory}\value",  # extended interpolation
         "option_5": ["abc", 345, 232.545, "3534.5435", True, {"key_": "value_"}, False],
-    },
+    }
 }
-```
-
-For interpolation, refer to `interpolation-of-values`
-[documentation](https://docs.python.org/3.7/library/configparser.html#interpolation-of-values).
-
-```python
-# mymodule.py
 
-from cfgpie import CfgParser, get_config
+cfg: CfgParser = CfgParser(
+    "root",
+    defaults={"directory": ROOT}
+)
 
-from .constants import ROOT, CONFIG, BACKUP
-
-cfg: CfgParser = get_config(name="main")
-
-# we can set default section options:
-cfg.set_defaults(directory=ROOT)
-# also possible at instance creation:
-# cfg: CfgParser = get_config(defaults=some_dict)
+# we can update `DEFAULT` section:
+# cfg.set_defaults(directory=ROOT)
 
 # we can provide a backup dictionary
 # in case our config file does not exist
 # and by default a new file will be created
-cfg.open(file_path=CONFIG, encoding="UTF-8", fallback=BACKUP)
+cfg.open(
+    file_path=CONFIG,
+    encoding="UTF-8",
+    fallback=BACKUP,
+)
 
 
 if __name__ == '__main__':
 
     # we're parsing cmd-line arguments
-    cfg.parse()
+    cfg.read_argv()
+    
+    # cmd-args are fetched as a list of strings:
+    # cfg.read_argv(["--tests-option_1", "another_value", "--tests-option_2", "6543"])
 
     print(cfg.get("TESTS", "option_1"))
     print(cfg.getint("TESTS", "option_2"))
 ```
 
-This is also possible given that cmd-args are fetched as a list of strings:
-
-```python
-if __name__ == '__main__':
-    cfg.parse(["--tests-option_1", "another_value", "--tests-option_2", "6543"])
-
-    print(cfg.get("TESTS", "option_1"))
-    print(cfg.getint("TESTS", "option_2"))
-```
+For interpolation, refer to `interpolation-of-values`
+[documentation](https://docs.python.org/3.7/library/configparser.html#interpolation-of-values).
 
 To pass cmd-line arguments:
 
 ```commandline
 python -O main.py --section-option value --section-option value
 ```
 cmd-line args have priority over config file and will override the cfg params.
```

### Comparing `cfgpie-2.3.9/README.md` & `cfgpie-3.0.0/src/cfgpie.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: cfgpie
+Version: 3.0.0
+Summary: Simplified `ConfigParser` setup.
+Home-page: https://github.com/ClaudiuDrug/cfgpie
+Author: Claudiu DRUG
+Author-email: claudiu.drug@outlook.com
+License: MIT License
+Project-URL: Bug Tracker, https://github.com/ClaudiuDrug/cfgpie/issues
+Classifier: Programming Language :: Python :: 3.7
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # cfgpie
 
 Simplified `ConfigParser` setup.
 
 This module automates, to some extent, the setup of [ConfigParser](https://docs.python.org/3.7/library/configparser.html)
 with cmd-line args parsing ability.
 
@@ -13,133 +34,126 @@
 python -m pip install [--upgrade] cfgpie
 ```
 
 ---
 
 #### Usage:
 
-After installation, simply import the method `get_config` from `cfgpie` module:
+After installation, simply import the class `CfgParser` from `cfgpie` module:
+
 ```python
-from cfgpie import CfgParser, get_config
+from cfgpie import CfgParser
 ```
 
-By passing a name with the `name` param we can have multiple instances:
+By passing a name with the `name` param we can have multiple named instances:
+
 ```python
 # mymodule.py
 
-from cfgpie import CfgParser, get_config
+from cfgpie import CfgParser
 
-cfg: CfgParser = get_config(name="main")
-cfg2: CfgParser = get_config(name="main")
-other: CfgParser = get_config(name="other")
+cfg1: CfgParser = CfgParser(name="root")
+cfg2: CfgParser = CfgParser(name="root")
+cfg3: CfgParser = CfgParser(name="other")
 
 
 if __name__ == '__main__':
 
     print("*" * 80)
-    print("cfg:", cfg.name)
+    print("cfg1:", cfg1.name)
     print("cfg2:", cfg2.name)
-    print("other:", other.name)
+    print("cfg3:", cfg3.name)
 
     print("*" * 80)
-    print("cfg == other:", cfg == other)
-    print("cfg is other:", cfg is other)
+    print("cfg1 == cfg3:", cfg1 == cfg3)
+    print("cfg1 is cfg3:", cfg1 is cfg3)
 
     print("*" * 80)
-    print("cfg == cfg2:", cfg == cfg2)
-    print("cfg is cfg2:", cfg is cfg2)
+    print("cfg1 == cfg2:", cfg1 == cfg2)
+    print("cfg1 is cfg2:", cfg1 is cfg2)
 ```
 
 ```
 ********************************************************************************
-cfg: main.CfgParser
-cfg2: main.CfgParser
-other: other.CfgParser
+cfg1: root
+cfg2: root
+cfg3: other
 ********************************************************************************
-cfg == other: False
-cfg is other: False
+cfg1 == cfg3: False
+cfg1 is cfg3: False
 ********************************************************************************
-cfg == cfg2: True
-cfg is cfg2: True
+cfg1 == cfg2: True
+cfg1 is cfg2: True
 ```
 
-Setting up our config environment:
+Setting up our configuration:
 
 ```python
-# constants.py
+# -*- coding: UTF-8 -*-
 
-from os.path import join, dirname, realpath
+from os.path import dirname, realpath, join
 from sys import modules
 from types import ModuleType
 
-# main module:
+from cfgpie import CfgParser
+
+# main python module:
 MODULE: ModuleType = modules.get("__main__")
 
 # root directory:
 ROOT: str = dirname(realpath(MODULE.__file__))
 
-# default config file path:
+# config default file path:
 CONFIG: str = join(ROOT, "config", "config.ini")
 
-# backup config params:
 BACKUP: dict = {
     "FOLDERS": {
-        "logger": r"${DEFAULT:directory}\logs",
+        "logger": r"${DEFAULT:directory}\logs",  # extended interpolation
     },
     "TESTS": {
         "option_1": "some_value",
         "option_2": 23453,
         "option_3": True,
         "option_4": r"${DEFAULT:directory}\value",  # extended interpolation
         "option_5": ["abc", 345, 232.545, "3534.5435", True, {"key_": "value_"}, False],
-    },
+    }
 }
-```
-
-For interpolation, refer to `interpolation-of-values`
-[documentation](https://docs.python.org/3.7/library/configparser.html#interpolation-of-values).
-
-```python
-# mymodule.py
 
-from cfgpie import CfgParser, get_config
+cfg: CfgParser = CfgParser(
+    "root",
+    defaults={"directory": ROOT}
+)
 
-from .constants import ROOT, CONFIG, BACKUP
-
-cfg: CfgParser = get_config(name="main")
-
-# we can set default section options:
-cfg.set_defaults(directory=ROOT)
-# also possible at instance creation:
-# cfg: CfgParser = get_config(defaults=some_dict)
+# we can update `DEFAULT` section:
+# cfg.set_defaults(directory=ROOT)
 
 # we can provide a backup dictionary
 # in case our config file does not exist
 # and by default a new file will be created
-cfg.open(file_path=CONFIG, encoding="UTF-8", fallback=BACKUP)
+cfg.open(
+    file_path=CONFIG,
+    encoding="UTF-8",
+    fallback=BACKUP,
+)
 
 
 if __name__ == '__main__':
 
     # we're parsing cmd-line arguments
-    cfg.parse()
+    cfg.read_argv()
+    
+    # cmd-args are fetched as a list of strings:
+    # cfg.read_argv(["--tests-option_1", "another_value", "--tests-option_2", "6543"])
 
     print(cfg.get("TESTS", "option_1"))
     print(cfg.getint("TESTS", "option_2"))
 ```
 
-This is also possible given that cmd-args are fetched as a list of strings:
-
-```python
-if __name__ == '__main__':
-    cfg.parse(["--tests-option_1", "another_value", "--tests-option_2", "6543"])
-
-    print(cfg.get("TESTS", "option_1"))
-    print(cfg.getint("TESTS", "option_2"))
-```
+For interpolation, refer to `interpolation-of-values`
+[documentation](https://docs.python.org/3.7/library/configparser.html#interpolation-of-values).
 
 To pass cmd-line arguments:
 
 ```commandline
 python -O main.py --section-option value --section-option value
 ```
 cmd-line args have priority over config file and will override the cfg params.
```

### Comparing `cfgpie-2.3.9/setup.cfg` & `cfgpie-3.0.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6667 7069 650d 0a76 6572 7369   = cfgpie..versi
-00000020: 6f6e 203d 2032 2e33 2e39 0d0a 6175 7468  on = 2.3.9..auth
+00000020: 6f6e 203d 2033 2e30 2e30 0d0a 6175 7468  on = 3.0.0..auth
 00000030: 6f72 203d 2043 6c61 7564 6975 2044 5255  or = Claudiu DRU
 00000040: 470d 0a61 7574 686f 725f 656d 6169 6c20  G..author_email 
 00000050: 3d20 636c 6175 6469 752e 6472 7567 406f  = claudiu.drug@o
 00000060: 7574 6c6f 6f6b 2e63 6f6d 0d0a 6c69 6365  utlook.com..lice
 00000070: 6e73 6520 3d20 4d49 5420 4c69 6365 6e73  nse = MIT Licens
 00000080: 650d 0a64 6573 6372 6970 7469 6f6e 203d  e..description =
 00000090: 2053 696d 706c 6966 6965 6420 6043 6f6e   Simplified `Con
@@ -21,48 +21,41 @@
 00000140: 3d20 0d0a 0942 7567 2054 7261 636b 6572  = ...Bug Tracker
 00000150: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
 00000160: 622e 636f 6d2f 436c 6175 6469 7544 7275  b.com/ClaudiuDru
 00000170: 672f 6366 6770 6965 2f69 7373 7565 730d  g/cfgpie/issues.
 00000180: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
 00000190: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
 000001a0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000001b0: 203a 3a20 332e 370d 0a09 5072 6f67 7261   :: 3.7...Progra
-000001c0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000001d0: 3a20 5079 7468 6f6e 203a 3a20 332e 380d  : Python :: 3.8.
-000001e0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-000001f0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000200: 203a 3a20 332e 390d 0a09 5072 6f67 7261   :: 3.9...Progra
-00000210: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000220: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
-00000230: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
-00000240: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
-00000250: 5420 4c69 6365 6e73 650d 0a09 4f70 6572  T License...Oper
-00000260: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000270: 4d69 6372 6f73 6f66 7420 3a3a 2057 696e  Microsoft :: Win
-00000280: 646f 7773 203a 3a20 5769 6e64 6f77 7320  dows :: Windows 
-00000290: 3130 0d0a 094f 7065 7261 7469 6e67 2053  10...Operating S
-000002a0: 7973 7465 6d20 3a3a 2050 4f53 4958 203a  ystem :: POSIX :
-000002b0: 3a20 4c69 6e75 780d 0a09 496e 7465 6e64  : Linux...Intend
-000002c0: 6564 2041 7564 6965 6e63 6520 3a3a 2044  ed Audience :: D
-000002d0: 6576 656c 6f70 6572 730d 0a09 4e61 7475  evelopers...Natu
-000002e0: 7261 6c20 4c61 6e67 7561 6765 203a 3a20  ral Language :: 
-000002f0: 456e 676c 6973 680d 0a09 546f 7069 6320  English...Topic 
-00000300: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
-00000310: 6c6f 706d 656e 7420 3a3a 204c 6962 7261  lopment :: Libra
-00000320: 7269 6573 203a 3a20 5079 7468 6f6e 204d  ries :: Python M
-00000330: 6f64 756c 6573 0d0a 0954 6f70 6963 203a  odules...Topic :
-00000340: 3a20 5574 696c 6974 6965 730d 0a0d 0a5b  : Utilities....[
-00000350: 6f70 7469 6f6e 735d 0d0a 7a69 705f 7361  options]..zip_sa
-00000360: 6665 203d 2046 616c 7365 0d0a 7061 636b  fe = False..pack
-00000370: 6167 6573 203d 2066 696e 645f 6e61 6d65  ages = find_name
-00000380: 7370 6163 653a 0d0a 7061 636b 6167 655f  space:..package_
-00000390: 6469 7220 3d20 0d0a 093d 2073 7263 0d0a  dir = ...= src..
-000003a0: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
-000003b0: 6461 7461 203d 2054 7275 650d 0a70 7974  data = True..pyt
-000003c0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-000003d0: 3d20 332e 370d 0a0d 0a5b 6f70 7469 6f6e  = 3.7....[option
-000003e0: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
-000003f0: 0d0a 7768 6572 6520 3d20 7372 630d 0a65  ..where = src..e
-00000400: 7863 6c75 6465 203d 2074 6573 7473 0d0a  xclude = tests..
-00000410: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-00000420: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000430: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+000001b0: 203a 3a20 332e 370d 0a09 4c69 6365 6e73   :: 3.7...Licens
+000001c0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+000001d0: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
+000001e0: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
+000001f0: 7465 6d20 3a3a 204d 6963 726f 736f 6674  tem :: Microsoft
+00000200: 203a 3a20 5769 6e64 6f77 7320 3a3a 2057   :: Windows :: W
+00000210: 696e 646f 7773 2031 300d 0a09 4f70 6572  indows 10...Oper
+00000220: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+00000230: 504f 5349 5820 3a3a 204c 696e 7578 0d0a  POSIX :: Linux..
+00000240: 0949 6e74 656e 6465 6420 4175 6469 656e  .Intended Audien
+00000250: 6365 203a 3a20 4465 7665 6c6f 7065 7273  ce :: Developers
+00000260: 0d0a 094e 6174 7572 616c 204c 616e 6775  ...Natural Langu
+00000270: 6167 6520 3a3a 2045 6e67 6c69 7368 0d0a  age :: English..
+00000280: 0954 6f70 6963 203a 3a20 536f 6674 7761  .Topic :: Softwa
+00000290: 7265 2044 6576 656c 6f70 6d65 6e74 203a  re Development :
+000002a0: 3a20 4c69 6272 6172 6965 7320 3a3a 2050  : Libraries :: P
+000002b0: 7974 686f 6e20 4d6f 6475 6c65 730d 0a09  ython Modules...
+000002c0: 546f 7069 6320 3a3a 2055 7469 6c69 7469  Topic :: Utiliti
+000002d0: 6573 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  es....[options].
+000002e0: 0a7a 6970 5f73 6166 6520 3d20 4661 6c73  .zip_safe = Fals
+000002f0: 650d 0a70 6163 6b61 6765 7320 3d20 6669  e..packages = fi
+00000300: 6e64 5f6e 616d 6573 7061 6365 3a0d 0a70  nd_namespace:..p
+00000310: 6163 6b61 6765 5f64 6972 203d 200d 0a09  ackage_dir = ...
+00000320: 3d20 7372 630d 0a69 6e63 6c75 6465 5f70  = src..include_p
+00000330: 6163 6b61 6765 5f64 6174 6120 3d20 5472  ackage_data = Tr
+00000340: 7565 0d0a 7079 7468 6f6e 5f72 6571 7569  ue..python_requi
+00000350: 7265 7320 3d20 3e3d 2033 2e37 0d0a 0d0a  res = >= 3.7....
+00000360: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+00000370: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
+00000380: 2073 7263 0d0a 6578 636c 7564 6520 3d20   src..exclude = 
+00000390: 7465 7374 730d 0a0d 0a5b 6567 675f 696e  tests....[egg_in
+000003a0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
+000003b0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
+000003c0: 0a0d 0a                                  ...
```

### Comparing `cfgpie-2.3.9/src/cfgpie/constants.py` & `cfgpie-3.0.0/src/cfgpie/constants.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 # -*- coding: UTF-8 -*-
 
 from os.path import dirname, realpath, join
 from sys import modules
 from types import ModuleType
-from typing import TypeVar
 from weakref import WeakValueDictionary
 
-# types:
-Key = TypeVar("Key")
-Value = TypeVar("Value")
+__all__ = [
+    "NAME",
+    "INSTANCES",
+    "RLOCKS",
+    "ROOT",
+    "CONFIG",
+]
 
-# container for all instances:
-INSTANCES = WeakValueDictionary()
+# default instance name:
+NAME: str = "cfgpie"
+
+# config parser instances container:
+INSTANCES: WeakValueDictionary = WeakValueDictionary()
+
+# recursive thread locks container:
+RLOCKS: WeakValueDictionary = WeakValueDictionary()
 
 # main python module:
 MODULE: ModuleType = modules.get("__main__")
 
 # root directory:
 ROOT: str = dirname(realpath(MODULE.__file__))
```

