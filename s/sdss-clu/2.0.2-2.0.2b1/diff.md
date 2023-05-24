# Comparing `tmp/sdss_clu-2.0.2.tar.gz` & `tmp/sdss_clu-2.0.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_clu-2.0.2.tar", max compression
+gzip compressed data, was "sdss_clu-2.0.2b1.tar", max compression
```

## Comparing `sdss_clu-2.0.2.tar` & `sdss_clu-2.0.2b1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1504 2023-05-24 07:44:31.223858 sdss_clu-2.0.2/LICENSE.md
--rw-r--r--   0        0        0     5049 2023-05-24 07:44:31.224176 sdss_clu-2.0.2/README.rst
--rw-r--r--   0        0        0     2642 2023-05-24 07:44:31.235792 sdss_clu-2.0.2/pyproject.toml
--rw-r--r--   0        0        0      889 2023-05-24 07:44:31.236187 sdss_clu-2.0.2/python/clu/__init__.py
--rwxr-xr-x   0        0        0     7376 2023-05-24 07:44:31.236490 sdss_clu-2.0.2/python/clu/__main__.py
--rw-r--r--   0        0        0    13555 2023-05-24 07:44:31.236749 sdss_clu-2.0.2/python/clu/actor.py
--rw-r--r--   0        0        0    19832 2023-05-24 07:44:31.237054 sdss_clu-2.0.2/python/clu/base.py
--rw-r--r--   0        0        0    14596 2023-05-24 07:44:31.237344 sdss_clu-2.0.2/python/clu/client.py
--rw-r--r--   0        0        0    20069 2023-05-24 07:44:31.237629 sdss_clu-2.0.2/python/clu/command.py
--rw-r--r--   0        0        0     4135 2023-05-24 07:44:31.237880 sdss_clu-2.0.2/python/clu/device.py
--rw-r--r--   0        0        0     1347 2023-05-24 07:44:31.238087 sdss_clu-2.0.2/python/clu/exceptions.py
--rw-r--r--   0        0        0       41 2023-05-24 07:44:31.238364 sdss_clu-2.0.2/python/clu/legacy/__init__.py
--rw-r--r--   0        0        0    17892 2023-05-24 07:44:31.238696 sdss_clu-2.0.2/python/clu/legacy/actor.py
--rw-r--r--   0        0        0    13538 2023-05-24 07:44:31.238998 sdss_clu-2.0.2/python/clu/legacy/tron.py
--rw-r--r--   0        0        0        0 2023-05-24 07:44:31.239212 sdss_clu-2.0.2/python/clu/legacy/types/__init__.py
--rw-r--r--   0        0        0    15014 2023-05-24 07:44:31.239453 sdss_clu-2.0.2/python/clu/legacy/types/html.py
--rw-r--r--   0        0        0    17888 2023-05-24 07:44:31.239737 sdss_clu-2.0.2/python/clu/legacy/types/keys.py
--rw-r--r--   0        0        0    17508 2023-05-24 07:44:31.240038 sdss_clu-2.0.2/python/clu/legacy/types/messages.py
--rw-r--r--   0        0        0     9489 2023-05-24 07:44:31.240313 sdss_clu-2.0.2/python/clu/legacy/types/parser.py
--rwxr-xr-x   0        0        0      104 2023-05-24 07:44:31.240615 sdss_clu-2.0.2/python/clu/legacy/types/ply/__init__.py
--rwxr-xr-x   0        0        0    38405 2023-05-24 07:44:31.241019 sdss_clu-2.0.2/python/clu/legacy/types/ply/cpp.py
--rwxr-xr-x   0        0        0     2877 2023-05-24 07:44:31.241404 sdss_clu-2.0.2/python/clu/legacy/types/ply/ctokens.py
--rwxr-xr-x   0        0        0    45219 2023-05-24 07:44:31.242267 sdss_clu-2.0.2/python/clu/legacy/types/ply/lex.py
--rwxr-xr-x   0        0        0   140885 2023-05-24 07:44:31.243049 sdss_clu-2.0.2/python/clu/legacy/types/ply/yacc.py
--rwxr-xr-x   0        0        0     2314 2023-05-24 07:44:31.243370 sdss_clu-2.0.2/python/clu/legacy/types/ply/ygen.py
--rw-r--r--   0        0        0     5487 2023-05-24 07:44:31.243649 sdss_clu-2.0.2/python/clu/legacy/types/pvt.py
--rw-r--r--   0        0        0    19685 2023-05-24 07:44:31.243962 sdss_clu-2.0.2/python/clu/legacy/types/types.py
--rw-r--r--   0        0        0    11758 2023-05-24 07:44:31.244262 sdss_clu-2.0.2/python/clu/model.py
--rw-r--r--   0        0        0      309 2023-05-24 07:44:31.244581 sdss_clu-2.0.2/python/clu/parsers/__init__.py
--rw-r--r--   0        0        0    20428 2023-05-24 07:44:31.244886 sdss_clu-2.0.2/python/clu/parsers/click.py
--rw-r--r--   0        0        0     2685 2023-05-24 07:44:31.245134 sdss_clu-2.0.2/python/clu/parsers/json.py
--rw-r--r--   0        0        0    19724 2023-05-24 07:44:31.245432 sdss_clu-2.0.2/python/clu/protocol.py
--rw-r--r--   0        0        0     2805 2023-05-24 07:44:31.245720 sdss_clu-2.0.2/python/clu/store.py
--rw-r--r--   0        0        0     7820 2023-05-24 07:44:31.245970 sdss_clu-2.0.2/python/clu/testing.py
--rw-r--r--   0        0        0    16901 2023-05-24 07:44:31.246257 sdss_clu-2.0.2/python/clu/tools.py
--rw-r--r--   0        0        0     6367 1970-01-01 00:00:00.000000 sdss_clu-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-05-23 18:42:10.362267 sdss_clu-2.0.2b1/LICENSE.md
+-rw-r--r--   0        0        0     5049 2023-05-23 18:42:10.362498 sdss_clu-2.0.2b1/README.rst
+-rw-r--r--   0        0        0     2644 2023-05-23 18:42:10.376156 sdss_clu-2.0.2b1/pyproject.toml
+-rw-r--r--   0        0        0      889 2023-05-23 18:42:10.376648 sdss_clu-2.0.2b1/python/clu/__init__.py
+-rwxr-xr-x   0        0        0     7260 2023-05-23 18:42:10.377014 sdss_clu-2.0.2b1/python/clu/__main__.py
+-rw-r--r--   0        0        0    13555 2023-05-23 18:42:10.377447 sdss_clu-2.0.2b1/python/clu/actor.py
+-rw-r--r--   0        0        0    19832 2023-05-23 18:42:10.377898 sdss_clu-2.0.2b1/python/clu/base.py
+-rw-r--r--   0        0        0    14596 2023-05-23 18:42:10.378353 sdss_clu-2.0.2b1/python/clu/client.py
+-rw-r--r--   0        0        0    20069 2023-05-23 18:42:10.378854 sdss_clu-2.0.2b1/python/clu/command.py
+-rw-r--r--   0        0        0     4135 2023-05-23 18:42:10.421280 sdss_clu-2.0.2b1/python/clu/device.py
+-rw-r--r--   0        0        0     1347 2023-05-23 18:42:10.502589 sdss_clu-2.0.2b1/python/clu/exceptions.py
+-rw-r--r--   0        0        0       41 2023-05-23 18:42:10.502970 sdss_clu-2.0.2b1/python/clu/legacy/__init__.py
+-rw-r--r--   0        0        0    17892 2023-05-23 18:42:10.503291 sdss_clu-2.0.2b1/python/clu/legacy/actor.py
+-rw-r--r--   0        0        0    13538 2023-05-23 18:42:10.503623 sdss_clu-2.0.2b1/python/clu/legacy/tron.py
+-rw-r--r--   0        0        0        0 2023-05-23 18:42:10.503839 sdss_clu-2.0.2b1/python/clu/legacy/types/__init__.py
+-rw-r--r--   0        0        0    15014 2023-05-23 18:42:10.504088 sdss_clu-2.0.2b1/python/clu/legacy/types/html.py
+-rw-r--r--   0        0        0    17888 2023-05-23 18:42:10.504395 sdss_clu-2.0.2b1/python/clu/legacy/types/keys.py
+-rw-r--r--   0        0        0    17508 2023-05-23 18:42:10.504711 sdss_clu-2.0.2b1/python/clu/legacy/types/messages.py
+-rw-r--r--   0        0        0     9489 2023-05-23 18:42:10.505080 sdss_clu-2.0.2b1/python/clu/legacy/types/parser.py
+-rwxr-xr-x   0        0        0      104 2023-05-23 18:42:10.505376 sdss_clu-2.0.2b1/python/clu/legacy/types/ply/__init__.py
+-rwxr-xr-x   0        0        0    38405 2023-05-23 18:42:10.505775 sdss_clu-2.0.2b1/python/clu/legacy/types/ply/cpp.py
+-rwxr-xr-x   0        0        0     2877 2023-05-23 18:42:10.506167 sdss_clu-2.0.2b1/python/clu/legacy/types/ply/ctokens.py
+-rwxr-xr-x   0        0        0    45219 2023-05-23 18:42:10.506647 sdss_clu-2.0.2b1/python/clu/legacy/types/ply/lex.py
+-rwxr-xr-x   0        0        0   140885 2023-05-23 18:42:10.507599 sdss_clu-2.0.2b1/python/clu/legacy/types/ply/yacc.py
+-rwxr-xr-x   0        0        0     2314 2023-05-23 18:42:10.508114 sdss_clu-2.0.2b1/python/clu/legacy/types/ply/ygen.py
+-rw-r--r--   0        0        0     5487 2023-05-23 18:42:10.508442 sdss_clu-2.0.2b1/python/clu/legacy/types/pvt.py
+-rw-r--r--   0        0        0    19685 2023-05-23 18:42:10.508900 sdss_clu-2.0.2b1/python/clu/legacy/types/types.py
+-rw-r--r--   0        0        0    11758 2023-05-23 18:42:10.509180 sdss_clu-2.0.2b1/python/clu/model.py
+-rw-r--r--   0        0        0      309 2023-05-23 18:42:10.509537 sdss_clu-2.0.2b1/python/clu/parsers/__init__.py
+-rw-r--r--   0        0        0    20428 2023-05-23 18:42:10.509825 sdss_clu-2.0.2b1/python/clu/parsers/click.py
+-rw-r--r--   0        0        0     2685 2023-05-23 18:42:10.510042 sdss_clu-2.0.2b1/python/clu/parsers/json.py
+-rw-r--r--   0        0        0    19724 2023-05-23 18:42:10.510306 sdss_clu-2.0.2b1/python/clu/protocol.py
+-rw-r--r--   0        0        0     2805 2023-05-23 18:42:10.510527 sdss_clu-2.0.2b1/python/clu/store.py
+-rw-r--r--   0        0        0     7820 2023-05-23 18:42:10.510746 sdss_clu-2.0.2b1/python/clu/testing.py
+-rw-r--r--   0        0        0    16901 2023-05-23 18:42:10.511034 sdss_clu-2.0.2b1/python/clu/tools.py
+-rw-r--r--   0        0        0     6369 1970-01-01 00:00:00.000000 sdss_clu-2.0.2b1/PKG-INFO
```

### Comparing `sdss_clu-2.0.2/LICENSE.md` & `sdss_clu-2.0.2b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/README.rst` & `sdss_clu-2.0.2b1/README.rst`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/pyproject.toml` & `sdss_clu-2.0.2b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-clu"
-version = "2.0.2"
+version = "2.0.2b1"
 description = "A new protocol for SDSS actors."
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.rst"
 homepage = "https://github.com/sdss/clu"
 repository = "https://github.com/sdss/clu"
 documentation = "https://clu.readthedocs.io/en/latest/"
```

### Comparing `sdss_clu-2.0.2/python/clu/__init__.py` & `sdss_clu-2.0.2b1/python/clu/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/__main__.py` & `sdss_clu-2.0.2b1/python/clu/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,19 +176,15 @@
                     if len(chunks) < 2:
                         print(f"Invalid command {text!r}")
                         continue
 
                     actor = chunks[0]
                     command_string = " ".join(chunks[1:])
 
-                    await client.send_command(
-                        actor,
-                        command_string,
-                        await_command=False,
-                    )
+                    await client.send_command(actor, command_string)
 
 
 @click.command(name="clu")
 @click.argument(
     "ACTORS",
     type=str,
     required=False,
```

### Comparing `sdss_clu-2.0.2/python/clu/actor.py` & `sdss_clu-2.0.2b1/python/clu/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/base.py` & `sdss_clu-2.0.2b1/python/clu/base.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/client.py` & `sdss_clu-2.0.2b1/python/clu/client.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/command.py` & `sdss_clu-2.0.2b1/python/clu/command.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/device.py` & `sdss_clu-2.0.2b1/python/clu/device.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/exceptions.py` & `sdss_clu-2.0.2b1/python/clu/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/legacy/actor.py` & `sdss_clu-2.0.2b1/python/clu/legacy/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/legacy/tron.py` & `sdss_clu-2.0.2b1/python/clu/legacy/tron.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/legacy/types/html.py` & `sdss_clu-2.0.2b1/python/clu/legacy/types/html.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/legacy/types/keys.py` & `sdss_clu-2.0.2b1/python/clu/legacy/types/keys.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/legacy/types/messages.py` & `sdss_clu-2.0.2b1/python/clu/legacy/types/messages.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/legacy/types/parser.py` & `sdss_clu-2.0.2b1/python/clu/legacy/types/parser.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/legacy/types/ply/cpp.py` & `sdss_clu-2.0.2b1/python/clu/legacy/types/ply/cpp.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/legacy/types/ply/ctokens.py` & `sdss_clu-2.0.2b1/python/clu/legacy/types/ply/ctokens.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/legacy/types/ply/lex.py` & `sdss_clu-2.0.2b1/python/clu/legacy/types/ply/lex.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/legacy/types/ply/yacc.py` & `sdss_clu-2.0.2b1/python/clu/legacy/types/ply/yacc.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/legacy/types/ply/ygen.py` & `sdss_clu-2.0.2b1/python/clu/legacy/types/ply/ygen.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/legacy/types/pvt.py` & `sdss_clu-2.0.2b1/python/clu/legacy/types/pvt.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/legacy/types/types.py` & `sdss_clu-2.0.2b1/python/clu/legacy/types/types.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/model.py` & `sdss_clu-2.0.2b1/python/clu/model.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/parsers/click.py` & `sdss_clu-2.0.2b1/python/clu/parsers/click.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/parsers/json.py` & `sdss_clu-2.0.2b1/python/clu/parsers/json.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/protocol.py` & `sdss_clu-2.0.2b1/python/clu/protocol.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/store.py` & `sdss_clu-2.0.2b1/python/clu/store.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/testing.py` & `sdss_clu-2.0.2b1/python/clu/testing.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/python/clu/tools.py` & `sdss_clu-2.0.2b1/python/clu/tools.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.0.2/PKG-INFO` & `sdss_clu-2.0.2b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-clu
-Version: 2.0.2
+Version: 2.0.2b1
 Summary: A new protocol for SDSS actors.
 Home-page: https://github.com/sdss/clu
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.8,<4.0
```

