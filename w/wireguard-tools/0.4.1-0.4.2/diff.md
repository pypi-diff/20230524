# Comparing `tmp/wireguard_tools-0.4.1.tar.gz` & `tmp/wireguard_tools-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wireguard_tools-0.4.1.tar", max compression
+gzip compressed data, was "wireguard_tools-0.4.2.tar", max compression
```

## Comparing `wireguard_tools-0.4.1.tar` & `wireguard_tools-0.4.2.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0     1083 2022-12-13 17:55:51.419036 wireguard_tools-0.4.1/LICENSE
-drwxr-xr-x   0        0        0        0 2022-12-13 17:55:51.419036 wireguard_tools-0.4.1/LICENSES/
--rw-r--r--   0        0        0      643 2022-12-13 17:55:51.419036 wireguard_tools-0.4.1/LICENSES/0BSD.txt
--rw-r--r--   0        0        0     1593 2022-12-13 17:55:51.419036 wireguard_tools-0.4.1/LICENSES/CC-PDDC.txt
--rw-r--r--   0        0        0     1078 2022-12-13 17:55:51.419036 wireguard_tools-0.4.1/LICENSES/MIT.txt
--rw-r--r--   0        0        0     6461 2023-02-10 16:50:15.058517 wireguard_tools-0.4.1/README.md
--rw-r--r--   0        0        0     2151 2023-03-15 18:16:02.523913 wireguard_tools-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      362 2023-03-15 18:16:02.523913 wireguard_tools-0.4.1/src/wireguard_tools/__init__.py
--rw-r--r--   0        0        0      188 2022-12-13 17:55:51.423036 wireguard_tools-0.4.1/src/wireguard_tools/__main__.py
--rw-r--r--   0        0        0     7924 2022-12-16 20:19:27.612313 wireguard_tools-0.4.1/src/wireguard_tools/cli.py
--rw-r--r--   0        0        0     5689 2022-12-19 15:20:49.914859 wireguard_tools-0.4.1/src/wireguard_tools/curve25519.py
--rw-r--r--   0        0        0        0 2022-12-13 17:55:51.423036 wireguard_tools-0.4.1/src/wireguard_tools/py.typed
--rw-r--r--   0        0        0      335 2023-03-15 16:34:00.717711 wireguard_tools-0.4.1/src/wireguard_tools/tunnel.conf
--rw-r--r--   0        0        0    10566 2023-03-15 18:09:02.843944 wireguard_tools-0.4.1/src/wireguard_tools/wireguard_config.py
--rw-r--r--   0        0        0     1250 2022-12-16 19:21:20.697346 wireguard_tools-0.4.1/src/wireguard_tools/wireguard_device.py
--rw-r--r--   0        0        0     2571 2022-12-19 15:53:22.370441 wireguard_tools-0.4.1/src/wireguard_tools/wireguard_key.py
--rw-r--r--   0        0        0     4451 2022-12-19 14:37:47.782818 wireguard_tools-0.4.1/src/wireguard_tools/wireguard_netlink.py
--rw-r--r--   0        0        0     5964 2022-12-19 15:53:36.746821 wireguard_tools-0.4.1/src/wireguard_tools/wireguard_uapi.py
--rw-r--r--   0        0        0        0 2022-12-13 17:55:51.423036 wireguard_tools-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0      215 2022-12-13 17:55:51.423036 wireguard_tools-0.4.1/tests/conftest.py
--rw-r--r--   0        0        0     8965 2022-12-13 17:55:51.423036 wireguard_tools-0.4.1/tests/test_curve25519.py
--rw-r--r--   0        0        0     1460 2022-12-13 17:55:51.423036 wireguard_tools-0.4.1/tests/test_wireguard_config.py
--rw-r--r--   0        0        0      661 2022-12-13 17:55:51.423036 wireguard_tools-0.4.1/tests/test_wireguard_key.py
--rw-r--r--   0        0        0     7593 1970-01-01 00:00:00.000000 wireguard_tools-0.4.1/setup.py
--rw-r--r--   0        0        0     7570 1970-01-01 00:00:00.000000 wireguard_tools-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-12-13 17:55:51.419036 wireguard_tools-0.4.2/LICENSE
+drwxr-xr-x   0        0        0        0 2022-12-13 17:55:51.419036 wireguard_tools-0.4.2/LICENSES/
+-rw-r--r--   0        0        0      643 2022-12-13 17:55:51.419036 wireguard_tools-0.4.2/LICENSES/0BSD.txt
+-rw-r--r--   0        0        0     1593 2022-12-13 17:55:51.419036 wireguard_tools-0.4.2/LICENSES/CC-PDDC.txt
+-rw-r--r--   0        0        0     1078 2022-12-13 17:55:51.419036 wireguard_tools-0.4.2/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     6461 2023-02-10 16:50:15.058517 wireguard_tools-0.4.2/README.md
+-rw-r--r--   0        0        0     2151 2023-05-24 16:10:48.981131 wireguard_tools-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      362 2023-05-24 16:10:48.981131 wireguard_tools-0.4.2/src/wireguard_tools/__init__.py
+-rw-r--r--   0        0        0      188 2022-12-13 17:55:51.423036 wireguard_tools-0.4.2/src/wireguard_tools/__main__.py
+-rw-r--r--   0        0        0     7924 2022-12-16 20:19:27.612313 wireguard_tools-0.4.2/src/wireguard_tools/cli.py
+-rw-r--r--   0        0        0     5689 2022-12-19 15:20:49.914859 wireguard_tools-0.4.2/src/wireguard_tools/curve25519.py
+-rw-r--r--   0        0        0        0 2022-12-13 17:55:51.423036 wireguard_tools-0.4.2/src/wireguard_tools/py.typed
+-rw-r--r--   0        0        0      335 2023-03-15 16:34:00.717711 wireguard_tools-0.4.2/src/wireguard_tools/tunnel.conf
+-rw-r--r--   0        0        0    10566 2023-03-15 18:09:02.843944 wireguard_tools-0.4.2/src/wireguard_tools/wireguard_config.py
+-rw-r--r--   0        0        0     1250 2022-12-16 19:21:20.697346 wireguard_tools-0.4.2/src/wireguard_tools/wireguard_device.py
+-rw-r--r--   0        0        0     2571 2022-12-19 15:53:22.370441 wireguard_tools-0.4.2/src/wireguard_tools/wireguard_key.py
+-rw-r--r--   0        0        0     4456 2023-05-24 16:10:17.684255 wireguard_tools-0.4.2/src/wireguard_tools/wireguard_netlink.py
+-rw-r--r--   0        0        0     5964 2022-12-19 15:53:36.746821 wireguard_tools-0.4.2/src/wireguard_tools/wireguard_uapi.py
+-rw-r--r--   0        0        0        0 2022-12-13 17:55:51.423036 wireguard_tools-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0      215 2022-12-13 17:55:51.423036 wireguard_tools-0.4.2/tests/conftest.py
+-rw-r--r--   0        0        0     8965 2022-12-13 17:55:51.423036 wireguard_tools-0.4.2/tests/test_curve25519.py
+-rw-r--r--   0        0        0     1460 2022-12-13 17:55:51.423036 wireguard_tools-0.4.2/tests/test_wireguard_config.py
+-rw-r--r--   0        0        0      661 2022-12-13 17:55:51.423036 wireguard_tools-0.4.2/tests/test_wireguard_key.py
+-rw-r--r--   0        0        0     7570 1970-01-01 00:00:00.000000 wireguard_tools-0.4.2/PKG-INFO
```

### Comparing `wireguard_tools-0.4.1/LICENSE` & `wireguard_tools-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.1/LICENSES/0BSD.txt` & `wireguard_tools-0.4.2/LICENSES/0BSD.txt`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.1/LICENSES/CC-PDDC.txt` & `wireguard_tools-0.4.2/LICENSES/CC-PDDC.txt`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.1/LICENSES/MIT.txt` & `wireguard_tools-0.4.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.1/README.md` & `wireguard_tools-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.1/pyproject.toml` & `wireguard_tools-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2022-2023 Carnegie Mellon University
 # SPDX-License-Identifier: 0BSD
 
 [tool.poetry]
 name = "wireguard-tools"
-version = "0.4.1"
+version = "0.4.2"
 description = "Pure python reimplementation of wireguard-tools"
 authors = [
     "Carnegie Mellon University <satya+group@cs.cmu.edu>",
     "Jan Harkes <jaharkes@cs.cmu.edu>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `wireguard_tools-0.4.1/src/wireguard_tools/cli.py` & `wireguard_tools-0.4.2/src/wireguard_tools/cli.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.1/src/wireguard_tools/curve25519.py` & `wireguard_tools-0.4.2/src/wireguard_tools/curve25519.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.1/src/wireguard_tools/wireguard_config.py` & `wireguard_tools-0.4.2/src/wireguard_tools/wireguard_config.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.1/src/wireguard_tools/wireguard_device.py` & `wireguard_tools-0.4.2/src/wireguard_tools/wireguard_device.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.1/src/wireguard_tools/wireguard_key.py` & `wireguard_tools-0.4.2/src/wireguard_tools/wireguard_key.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.1/src/wireguard_tools/wireguard_netlink.py` & `wireguard_tools-0.4.2/src/wireguard_tools/wireguard_netlink.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         )
 
         cur_peers = set(current_config.peers)
         new_peers = set(config.peers)
 
         # remove peers that are no longer in the configuration
         for key in cur_peers.difference(new_peers):
-            self.wg.set(self.interface, peer=dict(public_key=key, remove=True))
+            self.wg.set(self.interface, peer=dict(public_key=str(key), remove=True))
 
         # update any changed peers
         for key in cur_peers.intersection(new_peers):
             peer = config.peers[key]
             if peer != current_config.peers[key]:
                 self.wg.set(self.interface, peer=self._wg_set_peer_arg(peer))
```

### Comparing `wireguard_tools-0.4.1/src/wireguard_tools/wireguard_uapi.py` & `wireguard_tools-0.4.2/src/wireguard_tools/wireguard_uapi.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.1/tests/test_curve25519.py` & `wireguard_tools-0.4.2/tests/test_curve25519.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.1/tests/test_wireguard_config.py` & `wireguard_tools-0.4.2/tests/test_wireguard_config.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.1/tests/test_wireguard_key.py` & `wireguard_tools-0.4.2/tests/test_wireguard_key.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.1/setup.py` & `wireguard_tools-0.4.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,229 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: wireguard-tools
+Version: 0.4.2
+Summary: Pure python reimplementation of wireguard-tools
+Home-page: https://github.com/cmusatyalab/wireguard-tools
+License: MIT
+Author: Carnegie Mellon University
+Author-email: satya+group@cs.cmu.edu
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: attrs (>=22.1.0)
+Requires-Dist: pyroute2 (>=0.7.3,<0.8.0)
+Requires-Dist: segno (>=1.5.2,<2.0.0)
+Project-URL: Repository, https://github.com/cmusatyalab/wireguard-tools
+Description-Content-Type: text/markdown
+
+# WireGuard-tools
+
+Pure Python reimplementation of wireguard-tools with an aim to provide easily
+reusable library functions to handle reading and writing of
+[WireGuard®](https://www.wireguard.com/) configuration files as well as
+interacting with WireGuard devices, both in-kernel through the Netlink API and
+userspace implementations through the cross-platform UAPI API.
+
+
+## Installation/Usage
+
+```sh
+    pipx install wireguard-tools
+    wg-py --help
+```
+
+Implemented `wg` command line functionality,
+
+- [x] show - Show configuration and device information
+- [x] showconf - Dump current device configuration
+- [ ] set - Change current configuration, add/remove/change peers
+- [x] setconf - Apply configuration to device
+- [ ] addconf - Append configuration to device
+- [x] syncconf - Synchronizes configuration with device
+- [x] genkey, genpsk, pubkey - Key generation
+
+
+Also includes some `wg-quick` functions,
+
+- [ ] up, down - Create and configure WireGuard device and interface
+- [ ] save - Dump device and interface configuration
+- [x] strip - Filter wg-quick settings from configuration
+
+
+Needs root (sudo) access to query and configure the WireGuard devices through
+netlink. But root doesn't know about the currently active virtualenv, you may
+have to pass the full path to the script in the virtualenv, or use
+`python3 -m wireguard_tools`
+
+```sh
+    sudo `which wg-py` showconf <interface>
+    sudo /path/to/venv/python3 -m wireguard_tools showconf <interface>
+```
+
+
+## Library usage
+
+### Parsing WireGuard keys
+
+The WireguardKey class will parse base64-encoded keys, the default base64
+encoded string, but also an urlsafe base64 encoded variant. It also exposes
+both private key generating and public key deriving functions. Be sure to pass
+any base64 or hex encoded keys as 'str' and not 'bytes', otherwise it will
+assume the key was already decoded to its raw form.
+
+```python
+from wireguard_tools import WireguardKey
+
+private_key = WireguardKey.generate()
+public_key = private_key.public_key()
+
+# print base64 encoded key
+print(public_key)
+
+# print urlsafe encoded key
+print(public_key.urlsafe)
+
+# print hexadecimal encoded key
+print(public_key.hex())
+```
+
+### Working with WireGuard configuration files
+
+The WireGuard configuration file is similar to, but not quite, the INI format
+because it has duplicate keys for both section names (i.e. [Peer]) as well as
+configuration keys within a section. According to the format description,
+AllowedIPs, Address, and DNS configuration keys 'may be specified multiple
+times'.
+
+```python
+from wireguard_tools import WireguardConfig
+
+with open("wg0.conf") as fh:
+    config = WireguardConfig.from_wgconfig(fh)
+```
+
+We can also serialize and deserialize from a simple dict-based format which
+uses only basic JSON datatypes and, as such, can be used to convert to various
+formats (i.e. json, yaml, toml, pickle) either to disk or to pass over a
+network.
+
+```python
+from wireguard_tools import WireguardConfig
+from pprint import pprint
+
+dict_config = dict(
+    private_key="...",
+    peers=[
+        dict(
+            public_key="...",
+            preshared_key=None,
+            endpoint_host="remote_host",
+            endpoint_port=5120,
+            persistent_keepalive=30,
+            allowed_ips=["0.0.0.0/0"],
+        ),
+    ],
+)
+config = WireguardConfig.from_dict(dict_config)
+
+dict_config = config.asdict()
+pprint(dict_config)
+```
+
+Finally, there is a `to_qrcode` function that returns a segno.QRCode object
+which contains the configuration. This can be printed and scanned with the
+wireguard-android application. Careful with these because the QRcode exposes
+an easily captured copy of the private key as part of the configuration file.
+It is convenient, but definitely not secure.
+
+```python
+from wireguard_tools import WireguardConfig
+from pprint import pprint
+
+dict_config = dict(
+    private_key="...",
+    peers=[
+        dict(
+            public_key="...",
+            preshared_key=None,
+            endpoint_host="remote_host",
+            endpoint_port=5120,
+            persistent_keepalive=30,
+            allowed_ips=["0.0.0.0/0"],
+        ),
+    ],
+)
+config = WireguardConfig.from_dict(dict_config)
+
+qr = config.to_qrcode()
+qr.save("wgconfig.png")
+qr.terminal(compact=True)
+```
+
+
+### Working with WireGuard devices
+
+```python
+from wireguard_tools import WireguardDevice
+
+ifnames = [device.interface for device in WireguardDevice.list()]
+
+device = WireguardDevice.get("wg0")
+
+wgconfig = device.get_config()
+
+device.set_config(wgconfig)
+```
+
+## Bugs
+
+The setconf/syncconf implementation is not quite correct. They currently use
+the same underlying set of operations but netlink-api's `set_config`
+implementation actually does something closer to syncconf, while the uapi-api
+implementation matches setconf.
+
+This implementation has only been tested on Linux where we've only actively
+used a subset of the available functionality, i.e. the common scenario is
+configuring an interface only once with just a single peer.
+
+
+## Licenses
+
+wireguard-tools is MIT licensed
+
+    Copyright (c) 2022-2023 Carnegie Mellon University
+
+    Permission is hereby granted, free of charge, to any person obtaining a copy of
+    this software and associated documentation files (the "Software"), to deal in
+    the Software without restriction, including without limitation the rights to
+    use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+    of the Software, and to permit persons to whom the Software is furnished to do
+    so, subject to the following conditions:
+
+    The above copyright notice and this permission notice shall be included in all
+    copies or substantial portions of the Software.
+
+    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+    SOFTWARE.
 
-package_dir = \
-{'': 'src'}
+`wireguard_tools/curve25519.py` was released in the public domain
 
-packages = \
-['wireguard_tools']
+    Copyright Nicko van Someren, 2021. This code is released into the public domain.
+    https://gist.github.com/nickovs/cc3c22d15f239a2640c185035c06f8a3
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['attrs>=22.1.0', 'pyroute2>=0.7.3,<0.8.0', 'segno>=1.5.2,<2.0.0']
-
-entry_points = \
-{'console_scripts': ['wg-py = wireguard_tools.cli:main']}
-
-setup_kwargs = {
-    'name': 'wireguard-tools',
-    'version': '0.4.1',
-    'description': 'Pure python reimplementation of wireguard-tools',
-    'long_description': '# WireGuard-tools\n\nPure Python reimplementation of wireguard-tools with an aim to provide easily\nreusable library functions to handle reading and writing of\n[WireGuard®](https://www.wireguard.com/) configuration files as well as\ninteracting with WireGuard devices, both in-kernel through the Netlink API and\nuserspace implementations through the cross-platform UAPI API.\n\n\n## Installation/Usage\n\n```sh\n    pipx install wireguard-tools\n    wg-py --help\n```\n\nImplemented `wg` command line functionality,\n\n- [x] show - Show configuration and device information\n- [x] showconf - Dump current device configuration\n- [ ] set - Change current configuration, add/remove/change peers\n- [x] setconf - Apply configuration to device\n- [ ] addconf - Append configuration to device\n- [x] syncconf - Synchronizes configuration with device\n- [x] genkey, genpsk, pubkey - Key generation\n\n\nAlso includes some `wg-quick` functions,\n\n- [ ] up, down - Create and configure WireGuard device and interface\n- [ ] save - Dump device and interface configuration\n- [x] strip - Filter wg-quick settings from configuration\n\n\nNeeds root (sudo) access to query and configure the WireGuard devices through\nnetlink. But root doesn\'t know about the currently active virtualenv, you may\nhave to pass the full path to the script in the virtualenv, or use\n`python3 -m wireguard_tools`\n\n```sh\n    sudo `which wg-py` showconf <interface>\n    sudo /path/to/venv/python3 -m wireguard_tools showconf <interface>\n```\n\n\n## Library usage\n\n### Parsing WireGuard keys\n\nThe WireguardKey class will parse base64-encoded keys, the default base64\nencoded string, but also an urlsafe base64 encoded variant. It also exposes\nboth private key generating and public key deriving functions. Be sure to pass\nany base64 or hex encoded keys as \'str\' and not \'bytes\', otherwise it will\nassume the key was already decoded to its raw form.\n\n```python\nfrom wireguard_tools import WireguardKey\n\nprivate_key = WireguardKey.generate()\npublic_key = private_key.public_key()\n\n# print base64 encoded key\nprint(public_key)\n\n# print urlsafe encoded key\nprint(public_key.urlsafe)\n\n# print hexadecimal encoded key\nprint(public_key.hex())\n```\n\n### Working with WireGuard configuration files\n\nThe WireGuard configuration file is similar to, but not quite, the INI format\nbecause it has duplicate keys for both section names (i.e. [Peer]) as well as\nconfiguration keys within a section. According to the format description,\nAllowedIPs, Address, and DNS configuration keys \'may be specified multiple\ntimes\'.\n\n```python\nfrom wireguard_tools import WireguardConfig\n\nwith open("wg0.conf") as fh:\n    config = WireguardConfig.from_wgconfig(fh)\n```\n\nWe can also serialize and deserialize from a simple dict-based format which\nuses only basic JSON datatypes and, as such, can be used to convert to various\nformats (i.e. json, yaml, toml, pickle) either to disk or to pass over a\nnetwork.\n\n```python\nfrom wireguard_tools import WireguardConfig\nfrom pprint import pprint\n\ndict_config = dict(\n    private_key="...",\n    peers=[\n        dict(\n            public_key="...",\n            preshared_key=None,\n            endpoint_host="remote_host",\n            endpoint_port=5120,\n            persistent_keepalive=30,\n            allowed_ips=["0.0.0.0/0"],\n        ),\n    ],\n)\nconfig = WireguardConfig.from_dict(dict_config)\n\ndict_config = config.asdict()\npprint(dict_config)\n```\n\nFinally, there is a `to_qrcode` function that returns a segno.QRCode object\nwhich contains the configuration. This can be printed and scanned with the\nwireguard-android application. Careful with these because the QRcode exposes\nan easily captured copy of the private key as part of the configuration file.\nIt is convenient, but definitely not secure.\n\n```python\nfrom wireguard_tools import WireguardConfig\nfrom pprint import pprint\n\ndict_config = dict(\n    private_key="...",\n    peers=[\n        dict(\n            public_key="...",\n            preshared_key=None,\n            endpoint_host="remote_host",\n            endpoint_port=5120,\n            persistent_keepalive=30,\n            allowed_ips=["0.0.0.0/0"],\n        ),\n    ],\n)\nconfig = WireguardConfig.from_dict(dict_config)\n\nqr = config.to_qrcode()\nqr.save("wgconfig.png")\nqr.terminal(compact=True)\n```\n\n\n### Working with WireGuard devices\n\n```python\nfrom wireguard_tools import WireguardDevice\n\nifnames = [device.interface for device in WireguardDevice.list()]\n\ndevice = WireguardDevice.get("wg0")\n\nwgconfig = device.get_config()\n\ndevice.set_config(wgconfig)\n```\n\n## Bugs\n\nThe setconf/syncconf implementation is not quite correct. They currently use\nthe same underlying set of operations but netlink-api\'s `set_config`\nimplementation actually does something closer to syncconf, while the uapi-api\nimplementation matches setconf.\n\nThis implementation has only been tested on Linux where we\'ve only actively\nused a subset of the available functionality, i.e. the common scenario is\nconfiguring an interface only once with just a single peer.\n\n\n## Licenses\n\nwireguard-tools is MIT licensed\n\n    Copyright (c) 2022-2023 Carnegie Mellon University\n\n    Permission is hereby granted, free of charge, to any person obtaining a copy of\n    this software and associated documentation files (the "Software"), to deal in\n    the Software without restriction, including without limitation the rights to\n    use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies\n    of the Software, and to permit persons to whom the Software is furnished to do\n    so, subject to the following conditions:\n\n    The above copyright notice and this permission notice shall be included in all\n    copies or substantial portions of the Software.\n\n    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\n    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\n    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\n    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\n    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\n    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\n    SOFTWARE.\n\n`wireguard_tools/curve25519.py` was released in the public domain\n\n    Copyright Nicko van Someren, 2021. This code is released into the public domain.\n    https://gist.github.com/nickovs/cc3c22d15f239a2640c185035c06f8a3\n\n"WireGuard" is a registered trademark of Jason A. Donenfeld.\n',
-    'author': 'Carnegie Mellon University',
-    'author_email': 'satya+group@cs.cmu.edu',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/cmusatyalab/wireguard-tools',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+"WireGuard" is a registered trademark of Jason A. Donenfeld.
 
-
-setup(**setup_kwargs)
```

