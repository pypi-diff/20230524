# Comparing `tmp/vedro-valera-validator-1.1.0.tar.gz` & `tmp/vedro-valera-validator-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vedro-valera-validator-1.1.0.tar", last modified: Wed Aug 24 20:05:52 2022, max compression
+gzip compressed data, was "vedro-valera-validator-1.1.1.tar", last modified: Wed May 24 20:35:12 2023, max compression
```

## Comparing `vedro-valera-validator-1.1.0.tar` & `vedro-valera-validator-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 20:05:52.787388 vedro-valera-validator-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-24 20:05:43.000000 vedro-valera-validator-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2295 2022-08-24 20:05:52.787388 vedro-valera-validator-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1704 2022-08-24 20:05:43.000000 vedro-valera-validator-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-08-24 20:05:52.787388 vedro-valera-validator-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-08-24 20:05:43.000000 vedro-valera-validator-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 20:05:52.787388 vedro-valera-validator-1.1.0/vedro_valera_validator/
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-08-24 20:05:43.000000 vedro-valera-validator-1.1.0/vedro_valera_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-08-24 20:05:43.000000 vedro-valera-validator-1.1.0/vedro_valera_validator/_valera_validator.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-24 20:05:43.000000 vedro-valera-validator-1.1.0/vedro_valera_validator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 20:05:52.787388 vedro-valera-validator-1.1.0/vedro_valera_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2295 2022-08-24 20:05:52.000000 vedro-valera-validator-1.1.0/vedro_valera_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-08-24 20:05:52.000000 vedro-valera-validator-1.1.0/vedro_valera_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-24 20:05:52.000000 vedro-valera-validator-1.1.0/vedro_valera_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-08-24 20:05:52.000000 vedro-valera-validator-1.1.0/vedro_valera_validator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-24 20:05:52.000000 vedro-valera-validator-1.1.0/vedro_valera_validator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:35:12.767815 vedro-valera-validator-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 20:35:03.000000 vedro-valera-validator-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-24 20:35:12.767815 vedro-valera-validator-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-24 20:35:03.000000 vedro-valera-validator-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-24 20:35:12.767815 vedro-valera-validator-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-24 20:35:03.000000 vedro-valera-validator-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:35:12.767815 vedro-valera-validator-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-24 20:35:03.000000 vedro-valera-validator-1.1.1/tests/test_valera_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:35:12.767815 vedro-valera-validator-1.1.1/vedro_valera_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-24 20:35:03.000000 vedro-valera-validator-1.1.1/vedro_valera_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-24 20:35:03.000000 vedro-valera-validator-1.1.1/vedro_valera_validator/_valera_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:35:03.000000 vedro-valera-validator-1.1.1/vedro_valera_validator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:35:12.767815 vedro-valera-validator-1.1.1/vedro_valera_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-24 20:35:12.000000 vedro-valera-validator-1.1.1/vedro_valera_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-24 20:35:12.000000 vedro-valera-validator-1.1.1/vedro_valera_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:35:12.000000 vedro-valera-validator-1.1.1/vedro_valera_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-24 20:35:12.000000 vedro-valera-validator-1.1.1/vedro_valera_validator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 20:35:12.000000 vedro-valera-validator-1.1.1/vedro_valera_validator.egg-info/top_level.txt
```

### Comparing `vedro-valera-validator-1.1.0/LICENSE` & `vedro-valera-validator-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vedro-valera-validator-1.1.0/PKG-INFO` & `vedro-valera-validator-1.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,64 @@
-Metadata-Version: 2.1
-Name: vedro-valera-validator
-Version: 1.1.0
-Summary: Validator for Vedro framework
-Home-page: https://github.com/nikitanovosibirsk/vedro-valera-validator
-Author: Nikita Tsvetkov
-Author-email: nikitanovosibirsk@yandex.com
-License: Apache-2.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Typing :: Typed
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Vedro Valera Validator
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/vedro-valera-validator/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/vedro-valera-validator)
+[![Codecov](https://img.shields.io/codecov/c/github/vedro-universe/vedro-valera-validator/master.svg?style=flat-square)](https://codecov.io/gh/vedro-universe/vedro-valera-validator)
 [![PyPI](https://img.shields.io/pypi/v/vedro-valera-validator.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-valera-validator/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-valera-validator?style=flat-square)](https://pypi.python.org/pypi/vedro-valera-validator/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro-valera-validator.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-valera-validator/)
 
-## Installation
+Validator plugin for the [Vedro](https://vedro.io) testing framework.
+
+## How to Install
 
-### 1. Install package
+<details open>
+<summary>Quick</summary>
+<p>
+
+For a quick installation, you can use a plugin manager like so:
+
+```shell
+$ vedro plugin install vedro-valera-validator
+```
+
+</p>
+</details>
+
+<details>
+<summary>Manual</summary>
+<p>
+
+To install manually, follow these steps:
+
+1. Install the package using pip:
 
 ```shell
 $ pip3 install vedro-valera-validator
 ```
 
-### 2. Enable plugin
+2. Then, enable the plugin in the `vedro.cfg.py` configuration file:
 
 ```python
 # ./vedro.cfg.py
 import vedro
-import vedro_valera_validator as valera_validator
+import vedro_valera_validator
 
 class Config(vedro.Config):
 
     class Plugins(vedro.Config.Plugins):
 
-        class ValeraValidator(valera_validator.ValeraValidator):
+        class ValeraValidator(vedro_valera_validator.ValeraValidator):
             enabled = True
 ```
 
-## Usage
+</p>
+</details>
+
+## How to Use
+
+Here is an example scenario demonstrating how to decode a base64 encoded string:
 
 ```python
 # ./scenarios/decode_base64_encoded_string.py
 import vedro
 from base64 import b64decode
 from d42 import schema
 
@@ -66,17 +75,23 @@
 
     def then(self):
         assert self.result == schema.dict({
             "result": schema.bytes(b"banana")
         })
 ```
 
-### Run tests
+Run the test using the command:
 
 ```shell
 $ vedro run -vv
 ```
 
+If the expected and actual results do not match, a `ValidationException` will be thrown, as shown below:
+
 ```shell
 ValidationException:
  - Value <class 'bytes'> at _['result'] must be equal to b'banana', but b'cucumber' given
  ```
+
+## Further Reading
+
+For comprehensive guidance and more information, refer to the [official documentation](https://vedro.io/en/docs/integrations/valera-validator).
```

### Comparing `vedro-valera-validator-1.1.0/setup.cfg` & `vedro-valera-validator-1.1.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.1.0
+current_version = 1.1.1
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `vedro-valera-validator-1.1.0/setup.py` & `vedro-valera-validator-1.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="vedro-valera-validator",
-    version="1.1.0",
-    description="Validator for Vedro framework",
+    version="1.1.1",
+    description="Validator plugin for the Vedro testing framework",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
-    author_email="nikitanovosibirsk@yandex.com",
+    author_email="tsv1@fastmail.com",
     python_requires=">=3.8",
-    url="https://github.com/nikitanovosibirsk/vedro-valera-validator",
+    url="https://github.com/vedro-universe/vedro-valera-validator",
     license="Apache-2.0",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"vedro_valera_validator": ["py.typed"]},
     install_requires=find_required(),
     tests_require=find_dev_required(),
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
     ],
 )
```

### Comparing `vedro-valera-validator-1.1.0/vedro_valera_validator/_valera_validator.py` & `vedro-valera-validator-1.1.1/vedro_valera_validator/_valera_validator.py`

 * *Files identical despite different names*

### Comparing `vedro-valera-validator-1.1.0/vedro_valera_validator.egg-info/PKG-INFO` & `vedro-valera-validator-1.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,82 @@
 Metadata-Version: 2.1
 Name: vedro-valera-validator
-Version: 1.1.0
-Summary: Validator for Vedro framework
-Home-page: https://github.com/nikitanovosibirsk/vedro-valera-validator
+Version: 1.1.1
+Summary: Validator plugin for the Vedro testing framework
+Home-page: https://github.com/vedro-universe/vedro-valera-validator
 Author: Nikita Tsvetkov
-Author-email: nikitanovosibirsk@yandex.com
+Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Vedro Valera Validator
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/vedro-valera-validator/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/vedro-valera-validator)
+[![Codecov](https://img.shields.io/codecov/c/github/vedro-universe/vedro-valera-validator/master.svg?style=flat-square)](https://codecov.io/gh/vedro-universe/vedro-valera-validator)
 [![PyPI](https://img.shields.io/pypi/v/vedro-valera-validator.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-valera-validator/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-valera-validator?style=flat-square)](https://pypi.python.org/pypi/vedro-valera-validator/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro-valera-validator.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-valera-validator/)
 
-## Installation
+Validator plugin for the [Vedro](https://vedro.io) testing framework.
 
-### 1. Install package
+## How to Install
+
+<details open>
+<summary>Quick</summary>
+<p>
+
+For a quick installation, you can use a plugin manager like so:
+
+```shell
+$ vedro plugin install vedro-valera-validator
+```
+
+</p>
+</details>
+
+<details>
+<summary>Manual</summary>
+<p>
+
+To install manually, follow these steps:
+
+1. Install the package using pip:
 
 ```shell
 $ pip3 install vedro-valera-validator
 ```
 
-### 2. Enable plugin
+2. Then, enable the plugin in the `vedro.cfg.py` configuration file:
 
 ```python
 # ./vedro.cfg.py
 import vedro
-import vedro_valera_validator as valera_validator
+import vedro_valera_validator
 
 class Config(vedro.Config):
 
     class Plugins(vedro.Config.Plugins):
 
-        class ValeraValidator(valera_validator.ValeraValidator):
+        class ValeraValidator(vedro_valera_validator.ValeraValidator):
             enabled = True
 ```
 
-## Usage
+</p>
+</details>
+
+## How to Use
+
+Here is an example scenario demonstrating how to decode a base64 encoded string:
 
 ```python
 # ./scenarios/decode_base64_encoded_string.py
 import vedro
 from base64 import b64decode
 from d42 import schema
 
@@ -66,17 +93,23 @@
 
     def then(self):
         assert self.result == schema.dict({
             "result": schema.bytes(b"banana")
         })
 ```
 
-### Run tests
+Run the test using the command:
 
 ```shell
 $ vedro run -vv
 ```
 
+If the expected and actual results do not match, a `ValidationException` will be thrown, as shown below:
+
 ```shell
 ValidationException:
  - Value <class 'bytes'> at _['result'] must be equal to b'banana', but b'cucumber' given
  ```
+
+## Further Reading
+
+For comprehensive guidance and more information, refer to the [official documentation](https://vedro.io/en/docs/integrations/valera-validator).
```

