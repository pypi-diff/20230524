# Comparing `tmp/jsonfmt-0.1.4.tar.gz` & `tmp/jsonfmt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonfmt-0.1.4.tar", last modified: Wed May 17 03:16:09 2023, max compression
+gzip compressed data, was "jsonfmt-0.2.0.tar", last modified: Wed May 24 03:53:33 2023, max compression
```

## Comparing `jsonfmt-0.1.4.tar` & `jsonfmt-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:16:09.595387 jsonfmt-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-17 03:15:53.000000 jsonfmt-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-17 03:16:09.595387 jsonfmt-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-17 03:15:53.000000 jsonfmt-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:16:09.591387 jsonfmt-0.1.4/jsonfmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-17 03:16:09.000000 jsonfmt-0.1.4/jsonfmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-17 03:16:09.000000 jsonfmt-0.1.4/jsonfmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 03:16:09.000000 jsonfmt-0.1.4/jsonfmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-17 03:16:09.000000 jsonfmt-0.1.4/jsonfmt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-17 03:16:09.000000 jsonfmt-0.1.4/jsonfmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 03:16:09.000000 jsonfmt-0.1.4/jsonfmt.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     5020 2023-05-17 03:15:53.000000 jsonfmt-0.1.4/jsonfmt.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-17 03:15:53.000000 jsonfmt-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 03:16:09.595387 jsonfmt-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:53:33.813517 jsonfmt-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-24 03:53:18.000000 jsonfmt-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-05-24 03:53:33.813517 jsonfmt-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-24 03:53:18.000000 jsonfmt-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:53:33.813517 jsonfmt-0.2.0/jsonfmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-05-24 03:53:33.000000 jsonfmt-0.2.0/jsonfmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-24 03:53:33.000000 jsonfmt-0.2.0/jsonfmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 03:53:33.000000 jsonfmt-0.2.0/jsonfmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-24 03:53:33.000000 jsonfmt-0.2.0/jsonfmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-24 03:53:33.000000 jsonfmt-0.2.0/jsonfmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 03:53:33.000000 jsonfmt-0.2.0/jsonfmt.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6926 2023-05-24 03:53:18.000000 jsonfmt-0.2.0/jsonfmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-24 03:53:18.000000 jsonfmt-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 03:53:33.813517 jsonfmt-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:53:33.813517 jsonfmt-0.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-05-24 03:53:18.000000 jsonfmt-0.2.0/test/test.py
```

### Comparing `jsonfmt-0.1.4/LICENSE` & `jsonfmt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonfmt-0.1.4/PKG-INFO` & `jsonfmt-0.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,196 +1,218 @@
 Metadata-Version: 2.1
 Name: jsonfmt
-Version: 0.1.4
+Version: 0.2.0
 Summary: A simple tool for formatting JSON object.
 Author-email: Seamile <lanhuermao@gmail.com>
-License: MIT
+License: MIT License
+Project-URL: homepage, https://github.com/seamile/jsonfmt
+Project-URL: repository, https://github.com/seamile/jsonfmt
+Project-URL: documentation, https://seamile.github.io/jsonfmt/
+Keywords: json,formatter,pretty-print,highlight,jsonpath
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: File Formats :: JSON
+Classifier: Topic :: Printing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JSON Formator
 
-![GitHub Build Status](https://img.shields.io/github/actions/workflow/status/seamile/jsonfmt/python-package.yml?label=Build&logo=python&logoColor=white)
-[![Downloads](https://static.pepy.tech/personalized-badge/jsonfmt?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Installs)](https://pepy.tech/project/jsonfmt)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
-[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
+[![Build Status](https://github.com/seamile/jsonfmt/actions/workflows/python-package.yml/badge.svg)](https://github.com/seamile/jsonfmt/actions)
+[![PyPI Version](https://img.shields.io/pypi/v/jsonfmt?color=blue&label=Version&logo=python&logoColor=white)](https://pypi.org/project/jsonfmt/)
+[![Installs](https://static.pepy.tech/personalized-badge/jsonfmt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Installs)](https://pepy.tech/project/jsonfmt)
+[![Code Grade](https://app.codacy.com/project/badge/Grade/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![Test Coverage](https://app.codacy.com/project/badge/Coverage/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 
 **jsonfmt** is a CLI tool for pretty printing or compressing JSON objects.
 
 It has the following features:
 
-1. Print the JSON object with **hightlight** and **pretty format** from files or stdin.
-2. Minimize the JSON object to a single line.
-3. Output part of a large JSON object via jsonpath.
+- [Print JSON with **hightlight** and **pretty format** from files or stdin.](#1-pretty-print-json-object)
+- [Minimize JSON to a single line.](#2-minimize-the-json-object)
+- [Output part of a large JSON via jsonpath.](#3-use-jsonpath-to-match-part-of-the-object)
+- [Format JSON to TOML or YAML](#4-format-json-to-toml-or-yaml)
+- [Convert between other formats](#5-convert-between-json-toml-and-yaml-formats)
+
 
 ## Install
 
 ```shell
 $ pip install jsonfmt
 ```
 
+
 ## Usage
 
 ```shell
-$ jsonfmt [-h] [-c] [-O] [-p JSONPATH] [json_files ...]
+$ jsonfmt [Options] [Files ...]
 ```
 
-- positional arguments:
-
-    - `json_files`   the json files that will be processed
+- Positional arguments:
 
-- options:
+    - `files`: the files that will be processed
 
-    - `-h, --help`: show this help message and exit.
-    - `-c`: compression the JSON object in the files or stdin.
-    - `-e`: escape non-ASCII characters.
-    - `-i INDENT`: number of spaces to use for indentation. (default: 4)
-    - `-O`: overwrite to the json file.
-    - `-p JSONPATH`: output part of JSON object via jsonpath.
-    - `-v`: show the version.
+- Options:
+  - `-h, --help`: show this help message and exit
+  - `-c`: compact the json object to a single line
+  - `-e`: escape non-ASCII characters
+  - `-f {json,toml,yaml}`: the format to output (default: json)
+  - `-i INDENT`: number of spaces to use for indentation (default: 2)
+  - `-O`: overwrite the formated text to original file
+  - `-p JSONPATH`: output part of the object via jsonpath
+  - `-v`: show the version
 
 
 ## Example
 
-In the file example.json there is a compressed JSON object.
+There are some test data in folder `test`:
+```
+test/
+|- example.json
+|- example.toml
+|- example.yaml
+```
+
+### 1. Pretty print JSON object.
 
-1. Pretty print from json file.
+- read from file
 
     ```shell
-    $ jsonfmt example.json
+    $ jsonfmt test/example.json
     ```
 
     Output:
     ```json
     {
-        "age": 23,
-        "gender": "纯爷们",
-        "history": [
-            {
-                "action": "eat",
-                "date": "2021-03-02",
-                "items": [
-                    {
-                        "calorie": 294.9,
-                        "name": "hamburger"
-                    },
-                    {
-                        "calorie": 266,
-                        "name": "pizza"
-                    }
-                ]
-            },
+        "actions": [
             {
-                "action": "drink",
-                "date": "2022-11-01",
-                "items": [
-                    {
-                        "calorie": 37.5,
-                        "name": "Coca Cola"
-                    },
-                    {
-                        "calorie": 54.5,
-                        "name": "juice"
-                    }
-                ]
+            "calorie": 294.9,
+            "date": "2021-03-02",
+            "name": "eat"
             },
             {
-                "action": "sport",
-                "date": "2023-04-27",
-                "items": [
-                    {
-                        "calorie": -375,
-                        "name": "running"
-                    },
-                    {
-                        "calorie": -350,
-                        "name": "swimming"
-                    }
-                ]
+            "calorie": -375,
+            "date": "2023-04-27",
+            "name": "sport"
             }
         ],
+        "age": 23,
+        "gender": "纯爷们",
+        "money": 3.1415926,
         "name": "Bob"
     }
     ```
 
-2. Format a JSON object from stdin via pipeline.
+- read from stdin
 
     ```shell
-    $ curl https://raw.githubusercontent.com/seamile/jsonfmt/main/example.json | jsonfmt
+    $ cat test/example.json | jsonfmt
     ```
 
     Output: Ditto.
 
+### 2. Minimize the JSON object.
+
+```shell
+$ echo '{ "name": "alex", "age": 21, "items": ["pen", "phone"] }' | jsonfmt -c
+```
+
+Output:
+```json
+{"age":21,"items":["pen","phone"],"name":"alex"}
+```
+
+### 3. Use jsonpath to match part of the object.
+
+**jsonfmt** uses a simplified jsonpath syntax.
+
+- It matches JSON objects starting from the root node.
+
+- You can use keys to match dictionaries and indexes to match lists, and use `/` to separate different levels.
+
+    ```shell
+    $ jsonfmt -p 'actions/0' test/example.json
+    ```
+
+    Output:
+    ```json
+    {
+        "calorie": 294.9,
+        "date": "2021-03-02",
+        "name": "eat"
+    }
+    ```
 
-3. Minimize the JSON object.
+- If you want to match all items in a list, just use `*` to match.
 
     ```shell
-    $ echo '{
-        "name": "alex",
-        "age": 21,
-        "items": ["pen", "ruler", "phone"]
-    }' | jsonfmt -c
+    $ jsonfmt -p 'actions/*/name' test/example.json
     ```
 
     Output:
     ```json
-    {"age":21,"items":["pen","ruler","phone"],"name":"alex"}
+    [
+        "eat",
+        "sport"
+    ]
     ```
 
-4. Use jsonpath to match part of a JSON object.
+### 4. Format JSON to TOML or YAML.
 
-    **jsonfmt** uses a simplified jsonpath syntax.
+```shell
+$ jsonfmt -f toml test/example.json
+```
 
-    - It matches JSON objects starting from the root node.
-    - You can use keys to match dictionaries and indexes to match lists, and use `/` to separate different levels.
-
-        ```shell
-        $ jsonfmt -p 'history/0/date' example.json
-        ```
-
-        Output:
-        ```json
-        "2021-03-02"
-        ```
-
-    - If you want to match all items in a list, just use `*` to match.
-
-        ```shell
-        $ jsonfmt -p 'history/*/items/*/name' example.json
-        ```
-
-        Output:
-        ```json
-        [
-            [
-                "hamburger",
-                "pizza"
-            ],
-            [
-                "Coca Cola",
-                "juice"
-            ],
-            [
-                "running",
-                "swimming"
-            ]
-        ]
-        ```
+Output:
+```toml
+age = 23
+gender = "纯爷们"
+money = 3.1415926
+name = "Bob"
+[[actions]]
+calorie = 294.9
+date = "2021-03-02"
+name = "eat"
+
+[[actions]]
+calorie = -375
+date = "2023-04-27"
+name = "sport"
+```
 
-4. You can use the `-O` parameter to overwrite the file with the result.
+### 5. Convert between JSON, TOML and YAML formats.
 
-    ```shell
-    $ jsonfmt -O example.json
-    ```
+```shell
+# json to yaml
+$ jsonfmt -f yaml test/example.json
 
-5. To output the result to a new file, you can use the redirect symbol `>`.
+# yaml to toml
+$ jsonfmt -f toml test/example.yaml
 
-    ```shell
-    $ jsonfmt example.json > formatted.json
-    ```
+# toml to json
+$ jsonfmt -f json test/example.toml
+```
+
+### 6. Other usages
+
+- use the `-O` parameter to overwrite the file with the result.
+
+```shell
+$ jsonfmt -O test/example.json
+```
+
+- write the result to a new file (use symbol `>`).
+
+```shell
+$ jsonfmt test/example.json > formatted.json
+```
```

### Comparing `jsonfmt-0.1.4/README.md` & `jsonfmt-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,180 +1,190 @@
 # JSON Formator
 
-![GitHub Build Status](https://img.shields.io/github/actions/workflow/status/seamile/jsonfmt/python-package.yml?label=Build&logo=python&logoColor=white)
-[![Downloads](https://static.pepy.tech/personalized-badge/jsonfmt?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Installs)](https://pepy.tech/project/jsonfmt)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
-[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
+[![Build Status](https://github.com/seamile/jsonfmt/actions/workflows/python-package.yml/badge.svg)](https://github.com/seamile/jsonfmt/actions)
+[![PyPI Version](https://img.shields.io/pypi/v/jsonfmt?color=blue&label=Version&logo=python&logoColor=white)](https://pypi.org/project/jsonfmt/)
+[![Installs](https://static.pepy.tech/personalized-badge/jsonfmt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Installs)](https://pepy.tech/project/jsonfmt)
+[![Code Grade](https://app.codacy.com/project/badge/Grade/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![Test Coverage](https://app.codacy.com/project/badge/Coverage/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 
 **jsonfmt** is a CLI tool for pretty printing or compressing JSON objects.
 
 It has the following features:
 
-1. Print the JSON object with **hightlight** and **pretty format** from files or stdin.
-2. Minimize the JSON object to a single line.
-3. Output part of a large JSON object via jsonpath.
+- [Print JSON with **hightlight** and **pretty format** from files or stdin.](#1-pretty-print-json-object)
+- [Minimize JSON to a single line.](#2-minimize-the-json-object)
+- [Output part of a large JSON via jsonpath.](#3-use-jsonpath-to-match-part-of-the-object)
+- [Format JSON to TOML or YAML](#4-format-json-to-toml-or-yaml)
+- [Convert between other formats](#5-convert-between-json-toml-and-yaml-formats)
+
 
 ## Install
 
 ```shell
 $ pip install jsonfmt
 ```
 
+
 ## Usage
 
 ```shell
-$ jsonfmt [-h] [-c] [-O] [-p JSONPATH] [json_files ...]
+$ jsonfmt [Options] [Files ...]
 ```
 
-- positional arguments:
-
-    - `json_files`   the json files that will be processed
+- Positional arguments:
 
-- options:
+    - `files`: the files that will be processed
 
-    - `-h, --help`: show this help message and exit.
-    - `-c`: compression the JSON object in the files or stdin.
-    - `-e`: escape non-ASCII characters.
-    - `-i INDENT`: number of spaces to use for indentation. (default: 4)
-    - `-O`: overwrite to the json file.
-    - `-p JSONPATH`: output part of JSON object via jsonpath.
-    - `-v`: show the version.
+- Options:
+  - `-h, --help`: show this help message and exit
+  - `-c`: compact the json object to a single line
+  - `-e`: escape non-ASCII characters
+  - `-f {json,toml,yaml}`: the format to output (default: json)
+  - `-i INDENT`: number of spaces to use for indentation (default: 2)
+  - `-O`: overwrite the formated text to original file
+  - `-p JSONPATH`: output part of the object via jsonpath
+  - `-v`: show the version
 
 
 ## Example
 
-In the file example.json there is a compressed JSON object.
+There are some test data in folder `test`:
+```
+test/
+|- example.json
+|- example.toml
+|- example.yaml
+```
+
+### 1. Pretty print JSON object.
 
-1. Pretty print from json file.
+- read from file
 
     ```shell
-    $ jsonfmt example.json
+    $ jsonfmt test/example.json
     ```
 
     Output:
     ```json
     {
-        "age": 23,
-        "gender": "纯爷们",
-        "history": [
-            {
-                "action": "eat",
-                "date": "2021-03-02",
-                "items": [
-                    {
-                        "calorie": 294.9,
-                        "name": "hamburger"
-                    },
-                    {
-                        "calorie": 266,
-                        "name": "pizza"
-                    }
-                ]
-            },
+        "actions": [
             {
-                "action": "drink",
-                "date": "2022-11-01",
-                "items": [
-                    {
-                        "calorie": 37.5,
-                        "name": "Coca Cola"
-                    },
-                    {
-                        "calorie": 54.5,
-                        "name": "juice"
-                    }
-                ]
+            "calorie": 294.9,
+            "date": "2021-03-02",
+            "name": "eat"
             },
             {
-                "action": "sport",
-                "date": "2023-04-27",
-                "items": [
-                    {
-                        "calorie": -375,
-                        "name": "running"
-                    },
-                    {
-                        "calorie": -350,
-                        "name": "swimming"
-                    }
-                ]
+            "calorie": -375,
+            "date": "2023-04-27",
+            "name": "sport"
             }
         ],
+        "age": 23,
+        "gender": "纯爷们",
+        "money": 3.1415926,
         "name": "Bob"
     }
     ```
 
-2. Format a JSON object from stdin via pipeline.
+- read from stdin
 
     ```shell
-    $ curl https://raw.githubusercontent.com/seamile/jsonfmt/main/example.json | jsonfmt
+    $ cat test/example.json | jsonfmt
     ```
 
     Output: Ditto.
 
+### 2. Minimize the JSON object.
+
+```shell
+$ echo '{ "name": "alex", "age": 21, "items": ["pen", "phone"] }' | jsonfmt -c
+```
+
+Output:
+```json
+{"age":21,"items":["pen","phone"],"name":"alex"}
+```
+
+### 3. Use jsonpath to match part of the object.
+
+**jsonfmt** uses a simplified jsonpath syntax.
+
+- It matches JSON objects starting from the root node.
+
+- You can use keys to match dictionaries and indexes to match lists, and use `/` to separate different levels.
+
+    ```shell
+    $ jsonfmt -p 'actions/0' test/example.json
+    ```
+
+    Output:
+    ```json
+    {
+        "calorie": 294.9,
+        "date": "2021-03-02",
+        "name": "eat"
+    }
+    ```
 
-3. Minimize the JSON object.
+- If you want to match all items in a list, just use `*` to match.
 
     ```shell
-    $ echo '{
-        "name": "alex",
-        "age": 21,
-        "items": ["pen", "ruler", "phone"]
-    }' | jsonfmt -c
+    $ jsonfmt -p 'actions/*/name' test/example.json
     ```
 
     Output:
     ```json
-    {"age":21,"items":["pen","ruler","phone"],"name":"alex"}
+    [
+        "eat",
+        "sport"
+    ]
     ```
 
-4. Use jsonpath to match part of a JSON object.
+### 4. Format JSON to TOML or YAML.
 
-    **jsonfmt** uses a simplified jsonpath syntax.
+```shell
+$ jsonfmt -f toml test/example.json
+```
 
-    - It matches JSON objects starting from the root node.
-    - You can use keys to match dictionaries and indexes to match lists, and use `/` to separate different levels.
-
-        ```shell
-        $ jsonfmt -p 'history/0/date' example.json
-        ```
-
-        Output:
-        ```json
-        "2021-03-02"
-        ```
-
-    - If you want to match all items in a list, just use `*` to match.
-
-        ```shell
-        $ jsonfmt -p 'history/*/items/*/name' example.json
-        ```
-
-        Output:
-        ```json
-        [
-            [
-                "hamburger",
-                "pizza"
-            ],
-            [
-                "Coca Cola",
-                "juice"
-            ],
-            [
-                "running",
-                "swimming"
-            ]
-        ]
-        ```
+Output:
+```toml
+age = 23
+gender = "纯爷们"
+money = 3.1415926
+name = "Bob"
+[[actions]]
+calorie = 294.9
+date = "2021-03-02"
+name = "eat"
+
+[[actions]]
+calorie = -375
+date = "2023-04-27"
+name = "sport"
+```
 
-4. You can use the `-O` parameter to overwrite the file with the result.
+### 5. Convert between JSON, TOML and YAML formats.
 
-    ```shell
-    $ jsonfmt -O example.json
-    ```
+```shell
+# json to yaml
+$ jsonfmt -f yaml test/example.json
 
-5. To output the result to a new file, you can use the redirect symbol `>`.
+# yaml to toml
+$ jsonfmt -f toml test/example.yaml
 
-    ```shell
-    $ jsonfmt example.json > formatted.json
-    ```
+# toml to json
+$ jsonfmt -f json test/example.toml
+```
+
+### 6. Other usages
+
+- use the `-O` parameter to overwrite the file with the result.
+
+```shell
+$ jsonfmt -O test/example.json
+```
+
+- write the result to a new file (use symbol `>`).
+
+```shell
+$ jsonfmt test/example.json > formatted.json
+```
```

### Comparing `jsonfmt-0.1.4/jsonfmt.egg-info/PKG-INFO` & `jsonfmt-0.2.0/jsonfmt.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,196 +1,218 @@
 Metadata-Version: 2.1
 Name: jsonfmt
-Version: 0.1.4
+Version: 0.2.0
 Summary: A simple tool for formatting JSON object.
 Author-email: Seamile <lanhuermao@gmail.com>
-License: MIT
+License: MIT License
+Project-URL: homepage, https://github.com/seamile/jsonfmt
+Project-URL: repository, https://github.com/seamile/jsonfmt
+Project-URL: documentation, https://seamile.github.io/jsonfmt/
+Keywords: json,formatter,pretty-print,highlight,jsonpath
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: File Formats :: JSON
+Classifier: Topic :: Printing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JSON Formator
 
-![GitHub Build Status](https://img.shields.io/github/actions/workflow/status/seamile/jsonfmt/python-package.yml?label=Build&logo=python&logoColor=white)
-[![Downloads](https://static.pepy.tech/personalized-badge/jsonfmt?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Installs)](https://pepy.tech/project/jsonfmt)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
-[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
+[![Build Status](https://github.com/seamile/jsonfmt/actions/workflows/python-package.yml/badge.svg)](https://github.com/seamile/jsonfmt/actions)
+[![PyPI Version](https://img.shields.io/pypi/v/jsonfmt?color=blue&label=Version&logo=python&logoColor=white)](https://pypi.org/project/jsonfmt/)
+[![Installs](https://static.pepy.tech/personalized-badge/jsonfmt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Installs)](https://pepy.tech/project/jsonfmt)
+[![Code Grade](https://app.codacy.com/project/badge/Grade/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![Test Coverage](https://app.codacy.com/project/badge/Coverage/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 
 **jsonfmt** is a CLI tool for pretty printing or compressing JSON objects.
 
 It has the following features:
 
-1. Print the JSON object with **hightlight** and **pretty format** from files or stdin.
-2. Minimize the JSON object to a single line.
-3. Output part of a large JSON object via jsonpath.
+- [Print JSON with **hightlight** and **pretty format** from files or stdin.](#1-pretty-print-json-object)
+- [Minimize JSON to a single line.](#2-minimize-the-json-object)
+- [Output part of a large JSON via jsonpath.](#3-use-jsonpath-to-match-part-of-the-object)
+- [Format JSON to TOML or YAML](#4-format-json-to-toml-or-yaml)
+- [Convert between other formats](#5-convert-between-json-toml-and-yaml-formats)
+
 
 ## Install
 
 ```shell
 $ pip install jsonfmt
 ```
 
+
 ## Usage
 
 ```shell
-$ jsonfmt [-h] [-c] [-O] [-p JSONPATH] [json_files ...]
+$ jsonfmt [Options] [Files ...]
 ```
 
-- positional arguments:
-
-    - `json_files`   the json files that will be processed
+- Positional arguments:
 
-- options:
+    - `files`: the files that will be processed
 
-    - `-h, --help`: show this help message and exit.
-    - `-c`: compression the JSON object in the files or stdin.
-    - `-e`: escape non-ASCII characters.
-    - `-i INDENT`: number of spaces to use for indentation. (default: 4)
-    - `-O`: overwrite to the json file.
-    - `-p JSONPATH`: output part of JSON object via jsonpath.
-    - `-v`: show the version.
+- Options:
+  - `-h, --help`: show this help message and exit
+  - `-c`: compact the json object to a single line
+  - `-e`: escape non-ASCII characters
+  - `-f {json,toml,yaml}`: the format to output (default: json)
+  - `-i INDENT`: number of spaces to use for indentation (default: 2)
+  - `-O`: overwrite the formated text to original file
+  - `-p JSONPATH`: output part of the object via jsonpath
+  - `-v`: show the version
 
 
 ## Example
 
-In the file example.json there is a compressed JSON object.
+There are some test data in folder `test`:
+```
+test/
+|- example.json
+|- example.toml
+|- example.yaml
+```
+
+### 1. Pretty print JSON object.
 
-1. Pretty print from json file.
+- read from file
 
     ```shell
-    $ jsonfmt example.json
+    $ jsonfmt test/example.json
     ```
 
     Output:
     ```json
     {
-        "age": 23,
-        "gender": "纯爷们",
-        "history": [
-            {
-                "action": "eat",
-                "date": "2021-03-02",
-                "items": [
-                    {
-                        "calorie": 294.9,
-                        "name": "hamburger"
-                    },
-                    {
-                        "calorie": 266,
-                        "name": "pizza"
-                    }
-                ]
-            },
+        "actions": [
             {
-                "action": "drink",
-                "date": "2022-11-01",
-                "items": [
-                    {
-                        "calorie": 37.5,
-                        "name": "Coca Cola"
-                    },
-                    {
-                        "calorie": 54.5,
-                        "name": "juice"
-                    }
-                ]
+            "calorie": 294.9,
+            "date": "2021-03-02",
+            "name": "eat"
             },
             {
-                "action": "sport",
-                "date": "2023-04-27",
-                "items": [
-                    {
-                        "calorie": -375,
-                        "name": "running"
-                    },
-                    {
-                        "calorie": -350,
-                        "name": "swimming"
-                    }
-                ]
+            "calorie": -375,
+            "date": "2023-04-27",
+            "name": "sport"
             }
         ],
+        "age": 23,
+        "gender": "纯爷们",
+        "money": 3.1415926,
         "name": "Bob"
     }
     ```
 
-2. Format a JSON object from stdin via pipeline.
+- read from stdin
 
     ```shell
-    $ curl https://raw.githubusercontent.com/seamile/jsonfmt/main/example.json | jsonfmt
+    $ cat test/example.json | jsonfmt
     ```
 
     Output: Ditto.
 
+### 2. Minimize the JSON object.
+
+```shell
+$ echo '{ "name": "alex", "age": 21, "items": ["pen", "phone"] }' | jsonfmt -c
+```
+
+Output:
+```json
+{"age":21,"items":["pen","phone"],"name":"alex"}
+```
+
+### 3. Use jsonpath to match part of the object.
+
+**jsonfmt** uses a simplified jsonpath syntax.
+
+- It matches JSON objects starting from the root node.
+
+- You can use keys to match dictionaries and indexes to match lists, and use `/` to separate different levels.
+
+    ```shell
+    $ jsonfmt -p 'actions/0' test/example.json
+    ```
+
+    Output:
+    ```json
+    {
+        "calorie": 294.9,
+        "date": "2021-03-02",
+        "name": "eat"
+    }
+    ```
 
-3. Minimize the JSON object.
+- If you want to match all items in a list, just use `*` to match.
 
     ```shell
-    $ echo '{
-        "name": "alex",
-        "age": 21,
-        "items": ["pen", "ruler", "phone"]
-    }' | jsonfmt -c
+    $ jsonfmt -p 'actions/*/name' test/example.json
     ```
 
     Output:
     ```json
-    {"age":21,"items":["pen","ruler","phone"],"name":"alex"}
+    [
+        "eat",
+        "sport"
+    ]
     ```
 
-4. Use jsonpath to match part of a JSON object.
+### 4. Format JSON to TOML or YAML.
 
-    **jsonfmt** uses a simplified jsonpath syntax.
+```shell
+$ jsonfmt -f toml test/example.json
+```
 
-    - It matches JSON objects starting from the root node.
-    - You can use keys to match dictionaries and indexes to match lists, and use `/` to separate different levels.
-
-        ```shell
-        $ jsonfmt -p 'history/0/date' example.json
-        ```
-
-        Output:
-        ```json
-        "2021-03-02"
-        ```
-
-    - If you want to match all items in a list, just use `*` to match.
-
-        ```shell
-        $ jsonfmt -p 'history/*/items/*/name' example.json
-        ```
-
-        Output:
-        ```json
-        [
-            [
-                "hamburger",
-                "pizza"
-            ],
-            [
-                "Coca Cola",
-                "juice"
-            ],
-            [
-                "running",
-                "swimming"
-            ]
-        ]
-        ```
+Output:
+```toml
+age = 23
+gender = "纯爷们"
+money = 3.1415926
+name = "Bob"
+[[actions]]
+calorie = 294.9
+date = "2021-03-02"
+name = "eat"
+
+[[actions]]
+calorie = -375
+date = "2023-04-27"
+name = "sport"
+```
 
-4. You can use the `-O` parameter to overwrite the file with the result.
+### 5. Convert between JSON, TOML and YAML formats.
 
-    ```shell
-    $ jsonfmt -O example.json
-    ```
+```shell
+# json to yaml
+$ jsonfmt -f yaml test/example.json
 
-5. To output the result to a new file, you can use the redirect symbol `>`.
+# yaml to toml
+$ jsonfmt -f toml test/example.yaml
 
-    ```shell
-    $ jsonfmt example.json > formatted.json
-    ```
+# toml to json
+$ jsonfmt -f json test/example.toml
+```
+
+### 6. Other usages
+
+- use the `-O` parameter to overwrite the file with the result.
+
+```shell
+$ jsonfmt -O test/example.json
+```
+
+- write the result to a new file (use symbol `>`).
+
+```shell
+$ jsonfmt test/example.json > formatted.json
+```
```

### Comparing `jsonfmt-0.1.4/jsonfmt.py` & `jsonfmt-0.2.0/jsonfmt.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,88 @@
 #!/usr/bin/env python
 '''JSON Format Tool'''
 
 import json
-from sys import stdin, stdout, stderr
+import toml
+import yaml
 from argparse import ArgumentParser
-from typing import Any, List, IO, Optional, Sequence, Union
-
+from functools import partial
 from pygments import highlight
-from pygments.lexers import JsonLexer
 from pygments.formatters import TerminalFormatter
+from pygments.lexers import JsonLexer, TOMLLexer, YamlLexer
+from sys import stdin, stdout, stderr, exit
+from typing import Any, List, IO, Optional, Sequence, Union
 
-__version__ = '0.1.4'
+__version__ = '0.2.0'
 
 
 def print_err(msg: str):
     print(f'\033[1;91mjsonfmt:\033[0m \033[0;91m{msg}\033[0m', file=stderr)
 
 
 class JSONPathError(Exception):
     pass
 
 
-class JSONParseError(Exception):
+class ParseError(Exception):
     pass
 
 
 def parse_jsonpath(jsonpath: str) -> List[Union[str, int]]:
     '''parse the jsonpath into a list of pathname components'''
-    jsonpath = jsonpath.strip().strip('/')
-    if not jsonpath:
-        return []
-    else:
+    if jsonpath := jsonpath.strip().strip('/'):
         components = jsonpath.split('/')
-        for i, c in enumerate(components):
-            if c.isdecimal():
-                components[i] = int(c)  # type: ignore
+        for i, component in enumerate(components):
+            if component.isdecimal():
+                components[i] = int(component)  # type: ignore
         return components  # type: ignore
+    else:
+        return []
 
 
 def match_element(py_obj: Any, jpath_components: List[Union[str, int]]) -> Any:
-    for i, c in enumerate(jpath_components):
-        if c == '*' and isinstance(py_obj, list):
+    for i, component in enumerate(jpath_components):
+        if component == '*' and isinstance(py_obj, list):
             return [match_element(sub_obj, jpath_components[i + 1:])
                     for sub_obj in py_obj]
         else:
             try:
-                py_obj = py_obj[c]
-            except (IndexError, KeyError, TypeError):
-                raise JSONPathError(f'invalid path node `{c}`')
+                py_obj = py_obj[component]
+            except (IndexError, KeyError, TypeError) as err:
+                raise JSONPathError(f'invalid path node `{component}`') from err
 
     return py_obj
 
 
-def read_json_to_py(json_fp: IO, jsonpath: str) -> Any:
-    '''read json obj from IO and match sub-element by jsonpath'''
-    # parse json object to python object
-    try:
-        py_obj = json.load(json_fp)
-    except (json.JSONDecodeError, UnicodeDecodeError) as e:
-        print_err(f"no json object in `{json_fp.name}`")
-        raise JSONParseError from e
+def parse_to_pyobj(input_fp: IO, jsonpath: str) -> Any:
+    '''read json, toml or yaml from IO and then match sub-element by jsonpath'''
+    # parse json, toml or yaml to python object
+    obj_text = input_fp.read()
+    yaml_load = partial(yaml.load, Loader=yaml.Loader)
+    for fn_loads in [json.loads, toml.loads, yaml_load]:
+        try:
+            py_obj = fn_loads(obj_text)
+            break
+        except Exception:
+            continue
+    else:
+        print_err(f"no json, toml or yaml object in `{input_fp.name}`")
+        raise ParseError
 
     # parse jsonpath and match the sub-element of py_obj
     jpath_components = parse_jsonpath(jsonpath)
     try:
         return match_element(py_obj, jpath_components)
-    except JSONPathError as e:
-        print_err(f'{e}')
-        raise JSONParseError from e
+    except JSONPathError as err:
+        print_err(f'{err}')
+        raise ParseError from err
 
 
-def output(py_obj: Any, compact: bool, escape: bool, indent: int,
-           output_fp: IO = stdout):
+def output_json(py_obj: Any, output_fp: IO, compact: bool,
+                escape: bool, indent: int):
     '''output formated json to file or stdout'''
     if output_fp.fileno() > 2:
         output_fp.seek(0)
         output_fp.truncate()
 
     if compact:
         json_text = json.dumps(py_obj, ensure_ascii=escape, sort_keys=True,
@@ -91,56 +98,101 @@
     # append a blank line at the end of `fp``
     if json_text[-1] != '\n':
         json_text += '\n'
 
     output_fp.write(json_text)
 
 
+def output_toml(py_obj: Any, output_fp: IO):
+    '''output formated toml to file or stdout'''
+    if not isinstance(py_obj, dict):
+        print_err('the pyobj must be a Mapping when format to toml')
+        exit(3)
+
+    if output_fp.fileno() > 2:
+        output_fp.seek(0)
+        output_fp.truncate()
+
+    # highlight the toml code when output to TTY divice
+    if output_fp.isatty():
+        toml_text = toml.dumps(py_obj)
+        highlight_toml = highlight(toml_text, TOMLLexer(), TerminalFormatter())
+        output_fp.write(highlight_toml)
+    else:
+        toml.dump(py_obj, output_fp)
+
+
+def output_yaml(py_obj: Any, output_fp: IO, escape: bool, indent: int):
+    '''output formated yaml to file or stdout'''
+    if output_fp.fileno() > 2:
+        output_fp.seek(0)
+        output_fp.truncate()
+
+    # highlight the yaml code when output to TTY divice
+    if output_fp.isatty():
+        yaml_text = yaml.safe_dump(py_obj, allow_unicode=not escape,
+                                   indent=indent, sort_keys=True)
+        highlight_yaml = highlight(yaml_text, YamlLexer(), TerminalFormatter())
+        output_fp.write(highlight_yaml)
+    else:
+        yaml.safe_dump(py_obj, output_fp, allow_unicode=not escape,
+                       indent=indent, sort_keys=True)
+
+
 def parse_cmdline_args(args: Optional[Sequence[str]] = None):
     parser = ArgumentParser('jsonfmt')
-    parser.add_argument('-c', dest='compression', action='store_true',
-                        help='compression the json object in the files or stdin')
+    parser.add_argument('-c', dest='compact', action='store_true',
+                        help='compact the json object to a single line')
     parser.add_argument('-e', dest='escape', action='store_true',
                         help='escape non-ASCII characters')
-    parser.add_argument('-i', dest='indent', type=int, default=4,
+    parser.add_argument('-f', dest='format', choices=['json', 'toml', 'yaml'],
+                        default='json', help='the format to output (default: %(default)s)')
+    parser.add_argument('-i', dest='indent', type=int, default=2,
                         help='number of spaces to use for indentation (default: %(default)s)')
     parser.add_argument('-O', dest='overwrite', action='store_true',
-                        help='overwrite the formated json object into the json file')
+                        help='overwrite the formated text to original file')
     parser.add_argument('-p', dest='jsonpath', type=str, default='',
-                        help='output part of json object via jsonpath')
-    parser.add_argument(dest='json_files', nargs='*',
-                        help='the json files that will be processed')
-    parser.add_argument('-v', dest='version', action='version', version=__version__,
-                        help="show the version")
+                        help='output part of the object via jsonpath')
+    parser.add_argument(dest='files', nargs='*',
+                        help='the files that will be processed')
+    parser.add_argument('-v', dest='version', action='version',
+                        version=__version__, help="show the version")
     return parser.parse_args(args)
 
 
 def main():
     args = parse_cmdline_args()
 
-    if args.json_files:
-        for j_file in args.json_files:
+    # match the specified output function
+    fn_output = {
+        'json': partial(output_json, compact=args.compact,
+                        escape=args.escape, indent=args.indent),
+        'yaml': partial(output_yaml, escape=args.escape, indent=args.indent),
+        'toml': output_toml,
+    }[args.format]
+
+    if args.files:
+        for file in args.files:
             try:
-                # read json from file
-                with open(j_file, 'r+') as json_fp:
+                # read from file
+                with open(file, 'r+') as input_fp:
                     try:
-                        py_obj = read_json_to_py(json_fp, args.jsonpath)
-                    except JSONParseError:
+                        py_obj = parse_to_pyobj(input_fp, args.jsonpath)
+                    except ParseError:
                         exit(1)
                     else:
-                        output_fp = json_fp if args.overwrite else stdout
-                        output(py_obj, args.compression, args.escape,
-                               args.indent, output_fp)
+                        output_fp = input_fp if args.overwrite else stdout
+                        fn_output(py_obj, output_fp)
             except FileNotFoundError:
-                print_err(f'no such file `{j_file}`')
+                print_err(f'no such file `{file}`')
     else:
-        # read json from stdin
+        # read from stdin
         try:
-            py_obj = read_json_to_py(stdin, args.jsonpath)
-        except JSONParseError:
-            exit(1)
+            py_obj = parse_to_pyobj(stdin, args.jsonpath)
+        except ParseError:
+            exit(2)
         else:
-            output(py_obj, args.compression, args.escape, args.indent, stdout)
+            fn_output(py_obj, stdout)
 
 
 if __name__ == "__main__":
     main()
```

