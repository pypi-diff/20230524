# Comparing `tmp/pyocient-1.0.9.tar.gz` & `tmp/pyocient-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyocient-1.0.9.tar", last modified: Fri May 20 16:21:03 2022, max compression
+gzip compressed data, was "pyocient-2.0.0.tar", last modified: Wed May 24 09:33:51 2023, max compression
```

## Comparing `pyocient-1.0.9.tar` & `pyocient-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 16:21:03.742177 pyocient-1.0.9/
--r-xr-xr-x   0 root         (0) root         (0)   312011 2022-05-10 16:56:57.000000 pyocient-1.0.9/ClientWireProtocol_pb2.py
--r-xr-xr-x   0 root         (0) root         (0)      581 2022-05-20 16:21:03.000000 pyocient-1.0.9/LICENSE.txt
--r-xr-xr-x   0 root         (0) root         (0)       93 2022-05-20 16:21:03.000000 pyocient-1.0.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2054 2022-05-20 16:21:03.742177 pyocient-1.0.9/PKG-INFO
--r-xr-xr-x   0 root         (0) root         (0)     1175 2022-05-20 16:21:03.000000 pyocient-1.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-20 16:21:03.742177 pyocient-1.0.9/pyocient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2054 2022-05-20 16:21:03.000000 pyocient-1.0.9/pyocient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      295 2022-05-20 16:21:03.000000 pyocient-1.0.9/pyocient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-20 16:21:03.000000 pyocient-1.0.9/pyocient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2022-05-20 16:21:03.000000 pyocient-1.0.9/pyocient.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      133 2022-05-20 16:21:03.000000 pyocient-1.0.9/pyocient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       40 2022-05-20 16:21:03.000000 pyocient-1.0.9/pyocient.egg-info/top_level.txt
--r-xr-xr-x   0 root         (0) root         (0)   107463 2022-05-17 17:43:55.000000 pyocient-1.0.9/pyocient.py
--r-xr-xr-x   0 root         (0) root         (0)      107 2022-05-20 16:21:03.743177 pyocient-1.0.9/setup.cfg
--r-xr-xr-x   0 root         (0) root         (0)     2098 2022-05-20 16:21:03.000000 pyocient-1.0.9/setup.py
--r-xr-xr-x   0 root         (0) root         (0)       20 2022-05-20 16:21:03.000000 pyocient-1.0.9/version.py
+drwxr-xr-x   0 buildfarm  (1789) users      (100)        0 2023-05-24 09:33:51.914239 pyocient-2.0.0/
+-r-xr-xr-x   0 buildfarm  (1789) users      (100)      581 2023-05-24 09:33:50.000000 pyocient-2.0.0/LICENSE.txt
+-rw-r--r--   0 buildfarm  (1789) users      (100)     2178 2023-05-24 09:33:51.914239 pyocient-2.0.0/PKG-INFO
+-r-xr-xr-x   0 buildfarm  (1789) users      (100)     1247 2023-05-24 09:33:50.000000 pyocient-2.0.0/README.md
+drwxr-xr-x   0 buildfarm  (1789) users      (100)        0 2023-05-24 09:33:51.914239 pyocient-2.0.0/pyocient/
+-r-xr-xr-x   0 buildfarm  (1789) users      (100)    45506 2023-04-28 19:29:28.000000 pyocient-2.0.0/pyocient/ClientWireProtocol_pb2.py
+-r-xr-xr-x   0 buildfarm  (1789) users      (100)     2656 2023-05-23 07:54:04.000000 pyocient-2.0.0/pyocient/__init__.py
+-r-xr-xr-x   0 buildfarm  (1789) users      (100)   107955 2023-05-23 07:54:04.000000 pyocient-2.0.0/pyocient/api.py
+-r-xr-xr-x   0 buildfarm  (1789) users      (100)    18021 2023-05-23 07:54:04.000000 pyocient-2.0.0/pyocient/cli.py
+-r-xr-xr-x   0 buildfarm  (1789) users      (100)       21 2023-05-23 07:54:04.000000 pyocient-2.0.0/pyocient/pkg_version.py
+-rw-r--r--   0 buildfarm  (1789) users      (100)        0 2023-05-24 09:33:50.000000 pyocient-2.0.0/pyocient/py.typed
+drwxr-xr-x   0 buildfarm  (1789) users      (100)        0 2023-05-24 09:33:51.914239 pyocient-2.0.0/pyocient.egg-info/
+-rw-r--r--   0 buildfarm  (1789) users      (100)     2178 2023-05-24 09:33:51.000000 pyocient-2.0.0/pyocient.egg-info/PKG-INFO
+-rw-r--r--   0 buildfarm  (1789) users      (100)      354 2023-05-24 09:33:51.000000 pyocient-2.0.0/pyocient.egg-info/SOURCES.txt
+-rw-r--r--   0 buildfarm  (1789) users      (100)        1 2023-05-24 09:33:51.000000 pyocient-2.0.0/pyocient.egg-info/dependency_links.txt
+-rw-r--r--   0 buildfarm  (1789) users      (100)       48 2023-05-24 09:33:51.000000 pyocient-2.0.0/pyocient.egg-info/entry_points.txt
+-rw-r--r--   0 buildfarm  (1789) users      (100)       89 2023-05-24 09:33:51.000000 pyocient-2.0.0/pyocient.egg-info/requires.txt
+-rw-r--r--   0 buildfarm  (1789) users      (100)        9 2023-05-24 09:33:51.000000 pyocient-2.0.0/pyocient.egg-info/top_level.txt
+-rw-r--r--   0 buildfarm  (1789) users      (100)       38 2023-05-24 09:33:51.914239 pyocient-2.0.0/setup.cfg
+-r-xr-xr-x   0 buildfarm  (1789) users      (100)     1941 2023-05-24 09:33:50.000000 pyocient-2.0.0/setup.py
```

### Comparing `pyocient-1.0.9/LICENSE.txt` & `pyocient-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyocient-1.0.9/PKG-INFO` & `pyocient-2.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 Metadata-Version: 2.1
 Name: pyocient
-Version: 1.0.9
+Version: 2.0.0
 Summary: Ocient Database Python API
 Home-page: https://www.ocient.com/
 Author: Ocient Inc
 Author-email: info@ocient.com
 License: UNKNOWN
 Description: # Ocient Database Python API
         
         This python database API conforms to the Python Database API
         Specification 2.0 and can be used to access the Ocient database.
         
         This module can also be called as a main function, in which case
-        it acts as a primitive CLI for the database.
+        it acts as a CLI for the database.
         
         When called as main, it a connection string in DSN (data source name)
         format, followed by zero or more query strings that will be executed.
         Output is returned in JSON format.
         
         The Ocient DSN is of the format:
            `ocient://user:password@[host][:port][/database][?param1=value1&...]`
         
         `user` and `password` must be supplied.  `host` defaults to localhost,
         port defaults to 4050, database defaults to `system` and `tls` defaults
-        to `off`.
+        to `unverified`.
         
         Currently supported parameters are:
         
         - tls: Which can have the values "off", "unverified", or "on"
         - force: Which can have the values "true"
-        - handshake: Which can have the value "cbc", "gcm", or "sso".
+        - handshake: Which can have the value "cbc", "gcm", or "sso"
         
         For the handshake protocols, "cbc" (Cipher Block Chaining) denotes a previous password encryption protocol which
-        should be avoided. "gcm" (Galois/Counter Mode), which pyocient will default to,  is recommended. If single sign
+        should be avoided. "gcm" (Galois/Counter Mode), which pyocient will default to, is recommended. If single sign
         on is desired, then "sso" should be used.
+        
+        Release notes are available at https://github.com/ocient/pyocient_release/
+        
 Keywords: database,sql,development
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.5, <4
+Classifier: Typing :: Typed
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

### Comparing `pyocient-1.0.9/README.md` & `pyocient-2.0.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # Ocient Database Python API
 
 This python database API conforms to the Python Database API
 Specification 2.0 and can be used to access the Ocient database.
 
 This module can also be called as a main function, in which case
-it acts as a primitive CLI for the database.
+it acts as a CLI for the database.
 
 When called as main, it a connection string in DSN (data source name)
 format, followed by zero or more query strings that will be executed.
 Output is returned in JSON format.
 
 The Ocient DSN is of the format:
    `ocient://user:password@[host][:port][/database][?param1=value1&...]`
 
 `user` and `password` must be supplied.  `host` defaults to localhost,
 port defaults to 4050, database defaults to `system` and `tls` defaults
-to `off`.
+to `unverified`.
 
 Currently supported parameters are:
 
 - tls: Which can have the values "off", "unverified", or "on"
 - force: Which can have the values "true"
-- handshake: Which can have the value "cbc", "gcm", or "sso".
+- handshake: Which can have the value "cbc", "gcm", or "sso"
 
 For the handshake protocols, "cbc" (Cipher Block Chaining) denotes a previous password encryption protocol which
-should be avoided. "gcm" (Galois/Counter Mode), which pyocient will default to,  is recommended. If single sign
-on is desired, then "sso" should be used.
+should be avoided. "gcm" (Galois/Counter Mode), which pyocient will default to, is recommended. If single sign
+on is desired, then "sso" should be used.
+
+Release notes are available at https://github.com/ocient/pyocient_release/
```

### Comparing `pyocient-1.0.9/pyocient.egg-info/PKG-INFO` & `pyocient-2.0.0/pyocient.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 Metadata-Version: 2.1
 Name: pyocient
-Version: 1.0.9
+Version: 2.0.0
 Summary: Ocient Database Python API
 Home-page: https://www.ocient.com/
 Author: Ocient Inc
 Author-email: info@ocient.com
 License: UNKNOWN
 Description: # Ocient Database Python API
         
         This python database API conforms to the Python Database API
         Specification 2.0 and can be used to access the Ocient database.
         
         This module can also be called as a main function, in which case
-        it acts as a primitive CLI for the database.
+        it acts as a CLI for the database.
         
         When called as main, it a connection string in DSN (data source name)
         format, followed by zero or more query strings that will be executed.
         Output is returned in JSON format.
         
         The Ocient DSN is of the format:
            `ocient://user:password@[host][:port][/database][?param1=value1&...]`
         
         `user` and `password` must be supplied.  `host` defaults to localhost,
         port defaults to 4050, database defaults to `system` and `tls` defaults
-        to `off`.
+        to `unverified`.
         
         Currently supported parameters are:
         
         - tls: Which can have the values "off", "unverified", or "on"
         - force: Which can have the values "true"
-        - handshake: Which can have the value "cbc", "gcm", or "sso".
+        - handshake: Which can have the value "cbc", "gcm", or "sso"
         
         For the handshake protocols, "cbc" (Cipher Block Chaining) denotes a previous password encryption protocol which
-        should be avoided. "gcm" (Galois/Counter Mode), which pyocient will default to,  is recommended. If single sign
+        should be avoided. "gcm" (Galois/Counter Mode), which pyocient will default to, is recommended. If single sign
         on is desired, then "sso" should be used.
+        
+        Release notes are available at https://github.com/ocient/pyocient_release/
+        
 Keywords: database,sql,development
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.5, <4
+Classifier: Typing :: Typed
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

### Comparing `pyocient-1.0.9/pyocient.py` & `pyocient-2.0.0/pyocient/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,6717 +1,6748 @@
 00000000: 2321 2f75 7372 2f62 696e 2f65 6e76 2070  #!/usr/bin/env p
-00000010: 7974 686f 6e33 0a22 2222 5079 7468 6f6e  ython3."""Python
-00000020: 2044 6174 6162 6173 6520 4150 4920 666f   Database API fo
-00000030: 7220 7468 6520 4f63 6965 6e74 2044 6174  r the Ocient Dat
-00000040: 6162 6173 650a 0a54 6869 7320 7079 7468  abase..This pyth
-00000050: 6f6e 2064 6174 6162 6173 6520 4150 4920  on database API 
-00000060: 636f 6e66 6f72 6d73 2074 6f20 7468 6520  conforms to the 
-00000070: 5079 7468 6f6e 2044 6174 6162 6173 6520  Python Database 
-00000080: 4150 490a 5370 6563 6966 6963 6174 696f  API.Specificatio
-00000090: 6e20 322e 3020 616e 6420 6361 6e20 6265  n 2.0 and can be
-000000a0: 2075 7365 6420 746f 2061 6363 6573 7320   used to access 
-000000b0: 7468 6520 4f63 6965 6e74 2064 6174 6162  the Ocient datab
-000000c0: 6173 652e 0a0a 5468 6973 206d 6f64 756c  ase...This modul
-000000d0: 6520 6361 6e20 616c 736f 2062 6520 6361  e can also be ca
-000000e0: 6c6c 6564 2061 7320 6120 6d61 696e 2066  lled as a main f
-000000f0: 756e 6374 696f 6e2c 2069 6e20 7768 6963  unction, in whic
-00000100: 6820 6361 7365 0a69 7420 6163 7473 2061  h case.it acts a
-00000110: 7320 6120 7072 696d 6974 6976 6520 434c  s a primitive CL
-00000120: 4920 666f 7220 7468 6520 6461 7461 6261  I for the databa
-00000130: 7365 2e0a 0a57 6865 6e20 6361 6c6c 6564  se...When called
-00000140: 2061 7320 6d61 696e 2c20 6974 2061 2063   as main, it a c
-00000150: 6f6e 6e65 6374 696f 6e20 7374 7269 6e67  onnection string
-00000160: 2069 6e20 4453 4e20 2864 6174 6120 736f   in DSN (data so
-00000170: 7572 6365 206e 616d 6529 0a66 6f72 6d61  urce name).forma
-00000180: 742c 2066 6f6c 6c6f 7765 6420 6279 207a  t, followed by z
-00000190: 6572 6f20 6f72 206d 6f72 6520 7175 6572  ero or more quer
-000001a0: 7920 7374 7269 6e67 7320 7468 6174 2077  y strings that w
-000001b0: 696c 6c20 6265 2065 7865 6375 7465 642e  ill be executed.
-000001c0: 0a4f 7574 7075 7420 6973 2072 6574 7572  .Output is retur
-000001d0: 6e65 6420 696e 204a 534f 4e20 666f 726d  ned in JSON form
-000001e0: 6174 2e0a 0a54 6865 204f 6369 656e 7420  at...The Ocient 
-000001f0: 4453 4e20 6973 206f 6620 7468 6520 666f  DSN is of the fo
-00000200: 726d 6174 3a0a 2020 2060 6f63 6965 6e74  rmat:.   `ocient
-00000210: 3a2f 2f75 7365 723a 7061 7373 776f 7264  ://user:password
-00000220: 405b 686f 7374 5d5b 3a70 6f72 745d 5b2f  @[host][:port][/
-00000230: 6461 7461 6261 7365 5d5b 3f70 6172 616d  database][?param
-00000240: 313d 7661 6c75 6531 262e 2e2e 5d60 0a0a  1=value1&...]`..
-00000250: 6075 7365 7260 2061 6e64 2060 7061 7373  `user` and `pass
-00000260: 776f 7264 6020 6d75 7374 2062 6520 7375  word` must be su
-00000270: 7070 6c69 6564 2e20 2060 686f 7374 6020  pplied.  `host` 
-00000280: 6465 6661 756c 7473 2074 6f20 6c6f 6361  defaults to loca
-00000290: 6c68 6f73 742c 0a70 6f72 7420 6465 6661  lhost,.port defa
-000002a0: 756c 7473 2074 6f20 3430 3530 2c20 6461  ults to 4050, da
-000002b0: 7461 6261 7365 2064 6566 6175 6c74 7320  tabase defaults 
-000002c0: 746f 2060 7379 7374 656d 6020 616e 6420  to `system` and 
-000002d0: 6074 6c73 6020 6465 6661 756c 7473 0a74  `tls` defaults.t
-000002e0: 6f20 606f 6666 602e 0a0a 4d75 6c74 6970  o `off`...Multip
-000002f0: 6c65 2068 6f73 7473 206d 6179 2062 6520  le hosts may be 
-00000300: 7370 6563 6966 6965 642c 2073 6570 6172  specified, separ
-00000310: 6174 6564 2062 7920 6120 636f 6d6d 612c  ated by a comma,
-00000320: 2069 6e20 7768 6963 6820 6361 7365 2074   in which case t
-00000330: 6865 0a68 6f73 7473 2077 696c 6c20 6265  he.hosts will be
-00000340: 2074 7269 6564 2069 6e20 6f72 6465 7220   tried in order 
-00000350: 2054 6875 7320 616e 2065 7861 6d70 6c65   Thus an example
-00000360: 2044 534e 206d 6967 6874 2062 650a 606f   DSN might be.`o
-00000370: 6369 656e 743a 2f2f 736f 6d65 6f6e 653a  cient://someone:
-00000380: 736f 6d65 7061 7373 776f 7264 4068 6f73  somepassword@hos
-00000390: 7431 2c68 6f73 7432 3a34 3035 312f 6d79  t1,host2:4051/my
-000003a0: 6462 600a 0a43 7572 7265 6e74 6c79 2073  db`..Currently s
-000003b0: 7570 706f 7274 6564 2070 6172 616d 6574  upported paramet
-000003c0: 6572 7320 6172 653a 0a0a 2d20 746c 733a  ers are:..- tls:
-000003d0: 2057 6869 6368 2063 616e 2068 6176 6520   Which can have 
-000003e0: 7468 6520 7661 6c75 6573 2022 6f66 6622  the values "off"
-000003f0: 2c20 2275 6e76 6572 6966 6965 6422 2c20  , "unverified", 
-00000400: 6f72 2022 6f6e 220a 2d20 666f 7263 653a  or "on".- force:
-00000410: 2074 7275 6520 6f72 2066 616c 7365 2074   true or false t
-00000420: 6f20 666f 7263 6520 7468 6520 636f 6e6e  o force the conn
-00000430: 6563 7469 6f6e 2074 6f20 7374 6179 206f  ection to stay o
-00000440: 6e20 7468 6973 2073 6572 7665 720a 0a41  n this server..A
-00000450: 6e79 2077 6172 6e69 6e67 7320 7265 7475  ny warnings retu
-00000460: 726e 6564 2062 7920 7468 6520 6461 7461  rned by the data
-00000470: 6261 7365 2061 7265 2073 656e 7420 746f  base are sent to
-00000480: 2074 6865 2070 7974 686f 6e20 7761 726e   the python warn
-00000490: 696e 6773 0a6d 6f64 756c 652e 2020 4279  ings.module.  By
-000004a0: 2064 6566 6175 6c74 2074 6861 7420 6d6f   default that mo
-000004b0: 6475 6c65 2073 656e 6473 2077 6172 6e69  dule sends warni
-000004c0: 6e67 7320 746f 2073 7464 6f75 742c 2068  ngs to stdout, h
-000004d0: 6f77 6576 6572 0a74 6865 2062 6568 6176  owever.the behav
-000004e0: 696f 7572 2063 616e 2062 6520 6368 616e  iour can be chan
-000004f0: 6765 6420 6279 2075 7369 6e67 2074 6861  ged by using tha
-00000500: 7420 6d6f 6475 6c65 2e0a 2222 220a 2320  t module..""".# 
-00000510: 7079 6c69 6e74 3a20 6469 7361 626c 653d  pylint: disable=
-00000520: 746f 6f2d 6d61 6e79 2d6c 696e 6573 0a69  too-many-lines.i
-00000530: 6d70 6f72 7420 7379 730a 696d 706f 7274  mport sys.import
-00000540: 206f 730a 696d 706f 7274 2073 6f63 6b65   os.import socke
-00000550: 740a 696d 706f 7274 2073 736c 0a69 6d70  t.import ssl.imp
-00000560: 6f72 7420 7374 7275 6374 0a69 6d70 6f72  ort struct.impor
-00000570: 7420 7575 6964 0a69 6d70 6f72 7420 6461  t uuid.import da
-00000580: 7465 7469 6d65 0a69 6d70 6f72 7420 7061  tetime.import pa
-00000590: 7468 6c69 620a 696d 706f 7274 2064 6563  thlib.import dec
-000005a0: 696d 616c 0a69 6d70 6f72 7420 6970 6164  imal.import ipad
-000005b0: 6472 6573 730a 696d 706f 7274 2063 6f6e  dress.import con
-000005c0: 6669 6770 6172 7365 720a 696d 706f 7274  figparser.import
-000005d0: 2072 650a 696d 706f 7274 206c 6f67 6769   re.import loggi
-000005e0: 6e67 0a66 726f 6d20 7761 726e 696e 6773  ng.from warnings
-000005f0: 2069 6d70 6f72 7420 7761 726e 0a66 726f   import warn.fro
-00000600: 6d20 7469 6d65 2069 6d70 6f72 7420 736c  m time import sl
-00000610: 6565 702c 2074 696d 655f 6e73 0a66 726f  eep, time_ns.fro
-00000620: 6d20 636f 6c6c 6563 7469 6f6e 7320 696d  m collections im
-00000630: 706f 7274 206e 616d 6564 7475 706c 650a  port namedtuple.
-00000640: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
-00000650: 7274 204f 7074 696f 6e61 6c2c 204e 6577  rt Optional, New
-00000660: 5479 7065 2c20 5475 706c 652c 2043 616c  Type, Tuple, Cal
-00000670: 6c61 626c 652c 204e 616d 6564 5475 706c  lable, NamedTupl
-00000680: 652c 2041 6e79 2c20 5479 7065 2c20 4c69  e, Any, Type, Li
-00000690: 7374 0a66 726f 6d20 6d61 7468 2069 6d70  st.from math imp
-000006a0: 6f72 7420 6973 696e 660a 696d 706f 7274  ort isinf.import
-000006b0: 2064 736e 7061 7273 650a 0a66 726f 6d20   dsnparse..from 
-000006c0: 6372 7970 746f 6772 6170 6879 2e68 617a  cryptography.haz
-000006d0: 6d61 742e 7072 696d 6974 6976 6573 2069  mat.primitives i
-000006e0: 6d70 6f72 7420 6861 7368 6573 2c20 686d  mport hashes, hm
-000006f0: 6163 0a66 726f 6d20 6372 7970 746f 6772  ac.from cryptogr
-00000700: 6170 6879 2e68 617a 6d61 742e 7072 696d  aphy.hazmat.prim
-00000710: 6974 6976 6573 2e73 6572 6961 6c69 7a61  itives.serializa
-00000720: 7469 6f6e 2069 6d70 6f72 7420 6c6f 6164  tion import load
-00000730: 5f70 656d 5f70 7562 6c69 635f 6b65 790a  _pem_public_key.
-00000740: 6672 6f6d 2063 7279 7074 6f67 7261 7068  from cryptograph
-00000750: 792e 6861 7a6d 6174 2e70 7269 6d69 7469  y.hazmat.primiti
-00000760: 7665 732e 6369 7068 6572 7320 696d 706f  ves.ciphers impo
-00000770: 7274 2043 6970 6865 722c 2061 6c67 6f72  rt Cipher, algor
-00000780: 6974 686d 732c 206d 6f64 6573 0a66 726f  ithms, modes.fro
-00000790: 6d20 6372 7970 746f 6772 6170 6879 2e68  m cryptography.h
-000007a0: 617a 6d61 742e 7072 696d 6974 6976 6573  azmat.primitives
-000007b0: 2069 6d70 6f72 7420 7365 7269 616c 697a   import serializ
-000007c0: 6174 696f 6e0a 6672 6f6d 2063 7279 7074  ation.from crypt
-000007d0: 6f67 7261 7068 792e 6861 7a6d 6174 2e70  ography.hazmat.p
-000007e0: 7269 6d69 7469 7665 7320 696d 706f 7274  rimitives import
-000007f0: 2070 6164 6469 6e67 0a66 726f 6d20 6372   padding.from cr
-00000800: 7970 746f 6772 6170 6879 2e68 617a 6d61  yptography.hazma
-00000810: 742e 6261 636b 656e 6473 2069 6d70 6f72  t.backends impor
-00000820: 7420 6465 6661 756c 745f 6261 636b 656e  t default_backen
-00000830: 640a 0a6c 6f67 6765 7220 3d20 6c6f 6767  d..logger = logg
-00000840: 696e 672e 6765 744c 6f67 6765 7228 2270  ing.getLogger("p
-00000850: 796f 6369 656e 7422 290a 0a23 2053 6565  yocient")..# See
-00000860: 2050 4550 2032 3439 2066 6f72 2074 6865   PEP 249 for the
-00000870: 2076 616c 7565 7320 6f66 2074 6865 7365   values of these
-00000880: 2061 7474 7269 6275 7465 730a 6170 696c   attributes.apil
-00000890: 6576 656c 203d 2022 322e 3022 2020 2320  evel = "2.0"  # 
-000008a0: 7079 6c69 6e74 3a20 6469 7361 626c 653d  pylint: disable=
-000008b0: 696e 7661 6c69 642d 6e61 6d65 0a74 6872  invalid-name.thr
-000008c0: 6561 6473 6166 6574 7920 3d20 3120 2023  eadsafety = 1  #
-000008d0: 2070 796c 696e 743a 2064 6973 6162 6c65   pylint: disable
-000008e0: 3d69 6e76 616c 6964 2d6e 616d 650a 7061  =invalid-name.pa
-000008f0: 7261 6d73 7479 6c65 203d 2022 7079 666f  ramstyle = "pyfo
-00000900: 726d 6174 2220 2023 2070 796c 696e 743a  rmat"  # pylint:
-00000910: 2064 6973 6162 6c65 3d69 6e76 616c 6964   disable=invalid
-00000920: 2d6e 616d 650a 4452 4956 4552 5f49 4420  -name.DRIVER_ID 
-00000930: 3d20 2270 796f 6369 656e 7422 0a50 524f  = "pyocient".PRO
-00000940: 544f 434f 4c5f 5645 5253 494f 4e20 3d20  TOCOL_VERSION = 
-00000950: 2237 2e30 2e31 220a 5345 5353 494f 4e5f  "7.0.1".SESSION_
-00000960: 4558 5049 5245 445f 434f 4445 203d 202d  EXPIRED_CODE = -
-00000970: 3733 330a 0a68 6572 6520 3d20 7061 7468  733..here = path
-00000980: 6c69 622e 5061 7468 285f 5f66 696c 655f  lib.Path(__file_
-00000990: 5f29 2e70 6172 656e 742e 6162 736f 6c75  _).parent.absolu
-000009a0: 7465 2829 0a0a 7665 7273 696f 6e20 3d20  te()..version = 
-000009b0: 7b7d 0a77 6974 6820 6f70 656e 286f 732e  {}.with open(os.
-000009c0: 7061 7468 2e6a 6f69 6e28 6865 7265 2c20  path.join(here, 
-000009d0: 2276 6572 7369 6f6e 2e70 7922 2929 2061  "version.py")) a
-000009e0: 7320 7665 7273 696f 6e5f 6669 6c65 3a0a  s version_file:.
-000009f0: 2020 2020 6578 6563 2876 6572 7369 6f6e      exec(version
-00000a00: 5f66 696c 652e 7265 6164 2829 2c20 7665  _file.read(), ve
-00000a10: 7273 696f 6e29 0a20 2020 2076 6572 7369  rsion).    versi
-00000a20: 6f6e 203d 2076 6572 7369 6f6e 5b22 5f5f  on = version["__
-00000a30: 7665 7273 696f 6e5f 5f22 5d0a 2020 2020  version__"].    
-00000a40: 7061 7274 7320 3d20 7665 7273 696f 6e2e  parts = version.
-00000a50: 7370 6c69 7428 222e 2229 0a20 2020 2076  split(".").    v
-00000a60: 6572 7369 6f6e 5f6d 616a 6f72 203d 2069  ersion_major = i
-00000a70: 6e74 2870 6172 7473 5b30 5d29 0a20 2020  nt(parts[0]).   
-00000a80: 2076 6572 7369 6f6e 5f6d 696e 6f72 203d   version_minor =
-00000a90: 2069 6e74 2870 6172 7473 5b31 5d29 0a0a   int(parts[1])..
-00000aa0: 0a63 6c61 7373 2053 514c 4578 6365 7074  .class SQLExcept
-00000ab0: 696f 6e28 4578 6365 7074 696f 6e29 3a0a  ion(Exception):.
-00000ac0: 2020 2020 2222 2242 6173 6520 6578 6365      """Base exce
-00000ad0: 7074 696f 6e20 666f 7220 616c 6c20 4f63  ption for all Oc
-00000ae0: 6965 6e74 2065 7863 6570 7469 6f6e 732e  ient exceptions.
-00000af0: 0a0a 2020 2020 4174 7472 6962 7574 6573  ..    Attributes
-00000b00: 3a0a 0a20 2020 202d 2073 716c 5f73 7461  :..    - sql_sta
-00000b10: 7465 3a20 5468 6520 5351 4c53 5441 5445  te: The SQLSTATE
-00000b20: 2064 6566 696e 6564 2069 6e20 7468 6520   defined in the 
-00000b30: 5351 4c20 7374 616e 6461 7264 0a20 2020  SQL standard.   
-00000b40: 202d 2072 6561 736f 6e3a 2041 2073 7472   - reason: A str
-00000b50: 696e 6720 6465 7363 7269 7074 696f 6e20  ing description 
-00000b60: 6f66 2074 6865 2065 7863 6570 7469 6f6e  of the exception
-00000b70: 0a20 2020 202d 2076 656e 646f 725f 636f  .    - vendor_co
-00000b80: 6465 3a20 416e 204f 6369 656e 7420 7370  de: An Ocient sp
-00000b90: 6563 6966 6963 2065 7272 6f72 2063 6f64  ecific error cod
-00000ba0: 650a 2020 2020 2222 220a 0a20 2020 2064  e.    """..    d
-00000bb0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00000bc0: 2c20 7265 6173 6f6e 3d22 222c 2073 716c  , reason="", sql
-00000bd0: 5f73 7461 7465 3d22 3030 3030 3022 2c20  _state="00000", 
-00000be0: 7665 6e64 6f72 5f63 6f64 653d 3029 3a0a  vendor_code=0):.
-00000bf0: 2020 2020 2020 2020 7375 7065 7228 292e          super().
-00000c00: 5f5f 696e 6974 5f5f 2829 0a20 2020 2020  __init__().     
-00000c10: 2020 2073 656c 662e 7371 6c5f 7374 6174     self.sql_stat
-00000c20: 6520 3d20 7371 6c5f 7374 6174 650a 2020  e = sql_state.  
-00000c30: 2020 2020 2020 7365 6c66 2e72 6561 736f        self.reaso
-00000c40: 6e20 3d20 7265 6173 6f6e 0a20 2020 2020  n = reason.     
-00000c50: 2020 2073 656c 662e 7665 6e64 6f72 5f63     self.vendor_c
-00000c60: 6f64 6520 3d20 7665 6e64 6f72 5f63 6f64  ode = vendor_cod
-00000c70: 650a 0a20 2020 2064 6566 205f 5f73 7472  e..    def __str
-00000c80: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
-00000c90: 2020 7265 7475 726e 2066 2253 7461 7465    return f"State
-00000ca0: 3a20 7b73 656c 662e 7371 6c5f 7374 6174  : {self.sql_stat
-00000cb0: 657d 2043 6f64 653a 207b 7365 6c66 2e76  e} Code: {self.v
-00000cc0: 656e 646f 725f 636f 6465 7d20 5265 6173  endor_code} Reas
-00000cd0: 6f6e 3a20 7b73 656c 662e 7265 6173 6f6e  on: {self.reason
-00000ce0: 7d22 0a0a 0a23 2323 2323 2323 2323 2323  }"...###########
-00000cf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000d00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000d10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000d20: 2323 2323 2323 2323 2323 2323 2323 0a23  ##############.#
-00000d30: 2044 6174 6162 6173 6520 4150 4920 322e   Database API 2.
-00000d40: 3020 6578 6365 7074 696f 6e73 2e20 2054  0 exceptions.  T
-00000d50: 6865 7365 2061 7265 2072 6571 7569 7265  hese are require
-00000d60: 6420 6279 2050 454d 2032 3439 0a23 2323  d by PEM 249.###
-00000d70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000d80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000d90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000da0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000db0: 2323 2323 2323 0a0a 0a63 6c61 7373 2045  ######...class E
-00000dc0: 7272 6f72 2853 514c 4578 6365 7074 696f  rror(SQLExceptio
-00000dd0: 6e29 3a0a 2020 2020 2222 2245 7863 6570  n):.    """Excep
-00000de0: 7469 6f6e 2074 6861 7420 6973 2074 6865  tion that is the
-00000df0: 2062 6173 6520 636c 6173 7320 6f66 2061   base class of a
-00000e00: 6c6c 206f 7468 6572 2065 7272 6f72 2065  ll other error e
-00000e10: 7863 6570 7469 6f6e 732e 2222 220a 0a20  xceptions.""".. 
-00000e20: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00000e30: 7365 6c66 2c20 7265 6173 6f6e 2c20 7371  self, reason, sq
-00000e40: 6c5f 7374 6174 653d 2235 3830 3035 222c  l_state="58005",
-00000e50: 2076 656e 646f 725f 636f 6465 3d2d 3130   vendor_code=-10
-00000e60: 3029 3a0a 2020 2020 2020 2020 7375 7065  0):.        supe
-00000e70: 7228 292e 5f5f 696e 6974 5f5f 2872 6561  r().__init__(rea
-00000e80: 736f 6e2c 2073 716c 5f73 7461 7465 3d73  son, sql_state=s
-00000e90: 716c 5f73 7461 7465 2c20 7665 6e64 6f72  ql_state, vendor
-00000ea0: 5f63 6f64 653d 7665 6e64 6f72 5f63 6f64  _code=vendor_cod
-00000eb0: 6529 0a0a 0a63 6c61 7373 2057 6172 6e69  e)...class Warni
-00000ec0: 6e67 2853 514c 4578 6365 7074 696f 6e29  ng(SQLException)
-00000ed0: 3a20 2023 2070 796c 696e 743a 2064 6973  :  # pylint: dis
-00000ee0: 6162 6c65 3d72 6564 6566 696e 6564 2d62  able=redefined-b
-00000ef0: 7569 6c74 696e 0a20 2020 2022 2222 4578  uiltin.    """Ex
-00000f00: 6365 7074 696f 6e20 7468 6174 2069 7320  ception that is 
-00000f10: 7468 6520 6261 7365 2063 6c61 7373 206f  the base class o
-00000f20: 6620 616c 6c20 6f74 6865 7220 7761 726e  f all other warn
-00000f30: 696e 6720 6578 6365 7074 696f 6e73 2e22  ing exceptions."
-00000f40: 2222 0a0a 0a63 6c61 7373 2049 6e74 6572  ""...class Inter
-00000f50: 6661 6365 4572 726f 7228 4572 726f 7229  faceError(Error)
-00000f60: 3a0a 2020 2020 2222 2245 7863 6570 7469  :.    """Excepti
-00000f70: 6f6e 2072 6169 7365 6420 666f 7220 6572  on raised for er
-00000f80: 726f 7273 2074 6861 7420 6172 6520 7265  rors that are re
-00000f90: 6c61 7465 6420 746f 2074 6865 0a20 2020  lated to the.   
-00000fa0: 2064 6174 6162 6173 6520 696e 7465 7266   database interf
-00000fb0: 6163 6520 7261 7468 6572 2074 6861 6e20  ace rather than 
-00000fc0: 7468 6520 6461 7461 6261 7365 2069 7473  the database its
-00000fd0: 656c 662e 0a20 2020 2022 2222 0a0a 0a63  elf..    """...c
-00000fe0: 6c61 7373 2044 6174 6162 6173 6545 7272  lass DatabaseErr
-00000ff0: 6f72 2845 7272 6f72 293a 0a20 2020 2022  or(Error):.    "
-00001000: 2222 4578 6365 7074 696f 6e20 7261 6973  ""Exception rais
-00001010: 6564 2066 6f72 2065 7272 6f72 7320 7468  ed for errors th
-00001020: 6174 2061 7265 2072 656c 6174 6564 2074  at are related t
-00001030: 6f20 7468 6520 6461 7461 6261 7365 2e22  o the database."
-00001040: 2222 0a0a 0a63 6c61 7373 2049 6e74 6572  ""...class Inter
-00001050: 6e61 6c45 7272 6f72 2844 6174 6162 6173  nalError(Databas
-00001060: 6545 7272 6f72 293a 0a20 2020 2022 2222  eError):.    """
-00001070: 4578 6365 7074 696f 6e20 7261 6973 6564  Exception raised
-00001080: 2077 6865 6e20 7468 6520 6461 7461 6261   when the databa
-00001090: 7365 2065 6e63 6f75 6e74 6572 7320 616e  se encounters an
-000010a0: 2069 6e74 6572 6e61 6c20 6572 726f 722c   internal error,
-000010b0: 0a20 2020 2065 2e67 2e20 7468 6520 6375  .    e.g. the cu
-000010c0: 7273 6f72 2069 7320 6e6f 7420 7661 6c69  rsor is not vali
-000010d0: 6420 616e 796d 6f72 650a 2020 2020 2222  d anymore.    ""
-000010e0: 220a 0a0a 636c 6173 7320 4f70 6572 6174  "...class Operat
-000010f0: 696f 6e61 6c45 7272 6f72 2844 6174 6162  ionalError(Datab
-00001100: 6173 6545 7272 6f72 293a 0a20 2020 2022  aseError):.    "
-00001110: 2222 4578 6365 7074 696f 6e20 7261 6973  ""Exception rais
-00001120: 6564 2066 6f72 2065 7272 6f72 7320 7468  ed for errors th
-00001130: 6174 2061 7265 2072 656c 6174 6564 2074  at are related t
-00001140: 6f20 7468 6520 6461 7461 6261 7365 2773  o the database's
-00001150: 0a20 2020 206f 7065 7261 7469 6f6e 2061  .    operation a
-00001160: 6e64 206e 6f74 206e 6563 6573 7361 7269  nd not necessari
-00001170: 6c79 2075 6e64 6572 2074 6865 2063 6f6e  ly under the con
-00001180: 7472 6f6c 206f 6620 7468 6520 7072 6f67  trol of the prog
-00001190: 7261 6d6d 6572 2c0a 2020 2020 652e 672e  rammer,.    e.g.
-000011a0: 2061 6e20 756e 6578 7065 6374 6564 2064   an unexpected d
-000011b0: 6973 636f 6e6e 6563 7420 6f63 6375 7273  isconnect occurs
-000011c0: 2c20 7468 6520 6461 7461 2073 6f75 7263  , the data sourc
-000011d0: 6520 6e61 6d65 2069 7320 6e6f 7420 666f  e name is not fo
-000011e0: 756e 642e 0a20 2020 2022 2222 0a0a 0a63  und..    """...c
-000011f0: 6c61 7373 2050 726f 6772 616d 6d69 6e67  lass Programming
-00001200: 4572 726f 7228 4461 7461 6261 7365 4572  Error(DatabaseEr
-00001210: 726f 7229 3a0a 2020 2020 2222 2245 7863  ror):.    """Exc
-00001220: 6570 7469 6f6e 2072 6169 7365 6420 666f  eption raised fo
-00001230: 7220 7072 6f67 7261 6d6d 696e 6720 6572  r programming er
-00001240: 726f 7273 2c20 652e 672e 2074 6162 6c65  rors, e.g. table
-00001250: 206e 6f74 2066 6f75 6e64 2c0a 2020 2020   not found,.    
-00001260: 7379 6e74 6178 2065 7272 6f72 2069 6e20  syntax error in 
-00001270: 7468 6520 5351 4c20 7374 6174 656d 656e  the SQL statemen
-00001280: 742c 2077 726f 6e67 206e 756d 6265 7220  t, wrong number 
-00001290: 6f66 2070 6172 616d 6574 6572 730a 2020  of parameters.  
-000012a0: 2020 7370 6563 6966 6965 642c 2065 7463    specified, etc
-000012b0: 2e0a 2020 2020 2222 220a 0a0a 636c 6173  ..    """...clas
-000012c0: 7320 496e 7465 6772 6974 7945 7272 6f72  s IntegrityError
-000012d0: 2844 6174 6162 6173 6545 7272 6f72 293a  (DatabaseError):
-000012e0: 0a20 2020 2022 2222 4578 6365 7074 696f  .    """Exceptio
-000012f0: 6e20 7261 6973 6564 2077 6865 6e20 7468  n raised when th
-00001300: 6520 7265 6c61 7469 6f6e 616c 2069 6e74  e relational int
-00001310: 6567 7269 7479 206f 6620 7468 6520 6461  egrity of the da
-00001320: 7461 6261 7365 0a20 2020 2069 7320 6166  tabase.    is af
-00001330: 6665 6374 6564 2c20 652e 672e 2061 2066  fected, e.g. a f
-00001340: 6f72 6569 676e 206b 6579 2063 6865 636b  oreign key check
-00001350: 2066 6169 6c73 0a20 2020 2022 2222 0a0a   fails.    """..
-00001360: 0a63 6c61 7373 2044 6174 6145 7272 6f72  .class DataError
-00001370: 2844 6174 6162 6173 6545 7272 6f72 293a  (DatabaseError):
-00001380: 0a20 2020 2022 2222 4578 6365 7074 696f  .    """Exceptio
-00001390: 6e20 7261 6973 6564 2066 6f72 2065 7272  n raised for err
-000013a0: 6f72 7320 7468 6174 2061 7265 2064 7565  ors that are due
-000013b0: 2074 6f20 7072 6f62 6c65 6d73 2077 6974   to problems wit
-000013c0: 6820 7468 650a 2020 2020 7072 6f63 6573  h the.    proces
-000013d0: 7365 6420 6461 7461 206c 696b 6520 6469  sed data like di
-000013e0: 7669 7369 6f6e 2062 7920 7a65 726f 2c20  vision by zero, 
-000013f0: 6e75 6d65 7269 6320 7661 6c75 6520 6f75  numeric value ou
-00001400: 7420 6f66 2072 616e 6765 2c20 6574 632e  t of range, etc.
-00001410: 0a20 2020 2022 2222 0a0a 0a63 6c61 7373  .    """...class
-00001420: 204e 6f74 5375 7070 6f72 7465 6445 7272   NotSupportedErr
-00001430: 6f72 2844 6174 6162 6173 6545 7272 6f72  or(DatabaseError
-00001440: 293a 0a20 2020 2022 2222 4578 6365 7074  ):.    """Except
-00001450: 696f 6e20 7261 6973 6564 2069 6e20 6361  ion raised in ca
-00001460: 7365 2061 206d 6574 686f 6420 6f72 2064  se a method or d
-00001470: 6174 6162 6173 6520 4150 4920 7761 7320  atabase API was 
-00001480: 7573 6564 2077 6869 6368 2069 7320 6e6f  used which is no
-00001490: 740a 2020 2020 7375 7070 6f72 7465 6420  t.    supported 
-000014a0: 6279 2074 6865 2064 6174 6162 6173 650a  by the database.
-000014b0: 2020 2020 2222 220a 0a0a 636c 6173 7320      """...class 
-000014c0: 4d61 6c66 6f72 6d65 6455 524c 2844 6174  MalformedURL(Dat
-000014d0: 6162 6173 6545 7272 6f72 293a 0a20 2020  abaseError):.   
-000014e0: 2022 2222 4578 6365 7074 696f 6e20 7261   """Exception ra
-000014f0: 6973 6564 2069 6e20 6361 7365 2061 206d  ised in case a m
-00001500: 616c 666f 726d 6564 2044 534e 2069 7320  alformed DSN is 
-00001510: 7265 6365 6976 6564 2222 220a 0a20 2020  received"""..   
-00001520: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00001530: 6c66 2c20 7265 6173 6f6e 293a 0a20 2020  lf, reason):.   
-00001540: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
-00001550: 6e69 745f 5f28 7371 6c5f 7374 6174 653d  nit__(sql_state=
-00001560: 2230 3830 3031 222c 2076 656e 646f 725f  "08001", vendor_
-00001570: 636f 6465 3d2d 3230 302c 2072 6561 736f  code=-200, reaso
-00001580: 6e3d 7265 6173 6f6e 290a 0a0a 636c 6173  n=reason)...clas
-00001590: 7320 5379 6e74 6178 4572 726f 7228 5072  s SyntaxError(Pr
-000015a0: 6f67 7261 6d6d 696e 6745 7272 6f72 293a  ogrammingError):
-000015b0: 0a20 2020 2022 2222 4578 6365 7074 696f  .    """Exceptio
-000015c0: 6e20 7261 6973 6564 2069 6e20 6361 7365  n raised in case
-000015d0: 2061 206d 616c 666f 726d 6564 2044 534e   a malformed DSN
-000015e0: 2069 7320 7265 6365 6976 6564 2222 220a   is received""".
-000015f0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00001600: 5f28 7365 6c66 2c20 7265 6173 6f6e 293a  _(self, reason):
-00001610: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
-00001620: 2e5f 5f69 6e69 745f 5f28 7371 6c5f 7374  .__init__(sql_st
-00001630: 6174 653d 2234 3236 3031 222c 2076 656e  ate="42601", ven
-00001640: 646f 725f 636f 6465 3d2d 3530 302c 2072  dor_code=-500, r
-00001650: 6561 736f 6e3d 7265 6173 6f6e 290a 0a0a  eason=reason)...
-00001660: 636c 6173 7320 5479 7065 436f 6465 733a  class TypeCodes:
-00001670: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
-00001680: 626c 653d 746f 6f2d 6665 772d 7075 626c  ble=too-few-publ
-00001690: 6963 2d6d 6574 686f 6473 0a20 2020 2022  ic-methods.    "
-000016a0: 2222 0a20 2020 2044 6174 6162 6173 6520  "".    Database 
-000016b0: 636f 6c75 6d6e 2074 7970 6520 636f 6465  column type code
-000016c0: 730a 0a20 2020 203a 6d65 7461 2070 7269  s..    :meta pri
-000016d0: 7661 7465 3a0a 2020 2020 2222 220a 0a20  vate:.    """.. 
-000016e0: 2020 2044 454d 203d 2030 0a20 2020 2049     DEM = 0.    I
-000016f0: 4e54 203d 2031 0a20 2020 204c 4f4e 4720  NT = 1.    LONG 
-00001700: 3d20 320a 2020 2020 464c 4f41 5420 3d20  = 2.    FLOAT = 
-00001710: 330a 2020 2020 444f 5542 4c45 203d 2034  3.    DOUBLE = 4
-00001720: 0a20 2020 2053 5452 494e 4720 3d20 350a  .    STRING = 5.
-00001730: 2020 2020 4348 4152 203d 2035 0a20 2020      CHAR = 5.   
-00001740: 2054 494d 4553 5441 4d50 203d 2036 0a20   TIMESTAMP = 6. 
-00001750: 2020 204e 554c 4c20 3d20 370a 2020 2020     NULL = 7.    
-00001760: 424f 4f4c 4541 4e20 3d20 380a 2020 2020  BOOLEAN = 8.    
-00001770: 4249 4e41 5259 203d 2039 0a20 2020 2042  BINARY = 9.    B
-00001780: 5954 4520 3d20 3130 0a20 2020 2053 484f  YTE = 10.    SHO
-00001790: 5254 203d 2031 310a 2020 2020 5449 4d45  RT = 11.    TIME
-000017a0: 203d 2031 320a 2020 2020 4445 4349 4d41   = 12.    DECIMA
-000017b0: 4c20 3d20 3133 0a20 2020 2041 5252 4159  L = 13.    ARRAY
-000017c0: 203d 2031 340a 2020 2020 5555 4944 203d   = 14.    UUID =
-000017d0: 2031 350a 2020 2020 5354 5f50 4f49 4e54   15.    ST_POINT
-000017e0: 203d 2031 360a 2020 2020 4950 203d 2031   = 16.    IP = 1
-000017f0: 370a 2020 2020 4950 5634 203d 2031 380a  7.    IPV4 = 18.
-00001800: 2020 2020 4441 5445 203d 2031 390a 2020      DATE = 19.  
-00001810: 2020 5449 4d45 5354 414d 505f 4e41 4e4f    TIMESTAMP_NANO
-00001820: 5320 3d20 3230 0a20 2020 2054 494d 455f  S = 20.    TIME_
-00001830: 4e41 4e4f 5320 3d20 3231 0a20 2020 2054  NANOS = 21.    T
-00001840: 5550 4c45 203d 2032 320a 2020 2020 5354  UPLE = 22.    ST
-00001850: 5f4c 494e 4553 5452 494e 4720 3d20 3233  _LINESTRING = 23
-00001860: 0a20 2020 2053 545f 504f 4c59 474f 4e20  .    ST_POLYGON 
-00001870: 3d20 3234 0a0a 2020 2020 4063 6c61 7373  = 24..    @class
-00001880: 6d65 7468 6f64 0a20 2020 2064 6566 2074  method.    def t
-00001890: 6f5f 7479 7065 2863 6c73 2c20 7479 7065  o_type(cls, type
-000018a0: 7374 7229 3a0a 2020 2020 2020 2020 2222  str):.        ""
-000018b0: 2247 6976 656e 2061 2073 7472 696e 6720  "Given a string 
-000018c0: 7479 7065 2c20 7265 7475 726e 2069 7473  type, return its
-000018d0: 2074 7970 6520 636f 6465 2222 220a 2020   type code""".  
-000018e0: 2020 2020 2020 6966 2068 6173 6174 7472        if hasattr
-000018f0: 2863 6c73 2c20 7479 7065 7374 7229 3a0a  (cls, typestr):.
-00001900: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00001910: 726e 2067 6574 6174 7472 2863 6c73 2c20  rn getattr(cls, 
-00001920: 7479 7065 7374 7229 0a20 2020 2020 2020  typestr).       
-00001930: 2072 6169 7365 2045 7272 6f72 2866 2255   raise Error(f"U
-00001940: 6e6b 6e6f 776e 2063 6f6c 756d 6e20 7479  nknown column ty
-00001950: 7065 207b 7374 727d 2229 0a0a 2020 2020  pe {str}")..    
-00001960: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
-00001970: 2064 6566 2063 6c73 5f74 6f5f 7479 7065   def cls_to_type
-00001980: 2863 6c73 2c20 7063 6c61 7373 293a 0a20  (cls, pclass):. 
-00001990: 2020 2020 2020 2069 6620 7063 6c61 7373         if pclass
-000019a0: 203d 3d20 7374 723a 0a20 2020 2020 2020   == str:.       
-000019b0: 2020 2020 2072 6574 7572 6e20 636c 732e       return cls.
-000019c0: 5354 5249 4e47 0a20 2020 2020 2020 2065  STRING.        e
-000019d0: 6c69 6620 7063 6c61 7373 203d 3d20 696e  lif pclass == in
-000019e0: 743a 0a20 2020 2020 2020 2020 2020 2072  t:.            r
-000019f0: 6574 7572 6e20 636c 732e 494e 540a 2020  eturn cls.INT.  
-00001a00: 2020 2020 2020 656c 6966 2070 636c 6173        elif pclas
-00001a10: 7320 3d3d 2066 6c6f 6174 3a0a 2020 2020  s == float:.    
-00001a20: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-00001a30: 6c73 2e46 4c4f 4154 0a20 2020 2020 2020  ls.FLOAT.       
-00001a40: 2065 6c69 6620 7063 6c61 7373 203d 3d20   elif pclass == 
-00001a50: 7575 6964 2e55 5549 443a 0a20 2020 2020  uuid.UUID:.     
-00001a60: 2020 2020 2020 2072 6574 7572 6e20 636c         return cl
-00001a70: 732e 5555 4944 0a20 2020 2020 2020 2065  s.UUID.        e
-00001a80: 6c69 6620 7063 6c61 7373 203d 3d20 4f70  lif pclass == Op
-00001a90: 7469 6f6e 616c 5b75 7569 642e 5555 4944  tional[uuid.UUID
-00001aa0: 5d3a 0a20 2020 2020 2020 2020 2020 2072  ]:.            r
-00001ab0: 6574 7572 6e20 636c 732e 5555 4944 0a20  eturn cls.UUID. 
-00001ac0: 2020 2020 2020 2072 6169 7365 2045 7272         raise Err
-00001ad0: 6f72 2866 2255 6e6b 6e6f 776e 2063 6f6c  or(f"Unknown col
-00001ae0: 756d 6e20 636c 6173 7320 7b70 636c 6173  umn class {pclas
-00001af0: 737d 2229 0a0a 0a23 2042 7920 696e 7374  s}")...# By inst
-00001b00: 616e 7469 6174 696e 6720 7468 6573 6520  antiating these 
-00001b10: 6865 7265 2077 6520 7265 6475 6365 2074  here we reduce t
-00001b20: 6865 206f 7665 7268 6561 6420 6f66 2073  he overhead of s
-00001b30: 6574 7469 6e67 2074 6869 7320 7570 0a23  etting this up.#
-00001b40: 2065 6163 6820 7469 6d65 2077 6520 6361   each time we ca
-00001b50: 6c6c 2069 740a 5f75 6e70 6163 6b5f 7368  ll it._unpack_sh
-00001b60: 6f72 7420 3d20 7374 7275 6374 2e53 7472  ort = struct.Str
-00001b70: 7563 7428 2221 6822 292e 756e 7061 636b  uct("!h").unpack
-00001b80: 5f66 726f 6d0a 5f75 6e70 6163 6b5f 696e  _from._unpack_in
-00001b90: 7420 3d20 7374 7275 6374 2e53 7472 7563  t = struct.Struc
-00001ba0: 7428 2221 6922 292e 756e 7061 636b 5f66  t("!i").unpack_f
-00001bb0: 726f 6d0a 5f75 6e70 6163 6b5f 6c6f 6e67  rom._unpack_long
-00001bc0: 203d 2073 7472 7563 742e 5374 7275 6374   = struct.Struct
-00001bd0: 2822 2171 2229 2e75 6e70 6163 6b5f 6672  ("!q").unpack_fr
-00001be0: 6f6d 0a5f 756e 7061 636b 5f66 6c6f 6174  om._unpack_float
-00001bf0: 203d 2073 7472 7563 742e 5374 7275 6374   = struct.Struct
-00001c00: 2822 2166 2229 2e75 6e70 6163 6b5f 6672  ("!f").unpack_fr
-00001c10: 6f6d 0a5f 756e 7061 636b 5f64 6f75 626c  om._unpack_doubl
-00001c20: 6520 3d20 7374 7275 6374 2e53 7472 7563  e = struct.Struc
-00001c30: 7428 2221 6422 292e 756e 7061 636b 5f66  t("!d").unpack_f
-00001c40: 726f 6d0a 5f75 6e70 6163 6b5f 626f 6f6c  rom._unpack_bool
-00001c50: 203d 2073 7472 7563 742e 5374 7275 6374   = struct.Struct
-00001c60: 2822 3f22 292e 756e 7061 636b 5f66 726f  ("?").unpack_fro
-00001c70: 6d0a 5f75 6e70 6163 6b5f 6368 6172 203d  m._unpack_char =
-00001c80: 2073 7472 7563 742e 5374 7275 6374 2822   struct.Struct("
-00001c90: 6322 292e 756e 7061 636b 5f66 726f 6d0a  c").unpack_from.
-00001ca0: 0a23 2065 6173 7920 636f 6e76 6572 7369  .# easy conversi
-00001cb0: 6f6e 7320 7765 2063 616e 2064 6f20 7769  ons we can do wi
-00001cc0: 7468 2073 7472 7563 7473 0a5f 7479 7065  th structs._type
-00001cd0: 5f6d 6170 203d 207b 0a20 2020 2054 7970  _map = {.    Typ
-00001ce0: 6543 6f64 6573 2e49 4e54 3a20 2873 7472  eCodes.INT: (str
-00001cf0: 7563 742e 6361 6c63 7369 7a65 2822 2169  uct.calcsize("!i
-00001d00: 2229 2c20 5f75 6e70 6163 6b5f 696e 7429  "), _unpack_int)
-00001d10: 2c0a 2020 2020 5479 7065 436f 6465 732e  ,.    TypeCodes.
-00001d20: 4c4f 4e47 3a20 2873 7472 7563 742e 6361  LONG: (struct.ca
-00001d30: 6c63 7369 7a65 2822 2171 2229 2c20 5f75  lcsize("!q"), _u
-00001d40: 6e70 6163 6b5f 6c6f 6e67 292c 0a20 2020  npack_long),.   
-00001d50: 2054 7970 6543 6f64 6573 2e46 4c4f 4154   TypeCodes.FLOAT
-00001d60: 3a20 2873 7472 7563 742e 6361 6c63 7369  : (struct.calcsi
-00001d70: 7a65 2822 2166 2229 2c20 5f75 6e70 6163  ze("!f"), _unpac
-00001d80: 6b5f 666c 6f61 7429 2c0a 2020 2020 5479  k_float),.    Ty
-00001d90: 7065 436f 6465 732e 444f 5542 4c45 3a20  peCodes.DOUBLE: 
-00001da0: 2873 7472 7563 742e 6361 6c63 7369 7a65  (struct.calcsize
-00001db0: 2822 2164 2229 2c20 5f75 6e70 6163 6b5f  ("!d"), _unpack_
-00001dc0: 646f 7562 6c65 292c 0a20 2020 2054 7970  double),.    Typ
-00001dd0: 6543 6f64 6573 2e42 4f4f 4c45 414e 3a20  eCodes.BOOLEAN: 
-00001de0: 2873 7472 7563 742e 6361 6c63 7369 7a65  (struct.calcsize
-00001df0: 2822 3f22 292c 205f 756e 7061 636b 5f62  ("?"), _unpack_b
-00001e00: 6f6f 6c29 2c0a 2020 2020 5479 7065 436f  ool),.    TypeCo
-00001e10: 6465 732e 5348 4f52 543a 2028 7374 7275  des.SHORT: (stru
-00001e20: 6374 2e63 616c 6373 697a 6528 2221 6822  ct.calcsize("!h"
-00001e30: 292c 205f 756e 7061 636b 5f73 686f 7274  ), _unpack_short
-00001e40: 292c 0a7d 0a0a 0a23 2323 2323 2323 2323  ),.}...#########
-00001e50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001e60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001e70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001e80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001e90: 0a23 2044 6174 6162 6173 6520 4150 4920  .# Database API 
-00001ea0: 322e 3020 7479 7065 732e 2020 5468 6573  2.0 types.  Thes
-00001eb0: 6520 6172 6520 7265 7175 6972 6564 2062  e are required b
-00001ec0: 7920 5045 4d20 3234 390a 2323 2323 2323  y PEM 249.######
-00001ed0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001ee0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001ef0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001f00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001f10: 2323 230a 4269 6e61 7279 203d 2062 7974  ###.Binary = byt
-00001f20: 6573 2020 2320 3a20 3a6d 6574 6120 7072  es  # : :meta pr
-00001f30: 6976 6174 653a 0a53 5452 494e 4720 3d20  ivate:.STRING = 
-00001f40: 5479 7065 436f 6465 732e 5354 5249 4e47  TypeCodes.STRING
-00001f50: 2020 2320 3a20 3a6d 6574 6120 7072 6976    # : :meta priv
-00001f60: 6174 653a 0a42 494e 4152 5920 3d20 5479  ate:.BINARY = Ty
-00001f70: 7065 436f 6465 732e 4249 4e41 5259 2020  peCodes.BINARY  
-00001f80: 2320 3a20 3a6d 6574 6120 7072 6976 6174  # : :meta privat
-00001f90: 653a 0a4e 554d 4245 5220 3d20 5479 7065  e:.NUMBER = Type
-00001fa0: 436f 6465 732e 494e 5420 2023 203a 203a  Codes.INT  # : :
-00001fb0: 6d65 7461 2070 7269 7661 7465 3a0a 4441  meta private:.DA
-00001fc0: 5445 5449 4d45 203d 2054 7970 6543 6f64  TETIME = TypeCod
-00001fd0: 6573 2e54 494d 4553 5441 4d50 2020 2320  es.TIMESTAMP  # 
-00001fe0: 3a20 3a6d 6574 6120 7072 6976 6174 653a  : :meta private:
-00001ff0: 0a52 4f57 4944 203d 2054 7970 6543 6f64  .ROWID = TypeCod
-00002000: 6573 2e49 4e54 2020 2320 3a20 3a6d 6574  es.INT  # : :met
-00002010: 6120 7072 6976 6174 653a 0a0a 2323 2323  a private:..####
-00002020: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002030: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002040: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002050: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002060: 2323 2323 230a 2320 496d 706f 7274 206f  #####.# Import o
-00002070: 7572 2067 6f6f 676c 6520 7072 6f74 6f62  ur google protob
-00002080: 7566 206d 6573 7361 6765 2064 6566 696e  uf message defin
-00002090: 6974 696f 6e73 0a23 2057 6520 6173 7375  itions.# We assu
-000020a0: 6d65 2074 6861 7420 7468 6520 436c 6965  me that the Clie
-000020b0: 6e74 5769 7265 5072 6f74 6f63 6f6c 5f70  ntWireProtocol_p
-000020c0: 622e 7079 2066 696c 6520 6973 2069 6e20  b.py file is in 
-000020d0: 7468 6520 7361 6d65 2064 6972 6563 746f  the same directo
-000020e0: 7279 0a23 2061 7320 7468 6973 2066 696c  ry.# as this fil
-000020f0: 650a 2323 2323 2323 2323 2323 2323 2323  e.##############
-00002100: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002110: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002120: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002130: 2323 2323 2323 2323 2323 230a 7379 732e  ###########.sys.
-00002140: 7061 7468 2e61 7070 656e 6428 6f73 2e70  path.append(os.p
-00002150: 6174 682e 6162 7370 6174 6828 6f73 2e70  ath.abspath(os.p
-00002160: 6174 682e 6469 726e 616d 6528 225f 5f66  ath.dirname("__f
-00002170: 696c 655f 5f22 2929 290a 0a23 2054 7279  ile__")))..# Try
-00002180: 2061 6e64 2069 6d70 6f72 7420 6f75 7420   and import out 
-00002190: 7072 6f74 6f62 7566 2064 6566 696e 6974  protobuf definit
-000021a0: 696f 6e73 2e0a 2320 5768 696c 6520 7765  ions..# While we
-000021b0: 2074 7261 6e73 6974 696f 6e20 746f 2062   transition to b
-000021c0: 617a 656c 2077 6520 7761 6e74 2074 6f20  azel we want to 
-000021d0: 7375 7070 6f72 7420 626f 7468 2074 6865  support both the
-000021e0: 206d 616b 6566 696c 6520 7761 7920 616e   makefile way an
-000021f0: 6420 7468 6520 6e65 7720 7761 7920 2844  d the new way (D
-00002200: 422d 3133 3934 3729 0a74 7279 3a0a 2020  B-13947).try:.  
-00002210: 2020 696d 706f 7274 2043 6c69 656e 7457    import ClientW
-00002220: 6972 6550 726f 746f 636f 6c5f 7062 3220  ireProtocol_pb2 
-00002230: 6173 2070 726f 746f 2020 2320 7079 6c69  as proto  # pyli
-00002240: 6e74 3a20 6469 7361 626c 653d 696d 706f  nt: disable=impo
-00002250: 7274 2d65 7272 6f72 2c77 726f 6e67 2d69  rt-error,wrong-i
-00002260: 6d70 6f72 742d 706f 7369 7469 6f6e 0a65  mport-position.e
-00002270: 7863 6570 7420 496d 706f 7274 4572 726f  xcept ImportErro
-00002280: 7220 6173 2065 7863 3a0a 2020 2020 6672  r as exc:.    fr
-00002290: 6f6d 2073 6861 7265 644d 6573 7361 6765  om sharedMessage
-000022a0: 7320 696d 706f 7274 2063 6c69 656e 7457  s import clientW
-000022b0: 6972 6550 726f 746f 636f 6c5f 7062 3220  ireProtocol_pb2 
-000022c0: 6173 2070 726f 746f 2020 2320 7079 6c69  as proto  # pyli
-000022d0: 6e74 3a20 6469 7361 626c 653d 696d 706f  nt: disable=impo
-000022e0: 7274 2d65 7272 6f72 2c77 726f 6e67 2d69  rt-error,wrong-i
-000022f0: 6d70 6f72 742d 706f 7369 7469 6f6e 0a0a  mport-position..
-00002300: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002310: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002320: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002330: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002340: 2323 2323 2323 2323 230a 2320 4c69 6768  #########.# Ligh
-00002350: 7477 6569 6768 7420 4749 5320 636c 6173  tweight GIS clas
-00002360: 7365 730a 2323 2323 2323 2323 2323 2323  ses.############
-00002370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002390: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000023a0: 2323 2323 2323 2323 2323 2323 230a 0a0a  #############...
-000023b0: 636c 6173 7320 5f53 5450 6f69 6e74 3a0a  class _STPoint:.
-000023c0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-000023d0: 2873 656c 662c 206c 6f6e 673a 2066 6c6f  (self, long: flo
-000023e0: 6174 2c20 6c61 743a 2066 6c6f 6174 293a  at, lat: float):
-000023f0: 0a20 2020 2020 2020 2073 656c 662e 6c6f  .        self.lo
-00002400: 6e67 203d 206c 6f6e 670a 2020 2020 2020  ng = long.      
-00002410: 2020 7365 6c66 2e6c 6174 203d 206c 6174    self.lat = lat
-00002420: 0a0a 2020 2020 6465 6620 776b 745f 696e  ..    def wkt_in
-00002430: 6e65 7228 7365 6c66 2920 2d3e 2073 7472  ner(self) -> str
-00002440: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00002450: 2073 7472 2873 656c 662e 6c6f 6e67 2920   str(self.long) 
-00002460: 2b20 2220 2220 2b20 7374 7228 7365 6c66  + " " + str(self
-00002470: 2e6c 6174 290a 0a20 2020 2064 6566 205f  .lat)..    def _
-00002480: 5f72 6570 725f 5f28 7365 6c66 293a 0a20  _repr__(self):. 
-00002490: 2020 2020 2020 2069 6620 6973 696e 6628         if isinf(
-000024a0: 7365 6c66 2e6c 6f6e 6729 206f 7220 6973  self.long) or is
-000024b0: 696e 6628 7365 6c66 2e6c 6174 293a 0a20  inf(self.lat):. 
-000024c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000024d0: 6e20 2250 4f49 4e54 2045 4d50 5459 220a  n "POINT EMPTY".
-000024e0: 2020 2020 2020 2020 7265 7475 726e 2022          return "
-000024f0: 504f 494e 5428 2220 2b20 7365 6c66 2e77  POINT(" + self.w
-00002500: 6b74 5f69 6e6e 6572 2829 202b 2022 2922  kt_inner() + ")"
-00002510: 0a0a 2020 2020 6465 6620 5f5f 6571 5f5f  ..    def __eq__
-00002520: 2873 656c 662c 206f 7468 6572 293a 0a20  (self, other):. 
-00002530: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00002540: 616e 6365 286f 7468 6572 2c20 5f53 5450  ance(other, _STP
-00002550: 6f69 6e74 293a 0a20 2020 2020 2020 2020  oint):.         
-00002560: 2020 2072 6574 7572 6e20 7365 6c66 2e6c     return self.l
-00002570: 6f6e 6720 3d3d 206f 7468 6572 2e6c 6f6e  ong == other.lon
-00002580: 6720 616e 6420 7365 6c66 2e6c 6174 203d  g and self.lat =
-00002590: 3d20 6f74 6865 722e 6c61 740a 2020 2020  = other.lat.    
-000025a0: 2020 2020 7265 7475 726e 204e 6f74 496d      return NotIm
-000025b0: 706c 656d 656e 7465 640a 0a0a 6465 6620  plemented...def 
-000025c0: 5f6c 696e 6573 7472 696e 675f 776b 745f  _linestring_wkt_
-000025d0: 696e 6e65 7228 706f 696e 7473 3a20 4c69  inner(points: Li
-000025e0: 7374 5b5f 5354 506f 696e 745d 2920 2d3e  st[_STPoint]) ->
-000025f0: 2073 7472 3a0a 2020 2020 7265 7475 726e   str:.    return
-00002600: 2022 2822 202b 2022 2c20 222e 6a6f 696e   "(" + ", ".join
-00002610: 2828 702e 776b 745f 696e 6e65 7228 2920  ((p.wkt_inner() 
-00002620: 666f 7220 7020 696e 2070 6f69 6e74 7329  for p in points)
-00002630: 2920 2b20 2229 220a 0a0a 636c 6173 7320  ) + ")"...class 
-00002640: 5f53 544c 696e 6573 7472 696e 673a 0a20  _STLinestring:. 
-00002650: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00002660: 7365 6c66 2c20 706f 696e 7473 3a20 4c69  self, points: Li
-00002670: 7374 5b5f 5354 506f 696e 745d 293a 0a20  st[_STPoint]):. 
-00002680: 2020 2020 2020 2073 656c 662e 706f 696e         self.poin
-00002690: 7473 203d 2070 6f69 6e74 730a 0a20 2020  ts = points..   
-000026a0: 2064 6566 205f 5f72 6570 725f 5f28 7365   def __repr__(se
-000026b0: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
-000026c0: 6e6f 7420 7365 6c66 2e70 6f69 6e74 733a  not self.points:
-000026d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000026e0: 7572 6e20 224c 494e 4553 5452 494e 4720  urn "LINESTRING 
-000026f0: 454d 5054 5922 0a20 2020 2020 2020 2072  EMPTY".        r
-00002700: 6574 7572 6e20 224c 494e 4553 5452 494e  eturn "LINESTRIN
-00002710: 4722 202b 205f 6c69 6e65 7374 7269 6e67  G" + _linestring
-00002720: 5f77 6b74 5f69 6e6e 6572 2873 656c 662e  _wkt_inner(self.
-00002730: 706f 696e 7473 290a 0a20 2020 2064 6566  points)..    def
-00002740: 205f 5f65 715f 5f28 7365 6c66 2c20 6f74   __eq__(self, ot
-00002750: 6865 7229 3a0a 2020 2020 2020 2020 2320  her):.        # 
-00002760: 7374 7269 6374 2065 7175 616c 6974 792c  strict equality,
-00002770: 206e 6f74 2073 656d 616e 7469 630a 2020   not semantic.  
-00002780: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00002790: 6e63 6528 6f74 6865 722c 205f 5354 4c69  nce(other, _STLi
-000027a0: 6e65 7374 7269 6e67 293a 0a20 2020 2020  nestring):.     
-000027b0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000027c0: 6c66 2e70 6f69 6e74 7320 3d3d 206f 7468  lf.points == oth
-000027d0: 6572 2e70 6f69 6e74 730a 2020 2020 2020  er.points.      
-000027e0: 2020 7265 7475 726e 204e 6f74 496d 706c    return NotImpl
-000027f0: 656d 656e 7465 640a 0a0a 636c 6173 7320  emented...class 
-00002800: 5f53 5450 6f6c 7967 6f6e 3a0a 2020 2020  _STPolygon:.    
-00002810: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00002820: 662c 2065 7874 6572 696f 723a 204c 6973  f, exterior: Lis
-00002830: 745b 5f53 5450 6f69 6e74 5d2c 2068 6f6c  t[_STPoint], hol
-00002840: 6573 3a20 4c69 7374 5b4c 6973 745b 5f53  es: List[List[_S
-00002850: 5450 6f69 6e74 5d5d 293a 0a20 2020 2020  TPoint]]):.     
-00002860: 2020 2073 656c 662e 6578 7465 7269 6f72     self.exterior
-00002870: 203d 2065 7874 6572 696f 720a 2020 2020   = exterior.    
-00002880: 2020 2020 7365 6c66 2e68 6f6c 6573 203d      self.holes =
-00002890: 2068 6f6c 6573 0a0a 2020 2020 6465 6620   holes..    def 
-000028a0: 5f5f 7265 7072 5f5f 2873 656c 6629 3a0a  __repr__(self):.
-000028b0: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-000028c0: 656c 662e 6578 7465 7269 6f72 3a0a 2020  elf.exterior:.  
-000028d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000028e0: 2022 504f 4c59 474f 4e20 454d 5054 5922   "POLYGON EMPTY"
-000028f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00002900: 2250 4f4c 5947 4f4e 2822 202b 2022 2c20  "POLYGON(" + ", 
-00002910: 222e 6a6f 696e 2828 5f6c 696e 6573 7472  ".join((_linestr
-00002920: 696e 675f 776b 745f 696e 6e65 7228 706c  ing_wkt_inner(pl
-00002930: 2920 666f 7220 706c 2069 6e20 5b73 656c  ) for pl in [sel
-00002940: 662e 6578 7465 7269 6f72 5d20 2b20 7365  f.exterior] + se
-00002950: 6c66 2e68 6f6c 6573 2929 202b 2022 2922  lf.holes)) + ")"
-00002960: 0a0a 2020 2020 6465 6620 5f5f 6571 5f5f  ..    def __eq__
-00002970: 2873 656c 662c 206f 7468 6572 293a 0a20  (self, other):. 
-00002980: 2020 2020 2020 2023 2073 7472 6963 7420         # strict 
-00002990: 6571 7561 6c69 7479 2c20 6e6f 7420 7365  equality, not se
-000029a0: 6d61 6e74 6963 0a20 2020 2020 2020 2069  mantic.        i
-000029b0: 6620 6973 696e 7374 616e 6365 286f 7468  f isinstance(oth
-000029c0: 6572 2c20 5f53 5450 6f6c 7967 6f6e 293a  er, _STPolygon):
-000029d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000029e0: 7572 6e20 7365 6c66 2e65 7874 6572 696f  urn self.exterio
-000029f0: 7220 3d3d 206f 7468 6572 2e65 7874 6572  r == other.exter
-00002a00: 696f 7220 616e 6420 7365 6c66 2e68 6f6c  ior and self.hol
-00002a10: 6573 203d 3d20 6f74 6865 722e 686f 6c65  es == other.hole
-00002a20: 730a 2020 2020 2020 2020 7265 7475 726e  s.        return
-00002a30: 204e 6f74 496d 706c 656d 656e 7465 640a   NotImplemented.
-00002a40: 0a0a 2323 2323 2323 2323 2323 2323 2323  ..##############
-00002a50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002a60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002a70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002a80: 2323 2323 2323 2323 2323 230a 2320 4275  ###########.# Bu
-00002a90: 696c 6420 7375 7070 6f72 7465 6420 7265  ild supported re
-00002aa0: 7175 6573 742f 7265 7370 6f6e 7365 2074  quest/response t
-00002ab0: 7970 6520 6d61 7070 696e 6773 0a23 2323  ype mappings.###
-00002ac0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002ad0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002ae0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002af0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002b00: 2323 2323 2323 0a0a 0a63 6c61 7373 205f  ######...class _
-00002b10: 4f63 6965 6e74 5265 7175 6573 7446 6163  OcientRequestFac
-00002b20: 746f 7279 3a0a 2020 2020 6465 6620 7265  tory:.    def re
-00002b30: 7175 6573 7428 7365 6c66 2c20 6f70 6572  quest(self, oper
-00002b40: 6174 696f 6e3a 2073 7472 293a 0a20 2020  ation: str):.   
-00002b50: 2020 2020 2022 2222 4765 6e65 7261 7465       """Generate
-00002b60: 7320 6120 6675 6c6c 7920 706f 7075 6c61  s a fully popula
-00002b70: 7465 6420 7265 7175 6573 7420 7072 6f74  ted request prot
-00002b80: 6f62 7566 2222 220a 2020 2020 2020 2020  obuf""".        
-00002b90: 7261 6973 6520 4e6f 7449 6d70 6c65 6d65  raise NotImpleme
-00002ba0: 6e74 6564 4572 726f 720a 0a20 2020 2064  ntedError..    d
-00002bb0: 6566 2072 6573 706f 6e73 6528 7365 6c66  ef response(self
-00002bc0: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
-00002bd0: 6e65 7261 7465 7320 6120 6675 6c6c 7920  nerates a fully 
-00002be0: 706f 7075 6c61 7465 6420 7265 7370 6f6e  populated respon
-00002bf0: 7365 2070 726f 746f 6275 6622 2222 0a20  se protobuf""". 
-00002c00: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
-00002c10: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
-00002c20: 0a0a 2020 2020 6465 6620 7072 6f63 6573  ..    def proces
-00002c30: 7328 7365 6c66 2c20 7273 7029 202d 3e20  s(self, rsp) -> 
-00002c40: 416e 793a 0a20 2020 2020 2020 2022 2222  Any:.        """
-00002c50: 5072 6f63 6573 7320 7468 6520 636c 6965  Process the clie
-00002c60: 6e74 2072 6573 706f 6e73 6522 2222 0a20  nt response""". 
-00002c70: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
-00002c80: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
-00002c90: 0a0a 0a63 6c61 7373 205f 4578 6563 7574  ...class _Execut
-00002ca0: 6551 7565 7279 4661 6374 6f72 7928 5f4f  eQueryFactory(_O
-00002cb0: 6369 656e 7452 6571 7565 7374 4661 6374  cientRequestFact
-00002cc0: 6f72 7929 3a0a 2020 2020 6465 6620 7265  ory):.    def re
-00002cd0: 7175 6573 7428 7365 6c66 2c20 6f70 6572  quest(self, oper
-00002ce0: 6174 696f 6e3a 2073 7472 293a 0a20 2020  ation: str):.   
-00002cf0: 2020 2020 2022 2222 4765 6e65 7261 7465       """Generate
-00002d00: 7320 6120 6675 6c6c 7920 706f 7075 6c61  s a fully popula
-00002d10: 7465 6420 4558 4543 5554 455f 5155 4552  ted EXECUTE_QUER
-00002d20: 5920 7265 7175 6573 7420 7072 6f74 6f62  Y request protob
-00002d30: 7566 2222 220a 2020 2020 2020 2020 7265  uf""".        re
-00002d40: 7120 3d20 7072 6f74 6f2e 5265 7175 6573  q = proto.Reques
-00002d50: 7428 290a 2020 2020 2020 2020 7265 712e  t().        req.
-00002d60: 7479 7065 203d 2070 726f 746f 2e52 6571  type = proto.Req
-00002d70: 7565 7374 2e52 6571 7565 7374 5479 7065  uest.RequestType
-00002d80: 2e56 616c 7565 2822 4558 4543 5554 455f  .Value("EXECUTE_
-00002d90: 5155 4552 5922 290a 2020 2020 2020 2020  QUERY").        
-00002da0: 7265 712e 6578 6563 7574 655f 7175 6572  req.execute_quer
-00002db0: 792e 7371 6c20 3d20 6f70 6572 6174 696f  y.sql = operatio
-00002dc0: 6e0a 2020 2020 2020 2020 7265 712e 6578  n.        req.ex
-00002dd0: 6563 7574 655f 7175 6572 792e 666f 7263  ecute_query.forc
-00002de0: 6520 3d20 4661 6c73 650a 2020 2020 2020  e = False.      
-00002df0: 2020 7265 7475 726e 2072 6571 0a0a 2020    return req..  
-00002e00: 2020 6465 6620 7265 7370 6f6e 7365 2873    def response(s
-00002e10: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00002e20: 2247 656e 6572 6174 6573 2061 2066 756c  "Generates a ful
-00002e30: 6c79 2070 6f70 756c 6174 6564 2045 5845  ly populated EXE
-00002e40: 4355 5445 5f51 5545 5259 2072 6573 706f  CUTE_QUERY respo
-00002e50: 6e73 6520 7072 6f74 6f62 7566 2222 220a  nse protobuf""".
-00002e60: 2020 2020 2020 2020 7265 7475 726e 2070          return p
-00002e70: 726f 746f 2e45 7865 6375 7465 5175 6572  roto.ExecuteQuer
-00002e80: 7952 6573 706f 6e73 6528 290a 0a0a 636c  yResponse()...cl
-00002e90: 6173 7320 5f45 7865 6375 7465 4578 706c  ass _ExecuteExpl
-00002ea0: 6169 6e46 6163 746f 7279 285f 4f63 6965  ainFactory(_Ocie
-00002eb0: 6e74 5265 7175 6573 7446 6163 746f 7279  ntRequestFactory
-00002ec0: 293a 0a20 2020 2064 6566 2072 6571 7565  ):.    def reque
-00002ed0: 7374 2873 656c 662c 206f 7065 7261 7469  st(self, operati
-00002ee0: 6f6e 3a20 7374 7229 3a0a 2020 2020 2020  on: str):.      
-00002ef0: 2020 2222 2247 656e 6572 6174 6573 2061    """Generates a
-00002f00: 2066 756c 6c79 2070 6f70 756c 6174 6564   fully populated
-00002f10: 2045 5845 4355 5445 5f45 5850 4c41 494e   EXECUTE_EXPLAIN
-00002f20: 2072 6571 7565 7374 2070 726f 746f 6275   request protobu
-00002f30: 6622 2222 0a20 2020 2020 2020 2072 6571  f""".        req
-00002f40: 203d 2070 726f 746f 2e52 6571 7565 7374   = proto.Request
-00002f50: 2829 0a20 2020 2020 2020 2072 6571 2e74  ().        req.t
-00002f60: 7970 6520 3d20 7072 6f74 6f2e 5265 7175  ype = proto.Requ
-00002f70: 6573 742e 5265 7175 6573 7454 7970 652e  est.RequestType.
-00002f80: 5661 6c75 6528 2245 5845 4355 5445 5f45  Value("EXECUTE_E
-00002f90: 5850 4c41 494e 2229 0a20 2020 2020 2020  XPLAIN").       
-00002fa0: 2072 6571 2e65 7865 6375 7465 5f65 7870   req.execute_exp
-00002fb0: 6c61 696e 2e66 6f72 6d61 7420 3d20 7072  lain.format = pr
-00002fc0: 6f74 6f2e 4578 706c 6169 6e46 6f72 6d61  oto.ExplainForma
-00002fd0: 742e 4a53 4f4e 0a20 2020 2020 2020 2073  t.JSON.        s
-00002fe0: 706c 6974 7465 6420 3d20 6f70 6572 6174  plitted = operat
-00002ff0: 696f 6e2e 7370 6c69 7428 6d61 7873 706c  ion.split(maxspl
-00003000: 6974 3d31 290a 2020 2020 2020 2020 6966  it=1).        if
-00003010: 206c 656e 2873 706c 6974 7465 6429 203d   len(splitted) =
-00003020: 3d20 323a 0a20 2020 2020 2020 2020 2020  = 2:.           
-00003030: 2072 6571 2e65 7865 6375 7465 5f65 7870   req.execute_exp
-00003040: 6c61 696e 2e73 716c 203d 2073 706c 6974  lain.sql = split
-00003050: 7465 645b 315d 0a20 2020 2020 2020 2072  ted[1].        r
-00003060: 6574 7572 6e20 7265 710a 0a20 2020 2064  eturn req..    d
-00003070: 6566 2072 6573 706f 6e73 6528 7365 6c66  ef response(self
-00003080: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
-00003090: 6e65 7261 7465 7320 6120 6675 6c6c 7920  nerates a fully 
-000030a0: 706f 7075 6c61 7465 6420 4558 4543 5554  populated EXECUT
-000030b0: 455f 4558 504c 4149 4e20 7265 7370 6f6e  E_EXPLAIN respon
-000030c0: 7365 2070 726f 746f 6275 6622 2222 0a20  se protobuf""". 
-000030d0: 2020 2020 2020 2072 6574 7572 6e20 7072         return pr
-000030e0: 6f74 6f2e 4578 706c 6169 6e52 6573 706f  oto.ExplainRespo
-000030f0: 6e73 6553 7472 696e 6750 6c61 6e28 290a  nseStringPlan().
-00003100: 0a0a 636c 6173 7320 5f45 7865 6375 7465  ..class _Execute
-00003110: 4578 706f 7274 4661 6374 6f72 7928 5f4f  ExportFactory(_O
-00003120: 6369 656e 7452 6571 7565 7374 4661 6374  cientRequestFact
-00003130: 6f72 7929 3a0a 2020 2020 6465 6620 7265  ory):.    def re
-00003140: 7175 6573 7428 7365 6c66 2c20 6f70 6572  quest(self, oper
-00003150: 6174 696f 6e3a 2073 7472 293a 0a20 2020  ation: str):.   
-00003160: 2020 2020 2022 2222 4765 6e65 7261 7465       """Generate
-00003170: 7320 6120 6675 6c6c 7920 706f 7075 6c61  s a fully popula
-00003180: 7465 6420 4558 4543 5554 455f 4558 504f  ted EXECUTE_EXPO
-00003190: 5254 2072 6571 7565 7374 2070 726f 746f  RT request proto
-000031a0: 6275 6622 2222 0a20 2020 2020 2020 2072  buf""".        r
-000031b0: 6571 203d 2070 726f 746f 2e52 6571 7565  eq = proto.Reque
-000031c0: 7374 2829 0a20 2020 2020 2020 2072 6571  st().        req
-000031d0: 2e74 7970 6520 3d20 7072 6f74 6f2e 5265  .type = proto.Re
-000031e0: 7175 6573 742e 5265 7175 6573 7454 7970  quest.RequestTyp
-000031f0: 652e 5661 6c75 6528 2245 5845 4355 5445  e.Value("EXECUTE
-00003200: 5f45 5850 4f52 5422 290a 2020 2020 2020  _EXPORT").      
-00003210: 2020 7265 712e 6578 6563 7574 655f 6578    req.execute_ex
-00003220: 706f 7274 2e73 716c 203d 206f 7065 7261  port.sql = opera
-00003230: 7469 6f6e 0a20 2020 2020 2020 2072 6574  tion.        ret
-00003240: 7572 6e20 7265 710a 0a20 2020 2064 6566  urn req..    def
-00003250: 2072 6573 706f 6e73 6528 7365 6c66 293a   response(self):
-00003260: 0a20 2020 2020 2020 2022 2222 4765 6e65  .        """Gene
-00003270: 7261 7465 7320 6120 6675 6c6c 7920 706f  rates a fully po
-00003280: 7075 6c61 7465 6420 4558 4543 5554 455f  pulated EXECUTE_
-00003290: 4558 504f 5254 2072 6573 706f 6e73 6520  EXPORT response 
-000032a0: 7072 6f74 6f62 7566 2222 220a 2020 2020  protobuf""".    
-000032b0: 2020 2020 7265 7475 726e 2070 726f 746f      return proto
-000032c0: 2e45 7865 6375 7465 4578 706f 7274 5265  .ExecuteExportRe
-000032d0: 7370 6f6e 7365 2829 0a0a 0a63 6c61 7373  sponse()...class
-000032e0: 205f 4578 706c 6169 6e50 6970 656c 696e   _ExplainPipelin
-000032f0: 6546 6163 746f 7279 285f 4f63 6965 6e74  eFactory(_Ocient
-00003300: 5265 7175 6573 7446 6163 746f 7279 293a  RequestFactory):
-00003310: 0a20 2020 2064 6566 2072 6571 7565 7374  .    def request
-00003320: 2873 656c 662c 206f 7065 7261 7469 6f6e  (self, operation
-00003330: 3a20 7374 7229 3a0a 2020 2020 2020 2020  : str):.        
-00003340: 2222 2247 656e 6572 6174 6573 2061 2066  """Generates a f
-00003350: 756c 6c79 2070 6f70 756c 6174 6564 2045  ully populated E
-00003360: 5850 4c41 494e 5f50 4950 454c 494e 4520  XPLAIN_PIPELINE 
-00003370: 7265 7175 6573 7420 7072 6f74 6f62 7566  request protobuf
-00003380: 2222 220a 2020 2020 2020 2020 7265 7120  """.        req 
-00003390: 3d20 7072 6f74 6f2e 5265 7175 6573 7428  = proto.Request(
-000033a0: 290a 2020 2020 2020 2020 7265 712e 7479  ).        req.ty
-000033b0: 7065 203d 2070 726f 746f 2e52 6571 7565  pe = proto.Reque
-000033c0: 7374 2e52 6571 7565 7374 5479 7065 2e56  st.RequestType.V
-000033d0: 616c 7565 2822 4558 504c 4149 4e5f 5049  alue("EXPLAIN_PI
-000033e0: 5045 4c49 4e45 2229 0a20 2020 2020 2020  PELINE").       
-000033f0: 2072 6571 2e65 7870 6c61 696e 5f70 6970   req.explain_pip
-00003400: 656c 696e 652e 7371 6c20 3d20 6f70 6572  eline.sql = oper
-00003410: 6174 696f 6e0a 2020 2020 2020 2020 7265  ation.        re
-00003420: 7475 726e 2072 6571 0a0a 2020 2020 6465  turn req..    de
-00003430: 6620 7265 7370 6f6e 7365 2873 656c 6629  f response(self)
-00003440: 3a0a 2020 2020 2020 2020 2222 2247 656e  :.        """Gen
-00003450: 6572 6174 6573 2061 2066 756c 6c79 2070  erates a fully p
-00003460: 6f70 756c 6174 6564 2045 5850 4c41 494e  opulated EXPLAIN
-00003470: 5f50 4950 454c 494e 4520 7265 7370 6f6e  _PIPELINE respon
-00003480: 7365 2070 726f 746f 6275 6622 2222 0a20  se protobuf""". 
-00003490: 2020 2020 2020 2072 6574 7572 6e20 7072         return pr
-000034a0: 6f74 6f2e 4578 706c 6169 6e50 6970 656c  oto.ExplainPipel
-000034b0: 696e 6552 6573 706f 6e73 6528 290a 0a0a  ineResponse()...
-000034c0: 636c 6173 7320 5f43 6865 636b 4461 7461  class _CheckData
-000034d0: 4661 6374 6f72 7928 5f4f 6369 656e 7452  Factory(_OcientR
-000034e0: 6571 7565 7374 4661 6374 6f72 7929 3a0a  equestFactory):.
-000034f0: 2020 2020 6465 6620 7265 7175 6573 7428      def request(
-00003500: 7365 6c66 2c20 6f70 6572 6174 696f 6e3a  self, operation:
-00003510: 2073 7472 293a 0a20 2020 2020 2020 2022   str):.        "
-00003520: 2222 4765 6e65 7261 7465 7320 6120 6675  ""Generates a fu
-00003530: 6c6c 7920 706f 7075 6c61 7465 6420 4348  lly populated CH
-00003540: 4543 4b5f 4441 5441 2072 6571 7565 7374  ECK_DATA request
-00003550: 2070 726f 746f 6275 6622 2222 0a20 2020   protobuf""".   
-00003560: 2020 2020 2072 6571 203d 2070 726f 746f       req = proto
-00003570: 2e52 6571 7565 7374 2829 0a20 2020 2020  .Request().     
-00003580: 2020 2072 6571 2e74 7970 6520 3d20 7072     req.type = pr
-00003590: 6f74 6f2e 5265 7175 6573 742e 5265 7175  oto.Request.Requ
-000035a0: 6573 7454 7970 652e 5661 6c75 6528 2243  estType.Value("C
-000035b0: 4845 434b 5f44 4154 4122 290a 2020 2020  HECK_DATA").    
-000035c0: 2020 2020 7265 712e 6368 6563 6b5f 6461      req.check_da
-000035d0: 7461 2e73 716c 203d 206f 7065 7261 7469  ta.sql = operati
-000035e0: 6f6e 0a20 2020 2020 2020 2072 6574 7572  on.        retur
-000035f0: 6e20 7265 710a 0a20 2020 2064 6566 2072  n req..    def r
-00003600: 6573 706f 6e73 6528 7365 6c66 293a 0a20  esponse(self):. 
-00003610: 2020 2020 2020 2022 2222 4765 6e65 7261         """Genera
-00003620: 7465 7320 6120 6675 6c6c 7920 706f 7075  tes a fully popu
-00003630: 6c61 7465 6420 4348 4543 4b5f 4441 5441  lated CHECK_DATA
-00003640: 2072 6573 706f 6e73 6520 7072 6f74 6f62   response protob
-00003650: 7566 2222 220a 2020 2020 2020 2020 7265  uf""".        re
-00003660: 7475 726e 2070 726f 746f 2e43 6865 636b  turn proto.Check
-00003670: 4461 7461 5265 7370 6f6e 7365 2829 0a0a  DataResponse()..
-00003680: 0a63 6c61 7373 205f 466f 7263 6545 7874  .class _ForceExt
-00003690: 6572 6e61 6c46 6163 746f 7279 285f 4f63  ernalFactory(_Oc
-000036a0: 6965 6e74 5265 7175 6573 7446 6163 746f  ientRequestFacto
-000036b0: 7279 293a 0a20 2020 2064 6566 2072 6571  ry):.    def req
-000036c0: 7565 7374 2873 656c 662c 206f 7065 7261  uest(self, opera
-000036d0: 7469 6f6e 3a20 7374 7229 3a0a 2020 2020  tion: str):.    
-000036e0: 2020 2020 2222 2247 656e 6572 6174 6573      """Generates
-000036f0: 2061 2066 756c 6c79 2070 6f70 756c 6174   a fully populat
-00003700: 6564 2046 4f52 4345 5f45 5854 4552 4e41  ed FORCE_EXTERNA
-00003710: 4c20 7265 7175 6573 7420 7072 6f74 6f62  L request protob
-00003720: 7566 2222 220a 2020 2020 2020 2020 7265  uf""".        re
-00003730: 7120 3d20 7072 6f74 6f2e 5265 7175 6573  q = proto.Reques
-00003740: 7428 290a 2020 2020 2020 2020 7265 712e  t().        req.
-00003750: 7479 7065 203d 2070 726f 746f 2e52 6571  type = proto.Req
-00003760: 7565 7374 2e52 6571 7565 7374 5479 7065  uest.RequestType
-00003770: 2e56 616c 7565 2822 5345 545f 5041 5241  .Value("SET_PARA
-00003780: 4d45 5445 5222 290a 2020 2020 2020 2020  METER").        
-00003790: 7370 203d 2072 6571 2e73 6574 5f70 6172  sp = req.set_par
-000037a0: 616d 6574 6572 0a20 2020 2020 2020 2069  ameter.        i
-000037b0: 6620 6f70 6572 6174 696f 6e2e 656e 6473  f operation.ends
-000037c0: 7769 7468 2822 6f6e 2229 3a0a 2020 2020  with("on"):.    
-000037d0: 2020 2020 2020 2020 7370 2e66 6f72 6365          sp.force
-000037e0: 5f65 7874 6572 6e61 6c2e 6973 5f6f 6e20  _external.is_on 
-000037f0: 3d20 5472 7565 0a20 2020 2020 2020 2065  = True.        e
-00003800: 6c69 6620 6f70 6572 6174 696f 6e2e 656e  lif operation.en
-00003810: 6473 7769 7468 2822 6f66 6622 293a 0a20  dswith("off"):. 
-00003820: 2020 2020 2020 2020 2020 2073 702e 666f             sp.fo
-00003830: 7263 655f 6578 7465 726e 616c 2e69 735f  rce_external.is_
-00003840: 6f6e 203d 2046 616c 7365 0a20 2020 2020  on = False.     
-00003850: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00003860: 2020 2020 2072 6169 7365 2053 796e 7461       raise Synta
-00003870: 7845 7272 6f72 2827 466f 726d 6174 206d  xError('Format m
-00003880: 7573 7420 6265 2022 464f 5243 4520 4558  ust be "FORCE EX
-00003890: 5445 524e 414c 2028 6f6e 7c6f 6666 2922  TERNAL (on|off)"
-000038a0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-000038b0: 6e20 7265 710a 0a20 2020 2064 6566 2072  n req..    def r
-000038c0: 6573 706f 6e73 6528 7365 6c66 293a 0a20  esponse(self):. 
-000038d0: 2020 2020 2020 2022 2222 4765 6e65 7261         """Genera
-000038e0: 7465 7320 6120 6675 6c6c 7920 706f 7075  tes a fully popu
-000038f0: 6c61 7465 6420 464f 5243 455f 4558 5445  lated FORCE_EXTE
-00003900: 524e 414c 2072 6573 706f 6e73 6520 7072  RNAL response pr
-00003910: 6f74 6f62 7566 2222 220a 2020 2020 2020  otobuf""".      
-00003920: 2020 7265 7475 726e 2070 726f 746f 2e43    return proto.C
-00003930: 6f6e 6669 726d 6174 696f 6e52 6573 706f  onfirmationRespo
-00003940: 6e73 6528 290a 0a0a 636c 6173 7320 5f53  nse()...class _S
-00003950: 6574 5363 6865 6d61 4661 6374 6f72 7928  etSchemaFactory(
-00003960: 5f4f 6369 656e 7452 6571 7565 7374 4661  _OcientRequestFa
-00003970: 6374 6f72 7929 3a0a 2020 2020 6465 6620  ctory):.    def 
-00003980: 7265 7175 6573 7428 7365 6c66 2c20 7363  request(self, sc
-00003990: 6865 6d61 3a20 7374 7229 3a0a 2020 2020  hema: str):.    
-000039a0: 2020 2020 2222 2247 656e 6572 6174 6573      """Generates
-000039b0: 2061 2066 756c 6c79 2070 6f70 756c 6174   a fully populat
-000039c0: 6564 2053 4554 2053 4348 454d 4120 7265  ed SET SCHEMA re
-000039d0: 7175 6573 7420 7072 6f74 6f62 7566 2222  quest protobuf""
-000039e0: 220a 2020 2020 2020 2020 7265 7120 3d20  ".        req = 
-000039f0: 7072 6f74 6f2e 5265 7175 6573 7428 290a  proto.Request().
-00003a00: 2020 2020 2020 2020 7265 712e 7479 7065          req.type
-00003a10: 203d 2070 726f 746f 2e52 6571 7565 7374   = proto.Request
-00003a20: 2e52 6571 7565 7374 5479 7065 2e56 616c  .RequestType.Val
-00003a30: 7565 2822 5345 545f 5343 4845 4d41 2229  ue("SET_SCHEMA")
-00003a40: 0a20 2020 2020 2020 2072 6571 2e73 6574  .        req.set
-00003a50: 5f73 6368 656d 612e 7363 6865 6d61 203d  _schema.schema =
-00003a60: 2073 6368 656d 610a 2020 2020 2020 2020   schema.        
-00003a70: 7265 7475 726e 2072 6571 0a0a 2020 2020  return req..    
-00003a80: 6465 6620 7265 7370 6f6e 7365 2873 656c  def response(sel
-00003a90: 6629 3a0a 2020 2020 2020 2020 2222 2247  f):.        """G
-00003aa0: 656e 6572 6174 6573 2053 4554 5f53 4348  enerates SET_SCH
-00003ab0: 454d 4120 7265 7370 6f6e 7365 2070 726f  EMA response pro
-00003ac0: 746f 6275 6622 2222 0a20 2020 2020 2020  tobuf""".       
-00003ad0: 2072 6574 7572 6e20 7072 6f74 6f2e 436f   return proto.Co
-00003ae0: 6e66 6972 6d61 7469 6f6e 5265 7370 6f6e  nfirmationRespon
-00003af0: 7365 2829 0a0a 0a63 6c61 7373 205f 4765  se()...class _Ge
-00003b00: 7453 6368 656d 6146 6163 746f 7279 285f  tSchemaFactory(_
-00003b10: 4f63 6965 6e74 5265 7175 6573 7446 6163  OcientRequestFac
-00003b20: 746f 7279 293a 0a20 2020 2064 6566 2072  tory):.    def r
-00003b30: 6571 7565 7374 2873 656c 6629 3a0a 2020  equest(self):.  
-00003b40: 2020 2020 2020 2222 2247 656e 6572 6174        """Generat
-00003b50: 6573 2061 2066 756c 6c79 2070 6f70 756c  es a fully popul
-00003b60: 6174 6564 2047 4554 2053 4348 454d 4120  ated GET SCHEMA 
-00003b70: 7265 7175 6573 7420 7072 6f74 6f62 7566  request protobuf
-00003b80: 2222 220a 2020 2020 2020 2020 7265 7120  """.        req 
-00003b90: 3d20 7072 6f74 6f2e 5265 7175 6573 7428  = proto.Request(
-00003ba0: 290a 2020 2020 2020 2020 7265 712e 7479  ).        req.ty
-00003bb0: 7065 203d 2070 726f 746f 2e52 6571 7565  pe = proto.Reque
-00003bc0: 7374 2e52 6571 7565 7374 5479 7065 2e56  st.RequestType.V
-00003bd0: 616c 7565 2822 4745 545f 5343 4845 4d41  alue("GET_SCHEMA
-00003be0: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
-00003bf0: 6e20 7265 710a 0a20 2020 2064 6566 2072  n req..    def r
-00003c00: 6573 706f 6e73 6528 7365 6c66 293a 0a20  esponse(self):. 
-00003c10: 2020 2020 2020 2022 2222 4765 6e65 7261         """Genera
-00003c20: 7465 7320 5345 545f 5343 4845 4d41 2072  tes SET_SCHEMA r
-00003c30: 6573 706f 6e73 6520 7072 6f74 6f62 7566  esponse protobuf
-00003c40: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-00003c50: 726e 2070 726f 746f 2e47 6574 5363 6865  rn proto.GetSche
-00003c60: 6d61 5265 7370 6f6e 7365 2829 0a0a 0a63  maResponse()...c
-00003c70: 6c61 7373 205f 436c 6561 7243 6163 6865  lass _ClearCache
-00003c80: 4661 6374 6f72 7928 5f4f 6369 656e 7452  Factory(_OcientR
-00003c90: 6571 7565 7374 4661 6374 6f72 7929 3a0a  equestFactory):.
-00003ca0: 2020 2020 6465 6620 7265 7175 6573 7428      def request(
-00003cb0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00003cc0: 2222 4765 6e65 7261 7465 7320 6120 6675  ""Generates a fu
-00003cd0: 6c6c 7920 706f 7075 6c61 7465 6420 434c  lly populated CL
-00003ce0: 4541 5220 4341 4348 4520 7265 7175 6573  EAR CACHE reques
-00003cf0: 7420 7072 6f74 6f62 7566 2222 220a 2020  t protobuf""".  
-00003d00: 2020 2020 2020 7265 7120 3d20 7072 6f74        req = prot
-00003d10: 6f2e 5265 7175 6573 7428 290a 2020 2020  o.Request().    
-00003d20: 2020 2020 7265 712e 7479 7065 203d 2070      req.type = p
-00003d30: 726f 746f 2e52 6571 7565 7374 2e52 6571  roto.Request.Req
-00003d40: 7565 7374 5479 7065 2e56 616c 7565 2822  uestType.Value("
-00003d50: 434c 4541 525f 4341 4348 4522 290a 2020  CLEAR_CACHE").  
-00003d60: 2020 2020 2020 7265 712e 636c 6561 725f        req.clear_
-00003d70: 6361 6368 652e 616c 6c5f 6e6f 6465 7320  cache.all_nodes 
-00003d80: 3d20 5472 7565 0a20 2020 2020 2020 2072  = True.        r
-00003d90: 6574 7572 6e20 7265 710a 0a20 2020 2064  eturn req..    d
-00003da0: 6566 2072 6573 706f 6e73 6528 7365 6c66  ef response(self
-00003db0: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
-00003dc0: 6e65 7261 7465 7320 5345 545f 5343 4845  nerates SET_SCHE
-00003dd0: 4d41 2072 6573 706f 6e73 6520 7072 6f74  MA response prot
-00003de0: 6f62 7566 2222 220a 2020 2020 2020 2020  obuf""".        
-00003df0: 7265 7475 726e 2070 726f 746f 2e43 6f6e  return proto.Con
-00003e00: 6669 726d 6174 696f 6e52 6573 706f 6e73  firmationRespons
-00003e10: 6528 290a 0a0a 636c 6173 7320 5f53 6574  e()...class _Set
-00003e20: 5061 7261 6d65 7465 7246 6163 746f 7279  ParameterFactory
-00003e30: 285f 4f63 6965 6e74 5265 7175 6573 7446  (_OcientRequestF
-00003e40: 6163 746f 7279 293a 0a20 2020 2064 6566  actory):.    def
-00003e50: 2072 6571 7565 7374 2873 656c 662c 206f   request(self, o
-00003e60: 703a 2073 7472 2c20 7661 6c3a 2069 6e74  p: str, val: int
-00003e70: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
-00003e80: 6e65 7261 7465 7320 6120 6675 6c6c 7920  nerates a fully 
-00003e90: 706f 7075 6c61 7465 6420 5345 5420 5041  populated SET PA
-00003ea0: 5241 4d45 5445 5220 7265 7175 6573 7420  RAMETER request 
-00003eb0: 7072 6f74 6f62 7566 2222 220a 2020 2020  protobuf""".    
-00003ec0: 2020 2020 7265 7120 3d20 7072 6f74 6f2e      req = proto.
-00003ed0: 5265 7175 6573 7428 290a 2020 2020 2020  Request().      
-00003ee0: 2020 7265 712e 7479 7065 203d 2070 726f    req.type = pro
-00003ef0: 746f 2e52 6571 7565 7374 2e52 6571 7565  to.Request.Reque
-00003f00: 7374 5479 7065 2e56 616c 7565 2822 5345  stType.Value("SE
-00003f10: 545f 5041 5241 4d45 5445 5222 290a 0a20  T_PARAMETER").. 
-00003f20: 2020 2020 2020 2073 7020 3d20 7265 712e         sp = req.
-00003f30: 7365 745f 7061 7261 6d65 7465 720a 0a20  set_parameter.. 
-00003f40: 2020 2020 2020 2069 6620 6f70 203d 3d20         if op == 
-00003f50: 224d 4158 524f 5753 223a 0a20 2020 2020  "MAXROWS":.     
-00003f60: 2020 2020 2020 2073 702e 726f 775f 6c69         sp.row_li
-00003f70: 6d69 742e 726f 774c 696d 6974 203d 2076  mit.rowLimit = v
-00003f80: 616c 0a20 2020 2020 2020 2065 6c69 6620  al.        elif 
-00003f90: 6f70 203d 3d20 224d 4158 5449 4d45 223a  op == "MAXTIME":
-00003fa0: 0a20 2020 2020 2020 2020 2020 2073 702e  .            sp.
-00003fb0: 7469 6d65 5f6c 696d 6974 2e74 696d 654c  time_limit.timeL
-00003fc0: 696d 6974 203d 2076 616c 0a20 2020 2020  imit = val.     
-00003fd0: 2020 2065 6c69 6620 6f70 203d 3d20 224d     elif op == "M
-00003fe0: 4158 5445 4d50 4449 534b 223a 0a20 2020  AXTEMPDISK":.   
-00003ff0: 2020 2020 2020 2020 2073 702e 7465 6d70           sp.temp
-00004000: 5f64 6973 6b5f 6c69 6d69 742e 7465 6d70  _disk_limit.temp
-00004010: 4469 736b 4c69 6d69 7420 3d20 7661 6c0a  DiskLimit = val.
-00004020: 2020 2020 2020 2020 656c 6966 206f 7020          elif op 
-00004030: 3d3d 2022 5052 494f 5249 5459 223a 0a20  == "PRIORITY":. 
-00004040: 2020 2020 2020 2020 2020 2073 702e 7072             sp.pr
-00004050: 696f 7269 7479 2e70 7269 6f72 6974 7920  iority.priority 
-00004060: 3d20 7661 6c0a 2020 2020 2020 2020 656c  = val.        el
-00004070: 6966 206f 7020 3d3d 2022 5041 5241 4c4c  if op == "PARALL
-00004080: 454c 4953 4d22 3a0a 2020 2020 2020 2020  ELISM":.        
-00004090: 2020 2020 7370 2e63 6f6e 6375 7272 656e      sp.concurren
-000040a0: 6379 2e63 6f6e 6375 7272 656e 6379 203d  cy.concurrency =
-000040b0: 2076 616c 0a20 2020 2020 2020 2065 6c69   val.        eli
-000040c0: 6620 6f70 203d 3d20 2250 5249 4f52 4954  f op == "PRIORIT
-000040d0: 595f 4144 4a55 5354 4d45 4e54 5f46 4143  Y_ADJUSTMENT_FAC
-000040e0: 544f 5222 3a0a 2020 2020 2020 2020 2020  TOR":.          
-000040f0: 2020 7370 2e70 7269 6f72 6974 795f 6164    sp.priority_ad
-00004100: 6a75 7374 5f66 6163 746f 722e 7072 696f  just_factor.prio
-00004110: 7269 7479 5f61 646a 7573 745f 6661 6374  rity_adjust_fact
-00004120: 6f72 203d 2076 616c 0a20 2020 2020 2020  or = val.       
-00004130: 2065 6c69 6620 6f70 203d 3d20 2250 5249   elif op == "PRI
-00004140: 4f52 4954 595f 4144 4a55 5354 4d45 4e54  ORITY_ADJUSTMENT
-00004150: 5f54 494d 4522 3a0a 2020 2020 2020 2020  _TIME":.        
-00004160: 2020 2020 7370 2e70 7269 6f72 6974 795f      sp.priority_
-00004170: 6164 6a75 7374 5f74 696d 652e 7072 696f  adjust_time.prio
-00004180: 7269 7479 5f61 646a 7573 745f 7469 6d65  rity_adjust_time
-00004190: 203d 2076 616c 0a20 2020 2020 2020 2065   = val.        e
-000041a0: 6c69 6620 6f70 203d 3d20 224d 494e 5f50  lif op == "MIN_P
-000041b0: 5249 4f52 4954 5922 3a0a 2020 2020 2020  RIORITY":.      
-000041c0: 2020 2020 2020 7370 2e6d 696e 5f70 7269        sp.min_pri
-000041d0: 6f72 6974 792e 6d69 6e5f 7072 696f 7269  ority.min_priori
-000041e0: 7479 203d 2076 616c 0a20 2020 2020 2020  ty = val.       
-000041f0: 2065 6c69 6620 6f70 203d 3d20 224d 4158   elif op == "MAX
-00004200: 5f50 5249 4f52 4954 5922 3a0a 2020 2020  _PRIORITY":.    
-00004210: 2020 2020 2020 2020 7370 2e6d 6178 5f70          sp.max_p
-00004220: 7269 6f72 6974 792e 6d61 785f 7072 696f  riority.max_prio
-00004230: 7269 7479 203d 2076 616c 0a20 2020 2020  rity = val.     
-00004240: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00004250: 2020 2020 2072 6169 7365 2050 726f 6772       raise Progr
-00004260: 616d 6d69 6e67 4572 726f 7228 7265 6173  ammingError(reas
-00004270: 6f6e 3d66 2253 796e 7461 7820 6572 726f  on=f"Syntax erro
-00004280: 722e 2049 6e76 616c 6964 2053 4554 207b  r. Invalid SET {
-00004290: 6f70 7d22 290a 0a20 2020 2020 2020 2072  op}")..        r
-000042a0: 6574 7572 6e20 7265 710a 0a20 2020 2064  eturn req..    d
-000042b0: 6566 2072 6573 706f 6e73 6528 7365 6c66  ef response(self
-000042c0: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
-000042d0: 6e65 7261 7465 7320 6120 5345 545f 5041  nerates a SET_PA
-000042e0: 5241 4d45 5445 5220 7265 7370 6f6e 7365  RAMETER response
-000042f0: 2070 726f 746f 6275 6622 2222 0a20 2020   protobuf""".   
-00004300: 2020 2020 2072 6574 7572 6e20 7072 6f74       return prot
-00004310: 6f2e 436f 6e66 6972 6d61 7469 6f6e 5265  o.ConfirmationRe
-00004320: 7370 6f6e 7365 2829 0a0a 0a63 6c61 7373  sponse()...class
-00004330: 205f 4361 6e63 656c 5175 6572 7946 6163   _CancelQueryFac
-00004340: 746f 7279 285f 4f63 6965 6e74 5265 7175  tory(_OcientRequ
-00004350: 6573 7446 6163 746f 7279 293a 0a20 2020  estFactory):.   
-00004360: 2064 6566 2072 6571 7565 7374 2873 656c   def request(sel
-00004370: 662c 2069 643a 2073 7472 293a 0a20 2020  f, id: str):.   
-00004380: 2020 2020 2022 2222 4765 6e65 7261 7465       """Generate
-00004390: 7320 6120 6675 6c6c 7920 706f 7075 6c61  s a fully popula
-000043a0: 7465 6420 4341 4e43 454c 2051 5545 5259  ted CANCEL QUERY
-000043b0: 2072 6571 7565 7374 2070 726f 746f 6275   request protobu
-000043c0: 6622 2222 0a20 2020 2020 2020 2072 6571  f""".        req
-000043d0: 203d 2070 726f 746f 2e52 6571 7565 7374   = proto.Request
-000043e0: 2829 0a20 2020 2020 2020 2072 6571 2e74  ().        req.t
-000043f0: 7970 6520 3d20 7072 6f74 6f2e 5265 7175  ype = proto.Requ
-00004400: 6573 742e 5265 7175 6573 7454 7970 652e  est.RequestType.
-00004410: 5661 6c75 6528 2243 414e 4345 4c5f 5155  Value("CANCEL_QU
-00004420: 4552 5922 290a 2020 2020 2020 2020 7265  ERY").        re
-00004430: 712e 6361 6e63 656c 5f71 7565 7279 2e73  q.cancel_query.s
-00004440: 716c 203d 2069 640a 2020 2020 2020 2020  ql = id.        
-00004450: 7265 7475 726e 2072 6571 0a0a 2020 2020  return req..    
-00004460: 6465 6620 7265 7370 6f6e 7365 2873 656c  def response(sel
-00004470: 6629 3a0a 2020 2020 2020 2020 2222 2247  f):.        """G
-00004480: 656e 6572 6174 6573 2061 2043 414e 4345  enerates a CANCE
-00004490: 4c5f 5155 4552 5920 7265 7370 6f6e 7365  L_QUERY response
-000044a0: 2070 726f 746f 6275 6622 2222 0a20 2020   protobuf""".   
-000044b0: 2020 2020 2072 6574 7572 6e20 7072 6f74       return prot
-000044c0: 6f2e 4361 6e63 656c 5175 6572 7952 6573  o.CancelQueryRes
-000044d0: 706f 6e73 6528 290a 0a0a 636c 6173 7320  ponse()...class 
-000044e0: 5f4b 696c 6c51 7565 7279 4661 6374 6f72  _KillQueryFactor
-000044f0: 7928 5f4f 6369 656e 7452 6571 7565 7374  y(_OcientRequest
-00004500: 4661 6374 6f72 7929 3a0a 2020 2020 6465  Factory):.    de
-00004510: 6620 7265 7175 6573 7428 7365 6c66 2c20  f request(self, 
-00004520: 6964 3a20 7374 7229 3a0a 2020 2020 2020  id: str):.      
-00004530: 2020 2222 2247 656e 6572 6174 6573 2061    """Generates a
-00004540: 2066 756c 6c79 2070 6f70 756c 6174 6564   fully populated
-00004550: 204b 494c 4c20 5155 4552 5920 7265 7175   KILL QUERY requ
-00004560: 6573 7420 7072 6f74 6f62 7566 2222 220a  est protobuf""".
-00004570: 2020 2020 2020 2020 7265 7120 3d20 7072          req = pr
-00004580: 6f74 6f2e 5265 7175 6573 7428 290a 2020  oto.Request().  
-00004590: 2020 2020 2020 7265 712e 7479 7065 203d        req.type =
-000045a0: 2070 726f 746f 2e52 6571 7565 7374 2e52   proto.Request.R
-000045b0: 6571 7565 7374 5479 7065 2e56 616c 7565  equestType.Value
-000045c0: 2822 4b49 4c4c 5f51 5545 5259 2229 0a20  ("KILL_QUERY"). 
-000045d0: 2020 2020 2020 2072 6571 2e6b 696c 6c5f         req.kill_
-000045e0: 7175 6572 792e 7371 6c20 3d20 6964 0a20  query.sql = id. 
-000045f0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00004600: 710a 0a20 2020 2064 6566 2072 6573 706f  q..    def respo
-00004610: 6e73 6528 7365 6c66 293a 0a20 2020 2020  nse(self):.     
-00004620: 2020 2022 2222 4765 6e65 7261 7465 7320     """Generates 
-00004630: 6120 4b49 4c4c 5f51 5545 5259 2072 6573  a KILL_QUERY res
-00004640: 706f 6e73 6520 7072 6f74 6f62 7566 2222  ponse protobuf""
-00004650: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-00004660: 2070 726f 746f 2e4b 696c 6c51 7565 7279   proto.KillQuery
-00004670: 5265 7370 6f6e 7365 2829 0a0a 0a63 6c61  Response()...cla
-00004680: 7373 205f 4765 7453 7973 7465 6d4d 6574  ss _GetSystemMet
-00004690: 6164 6174 6146 6163 746f 7279 285f 4f63  adataFactory(_Oc
-000046a0: 6965 6e74 5265 7175 6573 7446 6163 746f  ientRequestFacto
-000046b0: 7279 293a 0a20 2020 2064 6566 2072 6571  ry):.    def req
-000046c0: 7565 7374 2873 656c 662c 206f 702c 2073  uest(self, op, s
-000046d0: 6368 656d 612c 2074 6162 6c65 2c20 636f  chema, table, co
-000046e0: 6c75 6d6e 2c20 7669 6577 293a 0a20 2020  lumn, view):.   
-000046f0: 2020 2020 2022 2222 4765 6e65 7261 7465       """Generate
-00004700: 7320 6120 6675 6c6c 7920 706f 7075 6c61  s a fully popula
-00004710: 7465 6420 4745 545f 5359 5354 454d 5f4d  ted GET_SYSTEM_M
-00004720: 4554 4144 4154 4120 7265 7175 6573 7420  ETADATA request 
-00004730: 7072 6f74 6f62 7566 2222 220a 2020 2020  protobuf""".    
-00004740: 2020 2020 7265 7120 3d20 7072 6f74 6f2e      req = proto.
-00004750: 5265 7175 6573 7428 290a 2020 2020 2020  Request().      
-00004760: 2020 7265 712e 7479 7065 203d 2070 726f    req.type = pro
-00004770: 746f 2e52 6571 7565 7374 2e52 6571 7565  to.Request.Reque
-00004780: 7374 5479 7065 2e56 616c 7565 2822 4645  stType.Value("FE
-00004790: 5443 485f 5359 5354 454d 5f4d 4554 4144  TCH_SYSTEM_METAD
-000047a0: 4154 4122 290a 2020 2020 2020 2020 7265  ATA").        re
-000047b0: 712e 6665 7463 685f 7379 7374 656d 5f6d  q.fetch_system_m
-000047c0: 6574 6164 6174 612e 6361 6c6c 203d 206f  etadata.call = o
-000047d0: 700a 0a20 2020 2020 2020 2069 6620 7363  p..        if sc
-000047e0: 6865 6d61 2069 7320 6e6f 7420 4e6f 6e65  hema is not None
-000047f0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00004800: 712e 6665 7463 685f 7379 7374 656d 5f6d  q.fetch_system_m
-00004810: 6574 6164 6174 612e 7363 6865 6d61 203d  etadata.schema =
-00004820: 2073 6368 656d 610a 2020 2020 2020 2020   schema.        
-00004830: 6966 2074 6162 6c65 2069 7320 6e6f 7420  if table is not 
-00004840: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00004850: 2020 7265 712e 6665 7463 685f 7379 7374    req.fetch_syst
-00004860: 656d 5f6d 6574 6164 6174 612e 7461 626c  em_metadata.tabl
-00004870: 6520 3d20 7461 626c 650a 2020 2020 2020  e = table.      
-00004880: 2020 6966 2063 6f6c 756d 6e20 6973 206e    if column is n
-00004890: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000048a0: 2020 2020 2072 6571 2e66 6574 6368 5f73       req.fetch_s
-000048b0: 7973 7465 6d5f 6d65 7461 6461 7461 2e63  ystem_metadata.c
-000048c0: 6f6c 756d 6e20 3d20 636f 6c75 6d6e 0a20  olumn = column. 
-000048d0: 2020 2020 2020 2069 6620 7669 6577 2069         if view i
-000048e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000048f0: 2020 2020 2020 2020 7265 712e 6665 7463          req.fetc
-00004900: 685f 7379 7374 656d 5f6d 6574 6164 6174  h_system_metadat
-00004910: 612e 7669 6577 203d 2076 6965 770a 0a20  a.view = view.. 
-00004920: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00004930: 710a 0a20 2020 2064 6566 2072 6573 706f  q..    def respo
-00004940: 6e73 6528 7365 6c66 293a 0a20 2020 2020  nse(self):.     
-00004950: 2020 2022 2222 4765 6e65 7261 7465 7320     """Generates 
-00004960: 6120 6675 6c6c 7920 706f 7075 6c61 7465  a fully populate
-00004970: 6420 4348 4543 4b5f 4441 5441 2072 6573  d CHECK_DATA res
-00004980: 706f 6e73 6520 7072 6f74 6f62 7566 2222  ponse protobuf""
-00004990: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-000049a0: 2070 726f 746f 2e46 6574 6368 5379 7374   proto.FetchSyst
-000049b0: 656d 4d65 7461 6461 7461 5265 7370 6f6e  emMetadataRespon
-000049c0: 7365 2829 0a0a 0a22 2222 4d61 7070 696e  se()..."""Mappin
-000049d0: 6720 6672 6f6d 2071 7565 7279 2074 7970  g from query typ
-000049e0: 6520 746f 2069 7473 2072 6571 7565 7374  e to its request
-000049f0: 2066 6163 746f 7279 2222 220a 5f4f 4349   factory"""._OCI
-00004a00: 454e 545f 5245 5155 4553 545f 4641 4354  ENT_REQUEST_FACT
-00004a10: 4f52 4945 5320 3d20 7b0a 2020 2020 2253  ORIES = {.    "S
-00004a20: 454c 4543 5422 3a20 5f45 7865 6375 7465  ELECT": _Execute
-00004a30: 5175 6572 7946 6163 746f 7279 2829 2c0a  QueryFactory(),.
-00004a40: 2020 2020 2257 4954 4822 3a20 5f45 7865      "WITH": _Exe
-00004a50: 6375 7465 5175 6572 7946 6163 746f 7279  cuteQueryFactory
-00004a60: 2829 2c0a 2020 2020 2245 5850 4c41 494e  (),.    "EXPLAIN
-00004a70: 2050 4950 454c 494e 4522 3a20 5f45 7870   PIPELINE": _Exp
-00004a80: 6c61 696e 5069 7065 6c69 6e65 4661 6374  lainPipelineFact
-00004a90: 6f72 7928 292c 0a20 2020 2022 4558 504c  ory(),.    "EXPL
-00004aa0: 4149 4e22 3a20 5f45 7865 6375 7465 4578  AIN": _ExecuteEx
-00004ab0: 706c 6169 6e46 6163 746f 7279 2829 2c0a  plainFactory(),.
-00004ac0: 2020 2020 2245 5850 4f52 5422 3a20 5f45      "EXPORT": _E
-00004ad0: 7865 6375 7465 4578 706f 7274 4661 6374  xecuteExportFact
-00004ae0: 6f72 7928 292c 0a20 2020 2022 4348 4543  ory(),.    "CHEC
-00004af0: 4b22 3a20 5f43 6865 636b 4461 7461 4661  K": _CheckDataFa
-00004b00: 6374 6f72 7928 292c 0a20 2020 2022 464f  ctory(),.    "FO
-00004b10: 5243 4522 3a20 5f46 6f72 6365 4578 7465  RCE": _ForceExte
-00004b20: 726e 616c 4661 6374 6f72 7928 292c 0a20  rnalFactory(),. 
-00004b30: 2020 2022 5345 5420 5343 4845 4d41 223a     "SET SCHEMA":
-00004b40: 205f 5365 7453 6368 656d 6146 6163 746f   _SetSchemaFacto
-00004b50: 7279 2829 2c0a 2020 2020 2247 4554 2053  ry(),.    "GET S
-00004b60: 4348 454d 4122 3a20 5f47 6574 5363 6865  CHEMA": _GetSche
-00004b70: 6d61 4661 6374 6f72 7928 292c 0a20 2020  maFactory(),.   
-00004b80: 2022 434c 4541 5220 4341 4348 4522 3a20   "CLEAR CACHE": 
-00004b90: 5f43 6c65 6172 4361 6368 6546 6163 746f  _ClearCacheFacto
-00004ba0: 7279 2829 2c0a 2020 2020 2253 4554 223a  ry(),.    "SET":
-00004bb0: 205f 5365 7450 6172 616d 6574 6572 4661   _SetParameterFa
-00004bc0: 6374 6f72 7928 292c 0a20 2020 2022 4341  ctory(),.    "CA
-00004bd0: 4e43 454c 223a 205f 4361 6e63 656c 5175  NCEL": _CancelQu
-00004be0: 6572 7946 6163 746f 7279 2829 2c0a 2020  eryFactory(),.  
-00004bf0: 2020 224b 494c 4c22 3a20 5f4b 696c 6c51    "KILL": _KillQ
-00004c00: 7565 7279 4661 6374 6f72 7928 292c 0a20  ueryFactory(),. 
-00004c10: 2020 2022 4745 5420 5359 5354 454d 204d     "GET SYSTEM M
-00004c20: 4554 4144 4154 4122 3a20 5f47 6574 5379  ETADATA": _GetSy
-00004c30: 7374 656d 4d65 7461 6461 7461 4661 6374  stemMetadataFact
-00004c40: 6f72 7928 292c 0a7d 0a0a 0a64 6566 205f  ory(),.}...def _
-00004c50: 636f 6e76 6572 745f 6578 6365 7074 696f  convert_exceptio
-00004c60: 6e28 6d73 6729 3a0a 2020 2020 2222 2249  n(msg):.    """I
-00004c70: 6e74 6572 6e61 6c20 726f 7574 696e 6520  nternal routine 
-00004c80: 746f 2063 6f6e 7665 7274 2074 6865 2067  to convert the g
-00004c90: 6f6f 676c 6520 7072 6f74 6f62 7566 2043  oogle protobuf C
-00004ca0: 6f6e 6669 726d 6174 696f 6e52 6573 706f  onfirmationRespo
-00004cb0: 6e73 650a 2020 2020 746f 2061 6e20 6578  nse.    to an ex
-00004cc0: 6365 7074 696f 6e0a 2020 2020 2222 220a  ception.    """.
-00004cd0: 2020 2020 6966 206d 7367 2e76 656e 646f      if msg.vendo
-00004ce0: 725f 636f 6465 203c 2030 3a0a 2020 2020  r_code < 0:.    
-00004cf0: 2020 2020 7265 7475 726e 2045 7272 6f72      return Error
-00004d00: 2873 716c 5f73 7461 7465 3d6d 7367 2e73  (sql_state=msg.s
-00004d10: 716c 5f73 7461 7465 2c20 7265 6173 6f6e  ql_state, reason
-00004d20: 3d6d 7367 2e72 6561 736f 6e2c 2076 656e  =msg.reason, ven
-00004d30: 646f 725f 636f 6465 3d6d 7367 2e76 656e  dor_code=msg.ven
-00004d40: 646f 725f 636f 6465 290a 0a20 2020 2072  dor_code)..    r
-00004d50: 6574 7572 6e20 5761 726e 696e 6728 7371  eturn Warning(sq
-00004d60: 6c5f 7374 6174 653d 6d73 672e 7371 6c5f  l_state=msg.sql_
-00004d70: 7374 6174 652c 2072 6561 736f 6e3d 6d73  state, reason=ms
-00004d80: 672e 7265 6173 6f6e 2c20 7665 6e64 6f72  g.reason, vendor
-00004d90: 5f63 6f64 653d 6d73 672e 7665 6e64 6f72  _code=msg.vendor
-00004da0: 5f63 6f64 6529 0a0a 0a64 6566 205f 7365  _code)...def _se
-00004db0: 6e64 5f6d 7367 2863 6f6e 6e2c 2070 726f  nd_msg(conn, pro
-00004dc0: 746f 6275 665f 6d73 6729 3a0a 2020 2020  tobuf_msg):.    
-00004dd0: 2222 2249 6e74 6572 6e61 6c20 726f 7574  """Internal rout
-00004de0: 696e 6520 746f 2073 656e 6420 6120 7072  ine to send a pr
-00004df0: 6f74 6f62 7566 206d 6573 7361 6765 206f  otobuf message o
-00004e00: 6e20 6120 636f 6e6e 6563 7469 6f6e 2222  n a connection""
-00004e10: 220a 2020 2020 6966 206e 6f74 2063 6f6e  ".    if not con
-00004e20: 6e2e 736f 636b 3a0a 2020 2020 2020 2020  n.sock:.        
-00004e30: 7261 6973 6520 5072 6f67 7261 6d6d 696e  raise Programmin
-00004e40: 6745 7272 6f72 2822 436f 6e6e 6563 7469  gError("Connecti
-00004e50: 6f6e 206e 6f74 2061 7661 696c 6162 6c65  on not available
-00004e60: 2229 0a0a 2020 2020 6c6f 6767 6572 2e64  ")..    logger.d
-00004e70: 6562 7567 2866 2253 656e 6469 6e67 206d  ebug(f"Sending m
-00004e80: 6573 7361 6765 206f 6e20 736f 636b 6574  essage on socket
-00004e90: 207b 636f 6e6e 2e73 6f63 6b7d 3a20 7b70   {conn.sock}: {p
-00004ea0: 726f 746f 6275 665f 6d73 677d 2229 0a0a  rotobuf_msg}")..
-00004eb0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00004ec0: 2063 6f6e 6e2e 736f 636b 2e73 656e 6461   conn.sock.senda
-00004ed0: 6c6c 2873 7472 7563 742e 7061 636b 2822  ll(struct.pack("
-00004ee0: 2169 222c 2070 726f 746f 6275 665f 6d73  !i", protobuf_ms
-00004ef0: 672e 4279 7465 5369 7a65 2829 2920 2b20  g.ByteSize()) + 
-00004f00: 7072 6f74 6f62 7566 5f6d 7367 2e53 6572  protobuf_msg.Ser
-00004f10: 6961 6c69 7a65 546f 5374 7269 6e67 2829  ializeToString()
-00004f20: 290a 2020 2020 6578 6365 7074 2049 4f45  ).    except IOE
-00004f30: 7272 6f72 3a0a 2020 2020 2020 2020 7261  rror:.        ra
-00004f40: 6973 6520 494f 4572 726f 7228 224e 6574  ise IOError("Net
-00004f50: 776f 726b 2073 656e 6420 6572 726f 7222  work send error"
-00004f60: 290a 0a0a 6465 6620 5f72 6563 765f 616c  )...def _recv_al
-00004f70: 6c28 636f 6e6e 2c20 7369 7a65 293a 0a20  l(conn, size):. 
-00004f80: 2020 2022 2222 496e 7465 726e 616c 2072     """Internal r
-00004f90: 6f75 7469 6e65 2074 6f20 7265 6365 6976  outine to receiv
-00004fa0: 6520 6073 697a 6560 2062 7974 6573 206f  e `size` bytes o
-00004fb0: 6620 6461 7461 2066 726f 6d20 6120 636f  f data from a co
-00004fc0: 6e6e 6563 7469 6f6e 2222 220a 2020 2020  nnection""".    
-00004fd0: 6966 206e 6f74 2063 6f6e 6e2e 736f 636b  if not conn.sock
-00004fe0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-00004ff0: 4572 726f 7228 2243 6f6e 6e65 6374 696f  Error("Connectio
-00005000: 6e20 6e6f 7420 6176 6169 6c61 626c 6522  n not available"
-00005010: 290a 0a20 2020 2077 6869 6c65 206c 656e  )..    while len
-00005020: 2863 6f6e 6e2e 5f62 7566 6665 7229 203c  (conn._buffer) <
-00005030: 2073 697a 653a 0a20 2020 2020 2020 2072   size:.        r
-00005040: 6563 6569 7665 6420 3d20 636f 6e6e 2e73  eceived = conn.s
-00005050: 6f63 6b2e 7265 6376 2831 3637 3737 3231  ock.recv(1677721
-00005060: 3629 2020 2320 3136 4d42 2062 7566 6665  6)  # 16MB buffe
-00005070: 720a 2020 2020 2020 2020 6966 206e 6f74  r.        if not
-00005080: 2072 6563 6569 7665 643a 0a20 2020 2020   received:.     
-00005090: 2020 2020 2020 2072 6169 7365 2049 4f45         raise IOE
-000050a0: 7272 6f72 2822 4e65 7477 6f72 6b20 7265  rror("Network re
-000050b0: 6365 6976 6520 6572 726f 7222 290a 2020  ceive error").  
-000050c0: 2020 2020 2020 636f 6e6e 2e5f 6275 6666        conn._buff
-000050d0: 6572 202b 3d20 7265 6365 6976 6564 0a0a  er += received..
-000050e0: 2020 2020 7265 7420 3d20 636f 6e6e 2e5f      ret = conn._
-000050f0: 6275 6666 6572 5b3a 7369 7a65 5d0a 2020  buffer[:size].  
-00005100: 2020 636f 6e6e 2e5f 6275 6666 6572 203d    conn._buffer =
-00005110: 2063 6f6e 6e2e 5f62 7566 6665 725b 7369   conn._buffer[si
-00005120: 7a65 3a5d 0a0a 2020 2020 7265 7475 726e  ze:]..    return
-00005130: 2072 6574 0a0a 0a64 6566 205f 7265 6376   ret...def _recv
-00005140: 5f6d 7367 2863 6f6e 6e2c 2070 726f 746f  _msg(conn, proto
-00005150: 6275 665f 6d73 6729 3a0a 2020 2020 2222  buf_msg):.    ""
-00005160: 2249 6e74 6572 6e61 6c20 726f 7574 696e  "Internal routin
-00005170: 6520 746f 2072 6563 6569 7665 2061 2070  e to receive a p
-00005180: 726f 746f 6275 6620 6d65 7373 6167 6520  rotobuf message 
-00005190: 6f6e 2061 2063 6f6e 6e65 6374 696f 6e22  on a connection"
-000051a0: 2222 0a20 2020 2068 6472 203d 205f 7265  "".    hdr = _re
-000051b0: 6376 5f61 6c6c 2863 6f6e 6e2c 2034 290a  cv_all(conn, 4).
-000051c0: 2020 2020 6d73 6773 697a 6520 3d20 5f75      msgsize = _u
-000051d0: 6e70 6163 6b5f 696e 7428 6864 7229 5b30  npack_int(hdr)[0
-000051e0: 5d0a 0a20 2020 206d 7367 203d 205f 7265  ]..    msg = _re
-000051f0: 6376 5f61 6c6c 2863 6f6e 6e2c 206d 7367  cv_all(conn, msg
-00005200: 7369 7a65 290a 0a20 2020 2070 726f 746f  size)..    proto
-00005210: 6275 665f 6d73 672e 5061 7273 6546 726f  buf_msg.ParseFro
-00005220: 6d53 7472 696e 6728 6d73 6729 0a0a 2020  mString(msg)..  
-00005230: 2020 6c6f 6767 6572 2e64 6562 7567 2866    logger.debug(f
-00005240: 2252 6563 6569 7665 6420 6d65 7373 6167  "Received messag
-00005250: 6520 6f6e 2063 6f6e 6e65 6374 696f 6e20  e on connection 
-00005260: 7b63 6f6e 6e2e 736f 636b 7d3a 207b 7072  {conn.sock}: {pr
-00005270: 6f74 6f62 7566 5f6d 7367 7d22 290a 0a20  otobuf_msg}").. 
-00005280: 2020 2072 6574 7572 6e20 7072 6f74 6f62     return protob
-00005290: 7566 5f6d 7367 0a0a 0a64 6566 2044 6174  uf_msg...def Dat
-000052a0: 6528 7965 6172 2c20 6d6f 6e74 682c 2064  e(year, month, d
-000052b0: 6179 293a 2020 2320 7079 6c69 6e74 3a20  ay):  # pylint: 
-000052c0: 6469 7361 626c 653d 696e 7661 6c69 642d  disable=invalid-
-000052d0: 6e61 6d65 0a20 2020 2022 2222 5479 7065  name.    """Type
-000052e0: 2063 6f6e 7374 7275 6374 6f72 2072 6571   constructor req
-000052f0: 7569 7265 6420 696e 2050 4550 2032 3439  uired in PEP 249
-00005300: 2074 6f20 636f 6e73 7472 7563 7420 610a   to construct a.
-00005310: 2020 2020 4461 7465 206f 626a 6563 7420      Date object 
-00005320: 6672 6f6d 2079 6561 722c 206d 6f6e 7468  from year, month
-00005330: 2c20 6461 790a 2020 2020 2222 220a 2020  , day.    """.  
-00005340: 2020 7265 7475 726e 2064 6174 6574 696d    return datetim
-00005350: 652e 6461 7465 7469 6d65 2879 6561 722c  e.datetime(year,
-00005360: 206d 6f6e 7468 2c20 6461 7929 0a0a 0a64   month, day)...d
-00005370: 6566 2054 696d 6528 686f 7572 2c20 6d69  ef Time(hour, mi
-00005380: 6e75 7465 2c20 7365 636f 6e64 293a 2020  nute, second):  
-00005390: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
-000053a0: 653d 696e 7661 6c69 642d 6e61 6d65 0a20  e=invalid-name. 
-000053b0: 2020 2022 2222 5479 7065 2063 6f6e 7374     """Type const
-000053c0: 7275 6374 6f72 2072 6571 7569 7265 6420  ructor required 
-000053d0: 696e 2050 4550 2032 3439 2074 6f20 636f  in PEP 249 to co
-000053e0: 6e73 7472 7563 7420 610a 2020 2020 5469  nstruct a.    Ti
-000053f0: 6d65 206f 626a 6563 7420 6672 6f6d 2068  me object from h
-00005400: 6f75 722c 206d 696e 7574 652c 2073 6563  our, minute, sec
-00005410: 6f6e 640a 2020 2020 2222 220a 2020 2020  ond.    """.    
-00005420: 7265 7475 726e 2064 6174 6574 696d 652e  return datetime.
-00005430: 7469 6d65 2868 6f75 722c 206d 696e 7574  time(hour, minut
-00005440: 652c 2073 6563 6f6e 6429 0a0a 0a64 6566  e, second)...def
-00005450: 2054 696d 6573 7461 6d70 2879 6561 722c   Timestamp(year,
-00005460: 206d 6f6e 7468 2c20 6461 792c 2068 6f75   month, day, hou
-00005470: 722c 206d 696e 7574 652c 2073 6563 6f6e  r, minute, secon
-00005480: 6429 3a20 2023 2070 796c 696e 743a 2064  d):  # pylint: d
-00005490: 6973 6162 6c65 3d69 6e76 616c 6964 2d6e  isable=invalid-n
-000054a0: 616d 652c 746f 6f2d 6d61 6e79 2d61 7267  ame,too-many-arg
-000054b0: 756d 656e 7473 0a20 2020 2022 2222 5479  uments.    """Ty
-000054c0: 7065 2063 6f6e 7374 7275 6374 6f72 2072  pe constructor r
-000054d0: 6571 7569 7265 6420 696e 2050 4550 2032  equired in PEP 2
-000054e0: 3439 2074 6f20 636f 6e73 7472 7563 740a  49 to construct.
-000054f0: 2020 2020 6120 5469 6d65 7374 616d 7020      a Timestamp 
-00005500: 6f62 6a65 6374 2066 726f 6d20 7965 6172  object from year
-00005510: 2c20 6d6f 6e74 682c 2064 6179 2c20 686f  , month, day, ho
-00005520: 7572 2c20 6d69 6e75 7465 2c20 7365 636f  ur, minute, seco
-00005530: 6e64 0a20 2020 2022 2222 0a20 2020 2072  nd.    """.    r
-00005540: 6574 7572 6e20 6461 7465 7469 6d65 2e64  eturn datetime.d
-00005550: 6174 6574 696d 6528 7965 6172 2c20 6d6f  atetime(year, mo
-00005560: 6e74 682c 2064 6179 2c20 686f 7572 2c20  nth, day, hour, 
-00005570: 6d69 6e75 7465 2c20 7365 636f 6e64 292e  minute, second).
-00005580: 7469 6d65 7374 616d 7028 290a 0a0a 6465  timestamp()...de
-00005590: 6620 4461 7465 4672 6f6d 5469 636b 7328  f DateFromTicks(
-000055a0: 7469 636b 7329 3a20 2023 2070 796c 696e  ticks):  # pylin
-000055b0: 743a 2064 6973 6162 6c65 3d69 6e76 616c  t: disable=inval
-000055c0: 6964 2d6e 616d 650a 2020 2020 2222 2254  id-name.    """T
-000055d0: 7970 6520 636f 6e73 7472 7563 746f 7220  ype constructor 
-000055e0: 7265 7175 6972 6564 2069 6e20 5045 5020  required in PEP 
-000055f0: 3234 3920 746f 2063 6f6e 7374 7275 6374  249 to construct
-00005600: 0a20 2020 2061 2044 6174 6520 6f62 6a65  .    a Date obje
-00005610: 6374 2066 726f 6d20 6120 7469 6d65 7374  ct from a timest
-00005620: 616d 7020 6f66 2073 6563 6f6e 6473 2073  amp of seconds s
-00005630: 696e 6365 2065 706f 6368 0a20 2020 2022  ince epoch.    "
-00005640: 2222 0a20 2020 2072 6574 7572 6e20 6461  "".    return da
-00005650: 7465 7469 6d65 2e64 6174 6574 696d 652e  tetime.datetime.
-00005660: 7574 6366 726f 6d74 696d 6573 7461 6d70  utcfromtimestamp
-00005670: 2874 6963 6b73 290a 0a0a 6465 6620 5469  (ticks)...def Ti
-00005680: 6d65 4672 6f6d 5469 636b 7328 7469 636b  meFromTicks(tick
-00005690: 7329 3a20 2023 2070 796c 696e 743a 2064  s):  # pylint: d
-000056a0: 6973 6162 6c65 3d69 6e76 616c 6964 2d6e  isable=invalid-n
-000056b0: 616d 650a 2020 2020 2222 2254 7970 6520  ame.    """Type 
-000056c0: 636f 6e73 7472 7563 746f 7220 7265 7175  constructor requ
-000056d0: 6972 6564 2069 6e20 5045 5020 3234 3920  ired in PEP 249 
-000056e0: 746f 2063 6f6e 7374 7275 6374 0a20 2020  to construct.   
-000056f0: 2061 2054 696d 6520 6f62 6a65 6374 2066   a Time object f
-00005700: 726f 6d20 6120 7469 6d65 7374 616d 7020  rom a timestamp 
-00005710: 6f66 2073 6563 6f6e 6473 2073 696e 6365  of seconds since
-00005720: 2065 706f 6368 0a20 2020 2022 2222 0a20   epoch.    """. 
-00005730: 2020 2064 6174 655f 7469 6d65 203d 2064     date_time = d
-00005740: 6174 6574 696d 652e 6461 7465 7469 6d65  atetime.datetime
-00005750: 2e75 7463 6672 6f6d 7469 6d65 7374 616d  .utcfromtimestam
-00005760: 7028 7469 636b 7329 0a20 2020 2072 6574  p(ticks).    ret
-00005770: 7572 6e20 6461 7465 7469 6d65 2e74 696d  urn datetime.tim
-00005780: 6528 6461 7465 5f74 696d 652e 686f 7572  e(date_time.hour
-00005790: 2c20 6461 7465 5f74 696d 652e 6d69 6e75  , date_time.minu
-000057a0: 7465 2c20 6461 7465 5f74 696d 652e 7365  te, date_time.se
-000057b0: 636f 6e64 290a 0a0a 6465 6620 5469 6d65  cond)...def Time
-000057c0: 7374 616d 7046 726f 6d54 6963 6b73 2874  stampFromTicks(t
-000057d0: 6963 6b73 293a 2020 2320 7079 6c69 6e74  icks):  # pylint
-000057e0: 3a20 6469 7361 626c 653d 696e 7661 6c69  : disable=invali
-000057f0: 642d 6e61 6d65 0a20 2020 2022 2222 5479  d-name.    """Ty
-00005800: 7065 2063 6f6e 7374 7275 6374 6f72 2072  pe constructor r
-00005810: 6571 7569 7265 6420 696e 2050 4550 2032  equired in PEP 2
-00005820: 3439 2074 6f20 636f 6e73 7472 7563 740a  49 to construct.
-00005830: 2020 2020 6120 5469 6d65 7374 616d 7020      a Timestamp 
-00005840: 6f62 6a65 6374 2066 726f 6d20 6120 7469  object from a ti
-00005850: 6d65 7374 616d 7020 6f66 2073 6563 6f6e  mestamp of secon
-00005860: 6473 2073 696e 6365 2065 706f 6368 0a20  ds since epoch. 
-00005870: 2020 2022 2222 0a20 2020 2072 6574 7572     """.    retur
-00005880: 6e20 7469 636b 730a 0a0a 6465 6620 5f68  n ticks...def _h
-00005890: 6173 685f 6b65 7928 7368 6172 6564 5f6b  ash_key(shared_k
-000058a0: 6579 2c20 7361 6c74 293a 0a20 2020 2022  ey, salt):.    "
-000058b0: 2222 496e 7465 726e 616c 206b 6579 2068  ""Internal key h
-000058c0: 6173 6820 6675 6e63 7469 6f6e 2222 220a  ash function""".
-000058d0: 2020 2020 2320 4e6f 2069 6465 6120 7768      # No idea wh
-000058e0: 6572 6520 7468 6973 2061 6c67 6f72 6974  ere this algorit
-000058f0: 686d 2063 616d 6520 6672 6f6d 2c20 6275  hm came from, bu
-00005900: 7420 646f 2061 2068 6f6d 6520 6772 6f77  t do a home grow
-00005910: 6e20 6b65 790a 2020 2020 2320 6465 7269  n key.    # deri
-00005920: 7661 7469 6f6e 2066 756e 6374 696f 6e0a  vation function.
-00005930: 2020 2020 6275 6666 6572 203d 2073 7472      buffer = str
-00005940: 7563 742e 7061 636b 2822 2169 222c 206c  uct.pack("!i", l
-00005950: 656e 2873 6861 7265 645f 6b65 7929 290a  en(shared_key)).
-00005960: 2020 2020 6275 6666 6572 203d 2062 7566      buffer = buf
-00005970: 6665 7220 2b20 7361 6c74 0a20 2020 2062  fer + salt.    b
-00005980: 7566 6665 7220 3d20 6275 6666 6572 202b  uffer = buffer +
-00005990: 2073 6861 7265 645f 6b65 790a 2020 2020   shared_key.    
-000059a0: 6861 7368 6572 203d 2068 6173 6865 732e  hasher = hashes.
-000059b0: 4861 7368 2868 6173 6865 732e 5348 4132  Hash(hashes.SHA2
-000059c0: 3536 2829 2c20 6261 636b 656e 643d 6465  56(), backend=de
-000059d0: 6661 756c 745f 6261 636b 656e 6428 2929  fault_backend())
-000059e0: 0a20 2020 2068 6173 6865 722e 7570 6461  .    hasher.upda
-000059f0: 7465 2862 7566 6665 7229 0a20 2020 2072  te(buffer).    r
-00005a00: 6574 7572 6e20 6861 7368 6572 2e66 696e  eturn hasher.fin
-00005a10: 616c 697a 6528 290a 0a0a 2320 5365 7373  alize()...# Sess
-00005a20: 696f 6e73 2063 6f64 650a 0a23 2055 7365  ions code..# Use
-00005a30: 6420 666f 7220 7265 7072 6573 656e 7469  d for representi
-00005a40: 6e67 2061 2073 6573 7369 6f6e 2063 7265  ng a session cre
-00005a50: 6174 6564 2077 6974 6820 6120 7365 6375  ated with a secu
-00005a60: 7269 7479 2074 6f6b 656e 2073 6967 6e20  rity token sign 
-00005a70: 696e 0a0a 0a63 6c61 7373 2053 6563 7572  in...class Secur
-00005a80: 6974 7954 6f6b 656e 3a0a 2020 2020 6465  ityToken:.    de
-00005a90: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-00005aa0: 2074 6f6b 656e 4461 7461 3a20 7374 722c   tokenData: str,
-00005ab0: 2074 6f6b 656e 5369 676e 6174 7572 653a   tokenSignature:
-00005ac0: 2073 7472 2c20 6973 7375 6572 4669 6e67   str, issuerFing
-00005ad0: 6572 7072 696e 743a 2073 7472 293a 0a20  erprint: str):. 
-00005ae0: 2020 2020 2020 2073 656c 662e 746f 6b65         self.toke
-00005af0: 6e44 6174 6120 3d20 746f 6b65 6e44 6174  nData = tokenDat
-00005b00: 610a 2020 2020 2020 2020 7365 6c66 2e74  a.        self.t
-00005b10: 6f6b 656e 5369 676e 6174 7572 6520 3d20  okenSignature = 
-00005b20: 746f 6b65 6e53 6967 6e61 7475 7265 0a20  tokenSignature. 
-00005b30: 2020 2020 2020 2073 656c 662e 6973 7375         self.issu
-00005b40: 6572 4669 6e67 6572 7072 696e 7420 3d20  erFingerprint = 
-00005b50: 6973 7375 6572 4669 6e67 6572 7072 696e  issuerFingerprin
-00005b60: 740a 0a0a 2320 5573 6564 2066 6f72 2072  t...# Used for r
-00005b70: 6570 7265 7365 6e74 696e 6720 6120 7365  epresenting a se
-00005b80: 7373 696f 6e20 6372 6561 7465 6420 7769  ssion created wi
-00005b90: 7468 2061 2075 7365 7220 616e 6420 7061  th a user and pa
-00005ba0: 7373 776f 7264 2073 6967 6e20 696e 2e0a  ssword sign in..
-00005bb0: 0a0a 636c 6173 7320 5573 6572 416e 6450  ..class UserAndP
-00005bc0: 6173 7377 6f72 643a 0a20 2020 2064 6566  assword:.    def
-00005bd0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00005be0: 7573 6572 3a20 7374 722c 2070 6173 7377  user: str, passw
-00005bf0: 6f72 643a 2073 7472 293a 0a20 2020 2020  ord: str):.     
-00005c00: 2020 2073 656c 662e 7573 6572 203d 2075     self.user = u
-00005c10: 7365 720a 2020 2020 2020 2020 7365 6c66  ser.        self
-00005c20: 2e70 6173 7377 6f72 6420 3d20 7061 7373  .password = pass
-00005c30: 776f 7264 0a0a 0a63 6c61 7373 2053 6573  word...class Ses
-00005c40: 7369 6f6e 3a0a 2020 2020 6465 6620 5f5f  sion:.    def __
-00005c50: 696e 6974 5f5f 2873 656c 662c 2073 6563  init__(self, sec
-00005c60: 7572 6974 7954 6f6b 656e 3d4e 6f6e 652c  urityToken=None,
-00005c70: 2075 7365 7241 6e64 5061 7373 776f 7264   userAndPassword
-00005c80: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-00005c90: 2320 4f6e 6c79 206f 6e65 206f 6620 7468  # Only one of th
-00005ca0: 6573 6520 7368 6f75 6c64 2062 6520 696e  ese should be in
-00005cb0: 7374 616e 7469 6174 6564 2e20 5468 6520  stantiated. The 
-00005cc0: 6f74 6865 7220 4d55 5354 2062 6520 6e6f  other MUST be no
-00005cd0: 6e65 2e0a 2020 2020 2020 2020 7365 6c66  ne..        self
-00005ce0: 2e73 6563 7572 6974 7954 6f6b 656e 203d  .securityToken =
-00005cf0: 2073 6563 7572 6974 7954 6f6b 656e 0a20   securityToken. 
-00005d00: 2020 2020 2020 2073 656c 662e 7573 6572         self.user
-00005d10: 416e 6450 6173 7377 6f72 6420 3d20 7573  AndPassword = us
-00005d20: 6572 416e 6450 6173 7377 6f72 640a 0a0a  erAndPassword...
-00005d30: 636c 6173 7320 436f 6e6e 6563 7469 6f6e  class Connection
-00005d40: 3a0a 2020 2020 2222 2241 2063 6f6e 6e65  :.    """A conne
-00005d50: 6374 696f 6e20 746f 2074 6865 204f 6369  ction to the Oci
-00005d60: 656e 7420 6461 7461 6261 7365 2e20 4e6f  ent database. No
-00005d70: 726d 616c 6c79 2063 6f6e 7374 7275 6374  rmally construct
-00005d80: 6564 2062 790a 2020 2020 6361 6c6c 696e  ed by.    callin
-00005d90: 6720 7468 6520 6d6f 6475 6c65 2060 636f  g the module `co
-00005da0: 6e6e 6563 7428 2960 2063 616c 6c2c 2062  nnect()` call, b
-00005db0: 7574 2063 616e 2062 6520 636f 6e73 7472  ut can be constr
-00005dc0: 7563 7465 640a 2020 2020 6469 7265 6374  ucted.    direct
-00005dd0: 6c79 0a20 2020 2022 2222 0a0a 2020 2020  ly.    """..    
-00005de0: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
-00005df0: 653d 746f 6f2d 6d61 6e79 2d69 6e73 7461  e=too-many-insta
-00005e00: 6e63 652d 6174 7472 6962 7574 6573 0a20  nce-attributes. 
-00005e10: 2020 2054 4c53 5f4e 4f4e 4520 3d20 3120     TLS_NONE = 1 
-00005e20: 2023 203a 203a 6d65 7461 2070 7269 7661   # : :meta priva
-00005e30: 7465 3a0a 2020 2020 544c 535f 554e 5645  te:.    TLS_UNVE
-00005e40: 5249 4649 4544 203d 2032 2020 2320 3a20  RIFIED = 2  # : 
-00005e50: 3a6d 6574 6120 7072 6976 6174 653a 0a20  :meta private:. 
-00005e60: 2020 2054 4c53 5f4f 4e20 3d20 3320 2023     TLS_ON = 3  #
-00005e70: 203a 203a 6d65 7461 2070 7269 7661 7465   : :meta private
-00005e80: 3a0a 0a20 2020 2048 414e 4453 4841 4b45  :..    HANDSHAKE
-00005e90: 5f43 4243 203d 2031 0a20 2020 2048 414e  _CBC = 1.    HAN
-00005ea0: 4453 4841 4b45 5f47 434d 203d 2032 0a20  DSHAKE_GCM = 2. 
-00005eb0: 2020 2048 414e 4453 4841 4b45 5f53 534f     HANDSHAKE_SSO
-00005ec0: 203d 2033 0a0a 2020 2020 4445 4641 554c   = 3..    DEFAUL
-00005ed0: 545f 484f 5354 203d 2022 6c6f 6361 6c68  T_HOST = "localh
-00005ee0: 6f73 7422 0a20 2020 2044 4546 4155 4c54  ost".    DEFAULT
-00005ef0: 5f50 4f52 5420 3d20 3430 3530 0a20 2020  _PORT = 4050.   
-00005f00: 2044 4546 4155 4c54 5f44 4154 4142 4153   DEFAULT_DATABAS
-00005f10: 4520 3d20 2273 7973 7465 6d22 0a0a 2020  E = "system"..  
-00005f20: 2020 686f 7374 7320 3d20 5b5d 0a20 2020    hosts = [].   
-00005f30: 2070 6f72 7420 3d20 4e6f 6e65 0a20 2020   port = None.   
-00005f40: 2064 6174 6162 6173 6520 3d20 4e6f 6e65   database = None
-00005f50: 0a20 2020 2074 6c73 203d 204e 6f6e 650a  .    tls = None.
-00005f60: 2020 2020 666f 7263 6520 3d20 4e6f 6e65      force = None
-00005f70: 0a20 2020 2068 616e 6473 6861 6b65 203d  .    handshake =
-00005f80: 204e 6f6e 650a 2020 2020 7573 6572 203d   None.    user =
-00005f90: 204e 6f6e 650a 2020 2020 7061 7373 776f   None.    passwo
-00005fa0: 7264 203d 204e 6f6e 650a 2020 2020 7365  rd = None.    se
-00005fb0: 636f 6e64 6172 795f 696e 7465 7266 6163  condary_interfac
-00005fc0: 6573 203d 204e 6f6e 650a 2020 2020 7365  es = None.    se
-00005fd0: 636f 6e64 6172 795f 696e 6465 7820 3d20  condary_index = 
-00005fe0: 2d31 0a20 2020 2073 6f63 6b20 3d20 4e6f  -1.    sock = No
-00005ff0: 6e65 0a20 2020 2073 6573 7369 6f6e 5f69  ne.    session_i
-00006000: 6420 3d20 7374 7228 7575 6964 2e75 7569  d = str(uuid.uui
-00006010: 6431 2829 290a 0a20 2020 2073 6573 7369  d1())..    sessi
-00006020: 6f6e 203d 204e 6f6e 650a 2020 2020 7365  on = None.    se
-00006030: 7276 6572 5365 7373 696f 6e49 6420 3d20  rverSessionId = 
-00006040: 4e6f 6e65 0a0a 2020 2020 2320 5768 6574  None..    # Whet
-00006050: 6865 7220 7468 6520 6e65 7874 2065 7865  her the next exe
-00006060: 6375 7465 2071 7565 7279 2072 756e 206f  cute query run o
-00006070: 6e20 7468 6973 2063 6f6e 6e65 6374 696f  n this connectio
-00006080: 6e20 7769 6c6c 2062 6520 7265 6469 7265  n will be redire
-00006090: 6374 6564 2e20 446f 6573 206e 6f74 6869  cted. Does nothi
-000060a0: 6e67 2069 6620 666f 7263 6520 6973 2073  ng if force is s
-000060b0: 6574 2074 6f20 7472 7565 0a20 2020 2066  et to true.    f
-000060c0: 6f72 6365 5f6e 6578 745f 7265 6469 7265  orce_next_redire
-000060d0: 6374 203d 2046 616c 7365 0a0a 2020 2020  ct = False..    
-000060e0: 2320 5365 7373 696f 6e73 2063 6f64 6520  # Sessions code 
-000060f0: 656e 640a 0a20 2020 2023 2074 6865 2050  end..    # the P
-00006100: 4550 2032 3439 2073 7461 6e64 6172 6420  EP 249 standard 
-00006110: 7265 636f 6d6d 656e 6473 206d 616b 696e  recommends makin
-00006120: 6720 7468 6520 6d6f 6475 6c65 206c 6576  g the module lev
-00006130: 656c 2065 7863 6570 7469 6f6e 730a 2020  el exceptions.  
-00006140: 2020 2320 616c 736f 2061 7474 7269 6275    # also attribu
-00006150: 7465 7320 6f6e 2074 6865 2043 6f6e 6e65  tes on the Conne
-00006160: 6374 696f 6e20 636c 6173 730a 2020 2020  ction class.    
-00006170: 4572 726f 7220 3d20 4572 726f 720a 2020  Error = Error.  
-00006180: 2020 5761 726e 696e 6720 3d20 5761 726e    Warning = Warn
-00006190: 696e 670a 2020 2020 496e 7465 7266 6163  ing.    Interfac
-000061a0: 6545 7272 6f72 203d 2049 6e74 6572 6661  eError = Interfa
-000061b0: 6365 4572 726f 720a 2020 2020 4461 7461  ceError.    Data
-000061c0: 6261 7365 4572 726f 7220 3d20 4461 7461  baseError = Data
-000061d0: 6261 7365 4572 726f 720a 2020 2020 496e  baseError.    In
-000061e0: 7465 726e 616c 4572 726f 7220 3d20 496e  ternalError = In
-000061f0: 7465 726e 616c 4572 726f 720a 2020 2020  ternalError.    
-00006200: 4f70 6572 6174 696f 6e61 6c45 7272 6f72  OperationalError
-00006210: 203d 204f 7065 7261 7469 6f6e 616c 4572   = OperationalEr
-00006220: 726f 720a 2020 2020 5072 6f67 7261 6d6d  ror.    Programm
-00006230: 696e 6745 7272 6f72 203d 2050 726f 6772  ingError = Progr
-00006240: 616d 6d69 6e67 4572 726f 720a 2020 2020  ammingError.    
-00006250: 496e 7465 6772 6974 7945 7272 6f72 203d  IntegrityError =
-00006260: 2049 6e74 6567 7269 7479 4572 726f 720a   IntegrityError.
-00006270: 2020 2020 4461 7461 4572 726f 7220 3d20      DataError = 
-00006280: 4461 7461 4572 726f 720a 2020 2020 4e6f  DataError.    No
-00006290: 7453 7570 706f 7274 6564 4572 726f 7220  tSupportedError 
-000062a0: 3d20 4e6f 7453 7570 706f 7274 6564 4572  = NotSupportedEr
-000062b0: 726f 720a 0a20 2020 2064 6566 205f 7373  ror..    def _ss
-000062c0: 6c69 7a65 5f63 6f6e 6e65 6374 696f 6e28  lize_connection(
-000062d0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-000062e0: 2222 0a20 2020 2020 2020 2049 6620 5353  "".        If SS
-000062f0: 4c20 6973 2073 7065 6369 6669 6564 2c20  L is specified, 
-00006300: 7772 6170 2074 6865 2073 6f63 6b65 7420  wrap the socket 
-00006310: 696e 2061 6e20 5353 4c20 636f 6e6e 6563  in an SSL connec
-00006320: 7469 6f6e 0a20 2020 2020 2020 2022 2222  tion.        """
-00006330: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00006340: 2e74 6c73 2021 3d20 7365 6c66 2e54 4c53  .tls != self.TLS
-00006350: 5f4e 4f4e 453a 0a20 2020 2020 2020 2020  _NONE:.         
-00006360: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-00006370: 2243 7265 6174 696e 6720 544c 5320 636f  "Creating TLS co
-00006380: 6e6e 6563 7469 6f6e 2229 0a20 2020 2020  nnection").     
-00006390: 2020 2020 2020 2063 6f6e 7465 7874 203d         context =
-000063a0: 2073 736c 2e63 7265 6174 655f 6465 6661   ssl.create_defa
-000063b0: 756c 745f 636f 6e74 6578 7428 290a 2020  ult_context().  
-000063c0: 2020 2020 2020 2020 2020 636f 6e74 6578            contex
-000063d0: 742e 6368 6563 6b5f 686f 7374 6e61 6d65  t.check_hostname
-000063e0: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
-000063f0: 2020 2020 2069 6620 7365 6c66 2e74 6c73       if self.tls
-00006400: 2021 3d20 7365 6c66 2e54 4c53 5f4f 4e3a   != self.TLS_ON:
-00006410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006420: 2063 6f6e 7465 7874 2e76 6572 6966 795f   context.verify_
-00006430: 6d6f 6465 203d 2073 736c 2e43 4552 545f  mode = ssl.CERT_
-00006440: 4e4f 4e45 0a20 2020 2020 2020 2020 2020  NONE.           
-00006450: 2073 656c 662e 736f 636b 203d 2063 6f6e   self.sock = con
-00006460: 7465 7874 2e77 7261 705f 736f 636b 6574  text.wrap_socket
-00006470: 2873 656c 662e 736f 636b 290a 0a20 2020  (self.sock)..   
-00006480: 2023 204e 6f74 6520 7468 6174 2074 6865   # Note that the
-00006490: 7265 2061 7265 2061 2063 6f75 706c 6520  re are a couple 
-000064a0: 6f66 2070 6c61 6365 7320 696e 2074 6865  of places in the
-000064b0: 2063 6f64 6520 7768 6572 6520 7765 2072   code where we r
-000064c0: 6563 6f6e 7374 7275 6374 2074 6865 2043  econstruct the C
-000064d0: 6f6e 6e65 6374 696f 6e2e 2020 4966 2079  onnection.  If y
-000064e0: 6f75 2061 6464 2061 2070 6172 616d 6574  ou add a paramet
-000064f0: 6572 2068 6572 652c 206d 616b 6520 7375  er here, make su
-00006500: 7265 2074 6f20 7570 6461 7465 2074 686f  re to update tho
-00006510: 7365 0a20 2020 2023 2070 6c61 6365 730a  se.    # places.
-00006520: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00006530: 2873 656c 662c 2064 736e 3d4e 6f6e 652c  (self, dsn=None,
-00006540: 2075 7365 723d 4e6f 6e65 2c20 7061 7373   user=None, pass
-00006550: 776f 7264 3d4e 6f6e 652c 2068 6f73 743d  word=None, host=
-00006560: 4e6f 6e65 2c20 6461 7461 6261 7365 3d4e  None, database=N
-00006570: 6f6e 652c 2074 6c73 3d4e 6f6e 652c 2068  one, tls=None, h
-00006580: 616e 6473 6861 6b65 3d4e 6f6e 652c 2066  andshake=None, f
-00006590: 6f72 6365 3d4e 6f6e 652c 2063 6f6e 6669  orce=None, confi
-000065a0: 6766 696c 653d 4e6f 6e65 2c20 7365 7373  gfile=None, sess
-000065b0: 696f 6e3d 4e6f 6e65 293a 0a20 2020 2020  ion=None):.     
-000065c0: 2020 2023 2070 796c 696e 743a 2064 6973     # pylint: dis
-000065d0: 6162 6c65 3d74 6f6f 2d6d 616e 792d 6172  able=too-many-ar
-000065e0: 6775 6d65 6e74 732c 6e6f 2d6d 656d 6265  guments,no-membe
-000065f0: 720a 2020 2020 2020 2020 2222 2243 6f6e  r.        """Con
-00006600: 6e65 6374 696f 6e20 7061 7261 6d65 7465  nection paramete
-00006610: 7273 2063 616e 2062 6520 7370 6563 6966  rs can be specif
-00006620: 6965 6420 6173 2070 6172 7420 6f66 2074  ied as part of t
-00006630: 6865 2064 736e 2c0a 2020 2020 2020 2020  he dsn,.        
-00006640: 7573 696e 6720 6b65 7977 6f72 6420 6172  using keyword ar
-00006650: 6775 6d65 6e74 7320 6f72 2062 6f74 682e  guments or both.
-00006660: 2020 4966 2062 6f74 6820 6172 6520 7370    If both are sp
-00006670: 6563 6966 6965 642c 2074 6865 206b 6579  ecified, the key
-00006680: 776f 7264 0a20 2020 2020 2020 2070 6172  word.        par
-00006690: 616d 6574 6572 206f 7665 7272 6964 6573  ameter overrides
-000066a0: 2074 6865 2076 616c 7565 2069 6e20 7468   the value in th
-000066b0: 6520 6473 6e2e 0a0a 2020 2020 2020 2020  e dsn...        
-000066c0: 5468 6520 4f63 6965 6e74 2044 534e 2069  The Ocient DSN i
-000066d0: 7320 6f66 2074 6865 2066 6f72 6d61 743a  s of the format:
-000066e0: 0a20 2020 2020 2020 2060 6f63 6965 6e74  .        `ocient
-000066f0: 3a2f 2f75 7365 723a 7061 7373 776f 7264  ://user:password
-00006700: 405b 686f 7374 5d5b 3a70 6f72 745d 5b2f  @[host][:port][/
-00006710: 6461 7461 6261 7365 5d5b 3f70 6172 616d  database][?param
-00006720: 313d 7661 6c75 6531 262e 2e2e 5d60 0a0a  1=value1&...]`..
-00006730: 2020 2020 2020 2020 6075 7365 7260 2061          `user` a
-00006740: 6e64 2060 7061 7373 776f 7264 6020 6d75  nd `password` mu
-00006750: 7374 2062 6520 7375 7070 6c69 6564 2e20  st be supplied. 
-00006760: 2060 686f 7374 6020 6465 6661 756c 7473   `host` defaults
-00006770: 2074 6f20 6c6f 6361 6c68 6f73 742c 0a20   to localhost,. 
-00006780: 2020 2020 2020 2070 6f72 7420 6465 6661         port defa
-00006790: 756c 7473 2074 6f20 3430 3530 2c20 6461  ults to 4050, da
-000067a0: 7461 6261 7365 2064 6566 6175 6c74 7320  tabase defaults 
-000067b0: 746f 2060 7379 7374 656d 6020 616e 6420  to `system` and 
-000067c0: 6074 6c73 6020 6465 6661 756c 7473 0a20  `tls` defaults. 
-000067d0: 2020 2020 2020 2074 6f20 606f 6666 602e         to `off`.
-000067e0: 0a0a 2020 2020 2020 2020 4d75 6c74 6970  ..        Multip
-000067f0: 6c65 2068 6f73 7473 206d 6179 2062 6520  le hosts may be 
-00006800: 7370 6563 6966 6965 642c 2073 6570 6172  specified, separ
-00006810: 6174 6564 2062 7920 6120 636f 6d6d 612c  ated by a comma,
-00006820: 2069 6e20 7768 6963 6820 6361 7365 2074   in which case t
-00006830: 6865 0a20 2020 2020 2020 2068 6f73 7473  he.        hosts
-00006840: 2077 696c 6c20 6265 2074 7269 6564 2069   will be tried i
-00006850: 6e20 6f72 6465 7220 2054 6875 7320 616e  n order  Thus an
-00006860: 2065 7861 6d70 6c65 2044 534e 206d 6967   example DSN mig
-00006870: 6874 2062 650a 2020 2020 2020 2020 606f  ht be.        `o
-00006880: 6369 656e 743a 2f2f 736f 6d65 6f6e 653a  cient://someone:
-00006890: 736f 6d65 7061 7373 776f 7264 4068 6f73  somepassword@hos
-000068a0: 7431 2c68 6f73 7432 3a34 3035 312f 6d79  t1,host2:4051/my
-000068b0: 6462 600a 0a20 2020 2020 2020 2063 6f6e  db`..        con
-000068c0: 6669 6766 696c 6520 6973 2074 6865 206e  figfile is the n
-000068d0: 616d 6520 6f66 2061 2063 6f6e 6669 6775  ame of a configu
-000068e0: 7261 7469 6f6e 2066 696c 6520 696e 2049  ration file in I
-000068f0: 4e49 2066 6f72 6d61 742c 2077 6865 7265  NI format, where
-00006900: 2065 6163 680a 2020 2020 2020 2020 7365   each.        se
-00006910: 6374 696f 6e20 6973 2065 6974 6865 7220  ction is either 
-00006920: 6465 6661 756c 742c 206f 7220 6120 7061  default, or a pa
-00006930: 7474 6572 6e20 7468 6174 206d 6174 6368  ttern that match
-00006940: 6573 2074 6865 2068 6f73 7420 616e 6420  es the host and 
-00006950: 6f70 7469 6f6e 616c 6c79 0a20 2020 2020  optionally.     
-00006960: 2020 2064 6174 6162 6173 652e 2073 6563     database. sec
-00006970: 7469 6f6e 7320 6172 6520 6d61 7463 6865  tions are matche
-00006980: 6420 696e 206f 7264 6572 2c20 736f 206d  d in order, so m
-00006990: 6f72 6520 7370 6563 6966 6963 2073 6563  ore specific sec
-000069a0: 7469 6f6e 7320 7368 6f75 6c64 0a20 2020  tions should.   
-000069b0: 2020 2020 2070 7265 6365 6465 206c 6573       precede les
-000069c0: 7320 7370 6563 6966 6963 2073 6563 7469  s specific secti
-000069d0: 6f6e 733a 3a0a 0a20 2020 2020 2020 2020  ons::..         
-000069e0: 2020 205b 4445 4641 554c 545d 0a20 2020     [DEFAULT].   
-000069f0: 2020 2020 2020 2020 2074 6c73 203d 2075           tls = u
-00006a00: 6e76 6572 6966 6965 640a 0a20 2020 2020  nverified..     
-00006a10: 2020 2020 2020 2023 2054 6869 7320 7769         # This wi
-00006a20: 6c6c 206d 6174 6368 2074 6865 2073 7065  ll match the spe
-00006a30: 6369 6669 6320 686f 7374 2061 6e64 2064  cific host and d
-00006a40: 6174 6162 6173 650a 2020 2020 2020 2020  atabase.        
-00006a50: 2020 2020 5b66 6f6f 2e6f 6369 656e 742e      [foo.ocient.
-00006a60: 636f 6d2f 736f 6d65 6462 5d0a 2020 2020  com/somedb].    
-00006a70: 2020 2020 2020 2020 7573 6572 203d 2070          user = p
-00006a80: 616e 7468 6572 0a20 2020 2020 2020 2020  anther.         
-00006a90: 2020 2070 6173 7377 6f72 6420 3d20 7069     password = pi
-00006aa0: 6e6b 0a0a 2020 2020 2020 2020 2020 2020  nk..            
-00006ab0: 2320 5468 6973 2077 696c 6c20 6d61 7463  # This will matc
-00006ac0: 6820 7468 6520 7370 6563 6966 6963 2068  h the specific h
-00006ad0: 6f73 740a 2020 2020 2020 2020 2020 2020  ost.            
-00006ae0: 5b66 6f6f 2e6f 6369 656e 742e 636f 6d5d  [foo.ocient.com]
-00006af0: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
-00006b00: 7220 3d20 7061 6e74 6865 720a 2020 2020  r = panther.    
-00006b10: 2020 2020 2020 2020 7061 7373 776f 7264          password
-00006b20: 203d 2070 696e 6b0a 0a20 2020 2020 2020   = pink..       
-00006b30: 2020 2020 2023 2054 6869 7320 7769 6c6c       # This will
-00006b40: 206d 6174 6368 2061 6e79 2068 6f73 7420   match any host 
-00006b50: 696e 2074 6865 206f 6369 656e 742e 636f  in the ocient.co
-00006b60: 6d20 646f 6d61 696e 0a20 2020 2020 2020  m domain.       
-00006b70: 2020 2020 205b 2a2e 6f63 6965 6e74 2e63       [*.ocient.c
-00006b80: 6f6d 5d0a 2020 2020 2020 2020 2020 2020  om].            
-00006b90: 7573 6572 203d 2074 6f6d 0a20 2020 2020  user = tom.     
-00006ba0: 2020 2020 2020 2070 6173 7377 6f72 6420         password 
-00006bb0: 3d20 6a65 7272 790a 2020 2020 2020 2020  = jerry.        
-00006bc0: 2020 2020 6461 7461 6261 7365 203d 206d      database = m
-00006bd0: 6963 650a 0a20 2020 2020 2020 2020 2020  ice..           
-00006be0: 2023 2054 6869 7320 7769 6c6c 206d 6174   # This will mat
-00006bf0: 6368 2061 6e79 2068 6f73 7420 696e 2074  ch any host in t
-00006c00: 6865 206f 6369 656e 742e 636f 6d20 646f  he ocient.com do
-00006c10: 6d61 696e 0a20 2020 2020 2020 2020 2020  main.           
-00006c20: 205b 2a2e 6f63 6965 6e74 2e63 6f6d 5d0a   [*.ocient.com].
-00006c30: 2020 2020 2020 2020 2020 2020 7573 6572              user
-00006c40: 203d 2074 6f6d 0a20 2020 2020 2020 2020   = tom.         
-00006c50: 2020 2070 6173 7377 6f72 6420 3d20 6a65     password = je
-00006c60: 7272 790a 0a20 2020 2020 2020 2043 7572  rry..        Cur
-00006c70: 7265 6e74 6c79 2073 7570 706f 7274 6564  rently supported
-00006c80: 2070 6172 616d 6574 6572 7320 6172 653a   parameters are:
-00006c90: 0a0a 2020 2020 2020 2020 2d20 746c 733a  ..        - tls:
-00006ca0: 2057 6869 6368 2063 616e 2068 6176 6520   Which can have 
-00006cb0: 7468 6520 7661 6c75 6573 2022 6f66 6622  the values "off"
-00006cc0: 2c20 2275 6e76 6572 6966 6965 6422 2c20  , "unverified", 
-00006cd0: 6f72 2022 6f6e 2220 696e 2074 6865 2064  or "on" in the d
-00006ce0: 736e 2c0a 2020 2020 2020 2020 2020 2020  sn,.            
-00006cf0: 6f72 2043 6f6e 6e65 6374 696f 6e2e 544c  or Connection.TL
-00006d00: 535f 4e4f 4e45 2c20 436f 6e6e 6563 7469  S_NONE, Connecti
-00006d10: 6f6e 2e54 4c53 5f55 4e56 4552 4946 4945  on.TLS_UNVERIFIE
-00006d20: 442c 206f 720a 2020 2020 2020 2020 2020  D, or.          
-00006d30: 2020 436f 6e6e 6563 7469 6f6e 2e54 4c53    Connection.TLS
-00006d40: 5f4f 4e20 6173 2061 206b 6579 776f 7264  _ON as a keyword
-00006d50: 2070 6172 616d 6574 6572 2e0a 2020 2020   parameter..    
-00006d60: 2020 2020 2d20 666f 7263 653a 2054 7275      - force: Tru
-00006d70: 6520 6f72 2046 616c 7365 2c20 7768 6574  e or False, whet
-00006d80: 6865 7220 746f 2066 6f72 6365 2074 6865  her to force the
-00006d90: 2063 6f6e 6e65 6374 696f 6e20 746f 2072   connection to r
-00006da0: 656d 6169 6e20 6f6e 2074 6869 730a 2020  emain on this.  
-00006db0: 2020 2020 2020 2020 2020 7365 7276 6572            server
-00006dc0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00006dd0: 2020 2020 2023 2070 796c 696e 743a 2064       # pylint: d
-00006de0: 6973 6162 6c65 3d6e 6f2d 6d65 6d62 6572  isable=no-member
-00006df0: 0a20 2020 2020 2020 2073 656c 662e 5f70  .        self._p
-00006e00: 6172 7365 5f61 7267 7328 6473 6e2c 2075  arse_args(dsn, u
-00006e10: 7365 722c 2070 6173 7377 6f72 642c 2068  ser, password, h
-00006e20: 6f73 742c 2064 6174 6162 6173 652c 2074  ost, database, t
-00006e30: 6c73 2c20 6861 6e64 7368 616b 652c 2066  ls, handshake, f
-00006e40: 6f72 6365 2c20 636f 6e66 6967 6669 6c65  orce, configfile
-00006e50: 290a 0a20 2020 2020 2020 2073 6176 6564  )..        saved
-00006e60: 5f65 7863 203d 204e 6f6e 650a 2020 2020  _exc = None.    
-00006e70: 2020 2020 666f 7220 6f6e 655f 686f 7374      for one_host
-00006e80: 2069 6e20 7365 6c66 2e68 6f73 7473 3a0a   in self.hosts:.
-00006e90: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00006ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006eb0: 206c 6f67 6765 722e 696e 666f 2866 2254   logger.info(f"T
-00006ec0: 7279 696e 6720 746f 2063 6f6e 6e65 6374  rying to connect
-00006ed0: 2074 6f20 7b6f 6e65 5f68 6f73 747d 3a7b   to {one_host}:{
-00006ee0: 7365 6c66 2e70 6f72 747d 2229 0a20 2020  self.port}").   
-00006ef0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00006f00: 662e 736f 636b 203d 2073 6f63 6b65 742e  f.sock = socket.
-00006f10: 6372 6561 7465 5f63 6f6e 6e65 6374 696f  create_connectio
-00006f20: 6e28 286f 6e65 5f68 6f73 742c 2073 656c  n((one_host, sel
-00006f30: 662e 706f 7274 2929 0a20 2020 2020 2020  f.port)).       
-00006f40: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-00006f50: 696e 666f 2866 2243 6f6e 6e65 6374 6564  info(f"Connected
-00006f60: 2074 6f20 7b6f 6e65 5f68 6f73 747d 3a7b   to {one_host}:{
-00006f70: 7365 6c66 2e70 6f72 747d 206f 6e20 736f  self.port} on so
-00006f80: 636b 6574 207b 7365 6c66 2e73 6f63 6b7d  cket {self.sock}
-00006f90: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00006fa0: 2020 2073 6176 6564 5f65 7863 203d 204e     saved_exc = N
-00006fb0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-00006fc0: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
-00006fd0: 2020 2020 2020 6578 6365 7074 2043 6f6e        except Con
-00006fe0: 6e65 6374 696f 6e45 7272 6f72 2061 7320  nectionError as 
-00006ff0: 6578 633a 0a20 2020 2020 2020 2020 2020  exc:.           
-00007000: 2020 2020 2073 6176 6564 5f65 7863 203d       saved_exc =
-00007010: 2065 7863 0a20 2020 2020 2020 2020 2020   exc.           
-00007020: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-00007030: 6e20 6173 2065 7863 3a0a 2020 2020 2020  n as exc:.      
-00007040: 2020 2020 2020 2020 2020 7361 7665 645f            saved_
-00007050: 6578 6320 3d20 6578 630a 0a20 2020 2020  exc = exc..     
-00007060: 2020 2069 6620 7361 7665 645f 6578 6320     if saved_exc 
-00007070: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00007080: 2020 2020 2020 2020 2072 6169 7365 2045           raise E
-00007090: 7272 6f72 2866 2255 6e61 626c 6520 746f  rror(f"Unable to
-000070a0: 2063 6f6e 6e65 6374 2074 6f20 7b27 2c27   connect to {','
-000070b0: 2e6a 6f69 6e28 7365 6c66 2e68 6f73 7473  .join(self.hosts
-000070c0: 297d 3a7b 7365 6c66 2e70 6f72 747d 3a20  )}:{self.port}: 
-000070d0: 7b73 7472 2873 6176 6564 5f65 7863 297d  {str(saved_exc)}
-000070e0: 2229 2066 726f 6d20 7361 7665 645f 6578  ") from saved_ex
-000070f0: 630a 0a20 2020 2020 2020 2073 656c 662e  c..        self.
-00007100: 5f73 736c 697a 655f 636f 6e6e 6563 7469  _sslize_connecti
-00007110: 6f6e 2829 0a0a 2020 2020 2020 2020 7365  on()..        se
-00007120: 6c66 2e5f 6275 6666 6572 203d 2062 2222  lf._buffer = b""
-00007130: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-00007140: 7373 696f 6e20 3d20 7365 7373 696f 6e0a  ssion = session.
-00007150: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00007160: 6861 6e64 7368 616b 6520 3d3d 2073 656c  handshake == sel
-00007170: 662e 4841 4e44 5348 414b 455f 5353 4f3a  f.HANDSHAKE_SSO:
-00007180: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00007190: 7365 6c66 2e75 7365 722e 6c6f 7765 7228  self.user.lower(
-000071a0: 2920 213d 2022 2220 6f72 2073 656c 662e  ) != "" or self.
-000071b0: 7061 7373 776f 7264 2e6c 6f77 6572 2829  password.lower()
-000071c0: 2021 3d20 2222 3a0a 2020 2020 2020 2020   != "":.        
-000071d0: 2020 2020 2020 2020 2320 4966 2065 6974          # If eit
-000071e0: 6865 7220 6172 6520 6e6f 6e2d 656d 7074  her are non-empt
-000071f0: 792c 2075 7365 2074 6865 2043 4243 5f47  y, use the CBC_G
-00007200: 434d 2e0a 2020 2020 2020 2020 2020 2020  CM..            
-00007210: 2020 2020 7365 6c66 2e5f 636c 6965 6e74      self._client
-00007220: 5f68 616e 6473 6861 6b65 5f43 4243 5f47  _handshake_CBC_G
-00007230: 434d 2869 735f 6578 706c 6963 6974 5f73  CM(is_explicit_s
-00007240: 736f 3d54 7275 652c 2066 6f72 6365 3d73  so=True, force=s
-00007250: 656c 662e 666f 7263 6529 0a20 2020 2020  elf.force).     
-00007260: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00007270: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00007280: 7365 6c66 2e73 6573 7369 6f6e 2069 7320  self.session is 
-00007290: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000072a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000072b0: 6c66 2e5f 636c 6965 6e74 5f68 616e 6473  lf._client_hands
-000072c0: 6861 6b65 5f73 6563 7572 6974 795f 746f  hake_security_to
-000072d0: 6b65 6e28 290a 2020 2020 2020 2020 2020  ken().          
-000072e0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000072f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007300: 7365 6c66 2e5f 636c 6965 6e74 5f68 616e  self._client_han
-00007310: 6473 6861 6b65 5f53 534f 2829 0a20 2020  dshake_SSO().   
-00007320: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00007330: 2020 2020 2020 2073 656c 662e 5f63 6c69         self._cli
-00007340: 656e 745f 6861 6e64 7368 616b 655f 4342  ent_handshake_CB
-00007350: 435f 4743 4d28 6973 5f65 7870 6c69 6369  C_GCM(is_explici
-00007360: 745f 7373 6f3d 4661 6c73 652c 2066 6f72  t_sso=False, for
-00007370: 6365 3d73 656c 662e 666f 7263 6529 0a0a  ce=self.force)..
-00007380: 2020 2020 6465 6620 5f69 6e69 7469 616c      def _initial
-00007390: 697a 655f 636c 6965 6e74 5f63 6f6e 6e65  ize_client_conne
-000073a0: 6374 696f 6e28 7365 6c66 2c20 636c 6965  ction(self, clie
-000073b0: 6e74 5f63 6f6e 6e65 6374 696f 6e5f 6d65  nt_connection_me
-000073c0: 7373 6167 6529 3a0a 2020 2020 2020 2020  ssage):.        
-000073d0: 2222 2249 6e69 7469 616c 697a 6573 2066  """Initializes f
-000073e0: 6965 6c64 7320 7573 6564 2069 6e20 696e  ields used in in
-000073f0: 6974 6961 6c20 636c 6965 6e74 2068 616e  itial client han
-00007400: 6473 6861 6b65 2072 6571 7565 7374 732e  dshake requests.
-00007410: 0a20 2020 2020 2020 2031 2e20 6461 7461  .        1. data
-00007420: 6261 7365 0a20 2020 2020 2020 2032 2e20  base.        2. 
-00007430: 636c 6965 6e74 6964 2028 7079 6f63 6965  clientid (pyocie
-00007440: 6e74 290a 2020 2020 2020 2020 332e 2070  nt).        3. p
-00007450: 726f 746f 636f 6c20 7665 7273 696f 6e0a  rotocol version.
-00007460: 2020 2020 2020 2020 342e 2076 6572 7369          4. versi
-00007470: 6f6e 5f6d 616a 6f72 0a20 2020 2020 2020  on_major.       
-00007480: 2035 2e20 7665 7273 696f 6e5f 6d69 6e6f   5. version_mino
-00007490: 720a 2020 2020 2020 2020 362e 2073 6573  r.        6. ses
-000074a0: 7369 6f6e 2069 640a 0a20 2020 2020 2020  sion id..       
-000074b0: 204e 6f74 652c 206e 6f74 2061 6c6c 2066   Note, not all f
-000074c0: 6965 6c64 7320 6172 6520 696e 6974 6961  ields are initia
-000074d0: 6c69 7a65 642e 2053 6f6d 6520 6669 656c  lized. Some fiel
-000074e0: 6473 2061 7265 2073 7065 6369 616c 2074  ds are special t
-000074f0: 6f20 6365 7274 6169 6e20 636c 6965 6e74  o certain client
-00007500: 2068 616e 6473 6861 6b65 732e 0a20 2020   handshakes..   
-00007510: 2020 2020 2046 6f72 2065 7861 6d70 6c65       For example
-00007520: 2c20 7468 6520 5353 4f20 6861 6e64 7368  , the SSO handsh
-00007530: 616b 6520 7769 7468 2074 6f6b 656e 2064  ake with token d
-00007540: 6f65 7320 6e6f 7420 7461 6b65 2075 7365  oes not take use
-00007550: 7220 616e 6420 696e 7374 6561 6420 7461  r and instead ta
-00007560: 6b65 7320 6120 7365 6375 7269 7479 2074  kes a security t
-00007570: 6f6b 656e 2e0a 0a20 2020 2020 2020 2041  oken...        A
-00007580: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00007590: 2063 6c69 656e 745f 636f 6e6e 6563 7469   client_connecti
-000075a0: 6f6e 5f6d 6573 7361 6765 2028 5b70 726f  on_message ([pro
-000075b0: 746f 206d 6573 7361 6765 5d29 3a20 7468  to message]): th
-000075c0: 6520 636c 6965 6e74 2068 616e 6473 6861  e client handsha
-000075d0: 6b65 2072 6571 7565 7374 2074 6f20 696e  ke request to in
-000075e0: 6974 6961 6c69 7a65 0a20 2020 2020 2020  itialize.       
-000075f0: 2022 2222 0a20 2020 2020 2020 2063 6c69   """.        cli
-00007600: 656e 745f 636f 6e6e 6563 7469 6f6e 5f6d  ent_connection_m
-00007610: 6573 7361 6765 2e64 6174 6162 6173 6520  essage.database 
-00007620: 3d20 7365 6c66 2e64 6174 6162 6173 650a  = self.database.
-00007630: 2020 2020 2020 2020 636c 6965 6e74 5f63          client_c
-00007640: 6f6e 6e65 6374 696f 6e5f 6d65 7373 6167  onnection_messag
-00007650: 652e 636c 6965 6e74 6964 203d 2044 5249  e.clientid = DRI
-00007660: 5645 525f 4944 0a20 2020 2020 2020 2063  VER_ID.        c
-00007670: 6c69 656e 745f 636f 6e6e 6563 7469 6f6e  lient_connection
-00007680: 5f6d 6573 7361 6765 2e76 6572 7369 6f6e  _message.version
-00007690: 203d 2050 524f 544f 434f 4c5f 5645 5253   = PROTOCOL_VERS
-000076a0: 494f 4e0a 2020 2020 2020 2020 636c 6965  ION.        clie
-000076b0: 6e74 5f63 6f6e 6e65 6374 696f 6e5f 6d65  nt_connection_me
-000076c0: 7373 6167 652e 6d61 6a6f 7243 6c69 656e  ssage.majorClien
-000076d0: 7456 6572 7369 6f6e 203d 2076 6572 7369  tVersion = versi
-000076e0: 6f6e 5f6d 616a 6f72 0a20 2020 2020 2020  on_major.       
-000076f0: 2063 6c69 656e 745f 636f 6e6e 6563 7469   client_connecti
-00007700: 6f6e 5f6d 6573 7361 6765 2e6d 696e 6f72  on_message.minor
-00007710: 436c 6965 6e74 5665 7273 696f 6e20 3d20  ClientVersion = 
-00007720: 7665 7273 696f 6e5f 6d69 6e6f 720a 2020  version_minor.  
-00007730: 2020 2020 2020 636c 6965 6e74 5f63 6f6e        client_con
-00007740: 6e65 6374 696f 6e5f 6d65 7373 6167 652e  nection_message.
-00007750: 7365 7373 696f 6e49 4420 3d20 7365 6c66  sessionID = self
-00007760: 2e73 6573 7369 6f6e 5f69 640a 0a20 2020  .session_id..   
-00007770: 2064 6566 205f 636c 6965 6e74 5f68 616e   def _client_han
-00007780: 6473 6861 6b65 5f43 4243 5f47 434d 2873  dshake_CBC_GCM(s
-00007790: 656c 662c 2069 735f 6578 706c 6963 6974  elf, is_explicit
-000077a0: 5f73 736f 3d46 616c 7365 2c20 666f 7263  _sso=False, forc
-000077b0: 653d 4661 6c73 6529 3a0a 2020 2020 2020  e=False):.      
-000077c0: 2020 7768 696c 6520 5472 7565 3a0a 2020    while True:.  
-000077d0: 2020 2020 2020 2020 2020 2323 2323 2323            ######
-000077e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000077f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007800: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007810: 2323 2323 2323 2323 2323 2323 0a20 2020  ############.   
-00007820: 2020 2020 2020 2020 2023 2053 656e 6420           # Send 
-00007830: 7468 6520 434c 4945 4e54 5f43 4f4e 4e45  the CLIENT_CONNE
-00007840: 4354 494f 4e20 7265 7175 6573 740a 2020  CTION request.  
-00007850: 2020 2020 2020 2020 2020 2323 2323 2323            ######
-00007860: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007870: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007880: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007890: 2323 2323 2323 2323 2323 2323 0a20 2020  ############.   
-000078a0: 2020 2020 2020 2020 2072 6571 203d 2070           req = p
-000078b0: 726f 746f 2e52 6571 7565 7374 2829 0a20  roto.Request(). 
-000078c0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-000078d0: 6c66 2e68 616e 6473 6861 6b65 203d 3d20  lf.handshake == 
-000078e0: 7365 6c66 2e48 414e 4453 4841 4b45 5f43  self.HANDSHAKE_C
-000078f0: 4243 3a0a 2020 2020 2020 2020 2020 2020  BC:.            
-00007900: 2020 2020 7265 712e 7479 7065 203d 2072      req.type = r
-00007910: 6571 2e43 4c49 454e 545f 434f 4e4e 4543  eq.CLIENT_CONNEC
-00007920: 5449 4f4e 0a20 2020 2020 2020 2020 2020  TION.           
-00007930: 2020 2020 2063 6c69 656e 745f 636f 6e6e       client_conn
-00007940: 6563 7469 6f6e 203d 2072 6571 2e63 6c69  ection = req.cli
-00007950: 656e 745f 636f 6e6e 6563 7469 6f6e 0a20  ent_connection. 
-00007960: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00007970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007980: 2023 2053 686f 756c 6420 6265 2047 434d   # Should be GCM
-00007990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000079a0: 2072 6571 2e74 7970 6520 3d20 7265 712e   req.type = req.
-000079b0: 434c 4945 4e54 5f43 4f4e 4e45 4354 494f  CLIENT_CONNECTIO
-000079c0: 4e5f 4743 4d0a 2020 2020 2020 2020 2020  N_GCM.          
-000079d0: 2020 2020 2020 636c 6965 6e74 5f63 6f6e        client_con
-000079e0: 6e65 6374 696f 6e20 3d20 7265 712e 636c  nection = req.cl
-000079f0: 6965 6e74 5f63 6f6e 6e65 6374 696f 6e5f  ient_connection_
-00007a00: 6763 6d0a 2020 2020 2020 2020 2020 2020  gcm.            
-00007a10: 2020 2020 636c 6965 6e74 5f63 6f6e 6e65      client_conne
-00007a20: 6374 696f 6e2e 6578 706c 6963 6974 5353  ction.explicitSS
-00007a30: 4f20 3d20 6973 5f65 7870 6c69 6369 745f  O = is_explicit_
-00007a40: 7373 6f0a 2020 2020 2020 2020 2020 2020  sso.            
-00007a50: 636c 6965 6e74 5f63 6f6e 6e65 6374 696f  client_connectio
-00007a60: 6e2e 7573 6572 6964 203d 2073 656c 662e  n.userid = self.
-00007a70: 7573 6572 0a20 2020 2020 2020 2020 2020  user.           
-00007a80: 2073 656c 662e 5f69 6e69 7469 616c 697a   self._initializ
-00007a90: 655f 636c 6965 6e74 5f63 6f6e 6e65 6374  e_client_connect
-00007aa0: 696f 6e28 636c 6965 6e74 5f63 6f6e 6e65  ion(client_conne
-00007ab0: 6374 696f 6e29 0a0a 2020 2020 2020 2020  ction)..        
-00007ac0: 2020 2020 5f73 656e 645f 6d73 6728 7365      _send_msg(se
-00007ad0: 6c66 2c20 7265 7129 0a0a 2020 2020 2020  lf, req)..      
-00007ae0: 2020 2020 2020 2323 2323 2323 2323 2323        ##########
-00007af0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007b00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007b10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007b20: 2323 2323 2323 2323 0a20 2020 2020 2020  ########.       
-00007b30: 2020 2020 2023 2047 6574 2074 6865 2043       # Get the C
-00007b40: 4c49 454e 545f 434f 4e4e 4543 5449 4f4e  LIENT_CONNECTION
-00007b50: 2072 6573 706f 6e73 6520 616e 6420 7072   response and pr
-00007b60: 6f63 6573 7320 6974 0a20 2020 2020 2020  ocess it.       
-00007b70: 2020 2020 2023 2323 2323 2323 2323 2323       ###########
-00007b80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007b90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007ba0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007bb0: 2323 2323 2323 230a 2020 2020 2020 2020  #######.        
-00007bc0: 2020 2020 6966 2073 656c 662e 6861 6e64      if self.hand
-00007bd0: 7368 616b 6520 3d3d 2073 656c 662e 4841  shake == self.HA
-00007be0: 4e44 5348 414b 455f 4342 433a 0a20 2020  NDSHAKE_CBC:.   
-00007bf0: 2020 2020 2020 2020 2020 2020 2023 2043               # C
-00007c00: 4243 0a20 2020 2020 2020 2020 2020 2020  BC.             
-00007c10: 2020 2072 7370 203d 205f 7265 6376 5f6d     rsp = _recv_m
-00007c20: 7367 2873 656c 662c 2070 726f 746f 2e43  sg(self, proto.C
-00007c30: 6c69 656e 7443 6f6e 6e65 6374 696f 6e52  lientConnectionR
-00007c40: 6573 706f 6e73 6528 2929 0a20 2020 2020  esponse()).     
-00007c50: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00007c60: 2020 2020 2020 2020 2020 2020 2023 2047               # G
-00007c70: 434d 206f 7220 6578 706c 6963 6974 2053  CM or explicit S
-00007c80: 534f 0a20 2020 2020 2020 2020 2020 2020  SO.             
-00007c90: 2020 2072 7370 203d 205f 7265 6376 5f6d     rsp = _recv_m
-00007ca0: 7367 2873 656c 662c 2070 726f 746f 2e43  sg(self, proto.C
-00007cb0: 6c69 656e 7443 6f6e 6e65 6374 696f 6e47  lientConnectionG
-00007cc0: 434d 5265 7370 6f6e 7365 2829 290a 0a20  CMResponse()).. 
-00007cd0: 2020 2020 2020 2020 2020 2069 6620 7273             if rs
-00007ce0: 702e 7265 7370 6f6e 7365 2e74 7970 6520  p.response.type 
-00007cf0: 3d3d 2070 726f 746f 2e43 6f6e 6669 726d  == proto.Confirm
-00007d00: 6174 696f 6e52 6573 706f 6e73 652e 5245  ationResponse.RE
-00007d10: 5350 4f4e 5345 5f57 4152 4e3a 0a20 2020  SPONSE_WARN:.   
-00007d20: 2020 2020 2020 2020 2020 2020 2077 6172               war
-00007d30: 6e28 7273 702e 7265 7370 6f6e 7365 2e72  n(rsp.response.r
-00007d40: 6561 736f 6e29 0a20 2020 2020 2020 2020  eason).         
-00007d50: 2020 2065 6c69 6620 6e6f 7420 7273 702e     elif not rsp.
-00007d60: 7265 7370 6f6e 7365 2e74 7970 6520 3d3d  response.type ==
-00007d70: 2070 726f 746f 2e43 6f6e 6669 726d 6174   proto.Confirmat
-00007d80: 696f 6e52 6573 706f 6e73 652e 5245 5350  ionResponse.RESP
-00007d90: 4f4e 5345 5f4f 4b3a 0a20 2020 2020 2020  ONSE_OK:.       
-00007da0: 2020 2020 2020 2020 2072 6169 7365 205f           raise _
-00007db0: 636f 6e76 6572 745f 6578 6365 7074 696f  convert_exceptio
-00007dc0: 6e28 7273 702e 7265 7370 6f6e 7365 290a  n(rsp.response).
-00007dd0: 0a20 2020 2020 2020 2020 2020 2070 6565  .            pee
-00007de0: 725f 6b65 7920 3d20 6c6f 6164 5f70 656d  r_key = load_pem
-00007df0: 5f70 7562 6c69 635f 6b65 7928 7273 702e  _public_key(rsp.
-00007e00: 7075 624b 6579 2e65 6e63 6f64 6528 656e  pubKey.encode(en
-00007e10: 636f 6469 6e67 3d22 5554 462d 3822 2c20  coding="UTF-8", 
-00007e20: 6572 726f 7273 3d22 7374 7269 6374 2229  errors="strict")
-00007e30: 2c20 6261 636b 656e 643d 6465 6661 756c  , backend=defaul
-00007e40: 745f 6261 636b 656e 6428 2929 0a20 2020  t_backend()).   
-00007e50: 2020 2020 2020 2020 2028 6369 7068 6572           (cipher
-00007e60: 2c20 6765 6e65 7261 7465 645f 686d 6163  , generated_hmac
-00007e70: 2c20 7075 626c 6963 5f6b 6579 2920 3d20  , public_key) = 
-00007e80: 7365 6c66 2e5f 656e 6372 7970 7469 6f6e  self._encryption
-00007e90: 5f72 6f75 7469 6e65 2872 7370 2e69 762c  _routine(rsp.iv,
-00007ea0: 2070 6565 725f 6b65 7929 0a0a 2020 2020   peer_key)..    
-00007eb0: 2020 2020 2020 2020 2323 2323 2323 2323          ########
-00007ec0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007ed0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007ee0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007ef0: 2323 2323 2323 2323 2323 0a20 2020 2020  ##########.     
-00007f00: 2020 2020 2020 2023 2053 656e 6420 7468         # Send th
-00007f10: 6520 434c 4945 4e54 5f43 4f4e 4e45 4354  e CLIENT_CONNECT
-00007f20: 494f 4e32 2072 6571 7565 7374 0a20 2020  ION2 request.   
-00007f30: 2020 2020 2020 2020 2023 2323 2323 2323           #######
-00007f40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007f50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007f60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007f70: 2323 2323 2323 2323 2323 230a 2020 2020  ###########.    
-00007f80: 2020 2020 2020 2020 7265 7120 3d20 7072          req = pr
-00007f90: 6f74 6f2e 5265 7175 6573 7428 290a 2020  oto.Request().  
-00007fa0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00007fb0: 662e 6861 6e64 7368 616b 6520 3d3d 2073  f.handshake == s
-00007fc0: 656c 662e 4841 4e44 5348 414b 455f 4342  elf.HANDSHAKE_CB
-00007fd0: 433a 0a20 2020 2020 2020 2020 2020 2020  C:.             
-00007fe0: 2020 2072 6571 2e74 7970 6520 3d20 7265     req.type = re
-00007ff0: 712e 434c 4945 4e54 5f43 4f4e 4e45 4354  q.CLIENT_CONNECT
-00008000: 494f 4e32 0a20 2020 2020 2020 2020 2020  ION2.           
-00008010: 2020 2020 2072 6571 2e63 6c69 656e 745f       req.client_
-00008020: 636f 6e6e 6563 7469 6f6e 322e 6369 7068  connection2.ciph
-00008030: 6572 203d 2063 6970 6865 720a 2020 2020  er = cipher.    
-00008040: 2020 2020 2020 2020 2020 2020 7265 712e              req.
-00008050: 636c 6965 6e74 5f63 6f6e 6e65 6374 696f  client_connectio
-00008060: 6e32 2e66 6f72 6365 203d 2066 6f72 6365  n2.force = force
-00008070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008080: 2072 6571 2e63 6c69 656e 745f 636f 6e6e   req.client_conn
-00008090: 6563 7469 6f6e 322e 686d 6163 203d 2067  ection2.hmac = g
-000080a0: 656e 6572 6174 6564 5f68 6d61 630a 2020  enerated_hmac.  
-000080b0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000080c0: 712e 636c 6965 6e74 5f63 6f6e 6e65 6374  q.client_connect
-000080d0: 696f 6e32 2e70 7562 4b65 7920 3d20 7075  ion2.pubKey = pu
-000080e0: 626c 6963 5f6b 6579 2e70 7562 6c69 635f  blic_key.public_
-000080f0: 6279 7465 7328 656e 636f 6469 6e67 3d73  bytes(encoding=s
-00008100: 6572 6961 6c69 7a61 7469 6f6e 2e45 6e63  erialization.Enc
-00008110: 6f64 696e 672e 5045 4d2c 2066 6f72 6d61  oding.PEM, forma
-00008120: 743d 7365 7269 616c 697a 6174 696f 6e2e  t=serialization.
-00008130: 5075 626c 6963 466f 726d 6174 2e53 7562  PublicFormat.Sub
-00008140: 6a65 6374 5075 626c 6963 4b65 7949 6e66  jectPublicKeyInf
-00008150: 6f29 0a20 2020 2020 2020 2020 2020 2065  o).            e
-00008160: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00008170: 2020 2020 2072 6571 2e74 7970 6520 3d20       req.type = 
-00008180: 7265 712e 434c 4945 4e54 5f43 4f4e 4e45  req.CLIENT_CONNE
-00008190: 4354 494f 4e5f 4743 4d32 0a20 2020 2020  CTION_GCM2.     
-000081a0: 2020 2020 2020 2020 2020 2072 6571 2e63             req.c
-000081b0: 6c69 656e 745f 636f 6e6e 6563 7469 6f6e  lient_connection
-000081c0: 5f67 636d 322e 6369 7068 6572 203d 2063  _gcm2.cipher = c
-000081d0: 6970 6865 720a 2020 2020 2020 2020 2020  ipher.          
-000081e0: 2020 2020 2020 7265 712e 636c 6965 6e74        req.client
-000081f0: 5f63 6f6e 6e65 6374 696f 6e5f 6763 6d32  _connection_gcm2
-00008200: 2e66 6f72 6365 203d 2066 6f72 6365 0a20  .force = force. 
-00008210: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00008220: 6571 2e63 6c69 656e 745f 636f 6e6e 6563  eq.client_connec
-00008230: 7469 6f6e 5f67 636d 322e 686d 6163 203d  tion_gcm2.hmac =
-00008240: 2067 656e 6572 6174 6564 5f68 6d61 630a   generated_hmac.
-00008250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008260: 7265 712e 636c 6965 6e74 5f63 6f6e 6e65  req.client_conne
-00008270: 6374 696f 6e5f 6763 6d32 2e65 7870 6c69  ction_gcm2.expli
-00008280: 6369 7453 534f 203d 2069 735f 6578 706c  citSSO = is_expl
-00008290: 6963 6974 5f73 736f 0a20 2020 2020 2020  icit_sso.       
-000082a0: 2020 2020 2020 2020 2072 6571 2e63 6c69           req.cli
-000082b0: 656e 745f 636f 6e6e 6563 7469 6f6e 5f67  ent_connection_g
-000082c0: 636d 322e 7075 624b 6579 203d 2070 7562  cm2.pubKey = pub
-000082d0: 6c69 635f 6b65 792e 7075 626c 6963 5f62  lic_key.public_b
-000082e0: 7974 6573 2865 6e63 6f64 696e 673d 7365  ytes(encoding=se
-000082f0: 7269 616c 697a 6174 696f 6e2e 456e 636f  rialization.Enco
-00008300: 6469 6e67 2e50 454d 2c20 666f 726d 6174  ding.PEM, format
-00008310: 3d73 6572 6961 6c69 7a61 7469 6f6e 2e50  =serialization.P
-00008320: 7562 6c69 6346 6f72 6d61 742e 5375 626a  ublicFormat.Subj
-00008330: 6563 7450 7562 6c69 634b 6579 496e 666f  ectPublicKeyInfo
-00008340: 290a 0a20 2020 2020 2020 2020 2020 205f  )..            _
-00008350: 7365 6e64 5f6d 7367 2873 656c 662c 2072  send_msg(self, r
-00008360: 6571 290a 0a20 2020 2020 2020 2020 2020  eq)..           
-00008370: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
-00008380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00008390: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000083a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000083b0: 2323 230a 2020 2020 2020 2020 2020 2020  ###.            
-000083c0: 2320 4765 7420 7468 6520 434c 4945 4e54  # Get the CLIENT
-000083d0: 5f43 4f4e 4e45 4354 494f 4e20 7265 7370  _CONNECTION resp
-000083e0: 6f6e 7365 2061 6e64 2070 726f 6365 7373  onse and process
-000083f0: 2069 740a 2020 2020 2020 2020 2020 2020   it.            
-00008400: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00008410: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00008420: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00008430: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00008440: 2323 0a20 2020 2020 2020 2020 2020 2069  ##.            i
-00008450: 6620 7365 6c66 2e68 616e 6473 6861 6b65  f self.handshake
-00008460: 203d 3d20 7365 6c66 2e48 414e 4453 4841   == self.HANDSHA
-00008470: 4b45 5f43 4243 3a0a 2020 2020 2020 2020  KE_CBC:.        
-00008480: 2020 2020 2020 2020 2320 4342 430a 2020          # CBC.  
-00008490: 2020 2020 2020 2020 2020 2020 2020 7273                rs
-000084a0: 7020 3d20 5f72 6563 765f 6d73 6728 7365  p = _recv_msg(se
-000084b0: 6c66 2c20 7072 6f74 6f2e 436c 6965 6e74  lf, proto.Client
-000084c0: 436f 6e6e 6563 7469 6f6e 3252 6573 706f  Connection2Respo
-000084d0: 6e73 6528 2929 0a20 2020 2020 2020 2020  nse()).         
-000084e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000084f0: 2020 2020 2020 2020 2023 2047 434d 206f           # GCM o
-00008500: 7220 6578 706c 6963 6974 2053 534f 0a20  r explicit SSO. 
-00008510: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00008520: 7370 203d 205f 7265 6376 5f6d 7367 2873  sp = _recv_msg(s
-00008530: 656c 662c 2070 726f 746f 2e43 6c69 656e  elf, proto.Clien
-00008540: 7443 6f6e 6e65 6374 696f 6e47 434d 3252  tConnectionGCM2R
-00008550: 6573 706f 6e73 6528 2929 0a0a 2020 2020  esponse())..    
-00008560: 2020 2020 2020 2020 6966 2072 7370 2e72          if rsp.r
-00008570: 6573 706f 6e73 652e 7479 7065 203d 3d20  esponse.type == 
-00008580: 7072 6f74 6f2e 436f 6e66 6972 6d61 7469  proto.Confirmati
-00008590: 6f6e 5265 7370 6f6e 7365 2e52 4553 504f  onResponse.RESPO
-000085a0: 4e53 455f 5741 524e 3a0a 2020 2020 2020  NSE_WARN:.      
-000085b0: 2020 2020 2020 2020 2020 7761 726e 2872            warn(r
-000085c0: 7370 2e72 6573 706f 6e73 652e 7265 6173  sp.response.reas
-000085d0: 6f6e 290a 2020 2020 2020 2020 2020 2020  on).            
-000085e0: 656c 6966 2072 7370 2e72 6573 706f 6e73  elif rsp.respons
-000085f0: 652e 7479 7065 203d 3d20 7072 6f74 6f2e  e.type == proto.
-00008600: 436f 6e66 6972 6d61 7469 6f6e 5265 7370  ConfirmationResp
-00008610: 6f6e 7365 2e52 4553 504f 4e53 455f 4f4b  onse.RESPONSE_OK
-00008620: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008630: 2020 2320 5361 7665 2074 6865 2073 6572    # Save the ser
-00008640: 7665 7220 7365 7373 696f 6e20 6964 0a20  ver session id. 
-00008650: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00008660: 656c 662e 7365 7276 6572 5365 7373 696f  elf.serverSessio
-00008670: 6e49 6420 3d20 7273 702e 7365 7276 6572  nId = rsp.server
-00008680: 5365 7373 696f 6e49 640a 2020 2020 2020  SessionId.      
-00008690: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-000086a0: 6573 7369 6f6e 203d 2053 6573 7369 6f6e  ession = Session
-000086b0: 2875 7365 7241 6e64 5061 7373 776f 7264  (userAndPassword
-000086c0: 3d55 7365 7241 6e64 5061 7373 776f 7264  =UserAndPassword
-000086d0: 2873 656c 662e 7573 6572 2c20 7365 6c66  (self.user, self
-000086e0: 2e70 6173 7377 6f72 6429 290a 2020 2020  .password)).    
-000086f0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00008700: 6572 2e69 6e66 6f28 6622 436f 6e6e 6563  er.info(f"Connec
-00008710: 7465 6420 746f 2073 6572 7665 7220 7365  ted to server se
-00008720: 7373 696f 6e20 4964 3a20 7b73 656c 662e  ssion Id: {self.
-00008730: 7365 7276 6572 5365 7373 696f 6e49 647d  serverSessionId}
-00008740: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00008750: 2020 2023 2053 6176 6520 7365 636f 6e64     # Save second
-00008760: 6172 7920 696e 7465 7266 6163 6573 2e0a  ary interfaces..
-00008770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008780: 7365 6c66 2e5f 7361 7665 5f73 6563 6f6e  self._save_secon
-00008790: 6461 7279 5f69 6e74 6572 6661 6365 7328  dary_interfaces(
-000087a0: 7273 702e 7365 636f 6e64 6172 7929 0a0a  rsp.secondary)..
-000087b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087c0: 2320 5265 6469 7265 6374 2074 6865 2063  # Redirect the c
-000087d0: 6f6e 6e65 6374 696f 6e0a 2020 2020 2020  onnection.      
-000087e0: 2020 2020 2020 2020 2020 6966 2072 7370            if rsp
-000087f0: 2e72 6564 6972 6563 743a 0a20 2020 2020  .redirect:.     
-00008800: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00008810: 656c 662e 736f 636b 2e63 6c6f 7365 2829  elf.sock.close()
-00008820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008830: 2020 2020 206d 6170 7065 645f 686f 7374       mapped_host
-00008840: 2c20 6d61 7070 6564 5f70 6f72 7420 3d20  , mapped_port = 
-00008850: 7365 6c66 2e72 6573 6f6c 7665 5f6e 6577  self.resolve_new
-00008860: 5f65 6e64 706f 696e 7428 7273 702e 7265  _endpoint(rsp.re
-00008870: 6469 7265 6374 486f 7374 2c20 7273 702e  directHost, rsp.
-00008880: 7265 6469 7265 6374 506f 7274 290a 2020  redirectPort).  
-00008890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088a0: 2020 6c6f 6767 6572 2e64 6562 7567 2866    logger.debug(f
-000088b0: 2252 6564 6972 6563 7469 6e67 2063 6f6e  "Redirecting con
-000088c0: 6e65 6374 696f 6e20 746f 207b 7273 702e  nection to {rsp.
-000088d0: 7265 6469 7265 6374 486f 7374 7d3a 7b72  redirectHost}:{r
-000088e0: 7370 2e72 6564 6972 6563 7450 6f72 747d  sp.redirectPort}
-000088f0: 2c20 7768 6963 6820 6d61 7073 2074 6f20  , which maps to 
-00008900: 7b6d 6170 7065 645f 686f 7374 7d3a 7b6d  {mapped_host}:{m
-00008910: 6170 7065 645f 706f 7274 7d22 290a 2020  apped_port}").  
-00008920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008930: 2020 7365 6c66 2e73 6f63 6b20 3d20 736f    self.sock = so
-00008940: 636b 6574 2e63 7265 6174 655f 636f 6e6e  cket.create_conn
-00008950: 6563 7469 6f6e 2828 6d61 7070 6564 5f68  ection((mapped_h
-00008960: 6f73 742c 206d 6170 7065 645f 706f 7274  ost, mapped_port
-00008970: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00008980: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
-00008990: 666f 2866 2243 6f6e 6e65 6374 6564 2074  fo(f"Connected t
-000089a0: 6f20 7b6d 6170 7065 645f 686f 7374 7d3a  o {mapped_host}:
-000089b0: 7b6d 6170 7065 645f 706f 7274 7d20 6f6e  {mapped_port} on
-000089c0: 2073 6f63 6b65 7420 7b73 656c 662e 736f   socket {self.so
-000089d0: 636b 7d22 290a 2020 2020 2020 2020 2020  ck}").          
-000089e0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000089f0: 7373 6c69 7a65 5f63 6f6e 6e65 6374 696f  sslize_connectio
-00008a00: 6e28 290a 0a20 2020 2020 2020 2020 2020  n()..           
-00008a10: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00008a20: 7365 6c66 2e5f 636c 6965 6e74 5f68 616e  self._client_han
-00008a30: 6473 6861 6b65 5f43 4243 5f47 434d 2869  dshake_CBC_GCM(i
-00008a40: 735f 6578 706c 6963 6974 5f73 736f 2c20  s_explicit_sso, 
-00008a50: 5472 7565 290a 0a20 2020 2020 2020 2020  True)..         
-00008a60: 2020 2020 2020 2062 7265 616b 0a0a 2020         break..  
-00008a70: 2020 2020 2020 2020 2020 2320 7468 6572            # ther
-00008a80: 6520 6973 2073 6f6d 6574 6869 6e67 2062  e is something b
-00008a90: 726f 6b65 6e20 696e 206f 7572 2068 616e  roken in our han
-00008aa0: 6473 6861 6b65 2e2e 2e72 6574 7279 0a20  dshake...retry. 
-00008ab0: 2020 2020 2020 2020 2020 2069 6620 7273             if rs
-00008ac0: 702e 7265 7370 6f6e 7365 2e76 656e 646f  p.response.vendo
-00008ad0: 725f 636f 6465 203d 3d20 2d32 3032 3a0a  r_code == -202:.
-00008ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008af0: 6c6f 6767 6572 2e64 6562 7567 2822 4861  logger.debug("Ha
-00008b00: 6e64 7368 616b 6520 6572 726f 722e 2e2e  ndshake error...
-00008b10: 7265 7472 7969 6e67 2229 0a20 2020 2020  retrying").     
-00008b20: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-00008b30: 6e75 650a 0a20 2020 2020 2020 2020 2020  nue..           
-00008b40: 2072 6169 7365 205f 636f 6e76 6572 745f   raise _convert_
-00008b50: 6578 6365 7074 696f 6e28 7273 702e 7265  exception(rsp.re
-00008b60: 7370 6f6e 7365 290a 0a20 2020 2064 6566  sponse)..    def
-00008b70: 205f 636c 6965 6e74 5f68 616e 6473 6861   _client_handsha
-00008b80: 6b65 5f53 534f 2873 656c 6629 3a0a 2020  ke_SSO(self):.  
-00008b90: 2020 2020 2020 2222 2249 6e74 6572 6e61        """Interna
-00008ba0: 6c20 726f 7574 696e 6520 666f 7220 7369  l routine for si
-00008bb0: 6e67 6c65 2073 6967 6e20 6f6e 2068 616e  ngle sign on han
-00008bc0: 6473 6861 6b65 2028 5353 4f29 2e0a 2020  dshake (SSO)..  
-00008bd0: 2020 2020 2020 312e 2044 7269 7665 7220        1. Driver 
-00008be0: 7265 7175 6573 7473 2074 6f20 7369 676e  requests to sign
-00008bf0: 206f 6e20 7669 6120 5353 4f2e 0a20 2020   on via SSO..   
-00008c00: 2020 2020 2032 2e20 5365 7276 6572 2073       2. Server s
-00008c10: 656e 6473 2062 6163 6b20 616e 2061 7574  ends back an aut
-00008c20: 6874 6865 6e74 6963 6174 696f 6e20 5552  hthentication UR
-00008c30: 4c2e 0a20 2020 2020 2020 2033 2e20 4472  L..        3. Dr
-00008c40: 6976 6572 206c 6175 6e63 6865 7320 5552  iver launches UR
-00008c50: 4c20 696e 2064 6566 6175 6c74 2062 726f  L in default bro
-00008c60: 7773 6572 2028 6f72 2070 7269 6e74 7320  wser (or prints 
-00008c70: 7468 6520 7572 6c20 746f 2073 7464 206f  the url to std o
-00008c80: 7574 2069 6620 6e6f 7420 706f 7373 6962  ut if not possib
-00008c90: 6c65 290a 2020 2020 2020 2020 342e 2055  le).        4. U
-00008ca0: 7365 7220 6175 7468 656e 7469 6361 7465  ser authenticate
-00008cb0: 7320 696e 2062 726f 7773 6572 2e0a 2020  s in browser..  
-00008cc0: 2020 2020 2020 352e 2044 7269 7665 7220        5. Driver 
-00008cd0: 636f 6e74 696e 756f 7573 6c79 2070 6f6c  continuously pol
-00008ce0: 6c73 2074 6865 2064 6174 6162 6173 6520  ls the database 
-00008cf0: 756e 7469 6c20 6c6f 6769 6e20 636f 6d70  until login comp
-00008d00: 6c65 7465 732e 0a20 2020 2020 2020 2036  letes..        6
-00008d10: 2e20 5570 6f6e 2063 6f6d 706c 6574 6574  . Upon completet
-00008d20: 696f 6e2c 2073 6572 7665 7220 7365 6e64  ion, server send
-00008d30: 7320 6261 636b 2061 2073 6563 7572 6974  s back a securit
-00008d40: 7920 746f 6b65 6e20 7769 7468 2077 6869  y token with whi
-00008d50: 6368 2074 6865 2064 7269 7665 7220 6361  ch the driver ca
-00008d60: 6e20 636f 6e6e 6563 742e 2028 5573 6564  n connect. (Used
-00008d70: 2066 6f72 2072 6564 6972 6563 7469 6e67   for redirecting
-00008d80: 202f 2072 6563 6f6e 6e65 6374 696e 6729   / reconnecting)
-00008d90: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00008da0: 2020 2020 2066 726f 6d20 7765 6262 726f       from webbro
-00008db0: 7773 6572 2069 6d70 6f72 7420 6f70 656e  wser import open
-00008dc0: 5f6e 6577 0a0a 2020 2020 2020 2020 7265  _new..        re
-00008dd0: 7120 3d20 7072 6f74 6f2e 5265 7175 6573  q = proto.Reques
-00008de0: 7428 290a 2020 2020 2020 2020 7265 712e  t().        req.
-00008df0: 7479 7065 203d 2072 6571 2e43 4c49 454e  type = req.CLIEN
-00008e00: 545f 434f 4e4e 4543 5449 4f4e 5f53 534f  T_CONNECTION_SSO
-00008e10: 0a20 2020 2020 2020 2063 6c69 656e 745f  .        client_
-00008e20: 636f 6e6e 6563 7469 6f6e 203d 2072 6571  connection = req
-00008e30: 2e63 6c69 656e 745f 636f 6e6e 6563 7469  .client_connecti
-00008e40: 6f6e 5f73 736f 0a0a 2020 2020 2020 2020  on_sso..        
-00008e50: 7365 6c66 2e5f 696e 6974 6961 6c69 7a65  self._initialize
-00008e60: 5f63 6c69 656e 745f 636f 6e6e 6563 7469  _client_connecti
-00008e70: 6f6e 2863 6c69 656e 745f 636f 6e6e 6563  on(client_connec
-00008e80: 7469 6f6e 290a 2020 2020 2020 2020 2320  tion).        # 
-00008e90: 5365 6e64 206d 6573 7361 6765 0a20 2020  Send message.   
-00008ea0: 2020 2020 205f 7365 6e64 5f6d 7367 2873       _send_msg(s
-00008eb0: 656c 662c 2072 6571 290a 2020 2020 2020  elf, req).      
-00008ec0: 2020 2320 5265 6365 6976 6520 7265 7370    # Receive resp
-00008ed0: 6f6e 7365 0a20 2020 2020 2020 2072 7370  onse.        rsp
-00008ee0: 203d 205f 7265 6376 5f6d 7367 2873 656c   = _recv_msg(sel
-00008ef0: 662c 2070 726f 746f 2e43 6c69 656e 7443  f, proto.ClientC
-00008f00: 6f6e 6e65 6374 696f 6e53 534f 5265 7370  onnectionSSOResp
-00008f10: 6f6e 7365 2829 290a 0a20 2020 2020 2020  onse())..       
-00008f20: 2069 6620 7273 702e 7265 7370 6f6e 7365   if rsp.response
-00008f30: 2e74 7970 6520 3d3d 2070 726f 746f 2e43  .type == proto.C
-00008f40: 6f6e 6669 726d 6174 696f 6e52 6573 706f  onfirmationRespo
-00008f50: 6e73 652e 5245 5350 4f4e 5345 5f57 4152  nse.RESPONSE_WAR
-00008f60: 4e3a 0a20 2020 2020 2020 2020 2020 2077  N:.            w
-00008f70: 6172 6e28 7273 702e 7265 7370 6f6e 7365  arn(rsp.response
-00008f80: 2e72 6561 736f 6e29 0a20 2020 2020 2020  .reason).       
-00008f90: 2065 6c69 6620 6e6f 7420 7273 702e 7265   elif not rsp.re
-00008fa0: 7370 6f6e 7365 2e74 7970 6520 3d3d 2070  sponse.type == p
-00008fb0: 726f 746f 2e43 6f6e 6669 726d 6174 696f  roto.Confirmatio
-00008fc0: 6e52 6573 706f 6e73 652e 5245 5350 4f4e  nResponse.RESPON
-00008fd0: 5345 5f4f 4b3a 0a20 2020 2020 2020 2020  SE_OK:.         
-00008fe0: 2020 2072 6169 7365 205f 636f 6e76 6572     raise _conver
-00008ff0: 745f 6578 6365 7074 696f 6e28 7273 702e  t_exception(rsp.
-00009000: 7265 7370 6f6e 7365 290a 0a20 2020 2020  response)..     
-00009010: 2020 2023 204f 7065 6e20 6272 6f77 7365     # Open browse
-00009020: 7220 666f 7220 7573 6572 2074 6f20 6175  r for user to au
-00009030: 7468 656e 7469 6361 7465 2e0a 2020 2020  thenticate..    
-00009040: 2020 2020 6966 206e 6f74 206f 7065 6e5f      if not open_
-00009050: 6e65 7728 7273 702e 6175 7468 5572 6c29  new(rsp.authUrl)
-00009060: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
-00009070: 6767 6572 2e69 6e66 6f28 225b 7079 6f63  gger.info("[pyoc
-00009080: 6965 6e74 5d20 436f 756c 6420 6e6f 7420  ient] Could not 
-00009090: 6f70 656e 2064 6566 6175 6c74 2062 726f  open default bro
-000090a0: 7773 6572 2077 6974 6820 7765 6262 726f  wser with webbro
-000090b0: 7773 6572 206c 6962 7261 7279 2e20 506c  wser library. Pl
-000090c0: 6561 7365 2061 7574 6865 6e74 6963 6174  ease authenticat
-000090d0: 6520 6174 3a20 2220 2b20 7273 702e 6175  e at: " + rsp.au
-000090e0: 7468 5572 6c29 0a20 2020 2020 2020 2020  thUrl).         
-000090f0: 2020 2070 7269 6e74 2822 5b70 796f 6369     print("[pyoci
-00009100: 656e 745d 2043 6f75 6c64 206e 6f74 206f  ent] Could not o
-00009110: 7065 6e20 6465 6661 756c 7420 6272 6f77  pen default brow
-00009120: 7365 7220 7769 7468 2077 6562 6272 6f77  ser with webbrow
-00009130: 7365 7220 6c69 6272 6172 792e 2050 6c65  ser library. Ple
-00009140: 6173 6520 6175 7468 656e 7469 6361 7465  ase authenticate
-00009150: 2061 743a 2022 2c20 7273 702e 6175 7468   at: ", rsp.auth
-00009160: 5572 6c29 0a0a 2020 2020 2020 2020 2320  Url)..        # 
-00009170: 506f 6c6c 2074 6865 2064 6174 6162 6173  Poll the databas
-00009180: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
-00009190: 706f 6c6c 5f64 6174 6162 6173 6528 7273  poll_database(rs
-000091a0: 702e 7265 7175 6573 7449 6429 0a0a 2020  p.requestId)..  
-000091b0: 2020 6465 6620 5f70 6f6c 6c5f 6461 7461    def _poll_data
-000091c0: 6261 7365 2873 656c 662c 2072 6571 7565  base(self, reque
-000091d0: 7374 4964 293a 0a20 2020 2020 2020 2022  stId):.        "
-000091e0: 2222 506f 6c6c 7320 7468 6520 6461 7461  ""Polls the data
-000091f0: 6261 7365 2075 6e74 696c 2077 6520 6569  base until we ei
-00009200: 7468 6572 2072 6563 6569 7665 2061 6e20  ther receive an 
-00009210: 6572 726f 7220 6f72 2061 2073 7563 6365  error or a succe
-00009220: 7373 6675 6c20 6c6f 6769 6e20 6d65 7373  ssful login mess
-00009230: 6167 652e 0a0a 2020 2020 2020 2020 4172  age...        Ar
-00009240: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00009250: 7265 7175 6573 7449 6420 2853 7472 696e  requestId (Strin
-00009260: 6729 3a20 7468 6520 7265 7175 6573 7420  g): the request 
-00009270: 4944 2061 7373 6f63 6961 7465 6420 7769  ID associated wi
-00009280: 7468 2074 6869 7320 6c6f 6769 6e20 6174  th this login at
-00009290: 7465 6d70 742e 0a20 2020 2020 2020 2022  tempt..        "
-000092a0: 2222 0a0a 2020 2020 2020 2020 7265 7120  ""..        req 
-000092b0: 3d20 7072 6f74 6f2e 5265 7175 6573 7428  = proto.Request(
-000092c0: 290a 2020 2020 2020 2020 7265 712e 7479  ).        req.ty
-000092d0: 7065 203d 2072 6571 2e43 4c49 454e 545f  pe = req.CLIENT_
-000092e0: 434f 4e4e 4543 5449 4f4e 5f53 534f 320a  CONNECTION_SSO2.
-000092f0: 2020 2020 2020 2020 7265 712e 636c 6965          req.clie
-00009300: 6e74 5f63 6f6e 6e65 6374 696f 6e5f 7373  nt_connection_ss
-00009310: 6f32 2e66 6f72 6365 203d 2073 656c 662e  o2.force = self.
-00009320: 666f 7263 650a 2020 2020 2020 2020 7265  force.        re
-00009330: 712e 636c 6965 6e74 5f63 6f6e 6e65 6374  q.client_connect
-00009340: 696f 6e5f 7373 6f32 2e72 6571 7565 7374  ion_sso2.request
-00009350: 4964 203d 2072 6571 7565 7374 4964 0a0a  Id = requestId..
-00009360: 2020 2020 2020 2020 6b65 6570 506f 6c6c          keepPoll
-00009370: 696e 6720 3d20 5472 7565 0a20 2020 2020  ing = True.     
-00009380: 2020 2077 6169 7446 6f72 203d 2030 0a20     waitFor = 0. 
-00009390: 2020 2020 2020 2077 6869 6c65 206b 6565         while kee
-000093a0: 7050 6f6c 6c69 6e67 3a0a 2020 2020 2020  pPolling:.      
-000093b0: 2020 2020 2020 736c 6565 7028 7761 6974        sleep(wait
-000093c0: 466f 7229 0a20 2020 2020 2020 2020 2020  For).           
-000093d0: 2023 2050 6f6c 6c0a 2020 2020 2020 2020   # Poll.        
-000093e0: 2020 2020 5f73 656e 645f 6d73 6728 7365      _send_msg(se
-000093f0: 6c66 2c20 7265 7129 0a0a 2020 2020 2020  lf, req)..      
-00009400: 2020 2020 2020 2320 5265 6365 6976 6520        # Receive 
-00009410: 7265 7370 6f6e 7365 0a20 2020 2020 2020  response.       
-00009420: 2020 2020 2072 7370 203d 205f 7265 6376       rsp = _recv
-00009430: 5f6d 7367 2873 656c 662c 2070 726f 746f  _msg(self, proto
-00009440: 2e43 6c69 656e 7443 6f6e 6e65 6374 696f  .ClientConnectio
-00009450: 6e53 534f 3252 6573 706f 6e73 6528 2929  nSSO2Response())
-00009460: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00009470: 2072 7370 2e72 6573 706f 6e73 652e 7479   rsp.response.ty
-00009480: 7065 203d 3d20 7072 6f74 6f2e 436f 6e66  pe == proto.Conf
-00009490: 6972 6d61 7469 6f6e 5265 7370 6f6e 7365  irmationResponse
-000094a0: 2e52 4553 504f 4e53 455f 5741 524e 3a0a  .RESPONSE_WARN:.
-000094b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094c0: 7761 726e 2872 7370 2e72 6573 706f 6e73  warn(rsp.respons
-000094d0: 652e 7265 6173 6f6e 290a 2020 2020 2020  e.reason).      
-000094e0: 2020 2020 2020 656c 6966 206e 6f74 2072        elif not r
-000094f0: 7370 2e72 6573 706f 6e73 652e 7479 7065  sp.response.type
-00009500: 203d 3d20 7072 6f74 6f2e 436f 6e66 6972   == proto.Confir
-00009510: 6d61 7469 6f6e 5265 7370 6f6e 7365 2e52  mationResponse.R
-00009520: 4553 504f 4e53 455f 4f4b 3a0a 2020 2020  ESPONSE_OK:.    
-00009530: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00009540: 6520 5f63 6f6e 7665 7274 5f65 7863 6570  e _convert_excep
-00009550: 7469 6f6e 2872 7370 2e72 6573 706f 6e73  tion(rsp.respons
-00009560: 6529 0a0a 2020 2020 2020 2020 2020 2020  e)..            
-00009570: 6966 2072 7370 2e48 6173 4669 656c 6428  if rsp.HasField(
-00009580: 2270 6f6c 6c69 6e67 496e 7465 7276 616c  "pollingInterval
-00009590: 5365 636f 6e64 7322 293a 0a20 2020 2020  Seconds"):.     
-000095a0: 2020 2020 2020 2020 2020 2023 2043 6f6e             # Con
-000095b0: 7469 6e75 6520 706f 6c6c 696e 670a 2020  tinue polling.  
-000095c0: 2020 2020 2020 2020 2020 2020 2020 7761                wa
-000095d0: 6974 466f 7220 3d20 7273 702e 706f 6c6c  itFor = rsp.poll
-000095e0: 696e 6749 6e74 6572 7661 6c53 6563 6f6e  ingIntervalSecon
-000095f0: 6473 0a20 2020 2020 2020 2020 2020 2020  ds.             
-00009600: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
-00009610: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00009620: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00009630: 5375 6363 6573 730a 2020 2020 2020 2020  Success.        
-00009640: 2020 2020 2020 2020 7761 6974 466f 7220          waitFor 
-00009650: 3d20 300a 2020 2020 2020 2020 2020 2020  = 0.            
-00009660: 2020 2020 6b65 6570 506f 6c6c 696e 6720      keepPolling 
-00009670: 3d20 4661 6c73 650a 0a20 2020 2020 2020  = False..       
-00009680: 2073 656c 662e 7365 7276 6572 5365 7373   self.serverSess
-00009690: 696f 6e49 6420 3d20 7273 702e 7365 7373  ionId = rsp.sess
-000096a0: 696f 6e49 6e66 6f2e 7365 7276 6572 5365  ionInfo.serverSe
-000096b0: 7373 696f 6e49 640a 2020 2020 2020 2020  ssionId.        
-000096c0: 6c6f 6767 6572 2e64 6562 7567 2866 2243  logger.debug(f"C
-000096d0: 6f6e 6e65 6374 6564 2074 6f20 7365 7276  onnected to serv
-000096e0: 6572 2073 6573 7369 6f6e 2049 643a 207b  er session Id: {
-000096f0: 7365 6c66 2e73 6572 7665 7253 6573 7369  self.serverSessi
-00009700: 6f6e 4964 7d22 290a 2020 2020 2020 2020  onId}").        
-00009710: 7265 6365 6976 6564 5f74 6f6b 656e 203d  received_token =
-00009720: 2072 7370 2e73 6573 7369 6f6e 496e 666f   rsp.sessionInfo
-00009730: 2e73 6563 7572 6974 7954 6f6b 656e 0a20  .securityToken. 
-00009740: 2020 2020 2020 2073 656c 662e 7365 7373         self.sess
-00009750: 696f 6e20 3d20 5365 7373 696f 6e28 7365  ion = Session(se
-00009760: 6375 7269 7479 546f 6b65 6e3d 5365 6375  curityToken=Secu
-00009770: 7269 7479 546f 6b65 6e28 7265 6365 6976  rityToken(receiv
-00009780: 6564 5f74 6f6b 656e 2e64 6174 612c 2072  ed_token.data, r
-00009790: 6563 6569 7665 645f 746f 6b65 6e2e 7369  eceived_token.si
-000097a0: 676e 6174 7572 652c 2072 6563 6569 7665  gnature, receive
-000097b0: 645f 746f 6b65 6e2e 6973 7375 6572 4669  d_token.issuerFi
-000097c0: 6e67 6572 7072 696e 7429 290a 0a20 2020  ngerprint))..   
-000097d0: 2020 2020 2023 2053 6176 6520 7365 636f       # Save seco
-000097e0: 6e64 6172 7920 696e 7465 7266 6163 6573  ndary interfaces
-000097f0: 2e0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00009800: 7361 7665 5f73 6563 6f6e 6461 7279 5f69  save_secondary_i
-00009810: 6e74 6572 6661 6365 7328 7273 702e 7365  nterfaces(rsp.se
-00009820: 636f 6e64 6172 7929 0a0a 2020 2020 2020  condary)..      
-00009830: 2020 2320 5265 6469 7265 6374 2074 6865    # Redirect the
-00009840: 2063 6f6e 6e65 6374 696f 6e0a 2020 2020   connection.    
-00009850: 2020 2020 6966 2072 7370 2e72 6564 6972      if rsp.redir
-00009860: 6563 743a 0a20 2020 2020 2020 2020 2020  ect:.           
-00009870: 2073 656c 662e 736f 636b 2e63 6c6f 7365   self.sock.close
-00009880: 2829 0a20 2020 2020 2020 2020 2020 206d  ().            m
-00009890: 6170 7065 645f 686f 7374 2c20 6d61 7070  apped_host, mapp
-000098a0: 6564 5f70 6f72 7420 3d20 7365 6c66 2e72  ed_port = self.r
-000098b0: 6573 6f6c 7665 5f6e 6577 5f65 6e64 706f  esolve_new_endpo
-000098c0: 696e 7428 7273 702e 7265 6469 7265 6374  int(rsp.redirect
-000098d0: 486f 7374 2c20 7273 702e 7265 6469 7265  Host, rsp.redire
-000098e0: 6374 506f 7274 290a 2020 2020 2020 2020  ctPort).        
-000098f0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-00009900: 2866 2252 6564 6972 6563 7469 6e67 2063  (f"Redirecting c
-00009910: 6f6e 6e65 6374 696f 6e20 746f 207b 7273  onnection to {rs
-00009920: 702e 7265 6469 7265 6374 486f 7374 7d3a  p.redirectHost}:
-00009930: 7b72 7370 2e72 6564 6972 6563 7450 6f72  {rsp.redirectPor
-00009940: 747d 2c20 7768 6963 6820 6d61 7073 2074  t}, which maps t
-00009950: 6f20 7b6d 6170 7065 645f 686f 7374 7d3a  o {mapped_host}:
-00009960: 7b6d 6170 7065 645f 706f 7274 7d22 290a  {mapped_port}").
-00009970: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00009980: 2e73 6f63 6b20 3d20 736f 636b 6574 2e63  .sock = socket.c
-00009990: 7265 6174 655f 636f 6e6e 6563 7469 6f6e  reate_connection
-000099a0: 2828 6d61 7070 6564 5f68 6f73 742c 206d  ((mapped_host, m
-000099b0: 6170 7065 645f 706f 7274 2929 0a20 2020  apped_port)).   
-000099c0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-000099d0: 696e 666f 2866 2243 6f6e 6e65 6374 6564  info(f"Connected
-000099e0: 2074 6f20 7b6d 6170 7065 645f 686f 7374   to {mapped_host
-000099f0: 7d3a 7b6d 6170 7065 645f 706f 7274 7d20  }:{mapped_port} 
-00009a00: 6f6e 2073 6f63 6b65 7420 7b73 656c 662e  on socket {self.
-00009a10: 736f 636b 7d22 290a 2020 2020 2020 2020  sock}").        
-00009a20: 2020 2020 7365 6c66 2e5f 7373 6c69 7a65      self._sslize
-00009a30: 5f63 6f6e 6e65 6374 696f 6e28 290a 0a20  _connection().. 
-00009a40: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00009a50: 6e20 7365 6c66 2e5f 636c 6965 6e74 5f68  n self._client_h
-00009a60: 616e 6473 6861 6b65 5f73 6563 7572 6974  andshake_securit
-00009a70: 795f 746f 6b65 6e28 5472 7565 290a 0a20  y_token(True).. 
-00009a80: 2020 2064 6566 205f 636c 6965 6e74 5f68     def _client_h
-00009a90: 616e 6473 6861 6b65 5f73 6563 7572 6974  andshake_securit
-00009aa0: 795f 746f 6b65 6e28 7365 6c66 2c20 666f  y_token(self, fo
-00009ab0: 7263 653d 4661 6c73 6529 3a0a 2020 2020  rce=False):.    
-00009ac0: 2020 2020 2222 224f 6e63 6520 6120 636f      """Once a co
-00009ad0: 6e6e 6563 7469 6f6e 2061 6371 7569 7265  nnection acquire
-00009ae0: 7320 6120 7365 6375 7269 7479 2074 6f6b  s a security tok
-00009af0: 656e 2c20 6974 2063 616e 2075 7365 2074  en, it can use t
-00009b00: 6861 7420 746f 206c 6f67 2069 6e2e 2054  hat to log in. T
-00009b10: 6869 7320 6861 6e64 7368 616b 6520 6f6e  his handshake on
-00009b20: 6c79 0a20 2020 2020 2020 2073 656e 6473  ly.        sends
-00009b30: 2031 206d 6573 7361 6765 2077 6865 7265   1 message where
-00009b40: 6173 2074 6865 206f 7468 6572 2068 616e  as the other han
-00009b50: 6473 6861 6b65 7320 7365 6e64 2032 2e0a  dshakes send 2..
-00009b60: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00009b70: 2020 2020 7768 696c 6520 5472 7565 3a0a      while True:.
-00009b80: 2020 2020 2020 2020 2020 2020 7265 7120              req 
-00009b90: 3d20 7072 6f74 6f2e 5265 7175 6573 7428  = proto.Request(
-00009ba0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00009bb0: 712e 7479 7065 203d 2072 6571 2e43 4c49  q.type = req.CLI
-00009bc0: 454e 545f 434f 4e4e 4543 5449 4f4e 5f53  ENT_CONNECTION_S
-00009bd0: 4543 5552 4954 595f 544f 4b45 4e0a 2020  ECURITY_TOKEN.  
-00009be0: 2020 2020 2020 2020 2020 636c 6965 6e74            client
-00009bf0: 5f63 6f6e 6e65 6374 696f 6e20 3d20 7265  _connection = re
-00009c00: 712e 636c 6965 6e74 5f63 6f6e 6e65 6374  q.client_connect
-00009c10: 696f 6e5f 7365 6375 7269 7479 5f74 6f6b  ion_security_tok
-00009c20: 656e 0a0a 2020 2020 2020 2020 2020 2020  en..            
-00009c30: 7365 6c66 2e5f 696e 6974 6961 6c69 7a65  self._initialize
-00009c40: 5f63 6c69 656e 745f 636f 6e6e 6563 7469  _client_connecti
-00009c50: 6f6e 2863 6c69 656e 745f 636f 6e6e 6563  on(client_connec
-00009c60: 7469 6f6e 290a 2020 2020 2020 2020 2020  tion).          
-00009c70: 2020 2320 4174 7461 6368 2074 6865 2073    # Attach the s
-00009c80: 6563 7572 6974 7920 746f 6b65 6e20 7573  ecurity token us
-00009c90: 6564 2074 6f20 6c6f 6720 696e 0a20 2020  ed to log in.   
-00009ca0: 2020 2020 2020 2020 2063 6c69 656e 745f           client_
-00009cb0: 636f 6e6e 6563 7469 6f6e 2e73 6563 7572  connection.secur
-00009cc0: 6974 7954 6f6b 656e 203d 2073 656c 662e  ityToken = self.
-00009cd0: 7365 7373 696f 6e2e 7365 6375 7269 7479  session.security
-00009ce0: 546f 6b65 6e2e 746f 6b65 6e44 6174 610a  Token.tokenData.
-00009cf0: 2020 2020 2020 2020 2020 2020 636c 6965              clie
-00009d00: 6e74 5f63 6f6e 6e65 6374 696f 6e2e 746f  nt_connection.to
-00009d10: 6b65 6e53 6967 6e61 7475 7265 203d 2073  kenSignature = s
-00009d20: 656c 662e 7365 7373 696f 6e2e 7365 6375  elf.session.secu
-00009d30: 7269 7479 546f 6b65 6e2e 746f 6b65 6e53  rityToken.tokenS
-00009d40: 6967 6e61 7475 7265 0a20 2020 2020 2020  ignature.       
-00009d50: 2020 2020 2063 6c69 656e 745f 636f 6e6e       client_conn
-00009d60: 6563 7469 6f6e 2e69 7373 7565 7246 696e  ection.issuerFin
-00009d70: 6765 7270 7269 6e74 203d 2073 656c 662e  gerprint = self.
-00009d80: 7365 7373 696f 6e2e 7365 6375 7269 7479  session.security
-00009d90: 546f 6b65 6e2e 6973 7375 6572 4669 6e67  Token.issuerFing
-00009da0: 6572 7072 696e 740a 2020 2020 2020 2020  erprint.        
-00009db0: 2020 2020 636c 6965 6e74 5f63 6f6e 6e65      client_conne
-00009dc0: 6374 696f 6e2e 666f 7263 6520 3d20 666f  ction.force = fo
-00009dd0: 7263 650a 0a20 2020 2020 2020 2020 2020  rce..           
-00009de0: 205f 7365 6e64 5f6d 7367 2873 656c 662c   _send_msg(self,
-00009df0: 2072 6571 290a 0a20 2020 2020 2020 2020   req)..         
-00009e00: 2020 2072 7370 203d 205f 7265 6376 5f6d     rsp = _recv_m
-00009e10: 7367 2873 656c 662c 2070 726f 746f 2e43  sg(self, proto.C
-00009e20: 6c69 656e 7443 6f6e 6e65 6374 696f 6e53  lientConnectionS
-00009e30: 6563 7572 6974 7954 6f6b 656e 5265 7370  ecurityTokenResp
-00009e40: 6f6e 7365 2829 290a 0a20 2020 2020 2020  onse())..       
-00009e50: 2020 2020 2069 6620 7273 702e 7265 7370       if rsp.resp
-00009e60: 6f6e 7365 2e74 7970 6520 3d3d 2070 726f  onse.type == pro
-00009e70: 746f 2e43 6f6e 6669 726d 6174 696f 6e52  to.ConfirmationR
-00009e80: 6573 706f 6e73 652e 5245 5350 4f4e 5345  esponse.RESPONSE
-00009e90: 5f57 4152 4e3a 0a20 2020 2020 2020 2020  _WARN:.         
-00009ea0: 2020 2020 2020 2077 6172 6e28 7273 702e         warn(rsp.
-00009eb0: 7265 7370 6f6e 7365 2e72 6561 736f 6e29  response.reason)
-00009ec0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-00009ed0: 6620 7273 702e 7265 7370 6f6e 7365 2e74  f rsp.response.t
-00009ee0: 7970 6520 3d3d 2070 726f 746f 2e43 6f6e  ype == proto.Con
-00009ef0: 6669 726d 6174 696f 6e52 6573 706f 6e73  firmationRespons
-00009f00: 652e 5245 5350 4f4e 5345 5f4f 4b3a 0a20  e.RESPONSE_OK:. 
-00009f10: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00009f20: 2053 6176 6520 7365 636f 6e64 6172 7920   Save secondary 
-00009f30: 696e 7465 7266 6163 6573 2e0a 2020 2020  interfaces..    
-00009f40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00009f50: 2e5f 7361 7665 5f73 6563 6f6e 6461 7279  ._save_secondary
-00009f60: 5f69 6e74 6572 6661 6365 7328 7273 702e  _interfaces(rsp.
-00009f70: 7365 636f 6e64 6172 7929 0a20 2020 2020  secondary).     
-00009f80: 2020 2020 2020 2020 2020 2023 2052 6564             # Red
-00009f90: 6972 6563 7420 7468 6520 636f 6e6e 6563  irect the connec
-00009fa0: 7469 6f6e 2069 6620 7265 7175 6573 7465  tion if requeste
-00009fb0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-00009fc0: 2020 6966 2072 7370 2e72 6564 6972 6563    if rsp.redirec
-00009fd0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-00009fe0: 2020 2020 2020 2073 656c 662e 736f 636b         self.sock
-00009ff0: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
-0000a000: 2020 2020 2020 2020 2020 2020 206d 6170               map
-0000a010: 7065 645f 686f 7374 2c20 6d61 7070 6564  ped_host, mapped
-0000a020: 5f70 6f72 7420 3d20 7365 6c66 2e72 6573  _port = self.res
-0000a030: 6f6c 7665 5f6e 6577 5f65 6e64 706f 696e  olve_new_endpoin
-0000a040: 7428 7273 702e 7265 6469 7265 6374 486f  t(rsp.redirectHo
-0000a050: 7374 2c20 7273 702e 7265 6469 7265 6374  st, rsp.redirect
-0000a060: 506f 7274 290a 2020 2020 2020 2020 2020  Port).          
-0000a070: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000a080: 2e64 6562 7567 2866 2252 6564 6972 6563  .debug(f"Redirec
-0000a090: 7469 6e67 2063 6f6e 6e65 6374 696f 6e20  ting connection 
-0000a0a0: 746f 207b 7273 702e 7265 6469 7265 6374  to {rsp.redirect
-0000a0b0: 486f 7374 7d3a 7b72 7370 2e72 6564 6972  Host}:{rsp.redir
-0000a0c0: 6563 7450 6f72 747d 2c20 7768 6963 6820  ectPort}, which 
-0000a0d0: 6d61 7073 2074 6f20 7b6d 6170 7065 645f  maps to {mapped_
-0000a0e0: 686f 7374 7d3a 7b6d 6170 7065 645f 706f  host}:{mapped_po
-0000a0f0: 7274 7d22 290a 2020 2020 2020 2020 2020  rt}").          
-0000a100: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0000a110: 6f63 6b20 3d20 736f 636b 6574 2e63 7265  ock = socket.cre
-0000a120: 6174 655f 636f 6e6e 6563 7469 6f6e 2828  ate_connection((
-0000a130: 6d61 7070 6564 5f68 6f73 742c 206d 6170  mapped_host, map
-0000a140: 7065 645f 706f 7274 2929 0a20 2020 2020  ped_port)).     
-0000a150: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000a160: 6f67 6765 722e 696e 666f 2866 2243 6f6e  ogger.info(f"Con
-0000a170: 6e65 6374 6564 2074 6f20 7b6d 6170 7065  nected to {mappe
-0000a180: 645f 686f 7374 7d3a 7b6d 6170 7065 645f  d_host}:{mapped_
-0000a190: 706f 7274 7d20 6f6e 2073 6f63 6b65 7420  port} on socket 
-0000a1a0: 7b73 656c 662e 736f 636b 7d22 290a 2020  {self.sock}").  
-0000a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1c0: 2020 7365 6c66 2e5f 7373 6c69 7a65 5f63    self._sslize_c
-0000a1d0: 6f6e 6e65 6374 696f 6e28 290a 0a20 2020  onnection()..   
-0000a1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1f0: 2072 6574 7572 6e20 7365 6c66 2e5f 636c   return self._cl
-0000a200: 6965 6e74 5f68 616e 6473 6861 6b65 5f73  ient_handshake_s
-0000a210: 6563 7572 6974 795f 746f 6b65 6e28 5472  ecurity_token(Tr
-0000a220: 7565 290a 0a20 2020 2020 2020 2020 2020  ue)..           
-0000a230: 2020 2020 2023 2043 6170 7475 7265 2074       # Capture t
-0000a240: 6865 2073 6573 7369 6f6e 2069 640a 2020  he session id.  
-0000a250: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000a260: 6c66 2e73 6572 7665 7253 6573 7369 6f6e  lf.serverSession
-0000a270: 4964 203d 2072 7370 2e73 6572 7665 7253  Id = rsp.serverS
-0000a280: 6573 7369 6f6e 4964 0a20 2020 2020 2020  essionId.       
-0000a290: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-0000a2a0: 6465 6275 6728 6622 436f 6e6e 6563 7465  debug(f"Connecte
-0000a2b0: 6420 746f 2073 6572 7665 7220 7365 7373  d to server sess
-0000a2c0: 696f 6e20 4964 3a20 7b73 656c 662e 7365  ion Id: {self.se
-0000a2d0: 7276 6572 5365 7373 696f 6e49 647d 2229  rverSessionId}")
-0000a2e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a2f0: 2062 7265 616b 0a20 2020 2020 2020 2020   break.         
-0000a300: 2020 2023 2074 6865 7265 2069 7320 736f     # there is so
-0000a310: 6d65 7468 696e 6720 6272 6f6b 656e 2069  mething broken i
-0000a320: 6e20 6f75 7220 6861 6e64 7368 616b 652e  n our handshake.
-0000a330: 2e2e 7265 7472 790a 2020 2020 2020 2020  ..retry.        
-0000a340: 2020 2020 6966 2072 7370 2e72 6573 706f      if rsp.respo
-0000a350: 6e73 652e 7665 6e64 6f72 5f63 6f64 6520  nse.vendor_code 
-0000a360: 3d3d 202d 3230 323a 0a20 2020 2020 2020  == -202:.       
-0000a370: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-0000a380: 6465 6275 6728 2248 616e 6473 6861 6b65  debug("Handshake
-0000a390: 2065 7272 6f72 2e2e 2e72 6574 7279 696e   error...retryin
-0000a3a0: 6722 290a 2020 2020 2020 2020 2020 2020  g").            
-0000a3b0: 2020 2020 636f 6e74 696e 7565 0a0a 2020      continue..  
-0000a3c0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000a3d0: 5f63 6f6e 7665 7274 5f65 7863 6570 7469  _convert_excepti
-0000a3e0: 6f6e 2872 7370 2e72 6573 706f 6e73 6529  on(rsp.response)
-0000a3f0: 0a0a 2020 2020 6465 6620 5f73 6176 655f  ..    def _save_
-0000a400: 7365 636f 6e64 6172 795f 696e 7465 7266  secondary_interf
-0000a410: 6163 6573 2873 656c 662c 206e 6577 5f73  aces(self, new_s
-0000a420: 6563 6f6e 6461 7279 5f69 6e74 6572 6661  econdary_interfa
-0000a430: 6365 7329 3a0a 2020 2020 2020 2020 2222  ces):.        ""
-0000a440: 2241 6674 6572 2073 6563 6f6e 6461 7279  "After secondary
-0000a450: 2069 6e74 6572 6661 6365 7320 6172 6520   interfaces are 
-0000a460: 7365 6e74 2066 726f 6d20 7468 6520 7365  sent from the se
-0000a470: 7276 6572 2c20 7765 206e 6565 6420 746f  rver, we need to
-0000a480: 0a20 2020 2020 2020 2073 6176 6520 7468  .        save th
-0000a490: 656d 2061 6e64 2075 7365 2074 6865 6d20  em and use them 
-0000a4a0: 666f 7220 7265 6469 7265 6374 696e 672e  for redirecting.
-0000a4b0: 2054 6869 7320 6973 2069 6d70 6f72 7461   This is importa
-0000a4c0: 6e74 2069 6620 7765 0a20 2020 2020 2020  nt if we.       
-0000a4d0: 2067 6574 2072 6564 6972 6563 7465 6420   get redirected 
-0000a4e0: 746f 206d 6170 7065 6420 7371 6c20 656e  to mapped sql en
-0000a4f0: 6470 6f69 6e74 732e 0a0a 2020 2020 2020  dpoints...      
-0000a500: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-0000a510: 2020 2020 7365 636f 6e64 6172 795f 696e      secondary_in
-0000a520: 7465 7266 6163 6573 2028 5b63 6c61 7373  terfaces ([class
-0000a530: 2027 676f 6f67 6c65 2e70 726f 746f 6275   'google.protobu
-0000a540: 662e 7079 6578 742e 5f6d 6573 7361 6765  f.pyext._message
-0000a550: 2e52 6570 6561 7465 6443 6f6d 706f 7369  .RepeatedComposi
-0000a560: 7465 436f 6e74 6169 6e65 7227 5d29 3a0a  teContainer']):.
-0000a570: 2020 2020 2020 2020 2020 2020 7468 6520              the 
-0000a580: 7365 636f 6e64 6172 7920 696e 7465 7266  secondary interf
-0000a590: 6163 6573 2c20 7768 6963 6820 6973 2072  aces, which is r
-0000a5a0: 6561 6c6c 7920 6120 6c69 7374 206f 6620  eally a list of 
-0000a5b0: 6c69 7374 206f 6620 7374 7269 6e67 732e  list of strings.
-0000a5c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000a5d0: 2020 2020 2073 656c 662e 7365 636f 6e64       self.second
-0000a5e0: 6172 795f 696e 7465 7266 6163 6573 203d  ary_interfaces =
-0000a5f0: 205b 5d0a 2020 2020 2020 2020 666f 7220   [].        for 
-0000a600: 6920 696e 2072 616e 6765 286c 656e 286e  i in range(len(n
-0000a610: 6577 5f73 6563 6f6e 6461 7279 5f69 6e74  ew_secondary_int
-0000a620: 6572 6661 6365 7329 293a 0a20 2020 2020  erfaces)):.     
-0000a630: 2020 2020 2020 2073 656c 662e 7365 636f         self.seco
-0000a640: 6e64 6172 795f 696e 7465 7266 6163 6573  ndary_interfaces
-0000a650: 2e61 7070 656e 6428 5b5d 290a 2020 2020  .append([]).    
-0000a660: 2020 2020 2020 2020 666f 7220 6a20 696e          for j in
-0000a670: 2072 616e 6765 286c 656e 286e 6577 5f73   range(len(new_s
-0000a680: 6563 6f6e 6461 7279 5f69 6e74 6572 6661  econdary_interfa
-0000a690: 6365 735b 695d 2e61 6464 7265 7373 2929  ces[i].address))
-0000a6a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a6b0: 2020 696e 7465 7266 6163 6520 3d20 6e65    interface = ne
-0000a6c0: 775f 7365 636f 6e64 6172 795f 696e 7465  w_secondary_inte
-0000a6d0: 7266 6163 6573 5b69 5d2e 6164 6472 6573  rfaces[i].addres
-0000a6e0: 735b 6a5d 0a20 2020 2020 2020 2020 2020  s[j].           
-0000a6f0: 2020 2020 2028 696e 7465 7266 6163 655f       (interface_
-0000a700: 6970 2c20 696e 7465 7266 6163 655f 706f  ip, interface_po
-0000a710: 7274 2920 3d20 696e 7465 7266 6163 652e  rt) = interface.
-0000a720: 7370 6c69 7428 223a 2229 0a20 2020 2020  split(":").     
-0000a730: 2020 2020 2020 2020 2020 2023 2052 6574             # Ret
-0000a740: 7572 6e20 6f66 2067 6574 686f 7374 6279  urn of gethostby
-0000a750: 6e61 6d65 5f65 7820 6973 2028 686f 7374  name_ex is (host
-0000a760: 6e61 6d65 2c20 616c 6961 7320 6f66 2068  name, alias of h
-0000a770: 6f73 7420 6e61 6d65 2c20 6f74 6865 7220  ost name, other 
-0000a780: 6970 2061 6464 7265 7373 6573 206f 6620  ip addresses of 
-0000a790: 686f 7374 206e 616d 6529 0a20 2020 2020  host name).     
-0000a7a0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-0000a7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7c0: 2020 2020 6f74 6865 725f 6970 7320 3d20      other_ips = 
-0000a7d0: 736f 636b 6574 2e67 6574 686f 7374 6279  socket.gethostby
-0000a7e0: 6e61 6d65 5f65 7828 696e 7465 7266 6163  name_ex(interfac
-0000a7f0: 655f 6970 295b 325d 0a20 2020 2020 2020  e_ip)[2].       
-0000a800: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000a810: 206f 7468 6572 5f69 7020 696e 206f 7468   other_ip in oth
-0000a820: 6572 5f69 7073 3a0a 2020 2020 2020 2020  er_ips:.        
-0000a830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a840: 7365 6c66 2e73 6563 6f6e 6461 7279 5f69  self.secondary_i
-0000a850: 6e74 6572 6661 6365 735b 695d 2e61 7070  nterfaces[i].app
-0000a860: 656e 6428 286f 7468 6572 5f69 702c 2069  end((other_ip, i
-0000a870: 6e74 2869 6e74 6572 6661 6365 5f70 6f72  nt(interface_por
-0000a880: 7429 2929 0a20 2020 2020 2020 2020 2020  t))).           
-0000a890: 2020 2020 2065 7863 6570 7420 736f 636b       except sock
-0000a8a0: 6574 2e67 6169 6572 726f 723a 0a20 2020  et.gaierror:.   
-0000a8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8c0: 2070 6173 730a 0a20 2020 2020 2020 2068   pass..        h
-0000a8d0: 6f73 7473 203d 205b 5d0a 2020 2020 2020  osts = [].      
-0000a8e0: 2020 666f 7220 6f6e 655f 686f 7374 2069    for one_host i
-0000a8f0: 6e20 7365 6c66 2e68 6f73 7473 3a0a 2020  n self.hosts:.  
-0000a900: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
-0000a910: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-0000a920: 6f73 7473 203d 2068 6f73 7473 202b 205b  osts = hosts + [
-0000a930: 2868 6f73 742c 2073 656c 662e 706f 7274  (host, self.port
-0000a940: 2920 666f 7220 686f 7374 2069 6e20 736f  ) for host in so
-0000a950: 636b 6574 2e67 6574 686f 7374 6279 6e61  cket.gethostbyna
-0000a960: 6d65 5f65 7828 6f6e 655f 686f 7374 295b  me_ex(one_host)[
-0000a970: 325d 5d0a 2020 2020 2020 2020 2020 2020  2]].            
-0000a980: 6578 6365 7074 2073 6f63 6b65 742e 6761  except socket.ga
-0000a990: 6965 7272 6f72 3a0a 2020 2020 2020 2020  ierror:.        
-0000a9a0: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
-0000a9b0: 2020 2020 2066 6f72 206f 7574 6572 5f6c       for outer_l
-0000a9c0: 6973 7420 696e 2073 656c 662e 7365 636f  ist in self.seco
-0000a9d0: 6e64 6172 795f 696e 7465 7266 6163 6573  ndary_interfaces
-0000a9e0: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-0000a9f0: 7220 696e 6465 7820 696e 2072 616e 6765  r index in range
-0000aa00: 286c 656e 286f 7574 6572 5f6c 6973 7429  (len(outer_list)
-0000aa10: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000aa20: 2020 2069 6620 6f75 7465 725f 6c69 7374     if outer_list
-0000aa30: 5b69 6e64 6578 5d20 696e 2068 6f73 7473  [index] in hosts
-0000aa40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000aa50: 2020 2020 2020 7365 6c66 2e73 6563 6f6e        self.secon
-0000aa60: 6461 7279 5f69 6e64 6578 203d 2069 6e64  dary_index = ind
-0000aa70: 6578 0a20 2020 2020 2020 2020 2020 2020  ex.             
-0000aa80: 2020 2020 2020 2062 7265 616b 0a0a 2020         break..  
-0000aa90: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-0000aaa0: 7567 2866 2253 6176 696e 6720 7365 636f  ug(f"Saving seco
-0000aab0: 6e64 6172 7920 696e 7465 7266 6163 6573  ndary interfaces
-0000aac0: 3a20 696e 6465 7820 7b73 656c 662e 7365  : index {self.se
-0000aad0: 636f 6e64 6172 795f 696e 6465 787d 2069  condary_index} i
-0000aae0: 6e74 6572 6661 6365 733a 207b 7365 6c66  nterfaces: {self
-0000aaf0: 2e73 6563 6f6e 6461 7279 5f69 6e74 6572  .secondary_inter
-0000ab00: 6661 6365 737d 2229 0a0a 2020 2020 6465  faces}")..    de
-0000ab10: 6620 5f65 6e63 7279 7074 696f 6e5f 726f  f _encryption_ro
-0000ab20: 7574 696e 6528 7365 6c66 2c20 696e 6974  utine(self, init
-0000ab30: 6961 6c69 7a61 7469 6f6e 5f76 6563 746f  ialization_vecto
-0000ab40: 722c 2070 6565 725f 6b65 7929 3a0a 2020  r, peer_key):.  
-0000ab50: 2020 2020 2020 2222 2249 6e74 6572 6e61        """Interna
-0000ab60: 6c20 726f 7574 696e 6520 746f 2064 6f20  l routine to do 
-0000ab70: 7468 6520 656e 6372 7970 7469 6f6e 2068  the encryption h
-0000ab80: 616e 6473 6861 6b65 206f 660a 2020 2020  andshake of.    
-0000ab90: 2020 2020 7468 6520 7061 7373 776f 7264      the password
-0000aba0: 0a20 2020 2020 2020 2043 4243 2069 7320  .        CBC is 
-0000abb0: 7468 6520 7072 6576 696f 7573 2066 6f72  the previous for
-0000abc0: 6d20 6f66 2065 6e63 7279 7074 696f 6e2e  m of encryption.
-0000abd0: 2057 6520 6e6f 7720 7573 6520 4743 4d20   We now use GCM 
-0000abe0: 6279 2064 6566 6175 6c74 2e0a 2020 2020  by default..    
-0000abf0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000ac00: 2320 4372 6561 7465 206f 7572 206b 6579  # Create our key
-0000ac10: 7320 7573 696e 6720 7468 6520 7061 7261  s using the para
-0000ac20: 6d65 7465 7273 2066 726f 6d20 7468 6520  meters from the 
-0000ac30: 7065 6572 206b 6579 0a20 2020 2020 2020  peer key.       
-0000ac40: 2070 6172 616d 7320 3d20 7065 6572 5f6b   params = peer_k
-0000ac50: 6579 2e70 6172 616d 6574 6572 7328 290a  ey.parameters().
-0000ac60: 2020 2020 2020 2020 7072 6976 6174 655f          private_
-0000ac70: 6b65 7920 3d20 7061 7261 6d73 2e67 656e  key = params.gen
-0000ac80: 6572 6174 655f 7072 6976 6174 655f 6b65  erate_private_ke
-0000ac90: 7928 290a 0a20 2020 2020 2020 2023 2043  y()..        # C
-0000aca0: 7265 6174 6520 6120 7368 6172 6564 206b  reate a shared k
-0000acb0: 6579 0a20 2020 2020 2020 2073 6861 7265  ey.        share
-0000acc0: 645f 6b65 7920 3d20 7072 6976 6174 655f  d_key = private_
-0000acd0: 6b65 792e 6578 6368 616e 6765 2870 6565  key.exchange(pee
-0000ace0: 725f 6b65 7929 0a0a 2020 2020 2020 2020  r_key)..        
-0000acf0: 6b65 7920 3d20 5f68 6173 685f 6b65 7928  key = _hash_key(
-0000ad00: 7368 6172 6564 5f6b 6579 2c20 6222 5c30  shared_key, b"\0
-0000ad10: 2229 0a20 2020 2020 2020 206d 6163 5f6b  ").        mac_k
-0000ad20: 6579 203d 205f 6861 7368 5f6b 6579 2873  ey = _hash_key(s
-0000ad30: 6861 7265 645f 6b65 792c 2062 225c 3122  hared_key, b"\1"
-0000ad40: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
-0000ad50: 6c66 2e68 616e 6473 6861 6b65 203d 3d20  lf.handshake == 
-0000ad60: 7365 6c66 2e48 414e 4453 4841 4b45 5f43  self.HANDSHAKE_C
-0000ad70: 4243 3a0a 2020 2020 2020 2020 2020 2020  BC:.            
-0000ad80: 2320 5061 6420 7468 6520 706c 6169 6e74  # Pad the plaint
-0000ad90: 6578 7420 7061 7373 776f 7264 206f 7574  ext password out
-0000ada0: 2075 7369 6e67 2050 4b43 5337 0a20 2020   using PKCS7.   
-0000adb0: 2020 2020 2020 2020 2070 6164 6465 7220           padder 
-0000adc0: 3d20 7061 6464 696e 672e 504b 4353 3728  = padding.PKCS7(
-0000add0: 3132 3829 2e70 6164 6465 7228 290a 2020  128).padder().  
-0000ade0: 2020 2020 2020 2020 2020 7061 6464 6564            padded
-0000adf0: 5f64 6174 6120 3d20 7061 6464 6572 2e75  _data = padder.u
-0000ae00: 7064 6174 6528 7365 6c66 2e70 6173 7377  pdate(self.passw
-0000ae10: 6f72 642e 656e 636f 6465 2865 6e63 6f64  ord.encode(encod
-0000ae20: 696e 673d 2255 5446 2d38 222c 2065 7272  ing="UTF-8", err
-0000ae30: 6f72 733d 2273 7472 6963 7422 2929 0a20  ors="strict")). 
-0000ae40: 2020 2020 2020 2020 2020 2070 6164 6465             padde
-0000ae50: 645f 6461 7461 202b 3d20 7061 6464 6572  d_data += padder
-0000ae60: 2e66 696e 616c 697a 6528 290a 0a20 2020  .finalize()..   
-0000ae70: 2020 2020 2020 2020 2023 2045 6e63 7279           # Encry
-0000ae80: 7074 2074 6865 2070 6164 6465 6420 706c  pt the padded pl
-0000ae90: 6169 6e74 6578 7420 7061 7373 776f 7264  aintext password
-0000aea0: 2075 7369 6e67 2041 4553 2043 4243 2061   using AES CBC a
-0000aeb0: 6e64 2074 6865 206b 6579 0a20 2020 2020  nd the key.     
-0000aec0: 2020 2020 2020 2023 2077 6520 676f 7420         # we got 
-0000aed0: 6672 6f6d 206f 7572 204b 4446 0a20 2020  from our KDF.   
-0000aee0: 2020 2020 2020 2020 2065 6e63 7279 7074           encrypt
-0000aef0: 6f72 203d 2043 6970 6865 7228 616c 676f  or = Cipher(algo
-0000af00: 7269 7468 6d73 2e41 4553 286b 6579 292c  rithms.AES(key),
-0000af10: 206d 6f64 6573 2e43 4243 2869 6e69 7469   modes.CBC(initi
-0000af20: 616c 697a 6174 696f 6e5f 7665 6374 6f72  alization_vector
-0000af30: 292c 2062 6163 6b65 6e64 3d64 6566 6175  ), backend=defau
-0000af40: 6c74 5f62 6163 6b65 6e64 2829 292e 656e  lt_backend()).en
-0000af50: 6372 7970 746f 7228 290a 2020 2020 2020  cryptor().      
-0000af60: 2020 2020 2020 6d69 6e5f 6369 7068 6572        min_cipher
-0000af70: 5f62 7974 6573 203d 206c 656e 2870 6164  _bytes = len(pad
-0000af80: 6465 645f 6461 7461 2920 2b20 3430 3936  ded_data) + 4096
-0000af90: 0a20 2020 2020 2020 2020 2020 2063 6970  .            cip
-0000afa0: 6865 7220 3d20 6279 7465 6172 7261 7928  her = bytearray(
-0000afb0: 6d69 6e5f 6369 7068 6572 5f62 7974 6573  min_cipher_bytes
-0000afc0: 290a 2020 2020 2020 2020 2020 2020 6c65  ).            le
-0000afd0: 6e5f 656e 6372 7970 7465 6420 3d20 656e  n_encrypted = en
-0000afe0: 6372 7970 746f 722e 7570 6461 7465 5f69  cryptor.update_i
-0000aff0: 6e74 6f28 7061 6464 6564 5f64 6174 612c  nto(padded_data,
-0000b000: 2063 6970 6865 7229 0a20 2020 2020 2020   cipher).       
-0000b010: 2020 2020 2063 6970 6865 7220 3d20 6279       cipher = by
-0000b020: 7465 7328 6369 7068 6572 5b3a 6c65 6e5f  tes(cipher[:len_
-0000b030: 656e 6372 7970 7465 645d 2920 2b20 656e  encrypted]) + en
-0000b040: 6372 7970 746f 722e 6669 6e61 6c69 7a65  cryptor.finalize
-0000b050: 2829 0a20 2020 2020 2020 2065 6c73 653a  ().        else:
-0000b060: 0a20 2020 2020 2020 2020 2020 2065 6e63  .            enc
-0000b070: 7279 7074 6f72 203d 2043 6970 6865 7228  ryptor = Cipher(
-0000b080: 616c 676f 7269 7468 6d73 2e41 4553 286b  algorithms.AES(k
-0000b090: 6579 292c 206d 6f64 6573 2e47 434d 2869  ey), modes.GCM(i
-0000b0a0: 6e69 7469 616c 697a 6174 696f 6e5f 7665  nitialization_ve
-0000b0b0: 6374 6f72 292c 2062 6163 6b65 6e64 3d64  ctor), backend=d
-0000b0c0: 6566 6175 6c74 5f62 6163 6b65 6e64 2829  efault_backend()
-0000b0d0: 292e 656e 6372 7970 746f 7228 290a 2020  ).encryptor().  
-0000b0e0: 2020 2020 2020 2020 2020 2320 5765 2064            # We d
-0000b0f0: 6f20 6e6f 7420 7573 6520 4141 440a 2020  o not use AAD.  
-0000b100: 2020 2020 2020 2020 2020 6369 7068 6572            cipher
-0000b110: 203d 2065 6e63 7279 7074 6f72 2e75 7064   = encryptor.upd
-0000b120: 6174 6528 7365 6c66 2e70 6173 7377 6f72  ate(self.passwor
-0000b130: 642e 656e 636f 6465 2865 6e63 6f64 696e  d.encode(encodin
-0000b140: 673d 2255 5446 2d38 222c 2065 7272 6f72  g="UTF-8", error
-0000b150: 733d 2273 7472 6963 7422 2929 202b 2065  s="strict")) + e
-0000b160: 6e63 7279 7074 6f72 2e66 696e 616c 697a  ncryptor.finaliz
-0000b170: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-0000b180: 2320 5365 7276 6572 2073 6964 6520 6578  # Server side ex
-0000b190: 7065 6374 7320 7468 6174 2074 6865 2074  pects that the t
-0000b1a0: 6167 2069 7320 6174 2074 6865 2065 6e64  ag is at the end
-0000b1b0: 206f 6620 7468 6520 6369 7068 6572 2074   of the cipher t
-0000b1c0: 6578 742e 0a20 2020 2020 2020 2020 2020  ext..           
-0000b1d0: 2063 6970 6865 7220 2b3d 2065 6e63 7279   cipher += encry
-0000b1e0: 7074 6f72 2e74 6167 0a0a 2020 2020 2020  ptor.tag..      
-0000b1f0: 2020 2320 4e6f 7720 6372 6561 7465 2061    # Now create a
-0000b200: 6e20 484d 4143 2075 7369 6e67 2074 6865  n HMAC using the
-0000b210: 206f 7468 6572 204b 4446 2064 6572 6976   other KDF deriv
-0000b220: 6564 206b 6579 2061 6e64 2074 6865 0a20  ed key and the. 
-0000b230: 2020 2020 2020 2023 2065 6e63 7279 7074         # encrypt
-0000b240: 6564 2070 6173 7377 6f72 640a 2020 2020  ed password.    
-0000b250: 2020 2020 6861 7368 6572 203d 2068 6d61      hasher = hma
-0000b260: 632e 484d 4143 286d 6163 5f6b 6579 2c20  c.HMAC(mac_key, 
-0000b270: 6861 7368 6573 2e53 4841 3235 3628 292c  hashes.SHA256(),
-0000b280: 2062 6163 6b65 6e64 3d64 6566 6175 6c74   backend=default
-0000b290: 5f62 6163 6b65 6e64 2829 290a 2020 2020  _backend()).    
-0000b2a0: 2020 2020 6861 7368 6572 2e75 7064 6174      hasher.updat
-0000b2b0: 6528 6369 7068 6572 290a 2020 2020 2020  e(cipher).      
-0000b2c0: 2020 6765 6e65 7261 7465 645f 686d 6163    generated_hmac
-0000b2d0: 203d 2068 6173 6865 722e 6669 6e61 6c69   = hasher.finali
-0000b2e0: 7a65 2829 0a0a 2020 2020 2020 2020 7265  ze()..        re
-0000b2f0: 7475 726e 2028 6369 7068 6572 2c20 6765  turn (cipher, ge
-0000b300: 6e65 7261 7465 645f 686d 6163 2c20 7072  nerated_hmac, pr
-0000b310: 6976 6174 655f 6b65 792e 7075 626c 6963  ivate_key.public
-0000b320: 5f6b 6579 2829 290a 0a20 2020 2064 6566  _key())..    def
-0000b330: 205f 7061 7273 655f 6172 6773 2873 656c   _parse_args(sel
-0000b340: 662c 2064 736e 2c20 7573 6572 2c20 7061  f, dsn, user, pa
-0000b350: 7373 776f 7264 2c20 686f 7374 2c20 6461  ssword, host, da
-0000b360: 7461 6261 7365 2c20 746c 732c 2068 616e  tabase, tls, han
-0000b370: 6473 6861 6b65 2c20 666f 7263 652c 2063  dshake, force, c
-0000b380: 6f6e 6669 6766 696c 6529 3a20 2023 2070  onfigfile):  # p
-0000b390: 796c 696e 743a 2064 6973 6162 6c65 3d74  ylint: disable=t
-0000b3a0: 6f6f 2d6d 616e 792d 6172 6775 6d65 6e74  oo-many-argument
-0000b3b0: 730a 2020 2020 2020 2020 2222 2249 6e74  s.        """Int
-0000b3c0: 6572 6e61 6c20 726f 7574 696e 6520 746f  ernal routine to
-0000b3d0: 2072 6573 6f6c 7665 2066 756e 6374 696f   resolve functio
-0000b3e0: 6e20 6172 6775 6d65 6e74 732c 2063 6f6e  n arguments, con
-0000b3f0: 6669 6720 6669 6c65 2c20 616e 6420 6473  fig file, and ds
-0000b400: 6e22 2222 0a20 2020 2020 2020 2023 2070  n""".        # p
-0000b410: 796c 696e 743a 2064 6973 6162 6c65 3d6e  ylint: disable=n
-0000b420: 6f2d 6d65 6d62 6572 2c74 6f6f 2d6d 616e  o-member,too-man
-0000b430: 792d 6272 616e 6368 6573 2c74 6f6f 2d6d  y-branches,too-m
-0000b440: 616e 792d 7374 6174 656d 656e 7473 0a20  any-statements. 
-0000b450: 2020 2020 2020 2023 2046 6972 7374 2c20         # First, 
-0000b460: 7061 7273 6520 7468 6520 4453 4e20 6966  parse the DSN if
-0000b470: 2069 7420 6578 6973 7473 0a20 2020 2020   it exists.     
-0000b480: 2020 2069 6620 6473 6e20 6973 206e 6f74     if dsn is not
-0000b490: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000b4a0: 2020 2070 6172 7365 6420 3d20 6473 6e70     parsed = dsnp
-0000b4b0: 6172 7365 2e70 6172 7365 2864 736e 290a  arse.parse(dsn).
-0000b4c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000b4d0: 7061 7273 6564 2e73 6368 656d 6520 616e  parsed.scheme an
-0000b4e0: 6420 7061 7273 6564 2e73 6368 656d 652e  d parsed.scheme.
-0000b4f0: 6c6f 7765 7228 2920 213d 2022 6f63 6965  lower() != "ocie
-0000b500: 6e74 223a 0a20 2020 2020 2020 2020 2020  nt":.           
-0000b510: 2020 2020 2072 6169 7365 204d 616c 666f       raise Malfo
-0000b520: 726d 6564 5552 4c28 6622 496e 7661 6c69  rmedURL(f"Invali
-0000b530: 6420 4453 4e20 7363 6865 6d65 3a20 7b70  d DSN scheme: {p
-0000b540: 6172 7365 642e 7363 6865 6d65 7d22 290a  arsed.scheme}").
-0000b550: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000b560: 2061 7474 7220 696e 205b 2264 6174 6162   attr in ["datab
-0000b570: 6173 6522 2c20 2275 7365 7222 2c20 2270  ase", "user", "p
-0000b580: 6173 7377 6f72 6422 2c20 2270 6f72 7422  assword", "port"
-0000b590: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-0000b5a0: 2020 2073 6574 6174 7472 2873 656c 662c     setattr(self,
-0000b5b0: 2061 7474 722c 2067 6574 6174 7472 2870   attr, getattr(p
-0000b5c0: 6172 7365 642c 2061 7474 7229 290a 0a20  arsed, attr)).. 
-0000b5d0: 2020 2020 2020 2020 2020 2069 6620 7061             if pa
-0000b5e0: 7273 6564 2e68 6f73 743a 0a20 2020 2020  rsed.host:.     
-0000b5f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b600: 686f 7374 7320 3d20 7061 7273 6564 2e68  hosts = parsed.h
-0000b610: 6f73 742e 7370 6c69 7428 222c 2229 0a0a  ost.split(",")..
-0000b620: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000b630: 656c 662e 6461 7461 6261 7365 2069 7320  elf.database is 
-0000b640: 6e6f 7420 4e6f 6e65 2061 6e64 206c 656e  not None and len
-0000b650: 2873 656c 662e 6461 7461 6261 7365 2920  (self.database) 
-0000b660: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
-0000b670: 2020 2020 2020 7365 6c66 2e64 6174 6162        self.datab
-0000b680: 6173 6520 3d20 4e6f 6e65 0a20 2020 2020  ase = None.     
-0000b690: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
-0000b6a0: 6174 6162 6173 6520 6973 206e 6f74 204e  atabase is not N
-0000b6b0: 6f6e 6520 616e 6420 7365 6c66 2e64 6174  one and self.dat
-0000b6c0: 6162 6173 655b 305d 203d 3d20 222f 223a  abase[0] == "/":
-0000b6d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b6e0: 2073 656c 662e 6461 7461 6261 7365 203d   self.database =
-0000b6f0: 2073 656c 662e 6461 7461 6261 7365 5b31   self.database[1
-0000b700: 3a5d 0a0a 2020 2020 2020 2020 2020 2020  :]..            
-0000b710: 6966 2022 746c 7322 2069 6e20 7061 7273  if "tls" in pars
-0000b720: 6564 2e71 7565 7279 3a0a 2020 2020 2020  ed.query:.      
-0000b730: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-0000b740: 6c73 203d 2070 6172 7365 642e 7175 6572  ls = parsed.quer
-0000b750: 795b 2274 6c73 225d 0a0a 2020 2020 2020  y["tls"]..      
-0000b760: 2020 2020 2020 6966 2022 666f 7263 6522        if "force"
-0000b770: 2069 6e20 7061 7273 6564 2e71 7565 7279   in parsed.query
-0000b780: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b790: 2020 7368 6f75 6c64 466f 7263 6520 3d20    shouldForce = 
-0000b7a0: 7061 7273 6564 2e71 7565 7279 5b22 666f  parsed.query["fo
-0000b7b0: 7263 6522 5d0a 2020 2020 2020 2020 2020  rce"].          
-0000b7c0: 2020 2020 2020 6966 2073 686f 756c 6446        if shouldF
-0000b7d0: 6f72 6365 2e75 7070 6572 2829 203d 3d20  orce.upper() == 
-0000b7e0: 2254 5255 4522 3a0a 2020 2020 2020 2020  "TRUE":.        
-0000b7f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b800: 2e66 6f72 6365 203d 2054 7275 650a 2020  .force = True.  
-0000b810: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0000b820: 6966 2073 686f 756c 6446 6f72 6365 2e75  if shouldForce.u
-0000b830: 7070 6572 2829 203d 3d20 2246 414c 5345  pper() == "FALSE
-0000b840: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-0000b850: 2020 2020 2020 2073 656c 662e 666f 7263         self.forc
-0000b860: 6520 3d20 4661 6c73 650a 2020 2020 2020  e = False.      
-0000b870: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0000b880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b890: 2020 2020 7261 6973 6520 4d61 6c66 6f72      raise Malfor
-0000b8a0: 6d65 6455 524c 2866 2249 6e76 616c 6964  medURL(f"Invalid
-0000b8b0: 2066 6f72 6365 2073 7472 696e 673a 207b   force string: {
-0000b8c0: 7368 6f75 6c64 466f 7263 657d 2229 0a0a  shouldForce}")..
-0000b8d0: 2020 2020 2020 2020 2020 2020 6966 2066              if f
-0000b8e0: 6f72 6365 2069 7320 6e6f 7420 4e6f 6e65  orce is not None
-0000b8f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b900: 2020 7365 6c66 2e66 6f72 6365 203d 2066    self.force = f
-0000b910: 6f72 6365 0a0a 2020 2020 2020 2020 2020  orce..          
-0000b920: 2020 6966 2022 6861 6e64 7368 616b 6522    if "handshake"
-0000b930: 2069 6e20 7061 7273 6564 2e71 7565 7279   in parsed.query
-0000b940: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b950: 2020 6861 6e64 7368 616b 6520 3d20 7061    handshake = pa
-0000b960: 7273 6564 2e71 7565 7279 5b22 6861 6e64  rsed.query["hand
-0000b970: 7368 616b 6522 5d2e 6c6f 7765 7228 290a  shake"].lower().
-0000b980: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000b990: 7365 6c66 2e75 7365 7220 6973 204e 6f6e  self.user is Non
-0000b9a0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000b9b0: 2020 2073 656c 662e 7573 6572 203d 2022     self.user = "
-0000b9c0: 220a 0a20 2020 2020 2020 2020 2020 2069  "..            i
-0000b9d0: 6620 7365 6c66 2e70 6173 7377 6f72 6420  f self.password 
-0000b9e0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0000b9f0: 2020 2020 2020 2020 2073 656c 662e 7061           self.pa
-0000ba00: 7373 776f 7264 203d 2022 220a 0a20 2020  ssword = ""..   
-0000ba10: 2020 2020 2023 204e 6f77 206f 7665 7272       # Now overr
-0000ba20: 6964 6520 7468 6520 4453 4e20 7661 6c75  ide the DSN valu
-0000ba30: 6573 2077 6974 6820 616e 7920 7661 6c75  es with any valu
-0000ba40: 6573 2070 6173 7365 6420 696e 2061 7320  es passed in as 
-0000ba50: 7061 7261 6d65 7465 7273 0a20 2020 2020  parameters.     
-0000ba60: 2020 2069 6620 7573 6572 2069 7320 6e6f     if user is no
-0000ba70: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000ba80: 2020 2020 7365 6c66 2e75 7365 7220 3d20      self.user = 
-0000ba90: 7573 6572 0a0a 2020 2020 2020 2020 6966  user..        if
-0000baa0: 2070 6173 7377 6f72 6420 6973 206e 6f74   password is not
-0000bab0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000bac0: 2020 2073 656c 662e 7061 7373 776f 7264     self.password
-0000bad0: 203d 2070 6173 7377 6f72 640a 0a20 2020   = password..   
-0000bae0: 2020 2020 2069 6620 686f 7374 3a0a 2020       if host:.  
-0000baf0: 2020 2020 2020 2020 2020 2320 4861 6e64            # Hand
-0000bb00: 6c65 2068 6f73 743a 706f 7274 0a20 2020  le host:port.   
-0000bb10: 2020 2020 2020 2020 2070 6172 7473 203d           parts =
-0000bb20: 2068 6f73 742e 7370 6c69 7428 223a 2229   host.split(":")
-0000bb30: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000bb40: 6c65 6e28 7061 7274 7329 203d 3d20 313a  len(parts) == 1:
-0000bb50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bb60: 2073 656c 662e 686f 7374 7320 3d20 7061   self.hosts = pa
-0000bb70: 7274 735b 305d 2e73 706c 6974 2822 2c22  rts[0].split(","
-0000bb80: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-0000bb90: 6966 206c 656e 2870 6172 7473 2920 3d3d  if len(parts) ==
-0000bba0: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
-0000bbb0: 2020 2020 7365 6c66 2e68 6f73 7473 203d      self.hosts =
-0000bbc0: 2070 6172 7473 5b30 5d2e 7370 6c69 7428   parts[0].split(
-0000bbd0: 222c 2229 0a20 2020 2020 2020 2020 2020  ",").           
-0000bbe0: 2020 2020 2073 656c 662e 706f 7274 203d       self.port =
-0000bbf0: 2069 6e74 2870 6172 7473 5b31 5d29 0a20   int(parts[1]). 
-0000bc00: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000bc10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bc20: 2072 6169 7365 204d 616c 666f 726d 6564   raise Malformed
-0000bc30: 5552 4c28 6622 496e 7661 6c69 6420 686f  URL(f"Invalid ho
-0000bc40: 7374 2076 616c 7565 3a20 7b68 6f73 747d  st value: {host}
-0000bc50: 2229 0a0a 2020 2020 2020 2020 6966 2064  ")..        if d
-0000bc60: 6174 6162 6173 653a 0a20 2020 2020 2020  atabase:.       
-0000bc70: 2020 2020 2073 656c 662e 6461 7461 6261       self.databa
-0000bc80: 7365 203d 2064 6174 6162 6173 650a 0a20  se = database.. 
-0000bc90: 2020 2020 2020 2069 6620 746c 7320 6973         if tls is
-0000bca0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000bcb0: 2020 2020 2020 2073 656c 662e 746c 7320         self.tls 
-0000bcc0: 3d20 746c 730a 0a20 2020 2020 2020 2069  = tls..        i
-0000bcd0: 6620 6861 6e64 7368 616b 6520 6973 206e  f handshake is n
-0000bce0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000bcf0: 2020 2020 2073 656c 662e 6861 6e64 7368       self.handsh
-0000bd00: 616b 6520 3d20 6861 6e64 7368 616b 650a  ake = handshake.
-0000bd10: 0a20 2020 2020 2020 2023 2053 6574 2074  .        # Set t
-0000bd20: 6865 2064 6566 6175 6c74 2068 6f73 7420  he default host 
-0000bd30: 6e6f 772c 2073 696e 6365 2077 6520 7573  now, since we us
-0000bd40: 6520 7468 6174 2061 7320 6120 6b65 7920  e that as a key 
-0000bd50: 696e 746f 2074 6865 0a20 2020 2020 2020  into the.       
-0000bd60: 2023 2063 6f6e 6669 6720 6669 6c65 0a20   # config file. 
-0000bd70: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
-0000bd80: 6f73 7473 2069 7320 4e6f 6e65 3a0a 2020  osts is None:.  
-0000bd90: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
-0000bda0: 6f73 7473 203d 205b 7365 6c66 2e44 4546  osts = [self.DEF
-0000bdb0: 4155 4c54 5f48 4f53 545d 0a0a 2020 2020  AULT_HOST]..    
-0000bdc0: 2020 2020 2320 4e6f 7720 6275 696c 6420      # Now build 
-0000bdd0: 6120 636f 6e66 6967 7061 7273 6572 2077  a configparser w
-0000bde0: 6974 6820 6465 6661 756c 7420 7661 6c75  ith default valu
-0000bdf0: 6573 0a20 2020 2020 2020 2063 6f6e 6669  es.        confi
-0000be00: 6720 3d20 636f 6e66 6967 7061 7273 6572  g = configparser
-0000be10: 2e43 6f6e 6669 6750 6172 7365 7228 0a20  .ConfigParser(. 
-0000be20: 2020 2020 2020 2020 2020 2064 6566 6175             defau
-0000be30: 6c74 733d 7b22 706f 7274 223a 2073 7472  lts={"port": str
-0000be40: 2873 656c 662e 4445 4641 554c 545f 504f  (self.DEFAULT_PO
-0000be50: 5254 292c 2022 6461 7461 6261 7365 223a  RT), "database":
-0000be60: 2073 656c 662e 4445 4641 554c 545f 4441   self.DEFAULT_DA
-0000be70: 5441 4241 5345 2c20 2274 6c73 223a 2022  TABASE, "tls": "
-0000be80: 756e 7665 7269 6669 6564 222c 2022 666f  unverified", "fo
-0000be90: 7263 6522 3a20 2266 616c 7365 222c 2022  rce": "false", "
-0000bea0: 6861 6e64 7368 616b 6522 3a20 2222 7d2c  handshake": ""},
-0000beb0: 2069 6e74 6572 706f 6c61 7469 6f6e 3d4e   interpolation=N
-0000bec0: 6f6e 650a 2020 2020 2020 2020 290a 2020  one.        ).  
-0000bed0: 2020 2020 2020 636f 6e66 6967 7661 6c73        configvals
-0000bee0: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
-0000bef0: 2023 2049 6620 7765 2068 6176 6520 6120   # If we have a 
-0000bf00: 636f 6e66 6967 2066 696c 6520 7472 7920  config file try 
-0000bf10: 6c6f 6164 696e 6720 7468 6174 0a20 2020  loading that.   
-0000bf20: 2020 2020 2069 6620 636f 6e66 6967 6669       if configfi
-0000bf30: 6c65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  le is not None:.
-0000bf40: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-0000bf50: 6669 672e 7265 6164 2863 6f6e 6669 6766  fig.read(configf
-0000bf60: 696c 6529 0a0a 2020 2020 2020 2020 2020  ile)..          
-0000bf70: 2020 2320 576f 726b 206f 7574 2074 6865    # Work out the
-0000bf80: 2068 6f73 742f 6461 7461 6261 7365 2069   host/database i
-0000bf90: 6620 7765 206b 6e6f 7720 6974 0a20 2020  f we know it.   
-0000bfa0: 2020 2020 2020 2020 2068 6f73 745f 6462           host_db
-0000bfb0: 203d 2022 2c22 2e6a 6f69 6e28 7365 6c66   = ",".join(self
-0000bfc0: 2e68 6f73 7473 290a 2020 2020 2020 2020  .hosts).        
-0000bfd0: 2020 2020 6966 2073 656c 662e 6461 7461      if self.data
-0000bfe0: 6261 7365 2069 7320 6e6f 7420 4e6f 6e65  base is not None
-0000bff0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000c000: 2020 686f 7374 5f64 6220 3d20 686f 7374    host_db = host
-0000c010: 5f64 6220 2b20 222f 2220 2b20 7365 6c66  _db + "/" + self
-0000c020: 2e64 6174 6162 6173 650a 0a20 2020 2020  .database..     
-0000c030: 2020 2020 2020 2023 2054 7279 2061 6e64         # Try and
-0000c040: 206d 6174 6368 2065 6163 6820 7365 6374   match each sect
-0000c050: 696f 6e20 696e 2074 6865 2049 4e49 2066  ion in the INI f
-0000c060: 696c 6520 7769 7468 2074 6865 2068 6f73  ile with the hos
-0000c070: 742f 6461 7461 6261 7365 0a20 2020 2020  t/database.     
-0000c080: 2020 2020 2020 2066 6f72 2073 2069 6e20         for s in 
-0000c090: 636f 6e66 6967 2e73 6563 7469 6f6e 7328  config.sections(
-0000c0a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000c0b0: 2020 2069 6620 7265 2e6d 6174 6368 2873     if re.match(s
-0000c0c0: 2c20 686f 7374 5f64 6229 3a0a 2020 2020  , host_db):.    
-0000c0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0e0: 636f 6e66 6967 7661 6c73 203d 2063 6f6e  configvals = con
-0000c0f0: 6669 675b 735d 0a20 2020 2020 2020 2020  fig[s].         
-0000c100: 2020 2020 2020 2020 2020 2062 7265 616b             break
-0000c110: 0a0a 2020 2020 2020 2020 2320 6966 2077  ..        # if w
-0000c120: 6520 6469 646e 2774 2066 696e 6420 6120  e didn't find a 
-0000c130: 6d61 7463 6869 6e67 2068 6f73 7420 286f  matching host (o
-0000c140: 7220 7468 6572 6520 6973 206e 6f20 6669  r there is no fi
-0000c150: 6c65 292e 2075 7365 2074 6865 2064 6566  le). use the def
-0000c160: 6175 6c74 730a 2020 2020 2020 2020 6966  aults.        if
-0000c170: 2063 6f6e 6669 6776 616c 7320 6973 204e   configvals is N
-0000c180: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000c190: 2063 6f6e 6669 6776 616c 7320 3d20 636f   configvals = co
-0000c1a0: 6e66 6967 5b22 4445 4641 554c 5422 5d0a  nfig["DEFAULT"].
-0000c1b0: 2020 2020 2020 2020 2320 466f 7263 6520          # Force 
-0000c1c0: 6973 206e 6f74 2070 6c61 6365 7320 6865  is not places he
-0000c1d0: 7265 2073 6f20 6974 2063 616e 2067 6574  re so it can get
-0000c1e0: 2070 6172 7365 6420 6265 6c6f 772e 0a20   parsed below.. 
-0000c1f0: 2020 2020 2020 2066 6f72 2061 7474 7220         for attr 
-0000c200: 696e 205b 2270 6f72 7422 2c20 2264 6174  in ["port", "dat
-0000c210: 6162 6173 6522 2c20 2274 6c73 222c 2022  abase", "tls", "
-0000c220: 6861 6e64 7368 616b 6522 5d3a 0a20 2020  handshake"]:.   
-0000c230: 2020 2020 2020 2020 2069 6620 6765 7461           if geta
-0000c240: 7474 7228 7365 6c66 2c20 6174 7472 2920  ttr(self, attr) 
-0000c250: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0000c260: 2020 2020 2020 2020 2073 6574 6174 7472           setattr
-0000c270: 2873 656c 662c 2061 7474 722c 2063 6f6e  (self, attr, con
-0000c280: 6669 6776 616c 735b 6174 7472 5d29 0a0a  figvals[attr])..
-0000c290: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-0000c2a0: 656c 662e 7573 6572 3a0a 2020 2020 2020  elf.user:.      
-0000c2b0: 2020 2020 2020 7365 6c66 2e75 7365 7220        self.user 
-0000c2c0: 3d20 636f 6e66 6967 7661 6c73 2e67 6574  = configvals.get
-0000c2d0: 2822 7573 6572 222c 2022 2229 0a0a 2020  ("user", "")..  
-0000c2e0: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-0000c2f0: 662e 7061 7373 776f 7264 3a0a 2020 2020  f.password:.    
-0000c300: 2020 2020 2020 2020 7365 6c66 2e70 6173          self.pas
-0000c310: 7377 6f72 6420 3d20 636f 6e66 6967 7661  sword = configva
-0000c320: 6c73 2e67 6574 2822 7061 7373 776f 7264  ls.get("password
-0000c330: 222c 2022 2229 0a0a 2020 2020 2020 2020  ", "")..        
-0000c340: 6966 2073 656c 662e 666f 7263 6520 6973  if self.force is
-0000c350: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000c360: 2020 2073 656c 662e 666f 7263 6520 3d20     self.force = 
-0000c370: 636f 6e66 6967 7661 6c73 2e67 6574 626f  configvals.getbo
-0000c380: 6f6c 6561 6e28 2266 6f72 6365 2229 0a0a  olean("force")..
-0000c390: 2020 2020 2020 2020 2320 416e 6420 6669          # And fi
-0000c3a0: 6e61 6c6c 7920 7469 6479 2075 7020 736f  nally tidy up so
-0000c3b0: 6d65 2074 6869 6e67 730a 2020 2020 2020  me things.      
-0000c3c0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-0000c3d0: 7365 6c66 2e70 6f72 742c 2073 7472 293a  self.port, str):
-0000c3e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000c3f0: 662e 706f 7274 203d 2069 6e74 2873 656c  f.port = int(sel
-0000c400: 662e 706f 7274 290a 0a20 2020 2020 2020  f.port)..       
-0000c410: 2069 6620 6973 696e 7374 616e 6365 2873   if isinstance(s
-0000c420: 656c 662e 746c 732c 2073 7472 293a 0a20  elf.tls, str):. 
-0000c430: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000c440: 6c66 2e74 6c73 2e6c 6f77 6572 2829 203d  lf.tls.lower() =
-0000c450: 3d20 226f 6666 223a 0a20 2020 2020 2020  = "off":.       
-0000c460: 2020 2020 2020 2020 2073 656c 662e 746c           self.tl
-0000c470: 7320 3d20 7365 6c66 2e54 4c53 5f4e 4f4e  s = self.TLS_NON
-0000c480: 450a 2020 2020 2020 2020 2020 2020 656c  E.            el
-0000c490: 6966 2073 656c 662e 746c 732e 6c6f 7765  if self.tls.lowe
-0000c4a0: 7228 2920 3d3d 2022 756e 7665 7269 6669  r() == "unverifi
-0000c4b0: 6564 223a 0a20 2020 2020 2020 2020 2020  ed":.           
-0000c4c0: 2020 2020 2073 656c 662e 746c 7320 3d20       self.tls = 
-0000c4d0: 7365 6c66 2e54 4c53 5f55 4e56 4552 4946  self.TLS_UNVERIF
-0000c4e0: 4945 440a 2020 2020 2020 2020 2020 2020  IED.            
-0000c4f0: 656c 6966 2073 656c 662e 746c 732e 6c6f  elif self.tls.lo
-0000c500: 7765 7228 2920 3d3d 2022 6f6e 223a 0a20  wer() == "on":. 
-0000c510: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000c520: 656c 662e 746c 7320 3d20 7365 6c66 2e54  elf.tls = self.T
-0000c530: 4c53 5f4f 4e0a 2020 2020 2020 2020 2020  LS_ON.          
-0000c540: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000c550: 2020 2020 2020 2020 7261 6973 6520 4d61          raise Ma
-0000c560: 6c66 6f72 6d65 6455 524c 2866 2249 6e76  lformedURL(f"Inv
-0000c570: 616c 6964 2074 6c73 2076 616c 7565 3a20  alid tls value: 
-0000c580: 7b73 656c 662e 746c 737d 2229 0a20 2020  {self.tls}").   
-0000c590: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
-0000c5a0: 616e 6365 2873 656c 662e 746c 732c 206c  ance(self.tls, l
-0000c5b0: 6973 7429 3a0a 2020 2020 2020 2020 2020  ist):.          
-0000c5c0: 2020 7261 6973 6520 4d61 6c66 6f72 6d65    raise Malforme
-0000c5d0: 6455 524c 2866 224d 756c 7469 706c 6520  dURL(f"Multiple 
-0000c5e0: 544c 5320 7661 6c75 6573 2064 6574 6563  TLS values detec
-0000c5f0: 7465 643a 207b 7365 6c66 2e74 6c73 7d22  ted: {self.tls}"
-0000c600: 290a 0a20 2020 2020 2020 2069 6620 6973  )..        if is
-0000c610: 696e 7374 616e 6365 2873 656c 662e 6861  instance(self.ha
-0000c620: 6e64 7368 616b 652c 2073 7472 293a 0a20  ndshake, str):. 
-0000c630: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000c640: 6c66 2e68 616e 6473 6861 6b65 2e6c 6f77  lf.handshake.low
-0000c650: 6572 2829 203d 3d20 2263 6263 223a 0a20  er() == "cbc":. 
-0000c660: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000c670: 656c 662e 6861 6e64 7368 616b 6520 3d20  elf.handshake = 
-0000c680: 7365 6c66 2e48 414e 4453 4841 4b45 5f43  self.HANDSHAKE_C
-0000c690: 4243 0a20 2020 2020 2020 2020 2020 2065  BC.            e
-0000c6a0: 6c69 6620 7365 6c66 2e68 616e 6473 6861  lif self.handsha
-0000c6b0: 6b65 2e6c 6f77 6572 2829 203d 3d20 2273  ke.lower() == "s
-0000c6c0: 736f 223a 0a20 2020 2020 2020 2020 2020  so":.           
-0000c6d0: 2020 2020 2073 656c 662e 6861 6e64 7368       self.handsh
-0000c6e0: 616b 6520 3d20 7365 6c66 2e48 414e 4453  ake = self.HANDS
-0000c6f0: 4841 4b45 5f53 534f 0a20 2020 2020 2020  HAKE_SSO.       
-0000c700: 2020 2020 2023 2049 6620 7468 6579 2064       # If they d
-0000c710: 6964 6e27 7420 7370 6563 6966 7920 6861  idn't specify ha
-0000c720: 6e64 7368 616b 652c 2069 7420 7769 6c6c  ndshake, it will
-0000c730: 2062 6520 626c 616e 6b20 616e 6420 7468   be blank and th
-0000c740: 7573 2073 686f 756c 6420 6265 2047 434d  us should be GCM
-0000c750: 2e0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-0000c760: 6966 2073 656c 662e 6861 6e64 7368 616b  if self.handshak
-0000c770: 652e 6c6f 7765 7228 2920 3d3d 2022 6763  e.lower() == "gc
-0000c780: 6d22 206f 7220 7365 6c66 2e68 616e 6473  m" or self.hands
-0000c790: 6861 6b65 2e6c 6f77 6572 2829 203d 3d20  hake.lower() == 
-0000c7a0: 2222 3a0a 2020 2020 2020 2020 2020 2020  "":.            
-0000c7b0: 2020 2020 7365 6c66 2e68 616e 6473 6861      self.handsha
-0000c7c0: 6b65 203d 2073 656c 662e 4841 4e44 5348  ke = self.HANDSH
-0000c7d0: 414b 455f 4743 4d0a 2020 2020 2020 2020  AKE_GCM.        
-0000c7e0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000c7f0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-0000c800: 7365 6c66 2e68 616e 6473 6861 6b65 290a  self.handshake).
-0000c810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c820: 7261 6973 6520 4d61 6c66 6f72 6d65 6455  raise MalformedU
-0000c830: 524c 2866 2249 6e76 616c 6964 2068 616e  RL(f"Invalid han
-0000c840: 6473 6861 6b65 2076 616c 7565 3a20 7b73  dshake value: {s
-0000c850: 656c 662e 6861 6e64 7368 616b 657d 2229  elf.handshake}")
-0000c860: 0a0a 2020 2020 2020 2020 2320 446f 6e27  ..        # Don'
-0000c870: 7420 6173 7365 7274 2061 2075 7365 7220  t assert a user 
-0000c880: 7061 7261 6d65 7465 7220 6861 7320 6265  parameter has be
-0000c890: 656e 2073 6574 2e20 416e 2065 6d70 7479  en set. An empty
-0000c8a0: 0a20 2020 2020 2020 2023 2073 7472 696e  .        # strin
-0000c8b0: 6720 666f 7220 7468 6973 2066 6965 6c64  g for this field
-0000c8c0: 2069 7320 7573 6564 2066 6f72 2061 7574   is used for aut
-0000c8d0: 6865 6e74 6963 6174 696e 6720 5353 4f20  henticating SSO 
-0000c8e0: 7573 6572 730a 0a20 2020 2020 2020 2023  users..        #
-0000c8f0: 2044 6f6e 2774 2061 7373 6572 7420 6120   Don't assert a 
-0000c900: 7061 7373 776f 7264 2070 6172 616d 6574  password paramet
-0000c910: 6572 2068 6173 2062 6565 6e20 7365 742e  er has been set.
-0000c920: 2041 7420 656d 7074 790a 2020 2020 2020   At empty.      
-0000c930: 2020 2320 7573 6572 2061 6e64 2070 6173    # user and pas
-0000c940: 7377 6f72 6420 6973 2066 6f72 2061 7574  sword is for aut
-0000c950: 6865 6e74 6963 6174 696f 6e20 666c 6f77  hentication flow
-0000c960: 2077 6974 6820 5353 4f2e 0a0a 2020 2020   with SSO...    
-0000c970: 6465 6620 636c 6f73 6528 7365 6c66 293a  def close(self):
-0000c980: 0a20 2020 2020 2020 2022 2222 436c 6f73  .        """Clos
-0000c990: 6520 7468 6520 636f 6e6e 6563 7469 6f6e  e the connection
-0000c9a0: 2e20 5375 6273 6571 7565 6e74 2071 7565  . Subsequent que
-0000c9b0: 7269 6573 206f 6e20 7468 6973 2063 6f6e  ries on this con
-0000c9c0: 6e65 6374 696f 6e0a 2020 2020 2020 2020  nection.        
-0000c9d0: 7769 6c6c 2066 6169 6c0a 2020 2020 2020  will fail.      
-0000c9e0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-0000c9f0: 206e 6f74 2073 656c 662e 736f 636b 3a0a   not self.sock:.
-0000ca00: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000ca10: 6520 4572 726f 7228 224e 6f20 636f 6e6e  e Error("No conn
-0000ca20: 6563 7469 6f6e 2229 0a0a 2020 2020 2020  ection")..      
-0000ca30: 2020 6c6f 6767 6572 2e64 6562 7567 2866    logger.debug(f
-0000ca40: 2243 6c6f 7369 6e67 2063 6f6e 6e65 6374  "Closing connect
-0000ca50: 696f 6e20 6f6e 2073 6f63 6b65 7420 7b73  ion on socket {s
-0000ca60: 656c 662e 736f 636b 7d22 290a 2020 2020  elf.sock}").    
-0000ca70: 2020 2020 2320 446f 2074 6869 7320 6c69      # Do this li
-0000ca80: 7474 6c65 2064 616e 6365 2073 6f20 7468  ttle dance so th
-0000ca90: 6174 2065 7665 6e20 6966 2074 6865 2063  at even if the c
-0000caa0: 6c6f 7365 2829 2063 616c 6c0a 2020 2020  lose() call.    
-0000cab0: 2020 2020 2320 626c 6f77 7320 7570 2c20      # blows up, 
-0000cac0: 7765 2068 6176 6520 616c 7265 6164 7920  we have already 
-0000cad0: 7365 7420 7365 6c66 2e73 6f63 6b20 746f  set self.sock to
-0000cae0: 204e 6f6e 650a 2020 2020 2020 2020 736f   None.        so
-0000caf0: 636b 203d 2073 656c 662e 736f 636b 0a20  ck = self.sock. 
-0000cb00: 2020 2020 2020 2073 656c 662e 736f 636b         self.sock
-0000cb10: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-0000cb20: 736f 636b 2e63 6c6f 7365 2829 0a0a 2020  sock.close()..  
-0000cb30: 2020 6465 6620 636f 6d6d 6974 2873 656c    def commit(sel
-0000cb40: 6629 3a0a 2020 2020 2020 2020 2222 2243  f):.        """C
-0000cb50: 6f6d 6d69 7420 6120 7472 616e 7361 6374  ommit a transact
-0000cb60: 696f 6e2e 2043 7572 7265 6e74 6c79 2069  ion. Currently i
-0000cb70: 676e 6f72 6564 2222 220a 0a20 2020 2064  gnored"""..    d
-0000cb80: 6566 2063 7572 736f 7228 7365 6c66 293a  ef cursor(self):
-0000cb90: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-0000cba0: 726e 2061 206e 6577 2063 7572 736f 7220  rn a new cursor 
-0000cbb0: 666f 7220 7468 6973 2063 6f6e 6e65 6374  for this connect
-0000cbc0: 696f 6e22 2222 0a20 2020 2020 2020 2069  ion""".        i
-0000cbd0: 6620 6e6f 7420 7365 6c66 2e73 6f63 6b3a  f not self.sock:
-0000cbe0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0000cbf0: 7365 2045 7272 6f72 2822 4e6f 2063 6f6e  se Error("No con
-0000cc00: 6e65 6374 696f 6e22 290a 2020 2020 2020  nection").      
-0000cc10: 2020 7265 7475 726e 2043 7572 736f 7228    return Cursor(
-0000cc20: 7365 6c66 290a 0a20 2020 2064 6566 205f  self)..    def _
-0000cc30: 5f64 656c 5f5f 2873 656c 6629 3a0a 2020  _del__(self):.  
-0000cc40: 2020 2020 2020 6966 2073 656c 662e 736f        if self.so
-0000cc50: 636b 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ck is not None:.
-0000cc60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000cc70: 2e63 6c6f 7365 2829 0a0a 2020 2020 6465  .close()..    de
-0000cc80: 6620 7265 736f 6c76 655f 6e65 775f 656e  f resolve_new_en
-0000cc90: 6470 6f69 6e74 2873 656c 662c 206e 6577  dpoint(self, new
-0000cca0: 5f68 6f73 742c 206e 6577 5f70 6f72 7429  _host, new_port)
-0000ccb0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000ccc0: 2020 2020 2020 4861 6e64 6c65 7320 6d61        Handles ma
-0000ccd0: 7070 696e 6720 746f 2061 2073 6563 6f6e  pping to a secon
-0000cce0: 6461 7279 2069 6e74 6572 6661 6365 2062  dary interface b
-0000ccf0: 6173 6564 206f 6e20 7468 6520 7365 636f  ased on the seco
-0000cd00: 6e64 6172 7920 696e 7465 7266 6163 6520  ndary interface 
-0000cd10: 6d61 7070 696e 6720 7361 7665 6420 6f6e  mapping saved on
-0000cd20: 2074 6869 7320 636f 6e6e 6563 7469 6f6e   this connection
-0000cd30: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-0000cd40: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
-0000cd50: 5f68 6f73 745b 7374 7269 6e67 5d3a 2074  _host[string]: t
-0000cd60: 6865 206e 6577 2068 6f73 7420 746f 2062  he new host to b
-0000cd70: 6520 7265 6d61 7070 6564 0a20 2020 2020  e remapped.     
-0000cd80: 2020 2020 2020 206e 6577 5f70 6f72 745b         new_port[
-0000cd90: 696e 745d 3a20 7468 6520 6e65 7720 706f  int]: the new po
-0000cda0: 7274 2074 6f20 6265 2072 656d 6170 7065  rt to be remappe
-0000cdb0: 640a 0a20 2020 2020 2020 2052 6574 7572  d..        Retur
-0000cdc0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-0000cdd0: 5b74 7570 6c65 2873 7472 696e 672c 2069  [tuple(string, i
-0000cde0: 6e74 295d 3a20 5468 6520 6163 7475 616c  nt)]: The actual
-0000cdf0: 2065 6e64 706f 696e 7420 746f 2063 6f6e   endpoint to con
-0000ce00: 6e65 6374 2074 6f20 696e 2074 6865 2066  nect to in the f
-0000ce10: 6f72 6d61 743a 2028 686f 7374 2c20 706f  ormat: (host, po
-0000ce20: 7274 292e 0a20 2020 2020 2020 2022 2222  rt)..        """
-0000ce30: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-0000ce40: 6465 6275 6728 6622 5265 736f 6c76 696e  debug(f"Resolvin
-0000ce50: 6720 6e65 7720 656e 6470 6f69 6e74 207b  g new endpoint {
-0000ce60: 6e65 775f 686f 7374 7d3a 7b6e 6577 5f70  new_host}:{new_p
-0000ce70: 6f72 747d 2077 6974 6820 7365 636f 6e64  ort} with second
-0000ce80: 6172 795f 696e 6465 7820 7b73 656c 662e  ary_index {self.
-0000ce90: 7365 636f 6e64 6172 795f 696e 6465 787d  secondary_index}
-0000cea0: 2061 6e64 2073 6563 6f6e 6461 7279 5f69   and secondary_i
-0000ceb0: 6e74 6572 6661 6365 207b 7365 6c66 2e73  nterface {self.s
-0000cec0: 6563 6f6e 6461 7279 5f69 6e74 6572 6661  econdary_interfa
-0000ced0: 6365 737d 2229 0a0a 2020 2020 2020 2020  ces}")..        
-0000cee0: 6e65 775f 656e 6470 6f69 6e74 203d 2028  new_endpoint = (
-0000cef0: 6e65 775f 686f 7374 2c20 6e65 775f 706f  new_host, new_po
-0000cf00: 7274 290a 2020 2020 2020 2020 656e 6470  rt).        endp
-0000cf10: 6f69 6e74 5f74 6f5f 636f 6e6e 6563 7420  oint_to_connect 
-0000cf20: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
-0000cf30: 6620 7365 6c66 2e73 6563 6f6e 6461 7279  f self.secondary
-0000cf40: 5f69 6e64 6578 2021 3d20 2d31 3a0a 2020  _index != -1:.  
-0000cf50: 2020 2020 2020 2020 2020 6f75 7465 725f            outer_
-0000cf60: 696e 6465 7820 3d20 300a 2020 2020 2020  index = 0.      
-0000cf70: 2020 2020 2020 666f 7220 6f75 7465 725f        for outer_
-0000cf80: 6c69 7374 2069 6e20 7365 6c66 2e73 6563  list in self.sec
-0000cf90: 6f6e 6461 7279 5f69 6e74 6572 6661 6365  ondary_interface
-0000cfa0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0000cfb0: 2020 2069 6620 6f75 7465 725f 6c69 7374     if outer_list
-0000cfc0: 5b30 5d20 3d3d 206e 6577 5f65 6e64 706f  [0] == new_endpo
-0000cfd0: 696e 743a 0a20 2020 2020 2020 2020 2020  int:.           
-0000cfe0: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
-0000cff0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-0000d000: 7574 6572 5f69 6e64 6578 202b 3d20 310a  uter_index += 1.
-0000d010: 2020 2020 2020 2020 2020 2020 6966 206f              if o
-0000d020: 7574 6572 5f69 6e64 6578 203c 206c 656e  uter_index < len
-0000d030: 2873 656c 662e 7365 636f 6e64 6172 795f  (self.secondary_
-0000d040: 696e 7465 7266 6163 6573 293a 0a20 2020  interfaces):.   
-0000d050: 2020 2020 2020 2020 2020 2020 2065 6e64               end
-0000d060: 706f 696e 745f 746f 5f63 6f6e 6e65 6374  point_to_connect
-0000d070: 203d 2073 656c 662e 7365 636f 6e64 6172   = self.secondar
-0000d080: 795f 696e 7465 7266 6163 6573 5b6f 7574  y_interfaces[out
-0000d090: 6572 5f69 6e64 6578 5d5b 7365 6c66 2e73  er_index][self.s
-0000d0a0: 6563 6f6e 6461 7279 5f69 6e64 6578 5d0a  econdary_index].
-0000d0b0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000d0c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000d0d0: 2020 656e 6470 6f69 6e74 5f74 6f5f 636f    endpoint_to_co
-0000d0e0: 6e6e 6563 7420 3d20 6e65 775f 656e 6470  nnect = new_endp
-0000d0f0: 6f69 6e74 0a0a 2020 2020 2020 2020 656c  oint..        el
-0000d100: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000d110: 656e 6470 6f69 6e74 5f74 6f5f 636f 6e6e  endpoint_to_conn
-0000d120: 6563 7420 3d20 6e65 775f 656e 6470 6f69  ect = new_endpoi
-0000d130: 6e74 0a0a 2020 2020 2020 2020 6c6f 6767  nt..        logg
-0000d140: 6572 2e64 6562 7567 2866 2252 6573 6f6c  er.debug(f"Resol
-0000d150: 7665 6420 6e65 7720 656e 6470 6f69 6e74  ved new endpoint
-0000d160: 207b 6e65 775f 686f 7374 7d3a 7b6e 6577   {new_host}:{new
-0000d170: 5f70 6f72 747d 2074 6f20 7b65 6e64 706f  _port} to {endpo
-0000d180: 696e 745f 746f 5f63 6f6e 6e65 6374 7d22  int_to_connect}"
-0000d190: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-0000d1a0: 6e20 656e 6470 6f69 6e74 5f74 6f5f 636f  n endpoint_to_co
-0000d1b0: 6e6e 6563 740a 0a20 2020 2064 6566 2072  nnect..    def r
-0000d1c0: 6564 6972 6563 7428 7365 6c66 2c20 6e65  edirect(self, ne
-0000d1d0: 775f 686f 7374 2c20 6e65 775f 706f 7274  w_host, new_port
-0000d1e0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-0000d1f0: 2020 2020 2020 2052 6564 6972 6563 7473         Redirects
-0000d200: 2074 6f20 7468 6520 7072 6f70 6572 2073   to the proper s
-0000d210: 6563 6f6e 6461 7279 2069 6e74 6572 6661  econdary interfa
-0000d220: 6365 2067 6976 656e 2061 206e 6577 2065  ce given a new e
-0000d230: 6e64 706f 696e 742e 0a0a 2020 2020 2020  ndpoint...      
-0000d240: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-0000d250: 2020 2020 6e65 775f 686f 7374 5b73 7472      new_host[str
-0000d260: 696e 675d 3a20 7468 6520 6e65 7720 686f  ing]: the new ho
-0000d270: 7374 2074 6f20 6265 2072 656d 6170 7065  st to be remappe
-0000d280: 640a 2020 2020 2020 2020 2020 2020 6e65  d.            ne
-0000d290: 775f 706f 7274 5b69 6e74 5d3a 2074 6865  w_port[int]: the
-0000d2a0: 206e 6577 2070 6f72 7420 746f 2062 6520   new port to be 
-0000d2b0: 7265 6d61 7070 6564 0a0a 2020 2020 2020  remapped..      
-0000d2c0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-0000d2d0: 2020 2020 2020 205b 436f 6e6e 6563 7469         [Connecti
-0000d2e0: 6f6e 5d3a 2041 206e 6577 2063 6f6e 6e65  on]: A new conne
-0000d2f0: 6374 696f 6e2e 0a20 2020 2020 2020 2022  ction..        "
-0000d300: 2222 0a20 2020 2020 2020 2072 656d 6170  "".        remap
-0000d310: 7065 645f 686f 7374 2c20 7265 6d61 7070  ped_host, remapp
-0000d320: 6564 5f70 6f72 7420 3d20 7365 6c66 2e72  ed_port = self.r
-0000d330: 6573 6f6c 7665 5f6e 6577 5f65 6e64 706f  esolve_new_endpo
-0000d340: 696e 7428 6e65 775f 686f 7374 2c20 6e65  int(new_host, ne
-0000d350: 775f 706f 7274 290a 2020 2020 2020 2020  w_port).        
-0000d360: 6e65 775f 656e 6470 6f69 6e74 203d 2066  new_endpoint = f
-0000d370: 227b 7265 6d61 7070 6564 5f68 6f73 747d  "{remapped_host}
-0000d380: 3a7b 7265 6d61 7070 6564 5f70 6f72 747d  :{remapped_port}
-0000d390: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
-0000d3a0: 2e64 6562 7567 2866 2252 6564 6972 6563  .debug(f"Redirec
-0000d3b0: 7469 6e67 2063 6f6e 6e65 6374 696f 6e20  ting connection 
-0000d3c0: 746f 207b 6e65 775f 686f 7374 7d3a 7b6e  to {new_host}:{n
-0000d3d0: 6577 5f70 6f72 747d 2c20 7768 6963 6820  ew_port}, which 
-0000d3e0: 6d61 7073 2074 6f20 7b72 656d 6170 7065  maps to {remappe
-0000d3f0: 645f 686f 7374 7d3a 7b72 656d 6170 7065  d_host}:{remappe
-0000d400: 645f 706f 7274 7d22 290a 0a20 2020 2020  d_port}")..     
-0000d410: 2020 2072 6574 7572 6e20 436f 6e6e 6563     return Connec
-0000d420: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
-0000d430: 2020 7573 6572 3d73 656c 662e 7573 6572    user=self.user
-0000d440: 2c20 7061 7373 776f 7264 3d73 656c 662e  , password=self.
-0000d450: 7061 7373 776f 7264 2c20 686f 7374 3d6e  password, host=n
-0000d460: 6577 5f65 6e64 706f 696e 742c 2064 6174  ew_endpoint, dat
-0000d470: 6162 6173 653d 7365 6c66 2e64 6174 6162  abase=self.datab
-0000d480: 6173 652c 2074 6c73 3d73 656c 662e 746c  ase, tls=self.tl
-0000d490: 732c 2068 616e 6473 6861 6b65 3d73 656c  s, handshake=sel
-0000d4a0: 662e 6861 6e64 7368 616b 652c 2066 6f72  f.handshake, for
-0000d4b0: 6365 3d73 656c 662e 666f 7263 652c 2073  ce=self.force, s
-0000d4c0: 6573 7369 6f6e 3d73 656c 662e 7365 7373  ession=self.sess
-0000d4d0: 696f 6e0a 2020 2020 2020 2020 290a 0a20  ion.        ).. 
-0000d4e0: 2020 2064 6566 2072 6566 7265 7368 2873     def refresh(s
-0000d4f0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000d500: 220a 2020 2020 2020 2020 5573 6564 2074  ".        Used t
-0000d510: 6f20 7265 6672 6573 6820 7468 6520 7365  o refresh the se
-0000d520: 7373 696f 6e20 6173 736f 6369 6174 6564  ssion associated
-0000d530: 2077 6974 6820 7468 6973 2063 6f6e 6e65   with this conne
-0000d540: 6374 696f 6e2e 2054 6865 2073 6572 7665  ction. The serve
-0000d550: 7220 7769 6c6c 0a20 2020 2020 2020 2072  r will.        r
-0000d560: 6574 7572 6e20 6120 6e65 7720 7365 7276  eturn a new serv
-0000d570: 6572 2073 6573 7369 6f6e 2069 6420 616e  er session id an
-0000d580: 6420 7365 6375 7269 7479 2074 6f6b 656e  d security token
-0000d590: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0000d5a0: 2020 2020 2020 7265 7120 3d20 7072 6f74        req = prot
-0000d5b0: 6f2e 5265 7175 6573 7428 290a 2020 2020  o.Request().    
-0000d5c0: 2020 2020 7265 712e 7479 7065 203d 2072      req.type = r
-0000d5d0: 6571 2e43 4c49 454e 545f 434f 4e4e 4543  eq.CLIENT_CONNEC
-0000d5e0: 5449 4f4e 5f52 4546 5245 5348 5f53 4553  TION_REFRESH_SES
-0000d5f0: 5349 4f4e 0a20 2020 2020 2020 2063 6c69  SION.        cli
-0000d600: 656e 745f 636f 6e6e 6563 7469 6f6e 203d  ent_connection =
-0000d610: 2072 6571 2e63 6c69 656e 745f 636f 6e6e   req.client_conn
-0000d620: 6563 7469 6f6e 5f72 6566 7265 7368 5f73  ection_refresh_s
-0000d630: 6573 7369 6f6e 0a0a 2020 2020 2020 2020  ession..        
-0000d640: 2320 5365 6e64 206d 6573 7361 6765 0a20  # Send message. 
-0000d650: 2020 2020 2020 205f 7365 6e64 5f6d 7367         _send_msg
-0000d660: 2873 656c 662c 2072 6571 290a 2020 2020  (self, req).    
-0000d670: 2020 2020 2320 5265 6365 6976 6520 6d65      # Receive me
-0000d680: 7373 6167 650a 2020 2020 2020 2020 7273  ssage.        rs
-0000d690: 7020 3d20 5f72 6563 765f 6d73 6728 7365  p = _recv_msg(se
-0000d6a0: 6c66 2c20 7072 6f74 6f2e 436c 6965 6e74  lf, proto.Client
-0000d6b0: 436f 6e6e 6563 7469 6f6e 5265 6672 6573  ConnectionRefres
-0000d6c0: 6853 6573 7369 6f6e 5265 7370 6f6e 7365  hSessionResponse
-0000d6d0: 2829 290a 0a20 2020 2020 2020 2069 6620  ())..        if 
-0000d6e0: 7273 702e 7265 7370 6f6e 7365 2e74 7970  rsp.response.typ
-0000d6f0: 6520 3d3d 2070 726f 746f 2e43 6f6e 6669  e == proto.Confi
-0000d700: 726d 6174 696f 6e52 6573 706f 6e73 652e  rmationResponse.
-0000d710: 5245 5350 4f4e 5345 5f57 4152 4e3a 0a20  RESPONSE_WARN:. 
-0000d720: 2020 2020 2020 2020 2020 2077 6172 6e28             warn(
-0000d730: 7273 702e 7265 7370 6f6e 7365 2e72 6561  rsp.response.rea
-0000d740: 736f 6e29 0a20 2020 2020 2020 2065 6c69  son).        eli
-0000d750: 6620 7273 702e 7265 7370 6f6e 7365 2e74  f rsp.response.t
-0000d760: 7970 6520 3d3d 2070 726f 746f 2e43 6f6e  ype == proto.Con
-0000d770: 6669 726d 6174 696f 6e52 6573 706f 6e73  firmationRespons
-0000d780: 652e 5245 5350 4f4e 5345 5f4f 4b3a 0a20  e.RESPONSE_OK:. 
-0000d790: 2020 2020 2020 2020 2020 2023 2043 6170             # Cap
-0000d7a0: 7475 7265 2074 6865 2073 6573 7369 6f6e  ture the session
-0000d7b0: 2069 640a 2020 2020 2020 2020 2020 2020   id.            
-0000d7c0: 7365 6c66 2e73 6572 7665 7253 6573 7369  self.serverSessi
-0000d7d0: 6f6e 4964 203d 2072 7370 2e73 6573 7369  onId = rsp.sessi
-0000d7e0: 6f6e 496e 666f 2e73 6572 7665 7253 6573  onInfo.serverSes
-0000d7f0: 7369 6f6e 4964 0a20 2020 2020 2020 2020  sionId.         
-0000d800: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0000d810: 6622 436f 6e6e 6563 7465 6420 746f 2073  f"Connected to s
-0000d820: 6572 7665 7220 7365 7373 696f 6e20 4964  erver session Id
-0000d830: 3a20 7b73 656c 662e 7365 7276 6572 5365  : {self.serverSe
-0000d840: 7373 696f 6e49 647d 2229 0a20 2020 2020  ssionId}").     
-0000d850: 2020 2020 2020 2072 6563 6569 7665 645f         received_
-0000d860: 746f 6b65 6e20 3d20 7273 702e 7365 7373  token = rsp.sess
-0000d870: 696f 6e49 6e66 6f2e 7365 6375 7269 7479  ionInfo.security
-0000d880: 546f 6b65 6e0a 2020 2020 2020 2020 2020  Token.          
-0000d890: 2020 6966 2073 656c 662e 7365 7373 696f    if self.sessio
-0000d8a0: 6e2e 7365 6375 7269 7479 546f 6b65 6e20  n.securityToken 
-0000d8b0: 213d 204e 6f6e 653a 0a20 2020 2020 2020  != None:.       
-0000d8c0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-0000d8d0: 7373 696f 6e20 3d20 5365 7373 696f 6e28  ssion = Session(
-0000d8e0: 7365 6375 7269 7479 546f 6b65 6e3d 5365  securityToken=Se
-0000d8f0: 6375 7269 7479 546f 6b65 6e28 7265 6365  curityToken(rece
-0000d900: 6976 6564 5f74 6f6b 656e 2e64 6174 612c  ived_token.data,
-0000d910: 2072 6563 6569 7665 645f 746f 6b65 6e2e   received_token.
-0000d920: 7369 676e 6174 7572 652c 2072 6563 6569  signature, recei
-0000d930: 7665 645f 746f 6b65 6e2e 6973 7375 6572  ved_token.issuer
-0000d940: 4669 6e67 6572 7072 696e 7429 290a 2020  Fingerprint)).  
-0000d950: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0000d960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d970: 2320 4967 6e6f 7265 2074 6865 2073 6563  # Ignore the sec
-0000d980: 7572 6974 7920 746f 6b65 6e0a 2020 2020  urity token.    
-0000d990: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d9a0: 2e73 6573 7369 6f6e 203d 2053 6573 7369  .session = Sessi
-0000d9b0: 6f6e 2875 7365 7241 6e64 5061 7373 776f  on(userAndPasswo
-0000d9c0: 7264 3d55 7365 7241 6e64 5061 7373 776f  rd=UserAndPasswo
-0000d9d0: 7264 2873 656c 662e 7573 6572 2c20 7365  rd(self.user, se
-0000d9e0: 6c66 2e70 6173 7377 6f72 6429 290a 2020  lf.password)).  
-0000d9f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000da00: 0a20 2020 2020 2020 2023 2053 6f6d 6574  .        # Somet
-0000da10: 6869 6e67 2062 6164 2068 6170 7065 6e65  hing bad happene
-0000da20: 6420 7769 7468 2074 6865 2072 6566 7265  d with the refre
-0000da30: 7368 2061 7474 656d 7074 2e0a 2020 2020  sh attempt..    
-0000da40: 2020 2020 7261 6973 6520 5f63 6f6e 7665      raise _conve
-0000da50: 7274 5f65 7863 6570 7469 6f6e 2872 7370  rt_exception(rsp
-0000da60: 2e72 6573 706f 6e73 6529 0a0a 0a63 6c61  .response)...cla
-0000da70: 7373 2043 7572 736f 723a 0a20 2020 2023  ss Cursor:.    #
-0000da80: 2070 796c 696e 743a 2064 6973 6162 6c65   pylint: disable
-0000da90: 3d74 6f6f 2d6d 616e 792d 696e 7374 616e  =too-many-instan
-0000daa0: 6365 2d61 7474 7269 6275 7465 730a 2020  ce-attributes.  
-0000dab0: 2020 2222 2241 2064 6174 6162 6173 6520    """A database 
-0000dac0: 6375 7273 6f72 2c20 7768 6963 6820 6973  cursor, which is
-0000dad0: 2075 7365 6420 746f 206d 616e 6167 6520   used to manage 
-0000dae0: 6120 7175 6572 7920 616e 6420 6974 7320  a query and its 
-0000daf0: 7265 7475 726e 6564 2072 6573 756c 7473  returned results
-0000db00: 2222 220a 0a20 2020 2064 6566 205f 5f69  """..    def __i
-0000db10: 6e69 745f 5f28 7365 6c66 2c20 636f 6e6e  nit__(self, conn
-0000db20: 293a 0a20 2020 2020 2020 2022 2222 4375  ):.        """Cu
-0000db30: 7273 6f72 7320 6172 6520 6e6f 726d 616c  rsors are normal
-0000db40: 6c79 2063 7265 6174 6564 2062 7920 7468  ly created by th
-0000db50: 6520 6375 7273 6f72 2829 2063 616c 6c20  e cursor() call 
-0000db60: 6f6e 2061 2063 6f6e 6e65 6374 696f 6e2c  on a connection,
-0000db70: 2062 7574 2063 616e 0a20 2020 2020 2020   but can.       
-0000db80: 2062 6520 6372 6561 7465 6420 6469 7265   be created dire
-0000db90: 6374 6c79 2062 7920 7072 6f76 6964 696e  ctly by providin
-0000dba0: 6720 6120 636f 6e6e 6563 7469 6f6e 0a20  g a connection. 
-0000dbb0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000dbc0: 2020 2073 656c 662e 636f 6e6e 6563 7469     self.connecti
-0000dbd0: 6f6e 203d 2063 6f6e 6e0a 2020 2020 2020  on = conn.      
-0000dbe0: 2020 7365 6c66 2e61 7272 6179 7369 7a65    self.arraysize
-0000dbf0: 203d 2031 0a0a 2020 2020 2020 2020 7365   = 1..        se
-0000dc00: 6c66 2e5f 7265 696e 6974 6961 6c69 7a65  lf._reinitialize
-0000dc10: 2829 0a0a 2020 2020 6465 6620 5f5f 6465  ()..    def __de
-0000dc20: 6c5f 5f28 7365 6c66 293a 0a20 2020 2020  l__(self):.     
-0000dc30: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-0000dc40: 2020 2020 7365 6c66 2e5f 636c 6f73 655f      self._close_
-0000dc50: 7265 7375 6c74 7365 7428 290a 2020 2020  resultset().    
-0000dc60: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
-0000dc70: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-0000dc80: 2020 6465 6620 5f72 6569 6e69 7469 616c    def _reinitial
-0000dc90: 697a 6528 7365 6c66 293a 0a20 2020 2020  ize(self):.     
-0000dca0: 2020 2022 2222 496e 7465 726e 616c 2066     """Internal f
-0000dcb0: 756e 6374 696f 6e20 746f 2069 6e69 7469  unction to initi
-0000dcc0: 616c 697a 6520 6120 6375 7273 6f72 2222  alize a cursor""
-0000dcd0: 220a 2020 2020 2020 2020 2320 5365 7420  ".        # Set 
-0000dce0: 7468 6520 7374 6174 650a 2020 2020 2020  the state.      
-0000dcf0: 2020 7365 6c66 2e71 7565 7279 5f69 6420    self.query_id 
-0000dd00: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
-0000dd10: 656c 662e 726f 7763 6f75 6e74 203d 202d  elf.rowcount = -
-0000dd20: 310a 2020 2020 2020 2020 7365 6c66 2e72  1.        self.r
-0000dd30: 6f77 6e75 6d62 6572 203d 204e 6f6e 650a  ownumber = None.
-0000dd40: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
-0000dd50: 756c 7473 6574 5f74 7570 6c65 203d 204e  ultset_tuple = N
-0000dd60: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
-0000dd70: 2e64 6573 6372 6970 7469 6f6e 203d 204e  .description = N
-0000dd80: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
-0000dd90: 2e65 6e64 5f6f 665f 6461 7461 203d 2046  .end_of_data = F
-0000dda0: 616c 7365 0a20 2020 2020 2020 2073 656c  alse.        sel
-0000ddb0: 662e 6578 706c 6169 6e5f 7265 7375 6c74  f.explain_result
-0000ddc0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-0000ddd0: 7365 6c66 2e6c 6973 745f 7265 7375 6c74  self.list_result
-0000dde0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-0000ddf0: 7365 6c66 2e5f 6275 6666 6572 7320 3d20  self._buffers = 
-0000de00: 5b5d 0a20 2020 2020 2020 2073 656c 662e  [].        self.
-0000de10: 5f6f 6666 7365 7420 3d20 300a 2020 2020  _offset = 0.    
-0000de20: 2020 2020 7365 6c66 2e5f 7065 6e64 696e      self._pendin
-0000de30: 675f 6f70 7320 3d20 5b5d 0a0a 2020 2020  g_ops = []..    
-0000de40: 6465 6620 7365 7469 6e70 7574 7369 7a65  def setinputsize
-0000de50: 7328 7365 6c66 2c20 7369 7a65 7329 3a0a  s(self, sizes):.
-0000de60: 2020 2020 2020 2020 2222 2254 6869 7320          """This 
-0000de70: 6361 6e20 6265 2075 7365 6420 6265 666f  can be used befo
-0000de80: 7265 2061 2063 616c 6c20 746f 202e 6578  re a call to .ex
-0000de90: 6563 7574 652a 2829 2074 6f20 7072 6564  ecute*() to pred
-0000dea0: 6566 696e 650a 2020 2020 2020 2020 6d65  efine.        me
-0000deb0: 6d6f 7279 2061 7265 6173 2066 6f72 2074  mory areas for t
-0000dec0: 6865 206f 7065 7261 7469 6f6e 2773 2070  he operation's p
-0000ded0: 6172 616d 6574 6572 732e 2043 7572 7265  arameters. Curre
-0000dee0: 6e74 6c79 2069 676e 6f72 6564 0a20 2020  ntly ignored.   
-0000def0: 2020 2020 2022 2222 0a0a 2020 2020 6465       """..    de
-0000df00: 6620 7365 746f 7574 7075 7473 697a 6528  f setoutputsize(
-0000df10: 7365 6c66 2c20 7369 7a65 2c20 636f 6c75  self, size, colu
-0000df20: 6d6e 3d4e 6f6e 6529 3a0a 2020 2020 2020  mn=None):.      
-0000df30: 2020 2222 2253 6574 2061 2063 6f6c 756d    """Set a colum
-0000df40: 6e20 6275 6666 6572 2073 697a 6520 666f  n buffer size fo
-0000df50: 7220 6665 7463 6865 7320 6f66 206c 6172  r fetches of lar
-0000df60: 6765 2063 6f6c 756d 6e73 0a20 2020 2020  ge columns.     
-0000df70: 2020 2028 652e 672e 204c 4f4e 4773 2c20     (e.g. LONGs, 
-0000df80: 424c 4f42 732c 2065 7463 2e29 2e20 5468  BLOBs, etc.). Th
-0000df90: 6520 636f 6c75 6d6e 2069 7320 7370 6563  e column is spec
-0000dfa0: 6966 6965 6420 6173 2061 6e0a 2020 2020  ified as an.    
-0000dfb0: 2020 2020 696e 6465 7820 696e 746f 2074      index into t
-0000dfc0: 6865 2072 6573 756c 7420 7365 7175 656e  he result sequen
-0000dfd0: 6365 2e20 4375 7272 656e 746c 7920 6967  ce. Currently ig
-0000dfe0: 6e6f 7265 640a 2020 2020 2020 2020 2222  nored.        ""
-0000dff0: 220a 0a20 2020 2064 6566 2063 6c6f 7365  "..    def close
-0000e000: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000e010: 2222 2243 6c6f 7365 2074 6869 7320 6375  """Close this cu
-0000e020: 7273 6f72 2e20 2054 6865 2063 7572 7265  rsor.  The curre
-0000e030: 6e74 2072 6573 756c 7420 7365 7420 6973  nt result set is
-0000e040: 2063 6c6f 7365 642c 2062 7574 0a20 2020   closed, but.   
-0000e050: 2020 2020 2074 6865 2063 7572 736f 7220       the cursor 
-0000e060: 6361 6e20 6265 2072 6575 7365 6420 666f  can be reused fo
-0000e070: 7220 7375 6273 6571 7565 6e74 2065 7865  r subsequent exe
-0000e080: 6375 7465 2829 2063 616c 6c73 2e0a 2020  cute() calls..  
-0000e090: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000e0a0: 2020 6966 2073 656c 662e 5f62 7566 6665    if self._buffe
-0000e0b0: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
-0000e0c0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-0000e0d0: 2020 2020 2073 656c 662e 5f63 6c6f 7365       self._close
-0000e0e0: 5f72 6573 756c 7473 6574 2829 0a20 2020  _resultset().   
-0000e0f0: 2020 2020 2020 2020 2065 7863 6570 743a           except:
-0000e100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e110: 2070 6173 730a 0a20 2020 2020 2020 2073   pass..        s
-0000e120: 656c 662e 5f72 6569 6e69 7469 616c 697a  elf._reinitializ
-0000e130: 6528 290a 0a20 2020 2064 6566 2065 7865  e()..    def exe
-0000e140: 6375 7465 6d61 6e79 2873 656c 662c 206f  cutemany(self, o
-0000e150: 7065 7261 7469 6f6e 2c20 7061 7261 6d65  peration, parame
-0000e160: 7465 726c 6973 7429 3a0a 2020 2020 2020  terlist):.      
-0000e170: 2020 2222 2250 7265 7061 7265 2061 2064    """Prepare a d
-0000e180: 6174 6162 6173 6520 6f70 6572 6174 696f  atabase operatio
-0000e190: 6e20 2871 7565 7279 206f 7220 636f 6d6d  n (query or comm
-0000e1a0: 616e 6429 2061 6e64 2074 6865 6e20 6578  and) and then ex
-0000e1b0: 6563 7574 6520 6974 2061 6761 696e 7374  ecute it against
-0000e1c0: 0a20 2020 2020 2020 2061 6c6c 2070 6172  .        all par
-0000e1d0: 616d 6574 6572 2073 6571 7565 6e63 6573  ameter sequences
-0000e1e0: 206f 7220 6d61 7070 696e 6773 2066 6f75   or mappings fou
-0000e1f0: 6e64 2069 6e20 7468 6520 7365 7175 656e  nd in the sequen
-0000e200: 6365 2070 6172 616d 6574 6572 6c69 7374  ce parameterlist
-0000e210: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-0000e220: 6574 6572 7320 6d61 7920 6265 2070 726f  eters may be pro
-0000e230: 7669 6465 6420 6173 2061 206d 6170 7069  vided as a mappi
-0000e240: 6e67 2061 6e64 2077 696c 6c20 6265 2062  ng and will be b
-0000e250: 6f75 6e64 2074 6f20 7661 7269 6162 6c65  ound to variable
-0000e260: 730a 2020 2020 2020 2020 696e 2074 6865  s.        in the
-0000e270: 206f 7065 7261 7469 6f6e 2e20 5661 7269   operation. Vari
-0000e280: 6162 6c65 7320 6172 6520 7370 6563 6966  ables are specif
-0000e290: 6965 6420 696e 2050 7974 686f 6e20 6578  ied in Python ex
-0000e2a0: 7465 6e64 6564 2066 6f72 6d61 7420 636f  tended format co
-0000e2b0: 6465 732c 0a20 2020 2020 2020 2065 2e67  des,.        e.g
-0000e2c0: 2e20 2e2e 2e57 4845 5245 206e 616d 653d  . ...WHERE name=
-0000e2d0: 2528 6e61 6d65 290a 2020 2020 2020 2020  %(name).        
-0000e2e0: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
-0000e2f0: 2e5f 7265 696e 6974 6961 6c69 7a65 2829  ._reinitialize()
-0000e300: 0a0a 2020 2020 2020 2020 2320 7765 2063  ..        # we c
-0000e310: 616e 2774 206a 7573 7420 6578 6563 7574  an't just execut
-0000e320: 6520 616c 6c20 7468 6520 7175 6572 6965  e all the querie
-0000e330: 7320 6174 206f 6e63 652e 2e2e 2e6f 6369  s at once....oci
-0000e340: 656e 7420 6f6e 6c79 2061 6c6c 6f77 730a  ent only allows.
-0000e350: 2020 2020 2020 2020 2320 6f6e 6520 7175          # one qu
-0000e360: 6572 7920 6174 2061 2074 696d 6520 6f6e  ery at a time on
-0000e370: 2061 2063 6f6e 6e65 6374 696f 6e2e 2020   a connection.  
-0000e380: 536f 2071 7565 7565 2075 7020 616c 6c20  So queue up all 
-0000e390: 7468 6520 7175 6572 6965 7320 616e 640a  the queries and.
-0000e3a0: 2020 2020 2020 2020 2320 7765 276c 6c20          # we'll 
-0000e3b0: 6361 6c6c 2074 6865 6d20 6c61 7465 720a  call them later.
-0000e3c0: 2020 2020 2020 2020 666f 7220 7061 7261          for para
-0000e3d0: 6d20 696e 2070 6172 616d 6574 6572 6c69  m in parameterli
-0000e3e0: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
-0000e3f0: 7365 6c66 2e5f 7065 6e64 696e 675f 6f70  self._pending_op
-0000e400: 732e 6170 7065 6e64 286f 7065 7261 7469  s.append(operati
-0000e410: 6f6e 2025 2070 6172 616d 290a 0a20 2020  on % param)..   
-0000e420: 2020 2020 2069 6620 7365 6c66 2e5f 7065       if self._pe
-0000e430: 6e64 696e 675f 6f70 733a 0a20 2020 2020  nding_ops:.     
-0000e440: 2020 2020 2020 2073 656c 662e 5f65 7865         self._exe
-0000e450: 6375 7465 5f69 6e74 6572 6e61 6c28 7365  cute_internal(se
-0000e460: 6c66 2e5f 7065 6e64 696e 675f 6f70 732e  lf._pending_ops.
-0000e470: 706f 7028 3029 290a 0a20 2020 2020 2020  pop(0))..       
-0000e480: 2072 6574 7572 6e20 7365 6c66 0a0a 2020   return self..  
-0000e490: 2020 6465 6620 6578 6563 7574 6528 7365    def execute(se
-0000e4a0: 6c66 2c20 6f70 6572 6174 696f 6e2c 2070  lf, operation, p
-0000e4b0: 6172 616d 6574 6572 733d 4e6f 6e65 293a  arameters=None):
-0000e4c0: 0a20 2020 2020 2020 2022 2222 5072 6570  .        """Prep
-0000e4d0: 6172 6520 616e 6420 6578 6563 7574 6520  are and execute 
-0000e4e0: 6120 6461 7461 6261 7365 206f 7065 7261  a database opera
-0000e4f0: 7469 6f6e 2028 7175 6572 7920 6f72 2063  tion (query or c
-0000e500: 6f6d 6d61 6e64 292e 0a0a 2020 2020 2020  ommand)...      
-0000e510: 2020 5061 7261 6d65 7465 7273 206d 6179    Parameters may
-0000e520: 2062 6520 7072 6f76 6964 6564 2061 7320   be provided as 
-0000e530: 6120 6d61 7070 696e 6720 616e 6420 7769  a mapping and wi
-0000e540: 6c6c 2062 6520 626f 756e 6420 746f 2076  ll be bound to v
-0000e550: 6172 6961 626c 6573 0a20 2020 2020 2020  ariables.       
-0000e560: 2069 6e20 7468 6520 6f70 6572 6174 696f   in the operatio
-0000e570: 6e2e 2056 6172 6961 626c 6573 2061 7265  n. Variables are
-0000e580: 2073 7065 6369 6669 6564 2069 6e20 5079   specified in Py
-0000e590: 7468 6f6e 2065 7874 656e 6465 6420 666f  thon extended fo
-0000e5a0: 726d 6174 2063 6f64 6573 2c0a 2020 2020  rmat codes,.    
-0000e5b0: 2020 2020 652e 672e 202e 2e2e 5748 4552      e.g. ...WHER
-0000e5c0: 4520 6e61 6d65 3d25 286e 616d 6529 0a20  E name=%(name). 
-0000e5d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000e5e0: 2020 2073 656c 662e 5f72 6569 6e69 7469     self._reiniti
-0000e5f0: 616c 697a 6528 290a 2020 2020 2020 2020  alize().        
-0000e600: 7365 6c66 2e5f 6578 6563 7574 655f 696e  self._execute_in
-0000e610: 7465 726e 616c 286f 7065 7261 7469 6f6e  ternal(operation
-0000e620: 2c20 7061 7261 6d65 7465 7273 290a 0a20  , parameters).. 
-0000e630: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000e640: 6c66 0a0a 2020 2020 6465 6620 5f65 7865  lf..    def _exe
-0000e650: 6375 7465 5f69 6e74 6572 6e61 6c28 7365  cute_internal(se
-0000e660: 6c66 2c20 6f70 6572 6174 696f 6e2c 2070  lf, operation, p
-0000e670: 6172 616d 6574 6572 733d 4e6f 6e65 293a  arameters=None):
-0000e680: 0a20 2020 2020 2020 2022 2222 496e 7465  .        """Inte
-0000e690: 726e 616c 2065 7865 6375 7465 2072 6f75  rnal execute rou
-0000e6a0: 7469 6e65 2074 6861 7420 6765 7473 2063  tine that gets c
-0000e6b0: 616c 6c65 6420 6672 6f6d 2065 7865 6375  alled from execu
-0000e6c0: 7465 2061 6e64 2065 7865 6375 7465 6d61  te and executema
-0000e6d0: 6e79 2222 220a 2020 2020 2020 2020 2320  ny""".        # 
-0000e6e0: 7079 6c69 6e74 3a20 6469 7361 626c 653d  pylint: disable=
-0000e6f0: 746f 6f2d 6d61 6e79 2d62 7261 6e63 6865  too-many-branche
-0000e700: 730a 0a20 2020 2020 2020 2069 6620 6861  s..        if ha
-0000e710: 7361 7474 7228 6f70 6572 6174 696f 6e2c  sattr(operation,
-0000e720: 2022 6465 636f 6465 2229 3a0a 2020 2020   "decode"):.    
-0000e730: 2020 2020 2020 2020 6f70 6572 6174 696f          operatio
-0000e740: 6e20 3d20 6f70 6572 6174 696f 6e2e 6465  n = operation.de
-0000e750: 636f 6465 2829 0a0a 2020 2020 2020 2020  code()..        
-0000e760: 6966 2070 6172 616d 6574 6572 7320 6973  if parameters is
-0000e770: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000e780: 2020 2020 2020 2069 6620 6861 7361 7474         if hasatt
-0000e790: 7228 6c69 7374 2870 6172 616d 6574 6572  r(list(parameter
-0000e7a0: 732e 6b65 7973 2829 295b 305d 2c20 2264  s.keys())[0], "d
-0000e7b0: 6563 6f64 6522 293a 0a20 2020 2020 2020  ecode"):.       
-0000e7c0: 2020 2020 2020 2020 2070 6172 616d 6574           paramet
-0000e7d0: 6572 7320 3d20 7b6b 6579 2e64 6563 6f64  ers = {key.decod
-0000e7e0: 6528 293a 2076 616c 7565 2066 6f72 2028  e(): value for (
-0000e7f0: 6b65 792c 2076 616c 7565 2920 696e 2070  key, value) in p
-0000e800: 6172 616d 6574 6572 732e 6974 656d 7328  arameters.items(
-0000e810: 297d 0a20 2020 2020 2020 2020 2020 206f  )}.            o
-0000e820: 7065 7261 7469 6f6e 203d 206f 7065 7261  peration = opera
-0000e830: 7469 6f6e 2025 2070 6172 616d 6574 6572  tion % parameter
-0000e840: 730a 0a20 2020 2020 2020 2023 2057 6520  s..        # We 
-0000e850: 6e65 6564 2074 6f20 6669 6775 7265 206f  need to figure o
-0000e860: 7574 2077 6865 7468 6572 2077 6520 7368  ut whether we sh
-0000e870: 6f75 6c64 2063 616c 6c0a 2020 2020 2020  ould call.      
-0000e880: 2020 2320 6578 6563 7574 655f 7175 6572    # execute_quer
-0000e890: 7920 6f72 2065 7865 6375 7465 5f75 7064  y or execute_upd
-0000e8a0: 6174 650a 2020 2020 2020 2020 7374 7269  ate.        stri
-0000e8b0: 7070 6564 203d 206f 7065 7261 7469 6f6e  pped = operation
-0000e8c0: 0a0a 2020 2020 2020 2020 2320 4c6f 6f70  ..        # Loop
-0000e8d0: 2075 6e74 696c 2077 6520 6861 7665 2073   until we have s
-0000e8e0: 6f6d 6520 7374 6172 7469 6e67 2077 6f72  ome starting wor
-0000e8f0: 6473 2e20 4e6f 7465 2074 6869 730a 2020  ds. Note this.  
-0000e900: 2020 2020 2020 2320 646f 6573 6e27 7420        # doesn't 
-0000e910: 6163 7475 616c 6c79 2068 616e 646c 6520  actually handle 
-0000e920: 7468 6520 6361 7365 206f 6620 2777 6f72  the case of 'wor
-0000e930: 6431 202f 2a20 636f 6d6d 656e 7420 2a2f  d1 /* comment */
-0000e940: 2077 6f72 6432 272c 0a20 2020 2020 2020   word2',.       
-0000e950: 2023 2062 7574 206e 6f6e 6520 6f66 2074   # but none of t
-0000e960: 6865 206f 7468 6572 2063 6c69 656e 7473  he other clients
-0000e970: 2064 6f20 6569 7468 6572 2e2e 2e0a 2020   do either....  
-0000e980: 2020 2020 2020 7768 696c 6520 5472 7565        while True
-0000e990: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-0000e9a0: 7374 7269 7020 6f66 6620 7374 6172 7469  strip off starti
-0000e9b0: 6e67 2073 7061 6365 730a 2020 2020 2020  ng spaces.      
-0000e9c0: 2020 2020 2020 7374 7269 7070 6564 203d        stripped =
-0000e9d0: 2073 7472 6970 7065 642e 6c73 7472 6970   stripped.lstrip
-0000e9e0: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
-0000e9f0: 2320 6966 2074 6869 7320 7374 6172 7473  # if this starts
-0000ea00: 2077 6974 6820 2d2d 2c20 7374 7269 7020   with --, strip 
-0000ea10: 7468 6520 7265 7374 206f 6620 7468 6520  the rest of the 
-0000ea20: 6c69 6e65 0a20 2020 2020 2020 2020 2020  line.           
-0000ea30: 2069 6620 7374 7269 7070 6564 2e73 7461   if stripped.sta
-0000ea40: 7274 7377 6974 6828 222d 2d22 293a 0a20  rtswith("--"):. 
-0000ea50: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000ea60: 6f73 203d 2073 7472 6970 7065 642e 6669  os = stripped.fi
-0000ea70: 6e64 2822 5c6e 2229 0a20 2020 2020 2020  nd("\n").       
-0000ea80: 2020 2020 2020 2020 2069 6620 706f 7320           if pos 
-0000ea90: 3d3d 202d 313a 0a20 2020 2020 2020 2020  == -1:.         
-0000eaa0: 2020 2020 2020 2020 2020 2073 7472 6970             strip
-0000eab0: 7065 6420 3d20 2222 0a20 2020 2020 2020  ped = "".       
-0000eac0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0000ead0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eae0: 2020 2073 7472 6970 7065 6420 3d20 7374     stripped = st
-0000eaf0: 7269 7070 6564 5b70 6f73 202b 2031 203a  ripped[pos + 1 :
-0000eb00: 5d0a 0a20 2020 2020 2020 2020 2020 2023  ]..            #
-0000eb10: 2069 6620 7468 6973 2073 7461 7274 7320   if this starts 
-0000eb20: 7769 7468 202f 2a2c 2073 7472 6970 2075  with /*, strip u
-0000eb30: 6e74 696c 202a 2f0a 2020 2020 2020 2020  ntil */.        
-0000eb40: 2020 2020 656c 6966 2073 7472 6970 7065      elif strippe
-0000eb50: 642e 7374 6172 7473 7769 7468 2822 2f2a  d.startswith("/*
-0000eb60: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-0000eb70: 2020 2020 706f 7320 3d20 7374 7269 7070      pos = stripp
-0000eb80: 6564 2e66 696e 6428 222a 2f22 290a 2020  ed.find("*/").  
-0000eb90: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000eba0: 2070 6f73 203d 3d20 2d31 3a0a 2020 2020   pos == -1:.    
-0000ebb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ebc0: 7374 7269 7070 6564 203d 2022 220a 2020  stripped = "".  
-0000ebd0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0000ebe0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000ebf0: 2020 2020 2020 2020 7374 7269 7070 6564          stripped
-0000ec00: 203d 2073 7472 6970 7065 645b 706f 7320   = stripped[pos 
-0000ec10: 2b20 3220 3a5d 0a20 2020 2020 2020 2020  + 2 :].         
-0000ec20: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000ec30: 2020 2020 2020 2020 2023 2079 6179 2c20           # yay, 
-0000ec40: 6e6f 2063 6f6d 6d65 6e74 732c 206d 6f76  no comments, mov
-0000ec50: 6520 746f 2074 6865 206e 6578 7420 7068  e to the next ph
-0000ec60: 6173 650a 2020 2020 2020 2020 2020 2020  ase.            
-0000ec70: 2020 2020 6272 6561 6b0a 0a20 2020 2020      break..     
-0000ec80: 2020 2023 2069 6620 7765 2064 6f6e 2774     # if we don't
-0000ec90: 2068 6176 6520 616e 7974 6869 6e67 206c   have anything l
-0000eca0: 6566 742c 206a 7573 7420 7265 7475 726e  eft, just return
-0000ecb0: 205b 5d0a 2020 2020 2020 2020 6966 206e   [].        if n
-0000ecc0: 6f74 2073 7472 6970 7065 643a 0a20 2020  ot stripped:.   
-0000ecd0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-0000ece0: 0a20 2020 2020 2020 2023 206e 6f77 2073  .        # now s
-0000ecf0: 706c 6974 206f 7574 2074 6865 2077 6f72  plit out the wor
-0000ed00: 6473 0a20 2020 2020 2020 2077 6f72 6473  ds.        words
-0000ed10: 203d 2073 7472 6970 7065 642e 7370 6c69   = stripped.spli
-0000ed20: 7428 4e6f 6e65 2c20 3329 0a0a 2020 2020  t(None, 3)..    
-0000ed30: 2020 2020 2320 5369 6e67 6c65 2077 6f72      # Single wor
-0000ed40: 6420 6d61 7463 6865 730a 2020 2020 2020  d matches.      
-0000ed50: 2020 7175 6572 795f 7479 7065 203d 2077    query_type = w
-0000ed60: 6f72 6473 5b30 5d2e 7570 7065 7228 290a  ords[0].upper().
-0000ed70: 2020 2020 2020 2020 6966 2071 7565 7279          if query
-0000ed80: 5f74 7970 6520 696e 205b 2253 454c 4543  _type in ["SELEC
-0000ed90: 5422 2c20 2257 4954 4822 2c20 2245 5850  T", "WITH", "EXP
-0000eda0: 4f52 5422 2c20 2243 4845 434b 225d 3a0a  ORT", "CHECK"]:.
-0000edb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000edc0: 726e 2073 656c 662e 5f65 7865 6375 7465  rn self._execute
-0000edd0: 5f71 7565 7279 286f 7065 7261 7469 6f6e  _query(operation
-0000ede0: 3d6f 7065 7261 7469 6f6e 2c20 7175 6572  =operation, quer
-0000edf0: 795f 7479 7065 3d71 7565 7279 5f74 7970  y_type=query_typ
-0000ee00: 6529 0a20 2020 2020 2020 2065 6c69 6620  e).        elif 
-0000ee10: 7175 6572 795f 7479 7065 2069 6e20 5b22  query_type in ["
-0000ee20: 4558 504c 4149 4e22 5d3a 0a20 2020 2020  EXPLAIN"]:.     
-0000ee30: 2020 2020 2020 2023 2065 7870 6c61 696e         # explain
-0000ee40: 2070 6970 656c 696e 650a 2020 2020 2020   pipeline.      
-0000ee50: 2020 2020 2020 6966 206c 656e 2877 6f72        if len(wor
-0000ee60: 6473 2920 3e20 3120 616e 6420 776f 7264  ds) > 1 and word
-0000ee70: 735b 315d 2e75 7070 6572 2829 203d 3d20  s[1].upper() == 
-0000ee80: 2250 4950 454c 494e 4522 3a0a 2020 2020  "PIPELINE":.    
-0000ee90: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000eea0: 726e 2073 656c 662e 5f65 7865 6375 7465  rn self._execute
-0000eeb0: 5f71 7565 7279 286f 7065 7261 7469 6f6e  _query(operation
-0000eec0: 3d6f 7065 7261 7469 6f6e 2c20 7175 6572  =operation, quer
-0000eed0: 795f 7479 7065 3d71 7565 7279 5f74 7970  y_type=query_typ
-0000eee0: 6520 2b20 2220 5049 5045 4c49 4e45 2229  e + " PIPELINE")
-0000eef0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0000ef00: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000ef10: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0000ef20: 6578 6563 7574 655f 7175 6572 7928 6f70  execute_query(op
-0000ef30: 6572 6174 696f 6e3d 6f70 6572 6174 696f  eration=operatio
-0000ef40: 6e2c 2071 7565 7279 5f74 7970 653d 7175  n, query_type=qu
-0000ef50: 6572 795f 7479 7065 290a 2020 2020 2020  ery_type).      
-0000ef60: 2020 656c 6966 2071 7565 7279 5f74 7970    elif query_typ
-0000ef70: 6520 696e 205b 224c 4953 5422 5d3a 0a20  e in ["LIST"]:. 
-0000ef80: 2020 2020 2020 2020 2020 2069 6620 6f70             if op
-0000ef90: 6572 6174 696f 6e2e 7570 7065 7228 2920  eration.upper() 
-0000efa0: 3d3d 2022 4c49 5354 2041 4c4c 2051 5545  == "LIST ALL QUE
-0000efb0: 5249 4553 223a 0a20 2020 2020 2020 2020  RIES":.         
-0000efc0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000efd0: 6c66 2e5f 6578 6563 7574 655f 7175 6572  lf._execute_quer
-0000efe0: 7928 6f70 6572 6174 696f 6e3d 2253 454c  y(operation="SEL
-0000eff0: 4543 5420 2a20 4652 4f4d 2053 5953 2e51  ECT * FROM SYS.Q
-0000f000: 5545 5249 4553 222c 2071 7565 7279 5f74  UERIES", query_t
-0000f010: 7970 653d 2253 454c 4543 5422 290a 2020  ype="SELECT").  
-0000f020: 2020 2020 2020 2020 2020 656c 6966 206f            elif o
-0000f030: 7065 7261 7469 6f6e 2e75 7070 6572 2829  peration.upper()
-0000f040: 203d 3d20 224c 4953 5420 414c 4c20 434f   == "LIST ALL CO
-0000f050: 4d50 4c45 5445 4420 5155 4552 4945 5322  MPLETED QUERIES"
-0000f060: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000f070: 2020 7265 7475 726e 2073 656c 662e 5f65    return self._e
-0000f080: 7865 6375 7465 5f71 7565 7279 286f 7065  xecute_query(ope
-0000f090: 7261 7469 6f6e 3d22 5345 4c45 4354 202a  ration="SELECT *
-0000f0a0: 2046 524f 4d20 5359 532e 434f 4d50 4c45   FROM SYS.COMPLE
-0000f0b0: 5445 445f 5155 4552 4945 5322 2c20 7175  TED_QUERIES", qu
-0000f0c0: 6572 795f 7479 7065 3d22 5345 4c45 4354  ery_type="SELECT
-0000f0d0: 2229 0a20 2020 2020 2020 2020 2020 2065  ").            e
-0000f0e0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000f0f0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000f100: 2e5f 6578 6563 7574 655f 6c69 7374 286f  ._execute_list(o
-0000f110: 7065 7261 7469 6f6e 3d6f 7065 7261 7469  peration=operati
-0000f120: 6f6e 290a 2020 2020 2020 2020 656c 6966  on).        elif
-0000f130: 2071 7565 7279 5f74 7970 6520 3d3d 2022   query_type == "
-0000f140: 464f 5243 4522 3a0a 2020 2020 2020 2020  FORCE":.        
-0000f150: 2020 2020 7365 6c66 2e5f 6578 6563 7574      self._execut
-0000f160: 655f 666f 7263 6528 6f70 6572 6174 696f  e_force(operatio
-0000f170: 6e3d 6f70 6572 6174 696f 6e29 0a20 2020  n=operation).   
-0000f180: 2020 2020 2065 6c69 6620 7175 6572 795f       elif query_
-0000f190: 7479 7065 203d 3d20 2253 4554 223a 0a20  type == "SET":. 
-0000f1a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f1b0: 5f65 7865 6375 7465 5f73 6574 2877 6f72  _execute_set(wor
-0000f1c0: 6473 5b31 3a5d 290a 2020 2020 2020 2020  ds[1:]).        
-0000f1d0: 656c 6966 2071 7565 7279 5f74 7970 6520  elif query_type 
-0000f1e0: 3d3d 2022 4745 5422 3a0a 2020 2020 2020  == "GET":.      
-0000f1f0: 2020 2020 2020 7365 6c66 2e5f 6578 6563        self._exec
-0000f200: 7574 655f 6765 7428 776f 7264 735b 313a  ute_get(words[1:
-0000f210: 5d29 0a20 2020 2020 2020 2065 6c69 6620  ]).        elif 
-0000f220: 7175 6572 795f 7479 7065 203d 3d20 224b  query_type == "K
-0000f230: 494c 4c22 206f 7220 7175 6572 795f 7479  ILL" or query_ty
-0000f240: 7065 203d 3d20 2243 414e 4345 4c22 3a0a  pe == "CANCEL":.
-0000f250: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f260: 2e5f 6578 6563 7574 655f 6361 6e63 656c  ._execute_cancel
-0000f270: 6b69 6c6c 2871 7565 7279 5f74 7970 652c  kill(query_type,
-0000f280: 2077 6f72 6473 5b31 3a5d 290a 2020 2020   words[1:]).    
-0000f290: 2020 2020 656c 6966 2071 7565 7279 5f74      elif query_t
-0000f2a0: 7970 6520 3d3d 2022 434c 4541 5222 3a0a  ype == "CLEAR":.
-0000f2b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f2c0: 2e5f 6578 6563 7574 655f 636c 6561 7228  ._execute_clear(
-0000f2d0: 776f 7264 735b 313a 5d29 0a20 2020 2020  words[1:]).     
-0000f2e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000f2f0: 2020 2020 2023 206f 6b2c 2074 6869 7320       # ok, this 
-0000f300: 6973 2061 6e20 7570 6461 7465 0a20 2020  is an update.   
-0000f310: 2020 2020 2020 2020 2073 656c 662e 5f65           self._e
-0000f320: 7865 6375 7465 5f75 7064 6174 6528 6f70  xecute_update(op
-0000f330: 6572 6174 696f 6e29 0a0a 2020 2020 6465  eration)..    de
-0000f340: 6620 7461 626c 6573 2873 656c 662c 2073  f tables(self, s
-0000f350: 6368 656d 613d 2225 222c 2074 6162 6c65  chema="%", table
-0000f360: 3d22 2522 293a 0a20 2020 2020 2020 2022  ="%"):.        "
-0000f370: 2222 4765 7420 7468 6520 6461 7461 6261  ""Get the databa
-0000f380: 7365 2074 6162 6c65 7322 2222 0a20 2020  se tables""".   
-0000f390: 2020 2020 2023 2070 796c 696e 743a 2064       # pylint: d
-0000f3a0: 6973 6162 6c65 3d6e 6f2d 6d65 6d62 6572  isable=no-member
-0000f3b0: 0a20 2020 2020 2020 2073 656c 662e 5f6d  .        self._m
-0000f3c0: 6574 6164 6174 615f 7265 7128 7072 6f74  etadata_req(prot
-0000f3d0: 6f2e 4665 7463 6853 7973 7465 6d4d 6574  o.FetchSystemMet
-0000f3e0: 6164 6174 612e 4745 545f 5441 424c 4553  adata.GET_TABLES
-0000f3f0: 2c20 7363 6865 6d61 3d73 6368 656d 612c  , schema=schema,
-0000f400: 2074 6162 6c65 3d74 6162 6c65 290a 2020   table=table).  
-0000f410: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000f420: 660a 0a20 2020 2064 6566 2073 7973 7465  f..    def syste
-0000f430: 6d5f 7461 626c 6573 2873 656c 662c 2074  m_tables(self, t
-0000f440: 6162 6c65 3d22 2522 293a 0a20 2020 2020  able="%"):.     
-0000f450: 2020 2022 2222 4765 7420 7468 6520 6461     """Get the da
-0000f460: 7461 6261 7365 2073 7973 7465 6d20 7461  tabase system ta
-0000f470: 626c 6573 2222 220a 2020 2020 2020 2020  bles""".        
-0000f480: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
-0000f490: 653d 6e6f 2d6d 656d 6265 720a 2020 2020  e=no-member.    
-0000f4a0: 2020 2020 7365 6c66 2e5f 6d65 7461 6461      self._metada
-0000f4b0: 7461 5f72 6571 2870 726f 746f 2e46 6574  ta_req(proto.Fet
-0000f4c0: 6368 5379 7374 656d 4d65 7461 6461 7461  chSystemMetadata
-0000f4d0: 2e47 4554 5f53 5953 5445 4d5f 5441 424c  .GET_SYSTEM_TABL
-0000f4e0: 4553 2c20 7461 626c 653d 7461 626c 6529  ES, table=table)
-0000f4f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000f500: 7365 6c66 0a0a 2020 2020 6465 6620 7669  self..    def vi
-0000f510: 6577 7328 7365 6c66 2c20 7669 6577 3d22  ews(self, view="
-0000f520: 2522 293a 0a20 2020 2020 2020 2022 2222  %"):.        """
-0000f530: 4765 7420 7468 6520 6461 7461 6261 7365  Get the database
-0000f540: 2076 6965 7773 2222 220a 2020 2020 2020   views""".      
-0000f550: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
-0000f560: 626c 653d 6e6f 2d6d 656d 6265 720a 2020  ble=no-member.  
-0000f570: 2020 2020 2020 7365 6c66 2e5f 6d65 7461        self._meta
-0000f580: 6461 7461 5f72 6571 2870 726f 746f 2e46  data_req(proto.F
-0000f590: 6574 6368 5379 7374 656d 4d65 7461 6461  etchSystemMetada
-0000f5a0: 7461 2e47 4554 5f56 4945 5753 2c20 7669  ta.GET_VIEWS, vi
-0000f5b0: 6577 3d76 6965 7729 0a20 2020 2020 2020  ew=view).       
-0000f5c0: 2072 6574 7572 6e20 7365 6c66 0a0a 2020   return self..  
-0000f5d0: 2020 6465 6620 636f 6c75 6d6e 7328 7365    def columns(se
-0000f5e0: 6c66 2c20 7363 6865 6d61 3d22 2522 2c20  lf, schema="%", 
-0000f5f0: 7461 626c 653d 2225 222c 2063 6f6c 756d  table="%", colum
-0000f600: 6e3d 2225 2229 3a0a 2020 2020 2020 2020  n="%"):.        
-0000f610: 2222 2247 6574 2074 6865 2064 6174 6162  """Get the datab
-0000f620: 6173 6520 636f 6c75 6d6e 7322 2222 0a20  ase columns""". 
-0000f630: 2020 2020 2020 2023 2070 796c 696e 743a         # pylint:
-0000f640: 2064 6973 6162 6c65 3d6e 6f2d 6d65 6d62   disable=no-memb
-0000f650: 6572 0a20 2020 2020 2020 2073 656c 662e  er.        self.
-0000f660: 5f6d 6574 6164 6174 615f 7265 7128 7072  _metadata_req(pr
-0000f670: 6f74 6f2e 4665 7463 6853 7973 7465 6d4d  oto.FetchSystemM
-0000f680: 6574 6164 6174 612e 4745 545f 434f 4c55  etadata.GET_COLU
-0000f690: 4d4e 532c 2073 6368 656d 613d 7363 6865  MNS, schema=sche
-0000f6a0: 6d61 2c20 7461 626c 653d 7461 626c 652c  ma, table=table,
-0000f6b0: 2063 6f6c 756d 6e3d 636f 6c75 6d6e 290a   column=column).
-0000f6c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000f6d0: 656c 660a 0a20 2020 2064 6566 2069 6e64  elf..    def ind
-0000f6e0: 6578 6573 2873 656c 662c 2073 6368 656d  exes(self, schem
-0000f6f0: 613d 2225 222c 2074 6162 6c65 3d22 2522  a="%", table="%"
-0000f700: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
-0000f710: 7420 7468 6520 6461 7461 6261 7365 2069  t the database i
-0000f720: 6e64 6578 6573 2222 220a 2020 2020 2020  ndexes""".      
-0000f730: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
-0000f740: 626c 653d 6e6f 2d6d 656d 6265 720a 2020  ble=no-member.  
-0000f750: 2020 2020 2020 7365 6c66 2e5f 6d65 7461        self._meta
-0000f760: 6461 7461 5f72 6571 2870 726f 746f 2e46  data_req(proto.F
-0000f770: 6574 6368 5379 7374 656d 4d65 7461 6461  etchSystemMetada
-0000f780: 7461 2e47 4554 5f49 4e44 4558 4553 2c20  ta.GET_INDEXES, 
-0000f790: 7363 6865 6d61 3d73 6368 656d 612c 2074  schema=schema, t
-0000f7a0: 6162 6c65 3d74 6162 6c65 290a 2020 2020  able=table).    
-0000f7b0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-0000f7c0: 0a20 2020 2064 6566 2067 6574 5479 7065  .    def getType
-0000f7d0: 496e 666f 2873 656c 6629 3a20 2023 2070  Info(self):  # p
-0000f7e0: 796c 696e 743a 2064 6973 6162 6c65 3d69  ylint: disable=i
-0000f7f0: 6e76 616c 6964 2d6e 616d 650a 2020 2020  nvalid-name.    
-0000f800: 2020 2020 2222 2247 6574 2074 6865 2064      """Get the d
-0000f810: 6174 6162 6173 6520 7479 7065 2069 6e66  atabase type inf
-0000f820: 6f22 2222 0a20 2020 2020 2020 2023 2070  o""".        # p
-0000f830: 796c 696e 743a 2064 6973 6162 6c65 3d6e  ylint: disable=n
-0000f840: 6f2d 6d65 6d62 6572 0a20 2020 2020 2020  o-member.       
-0000f850: 2073 656c 662e 5f6d 6574 6164 6174 615f   self._metadata_
-0000f860: 7265 7128 7072 6f74 6f2e 4665 7463 6853  req(proto.FetchS
-0000f870: 7973 7465 6d4d 6574 6164 6174 612e 4745  ystemMetadata.GE
-0000f880: 545f 5459 5045 5f49 4e46 4f29 0a20 2020  T_TYPE_INFO).   
-0000f890: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000f8a0: 0a0a 2020 2020 6465 6620 6765 7453 7973  ..    def getSys
-0000f8b0: 7465 6d56 6572 7369 6f6e 2873 656c 6629  temVersion(self)
-0000f8c0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-0000f8d0: 2073 656c 662e 5f65 7865 6375 7465 5f73   self._execute_s
-0000f8e0: 7973 7465 6d6d 6574 6164 6174 6128 7072  ystemmetadata(pr
-0000f8f0: 6f74 6f2e 4665 7463 6853 7973 7465 6d4d  oto.FetchSystemM
-0000f900: 6574 6164 6174 612e 4745 545f 4441 5441  etadata.GET_DATA
-0000f910: 4241 5345 5f50 524f 4455 4354 5f56 4552  BASE_PRODUCT_VER
-0000f920: 5349 4f4e 290a 0a20 2020 2064 6566 205f  SION)..    def _
-0000f930: 6d65 7461 6461 7461 5f72 6571 2873 656c  metadata_req(sel
-0000f940: 662c 2072 6571 7479 7065 2c20 7363 6865  f, reqtype, sche
-0000f950: 6d61 3d22 2522 2c20 7461 626c 653d 2225  ma="%", table="%
-0000f960: 222c 2063 6f6c 756d 6e3d 2225 222c 2076  ", column="%", v
-0000f970: 6965 773d 2225 2229 3a0a 2020 2020 2020  iew="%"):.      
-0000f980: 2020 2222 2249 6e74 6572 6e61 6c20 6675    """Internal fu
-0000f990: 6e63 7469 6f6e 2074 6f20 6765 7420 6461  nction to get da
-0000f9a0: 7461 6261 7365 206d 6574 6164 6174 6122  tabase metadata"
-0000f9b0: 2222 0a20 2020 2020 2020 2023 2070 796c  "".        # pyl
-0000f9c0: 696e 743a 2064 6973 6162 6c65 3d6e 6f2d  int: disable=no-
-0000f9d0: 6d65 6d62 6572 2c74 6f6f 2d6d 616e 792d  member,too-many-
-0000f9e0: 6172 6775 6d65 6e74 730a 2020 2020 2020  arguments.      
-0000f9f0: 2020 7365 6c66 2e5f 7265 696e 6974 6961    self._reinitia
-0000fa00: 6c69 7a65 2829 0a20 2020 2020 2020 2023  lize().        #
-0000fa10: 2072 6571 2e66 6574 6368 5f73 7973 7465   req.fetch_syste
-0000fa20: 6d5f 6d65 7461 6461 7461 2e47 4554 5f54  m_metadata.GET_T
-0000fa30: 4142 4c45 530a 2020 2020 2020 2020 7265  ABLES.        re
-0000fa40: 7120 3d20 7072 6f74 6f2e 5265 7175 6573  q = proto.Reques
-0000fa50: 7428 290a 2020 2020 2020 2020 7265 712e  t().        req.
-0000fa60: 7479 7065 203d 2072 6571 2e46 4554 4348  type = req.FETCH
-0000fa70: 5f53 5953 5445 4d5f 4d45 5441 4441 5441  _SYSTEM_METADATA
-0000fa80: 0a20 2020 2020 2020 2072 6571 2e66 6574  .        req.fet
-0000fa90: 6368 5f73 7973 7465 6d5f 6d65 7461 6461  ch_system_metada
-0000faa0: 7461 2e63 616c 6c20 3d20 7265 7174 7970  ta.call = reqtyp
-0000fab0: 650a 2020 2020 2020 2020 7265 712e 6665  e.        req.fe
-0000fac0: 7463 685f 7379 7374 656d 5f6d 6574 6164  tch_system_metad
-0000fad0: 6174 612e 7363 6865 6d61 203d 2073 6368  ata.schema = sch
-0000fae0: 656d 610a 2020 2020 2020 2020 7265 712e  ema.        req.
-0000faf0: 6665 7463 685f 7379 7374 656d 5f6d 6574  fetch_system_met
-0000fb00: 6164 6174 612e 7461 626c 6520 3d20 7461  adata.table = ta
-0000fb10: 626c 650a 2020 2020 2020 2020 7265 712e  ble.        req.
-0000fb20: 6665 7463 685f 7379 7374 656d 5f6d 6574  fetch_system_met
-0000fb30: 6164 6174 612e 636f 6c75 6d6e 203d 2063  adata.column = c
-0000fb40: 6f6c 756d 6e0a 2020 2020 2020 2020 7265  olumn.        re
-0000fb50: 712e 6665 7463 685f 7379 7374 656d 5f6d  q.fetch_system_m
-0000fb60: 6574 6164 6174 612e 7669 6577 203d 2076  etadata.view = v
-0000fb70: 6965 770a 2020 2020 2020 2020 7265 712e  iew.        req.
-0000fb80: 6665 7463 685f 7379 7374 656d 5f6d 6574  fetch_system_met
-0000fb90: 6164 6174 612e 7465 7374 203d 2054 7275  adata.test = Tru
-0000fba0: 650a 0a20 2020 2020 2020 205f 7365 6e64  e..        _send
-0000fbb0: 5f6d 7367 2873 656c 662e 636f 6e6e 6563  _msg(self.connec
-0000fbc0: 7469 6f6e 2c20 7265 7129 0a0a 2020 2020  tion, req)..    
-0000fbd0: 2020 2020 7273 7020 3d20 5f72 6563 765f      rsp = _recv_
-0000fbe0: 6d73 6728 7365 6c66 2e63 6f6e 6e65 6374  msg(self.connect
-0000fbf0: 696f 6e2c 2070 726f 746f 2e46 6574 6368  ion, proto.Fetch
-0000fc00: 5379 7374 656d 4d65 7461 6461 7461 5265  SystemMetadataRe
-0000fc10: 7370 6f6e 7365 2829 290a 0a20 2020 2020  sponse())..     
-0000fc20: 2020 2069 6620 7273 702e 7265 7370 6f6e     if rsp.respon
-0000fc30: 7365 2e74 7970 6520 3d3d 2070 726f 746f  se.type == proto
-0000fc40: 2e43 6f6e 6669 726d 6174 696f 6e52 6573  .ConfirmationRes
-0000fc50: 706f 6e73 652e 5245 5350 4f4e 5345 5f45  ponse.RESPONSE_E
-0000fc60: 5252 4f52 3a0a 2020 2020 2020 2020 2020  RROR:.          
-0000fc70: 2020 6966 2072 7370 2e72 6573 706f 6e73    if rsp.respons
-0000fc80: 652e 7665 6e64 6f72 5f63 6f64 6520 3d3d  e.vendor_code ==
-0000fc90: 2053 4553 5349 4f4e 5f45 5850 4952 4544   SESSION_EXPIRED
-0000fca0: 5f43 4f44 453a 0a20 2020 2020 2020 2020  _CODE:.         
-0000fcb0: 2020 2020 2020 2023 204e 6565 6420 746f         # Need to
-0000fcc0: 2072 6566 7265 7368 2074 6865 2073 6573   refresh the ses
-0000fcd0: 7369 6f6e 0a20 2020 2020 2020 2020 2020  sion.           
-0000fce0: 2020 2020 2073 656c 662e 636f 6e6e 6563       self.connec
-0000fcf0: 7469 6f6e 2e72 6566 7265 7368 2829 0a20  tion.refresh(). 
-0000fd00: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000fd10: 2061 6e64 2074 7279 2061 6761 696e 0a20   and try again. 
-0000fd20: 2020 2020 2020 2020 2020 2020 2020 205f                 _
-0000fd30: 6d65 7461 6461 7461 5f72 6571 2872 6571  metadata_req(req
-0000fd40: 7479 7065 2c20 7363 6865 6d61 3d73 6368  type, schema=sch
-0000fd50: 656d 612c 2074 6162 6c65 3d74 6162 6c65  ema, table=table
-0000fd60: 2c20 636f 6c75 6d6e 3d63 6f6c 756d 6e2c  , column=column,
-0000fd70: 2076 6965 773d 7669 6577 290a 2020 2020   view=view).    
-0000fd80: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000fd90: 726e 0a20 2020 2020 2020 2020 2020 2065  rn.            e
-0000fda0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000fdb0: 2020 2020 2072 6169 7365 205f 636f 6e76       raise _conv
-0000fdc0: 6572 745f 6578 6365 7074 696f 6e28 7273  ert_exception(rs
-0000fdd0: 702e 7265 7370 6f6e 7365 290a 0a20 2020  p.response)..   
-0000fde0: 2020 2020 2073 656c 662e 5f67 6574 5f72       self._get_r
-0000fdf0: 6573 756c 745f 6d65 7461 6461 7461 2829  esult_metadata()
-0000fe00: 0a0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
-0000fe10: 6f77 6e75 6d62 6572 203d 2030 0a20 2020  ownumber = 0.   
-0000fe20: 2020 2020 2066 6f72 2062 6c6f 6220 696e       for blob in
-0000fe30: 2072 7370 2e72 6573 756c 745f 7365 745f   rsp.result_set_
-0000fe40: 7661 6c2e 626c 6f62 733a 0a20 2020 2020  val.blobs:.     
-0000fe50: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-0000fe60: 6c66 2e5f 6275 6666 6572 733a 0a20 2020  lf._buffers:.   
-0000fe70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000fe80: 662e 5f6f 6666 7365 7420 3d20 300a 2020  f._offset = 0.  
-0000fe90: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000fea0: 6275 6666 6572 732e 6170 7065 6e64 2862  buffers.append(b
-0000feb0: 6c6f 6229 0a0a 2020 2020 6465 6620 5f65  lob)..    def _e
-0000fec0: 7865 6375 7465 5f71 7565 7279 2873 656c  xecute_query(sel
-0000fed0: 662c 206f 7065 7261 7469 6f6e 2c20 7175  f, operation, qu
-0000fee0: 6572 795f 7479 7065 3a20 7374 7220 3d20  ery_type: str = 
-0000fef0: 2253 454c 4543 5422 293a 0a20 2020 2020  "SELECT"):.     
-0000ff00: 2020 2022 2222 4578 6563 7574 6520 6120     """Execute a 
-0000ff10: 7175 6572 7922 2222 0a20 2020 2020 2020  query""".       
-0000ff20: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
-0000ff30: 6c65 3d6e 6f2d 6d65 6d62 6572 0a0a 2020  le=no-member..  
-0000ff40: 2020 2020 2020 6661 6374 6f72 7920 3d20        factory = 
-0000ff50: 5f4f 4349 454e 545f 5245 5155 4553 545f  _OCIENT_REQUEST_
-0000ff60: 4641 4354 4f52 4945 532e 6765 7428 7175  FACTORIES.get(qu
-0000ff70: 6572 795f 7479 7065 2e75 7070 6572 2829  ery_type.upper()
-0000ff80: 2c20 4e6f 6e65 290a 0a20 2020 2020 2020  , None)..       
-0000ff90: 2069 6620 6661 6374 6f72 7920 6973 204e   if factory is N
-0000ffa0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000ffb0: 2072 6169 7365 204e 6f74 5375 7070 6f72   raise NotSuppor
-0000ffc0: 7465 6445 7272 6f72 2866 2251 7565 7279  tedError(f"Query
-0000ffd0: 2074 7970 6520 277b 7175 6572 795f 7479   type '{query_ty
-0000ffe0: 7065 7d27 206e 6f74 2073 7570 706f 7274  pe}' not support
-0000fff0: 6564 2062 7920 7079 6f63 6965 6e74 2722  ed by pyocient'"
-00010000: 290a 0a20 2020 2020 2020 2023 2067 656e  )..        # gen
-00010010: 6572 6174 6520 7468 6520 6170 7072 6f70  erate the approp
-00010020: 7269 6174 6520 7265 7175 6573 740a 2020  riate request.  
-00010030: 2020 2020 2020 7265 7120 3d20 6661 6374        req = fact
-00010040: 6f72 792e 7265 7175 6573 7428 6f70 6572  ory.request(oper
-00010050: 6174 696f 6e29 0a0a 2020 2020 2020 2020  ation)..        
-00010060: 2320 4c6f 6f70 2077 6869 6c65 2077 6520  # Loop while we 
-00010070: 7265 7472 7920 7265 6469 7265 6374 7320  retry redirects 
-00010080: 616e 6420 7265 636f 6e6e 6563 7473 0a20  and reconnects. 
-00010090: 2020 2020 2020 2077 6869 6c65 2054 7275         while Tru
-000100a0: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-000100b0: 6620 7265 712e 7479 7065 203d 3d20 7072  f req.type == pr
-000100c0: 6f74 6f2e 5265 7175 6573 742e 5265 7175  oto.Request.Requ
-000100d0: 6573 7454 7970 652e 5661 6c75 6528 2245  estType.Value("E
-000100e0: 5845 4355 5445 5f51 5545 5259 2229 3a0a  XECUTE_QUERY"):.
-000100f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010100: 7265 712e 6578 6563 7574 655f 7175 6572  req.execute_quer
-00010110: 792e 666f 7263 6520 3d20 7365 6c66 2e63  y.force = self.c
-00010120: 6f6e 6e65 6374 696f 6e2e 666f 7263 650a  onnection.force.
-00010130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010140: 7265 712e 6578 6563 7574 655f 7175 6572  req.execute_quer
-00010150: 792e 666f 7263 6552 6564 6972 6563 7420  y.forceRedirect 
-00010160: 3d20 7365 6c66 2e63 6f6e 6e65 6374 696f  = self.connectio
-00010170: 6e2e 666f 7263 655f 6e65 7874 5f72 6564  n.force_next_red
-00010180: 6972 6563 740a 2020 2020 2020 2020 2020  irect.          
-00010190: 2020 2020 2020 7365 6c66 2e63 6f6e 6e65        self.conne
-000101a0: 6374 696f 6e2e 666f 7263 655f 6e65 7874  ction.force_next
-000101b0: 5f72 6564 6972 6563 7420 3d20 4661 6c73  _redirect = Fals
-000101c0: 650a 2020 2020 2020 2020 2020 2020 656c  e.            el
-000101d0: 6966 2072 6571 2e74 7970 6520 3d3d 2070  if req.type == p
-000101e0: 726f 746f 2e52 6571 7565 7374 2e52 6571  roto.Request.Req
-000101f0: 7565 7374 5479 7065 2e56 616c 7565 2822  uestType.Value("
-00010200: 4558 4543 5554 455f 4558 504c 4149 4e22  EXECUTE_EXPLAIN"
-00010210: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00010220: 2020 2072 6571 2e65 7865 6375 7465 5f65     req.execute_e
-00010230: 7870 6c61 696e 2e66 6f72 6365 203d 2073  xplain.force = s
-00010240: 656c 662e 636f 6e6e 6563 7469 6f6e 2e66  elf.connection.f
-00010250: 6f72 6365 0a20 2020 2020 2020 2020 2020  orce.           
-00010260: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00010270: 2020 2020 2020 5f73 656e 645f 6d73 6728        _send_msg(
-00010280: 7365 6c66 2e63 6f6e 6e65 6374 696f 6e2c  self.connection,
-00010290: 2072 6571 290a 0a20 2020 2020 2020 2020   req)..         
-000102a0: 2020 2020 2020 2072 7370 203d 205f 7265         rsp = _re
-000102b0: 6376 5f6d 7367 2873 656c 662e 636f 6e6e  cv_msg(self.conn
-000102c0: 6563 7469 6f6e 2c20 6661 6374 6f72 792e  ection, factory.
-000102d0: 7265 7370 6f6e 7365 2829 290a 2020 2020  response()).    
-000102e0: 2020 2020 2020 2020 6578 6365 7074 2049          except I
-000102f0: 4f45 7272 6f72 3a0a 2020 2020 2020 2020  OError:.        
-00010300: 2020 2020 2020 2020 2320 7265 6d61 6b65          # remake
-00010310: 206f 7572 2063 6f6e 6e65 6374 696f 6e0a   our connection.
-00010320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010330: 7365 6c66 2e63 6f6e 6e65 6374 696f 6e20  self.connection 
-00010340: 3d20 436f 6e6e 6563 7469 6f6e 280a 2020  = Connection(.  
-00010350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010360: 2020 7573 6572 3d73 656c 662e 636f 6e6e    user=self.conn
-00010370: 6563 7469 6f6e 2e75 7365 722c 0a20 2020  ection.user,.   
-00010380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010390: 2070 6173 7377 6f72 643d 7365 6c66 2e63   password=self.c
-000103a0: 6f6e 6e65 6374 696f 6e2e 7061 7373 776f  onnection.passwo
-000103b0: 7264 2c0a 2020 2020 2020 2020 2020 2020  rd,.            
-000103c0: 2020 2020 2020 2020 686f 7374 3d66 227b          host=f"{
-000103d0: 272c 272e 6a6f 696e 2873 656c 662e 636f  ','.join(self.co
-000103e0: 6e6e 6563 7469 6f6e 2e68 6f73 7473 297d  nnection.hosts)}
-000103f0: 3a7b 7365 6c66 2e63 6f6e 6e65 6374 696f  :{self.connectio
-00010400: 6e2e 706f 7274 7d22 2c0a 2020 2020 2020  n.port}",.      
-00010410: 2020 2020 2020 2020 2020 2020 2020 6461                da
-00010420: 7461 6261 7365 3d73 656c 662e 636f 6e6e  tabase=self.conn
-00010430: 6563 7469 6f6e 2e64 6174 6162 6173 652c  ection.database,
-00010440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010450: 2020 2020 2074 6c73 3d73 656c 662e 636f       tls=self.co
-00010460: 6e6e 6563 7469 6f6e 2e74 6c73 2c0a 2020  nnection.tls,.  
-00010470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010480: 2020 6861 6e64 7368 616b 653d 7365 6c66    handshake=self
-00010490: 2e63 6f6e 6e65 6374 696f 6e2e 6861 6e64  .connection.hand
-000104a0: 7368 616b 652c 0a20 2020 2020 2020 2020  shake,.         
-000104b0: 2020 2020 2020 2020 2020 2066 6f72 6365             force
-000104c0: 3d73 656c 662e 636f 6e6e 6563 7469 6f6e  =self.connection
-000104d0: 2e66 6f72 6365 2c0a 2020 2020 2020 2020  .force,.        
-000104e0: 2020 2020 2020 2020 2020 2020 7365 7373              sess
-000104f0: 696f 6e3d 7365 6c66 2e63 6f6e 6e65 6374  ion=self.connect
-00010500: 696f 6e2e 7365 7373 696f 6e2c 0a20 2020  ion.session,.   
-00010510: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
-00010520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010530: 636f 6e74 696e 7565 0a0a 2020 2020 2020  continue..      
-00010540: 2020 2020 2020 6966 2072 7370 2e72 6573        if rsp.res
-00010550: 706f 6e73 652e 7479 7065 203d 3d20 7072  ponse.type == pr
-00010560: 6f74 6f2e 436f 6e66 6972 6d61 7469 6f6e  oto.Confirmation
-00010570: 5265 7370 6f6e 7365 2e52 4553 504f 4e53  Response.RESPONS
-00010580: 455f 5741 524e 3a0a 2020 2020 2020 2020  E_WARN:.        
-00010590: 2020 2020 2020 2020 7761 726e 2872 7370          warn(rsp
-000105a0: 2e72 6573 706f 6e73 652e 7265 6173 6f6e  .response.reason
-000105b0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-000105c0: 6966 206e 6f74 2072 7370 2e72 6573 706f  if not rsp.respo
-000105d0: 6e73 652e 7479 7065 203d 3d20 7072 6f74  nse.type == prot
-000105e0: 6f2e 436f 6e66 6972 6d61 7469 6f6e 5265  o.ConfirmationRe
-000105f0: 7370 6f6e 7365 2e52 4553 504f 4e53 455f  sponse.RESPONSE_
-00010600: 4f4b 3a0a 2020 2020 2020 2020 2020 2020  OK:.            
-00010610: 2020 2020 6966 2072 7370 2e72 6573 706f      if rsp.respo
-00010620: 6e73 652e 7665 6e64 6f72 5f63 6f64 6520  nse.vendor_code 
-00010630: 3d3d 2053 4553 5349 4f4e 5f45 5850 4952  == SESSION_EXPIR
-00010640: 4544 5f43 4f44 453a 0a20 2020 2020 2020  ED_CODE:.       
-00010650: 2020 2020 2020 2020 2020 2020 2023 204e               # N
-00010660: 6565 6420 746f 2072 6566 7265 7368 2074  eed to refresh t
-00010670: 6865 2073 6573 7369 6f6e 0a20 2020 2020  he session.     
-00010680: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00010690: 656c 662e 636f 6e6e 6563 7469 6f6e 2e72  elf.connection.r
-000106a0: 6566 7265 7368 2829 0a20 2020 2020 2020  efresh().       
-000106b0: 2020 2020 2020 2020 2020 2020 2023 2061               # a
-000106c0: 6e64 2074 7279 2061 6761 696e 0a20 2020  nd try again.   
-000106d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106e0: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
-000106f0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00010700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010710: 2020 2020 7261 6973 6520 5f63 6f6e 7665      raise _conve
-00010720: 7274 5f65 7863 6570 7469 6f6e 2872 7370  rt_exception(rsp
-00010730: 2e72 6573 706f 6e73 6529 0a0a 2020 2020  .response)..    
-00010740: 2020 2020 2020 2020 2320 7365 6520 6966          # see if
-00010750: 2077 6520 6172 6520 6265 696e 6720 746f   we are being to
-00010760: 6c64 2074 6f20 7265 6469 7265 6374 0a20  ld to redirect. 
-00010770: 2020 2020 2020 2020 2020 2072 6564 6972             redir
-00010780: 6563 7420 3d20 6765 7461 7474 7228 7273  ect = getattr(rs
-00010790: 702c 2022 7265 6469 7265 6374 222c 2046  p, "redirect", F
-000107a0: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
-000107b0: 2020 6966 206e 6f74 2072 6564 6972 6563    if not redirec
-000107c0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-000107d0: 2020 2062 7265 616b 0a0a 2020 2020 2020     break..      
-000107e0: 2020 2020 2020 2320 7265 6d61 6b65 206f        # remake o
-000107f0: 7572 2063 6f6e 6e65 6374 696f 6e0a 2020  ur connection.  
-00010800: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00010810: 6f6e 6e65 6374 696f 6e2e 636c 6f73 6528  onnection.close(
-00010820: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00010830: 6c66 2e63 6f6e 6e65 6374 696f 6e20 3d20  lf.connection = 
-00010840: 7365 6c66 2e63 6f6e 6e65 6374 696f 6e2e  self.connection.
-00010850: 7265 6469 7265 6374 2872 7370 2e72 6564  redirect(rsp.red
-00010860: 6972 6563 7448 6f73 742c 2072 7370 2e72  irectHost, rsp.r
-00010870: 6564 6972 6563 7450 6f72 7429 0a0a 2020  edirectPort)..  
-00010880: 2020 2020 2020 7175 6572 795f 6964 203d        query_id =
-00010890: 2067 6574 6174 7472 2872 7370 2c20 2271   getattr(rsp, "q
-000108a0: 7565 7279 4964 222c 204e 6f6e 6529 0a20  ueryId", None). 
-000108b0: 2020 2020 2020 2069 6620 7175 6572 795f         if query_
-000108c0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-000108d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000108e0: 2e71 7565 7279 5f69 6420 3d20 7175 6572  .query_id = quer
-000108f0: 795f 6964 0a0a 2020 2020 2020 2020 7365  y_id..        se
-00010900: 6c66 2e72 6f77 6e75 6d62 6572 203d 2030  lf.rownumber = 0
-00010910: 0a0a 2020 2020 2020 2020 6966 2071 7565  ..        if que
-00010920: 7279 5f74 7970 6520 696e 205b 2253 454c  ry_type in ["SEL
-00010930: 4543 5422 2c20 2257 4954 4822 5d3a 0a20  ECT", "WITH"]:. 
-00010940: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010950: 5f67 6574 5f72 6573 756c 745f 6d65 7461  _get_result_meta
-00010960: 6461 7461 2829 0a0a 2020 2020 2020 2020  data()..        
-00010970: 656c 6966 2071 7565 7279 5f74 7970 6520  elif query_type 
-00010980: 3d3d 2022 4558 504c 4149 4e22 3a0a 2020  == "EXPLAIN":.  
-00010990: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-000109a0: 6573 6372 6970 7469 6f6e 203d 205b 2822  escription = [("
-000109b0: 6578 706c 6169 6e22 2c20 5479 7065 436f  explain", TypeCo
-000109c0: 6465 732e 4348 4152 2c20 4e6f 6e65 2c20  des.CHAR, None, 
-000109d0: 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65  None, None, None
-000109e0: 2c20 4e6f 6e65 295d 2020 2320 6469 7370  , None)]  # disp
-000109f0: 6c61 795f 7369 7a65 2020 2320 696e 7465  lay_size  # inte
-00010a00: 726e 616c 5f73 697a 6520 2023 2070 7265  rnal_size  # pre
-00010a10: 6369 7369 6f6e 2020 2320 7363 616c 6520  cision  # scale 
-00010a20: 2023 206e 756c 6c5f 6f6b 0a0a 2020 2020   # null_ok..    
-00010a30: 2020 2020 2020 2020 7365 6c66 2e65 7870          self.exp
-00010a40: 6c61 696e 5f72 6573 756c 7420 3d20 7273  lain_result = rs
-00010a50: 702e 706c 616e 0a0a 2020 2020 2320 4166  p.plan..    # Af
-00010a60: 7465 7220 6c69 7374 2061 6c6c 2071 7565  ter list all que
-00010a70: 7269 6573 2061 6e64 206c 6973 7420 616c  ries and list al
-00010a80: 6c20 636f 6d70 6c65 7465 6420 7175 6572  l completed quer
-00010a90: 6965 7320 6861 7665 2062 6565 6e20 7265  ies have been re
-00010aa0: 6d61 7070 6564 2c20 7468 6973 2069 7320  mapped, this is 
-00010ab0: 6e6f 206c 6f6e 6765 7220 7573 6564 2e20  no longer used. 
-00010ac0: 4275 7420 6974 2063 616e 2062 6520 7573  But it can be us
-00010ad0: 6564 2066 6f72 206f 7468 6572 2074 6869  ed for other thi
-00010ae0: 6e67 732e 0a20 2020 2023 2045 783a 206c  ngs..    # Ex: l
-00010af0: 6973 7420 7461 626c 6573 2c20 6c69 7374  ist tables, list
-00010b00: 2076 6965 7773 2c20 6c69 7374 2074 6162   views, list tab
-00010b10: 6c65 2070 7269 7669 6c65 6765 732e 204e  le privileges. N
-00010b20: 6f6e 6520 6f66 2074 6865 7365 2061 7265  one of these are
-00010b30: 2069 6d70 6c65 6d65 6e74 6564 2079 6574   implemented yet
-00010b40: 2e0a 2020 2020 6465 6620 5f65 7865 6375  ..    def _execu
-00010b50: 7465 5f6c 6973 7428 7365 6c66 2c20 6f70  te_list(self, op
-00010b60: 6572 6174 696f 6e3a 2073 7472 203d 2022  eration: str = "
-00010b70: 4c49 5354 2041 4c4c 2051 5545 5249 4553  LIST ALL QUERIES
-00010b80: 2229 3a0a 2020 2020 2020 2020 2222 2245  "):.        """E
-00010b90: 7865 6375 7465 204c 4953 545f 414c 4c5f  xecute LIST_ALL_
-00010ba0: 5155 4552 4945 5322 2222 0a20 2020 2020  QUERIES""".     
-00010bb0: 2020 2023 2070 796c 696e 743a 2064 6973     # pylint: dis
-00010bc0: 6162 6c65 3d6e 6f2d 6d65 6d62 6572 0a0a  able=no-member..
-00010bd0: 2020 2020 2020 2020 6661 6374 6f72 7920          factory 
-00010be0: 3d20 5f4f 4349 454e 545f 5245 5155 4553  = _OCIENT_REQUES
-00010bf0: 545f 4641 4354 4f52 4945 532e 6765 7428  T_FACTORIES.get(
-00010c00: 6f70 6572 6174 696f 6e2e 7570 7065 7228  operation.upper(
-00010c10: 292c 204e 6f6e 6529 0a0a 2020 2020 2020  ), None)..      
-00010c20: 2020 6966 2066 6163 746f 7279 2069 7320    if factory is 
-00010c30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00010c40: 2020 7261 6973 6520 4e6f 7453 7570 706f    raise NotSuppo
-00010c50: 7274 6564 4572 726f 7228 6622 4c69 7374  rtedError(f"List
-00010c60: 2071 7565 7279 2027 7b6f 7065 7261 7469   query '{operati
-00010c70: 6f6e 7d27 206e 6f74 2073 7570 706f 7274  on}' not support
-00010c80: 6564 2062 7920 7079 6f63 6965 6e74 2722  ed by pyocient'"
-00010c90: 290a 0a20 2020 2020 2020 2023 2067 6565  )..        # gee
-00010ca0: 7261 7465 2074 6865 2061 7070 726f 7072  rate the appropr
-00010cb0: 6961 7465 2072 6571 7565 7374 0a20 2020  iate request.   
-00010cc0: 2020 2020 2072 6571 203d 2066 6163 746f       req = facto
-00010cd0: 7279 2e72 6571 7565 7374 286f 7065 7261  ry.request(opera
-00010ce0: 7469 6f6e 290a 0a20 2020 2020 2020 2077  tion)..        w
-00010cf0: 6869 6c65 2054 7275 653a 0a20 2020 2020  hile True:.     
-00010d00: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00010d10: 2020 2020 2020 2020 2020 2020 5f73 656e              _sen
-00010d20: 645f 6d73 6728 7365 6c66 2e63 6f6e 6e65  d_msg(self.conne
-00010d30: 6374 696f 6e2c 2072 6571 290a 0a20 2020  ction, req)..   
-00010d40: 2020 2020 2020 2020 2020 2020 2072 7370               rsp
-00010d50: 203d 205f 7265 6376 5f6d 7367 2873 656c   = _recv_msg(sel
-00010d60: 662e 636f 6e6e 6563 7469 6f6e 2c20 6661  f.connection, fa
-00010d70: 6374 6f72 792e 7265 7370 6f6e 7365 2829  ctory.response()
-00010d80: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
-00010d90: 6365 7074 2049 4f45 7272 6f72 3a0a 2020  cept IOError:.  
-00010da0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00010db0: 7265 6d61 6b65 206f 7572 2063 6f6e 6e65  remake our conne
-00010dc0: 6374 696f 6e0a 2020 2020 2020 2020 2020  ction.          
-00010dd0: 2020 2020 2020 7365 6c66 2e63 6f6e 6e65        self.conne
-00010de0: 6374 696f 6e20 3d20 436f 6e6e 6563 7469  ction = Connecti
-00010df0: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
-00010e00: 2020 2020 2020 2020 7573 6572 3d73 656c          user=sel
-00010e10: 662e 636f 6e6e 6563 7469 6f6e 2e75 7365  f.connection.use
-00010e20: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-00010e30: 2020 2020 2020 2070 6173 7377 6f72 643d         password=
-00010e40: 7365 6c66 2e63 6f6e 6e65 6374 696f 6e2e  self.connection.
-00010e50: 7061 7373 776f 7264 2c0a 2020 2020 2020  password,.      
-00010e60: 2020 2020 2020 2020 2020 2020 2020 686f                ho
-00010e70: 7374 3d66 227b 272c 272e 6a6f 696e 2873  st=f"{','.join(s
-00010e80: 656c 662e 636f 6e6e 6563 7469 6f6e 2e68  elf.connection.h
-00010e90: 6f73 7473 297d 3a7b 7365 6c66 2e63 6f6e  osts)}:{self.con
-00010ea0: 6e65 6374 696f 6e2e 706f 7274 7d22 2c0a  nection.port}",.
-00010eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ec0: 2020 2020 6461 7461 6261 7365 3d73 656c      database=sel
-00010ed0: 662e 636f 6e6e 6563 7469 6f6e 2e64 6174  f.connection.dat
-00010ee0: 6162 6173 652c 0a20 2020 2020 2020 2020  abase,.         
-00010ef0: 2020 2020 2020 2020 2020 2074 6c73 3d73             tls=s
-00010f00: 656c 662e 636f 6e6e 6563 7469 6f6e 2e74  elf.connection.t
-00010f10: 6c73 2c0a 2020 2020 2020 2020 2020 2020  ls,.            
-00010f20: 2020 2020 2020 2020 6861 6e64 7368 616b          handshak
-00010f30: 653d 7365 6c66 2e63 6f6e 6e65 6374 696f  e=self.connectio
-00010f40: 6e2e 6861 6e64 7368 616b 652c 0a20 2020  n.handshake,.   
-00010f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f60: 2066 6f72 6365 3d73 656c 662e 636f 6e6e   force=self.conn
-00010f70: 6563 7469 6f6e 2e66 6f72 6365 2c0a 2020  ection.force,.  
-00010f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f90: 2020 7365 7373 696f 6e3d 7365 6c66 2e63    session=self.c
-00010fa0: 6f6e 6e65 6374 696f 6e2e 7365 7373 696f  onnection.sessio
-00010fb0: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
-00010fc0: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
-00010fd0: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
-00010fe0: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00010ff0: 0a0a 2020 2020 2020 2020 6966 2072 7370  ..        if rsp
-00011000: 2e72 6573 706f 6e73 652e 7479 7065 203d  .response.type =
-00011010: 3d20 7072 6f74 6f2e 436f 6e66 6972 6d61  = proto.Confirma
-00011020: 7469 6f6e 5265 7370 6f6e 7365 2e52 4553  tionResponse.RES
-00011030: 504f 4e53 455f 5741 524e 3a0a 2020 2020  PONSE_WARN:.    
-00011040: 2020 2020 2020 2020 7761 726e 2872 7370          warn(rsp
-00011050: 2e72 6573 706f 6e73 652e 7265 6173 6f6e  .response.reason
-00011060: 290a 2020 2020 2020 2020 656c 6966 206e  ).        elif n
-00011070: 6f74 2072 7370 2e72 6573 706f 6e73 652e  ot rsp.response.
-00011080: 7479 7065 203d 3d20 7072 6f74 6f2e 436f  type == proto.Co
-00011090: 6e66 6972 6d61 7469 6f6e 5265 7370 6f6e  nfirmationRespon
-000110a0: 7365 2e52 4553 504f 4e53 455f 4f4b 3a0a  se.RESPONSE_OK:.
-000110b0: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-000110c0: 7370 2e72 6573 706f 6e73 652e 7665 6e64  sp.response.vend
-000110d0: 6f72 5f63 6f64 6520 3d3d 2053 4553 5349  or_code == SESSI
-000110e0: 4f4e 5f45 5850 4952 4544 5f43 4f44 453a  ON_EXPIRED_CODE:
-000110f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011100: 2023 204e 6565 6420 746f 2072 6566 7265   # Need to refre
-00011110: 7368 2074 6865 2073 6573 7369 6f6e 0a20  sh the session. 
-00011120: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00011130: 656c 662e 636f 6e6e 6563 7469 6f6e 2e72  elf.connection.r
-00011140: 6566 7265 7368 2829 0a20 2020 2020 2020  efresh().       
-00011150: 2020 2020 2020 2020 2023 2061 6e64 2074           # and t
-00011160: 7279 2061 6761 696e 0a20 2020 2020 2020  ry again.       
-00011170: 2020 2020 2020 2020 2073 656c 662e 5f65           self._e
-00011180: 7865 6375 7465 5f6c 6973 7428 6f70 6572  xecute_list(oper
-00011190: 6174 696f 6e3d 6f70 6572 6174 696f 6e29  ation=operation)
-000111a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000111b0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-000111c0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000111d0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000111e0: 5f63 6f6e 7665 7274 5f65 7863 6570 7469  _convert_excepti
-000111f0: 6f6e 2872 7370 2e72 6573 706f 6e73 6529  on(rsp.response)
-00011200: 0a0a 2020 2020 2020 2020 7365 6c66 2e64  ..        self.d
-00011210: 6573 6372 6970 7469 6f6e 203d 205b 5d0a  escription = [].
-00011220: 0a20 2020 2020 2020 2072 6f77 7320 3d20  .        rows = 
-00011230: 6661 6374 6f72 792e 7072 6f63 6573 7328  factory.process(
-00011240: 7273 7029 0a20 2020 2020 2020 2069 6620  rsp).        if 
-00011250: 6e6f 7420 726f 7773 3a0a 2020 2020 2020  not rows:.      
-00011260: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00011270: 7265 7375 6c74 203d 205b 5d0a 2020 2020  result = [].    
-00011280: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
-00011290: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
-000112a0: 2074 6865 2063 6f6c 756d 6e20 6465 7363   the column desc
-000112b0: 7269 7074 696f 6e73 0a20 2020 2020 2020  riptions.       
-000112c0: 2072 6f77 203d 2072 6f77 735b 305d 0a20   row = rows[0]. 
-000112d0: 2020 2020 2020 2066 6f72 2066 6965 6c64         for field
-000112e0: 2069 6e20 726f 772e 5f66 6965 6c64 733a   in row._fields:
-000112f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00011300: 662e 6465 7363 7269 7074 696f 6e2e 6170  f.description.ap
-00011310: 7065 6e64 280a 2020 2020 2020 2020 2020  pend(.          
-00011320: 2020 2020 2020 2866 6965 6c64 2c20 5479        (field, Ty
-00011330: 7065 436f 6465 732e 636c 735f 746f 5f74  peCodes.cls_to_t
-00011340: 7970 6528 726f 772e 5f66 6965 6c64 5f74  ype(row._field_t
-00011350: 7970 6573 5b66 6965 6c64 5d29 2c20 4e6f  ypes[field]), No
-00011360: 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65 2c20  ne, None, None, 
-00011370: 4e6f 6e65 2c20 4e6f 6e65 2920 2023 2064  None, None)  # d
-00011380: 6973 706c 6179 5f73 697a 6520 2023 2069  isplay_size  # i
-00011390: 6e74 6572 6e61 6c5f 7369 7a65 2020 2320  nternal_size  # 
-000113a0: 7072 6563 6973 696f 6e20 2023 2073 6361  precision  # sca
-000113b0: 6c65 2020 2320 6e75 6c6c 5f6f 6b0a 2020  le  # null_ok.  
-000113c0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-000113d0: 2020 2020 2023 2061 6e64 2073 6574 2074       # and set t
-000113e0: 6865 2072 6573 756c 7473 0a20 2020 2020  he results.     
-000113f0: 2020 2073 656c 662e 6c69 7374 5f72 6573     self.list_res
-00011400: 756c 7420 3d20 726f 7773 0a0a 2020 2020  ult = rows..    
-00011410: 6465 6620 5f67 6574 5f72 6573 756c 745f  def _get_result_
-00011420: 6d65 7461 6461 7461 2873 656c 6629 3a0a  metadata(self):.
-00011430: 2020 2020 2020 2020 2222 2249 6e74 6572          """Inter
-00011440: 6e61 6c20 726f 7574 696e 6520 746f 2067  nal routine to g
-00011450: 6574 206d 6574 6164 6174 6120 666f 7220  et metadata for 
-00011460: 6120 7265 7375 6c74 2073 6574 2222 220a  a result set""".
-00011470: 2020 2020 2020 2020 2320 7079 6c69 6e74          # pylint
-00011480: 3a20 6469 7361 626c 653d 6e6f 2d6d 656d  : disable=no-mem
-00011490: 6265 720a 2020 2020 2020 2020 7265 7120  ber.        req 
-000114a0: 3d20 7072 6f74 6f2e 5265 7175 6573 7428  = proto.Request(
-000114b0: 290a 2020 2020 2020 2020 7265 712e 7479  ).        req.ty
-000114c0: 7065 203d 2072 6571 2e46 4554 4348 5f4d  pe = req.FETCH_M
-000114d0: 4554 4144 4154 410a 0a20 2020 2020 2020  ETADATA..       
-000114e0: 205f 7365 6e64 5f6d 7367 2873 656c 662e   _send_msg(self.
-000114f0: 636f 6e6e 6563 7469 6f6e 2c20 7265 7129  connection, req)
-00011500: 0a0a 2020 2020 2020 2020 7273 7020 3d20  ..        rsp = 
-00011510: 5f72 6563 765f 6d73 6728 7365 6c66 2e63  _recv_msg(self.c
-00011520: 6f6e 6e65 6374 696f 6e2c 2070 726f 746f  onnection, proto
-00011530: 2e46 6574 6368 4d65 7461 6461 7461 5265  .FetchMetadataRe
-00011540: 7370 6f6e 7365 2829 290a 2020 2020 2020  sponse()).      
-00011550: 2020 6966 2072 7370 2e72 6573 706f 6e73    if rsp.respons
-00011560: 652e 7479 7065 203d 3d20 7072 6f74 6f2e  e.type == proto.
-00011570: 436f 6e66 6972 6d61 7469 6f6e 5265 7370  ConfirmationResp
-00011580: 6f6e 7365 2e52 4553 504f 4e53 455f 5741  onse.RESPONSE_WA
-00011590: 524e 3a0a 2020 2020 2020 2020 2020 2020  RN:.            
-000115a0: 7761 726e 2872 7370 2e72 6573 706f 6e73  warn(rsp.respons
-000115b0: 652e 7265 6173 6f6e 290a 2020 2020 2020  e.reason).      
-000115c0: 2020 656c 6966 206e 6f74 2072 7370 2e72    elif not rsp.r
-000115d0: 6573 706f 6e73 652e 7479 7065 203d 3d20  esponse.type == 
-000115e0: 7072 6f74 6f2e 436f 6e66 6972 6d61 7469  proto.Confirmati
-000115f0: 6f6e 5265 7370 6f6e 7365 2e52 4553 504f  onResponse.RESPO
-00011600: 4e53 455f 4f4b 3a0a 2020 2020 2020 2020  NSE_OK:.        
-00011610: 2020 2020 7261 6973 6520 5f63 6f6e 7665      raise _conve
-00011620: 7274 5f65 7863 6570 7469 6f6e 2872 7370  rt_exception(rsp
-00011630: 2e72 6573 706f 6e73 6529 0a0a 2020 2020  .response)..    
-00011640: 2020 2020 636f 6c73 203d 207b 7d0a 2020      cols = {}.  
-00011650: 2020 2020 2020 666f 7220 286b 6579 2c20        for (key, 
-00011660: 7661 6c75 6529 2069 6e20 7273 702e 636f  value) in rsp.co
-00011670: 6c73 3270 6f73 2e69 7465 6d73 2829 3a0a  ls2pos.items():.
-00011680: 2020 2020 2020 2020 2020 2020 636f 6c73              cols
-00011690: 5b76 616c 7565 5d20 3d20 6b65 790a 0a20  [value] = key.. 
-000116a0: 2020 2020 2020 2073 656c 662e 6465 7363         self.desc
-000116b0: 7269 7074 696f 6e20 3d20 5b5d 0a20 2020  ription = [].   
-000116c0: 2020 2020 2063 6f6c 6e61 6d65 7320 3d20       colnames = 
-000116d0: 5b5d 0a20 2020 2020 2020 2066 6f72 2069  [].        for i
-000116e0: 2069 6e20 7261 6e67 6528 6c65 6e28 636f   in range(len(co
-000116f0: 6c73 2929 3a20 2023 2070 796c 696e 743a  ls)):  # pylint:
-00011700: 2064 6973 6162 6c65 3d63 6f6e 7369 6465   disable=conside
-00011710: 722d 7573 696e 672d 656e 756d 6572 6174  r-using-enumerat
-00011720: 650a 2020 2020 2020 2020 2020 2020 6e61  e.            na
-00011730: 6d65 203d 2063 6f6c 735b 695d 0a20 2020  me = cols[i].   
-00011740: 2020 2020 2020 2020 2023 2054 6869 7320           # This 
-00011750: 7475 706c 6520 6973 2064 6566 696e 6564  tuple is defined
-00011760: 2069 6e20 5045 5020 3234 390a 2020 2020   in PEP 249.    
-00011770: 2020 2020 2020 2020 7365 6c66 2e64 6573          self.des
-00011780: 6372 6970 7469 6f6e 2e61 7070 656e 6428  cription.append(
-00011790: 286e 616d 652c 2054 7970 6543 6f64 6573  (name, TypeCodes
-000117a0: 2e74 6f5f 7479 7065 2872 7370 2e63 6f6c  .to_type(rsp.col
-000117b0: 7332 5479 7065 735b 6e61 6d65 5d29 2c20  s2Types[name]), 
-000117c0: 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65  None, None, None
-000117d0: 2c20 4e6f 6e65 2c20 4e6f 6e65 2929 2020  , None, None))  
-000117e0: 2320 6469 7370 6c61 795f 7369 7a65 2020  # display_size  
-000117f0: 2320 696e 7465 726e 616c 5f73 697a 6520  # internal_size 
-00011800: 2023 2070 7265 6369 7369 6f6e 2020 2320   # precision  # 
-00011810: 7363 616c 6520 2023 206e 756c 6c5f 6f6b  scale  # null_ok
-00011820: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
-00011830: 6e61 6d65 732e 6170 7065 6e64 286e 616d  names.append(nam
-00011840: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
-00011850: 7265 7375 6c74 7365 745f 7475 706c 6520  resultset_tuple 
-00011860: 3d20 6e61 6d65 6474 7570 6c65 2822 526f  = namedtuple("Ro
-00011870: 7722 2c20 636f 6c6e 616d 6573 2c20 7265  w", colnames, re
-00011880: 6e61 6d65 3d54 7275 6529 0a0a 2020 2020  name=True)..    
-00011890: 6465 6620 5f65 7865 6375 7465 5f75 7064  def _execute_upd
-000118a0: 6174 6528 7365 6c66 2c20 6f70 6572 6174  ate(self, operat
-000118b0: 696f 6e29 3a0a 2020 2020 2020 2020 2222  ion):.        ""
-000118c0: 2245 7865 6375 7465 2061 6e20 7570 6461  "Execute an upda
-000118d0: 7465 2073 7461 7465 6d65 6e74 2222 220a  te statement""".
-000118e0: 2020 2020 2020 2020 2320 7079 6c69 6e74          # pylint
-000118f0: 3a20 6469 7361 626c 653d 6e6f 2d6d 656d  : disable=no-mem
-00011900: 6265 720a 2020 2020 2020 2020 2320 5768  ber.        # Wh
-00011910: 696c 6520 7765 2061 7265 2072 6564 6972  ile we are redir
-00011920: 6563 7469 6e67 2e2e 2e0a 0a20 2020 2020  ecting.....     
-00011930: 2020 2023 2054 6865 7265 2069 7320 6e6f     # There is no
-00011940: 2072 6573 756c 7473 6574 2064 6174 6120   resultset data 
-00011950: 6672 6f6d 2061 6e20 7570 6461 7465 0a20  from an update. 
-00011960: 2020 2020 2020 2073 656c 662e 656e 645f         self.end_
-00011970: 6f66 5f64 6174 6120 3d20 5472 7565 0a0a  of_data = True..
-00011980: 2020 2020 2020 2020 7768 696c 6520 5472          while Tr
-00011990: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
-000119a0: 7265 7120 3d20 7072 6f74 6f2e 5265 7175  req = proto.Requ
-000119b0: 6573 7428 290a 2020 2020 2020 2020 2020  est().          
-000119c0: 2020 7265 712e 7479 7065 203d 2072 6571    req.type = req
-000119d0: 2e45 5845 4355 5445 5f55 5044 4154 450a  .EXECUTE_UPDATE.
-000119e0: 2020 2020 2020 2020 2020 2020 7265 712e              req.
-000119f0: 6578 6563 7574 655f 7570 6461 7465 2e73  execute_update.s
-00011a00: 716c 203d 206f 7065 7261 7469 6f6e 0a20  ql = operation. 
-00011a10: 2020 2020 2020 2020 2020 2072 6571 2e65             req.e
-00011a20: 7865 6375 7465 5f75 7064 6174 652e 666f  xecute_update.fo
-00011a30: 7263 6520 3d20 7365 6c66 2e63 6f6e 6e65  rce = self.conne
-00011a40: 6374 696f 6e2e 666f 7263 650a 0a20 2020  ction.force..   
-00011a50: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
-00011a60: 2020 2020 2020 2020 2020 2020 2020 5f73                _s
-00011a70: 656e 645f 6d73 6728 7365 6c66 2e63 6f6e  end_msg(self.con
-00011a80: 6e65 6374 696f 6e2c 2072 6571 290a 0a20  nection, req).. 
-00011a90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00011aa0: 7370 203d 205f 7265 6376 5f6d 7367 2873  sp = _recv_msg(s
-00011ab0: 656c 662e 636f 6e6e 6563 7469 6f6e 2c20  elf.connection, 
-00011ac0: 7072 6f74 6f2e 4578 6563 7574 6555 7064  proto.ExecuteUpd
-00011ad0: 6174 6552 6573 706f 6e73 6528 2929 0a20  ateResponse()). 
-00011ae0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-00011af0: 7420 494f 4572 726f 723a 0a20 2020 2020  t IOError:.     
-00011b00: 2020 2020 2020 2020 2020 2023 2072 656d             # rem
-00011b10: 616b 6520 6f75 7220 636f 6e6e 6563 7469  ake our connecti
-00011b20: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
-00011b30: 2020 2073 656c 662e 636f 6e6e 6563 7469     self.connecti
-00011b40: 6f6e 203d 2043 6f6e 6e65 6374 696f 6e28  on = Connection(
-00011b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011b60: 2020 2020 2075 7365 723d 7365 6c66 2e63       user=self.c
-00011b70: 6f6e 6e65 6374 696f 6e2e 7573 6572 2c0a  onnection.user,.
-00011b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b90: 2020 2020 7061 7373 776f 7264 3d73 656c      password=sel
-00011ba0: 662e 636f 6e6e 6563 7469 6f6e 2e70 6173  f.connection.pas
-00011bb0: 7377 6f72 642c 0a20 2020 2020 2020 2020  sword,.         
-00011bc0: 2020 2020 2020 2020 2020 2068 6f73 743d             host=
-00011bd0: 6622 7b27 2c27 2e6a 6f69 6e28 7365 6c66  f"{','.join(self
-00011be0: 2e63 6f6e 6e65 6374 696f 6e2e 686f 7374  .connection.host
-00011bf0: 7329 7d3a 7b73 656c 662e 636f 6e6e 6563  s)}:{self.connec
-00011c00: 7469 6f6e 2e70 6f72 747d 222c 0a20 2020  tion.port}",.   
-00011c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c20: 2064 6174 6162 6173 653d 7365 6c66 2e63   database=self.c
-00011c30: 6f6e 6e65 6374 696f 6e2e 6461 7461 6261  onnection.databa
-00011c40: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-00011c50: 2020 2020 2020 2020 746c 733d 7365 6c66          tls=self
-00011c60: 2e63 6f6e 6e65 6374 696f 6e2e 746c 732c  .connection.tls,
-00011c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011c80: 2020 2020 2068 616e 6473 6861 6b65 3d73       handshake=s
-00011c90: 656c 662e 636f 6e6e 6563 7469 6f6e 2e68  elf.connection.h
-00011ca0: 616e 6473 6861 6b65 2c0a 2020 2020 2020  andshake,.      
-00011cb0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00011cc0: 7263 653d 7365 6c66 2e63 6f6e 6e65 6374  rce=self.connect
-00011cd0: 696f 6e2e 666f 7263 652c 0a20 2020 2020  ion.force,.     
-00011ce0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00011cf0: 6573 7369 6f6e 3d73 656c 662e 636f 6e6e  ession=self.conn
-00011d00: 6563 7469 6f6e 2e73 6573 7369 6f6e 2c0a  ection.session,.
-00011d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d20: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-00011d30: 2020 2063 6f6e 7469 6e75 650a 0a20 2020     continue..   
-00011d40: 2020 2020 2020 2020 2069 6620 7273 702e           if rsp.
-00011d50: 7265 7370 6f6e 7365 2e74 7970 6520 3d3d  response.type ==
-00011d60: 2070 726f 746f 2e43 6f6e 6669 726d 6174   proto.Confirmat
-00011d70: 696f 6e52 6573 706f 6e73 652e 5245 5350  ionResponse.RESP
-00011d80: 4f4e 5345 5f57 4152 4e3a 0a20 2020 2020  ONSE_WARN:.     
-00011d90: 2020 2020 2020 2020 2020 2077 6172 6e28             warn(
-00011da0: 7273 702e 7265 7370 6f6e 7365 2e72 6561  rsp.response.rea
-00011db0: 736f 6e29 0a20 2020 2020 2020 2020 2020  son).           
-00011dc0: 2065 6c69 6620 6e6f 7420 7273 702e 7265   elif not rsp.re
-00011dd0: 7370 6f6e 7365 2e74 7970 6520 3d3d 2070  sponse.type == p
-00011de0: 726f 746f 2e43 6f6e 6669 726d 6174 696f  roto.Confirmatio
-00011df0: 6e52 6573 706f 6e73 652e 5245 5350 4f4e  nResponse.RESPON
-00011e00: 5345 5f4f 4b3a 0a20 2020 2020 2020 2020  SE_OK:.         
-00011e10: 2020 2020 2020 2069 6620 7273 702e 7265         if rsp.re
-00011e20: 7370 6f6e 7365 2e76 656e 646f 725f 636f  sponse.vendor_co
-00011e30: 6465 203d 3d20 5345 5353 494f 4e5f 4558  de == SESSION_EX
-00011e40: 5049 5245 445f 434f 4445 3a0a 2020 2020  PIRED_CODE:.    
-00011e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e60: 2320 4e65 6564 2074 6f20 7265 6672 6573  # Need to refres
-00011e70: 6820 7468 6520 7365 7373 696f 6e0a 2020  h the session.  
-00011e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e90: 2020 7365 6c66 2e63 6f6e 6e65 6374 696f    self.connectio
-00011ea0: 6e2e 7265 6672 6573 6828 290a 2020 2020  n.refresh().    
-00011eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ec0: 2320 616e 6420 7472 7920 6167 6169 6e0a  # and try again.
-00011ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ee0: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
-00011ef0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00011f00: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00011f10: 2020 2020 2020 2072 6169 7365 205f 636f         raise _co
-00011f20: 6e76 6572 745f 6578 6365 7074 696f 6e28  nvert_exception(
-00011f30: 7273 702e 7265 7370 6f6e 7365 290a 0a20  rsp.response).. 
-00011f40: 2020 2020 2020 2020 2020 2023 2073 6565             # see
-00011f50: 2069 6620 7765 2061 7265 2062 6569 6e67   if we are being
-00011f60: 2074 6f6c 6420 746f 2072 6564 6972 6563   told to redirec
-00011f70: 740a 2020 2020 2020 2020 2020 2020 6966  t.            if
-00011f80: 206e 6f74 2072 7370 2e72 6564 6972 6563   not rsp.redirec
-00011f90: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-00011fa0: 2020 2062 7265 616b 0a0a 2020 2020 2020     break..      
-00011fb0: 2020 2020 2020 2320 7265 6d61 6b65 206f        # remake o
-00011fc0: 7572 2063 6f6e 6e65 6374 696f 6e0a 2020  ur connection.  
-00011fd0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00011fe0: 6f6e 6e65 6374 696f 6e20 3d20 7365 6c66  onnection = self
-00011ff0: 2e63 6f6e 6e65 6374 696f 6e2e 7265 6469  .connection.redi
-00012000: 7265 6374 2872 7370 2e72 6564 6972 6563  rect(rsp.redirec
-00012010: 7448 6f73 742c 2072 7370 2e72 6564 6972  tHost, rsp.redir
-00012020: 6563 7450 6f72 7429 0a0a 2020 2020 6465  ectPort)..    de
-00012030: 6620 5f65 7865 6375 7465 5f66 6f72 6365  f _execute_force
-00012040: 2873 656c 662c 206f 7065 7261 7469 6f6e  (self, operation
-00012050: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00012060: 2020 2069 6620 6f70 6572 6174 696f 6e2e     if operation.
-00012070: 7374 7269 7028 292e 7570 7065 7228 2920  strip().upper() 
-00012080: 3d3d 2022 464f 5243 4520 5245 4449 5245  == "FORCE REDIRE
-00012090: 4354 223a 0a20 2020 2020 2020 2020 2020  CT":.           
-000120a0: 2023 2053 6574 7320 7468 6520 6e65 7874   # Sets the next
-000120b0: 2063 6f6d 6d61 6e64 2074 6861 7420 6973   command that is
-000120c0: 2065 7865 6375 7465 2071 7565 7279 2074   execute query t
-000120d0: 6f20 7265 6469 7265 6374 0a20 2020 2020  o redirect.     
-000120e0: 2020 2020 2020 2073 656c 662e 636f 6e6e         self.conn
-000120f0: 6563 7469 6f6e 2e66 6f72 6365 5f6e 6578  ection.force_nex
-00012100: 745f 7265 6469 7265 6374 203d 2054 7275  t_redirect = Tru
-00012110: 650a 2020 2020 2020 2020 2020 2020 7365  e.            se
-00012120: 6c66 2e65 6e64 5f6f 665f 6461 7461 203d  lf.end_of_data =
-00012130: 2054 7275 650a 2020 2020 2020 2020 656c   True.        el
-00012140: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00012150: 2320 466f 7263 6520 6578 7465 726e 616c  # Force external
-00012160: 2063 6f6d 6d61 6e64 0a20 2020 2020 2020   command.       
-00012170: 2020 2020 2073 656c 662e 5f65 7865 6375       self._execu
-00012180: 7465 5f66 6f72 6365 5f65 7874 6572 6e61  te_force_externa
-00012190: 6c28 6f70 6572 6174 696f 6e29 0a0a 2020  l(operation)..  
-000121a0: 2020 6465 6620 5f65 7865 6375 7465 5f66    def _execute_f
-000121b0: 6f72 6365 5f65 7874 6572 6e61 6c28 7365  orce_external(se
-000121c0: 6c66 2c20 6f70 6572 6174 696f 6e29 202d  lf, operation) -
-000121d0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-000121e0: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
-000121f0: 653d 6e6f 2d6d 656d 6265 720a 2020 2020  e=no-member.    
-00012200: 2020 2020 2320 5768 696c 6520 7765 2061      # While we a
-00012210: 7265 2072 6564 6972 6563 7469 6e67 2e2e  re redirecting..
-00012220: 2e0a 2020 2020 2020 2020 6661 6374 6f72  ..        factor
-00012230: 7920 3d20 5f4f 4349 454e 545f 5245 5155  y = _OCIENT_REQU
-00012240: 4553 545f 4641 4354 4f52 4945 535b 2246  EST_FACTORIES["F
-00012250: 4f52 4345 225d 0a20 2020 2020 2020 2072  ORCE"].        r
-00012260: 6571 203d 2066 6163 746f 7279 2e72 6571  eq = factory.req
-00012270: 7565 7374 286f 7065 7261 7469 6f6e 3d6f  uest(operation=o
-00012280: 7065 7261 7469 6f6e 290a 0a20 2020 2020  peration)..     
-00012290: 2020 205f 7365 6e64 5f6d 7367 2873 656c     _send_msg(sel
-000122a0: 662e 636f 6e6e 6563 7469 6f6e 2c20 7265  f.connection, re
-000122b0: 7129 0a0a 2020 2020 2020 2020 7273 7020  q)..        rsp 
-000122c0: 3d20 5f72 6563 765f 6d73 6728 7365 6c66  = _recv_msg(self
-000122d0: 2e63 6f6e 6e65 6374 696f 6e2c 2070 726f  .connection, pro
-000122e0: 746f 2e43 6f6e 6669 726d 6174 696f 6e52  to.ConfirmationR
-000122f0: 6573 706f 6e73 6528 2929 0a0a 2020 2020  esponse())..    
-00012300: 2020 2020 6966 2072 7370 2e74 7970 6520      if rsp.type 
-00012310: 3d3d 2070 726f 746f 2e43 6f6e 6669 726d  == proto.Confirm
-00012320: 6174 696f 6e52 6573 706f 6e73 652e 5245  ationResponse.RE
-00012330: 5350 4f4e 5345 5f57 4152 4e3a 0a20 2020  SPONSE_WARN:.   
-00012340: 2020 2020 2020 2020 2077 6172 6e28 7273           warn(rs
-00012350: 702e 7265 6173 6f6e 290a 2020 2020 2020  p.reason).      
-00012360: 2020 656c 6966 206e 6f74 2072 7370 2e74    elif not rsp.t
-00012370: 7970 6520 3d3d 2070 726f 746f 2e43 6f6e  ype == proto.Con
-00012380: 6669 726d 6174 696f 6e52 6573 706f 6e73  firmationRespons
-00012390: 652e 5245 5350 4f4e 5345 5f4f 4b3a 0a20  e.RESPONSE_OK:. 
-000123a0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000123b0: 205f 636f 6e76 6572 745f 6578 6365 7074   _convert_except
-000123c0: 696f 6e28 7273 7029 0a0a 2020 2020 6465  ion(rsp)..    de
-000123d0: 6620 5f65 7865 6375 7465 5f73 6574 2873  f _execute_set(s
-000123e0: 656c 662c 2070 6172 616d 7329 202d 3e20  elf, params) -> 
-000123f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6966  None:.        if
-00012400: 206c 656e 2870 6172 616d 7329 2021 3d20   len(params) != 
-00012410: 323a 0a20 2020 2020 2020 2020 2020 2072  2:.            r
-00012420: 6169 7365 2050 726f 6772 616d 6d69 6e67  aise Programming
-00012430: 4572 726f 7228 7265 6173 6f6e 3d22 5379  Error(reason="Sy
-00012440: 6e74 6178 2065 7272 6f72 2229 0a0a 2020  ntax error")..  
-00012450: 2020 2020 2020 2320 5468 6572 6520 6973        # There is
-00012460: 206e 6f20 7265 7375 6c74 7365 7420 6461   no resultset da
-00012470: 7461 2066 726f 6d20 616e 2075 7064 6174  ta from an updat
-00012480: 650a 2020 2020 2020 2020 7365 6c66 2e65  e.        self.e
-00012490: 6e64 5f6f 665f 6461 7461 203d 2054 7275  nd_of_data = Tru
-000124a0: 650a 0a20 2020 2020 2020 206f 7020 3d20  e..        op = 
-000124b0: 7061 7261 6d73 5b30 5d2e 7570 7065 7228  params[0].upper(
-000124c0: 290a 2020 2020 2020 2020 7661 6c20 3d20  ).        val = 
-000124d0: 7061 7261 6d73 5b31 5d2e 7374 7269 7028  params[1].strip(
-000124e0: 290a 0a20 2020 2020 2020 2069 6620 6f70  )..        if op
-000124f0: 203d 3d20 2253 4348 454d 4122 3a0a 2020   == "SCHEMA":.  
-00012500: 2020 2020 2020 2020 2020 6661 6374 6f72            factor
-00012510: 7920 3d20 5f4f 4349 454e 545f 5245 5155  y = _OCIENT_REQU
-00012520: 4553 545f 4641 4354 4f52 4945 535b 2253  EST_FACTORIES["S
-00012530: 4554 2053 4348 454d 4122 5d0a 2020 2020  ET SCHEMA"].    
-00012540: 2020 2020 2020 2020 7265 7120 3d20 6661          req = fa
-00012550: 6374 6f72 792e 7265 7175 6573 7428 7661  ctory.request(va
-00012560: 6c29 0a20 2020 2020 2020 2065 6c73 653a  l).        else:
-00012570: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
-00012580: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012590: 2020 7661 6c20 3d20 696e 7428 7661 6c29    val = int(val)
-000125a0: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
-000125b0: 6570 7420 5661 6c75 6545 7272 6f72 3a0a  ept ValueError:.
-000125c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125d0: 7261 6973 6520 5072 6f67 7261 6d6d 696e  raise Programmin
-000125e0: 6745 7272 6f72 2872 6561 736f 6e3d 2253  gError(reason="S
-000125f0: 796e 7461 7820 6572 726f 7220 696e 2053  yntax error in S
-00012600: 4554 2e20 5661 6c75 6520 6d75 7374 2062  ET. Value must b
-00012610: 6520 6e75 6d65 7269 6322 290a 0a20 2020  e numeric")..   
-00012620: 2020 2020 2020 2020 2066 6163 746f 7279           factory
-00012630: 203d 205f 4f43 4945 4e54 5f52 4551 5545   = _OCIENT_REQUE
-00012640: 5354 5f46 4143 544f 5249 4553 5b22 5345  ST_FACTORIES["SE
-00012650: 5422 5d0a 2020 2020 2020 2020 2020 2020  T"].            
-00012660: 7265 7120 3d20 6661 6374 6f72 792e 7265  req = factory.re
-00012670: 7175 6573 7428 6f70 2c20 7661 6c29 0a0a  quest(op, val)..
-00012680: 2020 2020 2020 2020 5f73 656e 645f 6d73          _send_ms
-00012690: 6728 7365 6c66 2e63 6f6e 6e65 6374 696f  g(self.connectio
-000126a0: 6e2c 2072 6571 290a 0a20 2020 2020 2020  n, req)..       
-000126b0: 2072 7370 203d 205f 7265 6376 5f6d 7367   rsp = _recv_msg
-000126c0: 2873 656c 662e 636f 6e6e 6563 7469 6f6e  (self.connection
-000126d0: 2c20 6661 6374 6f72 792e 7265 7370 6f6e  , factory.respon
-000126e0: 7365 2829 290a 0a20 2020 2020 2020 2069  se())..        i
-000126f0: 6620 7273 702e 7479 7065 203d 3d20 7072  f rsp.type == pr
-00012700: 6f74 6f2e 436f 6e66 6972 6d61 7469 6f6e  oto.Confirmation
-00012710: 5265 7370 6f6e 7365 2e52 4553 504f 4e53  Response.RESPONS
-00012720: 455f 5741 524e 3a0a 2020 2020 2020 2020  E_WARN:.        
-00012730: 2020 2020 7761 726e 2872 7370 2e72 6561      warn(rsp.rea
-00012740: 736f 6e29 0a20 2020 2020 2020 2065 6c69  son).        eli
-00012750: 6620 6e6f 7420 7273 702e 7479 7065 203d  f not rsp.type =
-00012760: 3d20 7072 6f74 6f2e 436f 6e66 6972 6d61  = proto.Confirma
-00012770: 7469 6f6e 5265 7370 6f6e 7365 2e52 4553  tionResponse.RES
-00012780: 504f 4e53 455f 4f4b 3a0a 2020 2020 2020  PONSE_OK:.      
-00012790: 2020 2020 2020 6966 2072 7370 2e72 6573        if rsp.res
-000127a0: 706f 6e73 652e 7665 6e64 6f72 5f63 6f64  ponse.vendor_cod
-000127b0: 6520 3d3d 2053 4553 5349 4f4e 5f45 5850  e == SESSION_EXP
-000127c0: 4952 4544 5f43 4f44 453a 0a20 2020 2020  IRED_CODE:.     
-000127d0: 2020 2020 2020 2020 2020 2023 204e 6565             # Nee
-000127e0: 6420 746f 2072 6566 7265 7368 2074 6865  d to refresh the
-000127f0: 2073 6573 7369 6f6e 0a20 2020 2020 2020   session.       
-00012800: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00012810: 6e6e 6563 7469 6f6e 2e72 6566 7265 7368  nnection.refresh
-00012820: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00012830: 2020 2023 2061 6e64 2074 7279 2061 6761     # and try aga
-00012840: 696e 0a20 2020 2020 2020 2020 2020 2020  in.             
-00012850: 2020 2073 656c 662e 5f65 7865 6375 7465     self._execute
-00012860: 5f73 6574 2870 6172 616d 7329 0a20 2020  _set(params).   
-00012870: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00012880: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
-00012890: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000128a0: 2020 2020 2020 7261 6973 6520 5f63 6f6e        raise _con
-000128b0: 7665 7274 5f65 7863 6570 7469 6f6e 2872  vert_exception(r
-000128c0: 7370 290a 0a20 2020 2064 6566 205f 6578  sp)..    def _ex
-000128d0: 6563 7574 655f 6765 745f 7363 6865 6d61  ecute_get_schema
-000128e0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-000128f0: 2020 2020 2020 2020 6661 6374 6f72 7920          factory 
-00012900: 3d20 5f4f 4349 454e 545f 5245 5155 4553  = _OCIENT_REQUES
-00012910: 545f 4641 4354 4f52 4945 535b 2247 4554  T_FACTORIES["GET
-00012920: 2053 4348 454d 4122 5d0a 2020 2020 2020   SCHEMA"].      
-00012930: 2020 7265 7120 3d20 6661 6374 6f72 792e    req = factory.
-00012940: 7265 7175 6573 7428 290a 0a20 2020 2020  request()..     
-00012950: 2020 205f 7365 6e64 5f6d 7367 2873 656c     _send_msg(sel
-00012960: 662e 636f 6e6e 6563 7469 6f6e 2c20 7265  f.connection, re
-00012970: 7129 0a0a 2020 2020 2020 2020 7273 7020  q)..        rsp 
-00012980: 3d20 5f72 6563 765f 6d73 6728 7365 6c66  = _recv_msg(self
-00012990: 2e63 6f6e 6e65 6374 696f 6e2c 2066 6163  .connection, fac
-000129a0: 746f 7279 2e72 6573 706f 6e73 6528 2929  tory.response())
-000129b0: 0a0a 2020 2020 2020 2020 6966 2072 7370  ..        if rsp
-000129c0: 2e72 6573 706f 6e73 652e 7479 7065 203d  .response.type =
-000129d0: 3d20 7072 6f74 6f2e 436f 6e66 6972 6d61  = proto.Confirma
-000129e0: 7469 6f6e 5265 7370 6f6e 7365 2e52 4553  tionResponse.RES
-000129f0: 504f 4e53 455f 5741 524e 3a0a 2020 2020  PONSE_WARN:.    
-00012a00: 2020 2020 2020 2020 7761 726e 2872 7370          warn(rsp
-00012a10: 2e72 6573 706f 6e73 652e 7265 6173 6f6e  .response.reason
-00012a20: 290a 2020 2020 2020 2020 656c 6966 206e  ).        elif n
-00012a30: 6f74 2072 7370 2e72 6573 706f 6e73 652e  ot rsp.response.
-00012a40: 7479 7065 203d 3d20 7072 6f74 6f2e 436f  type == proto.Co
-00012a50: 6e66 6972 6d61 7469 6f6e 5265 7370 6f6e  nfirmationRespon
-00012a60: 7365 2e52 4553 504f 4e53 455f 4f4b 3a0a  se.RESPONSE_OK:.
-00012a70: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-00012a80: 7370 2e72 6573 706f 6e73 652e 7665 6e64  sp.response.vend
-00012a90: 6f72 5f63 6f64 6520 3d3d 2053 4553 5349  or_code == SESSI
-00012aa0: 4f4e 5f45 5850 4952 4544 5f43 4f44 453a  ON_EXPIRED_CODE:
-00012ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012ac0: 2023 204e 6565 6420 746f 2072 6566 7265   # Need to refre
-00012ad0: 7368 2074 6865 2073 6573 7369 6f6e 0a20  sh the session. 
-00012ae0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00012af0: 656c 662e 636f 6e6e 6563 7469 6f6e 2e72  elf.connection.r
-00012b00: 6566 7265 7368 2829 0a20 2020 2020 2020  efresh().       
-00012b10: 2020 2020 2020 2020 2023 2061 6e64 2074           # and t
-00012b20: 7279 2061 6761 696e 0a20 2020 2020 2020  ry again.       
-00012b30: 2020 2020 2020 2020 2073 656c 662e 5f65           self._e
-00012b40: 7865 6375 7465 5f67 6574 5f73 6368 656d  xecute_get_schem
-00012b50: 6128 290a 2020 2020 2020 2020 2020 2020  a().            
-00012b60: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-00012b70: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00012b80: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-00012b90: 7365 205f 636f 6e76 6572 745f 6578 6365  se _convert_exce
-00012ba0: 7074 696f 6e28 7273 702e 7265 7370 6f6e  ption(rsp.respon
-00012bb0: 7365 290a 0a20 2020 2020 2020 2073 656c  se)..        sel
-00012bc0: 662e 6465 7363 7269 7074 696f 6e20 3d20  f.description = 
-00012bd0: 5b28 2273 6368 656d 6122 2c20 5479 7065  [("schema", Type
-00012be0: 436f 6465 732e 4348 4152 2c20 4e6f 6e65  Codes.CHAR, None
-00012bf0: 2c20 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f  , None, None, No
-00012c00: 6e65 2c20 4e6f 6e65 295d 2020 2320 6469  ne, None)]  # di
-00012c10: 7370 6c61 795f 7369 7a65 2020 2320 696e  splay_size  # in
-00012c20: 7465 726e 616c 5f73 697a 6520 2023 2070  ternal_size  # p
-00012c30: 7265 6369 7369 6f6e 2020 2320 7363 616c  recision  # scal
-00012c40: 6520 2023 206e 756c 6c5f 6f6b 0a0a 2020  e  # null_ok..  
-00012c50: 2020 2020 2020 7365 6c66 2e6c 6973 745f        self.list_
-00012c60: 7265 7375 6c74 203d 205b 0a20 2020 2020  result = [.     
-00012c70: 2020 2020 2020 206e 616d 6564 7475 706c         namedtupl
-00012c80: 6528 2252 6f77 222c 2028 2273 6368 656d  e("Row", ("schem
-00012c90: 6122 2929 280a 2020 2020 2020 2020 2020  a"))(.          
-00012ca0: 2020 2020 2020 7273 702e 7363 6865 6d61        rsp.schema
-00012cb0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00012cc0: 2020 2020 2020 2020 5d0a 0a20 2020 2023          ]..    #
-00012cd0: 2049 6620 7765 206e 6565 6420 746f 2069   If we need to i
-00012ce0: 6d70 6c65 6d65 6e74 206d 6f72 6520 6f66  mplement more of
-00012cf0: 2074 6865 7365 2073 6f72 7473 206f 6620   these sorts of 
-00012d00: 6375 7374 6f6d 2063 6f6d 6d61 6e64 732c  custom commands,
-00012d10: 2063 6f6e 7369 6465 720a 2020 2020 2320   consider.    # 
-00012d20: 6d61 6b69 6e67 2061 2066 6163 746f 7279  making a factory
-00012d30: 2066 6f72 2074 6865 2064 6573 6372 6970   for the descrip
-00012d40: 7469 6f6e 2061 6e64 2072 6573 756c 7473  tion and results
-00012d50: 2e0a 2020 2020 6465 6620 5f65 7865 6375  ..    def _execu
-00012d60: 7465 5f67 6574 5f73 6572 7665 725f 7365  te_get_server_se
-00012d70: 7373 696f 6e5f 6964 2873 656c 6629 202d  ssion_id(self) -
-00012d80: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00012d90: 7365 6c66 2e64 6573 6372 6970 7469 6f6e  self.description
-00012da0: 203d 205b 2822 7365 7276 6572 5f73 6573   = [("server_ses
-00012db0: 7369 6f6e 5f69 6422 2c20 5479 7065 436f  sion_id", TypeCo
-00012dc0: 6465 732e 4348 4152 2c20 4e6f 6e65 2c20  des.CHAR, None, 
-00012dd0: 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65  None, None, None
-00012de0: 2c20 4e6f 6e65 295d 2020 2320 6469 7370  , None)]  # disp
-00012df0: 6c61 795f 7369 7a65 2020 2320 696e 7465  lay_size  # inte
-00012e00: 726e 616c 5f73 697a 6520 2023 2070 7265  rnal_size  # pre
-00012e10: 6369 7369 6f6e 2020 2320 7363 616c 6520  cision  # scale 
-00012e20: 2023 206e 756c 6c5f 6f6b 0a20 2020 2020   # null_ok.     
-00012e30: 2020 2073 656c 662e 6c69 7374 5f72 6573     self.list_res
-00012e40: 756c 7420 3d20 5b0a 2020 2020 2020 2020  ult = [.        
-00012e50: 2020 2020 6e61 6d65 6474 7570 6c65 2822      namedtuple("
-00012e60: 526f 7722 2c20 2822 7365 7276 6572 5f73  Row", ("server_s
-00012e70: 6573 7369 6f6e 5f69 6422 2929 280a 2020  ession_id"))(.  
-00012e80: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00012e90: 6c66 2e63 6f6e 6e65 6374 696f 6e2e 7365  lf.connection.se
-00012ea0: 7276 6572 5365 7373 696f 6e49 642c 0a20  rverSessionId,. 
-00012eb0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00012ec0: 2020 2020 205d 0a0a 2020 2020 6465 6620       ]..    def 
-00012ed0: 5f65 7865 6375 7465 5f67 6574 2873 656c  _execute_get(sel
-00012ee0: 662c 2070 6172 616d 7329 202d 3e20 4e6f  f, params) -> No
-00012ef0: 6e65 3a0a 2020 2020 2020 2020 6966 206c  ne:.        if l
-00012f00: 656e 2870 6172 616d 7329 203d 3d20 3120  en(params) == 1 
-00012f10: 616e 6420 7061 7261 6d73 5b30 5d2e 7570  and params[0].up
-00012f20: 7065 7228 2920 3d3d 2022 5343 4845 4d41  per() == "SCHEMA
-00012f30: 223a 0a20 2020 2020 2020 2020 2020 2073  ":.            s
-00012f40: 656c 662e 5f65 7865 6375 7465 5f67 6574  elf._execute_get
-00012f50: 5f73 6368 656d 6128 290a 2020 2020 2020  _schema().      
-00012f60: 2020 656c 6966 206c 656e 2870 6172 616d    elif len(param
-00012f70: 7329 203d 3d20 3320 616e 6420 7061 7261  s) == 3 and para
-00012f80: 6d73 5b30 5d2e 7570 7065 7228 2920 3d3d  ms[0].upper() ==
-00012f90: 2022 5345 5256 4552 2220 616e 6420 7061   "SERVER" and pa
-00012fa0: 7261 6d73 5b31 5d2e 7570 7065 7228 2920  rams[1].upper() 
-00012fb0: 3d3d 2022 5345 5353 494f 4e22 2061 6e64  == "SESSION" and
-00012fc0: 2070 6172 616d 735b 325d 2e75 7070 6572   params[2].upper
-00012fd0: 2829 203d 3d20 2249 4422 3a0a 2020 2020  () == "ID":.    
-00012fe0: 2020 2020 2020 2020 7365 6c66 2e5f 6578          self._ex
-00012ff0: 6563 7574 655f 6765 745f 7365 7276 6572  ecute_get_server
-00013000: 5f73 6573 7369 6f6e 5f69 6428 290a 2020  _session_id().  
-00013010: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00013020: 2020 2020 2020 2020 7261 6973 6520 5072          raise Pr
-00013030: 6f67 7261 6d6d 696e 6745 7272 6f72 2872  ogrammingError(r
-00013040: 6561 736f 6e3d 2253 796e 7461 7820 6572  eason="Syntax er
-00013050: 726f 7222 290a 0a20 2020 2064 6566 205f  ror")..    def _
-00013060: 6578 6563 7574 655f 636c 6561 7228 7365  execute_clear(se
-00013070: 6c66 2c20 7061 7261 6d73 2920 2d3e 204e  lf, params) -> N
-00013080: 6f6e 653a 0a20 2020 2020 2020 2069 6620  one:.        if 
-00013090: 6c65 6e28 7061 7261 6d73 2920 213d 2031  len(params) != 1
-000130a0: 206f 7220 7061 7261 6d73 5b30 5d2e 7570   or params[0].up
-000130b0: 7065 7228 2920 213d 2022 4341 4348 4522  per() != "CACHE"
-000130c0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-000130d0: 6973 6520 5072 6f67 7261 6d6d 696e 6745  ise ProgrammingE
-000130e0: 7272 6f72 2872 6561 736f 6e3d 2253 796e  rror(reason="Syn
-000130f0: 7461 7820 6572 726f 7222 290a 0a20 2020  tax error")..   
-00013100: 2020 2020 2023 2054 6865 7265 2069 7320       # There is 
-00013110: 6e6f 2072 6573 756c 7473 6574 2064 6174  no resultset dat
-00013120: 6120 6672 6f6d 2061 6e20 7570 6461 7465  a from an update
-00013130: 0a20 2020 2020 2020 2073 656c 662e 656e  .        self.en
-00013140: 645f 6f66 5f64 6174 6120 3d20 5472 7565  d_of_data = True
-00013150: 0a0a 2020 2020 2020 2020 6661 6374 6f72  ..        factor
-00013160: 7920 3d20 5f4f 4349 454e 545f 5245 5155  y = _OCIENT_REQU
-00013170: 4553 545f 4641 4354 4f52 4945 535b 2243  EST_FACTORIES["C
-00013180: 4c45 4152 2043 4143 4845 225d 0a20 2020  LEAR CACHE"].   
-00013190: 2020 2020 2072 6571 203d 2066 6163 746f       req = facto
-000131a0: 7279 2e72 6571 7565 7374 2829 0a0a 2020  ry.request()..  
-000131b0: 2020 2020 2020 5f73 656e 645f 6d73 6728        _send_msg(
-000131c0: 7365 6c66 2e63 6f6e 6e65 6374 696f 6e2c  self.connection,
-000131d0: 2072 6571 290a 0a20 2020 2020 2020 2072   req)..        r
-000131e0: 7370 203d 205f 7265 6376 5f6d 7367 2873  sp = _recv_msg(s
-000131f0: 656c 662e 636f 6e6e 6563 7469 6f6e 2c20  elf.connection, 
-00013200: 6661 6374 6f72 792e 7265 7370 6f6e 7365  factory.response
-00013210: 2829 290a 0a20 2020 2020 2020 2069 6620  ())..        if 
-00013220: 7273 702e 7479 7065 203d 3d20 7072 6f74  rsp.type == prot
-00013230: 6f2e 436f 6e66 6972 6d61 7469 6f6e 5265  o.ConfirmationRe
-00013240: 7370 6f6e 7365 2e52 4553 504f 4e53 455f  sponse.RESPONSE_
-00013250: 5741 524e 3a0a 2020 2020 2020 2020 2020  WARN:.          
-00013260: 2020 7761 726e 2872 7370 2e72 6561 736f    warn(rsp.reaso
-00013270: 6e29 0a20 2020 2020 2020 2065 6c69 6620  n).        elif 
-00013280: 6e6f 7420 7273 702e 7479 7065 203d 3d20  not rsp.type == 
-00013290: 7072 6f74 6f2e 436f 6e66 6972 6d61 7469  proto.Confirmati
-000132a0: 6f6e 5265 7370 6f6e 7365 2e52 4553 504f  onResponse.RESPO
-000132b0: 4e53 455f 4f4b 3a0a 2020 2020 2020 2020  NSE_OK:.        
-000132c0: 2020 2020 6966 2072 7370 2e76 656e 646f      if rsp.vendo
-000132d0: 725f 636f 6465 203d 3d20 5345 5353 494f  r_code == SESSIO
-000132e0: 4e5f 4558 5049 5245 445f 434f 4445 3a0a  N_EXPIRED_CODE:.
-000132f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013300: 2320 4e65 6564 2074 6f20 7265 6672 6573  # Need to refres
-00013310: 6820 7468 6520 7365 7373 696f 6e0a 2020  h the session.  
-00013320: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00013330: 6c66 2e63 6f6e 6e65 6374 696f 6e2e 7265  lf.connection.re
-00013340: 6672 6573 6828 290a 2020 2020 2020 2020  fresh().        
-00013350: 2020 2020 2020 2020 2320 616e 6420 7472          # and tr
-00013360: 7920 6167 6169 6e0a 2020 2020 2020 2020  y again.        
-00013370: 2020 2020 2020 2020 7365 6c66 2e5f 6578          self._ex
-00013380: 6563 7574 655f 636c 6561 7228 7061 7261  ecute_clear(para
-00013390: 6d73 290a 2020 2020 2020 2020 2020 2020  ms).            
-000133a0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-000133b0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000133c0: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-000133d0: 7365 205f 636f 6e76 6572 745f 6578 6365  se _convert_exce
-000133e0: 7074 696f 6e28 7273 7029 0a0a 2020 2020  ption(rsp)..    
-000133f0: 6465 6620 5f65 7865 6375 7465 5f63 616e  def _execute_can
-00013400: 6365 6c6b 696c 6c28 7365 6c66 2c20 6f70  celkill(self, op
-00013410: 2c20 6964 2920 2d3e 204e 6f6e 653a 0a20  , id) -> None:. 
-00013420: 2020 2020 2020 2069 6620 6c65 6e28 6964         if len(id
-00013430: 2920 213d 2031 3a0a 2020 2020 2020 2020  ) != 1:.        
-00013440: 2020 2020 7261 6973 6520 5072 6f67 7261      raise Progra
-00013450: 6d6d 696e 6745 7272 6f72 2872 6561 736f  mmingError(reaso
-00013460: 6e3d 2253 796e 7461 7820 6572 726f 7222  n="Syntax error"
-00013470: 290a 0a20 2020 2020 2020 2023 2054 6865  )..        # The
-00013480: 7265 2069 7320 6e6f 2072 6573 756c 7473  re is no results
-00013490: 6574 2064 6174 6120 6672 6f6d 2061 6e20  et data from an 
-000134a0: 7570 6461 7465 0a20 2020 2020 2020 2073  update.        s
-000134b0: 656c 662e 656e 645f 6f66 5f64 6174 6120  elf.end_of_data 
-000134c0: 3d20 5472 7565 0a0a 2020 2020 2020 2020  = True..        
-000134d0: 6661 6374 6f72 7920 3d20 5f4f 4349 454e  factory = _OCIEN
-000134e0: 545f 5245 5155 4553 545f 4641 4354 4f52  T_REQUEST_FACTOR
-000134f0: 4945 535b 6f70 5d0a 2020 2020 2020 2020  IES[op].        
-00013500: 7265 7120 3d20 6661 6374 6f72 792e 7265  req = factory.re
-00013510: 7175 6573 7428 6964 5b30 5d29 0a0a 2020  quest(id[0])..  
-00013520: 2020 2020 2020 5f73 656e 645f 6d73 6728        _send_msg(
-00013530: 7365 6c66 2e63 6f6e 6e65 6374 696f 6e2c  self.connection,
-00013540: 2072 6571 290a 0a20 2020 2020 2020 2072   req)..        r
-00013550: 7370 203d 205f 7265 6376 5f6d 7367 2873  sp = _recv_msg(s
-00013560: 656c 662e 636f 6e6e 6563 7469 6f6e 2c20  elf.connection, 
-00013570: 6661 6374 6f72 792e 7265 7370 6f6e 7365  factory.response
-00013580: 2829 290a 0a20 2020 2020 2020 2069 6620  ())..        if 
-00013590: 7273 702e 7265 7370 6f6e 7365 2e74 7970  rsp.response.typ
-000135a0: 6520 3d3d 2070 726f 746f 2e43 6f6e 6669  e == proto.Confi
-000135b0: 726d 6174 696f 6e52 6573 706f 6e73 652e  rmationResponse.
-000135c0: 5245 5350 4f4e 5345 5f57 4152 4e3a 0a20  RESPONSE_WARN:. 
-000135d0: 2020 2020 2020 2020 2020 2077 6172 6e28             warn(
-000135e0: 7273 702e 7265 7370 6f6e 7365 2e72 6561  rsp.response.rea
-000135f0: 736f 6e29 0a20 2020 2020 2020 2065 6c69  son).        eli
-00013600: 6620 6e6f 7420 7273 702e 7265 7370 6f6e  f not rsp.respon
-00013610: 7365 2e74 7970 6520 3d3d 2070 726f 746f  se.type == proto
-00013620: 2e43 6f6e 6669 726d 6174 696f 6e52 6573  .ConfirmationRes
-00013630: 706f 6e73 652e 5245 5350 4f4e 5345 5f4f  ponse.RESPONSE_O
-00013640: 4b3a 0a20 2020 2020 2020 2020 2020 2069  K:.            i
-00013650: 6620 7273 702e 7265 7370 6f6e 7365 2e76  f rsp.response.v
-00013660: 656e 646f 725f 636f 6465 203d 3d20 5345  endor_code == SE
-00013670: 5353 494f 4e5f 4558 5049 5245 445f 434f  SSION_EXPIRED_CO
-00013680: 4445 3a0a 2020 2020 2020 2020 2020 2020  DE:.            
-00013690: 2020 2020 2320 4e65 6564 2074 6f20 7265      # Need to re
-000136a0: 6672 6573 6820 7468 6520 7365 7373 696f  fresh the sessio
-000136b0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-000136c0: 2020 7365 6c66 2e63 6f6e 6e65 6374 696f    self.connectio
-000136d0: 6e2e 7265 6672 6573 6828 290a 2020 2020  n.refresh().    
-000136e0: 2020 2020 2020 2020 2020 2020 2320 616e              # an
-000136f0: 6420 7472 7920 6167 6169 6e0a 2020 2020  d try again.    
-00013700: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00013710: 2e5f 6578 6563 7574 655f 6361 6e63 656c  ._execute_cancel
-00013720: 6b69 6c6c 286f 702c 2069 6429 0a20 2020  kill(op, id).   
-00013730: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00013740: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
-00013750: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00013760: 2020 2020 2020 7261 6973 6520 5f63 6f6e        raise _con
-00013770: 7665 7274 5f65 7863 6570 7469 6f6e 2872  vert_exception(r
-00013780: 7370 2e72 6573 706f 6e73 6529 0a0a 2020  sp.response)..  
-00013790: 2020 2320 544f 444f 3a20 7265 706c 6163    # TODO: replac
-000137a0: 6520 7468 6520 6f74 6865 7220 6d65 7461  e the other meta
-000137b0: 6461 7461 2063 616c 6c0a 2020 2020 6465  data call.    de
-000137c0: 6620 5f65 7865 6375 7465 5f73 7973 7465  f _execute_syste
-000137d0: 6d6d 6574 6164 6174 6128 7365 6c66 2c20  mmetadata(self, 
-000137e0: 6f70 2c20 7363 6865 6d61 3d4e 6f6e 652c  op, schema=None,
-000137f0: 2074 6162 6c65 3d4e 6f6e 652c 2063 6f6c   table=None, col
-00013800: 756d 6e3d 4e6f 6e65 2c20 7669 6577 3d4e  umn=None, view=N
-00013810: 6f6e 6529 3a0a 2020 2020 2020 2020 6661  one):.        fa
-00013820: 6374 6f72 7920 3d20 5f4f 4349 454e 545f  ctory = _OCIENT_
-00013830: 5245 5155 4553 545f 4641 4354 4f52 4945  REQUEST_FACTORIE
-00013840: 535b 2247 4554 2053 5953 5445 4d20 4d45  S["GET SYSTEM ME
-00013850: 5441 4441 5441 225d 0a20 2020 2020 2020  TADATA"].       
-00013860: 2072 6571 203d 2066 6163 746f 7279 2e72   req = factory.r
-00013870: 6571 7565 7374 286f 702c 2073 6368 656d  equest(op, schem
-00013880: 612c 2074 6162 6c65 2c20 636f 6c75 6d6e  a, table, column
-00013890: 2c20 7669 6577 290a 0a20 2020 2020 2020  , view)..       
-000138a0: 205f 7365 6e64 5f6d 7367 2873 656c 662e   _send_msg(self.
-000138b0: 636f 6e6e 6563 7469 6f6e 2c20 7265 7129  connection, req)
-000138c0: 0a0a 2020 2020 2020 2020 7273 7020 3d20  ..        rsp = 
-000138d0: 5f72 6563 765f 6d73 6728 7365 6c66 2e63  _recv_msg(self.c
-000138e0: 6f6e 6e65 6374 696f 6e2c 2066 6163 746f  onnection, facto
-000138f0: 7279 2e72 6573 706f 6e73 6528 2929 0a0a  ry.response())..
-00013900: 2020 2020 2020 2020 6966 2072 7370 2e72          if rsp.r
-00013910: 6573 706f 6e73 652e 7479 7065 203d 3d20  esponse.type == 
-00013920: 7072 6f74 6f2e 436f 6e66 6972 6d61 7469  proto.Confirmati
-00013930: 6f6e 5265 7370 6f6e 7365 2e52 4553 504f  onResponse.RESPO
-00013940: 4e53 455f 5741 524e 3a0a 2020 2020 2020  NSE_WARN:.      
-00013950: 2020 2020 2020 7761 726e 2872 7370 2e72        warn(rsp.r
-00013960: 6573 706f 6e73 652e 7265 6173 6f6e 290a  esponse.reason).
-00013970: 2020 2020 2020 2020 656c 6966 206e 6f74          elif not
-00013980: 2072 7370 2e72 6573 706f 6e73 652e 7479   rsp.response.ty
-00013990: 7065 203d 3d20 7072 6f74 6f2e 436f 6e66  pe == proto.Conf
-000139a0: 6972 6d61 7469 6f6e 5265 7370 6f6e 7365  irmationResponse
-000139b0: 2e52 4553 504f 4e53 455f 4f4b 3a0a 2020  .RESPONSE_OK:.  
-000139c0: 2020 2020 2020 2020 2020 6966 2072 7370            if rsp
-000139d0: 2e72 6573 706f 6e73 652e 7665 6e64 6f72  .response.vendor
-000139e0: 5f63 6f64 6520 3d3d 2053 4553 5349 4f4e  _code == SESSION
-000139f0: 5f45 5850 4952 4544 5f43 4f44 453a 0a20  _EXPIRED_CODE:. 
-00013a00: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00013a10: 204e 6565 6420 746f 2072 6566 7265 7368   Need to refresh
-00013a20: 2074 6865 2073 6573 7369 6f6e 0a20 2020   the session.   
-00013a30: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00013a40: 662e 636f 6e6e 6563 7469 6f6e 2e72 6566  f.connection.ref
-00013a50: 7265 7368 2829 0a20 2020 2020 2020 2020  resh().         
-00013a60: 2020 2020 2020 2023 2061 6e64 2074 7279         # and try
-00013a70: 2061 6761 696e 0a20 2020 2020 2020 2020   again.         
-00013a80: 2020 2020 2020 2073 656c 662e 5f65 7865         self._exe
-00013a90: 6375 7465 5f73 7973 7465 6d6d 6574 6164  cute_systemmetad
-00013aa0: 6174 6128 6f70 2c20 7363 6865 6d61 3d73  ata(op, schema=s
-00013ab0: 6368 656d 612c 2074 6162 6c65 3d74 6162  chema, table=tab
-00013ac0: 6c65 2c20 636f 6c75 6d6e 3d63 6f6c 756d  le, column=colum
-00013ad0: 6e2c 2076 6965 773d 7669 6577 290a 2020  n, view=view).  
-00013ae0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00013af0: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
-00013b00: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00013b10: 2020 2020 2020 2072 6169 7365 205f 636f         raise _co
-00013b20: 6e76 6572 745f 6578 6365 7074 696f 6e28  nvert_exception(
-00013b30: 7273 702e 7265 7370 6f6e 7365 290a 0a20  rsp.response).. 
-00013b40: 2020 2020 2020 2069 6620 7273 702e 4861         if rsp.Ha
-00013b50: 7346 6965 6c64 2822 7265 7375 6c74 5f73  sField("result_s
-00013b60: 6574 5f76 616c 2229 3a0a 2020 2020 2020  et_val"):.      
-00013b70: 2020 2020 2020 7365 6c66 2e5f 6765 745f        self._get_
-00013b80: 7265 7375 6c74 5f6d 6574 6164 6174 6128  result_metadata(
-00013b90: 290a 0a20 2020 2020 2020 2020 2020 2066  )..            f
-00013ba0: 6f72 2062 6c6f 6220 696e 2072 7370 2e72  or blob in rsp.r
-00013bb0: 6573 756c 745f 7365 745f 7661 6c2e 626c  esult_set_val.bl
-00013bc0: 6f62 733a 0a20 2020 2020 2020 2020 2020  obs:.           
-00013bd0: 2020 2020 2073 656c 662e 5f62 7566 6665       self._buffe
-00013be0: 7273 2e61 7070 656e 6428 626c 6f62 290a  rs.append(blob).
-00013bf0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00013c00: 726e 204e 6f6e 650a 0a20 2020 2020 2020  rn None..       
-00013c10: 2069 6620 7273 702e 4861 7346 6965 6c64   if rsp.HasField
-00013c20: 2822 7374 7269 6e67 5f76 616c 2229 3a0a  ("string_val"):.
-00013c30: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00013c40: 726e 2072 7370 2e73 7472 696e 675f 7661  rn rsp.string_va
-00013c50: 6c0a 0a20 2020 2020 2020 2072 6574 7572  l..        retur
-00013c60: 6e20 7273 702e 696e 745f 7661 6c0a 0a20  n rsp.int_val.. 
-00013c70: 2020 2064 6566 205f 6765 745f 6d6f 7265     def _get_more
-00013c80: 5f64 6174 6128 7365 6c66 293a 0a20 2020  _data(self):.   
-00013c90: 2020 2020 2022 2222 496e 7465 726e 616c       """Internal
-00013ca0: 2072 6f75 7469 6e65 2074 6f20 6765 7420   routine to get 
-00013cb0: 6d6f 7265 2064 6174 6120 6672 6f6d 2061  more data from a
-00013cc0: 2071 7565 7279 2222 220a 2020 2020 2020   query""".      
-00013cd0: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
-00013ce0: 626c 653d 6e6f 2d6d 656d 6265 720a 2020  ble=no-member.  
-00013cf0: 2020 2020 2020 7265 7120 3d20 7072 6f74        req = prot
-00013d00: 6f2e 5265 7175 6573 7428 290a 2020 2020  o.Request().    
-00013d10: 2020 2020 7265 712e 7479 7065 203d 2072      req.type = r
-00013d20: 6571 2e46 4554 4348 5f44 4154 410a 2020  eq.FETCH_DATA.  
-00013d30: 2020 2020 2020 7265 712e 6665 7463 685f        req.fetch_
-00013d40: 6461 7461 2e66 6574 6368 5f73 697a 6520  data.fetch_size 
-00013d50: 3d20 7365 6c66 2e61 7272 6179 7369 7a65  = self.arraysize
-00013d60: 0a20 2020 2020 2020 205f 7365 6e64 5f6d  .        _send_m
-00013d70: 7367 2873 656c 662e 636f 6e6e 6563 7469  sg(self.connecti
-00013d80: 6f6e 2c20 7265 7129 0a0a 2020 2020 2020  on, req)..      
-00013d90: 2020 7273 7020 3d20 5f72 6563 765f 6d73    rsp = _recv_ms
-00013da0: 6728 7365 6c66 2e63 6f6e 6e65 6374 696f  g(self.connectio
-00013db0: 6e2c 2070 726f 746f 2e46 6574 6368 4461  n, proto.FetchDa
-00013dc0: 7461 5265 7370 6f6e 7365 2829 290a 0a20  taResponse()).. 
-00013dd0: 2020 2020 2020 2069 6620 7273 702e 7265         if rsp.re
-00013de0: 7370 6f6e 7365 2e74 7970 6520 3d3d 2070  sponse.type == p
-00013df0: 726f 746f 2e43 6f6e 6669 726d 6174 696f  roto.Confirmatio
-00013e00: 6e52 6573 706f 6e73 652e 5245 5350 4f4e  nResponse.RESPON
-00013e10: 5345 5f45 5252 4f52 3a0a 2020 2020 2020  SE_ERROR:.      
-00013e20: 2020 2020 2020 7261 6973 6520 5f63 6f6e        raise _con
-00013e30: 7665 7274 5f65 7863 6570 7469 6f6e 2872  vert_exception(r
-00013e40: 7370 2e72 6573 706f 6e73 6529 0a0a 2020  sp.response)..  
-00013e50: 2020 2020 2020 666f 7220 626c 6f62 2069        for blob i
-00013e60: 6e20 7273 702e 7265 7375 6c74 5f73 6574  n rsp.result_set
-00013e70: 2e62 6c6f 6273 3a0a 2020 2020 2020 2020  .blobs:.        
-00013e80: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
-00013e90: 5f62 7566 6665 7273 3a0a 2020 2020 2020  _buffers:.      
-00013ea0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00013eb0: 6f66 6673 6574 203d 2030 0a20 2020 2020  offset = 0.     
-00013ec0: 2020 2020 2020 2073 656c 662e 5f62 7566         self._buf
-00013ed0: 6665 7273 2e61 7070 656e 6428 626c 6f62  fers.append(blob
-00013ee0: 290a 0a20 2020 2064 6566 2066 6574 6368  )..    def fetch
-00013ef0: 6d61 6e79 2873 656c 662c 2073 697a 653d  many(self, size=
-00013f00: 4e6f 6e65 293a 0a20 2020 2020 2020 2022  None):.        "
-00013f10: 2222 4665 7463 6820 7468 6520 6e65 7874  ""Fetch the next
-00013f20: 2073 6574 206f 6620 726f 7773 206f 6620   set of rows of 
-00013f30: 6120 7175 6572 7920 7265 7375 6c74 2c20  a query result, 
-00013f40: 7265 7475 726e 696e 6720 6120 7365 7175  returning a sequ
-00013f50: 656e 6365 206f 660a 2020 2020 2020 2020  ence of.        
-00013f60: 7365 7175 656e 6365 7320 2865 2e67 2e20  sequences (e.g. 
-00013f70: 6120 6c69 7374 206f 6620 7475 706c 6573  a list of tuples
-00013f80: 292e 2041 6e20 656d 7074 7920 7365 7175  ). An empty sequ
-00013f90: 656e 6365 2069 7320 7265 7475 726e 6564  ence is returned
-00013fa0: 2077 6865 6e20 6e6f 0a20 2020 2020 2020   when no.       
-00013fb0: 206d 6f72 6520 726f 7773 2061 7265 2061   more rows are a
-00013fc0: 7661 696c 6162 6c65 2e0a 0a20 2020 2020  vailable...     
-00013fd0: 2020 2054 6865 206e 756d 6265 7220 6f66     The number of
-00013fe0: 2072 6f77 7320 746f 2066 6574 6368 2070   rows to fetch p
-00013ff0: 6572 2063 616c 6c20 6973 2073 7065 6369  er call is speci
-00014000: 6669 6564 2062 7920 7468 6520 7061 7261  fied by the para
-00014010: 6d65 7465 722e 2049 6620 6974 0a20 2020  meter. If it.   
-00014020: 2020 2020 2069 7320 6e6f 7420 6769 7665       is not give
-00014030: 6e2c 2074 6865 2063 7572 736f 7227 7320  n, the cursor's 
-00014040: 6172 7261 7973 697a 6520 6465 7465 726d  arraysize determ
-00014050: 696e 6573 2074 6865 206e 756d 6265 7220  ines the number 
-00014060: 6f66 2072 6f77 7320 746f 2062 650a 2020  of rows to be.  
-00014070: 2020 2020 2020 6665 7463 6865 642e 2054        fetched. T
-00014080: 6865 206d 6574 686f 6420 7769 6c6c 2074  he method will t
-00014090: 7279 2074 6f20 6665 7463 6820 6173 206d  ry to fetch as m
-000140a0: 616e 7920 726f 7773 2061 7320 696e 6469  any rows as indi
-000140b0: 6361 7465 6420 6279 2074 6865 2073 697a  cated by the siz
-000140c0: 650a 2020 2020 2020 2020 7061 7261 6d65  e.        parame
-000140d0: 7465 722e 2049 6620 7468 6973 2069 7320  ter. If this is 
-000140e0: 6e6f 7420 706f 7373 6962 6c65 2064 7565  not possible due
-000140f0: 2074 6f20 7468 6520 7370 6563 6966 6965   to the specifie
-00014100: 6420 6e75 6d62 6572 206f 6620 726f 7773  d number of rows
-00014110: 206e 6f74 0a20 2020 2020 2020 2062 6569   not.        bei
-00014120: 6e67 2061 7661 696c 6162 6c65 2c20 6665  ng available, fe
-00014130: 7765 7220 726f 7773 206d 6179 2062 6520  wer rows may be 
-00014140: 7265 7475 726e 6564 2e0a 2020 2020 2020  returned..      
-00014150: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-00014160: 2073 697a 6520 6973 204e 6f6e 653a 0a20   size is None:. 
-00014170: 2020 2020 2020 2020 2020 2073 697a 6520             size 
-00014180: 3d20 7365 6c66 2e61 7272 6179 7369 7a65  = self.arraysize
-00014190: 0a0a 2020 2020 2020 2020 726f 7773 203d  ..        rows =
-000141a0: 205b 5d0a 2020 2020 2020 2020 7768 696c   [].        whil
-000141b0: 6520 7369 7a65 203e 2030 3a0a 2020 2020  e size > 0:.    
-000141c0: 2020 2020 2020 2020 615f 726f 7720 3d20          a_row = 
-000141d0: 7365 6c66 2e66 6574 6368 6f6e 6528 290a  self.fetchone().
-000141e0: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-000141f0: 5f72 6f77 2069 7320 4e6f 6e65 3a0a 2020  _row is None:.  
-00014200: 2020 2020 2020 2020 2020 2020 2020 6272                br
-00014210: 6561 6b0a 2020 2020 2020 2020 2020 2020  eak.            
-00014220: 726f 7773 2e61 7070 656e 6428 615f 726f  rows.append(a_ro
-00014230: 7729 0a20 2020 2020 2020 2020 2020 2073  w).            s
-00014240: 697a 6520 2d3d 2031 0a20 2020 2020 2020  ize -= 1.       
-00014250: 2072 6574 7572 6e20 726f 7773 0a0a 2020   return rows..  
-00014260: 2020 6465 6620 6665 7463 6861 6c6c 2873    def fetchall(s
-00014270: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00014280: 2246 6574 6368 2061 6c6c 2028 7265 6d61  "Fetch all (rema
-00014290: 696e 696e 6729 2072 6f77 7320 6f66 2061  ining) rows of a
-000142a0: 2071 7565 7279 2072 6573 756c 742c 2072   query result, r
-000142b0: 6574 7572 6e69 6e67 2074 6865 6d20 6173  eturning them as
-000142c0: 2061 0a20 2020 2020 2020 2073 6571 7565   a.        seque
-000142d0: 6e63 6520 6f66 2073 6571 7565 6e63 6573  nce of sequences
-000142e0: 2028 652e 672e 2061 206c 6973 7420 6f66   (e.g. a list of
-000142f0: 2074 7570 6c65 7329 2e20 4e6f 7465 2074   tuples). Note t
-00014300: 6861 7420 7468 6520 6375 7273 6f72 2773  hat the cursor's
-00014310: 0a20 2020 2020 2020 2061 7272 6179 7369  .        arraysi
-00014320: 7a65 2061 7474 7269 6275 7465 2063 616e  ze attribute can
-00014330: 2061 6666 6563 7420 7468 6520 7065 7266   affect the perf
-00014340: 6f72 6d61 6e63 6520 6f66 2074 6869 7320  ormance of this 
-00014350: 6f70 6572 6174 696f 6e2e 0a20 2020 2020  operation..     
-00014360: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-00014370: 6574 7572 6e20 7365 6c66 2e66 6574 6368  eturn self.fetch
-00014380: 6d61 6e79 2873 697a 653d 7379 732e 6d61  many(size=sys.ma
-00014390: 7873 697a 6529 0a0a 2020 2020 6465 6620  xsize)..    def 
-000143a0: 5f5f 6e65 7874 5f5f 2873 656c 6629 3a0a  __next__(self):.
-000143b0: 2020 2020 2020 2020 615f 726f 7720 3d20          a_row = 
-000143c0: 7365 6c66 2e66 6574 6368 6f6e 6528 290a  self.fetchone().
-000143d0: 2020 2020 2020 2020 6966 2061 5f72 6f77          if a_row
-000143e0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-000143f0: 2020 2020 2020 7261 6973 6520 5374 6f70        raise Stop
-00014400: 4974 6572 6174 696f 6e0a 2020 2020 2020  Iteration.      
-00014410: 2020 7265 7475 726e 2061 5f72 6f77 0a0a    return a_row..
-00014420: 2020 2020 6465 6620 5f5f 6974 6572 5f5f      def __iter__
-00014430: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00014440: 7265 7475 726e 2073 656c 660a 0a20 2020  return self..   
-00014450: 2064 6566 2066 6574 6368 7661 6c28 7365   def fetchval(se
-00014460: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00014470: 5468 6520 6665 7463 6876 616c 2829 2063  The fetchval() c
-00014480: 6f6e 7665 6e69 656e 6365 206d 6574 686f  onvenience metho
-00014490: 6420 7265 7475 726e 7320 7468 6520 6669  d returns the fi
-000144a0: 7273 7420 636f 6c75 6d6e 206f 6620 7468  rst column of th
-000144b0: 650a 2020 2020 2020 2020 6669 7273 7420  e.        first 
-000144c0: 726f 7720 6966 2074 6865 7265 2061 7265  row if there are
-000144d0: 2072 6573 756c 7473 2c20 6f74 6865 7277   results, otherw
-000144e0: 6973 6520 6974 2072 6574 7572 6e73 204e  ise it returns N
-000144f0: 6f6e 652e 0a20 2020 2020 2020 2022 2222  one..        """
-00014500: 0a20 2020 2020 2020 2061 726f 7720 3d20  .        arow = 
-00014510: 7365 6c66 2e66 6574 6368 6f6e 6528 290a  self.fetchone().
-00014520: 2020 2020 2020 2020 6966 2061 726f 773a          if arow:
-00014530: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00014540: 7572 6e20 6172 6f77 5b30 5d0a 2020 2020  urn arow[0].    
-00014550: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-00014560: 0a20 2020 2064 6566 2066 6574 6368 6f6e  .    def fetchon
-00014570: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00014580: 2022 2222 4665 7463 6820 7468 6520 6e65   """Fetch the ne
-00014590: 7874 2072 6f77 206f 6620 6120 7175 6572  xt row of a quer
-000145a0: 7920 7265 7375 6c74 2073 6574 2c20 7265  y result set, re
-000145b0: 7475 726e 696e 6720 6120 7369 6e67 6c65  turning a single
-000145c0: 2073 6571 7565 6e63 652c 0a20 2020 2020   sequence,.     
-000145d0: 2020 206f 7220 4e6f 6e65 2077 6865 6e20     or None when 
-000145e0: 6e6f 206d 6f72 6520 6461 7461 2069 7320  no more data is 
-000145f0: 6176 6169 6c61 626c 652e 0a20 2020 2020  available..     
-00014600: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
-00014610: 2049 6620 7468 6572 6520 7761 7320 6e65   If there was ne
-00014620: 7665 7220 6120 7175 6572 7920 6578 6563  ver a query exec
-00014630: 7574 6564 2c20 7468 726f 7720 616e 2065  uted, throw an e
-00014640: 7272 6f72 0a20 2020 2020 2020 2069 6620  rror.        if 
-00014650: 7365 6c66 2e64 6573 6372 6970 7469 6f6e  self.description
-00014660: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00014670: 2020 2020 2020 7261 6973 6520 5072 6f67        raise Prog
-00014680: 7261 6d6d 696e 6745 7272 6f72 2822 4e6f  rammingError("No
-00014690: 2072 6573 756c 7420 7365 7420 6176 6169   result set avai
-000146a0: 6c61 626c 6522 290a 0a20 2020 2020 2020  lable")..       
-000146b0: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
-000146c0: 6c65 203d 2074 6f6f 2d6d 616e 792d 6272  le = too-many-br
-000146d0: 616e 6368 6573 0a20 2020 2020 2020 2069  anches.        i
-000146e0: 6620 7365 6c66 2e65 6e64 5f6f 665f 6461  f self.end_of_da
-000146f0: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
-00014700: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
-00014710: 2020 2020 2023 2073 7065 6369 616c 2063       # special c
-00014720: 6173 6520 6578 706c 6169 6e2e 0a20 2020  ase explain..   
-00014730: 2020 2020 2069 6620 7365 6c66 2e65 7870       if self.exp
-00014740: 6c61 696e 5f72 6573 756c 7420 6973 206e  lain_result is n
-00014750: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00014760: 2020 2020 2072 6574 203d 2073 656c 662e       ret = self.
-00014770: 6578 706c 6169 6e5f 7265 7375 6c74 0a20  explain_result. 
-00014780: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00014790: 656e 645f 6f66 5f64 6174 6120 3d20 5472  end_of_data = Tr
-000147a0: 7565 0a20 2020 2020 2020 2020 2020 2072  ue.            r
-000147b0: 6574 7572 6e20 5b72 6574 5d0a 0a20 2020  eturn [ret]..   
-000147c0: 2020 2020 2069 6620 7365 6c66 2e6c 6973       if self.lis
-000147d0: 745f 7265 7375 6c74 2069 7320 6e6f 7420  t_result is not 
-000147e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000147f0: 2020 6966 2073 656c 662e 5f6f 6666 7365    if self._offse
-00014800: 7420 3e3d 206c 656e 2873 656c 662e 6c69  t >= len(self.li
-00014810: 7374 5f72 6573 756c 7429 3a0a 2020 2020  st_result):.    
-00014820: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014830: 2e65 6e64 5f6f 665f 6461 7461 203d 2054  .end_of_data = T
-00014840: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-00014850: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-00014860: 2020 2020 2020 2020 2020 2020 615f 726f              a_ro
-00014870: 7720 3d20 7365 6c66 2e6c 6973 745f 7265  w = self.list_re
-00014880: 7375 6c74 5b73 656c 662e 5f6f 6666 7365  sult[self._offse
-00014890: 745d 0a20 2020 2020 2020 2020 2020 2073  t].            s
-000148a0: 656c 662e 5f6f 6666 7365 7420 2b3d 2031  elf._offset += 1
-000148b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000148c0: 7572 6e20 615f 726f 770a 0a20 2020 2020  urn a_row..     
-000148d0: 2020 2069 6620 7365 6c66 2e72 6f77 636f     if self.rowco
-000148e0: 756e 7420 3c20 303a 0a20 2020 2020 2020  unt < 0:.       
-000148f0: 2020 2020 2073 656c 662e 726f 7763 6f75       self.rowcou
-00014900: 6e74 203d 2030 0a0a 2020 2020 2020 2020  nt = 0..        
-00014910: 7768 696c 6520 6e6f 7420 7365 6c66 2e5f  while not self._
-00014920: 6275 6666 6572 733a 0a20 2020 2020 2020  buffers:.       
-00014930: 2020 2020 2073 656c 662e 5f67 6574 5f6d       self._get_m
-00014940: 6f72 655f 6461 7461 2829 0a20 2020 2020  ore_data().     
-00014950: 2020 2020 2020 2077 6869 6c65 2073 656c         while sel
-00014960: 662e 5f62 7566 6665 7273 2061 6e64 2073  f._buffers and s
-00014970: 656c 662e 5f62 7566 2829 203d 3d20 6222  elf._buf() == b"
-00014980: 5c30 5c30 5c30 5c30 223a 0a20 2020 2020  \0\0\0\0":.     
-00014990: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000149a0: 5f62 7566 6665 7273 2e70 6f70 2830 290a  _buffers.pop(0).
-000149b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000149c0: 6e6f 7420 7365 6c66 2e5f 6275 6666 6572  not self._buffer
-000149d0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-000149e0: 2020 2023 206e 6f20 6461 7461 2079 6574     # no data yet
-000149f0: 2e2e 2e77 6169 7420 736f 2077 6520 646f  ...wait so we do
-00014a00: 6e27 7420 6861 6d6d 6572 2074 6865 2068  n't hammer the h
-00014a10: 6f73 7420 6265 666f 7265 2061 736b 696e  ost before askin
-00014a20: 6720 666f 7220 6d6f 7265 0a20 2020 2020  g for more.     
-00014a30: 2020 2020 2020 2020 2020 2073 6c65 6570             sleep
-00014a40: 2830 2e32 3529 0a0a 2020 2020 2020 2020  (0.25)..        
-00014a50: 6966 2073 656c 662e 5f6f 6666 7365 7420  if self._offset 
-00014a60: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
-00014a70: 2020 7365 6c66 2e5f 6765 745f 6e75 6d5f    self._get_num_
-00014a80: 726f 7773 2829 0a0a 2020 2020 2020 2020  rows()..        
-00014a90: 726f 775f 6c65 6e67 7468 203d 2073 656c  row_length = sel
-00014aa0: 662e 5f67 6574 5f69 6e74 2829 202d 2034  f._get_int() - 4
-00014ab0: 2020 2320 726f 775f 6c65 6e67 7468 2069    # row_length i
-00014ac0: 6e63 6c75 6465 7320 7468 6520 3420 6279  ncludes the 4 by
-00014ad0: 7465 7320 7765 206a 7573 7420 636f 6e73  tes we just cons
-00014ae0: 756d 6564 0a20 2020 2020 2020 2065 6e64  umed.        end
-00014af0: 5f6f 6666 7365 7420 3d20 7365 6c66 2e5f  _offset = self._
-00014b00: 6f66 6673 6574 202b 2072 6f77 5f6c 656e  offset + row_len
-00014b10: 6774 680a 0a20 2020 2020 2020 2069 6620  gth..        if 
-00014b20: 7365 6c66 2e5f 6279 7465 735f 7265 6d61  self._bytes_rema
-00014b30: 696e 696e 6728 2920 3d3d 2031 2061 6e64  ining() == 1 and
-00014b40: 2073 656c 662e 5f62 7566 2829 5b73 656c   self._buf()[sel
-00014b50: 662e 5f6f 6666 7365 745d 203d 3d20 5479  f._offset] == Ty
-00014b60: 7065 436f 6465 732e 4445 4d3a 0a20 2020  peCodes.DEM:.   
-00014b70: 2020 2020 2020 2020 2073 656c 662e 726f           self.ro
-00014b80: 7763 6f75 6e74 202d 3d20 310a 2020 2020  wcount -= 1.    
-00014b90: 2020 2020 2020 2020 7365 6c66 2e5f 6275          self._bu
-00014ba0: 6666 6572 732e 706f 7028 3029 0a20 2020  ffers.pop(0).   
-00014bb0: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
-00014bc0: 6c6f 7365 5f72 6573 756c 7473 6574 2829  lose_resultset()
-00014bd0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00014be0: 7572 6e20 7365 6c66 2e5f 7072 6f63 6573  urn self._proces
-00014bf0: 735f 7065 6e64 696e 6728 290a 0a20 2020  s_pending()..   
-00014c00: 2020 2020 2061 5f72 6f77 203d 205b 5d0a       a_row = [].
-00014c10: 2020 2020 2020 2020 7768 696c 6520 7365          while se
-00014c20: 6c66 2e5f 6f66 6673 6574 203c 2065 6e64  lf._offset < end
-00014c30: 5f6f 6666 7365 743a 0a20 2020 2020 2020  _offset:.       
-00014c40: 2020 2020 2061 5f72 6f77 2e61 7070 656e       a_row.appen
-00014c50: 6428 7365 6c66 2e5f 6465 636f 6465 5f65  d(self._decode_e
-00014c60: 6e74 7279 2829 290a 0a20 2020 2020 2020  ntry())..       
-00014c70: 2069 6620 7365 6c66 2e5f 6f66 6673 6574   if self._offset
-00014c80: 203e 3d20 6c65 6e28 7365 6c66 2e5f 6275   >= len(self._bu
-00014c90: 6628 2929 3a0a 2020 2020 2020 2020 2020  f()):.          
-00014ca0: 2020 7365 6c66 2e5f 6275 6666 6572 732e    self._buffers.
-00014cb0: 706f 7028 3029 0a20 2020 2020 2020 2020  pop(0).         
-00014cc0: 2020 2073 656c 662e 5f6f 6666 7365 7420     self._offset 
-00014cd0: 3d20 300a 2020 2020 2020 2020 7365 6c66  = 0.        self
-00014ce0: 2e72 6f77 6e75 6d62 6572 202b 3d20 310a  .rownumber += 1.
-00014cf0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00014d00: 656c 662e 7265 7375 6c74 7365 745f 7475  elf.resultset_tu
-00014d10: 706c 652e 5f6d 616b 6528 615f 726f 7729  ple._make(a_row)
-00014d20: 0a0a 2020 2020 6465 6620 5f70 726f 6365  ..    def _proce
-00014d30: 7373 5f70 656e 6469 6e67 2873 656c 6629  ss_pending(self)
-00014d40: 3a0a 2020 2020 2020 2020 2320 6966 2077  :.        # if w
-00014d50: 6520 6861 7665 2061 6e79 2070 656e 6469  e have any pendi
-00014d60: 6e67 2071 7565 7269 6573 2074 6f20 6578  ng queries to ex
-00014d70: 6563 7574 652c 206b 6963 6b20 6f6e 6520  ecute, kick one 
-00014d80: 6f66 6620 6e6f 770a 2020 2020 2020 2020  off now.        
-00014d90: 6966 2073 656c 662e 5f70 656e 6469 6e67  if self._pending
-00014da0: 5f6f 7073 3a0a 2020 2020 2020 2020 2020  _ops:.          
-00014db0: 2020 7365 6c66 2e5f 6275 6666 6572 7320    self._buffers 
-00014dc0: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
-00014dd0: 2073 656c 662e 5f6f 6666 7365 7420 3d20   self._offset = 
-00014de0: 300a 2020 2020 2020 2020 2020 2020 7365  0.            se
-00014df0: 6c66 2e5f 6578 6563 7574 655f 696e 7465  lf._execute_inte
-00014e00: 726e 616c 2873 656c 662e 5f70 656e 6469  rnal(self._pendi
-00014e10: 6e67 5f6f 7073 2e70 6f70 2830 2929 0a20  ng_ops.pop(0)). 
-00014e20: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00014e30: 6e20 7365 6c66 2e66 6574 6368 6f6e 6528  n self.fetchone(
-00014e40: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00014e50: 656e 645f 6f66 5f64 6174 6120 3d20 5472  end_of_data = Tr
-00014e60: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
-00014e70: 6e20 4e6f 6e65 0a0a 2020 2020 6465 6620  n None..    def 
-00014e80: 5f62 7566 2873 656c 6629 3a0a 2020 2020  _buf(self):.    
-00014e90: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00014ea0: 5f62 7566 6665 7273 5b30 5d0a 0a20 2020  _buffers[0]..   
-00014eb0: 2064 6566 205f 6279 7465 735f 7265 6d61   def _bytes_rema
-00014ec0: 696e 696e 6728 7365 6c66 293a 0a20 2020  ining(self):.   
-00014ed0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-00014ee0: 2e5f 6275 6666 6572 733a 0a20 2020 2020  ._buffers:.     
-00014ef0: 2020 2020 2020 2072 6574 7572 6e20 300a         return 0.
-00014f00: 2020 2020 2020 2020 7265 7475 726e 206c          return l
-00014f10: 656e 2873 656c 662e 5f62 7566 6665 7273  en(self._buffers
-00014f20: 5b30 5d29 202d 2073 656c 662e 5f6f 6666  [0]) - self._off
-00014f30: 7365 740a 0a20 2020 2064 6566 205f 6765  set..    def _ge
-00014f40: 745f 6e75 6d5f 726f 7773 2873 656c 6629  t_num_rows(self)
-00014f50: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-00014f60: 662e 5f62 7974 6573 5f72 656d 6169 6e69  f._bytes_remaini
-00014f70: 6e67 2829 203e 3d20 343a 0a20 2020 2020  ng() >= 4:.     
-00014f80: 2020 2020 2020 2073 656c 662e 726f 7763         self.rowc
-00014f90: 6f75 6e74 202b 3d20 7365 6c66 2e5f 6765  ount += self._ge
-00014fa0: 745f 696e 7428 290a 0a20 2020 2064 6566  t_int()..    def
-00014fb0: 205f 6465 636f 6465 5f65 6e74 7279 2873   _decode_entry(s
-00014fc0: 656c 6629 3a0a 2020 2020 2020 2020 2320  elf):.        # 
-00014fd0: 7079 6c69 6e74 3a20 6469 7361 626c 653d  pylint: disable=
-00014fe0: 746f 6f2d 6d61 6e79 2d6c 6f63 616c 732c  too-many-locals,
-00014ff0: 746f 6f2d 6d61 6e79 2d72 6574 7572 6e2d  too-many-return-
-00015000: 7374 6174 656d 656e 7473 2c74 6f6f 2d6d  statements,too-m
-00015010: 616e 792d 6272 616e 6368 6573 2c74 6f6f  any-branches,too
-00015020: 2d6d 616e 792d 7374 6174 656d 656e 7473  -many-statements
-00015030: 0a20 2020 2020 2020 2063 6f6c 7479 7065  .        coltype
-00015040: 203d 2073 656c 662e 5f67 6574 5f62 7974   = self._get_byt
-00015050: 6528 290a 0a20 2020 2020 2020 2023 2069  e()..        # i
-00015060: 6620 7468 6973 2069 7320 7468 6520 6561  f this is the ea
-00015070: 7379 2063 6f6e 7665 7273 696f 6e2c 206a  sy conversion, j
-00015080: 7573 7420 646f 2069 740a 2020 2020 2020  ust do it.      
-00015090: 2020 6966 2063 6f6c 7479 7065 2069 6e20    if coltype in 
-000150a0: 5f74 7970 655f 6d61 703a 0a20 2020 2020  _type_map:.     
-000150b0: 2020 2020 2020 2074 6d20 3d20 5f74 7970         tm = _typ
-000150c0: 655f 6d61 705b 636f 6c74 7970 655d 0a20  e_map[coltype]. 
-000150d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000150e0: 6e20 7365 6c66 2e5f 6765 745f 7479 7065  n self._get_type
-000150f0: 2874 6d5b 305d 2c20 746d 5b31 5d29 0a0a  (tm[0], tm[1])..
-00015100: 2020 2020 2020 2020 6966 2063 6f6c 7479          if colty
-00015110: 7065 203d 3d20 5479 7065 436f 6465 732e  pe == TypeCodes.
-00015120: 5354 5249 4e47 3a0a 2020 2020 2020 2020  STRING:.        
-00015130: 2020 2020 7374 726c 656e 203d 2073 656c      strlen = sel
-00015140: 662e 5f67 6574 5f69 6e74 2829 0a20 2020  f._get_int().   
-00015150: 2020 2020 2020 2020 206f 6666 7365 7420           offset 
-00015160: 3d20 7365 6c66 2e5f 6f66 6673 6574 0a20  = self._offset. 
-00015170: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015180: 5f6f 6666 7365 7420 2b3d 2073 7472 6c65  _offset += strle
-00015190: 6e0a 2020 2020 2020 2020 2020 2020 7265  n.            re
-000151a0: 7475 726e 2073 656c 662e 5f62 7566 2829  turn self._buf()
-000151b0: 5b6f 6666 7365 7420 3a20 6f66 6673 6574  [offset : offset
-000151c0: 202b 2073 7472 6c65 6e5d 2e64 6563 6f64   + strlen].decod
-000151d0: 6528 2275 7466 2d38 222c 2065 7272 6f72  e("utf-8", error
-000151e0: 733d 2272 6570 6c61 6365 2229 0a0a 2020  s="replace")..  
-000151f0: 2020 2020 2020 6966 2063 6f6c 7479 7065        if coltype
-00015200: 203d 3d20 5479 7065 436f 6465 732e 5449   == TypeCodes.TI
-00015210: 4d45 5354 414d 503a 0a20 2020 2020 2020  MESTAMP:.       
-00015220: 2020 2020 2072 6574 7572 6e20 6461 7465       return date
-00015230: 7469 6d65 2e64 6174 6574 696d 652e 7574  time.datetime.ut
-00015240: 6366 726f 6d74 696d 6573 7461 6d70 2873  cfromtimestamp(s
-00015250: 656c 662e 5f67 6574 5f6c 6f6e 6728 2929  elf._get_long())
-00015260: 0a0a 2020 2020 2020 2020 6966 2063 6f6c  ..        if col
-00015270: 7479 7065 203d 3d20 5479 7065 436f 6465  type == TypeCode
-00015280: 732e 4e55 4c4c 3a0a 2020 2020 2020 2020  s.NULL:.        
-00015290: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-000152a0: 0a20 2020 2020 2020 2069 6620 636f 6c74  .        if colt
-000152b0: 7970 6520 3d3d 2054 7970 6543 6f64 6573  ype == TypeCodes
-000152c0: 2e42 5954 453a 0a20 2020 2020 2020 2020  .BYTE:.         
-000152d0: 2020 2072 6574 7572 6e20 696e 742e 6672     return int.fr
-000152e0: 6f6d 5f62 7974 6573 2873 656c 662e 5f67  om_bytes(self._g
-000152f0: 6574 5f74 7970 6528 312c 205f 756e 7061  et_type(1, _unpa
-00015300: 636b 5f63 6861 7229 2c20 2262 6967 222c  ck_char), "big",
-00015310: 2073 6967 6e65 643d 5472 7565 290a 0a20   signed=True).. 
-00015320: 2020 2020 2020 2069 6620 636f 6c74 7970         if coltyp
-00015330: 6520 3d3d 2054 7970 6543 6f64 6573 2e54  e == TypeCodes.T
-00015340: 494d 453a 0a20 2020 2020 2020 2020 2020  IME:.           
-00015350: 2073 6563 6f6e 6473 203d 2073 656c 662e   seconds = self.
-00015360: 5f67 6574 5f6c 6f6e 6728 290a 2020 2020  _get_long().    
-00015370: 2020 2020 2020 2020 7365 636f 6e64 203d          second =
-00015380: 2069 6e74 2873 6563 6f6e 6473 2025 2036   int(seconds % 6
-00015390: 3029 0a20 2020 2020 2020 2020 2020 206d  0).            m
-000153a0: 696e 7574 6573 203d 2073 6563 6f6e 6473  inutes = seconds
-000153b0: 202f 2036 300a 2020 2020 2020 2020 2020   / 60.          
-000153c0: 2020 6d69 6e75 7465 203d 2069 6e74 286d    minute = int(m
-000153d0: 696e 7574 6573 2025 2036 3029 0a20 2020  inutes % 60).   
-000153e0: 2020 2020 2020 2020 2068 6f75 7273 203d           hours =
-000153f0: 206d 696e 7574 6573 202f 2036 300a 2020   minutes / 60.  
-00015400: 2020 2020 2020 2020 2020 686f 7572 203d            hour =
-00015410: 2069 6e74 2868 6f75 7273 2025 2032 3429   int(hours % 24)
-00015420: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00015430: 7572 6e20 6461 7465 7469 6d65 2e74 696d  urn datetime.tim
-00015440: 6528 686f 7572 2c20 6d69 6e75 7465 2c20  e(hour, minute, 
-00015450: 7365 636f 6e64 290a 0a20 2020 2020 2020  second)..       
-00015460: 2069 6620 636f 6c74 7970 6520 3d3d 2054   if coltype == T
-00015470: 7970 6543 6f64 6573 2e42 494e 4152 593a  ypeCodes.BINARY:
-00015480: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
-00015490: 6c65 6e20 3d20 7365 6c66 2e5f 6765 745f  len = self._get_
-000154a0: 696e 7428 290a 2020 2020 2020 2020 2020  int().          
-000154b0: 2020 6f66 6673 6574 203d 2073 656c 662e    offset = self.
-000154c0: 5f6f 6666 7365 740a 2020 2020 2020 2020  _offset.        
-000154d0: 2020 2020 7365 6c66 2e5f 6f66 6673 6574      self._offset
-000154e0: 202b 3d20 7374 726c 656e 0a20 2020 2020   += strlen.     
-000154f0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00015500: 6c66 2e5f 6275 6628 295b 6f66 6673 6574  lf._buf()[offset
-00015510: 203a 206f 6666 7365 7420 2b20 7374 726c   : offset + strl
-00015520: 656e 5d0a 0a20 2020 2020 2020 2069 6620  en]..        if 
-00015530: 636f 6c74 7970 6520 3d3d 2054 7970 6543  coltype == TypeC
-00015540: 6f64 6573 2e44 4543 494d 414c 3a0a 2020  odes.DECIMAL:.  
-00015550: 2020 2020 2020 2020 2020 7072 6563 6973            precis
-00015560: 696f 6e20 3d20 7365 6c66 2e5f 6765 745f  ion = self._get_
-00015570: 6279 7465 2829 0a20 2020 2020 2020 2020  byte().         
-00015580: 2020 2073 6361 6c65 203d 2073 656c 662e     scale = self.
-00015590: 5f67 6574 5f62 7974 6528 290a 0a20 2020  _get_byte()..   
-000155a0: 2020 2020 2020 2020 2069 6620 7072 6563           if prec
-000155b0: 6973 696f 6e20 2520 3220 3d3d 2030 3a0a  ision % 2 == 0:.
-000155c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155d0: 7374 726c 656e 203d 2069 6e74 2828 7072  strlen = int((pr
-000155e0: 6563 6973 696f 6e20 2f20 3229 202b 2031  ecision / 2) + 1
-000155f0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-00015600: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00015610: 2020 2020 7374 726c 656e 203d 2069 6e74      strlen = int
-00015620: 2828 7072 6563 6973 696f 6e20 2b20 3129  ((precision + 1)
-00015630: 202f 2032 290a 0a20 2020 2020 2020 2020   / 2)..         
-00015640: 2020 2064 6174 6120 3d20 7365 6c66 2e5f     data = self._
-00015650: 6275 6628 295b 7365 6c66 2e5f 6f66 6673  buf()[self._offs
-00015660: 6574 203a 2028 7365 6c66 2e5f 6f66 6673  et : (self._offs
-00015670: 6574 202b 2073 7472 6c65 6e20 2d20 3129  et + strlen - 1)
-00015680: 5d0a 2020 2020 2020 2020 2020 2020 6469  ].            di
-00015690: 6769 7473 203d 205b 5d0a 2020 2020 2020  gits = [].      
-000156a0: 2020 2020 2020 666f 7220 6279 7465 2069        for byte i
-000156b0: 6e20 6461 7461 3a0a 2020 2020 2020 2020  n data:.        
-000156c0: 2020 2020 2020 2020 6469 6769 7473 2e61          digits.a
-000156d0: 7070 656e 6428 2862 7974 6520 2620 3078  ppend((byte & 0x
-000156e0: 4630 2920 3e3e 2034 290a 2020 2020 2020  F0) >> 4).      
-000156f0: 2020 2020 2020 2020 2020 6469 6769 7473            digits
-00015700: 2e61 7070 656e 6428 6279 7465 2026 2030  .append(byte & 0
-00015710: 7830 4629 0a0a 2020 2020 2020 2020 2020  x0F)..          
-00015720: 2020 7369 676e 203d 2073 656c 662e 5f62    sign = self._b
-00015730: 7566 2829 5b73 656c 662e 5f6f 6666 7365  uf()[self._offse
-00015740: 7420 2b20 7374 726c 656e 202d 2031 5d0a  t + strlen - 1].
-00015750: 0a20 2020 2020 2020 2020 2020 2064 6967  .            dig
-00015760: 6974 732e 6170 7065 6e64 2873 6967 6e20  its.append(sign 
-00015770: 3e3e 2034 290a 2020 2020 2020 2020 2020  >> 4).          
-00015780: 2020 7369 676e 203d 2073 6967 6e20 2620    sign = sign & 
-00015790: 3078 3046 0a0a 2020 2020 2020 2020 2020  0x0F..          
-000157a0: 2020 6966 2073 6967 6e20 3d3d 2031 323a    if sign == 12:
-000157b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000157c0: 2073 6967 6e20 3d20 300a 2020 2020 2020   sign = 0.      
-000157d0: 2020 2020 2020 656c 6966 2073 6967 6e20        elif sign 
-000157e0: 3d3d 2031 333a 0a20 2020 2020 2020 2020  == 13:.         
-000157f0: 2020 2020 2020 2073 6967 6e20 3d20 310a         sign = 1.
-00015800: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00015810: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00015820: 2020 7261 6973 6520 4572 726f 7228 7265    raise Error(re
-00015830: 6173 6f6e 3d66 2255 6e6b 6e6f 776e 2064  ason=f"Unknown d
-00015840: 6563 696d 616c 2073 6967 6e20 7661 6c75  ecimal sign valu
-00015850: 6520 7b73 6967 6e7d 2229 0a0a 2020 2020  e {sign}")..    
-00015860: 2020 2020 2020 2020 7365 6c66 2e5f 6f66          self._of
-00015870: 6673 6574 202b 3d20 7374 726c 656e 0a20  fset += strlen. 
-00015880: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00015890: 6e20 6465 6369 6d61 6c2e 4465 6369 6d61  n decimal.Decima
-000158a0: 6c28 2873 6967 6e2c 2064 6967 6974 732c  l((sign, digits,
-000158b0: 202d 7363 616c 6529 290a 0a20 2020 2020   -scale))..     
-000158c0: 2020 2069 6620 636f 6c74 7970 6520 3d3d     if coltype ==
-000158d0: 2054 7970 6543 6f64 6573 2e41 5252 4159   TypeCodes.ARRAY
-000158e0: 3a0a 2020 2020 2020 2020 2020 2020 6e65  :.            ne
-000158f0: 7374 6564 5f6c 6576 656c 203d 2030 0a0a  sted_level = 0..
-00015900: 2020 2020 2020 2020 2020 2020 6172 7261              arra
-00015910: 7974 7970 6520 3d20 7365 6c66 2e5f 6765  ytype = self._ge
-00015920: 745f 6279 7465 2829 0a0a 2020 2020 2020  t_byte()..      
-00015930: 2020 2020 2020 7768 696c 6520 6172 7261        while arra
-00015940: 7974 7970 6520 3d3d 2054 7970 6543 6f64  ytype == TypeCod
-00015950: 6573 2e41 5252 4159 3a0a 2020 2020 2020  es.ARRAY:.      
-00015960: 2020 2020 2020 2020 2020 6172 7261 7974            arrayt
-00015970: 7970 6520 3d20 7365 6c66 2e5f 6765 745f  ype = self._get_
-00015980: 6279 7465 2829 0a20 2020 2020 2020 2020  byte().         
-00015990: 2020 2020 2020 206e 6573 7465 645f 6c65         nested_le
-000159a0: 7665 6c20 2b3d 2031 0a0a 2020 2020 2020  vel += 1..      
-000159b0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000159c0: 662e 5f67 6574 5f61 7272 6179 286e 6573  f._get_array(nes
-000159d0: 7465 645f 6c65 7665 6c29 0a0a 2020 2020  ted_level)..    
-000159e0: 2020 2020 6966 2063 6f6c 7479 7065 203d      if coltype =
-000159f0: 3d20 5479 7065 436f 6465 732e 5555 4944  = TypeCodes.UUID
-00015a00: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00015a10: 6c66 2e5f 6f66 6673 6574 202b 3d20 3136  lf._offset += 16
-00015a20: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00015a30: 7572 6e20 7575 6964 2e55 5549 4428 6279  urn uuid.UUID(by
-00015a40: 7465 733d 7365 6c66 2e5f 6275 6628 295b  tes=self._buf()[
-00015a50: 7365 6c66 2e5f 6f66 6673 6574 202d 2031  self._offset - 1
-00015a60: 3620 3a20 7365 6c66 2e5f 6f66 6673 6574  6 : self._offset
-00015a70: 5d29 0a0a 2020 2020 2020 2020 6966 2063  ])..        if c
-00015a80: 6f6c 7479 7065 203d 3d20 5479 7065 436f  oltype == TypeCo
-00015a90: 6465 732e 5354 5f50 4f49 4e54 3a0a 2020  des.ST_POINT:.  
-00015aa0: 2020 2020 2020 2020 2020 6c6f 6e67 203d            long =
-00015ab0: 2073 656c 662e 5f67 6574 5f64 6f75 626c   self._get_doubl
-00015ac0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-00015ad0: 6c61 7420 3d20 7365 6c66 2e5f 6765 745f  lat = self._get_
-00015ae0: 646f 7562 6c65 2829 0a20 2020 2020 2020  double().       
-00015af0: 2020 2020 2072 6574 7572 6e20 5f53 5450       return _STP
-00015b00: 6f69 6e74 286c 6f6e 672c 206c 6174 290a  oint(long, lat).
-00015b10: 0a20 2020 2020 2020 2069 6620 636f 6c74  .        if colt
-00015b20: 7970 6520 3d3d 2054 7970 6543 6f64 6573  ype == TypeCodes
-00015b30: 2e44 4154 453a 0a20 2020 2020 2020 2020  .DATE:.         
-00015b40: 2020 2064 203d 2064 6174 6574 696d 652e     d = datetime.
-00015b50: 6461 7465 7469 6d65 2e75 7463 6672 6f6d  datetime.utcfrom
-00015b60: 7469 6d65 7374 616d 7028 7365 6c66 2e5f  timestamp(self._
-00015b70: 6765 745f 6c6f 6e67 2829 202f 2031 3030  get_long() / 100
-00015b80: 302e 3029 0a20 2020 2020 2020 2020 2020  0.0).           
-00015b90: 2072 6574 7572 6e20 6461 7465 7469 6d65   return datetime
-00015ba0: 2e64 6174 6528 642e 7965 6172 2c20 642e  .date(d.year, d.
-00015bb0: 6d6f 6e74 682c 2064 2e64 6179 290a 0a20  month, d.day).. 
-00015bc0: 2020 2020 2020 2069 6620 636f 6c74 7970         if coltyp
-00015bd0: 6520 3d3d 2054 7970 6543 6f64 6573 2e49  e == TypeCodes.I
-00015be0: 503a 0a20 2020 2020 2020 2020 2020 206f  P:.            o
-00015bf0: 6666 203d 2073 656c 662e 5f6f 6666 7365  ff = self._offse
-00015c00: 740a 2020 2020 2020 2020 2020 2020 7365  t.            se
-00015c10: 6c66 2e5f 6f66 6673 6574 202b 3d20 3136  lf._offset += 16
-00015c20: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00015c30: 7572 6e20 6970 6164 6472 6573 732e 6970  urn ipaddress.ip
-00015c40: 5f61 6464 7265 7373 2873 656c 662e 5f62  _address(self._b
-00015c50: 7566 2829 5b6f 6666 203a 206f 6666 202b  uf()[off : off +
-00015c60: 2031 365d 290a 0a20 2020 2020 2020 2069   16])..        i
-00015c70: 6620 636f 6c74 7970 6520 3d3d 2054 7970  f coltype == Typ
-00015c80: 6543 6f64 6573 2e49 5056 343a 0a20 2020  eCodes.IPV4:.   
-00015c90: 2020 2020 2020 2020 206f 6666 203d 2073           off = s
-00015ca0: 656c 662e 5f6f 6666 7365 740a 2020 2020  elf._offset.    
-00015cb0: 2020 2020 2020 2020 7365 6c66 2e5f 6f66          self._of
-00015cc0: 6673 6574 202b 3d20 340a 2020 2020 2020  fset += 4.      
-00015cd0: 2020 2020 2020 7265 7475 726e 2069 7061        return ipa
-00015ce0: 6464 7265 7373 2e69 705f 6164 6472 6573  ddress.ip_addres
-00015cf0: 7328 7365 6c66 2e5f 6275 6628 295b 6f66  s(self._buf()[of
-00015d00: 6620 3a20 6f66 6620 2b20 345d 290a 0a20  f : off + 4]).. 
-00015d10: 2020 2020 2020 2069 6620 636f 6c74 7970         if coltyp
-00015d20: 6520 3d3d 2054 7970 6543 6f64 6573 2e54  e == TypeCodes.T
-00015d30: 494d 4553 5441 4d50 5f4e 414e 4f53 3a0a  IMESTAMP_NANOS:.
-00015d40: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-00015d50: 7374 616d 7020 3d20 7365 6c66 2e5f 6765  stamp = self._ge
-00015d60: 745f 6c6f 6e67 2829 202f 2031 3030 3030  t_long() / 10000
-00015d70: 3030 3030 302e 300a 2020 2020 2020 2020  00000.0.        
-00015d80: 2020 2020 7265 7475 726e 2064 6174 6574      return datet
-00015d90: 696d 652e 6461 7465 7469 6d65 2e75 7463  ime.datetime.utc
-00015da0: 6672 6f6d 7469 6d65 7374 616d 7028 7469  fromtimestamp(ti
-00015db0: 6d65 7374 616d 7029 0a0a 2020 2020 2020  mestamp)..      
-00015dc0: 2020 6966 2063 6f6c 7479 7065 203d 3d20    if coltype == 
-00015dd0: 5479 7065 436f 6465 732e 5449 4d45 5f4e  TypeCodes.TIME_N
-00015de0: 414e 4f53 3a0a 2020 2020 2020 2020 2020  ANOS:.          
-00015df0: 2020 6e61 6e6f 7320 3d20 7365 6c66 2e5f    nanos = self._
-00015e00: 6765 745f 6c6f 6e67 2829 0a20 2020 2020  get_long().     
-00015e10: 2020 2020 2020 206d 6963 726f 7320 3d20         micros = 
-00015e20: 696e 7428 286e 616e 6f73 202f 2031 3030  int((nanos / 100
-00015e30: 3029 2025 2031 3030 3030 3030 290a 2020  0) % 1000000).  
-00015e40: 2020 2020 2020 2020 2020 7365 636f 6e64            second
-00015e50: 7320 3d20 6e61 6e6f 7320 2f20 3130 3030  s = nanos / 1000
-00015e60: 3030 3030 3030 0a20 2020 2020 2020 2020  000000.         
-00015e70: 2020 2073 6563 6f6e 6420 3d20 696e 7428     second = int(
-00015e80: 7365 636f 6e64 7320 2520 3630 290a 2020  seconds % 60).  
-00015e90: 2020 2020 2020 2020 2020 6d69 6e75 7465            minute
-00015ea0: 7320 3d20 7365 636f 6e64 7320 2f20 3630  s = seconds / 60
-00015eb0: 0a20 2020 2020 2020 2020 2020 206d 696e  .            min
-00015ec0: 7574 6520 3d20 696e 7428 6d69 6e75 7465  ute = int(minute
-00015ed0: 7320 2520 3630 290a 2020 2020 2020 2020  s % 60).        
-00015ee0: 2020 2020 686f 7572 7320 3d20 6d69 6e75      hours = minu
-00015ef0: 7465 7320 2f20 3630 0a20 2020 2020 2020  tes / 60.       
-00015f00: 2020 2020 2068 6f75 7220 3d20 696e 7428       hour = int(
-00015f10: 686f 7572 7320 2520 3234 290a 0a20 2020  hours % 24)..   
-00015f20: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00015f30: 6461 7465 7469 6d65 2e74 696d 6528 686f  datetime.time(ho
-00015f40: 7572 2c20 6d69 6e75 7465 2c20 7365 636f  ur, minute, seco
-00015f50: 6e64 2c20 6d69 6372 6f73 290a 0a20 2020  nd, micros)..   
-00015f60: 2020 2020 2069 6620 636f 6c74 7970 6520       if coltype 
-00015f70: 3d3d 2054 7970 6543 6f64 6573 2e54 5550  == TypeCodes.TUP
-00015f80: 4c45 3a0a 2020 2020 2020 2020 2020 2020  LE:.            
-00015f90: 7265 7475 726e 2073 656c 662e 5f67 6574  return self._get
-00015fa0: 5f74 7570 6c65 2829 0a0a 2020 2020 2020  _tuple()..      
-00015fb0: 2020 6966 2063 6f6c 7479 7065 203d 3d20    if coltype == 
-00015fc0: 5479 7065 436f 6465 732e 5354 5f4c 494e  TypeCodes.ST_LIN
-00015fd0: 4553 5452 494e 473a 0a20 2020 2020 2020  ESTRING:.       
-00015fe0: 2020 2020 2070 6f69 6e74 7320 3d20 5b5d       points = []
-00015ff0: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
-00016000: 5f65 6c65 6d65 6e74 7320 3d20 7365 6c66  _elements = self
-00016010: 2e5f 6765 745f 696e 7428 290a 2020 2020  ._get_int().    
-00016020: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00016030: 2072 616e 6765 286e 756d 5f65 6c65 6d65   range(num_eleme
-00016040: 6e74 7329 3a0a 2020 2020 2020 2020 2020  nts):.          
-00016050: 2020 2020 2020 6c6f 6e67 203d 2073 656c        long = sel
-00016060: 662e 5f67 6574 5f64 6f75 626c 6528 290a  f._get_double().
-00016070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016080: 6c61 7420 3d20 7365 6c66 2e5f 6765 745f  lat = self._get_
-00016090: 646f 7562 6c65 2829 0a20 2020 2020 2020  double().       
-000160a0: 2020 2020 2020 2020 2070 6f69 6e74 732e           points.
-000160b0: 6170 7065 6e64 285f 5354 506f 696e 7428  append(_STPoint(
-000160c0: 6c6f 6e67 2c20 6c61 7429 290a 2020 2020  long, lat)).    
-000160d0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-000160e0: 5354 4c69 6e65 7374 7269 6e67 2870 6f69  STLinestring(poi
-000160f0: 6e74 7329 0a0a 2020 2020 2020 2020 6966  nts)..        if
-00016100: 2063 6f6c 7479 7065 203d 3d20 5479 7065   coltype == Type
-00016110: 436f 6465 732e 5354 5f50 4f4c 5947 4f4e  Codes.ST_POLYGON
-00016120: 3a0a 2020 2020 2020 2020 2020 2020 6578  :.            ex
-00016130: 7465 7269 6f72 203d 205b 5d0a 2020 2020  terior = [].    
-00016140: 2020 2020 2020 2020 6e75 6d5f 656c 656d          num_elem
-00016150: 656e 7473 203d 2073 656c 662e 5f67 6574  ents = self._get
-00016160: 5f69 6e74 2829 0a20 2020 2020 2020 2020  _int().         
-00016170: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00016180: 6528 6e75 6d5f 656c 656d 656e 7473 293a  e(num_elements):
-00016190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000161a0: 206c 6f6e 6720 3d20 7365 6c66 2e5f 6765   long = self._ge
-000161b0: 745f 646f 7562 6c65 2829 0a20 2020 2020  t_double().     
-000161c0: 2020 2020 2020 2020 2020 206c 6174 203d             lat =
-000161d0: 2073 656c 662e 5f67 6574 5f64 6f75 626c   self._get_doubl
-000161e0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-000161f0: 2020 2020 6578 7465 7269 6f72 2e61 7070      exterior.app
-00016200: 656e 6428 5f53 5450 6f69 6e74 286c 6f6e  end(_STPoint(lon
-00016210: 672c 206c 6174 2929 0a20 2020 2020 2020  g, lat)).       
-00016220: 2020 2020 2068 6f6c 6573 203d 205b 5d0a       holes = [].
-00016230: 2020 2020 2020 2020 2020 2020 6e75 6d5f              num_
-00016240: 7269 6e67 7320 3d20 7365 6c66 2e5f 6765  rings = self._ge
-00016250: 745f 696e 7428 290a 2020 2020 2020 2020  t_int().        
-00016260: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00016270: 6765 286e 756d 5f72 696e 6773 293a 0a20  ge(num_rings):. 
-00016280: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00016290: 756d 5f65 6c65 6d65 6e74 7320 3d20 7365  um_elements = se
-000162a0: 6c66 2e5f 6765 745f 696e 7428 290a 2020  lf._get_int().  
-000162b0: 2020 2020 2020 2020 2020 2020 2020 7269                ri
-000162c0: 6e67 203d 205b 5d0a 2020 2020 2020 2020  ng = [].        
-000162d0: 2020 2020 2020 2020 666f 7220 6a20 696e          for j in
-000162e0: 2072 616e 6765 286e 756d 5f65 6c65 6d65   range(num_eleme
-000162f0: 6e74 7329 3a0a 2020 2020 2020 2020 2020  nts):.          
-00016300: 2020 2020 2020 2020 2020 6c6f 6e67 203d            long =
-00016310: 2073 656c 662e 5f67 6574 5f64 6f75 626c   self._get_doubl
-00016320: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-00016330: 2020 2020 2020 2020 6c61 7420 3d20 7365          lat = se
-00016340: 6c66 2e5f 6765 745f 646f 7562 6c65 2829  lf._get_double()
-00016350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016360: 2020 2020 2072 696e 672e 6170 7065 6e64       ring.append
-00016370: 285f 5354 506f 696e 7428 6c6f 6e67 2c20  (_STPoint(long, 
-00016380: 6c61 7429 290a 2020 2020 2020 2020 2020  lat)).          
-00016390: 2020 2020 2020 686f 6c65 732e 6170 7065        holes.appe
-000163a0: 6e64 2872 696e 6729 0a20 2020 2020 2020  nd(ring).       
-000163b0: 2020 2020 2072 6574 7572 6e20 5f53 5450       return _STP
-000163c0: 6f6c 7967 6f6e 2865 7874 6572 696f 722c  olygon(exterior,
-000163d0: 2068 6f6c 6573 290a 0a20 2020 2020 2020   holes)..       
-000163e0: 2073 656c 662e 656e 645f 6f66 5f64 6174   self.end_of_dat
-000163f0: 6120 3d20 5472 7565 0a20 2020 2020 2020  a = True.       
-00016400: 2072 6169 7365 2045 7272 6f72 2872 6561   raise Error(rea
-00016410: 736f 6e3d 6622 556e 6b6e 6f77 6e20 636f  son=f"Unknown co
-00016420: 6c75 6d6e 2074 7970 6520 7b63 6f6c 7479  lumn type {colty
-00016430: 7065 7d22 290a 0a20 2020 2064 6566 205f  pe}")..    def _
-00016440: 6765 745f 6279 7465 2873 656c 6629 3a0a  get_byte(self):.
-00016450: 2020 2020 2020 2020 6f66 6673 6574 203d          offset =
-00016460: 2073 656c 662e 5f6f 6666 7365 740a 2020   self._offset.  
-00016470: 2020 2020 2020 7365 6c66 2e5f 6f66 6673        self._offs
-00016480: 6574 202b 3d20 310a 2020 2020 2020 2020  et += 1.        
-00016490: 7265 7475 726e 2073 656c 662e 5f62 7566  return self._buf
-000164a0: 2829 5b6f 6666 7365 745d 0a0a 2020 2020  ()[offset]..    
-000164b0: 6465 6620 5f67 6574 5f69 6e74 2873 656c  def _get_int(sel
-000164c0: 6629 3a0a 2020 2020 2020 2020 6f66 6673  f):.        offs
-000164d0: 6574 203d 2073 656c 662e 5f6f 6666 7365  et = self._offse
-000164e0: 740a 2020 2020 2020 2020 7365 6c66 2e5f  t.        self._
-000164f0: 6f66 6673 6574 202b 3d20 340a 2020 2020  offset += 4.    
-00016500: 2020 2020 7265 7475 726e 205f 756e 7061      return _unpa
-00016510: 636b 5f69 6e74 2873 656c 662e 5f62 7566  ck_int(self._buf
-00016520: 2829 2c20 6f66 6673 6574 295b 305d 0a0a  (), offset)[0]..
-00016530: 2020 2020 6465 6620 5f67 6574 5f6c 6f6e      def _get_lon
-00016540: 6728 7365 6c66 293a 0a20 2020 2020 2020  g(self):.       
-00016550: 206f 6666 7365 7420 3d20 7365 6c66 2e5f   offset = self._
-00016560: 6f66 6673 6574 0a20 2020 2020 2020 2073  offset.        s
-00016570: 656c 662e 5f6f 6666 7365 7420 2b3d 2038  elf._offset += 8
-00016580: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00016590: 5f75 6e70 6163 6b5f 6c6f 6e67 2873 656c  _unpack_long(sel
-000165a0: 662e 5f62 7566 2829 2c20 6f66 6673 6574  f._buf(), offset
-000165b0: 295b 305d 0a0a 2020 2020 6465 6620 5f67  )[0]..    def _g
-000165c0: 6574 5f64 6f75 626c 6528 7365 6c66 293a  et_double(self):
-000165d0: 0a20 2020 2020 2020 206f 6666 7365 7420  .        offset 
-000165e0: 3d20 7365 6c66 2e5f 6f66 6673 6574 0a20  = self._offset. 
-000165f0: 2020 2020 2020 2073 656c 662e 5f6f 6666         self._off
-00016600: 7365 7420 2b3d 2038 0a20 2020 2020 2020  set += 8.       
-00016610: 2072 6574 7572 6e20 5f75 6e70 6163 6b5f   return _unpack_
-00016620: 646f 7562 6c65 2873 656c 662e 5f62 7566  double(self._buf
-00016630: 2829 2c20 6f66 6673 6574 295b 305d 0a0a  (), offset)[0]..
-00016640: 2020 2020 6465 6620 5f67 6574 5f74 7970      def _get_typ
-00016650: 6528 7365 6c66 2c20 6461 7461 6c65 6e2c  e(self, datalen,
-00016660: 2075 6e70 6163 6b65 7229 3a0a 2020 2020   unpacker):.    
-00016670: 2020 2020 6f66 6673 6574 203d 2073 656c      offset = sel
-00016680: 662e 5f6f 6666 7365 740a 2020 2020 2020  f._offset.      
-00016690: 2020 7365 6c66 2e5f 6f66 6673 6574 202b    self._offset +
-000166a0: 3d20 6461 7461 6c65 6e0a 2020 2020 2020  = datalen.      
-000166b0: 2020 7265 7475 726e 2075 6e70 6163 6b65    return unpacke
-000166c0: 7228 7365 6c66 2e5f 6275 6628 292c 206f  r(self._buf(), o
-000166d0: 6666 7365 7429 5b30 5d0a 0a20 2020 2064  ffset)[0]..    d
-000166e0: 6566 205f 6765 745f 6172 7261 7928 7365  ef _get_array(se
-000166f0: 6c66 2c20 6c65 7665 6c29 3a0a 2020 2020  lf, level):.    
-00016700: 2020 2020 6172 7261 7920 3d20 5b5d 0a0a      array = []..
-00016710: 2020 2020 2020 2020 6e75 6d5f 656c 656d          num_elem
-00016720: 656e 7473 203d 2073 656c 662e 5f67 6574  ents = self._get
-00016730: 5f69 6e74 2829 0a0a 2020 2020 2020 2020  _int()..        
-00016740: 616c 6c5f 6e75 6c6c 203d 2073 656c 662e  all_null = self.
-00016750: 5f67 6574 5f62 7974 6528 290a 0a20 2020  _get_byte()..   
-00016760: 2020 2020 2069 6620 616c 6c5f 6e75 6c6c       if all_null
-00016770: 2021 3d20 303a 0a20 2020 2020 2020 2020   != 0:.         
-00016780: 2020 2072 6574 7572 6e20 5b5d 0a0a 2020     return []..  
-00016790: 2020 2020 2020 666f 7220 5f20 696e 2072        for _ in r
-000167a0: 616e 6765 286e 756d 5f65 6c65 6d65 6e74  ange(num_element
-000167b0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-000167c0: 6966 206c 6576 656c 203e 2030 3a0a 2020  if level > 0:.  
-000167d0: 2020 2020 2020 2020 2020 2020 2020 6172                ar
-000167e0: 7261 792e 6170 7065 6e64 2873 656c 662e  ray.append(self.
-000167f0: 5f67 6574 5f61 7272 6179 286c 6576 656c  _get_array(level
-00016800: 202d 2031 2929 0a20 2020 2020 2020 2020   - 1)).         
-00016810: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00016820: 2020 2020 2020 2020 2061 7272 6179 2e61           array.a
-00016830: 7070 656e 6428 7365 6c66 2e5f 6465 636f  ppend(self._deco
-00016840: 6465 5f65 6e74 7279 2829 290a 0a20 2020  de_entry())..   
-00016850: 2020 2020 2072 6574 7572 6e20 6172 7261       return arra
-00016860: 790a 0a20 2020 2064 6566 205f 636c 6f73  y..    def _clos
-00016870: 655f 7265 7375 6c74 7365 7428 7365 6c66  e_resultset(self
-00016880: 293a 0a20 2020 2020 2020 2072 6571 203d  ):.        req =
-00016890: 2070 726f 746f 2e52 6571 7565 7374 2829   proto.Request()
-000168a0: 0a20 2020 2020 2020 2072 6571 2e74 7970  .        req.typ
-000168b0: 6520 3d20 7072 6f74 6f2e 5265 7175 6573  e = proto.Reques
-000168c0: 742e 5265 7175 6573 7454 7970 652e 5661  t.RequestType.Va
-000168d0: 6c75 6528 2243 4c4f 5345 5f52 4553 554c  lue("CLOSE_RESUL
-000168e0: 545f 5345 5422 290a 0a20 2020 2020 2020  T_SET")..       
-000168f0: 205f 7365 6e64 5f6d 7367 2873 656c 662e   _send_msg(self.
-00016900: 636f 6e6e 6563 7469 6f6e 2c20 7265 7129  connection, req)
-00016910: 0a0a 2020 2020 2020 2020 7273 7020 3d20  ..        rsp = 
-00016920: 5f72 6563 765f 6d73 6728 7365 6c66 2e63  _recv_msg(self.c
-00016930: 6f6e 6e65 6374 696f 6e2c 2070 726f 746f  onnection, proto
-00016940: 2e43 6f6e 6669 726d 6174 696f 6e52 6573  .ConfirmationRes
-00016950: 706f 6e73 6528 2929 0a0a 2020 2020 2020  ponse())..      
-00016960: 2020 6966 2072 7370 2e74 7970 6520 3d3d    if rsp.type ==
-00016970: 2070 726f 746f 2e43 6f6e 6669 726d 6174   proto.Confirmat
-00016980: 696f 6e52 6573 706f 6e73 652e 5245 5350  ionResponse.RESP
-00016990: 4f4e 5345 5f57 4152 4e3a 0a20 2020 2020  ONSE_WARN:.     
-000169a0: 2020 2020 2020 2077 6172 6e28 7273 702e         warn(rsp.
-000169b0: 7265 6173 6f6e 290a 2020 2020 2020 2020  reason).        
-000169c0: 656c 6966 206e 6f74 2072 7370 2e74 7970  elif not rsp.typ
-000169d0: 6520 3d3d 2070 726f 746f 2e43 6f6e 6669  e == proto.Confi
-000169e0: 726d 6174 696f 6e52 6573 706f 6e73 652e  rmationResponse.
-000169f0: 5245 5350 4f4e 5345 5f4f 4b3a 0a20 2020  RESPONSE_OK:.   
-00016a00: 2020 2020 2020 2020 2072 6169 7365 205f           raise _
-00016a10: 636f 6e76 6572 745f 6578 6365 7074 696f  convert_exceptio
-00016a20: 6e28 7273 7029 0a0a 2020 2020 6465 6620  n(rsp)..    def 
-00016a30: 5f67 6574 5f74 7570 6c65 2873 656c 6629  _get_tuple(self)
-00016a40: 3a0a 2020 2020 2020 2020 6e75 6d5f 656c  :.        num_el
-00016a50: 656d 656e 7473 203d 2073 656c 662e 5f67  ements = self._g
-00016a60: 6574 5f69 6e74 2829 0a20 2020 2020 2020  et_int().       
-00016a70: 2072 6573 7475 706c 6520 3d20 2829 0a20   restuple = (). 
-00016a80: 2020 2020 2020 2066 6f72 205f 2069 6e20         for _ in 
-00016a90: 7261 6e67 6528 6e75 6d5f 656c 656d 656e  range(num_elemen
-00016aa0: 7473 293a 0a20 2020 2020 2020 2020 2020  ts):.           
-00016ab0: 2072 6573 7475 706c 6520 2b3d 2028 7365   restuple += (se
-00016ac0: 6c66 2e5f 6465 636f 6465 5f65 6e74 7279  lf._decode_entry
-00016ad0: 2829 2c29 0a20 2020 2020 2020 2072 6574  (),).        ret
-00016ae0: 7572 6e20 7265 7374 7570 6c65 0a0a 0a64  urn restuple...d
-00016af0: 6566 2063 6f6e 6e65 6374 2864 736e 3d4e  ef connect(dsn=N
-00016b00: 6f6e 652c 2075 7365 723d 4e6f 6e65 2c20  one, user=None, 
-00016b10: 7061 7373 776f 7264 3d4e 6f6e 652c 2068  password=None, h
-00016b20: 6f73 743d 4e6f 6e65 2c20 6461 7461 6261  ost=None, databa
-00016b30: 7365 3d4e 6f6e 652c 2074 6c73 3d4e 6f6e  se=None, tls=Non
-00016b40: 652c 2066 6f72 6365 3d4e 6f6e 652c 2068  e, force=None, h
-00016b50: 616e 6473 6861 6b65 3d22 6763 6d22 2c20  andshake="gcm", 
-00016b60: 636f 6e66 6967 6669 6c65 3d4e 6f6e 6529  configfile=None)
-00016b70: 3a0a 2020 2020 2320 7079 6c69 6e74 3a20  :.    # pylint: 
-00016b80: 6469 7361 626c 653d 746f 6f2d 6d61 6e79  disable=too-many
-00016b90: 2d61 7267 756d 656e 7473 0a20 2020 2022  -arguments.    "
-00016ba0: 2222 4372 6561 7465 2061 206e 6577 2064  ""Create a new d
-00016bb0: 6174 6162 6173 6520 636f 6e6e 6563 7469  atabase connecti
-00016bc0: 6f6e 2e0a 0a20 2020 2054 6865 2063 6f6e  on...    The con
-00016bd0: 6e65 6374 696f 6e20 7061 7261 6d65 7465  nection paramete
-00016be0: 7273 2063 616e 2062 6520 7370 6563 6966  rs can be specif
-00016bf0: 6965 6420 6173 2070 6172 7420 6f66 2074  ied as part of t
-00016c00: 6865 2064 736e 2c0a 2020 2020 7573 696e  he dsn,.    usin
-00016c10: 6720 6b65 7977 6f72 6420 6172 6775 6d65  g keyword argume
-00016c20: 6e74 7320 6f72 2062 6f74 682e 2020 4966  nts or both.  If
-00016c30: 2062 6f74 6820 6172 6520 7370 6563 6966   both are specif
-00016c40: 6965 642c 2074 6865 206b 6579 776f 7264  ied, the keyword
-00016c50: 0a20 2020 2070 6172 616d 6574 6572 206f  .    parameter o
-00016c60: 7665 7272 6964 6573 2074 6865 2076 616c  verrides the val
-00016c70: 7565 2069 6e20 7468 6520 6473 6e2e 0a0a  ue in the dsn...
-00016c80: 2020 2020 5468 6520 4f63 6965 6e74 2044      The Ocient D
-00016c90: 534e 2069 7320 6f66 2074 6865 2066 6f72  SN is of the for
-00016ca0: 6d61 743a 0a20 2020 2060 6f63 6965 6e74  mat:.    `ocient
-00016cb0: 3a2f 2f75 7365 723a 7061 7373 776f 7264  ://user:password
-00016cc0: 405b 686f 7374 5d5b 3a70 6f72 745d 5b2f  @[host][:port][/
-00016cd0: 6461 7461 6261 7365 5d5b 3f70 6172 616d  database][?param
-00016ce0: 313d 7661 6c75 6531 262e 2e2e 5d60 0a0a  1=value1&...]`..
-00016cf0: 2020 2020 6075 7365 7260 2061 6e64 2060      `user` and `
-00016d00: 7061 7373 776f 7264 6020 6d75 7374 2062  password` must b
-00016d10: 6520 7375 7070 6c69 6564 2e20 2060 686f  e supplied.  `ho
-00016d20: 7374 6020 6465 6661 756c 7473 2074 6f20  st` defaults to 
-00016d30: 6c6f 6361 6c68 6f73 742c 0a20 2020 2070  localhost,.    p
-00016d40: 6f72 7420 6465 6661 756c 7473 2074 6f20  ort defaults to 
-00016d50: 3430 3530 2c20 6461 7461 6261 7365 2064  4050, database d
-00016d60: 6566 6175 6c74 7320 746f 2060 7379 7374  efaults to `syst
-00016d70: 656d 6020 616e 6420 6074 6c73 6020 6465  em` and `tls` de
-00016d80: 6661 756c 7473 0a20 2020 2074 6f20 6075  faults.    to `u
-00016d90: 6e76 6572 6966 6965 6460 2e0a 0a20 2020  nverified`...   
-00016da0: 204d 756c 7469 706c 6520 686f 7374 7320   Multiple hosts 
-00016db0: 6d61 7920 6265 2073 7065 6369 6669 6564  may be specified
-00016dc0: 2c20 7365 7061 7261 7465 6420 6279 2061  , separated by a
-00016dd0: 2063 6f6d 6d61 2c20 696e 2077 6869 6368   comma, in which
-00016de0: 2063 6173 6520 7468 650a 2020 2020 686f   case the.    ho
-00016df0: 7374 7320 7769 6c6c 2062 6520 7472 6965  sts will be trie
-00016e00: 6420 696e 206f 7264 6572 2020 5468 7573  d in order  Thus
-00016e10: 2061 6e20 6578 616d 706c 6520 4453 4e20   an example DSN 
-00016e20: 6d69 6768 7420 6265 0a20 2020 2060 6f63  might be.    `oc
-00016e30: 6965 6e74 3a2f 2f73 6f6d 656f 6e65 3a73  ient://someone:s
-00016e40: 6f6d 6570 6173 7377 6f72 6440 686f 7374  omepassword@host
-00016e50: 312c 686f 7374 323a 3430 3531 2f6d 7964  1,host2:4051/myd
-00016e60: 6260 0a0a 2020 2020 636f 6e66 6967 6669  b`..    configfi
-00016e70: 6c65 2073 7065 6369 6669 6573 2074 6865  le specifies the
-00016e80: 206e 616d 6520 6f66 2061 2063 6f6e 6669   name of a confi
-00016e90: 6775 7261 7469 6f6e 2066 696c 6520 696e  guration file in
-00016ea0: 2049 4e49 2066 6f72 6d61 742e 2053 6565   INI format. See
-00016eb0: 0a20 2020 2074 6865 2043 6f6e 6e65 6374  .    the Connect
-00016ec0: 696f 6e20 636c 6173 7320 666f 7220 6d6f  ion class for mo
-00016ed0: 7265 2064 6574 6169 6c65 6420 646f 6375  re detailed docu
-00016ee0: 6d65 6e74 6174 696f 6e2e 0a0a 2020 2020  mentation...    
-00016ef0: 4375 7272 656e 746c 7920 7375 7070 6f72  Currently suppor
-00016f00: 7465 6420 7061 7261 6d65 7465 7273 2061  ted parameters a
-00016f10: 7265 3a0a 0a20 2020 202d 2074 6c73 3a20  re:..    - tls: 
-00016f20: 5768 6963 6820 6361 6e20 6861 7665 2074  Which can have t
-00016f30: 6865 2076 616c 7565 7320 226f 6666 222c  he values "off",
-00016f40: 2022 756e 7665 7269 6669 6564 222c 206f   "unverified", o
-00016f50: 7220 226f 6e22 2069 6e20 7468 6520 6473  r "on" in the ds
-00016f60: 6e2c 0a20 2020 2020 2020 2020 6f72 2043  n,.         or C
-00016f70: 6f6e 6e65 6374 696f 6e2e 544c 535f 4e4f  onnection.TLS_NO
-00016f80: 4e45 2c20 436f 6e6e 6563 7469 6f6e 2e54  NE, Connection.T
-00016f90: 4c53 5f55 4e56 4552 4946 4945 442c 206f  LS_UNVERIFIED, o
-00016fa0: 720a 2020 2020 2020 2020 2043 6f6e 6e65  r.         Conne
-00016fb0: 6374 696f 6e2e 544c 535f 4f4e 2061 7320  ction.TLS_ON as 
-00016fc0: 6120 6b65 7977 6f72 6420 7061 7261 6d65  a keyword parame
-00016fd0: 7465 722e 0a20 2020 202d 2068 616e 6473  ter..    - hands
-00016fe0: 6861 6b65 3a20 2243 4243 222c 2022 4743  hake: "CBC", "GC
-00016ff0: 4d22 2c20 6f72 2022 5353 4f22 2e20 2247  M", or "SSO". "G
-00017000: 434d 2220 2847 616c 6f69 7320 436f 756e  CM" (Galois Coun
-00017010: 7465 7220 4d6f 6465 2920 7368 6f75 6c64  ter Mode) should
-00017020: 2062 6520 7573 6564 206f 7665 7220 2243   be used over "C
-00017030: 4243 2220 2843 6970 6865 7220 426c 6f63  BC" (Cipher Bloc
-00017040: 6b20 4368 6169 6e69 6e67 2920 666f 7220  k Chaining) for 
-00017050: 7061 7373 776f 7264 2065 6e63 7279 7074  password encrypt
-00017060: 696f 6e2e 2022 5353 4f22 2066 6f72 2073  ion. "SSO" for s
-00017070: 696e 676c 6520 7369 676e 206f 6e2e 0a20  ingle sign on.. 
-00017080: 2020 202d 2066 6f72 6365 3a20 666f 7263     - force: forc
-00017090: 6520 7468 6520 636f 6e6e 6563 7469 6f6e  e the connection
-000170a0: 2074 6f20 7265 6d61 696e 206f 6e20 7468   to remain on th
-000170b0: 6973 2068 6f73 740a 2020 2020 2222 220a  is host.    """.
-000170c0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-000170d0: 6528 6861 6e64 7368 616b 652c 2073 7472  e(handshake, str
-000170e0: 293a 0a20 2020 2020 2020 2069 6620 6861  ):.        if ha
-000170f0: 6e64 7368 616b 652e 6c6f 7765 7228 2920  ndshake.lower() 
-00017100: 3d3d 2022 6763 6d22 3a0a 2020 2020 2020  == "gcm":.      
-00017110: 2020 2020 2020 6861 6e64 7368 616b 6520        handshake 
-00017120: 3d20 436f 6e6e 6563 7469 6f6e 2e48 414e  = Connection.HAN
-00017130: 4453 4841 4b45 5f47 434d 0a20 2020 2020  DSHAKE_GCM.     
-00017140: 2020 2065 6c69 6620 6861 6e64 7368 616b     elif handshak
-00017150: 652e 6c6f 7765 7228 2920 3d3d 2022 6362  e.lower() == "cb
-00017160: 6322 3a0a 2020 2020 2020 2020 2020 2020  c":.            
-00017170: 6861 6e64 7368 616b 6520 3d20 436f 6e6e  handshake = Conn
-00017180: 6563 7469 6f6e 2e48 414e 4453 4841 4b45  ection.HANDSHAKE
-00017190: 5f43 4243 0a20 2020 2020 2020 2065 6c69  _CBC.        eli
-000171a0: 6620 6861 6e64 7368 616b 652e 6c6f 7765  f handshake.lowe
-000171b0: 7228 2920 3d3d 2022 7373 6f22 3a0a 2020  r() == "sso":.  
-000171c0: 2020 2020 2020 2020 2020 6861 6e64 7368            handsh
-000171d0: 616b 6520 3d20 436f 6e6e 6563 7469 6f6e  ake = Connection
-000171e0: 2e48 414e 4453 4841 4b45 5f53 534f 0a20  .HANDSHAKE_SSO. 
-000171f0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00017200: 2020 2020 2020 2020 2072 6169 7365 2052           raise R
-00017210: 756e 7469 6d65 4572 726f 7228 6622 556e  untimeError(f"Un
-00017220: 6b6e 6f77 6e20 4861 6e64 7368 616b 6520  known Handshake 
-00017230: 6d65 7468 6f64 207b 6861 6e64 7368 616b  method {handshak
-00017240: 657d 2229 0a0a 2020 2020 6966 2069 7369  e}")..    if isi
-00017250: 6e73 7461 6e63 6528 746c 732c 2073 7472  nstance(tls, str
-00017260: 293a 0a20 2020 2020 2020 2069 6620 746c  ):.        if tl
-00017270: 732e 6c6f 7765 7228 2920 3d3d 2022 6f6e  s.lower() == "on
-00017280: 223a 0a20 2020 2020 2020 2020 2020 2074  ":.            t
-00017290: 6c73 203d 2043 6f6e 6e65 6374 696f 6e2e  ls = Connection.
-000172a0: 544c 535f 4f4e 0a20 2020 2020 2020 2065  TLS_ON.        e
-000172b0: 6c69 6620 746c 732e 6c6f 7765 7228 2920  lif tls.lower() 
-000172c0: 3d3d 2022 756e 7665 7269 6669 6564 223a  == "unverified":
-000172d0: 0a20 2020 2020 2020 2020 2020 2074 6c73  .            tls
-000172e0: 203d 2043 6f6e 6e65 6374 696f 6e2e 544c   = Connection.TL
-000172f0: 535f 554e 5645 5249 4649 4544 0a20 2020  S_UNVERIFIED.   
-00017300: 2020 2020 2065 6c69 6620 746c 732e 6c6f       elif tls.lo
-00017310: 7765 7228 2920 3d3d 2022 6f66 6622 3a0a  wer() == "off":.
-00017320: 2020 2020 2020 2020 2020 2020 746c 7320              tls 
-00017330: 3d20 436f 6e6e 6563 7469 6f6e 2e54 4c53  = Connection.TLS
-00017340: 5f4e 4f4e 450a 2020 2020 2020 2020 656c  _NONE.        el
-00017350: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00017360: 7261 6973 6520 5275 6e74 696d 6545 7272  raise RuntimeErr
-00017370: 6f72 2866 2255 6e6b 6e6f 776e 2054 4c53  or(f"Unknown TLS
-00017380: 206d 6f64 6520 7b74 6c73 7d22 290a 0a20   mode {tls}").. 
-00017390: 2020 2070 6172 616d 7320 3d20 7b0a 2020     params = {.  
-000173a0: 2020 2020 2020 2275 7365 7222 3a20 7573        "user": us
-000173b0: 6572 2c0a 2020 2020 2020 2020 2270 6173  er,.        "pas
-000173c0: 7377 6f72 6422 3a20 222a 2a2a 2a2a 222c  sword": "*****",
-000173d0: 0a20 2020 2020 2020 2022 686f 7374 223a  .        "host":
-000173e0: 2068 6f73 742c 0a20 2020 2020 2020 2022   host,.        "
-000173f0: 6461 7461 6261 7365 223a 2064 6174 6162  database": datab
-00017400: 6173 652c 0a20 2020 2020 2020 2022 746c  ase,.        "tl
-00017410: 7322 3a20 746c 732c 0a20 2020 2020 2020  s": tls,.       
-00017420: 2022 6861 6e64 7368 616b 6522 3a20 6861   "handshake": ha
-00017430: 6e64 7368 616b 652c 0a20 2020 207d 0a0a  ndshake,.    }..
-00017440: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-00017450: 2866 2243 6f6e 6e65 6374 207b 7061 7261  (f"Connect {para
-00017460: 6d73 7d22 290a 0a20 2020 2072 6574 7572  ms}")..    retur
-00017470: 6e20 436f 6e6e 6563 7469 6f6e 2864 736e  n Connection(dsn
-00017480: 2c20 7573 6572 2c20 7061 7373 776f 7264  , user, password
-00017490: 2c20 686f 7374 2c20 6461 7461 6261 7365  , host, database
-000174a0: 2c20 746c 732c 2068 616e 6473 6861 6b65  , tls, handshake
-000174b0: 2c20 666f 7263 652c 2063 6f6e 6669 6766  , force, configf
-000174c0: 696c 6529 0a0a 0a64 6566 205f 6375 7374  ile)...def _cust
-000174d0: 6f6d 5f74 7970 655f 746f 5f6a 736f 6e28  om_type_to_json(
-000174e0: 6f62 6a29 3a0a 2020 2020 2222 2248 656c  obj):.    """Hel
-000174f0: 7065 7220 6675 6e63 7469 6f6e 2074 6f20  per function to 
-00017500: 636f 6e76 6572 7420 7479 7065 7320 7265  convert types re
-00017510: 7475 726e 6564 2066 726f 6d20 7175 6572  turned from quer
-00017520: 6965 7320 746f 0a20 2020 204a 534f 4e20  ies to.    JSON 
-00017530: 7661 6c75 6573 2e20 2054 7970 6963 616c  values.  Typical
-00017540: 6c79 2069 6e76 6f6b 6564 2070 6173 7365  ly invoked passe
-00017550: 6420 6173 2074 6865 2060 6465 6661 756c  d as the `defaul
-00017560: 7460 2070 6172 616d 6574 6572 0a20 2020  t` parameter.   
-00017570: 2074 6f20 6a73 6f6e 2e64 756d 7073 2061   to json.dumps a
-00017580: 7320 696e 3a0a 0a20 2020 2060 6a73 6f6e  s in:..    `json
-00017590: 2e64 756d 7073 2873 6f6d 655f 726f 7773  .dumps(some_rows
-000175a0: 2c20 6465 6661 756c 743d 5f63 7573 746f  , default=_custo
-000175b0: 6d5f 7479 7065 5f74 6f5f 6a73 6f6e 2960  m_type_to_json)`
-000175c0: 0a20 2020 2022 2222 0a20 2020 2069 6620  .    """.    if 
-000175d0: 6973 696e 7374 616e 6365 286f 626a 2c20  isinstance(obj, 
-000175e0: 6465 6369 6d61 6c2e 4465 6369 6d61 6c29  decimal.Decimal)
-000175f0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00017600: 2073 7472 286f 626a 290a 0a20 2020 2069   str(obj)..    i
-00017610: 6620 6973 696e 7374 616e 6365 286f 626a  f isinstance(obj
-00017620: 2c20 2864 6174 6574 696d 652e 6461 7465  , (datetime.date
-00017630: 7469 6d65 2c20 6461 7465 7469 6d65 2e64  time, datetime.d
-00017640: 6174 652c 2064 6174 6574 696d 652e 7469  ate, datetime.ti
-00017650: 6d65 2929 3a0a 2020 2020 2020 2020 7265  me)):.        re
-00017660: 7475 726e 206f 626a 2e69 736f 666f 726d  turn obj.isoform
-00017670: 6174 2829 0a0a 2020 2020 6966 2069 7369  at()..    if isi
-00017680: 6e73 7461 6e63 6528 6f62 6a2c 2062 7974  nstance(obj, byt
-00017690: 6573 293a 0a20 2020 2020 2020 2072 6574  es):.        ret
-000176a0: 7572 6e20 6c69 7374 286f 626a 290a 0a20  urn list(obj).. 
-000176b0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-000176c0: 286f 626a 2c20 2875 7569 642e 5555 4944  (obj, (uuid.UUID
-000176d0: 2c20 6970 6164 6472 6573 732e 4950 7634  , ipaddress.IPv4
-000176e0: 4164 6472 6573 732c 2069 7061 6464 7265  Address, ipaddre
-000176f0: 7373 2e49 5076 3641 6464 7265 7373 2929  ss.IPv6Address))
-00017700: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00017710: 2073 7472 286f 626a 290a 0a20 2020 2069   str(obj)..    i
-00017720: 6620 6973 696e 7374 616e 6365 286f 626a  f isinstance(obj
-00017730: 2c20 285f 5354 506f 696e 742c 205f 5354  , (_STPoint, _ST
-00017740: 4c69 6e65 7374 7269 6e67 2c20 5f53 5450  Linestring, _STP
-00017750: 6f6c 7967 6f6e 2929 3a0a 2020 2020 2020  olygon)):.      
-00017760: 2020 2320 544f 444f 2047 656f 4a53 4f4e    # TODO GeoJSON
-00017770: 3f3f 0a20 2020 2020 2020 2072 6574 7572  ??.        retur
-00017780: 6e20 7374 7228 6f62 6a29 0a0a 2020 2020  n str(obj)..    
-00017790: 7072 696e 7428 6622 7479 7065 5f74 6f5f  print(f"type_to_
-000177a0: 7374 7269 6e67 2067 6f74 2063 616c 6c65  string got calle
-000177b0: 6420 666f 7220 7479 7065 207b 7479 7065  d for type {type
-000177c0: 286f 626a 297d 2229 0a20 2020 2072 6574  (obj)}").    ret
-000177d0: 7572 6e20 6622 706c 6163 6568 6f6c 6465  urn f"placeholde
-000177e0: 7220 666f 7220 7b74 7970 6528 6f62 6a29  r for {type(obj)
-000177f0: 7d22 0a0a 0a64 6566 2061 7267 7061 7273  }"...def argpars
-00017800: 6572 2829 3a0a 2020 2020 6672 6f6d 2061  er():.    from a
-00017810: 7267 7061 7273 6520 696d 706f 7274 2041  rgparse import A
-00017820: 7267 756d 656e 7450 6172 7365 722c 2046  rgumentParser, F
-00017830: 696c 6554 7970 652c 2052 6177 4465 7363  ileType, RawDesc
-00017840: 7269 7074 696f 6e48 656c 7046 6f72 6d61  riptionHelpForma
-00017850: 7474 6572 0a0a 2020 2020 636f 6e66 6967  tter..    config
-00017860: 6669 6c65 203d 2070 6174 686c 6962 2e50  file = pathlib.P
-00017870: 6174 682e 686f 6d65 2829 202f 2022 2e70  ath.home() / ".p
-00017880: 796f 6369 656e 7422 0a0a 2020 2020 7061  yocient"..    pa
-00017890: 7273 6572 203d 2041 7267 756d 656e 7450  rser = ArgumentP
-000178a0: 6172 7365 7228 0a20 2020 2020 2020 2064  arser(.        d
-000178b0: 6573 6372 6970 7469 6f6e 3d66 2222 224f  escription=f"""O
-000178c0: 6369 656e 7420 5079 7468 6f6e 2063 6c69  cient Python cli
-000178d0: 656e 7420 7b76 6572 7369 6f6e 7d2e 0a49  ent {version}..I
-000178e0: 6e20 7468 6520 7369 6d70 6c65 7374 2063  n the simplest c
-000178f0: 6173 652c 2072 756e 2077 6974 6820 6120  ase, run with a 
-00017900: 4461 7461 2053 6f75 7263 6520 4e61 6d65  Data Source Name
-00017910: 2028 6473 6e29 2061 6e64 2061 0a71 7565   (dsn) and a.que
-00017920: 7279 2e20 2046 6f72 2065 7861 6d70 6c65  ry.  For example
-00017930: 3a0a 2020 7079 6f63 6965 6e74 206f 6369  :.  pyocient oci
-00017940: 656e 743a 2f2f 7573 6572 3a70 6173 7377  ent://user:passw
-00017950: 6f72 6440 6d79 686f 7374 3a34 3035 302f  ord@myhost:4050/
-00017960: 6d79 6462 2022 7365 6c65 6374 202a 2066  mydb "select * f
-00017970: 726f 6d20 6d79 7461 626c 6522 0a0a 4d75  rom mytable"..Mu
-00017980: 6c74 6970 6c65 2071 7565 7279 2073 7472  ltiple query str
-00017990: 696e 6773 206d 6179 2062 6520 7072 6f76  ings may be prov
-000179a0: 6964 6564 0a0a 4453 4e27 7320 6172 6520  ided..DSN's are 
-000179b0: 6f66 2074 6865 2066 6f72 6d3a 0a20 206f  of the form:.  o
-000179c0: 6369 656e 743a 2f2f 7573 6572 3a70 6173  cient://user:pas
-000179d0: 7377 6f72 6440 5b68 6f73 745d 5b3a 706f  sword@[host][:po
-000179e0: 7274 5d5b 2f64 6174 6162 6173 655d 5b3f  rt][/database][?
-000179f0: 7061 7261 6d31 3d76 616c 7565 3126 2e2e  param1=value1&..
-00017a00: 2e5d 0a0a 5375 7070 6f72 7465 6420 7061  .]..Supported pa
-00017a10: 7261 6d65 7465 7220 6172 653a 0a0a 2d20  rameter are:..- 
-00017a20: 746c 733a 2057 6869 6368 2063 616e 2068  tls: Which can h
-00017a30: 6176 6520 7468 6520 7661 6c75 6573 2022  ave the values "
-00017a40: 6f66 6622 2c20 2275 6e76 6572 6966 6965  off", "unverifie
-00017a50: 6422 2c20 6f72 2022 6f6e 220a 0a2d 2066  d", or "on"..- f
-00017a60: 6f72 6365 3a20 7472 7565 206f 7220 6661  orce: true or fa
-00017a70: 6c73 6520 746f 2066 6f72 6365 2074 6865  lse to force the
-00017a80: 2063 6f6e 6e65 6374 696f 6e20 746f 2073   connection to s
-00017a90: 7461 7920 6f6e 2074 6869 7320 7365 7276  tay on this serv
-00017aa0: 6572 0a0a 2d20 6861 6e64 7368 616b 653a  er..- handshake:
-00017ab0: 2057 6869 6368 2063 616e 2068 6176 6520   Which can have 
-00017ac0: 7468 6520 7661 6c75 6520 2263 6263 220a  the value "cbc".
-00017ad0: 0a4d 756c 7469 706c 6520 686f 7374 7320  .Multiple hosts 
-00017ae0: 6d61 7920 6265 2073 7065 6369 6669 6564  may be specified
-00017af0: 2c20 7365 7061 7261 7465 6420 6279 2061  , separated by a
-00017b00: 2063 6f6d 6d61 2c20 696e 2077 6869 6368   comma, in which
-00017b10: 2063 6173 6520 7468 650a 686f 7374 7320   case the.hosts 
-00017b20: 7769 6c6c 2062 6520 7472 6965 6420 696e  will be tried in
-00017b30: 206f 7264 6572 2020 5468 7573 2061 6e20   order  Thus an 
-00017b40: 6578 616d 706c 6520 4453 4e20 6d69 6768  example DSN migh
-00017b50: 7420 6265 0a60 6f63 6965 6e74 3a2f 2f73  t be.`ocient://s
-00017b60: 6f6d 656f 6e65 3a73 6f6d 6570 6173 7377  omeone:somepassw
-00017b70: 6f72 6440 686f 7374 312c 686f 7374 323a  ord@host1,host2:
-00017b80: 3430 3531 2f6d 7964 6260 0a0a 5768 656e  4051/mydb`..When
-00017b90: 2072 756e 6e69 6e67 2069 6e20 7468 6520   running in the 
-00017ba0: 636f 6d6d 616e 6420 6c69 6e65 2069 6e74  command line int
-00017bb0: 6572 6661 6365 2c20 7468 6520 666f 6c6c  erface, the foll
-00017bc0: 6f77 696e 6720 6578 7472 6120 636f 6d6d  owing extra comm
-00017bd0: 616e 6473 0a61 7265 2073 7570 706f 7274  ands.are support
-00017be0: 6564 3a0a 0a2d 2063 6f6e 6e65 6374 2074  ed:..- connect t
-00017bf0: 6f20 276f 6369 656e 743a 2f2f 2e2e 2e2e  o 'ocient://....
-00017c00: 2720 7573 6572 2073 6f6d 6575 7365 7220  ' user someuser 
-00017c10: 7573 696e 6720 736f 6d65 7061 7373 776f  using somepasswo
-00017c20: 7264 3b0a 0a20 2020 2077 6865 6e20 7468  rd;..    when th
-00017c30: 6520 4453 4e20 666f 6c6c 6f77 7320 7468  e DSN follows th
-00017c40: 6520 6e6f 726d 616c 2070 796f 6369 656e  e normal pyocien
-00017c50: 7420 4453 4e20 666f 726d 6174 2c20 6275  t DSN format, bu
-00017c60: 7420 7468 6520 7573 6572 6964 2061 6e64  t the userid and
-00017c70: 2070 6173 7377 6f72 6420 6d61 7920 6265   password may be
-00017c80: 2070 6173 7365 640a 2020 2020 7573 696e   passed.    usin
-00017c90: 6720 7468 6520 5553 4552 2061 6e64 2055  g the USER and U
-00017ca0: 5349 4e47 206b 6579 776f 7264 7320 2873  SING keywords (s
-00017cb0: 696d 696c 6172 2074 6f20 7468 6520 4f63  imilar to the Oc
-00017cc0: 6965 6e74 204a 4442 4320 6472 6976 6572  ient JDBC driver
-00017cd0: 292e 2020 5468 6520 4453 4e20 6d75 7374  ).  The DSN must
-00017ce0: 2062 6520 7175 6f74 6564 2e0a 0a2d 2073   be quoted...- s
-00017cf0: 6f75 7263 6520 2766 696c 6527 3b0a 0a20  ource 'file';.. 
-00017d00: 2020 2045 7865 6375 7465 2074 6865 2073     Execute the s
-00017d10: 7461 7465 6d65 6e74 7320 6672 6f6d 2074  tatements from t
-00017d20: 6865 2073 7065 6369 6669 6564 2066 696c  he specified fil
-00017d30: 652e 2020 5468 6520 6669 6c65 206e 616d  e.  The file nam
-00017d40: 6520 6d75 7374 2062 6520 7175 6f74 6564  e must be quoted
-00017d50: 2e0a 0a2d 2073 6574 2066 6f72 6d61 7420  ...- set format 
-00017d60: 7461 626c 653b 0a0a 2020 2020 5365 7420  table;..    Set 
-00017d70: 7468 6520 6f75 7470 7574 2066 6f72 6d61  the output forma
-00017d80: 7420 0a0a 2d20 7175 6974 3b0a 0a22 2222  t ..- quit;.."""
-00017d90: 2c0a 2020 2020 2020 2020 666f 726d 6174  ,.        format
-00017da0: 7465 725f 636c 6173 733d 5261 7744 6573  ter_class=RawDes
-00017db0: 6372 6970 7469 6f6e 4865 6c70 466f 726d  criptionHelpForm
-00017dc0: 6174 7465 722c 0a20 2020 2029 0a0a 2020  atter,.    )..  
-00017dd0: 2020 2320 466c 6167 7320 7468 6174 2061    # Flags that a
-00017de0: 7070 6c79 2074 6f20 626f 7468 2065 7865  pply to both exe
-00017df0: 6375 7469 6f6e 206d 6f64 6573 0a20 2020  cution modes.   
-00017e00: 206f 7574 6772 6f75 7020 3d20 7061 7273   outgroup = pars
-00017e10: 6572 2e61 6464 5f6d 7574 7561 6c6c 795f  er.add_mutually_
-00017e20: 6578 636c 7573 6976 655f 6772 6f75 7028  exclusive_group(
-00017e30: 290a 2020 2020 6f75 7467 726f 7570 2e61  ).    outgroup.a
-00017e40: 6464 5f61 7267 756d 656e 7428 222d 6f22  dd_argument("-o"
-00017e50: 2c20 222d 2d6f 7574 6669 6c65 222c 2074  , "--outfile", t
-00017e60: 7970 653d 4669 6c65 5479 7065 2822 7722  ype=FileType("w"
-00017e70: 292c 2064 6566 6175 6c74 3d22 2d22 2c20  ), default="-", 
-00017e80: 6865 6c70 3d22 4f75 7470 7574 2066 696c  help="Output fil
-00017e90: 6522 290a 2020 2020 6f75 7467 726f 7570  e").    outgroup
-00017ea0: 2e61 6464 5f61 7267 756d 656e 7428 222d  .add_argument("-
-00017eb0: 6e22 2c20 222d 2d6e 6f6f 7574 222c 2061  n", "--noout", a
-00017ec0: 6374 696f 6e3d 2273 746f 7265 5f63 6f6e  ction="store_con
-00017ed0: 7374 222c 2063 6f6e 7374 3d4e 6f6e 652c  st", const=None,
-00017ee0: 2064 6573 743d 226f 7574 6669 6c65 222c   dest="outfile",
-00017ef0: 2068 656c 703d 2244 6f20 6e6f 7420 6f75   help="Do not ou
-00017f00: 7470 7574 2072 6573 756c 7473 2229 0a20  tput results"). 
-00017f10: 2020 2063 6f6e 6669 6767 726f 7570 203d     configgroup =
-00017f20: 2070 6172 7365 722e 6164 645f 6d75 7475   parser.add_mutu
-00017f30: 616c 6c79 5f65 7863 6c75 7369 7665 5f67  ally_exclusive_g
-00017f40: 726f 7570 2829 0a20 2020 2063 6f6e 6669  roup().    confi
-00017f50: 6767 726f 7570 2e61 6464 5f61 7267 756d  ggroup.add_argum
-00017f60: 656e 7428 222d 6322 2c20 222d 2d63 6f6e  ent("-c", "--con
-00017f70: 6669 6766 696c 6522 2c20 7479 7065 3d73  figfile", type=s
-00017f80: 7472 2c20 6465 6661 756c 743d 7374 7228  tr, default=str(
-00017f90: 636f 6e66 6967 6669 6c65 292c 2068 656c  configfile), hel
-00017fa0: 703d 2243 6f6e 6669 6775 7261 7469 6f6e  p="Configuration
-00017fb0: 2066 696c 6522 290a 2020 2020 636f 6e66   file").    conf
-00017fc0: 6967 6772 6f75 702e 6164 645f 6172 6775  iggroup.add_argu
-00017fd0: 6d65 6e74 2822 2d2d 6e6f 636f 6e66 6967  ment("--noconfig
-00017fe0: 222c 2061 6374 696f 6e3d 2273 746f 7265  ", action="store
-00017ff0: 5f63 6f6e 7374 222c 2063 6f6e 7374 3d4e  _const", const=N
-00018000: 6f6e 652c 2064 6573 743d 2263 6f6e 6669  one, dest="confi
-00018010: 6766 696c 6522 2c20 6865 6c70 3d22 4e6f  gfile", help="No
-00018020: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
-00018030: 696c 6522 290a 2020 2020 7061 7273 6572  ile").    parser
-00018040: 2e61 6464 5f61 7267 756d 656e 7428 222d  .add_argument("-
-00018050: 6922 2c20 222d 2d69 6e66 696c 6522 2c20  i", "--infile", 
-00018060: 7479 7065 3d46 696c 6554 7970 6528 2272  type=FileType("r
-00018070: 2229 2c20 6465 6661 756c 743d 4e6f 6e65  "), default=None
-00018080: 2c20 6865 6c70 3d22 496e 7075 7420 6669  , help="Input fi
-00018090: 6c65 2063 6f6e 7461 696e 696e 6720 5351  le containing SQ
-000180a0: 4c20 7374 6174 656d 656e 7473 2229 0a20  L statements"). 
-000180b0: 2020 2070 6172 7365 722e 6164 645f 6172     parser.add_ar
-000180c0: 6775 6d65 6e74 2822 2d6c 222c 2022 2d2d  gument("-l", "--
-000180d0: 6c6f 676c 6576 656c 222c 2074 7970 653d  loglevel", type=
-000180e0: 7374 722c 2064 6566 6175 6c74 3d22 6372  str, default="cr
-000180f0: 6974 6963 616c 222c 2063 686f 6963 6573  itical", choices
-00018100: 3d5b 2263 7269 7469 6361 6c22 2c20 2265  =["critical", "e
-00018110: 7272 6f72 222c 2022 7761 726e 696e 6722  rror", "warning"
-00018120: 2c20 2269 6e66 6f22 2c20 2264 6562 7567  , "info", "debug
-00018130: 225d 2c20 6865 6c70 3d22 4c6f 6767 696e  "], help="Loggin
-00018140: 6720 6c65 7665 6c2c 2064 6566 6175 6c74  g level, default
-00018150: 7320 746f 2063 7269 7469 6361 6c22 290a  s to critical").
-00018160: 2020 2020 7061 7273 6572 2e61 6464 5f61      parser.add_a
-00018170: 7267 756d 656e 7428 222d 2d6c 6f67 6669  rgument("--logfi
-00018180: 6c65 222c 2074 7970 653d 4669 6c65 5479  le", type=FileTy
-00018190: 7065 2822 6122 292c 2064 6566 6175 6c74  pe("a"), default
-000181a0: 3d73 7973 2e73 7464 6f75 742c 2068 656c  =sys.stdout, hel
-000181b0: 703d 224c 6f67 2066 696c 6522 290a 2020  p="Log file").  
-000181c0: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
-000181d0: 756d 656e 7428 222d 7422 2c20 222d 2d74  ument("-t", "--t
-000181e0: 696d 6522 2c20 6163 7469 6f6e 3d22 7374  ime", action="st
-000181f0: 6f72 655f 7472 7565 222c 2068 656c 703d  ore_true", help=
-00018200: 224f 7574 7075 7420 7175 6572 7920 7469  "Output query ti
-00018210: 6d65 2229 0a20 2020 2070 6172 7365 722e  me").    parser.
-00018220: 6164 645f 6172 6775 6d65 6e74 2822 6473  add_argument("ds
-00018230: 6e22 2c20 6e61 7267 733d 223f 222c 2068  n", nargs="?", h
-00018240: 656c 703d 2244 534e 206f 6620 7468 6520  elp="DSN of the 
-00018250: 666f 726d 206f 6369 656e 743a 2f2f 7573  form ocient://us
-00018260: 6572 3a70 6173 7377 6f72 6440 5b68 6f73  er:password@[hos
-00018270: 745d 5b3a 706f 7274 5d5b 2f64 6174 6162  t][:port][/datab
-00018280: 6173 655d 5b3f 7061 7261 6d31 3d76 616c  ase][?param1=val
-00018290: 7565 3126 2e2e 2e5d 2229 0a20 2020 2070  ue1&...]").    p
-000182a0: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
-000182b0: 6e74 2822 7371 6c22 2c20 6e61 7267 733d  nt("sql", nargs=
-000182c0: 223f 222c 2068 656c 703d 2253 514c 2073  "?", help="SQL s
-000182d0: 7461 7465 6d65 6e74 2229 0a20 2020 2070  tatement").    p
-000182e0: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
-000182f0: 6e74 2822 2d2d 666f 726d 6174 222c 2022  nt("--format", "
-00018300: 2d66 222c 2074 7970 653d 7374 722c 2063  -f", type=str, c
-00018310: 686f 6963 6573 3d5b 226a 736f 6e22 2c20  hoices=["json", 
-00018320: 2274 6162 6c65 222c 2022 6373 7622 5d2c  "table", "csv"],
-00018330: 2064 6566 6175 6c74 3d22 6a73 6f6e 222c   default="json",
-00018340: 2068 656c 703d 224f 7574 7075 7420 666f   help="Output fo
-00018350: 726d 6174 2c20 6465 6661 756c 7473 2074  rmat, defaults t
-00018360: 6f20 6a73 6f6e 2229 0a20 2020 2070 6172  o json").    par
-00018370: 7365 722e 6164 645f 6172 6775 6d65 6e74  ser.add_argument
-00018380: 2822 2d2d 6e6f 636f 6c6f 7222 2c20 6163  ("--nocolor", ac
-00018390: 7469 6f6e 3d22 7374 6f72 655f 7472 7565  tion="store_true
-000183a0: 222c 2068 656c 703d 2257 6865 6e20 7573  ", help="When us
-000183b0: 696e 6720 7079 6f63 6965 6e74 2069 6e74  ing pyocient int
-000183c0: 6572 6163 7469 7665 6c79 2c20 646f 206e  eractively, do n
-000183d0: 6f74 2063 6f6c 6f72 2229 0a0a 2020 2020  ot color")..    
-000183e0: 7265 7475 726e 2070 6172 7365 720a 0a0a  return parser...
-000183f0: 6465 6620 6d61 696e 2829 3a0a 2020 2020  def main():.    
-00018400: 696d 706f 7274 206a 736f 6e0a 2020 2020  import json.    
-00018410: 696d 706f 7274 2063 7376 0a20 2020 2066  import csv.    f
-00018420: 726f 6d20 7461 6275 6c61 7465 2069 6d70  rom tabulate imp
-00018430: 6f72 7420 7461 6275 6c61 7465 0a20 2020  ort tabulate.   
-00018440: 2066 726f 6d20 7079 676d 656e 7473 2e6c   from pygments.l
-00018450: 6578 6572 732e 7371 6c20 696d 706f 7274  exers.sql import
-00018460: 2053 716c 4c65 7865 720a 2020 2020 6672   SqlLexer.    fr
-00018470: 6f6d 2070 7967 6d65 6e74 732e 746f 6b65  om pygments.toke
-00018480: 6e20 696d 706f 7274 2054 6f6b 656e 0a0a  n import Token..
-00018490: 2020 2020 6172 6773 203d 2061 7267 7061      args = argpa
-000184a0: 7273 6572 2829 2e70 6172 7365 5f61 7267  rser().parse_arg
-000184b0: 7328 7379 732e 6172 6776 5b31 3a5d 290a  s(sys.argv[1:]).
-000184c0: 0a20 2020 206c 6f67 5f6c 6576 656c 203d  .    log_level =
-000184d0: 2067 6574 6174 7472 286c 6f67 6769 6e67   getattr(logging
-000184e0: 2c20 6172 6773 2e6c 6f67 6c65 7665 6c2e  , args.loglevel.
-000184f0: 7570 7065 7228 292c 204e 6f6e 6529 0a20  upper(), None). 
-00018500: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
-00018510: 616e 6365 286c 6f67 5f6c 6576 656c 2c20  ance(log_level, 
-00018520: 696e 7429 3a0a 2020 2020 2020 2020 7261  int):.        ra
-00018530: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
-00018540: 496e 7661 6c69 6420 6c6f 6720 6c65 7665  Invalid log leve
-00018550: 6c3a 2025 7322 2025 2061 7267 732e 6c6f  l: %s" % args.lo
-00018560: 676c 6576 656c 290a 0a20 2020 206c 6f67  glevel)..    log
-00018570: 6769 6e67 2e62 6173 6963 436f 6e66 6967  ging.basicConfig
-00018580: 286c 6576 656c 3d6c 6f67 5f6c 6576 656c  (level=log_level
-00018590: 2c20 7374 7265 616d 3d61 7267 732e 6c6f  , stream=args.lo
-000185a0: 6766 696c 652c 2066 6f72 6d61 743d 225b  gfile, format="[
-000185b0: 2528 6173 6374 696d 6529 735d 5b25 286c  %(asctime)s][%(l
-000185c0: 6576 656c 6e61 6d65 2973 5d20 2528 6d65  evelname)s] %(me
-000185d0: 7373 6167 6529 7322 290a 0a20 2020 2073  ssage)s")..    s
-000185e0: 716c 5f73 746d 7420 3d20 2222 0a20 2020  ql_stmt = "".   
-000185f0: 206c 6578 6572 203d 2053 716c 4c65 7865   lexer = SqlLexe
-00018600: 7228 290a 0a20 2020 2064 6566 205f 756e  r()..    def _un
-00018610: 7175 6f74 6528 696e 7075 7429 3a0a 2020  quote(input):.  
-00018620: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00018630: 2020 556e 7175 6f74 6520 6120 7374 7269    Unquote a stri
-00018640: 6e67 2c20 7769 7468 2065 6974 6865 7220  ng, with either 
-00018650: 7369 6e67 6c65 206f 7220 646f 7562 6c65  single or double
-00018660: 2071 756f 7465 730a 2020 2020 2020 2020   quotes.        
-00018670: 2222 220a 2020 2020 2020 2020 6966 2069  """.        if i
-00018680: 6e70 7574 5b30 5d20 3d3d 2027 2227 2061  nput[0] == '"' a
-00018690: 6e64 2069 6e70 7574 5b2d 315d 203d 3d20  nd input[-1] == 
-000186a0: 2722 273a 0a20 2020 2020 2020 2020 2020  '"':.           
-000186b0: 2072 6574 7572 6e20 696e 7075 745b 313a   return input[1:
-000186c0: 2d31 5d0a 2020 2020 2020 2020 6966 2069  -1].        if i
-000186d0: 6e70 7574 5b30 5d20 3d3d 2022 2722 2061  nput[0] == "'" a
-000186e0: 6e64 2069 6e70 7574 5b2d 315d 203d 3d20  nd input[-1] == 
-000186f0: 2227 223a 0a20 2020 2020 2020 2020 2020  "'":.           
-00018700: 2072 6574 7572 6e20 696e 7075 745b 313a   return input[1:
-00018710: 2d31 5d0a 2020 2020 2020 2020 7265 7475  -1].        retu
-00018720: 726e 2069 6e70 7574 0a0a 2020 2020 6465  rn input..    de
-00018730: 6620 5f64 6f5f 6c69 6e65 2861 7267 732c  f _do_line(args,
-00018740: 2063 6f6e 6e65 6374 696f 6e2c 2074 6578   connection, tex
-00018750: 742c 2073 716c 5f73 746d 742c 2071 7565  t, sql_stmt, que
-00018760: 7279 5f66 6e29 3a0a 2020 2020 2020 2020  ry_fn):.        
-00018770: 6e65 775f 636f 6e6e 6563 7469 6f6e 203d  new_connection =
-00018780: 2063 6f6e 6e65 6374 696f 6e0a 2020 2020   connection.    
-00018790: 2020 2020 666f 7220 2874 6f6b 656e 5f74      for (token_t
-000187a0: 7970 652c 2074 6f6b 656e 5f76 616c 2920  ype, token_val) 
-000187b0: 696e 206c 6578 6572 2e67 6574 5f74 6f6b  in lexer.get_tok
-000187c0: 656e 7328 7465 7874 293a 0a20 2020 2020  ens(text):.     
-000187d0: 2020 2020 2020 2069 6620 746f 6b65 6e5f         if token_
-000187e0: 7479 7065 203d 3d20 546f 6b65 6e2e 5075  type == Token.Pu
-000187f0: 6e63 7475 6174 696f 6e20 616e 6420 746f  nctuation and to
-00018800: 6b65 6e5f 7661 6c20 3d3d 2022 3b22 3a0a  ken_val == ";":.
-00018810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018820: 6e65 775f 636f 6e6e 6563 7469 6f6e 203d  new_connection =
-00018830: 2071 7565 7279 5f66 6e28 6172 6773 2c20   query_fn(args, 
-00018840: 6e65 775f 636f 6e6e 6563 7469 6f6e 2c20  new_connection, 
-00018850: 7371 6c5f 7374 6d74 290a 2020 2020 2020  sql_stmt).      
-00018860: 2020 2020 2020 2020 2020 7371 6c5f 7374            sql_st
-00018870: 6d74 203d 2022 220a 2020 2020 2020 2020  mt = "".        
-00018880: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00018890: 2020 2020 2020 2020 2020 7371 6c5f 7374            sql_st
-000188a0: 6d74 202b 3d20 746f 6b65 6e5f 7661 6c0a  mt += token_val.
-000188b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000188c0: 2873 716c 5f73 746d 742c 206e 6577 5f63  (sql_stmt, new_c
-000188d0: 6f6e 6e65 6374 696f 6e29 0a0a 2020 2020  onnection)..    
-000188e0: 6465 6620 5f64 6f5f 7175 6572 7928 6172  def _do_query(ar
-000188f0: 6773 2c20 636f 6e6e 6563 7469 6f6e 2c20  gs, connection, 
-00018900: 7175 6572 7929 3a0a 2020 2020 2020 2020  query):.        
-00018910: 2320 4669 7273 742c 2073 6565 2069 6620  # First, see if 
-00018920: 7468 6973 2069 7320 736f 6d65 7468 696e  this is somethin
-00018930: 6720 7765 2073 686f 756c 6420 6861 6e64  g we should hand
-00018940: 6c65 2068 6572 6520 696e 2074 6865 2043  le here in the C
-00018950: 4c49 0a20 2020 2020 2020 2074 6f6b 656e  LI.        token
-00018960: 7320 3d20 5b74 6f6b 656e 2066 6f72 2028  s = [token for (
-00018970: 746f 6b65 6e5f 7479 7065 2c20 746f 6b65  token_type, toke
-00018980: 6e29 2069 6e20 6c65 7865 722e 6765 745f  n) in lexer.get_
-00018990: 746f 6b65 6e73 2871 7565 7279 2920 6966  tokens(query) if
-000189a0: 2074 6f6b 656e 5f74 7970 6520 696e 2028   token_type in (
-000189b0: 546f 6b65 6e2e 4b65 7977 6f72 642c 2054  Token.Keyword, T
-000189c0: 6f6b 656e 2e4e 616d 652c 2054 6f6b 656e  oken.Name, Token
-000189d0: 2e4c 6974 6572 616c 2e53 7472 696e 672e  .Literal.String.
-000189e0: 5379 6d62 6f6c 2c20 546f 6b65 6e2e 4c69  Symbol, Token.Li
-000189f0: 7465 7261 6c2e 5374 7269 6e67 2e53 696e  teral.String.Sin
-00018a00: 676c 6529 5d0a 0a20 2020 2020 2020 2023  gle)]..        #
-00018a10: 2063 6f6e 6e65 6374 2074 6f20 7374 6174   connect to stat
-00018a20: 656d 656e 740a 2020 2020 2020 2020 6966  ement.        if
-00018a30: 206c 656e 2874 6f6b 656e 7329 203e 2031   len(tokens) > 1
-00018a40: 2061 6e64 2074 6f6b 656e 735b 305d 2e6c   and tokens[0].l
-00018a50: 6f77 6572 2829 203d 3d20 2263 6f6e 6e65  ower() == "conne
-00018a60: 6374 2220 616e 6420 746f 6b65 6e73 5b31  ct" and tokens[1
-00018a70: 5d2e 6c6f 7765 7228 2920 3d3d 2022 746f  ].lower() == "to
-00018a80: 223a 0a20 2020 2020 2020 2020 2020 2074  ":.            t
-00018a90: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00018aa0: 2020 2020 6966 206c 656e 2874 6f6b 656e      if len(token
-00018ab0: 7329 203d 3d20 373a 0a20 2020 2020 2020  s) == 7:.       
-00018ac0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00018ad0: 746f 6b65 6e73 5b33 5d2e 6c6f 7765 7228  tokens[3].lower(
-00018ae0: 2920 213d 2022 7573 6572 2220 6f72 2074  ) != "user" or t
-00018af0: 6f6b 656e 735b 355d 2e6c 6f77 6572 2829  okens[5].lower()
-00018b00: 2021 3d20 2275 7369 6e67 223a 0a20 2020   != "using":.   
-00018b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b20: 2020 2020 2070 7269 6e74 2866 2249 6e76       print(f"Inv
-00018b30: 616c 6964 2055 5345 5220 6f72 2055 5349  alid USER or USI
-00018b40: 4e47 206b 6579 776f 7264 7320 6f6e 2043  NG keywords on C
-00018b50: 4f4e 4e45 4354 2054 4f22 290a 2020 2020  ONNECT TO").    
-00018b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b70: 2020 2020 7265 7475 726e 2063 6f6e 6e65      return conne
-00018b80: 6374 696f 6e0a 2020 2020 2020 2020 2020  ction.          
-00018b90: 2020 2020 2020 2020 2020 6473 6e20 3d20            dsn = 
-00018ba0: 5f75 6e71 756f 7465 2874 6f6b 656e 735b  _unquote(tokens[
-00018bb0: 325d 290a 2020 2020 2020 2020 2020 2020  2]).            
-00018bc0: 2020 2020 2020 2020 7573 6572 203d 205f          user = _
-00018bd0: 756e 7175 6f74 6528 746f 6b65 6e73 5b34  unquote(tokens[4
-00018be0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-00018bf0: 2020 2020 2020 2070 6173 7377 6f72 6420         password 
-00018c00: 3d20 5f75 6e71 756f 7465 2874 6f6b 656e  = _unquote(token
-00018c10: 735b 365d 290a 2020 2020 2020 2020 2020  s[6]).          
-00018c20: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00018c30: 2063 6f6e 6e65 6374 2864 736e 2c20 7573   connect(dsn, us
-00018c40: 6572 3d75 7365 722c 2070 6173 7377 6f72  er=user, passwor
-00018c50: 643d 7061 7373 776f 7264 2c20 636f 6e66  d=password, conf
-00018c60: 6967 6669 6c65 3d61 7267 732e 636f 6e66  igfile=args.conf
-00018c70: 6967 6669 6c65 290a 2020 2020 2020 2020  igfile).        
-00018c80: 2020 2020 2020 2020 656c 6966 206c 656e          elif len
-00018c90: 2874 6f6b 656e 7329 203d 3d20 333a 0a20  (tokens) == 3:. 
-00018ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018cb0: 2020 2064 736e 203d 205f 756e 7175 6f74     dsn = _unquot
-00018cc0: 6528 746f 6b65 6e73 5b32 5d29 0a20 2020  e(tokens[2]).   
-00018cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ce0: 2072 6574 7572 6e20 636f 6e6e 6563 7428   return connect(
-00018cf0: 6473 6e2c 2063 6f6e 6669 6766 696c 653d  dsn, configfile=
-00018d00: 6172 6773 2e63 6f6e 6669 6766 696c 6529  args.configfile)
-00018d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018d20: 2070 7269 6e74 2866 2249 6e76 616c 6964   print(f"Invalid
-00018d30: 2043 4f4e 4e45 4354 2054 4f20 7374 6174   CONNECT TO stat
-00018d40: 656d 656e 7420 7b6c 656e 2874 6f6b 656e  ement {len(token
-00018d50: 7329 7d20 7b74 6f6b 656e 737d 2229 0a20  s)} {tokens}"). 
-00018d60: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00018d70: 6574 7572 6e20 636f 6e6e 6563 7469 6f6e  eturn connection
-00018d80: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
-00018d90: 6570 7420 5351 4c45 7863 6570 7469 6f6e  ept SQLException
-00018da0: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
-00018db0: 2020 2020 2020 2070 7269 6e74 2865 290a         print(e).
-00018dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018dd0: 7265 7475 726e 2063 6f6e 6e65 6374 696f  return connectio
-00018de0: 6e0a 0a20 2020 2020 2020 2023 2073 6574  n..        # set
-00018df0: 2066 6f72 6d61 740a 2020 2020 2020 2020   format.        
-00018e00: 6966 206c 656e 2874 6f6b 656e 7329 203e  if len(tokens) >
-00018e10: 2031 2061 6e64 2074 6f6b 656e 735b 305d   1 and tokens[0]
-00018e20: 2e6c 6f77 6572 2829 203d 3d20 2273 6574  .lower() == "set
-00018e30: 2220 616e 6420 746f 6b65 6e73 5b31 5d2e  " and tokens[1].
-00018e40: 6c6f 7765 7228 2920 3d3d 2022 666f 726d  lower() == "form
-00018e50: 6174 223a 0a20 2020 2020 2020 2020 2020  at":.           
-00018e60: 206e 6577 5f66 6f72 6d61 7420 3d20 746f   new_format = to
-00018e70: 6b65 6e73 5b32 5d2e 6c6f 7765 7228 290a  kens[2].lower().
-00018e80: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00018e90: 6577 5f66 6f72 6d61 7420 696e 205b 226a  ew_format in ["j
-00018ea0: 736f 6e22 2c20 2274 6162 6c65 222c 2022  son", "table", "
-00018eb0: 6373 7622 5d3a 0a20 2020 2020 2020 2020  csv"]:.         
-00018ec0: 2020 2020 2020 2061 7267 732e 666f 726d         args.form
-00018ed0: 6174 203d 206e 6577 5f66 6f72 6d61 740a  at = new_format.
-00018ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ef0: 7072 696e 7428 224f 4b22 290a 2020 2020  print("OK").    
-00018f00: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00018f10: 726e 2063 6f6e 6e65 6374 696f 6e0a 2020  rn connection.  
-00018f20: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00018f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f40: 7072 696e 7428 6622 496e 7661 6c69 6420  print(f"Invalid 
-00018f50: 6f75 7470 7574 2066 6f72 6d61 7420 7b6e  output format {n
-00018f60: 6577 5f66 6f72 6d61 747d 2229 0a20 2020  ew_format}").   
-00018f70: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00018f80: 7572 6e20 636f 6e6e 6563 7469 6f6e 0a0a  urn connection..
-00018f90: 2020 2020 2020 2020 2320 736f 7572 6365          # source
-00018fa0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-00018fb0: 746f 6b65 6e73 2920 3e20 3020 616e 6420  tokens) > 0 and 
-00018fc0: 746f 6b65 6e73 5b30 5d2e 6c6f 7765 7228  tokens[0].lower(
-00018fd0: 2920 3d3d 2022 736f 7572 6365 223a 0a20  ) == "source":. 
-00018fe0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-00018ff0: 6e28 746f 6b65 6e73 2920 213d 2032 3a0a  n(tokens) != 2:.
-00019000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019010: 7072 696e 7428 2249 6e76 616c 6964 2053  print("Invalid S
-00019020: 4f55 5243 4520 7374 6174 656d 656e 7422  OURCE statement"
-00019030: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00019040: 2020 7265 7475 726e 2063 6f6e 6e65 6374    return connect
-00019050: 696f 6e0a 0a20 2020 2020 2020 2020 2020  ion..           
-00019060: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00019070: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
-00019080: 5f75 6e71 756f 7465 2874 6f6b 656e 735b  _unquote(tokens[
-00019090: 315d 292c 206d 6f64 653d 2272 2229 2061  1]), mode="r") a
-000190a0: 7320 663a 0a20 2020 2020 2020 2020 2020  s f:.           
-000190b0: 2020 2020 2020 2020 2028 7371 6c5f 7374           (sql_st
-000190c0: 6d74 2c20 636f 6e6e 6563 7469 6f6e 2920  mt, connection) 
-000190d0: 3d20 5f64 6f5f 6c69 6e65 2861 7267 732c  = _do_line(args,
-000190e0: 2063 6f6e 6e65 6374 696f 6e2c 2066 2e72   connection, f.r
-000190f0: 6561 6428 292c 2022 222c 205f 646f 5f71  ead(), "", _do_q
-00019100: 7565 7279 290a 2020 2020 2020 2020 2020  uery).          
-00019110: 2020 2020 2020 6966 206c 656e 2873 716c        if len(sql
-00019120: 5f73 746d 742e 7374 7269 7028 2929 3a0a  _stmt.strip()):.
-00019130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019140: 2020 2020 636f 6e6e 6563 7469 6f6e 203d      connection =
-00019150: 205f 646f 5f71 7565 7279 2861 7267 732c   _do_query(args,
-00019160: 2063 6f6e 6e65 6374 696f 6e2c 2073 716c   connection, sql
-00019170: 5f73 746d 7429 0a20 2020 2020 2020 2020  _stmt).         
-00019180: 2020 2020 2020 2072 6574 7572 6e20 636f         return co
-00019190: 6e6e 6563 7469 6f6e 0a20 2020 2020 2020  nnection.       
-000191a0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
-000191b0: 7074 696f 6e20 6173 2065 3a0a 2020 2020  ption as e:.    
-000191c0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-000191d0: 7428 6529 0a20 2020 2020 2020 2020 2020  t(e).           
-000191e0: 2020 2020 2072 6574 7572 6e20 636f 6e6e       return conn
-000191f0: 6563 7469 6f6e 0a0a 2020 2020 2020 2020  ection..        
-00019200: 2320 7175 6974 0a20 2020 2020 2020 2069  # quit.        i
-00019210: 6620 6c65 6e28 746f 6b65 6e73 2920 3e20  f len(tokens) > 
-00019220: 3020 616e 6420 746f 6b65 6e73 5b30 5d2e  0 and tokens[0].
-00019230: 6c6f 7765 7228 2920 3d3d 2022 7175 6974  lower() == "quit
-00019240: 223a 0a20 2020 2020 2020 2020 2020 2073  ":.            s
-00019250: 7973 2e65 7869 7428 3029 0a0a 2020 2020  ys.exit(0)..    
-00019260: 2020 2020 6966 2063 6f6e 6e65 6374 696f      if connectio
-00019270: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
-00019280: 2020 2020 2020 2070 7269 6e74 2866 224e         print(f"N
-00019290: 6f20 6163 7469 7665 2063 6f6e 6e65 6374  o active connect
-000192a0: 696f 6e22 290a 2020 2020 2020 2020 2020  ion").          
-000192b0: 2020 7265 7475 726e 2063 6f6e 6e65 6374    return connect
-000192c0: 696f 6e0a 0a20 2020 2020 2020 2023 204f  ion..        # O
-000192d0: 4b2c 2069 6620 7765 2066 616c 6c20 7468  K, if we fall th
-000192e0: 726f 7567 6820 746f 2068 6572 652c 2068  rough to here, h
-000192f0: 6176 6520 7468 6520 6e6f 726d 616c 206c  ave the normal l
-00019300: 6962 7261 7279 2068 616e 646c 6520 6974  ibrary handle it
-00019310: 0a20 2020 2020 2020 2069 6620 6172 6773  .        if args
-00019320: 2e74 696d 653a 0a20 2020 2020 2020 2020  .time:.         
-00019330: 2020 2073 7461 7274 7469 6d65 203d 2074     starttime = t
-00019340: 696d 655f 6e73 2829 0a0a 2020 2020 2020  ime_ns()..      
-00019350: 2020 6375 7273 6f72 203d 2063 6f6e 6e65    cursor = conne
-00019360: 6374 696f 6e2e 6375 7273 6f72 2829 0a0a  ction.cursor()..
-00019370: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00019380: 2020 2020 2020 2020 2063 7572 736f 722e           cursor.
-00019390: 6578 6563 7574 6528 7175 6572 7929 0a0a  execute(query)..
-000193a0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-000193b0: 7572 736f 722e 6465 7363 7269 7074 696f  ursor.descriptio
-000193c0: 6e20 616e 6420 6e6f 7420 6375 7273 6f72  n and not cursor
-000193d0: 2e65 7870 6c61 696e 5f72 6573 756c 743a  .explain_result:
-000193e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000193f0: 2072 6573 756c 7420 3d20 6375 7273 6f72   result = cursor
-00019400: 2e66 6574 6368 616c 6c28 290a 2020 2020  .fetchall().    
-00019410: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00019420: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00019430: 7375 6c74 203d 2063 7572 736f 722e 636f  sult = cursor.co
-00019440: 6e6e 6563 7469 6f6e 0a20 2020 2020 2020  nnection.       
-00019450: 2065 7863 6570 7420 5351 4c45 7863 6570   except SQLExcep
-00019460: 7469 6f6e 2061 7320 653a 0a20 2020 2020  tion as e:.     
-00019470: 2020 2020 2020 2070 7269 6e74 2865 290a         print(e).
-00019480: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00019490: 726e 2063 7572 736f 722e 636f 6e6e 6563  rn cursor.connec
-000194a0: 7469 6f6e 0a20 2020 2020 2020 2065 7863  tion.        exc
-000194b0: 6570 7420 4b65 7962 6f61 7264 496e 7465  ept KeyboardInte
-000194c0: 7272 7570 743a 0a20 2020 2020 2020 2020  rrupt:.         
-000194d0: 2020 2070 7269 6e74 2822 4f70 6572 6174     print("Operat
-000194e0: 696f 6e20 696e 7465 7272 7570 7465 642e  ion interrupted.
-000194f0: 2229 0a20 2020 2020 2020 2020 2020 2063  ").            c
-00019500: 7572 5f63 6f6e 6e20 3d20 6375 7273 6f72  ur_conn = cursor
-00019510: 2e63 6f6e 6e65 6374 696f 6e0a 2020 2020  .connection.    
-00019520: 2020 2020 2020 2020 6375 725f 636f 6e6e          cur_conn
-00019530: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
-00019540: 2020 2020 2072 6574 7572 6e20 436f 6e6e       return Conn
-00019550: 6563 7469 6f6e 280a 2020 2020 2020 2020  ection(.        
-00019560: 2020 2020 2020 2020 7573 6572 3d63 7572          user=cur
-00019570: 5f63 6f6e 6e2e 7573 6572 2c0a 2020 2020  _conn.user,.    
-00019580: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-00019590: 776f 7264 3d63 7572 5f63 6f6e 6e2e 7061  word=cur_conn.pa
-000195a0: 7373 776f 7264 2c0a 2020 2020 2020 2020  ssword,.        
-000195b0: 2020 2020 2020 2020 686f 7374 3d22 2c22          host=","
-000195c0: 2e6a 6f69 6e28 6375 725f 636f 6e6e 2e68  .join(cur_conn.h
-000195d0: 6f73 7473 292c 0a20 2020 2020 2020 2020  osts),.         
-000195e0: 2020 2020 2020 2064 6174 6162 6173 653d         database=
-000195f0: 6375 725f 636f 6e6e 2e64 6174 6162 6173  cur_conn.databas
-00019600: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00019610: 2020 2074 6c73 3d63 7572 5f63 6f6e 6e2e     tls=cur_conn.
-00019620: 746c 732c 0a20 2020 2020 2020 2020 2020  tls,.           
-00019630: 2020 2020 2068 616e 6473 6861 6b65 3d63       handshake=c
-00019640: 7572 5f63 6f6e 6e2e 6861 6e64 7368 616b  ur_conn.handshak
-00019650: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00019660: 2020 2066 6f72 6365 3d63 7572 5f63 6f6e     force=cur_con
-00019670: 6e2e 666f 7263 652c 0a20 2020 2020 2020  n.force,.       
-00019680: 2020 2020 2020 2020 2073 6573 7369 6f6e           session
-00019690: 3d63 7572 5f63 6f6e 6e2e 7365 7373 696f  =cur_conn.sessio
-000196a0: 6e2c 0a20 2020 2020 2020 2020 2020 2029  n,.            )
-000196b0: 0a0a 2020 2020 2020 2020 6966 2061 7267  ..        if arg
-000196c0: 732e 7469 6d65 3a0a 2020 2020 2020 2020  s.time:.        
-000196d0: 2020 2020 656e 6474 696d 6520 3d20 7469      endtime = ti
-000196e0: 6d65 5f6e 7328 290a 0a20 2020 2020 2020  me_ns()..       
-000196f0: 2069 6620 6375 7273 6f72 2e64 6573 6372   if cursor.descr
-00019700: 6970 7469 6f6e 2069 7320 4e6f 6e65 3a0a  iption is None:.
-00019710: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00019720: 7428 224f 4b22 290a 0a20 2020 2020 2020  t("OK")..       
-00019730: 2065 6c69 6620 6172 6773 2e6f 7574 6669   elif args.outfi
-00019740: 6c65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  le is not None:.
-00019750: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00019760: 6375 7273 6f72 2e65 7870 6c61 696e 5f72  cursor.explain_r
-00019770: 6573 756c 743a 0a20 2020 2020 2020 2020  esult:.         
-00019780: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00019790: 5b7b 2265 7870 6c61 696e 223a 206a 736f  [{"explain": jso
-000197a0: 6e2e 6c6f 6164 7328 6375 7273 6f72 2e65  n.loads(cursor.e
-000197b0: 7870 6c61 696e 5f72 6573 756c 7429 7d5d  xplain_result)}]
-000197c0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000197d0: 2020 7072 696e 7428 6a73 6f6e 2e64 756d    print(json.dum
-000197e0: 7073 2872 6573 756c 742c 2069 6e64 656e  ps(result, inden
-000197f0: 743d 342c 2064 6566 6175 6c74 3d5f 6375  t=4, default=_cu
-00019800: 7374 6f6d 5f74 7970 655f 746f 5f6a 736f  stom_type_to_jso
-00019810: 6e29 2c20 6669 6c65 3d61 7267 732e 6f75  n), file=args.ou
-00019820: 7466 696c 6529 0a20 2020 2020 2020 2020  tfile).         
-00019830: 2020 2065 6c69 6620 7265 7375 6c74 3a0a     elif result:.
-00019840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019850: 6966 2061 7267 732e 666f 726d 6174 203d  if args.format =
-00019860: 3d20 226a 736f 6e22 3a0a 2020 2020 2020  = "json":.      
-00019870: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00019880: 7375 6c74 203d 205b 726f 772e 5f61 7364  sult = [row._asd
-00019890: 6963 7428 2920 666f 7220 726f 7720 696e  ict() for row in
-000198a0: 2072 6573 756c 745d 0a0a 2020 2020 2020   result]..      
-000198b0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-000198c0: 696e 7428 6a73 6f6e 2e64 756d 7073 2872  int(json.dumps(r
-000198d0: 6573 756c 742c 2069 6e64 656e 743d 342c  esult, indent=4,
-000198e0: 2064 6566 6175 6c74 3d5f 6375 7374 6f6d   default=_custom
-000198f0: 5f74 7970 655f 746f 5f6a 736f 6e29 2c20  _type_to_json), 
-00019900: 6669 6c65 3d61 7267 732e 6f75 7466 696c  file=args.outfil
-00019910: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00019920: 2020 2065 6c69 6620 6172 6773 2e66 6f72     elif args.for
-00019930: 6d61 7420 3d3d 2022 7461 626c 6522 3a0a  mat == "table":.
-00019940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019950: 2020 2020 7072 696e 7428 7461 6275 6c61      print(tabula
-00019960: 7465 2872 6573 756c 742c 2068 6561 6465  te(result, heade
-00019970: 7273 3d5b 635b 305d 2066 6f72 2063 2069  rs=[c[0] for c i
-00019980: 6e20 6375 7273 6f72 2e64 6573 6372 6970  n cursor.descrip
-00019990: 7469 6f6e 5d2c 2074 6162 6c65 666d 743d  tion], tablefmt=
-000199a0: 2270 7371 6c22 292c 2066 696c 653d 6172  "psql"), file=ar
-000199b0: 6773 2e6f 7574 6669 6c65 290a 2020 2020  gs.outfile).    
-000199c0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-000199d0: 2061 7267 732e 666f 726d 6174 203d 3d20   args.format == 
-000199e0: 2263 7376 223a 0a20 2020 2020 2020 2020  "csv":.         
-000199f0: 2020 2020 2020 2020 2020 2063 7376 2e77             csv.w
-00019a00: 7269 7465 7228 6172 6773 2e6f 7574 6669  riter(args.outfi
-00019a10: 6c65 2c20 7175 6f74 696e 673d 6373 762e  le, quoting=csv.
-00019a20: 5155 4f54 455f 414c 4c29 2e77 7269 7465  QUOTE_ALL).write
-00019a30: 726f 7728 5b63 5b30 5d20 666f 7220 6320  row([c[0] for c 
-00019a40: 696e 2063 7572 736f 722e 6465 7363 7269  in cursor.descri
-00019a50: 7074 696f 6e5d 290a 2020 2020 2020 2020  ption]).        
-00019a60: 2020 2020 2020 2020 2020 2020 7772 6974              writ
-00019a70: 6572 203d 2063 7376 2e77 7269 7465 7228  er = csv.writer(
-00019a80: 6172 6773 2e6f 7574 6669 6c65 290a 2020  args.outfile).  
-00019a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019aa0: 2020 666f 7220 726f 7720 696e 2072 6573    for row in res
-00019ab0: 756c 743a 0a20 2020 2020 2020 2020 2020  ult:.           
-00019ac0: 2020 2020 2020 2020 2020 2020 2077 7269               wri
-00019ad0: 7465 722e 7772 6974 6572 6f77 2872 6f77  ter.writerow(row
-00019ae0: 290a 0a20 2020 2020 2020 2069 6620 6172  )..        if ar
-00019af0: 6773 2e74 696d 653a 0a20 2020 2020 2020  gs.time:.       
-00019b00: 2020 2020 2065 6e64 7469 6d65 203d 2074       endtime = t
-00019b10: 696d 655f 6e73 2829 0a20 2020 2020 2020  ime_ns().       
-00019b20: 2020 2020 2070 7269 6e74 2866 2245 7865       print(f"Exe
-00019b30: 6375 7469 6f6e 2074 696d 653a 207b 2865  cution time: {(e
-00019b40: 6e64 7469 6d65 202d 2073 7461 7274 7469  ndtime - startti
-00019b50: 6d65 292f 3130 3030 3030 3030 3030 3a2e  me)/1000000000:.
-00019b60: 3366 7d20 7365 636f 6e64 7322 290a 2020  3f} seconds").  
-00019b70: 2020 2020 2020 2320 4966 2077 6520 646f        # If we do
-00019b80: 6e27 7420 7265 7475 726e 2074 6869 7320  n't return this 
-00019b90: 636f 6e6e 6563 7469 6f6e 2c20 7468 656e  connection, then
-00019ba0: 2077 6520 656e 6420 7570 2075 7369 6e67   we end up using
-00019bb0: 2074 6865 206f 6c64 2063 6f6e 6e65 6374   the old connect
-00019bc0: 696f 6e20 7768 6963 6820 7765 2063 6f75  ion which we cou
-00019bd0: 6c64 2068 6176 6520 6265 656e 2072 6564  ld have been red
-00019be0: 6972 6563 7465 640a 2020 2020 2020 2020  irected.        
-00019bf0: 7265 7475 726e 2063 7572 736f 722e 636f  return cursor.co
-00019c00: 6e6e 6563 7469 6f6e 0a0a 2020 2020 6465  nnection..    de
-00019c10: 6620 5f64 6f5f 7265 706c 2861 7267 732c  f _do_repl(args,
-00019c20: 2063 6f6e 6e65 6374 696f 6e29 3a0a 2020   connection):.  
-00019c30: 2020 2020 2020 6672 6f6d 2070 726f 6d70        from promp
-00019c40: 745f 746f 6f6c 6b69 7420 696d 706f 7274  t_toolkit import
-00019c50: 2050 726f 6d70 7453 6573 7369 6f6e 0a20   PromptSession. 
-00019c60: 2020 2020 2020 2066 726f 6d20 7072 6f6d         from prom
-00019c70: 7074 5f74 6f6f 6c6b 6974 2e6c 6578 6572  pt_toolkit.lexer
-00019c80: 7320 696d 706f 7274 2050 7967 6d65 6e74  s import Pygment
-00019c90: 734c 6578 6572 0a20 2020 2020 2020 2066  sLexer.        f
-00019ca0: 726f 6d20 7072 6f6d 7074 5f74 6f6f 6c6b  rom prompt_toolk
-00019cb0: 6974 2e68 6973 746f 7279 2069 6d70 6f72  it.history impor
-00019cc0: 7420 4669 6c65 4869 7374 6f72 790a 2020  t FileHistory.  
-00019cd0: 2020 2020 2020 6672 6f6d 2070 6174 686c        from pathl
-00019ce0: 6962 2069 6d70 6f72 7420 5061 7468 0a0a  ib import Path..
-00019cf0: 2020 2020 2020 2020 7371 6c5f 7374 6d74          sql_stmt
-00019d00: 203d 2022 220a 0a20 2020 2020 2020 2069   = ""..        i
-00019d10: 6620 6172 6773 2e6e 6f63 6f6c 6f72 3a0a  f args.nocolor:.
-00019d20: 2020 2020 2020 2020 2020 2020 7365 7373              sess
-00019d30: 696f 6e20 3d20 5072 6f6d 7074 5365 7373  ion = PromptSess
-00019d40: 696f 6e28 6869 7374 6f72 793d 4669 6c65  ion(history=File
-00019d50: 4869 7374 6f72 7928 7374 7228 5061 7468  History(str(Path
-00019d60: 2e68 6f6d 6528 2920 2f20 222e 7079 6f63  .home() / ".pyoc
-00019d70: 6965 6e74 5f68 6973 746f 7279 2229 2929  ient_history")))
-00019d80: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00019d90: 2020 2020 2020 2020 2020 2073 6573 7369             sessi
-00019da0: 6f6e 203d 2050 726f 6d70 7453 6573 7369  on = PromptSessi
-00019db0: 6f6e 286c 6578 6572 3d50 7967 6d65 6e74  on(lexer=Pygment
-00019dc0: 734c 6578 6572 2853 716c 4c65 7865 7229  sLexer(SqlLexer)
-00019dd0: 2c20 6869 7374 6f72 793d 4669 6c65 4869  , history=FileHi
-00019de0: 7374 6f72 7928 7374 7228 5061 7468 2e68  story(str(Path.h
-00019df0: 6f6d 6528 2920 2f20 222e 7079 6f63 6965  ome() / ".pyocie
-00019e00: 6e74 5f68 6973 746f 7279 2229 2929 0a0a  nt_history")))..
-00019e10: 2020 2020 2020 2020 6966 2063 6f6e 6e65          if conne
-00019e20: 6374 696f 6e3a 0a20 2020 2020 2020 2020  ction:.         
-00019e30: 2020 2063 7572 736f 7220 3d20 636f 6e6e     cursor = conn
-00019e40: 6563 7469 6f6e 2e63 7572 736f 7228 290a  ection.cursor().
-00019e50: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00019e60: 7428 6622 4f63 6965 6e74 2044 6174 6162  t(f"Ocient Datab
-00019e70: 6173 65e2 84a2 2229 0a20 2020 2020 2020  ase...").       
-00019e80: 2020 2020 2070 7269 6e74 2866 2253 7973       print(f"Sys
-00019e90: 7465 6d20 5665 7273 696f 6e3a 207b 6375  tem Version: {cu
-00019ea0: 7273 6f72 2e67 6574 5379 7374 656d 5665  rsor.getSystemVe
-00019eb0: 7273 696f 6e28 297d 2c20 436c 6965 6e74  rsion()}, Client
-00019ec0: 2056 6572 7369 6f6e 207b 7665 7273 696f   Version {versio
-00019ed0: 6e7d 2229 0a20 2020 2020 2020 2065 6f66  n}").        eof
-00019ee0: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
-00019ef0: 2074 6578 7420 3d20 2222 0a20 2020 2020   text = "".     
-00019f00: 2020 2077 6869 6c65 206e 6f74 2065 6f66     while not eof
-00019f10: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
-00019f20: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-00019f30: 2020 2074 6578 7420 3d20 7365 7373 696f     text = sessio
-00019f40: 6e2e 7072 6f6d 7074 2822 3e20 2229 0a20  n.prompt("> "). 
-00019f50: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-00019f60: 7420 4b65 7962 6f61 7264 496e 7465 7272  t KeyboardInterr
-00019f70: 7570 743a 0a20 2020 2020 2020 2020 2020  upt:.           
-00019f80: 2020 2020 2073 716c 5f73 746d 7420 3d20       sql_stmt = 
-00019f90: 2222 0a20 2020 2020 2020 2020 2020 2020  "".             
-00019fa0: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
-00019fb0: 2020 2020 2020 2020 6578 6365 7074 2045          except E
-00019fc0: 4f46 4572 726f 723a 0a20 2020 2020 2020  OFError:.       
-00019fd0: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
-00019fe0: 2020 2020 2020 2020 2020 2028 7371 6c5f             (sql_
-00019ff0: 7374 6d74 2c20 636f 6e6e 6563 7469 6f6e  stmt, connection
-0001a000: 2920 3d20 5f64 6f5f 6c69 6e65 2861 7267  ) = _do_line(arg
-0001a010: 732c 2063 6f6e 6e65 6374 696f 6e2c 2074  s, connection, t
-0001a020: 6578 742c 2073 716c 5f73 746d 742c 205f  ext, sql_stmt, _
-0001a030: 646f 5f71 7565 7279 290a 0a20 2020 2020  do_query)..     
-0001a040: 2020 2069 6620 6c65 6e28 7371 6c5f 7374     if len(sql_st
-0001a050: 6d74 2e73 7472 6970 2829 293a 0a20 2020  mt.strip()):.   
-0001a060: 2020 2020 2020 2020 2063 6f6e 6e65 6374           connect
-0001a070: 696f 6e20 3d20 5f64 6f5f 7175 6572 7928  ion = _do_query(
-0001a080: 6172 6773 2c20 636f 6e6e 6563 7469 6f6e  args, connection
-0001a090: 2c20 7371 6c5f 7374 6d74 290a 0a20 2020  , sql_stmt)..   
-0001a0a0: 2020 2020 2070 7269 6e74 2822 476f 6f64       print("Good
-0001a0b0: 4279 6521 2229 0a0a 2020 2020 7472 793a  Bye!")..    try:
-0001a0c0: 0a20 2020 2020 2020 2069 6620 6172 6773  .        if args
-0001a0d0: 2e64 736e 3a0a 2020 2020 2020 2020 2020  .dsn:.          
-0001a0e0: 2020 636f 6e6e 6563 7469 6f6e 203d 2063    connection = c
-0001a0f0: 6f6e 6e65 6374 2861 7267 732e 6473 6e2c  onnect(args.dsn,
-0001a100: 2063 6f6e 6669 6766 696c 653d 6172 6773   configfile=args
-0001a110: 2e63 6f6e 6669 6766 696c 6529 0a20 2020  .configfile).   
-0001a120: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0001a130: 2020 2020 2020 2063 6f6e 6e65 6374 696f         connectio
-0001a140: 6e20 3d20 4e6f 6e65 0a0a 2020 2020 2020  n = None..      
-0001a150: 2020 6966 2061 7267 732e 7371 6c3a 0a20    if args.sql:. 
-0001a160: 2020 2020 2020 2020 2020 2063 6f6e 6e65             conne
-0001a170: 6374 696f 6e20 3d20 5f64 6f5f 7175 6572  ction = _do_quer
-0001a180: 7928 6172 6773 2c20 636f 6e6e 6563 7469  y(args, connecti
-0001a190: 6f6e 2c20 6172 6773 2e73 716c 290a 2020  on, args.sql).  
-0001a1a0: 2020 2020 2020 656c 6966 2061 7267 732e        elif args.
-0001a1b0: 696e 6669 6c65 3a0a 2020 2020 2020 2020  infile:.        
-0001a1c0: 2020 2020 2873 716c 5f73 746d 742c 2063      (sql_stmt, c
-0001a1d0: 6f6e 6e65 6374 696f 6e29 203d 205f 646f  onnection) = _do
-0001a1e0: 5f6c 696e 6528 6172 6773 2c20 636f 6e6e  _line(args, conn
-0001a1f0: 6563 7469 6f6e 2c20 6172 6773 2e69 6e66  ection, args.inf
-0001a200: 696c 652e 7265 6164 2829 2c20 7371 6c5f  ile.read(), sql_
-0001a210: 7374 6d74 2c20 5f64 6f5f 7175 6572 7929  stmt, _do_query)
-0001a220: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0001a230: 6c65 6e28 7371 6c5f 7374 6d74 2e73 7472  len(sql_stmt.str
-0001a240: 6970 2829 293a 0a20 2020 2020 2020 2020  ip()):.         
-0001a250: 2020 2020 2020 2063 6f6e 6e65 6374 696f         connectio
-0001a260: 6e20 3d20 5f64 6f5f 7175 6572 7928 6172  n = _do_query(ar
-0001a270: 6773 2c20 636f 6e6e 6563 7469 6f6e 2c20  gs, connection, 
-0001a280: 7371 6c5f 7374 6d74 290a 2020 2020 2020  sql_stmt).      
-0001a290: 2020 656c 6966 2073 7973 2e73 7464 696e    elif sys.stdin
-0001a2a0: 2e69 7361 7474 7928 293a 0a20 2020 2020  .isatty():.     
-0001a2b0: 2020 2020 2020 205f 646f 5f72 6570 6c28         _do_repl(
-0001a2c0: 6172 6773 2c20 636f 6e6e 6563 7469 6f6e  args, connection
-0001a2d0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-0001a2e0: 2020 2020 2020 2020 2020 2020 2873 716c              (sql
-0001a2f0: 5f73 746d 742c 2063 6f6e 6e65 6374 696f  _stmt, connectio
-0001a300: 6e29 203d 205f 646f 5f6c 696e 6528 6172  n) = _do_line(ar
-0001a310: 6773 2c20 636f 6e6e 6563 7469 6f6e 2c20  gs, connection, 
-0001a320: 7379 732e 7374 6469 6e2e 7265 6164 2829  sys.stdin.read()
-0001a330: 2c20 7371 6c5f 7374 6d74 2c20 5f64 6f5f  , sql_stmt, _do_
-0001a340: 7175 6572 7929 0a0a 2020 2020 6578 6365  query)..    exce
-0001a350: 7074 2053 514c 4578 6365 7074 696f 6e20  pt SQLException 
-0001a360: 6173 2065 7863 3a0a 2020 2020 2020 2020  as exc:.        
-0001a370: 7072 696e 7428 6622 4572 726f 723a 207b  print(f"Error: {
-0001a380: 6578 632e 7265 6173 6f6e 7d22 2c20 6669  exc.reason}", fi
-0001a390: 6c65 3d73 7973 2e73 7464 6572 7229 0a0a  le=sys.stderr)..
-0001a3a0: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
-0001a3b0: 225f 5f6d 6169 6e5f 5f22 3a0a 2020 2020  "__main__":.    
-0001a3c0: 6d61 696e 2829 0a                        main().
+00000010: 7974 686f 6e33 0a0a 696d 706f 7274 2063  ython3..import c
+00000020: 6f6e 6669 6770 6172 7365 720a 696d 706f  onfigparser.impo
+00000030: 7274 2064 6174 6574 696d 650a 696d 706f  rt datetime.impo
+00000040: 7274 2064 6563 696d 616c 0a69 6d70 6f72  rt decimal.impor
+00000050: 7420 6970 6164 6472 6573 730a 696d 706f  t ipaddress.impo
+00000060: 7274 206c 6f67 6769 6e67 0a69 6d70 6f72  rt logging.impor
+00000070: 7420 7265 0a69 6d70 6f72 7420 736f 636b  t re.import sock
+00000080: 6574 0a69 6d70 6f72 7420 7373 6c0a 696d  et.import ssl.im
+00000090: 706f 7274 2073 7472 7563 740a 0a23 2070  port struct..# p
+000000a0: 796c 696e 743a 2064 6973 6162 6c65 3d74  ylint: disable=t
+000000b0: 6f6f 2d6d 616e 792d 6c69 6e65 730a 696d  oo-many-lines.im
+000000c0: 706f 7274 2073 7973 0a69 6d70 6f72 7420  port sys.import 
+000000d0: 7575 6964 0a66 726f 6d20 636f 6c6c 6563  uuid.from collec
+000000e0: 7469 6f6e 7320 696d 706f 7274 206e 616d  tions import nam
+000000f0: 6564 7475 706c 650a 6672 6f6d 206d 6174  edtuple.from mat
+00000100: 6820 696d 706f 7274 2069 7369 6e66 0a66  h import isinf.f
+00000110: 726f 6d20 7469 6d65 2069 6d70 6f72 7420  rom time import 
+00000120: 736c 6565 702c 2074 696d 655f 6e73 0a66  sleep, time_ns.f
+00000130: 726f 6d20 7479 7065 7320 696d 706f 7274  rom types import
+00000140: 2054 7261 6365 6261 636b 5479 7065 0a66   TracebackType.f
+00000150: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+00000160: 7420 280a 2020 2020 416e 792c 0a20 2020  t (.    Any,.   
+00000170: 2043 616c 6c61 626c 652c 0a20 2020 2047   Callable,.    G
+00000180: 656e 6572 6963 2c0a 2020 2020 4974 6572  eneric,.    Iter
+00000190: 6162 6c65 2c0a 2020 2020 4c69 7374 2c0a  able,.    List,.
+000001a0: 2020 2020 4d61 7070 696e 672c 0a20 2020      Mapping,.   
+000001b0: 204e 616d 6564 5475 706c 652c 0a20 2020   NamedTuple,.   
+000001c0: 204f 7074 696f 6e61 6c2c 0a20 2020 2053   Optional,.    S
+000001d0: 6571 7565 6e63 652c 0a20 2020 2054 7570  equence,.    Tup
+000001e0: 6c65 2c0a 2020 2020 5479 7065 2c0a 2020  le,.    Type,.  
+000001f0: 2020 5479 7065 5661 722c 0a20 2020 2055    TypeVar,.    U
+00000200: 6e69 6f6e 2c0a 2020 2020 6361 7374 2c0a  nion,.    cast,.
+00000210: 290a 6672 6f6d 2077 6172 6e69 6e67 7320  ).from warnings 
+00000220: 696d 706f 7274 2077 6172 6e0a 0a69 6d70  import warn..imp
+00000230: 6f72 7420 6473 6e70 6172 7365 2020 2320  ort dsnparse  # 
+00000240: 7479 7065 3a20 6967 6e6f 7265 0a66 726f  type: ignore.fro
+00000250: 6d20 6372 7970 746f 6772 6170 6879 2e68  m cryptography.h
+00000260: 617a 6d61 742e 6261 636b 656e 6473 2069  azmat.backends i
+00000270: 6d70 6f72 7420 6465 6661 756c 745f 6261  mport default_ba
+00000280: 636b 656e 640a 6672 6f6d 2063 7279 7074  ckend.from crypt
+00000290: 6f67 7261 7068 792e 6861 7a6d 6174 2e70  ography.hazmat.p
+000002a0: 7269 6d69 7469 7665 7320 696d 706f 7274  rimitives import
+000002b0: 2068 6173 6865 732c 2068 6d61 632c 2070   hashes, hmac, p
+000002c0: 6164 6469 6e67 2c20 7365 7269 616c 697a  adding, serializ
+000002d0: 6174 696f 6e0a 6672 6f6d 2063 7279 7074  ation.from crypt
+000002e0: 6f67 7261 7068 792e 6861 7a6d 6174 2e70  ography.hazmat.p
+000002f0: 7269 6d69 7469 7665 732e 6173 796d 6d65  rimitives.asymme
+00000300: 7472 6963 2e64 6820 696d 706f 7274 2044  tric.dh import D
+00000310: 4850 7562 6c69 634b 6579 0a66 726f 6d20  HPublicKey.from 
+00000320: 6372 7970 746f 6772 6170 6879 2e68 617a  cryptography.haz
+00000330: 6d61 742e 7072 696d 6974 6976 6573 2e63  mat.primitives.c
+00000340: 6970 6865 7273 2069 6d70 6f72 7420 4369  iphers import Ci
+00000350: 7068 6572 2c20 616c 676f 7269 7468 6d73  pher, algorithms
+00000360: 2c20 6d6f 6465 730a 6672 6f6d 2063 7279  , modes.from cry
+00000370: 7074 6f67 7261 7068 792e 6861 7a6d 6174  ptography.hazmat
+00000380: 2e70 7269 6d69 7469 7665 732e 7365 7269  .primitives.seri
+00000390: 616c 697a 6174 696f 6e20 696d 706f 7274  alization import
+000003a0: 206c 6f61 645f 7065 6d5f 7075 626c 6963   load_pem_public
+000003b0: 5f6b 6579 0a66 726f 6d20 676f 6f67 6c65  _key.from google
+000003c0: 2e70 726f 746f 6275 662e 696e 7465 726e  .protobuf.intern
+000003d0: 616c 2e63 6f6e 7461 696e 6572 7320 696d  al.containers im
+000003e0: 706f 7274 2052 6570 6561 7465 6443 6f6d  port RepeatedCom
+000003f0: 706f 7369 7465 4669 656c 6443 6f6e 7461  positeFieldConta
+00000400: 696e 6572 0a66 726f 6d20 676f 6f67 6c65  iner.from google
+00000410: 2e70 726f 746f 6275 662e 6d65 7373 6167  .protobuf.messag
+00000420: 6520 696d 706f 7274 204d 6573 7361 6765  e import Message
+00000430: 0a0a 6672 6f6d 2070 796f 6369 656e 742e  ..from pyocient.
+00000440: 706b 675f 7665 7273 696f 6e20 696d 706f  pkg_version impo
+00000450: 7274 205f 5f76 6572 7369 6f6e 5f5f 2061  rt __version__ a
+00000460: 7320 7665 7273 696f 6e0a 0a5f 5420 3d20  s version.._T = 
+00000470: 5479 7065 5661 7228 225f 5422 290a 5f4d  TypeVar("_T")._M
+00000480: 7367 5420 3d20 5479 7065 5661 7228 225f  sgT = TypeVar("_
+00000490: 4d73 6754 222c 2062 6f75 6e64 3d4d 6573  MsgT", bound=Mes
+000004a0: 7361 6765 290a 0a6c 6f67 6765 7220 3d20  sage)..logger = 
+000004b0: 6c6f 6767 696e 672e 6765 744c 6f67 6765  logging.getLogge
+000004c0: 7228 2270 796f 6369 656e 7422 290a 0a23  r("pyocient")..#
+000004d0: 2053 6565 2050 4550 2032 3439 2066 6f72   See PEP 249 for
+000004e0: 2074 6865 2076 616c 7565 7320 6f66 2074   the values of t
+000004f0: 6865 7365 2061 7474 7269 6275 7465 730a  hese attributes.
+00000500: 6170 696c 6576 656c 203d 2022 322e 3022  apilevel = "2.0"
+00000510: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
+00000520: 626c 653d 696e 7661 6c69 642d 6e61 6d65  ble=invalid-name
+00000530: 0a74 6872 6561 6473 6166 6574 7920 3d20  .threadsafety = 
+00000540: 3120 2023 2070 796c 696e 743a 2064 6973  1  # pylint: dis
+00000550: 6162 6c65 3d69 6e76 616c 6964 2d6e 616d  able=invalid-nam
+00000560: 650a 7061 7261 6d73 7479 6c65 203d 2022  e.paramstyle = "
+00000570: 7079 666f 726d 6174 2220 2023 2070 796c  pyformat"  # pyl
+00000580: 696e 743a 2064 6973 6162 6c65 3d69 6e76  int: disable=inv
+00000590: 616c 6964 2d6e 616d 650a 4452 4956 4552  alid-name.DRIVER
+000005a0: 5f49 4420 3d20 2270 796f 6369 656e 7422  _ID = "pyocient"
+000005b0: 0a50 524f 544f 434f 4c5f 5645 5253 494f  .PROTOCOL_VERSIO
+000005c0: 4e20 3d20 2237 2e30 2e31 220a 5345 5353  N = "7.0.1".SESS
+000005d0: 494f 4e5f 4558 5049 5245 445f 434f 4445  ION_EXPIRED_CODE
+000005e0: 203d 202d 3733 330a 0a70 6172 7473 203d   = -733..parts =
+000005f0: 2076 6572 7369 6f6e 2e73 706c 6974 2822   version.split("
+00000600: 2e22 290a 7665 7273 696f 6e5f 6d61 6a6f  .").version_majo
+00000610: 7220 3d20 696e 7428 7061 7274 735b 305d  r = int(parts[0]
+00000620: 290a 7665 7273 696f 6e5f 6d69 6e6f 7220  ).version_minor 
+00000630: 3d20 696e 7428 7061 7274 735b 315d 290a  = int(parts[1]).
+00000640: 0a0a 636c 6173 7320 5351 4c45 7863 6570  ..class SQLExcep
+00000650: 7469 6f6e 2845 7863 6570 7469 6f6e 293a  tion(Exception):
+00000660: 0a20 2020 2022 2222 4261 7365 2065 7863  .    """Base exc
+00000670: 6570 7469 6f6e 2066 6f72 2061 6c6c 204f  eption for all O
+00000680: 6369 656e 7420 6578 6365 7074 696f 6e73  cient exceptions
+00000690: 2e0a 0a20 2020 2041 7474 7269 6275 7465  ...    Attribute
+000006a0: 733a 0a0a 2020 2020 2d20 7371 6c5f 7374  s:..    - sql_st
+000006b0: 6174 653a 2054 6865 2053 514c 5354 4154  ate: The SQLSTAT
+000006c0: 4520 6465 6669 6e65 6420 696e 2074 6865  E defined in the
+000006d0: 2053 514c 2073 7461 6e64 6172 640a 2020   SQL standard.  
+000006e0: 2020 2d20 7265 6173 6f6e 3a20 4120 7374    - reason: A st
+000006f0: 7269 6e67 2064 6573 6372 6970 7469 6f6e  ring description
+00000700: 206f 6620 7468 6520 6578 6365 7074 696f   of the exceptio
+00000710: 6e0a 2020 2020 2d20 7665 6e64 6f72 5f63  n.    - vendor_c
+00000720: 6f64 653a 2041 6e20 4f63 6965 6e74 2073  ode: An Ocient s
+00000730: 7065 6369 6669 6320 6572 726f 7220 636f  pecific error co
+00000740: 6465 0a20 2020 2022 2222 0a0a 2020 2020  de.    """..    
+00000750: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00000760: 662c 2072 6561 736f 6e3a 2073 7472 203d  f, reason: str =
+00000770: 2022 222c 2073 716c 5f73 7461 7465 3a20   "", sql_state: 
+00000780: 7374 7220 3d20 2230 3030 3030 222c 2076  str = "00000", v
+00000790: 656e 646f 725f 636f 6465 3a20 696e 7420  endor_code: int 
+000007a0: 3d20 3029 202d 3e20 4e6f 6e65 3a0a 2020  = 0) -> None:.  
+000007b0: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
+000007c0: 696e 6974 5f5f 2829 0a20 2020 2020 2020  init__().       
+000007d0: 2073 656c 662e 7371 6c5f 7374 6174 6520   self.sql_state 
+000007e0: 3d20 7371 6c5f 7374 6174 650a 2020 2020  = sql_state.    
+000007f0: 2020 2020 7365 6c66 2e72 6561 736f 6e20      self.reason 
+00000800: 3d20 7265 6173 6f6e 0a20 2020 2020 2020  = reason.       
+00000810: 2073 656c 662e 7665 6e64 6f72 5f63 6f64   self.vendor_cod
+00000820: 6520 3d20 7665 6e64 6f72 5f63 6f64 650a  e = vendor_code.
+00000830: 0a20 2020 2064 6566 205f 5f73 7472 5f5f  .    def __str__
+00000840: 2873 656c 6629 202d 3e20 7374 723a 0a20  (self) -> str:. 
+00000850: 2020 2020 2020 2072 6574 7572 6e20 6622         return f"
+00000860: 5374 6174 653a 207b 7365 6c66 2e73 716c  State: {self.sql
+00000870: 5f73 7461 7465 7d20 436f 6465 3a20 7b73  _state} Code: {s
+00000880: 656c 662e 7665 6e64 6f72 5f63 6f64 657d  elf.vendor_code}
+00000890: 2052 6561 736f 6e3a 207b 7365 6c66 2e72   Reason: {self.r
+000008a0: 6561 736f 6e7d 220a 0a0a 2323 2323 2323  eason}"...######
+000008b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000008c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000008d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000008e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000008f0: 2323 230a 2320 4461 7461 6261 7365 2041  ###.# Database A
+00000900: 5049 2032 2e30 2065 7863 6570 7469 6f6e  PI 2.0 exception
+00000910: 732e 2020 5468 6573 6520 6172 6520 7265  s.  These are re
+00000920: 7175 6972 6564 2062 7920 5045 4d20 3234  quired by PEM 24
+00000930: 390a 2323 2323 2323 2323 2323 2323 2323  9.##############
+00000940: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000950: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000960: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000970: 2323 2323 2323 2323 2323 230a 0a0a 636c  ###########...cl
+00000980: 6173 7320 4572 726f 7228 5351 4c45 7863  ass Error(SQLExc
+00000990: 6570 7469 6f6e 293a 0a20 2020 2022 2222  eption):.    """
+000009a0: 4578 6365 7074 696f 6e20 7468 6174 2069  Exception that i
+000009b0: 7320 7468 6520 6261 7365 2063 6c61 7373  s the base class
+000009c0: 206f 6620 616c 6c20 6f74 6865 7220 6572   of all other er
+000009d0: 726f 7220 6578 6365 7074 696f 6e73 2e22  ror exceptions."
+000009e0: 2222 0a0a 2020 2020 6465 6620 5f5f 696e  ""..    def __in
+000009f0: 6974 5f5f 2873 656c 662c 2072 6561 736f  it__(self, reaso
+00000a00: 6e3a 2073 7472 2c20 7371 6c5f 7374 6174  n: str, sql_stat
+00000a10: 653a 2073 7472 203d 2022 3538 3030 3522  e: str = "58005"
+00000a20: 2c20 7665 6e64 6f72 5f63 6f64 653a 2069  , vendor_code: i
+00000a30: 6e74 203d 202d 3130 3029 202d 3e20 4e6f  nt = -100) -> No
+00000a40: 6e65 3a0a 2020 2020 2020 2020 7375 7065  ne:.        supe
+00000a50: 7228 292e 5f5f 696e 6974 5f5f 2872 6561  r().__init__(rea
+00000a60: 736f 6e2c 2073 716c 5f73 7461 7465 3d73  son, sql_state=s
+00000a70: 716c 5f73 7461 7465 2c20 7665 6e64 6f72  ql_state, vendor
+00000a80: 5f63 6f64 653d 7665 6e64 6f72 5f63 6f64  _code=vendor_cod
+00000a90: 6529 0a0a 0a63 6c61 7373 2057 6172 6e69  e)...class Warni
+00000aa0: 6e67 2853 514c 4578 6365 7074 696f 6e29  ng(SQLException)
+00000ab0: 3a20 2023 2070 796c 696e 743a 2064 6973  :  # pylint: dis
+00000ac0: 6162 6c65 3d72 6564 6566 696e 6564 2d62  able=redefined-b
+00000ad0: 7569 6c74 696e 0a20 2020 2022 2222 4578  uiltin.    """Ex
+00000ae0: 6365 7074 696f 6e20 7468 6174 2069 7320  ception that is 
+00000af0: 7468 6520 6261 7365 2063 6c61 7373 206f  the base class o
+00000b00: 6620 616c 6c20 6f74 6865 7220 7761 726e  f all other warn
+00000b10: 696e 6720 6578 6365 7074 696f 6e73 2e22  ing exceptions."
+00000b20: 2222 0a0a 0a63 6c61 7373 2049 6e74 6572  ""...class Inter
+00000b30: 6661 6365 4572 726f 7228 4572 726f 7229  faceError(Error)
+00000b40: 3a0a 2020 2020 2222 2245 7863 6570 7469  :.    """Excepti
+00000b50: 6f6e 2072 6169 7365 6420 666f 7220 6572  on raised for er
+00000b60: 726f 7273 2074 6861 7420 6172 6520 7265  rors that are re
+00000b70: 6c61 7465 6420 746f 2074 6865 0a20 2020  lated to the.   
+00000b80: 2064 6174 6162 6173 6520 696e 7465 7266   database interf
+00000b90: 6163 6520 7261 7468 6572 2074 6861 6e20  ace rather than 
+00000ba0: 7468 6520 6461 7461 6261 7365 2069 7473  the database its
+00000bb0: 656c 662e 0a20 2020 2022 2222 0a0a 0a63  elf..    """...c
+00000bc0: 6c61 7373 2044 6174 6162 6173 6545 7272  lass DatabaseErr
+00000bd0: 6f72 2845 7272 6f72 293a 0a20 2020 2022  or(Error):.    "
+00000be0: 2222 4578 6365 7074 696f 6e20 7261 6973  ""Exception rais
+00000bf0: 6564 2066 6f72 2065 7272 6f72 7320 7468  ed for errors th
+00000c00: 6174 2061 7265 2072 656c 6174 6564 2074  at are related t
+00000c10: 6f20 7468 6520 6461 7461 6261 7365 2e22  o the database."
+00000c20: 2222 0a0a 0a63 6c61 7373 2049 6e74 6572  ""...class Inter
+00000c30: 6e61 6c45 7272 6f72 2844 6174 6162 6173  nalError(Databas
+00000c40: 6545 7272 6f72 293a 0a20 2020 2022 2222  eError):.    """
+00000c50: 4578 6365 7074 696f 6e20 7261 6973 6564  Exception raised
+00000c60: 2077 6865 6e20 7468 6520 6461 7461 6261   when the databa
+00000c70: 7365 2065 6e63 6f75 6e74 6572 7320 616e  se encounters an
+00000c80: 2069 6e74 6572 6e61 6c20 6572 726f 722c   internal error,
+00000c90: 0a20 2020 2065 2e67 2e20 7468 6520 6375  .    e.g. the cu
+00000ca0: 7273 6f72 2069 7320 6e6f 7420 7661 6c69  rsor is not vali
+00000cb0: 6420 616e 796d 6f72 650a 2020 2020 2222  d anymore.    ""
+00000cc0: 220a 0a0a 636c 6173 7320 4f70 6572 6174  "...class Operat
+00000cd0: 696f 6e61 6c45 7272 6f72 2844 6174 6162  ionalError(Datab
+00000ce0: 6173 6545 7272 6f72 293a 0a20 2020 2022  aseError):.    "
+00000cf0: 2222 4578 6365 7074 696f 6e20 7261 6973  ""Exception rais
+00000d00: 6564 2066 6f72 2065 7272 6f72 7320 7468  ed for errors th
+00000d10: 6174 2061 7265 2072 656c 6174 6564 2074  at are related t
+00000d20: 6f20 7468 6520 6461 7461 6261 7365 2773  o the database's
+00000d30: 0a20 2020 206f 7065 7261 7469 6f6e 2061  .    operation a
+00000d40: 6e64 206e 6f74 206e 6563 6573 7361 7269  nd not necessari
+00000d50: 6c79 2075 6e64 6572 2074 6865 2063 6f6e  ly under the con
+00000d60: 7472 6f6c 206f 6620 7468 6520 7072 6f67  trol of the prog
+00000d70: 7261 6d6d 6572 2c0a 2020 2020 652e 672e  rammer,.    e.g.
+00000d80: 2061 6e20 756e 6578 7065 6374 6564 2064   an unexpected d
+00000d90: 6973 636f 6e6e 6563 7420 6f63 6375 7273  isconnect occurs
+00000da0: 2c20 7468 6520 6461 7461 2073 6f75 7263  , the data sourc
+00000db0: 6520 6e61 6d65 2069 7320 6e6f 7420 666f  e name is not fo
+00000dc0: 756e 642e 0a20 2020 2022 2222 0a0a 0a63  und..    """...c
+00000dd0: 6c61 7373 2050 726f 6772 616d 6d69 6e67  lass Programming
+00000de0: 4572 726f 7228 4461 7461 6261 7365 4572  Error(DatabaseEr
+00000df0: 726f 7229 3a0a 2020 2020 2222 2245 7863  ror):.    """Exc
+00000e00: 6570 7469 6f6e 2072 6169 7365 6420 666f  eption raised fo
+00000e10: 7220 7072 6f67 7261 6d6d 696e 6720 6572  r programming er
+00000e20: 726f 7273 2c20 652e 672e 2074 6162 6c65  rors, e.g. table
+00000e30: 206e 6f74 2066 6f75 6e64 2c0a 2020 2020   not found,.    
+00000e40: 7379 6e74 6178 2065 7272 6f72 2069 6e20  syntax error in 
+00000e50: 7468 6520 5351 4c20 7374 6174 656d 656e  the SQL statemen
+00000e60: 742c 2077 726f 6e67 206e 756d 6265 7220  t, wrong number 
+00000e70: 6f66 2070 6172 616d 6574 6572 730a 2020  of parameters.  
+00000e80: 2020 7370 6563 6966 6965 642c 2065 7463    specified, etc
+00000e90: 2e0a 2020 2020 2222 220a 0a0a 636c 6173  ..    """...clas
+00000ea0: 7320 496e 7465 6772 6974 7945 7272 6f72  s IntegrityError
+00000eb0: 2844 6174 6162 6173 6545 7272 6f72 293a  (DatabaseError):
+00000ec0: 0a20 2020 2022 2222 4578 6365 7074 696f  .    """Exceptio
+00000ed0: 6e20 7261 6973 6564 2077 6865 6e20 7468  n raised when th
+00000ee0: 6520 7265 6c61 7469 6f6e 616c 2069 6e74  e relational int
+00000ef0: 6567 7269 7479 206f 6620 7468 6520 6461  egrity of the da
+00000f00: 7461 6261 7365 0a20 2020 2069 7320 6166  tabase.    is af
+00000f10: 6665 6374 6564 2c20 652e 672e 2061 2066  fected, e.g. a f
+00000f20: 6f72 6569 676e 206b 6579 2063 6865 636b  oreign key check
+00000f30: 2066 6169 6c73 0a20 2020 2022 2222 0a0a   fails.    """..
+00000f40: 0a63 6c61 7373 2044 6174 6145 7272 6f72  .class DataError
+00000f50: 2844 6174 6162 6173 6545 7272 6f72 293a  (DatabaseError):
+00000f60: 0a20 2020 2022 2222 4578 6365 7074 696f  .    """Exceptio
+00000f70: 6e20 7261 6973 6564 2066 6f72 2065 7272  n raised for err
+00000f80: 6f72 7320 7468 6174 2061 7265 2064 7565  ors that are due
+00000f90: 2074 6f20 7072 6f62 6c65 6d73 2077 6974   to problems wit
+00000fa0: 6820 7468 650a 2020 2020 7072 6f63 6573  h the.    proces
+00000fb0: 7365 6420 6461 7461 206c 696b 6520 6469  sed data like di
+00000fc0: 7669 7369 6f6e 2062 7920 7a65 726f 2c20  vision by zero, 
+00000fd0: 6e75 6d65 7269 6320 7661 6c75 6520 6f75  numeric value ou
+00000fe0: 7420 6f66 2072 616e 6765 2c20 6574 632e  t of range, etc.
+00000ff0: 0a20 2020 2022 2222 0a0a 0a63 6c61 7373  .    """...class
+00001000: 204e 6f74 5375 7070 6f72 7465 6445 7272   NotSupportedErr
+00001010: 6f72 2844 6174 6162 6173 6545 7272 6f72  or(DatabaseError
+00001020: 293a 0a20 2020 2022 2222 4578 6365 7074  ):.    """Except
+00001030: 696f 6e20 7261 6973 6564 2069 6e20 6361  ion raised in ca
+00001040: 7365 2061 206d 6574 686f 6420 6f72 2064  se a method or d
+00001050: 6174 6162 6173 6520 4150 4920 7761 7320  atabase API was 
+00001060: 7573 6564 2077 6869 6368 2069 7320 6e6f  used which is no
+00001070: 740a 2020 2020 7375 7070 6f72 7465 6420  t.    supported 
+00001080: 6279 2074 6865 2064 6174 6162 6173 650a  by the database.
+00001090: 2020 2020 2222 220a 0a0a 636c 6173 7320      """...class 
+000010a0: 4d61 6c66 6f72 6d65 6455 524c 2844 6174  MalformedURL(Dat
+000010b0: 6162 6173 6545 7272 6f72 293a 0a20 2020  abaseError):.   
+000010c0: 2022 2222 4578 6365 7074 696f 6e20 7261   """Exception ra
+000010d0: 6973 6564 2069 6e20 6361 7365 2061 206d  ised in case a m
+000010e0: 616c 666f 726d 6564 2044 534e 2069 7320  alformed DSN is 
+000010f0: 7265 6365 6976 6564 2222 220a 0a20 2020  received"""..   
+00001100: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00001110: 6c66 2c20 7265 6173 6f6e 3a20 7374 7229  lf, reason: str)
+00001120: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00001130: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
+00001140: 5f5f 2873 716c 5f73 7461 7465 3d22 3038  __(sql_state="08
+00001150: 3030 3122 2c20 7665 6e64 6f72 5f63 6f64  001", vendor_cod
+00001160: 653d 2d32 3030 2c20 7265 6173 6f6e 3d72  e=-200, reason=r
+00001170: 6561 736f 6e29 0a0a 0a63 6c61 7373 2054  eason)...class T
+00001180: 7970 6543 6f64 6573 3a20 2023 2070 796c  ypeCodes:  # pyl
+00001190: 696e 743a 2064 6973 6162 6c65 3d74 6f6f  int: disable=too
+000011a0: 2d66 6577 2d70 7562 6c69 632d 6d65 7468  -few-public-meth
+000011b0: 6f64 730a 2020 2020 2222 220a 2020 2020  ods.    """.    
+000011c0: 4461 7461 6261 7365 2063 6f6c 756d 6e20  Database column 
+000011d0: 7479 7065 2063 6f64 6573 0a0a 2020 2020  type codes..    
+000011e0: 3a6d 6574 6120 7072 6976 6174 653a 0a20  :meta private:. 
+000011f0: 2020 2022 2222 0a0a 2020 2020 4445 4d20     """..    DEM 
+00001200: 3d20 300a 2020 2020 494e 5420 3d20 310a  = 0.    INT = 1.
+00001210: 2020 2020 4c4f 4e47 203d 2032 0a20 2020      LONG = 2.   
+00001220: 2046 4c4f 4154 203d 2033 0a20 2020 2044   FLOAT = 3.    D
+00001230: 4f55 424c 4520 3d20 340a 2020 2020 5354  OUBLE = 4.    ST
+00001240: 5249 4e47 203d 2035 0a20 2020 2043 4841  RING = 5.    CHA
+00001250: 5220 3d20 350a 2020 2020 5449 4d45 5354  R = 5.    TIMEST
+00001260: 414d 5020 3d20 360a 2020 2020 4e55 4c4c  AMP = 6.    NULL
+00001270: 203d 2037 0a20 2020 2042 4f4f 4c45 414e   = 7.    BOOLEAN
+00001280: 203d 2038 0a20 2020 2042 494e 4152 5920   = 8.    BINARY 
+00001290: 3d20 390a 2020 2020 4259 5445 203d 2031  = 9.    BYTE = 1
+000012a0: 300a 2020 2020 5348 4f52 5420 3d20 3131  0.    SHORT = 11
+000012b0: 0a20 2020 2054 494d 4520 3d20 3132 0a20  .    TIME = 12. 
+000012c0: 2020 2044 4543 494d 414c 203d 2031 330a     DECIMAL = 13.
+000012d0: 2020 2020 4152 5241 5920 3d20 3134 0a20      ARRAY = 14. 
+000012e0: 2020 2055 5549 4420 3d20 3135 0a20 2020     UUID = 15.   
+000012f0: 2053 545f 504f 494e 5420 3d20 3136 0a20   ST_POINT = 16. 
+00001300: 2020 2049 5020 3d20 3137 0a20 2020 2049     IP = 17.    I
+00001310: 5056 3420 3d20 3138 0a20 2020 2044 4154  PV4 = 18.    DAT
+00001320: 4520 3d20 3139 0a20 2020 2054 494d 4553  E = 19.    TIMES
+00001330: 5441 4d50 5f4e 414e 4f53 203d 2032 300a  TAMP_NANOS = 20.
+00001340: 2020 2020 5449 4d45 5f4e 414e 4f53 203d      TIME_NANOS =
+00001350: 2032 310a 2020 2020 5455 504c 4520 3d20   21.    TUPLE = 
+00001360: 3232 0a20 2020 2053 545f 4c49 4e45 5354  22.    ST_LINEST
+00001370: 5249 4e47 203d 2032 330a 2020 2020 5354  RING = 23.    ST
+00001380: 5f50 4f4c 5947 4f4e 203d 2032 340a 0a20  _POLYGON = 24.. 
+00001390: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+000013a0: 2020 2020 6465 6620 746f 5f74 7970 6528      def to_type(
+000013b0: 636c 732c 2074 7970 6573 7472 3a20 7374  cls, typestr: st
+000013c0: 7229 202d 3e20 696e 743a 0a20 2020 2020  r) -> int:.     
+000013d0: 2020 2022 2222 4769 7665 6e20 6120 7374     """Given a st
+000013e0: 7269 6e67 2074 7970 652c 2072 6574 7572  ring type, retur
+000013f0: 6e20 6974 7320 7479 7065 2063 6f64 6522  n its type code"
+00001400: 2222 0a20 2020 2020 2020 2069 6620 6861  "".        if ha
+00001410: 7361 7474 7228 636c 732c 2074 7970 6573  sattr(cls, types
+00001420: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
+00001430: 2061 7474 7220 3d20 6765 7461 7474 7228   attr = getattr(
+00001440: 636c 732c 2074 7970 6573 7472 290a 2020  cls, typestr).  
+00001450: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+00001460: 6e73 7461 6e63 6528 6174 7472 2c20 696e  nstance(attr, in
+00001470: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00001480: 2020 2020 7265 7475 726e 2061 7474 720a      return attr.
+00001490: 2020 2020 2020 2020 7261 6973 6520 4572          raise Er
+000014a0: 726f 7228 6622 556e 6b6e 6f77 6e20 636f  ror(f"Unknown co
+000014b0: 6c75 6d6e 2074 7970 6520 7b74 7970 6573  lumn type {types
+000014c0: 7472 7d22 290a 0a20 2020 2040 636c 6173  tr}")..    @clas
+000014d0: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
+000014e0: 636c 735f 746f 5f74 7970 6528 636c 732c  cls_to_type(cls,
+000014f0: 2070 636c 6173 733a 206f 626a 6563 7429   pclass: object)
+00001500: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
+00001510: 2069 6620 7063 6c61 7373 203d 3d20 7374   if pclass == st
+00001520: 723a 0a20 2020 2020 2020 2020 2020 2072  r:.            r
+00001530: 6574 7572 6e20 636c 732e 5354 5249 4e47  eturn cls.STRING
+00001540: 0a20 2020 2020 2020 2065 6c69 6620 7063  .        elif pc
+00001550: 6c61 7373 203d 3d20 696e 743a 0a20 2020  lass == int:.   
+00001560: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00001570: 636c 732e 494e 540a 2020 2020 2020 2020  cls.INT.        
+00001580: 656c 6966 2070 636c 6173 7320 3d3d 2066  elif pclass == f
+00001590: 6c6f 6174 3a0a 2020 2020 2020 2020 2020  loat:.          
+000015a0: 2020 7265 7475 726e 2063 6c73 2e46 4c4f    return cls.FLO
+000015b0: 4154 0a20 2020 2020 2020 2065 6c69 6620  AT.        elif 
+000015c0: 7063 6c61 7373 203d 3d20 7575 6964 2e55  pclass == uuid.U
+000015d0: 5549 443a 0a20 2020 2020 2020 2020 2020  UID:.           
+000015e0: 2072 6574 7572 6e20 636c 732e 5555 4944   return cls.UUID
+000015f0: 0a20 2020 2020 2020 2065 6c69 6620 7063  .        elif pc
+00001600: 6c61 7373 203d 3d20 4f70 7469 6f6e 616c  lass == Optional
+00001610: 5b75 7569 642e 5555 4944 5d3a 0a20 2020  [uuid.UUID]:.   
+00001620: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00001630: 636c 732e 5555 4944 0a20 2020 2020 2020  cls.UUID.       
+00001640: 2072 6169 7365 2045 7272 6f72 2866 2255   raise Error(f"U
+00001650: 6e6b 6e6f 776e 2063 6f6c 756d 6e20 636c  nknown column cl
+00001660: 6173 7320 7b70 636c 6173 737d 2229 0a0a  ass {pclass}")..
+00001670: 0a23 2042 7920 696e 7374 616e 7469 6174  .# By instantiat
+00001680: 696e 6720 7468 6573 6520 6865 7265 2077  ing these here w
+00001690: 6520 7265 6475 6365 2074 6865 206f 7665  e reduce the ove
+000016a0: 7268 6561 6420 6f66 2073 6574 7469 6e67  rhead of setting
+000016b0: 2074 6869 7320 7570 0a23 2065 6163 6820   this up.# each 
+000016c0: 7469 6d65 2077 6520 6361 6c6c 2069 740a  time we call it.
+000016d0: 5f75 6e70 6163 6b5f 7368 6f72 7420 3d20  _unpack_short = 
+000016e0: 7374 7275 6374 2e53 7472 7563 7428 2221  struct.Struct("!
+000016f0: 6822 292e 756e 7061 636b 5f66 726f 6d0a  h").unpack_from.
+00001700: 5f75 6e70 6163 6b5f 696e 7420 3d20 7374  _unpack_int = st
+00001710: 7275 6374 2e53 7472 7563 7428 2221 6922  ruct.Struct("!i"
+00001720: 292e 756e 7061 636b 5f66 726f 6d0a 5f75  ).unpack_from._u
+00001730: 6e70 6163 6b5f 6c6f 6e67 203d 2073 7472  npack_long = str
+00001740: 7563 742e 5374 7275 6374 2822 2171 2229  uct.Struct("!q")
+00001750: 2e75 6e70 6163 6b5f 6672 6f6d 0a5f 756e  .unpack_from._un
+00001760: 7061 636b 5f66 6c6f 6174 203d 2073 7472  pack_float = str
+00001770: 7563 742e 5374 7275 6374 2822 2166 2229  uct.Struct("!f")
+00001780: 2e75 6e70 6163 6b5f 6672 6f6d 0a5f 756e  .unpack_from._un
+00001790: 7061 636b 5f64 6f75 626c 6520 3d20 7374  pack_double = st
+000017a0: 7275 6374 2e53 7472 7563 7428 2221 6422  ruct.Struct("!d"
+000017b0: 292e 756e 7061 636b 5f66 726f 6d0a 5f75  ).unpack_from._u
+000017c0: 6e70 6163 6b5f 626f 6f6c 203d 2073 7472  npack_bool = str
+000017d0: 7563 742e 5374 7275 6374 2822 3f22 292e  uct.Struct("?").
+000017e0: 756e 7061 636b 5f66 726f 6d0a 5f75 6e70  unpack_from._unp
+000017f0: 6163 6b5f 6368 6172 203d 2073 7472 7563  ack_char = struc
+00001800: 742e 5374 7275 6374 2822 6322 292e 756e  t.Struct("c").un
+00001810: 7061 636b 5f66 726f 6d0a 0a23 2065 6173  pack_from..# eas
+00001820: 7920 636f 6e76 6572 7369 6f6e 7320 7765  y conversions we
+00001830: 2063 616e 2064 6f20 7769 7468 2073 7472   can do with str
+00001840: 7563 7473 0a5f 7479 7065 5f6d 6170 203d  ucts._type_map =
+00001850: 207b 0a20 2020 2054 7970 6543 6f64 6573   {.    TypeCodes
+00001860: 2e49 4e54 3a20 2873 7472 7563 742e 6361  .INT: (struct.ca
+00001870: 6c63 7369 7a65 2822 2169 2229 2c20 5f75  lcsize("!i"), _u
+00001880: 6e70 6163 6b5f 696e 7429 2c0a 2020 2020  npack_int),.    
+00001890: 5479 7065 436f 6465 732e 4c4f 4e47 3a20  TypeCodes.LONG: 
+000018a0: 2873 7472 7563 742e 6361 6c63 7369 7a65  (struct.calcsize
+000018b0: 2822 2171 2229 2c20 5f75 6e70 6163 6b5f  ("!q"), _unpack_
+000018c0: 6c6f 6e67 292c 0a20 2020 2054 7970 6543  long),.    TypeC
+000018d0: 6f64 6573 2e46 4c4f 4154 3a20 2873 7472  odes.FLOAT: (str
+000018e0: 7563 742e 6361 6c63 7369 7a65 2822 2166  uct.calcsize("!f
+000018f0: 2229 2c20 5f75 6e70 6163 6b5f 666c 6f61  "), _unpack_floa
+00001900: 7429 2c0a 2020 2020 5479 7065 436f 6465  t),.    TypeCode
+00001910: 732e 444f 5542 4c45 3a20 2873 7472 7563  s.DOUBLE: (struc
+00001920: 742e 6361 6c63 7369 7a65 2822 2164 2229  t.calcsize("!d")
+00001930: 2c20 5f75 6e70 6163 6b5f 646f 7562 6c65  , _unpack_double
+00001940: 292c 0a20 2020 2054 7970 6543 6f64 6573  ),.    TypeCodes
+00001950: 2e42 4f4f 4c45 414e 3a20 2873 7472 7563  .BOOLEAN: (struc
+00001960: 742e 6361 6c63 7369 7a65 2822 3f22 292c  t.calcsize("?"),
+00001970: 205f 756e 7061 636b 5f62 6f6f 6c29 2c0a   _unpack_bool),.
+00001980: 2020 2020 5479 7065 436f 6465 732e 5348      TypeCodes.SH
+00001990: 4f52 543a 2028 7374 7275 6374 2e63 616c  ORT: (struct.cal
+000019a0: 6373 697a 6528 2221 6822 292c 205f 756e  csize("!h"), _un
+000019b0: 7061 636b 5f73 686f 7274 292c 0a7d 0a0a  pack_short),.}..
+000019c0: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
+000019d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000019e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000019f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001a00: 2323 2323 2323 2323 2323 0a23 2044 6174  ##########.# Dat
+00001a10: 6162 6173 6520 4150 4920 322e 3020 7479  abase API 2.0 ty
+00001a20: 7065 732e 2020 5468 6573 6520 6172 6520  pes.  These are 
+00001a30: 7265 7175 6972 6564 2062 7920 5045 4d20  required by PEM 
+00001a40: 3234 390a 2323 2323 2323 2323 2323 2323  249.############
+00001a50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001a60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001a70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001a80: 2323 2323 2323 2323 2323 2323 230a 4269  #############.Bi
+00001a90: 6e61 7279 203d 2062 7974 6573 2020 2320  nary = bytes  # 
+00001aa0: 3a20 3a6d 6574 6120 7072 6976 6174 653a  : :meta private:
+00001ab0: 0a53 5452 494e 4720 3d20 5479 7065 436f  .STRING = TypeCo
+00001ac0: 6465 732e 5354 5249 4e47 2020 2320 3a20  des.STRING  # : 
+00001ad0: 3a6d 6574 6120 7072 6976 6174 653a 0a42  :meta private:.B
+00001ae0: 494e 4152 5920 3d20 5479 7065 436f 6465  INARY = TypeCode
+00001af0: 732e 4249 4e41 5259 2020 2320 3a20 3a6d  s.BINARY  # : :m
+00001b00: 6574 6120 7072 6976 6174 653a 0a4e 554d  eta private:.NUM
+00001b10: 4245 5220 3d20 5479 7065 436f 6465 732e  BER = TypeCodes.
+00001b20: 494e 5420 2023 203a 203a 6d65 7461 2070  INT  # : :meta p
+00001b30: 7269 7661 7465 3a0a 4441 5445 5449 4d45  rivate:.DATETIME
+00001b40: 203d 2054 7970 6543 6f64 6573 2e54 494d   = TypeCodes.TIM
+00001b50: 4553 5441 4d50 2020 2320 3a20 3a6d 6574  ESTAMP  # : :met
+00001b60: 6120 7072 6976 6174 653a 0a52 4f57 4944  a private:.ROWID
+00001b70: 203d 2054 7970 6543 6f64 6573 2e49 4e54   = TypeCodes.INT
+00001b80: 2020 2320 3a20 3a6d 6574 6120 7072 6976    # : :meta priv
+00001b90: 6174 653a 0a0a 2323 2323 2323 2323 2323  ate:..##########
+00001ba0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001bb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001bc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001bd0: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
+00001be0: 2320 496d 706f 7274 206f 7572 2067 6f6f  # Import our goo
+00001bf0: 676c 6520 7072 6f74 6f62 7566 206d 6573  gle protobuf mes
+00001c00: 7361 6765 2064 6566 696e 6974 696f 6e73  sage definitions
+00001c10: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
+00001c20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001c30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001c40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001c50: 2323 2323 2323 2323 2323 0a74 7279 3a0a  ##########.try:.
+00001c60: 2020 2020 6672 6f6d 2073 6861 7265 644d      from sharedM
+00001c70: 6573 7361 6765 7320 696d 706f 7274 2063  essages import c
+00001c80: 6c69 656e 7457 6972 6550 726f 746f 636f  lientWireProtoco
+00001c90: 6c5f 7062 3220 6173 2070 726f 746f 0a65  l_pb2 as proto.e
+00001ca0: 7863 6570 7420 496d 706f 7274 4572 726f  xcept ImportErro
+00001cb0: 723a 0a20 2020 2069 6d70 6f72 7420 7079  r:.    import py
+00001cc0: 6f63 6965 6e74 2e43 6c69 656e 7457 6972  ocient.ClientWir
+00001cd0: 6550 726f 746f 636f 6c5f 7062 3220 6173  eProtocol_pb2 as
+00001ce0: 2070 726f 746f 0a0a 2323 2323 2323 2323   proto..########
+00001cf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001d00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001d10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001d20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001d30: 230a 2320 4c69 6768 7477 6569 6768 7420  #.# Lightweight 
+00001d40: 4749 5320 636c 6173 7365 730a 2323 2323  GIS classes.####
+00001d50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001d60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001d70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001d80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001d90: 2323 2323 230a 0a0a 636c 6173 7320 5f53  #####...class _S
+00001da0: 5450 6f69 6e74 3a0a 2020 2020 6465 6620  TPoint:.    def 
+00001db0: 5f5f 696e 6974 5f5f 2873 656c 662c 206c  __init__(self, l
+00001dc0: 6f6e 673a 2066 6c6f 6174 2c20 6c61 743a  ong: float, lat:
+00001dd0: 2066 6c6f 6174 2920 2d3e 204e 6f6e 653a   float) -> None:
+00001de0: 0a20 2020 2020 2020 2073 656c 662e 6c6f  .        self.lo
+00001df0: 6e67 203d 206c 6f6e 670a 2020 2020 2020  ng = long.      
+00001e00: 2020 7365 6c66 2e6c 6174 203d 206c 6174    self.lat = lat
+00001e10: 0a0a 2020 2020 6465 6620 776b 745f 696e  ..    def wkt_in
+00001e20: 6e65 7228 7365 6c66 2920 2d3e 2073 7472  ner(self) -> str
+00001e30: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00001e40: 2073 7472 2873 656c 662e 6c6f 6e67 2920   str(self.long) 
+00001e50: 2b20 2220 2220 2b20 7374 7228 7365 6c66  + " " + str(self
+00001e60: 2e6c 6174 290a 0a20 2020 2064 6566 205f  .lat)..    def _
+00001e70: 5f72 6570 725f 5f28 7365 6c66 2920 2d3e  _repr__(self) ->
+00001e80: 2073 7472 3a0a 2020 2020 2020 2020 6966   str:.        if
+00001e90: 2069 7369 6e66 2873 656c 662e 6c6f 6e67   isinf(self.long
+00001ea0: 2920 6f72 2069 7369 6e66 2873 656c 662e  ) or isinf(self.
+00001eb0: 6c61 7429 3a0a 2020 2020 2020 2020 2020  lat):.          
+00001ec0: 2020 7265 7475 726e 2022 504f 494e 5420    return "POINT 
+00001ed0: 454d 5054 5922 0a20 2020 2020 2020 2072  EMPTY".        r
+00001ee0: 6574 7572 6e20 2250 4f49 4e54 2822 202b  eturn "POINT(" +
+00001ef0: 2073 656c 662e 776b 745f 696e 6e65 7228   self.wkt_inner(
+00001f00: 2920 2b20 2229 220a 0a20 2020 2064 6566  ) + ")"..    def
+00001f10: 205f 5f65 715f 5f28 7365 6c66 2c20 6f74   __eq__(self, ot
+00001f20: 6865 723a 206f 626a 6563 7429 202d 3e20  her: object) -> 
+00001f30: 626f 6f6c 3a0a 2020 2020 2020 2020 6966  bool:.        if
+00001f40: 2069 7369 6e73 7461 6e63 6528 6f74 6865   isinstance(othe
+00001f50: 722c 205f 5354 506f 696e 7429 3a0a 2020  r, _STPoint):.  
+00001f60: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00001f70: 2073 656c 662e 6c6f 6e67 203d 3d20 6f74   self.long == ot
+00001f80: 6865 722e 6c6f 6e67 2061 6e64 2073 656c  her.long and sel
+00001f90: 662e 6c61 7420 3d3d 206f 7468 6572 2e6c  f.lat == other.l
+00001fa0: 6174 0a20 2020 2020 2020 2072 6574 7572  at.        retur
+00001fb0: 6e20 4e6f 7449 6d70 6c65 6d65 6e74 6564  n NotImplemented
+00001fc0: 0a0a 0a64 6566 205f 6c69 6e65 7374 7269  ...def _linestri
+00001fd0: 6e67 5f77 6b74 5f69 6e6e 6572 2870 6f69  ng_wkt_inner(poi
+00001fe0: 6e74 733a 204c 6973 745b 5f53 5450 6f69  nts: List[_STPoi
+00001ff0: 6e74 5d29 202d 3e20 7374 723a 0a20 2020  nt]) -> str:.   
+00002000: 2072 6574 7572 6e20 2228 2220 2b20 222c   return "(" + ",
+00002010: 2022 2e6a 6f69 6e28 2870 2e77 6b74 5f69   ".join((p.wkt_i
+00002020: 6e6e 6572 2829 2066 6f72 2070 2069 6e20  nner() for p in 
+00002030: 706f 696e 7473 2929 202b 2022 2922 0a0a  points)) + ")"..
+00002040: 0a63 6c61 7373 205f 5354 4c69 6e65 7374  .class _STLinest
+00002050: 7269 6e67 3a0a 2020 2020 6465 6620 5f5f  ring:.    def __
+00002060: 696e 6974 5f5f 2873 656c 662c 2070 6f69  init__(self, poi
+00002070: 6e74 733a 204c 6973 745b 5f53 5450 6f69  nts: List[_STPoi
+00002080: 6e74 5d29 202d 3e20 4e6f 6e65 3a0a 2020  nt]) -> None:.  
+00002090: 2020 2020 2020 7365 6c66 2e70 6f69 6e74        self.point
+000020a0: 7320 3d20 706f 696e 7473 0a0a 2020 2020  s = points..    
+000020b0: 6465 6620 5f5f 7265 7072 5f5f 2873 656c  def __repr__(sel
+000020c0: 6629 202d 3e20 7374 723a 0a20 2020 2020  f) -> str:.     
+000020d0: 2020 2069 6620 6e6f 7420 7365 6c66 2e70     if not self.p
+000020e0: 6f69 6e74 733a 0a20 2020 2020 2020 2020  oints:.         
+000020f0: 2020 2072 6574 7572 6e20 224c 494e 4553     return "LINES
+00002100: 5452 494e 4720 454d 5054 5922 0a20 2020  TRING EMPTY".   
+00002110: 2020 2020 2072 6574 7572 6e20 224c 494e       return "LIN
+00002120: 4553 5452 494e 4722 202b 205f 6c69 6e65  ESTRING" + _line
+00002130: 7374 7269 6e67 5f77 6b74 5f69 6e6e 6572  string_wkt_inner
+00002140: 2873 656c 662e 706f 696e 7473 290a 0a20  (self.points).. 
+00002150: 2020 2064 6566 205f 5f65 715f 5f28 7365     def __eq__(se
+00002160: 6c66 2c20 6f74 6865 723a 206f 626a 6563  lf, other: objec
+00002170: 7429 202d 3e20 626f 6f6c 3a0a 2020 2020  t) -> bool:.    
+00002180: 2020 2020 2320 7374 7269 6374 2065 7175      # strict equ
+00002190: 616c 6974 792c 206e 6f74 2073 656d 616e  ality, not seman
+000021a0: 7469 630a 2020 2020 2020 2020 6966 2069  tic.        if i
+000021b0: 7369 6e73 7461 6e63 6528 6f74 6865 722c  sinstance(other,
+000021c0: 205f 5354 4c69 6e65 7374 7269 6e67 293a   _STLinestring):
+000021d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000021e0: 7572 6e20 7365 6c66 2e70 6f69 6e74 7320  urn self.points 
+000021f0: 3d3d 206f 7468 6572 2e70 6f69 6e74 730a  == other.points.
+00002200: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+00002210: 6f74 496d 706c 656d 656e 7465 640a 0a0a  otImplemented...
+00002220: 636c 6173 7320 5f53 5450 6f6c 7967 6f6e  class _STPolygon
+00002230: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00002240: 5f5f 2873 656c 662c 2065 7874 6572 696f  __(self, exterio
+00002250: 723a 204c 6973 745b 5f53 5450 6f69 6e74  r: List[_STPoint
+00002260: 5d2c 2068 6f6c 6573 3a20 4c69 7374 5b4c  ], holes: List[L
+00002270: 6973 745b 5f53 5450 6f69 6e74 5d5d 2920  ist[_STPoint]]) 
+00002280: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00002290: 2073 656c 662e 6578 7465 7269 6f72 203d   self.exterior =
+000022a0: 2065 7874 6572 696f 720a 2020 2020 2020   exterior.      
+000022b0: 2020 7365 6c66 2e68 6f6c 6573 203d 2068    self.holes = h
+000022c0: 6f6c 6573 0a0a 2020 2020 6465 6620 5f5f  oles..    def __
+000022d0: 7265 7072 5f5f 2873 656c 6629 202d 3e20  repr__(self) -> 
+000022e0: 7374 723a 0a20 2020 2020 2020 2069 6620  str:.        if 
+000022f0: 6e6f 7420 7365 6c66 2e65 7874 6572 696f  not self.exterio
+00002300: 723a 0a20 2020 2020 2020 2020 2020 2072  r:.            r
+00002310: 6574 7572 6e20 2250 4f4c 5947 4f4e 2045  eturn "POLYGON E
+00002320: 4d50 5459 220a 2020 2020 2020 2020 7265  MPTY".        re
+00002330: 7475 726e 2022 504f 4c59 474f 4e28 2220  turn "POLYGON(" 
+00002340: 2b20 222c 2022 2e6a 6f69 6e28 285f 6c69  + ", ".join((_li
+00002350: 6e65 7374 7269 6e67 5f77 6b74 5f69 6e6e  nestring_wkt_inn
+00002360: 6572 2870 6c29 2066 6f72 2070 6c20 696e  er(pl) for pl in
+00002370: 205b 7365 6c66 2e65 7874 6572 696f 725d   [self.exterior]
+00002380: 202b 2073 656c 662e 686f 6c65 7329 2920   + self.holes)) 
+00002390: 2b20 2229 220a 0a20 2020 2064 6566 205f  + ")"..    def _
+000023a0: 5f65 715f 5f28 7365 6c66 2c20 6f74 6865  _eq__(self, othe
+000023b0: 723a 206f 626a 6563 7429 202d 3e20 626f  r: object) -> bo
+000023c0: 6f6c 3a0a 2020 2020 2020 2020 2320 7374  ol:.        # st
+000023d0: 7269 6374 2065 7175 616c 6974 792c 206e  rict equality, n
+000023e0: 6f74 2073 656d 616e 7469 630a 2020 2020  ot semantic.    
+000023f0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00002400: 6528 6f74 6865 722c 205f 5354 506f 6c79  e(other, _STPoly
+00002410: 676f 6e29 3a0a 2020 2020 2020 2020 2020  gon):.          
+00002420: 2020 7265 7475 726e 2073 656c 662e 6578    return self.ex
+00002430: 7465 7269 6f72 203d 3d20 6f74 6865 722e  terior == other.
+00002440: 6578 7465 7269 6f72 2061 6e64 2073 656c  exterior and sel
+00002450: 662e 686f 6c65 7320 3d3d 206f 7468 6572  f.holes == other
+00002460: 2e68 6f6c 6573 0a20 2020 2020 2020 2072  .holes.        r
+00002470: 6574 7572 6e20 4e6f 7449 6d70 6c65 6d65  eturn NotImpleme
+00002480: 6e74 6564 0a0a 0a23 2323 2323 2323 2323  nted...#########
+00002490: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000024a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000024b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000024c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000024d0: 0a23 2042 7569 6c64 2073 7570 706f 7274  .# Build support
+000024e0: 6564 2072 6571 7565 7374 2f72 6573 706f  ed request/respo
+000024f0: 6e73 6520 7479 7065 206d 6170 7069 6e67  nse type mapping
+00002500: 730a 2323 2323 2323 2323 2323 2323 2323  s.##############
+00002510: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002520: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002530: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002540: 2323 2323 2323 2323 2323 230a 0a0a 636c  ###########...cl
+00002550: 6173 7320 5f4f 6369 656e 7452 6571 7565  ass _OcientReque
+00002560: 7374 4661 6374 6f72 7928 4765 6e65 7269  stFactory(Generi
+00002570: 635b 5f54 5d29 3a0a 2020 2020 6465 6620  c[_T]):.    def 
+00002580: 7265 7175 6573 7428 7365 6c66 2c20 6f70  request(self, op
+00002590: 6572 6174 696f 6e3a 2073 7472 2920 2d3e  eration: str) ->
+000025a0: 2070 726f 746f 2e52 6571 7565 7374 3a0a   proto.Request:.
+000025b0: 2020 2020 2020 2020 2222 2247 656e 6572          """Gener
+000025c0: 6174 6573 2061 2066 756c 6c79 2070 6f70  ates a fully pop
+000025d0: 756c 6174 6564 2072 6571 7565 7374 2070  ulated request p
+000025e0: 726f 746f 6275 6622 2222 0a20 2020 2020  rotobuf""".     
+000025f0: 2020 2072 6169 7365 204e 6f74 496d 706c     raise NotImpl
+00002600: 656d 656e 7465 6445 7272 6f72 0a0a 2020  ementedError..  
+00002610: 2020 6465 6620 7265 7370 6f6e 7365 2873    def response(s
+00002620: 656c 6629 202d 3e20 5f54 3a0a 2020 2020  elf) -> _T:.    
+00002630: 2020 2020 2222 2247 656e 6572 6174 6573      """Generates
+00002640: 2061 2066 756c 6c79 2070 6f70 756c 6174   a fully populat
+00002650: 6564 2072 6573 706f 6e73 6520 7072 6f74  ed response prot
+00002660: 6f62 7566 2222 220a 2020 2020 2020 2020  obuf""".        
+00002670: 7261 6973 6520 4e6f 7449 6d70 6c65 6d65  raise NotImpleme
+00002680: 6e74 6564 4572 726f 720a 0a20 2020 2064  ntedError..    d
+00002690: 6566 2070 726f 6365 7373 2873 656c 662c  ef process(self,
+000026a0: 2072 7370 3a20 5f54 2920 2d3e 2041 6e79   rsp: _T) -> Any
+000026b0: 3a0a 2020 2020 2020 2020 2222 2250 726f  :.        """Pro
+000026c0: 6365 7373 2074 6865 2063 6c69 656e 7420  cess the client 
+000026d0: 7265 7370 6f6e 7365 2222 220a 2020 2020  response""".    
+000026e0: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
+000026f0: 6c65 6d65 6e74 6564 4572 726f 720a 0a0a  lementedError...
+00002700: 636c 6173 7320 5f45 7865 6375 7465 5175  class _ExecuteQu
+00002710: 6572 7946 6163 746f 7279 285f 4f63 6965  eryFactory(_Ocie
+00002720: 6e74 5265 7175 6573 7446 6163 746f 7279  ntRequestFactory
+00002730: 5b70 726f 746f 2e45 7865 6375 7465 5175  [proto.ExecuteQu
+00002740: 6572 7952 6573 706f 6e73 655d 293a 0a20  eryResponse]):. 
+00002750: 2020 2064 6566 2072 6571 7565 7374 2873     def request(s
+00002760: 656c 662c 206f 7065 7261 7469 6f6e 3a20  elf, operation: 
+00002770: 7374 7229 202d 3e20 7072 6f74 6f2e 5265  str) -> proto.Re
+00002780: 7175 6573 743a 0a20 2020 2020 2020 2022  quest:.        "
+00002790: 2222 4765 6e65 7261 7465 7320 6120 6675  ""Generates a fu
+000027a0: 6c6c 7920 706f 7075 6c61 7465 6420 4558  lly populated EX
+000027b0: 4543 5554 455f 5155 4552 5920 7265 7175  ECUTE_QUERY requ
+000027c0: 6573 7420 7072 6f74 6f62 7566 2222 220a  est protobuf""".
+000027d0: 2020 2020 2020 2020 7265 7120 3d20 7072          req = pr
+000027e0: 6f74 6f2e 5265 7175 6573 7428 290a 2020  oto.Request().  
+000027f0: 2020 2020 2020 7265 712e 7479 7065 203d        req.type =
+00002800: 2070 726f 746f 2e52 6571 7565 7374 2e52   proto.Request.R
+00002810: 6571 7565 7374 5479 7065 2e56 616c 7565  equestType.Value
+00002820: 2822 4558 4543 5554 455f 5155 4552 5922  ("EXECUTE_QUERY"
+00002830: 2920 2023 2074 7970 653a 2069 676e 6f72  )  # type: ignor
+00002840: 6520 2320 6874 7470 733a 2f2f 6769 7468  e # https://gith
+00002850: 7562 2e63 6f6d 2f70 726f 746f 636f 6c62  ub.com/protocolb
+00002860: 7566 6665 7273 2f70 726f 746f 6275 662f  uffers/protobuf/
+00002870: 6973 7375 6573 2f31 3032 3430 0a20 2020  issues/10240.   
+00002880: 2020 2020 2072 6571 2e65 7865 6375 7465       req.execute
+00002890: 5f71 7565 7279 2e73 716c 203d 206f 7065  _query.sql = ope
+000028a0: 7261 7469 6f6e 0a20 2020 2020 2020 2072  ration.        r
+000028b0: 6571 2e65 7865 6375 7465 5f71 7565 7279  eq.execute_query
+000028c0: 2e66 6f72 6365 203d 2046 616c 7365 0a20  .force = False. 
+000028d0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000028e0: 710a 0a20 2020 2064 6566 2072 6573 706f  q..    def respo
+000028f0: 6e73 6528 7365 6c66 2920 2d3e 2070 726f  nse(self) -> pro
+00002900: 746f 2e45 7865 6375 7465 5175 6572 7952  to.ExecuteQueryR
+00002910: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
+00002920: 2022 2222 4765 6e65 7261 7465 7320 6120   """Generates a 
+00002930: 6675 6c6c 7920 706f 7075 6c61 7465 6420  fully populated 
+00002940: 4558 4543 5554 455f 5155 4552 5920 7265  EXECUTE_QUERY re
+00002950: 7370 6f6e 7365 2070 726f 746f 6275 6622  sponse protobuf"
+00002960: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+00002970: 6e20 7072 6f74 6f2e 4578 6563 7574 6551  n proto.ExecuteQ
+00002980: 7565 7279 5265 7370 6f6e 7365 2829 0a0a  ueryResponse()..
+00002990: 0a63 6c61 7373 205f 4578 6563 7574 6545  .class _ExecuteE
+000029a0: 7870 6c61 696e 4661 6374 6f72 7928 5f4f  xplainFactory(_O
+000029b0: 6369 656e 7452 6571 7565 7374 4661 6374  cientRequestFact
+000029c0: 6f72 795b 7072 6f74 6f2e 4578 706c 6169  ory[proto.Explai
+000029d0: 6e52 6573 706f 6e73 6553 7472 696e 6750  nResponseStringP
+000029e0: 6c61 6e5d 293a 0a20 2020 2064 6566 2072  lan]):.    def r
+000029f0: 6571 7565 7374 2873 656c 662c 206f 7065  equest(self, ope
+00002a00: 7261 7469 6f6e 3a20 7374 7229 202d 3e20  ration: str) -> 
+00002a10: 7072 6f74 6f2e 5265 7175 6573 743a 0a20  proto.Request:. 
+00002a20: 2020 2020 2020 2022 2222 4765 6e65 7261         """Genera
+00002a30: 7465 7320 6120 6675 6c6c 7920 706f 7075  tes a fully popu
+00002a40: 6c61 7465 6420 4558 4543 5554 455f 4558  lated EXECUTE_EX
+00002a50: 504c 4149 4e20 7265 7175 6573 7420 7072  PLAIN request pr
+00002a60: 6f74 6f62 7566 2222 220a 2020 2020 2020  otobuf""".      
+00002a70: 2020 7265 7120 3d20 7072 6f74 6f2e 5265    req = proto.Re
+00002a80: 7175 6573 7428 290a 2020 2020 2020 2020  quest().        
+00002a90: 7265 712e 7479 7065 203d 2070 726f 746f  req.type = proto
+00002aa0: 2e52 6571 7565 7374 2e52 6571 7565 7374  .Request.Request
+00002ab0: 5479 7065 2e56 616c 7565 2822 4558 4543  Type.Value("EXEC
+00002ac0: 5554 455f 4558 504c 4149 4e22 2920 2023  UTE_EXPLAIN")  #
+00002ad0: 2074 7970 653a 2069 676e 6f72 6520 2320   type: ignore # 
+00002ae0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00002af0: 6f6d 2f70 726f 746f 636f 6c62 7566 6665  om/protocolbuffe
+00002b00: 7273 2f70 726f 746f 6275 662f 6973 7375  rs/protobuf/issu
+00002b10: 6573 2f31 3032 3430 0a20 2020 2020 2020  es/10240.       
+00002b20: 2072 6571 2e65 7865 6375 7465 5f65 7870   req.execute_exp
+00002b30: 6c61 696e 2e66 6f72 6d61 7420 3d20 7072  lain.format = pr
+00002b40: 6f74 6f2e 4578 706c 6169 6e46 6f72 6d61  oto.ExplainForma
+00002b50: 742e 4a53 4f4e 2020 2320 7479 7065 3a20  t.JSON  # type: 
+00002b60: 6967 6e6f 7265 2023 2068 7474 7073 3a2f  ignore # https:/
+00002b70: 2f67 6974 6875 622e 636f 6d2f 7072 6f74  /github.com/prot
+00002b80: 6f63 6f6c 6275 6666 6572 732f 7072 6f74  ocolbuffers/prot
+00002b90: 6f62 7566 2f69 7373 7565 732f 3130 3234  obuf/issues/1024
+00002ba0: 300a 2020 2020 2020 2020 7370 6c69 7474  0.        splitt
+00002bb0: 6564 203d 206f 7065 7261 7469 6f6e 2e73  ed = operation.s
+00002bc0: 706c 6974 286d 6178 7370 6c69 743d 3129  plit(maxsplit=1)
+00002bd0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+00002be0: 7370 6c69 7474 6564 2920 3d3d 2032 3a0a  splitted) == 2:.
+00002bf0: 2020 2020 2020 2020 2020 2020 7265 712e              req.
+00002c00: 6578 6563 7574 655f 6578 706c 6169 6e2e  execute_explain.
+00002c10: 7371 6c20 3d20 7370 6c69 7474 6564 5b31  sql = splitted[1
+00002c20: 5d0a 2020 2020 2020 2020 7265 7475 726e  ].        return
+00002c30: 2072 6571 0a0a 2020 2020 6465 6620 7265   req..    def re
+00002c40: 7370 6f6e 7365 2873 656c 6629 202d 3e20  sponse(self) -> 
+00002c50: 7072 6f74 6f2e 4578 706c 6169 6e52 6573  proto.ExplainRes
+00002c60: 706f 6e73 6553 7472 696e 6750 6c61 6e3a  ponseStringPlan:
+00002c70: 0a20 2020 2020 2020 2022 2222 4765 6e65  .        """Gene
+00002c80: 7261 7465 7320 6120 6675 6c6c 7920 706f  rates a fully po
+00002c90: 7075 6c61 7465 6420 4558 4543 5554 455f  pulated EXECUTE_
+00002ca0: 4558 504c 4149 4e20 7265 7370 6f6e 7365  EXPLAIN response
+00002cb0: 2070 726f 746f 6275 6622 2222 0a20 2020   protobuf""".   
+00002cc0: 2020 2020 2072 6574 7572 6e20 7072 6f74       return prot
+00002cd0: 6f2e 4578 706c 6169 6e52 6573 706f 6e73  o.ExplainRespons
+00002ce0: 6553 7472 696e 6750 6c61 6e28 290a 0a0a  eStringPlan()...
+00002cf0: 636c 6173 7320 5f45 7865 6375 7465 4578  class _ExecuteEx
+00002d00: 706f 7274 4661 6374 6f72 7928 5f4f 6369  portFactory(_Oci
+00002d10: 656e 7452 6571 7565 7374 4661 6374 6f72  entRequestFactor
+00002d20: 795b 7072 6f74 6f2e 4578 6563 7574 6545  y[proto.ExecuteE
+00002d30: 7870 6f72 7452 6573 706f 6e73 655d 293a  xportResponse]):
+00002d40: 0a20 2020 2064 6566 2072 6571 7565 7374  .    def request
+00002d50: 2873 656c 662c 206f 7065 7261 7469 6f6e  (self, operation
+00002d60: 3a20 7374 7229 202d 3e20 7072 6f74 6f2e  : str) -> proto.
+00002d70: 5265 7175 6573 743a 0a20 2020 2020 2020  Request:.       
+00002d80: 2022 2222 4765 6e65 7261 7465 7320 6120   """Generates a 
+00002d90: 6675 6c6c 7920 706f 7075 6c61 7465 6420  fully populated 
+00002da0: 4558 4543 5554 455f 4558 504f 5254 2072  EXECUTE_EXPORT r
+00002db0: 6571 7565 7374 2070 726f 746f 6275 6622  equest protobuf"
+00002dc0: 2222 0a20 2020 2020 2020 2072 6571 203d  "".        req =
+00002dd0: 2070 726f 746f 2e52 6571 7565 7374 2829   proto.Request()
+00002de0: 0a20 2020 2020 2020 2072 6571 2e74 7970  .        req.typ
+00002df0: 6520 3d20 7072 6f74 6f2e 5265 7175 6573  e = proto.Reques
+00002e00: 742e 5265 7175 6573 7454 7970 652e 5661  t.RequestType.Va
+00002e10: 6c75 6528 2245 5845 4355 5445 5f45 5850  lue("EXECUTE_EXP
+00002e20: 4f52 5422 2920 2023 2074 7970 653a 2069  ORT")  # type: i
+00002e30: 676e 6f72 6520 2320 6874 7470 733a 2f2f  gnore # https://
+00002e40: 6769 7468 7562 2e63 6f6d 2f70 726f 746f  github.com/proto
+00002e50: 636f 6c62 7566 6665 7273 2f70 726f 746f  colbuffers/proto
+00002e60: 6275 662f 6973 7375 6573 2f31 3032 3430  buf/issues/10240
+00002e70: 0a20 2020 2020 2020 2072 6571 2e65 7865  .        req.exe
+00002e80: 6375 7465 5f65 7870 6f72 742e 7371 6c20  cute_export.sql 
+00002e90: 3d20 6f70 6572 6174 696f 6e0a 2020 2020  = operation.    
+00002ea0: 2020 2020 7265 7475 726e 2072 6571 0a0a      return req..
+00002eb0: 2020 2020 6465 6620 7265 7370 6f6e 7365      def response
+00002ec0: 2873 656c 6629 202d 3e20 7072 6f74 6f2e  (self) -> proto.
+00002ed0: 4578 6563 7574 6545 7870 6f72 7452 6573  ExecuteExportRes
+00002ee0: 706f 6e73 653a 0a20 2020 2020 2020 2022  ponse:.        "
+00002ef0: 2222 4765 6e65 7261 7465 7320 6120 6675  ""Generates a fu
+00002f00: 6c6c 7920 706f 7075 6c61 7465 6420 4558  lly populated EX
+00002f10: 4543 5554 455f 4558 504f 5254 2072 6573  ECUTE_EXPORT res
+00002f20: 706f 6e73 6520 7072 6f74 6f62 7566 2222  ponse protobuf""
+00002f30: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+00002f40: 2070 726f 746f 2e45 7865 6375 7465 4578   proto.ExecuteEx
+00002f50: 706f 7274 5265 7370 6f6e 7365 2829 0a0a  portResponse()..
+00002f60: 0a63 6c61 7373 205f 4578 706c 6169 6e50  .class _ExplainP
+00002f70: 6970 656c 696e 6546 6163 746f 7279 285f  ipelineFactory(_
+00002f80: 4f63 6965 6e74 5265 7175 6573 7446 6163  OcientRequestFac
+00002f90: 746f 7279 5b70 726f 746f 2e45 7870 6c61  tory[proto.Expla
+00002fa0: 696e 5069 7065 6c69 6e65 5265 7370 6f6e  inPipelineRespon
+00002fb0: 7365 5d29 3a0a 2020 2020 6465 6620 7265  se]):.    def re
+00002fc0: 7175 6573 7428 7365 6c66 2c20 6f70 6572  quest(self, oper
+00002fd0: 6174 696f 6e3a 2073 7472 2920 2d3e 2070  ation: str) -> p
+00002fe0: 726f 746f 2e52 6571 7565 7374 3a0a 2020  roto.Request:.  
+00002ff0: 2020 2020 2020 2222 2247 656e 6572 6174        """Generat
+00003000: 6573 2061 2066 756c 6c79 2070 6f70 756c  es a fully popul
+00003010: 6174 6564 2045 5850 4c41 494e 5f50 4950  ated EXPLAIN_PIP
+00003020: 454c 494e 4520 7265 7175 6573 7420 7072  ELINE request pr
+00003030: 6f74 6f62 7566 2222 220a 2020 2020 2020  otobuf""".      
+00003040: 2020 7265 7120 3d20 7072 6f74 6f2e 5265    req = proto.Re
+00003050: 7175 6573 7428 290a 2020 2020 2020 2020  quest().        
+00003060: 7265 712e 7479 7065 203d 2070 726f 746f  req.type = proto
+00003070: 2e52 6571 7565 7374 2e52 6571 7565 7374  .Request.Request
+00003080: 5479 7065 2e56 616c 7565 2822 4558 504c  Type.Value("EXPL
+00003090: 4149 4e5f 5049 5045 4c49 4e45 2229 2020  AIN_PIPELINE")  
+000030a0: 2320 7479 7065 3a20 6967 6e6f 7265 2023  # type: ignore #
+000030b0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+000030c0: 636f 6d2f 7072 6f74 6f63 6f6c 6275 6666  com/protocolbuff
+000030d0: 6572 732f 7072 6f74 6f62 7566 2f69 7373  ers/protobuf/iss
+000030e0: 7565 732f 3130 3234 300a 2020 2020 2020  ues/10240.      
+000030f0: 2020 7265 712e 6578 706c 6169 6e5f 7069    req.explain_pi
+00003100: 7065 6c69 6e65 2e73 716c 203d 206f 7065  peline.sql = ope
+00003110: 7261 7469 6f6e 0a20 2020 2020 2020 2072  ration.        r
+00003120: 6574 7572 6e20 7265 710a 0a20 2020 2064  eturn req..    d
+00003130: 6566 2072 6573 706f 6e73 6528 7365 6c66  ef response(self
+00003140: 2920 2d3e 2070 726f 746f 2e45 7870 6c61  ) -> proto.Expla
+00003150: 696e 5069 7065 6c69 6e65 5265 7370 6f6e  inPipelineRespon
+00003160: 7365 3a0a 2020 2020 2020 2020 2222 2247  se:.        """G
+00003170: 656e 6572 6174 6573 2061 2066 756c 6c79  enerates a fully
+00003180: 2070 6f70 756c 6174 6564 2045 5850 4c41   populated EXPLA
+00003190: 494e 5f50 4950 454c 494e 4520 7265 7370  IN_PIPELINE resp
+000031a0: 6f6e 7365 2070 726f 746f 6275 6622 2222  onse protobuf"""
+000031b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000031c0: 7072 6f74 6f2e 4578 706c 6169 6e50 6970  proto.ExplainPip
+000031d0: 656c 696e 6552 6573 706f 6e73 6528 290a  elineResponse().
+000031e0: 0a0a 636c 6173 7320 5f43 6865 636b 4461  ..class _CheckDa
+000031f0: 7461 4661 6374 6f72 7928 5f4f 6369 656e  taFactory(_Ocien
+00003200: 7452 6571 7565 7374 4661 6374 6f72 795b  tRequestFactory[
+00003210: 7072 6f74 6f2e 4368 6563 6b44 6174 6152  proto.CheckDataR
+00003220: 6573 706f 6e73 655d 293a 0a20 2020 2022  esponse]):.    "
+00003230: 2222 4e4f 5445 3a20 7468 6973 2063 6f6d  ""NOTE: this com
+00003240: 6d61 6e64 2069 7320 6465 7072 6563 6174  mand is deprecat
+00003250: 6564 2222 220a 0a20 2020 2064 6566 2072  ed"""..    def r
+00003260: 6571 7565 7374 2873 656c 662c 206f 7065  equest(self, ope
+00003270: 7261 7469 6f6e 3a20 7374 7229 202d 3e20  ration: str) -> 
+00003280: 7072 6f74 6f2e 5265 7175 6573 743a 0a20  proto.Request:. 
+00003290: 2020 2020 2020 2022 2222 4765 6e65 7261         """Genera
+000032a0: 7465 7320 6120 6675 6c6c 7920 706f 7075  tes a fully popu
+000032b0: 6c61 7465 6420 4348 4543 4b5f 4441 5441  lated CHECK_DATA
+000032c0: 2072 6571 7565 7374 2070 726f 746f 6275   request protobu
+000032d0: 6622 2222 0a20 2020 2020 2020 2072 6571  f""".        req
+000032e0: 203d 2070 726f 746f 2e52 6571 7565 7374   = proto.Request
+000032f0: 2829 0a20 2020 2020 2020 2072 6571 2e74  ().        req.t
+00003300: 7970 6520 3d20 7072 6f74 6f2e 5265 7175  ype = proto.Requ
+00003310: 6573 742e 5265 7175 6573 7454 7970 652e  est.RequestType.
+00003320: 5661 6c75 6528 2243 4845 434b 5f44 4154  Value("CHECK_DAT
+00003330: 4122 2920 2023 2074 7970 653a 2069 676e  A")  # type: ign
+00003340: 6f72 6520 2320 6874 7470 733a 2f2f 6769  ore # https://gi
+00003350: 7468 7562 2e63 6f6d 2f70 726f 746f 636f  thub.com/protoco
+00003360: 6c62 7566 6665 7273 2f70 726f 746f 6275  lbuffers/protobu
+00003370: 662f 6973 7375 6573 2f31 3032 3430 0a20  f/issues/10240. 
+00003380: 2020 2020 2020 2072 6571 2e63 6865 636b         req.check
+00003390: 5f64 6174 612e 7371 6c20 3d20 6f70 6572  _data.sql = oper
+000033a0: 6174 696f 6e0a 2020 2020 2020 2020 7265  ation.        re
+000033b0: 7475 726e 2072 6571 0a0a 2020 2020 6465  turn req..    de
+000033c0: 6620 7265 7370 6f6e 7365 2873 656c 6629  f response(self)
+000033d0: 202d 3e20 7072 6f74 6f2e 4368 6563 6b44   -> proto.CheckD
+000033e0: 6174 6152 6573 706f 6e73 653a 0a20 2020  ataResponse:.   
+000033f0: 2020 2020 2022 2222 4765 6e65 7261 7465       """Generate
+00003400: 7320 6120 6675 6c6c 7920 706f 7075 6c61  s a fully popula
+00003410: 7465 6420 4348 4543 4b5f 4441 5441 2072  ted CHECK_DATA r
+00003420: 6573 706f 6e73 6520 7072 6f74 6f62 7566  esponse protobuf
+00003430: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+00003440: 726e 2070 726f 746f 2e43 6865 636b 4461  rn proto.CheckDa
+00003450: 7461 5265 7370 6f6e 7365 2829 0a0a 0a63  taResponse()...c
+00003460: 6c61 7373 205f 466f 7263 6545 7874 6572  lass _ForceExter
+00003470: 6e61 6c46 6163 746f 7279 285f 4f63 6965  nalFactory(_Ocie
+00003480: 6e74 5265 7175 6573 7446 6163 746f 7279  ntRequestFactory
+00003490: 5b70 726f 746f 2e43 6f6e 6669 726d 6174  [proto.Confirmat
+000034a0: 696f 6e52 6573 706f 6e73 655d 293a 0a20  ionResponse]):. 
+000034b0: 2020 2064 6566 2072 6571 7565 7374 2873     def request(s
+000034c0: 656c 662c 206f 7065 7261 7469 6f6e 3a20  elf, operation: 
+000034d0: 7374 7229 202d 3e20 7072 6f74 6f2e 5265  str) -> proto.Re
+000034e0: 7175 6573 743a 0a20 2020 2020 2020 2022  quest:.        "
+000034f0: 2222 4765 6e65 7261 7465 7320 6120 6675  ""Generates a fu
+00003500: 6c6c 7920 706f 7075 6c61 7465 6420 464f  lly populated FO
+00003510: 5243 455f 4558 5445 524e 414c 2072 6571  RCE_EXTERNAL req
+00003520: 7565 7374 2070 726f 746f 6275 6622 2222  uest protobuf"""
+00003530: 0a20 2020 2020 2020 2072 6571 203d 2070  .        req = p
+00003540: 726f 746f 2e52 6571 7565 7374 2829 0a20  roto.Request(). 
+00003550: 2020 2020 2020 2072 6571 2e74 7970 6520         req.type 
+00003560: 3d20 7072 6f74 6f2e 5265 7175 6573 742e  = proto.Request.
+00003570: 5265 7175 6573 7454 7970 652e 5661 6c75  RequestType.Valu
+00003580: 6528 2253 4554 5f50 4152 414d 4554 4552  e("SET_PARAMETER
+00003590: 2229 2020 2320 7479 7065 3a20 6967 6e6f  ")  # type: igno
+000035a0: 7265 2023 2068 7474 7073 3a2f 2f67 6974  re # https://git
+000035b0: 6875 622e 636f 6d2f 7072 6f74 6f63 6f6c  hub.com/protocol
+000035c0: 6275 6666 6572 732f 7072 6f74 6f62 7566  buffers/protobuf
+000035d0: 2f69 7373 7565 732f 3130 3234 300a 2020  /issues/10240.  
+000035e0: 2020 2020 2020 7370 203d 2072 6571 2e73        sp = req.s
+000035f0: 6574 5f70 6172 616d 6574 6572 0a20 2020  et_parameter.   
+00003600: 2020 2020 2069 6620 6f70 6572 6174 696f       if operatio
+00003610: 6e2e 656e 6473 7769 7468 2822 6f6e 2229  n.endswith("on")
+00003620: 3a0a 2020 2020 2020 2020 2020 2020 7370  :.            sp
+00003630: 2e66 6f72 6365 5f65 7874 6572 6e61 6c2e  .force_external.
+00003640: 6973 5f6f 6e20 3d20 5472 7565 0a20 2020  is_on = True.   
+00003650: 2020 2020 2065 6c69 6620 6f70 6572 6174       elif operat
+00003660: 696f 6e2e 656e 6473 7769 7468 2822 6f66  ion.endswith("of
+00003670: 6622 293a 0a20 2020 2020 2020 2020 2020  f"):.           
+00003680: 2073 702e 666f 7263 655f 6578 7465 726e   sp.force_extern
+00003690: 616c 2e69 735f 6f6e 203d 2046 616c 7365  al.is_on = False
+000036a0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+000036b0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+000036c0: 2050 726f 6772 616d 6d69 6e67 4572 726f   ProgrammingErro
+000036d0: 7228 2746 6f72 6d61 7420 6d75 7374 2062  r('Format must b
+000036e0: 6520 2246 4f52 4345 2045 5854 4552 4e41  e "FORCE EXTERNA
+000036f0: 4c20 286f 6e7c 6f66 6629 2227 290a 2020  L (on|off)"').  
+00003700: 2020 2020 2020 7265 7475 726e 2072 6571        return req
+00003710: 0a0a 2020 2020 6465 6620 7265 7370 6f6e  ..    def respon
+00003720: 7365 2873 656c 6629 202d 3e20 7072 6f74  se(self) -> prot
+00003730: 6f2e 436f 6e66 6972 6d61 7469 6f6e 5265  o.ConfirmationRe
+00003740: 7370 6f6e 7365 3a0a 2020 2020 2020 2020  sponse:.        
+00003750: 2222 2247 656e 6572 6174 6573 2061 2066  """Generates a f
+00003760: 756c 6c79 2070 6f70 756c 6174 6564 2046  ully populated F
+00003770: 4f52 4345 5f45 5854 4552 4e41 4c20 7265  ORCE_EXTERNAL re
+00003780: 7370 6f6e 7365 2070 726f 746f 6275 6622  sponse protobuf"
+00003790: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+000037a0: 6e20 7072 6f74 6f2e 436f 6e66 6972 6d61  n proto.Confirma
+000037b0: 7469 6f6e 5265 7370 6f6e 7365 2829 0a0a  tionResponse()..
+000037c0: 0a63 6c61 7373 205f 5365 7453 6368 656d  .class _SetSchem
+000037d0: 6146 6163 746f 7279 285f 4f63 6965 6e74  aFactory(_Ocient
+000037e0: 5265 7175 6573 7446 6163 746f 7279 5b70  RequestFactory[p
+000037f0: 726f 746f 2e43 6f6e 6669 726d 6174 696f  roto.Confirmatio
+00003800: 6e52 6573 706f 6e73 655d 293a 0a20 2020  nResponse]):.   
+00003810: 2064 6566 2072 6571 7565 7374 2873 656c   def request(sel
+00003820: 662c 2073 6368 656d 613a 2073 7472 2920  f, schema: str) 
+00003830: 2d3e 2070 726f 746f 2e52 6571 7565 7374  -> proto.Request
+00003840: 3a0a 2020 2020 2020 2020 2222 2247 656e  :.        """Gen
+00003850: 6572 6174 6573 2061 2066 756c 6c79 2070  erates a fully p
+00003860: 6f70 756c 6174 6564 2053 4554 2053 4348  opulated SET SCH
+00003870: 454d 4120 7265 7175 6573 7420 7072 6f74  EMA request prot
+00003880: 6f62 7566 2222 220a 2020 2020 2020 2020  obuf""".        
+00003890: 7265 7120 3d20 7072 6f74 6f2e 5265 7175  req = proto.Requ
+000038a0: 6573 7428 290a 2020 2020 2020 2020 7265  est().        re
+000038b0: 712e 7479 7065 203d 2070 726f 746f 2e52  q.type = proto.R
+000038c0: 6571 7565 7374 2e52 6571 7565 7374 5479  equest.RequestTy
+000038d0: 7065 2e56 616c 7565 2822 5345 545f 5343  pe.Value("SET_SC
+000038e0: 4845 4d41 2229 2020 2320 7479 7065 3a20  HEMA")  # type: 
+000038f0: 6967 6e6f 7265 2023 2068 7474 7073 3a2f  ignore # https:/
+00003900: 2f67 6974 6875 622e 636f 6d2f 7072 6f74  /github.com/prot
+00003910: 6f63 6f6c 6275 6666 6572 732f 7072 6f74  ocolbuffers/prot
+00003920: 6f62 7566 2f69 7373 7565 732f 3130 3234  obuf/issues/1024
+00003930: 300a 2020 2020 2020 2020 7265 712e 7365  0.        req.se
+00003940: 745f 7363 6865 6d61 2e73 6368 656d 6120  t_schema.schema 
+00003950: 3d20 7363 6865 6d61 0a20 2020 2020 2020  = schema.       
+00003960: 2072 6574 7572 6e20 7265 710a 0a20 2020   return req..   
+00003970: 2064 6566 2072 6573 706f 6e73 6528 7365   def response(se
+00003980: 6c66 2920 2d3e 2070 726f 746f 2e43 6f6e  lf) -> proto.Con
+00003990: 6669 726d 6174 696f 6e52 6573 706f 6e73  firmationRespons
+000039a0: 653a 0a20 2020 2020 2020 2022 2222 4765  e:.        """Ge
+000039b0: 6e65 7261 7465 7320 5345 545f 5343 4845  nerates SET_SCHE
+000039c0: 4d41 2072 6573 706f 6e73 6520 7072 6f74  MA response prot
+000039d0: 6f62 7566 2222 220a 2020 2020 2020 2020  obuf""".        
+000039e0: 7265 7475 726e 2070 726f 746f 2e43 6f6e  return proto.Con
+000039f0: 6669 726d 6174 696f 6e52 6573 706f 6e73  firmationRespons
+00003a00: 6528 290a 0a0a 636c 6173 7320 5f47 6574  e()...class _Get
+00003a10: 5363 6865 6d61 4661 6374 6f72 7928 5f4f  SchemaFactory(_O
+00003a20: 6369 656e 7452 6571 7565 7374 4661 6374  cientRequestFact
+00003a30: 6f72 795b 7072 6f74 6f2e 4765 7453 6368  ory[proto.GetSch
+00003a40: 656d 6152 6573 706f 6e73 655d 293a 0a20  emaResponse]):. 
+00003a50: 2020 2064 6566 2072 6571 7565 7374 2873     def request(s
+00003a60: 656c 6629 202d 3e20 7072 6f74 6f2e 5265  elf) -> proto.Re
+00003a70: 7175 6573 743a 2020 2320 7479 7065 3a20  quest:  # type: 
+00003a80: 6967 6e6f 7265 0a20 2020 2020 2020 2022  ignore.        "
+00003a90: 2222 4765 6e65 7261 7465 7320 6120 6675  ""Generates a fu
+00003aa0: 6c6c 7920 706f 7075 6c61 7465 6420 4745  lly populated GE
+00003ab0: 5420 5343 4845 4d41 2072 6571 7565 7374  T SCHEMA request
+00003ac0: 2070 726f 746f 6275 6622 2222 0a20 2020   protobuf""".   
+00003ad0: 2020 2020 2072 6571 203d 2070 726f 746f       req = proto
+00003ae0: 2e52 6571 7565 7374 2829 0a20 2020 2020  .Request().     
+00003af0: 2020 2072 6571 2e74 7970 6520 3d20 7072     req.type = pr
+00003b00: 6f74 6f2e 5265 7175 6573 742e 5265 7175  oto.Request.Requ
+00003b10: 6573 7454 7970 652e 5661 6c75 6528 2247  estType.Value("G
+00003b20: 4554 5f53 4348 454d 4122 2920 2023 2074  ET_SCHEMA")  # t
+00003b30: 7970 653a 2069 676e 6f72 6520 2320 6874  ype: ignore # ht
+00003b40: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00003b50: 2f70 726f 746f 636f 6c62 7566 6665 7273  /protocolbuffers
+00003b60: 2f70 726f 746f 6275 662f 6973 7375 6573  /protobuf/issues
+00003b70: 2f31 3032 3430 0a20 2020 2020 2020 2072  /10240.        r
+00003b80: 6574 7572 6e20 7265 710a 0a20 2020 2064  eturn req..    d
+00003b90: 6566 2072 6573 706f 6e73 6528 7365 6c66  ef response(self
+00003ba0: 2920 2d3e 2070 726f 746f 2e47 6574 5363  ) -> proto.GetSc
+00003bb0: 6865 6d61 5265 7370 6f6e 7365 3a0a 2020  hemaResponse:.  
+00003bc0: 2020 2020 2020 2222 2247 656e 6572 6174        """Generat
+00003bd0: 6573 2053 4554 5f53 4348 454d 4120 7265  es SET_SCHEMA re
+00003be0: 7370 6f6e 7365 2070 726f 746f 6275 6622  sponse protobuf"
+00003bf0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+00003c00: 6e20 7072 6f74 6f2e 4765 7453 6368 656d  n proto.GetSchem
+00003c10: 6152 6573 706f 6e73 6528 290a 0a0a 636c  aResponse()...cl
+00003c20: 6173 7320 5f43 6c65 6172 4361 6368 6546  ass _ClearCacheF
+00003c30: 6163 746f 7279 285f 4f63 6965 6e74 5265  actory(_OcientRe
+00003c40: 7175 6573 7446 6163 746f 7279 5b70 726f  questFactory[pro
+00003c50: 746f 2e43 6f6e 6669 726d 6174 696f 6e52  to.ConfirmationR
+00003c60: 6573 706f 6e73 655d 293a 0a20 2020 2064  esponse]):.    d
+00003c70: 6566 2072 6571 7565 7374 2873 656c 6629  ef request(self)
+00003c80: 202d 3e20 7072 6f74 6f2e 5265 7175 6573   -> proto.Reques
+00003c90: 743a 2020 2320 7479 7065 3a20 6967 6e6f  t:  # type: igno
+00003ca0: 7265 0a20 2020 2020 2020 2022 2222 4765  re.        """Ge
+00003cb0: 6e65 7261 7465 7320 6120 6675 6c6c 7920  nerates a fully 
+00003cc0: 706f 7075 6c61 7465 6420 434c 4541 5220  populated CLEAR 
+00003cd0: 4341 4348 4520 7265 7175 6573 7420 7072  CACHE request pr
+00003ce0: 6f74 6f62 7566 2222 220a 2020 2020 2020  otobuf""".      
+00003cf0: 2020 7265 7120 3d20 7072 6f74 6f2e 5265    req = proto.Re
+00003d00: 7175 6573 7428 290a 2020 2020 2020 2020  quest().        
+00003d10: 7265 712e 7479 7065 203d 2070 726f 746f  req.type = proto
+00003d20: 2e52 6571 7565 7374 2e52 6571 7565 7374  .Request.Request
+00003d30: 5479 7065 2e56 616c 7565 2822 434c 4541  Type.Value("CLEA
+00003d40: 525f 4341 4348 4522 2920 2023 2074 7970  R_CACHE")  # typ
+00003d50: 653a 2069 676e 6f72 6520 2320 6874 7470  e: ignore # http
+00003d60: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
+00003d70: 726f 746f 636f 6c62 7566 6665 7273 2f70  rotocolbuffers/p
+00003d80: 726f 746f 6275 662f 6973 7375 6573 2f31  rotobuf/issues/1
+00003d90: 3032 3430 0a20 2020 2020 2020 2072 6571  0240.        req
+00003da0: 2e63 6c65 6172 5f63 6163 6865 2e61 6c6c  .clear_cache.all
+00003db0: 5f6e 6f64 6573 203d 2054 7275 650a 2020  _nodes = True.  
+00003dc0: 2020 2020 2020 7265 7475 726e 2072 6571        return req
+00003dd0: 0a0a 2020 2020 6465 6620 7265 7370 6f6e  ..    def respon
+00003de0: 7365 2873 656c 6629 202d 3e20 7072 6f74  se(self) -> prot
+00003df0: 6f2e 436f 6e66 6972 6d61 7469 6f6e 5265  o.ConfirmationRe
+00003e00: 7370 6f6e 7365 3a0a 2020 2020 2020 2020  sponse:.        
+00003e10: 2222 2247 656e 6572 6174 6573 2053 4554  """Generates SET
+00003e20: 5f53 4348 454d 4120 7265 7370 6f6e 7365  _SCHEMA response
+00003e30: 2070 726f 746f 6275 6622 2222 0a20 2020   protobuf""".   
+00003e40: 2020 2020 2072 6574 7572 6e20 7072 6f74       return prot
+00003e50: 6f2e 436f 6e66 6972 6d61 7469 6f6e 5265  o.ConfirmationRe
+00003e60: 7370 6f6e 7365 2829 0a0a 0a63 6c61 7373  sponse()...class
+00003e70: 205f 5365 7450 6172 616d 6574 6572 4661   _SetParameterFa
+00003e80: 6374 6f72 7928 5f4f 6369 656e 7452 6571  ctory(_OcientReq
+00003e90: 7565 7374 4661 6374 6f72 795b 7072 6f74  uestFactory[prot
+00003ea0: 6f2e 436f 6e66 6972 6d61 7469 6f6e 5265  o.ConfirmationRe
+00003eb0: 7370 6f6e 7365 5d29 3a0a 2020 2020 6465  sponse]):.    de
+00003ec0: 6620 7265 7175 6573 7428 7365 6c66 2c20  f request(self, 
+00003ed0: 6f70 3a20 7374 722c 2076 616c 3a20 556e  op: str, val: Un
+00003ee0: 696f 6e5b 696e 742c 2073 7472 2c20 666c  ion[int, str, fl
+00003ef0: 6f61 745d 2920 2d3e 2070 726f 746f 2e52  oat]) -> proto.R
+00003f00: 6571 7565 7374 3a20 2023 2074 7970 653a  equest:  # type:
+00003f10: 2069 676e 6f72 650a 2020 2020 2020 2020   ignore.        
+00003f20: 2222 2247 656e 6572 6174 6573 2061 2066  """Generates a f
+00003f30: 756c 6c79 2070 6f70 756c 6174 6564 2053  ully populated S
+00003f40: 4554 2050 4152 414d 4554 4552 2072 6571  ET PARAMETER req
+00003f50: 7565 7374 2070 726f 746f 6275 6622 2222  uest protobuf"""
+00003f60: 0a20 2020 2020 2020 2072 6571 203d 2070  .        req = p
+00003f70: 726f 746f 2e52 6571 7565 7374 2829 0a20  roto.Request(). 
+00003f80: 2020 2020 2020 2072 6571 2e74 7970 6520         req.type 
+00003f90: 3d20 7072 6f74 6f2e 5265 7175 6573 742e  = proto.Request.
+00003fa0: 5265 7175 6573 7454 7970 652e 5661 6c75  RequestType.Valu
+00003fb0: 6528 2253 4554 5f50 4152 414d 4554 4552  e("SET_PARAMETER
+00003fc0: 2229 2020 2320 7479 7065 3a20 6967 6e6f  ")  # type: igno
+00003fd0: 7265 2023 2068 7474 7073 3a2f 2f67 6974  re # https://git
+00003fe0: 6875 622e 636f 6d2f 7072 6f74 6f63 6f6c  hub.com/protocol
+00003ff0: 6275 6666 6572 732f 7072 6f74 6f62 7566  buffers/protobuf
+00004000: 2f69 7373 7565 732f 3130 3234 300a 0a20  /issues/10240.. 
+00004010: 2020 2020 2020 2073 7020 3d20 7265 712e         sp = req.
+00004020: 7365 745f 7061 7261 6d65 7465 720a 0a20  set_parameter.. 
+00004030: 2020 2020 2020 2069 6620 7479 7065 2876         if type(v
+00004040: 616c 2920 3d3d 2073 7472 2061 6e64 2076  al) == str and v
+00004050: 616c 2e6c 6f77 6572 2829 203d 3d20 2272  al.lower() == "r
+00004060: 6573 6574 223a 0a20 2020 2020 2020 2020  eset":.         
+00004070: 2020 2023 2052 6573 6574 7320 6861 6e64     # Resets hand
+00004080: 6c65 6420 696e 2063 6d64 436f 6d70 5365  led in cmdCompSe
+00004090: 7276 6572 2e20 5365 7420 7661 6c20 746f  rver. Set val to
+000040a0: 2030 2061 7320 6120 5061 7261 6d65 7465   0 as a Paramete
+000040b0: 7220 7374 696c 6c20 6e65 6564 7320 746f  r still needs to
+000040c0: 2062 6520 7365 7420 666f 7220 666c 6f77   be set for flow
+000040d0: 2063 6f6e 7472 6f6c 2c20 616e 6420 6d6f   control, and mo
+000040e0: 7374 2072 6571 7569 7265 206e 756d 6265  st require numbe
+000040f0: 7220 7661 6c75 6573 0a20 2020 2020 2020  r values.       
+00004100: 2020 2020 2073 702e 7265 7365 7420 3d20       sp.reset = 
+00004110: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
+00004120: 2076 616c 203d 2030 2069 6620 6f70 2021   val = 0 if op !
+00004130: 3d20 2253 4552 5649 4345 434c 4153 5322  = "SERVICECLASS"
+00004140: 2065 6c73 6520 7661 6c0a 0a20 2020 2020   else val..     
+00004150: 2020 2023 2053 6574 2074 6865 2061 7070     # Set the app
+00004160: 726f 7072 6961 7465 2070 6172 616d 6574  ropriate paramet
+00004170: 6572 0a20 2020 2020 2020 2023 2070 726f  er.        # pro
+00004180: 746f 2066 6965 6c64 2061 7373 6967 6e6d  to field assignm
+00004190: 656e 7473 2061 7265 2074 7970 6520 6368  ents are type ch
+000041a0: 6563 6b65 6420 6174 2072 756e 7469 6d65  ecked at runtime
+000041b0: 0a20 2020 2020 2020 2069 6620 6f70 203d  .        if op =
+000041c0: 3d20 224d 4158 524f 5753 223a 0a20 2020  = "MAXROWS":.   
+000041d0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+000041e0: 6973 696e 7374 616e 6365 2876 616c 2c20  isinstance(val, 
+000041f0: 696e 7429 0a20 2020 2020 2020 2020 2020  int).           
+00004200: 2073 702e 726f 775f 6c69 6d69 742e 726f   sp.row_limit.ro
+00004210: 774c 696d 6974 203d 2076 616c 0a20 2020  wLimit = val.   
+00004220: 2020 2020 2065 6c69 6620 6f70 203d 3d20       elif op == 
+00004230: 224d 4158 5449 4d45 223a 0a20 2020 2020  "MAXTIME":.     
+00004240: 2020 2020 2020 2061 7373 6572 7420 6973         assert is
+00004250: 696e 7374 616e 6365 2876 616c 2c20 696e  instance(val, in
+00004260: 7429 0a20 2020 2020 2020 2020 2020 2073  t).            s
+00004270: 702e 7469 6d65 5f6c 696d 6974 2e74 696d  p.time_limit.tim
+00004280: 654c 696d 6974 203d 2076 616c 0a20 2020  eLimit = val.   
+00004290: 2020 2020 2065 6c69 6620 6f70 203d 3d20       elif op == 
+000042a0: 224d 4158 5445 4d50 4449 534b 223a 0a20  "MAXTEMPDISK":. 
+000042b0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+000042c0: 7420 6973 696e 7374 616e 6365 2876 616c  t isinstance(val
+000042d0: 2c20 696e 7429 0a20 2020 2020 2020 2020  , int).         
+000042e0: 2020 2073 702e 7465 6d70 5f64 6973 6b5f     sp.temp_disk_
+000042f0: 6c69 6d69 742e 7465 6d70 4469 736b 4c69  limit.tempDiskLi
+00004300: 6d69 7420 3d20 7661 6c0a 2020 2020 2020  mit = val.      
+00004310: 2020 656c 6966 206f 7020 3d3d 2022 5052    elif op == "PR
+00004320: 494f 5249 5459 223a 0a20 2020 2020 2020  IORITY":.       
+00004330: 2020 2020 2061 7373 6572 7420 6973 696e       assert isin
+00004340: 7374 616e 6365 2876 616c 2c20 666c 6f61  stance(val, floa
+00004350: 7429 0a20 2020 2020 2020 2020 2020 2073  t).            s
+00004360: 702e 7072 696f 7269 7479 2e70 7269 6f72  p.priority.prior
+00004370: 6974 7920 3d20 7661 6c0a 2020 2020 2020  ity = val.      
+00004380: 2020 656c 6966 206f 7020 3d3d 2022 5041    elif op == "PA
+00004390: 5241 4c4c 454c 4953 4d22 3a0a 2020 2020  RALLELISM":.    
+000043a0: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
+000043b0: 7369 6e73 7461 6e63 6528 7661 6c2c 2069  sinstance(val, i
+000043c0: 6e74 290a 2020 2020 2020 2020 2020 2020  nt).            
+000043d0: 7370 2e63 6f6e 6375 7272 656e 6379 2e63  sp.concurrency.c
+000043e0: 6f6e 6375 7272 656e 6379 203d 2076 616c  oncurrency = val
+000043f0: 0a20 2020 2020 2020 2065 6c69 6620 6f70  .        elif op
+00004400: 203d 3d20 2253 4552 5649 4345 434c 4153   == "SERVICECLAS
+00004410: 5322 3a0a 2020 2020 2020 2020 2020 2020  S":.            
+00004420: 6173 7365 7274 2069 7369 6e73 7461 6e63  assert isinstanc
+00004430: 6528 7661 6c2c 2073 7472 290a 2020 2020  e(val, str).    
+00004440: 2020 2020 2020 2020 7370 2e73 6572 7669          sp.servi
+00004450: 6365 5f63 6c61 7373 5f6e 616d 652e 7365  ce_class_name.se
+00004460: 7276 6963 655f 636c 6173 735f 6e61 6d65  rvice_class_name
+00004470: 203d 2076 616c 0a20 2020 2020 2020 2065   = val.        e
+00004480: 6c69 6620 6f70 203d 3d20 2250 534f 223a  lif op == "PSO":
+00004490: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
+000044a0: 6572 7420 6973 696e 7374 616e 6365 2876  ert isinstance(v
+000044b0: 616c 2c20 696e 7429 0a20 2020 2020 2020  al, int).       
+000044c0: 2020 2020 2073 702e 7073 6f5f 7468 7265       sp.pso_thre
+000044d0: 7368 6f6c 642e 7468 7265 7368 6f6c 6420  shold.threshold 
+000044e0: 3d20 7661 6c0a 2020 2020 2020 2020 656c  = val.        el
+000044f0: 6966 206f 7020 3d3d 2022 4144 4a55 5354  if op == "ADJUST
+00004500: 4641 4354 4f52 223a 0a20 2020 2020 2020  FACTOR":.       
+00004510: 2020 2020 2061 7373 6572 7420 6973 696e       assert isin
+00004520: 7374 616e 6365 2876 616c 2c20 666c 6f61  stance(val, floa
+00004530: 7429 0a20 2020 2020 2020 2020 2020 2073  t).            s
+00004540: 702e 7072 696f 7269 7479 5f61 646a 7573  p.priority_adjus
+00004550: 745f 6661 6374 6f72 2e70 7269 6f72 6974  t_factor.priorit
+00004560: 795f 6164 6a75 7374 5f66 6163 746f 7220  y_adjust_factor 
+00004570: 3d20 7661 6c0a 2020 2020 2020 2020 656c  = val.        el
+00004580: 6966 206f 7020 3d3d 2022 4144 4a55 5354  if op == "ADJUST
+00004590: 5449 4d45 223a 0a20 2020 2020 2020 2020  TIME":.         
+000045a0: 2020 2061 7373 6572 7420 6973 696e 7374     assert isinst
+000045b0: 616e 6365 2876 616c 2c20 696e 7429 0a20  ance(val, int). 
+000045c0: 2020 2020 2020 2020 2020 2073 702e 7072             sp.pr
+000045d0: 696f 7269 7479 5f61 646a 7573 745f 7469  iority_adjust_ti
+000045e0: 6d65 2e70 7269 6f72 6974 795f 6164 6a75  me.priority_adju
+000045f0: 7374 5f74 696d 6520 3d20 7661 6c0a 2020  st_time = val.  
+00004600: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00004610: 2020 2020 2020 2020 7261 6973 6520 5072          raise Pr
+00004620: 6f67 7261 6d6d 696e 6745 7272 6f72 2872  ogrammingError(r
+00004630: 6561 736f 6e3d 6622 5379 6e74 6178 2065  eason=f"Syntax e
+00004640: 7272 6f72 2e20 496e 7661 6c69 6420 5345  rror. Invalid SE
+00004650: 5420 7b6f 707d 2229 0a0a 2020 2020 2020  T {op}")..      
+00004660: 2020 7265 7475 726e 2072 6571 0a0a 2020    return req..  
+00004670: 2020 6465 6620 7265 7370 6f6e 7365 2873    def response(s
+00004680: 656c 6629 202d 3e20 7072 6f74 6f2e 436f  elf) -> proto.Co
+00004690: 6e66 6972 6d61 7469 6f6e 5265 7370 6f6e  nfirmationRespon
+000046a0: 7365 3a0a 2020 2020 2020 2020 2222 2247  se:.        """G
+000046b0: 656e 6572 6174 6573 2061 2053 4554 5f50  enerates a SET_P
+000046c0: 4152 414d 4554 4552 2072 6573 706f 6e73  ARAMETER respons
+000046d0: 6520 7072 6f74 6f62 7566 2222 220a 2020  e protobuf""".  
+000046e0: 2020 2020 2020 7265 7475 726e 2070 726f        return pro
+000046f0: 746f 2e43 6f6e 6669 726d 6174 696f 6e52  to.ConfirmationR
+00004700: 6573 706f 6e73 6528 290a 0a0a 636c 6173  esponse()...clas
+00004710: 7320 5f43 616e 6365 6c51 7565 7279 4661  s _CancelQueryFa
+00004720: 6374 6f72 7928 5f4f 6369 656e 7452 6571  ctory(_OcientReq
+00004730: 7565 7374 4661 6374 6f72 795b 7072 6f74  uestFactory[prot
+00004740: 6f2e 4361 6e63 656c 5175 6572 7952 6573  o.CancelQueryRes
+00004750: 706f 6e73 655d 293a 0a20 2020 2064 6566  ponse]):.    def
+00004760: 2072 6571 7565 7374 2873 656c 662c 2069   request(self, i
+00004770: 643a 2073 7472 2920 2d3e 2070 726f 746f  d: str) -> proto
+00004780: 2e52 6571 7565 7374 3a0a 2020 2020 2020  .Request:.      
+00004790: 2020 2222 2247 656e 6572 6174 6573 2061    """Generates a
+000047a0: 2066 756c 6c79 2070 6f70 756c 6174 6564   fully populated
+000047b0: 2043 414e 4345 4c20 5155 4552 5920 7265   CANCEL QUERY re
+000047c0: 7175 6573 7420 7072 6f74 6f62 7566 2222  quest protobuf""
+000047d0: 220a 2020 2020 2020 2020 7265 7120 3d20  ".        req = 
+000047e0: 7072 6f74 6f2e 5265 7175 6573 7428 290a  proto.Request().
+000047f0: 2020 2020 2020 2020 7265 712e 7479 7065          req.type
+00004800: 203d 2070 726f 746f 2e52 6571 7565 7374   = proto.Request
+00004810: 2e52 6571 7565 7374 5479 7065 2e56 616c  .RequestType.Val
+00004820: 7565 2822 4341 4e43 454c 5f51 5545 5259  ue("CANCEL_QUERY
+00004830: 2229 2020 2320 7479 7065 3a20 6967 6e6f  ")  # type: igno
+00004840: 7265 2023 2068 7474 7073 3a2f 2f67 6974  re # https://git
+00004850: 6875 622e 636f 6d2f 7072 6f74 6f63 6f6c  hub.com/protocol
+00004860: 6275 6666 6572 732f 7072 6f74 6f62 7566  buffers/protobuf
+00004870: 2f69 7373 7565 732f 3130 3234 300a 2020  /issues/10240.  
+00004880: 2020 2020 2020 7265 712e 6361 6e63 656c        req.cancel
+00004890: 5f71 7565 7279 2e73 716c 203d 2069 640a  _query.sql = id.
+000048a0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+000048b0: 6571 0a0a 2020 2020 6465 6620 7265 7370  eq..    def resp
+000048c0: 6f6e 7365 2873 656c 6629 202d 3e20 7072  onse(self) -> pr
+000048d0: 6f74 6f2e 4361 6e63 656c 5175 6572 7952  oto.CancelQueryR
+000048e0: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
+000048f0: 2022 2222 4765 6e65 7261 7465 7320 6120   """Generates a 
+00004900: 4341 4e43 454c 5f51 5545 5259 2072 6573  CANCEL_QUERY res
+00004910: 706f 6e73 6520 7072 6f74 6f62 7566 2222  ponse protobuf""
+00004920: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+00004930: 2070 726f 746f 2e43 616e 6365 6c51 7565   proto.CancelQue
+00004940: 7279 5265 7370 6f6e 7365 2829 0a0a 0a63  ryResponse()...c
+00004950: 6c61 7373 205f 4b69 6c6c 5175 6572 7946  lass _KillQueryF
+00004960: 6163 746f 7279 285f 4f63 6965 6e74 5265  actory(_OcientRe
+00004970: 7175 6573 7446 6163 746f 7279 5b70 726f  questFactory[pro
+00004980: 746f 2e4b 696c 6c51 7565 7279 5265 7370  to.KillQueryResp
+00004990: 6f6e 7365 5d29 3a0a 2020 2020 6465 6620  onse]):.    def 
+000049a0: 7265 7175 6573 7428 7365 6c66 2c20 6964  request(self, id
+000049b0: 3a20 7374 7229 202d 3e20 7072 6f74 6f2e  : str) -> proto.
+000049c0: 5265 7175 6573 743a 0a20 2020 2020 2020  Request:.       
+000049d0: 2022 2222 4765 6e65 7261 7465 7320 6120   """Generates a 
+000049e0: 6675 6c6c 7920 706f 7075 6c61 7465 6420  fully populated 
+000049f0: 4b49 4c4c 2051 5545 5259 2072 6571 7565  KILL QUERY reque
+00004a00: 7374 2070 726f 746f 6275 6622 2222 0a20  st protobuf""". 
+00004a10: 2020 2020 2020 2072 6571 203d 2070 726f         req = pro
+00004a20: 746f 2e52 6571 7565 7374 2829 0a20 2020  to.Request().   
+00004a30: 2020 2020 2072 6571 2e74 7970 6520 3d20       req.type = 
+00004a40: 7072 6f74 6f2e 5265 7175 6573 742e 5265  proto.Request.Re
+00004a50: 7175 6573 7454 7970 652e 5661 6c75 6528  questType.Value(
+00004a60: 224b 494c 4c5f 5155 4552 5922 2920 2023  "KILL_QUERY")  #
+00004a70: 2074 7970 653a 2069 676e 6f72 6520 2320   type: ignore # 
+00004a80: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00004a90: 6f6d 2f70 726f 746f 636f 6c62 7566 6665  om/protocolbuffe
+00004aa0: 7273 2f70 726f 746f 6275 662f 6973 7375  rs/protobuf/issu
+00004ab0: 6573 2f31 3032 3430 0a20 2020 2020 2020  es/10240.       
+00004ac0: 2072 6571 2e6b 696c 6c5f 7175 6572 792e   req.kill_query.
+00004ad0: 7371 6c20 3d20 6964 0a20 2020 2020 2020  sql = id.       
+00004ae0: 2072 6574 7572 6e20 7265 710a 0a20 2020   return req..   
+00004af0: 2064 6566 2072 6573 706f 6e73 6528 7365   def response(se
+00004b00: 6c66 2920 2d3e 2070 726f 746f 2e4b 696c  lf) -> proto.Kil
+00004b10: 6c51 7565 7279 5265 7370 6f6e 7365 3a0a  lQueryResponse:.
+00004b20: 2020 2020 2020 2020 2222 2247 656e 6572          """Gener
+00004b30: 6174 6573 2061 204b 494c 4c5f 5155 4552  ates a KILL_QUER
+00004b40: 5920 7265 7370 6f6e 7365 2070 726f 746f  Y response proto
+00004b50: 6275 6622 2222 0a20 2020 2020 2020 2072  buf""".        r
+00004b60: 6574 7572 6e20 7072 6f74 6f2e 4b69 6c6c  eturn proto.Kill
+00004b70: 5175 6572 7952 6573 706f 6e73 6528 290a  QueryResponse().
+00004b80: 0a0a 636c 6173 7320 5f47 6574 5379 7374  ..class _GetSyst
+00004b90: 656d 4d65 7461 6461 7461 4661 6374 6f72  emMetadataFactor
+00004ba0: 7928 5f4f 6369 656e 7452 6571 7565 7374  y(_OcientRequest
+00004bb0: 4661 6374 6f72 795b 7072 6f74 6f2e 4665  Factory[proto.Fe
+00004bc0: 7463 6853 7973 7465 6d4d 6574 6164 6174  tchSystemMetadat
+00004bd0: 6152 6573 706f 6e73 655d 293a 0a20 2020  aResponse]):.   
+00004be0: 2064 6566 2072 6571 7565 7374 2873 656c   def request(sel
+00004bf0: 662c 206f 703a 2070 726f 746f 2e46 6574  f, op: proto.Fet
+00004c00: 6368 5379 7374 656d 4d65 7461 6461 7461  chSystemMetadata
+00004c10: 2e53 7973 7465 6d4d 6574 6164 6174 6143  .SystemMetadataC
+00004c20: 616c 6c2c 2073 6368 656d 613a 204f 7074  all, schema: Opt
+00004c30: 696f 6e61 6c5b 7374 725d 2c20 7461 626c  ional[str], tabl
+00004c40: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
+00004c50: 2c20 636f 6c75 6d6e 3a20 4f70 7469 6f6e  , column: Option
+00004c60: 616c 5b73 7472 5d2c 2076 6965 773a 204f  al[str], view: O
+00004c70: 7074 696f 6e61 6c5b 7374 725d 2920 2d3e  ptional[str]) ->
+00004c80: 2070 726f 746f 2e52 6571 7565 7374 3a20   proto.Request: 
+00004c90: 2023 2074 7970 653a 2069 676e 6f72 650a   # type: ignore.
+00004ca0: 2020 2020 2020 2020 2222 2247 656e 6572          """Gener
+00004cb0: 6174 6573 2061 2066 756c 6c79 2070 6f70  ates a fully pop
+00004cc0: 756c 6174 6564 2047 4554 5f53 5953 5445  ulated GET_SYSTE
+00004cd0: 4d5f 4d45 5441 4441 5441 2072 6571 7565  M_METADATA reque
+00004ce0: 7374 2070 726f 746f 6275 6622 2222 0a20  st protobuf""". 
+00004cf0: 2020 2020 2020 2072 6571 203d 2070 726f         req = pro
+00004d00: 746f 2e52 6571 7565 7374 2829 0a20 2020  to.Request().   
+00004d10: 2020 2020 2072 6571 2e74 7970 6520 3d20       req.type = 
+00004d20: 7072 6f74 6f2e 5265 7175 6573 742e 5265  proto.Request.Re
+00004d30: 7175 6573 7454 7970 652e 5661 6c75 6528  questType.Value(
+00004d40: 2246 4554 4348 5f53 5953 5445 4d5f 4d45  "FETCH_SYSTEM_ME
+00004d50: 5441 4441 5441 2229 2020 2320 7479 7065  TADATA")  # type
+00004d60: 3a20 6967 6e6f 7265 2023 2068 7474 7073  : ignore # https
+00004d70: 3a2f 2f67 6974 6875 622e 636f 6d2f 7072  ://github.com/pr
+00004d80: 6f74 6f63 6f6c 6275 6666 6572 732f 7072  otocolbuffers/pr
+00004d90: 6f74 6f62 7566 2f69 7373 7565 732f 3130  otobuf/issues/10
+00004da0: 3234 300a 2020 2020 2020 2020 7265 712e  240.        req.
+00004db0: 6665 7463 685f 7379 7374 656d 5f6d 6574  fetch_system_met
+00004dc0: 6164 6174 612e 6361 6c6c 203d 206f 700a  adata.call = op.
+00004dd0: 0a20 2020 2020 2020 2069 6620 7363 6865  .        if sche
+00004de0: 6d61 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ma is not None:.
+00004df0: 2020 2020 2020 2020 2020 2020 7265 712e              req.
+00004e00: 6665 7463 685f 7379 7374 656d 5f6d 6574  fetch_system_met
+00004e10: 6164 6174 612e 7363 6865 6d61 203d 2073  adata.schema = s
+00004e20: 6368 656d 610a 2020 2020 2020 2020 6966  chema.        if
+00004e30: 2074 6162 6c65 2069 7320 6e6f 7420 4e6f   table is not No
+00004e40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00004e50: 7265 712e 6665 7463 685f 7379 7374 656d  req.fetch_system
+00004e60: 5f6d 6574 6164 6174 612e 7461 626c 6520  _metadata.table 
+00004e70: 3d20 7461 626c 650a 2020 2020 2020 2020  = table.        
+00004e80: 6966 2063 6f6c 756d 6e20 6973 206e 6f74  if column is not
+00004e90: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00004ea0: 2020 2072 6571 2e66 6574 6368 5f73 7973     req.fetch_sys
+00004eb0: 7465 6d5f 6d65 7461 6461 7461 2e63 6f6c  tem_metadata.col
+00004ec0: 756d 6e20 3d20 636f 6c75 6d6e 0a20 2020  umn = column.   
+00004ed0: 2020 2020 2069 6620 7669 6577 2069 7320       if view is 
+00004ee0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00004ef0: 2020 2020 2020 7265 712e 6665 7463 685f        req.fetch_
+00004f00: 7379 7374 656d 5f6d 6574 6164 6174 612e  system_metadata.
+00004f10: 7669 6577 203d 2076 6965 770a 0a20 2020  view = view..   
+00004f20: 2020 2020 2072 6574 7572 6e20 7265 710a       return req.
+00004f30: 0a20 2020 2064 6566 2072 6573 706f 6e73  .    def respons
+00004f40: 6528 7365 6c66 2920 2d3e 2070 726f 746f  e(self) -> proto
+00004f50: 2e46 6574 6368 5379 7374 656d 4d65 7461  .FetchSystemMeta
+00004f60: 6461 7461 5265 7370 6f6e 7365 3a0a 2020  dataResponse:.  
+00004f70: 2020 2020 2020 2222 2247 656e 6572 6174        """Generat
+00004f80: 6573 2061 2066 756c 6c79 2070 6f70 756c  es a fully popul
+00004f90: 6174 6564 2047 4554 5f53 5953 5445 4d5f  ated GET_SYSTEM_
+00004fa0: 4d45 5441 4441 5441 2072 6573 706f 6e73  METADATA respons
+00004fb0: 6520 7072 6f74 6f62 7566 2222 220a 2020  e protobuf""".  
+00004fc0: 2020 2020 2020 7265 7475 726e 2070 726f        return pro
+00004fd0: 746f 2e46 6574 6368 5379 7374 656d 4d65  to.FetchSystemMe
+00004fe0: 7461 6461 7461 5265 7370 6f6e 7365 2829  tadataResponse()
+00004ff0: 0a0a 0a5f 4f43 4945 4e54 5f52 4551 5545  ..._OCIENT_REQUE
+00005000: 5354 5f46 4143 544f 5249 4553 3a20 4d61  ST_FACTORIES: Ma
+00005010: 7070 696e 675b 7374 722c 205f 4f63 6965  pping[str, _Ocie
+00005020: 6e74 5265 7175 6573 7446 6163 746f 7279  ntRequestFactory
+00005030: 5b41 6e79 5d5d 203d 207b 0a20 2020 2022  [Any]] = {.    "
+00005040: 5345 4c45 4354 223a 205f 4578 6563 7574  SELECT": _Execut
+00005050: 6551 7565 7279 4661 6374 6f72 7928 292c  eQueryFactory(),
+00005060: 0a20 2020 2022 5749 5448 223a 205f 4578  .    "WITH": _Ex
+00005070: 6563 7574 6551 7565 7279 4661 6374 6f72  ecuteQueryFactor
+00005080: 7928 292c 0a20 2020 2022 4558 504c 4149  y(),.    "EXPLAI
+00005090: 4e20 5049 5045 4c49 4e45 223a 205f 4578  N PIPELINE": _Ex
+000050a0: 706c 6169 6e50 6970 656c 696e 6546 6163  plainPipelineFac
+000050b0: 746f 7279 2829 2c0a 2020 2020 2245 5850  tory(),.    "EXP
+000050c0: 4c41 494e 223a 205f 4578 6563 7574 6545  LAIN": _ExecuteE
+000050d0: 7870 6c61 696e 4661 6374 6f72 7928 292c  xplainFactory(),
+000050e0: 0a20 2020 2022 4558 504f 5254 223a 205f  .    "EXPORT": _
+000050f0: 4578 6563 7574 6545 7870 6f72 7446 6163  ExecuteExportFac
+00005100: 746f 7279 2829 2c0a 2020 2020 2243 4845  tory(),.    "CHE
+00005110: 434b 223a 205f 4368 6563 6b44 6174 6146  CK": _CheckDataF
+00005120: 6163 746f 7279 2829 2c0a 2020 2020 2246  actory(),.    "F
+00005130: 4f52 4345 223a 205f 466f 7263 6545 7874  ORCE": _ForceExt
+00005140: 6572 6e61 6c46 6163 746f 7279 2829 2c0a  ernalFactory(),.
+00005150: 2020 2020 2253 4554 2053 4348 454d 4122      "SET SCHEMA"
+00005160: 3a20 5f53 6574 5363 6865 6d61 4661 6374  : _SetSchemaFact
+00005170: 6f72 7928 292c 0a20 2020 2022 4745 5420  ory(),.    "GET 
+00005180: 5343 4845 4d41 223a 205f 4765 7453 6368  SCHEMA": _GetSch
+00005190: 656d 6146 6163 746f 7279 2829 2c0a 2020  emaFactory(),.  
+000051a0: 2020 2243 4c45 4152 2043 4143 4845 223a    "CLEAR CACHE":
+000051b0: 205f 436c 6561 7243 6163 6865 4661 6374   _ClearCacheFact
+000051c0: 6f72 7928 292c 0a20 2020 2022 5345 5422  ory(),.    "SET"
+000051d0: 3a20 5f53 6574 5061 7261 6d65 7465 7246  : _SetParameterF
+000051e0: 6163 746f 7279 2829 2c0a 2020 2020 2243  actory(),.    "C
+000051f0: 414e 4345 4c22 3a20 5f43 616e 6365 6c51  ANCEL": _CancelQ
+00005200: 7565 7279 4661 6374 6f72 7928 292c 0a20  ueryFactory(),. 
+00005210: 2020 2022 4b49 4c4c 223a 205f 4b69 6c6c     "KILL": _Kill
+00005220: 5175 6572 7946 6163 746f 7279 2829 2c0a  QueryFactory(),.
+00005230: 2020 2020 2247 4554 2053 5953 5445 4d20      "GET SYSTEM 
+00005240: 4d45 5441 4441 5441 223a 205f 4765 7453  METADATA": _GetS
+00005250: 7973 7465 6d4d 6574 6164 6174 6146 6163  ystemMetadataFac
+00005260: 746f 7279 2829 2c0a 2020 2020 2253 484f  tory(),.    "SHO
+00005270: 5722 3a20 5f45 7865 6375 7465 5175 6572  W": _ExecuteQuer
+00005280: 7946 6163 746f 7279 2829 2c0a 7d0a 2222  yFactory(),.}.""
+00005290: 224d 6170 7069 6e67 2066 726f 6d20 7175  "Mapping from qu
+000052a0: 6572 7920 7479 7065 2074 6f20 6974 7320  ery type to its 
+000052b0: 7265 7175 6573 7420 6661 6374 6f72 7922  request factory"
+000052c0: 2222 0a0a 0a64 6566 205f 636f 6e76 6572  ""...def _conver
+000052d0: 745f 6578 6365 7074 696f 6e28 6d73 673a  t_exception(msg:
+000052e0: 2070 726f 746f 2e43 6f6e 6669 726d 6174   proto.Confirmat
+000052f0: 696f 6e52 6573 706f 6e73 6529 202d 3e20  ionResponse) -> 
+00005300: 5351 4c45 7863 6570 7469 6f6e 3a0a 2020  SQLException:.  
+00005310: 2020 2222 2249 6e74 6572 6e61 6c20 726f    """Internal ro
+00005320: 7574 696e 6520 746f 2063 6f6e 7665 7274  utine to convert
+00005330: 2074 6865 2067 6f6f 676c 6520 7072 6f74   the google prot
+00005340: 6f62 7566 2043 6f6e 6669 726d 6174 696f  obuf Confirmatio
+00005350: 6e52 6573 706f 6e73 650a 2020 2020 746f  nResponse.    to
+00005360: 2061 6e20 6578 6365 7074 696f 6e0a 2020   an exception.  
+00005370: 2020 2222 220a 2020 2020 6966 206d 7367    """.    if msg
+00005380: 2e76 656e 646f 725f 636f 6465 203c 2030  .vendor_code < 0
+00005390: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+000053a0: 2045 7272 6f72 2873 716c 5f73 7461 7465   Error(sql_state
+000053b0: 3d6d 7367 2e73 716c 5f73 7461 7465 2c20  =msg.sql_state, 
+000053c0: 7265 6173 6f6e 3d6d 7367 2e72 6561 736f  reason=msg.reaso
+000053d0: 6e2c 2076 656e 646f 725f 636f 6465 3d6d  n, vendor_code=m
+000053e0: 7367 2e76 656e 646f 725f 636f 6465 290a  sg.vendor_code).
+000053f0: 0a20 2020 2072 6574 7572 6e20 5761 726e  .    return Warn
+00005400: 696e 6728 7371 6c5f 7374 6174 653d 6d73  ing(sql_state=ms
+00005410: 672e 7371 6c5f 7374 6174 652c 2072 6561  g.sql_state, rea
+00005420: 736f 6e3d 6d73 672e 7265 6173 6f6e 2c20  son=msg.reason, 
+00005430: 7665 6e64 6f72 5f63 6f64 653d 6d73 672e  vendor_code=msg.
+00005440: 7665 6e64 6f72 5f63 6f64 6529 0a0a 0a64  vendor_code)...d
+00005450: 6566 205f 7365 6e64 5f6d 7367 2863 6f6e  ef _send_msg(con
+00005460: 6e3a 2022 436f 6e6e 6563 7469 6f6e 222c  n: "Connection",
+00005470: 2070 726f 746f 6275 665f 6d73 673a 204d   protobuf_msg: M
+00005480: 6573 7361 6765 2920 2d3e 204e 6f6e 653a  essage) -> None:
+00005490: 0a20 2020 2022 2222 496e 7465 726e 616c  .    """Internal
+000054a0: 2072 6f75 7469 6e65 2074 6f20 7365 6e64   routine to send
+000054b0: 2061 2070 726f 746f 6275 6620 6d65 7373   a protobuf mess
+000054c0: 6167 6520 6f6e 2061 2063 6f6e 6e65 6374  age on a connect
+000054d0: 696f 6e22 2222 0a20 2020 2069 6620 6e6f  ion""".    if no
+000054e0: 7420 636f 6e6e 2e73 6f63 6b3a 0a20 2020  t conn.sock:.   
+000054f0: 2020 2020 2072 6169 7365 2050 726f 6772       raise Progr
+00005500: 616d 6d69 6e67 4572 726f 7228 2243 6f6e  ammingError("Con
+00005510: 6e65 6374 696f 6e20 6e6f 7420 6176 6169  nection not avai
+00005520: 6c61 626c 6522 290a 0a20 2020 206c 6f67  lable")..    log
+00005530: 6765 722e 6465 6275 6728 6622 5365 6e64  ger.debug(f"Send
+00005540: 696e 6720 6d65 7373 6167 6520 6f6e 2073  ing message on s
+00005550: 6f63 6b65 7420 7b63 6f6e 6e2e 736f 636b  ocket {conn.sock
+00005560: 7d3a 207b 7072 6f74 6f62 7566 5f6d 7367  }: {protobuf_msg
+00005570: 7d22 290a 0a20 2020 2074 7279 3a0a 2020  }")..    try:.  
+00005580: 2020 2020 2020 636f 6e6e 2e73 6f63 6b2e        conn.sock.
+00005590: 7365 6e64 616c 6c28 7374 7275 6374 2e70  sendall(struct.p
+000055a0: 6163 6b28 2221 6922 2c20 7072 6f74 6f62  ack("!i", protob
+000055b0: 7566 5f6d 7367 2e42 7974 6553 697a 6528  uf_msg.ByteSize(
+000055c0: 2929 202b 2070 726f 746f 6275 665f 6d73  )) + protobuf_ms
+000055d0: 672e 5365 7269 616c 697a 6554 6f53 7472  g.SerializeToStr
+000055e0: 696e 6728 2929 0a20 2020 2065 7863 6570  ing()).    excep
+000055f0: 7420 494f 4572 726f 723a 0a20 2020 2020  t IOError:.     
+00005600: 2020 2072 6169 7365 2049 4f45 7272 6f72     raise IOError
+00005610: 2822 4e65 7477 6f72 6b20 7365 6e64 2065  ("Network send e
+00005620: 7272 6f72 2229 0a0a 0a64 6566 205f 7265  rror")...def _re
+00005630: 6376 5f61 6c6c 2863 6f6e 6e3a 2022 436f  cv_all(conn: "Co
+00005640: 6e6e 6563 7469 6f6e 222c 2073 697a 653a  nnection", size:
+00005650: 2069 6e74 2920 2d3e 2062 7974 6573 3a0a   int) -> bytes:.
+00005660: 2020 2020 2222 2249 6e74 6572 6e61 6c20      """Internal 
+00005670: 726f 7574 696e 6520 746f 2072 6563 6569  routine to recei
+00005680: 7665 2060 7369 7a65 6020 6279 7465 7320  ve `size` bytes 
+00005690: 6f66 2064 6174 6120 6672 6f6d 2061 2063  of data from a c
+000056a0: 6f6e 6e65 6374 696f 6e22 2222 0a20 2020  onnection""".   
+000056b0: 2069 6620 6e6f 7420 636f 6e6e 2e73 6f63   if not conn.soc
+000056c0: 6b3a 0a20 2020 2020 2020 2072 6169 7365  k:.        raise
+000056d0: 2045 7272 6f72 2822 436f 6e6e 6563 7469   Error("Connecti
+000056e0: 6f6e 206e 6f74 2061 7661 696c 6162 6c65  on not available
+000056f0: 2229 0a0a 2020 2020 7768 696c 6520 6c65  ")..    while le
+00005700: 6e28 636f 6e6e 2e5f 6275 6666 6572 2920  n(conn._buffer) 
+00005710: 3c20 7369 7a65 3a0a 2020 2020 2020 2020  < size:.        
+00005720: 7265 6365 6976 6564 203d 2063 6f6e 6e2e  received = conn.
+00005730: 736f 636b 2e72 6563 7628 3136 3737 3732  sock.recv(167772
+00005740: 3136 2920 2023 2031 364d 4220 6275 6666  16)  # 16MB buff
+00005750: 6572 0a20 2020 2020 2020 2069 6620 6e6f  er.        if no
+00005760: 7420 7265 6365 6976 6564 3a0a 2020 2020  t received:.    
+00005770: 2020 2020 2020 2020 7261 6973 6520 494f          raise IO
+00005780: 4572 726f 7228 224e 6574 776f 726b 2072  Error("Network r
+00005790: 6563 6569 7665 2065 7272 6f72 2229 0a20  eceive error"). 
+000057a0: 2020 2020 2020 2063 6f6e 6e2e 5f62 7566         conn._buf
+000057b0: 6665 7220 2b3d 2072 6563 6569 7665 640a  fer += received.
+000057c0: 0a20 2020 2072 6574 203d 2063 6f6e 6e2e  .    ret = conn.
+000057d0: 5f62 7566 6665 725b 3a73 697a 655d 0a20  _buffer[:size]. 
+000057e0: 2020 2063 6f6e 6e2e 5f62 7566 6665 7220     conn._buffer 
+000057f0: 3d20 636f 6e6e 2e5f 6275 6666 6572 5b73  = conn._buffer[s
+00005800: 697a 653a 5d0a 0a20 2020 2072 6574 7572  ize:]..    retur
+00005810: 6e20 7265 740a 0a0a 6465 6620 5f72 6563  n ret...def _rec
+00005820: 765f 6d73 6728 636f 6e6e 3a20 2243 6f6e  v_msg(conn: "Con
+00005830: 6e65 6374 696f 6e22 2c20 7072 6f74 6f62  nection", protob
+00005840: 7566 5f6d 7367 3a20 5f4d 7367 5429 202d  uf_msg: _MsgT) -
+00005850: 3e20 5f4d 7367 543a 0a20 2020 2022 2222  > _MsgT:.    """
+00005860: 496e 7465 726e 616c 2072 6f75 7469 6e65  Internal routine
+00005870: 2074 6f20 7265 6365 6976 6520 6120 7072   to receive a pr
+00005880: 6f74 6f62 7566 206d 6573 7361 6765 206f  otobuf message o
+00005890: 6e20 6120 636f 6e6e 6563 7469 6f6e 2222  n a connection""
+000058a0: 220a 2020 2020 6864 7220 3d20 5f72 6563  ".    hdr = _rec
+000058b0: 765f 616c 6c28 636f 6e6e 2c20 3429 0a20  v_all(conn, 4). 
+000058c0: 2020 206d 7367 7369 7a65 203d 205f 756e     msgsize = _un
+000058d0: 7061 636b 5f69 6e74 2868 6472 295b 305d  pack_int(hdr)[0]
+000058e0: 0a0a 2020 2020 6d73 6720 3d20 5f72 6563  ..    msg = _rec
+000058f0: 765f 616c 6c28 636f 6e6e 2c20 6d73 6773  v_all(conn, msgs
+00005900: 697a 6529 0a0a 2020 2020 7072 6f74 6f62  ize)..    protob
+00005910: 7566 5f6d 7367 2e50 6172 7365 4672 6f6d  uf_msg.ParseFrom
+00005920: 5374 7269 6e67 286d 7367 290a 0a20 2020  String(msg)..   
+00005930: 206c 6f67 6765 722e 6465 6275 6728 6622   logger.debug(f"
+00005940: 5265 6365 6976 6564 206d 6573 7361 6765  Received message
+00005950: 206f 6e20 636f 6e6e 6563 7469 6f6e 207b   on connection {
+00005960: 636f 6e6e 2e73 6f63 6b7d 3a20 7b70 726f  conn.sock}: {pro
+00005970: 746f 6275 665f 6d73 677d 2229 0a0a 2020  tobuf_msg}")..  
+00005980: 2020 7265 7475 726e 2070 726f 746f 6275    return protobu
+00005990: 665f 6d73 670a 0a0a 6465 6620 4461 7465  f_msg...def Date
+000059a0: 2879 6561 723a 2069 6e74 2c20 6d6f 6e74  (year: int, mont
+000059b0: 683a 2069 6e74 2c20 6461 793a 2069 6e74  h: int, day: int
+000059c0: 2920 2d3e 2064 6174 6574 696d 652e 6461  ) -> datetime.da
+000059d0: 7465 7469 6d65 3a20 2023 2070 796c 696e  tetime:  # pylin
+000059e0: 743a 2064 6973 6162 6c65 3d69 6e76 616c  t: disable=inval
+000059f0: 6964 2d6e 616d 650a 2020 2020 2222 2254  id-name.    """T
+00005a00: 7970 6520 636f 6e73 7472 7563 746f 7220  ype constructor 
+00005a10: 7265 7175 6972 6564 2069 6e20 5045 5020  required in PEP 
+00005a20: 3234 3920 746f 2063 6f6e 7374 7275 6374  249 to construct
+00005a30: 2061 0a20 2020 2044 6174 6520 6f62 6a65   a.    Date obje
+00005a40: 6374 2066 726f 6d20 7965 6172 2c20 6d6f  ct from year, mo
+00005a50: 6e74 682c 2064 6179 0a20 2020 2022 2222  nth, day.    """
+00005a60: 0a20 2020 2072 6574 7572 6e20 6461 7465  .    return date
+00005a70: 7469 6d65 2e64 6174 6574 696d 6528 7965  time.datetime(ye
+00005a80: 6172 2c20 6d6f 6e74 682c 2064 6179 290a  ar, month, day).
+00005a90: 0a0a 6465 6620 5469 6d65 2868 6f75 723a  ..def Time(hour:
+00005aa0: 2069 6e74 2c20 6d69 6e75 7465 3a20 696e   int, minute: in
+00005ab0: 742c 2073 6563 6f6e 643a 2069 6e74 2920  t, second: int) 
+00005ac0: 2d3e 2064 6174 6574 696d 652e 7469 6d65  -> datetime.time
+00005ad0: 3a20 2023 2070 796c 696e 743a 2064 6973  :  # pylint: dis
+00005ae0: 6162 6c65 3d69 6e76 616c 6964 2d6e 616d  able=invalid-nam
+00005af0: 650a 2020 2020 2222 2254 7970 6520 636f  e.    """Type co
+00005b00: 6e73 7472 7563 746f 7220 7265 7175 6972  nstructor requir
+00005b10: 6564 2069 6e20 5045 5020 3234 3920 746f  ed in PEP 249 to
+00005b20: 2063 6f6e 7374 7275 6374 2061 0a20 2020   construct a.   
+00005b30: 2054 696d 6520 6f62 6a65 6374 2066 726f   Time object fro
+00005b40: 6d20 686f 7572 2c20 6d69 6e75 7465 2c20  m hour, minute, 
+00005b50: 7365 636f 6e64 0a20 2020 2022 2222 0a20  second.    """. 
+00005b60: 2020 2072 6574 7572 6e20 6461 7465 7469     return dateti
+00005b70: 6d65 2e74 696d 6528 686f 7572 2c20 6d69  me.time(hour, mi
+00005b80: 6e75 7465 2c20 7365 636f 6e64 290a 0a0a  nute, second)...
+00005b90: 6465 6620 5469 6d65 7374 616d 7028 0a20  def Timestamp(. 
+00005ba0: 2020 2079 6561 723a 2069 6e74 2c20 6d6f     year: int, mo
+00005bb0: 6e74 683a 2069 6e74 2c20 6461 793a 2069  nth: int, day: i
+00005bc0: 6e74 2c20 686f 7572 3a20 696e 742c 206d  nt, hour: int, m
+00005bd0: 696e 7574 653a 2069 6e74 2c20 7365 636f  inute: int, seco
+00005be0: 6e64 3a20 696e 740a 2920 2d3e 2066 6c6f  nd: int.) -> flo
+00005bf0: 6174 3a20 2023 2070 796c 696e 743a 2064  at:  # pylint: d
+00005c00: 6973 6162 6c65 3d69 6e76 616c 6964 2d6e  isable=invalid-n
+00005c10: 616d 652c 746f 6f2d 6d61 6e79 2d61 7267  ame,too-many-arg
+00005c20: 756d 656e 7473 0a20 2020 2022 2222 5479  uments.    """Ty
+00005c30: 7065 2063 6f6e 7374 7275 6374 6f72 2072  pe constructor r
+00005c40: 6571 7569 7265 6420 696e 2050 4550 2032  equired in PEP 2
+00005c50: 3439 2074 6f20 636f 6e73 7472 7563 740a  49 to construct.
+00005c60: 2020 2020 6120 5469 6d65 7374 616d 7020      a Timestamp 
+00005c70: 6f62 6a65 6374 2066 726f 6d20 7965 6172  object from year
+00005c80: 2c20 6d6f 6e74 682c 2064 6179 2c20 686f  , month, day, ho
+00005c90: 7572 2c20 6d69 6e75 7465 2c20 7365 636f  ur, minute, seco
+00005ca0: 6e64 0a20 2020 2022 2222 0a20 2020 2072  nd.    """.    r
+00005cb0: 6574 7572 6e20 6461 7465 7469 6d65 2e64  eturn datetime.d
+00005cc0: 6174 6574 696d 6528 7965 6172 2c20 6d6f  atetime(year, mo
+00005cd0: 6e74 682c 2064 6179 2c20 686f 7572 2c20  nth, day, hour, 
+00005ce0: 6d69 6e75 7465 2c20 7365 636f 6e64 292e  minute, second).
+00005cf0: 7469 6d65 7374 616d 7028 290a 0a0a 6465  timestamp()...de
+00005d00: 6620 4461 7465 4672 6f6d 5469 636b 7328  f DateFromTicks(
+00005d10: 7469 636b 733a 2066 6c6f 6174 2920 2d3e  ticks: float) ->
+00005d20: 2064 6174 6574 696d 652e 6461 7465 7469   datetime.dateti
+00005d30: 6d65 3a20 2023 2070 796c 696e 743a 2064  me:  # pylint: d
+00005d40: 6973 6162 6c65 3d69 6e76 616c 6964 2d6e  isable=invalid-n
+00005d50: 616d 650a 2020 2020 2222 2254 7970 6520  ame.    """Type 
+00005d60: 636f 6e73 7472 7563 746f 7220 7265 7175  constructor requ
+00005d70: 6972 6564 2069 6e20 5045 5020 3234 3920  ired in PEP 249 
+00005d80: 746f 2063 6f6e 7374 7275 6374 0a20 2020  to construct.   
+00005d90: 2061 2044 6174 6520 6f62 6a65 6374 2066   a Date object f
+00005da0: 726f 6d20 6120 7469 6d65 7374 616d 7020  rom a timestamp 
+00005db0: 6f66 2073 6563 6f6e 6473 2073 696e 6365  of seconds since
+00005dc0: 2065 706f 6368 0a20 2020 2022 2222 0a20   epoch.    """. 
+00005dd0: 2020 2072 6574 7572 6e20 6461 7465 7469     return dateti
+00005de0: 6d65 2e64 6174 6574 696d 652e 7574 6366  me.datetime.utcf
+00005df0: 726f 6d74 696d 6573 7461 6d70 2874 6963  romtimestamp(tic
+00005e00: 6b73 290a 0a0a 6465 6620 5469 6d65 4672  ks)...def TimeFr
+00005e10: 6f6d 5469 636b 7328 7469 636b 733a 2066  omTicks(ticks: f
+00005e20: 6c6f 6174 2920 2d3e 2064 6174 6574 696d  loat) -> datetim
+00005e30: 652e 7469 6d65 3a20 2023 2070 796c 696e  e.time:  # pylin
+00005e40: 743a 2064 6973 6162 6c65 3d69 6e76 616c  t: disable=inval
+00005e50: 6964 2d6e 616d 650a 2020 2020 2222 2254  id-name.    """T
+00005e60: 7970 6520 636f 6e73 7472 7563 746f 7220  ype constructor 
+00005e70: 7265 7175 6972 6564 2069 6e20 5045 5020  required in PEP 
+00005e80: 3234 3920 746f 2063 6f6e 7374 7275 6374  249 to construct
+00005e90: 0a20 2020 2061 2054 696d 6520 6f62 6a65  .    a Time obje
+00005ea0: 6374 2066 726f 6d20 6120 7469 6d65 7374  ct from a timest
+00005eb0: 616d 7020 6f66 2073 6563 6f6e 6473 2073  amp of seconds s
+00005ec0: 696e 6365 2065 706f 6368 0a20 2020 2022  ince epoch.    "
+00005ed0: 2222 0a20 2020 2064 6174 655f 7469 6d65  "".    date_time
+00005ee0: 203d 2064 6174 6574 696d 652e 6461 7465   = datetime.date
+00005ef0: 7469 6d65 2e75 7463 6672 6f6d 7469 6d65  time.utcfromtime
+00005f00: 7374 616d 7028 7469 636b 7329 0a20 2020  stamp(ticks).   
+00005f10: 2072 6574 7572 6e20 6461 7465 7469 6d65   return datetime
+00005f20: 2e74 696d 6528 6461 7465 5f74 696d 652e  .time(date_time.
+00005f30: 686f 7572 2c20 6461 7465 5f74 696d 652e  hour, date_time.
+00005f40: 6d69 6e75 7465 2c20 6461 7465 5f74 696d  minute, date_tim
+00005f50: 652e 7365 636f 6e64 290a 0a0a 6465 6620  e.second)...def 
+00005f60: 5469 6d65 7374 616d 7046 726f 6d54 6963  TimestampFromTic
+00005f70: 6b73 2874 6963 6b73 3a20 666c 6f61 7429  ks(ticks: float)
+00005f80: 202d 3e20 666c 6f61 743a 2020 2320 7079   -> float:  # py
+00005f90: 6c69 6e74 3a20 6469 7361 626c 653d 696e  lint: disable=in
+00005fa0: 7661 6c69 642d 6e61 6d65 0a20 2020 2022  valid-name.    "
+00005fb0: 2222 5479 7065 2063 6f6e 7374 7275 6374  ""Type construct
+00005fc0: 6f72 2072 6571 7569 7265 6420 696e 2050  or required in P
+00005fd0: 4550 2032 3439 2074 6f20 636f 6e73 7472  EP 249 to constr
+00005fe0: 7563 740a 2020 2020 6120 5469 6d65 7374  uct.    a Timest
+00005ff0: 616d 7020 6f62 6a65 6374 2066 726f 6d20  amp object from 
+00006000: 6120 7469 6d65 7374 616d 7020 6f66 2073  a timestamp of s
+00006010: 6563 6f6e 6473 2073 696e 6365 2065 706f  econds since epo
+00006020: 6368 0a20 2020 2022 2222 0a20 2020 2072  ch.    """.    r
+00006030: 6574 7572 6e20 7469 636b 730a 0a0a 6465  eturn ticks...de
+00006040: 6620 5f68 6173 685f 6b65 7928 7368 6172  f _hash_key(shar
+00006050: 6564 5f6b 6579 3a20 6279 7465 732c 2073  ed_key: bytes, s
+00006060: 616c 743a 2062 7974 6573 2920 2d3e 2062  alt: bytes) -> b
+00006070: 7974 6573 3a0a 2020 2020 2222 2249 6e74  ytes:.    """Int
+00006080: 6572 6e61 6c20 6b65 7920 6861 7368 2066  ernal key hash f
+00006090: 756e 6374 696f 6e22 2222 0a20 2020 2023  unction""".    #
+000060a0: 204e 6f20 6964 6561 2077 6865 7265 2074   No idea where t
+000060b0: 6869 7320 616c 676f 7269 7468 6d20 6361  his algorithm ca
+000060c0: 6d65 2066 726f 6d2c 2062 7574 2064 6f20  me from, but do 
+000060d0: 6120 686f 6d65 2067 726f 776e 206b 6579  a home grown key
+000060e0: 0a20 2020 2023 2064 6572 6976 6174 696f  .    # derivatio
+000060f0: 6e20 6675 6e63 7469 6f6e 0a20 2020 2062  n function.    b
+00006100: 7566 6665 7220 3d20 7374 7275 6374 2e70  uffer = struct.p
+00006110: 6163 6b28 2221 6922 2c20 6c65 6e28 7368  ack("!i", len(sh
+00006120: 6172 6564 5f6b 6579 2929 0a20 2020 2062  ared_key)).    b
+00006130: 7566 6665 7220 3d20 6275 6666 6572 202b  uffer = buffer +
+00006140: 2073 616c 740a 2020 2020 6275 6666 6572   salt.    buffer
+00006150: 203d 2062 7566 6665 7220 2b20 7368 6172   = buffer + shar
+00006160: 6564 5f6b 6579 0a20 2020 2068 6173 6865  ed_key.    hashe
+00006170: 7220 3d20 6861 7368 6573 2e48 6173 6828  r = hashes.Hash(
+00006180: 6861 7368 6573 2e53 4841 3235 3628 292c  hashes.SHA256(),
+00006190: 2062 6163 6b65 6e64 3d64 6566 6175 6c74   backend=default
+000061a0: 5f62 6163 6b65 6e64 2829 290a 2020 2020  _backend()).    
+000061b0: 6861 7368 6572 2e75 7064 6174 6528 6275  hasher.update(bu
+000061c0: 6666 6572 290a 2020 2020 7265 7475 726e  ffer).    return
+000061d0: 2068 6173 6865 722e 6669 6e61 6c69 7a65   hasher.finalize
+000061e0: 2829 0a0a 0a23 2053 6573 7369 6f6e 7320  ()...# Sessions 
+000061f0: 636f 6465 0a0a 2320 5573 6564 2066 6f72  code..# Used for
+00006200: 2072 6570 7265 7365 6e74 696e 6720 6120   representing a 
+00006210: 7365 7373 696f 6e20 6372 6561 7465 6420  session created 
+00006220: 7769 7468 2061 2073 6563 7572 6974 7920  with a security 
+00006230: 746f 6b65 6e20 7369 676e 2069 6e0a 0a0a  token sign in...
+00006240: 636c 6173 7320 5365 6375 7269 7479 546f  class SecurityTo
+00006250: 6b65 6e3a 0a20 2020 2064 6566 205f 5f69  ken:.    def __i
+00006260: 6e69 745f 5f28 7365 6c66 2c20 746f 6b65  nit__(self, toke
+00006270: 6e44 6174 613a 2073 7472 2c20 746f 6b65  nData: str, toke
+00006280: 6e53 6967 6e61 7475 7265 3a20 7374 722c  nSignature: str,
+00006290: 2069 7373 7565 7246 696e 6765 7270 7269   issuerFingerpri
+000062a0: 6e74 3a20 7374 7229 202d 3e20 4e6f 6e65  nt: str) -> None
+000062b0: 3a0a 2020 2020 2020 2020 7365 6c66 2e74  :.        self.t
+000062c0: 6f6b 656e 4461 7461 203d 2074 6f6b 656e  okenData = token
+000062d0: 4461 7461 0a20 2020 2020 2020 2073 656c  Data.        sel
+000062e0: 662e 746f 6b65 6e53 6967 6e61 7475 7265  f.tokenSignature
+000062f0: 203d 2074 6f6b 656e 5369 676e 6174 7572   = tokenSignatur
+00006300: 650a 2020 2020 2020 2020 7365 6c66 2e69  e.        self.i
+00006310: 7373 7565 7246 696e 6765 7270 7269 6e74  ssuerFingerprint
+00006320: 203d 2069 7373 7565 7246 696e 6765 7270   = issuerFingerp
+00006330: 7269 6e74 0a0a 0a23 2055 7365 6420 666f  rint...# Used fo
+00006340: 7220 7265 7072 6573 656e 7469 6e67 2061  r representing a
+00006350: 2073 6573 7369 6f6e 2063 7265 6174 6564   session created
+00006360: 2077 6974 6820 6120 7573 6572 2061 6e64   with a user and
+00006370: 2070 6173 7377 6f72 6420 7369 676e 2069   password sign i
+00006380: 6e2e 0a0a 0a63 6c61 7373 2055 7365 7241  n....class UserA
+00006390: 6e64 5061 7373 776f 7264 3a0a 2020 2020  ndPassword:.    
+000063a0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+000063b0: 662c 2075 7365 723a 2073 7472 2c20 7061  f, user: str, pa
+000063c0: 7373 776f 7264 3a20 7374 7229 202d 3e20  ssword: str) -> 
+000063d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7365  None:.        se
+000063e0: 6c66 2e75 7365 7220 3d20 7573 6572 0a20  lf.user = user. 
+000063f0: 2020 2020 2020 2073 656c 662e 7061 7373         self.pass
+00006400: 776f 7264 203d 2070 6173 7377 6f72 640a  word = password.
+00006410: 0a0a 636c 6173 7320 5365 7373 696f 6e3a  ..class Session:
+00006420: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00006430: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+00006440: 2073 6563 7572 6974 7954 6f6b 656e 3a20   securityToken: 
+00006450: 4f70 7469 6f6e 616c 5b53 6563 7572 6974  Optional[Securit
+00006460: 7954 6f6b 656e 5d20 3d20 4e6f 6e65 2c20  yToken] = None, 
+00006470: 7573 6572 416e 6450 6173 7377 6f72 643a  userAndPassword:
+00006480: 204f 7074 696f 6e61 6c5b 5573 6572 416e   Optional[UserAn
+00006490: 6450 6173 7377 6f72 645d 203d 204e 6f6e  dPassword] = Non
+000064a0: 650a 2020 2020 2920 2d3e 204e 6f6e 653a  e.    ) -> None:
+000064b0: 0a20 2020 2020 2020 2023 204f 6e6c 7920  .        # Only 
+000064c0: 6f6e 6520 6f66 2074 6865 7365 2073 686f  one of these sho
+000064d0: 756c 6420 6265 2069 6e73 7461 6e74 6961  uld be instantia
+000064e0: 7465 642e 2054 6865 206f 7468 6572 204d  ted. The other M
+000064f0: 5553 5420 6265 206e 6f6e 652e 0a20 2020  UST be none..   
+00006500: 2020 2020 2069 6620 2873 6563 7572 6974       if (securit
+00006510: 7954 6f6b 656e 2069 7320 4e6f 6e65 2061  yToken is None a
+00006520: 6e64 2075 7365 7241 6e64 5061 7373 776f  nd userAndPasswo
+00006530: 7264 2069 7320 4e6f 6e65 2920 6f72 2028  rd is None) or (
+00006540: 0a20 2020 2020 2020 2020 2020 2073 6563  .            sec
+00006550: 7572 6974 7954 6f6b 656e 2069 7320 6e6f  urityToken is no
+00006560: 7420 4e6f 6e65 2061 6e64 2075 7365 7241  t None and userA
+00006570: 6e64 5061 7373 776f 7264 2069 7320 6e6f  ndPassword is no
+00006580: 7420 4e6f 6e65 0a20 2020 2020 2020 2029  t None.        )
+00006590: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+000065a0: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+000065b0: 4578 6163 746c 7920 6f6e 6520 6f66 2073  Exactly one of s
+000065c0: 6563 7572 6974 7954 6f6b 656e 2061 6e64  ecurityToken and
+000065d0: 2075 7365 7241 6e64 5061 7373 776f 7264   userAndPassword
+000065e0: 206d 7573 7420 6265 2073 7065 6369 6669   must be specifi
+000065f0: 6564 2229 0a20 2020 2020 2020 2073 656c  ed").        sel
+00006600: 662e 7365 6375 7269 7479 546f 6b65 6e20  f.securityToken 
+00006610: 3d20 7365 6375 7269 7479 546f 6b65 6e0a  = securityToken.
+00006620: 2020 2020 2020 2020 7365 6c66 2e75 7365          self.use
+00006630: 7241 6e64 5061 7373 776f 7264 203d 2075  rAndPassword = u
+00006640: 7365 7241 6e64 5061 7373 776f 7264 0a0a  serAndPassword..
+00006650: 0a63 6c61 7373 2043 6f6e 6e65 6374 696f  .class Connectio
+00006660: 6e3a 0a20 2020 2022 2222 4120 636f 6e6e  n:.    """A conn
+00006670: 6563 7469 6f6e 2074 6f20 7468 6520 4f63  ection to the Oc
+00006680: 6965 6e74 2064 6174 6162 6173 652e 204e  ient database. N
+00006690: 6f72 6d61 6c6c 7920 636f 6e73 7472 7563  ormally construc
+000066a0: 7465 6420 6279 0a20 2020 2063 616c 6c69  ted by.    calli
+000066b0: 6e67 2074 6865 206d 6f64 756c 6520 6063  ng the module `c
+000066c0: 6f6e 6e65 6374 2829 6020 6361 6c6c 2c20  onnect()` call, 
+000066d0: 6275 7420 6361 6e20 6265 2063 6f6e 7374  but can be const
+000066e0: 7275 6374 6564 0a20 2020 2064 6972 6563  ructed.    direc
+000066f0: 746c 790a 2020 2020 2222 220a 0a20 2020  tly.    """..   
+00006700: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
+00006710: 6c65 3d74 6f6f 2d6d 616e 792d 696e 7374  le=too-many-inst
+00006720: 616e 6365 2d61 7474 7269 6275 7465 730a  ance-attributes.
+00006730: 2020 2020 544c 535f 4e4f 4e45 203d 2031      TLS_NONE = 1
+00006740: 2020 2320 3a20 3a6d 6574 6120 7072 6976    # : :meta priv
+00006750: 6174 653a 0a20 2020 2054 4c53 5f55 4e56  ate:.    TLS_UNV
+00006760: 4552 4946 4945 4420 3d20 3220 2023 203a  ERIFIED = 2  # :
+00006770: 203a 6d65 7461 2070 7269 7661 7465 3a0a   :meta private:.
+00006780: 2020 2020 544c 535f 4f4e 203d 2033 2020      TLS_ON = 3  
+00006790: 2320 3a20 3a6d 6574 6120 7072 6976 6174  # : :meta privat
+000067a0: 653a 0a0a 2020 2020 4841 4e44 5348 414b  e:..    HANDSHAK
+000067b0: 455f 4342 4320 3d20 310a 2020 2020 4841  E_CBC = 1.    HA
+000067c0: 4e44 5348 414b 455f 4743 4d20 3d20 320a  NDSHAKE_GCM = 2.
+000067d0: 2020 2020 4841 4e44 5348 414b 455f 5353      HANDSHAKE_SS
+000067e0: 4f20 3d20 330a 0a20 2020 2044 4546 4155  O = 3..    DEFAU
+000067f0: 4c54 5f48 4f53 5420 3d20 226c 6f63 616c  LT_HOST = "local
+00006800: 686f 7374 220a 2020 2020 4445 4641 554c  host".    DEFAUL
+00006810: 545f 504f 5254 203d 2034 3035 300a 2020  T_PORT = 4050.  
+00006820: 2020 4445 4641 554c 545f 4441 5441 4241    DEFAULT_DATABA
+00006830: 5345 203d 2022 7379 7374 656d 220a 0a20  SE = "system".. 
+00006840: 2020 2068 6f73 7473 3a20 4c69 7374 5b73     hosts: List[s
+00006850: 7472 5d20 3d20 5b5d 0a20 2020 2070 6f72  tr] = [].    por
+00006860: 7420 3d20 4e6f 6e65 0a20 2020 2064 6174  t = None.    dat
+00006870: 6162 6173 6520 3d20 4e6f 6e65 0a20 2020  abase = None.   
+00006880: 2074 6c73 203d 204e 6f6e 650a 2020 2020   tls = None.    
+00006890: 666f 7263 6520 3d20 4e6f 6e65 0a20 2020  force = None.   
+000068a0: 2068 616e 6473 6861 6b65 203d 204e 6f6e   handshake = Non
+000068b0: 650a 2020 2020 7573 6572 203d 204e 6f6e  e.    user = Non
+000068c0: 650a 2020 2020 7061 7373 776f 7264 203d  e.    password =
+000068d0: 204e 6f6e 650a 2020 2020 7365 636f 6e64   None.    second
+000068e0: 6172 795f 696e 7465 7266 6163 6573 3a20  ary_interfaces: 
+000068f0: 4f70 7469 6f6e 616c 5b4c 6973 745b 4c69  Optional[List[Li
+00006900: 7374 5b54 7570 6c65 5b73 7472 2c20 696e  st[Tuple[str, in
+00006910: 745d 5d5d 5d20 3d20 4e6f 6e65 0a20 2020  t]]]] = None.   
+00006920: 2073 6563 6f6e 6461 7279 5f69 6e64 6578   secondary_index
+00006930: 203d 202d 310a 2020 2020 736f 636b 3a20   = -1.    sock: 
+00006940: 4f70 7469 6f6e 616c 5b55 6e69 6f6e 5b73  Optional[Union[s
+00006950: 6f63 6b65 742e 736f 636b 6574 2c20 7373  ocket.socket, ss
+00006960: 6c2e 5353 4c53 6f63 6b65 745d 5d20 3d20  l.SSLSocket]] = 
+00006970: 4e6f 6e65 0a20 2020 2073 6573 7369 6f6e  None.    session
+00006980: 5f69 6420 3d20 7374 7228 7575 6964 2e75  _id = str(uuid.u
+00006990: 7569 6431 2829 290a 0a20 2020 2073 6573  uid1())..    ses
+000069a0: 7369 6f6e 203d 204e 6f6e 650a 2020 2020  sion = None.    
+000069b0: 7365 7276 6572 5365 7373 696f 6e49 6420  serverSessionId 
+000069c0: 3d20 4e6f 6e65 0a0a 2020 2020 2320 5768  = None..    # Wh
+000069d0: 6574 6865 7220 7468 6520 6e65 7874 2065  ether the next e
+000069e0: 7865 6375 7465 2071 7565 7279 2072 756e  xecute query run
+000069f0: 206f 6e20 7468 6973 2063 6f6e 6e65 6374   on this connect
+00006a00: 696f 6e20 7769 6c6c 2062 6520 7265 6469  ion will be redi
+00006a10: 7265 6374 6564 2e20 446f 6573 206e 6f74  rected. Does not
+00006a20: 6869 6e67 2069 6620 666f 7263 6520 6973  hing if force is
+00006a30: 2073 6574 2074 6f20 7472 7565 0a20 2020   set to true.   
+00006a40: 2066 6f72 6365 5f6e 6578 745f 7265 6469   force_next_redi
+00006a50: 7265 6374 203d 2046 616c 7365 0a0a 2020  rect = False..  
+00006a60: 2020 2320 5365 7373 696f 6e73 2063 6f64    # Sessions cod
+00006a70: 6520 656e 640a 0a20 2020 2023 2074 6865  e end..    # the
+00006a80: 2050 4550 2032 3439 2073 7461 6e64 6172   PEP 249 standar
+00006a90: 6420 7265 636f 6d6d 656e 6473 206d 616b  d recommends mak
+00006aa0: 696e 6720 7468 6520 6d6f 6475 6c65 206c  ing the module l
+00006ab0: 6576 656c 2065 7863 6570 7469 6f6e 730a  evel exceptions.
+00006ac0: 2020 2020 2320 616c 736f 2061 7474 7269      # also attri
+00006ad0: 6275 7465 7320 6f6e 2074 6865 2043 6f6e  butes on the Con
+00006ae0: 6e65 6374 696f 6e20 636c 6173 730a 2020  nection class.  
+00006af0: 2020 4572 726f 7220 3d20 4572 726f 720a    Error = Error.
+00006b00: 2020 2020 5761 726e 696e 6720 3d20 5761      Warning = Wa
+00006b10: 726e 696e 670a 2020 2020 496e 7465 7266  rning.    Interf
+00006b20: 6163 6545 7272 6f72 203d 2049 6e74 6572  aceError = Inter
+00006b30: 6661 6365 4572 726f 720a 2020 2020 4461  faceError.    Da
+00006b40: 7461 6261 7365 4572 726f 7220 3d20 4461  tabaseError = Da
+00006b50: 7461 6261 7365 4572 726f 720a 2020 2020  tabaseError.    
+00006b60: 496e 7465 726e 616c 4572 726f 7220 3d20  InternalError = 
+00006b70: 496e 7465 726e 616c 4572 726f 720a 2020  InternalError.  
+00006b80: 2020 4f70 6572 6174 696f 6e61 6c45 7272    OperationalErr
+00006b90: 6f72 203d 204f 7065 7261 7469 6f6e 616c  or = Operational
+00006ba0: 4572 726f 720a 2020 2020 5072 6f67 7261  Error.    Progra
+00006bb0: 6d6d 696e 6745 7272 6f72 203d 2050 726f  mmingError = Pro
+00006bc0: 6772 616d 6d69 6e67 4572 726f 720a 2020  grammingError.  
+00006bd0: 2020 496e 7465 6772 6974 7945 7272 6f72    IntegrityError
+00006be0: 203d 2049 6e74 6567 7269 7479 4572 726f   = IntegrityErro
+00006bf0: 720a 2020 2020 4461 7461 4572 726f 7220  r.    DataError 
+00006c00: 3d20 4461 7461 4572 726f 720a 2020 2020  = DataError.    
+00006c10: 4e6f 7453 7570 706f 7274 6564 4572 726f  NotSupportedErro
+00006c20: 7220 3d20 4e6f 7453 7570 706f 7274 6564  r = NotSupported
+00006c30: 4572 726f 720a 0a20 2020 2064 6566 205f  Error..    def _
+00006c40: 7373 6c69 7a65 5f63 6f6e 6e65 6374 696f  sslize_connectio
+00006c50: 6e28 7365 6c66 2920 2d3e 204e 6f6e 653a  n(self) -> None:
+00006c60: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00006c70: 2020 2020 2049 6620 5353 4c20 6973 2073       If SSL is s
+00006c80: 7065 6369 6669 6564 2c20 7772 6170 2074  pecified, wrap t
+00006c90: 6865 2043 6f6e 6e65 6374 696f 6e27 7320  he Connection's 
+00006ca0: 736f 636b 6574 2069 6e20 616e 2053 534c  socket in an SSL
+00006cb0: 2063 6f6e 6e65 6374 696f 6e0a 2020 2020   connection.    
+00006cc0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00006cd0: 6966 2073 656c 662e 746c 7320 213d 2073  if self.tls != s
+00006ce0: 656c 662e 544c 535f 4e4f 4e45 3a0a 2020  elf.TLS_NONE:.  
+00006cf0: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+00006d00: 2073 656c 662e 736f 636b 2069 7320 6e6f   self.sock is no
+00006d10: 7420 4e6f 6e65 0a20 2020 2020 2020 2020  t None.         
+00006d20: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+00006d30: 2243 7265 6174 696e 6720 544c 5320 636f  "Creating TLS co
+00006d40: 6e6e 6563 7469 6f6e 2229 0a20 2020 2020  nnection").     
+00006d50: 2020 2020 2020 2063 6f6e 7465 7874 203d         context =
+00006d60: 2073 736c 2e63 7265 6174 655f 6465 6661   ssl.create_defa
+00006d70: 756c 745f 636f 6e74 6578 7428 290a 2020  ult_context().  
+00006d80: 2020 2020 2020 2020 2020 636f 6e74 6578            contex
+00006d90: 742e 6368 6563 6b5f 686f 7374 6e61 6d65  t.check_hostname
+00006da0: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
+00006db0: 2020 2020 2069 6620 7365 6c66 2e74 6c73       if self.tls
+00006dc0: 2021 3d20 7365 6c66 2e54 4c53 5f4f 4e3a   != self.TLS_ON:
+00006dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006de0: 2063 6f6e 7465 7874 2e76 6572 6966 795f   context.verify_
+00006df0: 6d6f 6465 203d 2073 736c 2e43 4552 545f  mode = ssl.CERT_
+00006e00: 4e4f 4e45 0a20 2020 2020 2020 2020 2020  NONE.           
+00006e10: 2073 656c 662e 736f 636b 203d 2063 6f6e   self.sock = con
+00006e20: 7465 7874 2e77 7261 705f 736f 636b 6574  text.wrap_socket
+00006e30: 2873 656c 662e 736f 636b 290a 0a20 2020  (self.sock)..   
+00006e40: 2023 204e 6f74 6520 7468 6174 2074 6865   # Note that the
+00006e50: 7265 2061 7265 2061 2063 6f75 706c 6520  re are a couple 
+00006e60: 6f66 2070 6c61 6365 7320 696e 2074 6865  of places in the
+00006e70: 2063 6f64 6520 7768 6572 6520 7765 2072   code where we r
+00006e80: 6563 6f6e 7374 7275 6374 2074 6865 2043  econstruct the C
+00006e90: 6f6e 6e65 6374 696f 6e2e 2020 4966 2079  onnection.  If y
+00006ea0: 6f75 2061 6464 2061 2070 6172 616d 6574  ou add a paramet
+00006eb0: 6572 2068 6572 652c 206d 616b 6520 7375  er here, make su
+00006ec0: 7265 2074 6f20 7570 6461 7465 2074 686f  re to update tho
+00006ed0: 7365 0a20 2020 2023 2070 6c61 6365 730a  se.    # places.
+00006ee0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00006ef0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00006f00: 2020 2020 2020 2020 6473 6e3a 204f 7074          dsn: Opt
+00006f10: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00006f20: 652c 0a20 2020 2020 2020 2075 7365 723a  e,.        user:
+00006f30: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00006f40: 204e 6f6e 652c 0a20 2020 2020 2020 2070   None,.        p
+00006f50: 6173 7377 6f72 643a 204f 7074 696f 6e61  assword: Optiona
+00006f60: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
+00006f70: 2020 2020 2020 2068 6f73 743a 204f 7074         host: Opt
+00006f80: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00006f90: 652c 0a20 2020 2020 2020 2064 6174 6162  e,.        datab
+00006fa0: 6173 653a 204f 7074 696f 6e61 6c5b 7374  ase: Optional[st
+00006fb0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+00006fc0: 2020 2074 6c73 3a20 4f70 7469 6f6e 616c     tls: Optional
+00006fd0: 5b55 6e69 6f6e 5b73 7472 2c20 696e 745d  [Union[str, int]
+00006fe0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00006ff0: 2020 6861 6e64 7368 616b 653a 204f 7074    handshake: Opt
+00007000: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+00007010: 652c 0a20 2020 2020 2020 2066 6f72 6365  e,.        force
+00007020: 3a20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  : Optional[bool]
+00007030: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00007040: 2063 6f6e 6669 6766 696c 653a 204f 7074   configfile: Opt
+00007050: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00007060: 652c 0a20 2020 2020 2020 2073 6573 7369  e,.        sessi
+00007070: 6f6e 3a20 4f70 7469 6f6e 616c 5b53 6573  on: Optional[Ses
+00007080: 7369 6f6e 5d20 3d20 4e6f 6e65 2c0a 2020  sion] = None,.  
+00007090: 2020 2920 2d3e 204e 6f6e 653a 0a20 2020    ) -> None:.   
+000070a0: 2020 2020 2023 2070 796c 696e 743a 2064       # pylint: d
+000070b0: 6973 6162 6c65 3d74 6f6f 2d6d 616e 792d  isable=too-many-
+000070c0: 6172 6775 6d65 6e74 732c 6e6f 2d6d 656d  arguments,no-mem
+000070d0: 6265 720a 2020 2020 2020 2020 2222 2243  ber.        """C
+000070e0: 6f6e 6e65 6374 696f 6e20 7061 7261 6d65  onnection parame
+000070f0: 7465 7273 2063 616e 2062 6520 7370 6563  ters can be spec
+00007100: 6966 6965 6420 6173 2070 6172 7420 6f66  ified as part of
+00007110: 2074 6865 2064 736e 2c0a 2020 2020 2020   the dsn,.      
+00007120: 2020 7573 696e 6720 6b65 7977 6f72 6420    using keyword 
+00007130: 6172 6775 6d65 6e74 7320 6f72 2062 6f74  arguments or bot
+00007140: 682e 2020 4966 2062 6f74 6820 6172 6520  h.  If both are 
+00007150: 7370 6563 6966 6965 642c 2074 6865 206b  specified, the k
+00007160: 6579 776f 7264 0a20 2020 2020 2020 2070  eyword.        p
+00007170: 6172 616d 6574 6572 206f 7665 7272 6964  arameter overrid
+00007180: 6573 2074 6865 2076 616c 7565 2069 6e20  es the value in 
+00007190: 7468 6520 6473 6e2e 0a0a 2020 2020 2020  the dsn...      
+000071a0: 2020 5468 6520 4f63 6965 6e74 2044 534e    The Ocient DSN
+000071b0: 2069 7320 6f66 2074 6865 2066 6f72 6d61   is of the forma
+000071c0: 743a 0a20 2020 2020 2020 2060 6f63 6965  t:.        `ocie
+000071d0: 6e74 3a2f 2f75 7365 723a 7061 7373 776f  nt://user:passwo
+000071e0: 7264 405b 686f 7374 5d5b 3a70 6f72 745d  rd@[host][:port]
+000071f0: 5b2f 6461 7461 6261 7365 5d5b 3f70 6172  [/database][?par
+00007200: 616d 313d 7661 6c75 6531 262e 2e2e 5d60  am1=value1&...]`
+00007210: 0a0a 2020 2020 2020 2020 6075 7365 7260  ..        `user`
+00007220: 2061 6e64 2060 7061 7373 776f 7264 6020   and `password` 
+00007230: 6d75 7374 2062 6520 7375 7070 6c69 6564  must be supplied
+00007240: 2e20 2060 686f 7374 6020 6465 6661 756c  .  `host` defaul
+00007250: 7473 2074 6f20 6c6f 6361 6c68 6f73 742c  ts to localhost,
+00007260: 0a20 2020 2020 2020 2070 6f72 7420 6465  .        port de
+00007270: 6661 756c 7473 2074 6f20 3430 3530 2c20  faults to 4050, 
+00007280: 6461 7461 6261 7365 2064 6566 6175 6c74  database default
+00007290: 7320 746f 2060 7379 7374 656d 6020 616e  s to `system` an
+000072a0: 6420 6074 6c73 6020 6465 6661 756c 7473  d `tls` defaults
+000072b0: 0a20 2020 2020 2020 2074 6f20 606f 6666  .        to `off
+000072c0: 602e 0a0a 2020 2020 2020 2020 4d75 6c74  `...        Mult
+000072d0: 6970 6c65 2068 6f73 7473 206d 6179 2062  iple hosts may b
+000072e0: 6520 7370 6563 6966 6965 642c 2073 6570  e specified, sep
+000072f0: 6172 6174 6564 2062 7920 6120 636f 6d6d  arated by a comm
+00007300: 612c 2069 6e20 7768 6963 6820 6361 7365  a, in which case
+00007310: 2074 6865 0a20 2020 2020 2020 2068 6f73   the.        hos
+00007320: 7473 2077 696c 6c20 6265 2074 7269 6564  ts will be tried
+00007330: 2069 6e20 6f72 6465 7220 2054 6875 7320   in order  Thus 
+00007340: 616e 2065 7861 6d70 6c65 2044 534e 206d  an example DSN m
+00007350: 6967 6874 2062 650a 2020 2020 2020 2020  ight be.        
+00007360: 606f 6369 656e 743a 2f2f 736f 6d65 6f6e  `ocient://someon
+00007370: 653a 736f 6d65 7061 7373 776f 7264 4068  e:somepassword@h
+00007380: 6f73 7431 2c68 6f73 7432 3a34 3035 312f  ost1,host2:4051/
+00007390: 6d79 6462 600a 0a20 2020 2020 2020 2063  mydb`..        c
+000073a0: 6f6e 6669 6766 696c 6520 6973 2074 6865  onfigfile is the
+000073b0: 206e 616d 6520 6f66 2061 2063 6f6e 6669   name of a confi
+000073c0: 6775 7261 7469 6f6e 2066 696c 6520 696e  guration file in
+000073d0: 2049 4e49 2066 6f72 6d61 742c 2077 6865   INI format, whe
+000073e0: 7265 2065 6163 680a 2020 2020 2020 2020  re each.        
+000073f0: 7365 6374 696f 6e20 6973 2065 6974 6865  section is eithe
+00007400: 7220 6465 6661 756c 742c 206f 7220 6120  r default, or a 
+00007410: 7061 7474 6572 6e20 7468 6174 206d 6174  pattern that mat
+00007420: 6368 6573 2074 6865 2068 6f73 7420 616e  ches the host an
+00007430: 6420 6f70 7469 6f6e 616c 6c79 0a20 2020  d optionally.   
+00007440: 2020 2020 2064 6174 6162 6173 652e 2073       database. s
+00007450: 6563 7469 6f6e 7320 6172 6520 6d61 7463  ections are matc
+00007460: 6865 6420 696e 206f 7264 6572 2c20 736f  hed in order, so
+00007470: 206d 6f72 6520 7370 6563 6966 6963 2073   more specific s
+00007480: 6563 7469 6f6e 7320 7368 6f75 6c64 0a20  ections should. 
+00007490: 2020 2020 2020 2070 7265 6365 6465 206c         precede l
+000074a0: 6573 7320 7370 6563 6966 6963 2073 6563  ess specific sec
+000074b0: 7469 6f6e 733a 3a0a 0a20 2020 2020 2020  tions::..       
+000074c0: 2020 2020 205b 4445 4641 554c 545d 0a20       [DEFAULT]. 
+000074d0: 2020 2020 2020 2020 2020 2074 6c73 203d             tls =
+000074e0: 2075 6e76 6572 6966 6965 640a 0a20 2020   unverified..   
+000074f0: 2020 2020 2020 2020 2023 2054 6869 7320           # This 
+00007500: 7769 6c6c 206d 6174 6368 2074 6865 2073  will match the s
+00007510: 7065 6369 6669 6320 686f 7374 2061 6e64  pecific host and
+00007520: 2064 6174 6162 6173 650a 2020 2020 2020   database.      
+00007530: 2020 2020 2020 5b66 6f6f 2e6f 6369 656e        [foo.ocien
+00007540: 742e 636f 6d2f 736f 6d65 6462 5d0a 2020  t.com/somedb].  
+00007550: 2020 2020 2020 2020 2020 7573 6572 203d            user =
+00007560: 2070 616e 7468 6572 0a20 2020 2020 2020   panther.       
+00007570: 2020 2020 2070 6173 7377 6f72 6420 3d20       password = 
+00007580: 7069 6e6b 0a0a 2020 2020 2020 2020 2020  pink..          
+00007590: 2020 2320 5468 6973 2077 696c 6c20 6d61    # This will ma
+000075a0: 7463 6820 7468 6520 7370 6563 6966 6963  tch the specific
+000075b0: 2068 6f73 740a 2020 2020 2020 2020 2020   host.          
+000075c0: 2020 5b66 6f6f 2e6f 6369 656e 742e 636f    [foo.ocient.co
+000075d0: 6d5d 0a20 2020 2020 2020 2020 2020 2075  m].            u
+000075e0: 7365 7220 3d20 7061 6e74 6865 720a 2020  ser = panther.  
+000075f0: 2020 2020 2020 2020 2020 7061 7373 776f            passwo
+00007600: 7264 203d 2070 696e 6b0a 0a20 2020 2020  rd = pink..     
+00007610: 2020 2020 2020 2023 2054 6869 7320 7769         # This wi
+00007620: 6c6c 206d 6174 6368 2061 6e79 2068 6f73  ll match any hos
+00007630: 7420 696e 2074 6865 206f 6369 656e 742e  t in the ocient.
+00007640: 636f 6d20 646f 6d61 696e 0a20 2020 2020  com domain.     
+00007650: 2020 2020 2020 205b 2a2e 6f63 6965 6e74         [*.ocient
+00007660: 2e63 6f6d 5d0a 2020 2020 2020 2020 2020  .com].          
+00007670: 2020 7573 6572 203d 2074 6f6d 0a20 2020    user = tom.   
+00007680: 2020 2020 2020 2020 2070 6173 7377 6f72           passwor
+00007690: 6420 3d20 6a65 7272 790a 2020 2020 2020  d = jerry.      
+000076a0: 2020 2020 2020 6461 7461 6261 7365 203d        database =
+000076b0: 206d 6963 650a 0a20 2020 2020 2020 2020   mice..         
+000076c0: 2020 2023 2054 6869 7320 7769 6c6c 206d     # This will m
+000076d0: 6174 6368 2061 6e79 2068 6f73 7420 696e  atch any host in
+000076e0: 2074 6865 206f 6369 656e 742e 636f 6d20   the ocient.com 
+000076f0: 646f 6d61 696e 0a20 2020 2020 2020 2020  domain.         
+00007700: 2020 205b 2a2e 6f63 6965 6e74 2e63 6f6d     [*.ocient.com
+00007710: 5d0a 2020 2020 2020 2020 2020 2020 7573  ].            us
+00007720: 6572 203d 2074 6f6d 0a20 2020 2020 2020  er = tom.       
+00007730: 2020 2020 2070 6173 7377 6f72 6420 3d20       password = 
+00007740: 6a65 7272 790a 0a20 2020 2020 2020 2043  jerry..        C
+00007750: 7572 7265 6e74 6c79 2073 7570 706f 7274  urrently support
+00007760: 6564 2070 6172 616d 6574 6572 7320 6172  ed parameters ar
+00007770: 653a 0a0a 2020 2020 2020 2020 2d20 746c  e:..        - tl
+00007780: 733a 2057 6869 6368 2063 616e 2068 6176  s: Which can hav
+00007790: 6520 7468 6520 7661 6c75 6573 2022 6f66  e the values "of
+000077a0: 6622 2c20 2275 6e76 6572 6966 6965 6422  f", "unverified"
+000077b0: 2c20 6f72 2022 6f6e 2220 696e 2074 6865  , or "on" in the
+000077c0: 2064 736e 2c0a 2020 2020 2020 2020 2020   dsn,.          
+000077d0: 2020 6f72 2043 6f6e 6e65 6374 696f 6e2e    or Connection.
+000077e0: 544c 535f 4e4f 4e45 2c20 436f 6e6e 6563  TLS_NONE, Connec
+000077f0: 7469 6f6e 2e54 4c53 5f55 4e56 4552 4946  tion.TLS_UNVERIF
+00007800: 4945 442c 206f 720a 2020 2020 2020 2020  IED, or.        
+00007810: 2020 2020 436f 6e6e 6563 7469 6f6e 2e54      Connection.T
+00007820: 4c53 5f4f 4e20 6173 2061 206b 6579 776f  LS_ON as a keywo
+00007830: 7264 2070 6172 616d 6574 6572 2e0a 2020  rd parameter..  
+00007840: 2020 2020 2020 2d20 666f 7263 653a 2054        - force: T
+00007850: 7275 6520 6f72 2046 616c 7365 2c20 7768  rue or False, wh
+00007860: 6574 6865 7220 746f 2066 6f72 6365 2074  ether to force t
+00007870: 6865 2063 6f6e 6e65 6374 696f 6e20 746f  he connection to
+00007880: 2072 656d 6169 6e20 6f6e 2074 6869 730a   remain on this.
+00007890: 2020 2020 2020 2020 2020 2020 7365 7276              serv
+000078a0: 6572 0a20 2020 2020 2020 2022 2222 0a20  er.        """. 
+000078b0: 2020 2020 2020 2023 2070 796c 696e 743a         # pylint:
+000078c0: 2064 6973 6162 6c65 3d6e 6f2d 6d65 6d62   disable=no-memb
+000078d0: 6572 0a20 2020 2020 2020 2073 656c 662e  er.        self.
+000078e0: 5f70 6172 7365 5f61 7267 7328 6473 6e2c  _parse_args(dsn,
+000078f0: 2075 7365 722c 2070 6173 7377 6f72 642c   user, password,
+00007900: 2068 6f73 742c 2064 6174 6162 6173 652c   host, database,
+00007910: 2074 6c73 2c20 6861 6e64 7368 616b 652c   tls, handshake,
+00007920: 2066 6f72 6365 2c20 636f 6e66 6967 6669   force, configfi
+00007930: 6c65 290a 2020 2020 2020 2020 6173 7365  le).        asse
+00007940: 7274 2073 656c 662e 706f 7274 2069 7320  rt self.port is 
+00007950: 6e6f 7420 4e6f 6e65 0a0a 2020 2020 2020  not None..      
+00007960: 2020 7361 7665 645f 6578 633a 204f 7074    saved_exc: Opt
+00007970: 696f 6e61 6c5b 4578 6365 7074 696f 6e5d  ional[Exception]
+00007980: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00007990: 666f 7220 6f6e 655f 686f 7374 2069 6e20  for one_host in 
+000079a0: 7365 6c66 2e68 6f73 7473 3a0a 2020 2020  self.hosts:.    
+000079b0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+000079c0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+000079d0: 6765 722e 696e 666f 2866 2254 7279 696e  ger.info(f"Tryin
+000079e0: 6720 746f 2063 6f6e 6e65 6374 2074 6f20  g to connect to 
+000079f0: 7b6f 6e65 5f68 6f73 747d 3a7b 7365 6c66  {one_host}:{self
+00007a00: 2e70 6f72 747d 2229 0a20 2020 2020 2020  .port}").       
+00007a10: 2020 2020 2020 2020 2073 656c 662e 736f           self.so
+00007a20: 636b 203d 2073 6f63 6b65 742e 6372 6561  ck = socket.crea
+00007a30: 7465 5f63 6f6e 6e65 6374 696f 6e28 286f  te_connection((o
+00007a40: 6e65 5f68 6f73 742c 2073 656c 662e 706f  ne_host, self.po
+00007a50: 7274 2929 0a20 2020 2020 2020 2020 2020  rt)).           
+00007a60: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
+00007a70: 2866 2243 6f6e 6e65 6374 6564 2074 6f20  (f"Connected to 
+00007a80: 7b6f 6e65 5f68 6f73 747d 3a7b 7365 6c66  {one_host}:{self
+00007a90: 2e70 6f72 747d 206f 6e20 736f 636b 6574  .port} on socket
+00007aa0: 207b 7365 6c66 2e73 6f63 6b7d 2229 0a20   {self.sock}"). 
+00007ab0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00007ac0: 6176 6564 5f65 7863 203d 204e 6f6e 650a  aved_exc = None.
+00007ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ae0: 6272 6561 6b0a 2020 2020 2020 2020 2020  break.          
+00007af0: 2020 6578 6365 7074 2043 6f6e 6e65 6374    except Connect
+00007b00: 696f 6e45 7272 6f72 2061 7320 6578 633a  ionError as exc:
+00007b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007b20: 2073 6176 6564 5f65 7863 203d 2065 7863   saved_exc = exc
+00007b30: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+00007b40: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+00007b50: 2065 7863 3a0a 2020 2020 2020 2020 2020   exc:.          
+00007b60: 2020 2020 2020 7361 7665 645f 6578 6320        saved_exc 
+00007b70: 3d20 6578 630a 0a20 2020 2020 2020 2069  = exc..        i
+00007b80: 6620 7361 7665 645f 6578 6320 6973 206e  f saved_exc is n
+00007b90: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00007ba0: 2020 2020 2072 6169 7365 2045 7272 6f72       raise Error
+00007bb0: 2866 2255 6e61 626c 6520 746f 2063 6f6e  (f"Unable to con
+00007bc0: 6e65 6374 2074 6f20 7b27 2c27 2e6a 6f69  nect to {','.joi
+00007bd0: 6e28 7365 6c66 2e68 6f73 7473 297d 3a7b  n(self.hosts)}:{
+00007be0: 7365 6c66 2e70 6f72 747d 3a20 7b73 7472  self.port}: {str
+00007bf0: 2873 6176 6564 5f65 7863 297d 2229 2066  (saved_exc)}") f
+00007c00: 726f 6d20 7361 7665 645f 6578 630a 0a20  rom saved_exc.. 
+00007c10: 2020 2020 2020 2073 656c 662e 5f73 736c         self._ssl
+00007c20: 697a 655f 636f 6e6e 6563 7469 6f6e 2829  ize_connection()
+00007c30: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00007c40: 6275 6666 6572 3a20 6279 7465 7320 3d20  buffer: bytes = 
+00007c50: 6222 220a 2020 2020 2020 2020 7365 6c66  b"".        self
+00007c60: 2e73 6573 7369 6f6e 203d 2073 6573 7369  .session = sessi
+00007c70: 6f6e 0a20 2020 2020 2020 2069 6620 7365  on.        if se
+00007c80: 6c66 2e68 616e 6473 6861 6b65 203d 3d20  lf.handshake == 
+00007c90: 7365 6c66 2e48 414e 4453 4841 4b45 5f53  self.HANDSHAKE_S
+00007ca0: 534f 3a0a 2020 2020 2020 2020 2020 2020  SO:.            
+00007cb0: 6966 2073 656c 662e 7573 6572 206f 7220  if self.user or 
+00007cc0: 7365 6c66 2e70 6173 7377 6f72 643a 0a20  self.password:. 
+00007cd0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00007ce0: 2049 6620 6569 7468 6572 2061 7265 206e   If either are n
+00007cf0: 6f6e 2d65 6d70 7479 2c20 7573 6520 7468  on-empty, use th
+00007d00: 6520 4342 435f 4743 4d2e 0a20 2020 2020  e CBC_GCM..     
+00007d10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00007d20: 5f63 6c69 656e 745f 6861 6e64 7368 616b  _client_handshak
+00007d30: 655f 4342 435f 4743 4d28 6973 5f65 7870  e_CBC_GCM(is_exp
+00007d40: 6c69 6369 745f 7373 6f3d 5472 7565 2c20  licit_sso=True, 
+00007d50: 666f 7263 653d 7365 6c66 2e66 6f72 6365  force=self.force
+00007d60: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00007d70: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00007d80: 2020 2020 6966 2073 656c 662e 7365 7373      if self.sess
+00007d90: 696f 6e20 6973 206e 6f74 204e 6f6e 6520  ion is not None 
+00007da0: 616e 6420 7365 6c66 2e73 6573 7369 6f6e  and self.session
+00007db0: 2e73 6563 7572 6974 7954 6f6b 656e 2069  .securityToken i
+00007dc0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00007dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007de0: 7365 6c66 2e5f 636c 6965 6e74 5f68 616e  self._client_han
+00007df0: 6473 6861 6b65 5f73 6563 7572 6974 795f  dshake_security_
+00007e00: 746f 6b65 6e28 290a 2020 2020 2020 2020  token().        
+00007e10: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00007e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e30: 2020 7365 6c66 2e5f 636c 6965 6e74 5f68    self._client_h
+00007e40: 616e 6473 6861 6b65 5f53 534f 2829 0a20  andshake_SSO(). 
+00007e50: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00007e60: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+00007e70: 6c69 656e 745f 6861 6e64 7368 616b 655f  lient_handshake_
+00007e80: 4342 435f 4743 4d28 6973 5f65 7870 6c69  CBC_GCM(is_expli
+00007e90: 6369 745f 7373 6f3d 4661 6c73 652c 2066  cit_sso=False, f
+00007ea0: 6f72 6365 3d73 656c 662e 666f 7263 6529  orce=self.force)
+00007eb0: 0a0a 2020 2020 6465 6620 5f5f 656e 7465  ..    def __ente
+00007ec0: 725f 5f28 7365 6c66 2920 2d3e 2022 436f  r__(self) -> "Co
+00007ed0: 6e6e 6563 7469 6f6e 223a 0a20 2020 2020  nnection":.     
+00007ee0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+00007ef0: 2020 2020 6465 6620 5f5f 6578 6974 5f5f      def __exit__
+00007f00: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
+00007f10: 6578 635f 7479 7065 3a20 4f70 7469 6f6e  exc_type: Option
+00007f20: 616c 5b54 7970 655b 4261 7365 4578 6365  al[Type[BaseExce
+00007f30: 7074 696f 6e5d 5d2c 2065 7863 5f76 616c  ption]], exc_val
+00007f40: 3a20 4f70 7469 6f6e 616c 5b42 6173 6545  : Optional[BaseE
+00007f50: 7863 6570 7469 6f6e 5d2c 2065 7863 5f74  xception], exc_t
+00007f60: 623a 204f 7074 696f 6e61 6c5b 5472 6163  b: Optional[Trac
+00007f70: 6562 6163 6b54 7970 655d 0a20 2020 2029  ebackType].    )
+00007f80: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00007f90: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+00007fa0: 5f69 6e69 7469 616c 697a 655f 636c 6965  _initialize_clie
+00007fb0: 6e74 5f63 6f6e 6e65 6374 696f 6e28 0a20  nt_connection(. 
+00007fc0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00007fd0: 2020 2020 2063 6c69 656e 745f 636f 6e6e       client_conn
+00007fe0: 6563 7469 6f6e 5f6d 6573 7361 6765 3a20  ection_message: 
+00007ff0: 556e 696f 6e5b 0a20 2020 2020 2020 2020  Union[.         
+00008000: 2020 2070 726f 746f 2e43 6c69 656e 7443     proto.ClientC
+00008010: 6f6e 6e65 6374 696f 6e2c 0a20 2020 2020  onnection,.     
+00008020: 2020 2020 2020 2070 726f 746f 2e43 6c69         proto.Cli
+00008030: 656e 7443 6f6e 6e65 6374 696f 6e47 434d  entConnectionGCM
+00008040: 2c0a 2020 2020 2020 2020 2020 2020 7072  ,.            pr
+00008050: 6f74 6f2e 436c 6965 6e74 436f 6e6e 6563  oto.ClientConnec
+00008060: 7469 6f6e 5365 6375 7269 7479 546f 6b65  tionSecurityToke
+00008070: 6e2c 0a20 2020 2020 2020 2020 2020 2070  n,.            p
+00008080: 726f 746f 2e43 6c69 656e 7443 6f6e 6e65  roto.ClientConne
+00008090: 6374 696f 6e53 534f 2c0a 2020 2020 2020  ctionSSO,.      
+000080a0: 2020 5d2c 0a20 2020 2029 202d 3e20 4e6f    ],.    ) -> No
+000080b0: 6e65 3a0a 2020 2020 2020 2020 2222 2249  ne:.        """I
+000080c0: 6e69 7469 616c 697a 6573 2066 6965 6c64  nitializes field
+000080d0: 7320 7573 6564 2069 6e20 696e 6974 6961  s used in initia
+000080e0: 6c20 636c 6965 6e74 2068 616e 6473 6861  l client handsha
+000080f0: 6b65 2072 6571 7565 7374 732e 0a20 2020  ke requests..   
+00008100: 2020 2020 2031 2e20 6461 7461 6261 7365       1. database
+00008110: 0a20 2020 2020 2020 2032 2e20 636c 6965  .        2. clie
+00008120: 6e74 6964 2028 7079 6f63 6965 6e74 290a  ntid (pyocient).
+00008130: 2020 2020 2020 2020 332e 2070 726f 746f          3. proto
+00008140: 636f 6c20 7665 7273 696f 6e0a 2020 2020  col version.    
+00008150: 2020 2020 342e 2076 6572 7369 6f6e 5f6d      4. version_m
+00008160: 616a 6f72 0a20 2020 2020 2020 2035 2e20  ajor.        5. 
+00008170: 7665 7273 696f 6e5f 6d69 6e6f 720a 2020  version_minor.  
+00008180: 2020 2020 2020 362e 2073 6573 7369 6f6e        6. session
+00008190: 2069 640a 0a20 2020 2020 2020 204e 6f74   id..        Not
+000081a0: 652c 206e 6f74 2061 6c6c 2066 6965 6c64  e, not all field
+000081b0: 7320 6172 6520 696e 6974 6961 6c69 7a65  s are initialize
+000081c0: 642e 2053 6f6d 6520 6669 656c 6473 2061  d. Some fields a
+000081d0: 7265 2073 7065 6369 616c 2074 6f20 6365  re special to ce
+000081e0: 7274 6169 6e20 636c 6965 6e74 2068 616e  rtain client han
+000081f0: 6473 6861 6b65 732e 0a20 2020 2020 2020  dshakes..       
+00008200: 2046 6f72 2065 7861 6d70 6c65 2c20 7468   For example, th
+00008210: 6520 5353 4f20 6861 6e64 7368 616b 6520  e SSO handshake 
+00008220: 7769 7468 2074 6f6b 656e 2064 6f65 7320  with token does 
+00008230: 6e6f 7420 7461 6b65 2075 7365 7220 616e  not take user an
+00008240: 6420 696e 7374 6561 6420 7461 6b65 7320  d instead takes 
+00008250: 6120 7365 6375 7269 7479 2074 6f6b 656e  a security token
+00008260: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+00008270: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
+00008280: 656e 745f 636f 6e6e 6563 7469 6f6e 5f6d  ent_connection_m
+00008290: 6573 7361 6765 2028 5b70 726f 746f 206d  essage ([proto m
+000082a0: 6573 7361 6765 5d29 3a20 7468 6520 636c  essage]): the cl
+000082b0: 6965 6e74 2068 616e 6473 6861 6b65 2072  ient handshake r
+000082c0: 6571 7565 7374 2074 6f20 696e 6974 6961  equest to initia
+000082d0: 6c69 7a65 0a20 2020 2020 2020 2022 2222  lize.        """
+000082e0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+000082f0: 7365 6c66 2e64 6174 6162 6173 6520 6973  self.database is
+00008300: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
+00008310: 2020 636c 6965 6e74 5f63 6f6e 6e65 6374    client_connect
+00008320: 696f 6e5f 6d65 7373 6167 652e 6461 7461  ion_message.data
+00008330: 6261 7365 203d 2073 656c 662e 6461 7461  base = self.data
+00008340: 6261 7365 0a20 2020 2020 2020 2063 6c69  base.        cli
+00008350: 656e 745f 636f 6e6e 6563 7469 6f6e 5f6d  ent_connection_m
+00008360: 6573 7361 6765 2e63 6c69 656e 7469 6420  essage.clientid 
+00008370: 3d20 4452 4956 4552 5f49 440a 2020 2020  = DRIVER_ID.    
+00008380: 2020 2020 636c 6965 6e74 5f63 6f6e 6e65      client_conne
+00008390: 6374 696f 6e5f 6d65 7373 6167 652e 7665  ction_message.ve
+000083a0: 7273 696f 6e20 3d20 5052 4f54 4f43 4f4c  rsion = PROTOCOL
+000083b0: 5f56 4552 5349 4f4e 0a20 2020 2020 2020  _VERSION.       
+000083c0: 2063 6c69 656e 745f 636f 6e6e 6563 7469   client_connecti
+000083d0: 6f6e 5f6d 6573 7361 6765 2e6d 616a 6f72  on_message.major
+000083e0: 436c 6965 6e74 5665 7273 696f 6e20 3d20  ClientVersion = 
+000083f0: 7665 7273 696f 6e5f 6d61 6a6f 720a 2020  version_major.  
+00008400: 2020 2020 2020 636c 6965 6e74 5f63 6f6e        client_con
+00008410: 6e65 6374 696f 6e5f 6d65 7373 6167 652e  nection_message.
+00008420: 6d69 6e6f 7243 6c69 656e 7456 6572 7369  minorClientVersi
+00008430: 6f6e 203d 2076 6572 7369 6f6e 5f6d 696e  on = version_min
+00008440: 6f72 0a20 2020 2020 2020 2063 6c69 656e  or.        clien
+00008450: 745f 636f 6e6e 6563 7469 6f6e 5f6d 6573  t_connection_mes
+00008460: 7361 6765 2e73 6573 7369 6f6e 4944 203d  sage.sessionID =
+00008470: 2073 656c 662e 7365 7373 696f 6e5f 6964   self.session_id
+00008480: 0a0a 2020 2020 6465 6620 5f63 6c69 656e  ..    def _clien
+00008490: 745f 6861 6e64 7368 616b 655f 4342 435f  t_handshake_CBC_
+000084a0: 4743 4d28 7365 6c66 2c20 6973 5f65 7870  GCM(self, is_exp
+000084b0: 6c69 6369 745f 7373 6f3a 2062 6f6f 6c20  licit_sso: bool 
+000084c0: 3d20 4661 6c73 652c 2066 6f72 6365 3a20  = False, force: 
+000084d0: 626f 6f6c 203d 2046 616c 7365 2920 2d3e  bool = False) ->
+000084e0: 204e 6f6e 653a 0a20 2020 2020 2020 2077   None:.        w
+000084f0: 6869 6c65 2054 7275 653a 0a20 2020 2020  hile True:.     
+00008500: 2020 2020 2020 2023 2323 2323 2323 2323         #########
+00008510: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00008520: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00008530: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00008540: 2323 2323 2323 2323 230a 2020 2020 2020  #########.      
+00008550: 2020 2020 2020 2320 5365 6e64 2074 6865        # Send the
+00008560: 2043 4c49 454e 545f 434f 4e4e 4543 5449   CLIENT_CONNECTI
+00008570: 4f4e 2072 6571 7565 7374 0a20 2020 2020  ON request.     
+00008580: 2020 2020 2020 2023 2323 2323 2323 2323         #########
+00008590: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000085a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000085b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000085c0: 2323 2323 2323 2323 230a 2020 2020 2020  #########.      
+000085d0: 2020 2020 2020 636c 6965 6e74 5f63 6f6e        client_con
+000085e0: 6e65 6374 696f 6e3a 2055 6e69 6f6e 5b70  nection: Union[p
+000085f0: 726f 746f 2e43 6c69 656e 7443 6f6e 6e65  roto.ClientConne
+00008600: 6374 696f 6e2c 2070 726f 746f 2e43 6c69  ction, proto.Cli
+00008610: 656e 7443 6f6e 6e65 6374 696f 6e47 434d  entConnectionGCM
+00008620: 5d0a 2020 2020 2020 2020 2020 2020 7265  ].            re
+00008630: 7120 3d20 7072 6f74 6f2e 5265 7175 6573  q = proto.Reques
+00008640: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+00008650: 6966 2073 656c 662e 6861 6e64 7368 616b  if self.handshak
+00008660: 6520 3d3d 2073 656c 662e 4841 4e44 5348  e == self.HANDSH
+00008670: 414b 455f 4342 433a 0a20 2020 2020 2020  AKE_CBC:.       
+00008680: 2020 2020 2020 2020 2072 6571 2e74 7970           req.typ
+00008690: 6520 3d20 7265 712e 434c 4945 4e54 5f43  e = req.CLIENT_C
+000086a0: 4f4e 4e45 4354 494f 4e0a 2020 2020 2020  ONNECTION.      
+000086b0: 2020 2020 2020 2020 2020 636c 6965 6e74            client
+000086c0: 5f63 6f6e 6e65 6374 696f 6e20 3d20 7265  _connection = re
+000086d0: 712e 636c 6965 6e74 5f63 6f6e 6e65 6374  q.client_connect
+000086e0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+000086f0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00008700: 2020 2020 2020 2320 5368 6f75 6c64 2062        # Should b
+00008710: 6520 4743 4d0a 2020 2020 2020 2020 2020  e GCM.          
+00008720: 2020 2020 2020 7265 712e 7479 7065 203d        req.type =
+00008730: 2072 6571 2e43 4c49 454e 545f 434f 4e4e   req.CLIENT_CONN
+00008740: 4543 5449 4f4e 5f47 434d 0a20 2020 2020  ECTION_GCM.     
+00008750: 2020 2020 2020 2020 2020 2063 6c69 656e             clien
+00008760: 745f 636f 6e6e 6563 7469 6f6e 203d 2072  t_connection = r
+00008770: 6571 2e63 6c69 656e 745f 636f 6e6e 6563  eq.client_connec
+00008780: 7469 6f6e 5f67 636d 0a20 2020 2020 2020  tion_gcm.       
+00008790: 2020 2020 2020 2020 2063 6c69 656e 745f           client_
+000087a0: 636f 6e6e 6563 7469 6f6e 2e65 7870 6c69  connection.expli
+000087b0: 6369 7453 534f 203d 2069 735f 6578 706c  citSSO = is_expl
+000087c0: 6963 6974 5f73 736f 0a20 2020 2020 2020  icit_sso.       
+000087d0: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
+000087e0: 2e75 7365 7220 6973 206e 6f74 204e 6f6e  .user is not Non
+000087f0: 650a 2020 2020 2020 2020 2020 2020 636c  e.            cl
+00008800: 6965 6e74 5f63 6f6e 6e65 6374 696f 6e2e  ient_connection.
+00008810: 7573 6572 6964 203d 2073 656c 662e 7573  userid = self.us
+00008820: 6572 0a20 2020 2020 2020 2020 2020 2073  er.            s
+00008830: 656c 662e 5f69 6e69 7469 616c 697a 655f  elf._initialize_
+00008840: 636c 6965 6e74 5f63 6f6e 6e65 6374 696f  client_connectio
+00008850: 6e28 636c 6965 6e74 5f63 6f6e 6e65 6374  n(client_connect
+00008860: 696f 6e29 0a0a 2020 2020 2020 2020 2020  ion)..          
+00008870: 2020 5f73 656e 645f 6d73 6728 7365 6c66    _send_msg(self
+00008880: 2c20 7265 7129 0a0a 2020 2020 2020 2020  , req)..        
+00008890: 2020 2020 2323 2323 2323 2323 2323 2323      ############
+000088a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000088b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000088c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000088d0: 2323 2323 2323 0a20 2020 2020 2020 2020  ######.         
+000088e0: 2020 2023 2047 6574 2074 6865 2043 4c49     # Get the CLI
+000088f0: 454e 545f 434f 4e4e 4543 5449 4f4e 2072  ENT_CONNECTION r
+00008900: 6573 706f 6e73 6520 616e 6420 7072 6f63  esponse and proc
+00008910: 6573 7320 6974 0a20 2020 2020 2020 2020  ess it.         
+00008920: 2020 2023 2323 2323 2323 2323 2323 2323     #############
+00008930: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00008940: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00008950: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00008960: 2323 2323 230a 2020 2020 2020 2020 2020  #####.          
+00008970: 2020 7273 7031 3a20 556e 696f 6e5b 7072    rsp1: Union[pr
+00008980: 6f74 6f2e 436c 6965 6e74 436f 6e6e 6563  oto.ClientConnec
+00008990: 7469 6f6e 5265 7370 6f6e 7365 2c20 7072  tionResponse, pr
+000089a0: 6f74 6f2e 436c 6965 6e74 436f 6e6e 6563  oto.ClientConnec
+000089b0: 7469 6f6e 4743 4d52 6573 706f 6e73 655d  tionGCMResponse]
+000089c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000089d0: 7365 6c66 2e68 616e 6473 6861 6b65 203d  self.handshake =
+000089e0: 3d20 7365 6c66 2e48 414e 4453 4841 4b45  = self.HANDSHAKE
+000089f0: 5f43 4243 3a0a 2020 2020 2020 2020 2020  _CBC:.          
+00008a00: 2020 2020 2020 2320 4342 430a 2020 2020        # CBC.    
+00008a10: 2020 2020 2020 2020 2020 2020 7273 7031              rsp1
+00008a20: 203d 205f 7265 6376 5f6d 7367 2873 656c   = _recv_msg(sel
+00008a30: 662c 2070 726f 746f 2e43 6c69 656e 7443  f, proto.ClientC
+00008a40: 6f6e 6e65 6374 696f 6e52 6573 706f 6e73  onnectionRespons
+00008a50: 6528 2929 0a20 2020 2020 2020 2020 2020  e()).           
+00008a60: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00008a70: 2020 2020 2020 2023 2047 434d 206f 7220         # GCM or 
+00008a80: 6578 706c 6963 6974 2053 534f 0a20 2020  explicit SSO.   
+00008a90: 2020 2020 2020 2020 2020 2020 2072 7370               rsp
+00008aa0: 3120 3d20 5f72 6563 765f 6d73 6728 7365  1 = _recv_msg(se
+00008ab0: 6c66 2c20 7072 6f74 6f2e 436c 6965 6e74  lf, proto.Client
+00008ac0: 436f 6e6e 6563 7469 6f6e 4743 4d52 6573  ConnectionGCMRes
+00008ad0: 706f 6e73 6528 2929 0a0a 2020 2020 2020  ponse())..      
+00008ae0: 2020 2020 2020 6966 2072 7370 312e 7265        if rsp1.re
+00008af0: 7370 6f6e 7365 2e74 7970 6520 3d3d 2070  sponse.type == p
+00008b00: 726f 746f 2e43 6f6e 6669 726d 6174 696f  roto.Confirmatio
+00008b10: 6e52 6573 706f 6e73 652e 5245 5350 4f4e  nResponse.RESPON
+00008b20: 5345 5f57 4152 4e3a 0a20 2020 2020 2020  SE_WARN:.       
+00008b30: 2020 2020 2020 2020 2077 6172 6e28 7273           warn(rs
+00008b40: 7031 2e72 6573 706f 6e73 652e 7265 6173  p1.response.reas
+00008b50: 6f6e 290a 2020 2020 2020 2020 2020 2020  on).            
+00008b60: 656c 6966 206e 6f74 2072 7370 312e 7265  elif not rsp1.re
+00008b70: 7370 6f6e 7365 2e74 7970 6520 3d3d 2070  sponse.type == p
+00008b80: 726f 746f 2e43 6f6e 6669 726d 6174 696f  roto.Confirmatio
+00008b90: 6e52 6573 706f 6e73 652e 5245 5350 4f4e  nResponse.RESPON
+00008ba0: 5345 5f4f 4b3a 0a20 2020 2020 2020 2020  SE_OK:.         
+00008bb0: 2020 2020 2020 2072 6169 7365 205f 636f         raise _co
+00008bc0: 6e76 6572 745f 6578 6365 7074 696f 6e28  nvert_exception(
+00008bd0: 7273 7031 2e72 6573 706f 6e73 6529 0a0a  rsp1.response)..
+00008be0: 2020 2020 2020 2020 2020 2020 7065 6572              peer
+00008bf0: 5f6b 6579 203d 206c 6f61 645f 7065 6d5f  _key = load_pem_
+00008c00: 7075 626c 6963 5f6b 6579 280a 2020 2020  public_key(.    
+00008c10: 2020 2020 2020 2020 2020 2020 7273 7031              rsp1
+00008c20: 2e70 7562 4b65 792e 656e 636f 6465 2865  .pubKey.encode(e
+00008c30: 6e63 6f64 696e 673d 2255 5446 2d38 222c  ncoding="UTF-8",
+00008c40: 2065 7272 6f72 733d 2273 7472 6963 7422   errors="strict"
+00008c50: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00008c60: 2020 2062 6163 6b65 6e64 3d64 6566 6175     backend=defau
+00008c70: 6c74 5f62 6163 6b65 6e64 2829 2c0a 2020  lt_backend(),.  
+00008c80: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00008c90: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+00008ca0: 7369 6e73 7461 6e63 6528 7065 6572 5f6b  sinstance(peer_k
+00008cb0: 6579 2c20 4448 5075 626c 6963 4b65 7929  ey, DHPublicKey)
+00008cc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00008cd0: 2020 7261 6973 6520 4572 726f 7228 6622    raise Error(f"
+00008ce0: 5075 626c 6963 206b 6579 2077 6173 206e  Public key was n
+00008cf0: 6f74 2044 4850 7562 6c69 634b 6579 2c20  ot DHPublicKey, 
+00008d00: 7761 733a 207b 7479 7065 2870 6565 725f  was: {type(peer_
+00008d10: 6b65 7929 7d22 290a 2020 2020 2020 2020  key)}").        
+00008d20: 2020 2020 2863 6970 6865 722c 2067 656e      (cipher, gen
+00008d30: 6572 6174 6564 5f68 6d61 632c 2070 7562  erated_hmac, pub
+00008d40: 6c69 635f 6b65 7929 203d 2073 656c 662e  lic_key) = self.
+00008d50: 5f65 6e63 7279 7074 696f 6e5f 726f 7574  _encryption_rout
+00008d60: 696e 6528 7273 7031 2e69 762c 2070 6565  ine(rsp1.iv, pee
+00008d70: 725f 6b65 7929 0a0a 2020 2020 2020 2020  r_key)..        
+00008d80: 2020 2020 2323 2323 2323 2323 2323 2323      ############
+00008d90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00008da0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00008db0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00008dc0: 2323 2323 2323 0a20 2020 2020 2020 2020  ######.         
+00008dd0: 2020 2023 2053 656e 6420 7468 6520 434c     # Send the CL
+00008de0: 4945 4e54 5f43 4f4e 4e45 4354 494f 4e32  IENT_CONNECTION2
+00008df0: 2072 6571 7565 7374 0a20 2020 2020 2020   request.       
+00008e00: 2020 2020 2023 2323 2323 2323 2323 2323       ###########
+00008e10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00008e20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00008e30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00008e40: 2323 2323 2323 230a 2020 2020 2020 2020  #######.        
+00008e50: 2020 2020 7265 7120 3d20 7072 6f74 6f2e      req = proto.
+00008e60: 5265 7175 6573 7428 290a 2020 2020 2020  Request().      
+00008e70: 2020 2020 2020 6966 2073 656c 662e 6861        if self.ha
+00008e80: 6e64 7368 616b 6520 3d3d 2073 656c 662e  ndshake == self.
+00008e90: 4841 4e44 5348 414b 455f 4342 433a 0a20  HANDSHAKE_CBC:. 
+00008ea0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00008eb0: 6571 2e74 7970 6520 3d20 7265 712e 434c  eq.type = req.CL
+00008ec0: 4945 4e54 5f43 4f4e 4e45 4354 494f 4e32  IENT_CONNECTION2
+00008ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008ee0: 2072 6571 2e63 6c69 656e 745f 636f 6e6e   req.client_conn
+00008ef0: 6563 7469 6f6e 322e 6369 7068 6572 203d  ection2.cipher =
+00008f00: 2063 6970 6865 720a 2020 2020 2020 2020   cipher.        
+00008f10: 2020 2020 2020 2020 7265 712e 636c 6965          req.clie
+00008f20: 6e74 5f63 6f6e 6e65 6374 696f 6e32 2e66  nt_connection2.f
+00008f30: 6f72 6365 203d 2066 6f72 6365 0a20 2020  orce = force.   
+00008f40: 2020 2020 2020 2020 2020 2020 2072 6571               req
+00008f50: 2e63 6c69 656e 745f 636f 6e6e 6563 7469  .client_connecti
+00008f60: 6f6e 322e 686d 6163 203d 2067 656e 6572  on2.hmac = gener
+00008f70: 6174 6564 5f68 6d61 630a 2020 2020 2020  ated_hmac.      
+00008f80: 2020 2020 2020 2020 2020 7265 712e 636c            req.cl
+00008f90: 6965 6e74 5f63 6f6e 6e65 6374 696f 6e32  ient_connection2
+00008fa0: 2e70 7562 4b65 7920 3d20 7075 626c 6963  .pubKey = public
+00008fb0: 5f6b 6579 2e70 7562 6c69 635f 6279 7465  _key.public_byte
+00008fc0: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
+00008fd0: 2020 2020 2020 2065 6e63 6f64 696e 673d         encoding=
+00008fe0: 7365 7269 616c 697a 6174 696f 6e2e 456e  serialization.En
+00008ff0: 636f 6469 6e67 2e50 454d 2c0a 2020 2020  coding.PEM,.    
+00009000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009010: 666f 726d 6174 3d73 6572 6961 6c69 7a61  format=serializa
+00009020: 7469 6f6e 2e50 7562 6c69 6346 6f72 6d61  tion.PublicForma
+00009030: 742e 5375 626a 6563 7450 7562 6c69 634b  t.SubjectPublicK
+00009040: 6579 496e 666f 2c0a 2020 2020 2020 2020  eyInfo,.        
+00009050: 2020 2020 2020 2020 292e 6465 636f 6465          ).decode
+00009060: 2829 0a20 2020 2020 2020 2020 2020 2065  ().            e
+00009070: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00009080: 2020 2020 2072 6571 2e74 7970 6520 3d20       req.type = 
+00009090: 7265 712e 434c 4945 4e54 5f43 4f4e 4e45  req.CLIENT_CONNE
+000090a0: 4354 494f 4e5f 4743 4d32 0a20 2020 2020  CTION_GCM2.     
+000090b0: 2020 2020 2020 2020 2020 2072 6571 2e63             req.c
+000090c0: 6c69 656e 745f 636f 6e6e 6563 7469 6f6e  lient_connection
+000090d0: 5f67 636d 322e 6369 7068 6572 203d 2063  _gcm2.cipher = c
+000090e0: 6970 6865 720a 2020 2020 2020 2020 2020  ipher.          
+000090f0: 2020 2020 2020 7265 712e 636c 6965 6e74        req.client
+00009100: 5f63 6f6e 6e65 6374 696f 6e5f 6763 6d32  _connection_gcm2
+00009110: 2e66 6f72 6365 203d 2066 6f72 6365 0a20  .force = force. 
+00009120: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00009130: 6571 2e63 6c69 656e 745f 636f 6e6e 6563  eq.client_connec
+00009140: 7469 6f6e 5f67 636d 322e 686d 6163 203d  tion_gcm2.hmac =
+00009150: 2067 656e 6572 6174 6564 5f68 6d61 630a   generated_hmac.
+00009160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009170: 7265 712e 636c 6965 6e74 5f63 6f6e 6e65  req.client_conne
+00009180: 6374 696f 6e5f 6763 6d32 2e65 7870 6c69  ction_gcm2.expli
+00009190: 6369 7453 534f 203d 2069 735f 6578 706c  citSSO = is_expl
+000091a0: 6963 6974 5f73 736f 0a20 2020 2020 2020  icit_sso.       
+000091b0: 2020 2020 2020 2020 2072 6571 2e63 6c69           req.cli
+000091c0: 656e 745f 636f 6e6e 6563 7469 6f6e 5f67  ent_connection_g
+000091d0: 636d 322e 7075 624b 6579 203d 2070 7562  cm2.pubKey = pub
+000091e0: 6c69 635f 6b65 792e 7075 626c 6963 5f62  lic_key.public_b
+000091f0: 7974 6573 280a 2020 2020 2020 2020 2020  ytes(.          
+00009200: 2020 2020 2020 2020 2020 656e 636f 6469            encodi
+00009210: 6e67 3d73 6572 6961 6c69 7a61 7469 6f6e  ng=serialization
+00009220: 2e45 6e63 6f64 696e 672e 5045 4d2c 0a20  .Encoding.PEM,. 
+00009230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009240: 2020 2066 6f72 6d61 743d 7365 7269 616c     format=serial
+00009250: 697a 6174 696f 6e2e 5075 626c 6963 466f  ization.PublicFo
+00009260: 726d 6174 2e53 7562 6a65 6374 5075 626c  rmat.SubjectPubl
+00009270: 6963 4b65 7949 6e66 6f2c 0a20 2020 2020  icKeyInfo,.     
+00009280: 2020 2020 2020 2020 2020 2029 2e64 6563             ).dec
+00009290: 6f64 6528 290a 0a20 2020 2020 2020 2020  ode()..         
+000092a0: 2020 205f 7365 6e64 5f6d 7367 2873 656c     _send_msg(sel
+000092b0: 662c 2072 6571 290a 0a20 2020 2020 2020  f, req)..       
+000092c0: 2020 2020 2023 2323 2323 2323 2323 2323       ###########
+000092d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000092e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000092f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00009300: 2323 2323 2323 230a 2020 2020 2020 2020  #######.        
+00009310: 2020 2020 2320 4765 7420 7468 6520 434c      # Get the CL
+00009320: 4945 4e54 5f43 4f4e 4e45 4354 494f 4e20  IENT_CONNECTION 
+00009330: 7265 7370 6f6e 7365 2061 6e64 2070 726f  response and pro
+00009340: 6365 7373 2069 740a 2020 2020 2020 2020  cess it.        
+00009350: 2020 2020 2323 2323 2323 2323 2323 2323      ############
+00009360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00009370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00009380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00009390: 2323 2323 2323 0a20 2020 2020 2020 2020  ######.         
+000093a0: 2020 2072 7370 323a 2055 6e69 6f6e 5b70     rsp2: Union[p
+000093b0: 726f 746f 2e43 6c69 656e 7443 6f6e 6e65  roto.ClientConne
+000093c0: 6374 696f 6e32 5265 7370 6f6e 7365 2c20  ction2Response, 
+000093d0: 7072 6f74 6f2e 436c 6965 6e74 436f 6e6e  proto.ClientConn
+000093e0: 6563 7469 6f6e 4743 4d32 5265 7370 6f6e  ectionGCM2Respon
+000093f0: 7365 5d0a 2020 2020 2020 2020 2020 2020  se].            
+00009400: 6966 2073 656c 662e 6861 6e64 7368 616b  if self.handshak
+00009410: 6520 3d3d 2073 656c 662e 4841 4e44 5348  e == self.HANDSH
+00009420: 414b 455f 4342 433a 0a20 2020 2020 2020  AKE_CBC:.       
+00009430: 2020 2020 2020 2020 2023 2043 4243 0a20           # CBC. 
+00009440: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00009450: 7370 3220 3d20 5f72 6563 765f 6d73 6728  sp2 = _recv_msg(
+00009460: 7365 6c66 2c20 7072 6f74 6f2e 436c 6965  self, proto.Clie
+00009470: 6e74 436f 6e6e 6563 7469 6f6e 3252 6573  ntConnection2Res
+00009480: 706f 6e73 6528 2929 0a20 2020 2020 2020  ponse()).       
+00009490: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000094a0: 2020 2020 2020 2020 2020 2023 2047 434d             # GCM
+000094b0: 206f 7220 6578 706c 6963 6974 2053 534f   or explicit SSO
+000094c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000094d0: 2072 7370 3220 3d20 5f72 6563 765f 6d73   rsp2 = _recv_ms
+000094e0: 6728 7365 6c66 2c20 7072 6f74 6f2e 436c  g(self, proto.Cl
+000094f0: 6965 6e74 436f 6e6e 6563 7469 6f6e 4743  ientConnectionGC
+00009500: 4d32 5265 7370 6f6e 7365 2829 290a 0a20  M2Response()).. 
+00009510: 2020 2020 2020 2020 2020 2069 6620 7273             if rs
+00009520: 7032 2e72 6573 706f 6e73 652e 7479 7065  p2.response.type
+00009530: 203d 3d20 7072 6f74 6f2e 436f 6e66 6972   == proto.Confir
+00009540: 6d61 7469 6f6e 5265 7370 6f6e 7365 2e52  mationResponse.R
+00009550: 4553 504f 4e53 455f 5741 524e 3a0a 2020  ESPONSE_WARN:.  
+00009560: 2020 2020 2020 2020 2020 2020 2020 7761                wa
+00009570: 726e 2872 7370 322e 7265 7370 6f6e 7365  rn(rsp2.response
+00009580: 2e72 6561 736f 6e29 0a20 2020 2020 2020  .reason).       
+00009590: 2020 2020 2065 6c69 6620 7273 7032 2e72       elif rsp2.r
+000095a0: 6573 706f 6e73 652e 7479 7065 203d 3d20  esponse.type == 
+000095b0: 7072 6f74 6f2e 436f 6e66 6972 6d61 7469  proto.Confirmati
+000095c0: 6f6e 5265 7370 6f6e 7365 2e52 4553 504f  onResponse.RESPO
+000095d0: 4e53 455f 4f4b 3a0a 2020 2020 2020 2020  NSE_OK:.        
+000095e0: 2020 2020 2020 2020 2320 5361 7665 2074          # Save t
+000095f0: 6865 2073 6572 7665 7220 7365 7373 696f  he server sessio
+00009600: 6e20 6964 0a20 2020 2020 2020 2020 2020  n id.           
+00009610: 2020 2020 2073 656c 662e 7365 7276 6572       self.server
+00009620: 5365 7373 696f 6e49 6420 3d20 7273 7032  SessionId = rsp2
+00009630: 2e73 6572 7665 7253 6573 7369 6f6e 4964  .serverSessionId
+00009640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009650: 2073 656c 662e 7365 7373 696f 6e20 3d20   self.session = 
+00009660: 5365 7373 696f 6e28 7573 6572 416e 6450  Session(userAndP
+00009670: 6173 7377 6f72 643d 5573 6572 416e 6450  assword=UserAndP
+00009680: 6173 7377 6f72 6428 7365 6c66 2e75 7365  assword(self.use
+00009690: 722c 2073 656c 662e 7061 7373 776f 7264  r, self.password
+000096a0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+000096b0: 2020 206c 6f67 6765 722e 696e 666f 2866     logger.info(f
+000096c0: 2243 6f6e 6e65 6374 6564 2074 6f20 7365  "Connected to se
+000096d0: 7276 6572 2073 6573 7369 6f6e 2049 643a  rver session Id:
+000096e0: 207b 7365 6c66 2e73 6572 7665 7253 6573   {self.serverSes
+000096f0: 7369 6f6e 4964 7d22 290a 2020 2020 2020  sionId}").      
+00009700: 2020 2020 2020 2020 2020 2320 5361 7665            # Save
+00009710: 2073 6563 6f6e 6461 7279 2069 6e74 6572   secondary inter
+00009720: 6661 6365 732e 0a20 2020 2020 2020 2020  faces..         
+00009730: 2020 2020 2020 2073 656c 662e 5f73 6176         self._sav
+00009740: 655f 7365 636f 6e64 6172 795f 696e 7465  e_secondary_inte
+00009750: 7266 6163 6573 2872 7370 322e 7365 636f  rfaces(rsp2.seco
+00009760: 6e64 6172 7929 0a0a 2020 2020 2020 2020  ndary)..        
+00009770: 2020 2020 2020 2020 2320 5265 6469 7265          # Redire
+00009780: 6374 2074 6865 2063 6f6e 6e65 6374 696f  ct the connectio
+00009790: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+000097a0: 2020 6966 2072 7370 322e 7265 6469 7265    if rsp2.redire
+000097b0: 6374 3a0a 2020 2020 2020 2020 2020 2020  ct:.            
+000097c0: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
+000097d0: 656c 662e 736f 636b 2069 7320 6e6f 7420  elf.sock is not 
+000097e0: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+000097f0: 2020 2020 2020 2020 2073 656c 662e 736f           self.so
+00009800: 636b 2e63 6c6f 7365 2829 0a20 2020 2020  ck.close().     
+00009810: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00009820: 6170 7065 645f 686f 7374 2c20 6d61 7070  apped_host, mapp
+00009830: 6564 5f70 6f72 7420 3d20 7365 6c66 2e72  ed_port = self.r
+00009840: 6573 6f6c 7665 5f6e 6577 5f65 6e64 706f  esolve_new_endpo
+00009850: 696e 7428 7273 7032 2e72 6564 6972 6563  int(rsp2.redirec
+00009860: 7448 6f73 742c 2072 7370 322e 7265 6469  tHost, rsp2.redi
+00009870: 7265 6374 506f 7274 290a 2020 2020 2020  rectPort).      
+00009880: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00009890: 6767 6572 2e64 6562 7567 280a 2020 2020  gger.debug(.    
+000098a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098b0: 2020 2020 6622 5265 6469 7265 6374 696e      f"Redirectin
+000098c0: 6720 636f 6e6e 6563 7469 6f6e 2074 6f20  g connection to 
+000098d0: 7b72 7370 322e 7265 6469 7265 6374 486f  {rsp2.redirectHo
+000098e0: 7374 7d3a 7b72 7370 322e 7265 6469 7265  st}:{rsp2.redire
+000098f0: 6374 506f 7274 7d2c 2077 6869 6368 206d  ctPort}, which m
+00009900: 6170 7320 746f 207b 6d61 7070 6564 5f68  aps to {mapped_h
+00009910: 6f73 747d 3a7b 6d61 7070 6564 5f70 6f72  ost}:{mapped_por
+00009920: 747d 220a 2020 2020 2020 2020 2020 2020  t}".            
+00009930: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00009940: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00009950: 6c66 2e73 6f63 6b20 3d20 736f 636b 6574  lf.sock = socket
+00009960: 2e63 7265 6174 655f 636f 6e6e 6563 7469  .create_connecti
+00009970: 6f6e 2828 6d61 7070 6564 5f68 6f73 742c  on((mapped_host,
+00009980: 206d 6170 7065 645f 706f 7274 2929 0a20   mapped_port)). 
+00009990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099a0: 2020 206c 6f67 6765 722e 696e 666f 2866     logger.info(f
+000099b0: 2243 6f6e 6e65 6374 6564 2074 6f20 7b6d  "Connected to {m
+000099c0: 6170 7065 645f 686f 7374 7d3a 7b6d 6170  apped_host}:{map
+000099d0: 7065 645f 706f 7274 7d20 6f6e 2073 6f63  ped_port} on soc
+000099e0: 6b65 7420 7b73 656c 662e 736f 636b 7d22  ket {self.sock}"
+000099f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00009a00: 2020 2020 2020 7365 6c66 2e5f 7373 6c69        self._ssli
+00009a10: 7a65 5f63 6f6e 6e65 6374 696f 6e28 290a  ze_connection().
+00009a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009a30: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00009a40: 2e5f 636c 6965 6e74 5f68 616e 6473 6861  ._client_handsha
+00009a50: 6b65 5f43 4243 5f47 434d 2869 735f 6578  ke_CBC_GCM(is_ex
+00009a60: 706c 6963 6974 5f73 736f 2c20 5472 7565  plicit_sso, True
+00009a70: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+00009a80: 2020 2062 7265 616b 0a0a 2020 2020 2020     break..      
+00009a90: 2020 2020 2020 2320 7468 6572 6520 6973        # there is
+00009aa0: 2073 6f6d 6574 6869 6e67 2062 726f 6b65   something broke
+00009ab0: 6e20 696e 206f 7572 2068 616e 6473 6861  n in our handsha
+00009ac0: 6b65 2e2e 2e72 6574 7279 0a20 2020 2020  ke...retry.     
+00009ad0: 2020 2020 2020 2069 6620 7273 7032 2e72         if rsp2.r
+00009ae0: 6573 706f 6e73 652e 7665 6e64 6f72 5f63  esponse.vendor_c
+00009af0: 6f64 6520 3d3d 202d 3230 323a 0a20 2020  ode == -202:.   
+00009b00: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00009b10: 6765 722e 6465 6275 6728 2248 616e 6473  ger.debug("Hands
+00009b20: 6861 6b65 2065 7272 6f72 2e2e 2e72 6574  hake error...ret
+00009b30: 7279 696e 6722 290a 2020 2020 2020 2020  rying").        
+00009b40: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+00009b50: 0a0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
+00009b60: 6973 6520 5f63 6f6e 7665 7274 5f65 7863  ise _convert_exc
+00009b70: 6570 7469 6f6e 2872 7370 322e 7265 7370  eption(rsp2.resp
+00009b80: 6f6e 7365 290a 0a20 2020 2064 6566 205f  onse)..    def _
+00009b90: 636c 6965 6e74 5f68 616e 6473 6861 6b65  client_handshake
+00009ba0: 5f53 534f 2873 656c 6629 202d 3e20 4e6f  _SSO(self) -> No
+00009bb0: 6e65 3a0a 2020 2020 2020 2020 2222 2249  ne:.        """I
+00009bc0: 6e74 6572 6e61 6c20 726f 7574 696e 6520  nternal routine 
+00009bd0: 666f 7220 7369 6e67 6c65 2073 6967 6e20  for single sign 
+00009be0: 6f6e 2068 616e 6473 6861 6b65 2028 5353  on handshake (SS
+00009bf0: 4f29 2e0a 2020 2020 2020 2020 312e 2044  O)..        1. D
+00009c00: 7269 7665 7220 7265 7175 6573 7473 2074  river requests t
+00009c10: 6f20 7369 676e 206f 6e20 7669 6120 5353  o sign on via SS
+00009c20: 4f2e 0a20 2020 2020 2020 2032 2e20 5365  O..        2. Se
+00009c30: 7276 6572 2073 656e 6473 2062 6163 6b20  rver sends back 
+00009c40: 616e 2061 7574 6865 6e74 6963 6174 696f  an authenticatio
+00009c50: 6e20 5552 4c2e 0a20 2020 2020 2020 2033  n URL..        3
+00009c60: 2e20 4472 6976 6572 206c 6175 6e63 6865  . Driver launche
+00009c70: 7320 5552 4c20 696e 2064 6566 6175 6c74  s URL in default
+00009c80: 2062 726f 7773 6572 2028 6f72 2070 7269   browser (or pri
+00009c90: 6e74 7320 7468 6520 7572 6c20 746f 2073  nts the url to s
+00009ca0: 7464 206f 7574 2069 6620 6e6f 7420 706f  td out if not po
+00009cb0: 7373 6962 6c65 290a 2020 2020 2020 2020  ssible).        
+00009cc0: 342e 2055 7365 7220 6175 7468 656e 7469  4. User authenti
+00009cd0: 6361 7465 7320 696e 2062 726f 7773 6572  cates in browser
+00009ce0: 2e0a 2020 2020 2020 2020 352e 2044 7269  ..        5. Dri
+00009cf0: 7665 7220 636f 6e74 696e 756f 7573 6c79  ver continuously
+00009d00: 2070 6f6c 6c73 2074 6865 2064 6174 6162   polls the datab
+00009d10: 6173 6520 756e 7469 6c20 6c6f 6769 6e20  ase until login 
+00009d20: 636f 6d70 6c65 7465 732e 0a20 2020 2020  completes..     
+00009d30: 2020 2036 2e20 5570 6f6e 2063 6f6d 706c     6. Upon compl
+00009d40: 6574 696f 6e2c 2073 6572 7665 7220 7365  etion, server se
+00009d50: 6e64 7320 6261 636b 2061 2073 6563 7572  nds back a secur
+00009d60: 6974 7920 746f 6b65 6e20 7769 7468 2077  ity token with w
+00009d70: 6869 6368 2074 6865 2064 7269 7665 7220  hich the driver 
+00009d80: 6361 6e20 636f 6e6e 6563 742e 2028 5573  can connect. (Us
+00009d90: 6564 2066 6f72 2072 6564 6972 6563 7469  ed for redirecti
+00009da0: 6e67 202f 2072 6563 6f6e 6e65 6374 696e  ng / reconnectin
+00009db0: 6729 0a20 2020 2020 2020 2022 2222 0a20  g).        """. 
+00009dc0: 2020 2020 2020 2066 726f 6d20 7765 6262         from webb
+00009dd0: 726f 7773 6572 2069 6d70 6f72 7420 6f70  rowser import op
+00009de0: 656e 5f6e 6577 0a0a 2020 2020 2020 2020  en_new..        
+00009df0: 7265 7120 3d20 7072 6f74 6f2e 5265 7175  req = proto.Requ
+00009e00: 6573 7428 290a 2020 2020 2020 2020 7265  est().        re
+00009e10: 712e 7479 7065 203d 2072 6571 2e43 4c49  q.type = req.CLI
+00009e20: 454e 545f 434f 4e4e 4543 5449 4f4e 5f53  ENT_CONNECTION_S
+00009e30: 534f 0a20 2020 2020 2020 2063 6c69 656e  SO.        clien
+00009e40: 745f 636f 6e6e 6563 7469 6f6e 203d 2072  t_connection = r
+00009e50: 6571 2e63 6c69 656e 745f 636f 6e6e 6563  eq.client_connec
+00009e60: 7469 6f6e 5f73 736f 0a0a 2020 2020 2020  tion_sso..      
+00009e70: 2020 7365 6c66 2e5f 696e 6974 6961 6c69    self._initiali
+00009e80: 7a65 5f63 6c69 656e 745f 636f 6e6e 6563  ze_client_connec
+00009e90: 7469 6f6e 2863 6c69 656e 745f 636f 6e6e  tion(client_conn
+00009ea0: 6563 7469 6f6e 290a 2020 2020 2020 2020  ection).        
+00009eb0: 2320 5365 6e64 206d 6573 7361 6765 0a20  # Send message. 
+00009ec0: 2020 2020 2020 205f 7365 6e64 5f6d 7367         _send_msg
+00009ed0: 2873 656c 662c 2072 6571 290a 2020 2020  (self, req).    
+00009ee0: 2020 2020 2320 5265 6365 6976 6520 7265      # Receive re
+00009ef0: 7370 6f6e 7365 0a20 2020 2020 2020 2072  sponse.        r
+00009f00: 7370 203d 205f 7265 6376 5f6d 7367 2873  sp = _recv_msg(s
+00009f10: 656c 662c 2070 726f 746f 2e43 6c69 656e  elf, proto.Clien
+00009f20: 7443 6f6e 6e65 6374 696f 6e53 534f 5265  tConnectionSSORe
+00009f30: 7370 6f6e 7365 2829 290a 0a20 2020 2020  sponse())..     
+00009f40: 2020 2069 6620 7273 702e 7265 7370 6f6e     if rsp.respon
+00009f50: 7365 2e74 7970 6520 3d3d 2070 726f 746f  se.type == proto
+00009f60: 2e43 6f6e 6669 726d 6174 696f 6e52 6573  .ConfirmationRes
+00009f70: 706f 6e73 652e 5245 5350 4f4e 5345 5f57  ponse.RESPONSE_W
+00009f80: 4152 4e3a 0a20 2020 2020 2020 2020 2020  ARN:.           
+00009f90: 2077 6172 6e28 7273 702e 7265 7370 6f6e   warn(rsp.respon
+00009fa0: 7365 2e72 6561 736f 6e29 0a20 2020 2020  se.reason).     
+00009fb0: 2020 2065 6c69 6620 6e6f 7420 7273 702e     elif not rsp.
+00009fc0: 7265 7370 6f6e 7365 2e74 7970 6520 3d3d  response.type ==
+00009fd0: 2070 726f 746f 2e43 6f6e 6669 726d 6174   proto.Confirmat
+00009fe0: 696f 6e52 6573 706f 6e73 652e 5245 5350  ionResponse.RESP
+00009ff0: 4f4e 5345 5f4f 4b3a 0a20 2020 2020 2020  ONSE_OK:.       
+0000a000: 2020 2020 2072 6169 7365 205f 636f 6e76       raise _conv
+0000a010: 6572 745f 6578 6365 7074 696f 6e28 7273  ert_exception(rs
+0000a020: 702e 7265 7370 6f6e 7365 290a 0a20 2020  p.response)..   
+0000a030: 2020 2020 2023 204f 7065 6e20 6272 6f77       # Open brow
+0000a040: 7365 7220 666f 7220 7573 6572 2074 6f20  ser for user to 
+0000a050: 6175 7468 656e 7469 6361 7465 2e0a 2020  authenticate..  
+0000a060: 2020 2020 2020 6966 206e 6f74 206f 7065        if not ope
+0000a070: 6e5f 6e65 7728 7273 702e 6175 7468 5572  n_new(rsp.authUr
+0000a080: 6c29 3a0a 2020 2020 2020 2020 2020 2020  l):.            
+0000a090: 6c6f 6767 6572 2e69 6e66 6f28 0a20 2020  logger.info(.   
+0000a0a0: 2020 2020 2020 2020 2020 2020 2022 5b70               "[p
+0000a0b0: 796f 6369 656e 745d 2043 6f75 6c64 206e  yocient] Could n
+0000a0c0: 6f74 206f 7065 6e20 6465 6661 756c 7420  ot open default 
+0000a0d0: 6272 6f77 7365 7220 7769 7468 2077 6562  browser with web
+0000a0e0: 6272 6f77 7365 7220 6c69 6272 6172 792e  browser library.
+0000a0f0: 2050 6c65 6173 6520 6175 7468 656e 7469   Please authenti
+0000a100: 6361 7465 2061 743a 2022 0a20 2020 2020  cate at: ".     
+0000a110: 2020 2020 2020 2020 2020 202b 2072 7370             + rsp
+0000a120: 2e61 7574 6855 726c 0a20 2020 2020 2020  .authUrl.       
+0000a130: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000a140: 2020 2070 7269 6e74 280a 2020 2020 2020     print(.      
+0000a150: 2020 2020 2020 2020 2020 225b 7079 6f63            "[pyoc
+0000a160: 6965 6e74 5d20 436f 756c 6420 6e6f 7420  ient] Could not 
+0000a170: 6f70 656e 2064 6566 6175 6c74 2062 726f  open default bro
+0000a180: 7773 6572 2077 6974 6820 7765 6262 726f  wser with webbro
+0000a190: 7773 6572 206c 6962 7261 7279 2e20 506c  wser library. Pl
+0000a1a0: 6561 7365 2061 7574 6865 6e74 6963 6174  ease authenticat
+0000a1b0: 6520 6174 3a20 222c 0a20 2020 2020 2020  e at: ",.       
+0000a1c0: 2020 2020 2020 2020 2072 7370 2e61 7574           rsp.aut
+0000a1d0: 6855 726c 2c0a 2020 2020 2020 2020 2020  hUrl,.          
+0000a1e0: 2020 290a 0a20 2020 2020 2020 2023 2050    )..        # P
+0000a1f0: 6f6c 6c20 7468 6520 6461 7461 6261 7365  oll the database
+0000a200: 0a20 2020 2020 2020 2073 656c 662e 5f70  .        self._p
+0000a210: 6f6c 6c5f 6461 7461 6261 7365 2872 7370  oll_database(rsp
+0000a220: 2e72 6571 7565 7374 4964 290a 0a20 2020  .requestId)..   
+0000a230: 2064 6566 205f 706f 6c6c 5f64 6174 6162   def _poll_datab
+0000a240: 6173 6528 7365 6c66 2c20 7265 7175 6573  ase(self, reques
+0000a250: 7449 643a 2073 7472 2920 2d3e 204e 6f6e  tId: str) -> Non
+0000a260: 653a 0a20 2020 2020 2020 2022 2222 506f  e:.        """Po
+0000a270: 6c6c 7320 7468 6520 6461 7461 6261 7365  lls the database
+0000a280: 2075 6e74 696c 2077 6520 6569 7468 6572   until we either
+0000a290: 2072 6563 6569 7665 2061 6e20 6572 726f   receive an erro
+0000a2a0: 7220 6f72 2061 2073 7563 6365 7373 6675  r or a successfu
+0000a2b0: 6c20 6c6f 6769 6e20 6d65 7373 6167 652e  l login message.
+0000a2c0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+0000a2d0: 2020 2020 2020 2020 2020 2020 7265 7175              requ
+0000a2e0: 6573 7449 6420 2853 7472 696e 6729 3a20  estId (String): 
+0000a2f0: 7468 6520 7265 7175 6573 7420 4944 2061  the request ID a
+0000a300: 7373 6f63 6961 7465 6420 7769 7468 2074  ssociated with t
+0000a310: 6869 7320 6c6f 6769 6e20 6174 7465 6d70  his login attemp
+0000a320: 742e 0a20 2020 2020 2020 2022 2222 0a0a  t..        """..
+0000a330: 2020 2020 2020 2020 7265 7120 3d20 7072          req = pr
+0000a340: 6f74 6f2e 5265 7175 6573 7428 290a 2020  oto.Request().  
+0000a350: 2020 2020 2020 7265 712e 7479 7065 203d        req.type =
+0000a360: 2072 6571 2e43 4c49 454e 545f 434f 4e4e   req.CLIENT_CONN
+0000a370: 4543 5449 4f4e 5f53 534f 320a 2020 2020  ECTION_SSO2.    
+0000a380: 2020 2020 6173 7365 7274 2073 656c 662e      assert self.
+0000a390: 666f 7263 6520 6973 206e 6f74 204e 6f6e  force is not Non
+0000a3a0: 650a 2020 2020 2020 2020 7265 712e 636c  e.        req.cl
+0000a3b0: 6965 6e74 5f63 6f6e 6e65 6374 696f 6e5f  ient_connection_
+0000a3c0: 7373 6f32 2e66 6f72 6365 203d 2073 656c  sso2.force = sel
+0000a3d0: 662e 666f 7263 650a 2020 2020 2020 2020  f.force.        
+0000a3e0: 7265 712e 636c 6965 6e74 5f63 6f6e 6e65  req.client_conne
+0000a3f0: 6374 696f 6e5f 7373 6f32 2e72 6571 7565  ction_sso2.reque
+0000a400: 7374 4964 203d 2072 6571 7565 7374 4964  stId = requestId
+0000a410: 0a0a 2020 2020 2020 2020 6b65 6570 506f  ..        keepPo
+0000a420: 6c6c 696e 6720 3d20 5472 7565 0a20 2020  lling = True.   
+0000a430: 2020 2020 2077 6169 7446 6f72 203d 2030       waitFor = 0
+0000a440: 0a20 2020 2020 2020 2077 6869 6c65 206b  .        while k
+0000a450: 6565 7050 6f6c 6c69 6e67 3a0a 2020 2020  eepPolling:.    
+0000a460: 2020 2020 2020 2020 736c 6565 7028 7761          sleep(wa
+0000a470: 6974 466f 7229 0a20 2020 2020 2020 2020  itFor).         
+0000a480: 2020 2023 2050 6f6c 6c0a 2020 2020 2020     # Poll.      
+0000a490: 2020 2020 2020 5f73 656e 645f 6d73 6728        _send_msg(
+0000a4a0: 7365 6c66 2c20 7265 7129 0a0a 2020 2020  self, req)..    
+0000a4b0: 2020 2020 2020 2020 2320 5265 6365 6976          # Receiv
+0000a4c0: 6520 7265 7370 6f6e 7365 0a20 2020 2020  e response.     
+0000a4d0: 2020 2020 2020 2072 7370 203d 205f 7265         rsp = _re
+0000a4e0: 6376 5f6d 7367 2873 656c 662c 2070 726f  cv_msg(self, pro
+0000a4f0: 746f 2e43 6c69 656e 7443 6f6e 6e65 6374  to.ClientConnect
+0000a500: 696f 6e53 534f 3252 6573 706f 6e73 6528  ionSSO2Response(
+0000a510: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
+0000a520: 6966 2072 7370 2e72 6573 706f 6e73 652e  if rsp.response.
+0000a530: 7479 7065 203d 3d20 7072 6f74 6f2e 436f  type == proto.Co
+0000a540: 6e66 6972 6d61 7469 6f6e 5265 7370 6f6e  nfirmationRespon
+0000a550: 7365 2e52 4553 504f 4e53 455f 5741 524e  se.RESPONSE_WARN
+0000a560: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000a570: 2020 7761 726e 2872 7370 2e72 6573 706f    warn(rsp.respo
+0000a580: 6e73 652e 7265 6173 6f6e 290a 2020 2020  nse.reason).    
+0000a590: 2020 2020 2020 2020 656c 6966 206e 6f74          elif not
+0000a5a0: 2072 7370 2e72 6573 706f 6e73 652e 7479   rsp.response.ty
+0000a5b0: 7065 203d 3d20 7072 6f74 6f2e 436f 6e66  pe == proto.Conf
+0000a5c0: 6972 6d61 7469 6f6e 5265 7370 6f6e 7365  irmationResponse
+0000a5d0: 2e52 4553 504f 4e53 455f 4f4b 3a0a 2020  .RESPONSE_OK:.  
+0000a5e0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+0000a5f0: 6973 6520 5f63 6f6e 7665 7274 5f65 7863  ise _convert_exc
+0000a600: 6570 7469 6f6e 2872 7370 2e72 6573 706f  eption(rsp.respo
+0000a610: 6e73 6529 0a0a 2020 2020 2020 2020 2020  nse)..          
+0000a620: 2020 6966 2072 7370 2e48 6173 4669 656c    if rsp.HasFiel
+0000a630: 6428 2270 6f6c 6c69 6e67 496e 7465 7276  d("pollingInterv
+0000a640: 616c 5365 636f 6e64 7322 293a 0a20 2020  alSeconds"):.   
+0000a650: 2020 2020 2020 2020 2020 2020 2023 2043               # C
+0000a660: 6f6e 7469 6e75 6520 706f 6c6c 696e 670a  ontinue polling.
+0000a670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a680: 7761 6974 466f 7220 3d20 7273 702e 706f  waitFor = rsp.po
+0000a690: 6c6c 696e 6749 6e74 6572 7661 6c53 6563  llingIntervalSec
+0000a6a0: 6f6e 6473 0a20 2020 2020 2020 2020 2020  onds.           
+0000a6b0: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
+0000a6c0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0000a6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6e0: 2320 5375 6363 6573 730a 2020 2020 2020  # Success.      
+0000a6f0: 2020 2020 2020 2020 2020 7761 6974 466f            waitFo
+0000a700: 7220 3d20 300a 2020 2020 2020 2020 2020  r = 0.          
+0000a710: 2020 2020 2020 6b65 6570 506f 6c6c 696e        keepPollin
+0000a720: 6720 3d20 4661 6c73 650a 0a20 2020 2020  g = False..     
+0000a730: 2020 2073 656c 662e 7365 7276 6572 5365     self.serverSe
+0000a740: 7373 696f 6e49 6420 3d20 7273 702e 7365  ssionId = rsp.se
+0000a750: 7373 696f 6e49 6e66 6f2e 7365 7276 6572  ssionInfo.server
+0000a760: 5365 7373 696f 6e49 640a 2020 2020 2020  SessionId.      
+0000a770: 2020 6c6f 6767 6572 2e64 6562 7567 2866    logger.debug(f
+0000a780: 2243 6f6e 6e65 6374 6564 2074 6f20 7365  "Connected to se
+0000a790: 7276 6572 2073 6573 7369 6f6e 2049 643a  rver session Id:
+0000a7a0: 207b 7365 6c66 2e73 6572 7665 7253 6573   {self.serverSes
+0000a7b0: 7369 6f6e 4964 7d22 290a 2020 2020 2020  sionId}").      
+0000a7c0: 2020 7265 6365 6976 6564 5f74 6f6b 656e    received_token
+0000a7d0: 203d 2072 7370 2e73 6573 7369 6f6e 496e   = rsp.sessionIn
+0000a7e0: 666f 2e73 6563 7572 6974 7954 6f6b 656e  fo.securityToken
+0000a7f0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+0000a800: 7373 696f 6e20 3d20 5365 7373 696f 6e28  ssion = Session(
+0000a810: 0a20 2020 2020 2020 2020 2020 2073 6563  .            sec
+0000a820: 7572 6974 7954 6f6b 656e 3d53 6563 7572  urityToken=Secur
+0000a830: 6974 7954 6f6b 656e 280a 2020 2020 2020  ityToken(.      
+0000a840: 2020 2020 2020 2020 2020 7265 6365 6976            receiv
+0000a850: 6564 5f74 6f6b 656e 2e64 6174 612c 0a20  ed_token.data,. 
+0000a860: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000a870: 6563 6569 7665 645f 746f 6b65 6e2e 7369  eceived_token.si
+0000a880: 676e 6174 7572 652c 0a20 2020 2020 2020  gnature,.       
+0000a890: 2020 2020 2020 2020 2072 6563 6569 7665           receive
+0000a8a0: 645f 746f 6b65 6e2e 6973 7375 6572 4669  d_token.issuerFi
+0000a8b0: 6e67 6572 7072 696e 742c 0a20 2020 2020  ngerprint,.     
+0000a8c0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000a8d0: 2029 0a0a 2020 2020 2020 2020 2320 5361   )..        # Sa
+0000a8e0: 7665 2073 6563 6f6e 6461 7279 2069 6e74  ve secondary int
+0000a8f0: 6572 6661 6365 732e 0a20 2020 2020 2020  erfaces..       
+0000a900: 2073 656c 662e 5f73 6176 655f 7365 636f   self._save_seco
+0000a910: 6e64 6172 795f 696e 7465 7266 6163 6573  ndary_interfaces
+0000a920: 2872 7370 2e73 6563 6f6e 6461 7279 290a  (rsp.secondary).
+0000a930: 0a20 2020 2020 2020 2023 2052 6564 6972  .        # Redir
+0000a940: 6563 7420 7468 6520 636f 6e6e 6563 7469  ect the connecti
+0000a950: 6f6e 0a20 2020 2020 2020 2069 6620 7273  on.        if rs
+0000a960: 702e 7265 6469 7265 6374 3a0a 2020 2020  p.redirect:.    
+0000a970: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
+0000a980: 656c 662e 736f 636b 2069 7320 6e6f 7420  elf.sock is not 
+0000a990: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+0000a9a0: 2073 656c 662e 736f 636b 2e63 6c6f 7365   self.sock.close
+0000a9b0: 2829 0a20 2020 2020 2020 2020 2020 206d  ().            m
+0000a9c0: 6170 7065 645f 686f 7374 2c20 6d61 7070  apped_host, mapp
+0000a9d0: 6564 5f70 6f72 7420 3d20 7365 6c66 2e72  ed_port = self.r
+0000a9e0: 6573 6f6c 7665 5f6e 6577 5f65 6e64 706f  esolve_new_endpo
+0000a9f0: 696e 7428 7273 702e 7265 6469 7265 6374  int(rsp.redirect
+0000aa00: 486f 7374 2c20 7273 702e 7265 6469 7265  Host, rsp.redire
+0000aa10: 6374 506f 7274 290a 2020 2020 2020 2020  ctPort).        
+0000aa20: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0000aa30: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000aa40: 2020 6622 5265 6469 7265 6374 696e 6720    f"Redirecting 
+0000aa50: 636f 6e6e 6563 7469 6f6e 2074 6f20 7b72  connection to {r
+0000aa60: 7370 2e72 6564 6972 6563 7448 6f73 747d  sp.redirectHost}
+0000aa70: 3a7b 7273 702e 7265 6469 7265 6374 506f  :{rsp.redirectPo
+0000aa80: 7274 7d2c 2077 6869 6368 206d 6170 7320  rt}, which maps 
+0000aa90: 746f 207b 6d61 7070 6564 5f68 6f73 747d  to {mapped_host}
+0000aaa0: 3a7b 6d61 7070 6564 5f70 6f72 747d 220a  :{mapped_port}".
+0000aab0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000aac0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0000aad0: 6f63 6b20 3d20 736f 636b 6574 2e63 7265  ock = socket.cre
+0000aae0: 6174 655f 636f 6e6e 6563 7469 6f6e 2828  ate_connection((
+0000aaf0: 6d61 7070 6564 5f68 6f73 742c 206d 6170  mapped_host, map
+0000ab00: 7065 645f 706f 7274 2929 0a20 2020 2020  ped_port)).     
+0000ab10: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+0000ab20: 666f 2866 2243 6f6e 6e65 6374 6564 2074  fo(f"Connected t
+0000ab30: 6f20 7b6d 6170 7065 645f 686f 7374 7d3a  o {mapped_host}:
+0000ab40: 7b6d 6170 7065 645f 706f 7274 7d20 6f6e  {mapped_port} on
+0000ab50: 2073 6f63 6b65 7420 7b73 656c 662e 736f   socket {self.so
+0000ab60: 636b 7d22 290a 2020 2020 2020 2020 2020  ck}").          
+0000ab70: 2020 7365 6c66 2e5f 7373 6c69 7a65 5f63    self._sslize_c
+0000ab80: 6f6e 6e65 6374 696f 6e28 290a 0a20 2020  onnection()..   
+0000ab90: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000aba0: 7365 6c66 2e5f 636c 6965 6e74 5f68 616e  self._client_han
+0000abb0: 6473 6861 6b65 5f73 6563 7572 6974 795f  dshake_security_
+0000abc0: 746f 6b65 6e28 5472 7565 290a 0a20 2020  token(True)..   
+0000abd0: 2064 6566 205f 636c 6965 6e74 5f68 616e   def _client_han
+0000abe0: 6473 6861 6b65 5f73 6563 7572 6974 795f  dshake_security_
+0000abf0: 746f 6b65 6e28 7365 6c66 2c20 666f 7263  token(self, forc
+0000ac00: 653a 2062 6f6f 6c20 3d20 4661 6c73 6529  e: bool = False)
+0000ac10: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+0000ac20: 2020 2222 224f 6e63 6520 6120 636f 6e6e    """Once a conn
+0000ac30: 6563 7469 6f6e 2061 6371 7569 7265 7320  ection acquires 
+0000ac40: 6120 7365 6375 7269 7479 2074 6f6b 656e  a security token
+0000ac50: 2c20 6974 2063 616e 2075 7365 2074 6861  , it can use tha
+0000ac60: 7420 746f 206c 6f67 2069 6e2e 2054 6869  t to log in. Thi
+0000ac70: 7320 6861 6e64 7368 616b 6520 6f6e 6c79  s handshake only
+0000ac80: 0a20 2020 2020 2020 2073 656e 6473 2031  .        sends 1
+0000ac90: 206d 6573 7361 6765 2077 6865 7265 6173   message whereas
+0000aca0: 2074 6865 206f 7468 6572 2068 616e 6473   the other hands
+0000acb0: 6861 6b65 7320 7365 6e64 2032 2e20 7365  hakes send 2. se
+0000acc0: 6c66 2e73 6573 7369 6f6e 2e73 6563 7572  lf.session.secur
+0000acd0: 6974 7954 6f6b 656e 206d 7573 7420 6265  ityToken must be
+0000ace0: 2073 6574 2e0a 2020 2020 2020 2020 2222   set..        ""
+0000acf0: 220a 2020 2020 2020 2020 7768 696c 6520  ".        while 
+0000ad00: 5472 7565 3a0a 2020 2020 2020 2020 2020  True:.          
+0000ad10: 2020 7265 7120 3d20 7072 6f74 6f2e 5265    req = proto.Re
+0000ad20: 7175 6573 7428 290a 2020 2020 2020 2020  quest().        
+0000ad30: 2020 2020 7265 712e 7479 7065 203d 2072      req.type = r
+0000ad40: 6571 2e43 4c49 454e 545f 434f 4e4e 4543  eq.CLIENT_CONNEC
+0000ad50: 5449 4f4e 5f53 4543 5552 4954 595f 544f  TION_SECURITY_TO
+0000ad60: 4b45 4e0a 2020 2020 2020 2020 2020 2020  KEN.            
+0000ad70: 636c 6965 6e74 5f63 6f6e 6e65 6374 696f  client_connectio
+0000ad80: 6e20 3d20 7265 712e 636c 6965 6e74 5f63  n = req.client_c
+0000ad90: 6f6e 6e65 6374 696f 6e5f 7365 6375 7269  onnection_securi
+0000ada0: 7479 5f74 6f6b 656e 0a0a 2020 2020 2020  ty_token..      
+0000adb0: 2020 2020 2020 7365 6c66 2e5f 696e 6974        self._init
+0000adc0: 6961 6c69 7a65 5f63 6c69 656e 745f 636f  ialize_client_co
+0000add0: 6e6e 6563 7469 6f6e 2863 6c69 656e 745f  nnection(client_
+0000ade0: 636f 6e6e 6563 7469 6f6e 290a 2020 2020  connection).    
+0000adf0: 2020 2020 2020 2020 2320 4174 7461 6368          # Attach
+0000ae00: 2074 6865 2073 6563 7572 6974 7920 746f   the security to
+0000ae10: 6b65 6e20 7573 6564 2074 6f20 6c6f 6720  ken used to log 
+0000ae20: 696e 0a20 2020 2020 2020 2020 2020 2061  in.            a
+0000ae30: 7373 6572 7420 7365 6c66 2e73 6573 7369  ssert self.sessi
+0000ae40: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 0a20  on is not None. 
+0000ae50: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+0000ae60: 7420 7365 6c66 2e73 6573 7369 6f6e 2e73  t self.session.s
+0000ae70: 6563 7572 6974 7954 6f6b 656e 2069 7320  ecurityToken is 
+0000ae80: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
+0000ae90: 2020 2020 2063 6c69 656e 745f 636f 6e6e       client_conn
+0000aea0: 6563 7469 6f6e 2e73 6563 7572 6974 7954  ection.securityT
+0000aeb0: 6f6b 656e 203d 2073 656c 662e 7365 7373  oken = self.sess
+0000aec0: 696f 6e2e 7365 6375 7269 7479 546f 6b65  ion.securityToke
+0000aed0: 6e2e 746f 6b65 6e44 6174 610a 2020 2020  n.tokenData.    
+0000aee0: 2020 2020 2020 2020 636c 6965 6e74 5f63          client_c
+0000aef0: 6f6e 6e65 6374 696f 6e2e 746f 6b65 6e53  onnection.tokenS
+0000af00: 6967 6e61 7475 7265 203d 2073 656c 662e  ignature = self.
+0000af10: 7365 7373 696f 6e2e 7365 6375 7269 7479  session.security
+0000af20: 546f 6b65 6e2e 746f 6b65 6e53 6967 6e61  Token.tokenSigna
+0000af30: 7475 7265 0a20 2020 2020 2020 2020 2020  ture.           
+0000af40: 2063 6c69 656e 745f 636f 6e6e 6563 7469   client_connecti
+0000af50: 6f6e 2e69 7373 7565 7246 696e 6765 7270  on.issuerFingerp
+0000af60: 7269 6e74 203d 2073 656c 662e 7365 7373  rint = self.sess
+0000af70: 696f 6e2e 7365 6375 7269 7479 546f 6b65  ion.securityToke
+0000af80: 6e2e 6973 7375 6572 4669 6e67 6572 7072  n.issuerFingerpr
+0000af90: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
+0000afa0: 636c 6965 6e74 5f63 6f6e 6e65 6374 696f  client_connectio
+0000afb0: 6e2e 666f 7263 6520 3d20 666f 7263 650a  n.force = force.
+0000afc0: 0a20 2020 2020 2020 2020 2020 205f 7365  .            _se
+0000afd0: 6e64 5f6d 7367 2873 656c 662c 2072 6571  nd_msg(self, req
+0000afe0: 290a 0a20 2020 2020 2020 2020 2020 2072  )..            r
+0000aff0: 7370 203d 205f 7265 6376 5f6d 7367 2873  sp = _recv_msg(s
+0000b000: 656c 662c 2070 726f 746f 2e43 6c69 656e  elf, proto.Clien
+0000b010: 7443 6f6e 6e65 6374 696f 6e53 6563 7572  tConnectionSecur
+0000b020: 6974 7954 6f6b 656e 5265 7370 6f6e 7365  ityTokenResponse
+0000b030: 2829 290a 0a20 2020 2020 2020 2020 2020  ())..           
+0000b040: 2069 6620 7273 702e 7265 7370 6f6e 7365   if rsp.response
+0000b050: 2e74 7970 6520 3d3d 2070 726f 746f 2e43  .type == proto.C
+0000b060: 6f6e 6669 726d 6174 696f 6e52 6573 706f  onfirmationRespo
+0000b070: 6e73 652e 5245 5350 4f4e 5345 5f57 4152  nse.RESPONSE_WAR
+0000b080: 4e3a 0a20 2020 2020 2020 2020 2020 2020  N:.             
+0000b090: 2020 2077 6172 6e28 7273 702e 7265 7370     warn(rsp.resp
+0000b0a0: 6f6e 7365 2e72 6561 736f 6e29 0a20 2020  onse.reason).   
+0000b0b0: 2020 2020 2020 2020 2065 6c69 6620 7273           elif rs
+0000b0c0: 702e 7265 7370 6f6e 7365 2e74 7970 6520  p.response.type 
+0000b0d0: 3d3d 2070 726f 746f 2e43 6f6e 6669 726d  == proto.Confirm
+0000b0e0: 6174 696f 6e52 6573 706f 6e73 652e 5245  ationResponse.RE
+0000b0f0: 5350 4f4e 5345 5f4f 4b3a 0a20 2020 2020  SPONSE_OK:.     
+0000b100: 2020 2020 2020 2020 2020 2023 2053 6176             # Sav
+0000b110: 6520 7365 636f 6e64 6172 7920 696e 7465  e secondary inte
+0000b120: 7266 6163 6573 2e0a 2020 2020 2020 2020  rfaces..        
+0000b130: 2020 2020 2020 2020 7365 6c66 2e5f 7361          self._sa
+0000b140: 7665 5f73 6563 6f6e 6461 7279 5f69 6e74  ve_secondary_int
+0000b150: 6572 6661 6365 7328 7273 702e 7365 636f  erfaces(rsp.seco
+0000b160: 6e64 6172 7929 0a20 2020 2020 2020 2020  ndary).         
+0000b170: 2020 2020 2020 2023 2052 6564 6972 6563         # Redirec
+0000b180: 7420 7468 6520 636f 6e6e 6563 7469 6f6e  t the connection
+0000b190: 2069 6620 7265 7175 6573 7465 640a 2020   if requested.  
+0000b1a0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000b1b0: 2072 7370 2e72 6564 6972 6563 743a 0a20   rsp.redirect:. 
+0000b1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1d0: 2020 2061 7373 6572 7420 7365 6c66 2e73     assert self.s
+0000b1e0: 6f63 6b20 6973 206e 6f74 204e 6f6e 650a  ock is not None.
+0000b1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b200: 2020 2020 7365 6c66 2e73 6f63 6b2e 636c      self.sock.cl
+0000b210: 6f73 6528 290a 2020 2020 2020 2020 2020  ose().          
+0000b220: 2020 2020 2020 2020 2020 6d61 7070 6564            mapped
+0000b230: 5f68 6f73 742c 206d 6170 7065 645f 706f  _host, mapped_po
+0000b240: 7274 203d 2073 656c 662e 7265 736f 6c76  rt = self.resolv
+0000b250: 655f 6e65 775f 656e 6470 6f69 6e74 2872  e_new_endpoint(r
+0000b260: 7370 2e72 6564 6972 6563 7448 6f73 742c  sp.redirectHost,
+0000b270: 2072 7370 2e72 6564 6972 6563 7450 6f72   rsp.redirectPor
+0000b280: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
+0000b290: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+0000b2a0: 6275 6728 0a20 2020 2020 2020 2020 2020  bug(.           
+0000b2b0: 2020 2020 2020 2020 2020 2020 2066 2252               f"R
+0000b2c0: 6564 6972 6563 7469 6e67 2063 6f6e 6e65  edirecting conne
+0000b2d0: 6374 696f 6e20 746f 207b 7273 702e 7265  ction to {rsp.re
+0000b2e0: 6469 7265 6374 486f 7374 7d3a 7b72 7370  directHost}:{rsp
+0000b2f0: 2e72 6564 6972 6563 7450 6f72 747d 2c20  .redirectPort}, 
+0000b300: 7768 6963 6820 6d61 7073 2074 6f20 7b6d  which maps to {m
+0000b310: 6170 7065 645f 686f 7374 7d3a 7b6d 6170  apped_host}:{map
+0000b320: 7065 645f 706f 7274 7d22 0a20 2020 2020  ped_port}".     
+0000b330: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000b340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b350: 2020 2020 2073 656c 662e 736f 636b 203d       self.sock =
+0000b360: 2073 6f63 6b65 742e 6372 6561 7465 5f63   socket.create_c
+0000b370: 6f6e 6e65 6374 696f 6e28 286d 6170 7065  onnection((mappe
+0000b380: 645f 686f 7374 2c20 6d61 7070 6564 5f70  d_host, mapped_p
+0000b390: 6f72 7429 290a 2020 2020 2020 2020 2020  ort)).          
+0000b3a0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+0000b3b0: 2e69 6e66 6f28 6622 436f 6e6e 6563 7465  .info(f"Connecte
+0000b3c0: 6420 746f 207b 6d61 7070 6564 5f68 6f73  d to {mapped_hos
+0000b3d0: 747d 3a7b 6d61 7070 6564 5f70 6f72 747d  t}:{mapped_port}
+0000b3e0: 206f 6e20 736f 636b 6574 207b 7365 6c66   on socket {self
+0000b3f0: 2e73 6f63 6b7d 2229 0a20 2020 2020 2020  .sock}").       
+0000b400: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000b410: 662e 5f73 736c 697a 655f 636f 6e6e 6563  f._sslize_connec
+0000b420: 7469 6f6e 2829 0a0a 2020 2020 2020 2020  tion()..        
+0000b430: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000b440: 726e 2073 656c 662e 5f63 6c69 656e 745f  rn self._client_
+0000b450: 6861 6e64 7368 616b 655f 7365 6375 7269  handshake_securi
+0000b460: 7479 5f74 6f6b 656e 2854 7275 6529 0a0a  ty_token(True)..
+0000b470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b480: 2320 4361 7074 7572 6520 7468 6520 7365  # Capture the se
+0000b490: 7373 696f 6e20 6964 0a20 2020 2020 2020  ssion id.       
+0000b4a0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+0000b4b0: 7276 6572 5365 7373 696f 6e49 6420 3d20  rverSessionId = 
+0000b4c0: 7273 702e 7365 7276 6572 5365 7373 696f  rsp.serverSessio
+0000b4d0: 6e49 640a 2020 2020 2020 2020 2020 2020  nId.            
+0000b4e0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0000b4f0: 2866 2243 6f6e 6e65 6374 6564 2074 6f20  (f"Connected to 
+0000b500: 7365 7276 6572 2073 6573 7369 6f6e 2049  server session I
+0000b510: 643a 207b 7365 6c66 2e73 6572 7665 7253  d: {self.serverS
+0000b520: 6573 7369 6f6e 4964 7d22 290a 2020 2020  essionId}").    
+0000b530: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+0000b540: 6b0a 2020 2020 2020 2020 2020 2020 2320  k.            # 
+0000b550: 7468 6572 6520 6973 2073 6f6d 6574 6869  there is somethi
+0000b560: 6e67 2062 726f 6b65 6e20 696e 206f 7572  ng broken in our
+0000b570: 2068 616e 6473 6861 6b65 2e2e 2e72 6574   handshake...ret
+0000b580: 7279 0a20 2020 2020 2020 2020 2020 2069  ry.            i
+0000b590: 6620 7273 702e 7265 7370 6f6e 7365 2e76  f rsp.response.v
+0000b5a0: 656e 646f 725f 636f 6465 203d 3d20 2d32  endor_code == -2
+0000b5b0: 3032 3a0a 2020 2020 2020 2020 2020 2020  02:.            
+0000b5c0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0000b5d0: 2822 4861 6e64 7368 616b 6520 6572 726f  ("Handshake erro
+0000b5e0: 722e 2e2e 7265 7472 7969 6e67 2229 0a20  r...retrying"). 
+0000b5f0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000b600: 6f6e 7469 6e75 650a 0a20 2020 2020 2020  ontinue..       
+0000b610: 2020 2020 2072 6169 7365 205f 636f 6e76       raise _conv
+0000b620: 6572 745f 6578 6365 7074 696f 6e28 7273  ert_exception(rs
+0000b630: 702e 7265 7370 6f6e 7365 290a 0a20 2020  p.response)..   
+0000b640: 2064 6566 205f 7361 7665 5f73 6563 6f6e   def _save_secon
+0000b650: 6461 7279 5f69 6e74 6572 6661 6365 7328  dary_interfaces(
+0000b660: 0a20 2020 2020 2020 2073 656c 662c 206e  .        self, n
+0000b670: 6577 5f73 6563 6f6e 6461 7279 5f69 6e74  ew_secondary_int
+0000b680: 6572 6661 6365 733a 2052 6570 6561 7465  erfaces: Repeate
+0000b690: 6443 6f6d 706f 7369 7465 4669 656c 6443  dCompositeFieldC
+0000b6a0: 6f6e 7461 696e 6572 5b70 726f 746f 2e53  ontainer[proto.S
+0000b6b0: 6563 6f6e 6461 7279 496e 7465 7266 6163  econdaryInterfac
+0000b6c0: 654c 6973 745d 0a20 2020 2029 202d 3e20  eList].    ) -> 
+0000b6d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+0000b6e0: 2241 6674 6572 2073 6563 6f6e 6461 7279  "After secondary
+0000b6f0: 2069 6e74 6572 6661 6365 7320 6172 6520   interfaces are 
+0000b700: 7365 6e74 2066 726f 6d20 7468 6520 7365  sent from the se
+0000b710: 7276 6572 2c20 7765 206e 6565 6420 746f  rver, we need to
+0000b720: 0a20 2020 2020 2020 2073 6176 6520 7468  .        save th
+0000b730: 656d 2061 6e64 2075 7365 2074 6865 6d20  em and use them 
+0000b740: 666f 7220 7265 6469 7265 6374 696e 672e  for redirecting.
+0000b750: 2054 6869 7320 6973 2069 6d70 6f72 7461   This is importa
+0000b760: 6e74 2069 6620 7765 0a20 2020 2020 2020  nt if we.       
+0000b770: 2067 6574 2072 6564 6972 6563 7465 6420   get redirected 
+0000b780: 746f 206d 6170 7065 6420 7371 6c20 656e  to mapped sql en
+0000b790: 6470 6f69 6e74 732e 0a0a 2020 2020 2020  dpoints...      
+0000b7a0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+0000b7b0: 2020 2020 7365 636f 6e64 6172 795f 696e      secondary_in
+0000b7c0: 7465 7266 6163 6573 2028 5b63 6c61 7373  terfaces ([class
+0000b7d0: 2027 676f 6f67 6c65 2e70 726f 746f 6275   'google.protobu
+0000b7e0: 662e 696e 7465 726e 616c 2e63 6f6e 7461  f.internal.conta
+0000b7f0: 696e 6572 732e 5265 7065 6174 6564 436f  iners.RepeatedCo
+0000b800: 6d70 6f73 6974 6543 6f6e 7461 696e 6572  mpositeContainer
+0000b810: 275d 293a 0a20 2020 2020 2020 2020 2020  ']):.           
+0000b820: 2074 6865 2073 6563 6f6e 6461 7279 2069   the secondary i
+0000b830: 6e74 6572 6661 6365 732c 2077 6869 6368  nterfaces, which
+0000b840: 2069 7320 7265 616c 6c79 2061 206c 6973   is really a lis
+0000b850: 7420 6f66 206c 6973 7420 6f66 2073 7472  t of list of str
+0000b860: 696e 6773 2e0a 2020 2020 2020 2020 2222  ings..        ""
+0000b870: 220a 2020 2020 2020 2020 7365 6c66 2e73  ".        self.s
+0000b880: 6563 6f6e 6461 7279 5f69 6e74 6572 6661  econdary_interfa
+0000b890: 6365 7320 3d20 5b5d 0a20 2020 2020 2020  ces = [].       
+0000b8a0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+0000b8b0: 6c65 6e28 6e65 775f 7365 636f 6e64 6172  len(new_secondar
+0000b8c0: 795f 696e 7465 7266 6163 6573 2929 3a0a  y_interfaces)):.
+0000b8d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b8e0: 2e73 6563 6f6e 6461 7279 5f69 6e74 6572  .secondary_inter
+0000b8f0: 6661 6365 732e 6170 7065 6e64 285b 5d29  faces.append([])
+0000b900: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000b910: 206a 2069 6e20 7261 6e67 6528 6c65 6e28   j in range(len(
+0000b920: 6e65 775f 7365 636f 6e64 6172 795f 696e  new_secondary_in
+0000b930: 7465 7266 6163 6573 5b69 5d2e 6164 6472  terfaces[i].addr
+0000b940: 6573 7329 293a 0a20 2020 2020 2020 2020  ess)):.         
+0000b950: 2020 2020 2020 2069 6e74 6572 6661 6365         interface
+0000b960: 203d 206e 6577 5f73 6563 6f6e 6461 7279   = new_secondary
+0000b970: 5f69 6e74 6572 6661 6365 735b 695d 2e61  _interfaces[i].a
+0000b980: 6464 7265 7373 5b6a 5d0a 2020 2020 2020  ddress[j].      
+0000b990: 2020 2020 2020 2020 2020 2869 6e74 6572            (inter
+0000b9a0: 6661 6365 5f69 702c 2069 6e74 6572 6661  face_ip, interfa
+0000b9b0: 6365 5f70 6f72 7429 203d 2069 6e74 6572  ce_port) = inter
+0000b9c0: 6661 6365 2e73 706c 6974 2822 3a22 290a  face.split(":").
+0000b9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b9e0: 2320 5265 7475 726e 206f 6620 6765 7468  # Return of geth
+0000b9f0: 6f73 7462 796e 616d 655f 6578 2069 7320  ostbyname_ex is 
+0000ba00: 2868 6f73 746e 616d 652c 2061 6c69 6173  (hostname, alias
+0000ba10: 206f 6620 686f 7374 206e 616d 652c 206f   of host name, o
+0000ba20: 7468 6572 2069 7020 6164 6472 6573 7365  ther ip addresse
+0000ba30: 7320 6f66 2068 6f73 7420 6e61 6d65 290a  s of host name).
+0000ba40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba50: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+0000ba60: 2020 2020 2020 2020 206f 7468 6572 5f69           other_i
+0000ba70: 7073 203d 2073 6f63 6b65 742e 6765 7468  ps = socket.geth
+0000ba80: 6f73 7462 796e 616d 655f 6578 2869 6e74  ostbyname_ex(int
+0000ba90: 6572 6661 6365 5f69 7029 5b32 5d0a 2020  erface_ip)[2].  
+0000baa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bab0: 2020 666f 7220 6f74 6865 725f 6970 2069    for other_ip i
+0000bac0: 6e20 6f74 6865 725f 6970 733a 0a20 2020  n other_ips:.   
+0000bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bae0: 2020 2020 2073 656c 662e 7365 636f 6e64       self.second
+0000baf0: 6172 795f 696e 7465 7266 6163 6573 5b69  ary_interfaces[i
+0000bb00: 5d2e 6170 7065 6e64 2828 6f74 6865 725f  ].append((other_
+0000bb10: 6970 2c20 696e 7428 696e 7465 7266 6163  ip, int(interfac
+0000bb20: 655f 706f 7274 2929 290a 2020 2020 2020  e_port))).      
+0000bb30: 2020 2020 2020 2020 2020 6578 6365 7074            except
+0000bb40: 2073 6f63 6b65 742e 6761 6965 7272 6f72   socket.gaierror
+0000bb50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000bb60: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+0000bb70: 2020 2020 686f 7374 733a 204c 6973 745b      hosts: List[
+0000bb80: 5475 706c 655b 7374 722c 2069 6e74 5d5d  Tuple[str, int]]
+0000bb90: 203d 205b 5d0a 2020 2020 2020 2020 6173   = [].        as
+0000bba0: 7365 7274 2073 656c 662e 706f 7274 2069  sert self.port i
+0000bbb0: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2020  s not None.     
+0000bbc0: 2020 2066 6f72 206f 6e65 5f68 6f73 7420     for one_host 
+0000bbd0: 696e 2073 656c 662e 686f 7374 733a 0a20  in self.hosts:. 
+0000bbe0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+0000bbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc00: 686f 7374 7320 3d20 686f 7374 7320 2b20  hosts = hosts + 
+0000bc10: 5b28 686f 7374 2c20 7365 6c66 2e70 6f72  [(host, self.por
+0000bc20: 7429 2066 6f72 2068 6f73 7420 696e 2073  t) for host in s
+0000bc30: 6f63 6b65 742e 6765 7468 6f73 7462 796e  ocket.gethostbyn
+0000bc40: 616d 655f 6578 286f 6e65 5f68 6f73 7429  ame_ex(one_host)
+0000bc50: 5b32 5d5d 0a20 2020 2020 2020 2020 2020  [2]].           
+0000bc60: 2065 7863 6570 7420 736f 636b 6574 2e67   except socket.g
+0000bc70: 6169 6572 726f 723a 0a20 2020 2020 2020  aierror:.       
+0000bc80: 2020 2020 2020 2020 2070 6173 730a 2020           pass.  
+0000bc90: 2020 2020 2020 666f 7220 6f75 7465 725f        for outer_
+0000bca0: 6c69 7374 2069 6e20 7365 6c66 2e73 6563  list in self.sec
+0000bcb0: 6f6e 6461 7279 5f69 6e74 6572 6661 6365  ondary_interface
+0000bcc0: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
+0000bcd0: 6f72 2069 6e64 6578 2069 6e20 7261 6e67  or index in rang
+0000bce0: 6528 6c65 6e28 6f75 7465 725f 6c69 7374  e(len(outer_list
+0000bcf0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+0000bd00: 2020 2020 6966 206f 7574 6572 5f6c 6973      if outer_lis
+0000bd10: 745b 696e 6465 785d 2069 6e20 686f 7374  t[index] in host
+0000bd20: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+0000bd30: 2020 2020 2020 2073 656c 662e 7365 636f         self.seco
+0000bd40: 6e64 6172 795f 696e 6465 7820 3d20 696e  ndary_index = in
+0000bd50: 6465 780a 2020 2020 2020 2020 2020 2020  dex.            
+0000bd60: 2020 2020 2020 2020 6272 6561 6b0a 0a20          break.. 
+0000bd70: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+0000bd80: 6275 6728 0a20 2020 2020 2020 2020 2020  bug(.           
+0000bd90: 2066 2253 6176 696e 6720 7365 636f 6e64   f"Saving second
+0000bda0: 6172 7920 696e 7465 7266 6163 6573 3a20  ary interfaces: 
+0000bdb0: 696e 6465 7820 7b73 656c 662e 7365 636f  index {self.seco
+0000bdc0: 6e64 6172 795f 696e 6465 787d 2069 6e74  ndary_index} int
+0000bdd0: 6572 6661 6365 733a 207b 7365 6c66 2e73  erfaces: {self.s
+0000bde0: 6563 6f6e 6461 7279 5f69 6e74 6572 6661  econdary_interfa
+0000bdf0: 6365 737d 220a 2020 2020 2020 2020 290a  ces}".        ).
+0000be00: 0a20 2020 2064 6566 205f 656e 6372 7970  .    def _encryp
+0000be10: 7469 6f6e 5f72 6f75 7469 6e65 280a 2020  tion_routine(.  
+0000be20: 2020 2020 2020 7365 6c66 2c20 696e 6974        self, init
+0000be30: 6961 6c69 7a61 7469 6f6e 5f76 6563 746f  ialization_vecto
+0000be40: 723a 2062 7974 6573 2c20 7065 6572 5f6b  r: bytes, peer_k
+0000be50: 6579 3a20 4448 5075 626c 6963 4b65 790a  ey: DHPublicKey.
+0000be60: 2020 2020 2920 2d3e 2054 7570 6c65 5b62      ) -> Tuple[b
+0000be70: 7974 6573 2c20 6279 7465 732c 2044 4850  ytes, bytes, DHP
+0000be80: 7562 6c69 634b 6579 5d3a 0a20 2020 2020  ublicKey]:.     
+0000be90: 2020 2022 2222 496e 7465 726e 616c 2072     """Internal r
+0000bea0: 6f75 7469 6e65 2074 6f20 646f 2074 6865  outine to do the
+0000beb0: 2065 6e63 7279 7074 696f 6e20 6861 6e64   encryption hand
+0000bec0: 7368 616b 6520 6f66 0a20 2020 2020 2020  shake of.       
+0000bed0: 2074 6865 2070 6173 7377 6f72 640a 2020   the password.  
+0000bee0: 2020 2020 2020 4342 4320 6973 2074 6865        CBC is the
+0000bef0: 2070 7265 7669 6f75 7320 666f 726d 206f   previous form o
+0000bf00: 6620 656e 6372 7970 7469 6f6e 2e20 5765  f encryption. We
+0000bf10: 206e 6f77 2075 7365 2047 434d 2062 7920   now use GCM by 
+0000bf20: 6465 6661 756c 742e 0a20 2020 2020 2020  default..       
+0000bf30: 2022 2222 0a20 2020 2020 2020 2023 2043   """.        # C
+0000bf40: 7265 6174 6520 6f75 7220 6b65 7973 2075  reate our keys u
+0000bf50: 7369 6e67 2074 6865 2070 6172 616d 6574  sing the paramet
+0000bf60: 6572 7320 6672 6f6d 2074 6865 2070 6565  ers from the pee
+0000bf70: 7220 6b65 790a 2020 2020 2020 2020 7061  r key.        pa
+0000bf80: 7261 6d73 203d 2070 6565 725f 6b65 792e  rams = peer_key.
+0000bf90: 7061 7261 6d65 7465 7273 2829 0a20 2020  parameters().   
+0000bfa0: 2020 2020 2070 7269 7661 7465 5f6b 6579       private_key
+0000bfb0: 203d 2070 6172 616d 732e 6765 6e65 7261   = params.genera
+0000bfc0: 7465 5f70 7269 7661 7465 5f6b 6579 2829  te_private_key()
+0000bfd0: 0a0a 2020 2020 2020 2020 2320 4372 6561  ..        # Crea
+0000bfe0: 7465 2061 2073 6861 7265 6420 6b65 790a  te a shared key.
+0000bff0: 2020 2020 2020 2020 7368 6172 6564 5f6b          shared_k
+0000c000: 6579 203d 2070 7269 7661 7465 5f6b 6579  ey = private_key
+0000c010: 2e65 7863 6861 6e67 6528 7065 6572 5f6b  .exchange(peer_k
+0000c020: 6579 290a 0a20 2020 2020 2020 206b 6579  ey)..        key
+0000c030: 203d 205f 6861 7368 5f6b 6579 2873 6861   = _hash_key(sha
+0000c040: 7265 645f 6b65 792c 2062 225c 3022 290a  red_key, b"\0").
+0000c050: 2020 2020 2020 2020 6d61 635f 6b65 7920          mac_key 
+0000c060: 3d20 5f68 6173 685f 6b65 7928 7368 6172  = _hash_key(shar
+0000c070: 6564 5f6b 6579 2c20 6222 5c31 2229 0a0a  ed_key, b"\1")..
+0000c080: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
+0000c090: 656c 662e 7061 7373 776f 7264 2069 7320  elf.password is 
+0000c0a0: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
+0000c0b0: 2069 6620 7365 6c66 2e68 616e 6473 6861   if self.handsha
+0000c0c0: 6b65 203d 3d20 7365 6c66 2e48 414e 4453  ke == self.HANDS
+0000c0d0: 4841 4b45 5f43 4243 3a0a 2020 2020 2020  HAKE_CBC:.      
+0000c0e0: 2020 2020 2020 2320 5061 6420 7468 6520        # Pad the 
+0000c0f0: 706c 6169 6e74 6578 7420 7061 7373 776f  plaintext passwo
+0000c100: 7264 206f 7574 2075 7369 6e67 2050 4b43  rd out using PKC
+0000c110: 5337 0a20 2020 2020 2020 2020 2020 2070  S7.            p
+0000c120: 6164 6465 7220 3d20 7061 6464 696e 672e  adder = padding.
+0000c130: 504b 4353 3728 3132 3829 2e70 6164 6465  PKCS7(128).padde
+0000c140: 7228 290a 2020 2020 2020 2020 2020 2020  r().            
+0000c150: 7061 6464 6564 5f64 6174 6120 3d20 7061  padded_data = pa
+0000c160: 6464 6572 2e75 7064 6174 6528 7365 6c66  dder.update(self
+0000c170: 2e70 6173 7377 6f72 642e 656e 636f 6465  .password.encode
+0000c180: 2865 6e63 6f64 696e 673d 2255 5446 2d38  (encoding="UTF-8
+0000c190: 222c 2065 7272 6f72 733d 2273 7472 6963  ", errors="stric
+0000c1a0: 7422 2929 0a20 2020 2020 2020 2020 2020  t")).           
+0000c1b0: 2070 6164 6465 645f 6461 7461 202b 3d20   padded_data += 
+0000c1c0: 7061 6464 6572 2e66 696e 616c 697a 6528  padder.finalize(
+0000c1d0: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
+0000c1e0: 2045 6e63 7279 7074 2074 6865 2070 6164   Encrypt the pad
+0000c1f0: 6465 6420 706c 6169 6e74 6578 7420 7061  ded plaintext pa
+0000c200: 7373 776f 7264 2075 7369 6e67 2041 4553  ssword using AES
+0000c210: 2043 4243 2061 6e64 2074 6865 206b 6579   CBC and the key
+0000c220: 0a20 2020 2020 2020 2020 2020 2023 2077  .            # w
+0000c230: 6520 676f 7420 6672 6f6d 206f 7572 204b  e got from our K
+0000c240: 4446 0a20 2020 2020 2020 2020 2020 2065  DF.            e
+0000c250: 6e63 7279 7074 6f72 203d 2043 6970 6865  ncryptor = Ciphe
+0000c260: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+0000c270: 2020 2061 6c67 6f72 6974 686d 732e 4145     algorithms.AE
+0000c280: 5328 6b65 7929 2c0a 2020 2020 2020 2020  S(key),.        
+0000c290: 2020 2020 2020 2020 6d6f 6465 732e 4342          modes.CB
+0000c2a0: 4328 696e 6974 6961 6c69 7a61 7469 6f6e  C(initialization
+0000c2b0: 5f76 6563 746f 7229 2c0a 2020 2020 2020  _vector),.      
+0000c2c0: 2020 2020 2020 2020 2020 6261 636b 656e            backen
+0000c2d0: 643d 6465 6661 756c 745f 6261 636b 656e  d=default_backen
+0000c2e0: 6428 292c 0a20 2020 2020 2020 2020 2020  d(),.           
+0000c2f0: 2029 2e65 6e63 7279 7074 6f72 2829 0a20   ).encryptor(). 
+0000c300: 2020 2020 2020 2020 2020 206d 696e 5f63             min_c
+0000c310: 6970 6865 725f 6279 7465 7320 3d20 6c65  ipher_bytes = le
+0000c320: 6e28 7061 6464 6564 5f64 6174 6129 202b  n(padded_data) +
+0000c330: 2034 3039 360a 2020 2020 2020 2020 2020   4096.          
+0000c340: 2020 6275 6620 3d20 6279 7465 6172 7261    buf = bytearra
+0000c350: 7928 6d69 6e5f 6369 7068 6572 5f62 7974  y(min_cipher_byt
+0000c360: 6573 290a 2020 2020 2020 2020 2020 2020  es).            
+0000c370: 6c65 6e5f 656e 6372 7970 7465 6420 3d20  len_encrypted = 
+0000c380: 656e 6372 7970 746f 722e 7570 6461 7465  encryptor.update
+0000c390: 5f69 6e74 6f28 7061 6464 6564 5f64 6174  _into(padded_dat
+0000c3a0: 612c 2062 7566 290a 2020 2020 2020 2020  a, buf).        
+0000c3b0: 2020 2020 6369 7068 6572 203d 2062 7974      cipher = byt
+0000c3c0: 6573 2862 7566 5b3a 6c65 6e5f 656e 6372  es(buf[:len_encr
+0000c3d0: 7970 7465 645d 2920 2b20 656e 6372 7970  ypted]) + encryp
+0000c3e0: 746f 722e 6669 6e61 6c69 7a65 2829 0a20  tor.finalize(). 
+0000c3f0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000c400: 2020 2020 2020 2020 2065 6e63 7279 7074           encrypt
+0000c410: 6f72 203d 2043 6970 6865 7228 0a20 2020  or = Cipher(.   
+0000c420: 2020 2020 2020 2020 2020 2020 2061 6c67               alg
+0000c430: 6f72 6974 686d 732e 4145 5328 6b65 7929  orithms.AES(key)
+0000c440: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000c450: 2020 6d6f 6465 732e 4743 4d28 696e 6974    modes.GCM(init
+0000c460: 6961 6c69 7a61 7469 6f6e 5f76 6563 746f  ialization_vecto
+0000c470: 7229 2c0a 2020 2020 2020 2020 2020 2020  r),.            
+0000c480: 2020 2020 6261 636b 656e 643d 6465 6661      backend=defa
+0000c490: 756c 745f 6261 636b 656e 6428 292c 0a20  ult_backend(),. 
+0000c4a0: 2020 2020 2020 2020 2020 2029 2e65 6e63             ).enc
+0000c4b0: 7279 7074 6f72 2829 0a20 2020 2020 2020  ryptor().       
+0000c4c0: 2020 2020 2023 2057 6520 646f 206e 6f74       # We do not
+0000c4d0: 2075 7365 2041 4144 0a20 2020 2020 2020   use AAD.       
+0000c4e0: 2020 2020 2063 6970 6865 7220 3d20 656e       cipher = en
+0000c4f0: 6372 7970 746f 722e 7570 6461 7465 2873  cryptor.update(s
+0000c500: 656c 662e 7061 7373 776f 7264 2e65 6e63  elf.password.enc
+0000c510: 6f64 6528 656e 636f 6469 6e67 3d22 5554  ode(encoding="UT
+0000c520: 462d 3822 2c20 6572 726f 7273 3d22 7374  F-8", errors="st
+0000c530: 7269 6374 2229 2920 2b20 656e 6372 7970  rict")) + encryp
+0000c540: 746f 722e 6669 6e61 6c69 7a65 2829 0a20  tor.finalize(). 
+0000c550: 2020 2020 2020 2020 2020 2023 2053 6572             # Ser
+0000c560: 7665 7220 7369 6465 2065 7870 6563 7473  ver side expects
+0000c570: 2074 6861 7420 7468 6520 7461 6720 6973   that the tag is
+0000c580: 2061 7420 7468 6520 656e 6420 6f66 2074   at the end of t
+0000c590: 6865 2063 6970 6865 7220 7465 7874 2e0a  he cipher text..
+0000c5a0: 2020 2020 2020 2020 2020 2020 6369 7068              ciph
+0000c5b0: 6572 202b 3d20 656e 6372 7970 746f 722e  er += encryptor.
+0000c5c0: 7461 670a 0a20 2020 2020 2020 2023 204e  tag..        # N
+0000c5d0: 6f77 2063 7265 6174 6520 616e 2048 4d41  ow create an HMA
+0000c5e0: 4320 7573 696e 6720 7468 6520 6f74 6865  C using the othe
+0000c5f0: 7220 4b44 4620 6465 7269 7665 6420 6b65  r KDF derived ke
+0000c600: 7920 616e 6420 7468 650a 2020 2020 2020  y and the.      
+0000c610: 2020 2320 656e 6372 7970 7465 6420 7061    # encrypted pa
+0000c620: 7373 776f 7264 0a20 2020 2020 2020 2068  ssword.        h
+0000c630: 6173 6865 7220 3d20 686d 6163 2e48 4d41  asher = hmac.HMA
+0000c640: 4328 6d61 635f 6b65 792c 2068 6173 6865  C(mac_key, hashe
+0000c650: 732e 5348 4132 3536 2829 2c20 6261 636b  s.SHA256(), back
+0000c660: 656e 643d 6465 6661 756c 745f 6261 636b  end=default_back
+0000c670: 656e 6428 2929 0a20 2020 2020 2020 2068  end()).        h
+0000c680: 6173 6865 722e 7570 6461 7465 2863 6970  asher.update(cip
+0000c690: 6865 7229 0a20 2020 2020 2020 2067 656e  her).        gen
+0000c6a0: 6572 6174 6564 5f68 6d61 6320 3d20 6861  erated_hmac = ha
+0000c6b0: 7368 6572 2e66 696e 616c 697a 6528 290a  sher.finalize().
+0000c6c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000c6d0: 2863 6970 6865 722c 2067 656e 6572 6174  (cipher, generat
+0000c6e0: 6564 5f68 6d61 632c 2070 7269 7661 7465  ed_hmac, private
+0000c6f0: 5f6b 6579 2e70 7562 6c69 635f 6b65 7928  _key.public_key(
+0000c700: 2929 0a0a 2020 2020 6465 6620 5f70 6172  ))..    def _par
+0000c710: 7365 5f61 7267 7328 0a20 2020 2020 2020  se_args(.       
+0000c720: 2073 656c 662c 0a20 2020 2020 2020 2064   self,.        d
+0000c730: 736e 3a20 4f70 7469 6f6e 616c 5b73 7472  sn: Optional[str
+0000c740: 5d2c 0a20 2020 2020 2020 2075 7365 723a  ],.        user:
+0000c750: 204f 7074 696f 6e61 6c5b 7374 725d 2c0a   Optional[str],.
+0000c760: 2020 2020 2020 2020 7061 7373 776f 7264          password
+0000c770: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d2c  : Optional[str],
+0000c780: 0a20 2020 2020 2020 2068 6f73 743a 204f  .        host: O
+0000c790: 7074 696f 6e61 6c5b 7374 725d 2c0a 2020  ptional[str],.  
+0000c7a0: 2020 2020 2020 6461 7461 6261 7365 3a20        database: 
+0000c7b0: 4f70 7469 6f6e 616c 5b73 7472 5d2c 0a20  Optional[str],. 
+0000c7c0: 2020 2020 2020 2074 6c73 3a20 4f70 7469         tls: Opti
+0000c7d0: 6f6e 616c 5b55 6e69 6f6e 5b73 7472 2c20  onal[Union[str, 
+0000c7e0: 696e 745d 5d2c 0a20 2020 2020 2020 2068  int]],.        h
+0000c7f0: 616e 6473 6861 6b65 3a20 4f70 7469 6f6e  andshake: Option
+0000c800: 616c 5b69 6e74 5d2c 0a20 2020 2020 2020  al[int],.       
+0000c810: 2066 6f72 6365 3a20 4f70 7469 6f6e 616c   force: Optional
+0000c820: 5b62 6f6f 6c5d 2c0a 2020 2020 2020 2020  [bool],.        
+0000c830: 636f 6e66 6967 6669 6c65 3a20 4f70 7469  configfile: Opti
+0000c840: 6f6e 616c 5b73 7472 5d2c 0a20 2020 2029  onal[str],.    )
+0000c850: 202d 3e20 4e6f 6e65 3a20 2023 2070 796c   -> None:  # pyl
+0000c860: 696e 743a 2064 6973 6162 6c65 3d74 6f6f  int: disable=too
+0000c870: 2d6d 616e 792d 6172 6775 6d65 6e74 730a  -many-arguments.
+0000c880: 2020 2020 2020 2020 2222 2249 6e74 6572          """Inter
+0000c890: 6e61 6c20 726f 7574 696e 6520 746f 2072  nal routine to r
+0000c8a0: 6573 6f6c 7665 2066 756e 6374 696f 6e20  esolve function 
+0000c8b0: 6172 6775 6d65 6e74 732c 2063 6f6e 6669  arguments, confi
+0000c8c0: 6720 6669 6c65 2c20 616e 6420 6473 6e22  g file, and dsn"
+0000c8d0: 2222 0a20 2020 2020 2020 2023 2070 796c  "".        # pyl
+0000c8e0: 696e 743a 2064 6973 6162 6c65 3d6e 6f2d  int: disable=no-
+0000c8f0: 6d65 6d62 6572 2c74 6f6f 2d6d 616e 792d  member,too-many-
+0000c900: 6272 616e 6368 6573 2c74 6f6f 2d6d 616e  branches,too-man
+0000c910: 792d 7374 6174 656d 656e 7473 0a20 2020  y-statements.   
+0000c920: 2020 2020 2023 2046 6972 7374 2c20 7061       # First, pa
+0000c930: 7273 6520 7468 6520 4453 4e20 6966 2069  rse the DSN if i
+0000c940: 7420 6578 6973 7473 0a20 2020 2020 2020  t exists.       
+0000c950: 2069 6620 6473 6e20 6973 206e 6f74 204e   if dsn is not N
+0000c960: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000c970: 2070 6172 7365 6420 3d20 6473 6e70 6172   parsed = dsnpar
+0000c980: 7365 2e70 6172 7365 2864 736e 290a 0a20  se.parse(dsn).. 
+0000c990: 2020 2020 2020 2020 2020 2069 6620 7061             if pa
+0000c9a0: 7273 6564 2e73 6368 656d 6520 616e 6420  rsed.scheme and 
+0000c9b0: 7061 7273 6564 2e73 6368 656d 652e 6c6f  parsed.scheme.lo
+0000c9c0: 7765 7228 2920 213d 2022 6f63 6965 6e74  wer() != "ocient
+0000c9d0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+0000c9e0: 2020 2072 6169 7365 204d 616c 666f 726d     raise Malform
+0000c9f0: 6564 5552 4c28 6622 496e 7661 6c69 6420  edURL(f"Invalid 
+0000ca00: 4453 4e20 7363 6865 6d65 3a20 7b70 6172  DSN scheme: {par
+0000ca10: 7365 642e 7363 6865 6d65 7d22 290a 0a20  sed.scheme}").. 
+0000ca20: 2020 2020 2020 2020 2020 2066 6f72 2061             for a
+0000ca30: 7474 7220 696e 205b 2264 6174 6162 6173  ttr in ["databas
+0000ca40: 6522 2c20 2275 7365 7222 2c20 2270 6173  e", "user", "pas
+0000ca50: 7377 6f72 6422 2c20 2270 6f72 7422 5d3a  sword", "port"]:
+0000ca60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ca70: 2073 6574 6174 7472 2873 656c 662c 2061   setattr(self, a
+0000ca80: 7474 722c 2067 6574 6174 7472 2870 6172  ttr, getattr(par
+0000ca90: 7365 642c 2061 7474 7229 290a 0a20 2020  sed, attr))..   
+0000caa0: 2020 2020 2020 2020 2069 6620 7061 7273           if pars
+0000cab0: 6564 2e68 6f73 743a 0a20 2020 2020 2020  ed.host:.       
+0000cac0: 2020 2020 2020 2020 2073 656c 662e 686f           self.ho
+0000cad0: 7374 7320 3d20 7061 7273 6564 2e68 6f73  sts = parsed.hos
+0000cae0: 742e 7370 6c69 7428 222c 2229 0a0a 2020  t.split(",")..  
+0000caf0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000cb00: 662e 6461 7461 6261 7365 2069 7320 6e6f  f.database is no
+0000cb10: 7420 4e6f 6e65 2061 6e64 206c 656e 2873  t None and len(s
+0000cb20: 656c 662e 6461 7461 6261 7365 2920 3d3d  elf.database) ==
+0000cb30: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+0000cb40: 2020 2020 7365 6c66 2e64 6174 6162 6173      self.databas
+0000cb50: 6520 3d20 4e6f 6e65 0a20 2020 2020 2020  e = None.       
+0000cb60: 2020 2020 2069 6620 7365 6c66 2e64 6174       if self.dat
+0000cb70: 6162 6173 6520 6973 206e 6f74 204e 6f6e  abase is not Non
+0000cb80: 6520 616e 6420 7365 6c66 2e64 6174 6162  e and self.datab
+0000cb90: 6173 655b 305d 203d 3d20 222f 223a 0a20  ase[0] == "/":. 
+0000cba0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000cbb0: 656c 662e 6461 7461 6261 7365 203d 2073  elf.database = s
+0000cbc0: 656c 662e 6461 7461 6261 7365 5b31 3a5d  elf.database[1:]
+0000cbd0: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0000cbe0: 2022 746c 7322 2069 6e20 7061 7273 6564   "tls" in parsed
+0000cbf0: 2e71 7565 7279 3a0a 2020 2020 2020 2020  .query:.        
+0000cc00: 2020 2020 2020 2020 7365 6c66 2e74 6c73          self.tls
+0000cc10: 203d 2070 6172 7365 642e 7175 6572 795b   = parsed.query[
+0000cc20: 2274 6c73 225d 0a0a 2020 2020 2020 2020  "tls"]..        
+0000cc30: 2020 2020 6966 2022 666f 7263 6522 2069      if "force" i
+0000cc40: 6e20 7061 7273 6564 2e71 7565 7279 3a0a  n parsed.query:.
+0000cc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc60: 7368 6f75 6c64 466f 7263 6520 3d20 7061  shouldForce = pa
+0000cc70: 7273 6564 2e71 7565 7279 5b22 666f 7263  rsed.query["forc
+0000cc80: 6522 5d0a 2020 2020 2020 2020 2020 2020  e"].            
+0000cc90: 2020 2020 6966 2073 686f 756c 6446 6f72      if shouldFor
+0000cca0: 6365 2e75 7070 6572 2829 203d 3d20 2254  ce.upper() == "T
+0000ccb0: 5255 4522 3a0a 2020 2020 2020 2020 2020  RUE":.          
+0000ccc0: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
+0000ccd0: 6f72 6365 203d 2054 7275 650a 2020 2020  orce = True.    
+0000cce0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+0000ccf0: 2073 686f 756c 6446 6f72 6365 2e75 7070   shouldForce.upp
+0000cd00: 6572 2829 203d 3d20 2246 414c 5345 223a  er() == "FALSE":
+0000cd10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cd20: 2020 2020 2073 656c 662e 666f 7263 6520       self.force 
+0000cd30: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
+0000cd40: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000cd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd60: 2020 7261 6973 6520 4d61 6c66 6f72 6d65    raise Malforme
+0000cd70: 6455 524c 2866 2249 6e76 616c 6964 2066  dURL(f"Invalid f
+0000cd80: 6f72 6365 2073 7472 696e 673a 207b 7368  orce string: {sh
+0000cd90: 6f75 6c64 466f 7263 657d 2229 0a0a 2020  ouldForce}")..  
+0000cda0: 2020 2020 2020 2020 2020 6966 2066 6f72            if for
+0000cdb0: 6365 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ce is not None:.
+0000cdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdd0: 7365 6c66 2e66 6f72 6365 203d 2066 6f72  self.force = for
+0000cde0: 6365 0a0a 2020 2020 2020 2020 2020 2020  ce..            
+0000cdf0: 6966 2022 6861 6e64 7368 616b 6522 2069  if "handshake" i
+0000ce00: 6e20 7061 7273 6564 2e71 7565 7279 3a0a  n parsed.query:.
+0000ce10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce20: 6861 6e64 7368 616b 6520 3d20 7061 7273  handshake = pars
+0000ce30: 6564 2e71 7565 7279 5b22 6861 6e64 7368  ed.query["handsh
+0000ce40: 616b 6522 5d2e 6c6f 7765 7228 290a 0a20  ake"].lower().. 
+0000ce50: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000ce60: 6c66 2e75 7365 7220 6973 204e 6f6e 653a  lf.user is None:
+0000ce70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ce80: 2073 656c 662e 7573 6572 203d 2022 220a   self.user = "".
+0000ce90: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000cea0: 7365 6c66 2e70 6173 7377 6f72 6420 6973  self.password is
+0000ceb0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000cec0: 2020 2020 2020 2073 656c 662e 7061 7373         self.pass
+0000ced0: 776f 7264 203d 2022 220a 0a20 2020 2020  word = ""..     
+0000cee0: 2020 2023 204e 6f77 206f 7665 7272 6964     # Now overrid
+0000cef0: 6520 7468 6520 4453 4e20 7661 6c75 6573  e the DSN values
+0000cf00: 2077 6974 6820 616e 7920 7661 6c75 6573   with any values
+0000cf10: 2070 6173 7365 6420 696e 2061 7320 7061   passed in as pa
+0000cf20: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+0000cf30: 2069 6620 7573 6572 2069 7320 6e6f 7420   if user is not 
+0000cf40: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000cf50: 2020 7365 6c66 2e75 7365 7220 3d20 7573    self.user = us
+0000cf60: 6572 0a0a 2020 2020 2020 2020 6966 2070  er..        if p
+0000cf70: 6173 7377 6f72 6420 6973 206e 6f74 204e  assword is not N
+0000cf80: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000cf90: 2073 656c 662e 7061 7373 776f 7264 203d   self.password =
+0000cfa0: 2070 6173 7377 6f72 640a 0a20 2020 2020   password..     
+0000cfb0: 2020 2069 6620 686f 7374 3a0a 2020 2020     if host:.    
+0000cfc0: 2020 2020 2020 2020 2320 4861 6e64 6c65          # Handle
+0000cfd0: 2068 6f73 743a 706f 7274 0a20 2020 2020   host:port.     
+0000cfe0: 2020 2020 2020 2070 6172 7473 203d 2068         parts = h
+0000cff0: 6f73 742e 7370 6c69 7428 223a 2229 0a20  ost.split(":"). 
+0000d000: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+0000d010: 6e28 7061 7274 7329 203d 3d20 313a 0a20  n(parts) == 1:. 
+0000d020: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000d030: 656c 662e 686f 7374 7320 3d20 7061 7274  elf.hosts = part
+0000d040: 735b 305d 2e73 706c 6974 2822 2c22 290a  s[0].split(",").
+0000d050: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+0000d060: 206c 656e 2870 6172 7473 2920 3d3d 2032   len(parts) == 2
+0000d070: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000d080: 2020 7365 6c66 2e68 6f73 7473 203d 2070    self.hosts = p
+0000d090: 6172 7473 5b30 5d2e 7370 6c69 7428 222c  arts[0].split(",
+0000d0a0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+0000d0b0: 2020 2073 656c 662e 706f 7274 203d 2069     self.port = i
+0000d0c0: 6e74 2870 6172 7473 5b31 5d29 0a20 2020  nt(parts[1]).   
+0000d0d0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000d0e0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000d0f0: 6169 7365 204d 616c 666f 726d 6564 5552  aise MalformedUR
+0000d100: 4c28 6622 496e 7661 6c69 6420 686f 7374  L(f"Invalid host
+0000d110: 2076 616c 7565 3a20 7b68 6f73 747d 2229   value: {host}")
+0000d120: 0a0a 2020 2020 2020 2020 6966 2064 6174  ..        if dat
+0000d130: 6162 6173 653a 0a20 2020 2020 2020 2020  abase:.         
+0000d140: 2020 2073 656c 662e 6461 7461 6261 7365     self.database
+0000d150: 203d 2064 6174 6162 6173 650a 0a20 2020   = database..   
+0000d160: 2020 2020 2069 6620 746c 7320 6973 206e       if tls is n
+0000d170: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000d180: 2020 2020 2073 656c 662e 746c 7320 3d20       self.tls = 
+0000d190: 746c 730a 0a20 2020 2020 2020 2069 6620  tls..        if 
+0000d1a0: 6861 6e64 7368 616b 6520 6973 206e 6f74  handshake is not
+0000d1b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000d1c0: 2020 2073 656c 662e 6861 6e64 7368 616b     self.handshak
+0000d1d0: 6520 3d20 6861 6e64 7368 616b 650a 0a20  e = handshake.. 
+0000d1e0: 2020 2020 2020 2023 2053 6574 2074 6865         # Set the
+0000d1f0: 2064 6566 6175 6c74 2068 6f73 7420 6e6f   default host no
+0000d200: 772c 2073 696e 6365 2077 6520 7573 6520  w, since we use 
+0000d210: 7468 6174 2061 7320 6120 6b65 7920 696e  that as a key in
+0000d220: 746f 2074 6865 0a20 2020 2020 2020 2023  to the.        #
+0000d230: 2063 6f6e 6669 6720 6669 6c65 0a20 2020   config file.   
+0000d240: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+0000d250: 2e68 6f73 7473 3a0a 2020 2020 2020 2020  .hosts:.        
+0000d260: 2020 2020 7365 6c66 2e68 6f73 7473 203d      self.hosts =
+0000d270: 205b 7365 6c66 2e44 4546 4155 4c54 5f48   [self.DEFAULT_H
+0000d280: 4f53 545d 0a0a 2020 2020 2020 2020 2320  OST]..        # 
+0000d290: 4e6f 7720 6275 696c 6420 6120 636f 6e66  Now build a conf
+0000d2a0: 6967 7061 7273 6572 2077 6974 6820 6465  igparser with de
+0000d2b0: 6661 756c 7420 7661 6c75 6573 0a20 2020  fault values.   
+0000d2c0: 2020 2020 2063 6f6e 6669 6720 3d20 636f       config = co
+0000d2d0: 6e66 6967 7061 7273 6572 2e43 6f6e 6669  nfigparser.Confi
+0000d2e0: 6750 6172 7365 7228 0a20 2020 2020 2020  gParser(.       
+0000d2f0: 2020 2020 2064 6566 6175 6c74 733d 7b0a       defaults={.
+0000d300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d310: 2270 6f72 7422 3a20 7374 7228 7365 6c66  "port": str(self
+0000d320: 2e44 4546 4155 4c54 5f50 4f52 5429 2c0a  .DEFAULT_PORT),.
+0000d330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d340: 2264 6174 6162 6173 6522 3a20 7365 6c66  "database": self
+0000d350: 2e44 4546 4155 4c54 5f44 4154 4142 4153  .DEFAULT_DATABAS
+0000d360: 452c 0a20 2020 2020 2020 2020 2020 2020  E,.             
+0000d370: 2020 2022 746c 7322 3a20 2275 6e76 6572     "tls": "unver
+0000d380: 6966 6965 6422 2c0a 2020 2020 2020 2020  ified",.        
+0000d390: 2020 2020 2020 2020 2266 6f72 6365 223a          "force":
+0000d3a0: 2022 6661 6c73 6522 2c0a 2020 2020 2020   "false",.      
+0000d3b0: 2020 2020 2020 2020 2020 2268 616e 6473            "hands
+0000d3c0: 6861 6b65 223a 2022 222c 0a20 2020 2020  hake": "",.     
+0000d3d0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+0000d3e0: 2020 2020 2020 696e 7465 7270 6f6c 6174        interpolat
+0000d3f0: 696f 6e3d 4e6f 6e65 2c0a 2020 2020 2020  ion=None,.      
+0000d400: 2020 290a 2020 2020 2020 2020 636f 6e66    ).        conf
+0000d410: 6967 7661 6c73 203d 204e 6f6e 650a 0a20  igvals = None.. 
+0000d420: 2020 2020 2020 2023 2049 6620 7765 2068         # If we h
+0000d430: 6176 6520 6120 636f 6e66 6967 2066 696c  ave a config fil
+0000d440: 6520 7472 7920 6c6f 6164 696e 6720 7468  e try loading th
+0000d450: 6174 0a20 2020 2020 2020 2069 6620 636f  at.        if co
+0000d460: 6e66 6967 6669 6c65 2069 7320 6e6f 7420  nfigfile is not 
+0000d470: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000d480: 2020 636f 6e66 6967 2e72 6561 6428 636f    config.read(co
+0000d490: 6e66 6967 6669 6c65 290a 0a20 2020 2020  nfigfile)..     
+0000d4a0: 2020 2020 2020 2023 2057 6f72 6b20 6f75         # Work ou
+0000d4b0: 7420 7468 6520 686f 7374 2f64 6174 6162  t the host/datab
+0000d4c0: 6173 6520 6966 2077 6520 6b6e 6f77 2069  ase if we know i
+0000d4d0: 740a 2020 2020 2020 2020 2020 2020 686f  t.            ho
+0000d4e0: 7374 5f64 6220 3d20 222c 222e 6a6f 696e  st_db = ",".join
+0000d4f0: 2873 656c 662e 686f 7374 7329 0a20 2020  (self.hosts).   
+0000d500: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000d510: 2e64 6174 6162 6173 6520 6973 206e 6f74  .database is not
+0000d520: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000d530: 2020 2020 2020 2068 6f73 745f 6462 203d         host_db =
+0000d540: 2068 6f73 745f 6462 202b 2022 2f22 202b   host_db + "/" +
+0000d550: 2073 656c 662e 6461 7461 6261 7365 0a0a   self.database..
+0000d560: 2020 2020 2020 2020 2020 2020 2320 5472              # Tr
+0000d570: 7920 616e 6420 6d61 7463 6820 6561 6368  y and match each
+0000d580: 2073 6563 7469 6f6e 2069 6e20 7468 6520   section in the 
+0000d590: 494e 4920 6669 6c65 2077 6974 6820 7468  INI file with th
+0000d5a0: 6520 686f 7374 2f64 6174 6162 6173 650a  e host/database.
+0000d5b0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000d5c0: 7320 696e 2063 6f6e 6669 672e 7365 6374  s in config.sect
+0000d5d0: 696f 6e73 2829 3a0a 2020 2020 2020 2020  ions():.        
+0000d5e0: 2020 2020 2020 2020 6966 2072 652e 6d61          if re.ma
+0000d5f0: 7463 6828 732c 2068 6f73 745f 6462 293a  tch(s, host_db):
+0000d600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d610: 2020 2020 2063 6f6e 6669 6776 616c 7320       configvals 
+0000d620: 3d20 636f 6e66 6967 5b73 5d0a 2020 2020  = config[s].    
+0000d630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d640: 6272 6561 6b0a 0a20 2020 2020 2020 2023  break..        #
+0000d650: 2069 6620 7765 2064 6964 6e27 7420 6669   if we didn't fi
+0000d660: 6e64 2061 206d 6174 6368 696e 6720 686f  nd a matching ho
+0000d670: 7374 2028 6f72 2074 6865 7265 2069 7320  st (or there is 
+0000d680: 6e6f 2066 696c 6529 2e20 7573 6520 7468  no file). use th
+0000d690: 6520 6465 6661 756c 7473 0a20 2020 2020  e defaults.     
+0000d6a0: 2020 2069 6620 636f 6e66 6967 7661 6c73     if configvals
+0000d6b0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0000d6c0: 2020 2020 2020 636f 6e66 6967 7661 6c73        configvals
+0000d6d0: 203d 2063 6f6e 6669 675b 2244 4546 4155   = config["DEFAU
+0000d6e0: 4c54 225d 0a20 2020 2020 2020 2023 2046  LT"].        # F
+0000d6f0: 6f72 6365 2069 7320 6e6f 7420 706c 6163  orce is not plac
+0000d700: 6573 2068 6572 6520 736f 2069 7420 6361  es here so it ca
+0000d710: 6e20 6765 7420 7061 7273 6564 2062 656c  n get parsed bel
+0000d720: 6f77 2e0a 2020 2020 2020 2020 666f 7220  ow..        for 
+0000d730: 6174 7472 2069 6e20 5b22 706f 7274 222c  attr in ["port",
+0000d740: 2022 6461 7461 6261 7365 222c 2022 746c   "database", "tl
+0000d750: 7322 2c20 2268 616e 6473 6861 6b65 225d  s", "handshake"]
+0000d760: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0000d770: 2067 6574 6174 7472 2873 656c 662c 2061   getattr(self, a
+0000d780: 7474 7229 2069 7320 4e6f 6e65 3a0a 2020  ttr) is None:.  
+0000d790: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000d7a0: 7461 7474 7228 7365 6c66 2c20 6174 7472  tattr(self, attr
+0000d7b0: 2c20 636f 6e66 6967 7661 6c73 5b61 7474  , configvals[att
+0000d7c0: 725d 290a 0a20 2020 2020 2020 2069 6620  r])..        if 
+0000d7d0: 6e6f 7420 7365 6c66 2e75 7365 723a 0a20  not self.user:. 
+0000d7e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d7f0: 7573 6572 203d 2073 7472 2863 6f6e 6669  user = str(confi
+0000d800: 6776 616c 732e 6765 7428 2275 7365 7222  gvals.get("user"
+0000d810: 2c20 2222 2929 0a0a 2020 2020 2020 2020  , ""))..        
+0000d820: 6966 206e 6f74 2073 656c 662e 7061 7373  if not self.pass
+0000d830: 776f 7264 3a0a 2020 2020 2020 2020 2020  word:.          
+0000d840: 2020 7365 6c66 2e70 6173 7377 6f72 6420    self.password 
+0000d850: 3d20 7374 7228 636f 6e66 6967 7661 6c73  = str(configvals
+0000d860: 2e67 6574 2822 7061 7373 776f 7264 222c  .get("password",
+0000d870: 2022 2229 290a 0a20 2020 2020 2020 2069   ""))..        i
+0000d880: 6620 7365 6c66 2e66 6f72 6365 2069 7320  f self.force is 
+0000d890: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000d8a0: 2020 7365 6c66 2e66 6f72 6365 203d 2063    self.force = c
+0000d8b0: 6f6e 6669 6776 616c 732e 6765 7462 6f6f  onfigvals.getboo
+0000d8c0: 6c65 616e 2822 666f 7263 6522 290a 0a20  lean("force").. 
+0000d8d0: 2020 2020 2020 2023 2041 6e64 2066 696e         # And fin
+0000d8e0: 616c 6c79 2074 6964 7920 7570 2073 6f6d  ally tidy up som
+0000d8f0: 6520 7468 696e 6773 0a20 2020 2020 2020  e things.       
+0000d900: 2069 6620 6973 696e 7374 616e 6365 2873   if isinstance(s
+0000d910: 656c 662e 706f 7274 2c20 7374 7229 3a0a  elf.port, str):.
+0000d920: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d930: 2e70 6f72 7420 3d20 696e 7428 7365 6c66  .port = int(self
+0000d940: 2e70 6f72 7429 0a0a 2020 2020 2020 2020  .port)..        
+0000d950: 6966 2069 7369 6e73 7461 6e63 6528 7365  if isinstance(se
+0000d960: 6c66 2e74 6c73 2c20 7374 7229 3a0a 2020  lf.tls, str):.  
+0000d970: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000d980: 662e 746c 732e 6c6f 7765 7228 2920 3d3d  f.tls.lower() ==
+0000d990: 2022 6f66 6622 3a0a 2020 2020 2020 2020   "off":.        
+0000d9a0: 2020 2020 2020 2020 7365 6c66 2e74 6c73          self.tls
+0000d9b0: 203d 2073 656c 662e 544c 535f 4e4f 4e45   = self.TLS_NONE
+0000d9c0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+0000d9d0: 6620 7365 6c66 2e74 6c73 2e6c 6f77 6572  f self.tls.lower
+0000d9e0: 2829 203d 3d20 2275 6e76 6572 6966 6965  () == "unverifie
+0000d9f0: 6422 3a0a 2020 2020 2020 2020 2020 2020  d":.            
+0000da00: 2020 2020 7365 6c66 2e74 6c73 203d 2073      self.tls = s
+0000da10: 656c 662e 544c 535f 554e 5645 5249 4649  elf.TLS_UNVERIFI
+0000da20: 4544 0a20 2020 2020 2020 2020 2020 2065  ED.            e
+0000da30: 6c69 6620 7365 6c66 2e74 6c73 2e6c 6f77  lif self.tls.low
+0000da40: 6572 2829 203d 3d20 226f 6e22 3a0a 2020  er() == "on":.  
+0000da50: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000da60: 6c66 2e74 6c73 203d 2073 656c 662e 544c  lf.tls = self.TL
+0000da70: 535f 4f4e 0a20 2020 2020 2020 2020 2020  S_ON.           
+0000da80: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000da90: 2020 2020 2020 2072 6169 7365 204d 616c         raise Mal
+0000daa0: 666f 726d 6564 5552 4c28 6622 496e 7661  formedURL(f"Inva
+0000dab0: 6c69 6420 746c 7320 7661 6c75 653a 207b  lid tls value: {
+0000dac0: 7365 6c66 2e74 6c73 7d22 290a 2020 2020  self.tls}").    
+0000dad0: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
+0000dae0: 6e63 6528 7365 6c66 2e74 6c73 2c20 6c69  nce(self.tls, li
+0000daf0: 7374 293a 0a20 2020 2020 2020 2020 2020  st):.           
+0000db00: 2072 6169 7365 204d 616c 666f 726d 6564   raise Malformed
+0000db10: 5552 4c28 6622 4d75 6c74 6970 6c65 2054  URL(f"Multiple T
+0000db20: 4c53 2076 616c 7565 7320 6465 7465 6374  LS values detect
+0000db30: 6564 3a20 7b73 656c 662e 746c 737d 2229  ed: {self.tls}")
+0000db40: 0a0a 2020 2020 2020 2020 6966 2069 7369  ..        if isi
+0000db50: 6e73 7461 6e63 6528 7365 6c66 2e68 616e  nstance(self.han
+0000db60: 6473 6861 6b65 2c20 7374 7229 3a0a 2020  dshake, str):.  
+0000db70: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000db80: 662e 6861 6e64 7368 616b 652e 6c6f 7765  f.handshake.lowe
+0000db90: 7228 2920 3d3d 2022 6362 6322 3a0a 2020  r() == "cbc":.  
+0000dba0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000dbb0: 6c66 2e68 616e 6473 6861 6b65 203d 2073  lf.handshake = s
+0000dbc0: 656c 662e 4841 4e44 5348 414b 455f 4342  elf.HANDSHAKE_CB
+0000dbd0: 430a 2020 2020 2020 2020 2020 2020 656c  C.            el
+0000dbe0: 6966 2073 656c 662e 6861 6e64 7368 616b  if self.handshak
+0000dbf0: 652e 6c6f 7765 7228 2920 3d3d 2022 7373  e.lower() == "ss
+0000dc00: 6f22 3a0a 2020 2020 2020 2020 2020 2020  o":.            
+0000dc10: 2020 2020 7365 6c66 2e68 616e 6473 6861      self.handsha
+0000dc20: 6b65 203d 2073 656c 662e 4841 4e44 5348  ke = self.HANDSH
+0000dc30: 414b 455f 5353 4f0a 2020 2020 2020 2020  AKE_SSO.        
+0000dc40: 2020 2020 2320 4966 2074 6865 7920 6469      # If they di
+0000dc50: 646e 2774 2073 7065 6369 6679 2068 616e  dn't specify han
+0000dc60: 6473 6861 6b65 2c20 6974 2077 696c 6c20  dshake, it will 
+0000dc70: 6265 2062 6c61 6e6b 2061 6e64 2074 6875  be blank and thu
+0000dc80: 7320 7368 6f75 6c64 2062 6520 4743 4d2e  s should be GCM.
+0000dc90: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+0000dca0: 6620 7365 6c66 2e68 616e 6473 6861 6b65  f self.handshake
+0000dcb0: 2e6c 6f77 6572 2829 203d 3d20 2267 636d  .lower() == "gcm
+0000dcc0: 2220 6f72 2073 656c 662e 6861 6e64 7368  " or self.handsh
+0000dcd0: 616b 652e 6c6f 7765 7228 2920 3d3d 2022  ake.lower() == "
+0000dce0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+0000dcf0: 2020 2073 656c 662e 6861 6e64 7368 616b     self.handshak
+0000dd00: 6520 3d20 7365 6c66 2e48 414e 4453 4841  e = self.HANDSHA
+0000dd10: 4b45 5f47 434d 0a20 2020 2020 2020 2020  KE_GCM.         
+0000dd20: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000dd30: 2020 2020 2020 2020 2070 7269 6e74 2873           print(s
+0000dd40: 656c 662e 6861 6e64 7368 616b 6529 0a20  elf.handshake). 
+0000dd50: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000dd60: 6169 7365 204d 616c 666f 726d 6564 5552  aise MalformedUR
+0000dd70: 4c28 6622 496e 7661 6c69 6420 6861 6e64  L(f"Invalid hand
+0000dd80: 7368 616b 6520 7661 6c75 653a 207b 7365  shake value: {se
+0000dd90: 6c66 2e68 616e 6473 6861 6b65 7d22 290a  lf.handshake}").
+0000dda0: 0a20 2020 2020 2020 2023 2044 6f6e 2774  .        # Don't
+0000ddb0: 2061 7373 6572 7420 6120 7573 6572 2070   assert a user p
+0000ddc0: 6172 616d 6574 6572 2068 6173 2062 6565  arameter has bee
+0000ddd0: 6e20 7365 742e 2041 6e20 656d 7074 790a  n set. An empty.
+0000dde0: 2020 2020 2020 2020 2320 7374 7269 6e67          # string
+0000ddf0: 2066 6f72 2074 6869 7320 6669 656c 6420   for this field 
+0000de00: 6973 2075 7365 6420 666f 7220 6175 7468  is used for auth
+0000de10: 656e 7469 6361 7469 6e67 2053 534f 2075  enticating SSO u
+0000de20: 7365 7273 0a0a 2020 2020 2020 2020 2320  sers..        # 
+0000de30: 446f 6e27 7420 6173 7365 7274 2061 2070  Don't assert a p
+0000de40: 6173 7377 6f72 6420 7061 7261 6d65 7465  assword paramete
+0000de50: 7220 6861 7320 6265 656e 2073 6574 2e20  r has been set. 
+0000de60: 4174 2065 6d70 7479 0a20 2020 2020 2020  At empty.       
+0000de70: 2023 2075 7365 7220 616e 6420 7061 7373   # user and pass
+0000de80: 776f 7264 2069 7320 666f 7220 6175 7468  word is for auth
+0000de90: 656e 7469 6361 7469 6f6e 2066 6c6f 7720  entication flow 
+0000dea0: 7769 7468 2053 534f 2e0a 0a20 2020 2064  with SSO...    d
+0000deb0: 6566 2063 6c6f 7365 2873 656c 6629 202d  ef close(self) -
+0000dec0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000ded0: 2222 2243 6c6f 7365 2074 6865 2063 6f6e  """Close the con
+0000dee0: 6e65 6374 696f 6e2e 2053 7562 7365 7175  nection. Subsequ
+0000def0: 656e 7420 7175 6572 6965 7320 6f6e 2074  ent queries on t
+0000df00: 6869 7320 636f 6e6e 6563 7469 6f6e 0a20  his connection. 
+0000df10: 2020 2020 2020 2077 696c 6c20 6661 696c         will fail
+0000df20: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000df30: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+0000df40: 2e73 6f63 6b3a 0a20 2020 2020 2020 2020  .sock:.         
+0000df50: 2020 2072 6169 7365 2045 7272 6f72 2822     raise Error("
+0000df60: 4e6f 2063 6f6e 6e65 6374 696f 6e22 290a  No connection").
+0000df70: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+0000df80: 2020 2020 2020 2020 2020 2320 5365 6e64            # Send
+0000df90: 2065 6e64 2073 6573 7369 6f6e 206d 6573   end session mes
+0000dfa0: 7361 6765 0a20 2020 2020 2020 2020 2020  sage.           
+0000dfb0: 2072 6571 203d 2070 726f 746f 2e52 6571   req = proto.Req
+0000dfc0: 7565 7374 2829 0a20 2020 2020 2020 2020  uest().         
+0000dfd0: 2020 2072 6571 2e74 7970 6520 3d20 7265     req.type = re
+0000dfe0: 712e 434c 4f53 455f 434f 4e4e 4543 5449  q.CLOSE_CONNECTI
+0000dff0: 4f4e 0a20 2020 2020 2020 2020 2020 2072  ON.            r
+0000e000: 6571 2e63 6c6f 7365 5f63 6f6e 6e65 6374  eq.close_connect
+0000e010: 696f 6e2e 656e 6453 6573 7369 6f6e 203d  ion.endSession =
+0000e020: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
+0000e030: 2020 5f73 656e 645f 6d73 6728 7365 6c66    _send_msg(self
+0000e040: 2c20 7265 7129 0a20 2020 2020 2020 2065  , req).        e
+0000e050: 7863 6570 7420 494f 4572 726f 7220 6173  xcept IOError as
+0000e060: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
+0000e070: 2320 4967 6e6f 7265 2065 6e64 2073 6573  # Ignore end ses
+0000e080: 7369 6f6e 2065 7272 6f72 730a 2020 2020  sion errors.    
+0000e090: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
+0000e0a0: 2020 2020 2066 696e 616c 6c79 3a0a 2020       finally:.  
+0000e0b0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+0000e0c0: 2e64 6562 7567 2866 2243 6c6f 7369 6e67  .debug(f"Closing
+0000e0d0: 2063 6f6e 6e65 6374 696f 6e20 6f6e 2073   connection on s
+0000e0e0: 6f63 6b65 7420 7b73 656c 662e 736f 636b  ocket {self.sock
+0000e0f0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+0000e100: 2320 446f 2074 6869 7320 6c69 7474 6c65  # Do this little
+0000e110: 2064 616e 6365 2073 6f20 7468 6174 2065   dance so that e
+0000e120: 7665 6e20 6966 2074 6865 2063 6c6f 7365  ven if the close
+0000e130: 2829 2063 616c 6c0a 2020 2020 2020 2020  () call.        
+0000e140: 2020 2020 2320 626c 6f77 7320 7570 2c20      # blows up, 
+0000e150: 7765 2068 6176 6520 616c 7265 6164 7920  we have already 
+0000e160: 7365 7420 7365 6c66 2e73 6f63 6b20 746f  set self.sock to
+0000e170: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+0000e180: 2020 736f 636b 203d 2073 656c 662e 736f    sock = self.so
+0000e190: 636b 0a20 2020 2020 2020 2020 2020 2073  ck.            s
+0000e1a0: 656c 662e 736f 636b 203d 204e 6f6e 650a  elf.sock = None.
+0000e1b0: 2020 2020 2020 2020 2020 2020 736f 636b              sock
+0000e1c0: 2e63 6c6f 7365 2829 0a0a 2020 2020 6465  .close()..    de
+0000e1d0: 6620 636f 6d6d 6974 2873 656c 6629 202d  f commit(self) -
+0000e1e0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000e1f0: 2222 2243 6f6d 6d69 7420 6120 7472 616e  """Commit a tran
+0000e200: 7361 6374 696f 6e2e 2043 7572 7265 6e74  saction. Current
+0000e210: 6c79 2069 676e 6f72 6564 2222 220a 0a20  ly ignored""".. 
+0000e220: 2020 2064 6566 2063 7572 736f 7228 7365     def cursor(se
+0000e230: 6c66 2920 2d3e 2022 4375 7273 6f72 223a  lf) -> "Cursor":
+0000e240: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+0000e250: 726e 2061 206e 6577 2063 7572 736f 7220  rn a new cursor 
+0000e260: 666f 7220 7468 6973 2063 6f6e 6e65 6374  for this connect
+0000e270: 696f 6e22 2222 0a20 2020 2020 2020 2069  ion""".        i
+0000e280: 6620 6e6f 7420 7365 6c66 2e73 6f63 6b3a  f not self.sock:
+0000e290: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+0000e2a0: 7365 2045 7272 6f72 2822 4e6f 2063 6f6e  se Error("No con
+0000e2b0: 6e65 6374 696f 6e22 290a 2020 2020 2020  nection").      
+0000e2c0: 2020 7265 7475 726e 2043 7572 736f 7228    return Cursor(
+0000e2d0: 7365 6c66 290a 0a20 2020 2064 6566 205f  self)..    def _
+0000e2e0: 5f64 656c 5f5f 2873 656c 6629 202d 3e20  _del__(self) -> 
+0000e2f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6966  None:.        if
+0000e300: 2073 656c 662e 736f 636b 2069 7320 6e6f   self.sock is no
+0000e310: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000e320: 2020 2020 7365 6c66 2e63 6c6f 7365 2829      self.close()
+0000e330: 0a0a 2020 2020 6465 6620 7265 736f 6c76  ..    def resolv
+0000e340: 655f 6e65 775f 656e 6470 6f69 6e74 2873  e_new_endpoint(s
+0000e350: 656c 662c 206e 6577 5f68 6f73 743a 2073  elf, new_host: s
+0000e360: 7472 2c20 6e65 775f 706f 7274 3a20 696e  tr, new_port: in
+0000e370: 7429 202d 3e20 5475 706c 655b 7374 722c  t) -> Tuple[str,
+0000e380: 2069 6e74 5d3a 0a20 2020 2020 2020 2022   int]:.        "
+0000e390: 2222 0a20 2020 2020 2020 2048 616e 646c  "".        Handl
+0000e3a0: 6573 206d 6170 7069 6e67 2074 6f20 6120  es mapping to a 
+0000e3b0: 7365 636f 6e64 6172 7920 696e 7465 7266  secondary interf
+0000e3c0: 6163 6520 6261 7365 6420 6f6e 2074 6865  ace based on the
+0000e3d0: 2073 6563 6f6e 6461 7279 2069 6e74 6572   secondary inter
+0000e3e0: 6661 6365 206d 6170 7069 6e67 2073 6176  face mapping sav
+0000e3f0: 6564 206f 6e20 7468 6973 2063 6f6e 6e65  ed on this conne
+0000e400: 6374 696f 6e2e 0a0a 2020 2020 2020 2020  ction...        
+0000e410: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+0000e420: 2020 6e65 775f 686f 7374 5b73 7472 696e    new_host[strin
+0000e430: 675d 3a20 7468 6520 6e65 7720 686f 7374  g]: the new host
+0000e440: 2074 6f20 6265 2072 656d 6170 7065 640a   to be remapped.
+0000e450: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+0000e460: 706f 7274 5b69 6e74 5d3a 2074 6865 206e  port[int]: the n
+0000e470: 6577 2070 6f72 7420 746f 2062 6520 7265  ew port to be re
+0000e480: 6d61 7070 6564 0a0a 2020 2020 2020 2020  mapped..        
+0000e490: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+0000e4a0: 2020 2020 205b 7475 706c 6528 7374 7269       [tuple(stri
+0000e4b0: 6e67 2c20 696e 7429 5d3a 2054 6865 2061  ng, int)]: The a
+0000e4c0: 6374 7561 6c20 656e 6470 6f69 6e74 2074  ctual endpoint t
+0000e4d0: 6f20 636f 6e6e 6563 7420 746f 2069 6e20  o connect to in 
+0000e4e0: 7468 6520 666f 726d 6174 3a20 2868 6f73  the format: (hos
+0000e4f0: 742c 2070 6f72 7429 2e0a 2020 2020 2020  t, port)..      
+0000e500: 2020 2222 220a 2020 2020 2020 2020 6c6f    """.        lo
+0000e510: 6767 6572 2e64 6562 7567 280a 2020 2020  gger.debug(.    
+0000e520: 2020 2020 2020 2020 6622 5265 736f 6c76          f"Resolv
+0000e530: 696e 6720 6e65 7720 656e 6470 6f69 6e74  ing new endpoint
+0000e540: 207b 6e65 775f 686f 7374 7d3a 7b6e 6577   {new_host}:{new
+0000e550: 5f70 6f72 747d 2077 6974 6820 7365 636f  _port} with seco
+0000e560: 6e64 6172 795f 696e 6465 7820 7b73 656c  ndary_index {sel
+0000e570: 662e 7365 636f 6e64 6172 795f 696e 6465  f.secondary_inde
+0000e580: 787d 2061 6e64 2073 6563 6f6e 6461 7279  x} and secondary
+0000e590: 5f69 6e74 6572 6661 6365 207b 7365 6c66  _interface {self
+0000e5a0: 2e73 6563 6f6e 6461 7279 5f69 6e74 6572  .secondary_inter
+0000e5b0: 6661 6365 737d 220a 2020 2020 2020 2020  faces}".        
+0000e5c0: 290a 0a20 2020 2020 2020 206e 6577 5f65  )..        new_e
+0000e5d0: 6e64 706f 696e 7420 3d20 286e 6577 5f68  ndpoint = (new_h
+0000e5e0: 6f73 742c 206e 6577 5f70 6f72 7429 0a20  ost, new_port). 
+0000e5f0: 2020 2020 2020 2065 6e64 706f 696e 745f         endpoint_
+0000e600: 746f 5f63 6f6e 6e65 6374 203d 204e 6f6e  to_connect = Non
+0000e610: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+0000e620: 662e 7365 636f 6e64 6172 795f 696e 6465  f.secondary_inde
+0000e630: 7820 213d 202d 313a 0a20 2020 2020 2020  x != -1:.       
+0000e640: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
+0000e650: 2e73 6563 6f6e 6461 7279 5f69 6e74 6572  .secondary_inter
+0000e660: 6661 6365 7320 6973 206e 6f74 204e 6f6e  faces is not Non
+0000e670: 650a 2020 2020 2020 2020 2020 2020 6f75  e.            ou
+0000e680: 7465 725f 696e 6465 7820 3d20 300a 2020  ter_index = 0.  
+0000e690: 2020 2020 2020 2020 2020 666f 7220 6f75            for ou
+0000e6a0: 7465 725f 6c69 7374 2069 6e20 7365 6c66  ter_list in self
+0000e6b0: 2e73 6563 6f6e 6461 7279 5f69 6e74 6572  .secondary_inter
+0000e6c0: 6661 6365 733a 0a20 2020 2020 2020 2020  faces:.         
+0000e6d0: 2020 2020 2020 2069 6620 6f75 7465 725f         if outer_
+0000e6e0: 6c69 7374 5b30 5d20 3d3d 206e 6577 5f65  list[0] == new_e
+0000e6f0: 6e64 706f 696e 743a 0a20 2020 2020 2020  ndpoint:.       
+0000e700: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+0000e710: 616b 0a20 2020 2020 2020 2020 2020 2020  ak.             
+0000e720: 2020 206f 7574 6572 5f69 6e64 6578 202b     outer_index +
+0000e730: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
+0000e740: 6966 206f 7574 6572 5f69 6e64 6578 203c  if outer_index <
+0000e750: 206c 656e 2873 656c 662e 7365 636f 6e64   len(self.second
+0000e760: 6172 795f 696e 7465 7266 6163 6573 293a  ary_interfaces):
+0000e770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e780: 2065 6e64 706f 696e 745f 746f 5f63 6f6e   endpoint_to_con
+0000e790: 6e65 6374 203d 2073 656c 662e 7365 636f  nect = self.seco
+0000e7a0: 6e64 6172 795f 696e 7465 7266 6163 6573  ndary_interfaces
+0000e7b0: 5b6f 7574 6572 5f69 6e64 6578 5d5b 7365  [outer_index][se
+0000e7c0: 6c66 2e73 6563 6f6e 6461 7279 5f69 6e64  lf.secondary_ind
+0000e7d0: 6578 5d0a 2020 2020 2020 2020 2020 2020  ex].            
+0000e7e0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000e7f0: 2020 2020 2020 656e 6470 6f69 6e74 5f74        endpoint_t
+0000e800: 6f5f 636f 6e6e 6563 7420 3d20 6e65 775f  o_connect = new_
+0000e810: 656e 6470 6f69 6e74 0a0a 2020 2020 2020  endpoint..      
+0000e820: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000e830: 2020 2020 656e 6470 6f69 6e74 5f74 6f5f      endpoint_to_
+0000e840: 636f 6e6e 6563 7420 3d20 6e65 775f 656e  connect = new_en
+0000e850: 6470 6f69 6e74 0a0a 2020 2020 2020 2020  dpoint..        
+0000e860: 6c6f 6767 6572 2e64 6562 7567 2866 2252  logger.debug(f"R
+0000e870: 6573 6f6c 7665 6420 6e65 7720 656e 6470  esolved new endp
+0000e880: 6f69 6e74 207b 6e65 775f 686f 7374 7d3a  oint {new_host}:
+0000e890: 7b6e 6577 5f70 6f72 747d 2074 6f20 7b65  {new_port} to {e
+0000e8a0: 6e64 706f 696e 745f 746f 5f63 6f6e 6e65  ndpoint_to_conne
+0000e8b0: 6374 7d22 290a 0a20 2020 2020 2020 2072  ct}")..        r
+0000e8c0: 6574 7572 6e20 656e 6470 6f69 6e74 5f74  eturn endpoint_t
+0000e8d0: 6f5f 636f 6e6e 6563 740a 0a20 2020 2064  o_connect..    d
+0000e8e0: 6566 2072 6564 6972 6563 7428 7365 6c66  ef redirect(self
+0000e8f0: 2c20 6e65 775f 686f 7374 3a20 7374 722c  , new_host: str,
+0000e900: 206e 6577 5f70 6f72 743a 2069 6e74 2920   new_port: int) 
+0000e910: 2d3e 2022 436f 6e6e 6563 7469 6f6e 223a  -> "Connection":
+0000e920: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000e930: 2020 2020 2052 6564 6972 6563 7473 2074       Redirects t
+0000e940: 6f20 7468 6520 7072 6f70 6572 2073 6563  o the proper sec
+0000e950: 6f6e 6461 7279 2069 6e74 6572 6661 6365  ondary interface
+0000e960: 2067 6976 656e 2061 206e 6577 2065 6e64   given a new end
+0000e970: 706f 696e 742e 0a0a 2020 2020 2020 2020  point...        
+0000e980: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+0000e990: 2020 6e65 775f 686f 7374 5b73 7472 696e    new_host[strin
+0000e9a0: 675d 3a20 7468 6520 6e65 7720 686f 7374  g]: the new host
+0000e9b0: 2074 6f20 6265 2072 656d 6170 7065 640a   to be remapped.
+0000e9c0: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+0000e9d0: 706f 7274 5b69 6e74 5d3a 2074 6865 206e  port[int]: the n
+0000e9e0: 6577 2070 6f72 7420 746f 2062 6520 7265  ew port to be re
+0000e9f0: 6d61 7070 6564 0a0a 2020 2020 2020 2020  mapped..        
+0000ea00: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+0000ea10: 2020 2020 205b 436f 6e6e 6563 7469 6f6e       [Connection
+0000ea20: 5d3a 2041 206e 6577 2063 6f6e 6e65 6374  ]: A new connect
+0000ea30: 696f 6e2e 0a20 2020 2020 2020 2022 2222  ion..        """
+0000ea40: 0a20 2020 2020 2020 2072 656d 6170 7065  .        remappe
+0000ea50: 645f 686f 7374 2c20 7265 6d61 7070 6564  d_host, remapped
+0000ea60: 5f70 6f72 7420 3d20 7365 6c66 2e72 6573  _port = self.res
+0000ea70: 6f6c 7665 5f6e 6577 5f65 6e64 706f 696e  olve_new_endpoin
+0000ea80: 7428 6e65 775f 686f 7374 2c20 6e65 775f  t(new_host, new_
+0000ea90: 706f 7274 290a 2020 2020 2020 2020 6e65  port).        ne
+0000eaa0: 775f 656e 6470 6f69 6e74 203d 2066 227b  w_endpoint = f"{
+0000eab0: 7265 6d61 7070 6564 5f68 6f73 747d 3a7b  remapped_host}:{
+0000eac0: 7265 6d61 7070 6564 5f70 6f72 747d 220a  remapped_port}".
+0000ead0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000eae0: 6562 7567 2866 2252 6564 6972 6563 7469  ebug(f"Redirecti
+0000eaf0: 6e67 2063 6f6e 6e65 6374 696f 6e20 746f  ng connection to
+0000eb00: 207b 6e65 775f 686f 7374 7d3a 7b6e 6577   {new_host}:{new
+0000eb10: 5f70 6f72 747d 2c20 7768 6963 6820 6d61  _port}, which ma
+0000eb20: 7073 2074 6f20 7b72 656d 6170 7065 645f  ps to {remapped_
+0000eb30: 686f 7374 7d3a 7b72 656d 6170 7065 645f  host}:{remapped_
+0000eb40: 706f 7274 7d22 290a 0a20 2020 2020 2020  port}")..       
+0000eb50: 2072 6574 7572 6e20 436f 6e6e 6563 7469   return Connecti
+0000eb60: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+0000eb70: 7573 6572 3d73 656c 662e 7573 6572 2c0a  user=self.user,.
+0000eb80: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+0000eb90: 776f 7264 3d73 656c 662e 7061 7373 776f  word=self.passwo
+0000eba0: 7264 2c0a 2020 2020 2020 2020 2020 2020  rd,.            
+0000ebb0: 686f 7374 3d6e 6577 5f65 6e64 706f 696e  host=new_endpoin
+0000ebc0: 742c 0a20 2020 2020 2020 2020 2020 2064  t,.            d
+0000ebd0: 6174 6162 6173 653d 7365 6c66 2e64 6174  atabase=self.dat
+0000ebe0: 6162 6173 652c 0a20 2020 2020 2020 2020  abase,.         
+0000ebf0: 2020 2074 6c73 3d73 656c 662e 746c 732c     tls=self.tls,
+0000ec00: 0a20 2020 2020 2020 2020 2020 2068 616e  .            han
+0000ec10: 6473 6861 6b65 3d73 656c 662e 6861 6e64  dshake=self.hand
+0000ec20: 7368 616b 652c 0a20 2020 2020 2020 2020  shake,.         
+0000ec30: 2020 2066 6f72 6365 3d73 656c 662e 666f     force=self.fo
+0000ec40: 7263 652c 0a20 2020 2020 2020 2020 2020  rce,.           
+0000ec50: 2073 6573 7369 6f6e 3d73 656c 662e 7365   session=self.se
+0000ec60: 7373 696f 6e2c 0a20 2020 2020 2020 2029  ssion,.        )
+0000ec70: 0a0a 2020 2020 6465 6620 7265 6672 6573  ..    def refres
+0000ec80: 6828 7365 6c66 2920 2d3e 204e 6f6e 653a  h(self) -> None:
+0000ec90: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000eca0: 2020 2020 2055 7365 6420 746f 2072 6566       Used to ref
+0000ecb0: 7265 7368 2074 6865 2073 6573 7369 6f6e  resh the session
+0000ecc0: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
+0000ecd0: 2074 6869 7320 636f 6e6e 6563 7469 6f6e   this connection
+0000ece0: 2e20 5468 6520 7365 7276 6572 2077 696c  . The server wil
+0000ecf0: 6c0a 2020 2020 2020 2020 7265 7475 726e  l.        return
+0000ed00: 2061 206e 6577 2073 6572 7665 7220 7365   a new server se
+0000ed10: 7373 696f 6e20 6964 2061 6e64 2073 6563  ssion id and sec
+0000ed20: 7572 6974 7920 746f 6b65 6e2e 0a20 2020  urity token..   
+0000ed30: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000ed40: 2072 6571 203d 2070 726f 746f 2e52 6571   req = proto.Req
+0000ed50: 7565 7374 2829 0a20 2020 2020 2020 2072  uest().        r
+0000ed60: 6571 2e74 7970 6520 3d20 7265 712e 434c  eq.type = req.CL
+0000ed70: 4945 4e54 5f43 4f4e 4e45 4354 494f 4e5f  IENT_CONNECTION_
+0000ed80: 5245 4652 4553 485f 5345 5353 494f 4e0a  REFRESH_SESSION.
+0000ed90: 0a20 2020 2020 2020 2023 2053 656e 6420  .        # Send 
+0000eda0: 6d65 7373 6167 650a 2020 2020 2020 2020  message.        
+0000edb0: 5f73 656e 645f 6d73 6728 7365 6c66 2c20  _send_msg(self, 
+0000edc0: 7265 7129 0a20 2020 2020 2020 2023 2052  req).        # R
+0000edd0: 6563 6569 7665 206d 6573 7361 6765 0a20  eceive message. 
+0000ede0: 2020 2020 2020 2072 7370 203d 205f 7265         rsp = _re
+0000edf0: 6376 5f6d 7367 2873 656c 662c 2070 726f  cv_msg(self, pro
+0000ee00: 746f 2e43 6c69 656e 7443 6f6e 6e65 6374  to.ClientConnect
+0000ee10: 696f 6e52 6566 7265 7368 5365 7373 696f  ionRefreshSessio
+0000ee20: 6e52 6573 706f 6e73 6528 2929 0a0a 2020  nResponse())..  
+0000ee30: 2020 2020 2020 6966 2072 7370 2e72 6573        if rsp.res
+0000ee40: 706f 6e73 652e 7479 7065 203d 3d20 7072  ponse.type == pr
+0000ee50: 6f74 6f2e 436f 6e66 6972 6d61 7469 6f6e  oto.Confirmation
+0000ee60: 5265 7370 6f6e 7365 2e52 4553 504f 4e53  Response.RESPONS
+0000ee70: 455f 5741 524e 3a0a 2020 2020 2020 2020  E_WARN:.        
+0000ee80: 2020 2020 7761 726e 2872 7370 2e72 6573      warn(rsp.res
+0000ee90: 706f 6e73 652e 7265 6173 6f6e 290a 2020  ponse.reason).  
+0000eea0: 2020 2020 2020 656c 6966 2072 7370 2e72        elif rsp.r
+0000eeb0: 6573 706f 6e73 652e 7479 7065 203d 3d20  esponse.type == 
+0000eec0: 7072 6f74 6f2e 436f 6e66 6972 6d61 7469  proto.Confirmati
+0000eed0: 6f6e 5265 7370 6f6e 7365 2e52 4553 504f  onResponse.RESPO
+0000eee0: 4e53 455f 4f4b 3a0a 2020 2020 2020 2020  NSE_OK:.        
+0000eef0: 2020 2020 2320 4361 7074 7572 6520 7468      # Capture th
+0000ef00: 6520 7365 7373 696f 6e20 6964 0a20 2020  e session id.   
+0000ef10: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+0000ef20: 7276 6572 5365 7373 696f 6e49 6420 3d20  rverSessionId = 
+0000ef30: 7273 702e 7365 7373 696f 6e49 6e66 6f2e  rsp.sessionInfo.
+0000ef40: 7365 7276 6572 5365 7373 696f 6e49 640a  serverSessionId.
+0000ef50: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+0000ef60: 6572 2e64 6562 7567 2866 2243 6f6e 6e65  er.debug(f"Conne
+0000ef70: 6374 6564 2074 6f20 7365 7276 6572 2073  cted to server s
+0000ef80: 6573 7369 6f6e 2049 643a 207b 7365 6c66  ession Id: {self
+0000ef90: 2e73 6572 7665 7253 6573 7369 6f6e 4964  .serverSessionId
+0000efa0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+0000efb0: 7265 6365 6976 6564 5f74 6f6b 656e 203d  received_token =
+0000efc0: 2072 7370 2e73 6573 7369 6f6e 496e 666f   rsp.sessionInfo
+0000efd0: 2e73 6563 7572 6974 7954 6f6b 656e 0a20  .securityToken. 
+0000efe0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000eff0: 6c66 2e73 6573 7369 6f6e 2069 7320 6e6f  lf.session is no
+0000f000: 7420 4e6f 6e65 2061 6e64 2073 656c 662e  t None and self.
+0000f010: 7365 7373 696f 6e2e 7365 6375 7269 7479  session.security
+0000f020: 546f 6b65 6e20 6973 206e 6f74 204e 6f6e  Token is not Non
+0000f030: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000f040: 2020 2073 656c 662e 7365 7373 696f 6e20     self.session 
+0000f050: 3d20 5365 7373 696f 6e28 0a20 2020 2020  = Session(.     
+0000f060: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000f070: 6563 7572 6974 7954 6f6b 656e 3d53 6563  ecurityToken=Sec
+0000f080: 7572 6974 7954 6f6b 656e 280a 2020 2020  urityToken(.    
+0000f090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0a0: 2020 2020 7265 6365 6976 6564 5f74 6f6b      received_tok
+0000f0b0: 656e 2e64 6174 612c 0a20 2020 2020 2020  en.data,.       
+0000f0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0d0: 2072 6563 6569 7665 645f 746f 6b65 6e2e   received_token.
+0000f0e0: 7369 676e 6174 7572 652c 0a20 2020 2020  signature,.     
+0000f0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f100: 2020 2072 6563 6569 7665 645f 746f 6b65     received_toke
+0000f110: 6e2e 6973 7375 6572 4669 6e67 6572 7072  n.issuerFingerpr
+0000f120: 696e 742c 0a20 2020 2020 2020 2020 2020  int,.           
+0000f130: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000f140: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000f150: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000f160: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000f170: 2049 676e 6f72 6520 7468 6520 7365 6375   Ignore the secu
+0000f180: 7269 7479 2074 6f6b 656e 0a20 2020 2020  rity token.     
+0000f190: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+0000f1a0: 7420 7365 6c66 2e75 7365 7220 6973 206e  t self.user is n
+0000f1b0: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
+0000f1c0: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
+0000f1d0: 656c 662e 7061 7373 776f 7264 2069 7320  elf.password is 
+0000f1e0: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
+0000f1f0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+0000f200: 7373 696f 6e20 3d20 5365 7373 696f 6e28  ssion = Session(
+0000f210: 7573 6572 416e 6450 6173 7377 6f72 643d  userAndPassword=
+0000f220: 5573 6572 416e 6450 6173 7377 6f72 6428  UserAndPassword(
+0000f230: 7365 6c66 2e75 7365 722c 2073 656c 662e  self.user, self.
+0000f240: 7061 7373 776f 7264 2929 0a20 2020 2020  password)).     
+0000f250: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+0000f260: 2020 2020 2020 2320 536f 6d65 7468 696e        # Somethin
+0000f270: 6720 6261 6420 6861 7070 656e 6564 2077  g bad happened w
+0000f280: 6974 6820 7468 6520 7265 6672 6573 6820  ith the refresh 
+0000f290: 6174 7465 6d70 742e 0a20 2020 2020 2020  attempt..       
+0000f2a0: 2072 6169 7365 205f 636f 6e76 6572 745f   raise _convert_
+0000f2b0: 6578 6365 7074 696f 6e28 7273 702e 7265  exception(rsp.re
+0000f2c0: 7370 6f6e 7365 290a 0a0a 636c 6173 7320  sponse)...class 
+0000f2d0: 4375 7273 6f72 3a0a 2020 2020 2320 7079  Cursor:.    # py
+0000f2e0: 6c69 6e74 3a20 6469 7361 626c 653d 746f  lint: disable=to
+0000f2f0: 6f2d 6d61 6e79 2d69 6e73 7461 6e63 652d  o-many-instance-
+0000f300: 6174 7472 6962 7574 6573 0a20 2020 2022  attributes.    "
+0000f310: 2222 4120 6461 7461 6261 7365 2063 7572  ""A database cur
+0000f320: 736f 722c 2077 6869 6368 2069 7320 7573  sor, which is us
+0000f330: 6564 2074 6f20 6d61 6e61 6765 2061 2071  ed to manage a q
+0000f340: 7565 7279 2061 6e64 2069 7473 2072 6574  uery and its ret
+0000f350: 7572 6e65 6420 7265 7375 6c74 7322 2222  urned results"""
+0000f360: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+0000f370: 5f5f 2873 656c 662c 2063 6f6e 6e3a 2043  __(self, conn: C
+0000f380: 6f6e 6e65 6374 696f 6e29 202d 3e20 4e6f  onnection) -> No
+0000f390: 6e65 3a0a 2020 2020 2020 2020 2222 2243  ne:.        """C
+0000f3a0: 7572 736f 7273 2061 7265 206e 6f72 6d61  ursors are norma
+0000f3b0: 6c6c 7920 6372 6561 7465 6420 6279 2074  lly created by t
+0000f3c0: 6865 2063 7572 736f 7228 2920 6361 6c6c  he cursor() call
+0000f3d0: 206f 6e20 6120 636f 6e6e 6563 7469 6f6e   on a connection
+0000f3e0: 2c20 6275 7420 6361 6e0a 2020 2020 2020  , but can.      
+0000f3f0: 2020 6265 2063 7265 6174 6564 2064 6972    be created dir
+0000f400: 6563 746c 7920 6279 2070 726f 7669 6469  ectly by providi
+0000f410: 6e67 2061 2063 6f6e 6e65 6374 696f 6e0a  ng a connection.
+0000f420: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000f430: 2020 2020 7365 6c66 2e63 6f6e 6e65 6374      self.connect
+0000f440: 696f 6e20 3d20 636f 6e6e 0a20 2020 2020  ion = conn.     
+0000f450: 2020 2073 656c 662e 6172 7261 7973 697a     self.arraysiz
+0000f460: 6520 3d20 310a 0a20 2020 2020 2020 2073  e = 1..        s
+0000f470: 656c 662e 5f72 6569 6e69 7469 616c 697a  elf._reinitializ
+0000f480: 6528 290a 0a20 2020 2064 6566 205f 5f64  e()..    def __d
+0000f490: 656c 5f5f 2873 656c 6629 202d 3e20 4e6f  el__(self) -> No
+0000f4a0: 6e65 3a0a 2020 2020 2020 2020 7472 793a  ne:.        try:
+0000f4b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000f4c0: 662e 5f63 6c6f 7365 5f72 6573 756c 7473  f._close_results
+0000f4d0: 6574 2829 0a20 2020 2020 2020 2065 7863  et().        exc
+0000f4e0: 6570 7420 4578 6365 7074 696f 6e3a 0a20  ept Exception:. 
+0000f4f0: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
+0000f500: 0a20 2020 2064 6566 205f 5f65 6e74 6572  .    def __enter
+0000f510: 5f5f 2873 656c 6629 202d 3e20 2243 7572  __(self) -> "Cur
+0000f520: 736f 7222 3a0a 2020 2020 2020 2020 7265  sor":.        re
+0000f530: 7475 726e 2073 656c 660a 0a20 2020 2064  turn self..    d
+0000f540: 6566 205f 5f65 7869 745f 5f28 0a20 2020  ef __exit__(.   
+0000f550: 2020 2020 2073 656c 662c 2065 7863 5f74       self, exc_t
+0000f560: 7970 653a 204f 7074 696f 6e61 6c5b 5479  ype: Optional[Ty
+0000f570: 7065 5b42 6173 6545 7863 6570 7469 6f6e  pe[BaseException
+0000f580: 5d5d 2c20 6578 635f 7661 6c3a 204f 7074  ]], exc_val: Opt
+0000f590: 696f 6e61 6c5b 4261 7365 4578 6365 7074  ional[BaseExcept
+0000f5a0: 696f 6e5d 2c20 6578 635f 7462 3a20 4f70  ion], exc_tb: Op
+0000f5b0: 7469 6f6e 616c 5b54 7261 6365 6261 636b  tional[Traceback
+0000f5c0: 5479 7065 5d0a 2020 2020 2920 2d3e 204e  Type].    ) -> N
+0000f5d0: 6f6e 653a 0a20 2020 2020 2020 2070 6173  one:.        pas
+0000f5e0: 730a 0a20 2020 2064 6566 205f 7265 696e  s..    def _rein
+0000f5f0: 6974 6961 6c69 7a65 2873 656c 6629 202d  itialize(self) -
+0000f600: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000f610: 2222 2249 6e74 6572 6e61 6c20 6675 6e63  """Internal func
+0000f620: 7469 6f6e 2074 6f20 696e 6974 6961 6c69  tion to initiali
+0000f630: 7a65 2061 2063 7572 736f 7222 2222 0a20  ze a cursor""". 
+0000f640: 2020 2020 2020 2023 2053 6574 2074 6865         # Set the
+0000f650: 2073 7461 7465 0a20 2020 2020 2020 2073   state.        s
+0000f660: 656c 662e 7175 6572 795f 6964 203d 204e  elf.query_id = N
+0000f670: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+0000f680: 2e72 6f77 636f 756e 7420 3d20 2d31 0a20  .rowcount = -1. 
+0000f690: 2020 2020 2020 2073 656c 662e 726f 776e         self.rown
+0000f6a0: 756d 6265 723a 204f 7074 696f 6e61 6c5b  umber: Optional[
+0000f6b0: 696e 745d 203d 204e 6f6e 650a 2020 2020  int] = None.    
+0000f6c0: 2020 2020 7365 6c66 2e72 6573 756c 7473      self.results
+0000f6d0: 6574 5f74 7570 6c65 3a20 4f70 7469 6f6e  et_tuple: Option
+0000f6e0: 616c 5b54 7970 655b 4e61 6d65 6454 7570  al[Type[NamedTup
+0000f6f0: 6c65 5d5d 203d 204e 6f6e 650a 2020 2020  le]] = None.    
+0000f700: 2020 2020 7365 6c66 2e64 6573 6372 6970      self.descrip
+0000f710: 7469 6f6e 3a20 4f70 7469 6f6e 616c 5b4c  tion: Optional[L
+0000f720: 6973 745b 5475 706c 655b 7374 722c 2069  ist[Tuple[str, i
+0000f730: 6e74 2c20 4e6f 6e65 2c20 4e6f 6e65 2c20  nt, None, None, 
+0000f740: 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65  None, None, None
+0000f750: 5d5d 5d20 3d20 4e6f 6e65 0a20 2020 2020  ]]] = None.     
+0000f760: 2020 2073 656c 662e 656e 645f 6f66 5f64     self.end_of_d
+0000f770: 6174 6120 3d20 4661 6c73 650a 2020 2020  ata = False.    
+0000f780: 2020 2020 7365 6c66 2e67 656e 6572 6174      self.generat
+0000f790: 6564 5f72 6573 756c 743a 204f 7074 696f  ed_result: Optio
+0000f7a0: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+0000f7b0: 2020 2020 2020 2020 7365 6c66 2e6c 6973          self.lis
+0000f7c0: 745f 7265 7375 6c74 3a20 4f70 7469 6f6e  t_result: Option
+0000f7d0: 616c 5b4c 6973 745b 4e61 6d65 6454 7570  al[List[NamedTup
+0000f7e0: 6c65 5d5d 203d 204e 6f6e 650a 2020 2020  le]] = None.    
+0000f7f0: 2020 2020 7365 6c66 2e5f 6275 6666 6572      self._buffer
+0000f800: 733a 204c 6973 745b 6279 7465 735d 203d  s: List[bytes] =
+0000f810: 205b 5d0a 2020 2020 2020 2020 7365 6c66   [].        self
+0000f820: 2e5f 6f66 6673 6574 203d 2030 0a20 2020  ._offset = 0.   
+0000f830: 2020 2020 2073 656c 662e 5f70 656e 6469       self._pendi
+0000f840: 6e67 5f6f 7073 3a20 4c69 7374 5b73 7472  ng_ops: List[str
+0000f850: 5d20 3d20 5b5d 0a0a 2020 2020 6465 6620  ] = []..    def 
+0000f860: 7365 7469 6e70 7574 7369 7a65 7328 7365  setinputsizes(se
+0000f870: 6c66 2c20 7369 7a65 733a 2053 6571 7565  lf, sizes: Seque
+0000f880: 6e63 655b 4f70 7469 6f6e 616c 5b69 6e74  nce[Optional[int
+0000f890: 5d5d 2920 2d3e 204e 6f6e 653a 0a20 2020  ]]) -> None:.   
+0000f8a0: 2020 2020 2022 2222 5468 6973 2063 616e       """This can
+0000f8b0: 2062 6520 7573 6564 2062 6566 6f72 6520   be used before 
+0000f8c0: 6120 6361 6c6c 2074 6f20 2e65 7865 6375  a call to .execu
+0000f8d0: 7465 2a28 2920 746f 2070 7265 6465 6669  te*() to predefi
+0000f8e0: 6e65 0a20 2020 2020 2020 206d 656d 6f72  ne.        memor
+0000f8f0: 7920 6172 6561 7320 666f 7220 7468 6520  y areas for the 
+0000f900: 6f70 6572 6174 696f 6e27 7320 7061 7261  operation's para
+0000f910: 6d65 7465 7273 2e20 4375 7272 656e 746c  meters. Currentl
+0000f920: 7920 6967 6e6f 7265 640a 2020 2020 2020  y ignored.      
+0000f930: 2020 2222 220a 0a20 2020 2064 6566 2073    """..    def s
+0000f940: 6574 6f75 7470 7574 7369 7a65 2873 656c  etoutputsize(sel
+0000f950: 662c 2073 697a 653a 2069 6e74 2c20 636f  f, size: int, co
+0000f960: 6c75 6d6e 3a20 4f70 7469 6f6e 616c 5b69  lumn: Optional[i
+0000f970: 6e74 5d20 3d20 4e6f 6e65 2920 2d3e 204e  nt] = None) -> N
+0000f980: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+0000f990: 5365 7420 6120 636f 6c75 6d6e 2062 7566  Set a column buf
+0000f9a0: 6665 7220 7369 7a65 2066 6f72 2066 6574  fer size for fet
+0000f9b0: 6368 6573 206f 6620 6c61 7267 6520 636f  ches of large co
+0000f9c0: 6c75 6d6e 730a 2020 2020 2020 2020 2865  lumns.        (e
+0000f9d0: 2e67 2e20 4c4f 4e47 732c 2042 4c4f 4273  .g. LONGs, BLOBs
+0000f9e0: 2c20 6574 632e 292e 2054 6865 2063 6f6c  , etc.). The col
+0000f9f0: 756d 6e20 6973 2073 7065 6369 6669 6564  umn is specified
+0000fa00: 2061 7320 616e 0a20 2020 2020 2020 2069   as an.        i
+0000fa10: 6e64 6578 2069 6e74 6f20 7468 6520 7265  ndex into the re
+0000fa20: 7375 6c74 2073 6571 7565 6e63 652e 2043  sult sequence. C
+0000fa30: 7572 7265 6e74 6c79 2069 676e 6f72 6564  urrently ignored
+0000fa40: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+0000fa50: 2020 6465 6620 636c 6f73 6528 7365 6c66    def close(self
+0000fa60: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0000fa70: 2020 2022 2222 436c 6f73 6520 7468 6973     """Close this
+0000fa80: 2063 7572 736f 722e 2020 5468 6520 6375   cursor.  The cu
+0000fa90: 7272 656e 7420 7265 7375 6c74 2073 6574  rrent result set
+0000faa0: 2069 7320 636c 6f73 6564 2c20 6275 740a   is closed, but.
+0000fab0: 2020 2020 2020 2020 7468 6520 6375 7273          the curs
+0000fac0: 6f72 2063 616e 2062 6520 7265 7573 6564  or can be reused
+0000fad0: 2066 6f72 2073 7562 7365 7175 656e 7420   for subsequent 
+0000fae0: 6578 6563 7574 6528 2920 6361 6c6c 732e  execute() calls.
+0000faf0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000fb00: 2020 2020 2069 6620 7365 6c66 2e5f 6275       if self._bu
+0000fb10: 6666 6572 733a 0a20 2020 2020 2020 2020  ffers:.         
+0000fb20: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0000fb30: 2020 2020 2020 2020 7365 6c66 2e5f 636c          self._cl
+0000fb40: 6f73 655f 7265 7375 6c74 7365 7428 290a  ose_resultset().
+0000fb50: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+0000fb60: 7074 2045 7863 6570 7469 6f6e 3a0a 2020  pt Exception:.  
+0000fb70: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+0000fb80: 7373 0a0a 2020 2020 2020 2020 7365 6c66  ss..        self
+0000fb90: 2e5f 7265 696e 6974 6961 6c69 7a65 2829  ._reinitialize()
+0000fba0: 0a0a 2020 2020 6465 6620 6578 6563 7574  ..    def execut
+0000fbb0: 656d 616e 7928 0a20 2020 2020 2020 2073  emany(.        s
+0000fbc0: 656c 662c 206f 7065 7261 7469 6f6e 3a20  elf, operation: 
+0000fbd0: 556e 696f 6e5b 7374 722c 2062 7974 6573  Union[str, bytes
+0000fbe0: 5d2c 2070 6172 616d 6574 6572 6c69 7374  ], parameterlist
+0000fbf0: 3a20 4974 6572 6162 6c65 5b4d 6170 7069  : Iterable[Mappi
+0000fc00: 6e67 5b55 6e69 6f6e 5b73 7472 2c20 6279  ng[Union[str, by
+0000fc10: 7465 735d 2c20 6f62 6a65 6374 5d5d 0a20  tes], object]]. 
+0000fc20: 2020 2029 202d 3e20 2243 7572 736f 7222     ) -> "Cursor"
+0000fc30: 3a0a 2020 2020 2020 2020 2222 2250 7265  :.        """Pre
+0000fc40: 7061 7265 2061 2064 6174 6162 6173 6520  pare a database 
+0000fc50: 6f70 6572 6174 696f 6e20 2871 7565 7279  operation (query
+0000fc60: 206f 7220 636f 6d6d 616e 6429 2061 6e64   or command) and
+0000fc70: 2074 6865 6e20 6578 6563 7574 6520 6974   then execute it
+0000fc80: 2061 6761 696e 7374 0a20 2020 2020 2020   against.       
+0000fc90: 2061 6c6c 2070 6172 616d 6574 6572 2073   all parameter s
+0000fca0: 6571 7565 6e63 6573 206f 7220 6d61 7070  equences or mapp
+0000fcb0: 696e 6773 2066 6f75 6e64 2069 6e20 7468  ings found in th
+0000fcc0: 6520 7365 7175 656e 6365 2070 6172 616d  e sequence param
+0000fcd0: 6574 6572 6c69 7374 2e0a 0a20 2020 2020  eterlist...     
+0000fce0: 2020 2050 6172 616d 6574 6572 7320 6d61     Parameters ma
+0000fcf0: 7920 6265 2070 726f 7669 6465 6420 6173  y be provided as
+0000fd00: 2061 206d 6170 7069 6e67 2061 6e64 2077   a mapping and w
+0000fd10: 696c 6c20 6265 2062 6f75 6e64 2074 6f20  ill be bound to 
+0000fd20: 7661 7269 6162 6c65 730a 2020 2020 2020  variables.      
+0000fd30: 2020 696e 2074 6865 206f 7065 7261 7469    in the operati
+0000fd40: 6f6e 2e20 5661 7269 6162 6c65 7320 6172  on. Variables ar
+0000fd50: 6520 7370 6563 6966 6965 6420 696e 2050  e specified in P
+0000fd60: 7974 686f 6e20 6578 7465 6e64 6564 2066  ython extended f
+0000fd70: 6f72 6d61 7420 636f 6465 732c 0a20 2020  ormat codes,.   
+0000fd80: 2020 2020 2065 2e67 2e20 2e2e 2e57 4845       e.g. ...WHE
+0000fd90: 5245 206e 616d 653d 2528 6e61 6d65 2973  RE name=%(name)s
+0000fda0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000fdb0: 2020 2020 2073 656c 662e 5f72 6569 6e69       self._reini
+0000fdc0: 7469 616c 697a 6528 290a 0a20 2020 2020  tialize()..     
+0000fdd0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+0000fde0: 286f 7065 7261 7469 6f6e 2c20 6279 7465  (operation, byte
+0000fdf0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+0000fe00: 6f70 6572 6174 696f 6e20 3d20 6f70 6572  operation = oper
+0000fe10: 6174 696f 6e2e 6465 636f 6465 2829 0a0a  ation.decode()..
+0000fe20: 2020 2020 2020 2020 2320 7765 2063 616e          # we can
+0000fe30: 2774 206a 7573 7420 6578 6563 7574 6520  't just execute 
+0000fe40: 616c 6c20 7468 6520 7175 6572 6965 7320  all the queries 
+0000fe50: 6174 206f 6e63 652e 2e2e 2e6f 6369 656e  at once....ocien
+0000fe60: 7420 6f6e 6c79 2061 6c6c 6f77 730a 2020  t only allows.  
+0000fe70: 2020 2020 2020 2320 6f6e 6520 7175 6572        # one quer
+0000fe80: 7920 6174 2061 2074 696d 6520 6f6e 2061  y at a time on a
+0000fe90: 2063 6f6e 6e65 6374 696f 6e2e 2020 536f   connection.  So
+0000fea0: 2071 7565 7565 2075 7020 616c 6c20 7468   queue up all th
+0000feb0: 6520 7175 6572 6965 7320 616e 640a 2020  e queries and.  
+0000fec0: 2020 2020 2020 2320 7765 276c 6c20 6361        # we'll ca
+0000fed0: 6c6c 2074 6865 6d20 6c61 7465 720a 2020  ll them later.  
+0000fee0: 2020 2020 2020 666f 7220 7061 7261 6d20        for param 
+0000fef0: 696e 2070 6172 616d 6574 6572 6c69 7374  in parameterlist
+0000ff00: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
+0000ff10: 7261 6d20 3d20 7b6b 6579 2e64 6563 6f64  ram = {key.decod
+0000ff20: 6528 2920 6966 2069 7369 6e73 7461 6e63  e() if isinstanc
+0000ff30: 6528 6b65 792c 2062 7974 6573 2920 656c  e(key, bytes) el
+0000ff40: 7365 206b 6579 3a20 7661 6c75 6520 666f  se key: value fo
+0000ff50: 7220 286b 6579 2c20 7661 6c75 6529 2069  r (key, value) i
+0000ff60: 6e20 7061 7261 6d2e 6974 656d 7328 297d  n param.items()}
+0000ff70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000ff80: 662e 5f70 656e 6469 6e67 5f6f 7073 2e61  f._pending_ops.a
+0000ff90: 7070 656e 6428 6f70 6572 6174 696f 6e20  ppend(operation 
+0000ffa0: 2520 7061 7261 6d29 0a0a 2020 2020 2020  % param)..      
+0000ffb0: 2020 6966 2073 656c 662e 5f70 656e 6469    if self._pendi
+0000ffc0: 6e67 5f6f 7073 3a0a 2020 2020 2020 2020  ng_ops:.        
+0000ffd0: 2020 2020 7365 6c66 2e5f 6578 6563 7574      self._execut
+0000ffe0: 655f 696e 7465 726e 616c 2873 656c 662e  e_internal(self.
+0000fff0: 5f70 656e 6469 6e67 5f6f 7073 2e70 6f70  _pending_ops.pop
+00010000: 2830 2929 0a0a 2020 2020 2020 2020 7265  (0))..        re
+00010010: 7475 726e 2073 656c 660a 0a20 2020 2064  turn self..    d
+00010020: 6566 2065 7865 6375 7465 2873 656c 662c  ef execute(self,
+00010030: 206f 7065 7261 7469 6f6e 3a20 556e 696f   operation: Unio
+00010040: 6e5b 7374 722c 2062 7974 6573 5d2c 2070  n[str, bytes], p
+00010050: 6172 616d 6574 6572 733a 204d 6170 7069  arameters: Mappi
+00010060: 6e67 5b55 6e69 6f6e 5b73 7472 2c20 6279  ng[Union[str, by
+00010070: 7465 735d 2c20 6f62 6a65 6374 5d20 3d20  tes], object] = 
+00010080: 7b7d 2920 2d3e 2022 4375 7273 6f72 223a  {}) -> "Cursor":
+00010090: 0a20 2020 2020 2020 2022 2222 5072 6570  .        """Prep
+000100a0: 6172 6520 616e 6420 6578 6563 7574 6520  are and execute 
+000100b0: 6120 6461 7461 6261 7365 206f 7065 7261  a database opera
+000100c0: 7469 6f6e 2028 7175 6572 7920 6f72 2063  tion (query or c
+000100d0: 6f6d 6d61 6e64 292e 0a0a 2020 2020 2020  ommand)...      
+000100e0: 2020 5061 7261 6d65 7465 7273 206d 6179    Parameters may
+000100f0: 2062 6520 7072 6f76 6964 6564 2061 7320   be provided as 
+00010100: 6120 6d61 7070 696e 6720 616e 6420 7769  a mapping and wi
+00010110: 6c6c 2062 6520 626f 756e 6420 746f 2076  ll be bound to v
+00010120: 6172 6961 626c 6573 0a20 2020 2020 2020  ariables.       
+00010130: 2069 6e20 7468 6520 6f70 6572 6174 696f   in the operatio
+00010140: 6e2e 2056 6172 6961 626c 6573 2061 7265  n. Variables are
+00010150: 2073 7065 6369 6669 6564 2069 6e20 5079   specified in Py
+00010160: 7468 6f6e 2065 7874 656e 6465 6420 666f  thon extended fo
+00010170: 726d 6174 2063 6f64 6573 2c0a 2020 2020  rmat codes,.    
+00010180: 2020 2020 652e 672e 202e 2e2e 5748 4552      e.g. ...WHER
+00010190: 4520 6e61 6d65 3d25 286e 616d 6529 730a  E name=%(name)s.
+000101a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000101b0: 2020 2020 7365 6c66 2e5f 7265 696e 6974      self._reinit
+000101c0: 6961 6c69 7a65 2829 0a0a 2020 2020 2020  ialize()..      
+000101d0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+000101e0: 6f70 6572 6174 696f 6e2c 2062 7974 6573  operation, bytes
+000101f0: 293a 0a20 2020 2020 2020 2020 2020 206f  ):.            o
+00010200: 7065 7261 7469 6f6e 203d 206f 7065 7261  peration = opera
+00010210: 7469 6f6e 2e64 6563 6f64 6528 290a 0a20  tion.decode().. 
+00010220: 2020 2020 2020 2070 6172 616d 7320 3d20         params = 
+00010230: 7b6b 6579 2e64 6563 6f64 6528 2920 6966  {key.decode() if
+00010240: 2069 7369 6e73 7461 6e63 6528 6b65 792c   isinstance(key,
+00010250: 2062 7974 6573 2920 656c 7365 206b 6579   bytes) else key
+00010260: 3a20 7661 6c75 6520 666f 7220 286b 6579  : value for (key
+00010270: 2c20 7661 6c75 6529 2069 6e20 7061 7261  , value) in para
+00010280: 6d65 7465 7273 2e69 7465 6d73 2829 7d0a  meters.items()}.
+00010290: 0a20 2020 2020 2020 2073 656c 662e 5f65  .        self._e
+000102a0: 7865 6375 7465 5f69 6e74 6572 6e61 6c28  xecute_internal(
+000102b0: 6f70 6572 6174 696f 6e2c 2070 6172 616d  operation, param
+000102c0: 7329 0a0a 2020 2020 2020 2020 7265 7475  s)..        retu
+000102d0: 726e 2073 656c 660a 0a20 2020 2064 6566  rn self..    def
+000102e0: 205f 6578 6563 7574 655f 696e 7465 726e   _execute_intern
+000102f0: 616c 2873 656c 662c 206f 7065 7261 7469  al(self, operati
+00010300: 6f6e 3a20 7374 722c 2070 6172 616d 6574  on: str, paramet
+00010310: 6572 733a 204d 6170 7069 6e67 5b73 7472  ers: Mapping[str
+00010320: 2c20 6f62 6a65 6374 5d20 3d20 7b7d 2920  , object] = {}) 
+00010330: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00010340: 2022 2222 496e 7465 726e 616c 2065 7865   """Internal exe
+00010350: 6375 7465 2072 6f75 7469 6e65 2074 6861  cute routine tha
+00010360: 7420 6765 7473 2063 616c 6c65 6420 6672  t gets called fr
+00010370: 6f6d 2065 7865 6375 7465 2061 6e64 2065  om execute and e
+00010380: 7865 6375 7465 6d61 6e79 2222 220a 2020  xecutemany""".  
+00010390: 2020 2020 2020 2320 7079 6c69 6e74 3a20        # pylint: 
+000103a0: 6469 7361 626c 653d 746f 6f2d 6d61 6e79  disable=too-many
+000103b0: 2d62 7261 6e63 6865 730a 0a20 2020 2020  -branches..     
+000103c0: 2020 2023 2045 7870 616e 6420 666f 726d     # Expand form
+000103d0: 6174 2073 7472 696e 670a 2020 2020 2020  at string.      
+000103e0: 2020 6966 2070 6172 616d 6574 6572 733a    if parameters:
+000103f0: 0a20 2020 2020 2020 2020 2020 206f 7065  .            ope
+00010400: 7261 7469 6f6e 203d 206f 7065 7261 7469  ration = operati
+00010410: 6f6e 2025 2070 6172 616d 6574 6572 730a  on % parameters.
+00010420: 0a20 2020 2020 2020 2023 2057 6520 6e65  .        # We ne
+00010430: 6564 2074 6f20 6669 6775 7265 206f 7574  ed to figure out
+00010440: 2077 6865 7468 6572 2077 6520 7368 6f75   whether we shou
+00010450: 6c64 2063 616c 6c0a 2020 2020 2020 2020  ld call.        
+00010460: 2320 6578 6563 7574 655f 7175 6572 7920  # execute_query 
+00010470: 6f72 2065 7865 6375 7465 5f75 7064 6174  or execute_updat
+00010480: 650a 2020 2020 2020 2020 7374 7269 7070  e.        stripp
+00010490: 6564 203d 206f 7065 7261 7469 6f6e 0a0a  ed = operation..
+000104a0: 2020 2020 2020 2020 2320 4c6f 6f70 2075          # Loop u
+000104b0: 6e74 696c 2077 6520 6861 7665 2073 6f6d  ntil we have som
+000104c0: 6520 7374 6172 7469 6e67 2077 6f72 6473  e starting words
+000104d0: 2e20 4e6f 7465 2074 6869 730a 2020 2020  . Note this.    
+000104e0: 2020 2020 2320 646f 6573 6e27 7420 6163      # doesn't ac
+000104f0: 7475 616c 6c79 2068 616e 646c 6520 7468  tually handle th
+00010500: 6520 6361 7365 206f 6620 2777 6f72 6431  e case of 'word1
+00010510: 202f 2a20 636f 6d6d 656e 7420 2a2f 2077   /* comment */ w
+00010520: 6f72 6432 272c 0a20 2020 2020 2020 2023  ord2',.        #
+00010530: 2062 7574 206e 6f6e 6520 6f66 2074 6865   but none of the
+00010540: 206f 7468 6572 2063 6c69 656e 7473 2064   other clients d
+00010550: 6f20 6569 7468 6572 2e2e 2e0a 2020 2020  o either....    
+00010560: 2020 2020 7768 696c 6520 5472 7565 3a0a      while True:.
+00010570: 2020 2020 2020 2020 2020 2020 2320 7374              # st
+00010580: 7269 7020 6f66 6620 7374 6172 7469 6e67  rip off starting
+00010590: 2073 7061 6365 730a 2020 2020 2020 2020   spaces.        
+000105a0: 2020 2020 7374 7269 7070 6564 203d 2073      stripped = s
+000105b0: 7472 6970 7065 642e 6c73 7472 6970 2829  tripped.lstrip()
+000105c0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+000105d0: 6966 2074 6869 7320 7374 6172 7473 2077  if this starts w
+000105e0: 6974 6820 2d2d 2c20 7374 7269 7020 7468  ith --, strip th
+000105f0: 6520 7265 7374 206f 6620 7468 6520 6c69  e rest of the li
+00010600: 6e65 0a20 2020 2020 2020 2020 2020 2069  ne.            i
+00010610: 6620 7374 7269 7070 6564 2e73 7461 7274  f stripped.start
+00010620: 7377 6974 6828 222d 2d22 293a 0a20 2020  swith("--"):.   
+00010630: 2020 2020 2020 2020 2020 2020 2070 6f73               pos
+00010640: 203d 2073 7472 6970 7065 642e 6669 6e64   = stripped.find
+00010650: 2822 5c6e 2229 0a20 2020 2020 2020 2020  ("\n").         
+00010660: 2020 2020 2020 2069 6620 706f 7320 3d3d         if pos ==
+00010670: 202d 313a 0a20 2020 2020 2020 2020 2020   -1:.           
+00010680: 2020 2020 2020 2020 2073 7472 6970 7065           strippe
+00010690: 6420 3d20 2222 0a20 2020 2020 2020 2020  d = "".         
+000106a0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000106b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106c0: 2073 7472 6970 7065 6420 3d20 7374 7269   stripped = stri
+000106d0: 7070 6564 5b70 6f73 202b 2031 203a 5d0a  pped[pos + 1 :].
+000106e0: 0a20 2020 2020 2020 2020 2020 2023 2069  .            # i
+000106f0: 6620 7468 6973 2073 7461 7274 7320 7769  f this starts wi
+00010700: 7468 202f 2a2c 2073 7472 6970 2075 6e74  th /*, strip unt
+00010710: 696c 202a 2f0a 2020 2020 2020 2020 2020  il */.          
+00010720: 2020 656c 6966 2073 7472 6970 7065 642e    elif stripped.
+00010730: 7374 6172 7473 7769 7468 2822 2f2a 2229  startswith("/*")
+00010740: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00010750: 2020 706f 7320 3d20 7374 7269 7070 6564    pos = stripped
+00010760: 2e66 696e 6428 222a 2f22 290a 2020 2020  .find("*/").    
+00010770: 2020 2020 2020 2020 2020 2020 6966 2070              if p
+00010780: 6f73 203d 3d20 2d31 3a0a 2020 2020 2020  os == -1:.      
+00010790: 2020 2020 2020 2020 2020 2020 2020 7374                st
+000107a0: 7269 7070 6564 203d 2022 220a 2020 2020  ripped = "".    
+000107b0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000107c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000107d0: 2020 2020 2020 7374 7269 7070 6564 203d        stripped =
+000107e0: 2073 7472 6970 7065 645b 706f 7320 2b20   stripped[pos + 
+000107f0: 3220 3a5d 0a20 2020 2020 2020 2020 2020  2 :].           
+00010800: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00010810: 2020 2020 2020 2023 2079 6179 2c20 6e6f         # yay, no
+00010820: 2063 6f6d 6d65 6e74 732c 206d 6f76 6520   comments, move 
+00010830: 746f 2074 6865 206e 6578 7420 7068 6173  to the next phas
+00010840: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00010850: 2020 6272 6561 6b0a 0a20 2020 2020 2020    break..       
+00010860: 2023 2069 6620 7765 2064 6f6e 2774 2068   # if we don't h
+00010870: 6176 6520 616e 7974 6869 6e67 206c 6566  ave anything lef
+00010880: 742c 206a 7573 7420 7265 7475 726e 205b  t, just return [
+00010890: 5d0a 2020 2020 2020 2020 6966 206e 6f74  ].        if not
+000108a0: 2073 7472 6970 7065 643a 0a20 2020 2020   stripped:.     
+000108b0: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
+000108c0: 2020 2020 2020 2023 206e 6f77 2073 706c         # now spl
+000108d0: 6974 206f 7574 2074 6865 2077 6f72 6473  it out the words
+000108e0: 0a20 2020 2020 2020 2077 6f72 6473 203d  .        words =
+000108f0: 2073 7472 6970 7065 642e 7370 6c69 7428   stripped.split(
+00010900: 4e6f 6e65 2c20 3329 0a0a 2020 2020 2020  None, 3)..      
+00010910: 2020 2320 5369 6e67 6c65 2077 6f72 6420    # Single word 
+00010920: 6d61 7463 6865 730a 2020 2020 2020 2020  matches.        
+00010930: 7175 6572 795f 7479 7065 203d 2077 6f72  query_type = wor
+00010940: 6473 5b30 5d2e 7570 7065 7228 290a 2020  ds[0].upper().  
+00010950: 2020 2020 2020 6966 2071 7565 7279 5f74        if query_t
+00010960: 7970 6520 696e 205b 2253 454c 4543 5422  ype in ["SELECT"
+00010970: 2c20 2257 4954 4822 2c20 2245 5850 4f52  , "WITH", "EXPOR
+00010980: 5422 2c20 2243 4845 434b 222c 2022 5348  T", "CHECK", "SH
+00010990: 4f57 225d 3a0a 2020 2020 2020 2020 2020  OW"]:.          
+000109a0: 2020 7265 7475 726e 2073 656c 662e 5f65    return self._e
+000109b0: 7865 6375 7465 5f71 7565 7279 286f 7065  xecute_query(ope
+000109c0: 7261 7469 6f6e 3d6f 7065 7261 7469 6f6e  ration=operation
+000109d0: 2c20 7175 6572 795f 7479 7065 3d71 7565  , query_type=que
+000109e0: 7279 5f74 7970 6529 0a20 2020 2020 2020  ry_type).       
+000109f0: 2065 6c69 6620 7175 6572 795f 7479 7065   elif query_type
+00010a00: 2069 6e20 5b22 4558 504c 4149 4e22 5d3a   in ["EXPLAIN"]:
+00010a10: 0a20 2020 2020 2020 2020 2020 2023 2065  .            # e
+00010a20: 7870 6c61 696e 2070 6970 656c 696e 650a  xplain pipeline.
+00010a30: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00010a40: 656e 2877 6f72 6473 2920 3e20 3120 616e  en(words) > 1 an
+00010a50: 6420 776f 7264 735b 315d 2e75 7070 6572  d words[1].upper
+00010a60: 2829 203d 3d20 2250 4950 454c 494e 4522  () == "PIPELINE"
+00010a70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00010a80: 2020 7265 7475 726e 2073 656c 662e 5f65    return self._e
+00010a90: 7865 6375 7465 5f71 7565 7279 286f 7065  xecute_query(ope
+00010aa0: 7261 7469 6f6e 3d6f 7065 7261 7469 6f6e  ration=operation
+00010ab0: 2c20 7175 6572 795f 7479 7065 3d71 7565  , query_type=que
+00010ac0: 7279 5f74 7970 6520 2b20 2220 5049 5045  ry_type + " PIPE
+00010ad0: 4c49 4e45 2229 0a20 2020 2020 2020 2020  LINE").         
+00010ae0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00010af0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00010b00: 7365 6c66 2e5f 6578 6563 7574 655f 7175  self._execute_qu
+00010b10: 6572 7928 6f70 6572 6174 696f 6e3d 6f70  ery(operation=op
+00010b20: 6572 6174 696f 6e2c 2071 7565 7279 5f74  eration, query_t
+00010b30: 7970 653d 7175 6572 795f 7479 7065 290a  ype=query_type).
+00010b40: 2020 2020 2020 2020 656c 6966 2071 7565          elif que
+00010b50: 7279 5f74 7970 6520 696e 205b 224c 4953  ry_type in ["LIS
+00010b60: 5422 5d3a 0a20 2020 2020 2020 2020 2020  T"]:.           
+00010b70: 2069 6620 6f70 6572 6174 696f 6e2e 7570   if operation.up
+00010b80: 7065 7228 2920 3d3d 2022 4c49 5354 2041  per() == "LIST A
+00010b90: 4c4c 2051 5545 5249 4553 223a 0a20 2020  LL QUERIES":.   
+00010ba0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00010bb0: 7572 6e20 7365 6c66 2e5f 6578 6563 7574  urn self._execut
+00010bc0: 655f 7175 6572 7928 6f70 6572 6174 696f  e_query(operatio
+00010bd0: 6e3d 2253 454c 4543 5420 2a20 4652 4f4d  n="SELECT * FROM
+00010be0: 2053 5953 2e51 5545 5249 4553 222c 2071   SYS.QUERIES", q
+00010bf0: 7565 7279 5f74 7970 653d 2253 454c 4543  uery_type="SELEC
+00010c00: 5422 290a 2020 2020 2020 2020 2020 2020  T").            
+00010c10: 656c 6966 206f 7065 7261 7469 6f6e 2e75  elif operation.u
+00010c20: 7070 6572 2829 203d 3d20 224c 4953 5420  pper() == "LIST 
+00010c30: 414c 4c20 434f 4d50 4c45 5445 4420 5155  ALL COMPLETED QU
+00010c40: 4552 4945 5322 3a0a 2020 2020 2020 2020  ERIES":.        
+00010c50: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00010c60: 656c 662e 5f65 7865 6375 7465 5f71 7565  elf._execute_que
+00010c70: 7279 286f 7065 7261 7469 6f6e 3d22 5345  ry(operation="SE
+00010c80: 4c45 4354 202a 2046 524f 4d20 5359 532e  LECT * FROM SYS.
+00010c90: 434f 4d50 4c45 5445 445f 5155 4552 4945  COMPLETED_QUERIE
+00010ca0: 5322 2c20 7175 6572 795f 7479 7065 3d22  S", query_type="
+00010cb0: 5345 4c45 4354 2229 0a20 2020 2020 2020  SELECT").       
+00010cc0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00010cd0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00010ce0: 6e20 7365 6c66 2e5f 6578 6563 7574 655f  n self._execute_
+00010cf0: 6c69 7374 286f 7065 7261 7469 6f6e 3d6f  list(operation=o
+00010d00: 7065 7261 7469 6f6e 290a 2020 2020 2020  peration).      
+00010d10: 2020 656c 6966 2071 7565 7279 5f74 7970    elif query_typ
+00010d20: 6520 3d3d 2022 464f 5243 4522 3a0a 2020  e == "FORCE":.  
+00010d30: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00010d40: 6578 6563 7574 655f 666f 7263 6528 6f70  execute_force(op
+00010d50: 6572 6174 696f 6e3d 6f70 6572 6174 696f  eration=operatio
+00010d60: 6e29 0a20 2020 2020 2020 2065 6c69 6620  n).        elif 
+00010d70: 7175 6572 795f 7479 7065 203d 3d20 2253  query_type == "S
+00010d80: 4554 223a 0a20 2020 2020 2020 2020 2020  ET":.           
+00010d90: 2073 656c 662e 5f65 7865 6375 7465 5f73   self._execute_s
+00010da0: 6574 2877 6f72 6473 5b31 3a5d 290a 2020  et(words[1:]).  
+00010db0: 2020 2020 2020 656c 6966 2071 7565 7279        elif query
+00010dc0: 5f74 7970 6520 3d3d 2022 4745 5422 3a0a  _type == "GET":.
+00010dd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010de0: 2e5f 6578 6563 7574 655f 6765 7428 776f  ._execute_get(wo
+00010df0: 7264 735b 313a 5d29 0a20 2020 2020 2020  rds[1:]).       
+00010e00: 2065 6c69 6620 7175 6572 795f 7479 7065   elif query_type
+00010e10: 203d 3d20 224b 494c 4c22 3a0a 2020 2020   == "KILL":.    
+00010e20: 2020 2020 2020 2020 7365 6c66 2e5f 6578          self._ex
+00010e30: 6563 7574 655f 6361 6e63 656c 6b69 6c6c  ecute_cancelkill
+00010e40: 2871 7565 7279 5f74 7970 652c 2077 6f72  (query_type, wor
+00010e50: 6473 5b31 3a5d 290a 2020 2020 2020 2020  ds[1:]).        
+00010e60: 656c 6966 2071 7565 7279 5f74 7970 6520  elif query_type 
+00010e70: 3d3d 2022 4341 4e43 454c 223a 0a20 2020  == "CANCEL":.   
+00010e80: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
+00010e90: 776f 7264 7329 203e 2031 2061 6e64 2077  words) > 1 and w
+00010ea0: 6f72 6473 5b31 5d2e 7570 7065 7228 2920  ords[1].upper() 
+00010eb0: 3d3d 2022 5441 534b 223a 0a20 2020 2020  == "TASK":.     
+00010ec0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010ed0: 5f65 7865 6375 7465 5f75 7064 6174 6528  _execute_update(
+00010ee0: 6f70 6572 6174 696f 6e29 0a20 2020 2020  operation).     
+00010ef0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00010f00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00010f10: 662e 5f65 7865 6375 7465 5f63 616e 6365  f._execute_cance
+00010f20: 6c6b 696c 6c28 7175 6572 795f 7479 7065  lkill(query_type
+00010f30: 2c20 776f 7264 735b 313a 5d29 0a20 2020  , words[1:]).   
+00010f40: 2020 2020 2065 6c69 6620 7175 6572 795f       elif query_
+00010f50: 7479 7065 203d 3d20 2243 4c45 4152 223a  type == "CLEAR":
+00010f60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00010f70: 662e 5f65 7865 6375 7465 5f63 6c65 6172  f._execute_clear
+00010f80: 2877 6f72 6473 5b31 3a5d 290a 2020 2020  (words[1:]).    
+00010f90: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00010fa0: 2020 2020 2020 2320 6f6b 2c20 7468 6973        # ok, this
+00010fb0: 2069 7320 616e 2075 7064 6174 650a 2020   is an update.  
+00010fc0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00010fd0: 6578 6563 7574 655f 7570 6461 7465 286f  execute_update(o
+00010fe0: 7065 7261 7469 6f6e 290a 0a20 2020 2064  peration)..    d
+00010ff0: 6566 2074 6162 6c65 7328 7365 6c66 2c20  ef tables(self, 
+00011000: 7363 6865 6d61 3a20 7374 7220 3d20 2225  schema: str = "%
+00011010: 222c 2074 6162 6c65 3a20 7374 7220 3d20  ", table: str = 
+00011020: 2225 2229 202d 3e20 2243 7572 736f 7222  "%") -> "Cursor"
+00011030: 3a0a 2020 2020 2020 2020 2222 2247 6574  :.        """Get
+00011040: 2074 6865 2064 6174 6162 6173 6520 7461   the database ta
+00011050: 626c 6573 2222 220a 2020 2020 2020 2020  bles""".        
+00011060: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
+00011070: 653d 6e6f 2d6d 656d 6265 720a 2020 2020  e=no-member.    
+00011080: 2020 2020 7365 6c66 2e5f 6d65 7461 6461      self._metada
+00011090: 7461 5f72 6571 2870 726f 746f 2e46 6574  ta_req(proto.Fet
+000110a0: 6368 5379 7374 656d 4d65 7461 6461 7461  chSystemMetadata
+000110b0: 2e47 4554 5f54 4142 4c45 532c 2073 6368  .GET_TABLES, sch
+000110c0: 656d 613d 7363 6865 6d61 2c20 7461 626c  ema=schema, tabl
+000110d0: 653d 7461 626c 6529 0a20 2020 2020 2020  e=table).       
+000110e0: 2072 6574 7572 6e20 7365 6c66 0a0a 2020   return self..  
+000110f0: 2020 6465 6620 7379 7374 656d 5f74 6162    def system_tab
+00011100: 6c65 7328 7365 6c66 2c20 7461 626c 653a  les(self, table:
+00011110: 2073 7472 203d 2022 2522 2920 2d3e 2022   str = "%") -> "
+00011120: 4375 7273 6f72 223a 0a20 2020 2020 2020  Cursor":.       
+00011130: 2022 2222 4765 7420 7468 6520 6461 7461   """Get the data
+00011140: 6261 7365 2073 7973 7465 6d20 7461 626c  base system tabl
+00011150: 6573 2222 220a 2020 2020 2020 2020 2320  es""".        # 
+00011160: 7079 6c69 6e74 3a20 6469 7361 626c 653d  pylint: disable=
+00011170: 6e6f 2d6d 656d 6265 720a 2020 2020 2020  no-member.      
+00011180: 2020 7365 6c66 2e5f 6d65 7461 6461 7461    self._metadata
+00011190: 5f72 6571 2870 726f 746f 2e46 6574 6368  _req(proto.Fetch
+000111a0: 5379 7374 656d 4d65 7461 6461 7461 2e47  SystemMetadata.G
+000111b0: 4554 5f53 5953 5445 4d5f 5441 424c 4553  ET_SYSTEM_TABLES
+000111c0: 2c20 7461 626c 653d 7461 626c 6529 0a20  , table=table). 
+000111d0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000111e0: 6c66 0a0a 2020 2020 6465 6620 7669 6577  lf..    def view
+000111f0: 7328 7365 6c66 2c20 7669 6577 3a20 7374  s(self, view: st
+00011200: 7220 3d20 2225 2229 202d 3e20 2243 7572  r = "%") -> "Cur
+00011210: 736f 7222 3a0a 2020 2020 2020 2020 2222  sor":.        ""
+00011220: 2247 6574 2074 6865 2064 6174 6162 6173  "Get the databas
+00011230: 6520 7669 6577 7322 2222 0a20 2020 2020  e views""".     
+00011240: 2020 2023 2070 796c 696e 743a 2064 6973     # pylint: dis
+00011250: 6162 6c65 3d6e 6f2d 6d65 6d62 6572 0a20  able=no-member. 
+00011260: 2020 2020 2020 2073 656c 662e 5f6d 6574         self._met
+00011270: 6164 6174 615f 7265 7128 7072 6f74 6f2e  adata_req(proto.
+00011280: 4665 7463 6853 7973 7465 6d4d 6574 6164  FetchSystemMetad
+00011290: 6174 612e 4745 545f 5649 4557 532c 2076  ata.GET_VIEWS, v
+000112a0: 6965 773d 7669 6577 290a 2020 2020 2020  iew=view).      
+000112b0: 2020 7265 7475 726e 2073 656c 660a 0a20    return self.. 
+000112c0: 2020 2064 6566 2063 6f6c 756d 6e73 2873     def columns(s
+000112d0: 656c 662c 2073 6368 656d 613a 2073 7472  elf, schema: str
+000112e0: 203d 2022 2522 2c20 7461 626c 653a 2073   = "%", table: s
+000112f0: 7472 203d 2022 2522 2c20 636f 6c75 6d6e  tr = "%", column
+00011300: 3a20 7374 7220 3d20 2225 2229 202d 3e20  : str = "%") -> 
+00011310: 2243 7572 736f 7222 3a0a 2020 2020 2020  "Cursor":.      
+00011320: 2020 2222 2247 6574 2074 6865 2064 6174    """Get the dat
+00011330: 6162 6173 6520 636f 6c75 6d6e 7322 2222  abase columns"""
+00011340: 0a20 2020 2020 2020 2023 2070 796c 696e  .        # pylin
+00011350: 743a 2064 6973 6162 6c65 3d6e 6f2d 6d65  t: disable=no-me
+00011360: 6d62 6572 0a20 2020 2020 2020 2073 656c  mber.        sel
+00011370: 662e 5f6d 6574 6164 6174 615f 7265 7128  f._metadata_req(
+00011380: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+00011390: 746f 2e46 6574 6368 5379 7374 656d 4d65  to.FetchSystemMe
+000113a0: 7461 6461 7461 2e47 4554 5f43 4f4c 554d  tadata.GET_COLUM
+000113b0: 4e53 2c0a 2020 2020 2020 2020 2020 2020  NS,.            
+000113c0: 7363 6865 6d61 3d73 6368 656d 612c 0a20  schema=schema,. 
+000113d0: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+000113e0: 3d74 6162 6c65 2c0a 2020 2020 2020 2020  =table,.        
+000113f0: 2020 2020 636f 6c75 6d6e 3d63 6f6c 756d      column=colum
+00011400: 6e2c 0a20 2020 2020 2020 2029 0a20 2020  n,.        ).   
+00011410: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00011420: 0a0a 2020 2020 6465 6620 696e 6465 7865  ..    def indexe
+00011430: 7328 7365 6c66 2c20 7363 6865 6d61 3a20  s(self, schema: 
+00011440: 7374 7220 3d20 2225 222c 2074 6162 6c65  str = "%", table
+00011450: 3a20 7374 7220 3d20 2225 2229 202d 3e20  : str = "%") -> 
+00011460: 2243 7572 736f 7222 3a0a 2020 2020 2020  "Cursor":.      
+00011470: 2020 2222 2247 6574 2074 6865 2064 6174    """Get the dat
+00011480: 6162 6173 6520 696e 6465 7865 7322 2222  abase indexes"""
+00011490: 0a20 2020 2020 2020 2023 2070 796c 696e  .        # pylin
+000114a0: 743a 2064 6973 6162 6c65 3d6e 6f2d 6d65  t: disable=no-me
+000114b0: 6d62 6572 0a20 2020 2020 2020 2073 656c  mber.        sel
+000114c0: 662e 5f6d 6574 6164 6174 615f 7265 7128  f._metadata_req(
+000114d0: 7072 6f74 6f2e 4665 7463 6853 7973 7465  proto.FetchSyste
+000114e0: 6d4d 6574 6164 6174 612e 4745 545f 494e  mMetadata.GET_IN
+000114f0: 4445 585f 494e 464f 2c20 7363 6865 6d61  DEX_INFO, schema
+00011500: 3d73 6368 656d 612c 2074 6162 6c65 3d74  =schema, table=t
+00011510: 6162 6c65 290a 2020 2020 2020 2020 7265  able).        re
+00011520: 7475 726e 2073 656c 660a 0a20 2020 2064  turn self..    d
+00011530: 6566 2067 6574 5479 7065 496e 666f 2873  ef getTypeInfo(s
+00011540: 656c 6629 202d 3e20 2243 7572 736f 7222  elf) -> "Cursor"
+00011550: 3a20 2023 2070 796c 696e 743a 2064 6973  :  # pylint: dis
+00011560: 6162 6c65 3d69 6e76 616c 6964 2d6e 616d  able=invalid-nam
+00011570: 650a 2020 2020 2020 2020 2222 2247 6574  e.        """Get
+00011580: 2074 6865 2064 6174 6162 6173 6520 7479   the database ty
+00011590: 7065 2069 6e66 6f22 2222 0a20 2020 2020  pe info""".     
+000115a0: 2020 2023 2070 796c 696e 743a 2064 6973     # pylint: dis
+000115b0: 6162 6c65 3d6e 6f2d 6d65 6d62 6572 0a20  able=no-member. 
+000115c0: 2020 2020 2020 2073 656c 662e 5f6d 6574         self._met
+000115d0: 6164 6174 615f 7265 7128 7072 6f74 6f2e  adata_req(proto.
+000115e0: 4665 7463 6853 7973 7465 6d4d 6574 6164  FetchSystemMetad
+000115f0: 6174 612e 4745 545f 5459 5045 5f49 4e46  ata.GET_TYPE_INF
+00011600: 4f29 0a20 2020 2020 2020 2072 6574 7572  O).        retur
+00011610: 6e20 7365 6c66 0a0a 2020 2020 6465 6620  n self..    def 
+00011620: 6765 7453 7973 7465 6d56 6572 7369 6f6e  getSystemVersion
+00011630: 2873 656c 6629 202d 3e20 556e 696f 6e5b  (self) -> Union[
+00011640: 696e 742c 2073 7472 2c20 4e6f 6e65 5d3a  int, str, None]:
+00011650: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00011660: 7365 6c66 2e5f 6578 6563 7574 655f 7379  self._execute_sy
+00011670: 7374 656d 6d65 7461 6461 7461 2870 726f  stemmetadata(pro
+00011680: 746f 2e46 6574 6368 5379 7374 656d 4d65  to.FetchSystemMe
+00011690: 7461 6461 7461 2e47 4554 5f44 4154 4142  tadata.GET_DATAB
+000116a0: 4153 455f 5052 4f44 5543 545f 5645 5253  ASE_PRODUCT_VERS
+000116b0: 494f 4e29 0a0a 2020 2020 6465 6620 5f6d  ION)..    def _m
+000116c0: 6574 6164 6174 615f 7265 7128 0a20 2020  etadata_req(.   
+000116d0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+000116e0: 2020 2072 6571 7479 7065 3a20 7072 6f74     reqtype: prot
+000116f0: 6f2e 4665 7463 6853 7973 7465 6d4d 6574  o.FetchSystemMet
+00011700: 6164 6174 612e 5379 7374 656d 4d65 7461  adata.SystemMeta
+00011710: 6461 7461 4361 6c6c 2c0a 2020 2020 2020  dataCall,.      
+00011720: 2020 7363 6865 6d61 3a20 7374 7220 3d20    schema: str = 
+00011730: 2225 222c 0a20 2020 2020 2020 2074 6162  "%",.        tab
+00011740: 6c65 3a20 7374 7220 3d20 2225 222c 0a20  le: str = "%",. 
+00011750: 2020 2020 2020 2063 6f6c 756d 6e3a 2073         column: s
+00011760: 7472 203d 2022 2522 2c0a 2020 2020 2020  tr = "%",.      
+00011770: 2020 7669 6577 3a20 7374 7220 3d20 2225    view: str = "%
+00011780: 222c 0a20 2020 2029 202d 3e20 4e6f 6e65  ",.    ) -> None
+00011790: 3a0a 2020 2020 2020 2020 2222 2249 6e74  :.        """Int
+000117a0: 6572 6e61 6c20 6675 6e63 7469 6f6e 2074  ernal function t
+000117b0: 6f20 6765 7420 6461 7461 6261 7365 206d  o get database m
+000117c0: 6574 6164 6174 6122 2222 0a20 2020 2020  etadata""".     
+000117d0: 2020 2023 2070 796c 696e 743a 2064 6973     # pylint: dis
+000117e0: 6162 6c65 3d6e 6f2d 6d65 6d62 6572 2c74  able=no-member,t
+000117f0: 6f6f 2d6d 616e 792d 6172 6775 6d65 6e74  oo-many-argument
+00011800: 730a 2020 2020 2020 2020 7365 6c66 2e5f  s.        self._
+00011810: 7265 696e 6974 6961 6c69 7a65 2829 0a20  reinitialize(). 
+00011820: 2020 2020 2020 2023 2072 6571 2e66 6574         # req.fet
+00011830: 6368 5f73 7973 7465 6d5f 6d65 7461 6461  ch_system_metada
+00011840: 7461 2e47 4554 5f54 4142 4c45 530a 2020  ta.GET_TABLES.  
+00011850: 2020 2020 2020 7265 7120 3d20 7072 6f74        req = prot
+00011860: 6f2e 5265 7175 6573 7428 290a 2020 2020  o.Request().    
+00011870: 2020 2020 7265 712e 7479 7065 203d 2072      req.type = r
+00011880: 6571 2e46 4554 4348 5f53 5953 5445 4d5f  eq.FETCH_SYSTEM_
+00011890: 4d45 5441 4441 5441 0a20 2020 2020 2020  METADATA.       
+000118a0: 2072 6571 2e66 6574 6368 5f73 7973 7465   req.fetch_syste
+000118b0: 6d5f 6d65 7461 6461 7461 2e63 616c 6c20  m_metadata.call 
+000118c0: 3d20 7265 7174 7970 650a 2020 2020 2020  = reqtype.      
+000118d0: 2020 7265 712e 6665 7463 685f 7379 7374    req.fetch_syst
+000118e0: 656d 5f6d 6574 6164 6174 612e 7363 6865  em_metadata.sche
+000118f0: 6d61 203d 2073 6368 656d 610a 2020 2020  ma = schema.    
+00011900: 2020 2020 7265 712e 6665 7463 685f 7379      req.fetch_sy
+00011910: 7374 656d 5f6d 6574 6164 6174 612e 7461  stem_metadata.ta
+00011920: 626c 6520 3d20 7461 626c 650a 2020 2020  ble = table.    
+00011930: 2020 2020 7265 712e 6665 7463 685f 7379      req.fetch_sy
+00011940: 7374 656d 5f6d 6574 6164 6174 612e 636f  stem_metadata.co
+00011950: 6c75 6d6e 203d 2063 6f6c 756d 6e0a 2020  lumn = column.  
+00011960: 2020 2020 2020 7265 712e 6665 7463 685f        req.fetch_
+00011970: 7379 7374 656d 5f6d 6574 6164 6174 612e  system_metadata.
+00011980: 7669 6577 203d 2076 6965 770a 2020 2020  view = view.    
+00011990: 2020 2020 7265 712e 6665 7463 685f 7379      req.fetch_sy
+000119a0: 7374 656d 5f6d 6574 6164 6174 612e 7465  stem_metadata.te
+000119b0: 7374 203d 2054 7275 650a 0a20 2020 2020  st = True..     
+000119c0: 2020 205f 7365 6e64 5f6d 7367 2873 656c     _send_msg(sel
+000119d0: 662e 636f 6e6e 6563 7469 6f6e 2c20 7265  f.connection, re
+000119e0: 7129 0a0a 2020 2020 2020 2020 7273 7020  q)..        rsp 
+000119f0: 3d20 5f72 6563 765f 6d73 6728 7365 6c66  = _recv_msg(self
+00011a00: 2e63 6f6e 6e65 6374 696f 6e2c 2070 726f  .connection, pro
+00011a10: 746f 2e46 6574 6368 5379 7374 656d 4d65  to.FetchSystemMe
+00011a20: 7461 6461 7461 5265 7370 6f6e 7365 2829  tadataResponse()
+00011a30: 290a 0a20 2020 2020 2020 2069 6620 7273  )..        if rs
+00011a40: 702e 7265 7370 6f6e 7365 2e74 7970 6520  p.response.type 
+00011a50: 3d3d 2070 726f 746f 2e43 6f6e 6669 726d  == proto.Confirm
+00011a60: 6174 696f 6e52 6573 706f 6e73 652e 5245  ationResponse.RE
+00011a70: 5350 4f4e 5345 5f45 5252 4f52 3a0a 2020  SPONSE_ERROR:.  
+00011a80: 2020 2020 2020 2020 2020 6966 2072 7370            if rsp
+00011a90: 2e72 6573 706f 6e73 652e 7665 6e64 6f72  .response.vendor
+00011aa0: 5f63 6f64 6520 3d3d 2053 4553 5349 4f4e  _code == SESSION
+00011ab0: 5f45 5850 4952 4544 5f43 4f44 453a 0a20  _EXPIRED_CODE:. 
+00011ac0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00011ad0: 204e 6565 6420 746f 2072 6566 7265 7368   Need to refresh
+00011ae0: 2074 6865 2073 6573 7369 6f6e 0a20 2020   the session.   
+00011af0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00011b00: 662e 636f 6e6e 6563 7469 6f6e 2e72 6566  f.connection.ref
+00011b10: 7265 7368 2829 0a20 2020 2020 2020 2020  resh().         
+00011b20: 2020 2020 2020 2023 2061 6e64 2074 7279         # and try
+00011b30: 2061 6761 696e 0a20 2020 2020 2020 2020   again.         
+00011b40: 2020 2020 2020 2073 656c 662e 5f6d 6574         self._met
+00011b50: 6164 6174 615f 7265 7128 7265 7174 7970  adata_req(reqtyp
+00011b60: 652c 2073 6368 656d 613d 7363 6865 6d61  e, schema=schema
+00011b70: 2c20 7461 626c 653d 7461 626c 652c 2063  , table=table, c
+00011b80: 6f6c 756d 6e3d 636f 6c75 6d6e 2c20 7669  olumn=column, vi
+00011b90: 6577 3d76 6965 7729 0a20 2020 2020 2020  ew=view).       
+00011ba0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00011bb0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00011bc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00011bd0: 2020 7261 6973 6520 5f63 6f6e 7665 7274    raise _convert
+00011be0: 5f65 7863 6570 7469 6f6e 2872 7370 2e72  _exception(rsp.r
+00011bf0: 6573 706f 6e73 6529 0a0a 2020 2020 2020  esponse)..      
+00011c00: 2020 7365 6c66 2e5f 6765 745f 7265 7375    self._get_resu
+00011c10: 6c74 5f6d 6574 6164 6174 6128 290a 0a20  lt_metadata().. 
+00011c20: 2020 2020 2020 2073 656c 662e 726f 776e         self.rown
+00011c30: 756d 6265 7220 3d20 300a 2020 2020 2020  umber = 0.      
+00011c40: 2020 666f 7220 626c 6f62 2069 6e20 7273    for blob in rs
+00011c50: 702e 7265 7375 6c74 5f73 6574 5f76 616c  p.result_set_val
+00011c60: 2e62 6c6f 6273 3a0a 2020 2020 2020 2020  .blobs:.        
+00011c70: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+00011c80: 5f62 7566 6665 7273 3a0a 2020 2020 2020  _buffers:.      
+00011c90: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00011ca0: 6f66 6673 6574 203d 2030 0a20 2020 2020  offset = 0.     
+00011cb0: 2020 2020 2020 2073 656c 662e 5f62 7566         self._buf
+00011cc0: 6665 7273 2e61 7070 656e 6428 626c 6f62  fers.append(blob
+00011cd0: 290a 0a20 2020 2064 6566 205f 6578 6563  )..    def _exec
+00011ce0: 7574 655f 7175 6572 7928 7365 6c66 2c20  ute_query(self, 
+00011cf0: 6f70 6572 6174 696f 6e3a 2073 7472 2c20  operation: str, 
+00011d00: 7175 6572 795f 7479 7065 3a20 7374 7220  query_type: str 
+00011d10: 3d20 2253 454c 4543 5422 2920 2d3e 204e  = "SELECT") -> N
+00011d20: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00011d30: 4578 6563 7574 6520 6120 7175 6572 7922  Execute a query"
+00011d40: 2222 0a20 2020 2020 2020 2023 2070 796c  "".        # pyl
+00011d50: 696e 743a 2064 6973 6162 6c65 3d6e 6f2d  int: disable=no-
+00011d60: 6d65 6d62 6572 0a0a 2020 2020 2020 2020  member..        
+00011d70: 6661 6374 6f72 7920 3d20 5f4f 4349 454e  factory = _OCIEN
+00011d80: 545f 5245 5155 4553 545f 4641 4354 4f52  T_REQUEST_FACTOR
+00011d90: 4945 532e 6765 7428 7175 6572 795f 7479  IES.get(query_ty
+00011da0: 7065 2e75 7070 6572 2829 2c20 4e6f 6e65  pe.upper(), None
+00011db0: 290a 0a20 2020 2020 2020 2069 6620 6661  )..        if fa
+00011dc0: 6374 6f72 7920 6973 204e 6f6e 653a 0a20  ctory is None:. 
+00011dd0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00011de0: 204e 6f74 5375 7070 6f72 7465 6445 7272   NotSupportedErr
+00011df0: 6f72 2866 2251 7565 7279 2074 7970 6520  or(f"Query type 
+00011e00: 277b 7175 6572 795f 7479 7065 7d27 206e  '{query_type}' n
+00011e10: 6f74 2073 7570 706f 7274 6564 2062 7920  ot supported by 
+00011e20: 7079 6f63 6965 6e74 2722 290a 0a20 2020  pyocient'")..   
+00011e30: 2020 2020 2023 2067 656e 6572 6174 6520       # generate 
+00011e40: 7468 6520 6170 7072 6f70 7269 6174 6520  the appropriate 
+00011e50: 7265 7175 6573 740a 2020 2020 2020 2020  request.        
+00011e60: 7265 7120 3d20 6661 6374 6f72 792e 7265  req = factory.re
+00011e70: 7175 6573 7428 6f70 6572 6174 696f 6e29  quest(operation)
+00011e80: 0a0a 2020 2020 2020 2020 2320 4c6f 6f70  ..        # Loop
+00011e90: 2077 6869 6c65 2077 6520 7265 7472 7920   while we retry 
+00011ea0: 7265 6469 7265 6374 7320 616e 6420 7265  redirects and re
+00011eb0: 636f 6e6e 6563 7473 0a20 2020 2020 2020  connects.       
+00011ec0: 2077 6869 6c65 2054 7275 653a 0a20 2020   while True:.   
+00011ed0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+00011ee0: 7365 6c66 2e63 6f6e 6e65 6374 696f 6e2e  self.connection.
+00011ef0: 666f 7263 6520 6973 206e 6f74 204e 6f6e  force is not Non
+00011f00: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
+00011f10: 2072 6571 2e74 7970 6520 3d3d 2070 726f   req.type == pro
+00011f20: 746f 2e52 6571 7565 7374 2e52 6571 7565  to.Request.Reque
+00011f30: 7374 5479 7065 2e56 616c 7565 2822 4558  stType.Value("EX
+00011f40: 4543 5554 455f 5155 4552 5922 293a 2020  ECUTE_QUERY"):  
+00011f50: 2320 7479 7065 3a20 6967 6e6f 7265 2023  # type: ignore #
+00011f60: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00011f70: 636f 6d2f 7072 6f74 6f63 6f6c 6275 6666  com/protocolbuff
+00011f80: 6572 732f 7072 6f74 6f62 7566 2f69 7373  ers/protobuf/iss
+00011f90: 7565 732f 3130 3234 300a 2020 2020 2020  ues/10240.      
+00011fa0: 2020 2020 2020 2020 2020 7265 712e 6578            req.ex
+00011fb0: 6563 7574 655f 7175 6572 792e 666f 7263  ecute_query.forc
+00011fc0: 6520 3d20 7365 6c66 2e63 6f6e 6e65 6374  e = self.connect
+00011fd0: 696f 6e2e 666f 7263 650a 2020 2020 2020  ion.force.      
+00011fe0: 2020 2020 2020 2020 2020 7265 712e 6578            req.ex
+00011ff0: 6563 7574 655f 7175 6572 792e 666f 7263  ecute_query.forc
+00012000: 6552 6564 6972 6563 7420 3d20 7365 6c66  eRedirect = self
+00012010: 2e63 6f6e 6e65 6374 696f 6e2e 666f 7263  .connection.forc
+00012020: 655f 6e65 7874 5f72 6564 6972 6563 740a  e_next_redirect.
+00012030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012040: 7365 6c66 2e63 6f6e 6e65 6374 696f 6e2e  self.connection.
+00012050: 666f 7263 655f 6e65 7874 5f72 6564 6972  force_next_redir
+00012060: 6563 7420 3d20 4661 6c73 650a 2020 2020  ect = False.    
+00012070: 2020 2020 2020 2020 656c 6966 2072 6571          elif req
+00012080: 2e74 7970 6520 3d3d 2070 726f 746f 2e52  .type == proto.R
+00012090: 6571 7565 7374 2e52 6571 7565 7374 5479  equest.RequestTy
+000120a0: 7065 2e56 616c 7565 2822 4558 4543 5554  pe.Value("EXECUT
+000120b0: 455f 4558 504c 4149 4e22 293a 2020 2320  E_EXPLAIN"):  # 
+000120c0: 7479 7065 3a20 6967 6e6f 7265 2023 2068  type: ignore # h
+000120d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000120e0: 6d2f 7072 6f74 6f63 6f6c 6275 6666 6572  m/protocolbuffer
+000120f0: 732f 7072 6f74 6f62 7566 2f69 7373 7565  s/protobuf/issue
+00012100: 732f 3130 3234 300a 2020 2020 2020 2020  s/10240.        
+00012110: 2020 2020 2020 2020 7265 712e 6578 6563          req.exec
+00012120: 7574 655f 6578 706c 6169 6e2e 666f 7263  ute_explain.forc
+00012130: 6520 3d20 7365 6c66 2e63 6f6e 6e65 6374  e = self.connect
+00012140: 696f 6e2e 666f 7263 650a 2020 2020 2020  ion.force.      
+00012150: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00012160: 2020 2020 2020 2020 2020 205f 7365 6e64             _send
+00012170: 5f6d 7367 2873 656c 662e 636f 6e6e 6563  _msg(self.connec
+00012180: 7469 6f6e 2c20 7265 7129 0a0a 2020 2020  tion, req)..    
+00012190: 2020 2020 2020 2020 2020 2020 7273 7020              rsp 
+000121a0: 3d20 5f72 6563 765f 6d73 6728 7365 6c66  = _recv_msg(self
+000121b0: 2e63 6f6e 6e65 6374 696f 6e2c 2066 6163  .connection, fac
+000121c0: 746f 7279 2e72 6573 706f 6e73 6528 2929  tory.response())
+000121d0: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+000121e0: 6570 7420 494f 4572 726f 723a 0a20 2020  ept IOError:.   
+000121f0: 2020 2020 2020 2020 2020 2020 2023 2072               # r
+00012200: 656d 616b 6520 6f75 7220 636f 6e6e 6563  emake our connec
+00012210: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+00012220: 2020 2020 2073 656c 662e 636f 6e6e 6563       self.connec
+00012230: 7469 6f6e 203d 2043 6f6e 6e65 6374 696f  tion = Connectio
+00012240: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+00012250: 2020 2020 2020 2075 7365 723d 7365 6c66         user=self
+00012260: 2e63 6f6e 6e65 6374 696f 6e2e 7573 6572  .connection.user
+00012270: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00012280: 2020 2020 2020 7061 7373 776f 7264 3d73        password=s
+00012290: 656c 662e 636f 6e6e 6563 7469 6f6e 2e70  elf.connection.p
+000122a0: 6173 7377 6f72 642c 0a20 2020 2020 2020  assword,.       
+000122b0: 2020 2020 2020 2020 2020 2020 2068 6f73               hos
+000122c0: 743d 6622 7b27 2c27 2e6a 6f69 6e28 7365  t=f"{','.join(se
+000122d0: 6c66 2e63 6f6e 6e65 6374 696f 6e2e 686f  lf.connection.ho
+000122e0: 7374 7329 7d3a 7b73 656c 662e 636f 6e6e  sts)}:{self.conn
+000122f0: 6563 7469 6f6e 2e70 6f72 747d 222c 0a20  ection.port}",. 
+00012300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012310: 2020 2064 6174 6162 6173 653d 7365 6c66     database=self
+00012320: 2e63 6f6e 6e65 6374 696f 6e2e 6461 7461  .connection.data
+00012330: 6261 7365 2c0a 2020 2020 2020 2020 2020  base,.          
+00012340: 2020 2020 2020 2020 2020 746c 733d 7365            tls=se
+00012350: 6c66 2e63 6f6e 6e65 6374 696f 6e2e 746c  lf.connection.tl
+00012360: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+00012370: 2020 2020 2020 2068 616e 6473 6861 6b65         handshake
+00012380: 3d73 656c 662e 636f 6e6e 6563 7469 6f6e  =self.connection
+00012390: 2e68 616e 6473 6861 6b65 2c0a 2020 2020  .handshake,.    
+000123a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123b0: 666f 7263 653d 7365 6c66 2e63 6f6e 6e65  force=self.conne
+000123c0: 6374 696f 6e2e 666f 7263 652c 0a20 2020  ction.force,.   
+000123d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123e0: 2073 6573 7369 6f6e 3d73 656c 662e 636f   session=self.co
+000123f0: 6e6e 6563 7469 6f6e 2e73 6573 7369 6f6e  nnection.session
+00012400: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00012410: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+00012420: 2020 2020 2063 6f6e 7469 6e75 650a 0a20       continue.. 
+00012430: 2020 2020 2020 2020 2020 2069 6620 7273             if rs
+00012440: 702e 7265 7370 6f6e 7365 2e74 7970 6520  p.response.type 
+00012450: 3d3d 2070 726f 746f 2e43 6f6e 6669 726d  == proto.Confirm
+00012460: 6174 696f 6e52 6573 706f 6e73 652e 5245  ationResponse.RE
+00012470: 5350 4f4e 5345 5f57 4152 4e3a 0a20 2020  SPONSE_WARN:.   
+00012480: 2020 2020 2020 2020 2020 2020 2077 6172               war
+00012490: 6e28 7273 702e 7265 7370 6f6e 7365 2e72  n(rsp.response.r
+000124a0: 6561 736f 6e29 0a20 2020 2020 2020 2020  eason).         
+000124b0: 2020 2065 6c69 6620 6e6f 7420 7273 702e     elif not rsp.
+000124c0: 7265 7370 6f6e 7365 2e74 7970 6520 3d3d  response.type ==
+000124d0: 2070 726f 746f 2e43 6f6e 6669 726d 6174   proto.Confirmat
+000124e0: 696f 6e52 6573 706f 6e73 652e 5245 5350  ionResponse.RESP
+000124f0: 4f4e 5345 5f4f 4b3a 0a20 2020 2020 2020  ONSE_OK:.       
+00012500: 2020 2020 2020 2020 2069 6620 7273 702e           if rsp.
+00012510: 7265 7370 6f6e 7365 2e76 656e 646f 725f  response.vendor_
+00012520: 636f 6465 203d 3d20 5345 5353 494f 4e5f  code == SESSION_
+00012530: 4558 5049 5245 445f 434f 4445 3a0a 2020  EXPIRED_CODE:.  
+00012540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012550: 2020 2320 4e65 6564 2074 6f20 7265 6672    # Need to refr
+00012560: 6573 6820 7468 6520 7365 7373 696f 6e0a  esh the session.
+00012570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012580: 2020 2020 7365 6c66 2e63 6f6e 6e65 6374      self.connect
+00012590: 696f 6e2e 7265 6672 6573 6828 290a 2020  ion.refresh().  
+000125a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125b0: 2020 2320 616e 6420 7472 7920 6167 6169    # and try agai
+000125c0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+000125d0: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+000125e0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000125f0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00012600: 2020 2020 2020 2020 2072 6169 7365 205f           raise _
+00012610: 636f 6e76 6572 745f 6578 6365 7074 696f  convert_exceptio
+00012620: 6e28 7273 702e 7265 7370 6f6e 7365 290a  n(rsp.response).
+00012630: 0a20 2020 2020 2020 2020 2020 2023 2073  .            # s
+00012640: 6565 2069 6620 7765 2061 7265 2062 6569  ee if we are bei
+00012650: 6e67 2074 6f6c 6420 746f 2072 6564 6972  ng told to redir
+00012660: 6563 740a 2020 2020 2020 2020 2020 2020  ect.            
+00012670: 7265 6469 7265 6374 203d 2067 6574 6174  redirect = getat
+00012680: 7472 2872 7370 2c20 2272 6564 6972 6563  tr(rsp, "redirec
+00012690: 7422 2c20 4661 6c73 6529 0a20 2020 2020  t", False).     
+000126a0: 2020 2020 2020 2069 6620 6e6f 7420 7265         if not re
+000126b0: 6469 7265 6374 3a0a 2020 2020 2020 2020  direct:.        
+000126c0: 2020 2020 2020 2020 6272 6561 6b0a 0a20          break.. 
+000126d0: 2020 2020 2020 2020 2020 2023 2072 656d             # rem
+000126e0: 616b 6520 6f75 7220 636f 6e6e 6563 7469  ake our connecti
+000126f0: 6f6e 0a20 2020 2020 2020 2020 2020 2073  on.            s
+00012700: 656c 662e 636f 6e6e 6563 7469 6f6e 2e63  elf.connection.c
+00012710: 6c6f 7365 2829 0a20 2020 2020 2020 2020  lose().         
+00012720: 2020 2073 656c 662e 636f 6e6e 6563 7469     self.connecti
+00012730: 6f6e 203d 2073 656c 662e 636f 6e6e 6563  on = self.connec
+00012740: 7469 6f6e 2e72 6564 6972 6563 7428 7273  tion.redirect(rs
+00012750: 702e 7265 6469 7265 6374 486f 7374 2c20  p.redirectHost, 
+00012760: 7273 702e 7265 6469 7265 6374 506f 7274  rsp.redirectPort
+00012770: 290a 0a20 2020 2020 2020 2071 7565 7279  )..        query
+00012780: 5f69 6420 3d20 6765 7461 7474 7228 7273  _id = getattr(rs
+00012790: 702c 2022 7175 6572 7949 6422 2c20 4e6f  p, "queryId", No
+000127a0: 6e65 290a 2020 2020 2020 2020 6966 2071  ne).        if q
+000127b0: 7565 7279 5f69 6420 6973 206e 6f74 204e  uery_id is not N
+000127c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000127d0: 2073 656c 662e 7175 6572 795f 6964 203d   self.query_id =
+000127e0: 2071 7565 7279 5f69 640a 0a20 2020 2020   query_id..     
+000127f0: 2020 2073 656c 662e 726f 776e 756d 6265     self.rownumbe
+00012800: 7220 3d20 300a 0a20 2020 2020 2020 2069  r = 0..        i
+00012810: 6620 7175 6572 795f 7479 7065 2069 6e20  f query_type in 
+00012820: 5b22 5345 4c45 4354 222c 2022 5749 5448  ["SELECT", "WITH
+00012830: 222c 2022 5348 4f57 225d 3a0a 2020 2020  ", "SHOW"]:.    
+00012840: 2020 2020 2020 2020 7365 6c66 2e5f 6765          self._ge
+00012850: 745f 7265 7375 6c74 5f6d 6574 6164 6174  t_result_metadat
+00012860: 6128 290a 0a20 2020 2020 2020 2065 6c69  a()..        eli
+00012870: 6620 7175 6572 795f 7479 7065 203d 3d20  f query_type == 
+00012880: 2245 5850 4f52 5422 3a0a 2020 2020 2020  "EXPORT":.      
+00012890: 2020 2020 2020 7365 6c66 2e64 6573 6372        self.descr
+000128a0: 6970 7469 6f6e 203d 205b 0a20 2020 2020  iption = [.     
+000128b0: 2020 2020 2020 2020 2020 2028 2265 7870             ("exp
+000128c0: 6f72 7422 2c20 5479 7065 436f 6465 732e  ort", TypeCodes.
+000128d0: 4348 4152 2c20 4e6f 6e65 2c20 4e6f 6e65  CHAR, None, None
+000128e0: 2c20 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f  , None, None, No
+000128f0: 6e65 290a 2020 2020 2020 2020 2020 2020  ne).            
+00012900: 5d20 2023 2064 6973 706c 6179 5f73 697a  ]  # display_siz
+00012910: 6520 2023 2069 6e74 6572 6e61 6c5f 7369  e  # internal_si
+00012920: 7a65 2020 2320 7072 6563 6973 696f 6e20  ze  # precision 
+00012930: 2023 2073 6361 6c65 2020 2320 6e75 6c6c   # scale  # null
+00012940: 5f6f 6b0a 2020 2020 2020 2020 2020 2020  _ok.            
+00012950: 7365 6c66 2e72 6573 756c 7473 6574 5f74  self.resultset_t
+00012960: 7570 6c65 203d 206e 616d 6564 7475 706c  uple = namedtupl
+00012970: 6528 2252 6f77 222c 2028 2265 7870 6f72  e("Row", ("expor
+00012980: 7422 2c29 2920 2023 2074 7970 653a 2069  t",))  # type: i
+00012990: 676e 6f72 650a 2020 2020 2020 2020 2020  gnore.          
+000129a0: 2020 7365 6c66 2e67 656e 6572 6174 6564    self.generated
+000129b0: 5f72 6573 756c 7420 3d20 7273 702e 6578  _result = rsp.ex
+000129c0: 706f 7274 5374 6174 656d 656e 740a 2020  portStatement.  
+000129d0: 2020 2020 2020 656c 6966 2071 7565 7279        elif query
+000129e0: 5f74 7970 6520 3d3d 2022 4558 504c 4149  _type == "EXPLAI
+000129f0: 4e22 3a0a 2020 2020 2020 2020 2020 2020  N":.            
+00012a00: 7365 6c66 2e64 6573 6372 6970 7469 6f6e  self.description
+00012a10: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+00012a20: 2020 2020 2028 2265 7870 6c61 696e 222c       ("explain",
+00012a30: 2054 7970 6543 6f64 6573 2e43 4841 522c   TypeCodes.CHAR,
+00012a40: 204e 6f6e 652c 204e 6f6e 652c 204e 6f6e   None, None, Non
+00012a50: 652c 204e 6f6e 652c 204e 6f6e 6529 0a20  e, None, None). 
+00012a60: 2020 2020 2020 2020 2020 205d 2020 2320             ]  # 
+00012a70: 6469 7370 6c61 795f 7369 7a65 2020 2320  display_size  # 
+00012a80: 696e 7465 726e 616c 5f73 697a 6520 2023  internal_size  #
+00012a90: 2070 7265 6369 7369 6f6e 2020 2320 7363   precision  # sc
+00012aa0: 616c 6520 2023 206e 756c 6c5f 6f6b 0a20  ale  # null_ok. 
+00012ab0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012ac0: 7265 7375 6c74 7365 745f 7475 706c 6520  resultset_tuple 
+00012ad0: 3d20 6e61 6d65 6474 7570 6c65 2822 526f  = namedtuple("Ro
+00012ae0: 7722 2c20 2822 6578 706c 6169 6e22 2c29  w", ("explain",)
+00012af0: 2920 2023 2074 7970 653a 2069 676e 6f72  )  # type: ignor
+00012b00: 650a 2020 2020 2020 2020 2020 2020 7365  e.            se
+00012b10: 6c66 2e67 656e 6572 6174 6564 5f72 6573  lf.generated_res
+00012b20: 756c 7420 3d20 7273 702e 706c 616e 0a20  ult = rsp.plan. 
+00012b30: 2020 2020 2020 2065 6c69 6620 7175 6572         elif quer
+00012b40: 795f 7479 7065 203d 3d20 2245 5850 4c41  y_type == "EXPLA
+00012b50: 494e 2050 4950 454c 494e 4522 3a0a 2020  IN PIPELINE":.  
+00012b60: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00012b70: 6573 6372 6970 7469 6f6e 203d 205b 0a20  escription = [. 
+00012b80: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00012b90: 2265 7870 6c61 696e 5f70 6970 656c 696e  "explain_pipelin
+00012ba0: 6522 2c20 5479 7065 436f 6465 732e 4348  e", TypeCodes.CH
+00012bb0: 4152 2c20 4e6f 6e65 2c20 4e6f 6e65 2c20  AR, None, None, 
+00012bc0: 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65  None, None, None
+00012bd0: 290a 2020 2020 2020 2020 2020 2020 5d20  ).            ] 
+00012be0: 2023 2064 6973 706c 6179 5f73 697a 6520   # display_size 
+00012bf0: 2023 2069 6e74 6572 6e61 6c5f 7369 7a65   # internal_size
+00012c00: 2020 2320 7072 6563 6973 696f 6e20 2023    # precision  #
+00012c10: 2073 6361 6c65 2020 2320 6e75 6c6c 5f6f   scale  # null_o
+00012c20: 6b0a 2020 2020 2020 2020 2020 2020 7365  k.            se
+00012c30: 6c66 2e72 6573 756c 7473 6574 5f74 7570  lf.resultset_tup
+00012c40: 6c65 203d 206e 616d 6564 7475 706c 6528  le = namedtuple(
+00012c50: 2252 6f77 222c 2028 2265 7870 6c61 696e  "Row", ("explain
+00012c60: 5f70 6970 656c 696e 6522 2c29 2920 2023  _pipeline",))  #
+00012c70: 2074 7970 653a 2069 676e 6f72 650a 2020   type: ignore.  
+00012c80: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
+00012c90: 656e 6572 6174 6564 5f72 6573 756c 7420  enerated_result 
+00012ca0: 3d20 7273 702e 7069 7065 6c69 6e65 5374  = rsp.pipelineSt
+00012cb0: 6174 656d 656e 740a 2020 2020 2020 2020  atement.        
+00012cc0: 656c 6966 2071 7565 7279 5f74 7970 6520  elif query_type 
+00012cd0: 3d3d 2022 4348 4543 4b22 3a0a 2020 2020  == "CHECK":.    
+00012ce0: 2020 2020 2020 2020 2320 5468 6520 7265          # The re
+00012cf0: 7375 6c74 206f 6620 7468 6520 4348 4543  sult of the CHEC
+00012d00: 4b20 4441 5441 2073 7461 7465 6d65 6e74  K DATA statement
+00012d10: 2069 7320 6120 7374 7269 6e67 2077 6974   is a string wit
+00012d20: 6820 6120 6c6f 7420 6f66 206c 696e 6566  h a lot of linef
+00012d30: 6565 6473 2e20 544f 444f 2063 6f6e 7665  eeds. TODO conve
+00012d40: 7274 2069 7420 746f 2073 6f6d 6574 6869  rt it to somethi
+00012d50: 6e67 2072 6561 736f 6e61 626c 650a 2020  ng reasonable.  
+00012d60: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00012d70: 6573 6372 6970 7469 6f6e 203d 205b 0a20  escription = [. 
+00012d80: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00012d90: 2272 6573 756c 7422 2c20 5479 7065 436f  "result", TypeCo
+00012da0: 6465 732e 4348 4152 2c20 4e6f 6e65 2c20  des.CHAR, None, 
+00012db0: 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65  None, None, None
+00012dc0: 2c20 4e6f 6e65 292c 0a20 2020 2020 2020  , None),.       
+00012dd0: 2020 2020 205d 2020 2320 6469 7370 6c61       ]  # displa
+00012de0: 795f 7369 7a65 2020 2320 696e 7465 726e  y_size  # intern
+00012df0: 616c 5f73 697a 6520 2023 2070 7265 6369  al_size  # preci
+00012e00: 7369 6f6e 2020 2320 7363 616c 6520 2023  sion  # scale  #
+00012e10: 206e 756c 6c5f 6f6b 0a20 2020 2020 2020   null_ok.       
+00012e20: 2020 2020 2073 656c 662e 7265 7375 6c74       self.result
+00012e30: 7365 745f 7475 706c 6520 3d20 6e61 6d65  set_tuple = name
+00012e40: 6474 7570 6c65 2822 526f 7722 2c20 2822  dtuple("Row", ("
+00012e50: 7265 7375 6c74 222c 2929 2020 2320 7479  result",))  # ty
+00012e60: 7065 3a20 6967 6e6f 7265 0a20 2020 2020  pe: ignore.     
+00012e70: 2020 2020 2020 2073 656c 662e 6765 6e65         self.gene
+00012e80: 7261 7465 645f 7265 7375 6c74 203d 2072  rated_result = r
+00012e90: 7370 2e63 6865 636b 4461 7461 5374 6174  sp.checkDataStat
+00012ea0: 656d 656e 740a 0a20 2020 2023 2041 6674  ement..    # Aft
+00012eb0: 6572 206c 6973 7420 616c 6c20 7175 6572  er list all quer
+00012ec0: 6965 7320 616e 6420 6c69 7374 2061 6c6c  ies and list all
+00012ed0: 2063 6f6d 706c 6574 6564 2071 7565 7269   completed queri
+00012ee0: 6573 2068 6176 6520 6265 656e 2072 656d  es have been rem
+00012ef0: 6170 7065 642c 2074 6869 7320 6973 206e  apped, this is n
+00012f00: 6f20 6c6f 6e67 6572 2075 7365 642e 2042  o longer used. B
+00012f10: 7574 2069 7420 6361 6e20 6265 2075 7365  ut it can be use
+00012f20: 6420 666f 7220 6f74 6865 7220 7468 696e  d for other thin
+00012f30: 6773 2e0a 2020 2020 2320 4578 3a20 6c69  gs..    # Ex: li
+00012f40: 7374 2074 6162 6c65 732c 206c 6973 7420  st tables, list 
+00012f50: 7669 6577 732c 206c 6973 7420 7461 626c  views, list tabl
+00012f60: 6520 7072 6976 696c 6567 6573 2e20 4e6f  e privileges. No
+00012f70: 6e65 206f 6620 7468 6573 6520 6172 6520  ne of these are 
+00012f80: 696d 706c 656d 656e 7465 6420 7965 742e  implemented yet.
+00012f90: 0a20 2020 2064 6566 205f 6578 6563 7574  .    def _execut
+00012fa0: 655f 6c69 7374 2873 656c 662c 206f 7065  e_list(self, ope
+00012fb0: 7261 7469 6f6e 3a20 7374 7220 3d20 224c  ration: str = "L
+00012fc0: 4953 5420 414c 4c20 5155 4552 4945 5322  IST ALL QUERIES"
+00012fd0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00012fe0: 2020 2022 2222 4578 6563 7574 6520 4c49     """Execute LI
+00012ff0: 5354 5f41 4c4c 5f51 5545 5249 4553 2222  ST_ALL_QUERIES""
+00013000: 220a 2020 2020 2020 2020 2320 7079 6c69  ".        # pyli
+00013010: 6e74 3a20 6469 7361 626c 653d 6e6f 2d6d  nt: disable=no-m
+00013020: 656d 6265 720a 0a20 2020 2020 2020 2066  ember..        f
+00013030: 6163 746f 7279 203d 205f 4f43 4945 4e54  actory = _OCIENT
+00013040: 5f52 4551 5545 5354 5f46 4143 544f 5249  _REQUEST_FACTORI
+00013050: 4553 2e67 6574 286f 7065 7261 7469 6f6e  ES.get(operation
+00013060: 2e75 7070 6572 2829 2c20 4e6f 6e65 290a  .upper(), None).
+00013070: 0a20 2020 2020 2020 2069 6620 6661 6374  .        if fact
+00013080: 6f72 7920 6973 204e 6f6e 653a 0a20 2020  ory is None:.   
+00013090: 2020 2020 2020 2020 2072 6169 7365 204e           raise N
+000130a0: 6f74 5375 7070 6f72 7465 6445 7272 6f72  otSupportedError
+000130b0: 2866 224c 6973 7420 7175 6572 7920 277b  (f"List query '{
+000130c0: 6f70 6572 6174 696f 6e7d 2720 6e6f 7420  operation}' not 
+000130d0: 7375 7070 6f72 7465 6420 6279 2070 796f  supported by pyo
+000130e0: 6369 656e 7427 2229 0a0a 2020 2020 2020  cient'")..      
+000130f0: 2020 2320 6765 6572 6174 6520 7468 6520    # geerate the 
+00013100: 6170 7072 6f70 7269 6174 6520 7265 7175  appropriate requ
+00013110: 6573 740a 2020 2020 2020 2020 7265 7120  est.        req 
+00013120: 3d20 6661 6374 6f72 792e 7265 7175 6573  = factory.reques
+00013130: 7428 6f70 6572 6174 696f 6e29 0a0a 2020  t(operation)..  
+00013140: 2020 2020 2020 7768 696c 6520 5472 7565        while True
+00013150: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
+00013160: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+00013170: 2020 205f 7365 6e64 5f6d 7367 2873 656c     _send_msg(sel
+00013180: 662e 636f 6e6e 6563 7469 6f6e 2c20 7265  f.connection, re
+00013190: 7129 0a0a 2020 2020 2020 2020 2020 2020  q)..            
+000131a0: 2020 2020 7273 7020 3d20 5f72 6563 765f      rsp = _recv_
+000131b0: 6d73 6728 7365 6c66 2e63 6f6e 6e65 6374  msg(self.connect
+000131c0: 696f 6e2c 2066 6163 746f 7279 2e72 6573  ion, factory.res
+000131d0: 706f 6e73 6528 2929 0a20 2020 2020 2020  ponse()).       
+000131e0: 2020 2020 2065 7863 6570 7420 494f 4572       except IOEr
+000131f0: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
+00013200: 2020 2020 2023 2072 656d 616b 6520 6f75       # remake ou
+00013210: 7220 636f 6e6e 6563 7469 6f6e 0a20 2020  r connection.   
+00013220: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00013230: 662e 636f 6e6e 6563 7469 6f6e 203d 2043  f.connection = C
+00013240: 6f6e 6e65 6374 696f 6e28 0a20 2020 2020  onnection(.     
+00013250: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00013260: 7365 723d 7365 6c66 2e63 6f6e 6e65 6374  ser=self.connect
+00013270: 696f 6e2e 7573 6572 2c0a 2020 2020 2020  ion.user,.      
+00013280: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00013290: 7373 776f 7264 3d73 656c 662e 636f 6e6e  ssword=self.conn
+000132a0: 6563 7469 6f6e 2e70 6173 7377 6f72 642c  ection.password,
+000132b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000132c0: 2020 2020 2068 6f73 743d 6622 7b27 2c27       host=f"{','
+000132d0: 2e6a 6f69 6e28 7365 6c66 2e63 6f6e 6e65  .join(self.conne
+000132e0: 6374 696f 6e2e 686f 7374 7329 7d3a 7b73  ction.hosts)}:{s
+000132f0: 656c 662e 636f 6e6e 6563 7469 6f6e 2e70  elf.connection.p
+00013300: 6f72 747d 222c 0a20 2020 2020 2020 2020  ort}",.         
+00013310: 2020 2020 2020 2020 2020 2064 6174 6162             datab
+00013320: 6173 653d 7365 6c66 2e63 6f6e 6e65 6374  ase=self.connect
+00013330: 696f 6e2e 6461 7461 6261 7365 2c0a 2020  ion.database,.  
+00013340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013350: 2020 746c 733d 7365 6c66 2e63 6f6e 6e65    tls=self.conne
+00013360: 6374 696f 6e2e 746c 732c 0a20 2020 2020  ction.tls,.     
+00013370: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+00013380: 616e 6473 6861 6b65 3d73 656c 662e 636f  andshake=self.co
+00013390: 6e6e 6563 7469 6f6e 2e68 616e 6473 6861  nnection.handsha
+000133a0: 6b65 2c0a 2020 2020 2020 2020 2020 2020  ke,.            
+000133b0: 2020 2020 2020 2020 666f 7263 653d 7365          force=se
+000133c0: 6c66 2e63 6f6e 6e65 6374 696f 6e2e 666f  lf.connection.fo
+000133d0: 7263 652c 0a20 2020 2020 2020 2020 2020  rce,.           
+000133e0: 2020 2020 2020 2020 2073 6573 7369 6f6e           session
+000133f0: 3d73 656c 662e 636f 6e6e 6563 7469 6f6e  =self.connection
+00013400: 2e73 6573 7369 6f6e 2c0a 2020 2020 2020  .session,.      
+00013410: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+00013420: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00013430: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
+00013440: 2020 6272 6561 6b0a 0a20 2020 2020 2020    break..       
+00013450: 2069 6620 7273 702e 7265 7370 6f6e 7365   if rsp.response
+00013460: 2e74 7970 6520 3d3d 2070 726f 746f 2e43  .type == proto.C
+00013470: 6f6e 6669 726d 6174 696f 6e52 6573 706f  onfirmationRespo
+00013480: 6e73 652e 5245 5350 4f4e 5345 5f57 4152  nse.RESPONSE_WAR
+00013490: 4e3a 0a20 2020 2020 2020 2020 2020 2077  N:.            w
+000134a0: 6172 6e28 7273 702e 7265 7370 6f6e 7365  arn(rsp.response
+000134b0: 2e72 6561 736f 6e29 0a20 2020 2020 2020  .reason).       
+000134c0: 2065 6c69 6620 6e6f 7420 7273 702e 7265   elif not rsp.re
+000134d0: 7370 6f6e 7365 2e74 7970 6520 3d3d 2070  sponse.type == p
+000134e0: 726f 746f 2e43 6f6e 6669 726d 6174 696f  roto.Confirmatio
+000134f0: 6e52 6573 706f 6e73 652e 5245 5350 4f4e  nResponse.RESPON
+00013500: 5345 5f4f 4b3a 0a20 2020 2020 2020 2020  SE_OK:.         
+00013510: 2020 2069 6620 7273 702e 7265 7370 6f6e     if rsp.respon
+00013520: 7365 2e76 656e 646f 725f 636f 6465 203d  se.vendor_code =
+00013530: 3d20 5345 5353 494f 4e5f 4558 5049 5245  = SESSION_EXPIRE
+00013540: 445f 434f 4445 3a0a 2020 2020 2020 2020  D_CODE:.        
+00013550: 2020 2020 2020 2020 2320 4e65 6564 2074          # Need t
+00013560: 6f20 7265 6672 6573 6820 7468 6520 7365  o refresh the se
+00013570: 7373 696f 6e0a 2020 2020 2020 2020 2020  ssion.          
+00013580: 2020 2020 2020 7365 6c66 2e63 6f6e 6e65        self.conne
+00013590: 6374 696f 6e2e 7265 6672 6573 6828 290a  ction.refresh().
+000135a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000135b0: 2320 616e 6420 7472 7920 6167 6169 6e0a  # and try again.
+000135c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000135d0: 7365 6c66 2e5f 6578 6563 7574 655f 6c69  self._execute_li
+000135e0: 7374 286f 7065 7261 7469 6f6e 3d6f 7065  st(operation=ope
+000135f0: 7261 7469 6f6e 290a 2020 2020 2020 2020  ration).        
+00013600: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00013610: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00013620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013630: 2072 6169 7365 205f 636f 6e76 6572 745f   raise _convert_
+00013640: 6578 6365 7074 696f 6e28 7273 702e 7265  exception(rsp.re
+00013650: 7370 6f6e 7365 290a 0a20 2020 2020 2020  sponse)..       
+00013660: 2073 656c 662e 6465 7363 7269 7074 696f   self.descriptio
+00013670: 6e20 3d20 5b5d 0a0a 2020 2020 2020 2020  n = []..        
+00013680: 726f 7773 203d 2066 6163 746f 7279 2e70  rows = factory.p
+00013690: 726f 6365 7373 2872 7370 290a 2020 2020  rocess(rsp).    
+000136a0: 2020 2020 6966 206e 6f74 2072 6f77 733a      if not rows:
+000136b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000136c0: 662e 6c69 7374 5f72 6573 756c 7420 3d20  f.list_result = 
+000136d0: 5b5d 0a20 2020 2020 2020 2020 2020 2072  [].            r
+000136e0: 6574 7572 6e0a 0a20 2020 2020 2020 2023  eturn..        #
+000136f0: 2043 7265 6174 6520 7468 6520 636f 6c75   Create the colu
+00013700: 6d6e 2064 6573 6372 6970 7469 6f6e 730a  mn descriptions.
+00013710: 2020 2020 2020 2020 726f 7720 3d20 726f          row = ro
+00013720: 7773 5b30 5d0a 2020 2020 2020 2020 666f  ws[0].        fo
+00013730: 7220 6669 656c 6420 696e 2072 6f77 2e5f  r field in row._
+00013740: 6669 656c 6473 3a0a 2020 2020 2020 2020  fields:.        
+00013750: 2020 2020 7365 6c66 2e64 6573 6372 6970      self.descrip
+00013760: 7469 6f6e 2e61 7070 656e 6428 0a20 2020  tion.append(.   
+00013770: 2020 2020 2020 2020 2020 2020 2028 0a20               (. 
+00013780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013790: 2020 2066 6965 6c64 2c0a 2020 2020 2020     field,.      
+000137a0: 2020 2020 2020 2020 2020 2020 2020 5479                Ty
+000137b0: 7065 436f 6465 732e 636c 735f 746f 5f74  peCodes.cls_to_t
+000137c0: 7970 6528 726f 772e 5f66 6965 6c64 5f74  ype(row._field_t
+000137d0: 7970 6573 5b66 6965 6c64 5d29 2c0a 2020  ypes[field]),.  
+000137e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000137f0: 2020 4e6f 6e65 2c0a 2020 2020 2020 2020    None,.        
+00013800: 2020 2020 2020 2020 2020 2020 4e6f 6e65              None
+00013810: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00013820: 2020 2020 2020 4e6f 6e65 2c0a 2020 2020        None,.    
+00013830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013840: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00013850: 2020 2020 2020 2020 2020 4e6f 6e65 2c0a            None,.
+00013860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013870: 2920 2023 2064 6973 706c 6179 5f73 697a  )  # display_siz
+00013880: 6520 2023 2069 6e74 6572 6e61 6c5f 7369  e  # internal_si
+00013890: 7a65 2020 2320 7072 6563 6973 696f 6e20  ze  # precision 
+000138a0: 2023 2073 6361 6c65 2020 2320 6e75 6c6c   # scale  # null
+000138b0: 5f6f 6b0a 2020 2020 2020 2020 2020 2020  _ok.            
+000138c0: 290a 0a20 2020 2020 2020 2023 2061 6e64  )..        # and
+000138d0: 2073 6574 2074 6865 2072 6573 756c 7473   set the results
+000138e0: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+000138f0: 7374 5f72 6573 756c 7420 3d20 726f 7773  st_result = rows
+00013900: 0a0a 2020 2020 6465 6620 5f67 6574 5f72  ..    def _get_r
+00013910: 6573 756c 745f 6d65 7461 6461 7461 2873  esult_metadata(s
+00013920: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+00013930: 2020 2020 2020 2222 2249 6e74 6572 6e61        """Interna
+00013940: 6c20 726f 7574 696e 6520 746f 2067 6574  l routine to get
+00013950: 206d 6574 6164 6174 6120 666f 7220 6120   metadata for a 
+00013960: 7265 7375 6c74 2073 6574 2222 220a 2020  result set""".  
+00013970: 2020 2020 2020 2320 7079 6c69 6e74 3a20        # pylint: 
+00013980: 6469 7361 626c 653d 6e6f 2d6d 656d 6265  disable=no-membe
+00013990: 720a 2020 2020 2020 2020 7265 7120 3d20  r.        req = 
+000139a0: 7072 6f74 6f2e 5265 7175 6573 7428 290a  proto.Request().
+000139b0: 2020 2020 2020 2020 7265 712e 7479 7065          req.type
+000139c0: 203d 2072 6571 2e46 4554 4348 5f4d 4554   = req.FETCH_MET
+000139d0: 4144 4154 410a 0a20 2020 2020 2020 205f  ADATA..        _
+000139e0: 7365 6e64 5f6d 7367 2873 656c 662e 636f  send_msg(self.co
+000139f0: 6e6e 6563 7469 6f6e 2c20 7265 7129 0a0a  nnection, req)..
+00013a00: 2020 2020 2020 2020 7273 7020 3d20 5f72          rsp = _r
+00013a10: 6563 765f 6d73 6728 7365 6c66 2e63 6f6e  ecv_msg(self.con
+00013a20: 6e65 6374 696f 6e2c 2070 726f 746f 2e46  nection, proto.F
+00013a30: 6574 6368 4d65 7461 6461 7461 5265 7370  etchMetadataResp
+00013a40: 6f6e 7365 2829 290a 2020 2020 2020 2020  onse()).        
+00013a50: 6966 2072 7370 2e72 6573 706f 6e73 652e  if rsp.response.
+00013a60: 7479 7065 203d 3d20 7072 6f74 6f2e 436f  type == proto.Co
+00013a70: 6e66 6972 6d61 7469 6f6e 5265 7370 6f6e  nfirmationRespon
+00013a80: 7365 2e52 4553 504f 4e53 455f 5741 524e  se.RESPONSE_WARN
+00013a90: 3a0a 2020 2020 2020 2020 2020 2020 7761  :.            wa
+00013aa0: 726e 2872 7370 2e72 6573 706f 6e73 652e  rn(rsp.response.
+00013ab0: 7265 6173 6f6e 290a 2020 2020 2020 2020  reason).        
+00013ac0: 656c 6966 206e 6f74 2072 7370 2e72 6573  elif not rsp.res
+00013ad0: 706f 6e73 652e 7479 7065 203d 3d20 7072  ponse.type == pr
+00013ae0: 6f74 6f2e 436f 6e66 6972 6d61 7469 6f6e  oto.Confirmation
+00013af0: 5265 7370 6f6e 7365 2e52 4553 504f 4e53  Response.RESPONS
+00013b00: 455f 4f4b 3a0a 2020 2020 2020 2020 2020  E_OK:.          
+00013b10: 2020 7261 6973 6520 5f63 6f6e 7665 7274    raise _convert
+00013b20: 5f65 7863 6570 7469 6f6e 2872 7370 2e72  _exception(rsp.r
+00013b30: 6573 706f 6e73 6529 0a0a 2020 2020 2020  esponse)..      
+00013b40: 2020 636f 6c73 203d 207b 7d0a 2020 2020    cols = {}.    
+00013b50: 2020 2020 666f 7220 6b65 792c 2076 616c      for key, val
+00013b60: 7565 2069 6e20 7273 702e 636f 6c73 3270  ue in rsp.cols2p
+00013b70: 6f73 2e69 7465 6d73 2829 3a0a 2020 2020  os.items():.    
+00013b80: 2020 2020 2020 2020 636f 6c73 5b76 616c          cols[val
+00013b90: 7565 5d20 3d20 6b65 790a 0a20 2020 2020  ue] = key..     
+00013ba0: 2020 2073 656c 662e 6465 7363 7269 7074     self.descript
+00013bb0: 696f 6e20 3d20 5b5d 0a20 2020 2020 2020  ion = [].       
+00013bc0: 2063 6f6c 6e61 6d65 7320 3d20 5b5d 0a20   colnames = []. 
+00013bd0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00013be0: 7261 6e67 6528 6c65 6e28 636f 6c73 2929  range(len(cols))
+00013bf0: 3a20 2023 2070 796c 696e 743a 2064 6973  :  # pylint: dis
+00013c00: 6162 6c65 3d63 6f6e 7369 6465 722d 7573  able=consider-us
+00013c10: 696e 672d 656e 756d 6572 6174 650a 2020  ing-enumerate.  
+00013c20: 2020 2020 2020 2020 2020 6e61 6d65 203d            name =
+00013c30: 2063 6f6c 735b 695d 0a20 2020 2020 2020   cols[i].       
+00013c40: 2020 2020 2023 2054 6869 7320 7475 706c       # This tupl
+00013c50: 6520 6973 2064 6566 696e 6564 2069 6e20  e is defined in 
+00013c60: 5045 5020 3234 390a 2020 2020 2020 2020  PEP 249.        
+00013c70: 2020 2020 7365 6c66 2e64 6573 6372 6970      self.descrip
+00013c80: 7469 6f6e 2e61 7070 656e 6428 0a20 2020  tion.append(.   
+00013c90: 2020 2020 2020 2020 2020 2020 2028 0a20               (. 
+00013ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013cb0: 2020 206e 616d 652c 0a20 2020 2020 2020     name,.       
+00013cc0: 2020 2020 2020 2020 2020 2020 2054 7970               Typ
+00013cd0: 6543 6f64 6573 2e74 6f5f 7479 7065 2872  eCodes.to_type(r
+00013ce0: 7370 2e63 6f6c 7332 5479 7065 735b 6e61  sp.cols2Types[na
+00013cf0: 6d65 5d29 2c0a 2020 2020 2020 2020 2020  me]),.          
+00013d00: 2020 2020 2020 2020 2020 4e6f 6e65 2c0a            None,.
+00013d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d20: 2020 2020 4e6f 6e65 2c0a 2020 2020 2020      None,.      
+00013d30: 2020 2020 2020 2020 2020 2020 2020 4e6f                No
+00013d40: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00013d50: 2020 2020 2020 2020 4e6f 6e65 2c0a 2020          None,.  
+00013d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d70: 2020 4e6f 6e65 2c0a 2020 2020 2020 2020    None,.        
+00013d80: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00013d90: 2020 2020 2020 2920 2023 2064 6973 706c        )  # displ
+00013da0: 6179 5f73 697a 6520 2023 2069 6e74 6572  ay_size  # inter
+00013db0: 6e61 6c5f 7369 7a65 2020 2320 7072 6563  nal_size  # prec
+00013dc0: 6973 696f 6e20 2023 2073 6361 6c65 2020  ision  # scale  
+00013dd0: 2320 6e75 6c6c 5f6f 6b0a 2020 2020 2020  # null_ok.      
+00013de0: 2020 2020 2020 636f 6c6e 616d 6573 2e61        colnames.a
+00013df0: 7070 656e 6428 6e61 6d65 290a 2020 2020  ppend(name).    
+00013e00: 2020 2020 7365 6c66 2e72 6573 756c 7473      self.results
+00013e10: 6574 5f74 7570 6c65 203d 206e 616d 6564  et_tuple = named
+00013e20: 7475 706c 6528 2252 6f77 222c 2063 6f6c  tuple("Row", col
+00013e30: 6e61 6d65 732c 2072 656e 616d 653d 5472  names, rename=Tr
+00013e40: 7565 2920 2023 2074 7970 653a 2069 676e  ue)  # type: ign
+00013e50: 6f72 650a 0a20 2020 2064 6566 205f 6578  ore..    def _ex
+00013e60: 6563 7574 655f 7570 6461 7465 2873 656c  ecute_update(sel
+00013e70: 662c 206f 7065 7261 7469 6f6e 3a20 7374  f, operation: st
+00013e80: 7229 202d 3e20 4e6f 6e65 3a0a 2020 2020  r) -> None:.    
+00013e90: 2020 2020 2222 2245 7865 6375 7465 2061      """Execute a
+00013ea0: 6e20 7570 6461 7465 2073 7461 7465 6d65  n update stateme
+00013eb0: 6e74 2222 220a 2020 2020 2020 2020 2320  nt""".        # 
+00013ec0: 7079 6c69 6e74 3a20 6469 7361 626c 653d  pylint: disable=
+00013ed0: 6e6f 2d6d 656d 6265 720a 2020 2020 2020  no-member.      
+00013ee0: 2020 2320 5768 696c 6520 7765 2061 7265    # While we are
+00013ef0: 2072 6564 6972 6563 7469 6e67 2e2e 2e0a   redirecting....
+00013f00: 0a20 2020 2020 2020 2023 2054 6865 7265  .        # There
+00013f10: 2069 7320 6e6f 2072 6573 756c 7473 6574   is no resultset
+00013f20: 2064 6174 6120 6672 6f6d 2061 6e20 7570   data from an up
+00013f30: 6461 7465 0a20 2020 2020 2020 2073 656c  date.        sel
+00013f40: 662e 656e 645f 6f66 5f64 6174 6120 3d20  f.end_of_data = 
+00013f50: 5472 7565 0a0a 2020 2020 2020 2020 7768  True..        wh
+00013f60: 696c 6520 5472 7565 3a0a 2020 2020 2020  ile True:.      
+00013f70: 2020 2020 2020 7265 7120 3d20 7072 6f74        req = prot
+00013f80: 6f2e 5265 7175 6573 7428 290a 2020 2020  o.Request().    
+00013f90: 2020 2020 2020 2020 7265 712e 7479 7065          req.type
+00013fa0: 203d 2072 6571 2e45 5845 4355 5445 5f55   = req.EXECUTE_U
+00013fb0: 5044 4154 450a 2020 2020 2020 2020 2020  PDATE.          
+00013fc0: 2020 7265 712e 6578 6563 7574 655f 7570    req.execute_up
+00013fd0: 6461 7465 2e73 716c 203d 206f 7065 7261  date.sql = opera
+00013fe0: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+00013ff0: 2061 7373 6572 7420 7365 6c66 2e63 6f6e   assert self.con
+00014000: 6e65 6374 696f 6e2e 666f 7263 6520 6973  nection.force is
+00014010: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
+00014020: 2020 2020 2020 7265 712e 6578 6563 7574        req.execut
+00014030: 655f 7570 6461 7465 2e66 6f72 6365 203d  e_update.force =
+00014040: 2073 656c 662e 636f 6e6e 6563 7469 6f6e   self.connection
+00014050: 2e66 6f72 6365 0a0a 2020 2020 2020 2020  .force..        
+00014060: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00014070: 2020 2020 2020 2020 205f 7365 6e64 5f6d           _send_m
+00014080: 7367 2873 656c 662e 636f 6e6e 6563 7469  sg(self.connecti
+00014090: 6f6e 2c20 7265 7129 0a0a 2020 2020 2020  on, req)..      
+000140a0: 2020 2020 2020 2020 2020 7273 7020 3d20            rsp = 
+000140b0: 5f72 6563 765f 6d73 6728 7365 6c66 2e63  _recv_msg(self.c
+000140c0: 6f6e 6e65 6374 696f 6e2c 2070 726f 746f  onnection, proto
+000140d0: 2e45 7865 6375 7465 5570 6461 7465 5265  .ExecuteUpdateRe
+000140e0: 7370 6f6e 7365 2829 290a 2020 2020 2020  sponse()).      
+000140f0: 2020 2020 2020 6578 6365 7074 2049 4f45        except IOE
+00014100: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
+00014110: 2020 2020 2020 2320 7265 6d61 6b65 206f        # remake o
+00014120: 7572 2063 6f6e 6e65 6374 696f 6e0a 2020  ur connection.  
+00014130: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00014140: 6c66 2e63 6f6e 6e65 6374 696f 6e20 3d20  lf.connection = 
+00014150: 436f 6e6e 6563 7469 6f6e 280a 2020 2020  Connection(.    
+00014160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014170: 7573 6572 3d73 656c 662e 636f 6e6e 6563  user=self.connec
+00014180: 7469 6f6e 2e75 7365 722c 0a20 2020 2020  tion.user,.     
+00014190: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000141a0: 6173 7377 6f72 643d 7365 6c66 2e63 6f6e  assword=self.con
+000141b0: 6e65 6374 696f 6e2e 7061 7373 776f 7264  nection.password
+000141c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000141d0: 2020 2020 2020 686f 7374 3d66 227b 272c        host=f"{',
+000141e0: 272e 6a6f 696e 2873 656c 662e 636f 6e6e  '.join(self.conn
+000141f0: 6563 7469 6f6e 2e68 6f73 7473 297d 3a7b  ection.hosts)}:{
+00014200: 7365 6c66 2e63 6f6e 6e65 6374 696f 6e2e  self.connection.
+00014210: 706f 7274 7d22 2c0a 2020 2020 2020 2020  port}",.        
+00014220: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00014230: 6261 7365 3d73 656c 662e 636f 6e6e 6563  base=self.connec
+00014240: 7469 6f6e 2e64 6174 6162 6173 652c 0a20  tion.database,. 
+00014250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014260: 2020 2074 6c73 3d73 656c 662e 636f 6e6e     tls=self.conn
+00014270: 6563 7469 6f6e 2e74 6c73 2c0a 2020 2020  ection.tls,.    
+00014280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014290: 6861 6e64 7368 616b 653d 7365 6c66 2e63  handshake=self.c
+000142a0: 6f6e 6e65 6374 696f 6e2e 6861 6e64 7368  onnection.handsh
+000142b0: 616b 652c 0a20 2020 2020 2020 2020 2020  ake,.           
+000142c0: 2020 2020 2020 2020 2066 6f72 6365 3d73           force=s
+000142d0: 656c 662e 636f 6e6e 6563 7469 6f6e 2e66  elf.connection.f
+000142e0: 6f72 6365 2c0a 2020 2020 2020 2020 2020  orce,.          
+000142f0: 2020 2020 2020 2020 2020 7365 7373 696f            sessio
+00014300: 6e3d 7365 6c66 2e63 6f6e 6e65 6374 696f  n=self.connectio
+00014310: 6e2e 7365 7373 696f 6e2c 0a20 2020 2020  n.session,.     
+00014320: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00014330: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00014340: 6e74 696e 7565 0a0a 2020 2020 2020 2020  ntinue..        
+00014350: 2020 2020 6966 2072 7370 2e72 6573 706f      if rsp.respo
+00014360: 6e73 652e 7479 7065 203d 3d20 7072 6f74  nse.type == prot
+00014370: 6f2e 436f 6e66 6972 6d61 7469 6f6e 5265  o.ConfirmationRe
+00014380: 7370 6f6e 7365 2e52 4553 504f 4e53 455f  sponse.RESPONSE_
+00014390: 5741 524e 3a0a 2020 2020 2020 2020 2020  WARN:.          
+000143a0: 2020 2020 2020 7761 726e 2872 7370 2e72        warn(rsp.r
+000143b0: 6573 706f 6e73 652e 7265 6173 6f6e 290a  esponse.reason).
+000143c0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+000143d0: 206e 6f74 2072 7370 2e72 6573 706f 6e73   not rsp.respons
+000143e0: 652e 7479 7065 203d 3d20 7072 6f74 6f2e  e.type == proto.
+000143f0: 436f 6e66 6972 6d61 7469 6f6e 5265 7370  ConfirmationResp
+00014400: 6f6e 7365 2e52 4553 504f 4e53 455f 4f4b  onse.RESPONSE_OK
+00014410: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014420: 2020 6966 2072 7370 2e72 6573 706f 6e73    if rsp.respons
+00014430: 652e 7665 6e64 6f72 5f63 6f64 6520 3d3d  e.vendor_code ==
+00014440: 2053 4553 5349 4f4e 5f45 5850 4952 4544   SESSION_EXPIRED
+00014450: 5f43 4f44 453a 0a20 2020 2020 2020 2020  _CODE:.         
+00014460: 2020 2020 2020 2020 2020 2023 204e 6565             # Nee
+00014470: 6420 746f 2072 6566 7265 7368 2074 6865  d to refresh the
+00014480: 2073 6573 7369 6f6e 0a20 2020 2020 2020   session.       
+00014490: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000144a0: 662e 636f 6e6e 6563 7469 6f6e 2e72 6566  f.connection.ref
+000144b0: 7265 7368 2829 0a20 2020 2020 2020 2020  resh().         
+000144c0: 2020 2020 2020 2020 2020 2023 2061 6e64             # and
+000144d0: 2074 7279 2061 6761 696e 0a20 2020 2020   try again.     
+000144e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000144f0: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
+00014500: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00014510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014520: 2020 7261 6973 6520 5f63 6f6e 7665 7274    raise _convert
+00014530: 5f65 7863 6570 7469 6f6e 2872 7370 2e72  _exception(rsp.r
+00014540: 6573 706f 6e73 6529 0a0a 2020 2020 2020  esponse)..      
+00014550: 2020 2020 2020 2320 7365 6520 6966 2077        # see if w
+00014560: 6520 6172 6520 6265 696e 6720 746f 6c64  e are being told
+00014570: 2074 6f20 7265 6469 7265 6374 0a20 2020   to redirect.   
+00014580: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00014590: 7273 702e 7265 6469 7265 6374 3a0a 2020  rsp.redirect:.  
+000145a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000145b0: 6c66 2e72 6f77 636f 756e 7420 3d20 7273  lf.rowcount = rs
+000145c0: 702e 7570 6461 7465 526f 7743 6f75 6e74  p.updateRowCount
+000145d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000145e0: 2062 7265 616b 0a0a 2020 2020 2020 2020   break..        
+000145f0: 2020 2020 2320 7265 6d61 6b65 206f 7572      # remake our
+00014600: 2063 6f6e 6e65 6374 696f 6e0a 2020 2020   connection.    
+00014610: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00014620: 6e65 6374 696f 6e20 3d20 7365 6c66 2e63  nection = self.c
+00014630: 6f6e 6e65 6374 696f 6e2e 7265 6469 7265  onnection.redire
+00014640: 6374 2872 7370 2e72 6564 6972 6563 7448  ct(rsp.redirectH
+00014650: 6f73 742c 2072 7370 2e72 6564 6972 6563  ost, rsp.redirec
+00014660: 7450 6f72 7429 0a0a 2020 2020 6465 6620  tPort)..    def 
+00014670: 5f65 7865 6375 7465 5f66 6f72 6365 2873  _execute_force(s
+00014680: 656c 662c 206f 7065 7261 7469 6f6e 3a20  elf, operation: 
+00014690: 7374 7229 202d 3e20 4e6f 6e65 3a0a 2020  str) -> None:.  
+000146a0: 2020 2020 2020 6966 206f 7065 7261 7469        if operati
+000146b0: 6f6e 2e73 7472 6970 2829 2e75 7070 6572  on.strip().upper
+000146c0: 2829 203d 3d20 2246 4f52 4345 2052 4544  () == "FORCE RED
+000146d0: 4952 4543 5422 3a0a 2020 2020 2020 2020  IRECT":.        
+000146e0: 2020 2020 2320 5365 7473 2074 6865 206e      # Sets the n
+000146f0: 6578 7420 636f 6d6d 616e 6420 7468 6174  ext command that
+00014700: 2069 7320 6578 6563 7574 6520 7175 6572   is execute quer
+00014710: 7920 746f 2072 6564 6972 6563 740a 2020  y to redirect.  
+00014720: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00014730: 6f6e 6e65 6374 696f 6e2e 666f 7263 655f  onnection.force_
+00014740: 6e65 7874 5f72 6564 6972 6563 7420 3d20  next_redirect = 
+00014750: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
+00014760: 2073 656c 662e 656e 645f 6f66 5f64 6174   self.end_of_dat
+00014770: 6120 3d20 5472 7565 0a20 2020 2020 2020  a = True.       
+00014780: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00014790: 2020 2023 2046 6f72 6365 2065 7874 6572     # Force exter
+000147a0: 6e61 6c20 636f 6d6d 616e 640a 2020 2020  nal command.    
+000147b0: 2020 2020 2020 2020 7365 6c66 2e5f 6578          self._ex
+000147c0: 6563 7574 655f 666f 7263 655f 6578 7465  ecute_force_exte
+000147d0: 726e 616c 286f 7065 7261 7469 6f6e 290a  rnal(operation).
+000147e0: 0a20 2020 2064 6566 205f 6578 6563 7574  .    def _execut
+000147f0: 655f 666f 7263 655f 6578 7465 726e 616c  e_force_external
+00014800: 2873 656c 662c 206f 7065 7261 7469 6f6e  (self, operation
+00014810: 3a20 7374 7229 202d 3e20 4e6f 6e65 3a0a  : str) -> None:.
+00014820: 2020 2020 2020 2020 2320 7079 6c69 6e74          # pylint
+00014830: 3a20 6469 7361 626c 653d 6e6f 2d6d 656d  : disable=no-mem
+00014840: 6265 720a 2020 2020 2020 2020 2320 5768  ber.        # Wh
+00014850: 696c 6520 7765 2061 7265 2072 6564 6972  ile we are redir
+00014860: 6563 7469 6e67 2e2e 2e0a 2020 2020 2020  ecting....      
+00014870: 2020 6661 6374 6f72 7920 3d20 5f4f 4349    factory = _OCI
+00014880: 454e 545f 5245 5155 4553 545f 4641 4354  ENT_REQUEST_FACT
+00014890: 4f52 4945 535b 2246 4f52 4345 225d 0a20  ORIES["FORCE"]. 
+000148a0: 2020 2020 2020 2072 6571 203d 2066 6163         req = fac
+000148b0: 746f 7279 2e72 6571 7565 7374 286f 7065  tory.request(ope
+000148c0: 7261 7469 6f6e 3d6f 7065 7261 7469 6f6e  ration=operation
+000148d0: 290a 0a20 2020 2020 2020 205f 7365 6e64  )..        _send
+000148e0: 5f6d 7367 2873 656c 662e 636f 6e6e 6563  _msg(self.connec
+000148f0: 7469 6f6e 2c20 7265 7129 0a0a 2020 2020  tion, req)..    
+00014900: 2020 2020 7273 7020 3d20 5f72 6563 765f      rsp = _recv_
+00014910: 6d73 6728 7365 6c66 2e63 6f6e 6e65 6374  msg(self.connect
+00014920: 696f 6e2c 2070 726f 746f 2e43 6f6e 6669  ion, proto.Confi
+00014930: 726d 6174 696f 6e52 6573 706f 6e73 6528  rmationResponse(
+00014940: 2929 0a0a 2020 2020 2020 2020 6966 2072  ))..        if r
+00014950: 7370 2e74 7970 6520 3d3d 2070 726f 746f  sp.type == proto
+00014960: 2e43 6f6e 6669 726d 6174 696f 6e52 6573  .ConfirmationRes
+00014970: 706f 6e73 652e 5245 5350 4f4e 5345 5f57  ponse.RESPONSE_W
+00014980: 4152 4e3a 0a20 2020 2020 2020 2020 2020  ARN:.           
+00014990: 2077 6172 6e28 7273 702e 7265 6173 6f6e   warn(rsp.reason
+000149a0: 290a 2020 2020 2020 2020 656c 6966 206e  ).        elif n
+000149b0: 6f74 2072 7370 2e74 7970 6520 3d3d 2070  ot rsp.type == p
+000149c0: 726f 746f 2e43 6f6e 6669 726d 6174 696f  roto.Confirmatio
+000149d0: 6e52 6573 706f 6e73 652e 5245 5350 4f4e  nResponse.RESPON
+000149e0: 5345 5f4f 4b3a 0a20 2020 2020 2020 2020  SE_OK:.         
+000149f0: 2020 2072 6169 7365 205f 636f 6e76 6572     raise _conver
+00014a00: 745f 6578 6365 7074 696f 6e28 7273 7029  t_exception(rsp)
+00014a10: 0a0a 2020 2020 6465 6620 5f65 7865 6375  ..    def _execu
+00014a20: 7465 5f73 6574 2873 656c 662c 2070 6172  te_set(self, par
+00014a30: 616d 733a 2053 6571 7565 6e63 655b 7374  ams: Sequence[st
+00014a40: 725d 2920 2d3e 204e 6f6e 653a 0a20 2020  r]) -> None:.   
+00014a50: 2020 2020 2069 6620 6c65 6e28 7061 7261       if len(para
+00014a60: 6d73 2920 213d 2032 3a0a 2020 2020 2020  ms) != 2:.      
+00014a70: 2020 2020 2020 7261 6973 6520 5072 6f67        raise Prog
+00014a80: 7261 6d6d 696e 6745 7272 6f72 2872 6561  rammingError(rea
+00014a90: 736f 6e3d 2253 796e 7461 7820 6572 726f  son="Syntax erro
+00014aa0: 7222 290a 0a20 2020 2020 2020 2023 2054  r")..        # T
+00014ab0: 6865 7265 2069 7320 6e6f 2072 6573 756c  here is no resul
+00014ac0: 7473 6574 2064 6174 6120 6672 6f6d 2061  tset data from a
+00014ad0: 6e20 7570 6461 7465 0a20 2020 2020 2020  n update.       
+00014ae0: 2073 656c 662e 656e 645f 6f66 5f64 6174   self.end_of_dat
+00014af0: 6120 3d20 5472 7565 0a0a 2020 2020 2020  a = True..      
+00014b00: 2020 6f70 203d 2070 6172 616d 735b 305d    op = params[0]
+00014b10: 2e75 7070 6572 2829 0a20 2020 2020 2020  .upper().       
+00014b20: 2076 616c 3a20 556e 696f 6e5b 696e 742c   val: Union[int,
+00014b30: 2073 7472 2c20 666c 6f61 745d 0a20 2020   str, float].   
+00014b40: 2020 2020 2076 616c 203d 2070 6172 616d       val = param
+00014b50: 735b 315d 2e73 7472 6970 2829 0a0a 2020  s[1].strip()..  
+00014b60: 2020 2020 2020 6661 6374 6f72 793a 2055        factory: U
+00014b70: 6e69 6f6e 5b5f 5365 7453 6368 656d 6146  nion[_SetSchemaF
+00014b80: 6163 746f 7279 2c20 5f53 6574 5061 7261  actory, _SetPara
+00014b90: 6d65 7465 7246 6163 746f 7279 5d0a 2020  meterFactory].  
+00014ba0: 2020 2020 2020 6966 206f 7020 3d3d 2022        if op == "
+00014bb0: 5343 4845 4d41 223a 0a20 2020 2020 2020  SCHEMA":.       
+00014bc0: 2020 2020 2066 6163 746f 7279 203d 205f       factory = _
+00014bd0: 5365 7453 6368 656d 6146 6163 746f 7279  SetSchemaFactory
+00014be0: 2829 0a20 2020 2020 2020 2020 2020 2072  ().            r
+00014bf0: 6571 203d 2066 6163 746f 7279 2e72 6571  eq = factory.req
+00014c00: 7565 7374 2876 616c 290a 2020 2020 2020  uest(val).      
+00014c10: 2020 656c 6966 206f 7020 3d3d 2022 5345    elif op == "SE
+00014c20: 5256 4943 4543 4c41 5353 223a 2020 2320  RVICECLASS":  # 
+00014c30: 5365 7276 6963 6520 436c 6173 7365 7320  Service Classes 
+00014c40: 7461 6b65 2073 7472 696e 6720 7061 7261  take string para
+00014c50: 6d65 7465 7273 2c20 6e6f 7420 696e 740a  meters, not int.
+00014c60: 2020 2020 2020 2020 2020 2020 6661 6374              fact
+00014c70: 6f72 7920 3d20 5f53 6574 5061 7261 6d65  ory = _SetParame
+00014c80: 7465 7246 6163 746f 7279 2829 0a20 2020  terFactory().   
+00014c90: 2020 2020 2020 2020 2072 6571 203d 2066           req = f
+00014ca0: 6163 746f 7279 2e72 6571 7565 7374 286f  actory.request(o
+00014cb0: 702c 2076 616c 290a 2020 2020 2020 2020  p, val).        
+00014cc0: 656c 6966 206f 7020 3d3d 2022 5053 4f22  elif op == "PSO"
+00014cd0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00014ce0: 5053 4f20 7375 7070 6f72 7473 2027 6f6e  PSO supports 'on
+00014cf0: 2720 616e 6420 276f 6666 2720 696e 7374  ' and 'off' inst
+00014d00: 6561 6420 6f66 2027 7265 7365 7427 2e20  ead of 'reset'. 
+00014d10: 276f 6e27 2069 7320 6571 7569 7661 6c65  'on' is equivale
+00014d20: 6e74 2c20 616e 6420 276f 6666 2720 6469  nt, and 'off' di
+00014d30: 7361 626c 6573 2028 6571 7569 7661 6c65  sables (equivale
+00014d40: 6e74 2074 6f20 6120 6e65 6761 7469 7665  nt to a negative
+00014d50: 2076 616c 7565 290a 2020 2020 2020 2020   value).        
+00014d60: 2020 2020 7661 6c20 3d20 7661 6c2e 6c6f      val = val.lo
+00014d70: 7765 7228 290a 2020 2020 2020 2020 2020  wer().          
+00014d80: 2020 6966 2076 616c 203d 3d20 226f 6e22    if val == "on"
+00014d90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014da0: 2020 7661 6c20 3d20 2272 6573 6574 220a    val = "reset".
+00014db0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00014dc0: 2076 616c 203d 3d20 226f 6666 223a 0a20   val == "off":. 
+00014dd0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00014de0: 616c 203d 202d 310a 2020 2020 2020 2020  al = -1.        
+00014df0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00014e00: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+00014e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e20: 2020 2076 616c 203d 2069 6e74 2876 616c     val = int(val
+00014e30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00014e40: 2020 6578 6365 7074 2056 616c 7565 4572    except ValueEr
+00014e50: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
+00014e60: 2020 2020 2020 2020 2072 6169 7365 2050           raise P
+00014e70: 726f 6772 616d 6d69 6e67 4572 726f 7228  rogrammingError(
+00014e80: 7265 6173 6f6e 3d22 5379 6e74 6178 2065  reason="Syntax e
+00014e90: 7272 6f72 2069 6e20 5345 542e 2056 616c  rror in SET. Val
+00014ea0: 7565 206d 7573 7420 6265 206e 756d 6572  ue must be numer
+00014eb0: 6963 2c20 276f 6e27 2c20 6f72 2027 6f66  ic, 'on', or 'of
+00014ec0: 6627 2229 0a20 2020 2020 2020 2020 2020  f'").           
+00014ed0: 2066 6163 746f 7279 203d 205f 5365 7450   factory = _SetP
+00014ee0: 6172 616d 6574 6572 4661 6374 6f72 7928  arameterFactory(
+00014ef0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00014f00: 7120 3d20 6661 6374 6f72 792e 7265 7175  q = factory.requ
+00014f10: 6573 7428 6f70 2c20 7661 6c29 0a20 2020  est(op, val).   
+00014f20: 2020 2020 2065 6c69 6620 6f70 2069 6e20       elif op in 
+00014f30: 5b22 4144 4a55 5354 4641 4354 4f52 222c  ["ADJUSTFACTOR",
+00014f40: 2022 5052 494f 5249 5459 225d 3a0a 2020   "PRIORITY"]:.  
+00014f50: 2020 2020 2020 2020 2020 6966 2076 616c            if val
+00014f60: 2e6c 6f77 6572 2829 2021 3d20 2272 6573  .lower() != "res
+00014f70: 6574 223a 0a20 2020 2020 2020 2020 2020  et":.           
+00014f80: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00014f90: 2020 2020 2020 2020 2020 2020 2020 7661                va
+00014fa0: 6c20 3d20 666c 6f61 7428 7661 6c29 0a20  l = float(val). 
+00014fb0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00014fc0: 7863 6570 7420 5661 6c75 6545 7272 6f72  xcept ValueError
+00014fd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014fe0: 2020 2020 2020 7261 6973 6520 5072 6f67        raise Prog
+00014ff0: 7261 6d6d 696e 6745 7272 6f72 2872 6561  rammingError(rea
+00015000: 736f 6e3d 2253 796e 7461 7820 6572 726f  son="Syntax erro
+00015010: 7220 696e 2053 4554 2e20 5661 6c75 6520  r in SET. Value 
+00015020: 6d75 7374 2062 6520 6e75 6d65 7269 6320  must be numeric 
+00015030: 6f72 2027 7265 7365 7427 2229 0a20 2020  or 'reset'").   
+00015040: 2020 2020 2020 2020 2066 6163 746f 7279           factory
+00015050: 203d 205f 5365 7450 6172 616d 6574 6572   = _SetParameter
+00015060: 4661 6374 6f72 7928 290a 2020 2020 2020  Factory().      
+00015070: 2020 2020 2020 7265 7120 3d20 6661 6374        req = fact
+00015080: 6f72 792e 7265 7175 6573 7428 6f70 2c20  ory.request(op, 
+00015090: 7661 6c29 0a20 2020 2020 2020 2065 6c73  val).        els
+000150a0: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+000150b0: 6620 7661 6c2e 6c6f 7765 7228 2920 213d  f val.lower() !=
+000150c0: 2022 7265 7365 7422 3a0a 2020 2020 2020   "reset":.      
+000150d0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+000150e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000150f0: 2020 2076 616c 203d 2069 6e74 2876 616c     val = int(val
+00015100: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00015110: 2020 6578 6365 7074 2056 616c 7565 4572    except ValueEr
+00015120: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
+00015130: 2020 2020 2020 2020 2072 6169 7365 2050           raise P
+00015140: 726f 6772 616d 6d69 6e67 4572 726f 7228  rogrammingError(
+00015150: 7265 6173 6f6e 3d22 5379 6e74 6178 2065  reason="Syntax e
+00015160: 7272 6f72 2069 6e20 5345 542e 2056 616c  rror in SET. Val
+00015170: 7565 206d 7573 7420 6265 206e 756d 6572  ue must be numer
+00015180: 6963 206f 7220 2772 6573 6574 2722 290a  ic or 'reset'").
+00015190: 2020 2020 2020 2020 2020 2020 6661 6374              fact
+000151a0: 6f72 7920 3d20 5f53 6574 5061 7261 6d65  ory = _SetParame
+000151b0: 7465 7246 6163 746f 7279 2829 0a20 2020  terFactory().   
+000151c0: 2020 2020 2020 2020 2072 6571 203d 2066           req = f
+000151d0: 6163 746f 7279 2e72 6571 7565 7374 286f  actory.request(o
+000151e0: 702c 2076 616c 290a 0a20 2020 2020 2020  p, val)..       
+000151f0: 205f 7365 6e64 5f6d 7367 2873 656c 662e   _send_msg(self.
+00015200: 636f 6e6e 6563 7469 6f6e 2c20 7265 7129  connection, req)
+00015210: 0a0a 2020 2020 2020 2020 7273 7020 3d20  ..        rsp = 
+00015220: 5f72 6563 765f 6d73 6728 7365 6c66 2e63  _recv_msg(self.c
+00015230: 6f6e 6e65 6374 696f 6e2c 2066 6163 746f  onnection, facto
+00015240: 7279 2e72 6573 706f 6e73 6528 2929 0a0a  ry.response())..
+00015250: 2020 2020 2020 2020 6966 2072 7370 2e74          if rsp.t
+00015260: 7970 6520 3d3d 2070 726f 746f 2e43 6f6e  ype == proto.Con
+00015270: 6669 726d 6174 696f 6e52 6573 706f 6e73  firmationRespons
+00015280: 652e 5245 5350 4f4e 5345 5f57 4152 4e3a  e.RESPONSE_WARN:
+00015290: 0a20 2020 2020 2020 2020 2020 2077 6172  .            war
+000152a0: 6e28 7273 702e 7265 6173 6f6e 290a 2020  n(rsp.reason).  
+000152b0: 2020 2020 2020 656c 6966 206e 6f74 2072        elif not r
+000152c0: 7370 2e74 7970 6520 3d3d 2070 726f 746f  sp.type == proto
+000152d0: 2e43 6f6e 6669 726d 6174 696f 6e52 6573  .ConfirmationRes
+000152e0: 706f 6e73 652e 5245 5350 4f4e 5345 5f4f  ponse.RESPONSE_O
+000152f0: 4b3a 0a20 2020 2020 2020 2020 2020 2069  K:.            i
+00015300: 6620 7273 702e 7665 6e64 6f72 5f63 6f64  f rsp.vendor_cod
+00015310: 6520 3d3d 2053 4553 5349 4f4e 5f45 5850  e == SESSION_EXP
+00015320: 4952 4544 5f43 4f44 453a 0a20 2020 2020  IRED_CODE:.     
+00015330: 2020 2020 2020 2020 2020 2023 204e 6565             # Nee
+00015340: 6420 746f 2072 6566 7265 7368 2074 6865  d to refresh the
+00015350: 2073 6573 7369 6f6e 0a20 2020 2020 2020   session.       
+00015360: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00015370: 6e6e 6563 7469 6f6e 2e72 6566 7265 7368  nnection.refresh
+00015380: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00015390: 2020 2023 2061 6e64 2074 7279 2061 6761     # and try aga
+000153a0: 696e 0a20 2020 2020 2020 2020 2020 2020  in.             
+000153b0: 2020 2073 656c 662e 5f65 7865 6375 7465     self._execute
+000153c0: 5f73 6574 2870 6172 616d 7329 0a20 2020  _set(params).   
+000153d0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+000153e0: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
+000153f0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00015400: 2020 2020 2020 7261 6973 6520 5f63 6f6e        raise _con
+00015410: 7665 7274 5f65 7863 6570 7469 6f6e 2872  vert_exception(r
+00015420: 7370 290a 0a20 2020 2064 6566 205f 6578  sp)..    def _ex
+00015430: 6563 7574 655f 6765 745f 7363 6865 6d61  ecute_get_schema
+00015440: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+00015450: 2020 2020 2020 2020 6661 6374 6f72 7920          factory 
+00015460: 3d20 5f47 6574 5363 6865 6d61 4661 6374  = _GetSchemaFact
+00015470: 6f72 7928 290a 2020 2020 2020 2020 7265  ory().        re
+00015480: 7120 3d20 6661 6374 6f72 792e 7265 7175  q = factory.requ
+00015490: 6573 7428 290a 0a20 2020 2020 2020 205f  est()..        _
+000154a0: 7365 6e64 5f6d 7367 2873 656c 662e 636f  send_msg(self.co
+000154b0: 6e6e 6563 7469 6f6e 2c20 7265 7129 0a0a  nnection, req)..
+000154c0: 2020 2020 2020 2020 7273 7020 3d20 5f72          rsp = _r
+000154d0: 6563 765f 6d73 6728 7365 6c66 2e63 6f6e  ecv_msg(self.con
+000154e0: 6e65 6374 696f 6e2c 2066 6163 746f 7279  nection, factory
+000154f0: 2e72 6573 706f 6e73 6528 2929 0a0a 2020  .response())..  
+00015500: 2020 2020 2020 6966 2072 7370 2e72 6573        if rsp.res
+00015510: 706f 6e73 652e 7479 7065 203d 3d20 7072  ponse.type == pr
+00015520: 6f74 6f2e 436f 6e66 6972 6d61 7469 6f6e  oto.Confirmation
+00015530: 5265 7370 6f6e 7365 2e52 4553 504f 4e53  Response.RESPONS
+00015540: 455f 5741 524e 3a0a 2020 2020 2020 2020  E_WARN:.        
+00015550: 2020 2020 7761 726e 2872 7370 2e72 6573      warn(rsp.res
+00015560: 706f 6e73 652e 7265 6173 6f6e 290a 2020  ponse.reason).  
+00015570: 2020 2020 2020 656c 6966 206e 6f74 2072        elif not r
+00015580: 7370 2e72 6573 706f 6e73 652e 7479 7065  sp.response.type
+00015590: 203d 3d20 7072 6f74 6f2e 436f 6e66 6972   == proto.Confir
+000155a0: 6d61 7469 6f6e 5265 7370 6f6e 7365 2e52  mationResponse.R
+000155b0: 4553 504f 4e53 455f 4f4b 3a0a 2020 2020  ESPONSE_OK:.    
+000155c0: 2020 2020 2020 2020 6966 2072 7370 2e72          if rsp.r
+000155d0: 6573 706f 6e73 652e 7665 6e64 6f72 5f63  esponse.vendor_c
+000155e0: 6f64 6520 3d3d 2053 4553 5349 4f4e 5f45  ode == SESSION_E
+000155f0: 5850 4952 4544 5f43 4f44 453a 0a20 2020  XPIRED_CODE:.   
+00015600: 2020 2020 2020 2020 2020 2020 2023 204e               # N
+00015610: 6565 6420 746f 2072 6566 7265 7368 2074  eed to refresh t
+00015620: 6865 2073 6573 7369 6f6e 0a20 2020 2020  he session.     
+00015630: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015640: 636f 6e6e 6563 7469 6f6e 2e72 6566 7265  connection.refre
+00015650: 7368 2829 0a20 2020 2020 2020 2020 2020  sh().           
+00015660: 2020 2020 2023 2061 6e64 2074 7279 2061       # and try a
+00015670: 6761 696e 0a20 2020 2020 2020 2020 2020  gain.           
+00015680: 2020 2020 2073 656c 662e 5f65 7865 6375       self._execu
+00015690: 7465 5f67 6574 5f73 6368 656d 6128 290a  te_get_schema().
+000156a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000156b0: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
+000156c0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000156d0: 2020 2020 2020 2020 2072 6169 7365 205f           raise _
+000156e0: 636f 6e76 6572 745f 6578 6365 7074 696f  convert_exceptio
+000156f0: 6e28 7273 702e 7265 7370 6f6e 7365 290a  n(rsp.response).
+00015700: 0a20 2020 2020 2020 2073 656c 662e 6465  .        self.de
+00015710: 7363 7269 7074 696f 6e20 3d20 5b0a 2020  scription = [.  
+00015720: 2020 2020 2020 2020 2020 2822 7363 6865            ("sche
+00015730: 6d61 222c 2054 7970 6543 6f64 6573 2e43  ma", TypeCodes.C
+00015740: 4841 522c 204e 6f6e 652c 204e 6f6e 652c  HAR, None, None,
+00015750: 204e 6f6e 652c 204e 6f6e 652c 204e 6f6e   None, None, Non
+00015760: 6529 0a20 2020 2020 2020 205d 2020 2320  e).        ]  # 
+00015770: 6469 7370 6c61 795f 7369 7a65 2020 2320  display_size  # 
+00015780: 696e 7465 726e 616c 5f73 697a 6520 2023  internal_size  #
+00015790: 2070 7265 6369 7369 6f6e 2020 2320 7363   precision  # sc
+000157a0: 616c 6520 2023 206e 756c 6c5f 6f6b 0a0a  ale  # null_ok..
+000157b0: 2020 2020 2020 2020 526f 7720 3d20 6e61          Row = na
+000157c0: 6d65 6474 7570 6c65 2822 526f 7722 2c20  medtuple("Row", 
+000157d0: 2822 7363 6865 6d61 222c 2929 0a20 2020  ("schema",)).   
+000157e0: 2020 2020 2073 656c 662e 6c69 7374 5f72       self.list_r
+000157f0: 6573 756c 7420 3d20 5b52 6f77 2e5f 6d61  esult = [Row._ma
+00015800: 6b65 2828 7273 702e 7363 6865 6d61 2c29  ke((rsp.schema,)
+00015810: 295d 0a0a 2020 2020 2320 4966 2077 6520  )]..    # If we 
+00015820: 6e65 6564 2074 6f20 696d 706c 656d 656e  need to implemen
+00015830: 7420 6d6f 7265 206f 6620 7468 6573 6520  t more of these 
+00015840: 736f 7274 7320 6f66 2063 7573 746f 6d20  sorts of custom 
+00015850: 636f 6d6d 616e 6473 2c20 636f 6e73 6964  commands, consid
+00015860: 6572 0a20 2020 2023 206d 616b 696e 6720  er.    # making 
+00015870: 6120 6661 6374 6f72 7920 666f 7220 7468  a factory for th
+00015880: 6520 6465 7363 7269 7074 696f 6e20 616e  e description an
+00015890: 6420 7265 7375 6c74 732e 0a20 2020 2064  d results..    d
+000158a0: 6566 205f 6578 6563 7574 655f 6765 745f  ef _execute_get_
+000158b0: 7365 7276 6572 5f73 6573 7369 6f6e 5f69  server_session_i
+000158c0: 6428 7365 6c66 2920 2d3e 204e 6f6e 653a  d(self) -> None:
+000158d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000158e0: 2e63 6f6e 6e65 6374 696f 6e2e 7365 7276  .connection.serv
+000158f0: 6572 5365 7373 696f 6e49 6420 6973 204e  erSessionId is N
+00015900: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00015910: 2072 6169 7365 2045 7272 6f72 2872 6561   raise Error(rea
+00015920: 736f 6e3d 6622 436f 6e6e 6563 7469 6f6e  son=f"Connection
+00015930: 207b 7365 6c66 2e63 6f6e 6e65 6374 696f   {self.connectio
+00015940: 6e7d 2066 6f72 2063 7572 736f 7220 7b73  n} for cursor {s
+00015950: 656c 667d 2068 6173 206e 6f20 7365 7276  elf} has no serv
+00015960: 6572 5365 7373 696f 6e49 6422 290a 2020  erSessionId").  
+00015970: 2020 2020 2020 7365 6c66 2e64 6573 6372        self.descr
+00015980: 6970 7469 6f6e 203d 205b 0a20 2020 2020  iption = [.     
+00015990: 2020 2020 2020 2028 2273 6572 7665 725f         ("server_
+000159a0: 7365 7373 696f 6e5f 6964 222c 2054 7970  session_id", Typ
+000159b0: 6543 6f64 6573 2e43 4841 522c 204e 6f6e  eCodes.CHAR, Non
+000159c0: 652c 204e 6f6e 652c 204e 6f6e 652c 204e  e, None, None, N
+000159d0: 6f6e 652c 204e 6f6e 6529 0a20 2020 2020  one, None).     
+000159e0: 2020 205d 2020 2320 6469 7370 6c61 795f     ]  # display_
+000159f0: 7369 7a65 2020 2320 696e 7465 726e 616c  size  # internal
+00015a00: 5f73 697a 6520 2023 2070 7265 6369 7369  _size  # precisi
+00015a10: 6f6e 2020 2320 7363 616c 6520 2023 206e  on  # scale  # n
+00015a20: 756c 6c5f 6f6b 0a20 2020 2020 2020 2052  ull_ok.        R
+00015a30: 6f77 203d 206e 616d 6564 7475 706c 6528  ow = namedtuple(
+00015a40: 2252 6f77 222c 2028 2273 6572 7665 725f  "Row", ("server_
+00015a50: 7365 7373 696f 6e5f 6964 222c 2929 0a20  session_id",)). 
+00015a60: 2020 2020 2020 2073 656c 662e 6c69 7374         self.list
+00015a70: 5f72 6573 756c 7420 3d20 5b52 6f77 2e5f  _result = [Row._
+00015a80: 6d61 6b65 2828 7365 6c66 2e63 6f6e 6e65  make((self.conne
+00015a90: 6374 696f 6e2e 7365 7276 6572 5365 7373  ction.serverSess
+00015aa0: 696f 6e49 642c 2929 5d0a 0a20 2020 2064  ionId,))]..    d
+00015ab0: 6566 205f 6578 6563 7574 655f 6765 7428  ef _execute_get(
+00015ac0: 7365 6c66 2c20 7061 7261 6d73 3a20 5365  self, params: Se
+00015ad0: 7175 656e 6365 5b73 7472 5d29 202d 3e20  quence[str]) -> 
+00015ae0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6966  None:.        if
+00015af0: 206c 656e 2870 6172 616d 7329 203d 3d20   len(params) == 
+00015b00: 3120 616e 6420 7061 7261 6d73 5b30 5d2e  1 and params[0].
+00015b10: 7570 7065 7228 2920 3d3d 2022 5343 4845  upper() == "SCHE
+00015b20: 4d41 223a 0a20 2020 2020 2020 2020 2020  MA":.           
+00015b30: 2073 656c 662e 5f65 7865 6375 7465 5f67   self._execute_g
+00015b40: 6574 5f73 6368 656d 6128 290a 2020 2020  et_schema().    
+00015b50: 2020 2020 656c 6966 2028 0a20 2020 2020      elif (.     
+00015b60: 2020 2020 2020 206c 656e 2870 6172 616d         len(param
+00015b70: 7329 203d 3d20 330a 2020 2020 2020 2020  s) == 3.        
+00015b80: 2020 2020 616e 6420 7061 7261 6d73 5b30      and params[0
+00015b90: 5d2e 7570 7065 7228 2920 3d3d 2022 5345  ].upper() == "SE
+00015ba0: 5256 4552 220a 2020 2020 2020 2020 2020  RVER".          
+00015bb0: 2020 616e 6420 7061 7261 6d73 5b31 5d2e    and params[1].
+00015bc0: 7570 7065 7228 2920 3d3d 2022 5345 5353  upper() == "SESS
+00015bd0: 494f 4e22 0a20 2020 2020 2020 2020 2020  ION".           
+00015be0: 2061 6e64 2070 6172 616d 735b 325d 2e75   and params[2].u
+00015bf0: 7070 6572 2829 203d 3d20 2249 4422 0a20  pper() == "ID". 
+00015c00: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+00015c10: 2020 2020 2020 7365 6c66 2e5f 6578 6563        self._exec
+00015c20: 7574 655f 6765 745f 7365 7276 6572 5f73  ute_get_server_s
+00015c30: 6573 7369 6f6e 5f69 6428 290a 2020 2020  ession_id().    
+00015c40: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00015c50: 2020 2020 2020 7261 6973 6520 5072 6f67        raise Prog
+00015c60: 7261 6d6d 696e 6745 7272 6f72 2872 6561  rammingError(rea
+00015c70: 736f 6e3d 2253 796e 7461 7820 6572 726f  son="Syntax erro
+00015c80: 7222 290a 0a20 2020 2064 6566 205f 6578  r")..    def _ex
+00015c90: 6563 7574 655f 636c 6561 7228 7365 6c66  ecute_clear(self
+00015ca0: 2c20 7061 7261 6d73 3a20 5365 7175 656e  , params: Sequen
+00015cb0: 6365 5b73 7472 5d29 202d 3e20 4e6f 6e65  ce[str]) -> None
+00015cc0: 3a0a 2020 2020 2020 2020 6966 206c 656e  :.        if len
+00015cd0: 2870 6172 616d 7329 2021 3d20 3120 6f72  (params) != 1 or
+00015ce0: 2070 6172 616d 735b 305d 2e75 7070 6572   params[0].upper
+00015cf0: 2829 2021 3d20 2243 4143 4845 223a 0a20  () != "CACHE":. 
+00015d00: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00015d10: 2050 726f 6772 616d 6d69 6e67 4572 726f   ProgrammingErro
+00015d20: 7228 7265 6173 6f6e 3d22 5379 6e74 6178  r(reason="Syntax
+00015d30: 2065 7272 6f72 2229 0a0a 2020 2020 2020   error")..      
+00015d40: 2020 2320 5468 6572 6520 6973 206e 6f20    # There is no 
+00015d50: 7265 7375 6c74 7365 7420 6461 7461 2066  resultset data f
+00015d60: 726f 6d20 616e 2075 7064 6174 650a 2020  rom an update.  
+00015d70: 2020 2020 2020 7365 6c66 2e65 6e64 5f6f        self.end_o
+00015d80: 665f 6461 7461 203d 2054 7275 650a 0a20  f_data = True.. 
+00015d90: 2020 2020 2020 2066 6163 746f 7279 203d         factory =
+00015da0: 205f 436c 6561 7243 6163 6865 4661 6374   _ClearCacheFact
+00015db0: 6f72 7928 290a 2020 2020 2020 2020 7265  ory().        re
+00015dc0: 7120 3d20 6661 6374 6f72 792e 7265 7175  q = factory.requ
+00015dd0: 6573 7428 290a 0a20 2020 2020 2020 205f  est()..        _
+00015de0: 7365 6e64 5f6d 7367 2873 656c 662e 636f  send_msg(self.co
+00015df0: 6e6e 6563 7469 6f6e 2c20 7265 7129 0a0a  nnection, req)..
+00015e00: 2020 2020 2020 2020 7273 7020 3d20 5f72          rsp = _r
+00015e10: 6563 765f 6d73 6728 7365 6c66 2e63 6f6e  ecv_msg(self.con
+00015e20: 6e65 6374 696f 6e2c 2066 6163 746f 7279  nection, factory
+00015e30: 2e72 6573 706f 6e73 6528 2929 0a0a 2020  .response())..  
+00015e40: 2020 2020 2020 6966 2072 7370 2e74 7970        if rsp.typ
+00015e50: 6520 3d3d 2070 726f 746f 2e43 6f6e 6669  e == proto.Confi
+00015e60: 726d 6174 696f 6e52 6573 706f 6e73 652e  rmationResponse.
+00015e70: 5245 5350 4f4e 5345 5f57 4152 4e3a 0a20  RESPONSE_WARN:. 
+00015e80: 2020 2020 2020 2020 2020 2077 6172 6e28             warn(
+00015e90: 7273 702e 7265 6173 6f6e 290a 2020 2020  rsp.reason).    
+00015ea0: 2020 2020 656c 6966 206e 6f74 2072 7370      elif not rsp
+00015eb0: 2e74 7970 6520 3d3d 2070 726f 746f 2e43  .type == proto.C
+00015ec0: 6f6e 6669 726d 6174 696f 6e52 6573 706f  onfirmationRespo
+00015ed0: 6e73 652e 5245 5350 4f4e 5345 5f4f 4b3a  nse.RESPONSE_OK:
+00015ee0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00015ef0: 7273 702e 7665 6e64 6f72 5f63 6f64 6520  rsp.vendor_code 
+00015f00: 3d3d 2053 4553 5349 4f4e 5f45 5850 4952  == SESSION_EXPIR
+00015f10: 4544 5f43 4f44 453a 0a20 2020 2020 2020  ED_CODE:.       
+00015f20: 2020 2020 2020 2020 2023 204e 6565 6420           # Need 
+00015f30: 746f 2072 6566 7265 7368 2074 6865 2073  to refresh the s
+00015f40: 6573 7369 6f6e 0a20 2020 2020 2020 2020  ession.         
+00015f50: 2020 2020 2020 2073 656c 662e 636f 6e6e         self.conn
+00015f60: 6563 7469 6f6e 2e72 6566 7265 7368 2829  ection.refresh()
+00015f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015f80: 2023 2061 6e64 2074 7279 2061 6761 696e   # and try again
+00015f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015fa0: 2073 656c 662e 5f65 7865 6375 7465 5f63   self._execute_c
+00015fb0: 6c65 6172 2870 6172 616d 7329 0a20 2020  lear(params).   
+00015fc0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00015fd0: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
+00015fe0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00015ff0: 2020 2020 2020 7261 6973 6520 5f63 6f6e        raise _con
+00016000: 7665 7274 5f65 7863 6570 7469 6f6e 2872  vert_exception(r
+00016010: 7370 290a 0a20 2020 2064 6566 205f 6578  sp)..    def _ex
+00016020: 6563 7574 655f 6361 6e63 656c 6b69 6c6c  ecute_cancelkill
+00016030: 2873 656c 662c 206f 703a 2073 7472 2c20  (self, op: str, 
+00016040: 6964 3a20 5365 7175 656e 6365 5b73 7472  id: Sequence[str
+00016050: 5d29 202d 3e20 4e6f 6e65 3a0a 2020 2020  ]) -> None:.    
+00016060: 2020 2020 6966 206c 656e 2869 6429 2021      if len(id) !
+00016070: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
+00016080: 2072 6169 7365 2050 726f 6772 616d 6d69   raise Programmi
+00016090: 6e67 4572 726f 7228 7265 6173 6f6e 3d22  ngError(reason="
+000160a0: 5379 6e74 6178 2065 7272 6f72 2229 0a0a  Syntax error")..
+000160b0: 2020 2020 2020 2020 2320 5468 6572 6520          # There 
+000160c0: 6973 206e 6f20 7265 7375 6c74 7365 7420  is no resultset 
+000160d0: 6461 7461 2066 726f 6d20 616e 2075 7064  data from an upd
+000160e0: 6174 650a 2020 2020 2020 2020 7365 6c66  ate.        self
+000160f0: 2e65 6e64 5f6f 665f 6461 7461 203d 2054  .end_of_data = T
+00016100: 7275 650a 0a20 2020 2020 2020 2066 6163  rue..        fac
+00016110: 746f 7279 203d 205f 4f43 4945 4e54 5f52  tory = _OCIENT_R
+00016120: 4551 5545 5354 5f46 4143 544f 5249 4553  EQUEST_FACTORIES
+00016130: 5b6f 705d 0a20 2020 2020 2020 2072 6571  [op].        req
+00016140: 203d 2066 6163 746f 7279 2e72 6571 7565   = factory.reque
+00016150: 7374 2869 645b 305d 290a 0a20 2020 2020  st(id[0])..     
+00016160: 2020 205f 7365 6e64 5f6d 7367 2873 656c     _send_msg(sel
+00016170: 662e 636f 6e6e 6563 7469 6f6e 2c20 7265  f.connection, re
+00016180: 7129 0a0a 2020 2020 2020 2020 7273 7020  q)..        rsp 
+00016190: 3d20 5f72 6563 765f 6d73 6728 7365 6c66  = _recv_msg(self
+000161a0: 2e63 6f6e 6e65 6374 696f 6e2c 2066 6163  .connection, fac
+000161b0: 746f 7279 2e72 6573 706f 6e73 6528 2929  tory.response())
+000161c0: 0a0a 2020 2020 2020 2020 6966 2072 7370  ..        if rsp
+000161d0: 2e72 6573 706f 6e73 652e 7479 7065 203d  .response.type =
+000161e0: 3d20 7072 6f74 6f2e 436f 6e66 6972 6d61  = proto.Confirma
+000161f0: 7469 6f6e 5265 7370 6f6e 7365 2e52 4553  tionResponse.RES
+00016200: 504f 4e53 455f 5741 524e 3a0a 2020 2020  PONSE_WARN:.    
+00016210: 2020 2020 2020 2020 7761 726e 2872 7370          warn(rsp
+00016220: 2e72 6573 706f 6e73 652e 7265 6173 6f6e  .response.reason
+00016230: 290a 2020 2020 2020 2020 656c 6966 206e  ).        elif n
+00016240: 6f74 2072 7370 2e72 6573 706f 6e73 652e  ot rsp.response.
+00016250: 7479 7065 203d 3d20 7072 6f74 6f2e 436f  type == proto.Co
+00016260: 6e66 6972 6d61 7469 6f6e 5265 7370 6f6e  nfirmationRespon
+00016270: 7365 2e52 4553 504f 4e53 455f 4f4b 3a0a  se.RESPONSE_OK:.
+00016280: 2020 2020 2020 2020 2020 2020 6966 2072              if r
+00016290: 7370 2e72 6573 706f 6e73 652e 7665 6e64  sp.response.vend
+000162a0: 6f72 5f63 6f64 6520 3d3d 2053 4553 5349  or_code == SESSI
+000162b0: 4f4e 5f45 5850 4952 4544 5f43 4f44 453a  ON_EXPIRED_CODE:
+000162c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000162d0: 2023 204e 6565 6420 746f 2072 6566 7265   # Need to refre
+000162e0: 7368 2074 6865 2073 6573 7369 6f6e 0a20  sh the session. 
+000162f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016300: 656c 662e 636f 6e6e 6563 7469 6f6e 2e72  elf.connection.r
+00016310: 6566 7265 7368 2829 0a20 2020 2020 2020  efresh().       
+00016320: 2020 2020 2020 2020 2023 2061 6e64 2074           # and t
+00016330: 7279 2061 6761 696e 0a20 2020 2020 2020  ry again.       
+00016340: 2020 2020 2020 2020 2073 656c 662e 5f65           self._e
+00016350: 7865 6375 7465 5f63 616e 6365 6c6b 696c  xecute_cancelkil
+00016360: 6c28 6f70 2c20 6964 290a 2020 2020 2020  l(op, id).      
+00016370: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00016380: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00016390: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000163a0: 2020 2072 6169 7365 205f 636f 6e76 6572     raise _conver
+000163b0: 745f 6578 6365 7074 696f 6e28 7273 702e  t_exception(rsp.
+000163c0: 7265 7370 6f6e 7365 290a 0a20 2020 2023  response)..    #
+000163d0: 2054 4f44 4f3a 2072 6570 6c61 6365 2074   TODO: replace t
+000163e0: 6865 206f 7468 6572 206d 6574 6164 6174  he other metadat
+000163f0: 6120 6361 6c6c 0a20 2020 2064 6566 205f  a call.    def _
+00016400: 6578 6563 7574 655f 7379 7374 656d 6d65  execute_systemme
+00016410: 7461 6461 7461 280a 2020 2020 2020 2020  tadata(.        
+00016420: 7365 6c66 2c0a 2020 2020 2020 2020 6f70  self,.        op
+00016430: 3a20 7072 6f74 6f2e 4665 7463 6853 7973  : proto.FetchSys
+00016440: 7465 6d4d 6574 6164 6174 612e 5379 7374  temMetadata.Syst
+00016450: 656d 4d65 7461 6461 7461 4361 6c6c 2c0a  emMetadataCall,.
+00016460: 2020 2020 2020 2020 7363 6865 6d61 3a20          schema: 
+00016470: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00016480: 4e6f 6e65 2c0a 2020 2020 2020 2020 7461  None,.        ta
+00016490: 626c 653a 204f 7074 696f 6e61 6c5b 7374  ble: Optional[st
+000164a0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+000164b0: 2020 2063 6f6c 756d 6e3a 204f 7074 696f     column: Optio
+000164c0: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+000164d0: 0a20 2020 2020 2020 2076 6965 773a 204f  .        view: O
+000164e0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+000164f0: 6f6e 652c 0a20 2020 2029 202d 3e20 556e  one,.    ) -> Un
+00016500: 696f 6e5b 696e 742c 2073 7472 2c20 4e6f  ion[int, str, No
+00016510: 6e65 5d3a 0a20 2020 2020 2020 2066 6163  ne]:.        fac
+00016520: 746f 7279 203d 205f 4765 7453 7973 7465  tory = _GetSyste
+00016530: 6d4d 6574 6164 6174 6146 6163 746f 7279  mMetadataFactory
+00016540: 2829 0a20 2020 2020 2020 2072 6571 203d  ().        req =
+00016550: 2066 6163 746f 7279 2e72 6571 7565 7374   factory.request
+00016560: 286f 702c 2073 6368 656d 612c 2074 6162  (op, schema, tab
+00016570: 6c65 2c20 636f 6c75 6d6e 2c20 7669 6577  le, column, view
+00016580: 290a 0a20 2020 2020 2020 205f 7365 6e64  )..        _send
+00016590: 5f6d 7367 2873 656c 662e 636f 6e6e 6563  _msg(self.connec
+000165a0: 7469 6f6e 2c20 7265 7129 0a0a 2020 2020  tion, req)..    
+000165b0: 2020 2020 7273 7020 3d20 5f72 6563 765f      rsp = _recv_
+000165c0: 6d73 6728 7365 6c66 2e63 6f6e 6e65 6374  msg(self.connect
+000165d0: 696f 6e2c 2066 6163 746f 7279 2e72 6573  ion, factory.res
+000165e0: 706f 6e73 6528 2929 0a0a 2020 2020 2020  ponse())..      
+000165f0: 2020 6966 2072 7370 2e72 6573 706f 6e73    if rsp.respons
+00016600: 652e 7479 7065 203d 3d20 7072 6f74 6f2e  e.type == proto.
+00016610: 436f 6e66 6972 6d61 7469 6f6e 5265 7370  ConfirmationResp
+00016620: 6f6e 7365 2e52 4553 504f 4e53 455f 5741  onse.RESPONSE_WA
+00016630: 524e 3a0a 2020 2020 2020 2020 2020 2020  RN:.            
+00016640: 7761 726e 2872 7370 2e72 6573 706f 6e73  warn(rsp.respons
+00016650: 652e 7265 6173 6f6e 290a 2020 2020 2020  e.reason).      
+00016660: 2020 656c 6966 206e 6f74 2072 7370 2e72    elif not rsp.r
+00016670: 6573 706f 6e73 652e 7479 7065 203d 3d20  esponse.type == 
+00016680: 7072 6f74 6f2e 436f 6e66 6972 6d61 7469  proto.Confirmati
+00016690: 6f6e 5265 7370 6f6e 7365 2e52 4553 504f  onResponse.RESPO
+000166a0: 4e53 455f 4f4b 3a0a 2020 2020 2020 2020  NSE_OK:.        
+000166b0: 2020 2020 6966 2072 7370 2e72 6573 706f      if rsp.respo
+000166c0: 6e73 652e 7665 6e64 6f72 5f63 6f64 6520  nse.vendor_code 
+000166d0: 3d3d 2053 4553 5349 4f4e 5f45 5850 4952  == SESSION_EXPIR
+000166e0: 4544 5f43 4f44 453a 0a20 2020 2020 2020  ED_CODE:.       
+000166f0: 2020 2020 2020 2020 2023 204e 6565 6420           # Need 
+00016700: 746f 2072 6566 7265 7368 2074 6865 2073  to refresh the s
+00016710: 6573 7369 6f6e 0a20 2020 2020 2020 2020  ession.         
+00016720: 2020 2020 2020 2073 656c 662e 636f 6e6e         self.conn
+00016730: 6563 7469 6f6e 2e72 6566 7265 7368 2829  ection.refresh()
+00016740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016750: 2023 2061 6e64 2074 7279 2061 6761 696e   # and try again
+00016760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016770: 2072 6574 7572 6e20 7365 6c66 2e5f 6578   return self._ex
+00016780: 6563 7574 655f 7379 7374 656d 6d65 7461  ecute_systemmeta
+00016790: 6461 7461 286f 702c 2073 6368 656d 613d  data(op, schema=
+000167a0: 7363 6865 6d61 2c20 7461 626c 653d 7461  schema, table=ta
+000167b0: 626c 652c 2063 6f6c 756d 6e3d 636f 6c75  ble, column=colu
+000167c0: 6d6e 2c20 7669 6577 3d76 6965 7729 0a20  mn, view=view). 
+000167d0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000167e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000167f0: 2072 6169 7365 205f 636f 6e76 6572 745f   raise _convert_
+00016800: 6578 6365 7074 696f 6e28 7273 702e 7265  exception(rsp.re
+00016810: 7370 6f6e 7365 290a 0a20 2020 2020 2020  sponse)..       
+00016820: 2069 6620 7273 702e 4861 7346 6965 6c64   if rsp.HasField
+00016830: 2822 7265 7375 6c74 5f73 6574 5f76 616c  ("result_set_val
+00016840: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+00016850: 7365 6c66 2e5f 6765 745f 7265 7375 6c74  self._get_result
+00016860: 5f6d 6574 6164 6174 6128 290a 0a20 2020  _metadata()..   
+00016870: 2020 2020 2020 2020 2066 6f72 2062 6c6f           for blo
+00016880: 6220 696e 2072 7370 2e72 6573 756c 745f  b in rsp.result_
+00016890: 7365 745f 7661 6c2e 626c 6f62 733a 0a20  set_val.blobs:. 
+000168a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000168b0: 656c 662e 5f62 7566 6665 7273 2e61 7070  elf._buffers.app
+000168c0: 656e 6428 626c 6f62 290a 2020 2020 2020  end(blob).      
+000168d0: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+000168e0: 650a 0a20 2020 2020 2020 2069 6620 7273  e..        if rs
+000168f0: 702e 4861 7346 6965 6c64 2822 7374 7269  p.HasField("stri
+00016900: 6e67 5f76 616c 2229 3a0a 2020 2020 2020  ng_val"):.      
+00016910: 2020 2020 2020 7265 7475 726e 2072 7370        return rsp
+00016920: 2e73 7472 696e 675f 7661 6c0a 0a20 2020  .string_val..   
+00016930: 2020 2020 2072 6574 7572 6e20 7273 702e       return rsp.
+00016940: 696e 745f 7661 6c0a 0a20 2020 2064 6566  int_val..    def
+00016950: 205f 6765 745f 6d6f 7265 5f64 6174 6128   _get_more_data(
+00016960: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+00016970: 2020 2020 2020 2022 2222 496e 7465 726e         """Intern
+00016980: 616c 2072 6f75 7469 6e65 2074 6f20 6765  al routine to ge
+00016990: 7420 6d6f 7265 2064 6174 6120 6672 6f6d  t more data from
+000169a0: 2061 2071 7565 7279 2222 220a 2020 2020   a query""".    
+000169b0: 2020 2020 2320 7079 6c69 6e74 3a20 6469      # pylint: di
+000169c0: 7361 626c 653d 6e6f 2d6d 656d 6265 720a  sable=no-member.
+000169d0: 2020 2020 2020 2020 7265 7120 3d20 7072          req = pr
+000169e0: 6f74 6f2e 5265 7175 6573 7428 290a 2020  oto.Request().  
+000169f0: 2020 2020 2020 7265 712e 7479 7065 203d        req.type =
+00016a00: 2072 6571 2e46 4554 4348 5f44 4154 410a   req.FETCH_DATA.
+00016a10: 2020 2020 2020 2020 7265 712e 6665 7463          req.fetc
+00016a20: 685f 6461 7461 2e66 6574 6368 5f73 697a  h_data.fetch_siz
+00016a30: 6520 3d20 7365 6c66 2e61 7272 6179 7369  e = self.arraysi
+00016a40: 7a65 0a20 2020 2020 2020 205f 7365 6e64  ze.        _send
+00016a50: 5f6d 7367 2873 656c 662e 636f 6e6e 6563  _msg(self.connec
+00016a60: 7469 6f6e 2c20 7265 7129 0a0a 2020 2020  tion, req)..    
+00016a70: 2020 2020 7273 7020 3d20 5f72 6563 765f      rsp = _recv_
+00016a80: 6d73 6728 7365 6c66 2e63 6f6e 6e65 6374  msg(self.connect
+00016a90: 696f 6e2c 2070 726f 746f 2e46 6574 6368  ion, proto.Fetch
+00016aa0: 4461 7461 5265 7370 6f6e 7365 2829 290a  DataResponse()).
+00016ab0: 0a20 2020 2020 2020 2069 6620 7273 702e  .        if rsp.
+00016ac0: 7265 7370 6f6e 7365 2e74 7970 6520 3d3d  response.type ==
+00016ad0: 2070 726f 746f 2e43 6f6e 6669 726d 6174   proto.Confirmat
+00016ae0: 696f 6e52 6573 706f 6e73 652e 5245 5350  ionResponse.RESP
+00016af0: 4f4e 5345 5f45 5252 4f52 3a0a 2020 2020  ONSE_ERROR:.    
+00016b00: 2020 2020 2020 2020 7261 6973 6520 5f63          raise _c
+00016b10: 6f6e 7665 7274 5f65 7863 6570 7469 6f6e  onvert_exception
+00016b20: 2872 7370 2e72 6573 706f 6e73 6529 0a0a  (rsp.response)..
+00016b30: 2020 2020 2020 2020 666f 7220 626c 6f62          for blob
+00016b40: 2069 6e20 7273 702e 7265 7375 6c74 5f73   in rsp.result_s
+00016b50: 6574 2e62 6c6f 6273 3a0a 2020 2020 2020  et.blobs:.      
+00016b60: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
+00016b70: 662e 5f62 7566 6665 7273 3a0a 2020 2020  f._buffers:.    
+00016b80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016b90: 2e5f 6f66 6673 6574 203d 2030 0a20 2020  ._offset = 0.   
+00016ba0: 2020 2020 2020 2020 2073 656c 662e 5f62           self._b
+00016bb0: 7566 6665 7273 2e61 7070 656e 6428 626c  uffers.append(bl
+00016bc0: 6f62 290a 0a20 2020 2064 6566 2066 6574  ob)..    def fet
+00016bd0: 6368 6d61 6e79 2873 656c 662c 2073 697a  chmany(self, siz
+00016be0: 653a 204f 7074 696f 6e61 6c5b 696e 745d  e: Optional[int]
+00016bf0: 203d 204e 6f6e 6529 202d 3e20 4c69 7374   = None) -> List
+00016c00: 5b4e 616d 6564 5475 706c 655d 3a0a 2020  [NamedTuple]:.  
+00016c10: 2020 2020 2020 2222 2246 6574 6368 2074        """Fetch t
+00016c20: 6865 206e 6578 7420 7365 7420 6f66 2072  he next set of r
+00016c30: 6f77 7320 6f66 2061 2071 7565 7279 2072  ows of a query r
+00016c40: 6573 756c 742c 2072 6574 7572 6e69 6e67  esult, returning
+00016c50: 2061 2073 6571 7565 6e63 6520 6f66 0a20   a sequence of. 
+00016c60: 2020 2020 2020 2073 6571 7565 6e63 6573         sequences
+00016c70: 2028 652e 672e 2061 206c 6973 7420 6f66   (e.g. a list of
+00016c80: 2074 7570 6c65 7329 2e20 416e 2065 6d70   tuples). An emp
+00016c90: 7479 2073 6571 7565 6e63 6520 6973 2072  ty sequence is r
+00016ca0: 6574 7572 6e65 6420 7768 656e 206e 6f0a  eturned when no.
+00016cb0: 2020 2020 2020 2020 6d6f 7265 2072 6f77          more row
+00016cc0: 7320 6172 6520 6176 6169 6c61 626c 652e  s are available.
+00016cd0: 0a0a 2020 2020 2020 2020 5468 6520 6e75  ..        The nu
+00016ce0: 6d62 6572 206f 6620 726f 7773 2074 6f20  mber of rows to 
+00016cf0: 6665 7463 6820 7065 7220 6361 6c6c 2069  fetch per call i
+00016d00: 7320 7370 6563 6966 6965 6420 6279 2074  s specified by t
+00016d10: 6865 2070 6172 616d 6574 6572 2e20 4966  he parameter. If
+00016d20: 2069 740a 2020 2020 2020 2020 6973 206e   it.        is n
+00016d30: 6f74 2067 6976 656e 2c20 7468 6520 6375  ot given, the cu
+00016d40: 7273 6f72 2773 2061 7272 6179 7369 7a65  rsor's arraysize
+00016d50: 2064 6574 6572 6d69 6e65 7320 7468 6520   determines the 
+00016d60: 6e75 6d62 6572 206f 6620 726f 7773 2074  number of rows t
+00016d70: 6f20 6265 0a20 2020 2020 2020 2066 6574  o be.        fet
+00016d80: 6368 6564 2e20 5468 6520 6d65 7468 6f64  ched. The method
+00016d90: 2077 696c 6c20 7472 7920 746f 2066 6574   will try to fet
+00016da0: 6368 2061 7320 6d61 6e79 2072 6f77 7320  ch as many rows 
+00016db0: 6173 2069 6e64 6963 6174 6564 2062 7920  as indicated by 
+00016dc0: 7468 6520 7369 7a65 0a20 2020 2020 2020  the size.       
+00016dd0: 2070 6172 616d 6574 6572 2e20 4966 2074   parameter. If t
+00016de0: 6869 7320 6973 206e 6f74 2070 6f73 7369  his is not possi
+00016df0: 626c 6520 6475 6520 746f 2074 6865 2073  ble due to the s
+00016e00: 7065 6369 6669 6564 206e 756d 6265 7220  pecified number 
+00016e10: 6f66 2072 6f77 7320 6e6f 740a 2020 2020  of rows not.    
+00016e20: 2020 2020 6265 696e 6720 6176 6169 6c61      being availa
+00016e30: 626c 652c 2066 6577 6572 2072 6f77 7320  ble, fewer rows 
+00016e40: 6d61 7920 6265 2072 6574 7572 6e65 642e  may be returned.
+00016e50: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00016e60: 2020 2020 2069 6620 7369 7a65 2069 7320       if size is 
+00016e70: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00016e80: 2020 7369 7a65 203d 2073 656c 662e 6172    size = self.ar
+00016e90: 7261 7973 697a 650a 0a20 2020 2020 2020  raysize..       
+00016ea0: 2072 6f77 733a 204c 6973 745b 4e61 6d65   rows: List[Name
+00016eb0: 6454 7570 6c65 5d20 3d20 5b5d 0a20 2020  dTuple] = [].   
+00016ec0: 2020 2020 2077 6869 6c65 2073 697a 6520       while size 
+00016ed0: 3e20 303a 0a20 2020 2020 2020 2020 2020  > 0:.           
+00016ee0: 2061 5f72 6f77 203d 2073 656c 662e 6665   a_row = self.fe
+00016ef0: 7463 686f 6e65 2829 0a20 2020 2020 2020  tchone().       
+00016f00: 2020 2020 2069 6620 615f 726f 7720 6973       if a_row is
+00016f10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00016f20: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
+00016f30: 2020 2020 2020 2020 2072 6f77 732e 6170           rows.ap
+00016f40: 7065 6e64 2861 5f72 6f77 290a 2020 2020  pend(a_row).    
+00016f50: 2020 2020 2020 2020 7369 7a65 202d 3d20          size -= 
+00016f60: 310a 2020 2020 2020 2020 7265 7475 726e  1.        return
+00016f70: 2072 6f77 730a 0a20 2020 2064 6566 2066   rows..    def f
+00016f80: 6574 6368 616c 6c28 7365 6c66 2920 2d3e  etchall(self) ->
+00016f90: 204c 6973 745b 4e61 6d65 6454 7570 6c65   List[NamedTuple
+00016fa0: 5d3a 0a20 2020 2020 2020 2022 2222 4665  ]:.        """Fe
+00016fb0: 7463 6820 616c 6c20 2872 656d 6169 6e69  tch all (remaini
+00016fc0: 6e67 2920 726f 7773 206f 6620 6120 7175  ng) rows of a qu
+00016fd0: 6572 7920 7265 7375 6c74 2c20 7265 7475  ery result, retu
+00016fe0: 726e 696e 6720 7468 656d 2061 7320 610a  rning them as a.
+00016ff0: 2020 2020 2020 2020 7365 7175 656e 6365          sequence
+00017000: 206f 6620 7365 7175 656e 6365 7320 2865   of sequences (e
+00017010: 2e67 2e20 6120 6c69 7374 206f 6620 7475  .g. a list of tu
+00017020: 706c 6573 292e 204e 6f74 6520 7468 6174  ples). Note that
+00017030: 2074 6865 2063 7572 736f 7227 730a 2020   the cursor's.  
+00017040: 2020 2020 2020 6172 7261 7973 697a 6520        arraysize 
+00017050: 6174 7472 6962 7574 6520 6361 6e20 6166  attribute can af
+00017060: 6665 6374 2074 6865 2070 6572 666f 726d  fect the perform
+00017070: 616e 6365 206f 6620 7468 6973 206f 7065  ance of this ope
+00017080: 7261 7469 6f6e 2e0a 2020 2020 2020 2020  ration..        
+00017090: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+000170a0: 726e 2073 656c 662e 6665 7463 686d 616e  rn self.fetchman
+000170b0: 7928 7369 7a65 3d73 7973 2e6d 6178 7369  y(size=sys.maxsi
+000170c0: 7a65 290a 0a20 2020 2064 6566 205f 5f6e  ze)..    def __n
+000170d0: 6578 745f 5f28 7365 6c66 2920 2d3e 204e  ext__(self) -> N
+000170e0: 616d 6564 5475 706c 653a 0a20 2020 2020  amedTuple:.     
+000170f0: 2020 2061 5f72 6f77 203d 2073 656c 662e     a_row = self.
+00017100: 6665 7463 686f 6e65 2829 0a20 2020 2020  fetchone().     
+00017110: 2020 2069 6620 615f 726f 7720 6973 204e     if a_row is N
+00017120: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00017130: 2072 6169 7365 2053 746f 7049 7465 7261   raise StopItera
+00017140: 7469 6f6e 0a20 2020 2020 2020 2072 6574  tion.        ret
+00017150: 7572 6e20 615f 726f 770a 0a20 2020 2064  urn a_row..    d
+00017160: 6566 205f 5f69 7465 725f 5f28 7365 6c66  ef __iter__(self
+00017170: 2920 2d3e 2022 4375 7273 6f72 223a 0a20  ) -> "Cursor":. 
+00017180: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00017190: 6c66 0a0a 2020 2020 6465 6620 6665 7463  lf..    def fetc
+000171a0: 6876 616c 2873 656c 6629 202d 3e20 4f70  hval(self) -> Op
+000171b0: 7469 6f6e 616c 5b6f 626a 6563 745d 3a0a  tional[object]:.
+000171c0: 2020 2020 2020 2020 2222 2254 6865 2066          """The f
+000171d0: 6574 6368 7661 6c28 2920 636f 6e76 656e  etchval() conven
+000171e0: 6965 6e63 6520 6d65 7468 6f64 2072 6574  ience method ret
+000171f0: 7572 6e73 2074 6865 2066 6972 7374 2063  urns the first c
+00017200: 6f6c 756d 6e20 6f66 2074 6865 0a20 2020  olumn of the.   
+00017210: 2020 2020 2066 6972 7374 2072 6f77 2069       first row i
+00017220: 6620 7468 6572 6520 6172 6520 7265 7375  f there are resu
+00017230: 6c74 732c 206f 7468 6572 7769 7365 2069  lts, otherwise i
+00017240: 7420 7265 7475 726e 7320 4e6f 6e65 2e0a  t returns None..
+00017250: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00017260: 2020 2020 6172 6f77 203d 2073 656c 662e      arow = self.
+00017270: 6665 7463 686f 6e65 2829 0a20 2020 2020  fetchone().     
+00017280: 2020 2069 6620 6172 6f77 3a0a 2020 2020     if arow:.    
+00017290: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+000172a0: 6173 7428 6f62 6a65 6374 2c20 6172 6f77  ast(object, arow
+000172b0: 5b30 5d29 0a20 2020 2020 2020 2072 6574  [0]).        ret
+000172c0: 7572 6e20 4e6f 6e65 0a0a 2020 2020 6465  urn None..    de
+000172d0: 6620 6665 7463 686f 6e65 2873 656c 6629  f fetchone(self)
+000172e0: 202d 3e20 4f70 7469 6f6e 616c 5b4e 616d   -> Optional[Nam
+000172f0: 6564 5475 706c 655d 3a0a 2020 2020 2020  edTuple]:.      
+00017300: 2020 2222 2246 6574 6368 2074 6865 206e    """Fetch the n
+00017310: 6578 7420 726f 7720 6f66 2061 2071 7565  ext row of a que
+00017320: 7279 2072 6573 756c 7420 7365 742c 2072  ry result set, r
+00017330: 6574 7572 6e69 6e67 2061 2073 696e 676c  eturning a singl
+00017340: 6520 7365 7175 656e 6365 2c0a 2020 2020  e sequence,.    
+00017350: 2020 2020 6f72 204e 6f6e 6520 7768 656e      or None when
+00017360: 206e 6f20 6d6f 7265 2064 6174 6120 6973   no more data is
+00017370: 2061 7661 696c 6162 6c65 2e0a 2020 2020   available..    
+00017380: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00017390: 2320 4966 2074 6865 7265 2077 6173 206e  # If there was n
+000173a0: 6576 6572 2061 2071 7565 7279 2065 7865  ever a query exe
+000173b0: 6375 7465 642c 2074 6872 6f77 2061 6e20  cuted, throw an 
+000173c0: 6572 726f 720a 2020 2020 2020 2020 6966  error.        if
+000173d0: 2073 656c 662e 6465 7363 7269 7074 696f   self.descriptio
+000173e0: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
+000173f0: 2020 2020 2020 2072 6169 7365 2050 726f         raise Pro
+00017400: 6772 616d 6d69 6e67 4572 726f 7228 224e  grammingError("N
+00017410: 6f20 7265 7375 6c74 2073 6574 2061 7661  o result set ava
+00017420: 696c 6162 6c65 2229 0a0a 2020 2020 2020  ilable")..      
+00017430: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
+00017440: 626c 6520 3d20 746f 6f2d 6d61 6e79 2d62  ble = too-many-b
+00017450: 7261 6e63 6865 730a 2020 2020 2020 2020  ranches.        
+00017460: 6966 2073 656c 662e 656e 645f 6f66 5f64  if self.end_of_d
+00017470: 6174 613a 0a20 2020 2020 2020 2020 2020  ata:.           
+00017480: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
+00017490: 2020 2020 2020 2320 7370 6563 6961 6c20        # special 
+000174a0: 6361 7365 2065 7870 6c61 696e 2e0a 2020  case explain..  
+000174b0: 2020 2020 2020 6966 2073 656c 662e 6765        if self.ge
+000174c0: 6e65 7261 7465 645f 7265 7375 6c74 2069  nerated_result i
+000174d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000174e0: 2020 2020 2020 2020 7365 6c66 2e65 6e64          self.end
+000174f0: 5f6f 665f 6461 7461 203d 2054 7275 650a  _of_data = True.
+00017500: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+00017510: 7274 2073 656c 662e 7265 7375 6c74 7365  rt self.resultse
+00017520: 745f 7475 706c 6520 6973 206e 6f74 204e  t_tuple is not N
+00017530: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+00017540: 7265 7475 726e 2073 656c 662e 7265 7375  return self.resu
+00017550: 6c74 7365 745f 7475 706c 652e 5f6d 616b  ltset_tuple._mak
+00017560: 6528 2873 656c 662e 6765 6e65 7261 7465  e((self.generate
+00017570: 645f 7265 7375 6c74 2c29 290a 0a20 2020  d_result,))..   
+00017580: 2020 2020 2069 6620 7365 6c66 2e6c 6973       if self.lis
+00017590: 745f 7265 7375 6c74 2069 7320 6e6f 7420  t_result is not 
+000175a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000175b0: 2020 6966 2073 656c 662e 5f6f 6666 7365    if self._offse
+000175c0: 7420 3e3d 206c 656e 2873 656c 662e 6c69  t >= len(self.li
+000175d0: 7374 5f72 6573 756c 7429 3a0a 2020 2020  st_result):.    
+000175e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000175f0: 2e65 6e64 5f6f 665f 6461 7461 203d 2054  .end_of_data = T
+00017600: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
+00017610: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+00017620: 2020 2020 2020 2020 2020 2020 615f 726f              a_ro
+00017630: 7720 3d20 7365 6c66 2e6c 6973 745f 7265  w = self.list_re
+00017640: 7375 6c74 5b73 656c 662e 5f6f 6666 7365  sult[self._offse
+00017650: 745d 0a20 2020 2020 2020 2020 2020 2073  t].            s
+00017660: 656c 662e 5f6f 6666 7365 7420 2b3d 2031  elf._offset += 1
+00017670: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00017680: 7572 6e20 615f 726f 770a 0a20 2020 2020  urn a_row..     
+00017690: 2020 2069 6620 7365 6c66 2e72 6f77 636f     if self.rowco
+000176a0: 756e 7420 3c20 303a 0a20 2020 2020 2020  unt < 0:.       
+000176b0: 2020 2020 2073 656c 662e 726f 7763 6f75       self.rowcou
+000176c0: 6e74 203d 2030 0a0a 2020 2020 2020 2020  nt = 0..        
+000176d0: 7768 696c 6520 6e6f 7420 7365 6c66 2e5f  while not self._
+000176e0: 6275 6666 6572 733a 0a20 2020 2020 2020  buffers:.       
+000176f0: 2020 2020 2073 656c 662e 5f67 6574 5f6d       self._get_m
+00017700: 6f72 655f 6461 7461 2829 0a20 2020 2020  ore_data().     
+00017710: 2020 2020 2020 2077 6869 6c65 2073 656c         while sel
+00017720: 662e 5f62 7566 6665 7273 2061 6e64 2073  f._buffers and s
+00017730: 656c 662e 5f62 7566 2829 203d 3d20 6222  elf._buf() == b"
+00017740: 5c30 5c30 5c30 5c30 223a 0a20 2020 2020  \0\0\0\0":.     
+00017750: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017760: 5f62 7566 6665 7273 2e70 6f70 2830 290a  _buffers.pop(0).
+00017770: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00017780: 6e6f 7420 7365 6c66 2e5f 6275 6666 6572  not self._buffer
+00017790: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+000177a0: 2020 2023 206e 6f20 6461 7461 2079 6574     # no data yet
+000177b0: 2e2e 2e77 6169 7420 736f 2077 6520 646f  ...wait so we do
+000177c0: 6e27 7420 6861 6d6d 6572 2074 6865 2068  n't hammer the h
+000177d0: 6f73 7420 6265 666f 7265 2061 736b 696e  ost before askin
+000177e0: 6720 666f 7220 6d6f 7265 0a20 2020 2020  g for more.     
+000177f0: 2020 2020 2020 2020 2020 2073 6c65 6570             sleep
+00017800: 2830 2e32 3529 0a0a 2020 2020 2020 2020  (0.25)..        
+00017810: 6966 2073 656c 662e 5f6f 6666 7365 7420  if self._offset 
+00017820: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
+00017830: 2020 7365 6c66 2e5f 6765 745f 6e75 6d5f    self._get_num_
+00017840: 726f 7773 2829 0a0a 2020 2020 2020 2020  rows()..        
+00017850: 726f 775f 6c65 6e67 7468 203d 2073 656c  row_length = sel
+00017860: 662e 5f67 6574 5f69 6e74 2829 202d 2034  f._get_int() - 4
+00017870: 2020 2320 726f 775f 6c65 6e67 7468 2069    # row_length i
+00017880: 6e63 6c75 6465 7320 7468 6520 3420 6279  ncludes the 4 by
+00017890: 7465 7320 7765 206a 7573 7420 636f 6e73  tes we just cons
+000178a0: 756d 6564 0a20 2020 2020 2020 2065 6e64  umed.        end
+000178b0: 5f6f 6666 7365 7420 3d20 7365 6c66 2e5f  _offset = self._
+000178c0: 6f66 6673 6574 202b 2072 6f77 5f6c 656e  offset + row_len
+000178d0: 6774 680a 0a20 2020 2020 2020 2069 6620  gth..        if 
+000178e0: 7365 6c66 2e5f 6279 7465 735f 7265 6d61  self._bytes_rema
+000178f0: 696e 696e 6728 2920 3d3d 2031 2061 6e64  ining() == 1 and
+00017900: 2073 656c 662e 5f62 7566 2829 5b73 656c   self._buf()[sel
+00017910: 662e 5f6f 6666 7365 745d 203d 3d20 5479  f._offset] == Ty
+00017920: 7065 436f 6465 732e 4445 4d3a 0a20 2020  peCodes.DEM:.   
+00017930: 2020 2020 2020 2020 2073 656c 662e 726f           self.ro
+00017940: 7763 6f75 6e74 202d 3d20 310a 2020 2020  wcount -= 1.    
+00017950: 2020 2020 2020 2020 7365 6c66 2e5f 6275          self._bu
+00017960: 6666 6572 732e 706f 7028 3029 0a20 2020  ffers.pop(0).   
+00017970: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+00017980: 6c6f 7365 5f72 6573 756c 7473 6574 2829  lose_resultset()
+00017990: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000179a0: 7572 6e20 7365 6c66 2e5f 7072 6f63 6573  urn self._proces
+000179b0: 735f 7065 6e64 696e 6728 290a 0a20 2020  s_pending()..   
+000179c0: 2020 2020 2074 6d70 5f72 6f77 3a20 4c69       tmp_row: Li
+000179d0: 7374 5b6f 626a 6563 745d 203d 205b 5d0a  st[object] = [].
+000179e0: 2020 2020 2020 2020 7768 696c 6520 7365          while se
+000179f0: 6c66 2e5f 6f66 6673 6574 203c 2065 6e64  lf._offset < end
+00017a00: 5f6f 6666 7365 743a 0a20 2020 2020 2020  _offset:.       
+00017a10: 2020 2020 2074 6d70 5f72 6f77 2e61 7070       tmp_row.app
+00017a20: 656e 6428 7365 6c66 2e5f 6465 636f 6465  end(self._decode
+00017a30: 5f65 6e74 7279 2829 290a 0a20 2020 2020  _entry())..     
+00017a40: 2020 2069 6620 7365 6c66 2e5f 6f66 6673     if self._offs
+00017a50: 6574 203e 3d20 6c65 6e28 7365 6c66 2e5f  et >= len(self._
+00017a60: 6275 6628 2929 3a0a 2020 2020 2020 2020  buf()):.        
+00017a70: 2020 2020 7365 6c66 2e5f 6275 6666 6572      self._buffer
+00017a80: 732e 706f 7028 3029 0a20 2020 2020 2020  s.pop(0).       
+00017a90: 2020 2020 2073 656c 662e 5f6f 6666 7365       self._offse
+00017aa0: 7420 3d20 300a 2020 2020 2020 2020 6173  t = 0.        as
+00017ab0: 7365 7274 2073 656c 662e 726f 776e 756d  sert self.rownum
+00017ac0: 6265 7220 6973 206e 6f74 204e 6f6e 650a  ber is not None.
+00017ad0: 2020 2020 2020 2020 7365 6c66 2e72 6f77          self.row
+00017ae0: 6e75 6d62 6572 202b 3d20 310a 2020 2020  number += 1.    
+00017af0: 2020 2020 6173 7365 7274 2073 656c 662e      assert self.
+00017b00: 7265 7375 6c74 7365 745f 7475 706c 6520  resultset_tuple 
+00017b10: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
+00017b20: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00017b30: 7265 7375 6c74 7365 745f 7475 706c 652e  resultset_tuple.
+00017b40: 5f6d 616b 6528 746d 705f 726f 7729 0a0a  _make(tmp_row)..
+00017b50: 2020 2020 6465 6620 5f70 726f 6365 7373      def _process
+00017b60: 5f70 656e 6469 6e67 2873 656c 6629 202d  _pending(self) -
+00017b70: 3e20 4f70 7469 6f6e 616c 5b4e 616d 6564  > Optional[Named
+00017b80: 5475 706c 655d 3a0a 2020 2020 2020 2020  Tuple]:.        
+00017b90: 2320 6966 2077 6520 6861 7665 2061 6e79  # if we have any
+00017ba0: 2070 656e 6469 6e67 2071 7565 7269 6573   pending queries
+00017bb0: 2074 6f20 6578 6563 7574 652c 206b 6963   to execute, kic
+00017bc0: 6b20 6f6e 6520 6f66 6620 6e6f 770a 2020  k one off now.  
+00017bd0: 2020 2020 2020 6966 2073 656c 662e 5f70        if self._p
+00017be0: 656e 6469 6e67 5f6f 7073 3a0a 2020 2020  ending_ops:.    
+00017bf0: 2020 2020 2020 2020 7365 6c66 2e5f 6275          self._bu
+00017c00: 6666 6572 7320 3d20 5b5d 0a20 2020 2020  ffers = [].     
+00017c10: 2020 2020 2020 2073 656c 662e 5f6f 6666         self._off
+00017c20: 7365 7420 3d20 300a 2020 2020 2020 2020  set = 0.        
+00017c30: 2020 2020 7365 6c66 2e5f 6578 6563 7574      self._execut
+00017c40: 655f 696e 7465 726e 616c 2873 656c 662e  e_internal(self.
+00017c50: 5f70 656e 6469 6e67 5f6f 7073 2e70 6f70  _pending_ops.pop
+00017c60: 2830 2929 0a20 2020 2020 2020 2020 2020  (0)).           
+00017c70: 2072 6574 7572 6e20 7365 6c66 2e66 6574   return self.fet
+00017c80: 6368 6f6e 6528 290a 0a20 2020 2020 2020  chone()..       
+00017c90: 2073 656c 662e 656e 645f 6f66 5f64 6174   self.end_of_dat
+00017ca0: 6120 3d20 5472 7565 0a20 2020 2020 2020  a = True.       
+00017cb0: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
+00017cc0: 2020 6465 6620 5f62 7566 2873 656c 6629    def _buf(self)
+00017cd0: 202d 3e20 6279 7465 733a 0a20 2020 2020   -> bytes:.     
+00017ce0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00017cf0: 6275 6666 6572 735b 305d 0a0a 2020 2020  buffers[0]..    
+00017d00: 6465 6620 5f62 7974 6573 5f72 656d 6169  def _bytes_remai
+00017d10: 6e69 6e67 2873 656c 6629 202d 3e20 696e  ning(self) -> in
+00017d20: 743a 0a20 2020 2020 2020 2069 6620 6e6f  t:.        if no
+00017d30: 7420 7365 6c66 2e5f 6275 6666 6572 733a  t self._buffers:
+00017d40: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00017d50: 7572 6e20 300a 2020 2020 2020 2020 7265  urn 0.        re
+00017d60: 7475 726e 206c 656e 2873 656c 662e 5f62  turn len(self._b
+00017d70: 7566 6665 7273 5b30 5d29 202d 2073 656c  uffers[0]) - sel
+00017d80: 662e 5f6f 6666 7365 740a 0a20 2020 2064  f._offset..    d
+00017d90: 6566 205f 6765 745f 6e75 6d5f 726f 7773  ef _get_num_rows
+00017da0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+00017db0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00017dc0: 5f62 7974 6573 5f72 656d 6169 6e69 6e67  _bytes_remaining
+00017dd0: 2829 203e 3d20 343a 0a20 2020 2020 2020  () >= 4:.       
+00017de0: 2020 2020 2073 656c 662e 726f 7763 6f75       self.rowcou
+00017df0: 6e74 202b 3d20 7365 6c66 2e5f 6765 745f  nt += self._get_
+00017e00: 696e 7428 290a 0a20 2020 2064 6566 205f  int()..    def _
+00017e10: 6465 636f 6465 5f65 6e74 7279 2873 656c  decode_entry(sel
+00017e20: 6629 202d 3e20 6f62 6a65 6374 3a0a 2020  f) -> object:.  
+00017e30: 2020 2020 2020 2320 7079 6c69 6e74 3a20        # pylint: 
+00017e40: 6469 7361 626c 653d 746f 6f2d 6d61 6e79  disable=too-many
+00017e50: 2d6c 6f63 616c 732c 746f 6f2d 6d61 6e79  -locals,too-many
+00017e60: 2d72 6574 7572 6e2d 7374 6174 656d 656e  -return-statemen
+00017e70: 7473 2c74 6f6f 2d6d 616e 792d 6272 616e  ts,too-many-bran
+00017e80: 6368 6573 2c74 6f6f 2d6d 616e 792d 7374  ches,too-many-st
+00017e90: 6174 656d 656e 7473 0a20 2020 2020 2020  atements.       
+00017ea0: 2063 6f6c 7479 7065 203d 2073 656c 662e   coltype = self.
+00017eb0: 5f67 6574 5f62 7974 6528 290a 0a20 2020  _get_byte()..   
+00017ec0: 2020 2020 2023 2069 6620 7468 6973 2069       # if this i
+00017ed0: 7320 7468 6520 6561 7379 2063 6f6e 7665  s the easy conve
+00017ee0: 7273 696f 6e2c 206a 7573 7420 646f 2069  rsion, just do i
+00017ef0: 740a 2020 2020 2020 2020 6966 2063 6f6c  t.        if col
+00017f00: 7479 7065 2069 6e20 5f74 7970 655f 6d61  type in _type_ma
+00017f10: 703a 0a20 2020 2020 2020 2020 2020 2074  p:.            t
+00017f20: 6d20 3d20 5f74 7970 655f 6d61 705b 636f  m = _type_map[co
+00017f30: 6c74 7970 655d 0a20 2020 2020 2020 2020  ltype].         
+00017f40: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00017f50: 6765 745f 7479 7065 2874 6d5b 305d 2c20  get_type(tm[0], 
+00017f60: 746d 5b31 5d29 0a0a 2020 2020 2020 2020  tm[1])..        
+00017f70: 6966 2063 6f6c 7479 7065 203d 3d20 5479  if coltype == Ty
+00017f80: 7065 436f 6465 732e 5354 5249 4e47 3a0a  peCodes.STRING:.
+00017f90: 2020 2020 2020 2020 2020 2020 7374 726c              strl
+00017fa0: 656e 203d 2073 656c 662e 5f67 6574 5f69  en = self._get_i
+00017fb0: 6e74 2829 0a20 2020 2020 2020 2020 2020  nt().           
+00017fc0: 206f 6666 7365 7420 3d20 7365 6c66 2e5f   offset = self._
+00017fd0: 6f66 6673 6574 0a20 2020 2020 2020 2020  offset.         
+00017fe0: 2020 2073 656c 662e 5f6f 6666 7365 7420     self._offset 
+00017ff0: 2b3d 2073 7472 6c65 6e0a 2020 2020 2020  += strlen.      
+00018000: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00018010: 662e 5f62 7566 2829 5b6f 6666 7365 7420  f._buf()[offset 
+00018020: 3a20 6f66 6673 6574 202b 2073 7472 6c65  : offset + strle
+00018030: 6e5d 2e64 6563 6f64 6528 2275 7466 2d38  n].decode("utf-8
+00018040: 222c 2065 7272 6f72 733d 2272 6570 6c61  ", errors="repla
+00018050: 6365 2229 0a0a 2020 2020 2020 2020 6966  ce")..        if
+00018060: 2063 6f6c 7479 7065 203d 3d20 5479 7065   coltype == Type
+00018070: 436f 6465 732e 5449 4d45 5354 414d 503a  Codes.TIMESTAMP:
+00018080: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00018090: 7572 6e20 6461 7465 7469 6d65 2e64 6174  urn datetime.dat
+000180a0: 6574 696d 652e 7574 6366 726f 6d74 696d  etime.utcfromtim
+000180b0: 6573 7461 6d70 2873 656c 662e 5f67 6574  estamp(self._get
+000180c0: 5f6c 6f6e 6728 2929 0a0a 2020 2020 2020  _long())..      
+000180d0: 2020 6966 2063 6f6c 7479 7065 203d 3d20    if coltype == 
+000180e0: 5479 7065 436f 6465 732e 4e55 4c4c 3a0a  TypeCodes.NULL:.
+000180f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00018100: 726e 204e 6f6e 650a 0a20 2020 2020 2020  rn None..       
+00018110: 2069 6620 636f 6c74 7970 6520 3d3d 2054   if coltype == T
+00018120: 7970 6543 6f64 6573 2e42 5954 453a 0a20  ypeCodes.BYTE:. 
+00018130: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00018140: 6e20 696e 742e 6672 6f6d 5f62 7974 6573  n int.from_bytes
+00018150: 2873 656c 662e 5f67 6574 5f74 7970 6528  (self._get_type(
+00018160: 312c 205f 756e 7061 636b 5f63 6861 7229  1, _unpack_char)
+00018170: 2c20 2262 6967 222c 2073 6967 6e65 643d  , "big", signed=
+00018180: 5472 7565 290a 0a20 2020 2020 2020 2069  True)..        i
+00018190: 6620 636f 6c74 7970 6520 3d3d 2054 7970  f coltype == Typ
+000181a0: 6543 6f64 6573 2e54 494d 453a 0a20 2020  eCodes.TIME:.   
+000181b0: 2020 2020 2020 2020 206c 6f6e 675f 7365           long_se
+000181c0: 636f 6e64 7320 3d20 7365 6c66 2e5f 6765  conds = self._ge
+000181d0: 745f 6c6f 6e67 2829 0a20 2020 2020 2020  t_long().       
+000181e0: 2020 2020 2073 6563 6f6e 6420 3d20 6c6f       second = lo
+000181f0: 6e67 5f73 6563 6f6e 6473 2025 2036 300a  ng_seconds % 60.
+00018200: 2020 2020 2020 2020 2020 2020 6d69 6e75              minu
+00018210: 7465 7320 3d20 6c6f 6e67 5f73 6563 6f6e  tes = long_secon
+00018220: 6473 202f 2036 300a 2020 2020 2020 2020  ds / 60.        
+00018230: 2020 2020 6d69 6e75 7465 203d 2069 6e74      minute = int
+00018240: 286d 696e 7574 6573 2025 2036 3029 0a20  (minutes % 60). 
+00018250: 2020 2020 2020 2020 2020 2068 6f75 7273             hours
+00018260: 203d 206d 696e 7574 6573 202f 2036 300a   = minutes / 60.
+00018270: 2020 2020 2020 2020 2020 2020 686f 7572              hour
+00018280: 203d 2069 6e74 2868 6f75 7273 2025 2032   = int(hours % 2
+00018290: 3429 0a20 2020 2020 2020 2020 2020 2072  4).            r
+000182a0: 6574 7572 6e20 6461 7465 7469 6d65 2e74  eturn datetime.t
+000182b0: 696d 6528 686f 7572 2c20 6d69 6e75 7465  ime(hour, minute
+000182c0: 2c20 7365 636f 6e64 290a 0a20 2020 2020  , second)..     
+000182d0: 2020 2069 6620 636f 6c74 7970 6520 3d3d     if coltype ==
+000182e0: 2054 7970 6543 6f64 6573 2e42 494e 4152   TypeCodes.BINAR
+000182f0: 593a 0a20 2020 2020 2020 2020 2020 2073  Y:.            s
+00018300: 7472 6c65 6e20 3d20 7365 6c66 2e5f 6765  trlen = self._ge
+00018310: 745f 696e 7428 290a 2020 2020 2020 2020  t_int().        
+00018320: 2020 2020 6f66 6673 6574 203d 2073 656c      offset = sel
+00018330: 662e 5f6f 6666 7365 740a 2020 2020 2020  f._offset.      
+00018340: 2020 2020 2020 7365 6c66 2e5f 6f66 6673        self._offs
+00018350: 6574 202b 3d20 7374 726c 656e 0a20 2020  et += strlen.   
+00018360: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00018370: 7365 6c66 2e5f 6275 6628 295b 6f66 6673  self._buf()[offs
+00018380: 6574 203a 206f 6666 7365 7420 2b20 7374  et : offset + st
+00018390: 726c 656e 5d0a 0a20 2020 2020 2020 2069  rlen]..        i
+000183a0: 6620 636f 6c74 7970 6520 3d3d 2054 7970  f coltype == Typ
+000183b0: 6543 6f64 6573 2e44 4543 494d 414c 3a0a  eCodes.DECIMAL:.
+000183c0: 2020 2020 2020 2020 2020 2020 7072 6563              prec
+000183d0: 6973 696f 6e20 3d20 7365 6c66 2e5f 6765  ision = self._ge
+000183e0: 745f 6279 7465 2829 0a20 2020 2020 2020  t_byte().       
+000183f0: 2020 2020 2073 6361 6c65 203d 2073 656c       scale = sel
+00018400: 662e 5f67 6574 5f62 7974 6528 290a 0a20  f._get_byte().. 
+00018410: 2020 2020 2020 2020 2020 2069 6620 7072             if pr
+00018420: 6563 6973 696f 6e20 2520 3220 3d3d 2030  ecision % 2 == 0
+00018430: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00018440: 2020 7374 726c 656e 203d 2069 6e74 2828    strlen = int((
+00018450: 7072 6563 6973 696f 6e20 2f20 3229 202b  precision / 2) +
+00018460: 2031 290a 2020 2020 2020 2020 2020 2020   1).            
+00018470: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00018480: 2020 2020 2020 7374 726c 656e 203d 2069        strlen = i
+00018490: 6e74 2828 7072 6563 6973 696f 6e20 2b20  nt((precision + 
+000184a0: 3129 202f 2032 290a 0a20 2020 2020 2020  1) / 2)..       
+000184b0: 2020 2020 2064 6174 6120 3d20 7365 6c66       data = self
+000184c0: 2e5f 6275 6628 295b 7365 6c66 2e5f 6f66  ._buf()[self._of
+000184d0: 6673 6574 203a 2028 7365 6c66 2e5f 6f66  fset : (self._of
+000184e0: 6673 6574 202b 2073 7472 6c65 6e20 2d20  fset + strlen - 
+000184f0: 3129 5d0a 2020 2020 2020 2020 2020 2020  1)].            
+00018500: 6469 6769 7473 203d 205b 5d0a 2020 2020  digits = [].    
+00018510: 2020 2020 2020 2020 666f 7220 6279 7465          for byte
+00018520: 2069 6e20 6461 7461 3a0a 2020 2020 2020   in data:.      
+00018530: 2020 2020 2020 2020 2020 6469 6769 7473            digits
+00018540: 2e61 7070 656e 6428 2862 7974 6520 2620  .append((byte & 
+00018550: 3078 4630 2920 3e3e 2034 290a 2020 2020  0xF0) >> 4).    
+00018560: 2020 2020 2020 2020 2020 2020 6469 6769              digi
+00018570: 7473 2e61 7070 656e 6428 6279 7465 2026  ts.append(byte &
+00018580: 2030 7830 4629 0a0a 2020 2020 2020 2020   0x0F)..        
+00018590: 2020 2020 7369 676e 203d 2073 656c 662e      sign = self.
+000185a0: 5f62 7566 2829 5b73 656c 662e 5f6f 6666  _buf()[self._off
+000185b0: 7365 7420 2b20 7374 726c 656e 202d 2031  set + strlen - 1
+000185c0: 5d0a 0a20 2020 2020 2020 2020 2020 2064  ]..            d
+000185d0: 6967 6974 732e 6170 7065 6e64 2873 6967  igits.append(sig
+000185e0: 6e20 3e3e 2034 290a 2020 2020 2020 2020  n >> 4).        
+000185f0: 2020 2020 7369 676e 203d 2073 6967 6e20      sign = sign 
+00018600: 2620 3078 3046 0a0a 2020 2020 2020 2020  & 0x0F..        
+00018610: 2020 2020 6966 2073 6967 6e20 3d3d 2031      if sign == 1
+00018620: 323a 0a20 2020 2020 2020 2020 2020 2020  2:.             
+00018630: 2020 2073 6967 6e20 3d20 300a 2020 2020     sign = 0.    
+00018640: 2020 2020 2020 2020 656c 6966 2073 6967          elif sig
+00018650: 6e20 3d3d 2031 333a 0a20 2020 2020 2020  n == 13:.       
+00018660: 2020 2020 2020 2020 2073 6967 6e20 3d20           sign = 
+00018670: 310a 2020 2020 2020 2020 2020 2020 656c  1.            el
+00018680: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00018690: 2020 2020 7261 6973 6520 4572 726f 7228      raise Error(
+000186a0: 7265 6173 6f6e 3d66 2255 6e6b 6e6f 776e  reason=f"Unknown
+000186b0: 2064 6563 696d 616c 2073 6967 6e20 7661   decimal sign va
+000186c0: 6c75 6520 7b73 6967 6e7d 2229 0a0a 2020  lue {sign}")..  
+000186d0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000186e0: 6f66 6673 6574 202b 3d20 7374 726c 656e  offset += strlen
+000186f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00018700: 7572 6e20 6465 6369 6d61 6c2e 4465 6369  urn decimal.Deci
+00018710: 6d61 6c28 2873 6967 6e2c 2064 6967 6974  mal((sign, digit
+00018720: 732c 202d 7363 616c 6529 290a 0a20 2020  s, -scale))..   
+00018730: 2020 2020 2069 6620 636f 6c74 7970 6520       if coltype 
+00018740: 3d3d 2054 7970 6543 6f64 6573 2e41 5252  == TypeCodes.ARR
+00018750: 4159 3a0a 2020 2020 2020 2020 2020 2020  AY:.            
+00018760: 6e65 7374 6564 5f6c 6576 656c 203d 2030  nested_level = 0
+00018770: 0a0a 2020 2020 2020 2020 2020 2020 6172  ..            ar
+00018780: 7261 7974 7970 6520 3d20 7365 6c66 2e5f  raytype = self._
+00018790: 6765 745f 6279 7465 2829 0a0a 2020 2020  get_byte()..    
+000187a0: 2020 2020 2020 2020 7768 696c 6520 6172          while ar
+000187b0: 7261 7974 7970 6520 3d3d 2054 7970 6543  raytype == TypeC
+000187c0: 6f64 6573 2e41 5252 4159 3a0a 2020 2020  odes.ARRAY:.    
+000187d0: 2020 2020 2020 2020 2020 2020 6172 7261              arra
+000187e0: 7974 7970 6520 3d20 7365 6c66 2e5f 6765  ytype = self._ge
+000187f0: 745f 6279 7465 2829 0a20 2020 2020 2020  t_byte().       
+00018800: 2020 2020 2020 2020 206e 6573 7465 645f           nested_
+00018810: 6c65 7665 6c20 2b3d 2031 0a0a 2020 2020  level += 1..    
+00018820: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00018830: 656c 662e 5f67 6574 5f61 7272 6179 286e  elf._get_array(n
+00018840: 6573 7465 645f 6c65 7665 6c29 0a0a 2020  ested_level)..  
+00018850: 2020 2020 2020 6966 2063 6f6c 7479 7065        if coltype
+00018860: 203d 3d20 5479 7065 436f 6465 732e 5555   == TypeCodes.UU
+00018870: 4944 3a0a 2020 2020 2020 2020 2020 2020  ID:.            
+00018880: 7365 6c66 2e5f 6f66 6673 6574 202b 3d20  self._offset += 
+00018890: 3136 0a20 2020 2020 2020 2020 2020 2072  16.            r
+000188a0: 6574 7572 6e20 7575 6964 2e55 5549 4428  eturn uuid.UUID(
+000188b0: 6279 7465 733d 7365 6c66 2e5f 6275 6628  bytes=self._buf(
+000188c0: 295b 7365 6c66 2e5f 6f66 6673 6574 202d  )[self._offset -
+000188d0: 2031 3620 3a20 7365 6c66 2e5f 6f66 6673   16 : self._offs
+000188e0: 6574 5d29 0a0a 2020 2020 2020 2020 6966  et])..        if
+000188f0: 2063 6f6c 7479 7065 203d 3d20 5479 7065   coltype == Type
+00018900: 436f 6465 732e 5354 5f50 4f49 4e54 3a0a  Codes.ST_POINT:.
+00018910: 2020 2020 2020 2020 2020 2020 6c6f 6e67              long
+00018920: 203d 2073 656c 662e 5f67 6574 5f64 6f75   = self._get_dou
+00018930: 626c 6528 290a 2020 2020 2020 2020 2020  ble().          
+00018940: 2020 6c61 7420 3d20 7365 6c66 2e5f 6765    lat = self._ge
+00018950: 745f 646f 7562 6c65 2829 0a20 2020 2020  t_double().     
+00018960: 2020 2020 2020 2072 6574 7572 6e20 5f53         return _S
+00018970: 5450 6f69 6e74 286c 6f6e 672c 206c 6174  TPoint(long, lat
+00018980: 290a 0a20 2020 2020 2020 2069 6620 636f  )..        if co
+00018990: 6c74 7970 6520 3d3d 2054 7970 6543 6f64  ltype == TypeCod
+000189a0: 6573 2e44 4154 453a 0a20 2020 2020 2020  es.DATE:.       
+000189b0: 2020 2020 2064 203d 2064 6174 6574 696d       d = datetim
+000189c0: 652e 6461 7465 7469 6d65 2e75 7463 6672  e.datetime.utcfr
+000189d0: 6f6d 7469 6d65 7374 616d 7028 7365 6c66  omtimestamp(self
+000189e0: 2e5f 6765 745f 6c6f 6e67 2829 202f 2031  ._get_long() / 1
+000189f0: 3030 302e 3029 0a20 2020 2020 2020 2020  000.0).         
+00018a00: 2020 2072 6574 7572 6e20 6461 7465 7469     return dateti
+00018a10: 6d65 2e64 6174 6528 642e 7965 6172 2c20  me.date(d.year, 
+00018a20: 642e 6d6f 6e74 682c 2064 2e64 6179 290a  d.month, d.day).
+00018a30: 0a20 2020 2020 2020 2069 6620 636f 6c74  .        if colt
+00018a40: 7970 6520 3d3d 2054 7970 6543 6f64 6573  ype == TypeCodes
+00018a50: 2e49 503a 0a20 2020 2020 2020 2020 2020  .IP:.           
+00018a60: 206f 6666 203d 2073 656c 662e 5f6f 6666   off = self._off
+00018a70: 7365 740a 2020 2020 2020 2020 2020 2020  set.            
+00018a80: 7365 6c66 2e5f 6f66 6673 6574 202b 3d20  self._offset += 
+00018a90: 3136 0a20 2020 2020 2020 2020 2020 2072  16.            r
+00018aa0: 6574 7572 6e20 6970 6164 6472 6573 732e  eturn ipaddress.
+00018ab0: 6970 5f61 6464 7265 7373 2873 656c 662e  ip_address(self.
+00018ac0: 5f62 7566 2829 5b6f 6666 203a 206f 6666  _buf()[off : off
+00018ad0: 202b 2031 365d 290a 0a20 2020 2020 2020   + 16])..       
+00018ae0: 2069 6620 636f 6c74 7970 6520 3d3d 2054   if coltype == T
+00018af0: 7970 6543 6f64 6573 2e49 5056 343a 0a20  ypeCodes.IPV4:. 
+00018b00: 2020 2020 2020 2020 2020 206f 6666 203d             off =
+00018b10: 2073 656c 662e 5f6f 6666 7365 740a 2020   self._offset.  
+00018b20: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00018b30: 6f66 6673 6574 202b 3d20 340a 2020 2020  offset += 4.    
+00018b40: 2020 2020 2020 2020 7265 7475 726e 2069          return i
+00018b50: 7061 6464 7265 7373 2e69 705f 6164 6472  paddress.ip_addr
+00018b60: 6573 7328 7365 6c66 2e5f 6275 6628 295b  ess(self._buf()[
+00018b70: 6f66 6620 3a20 6f66 6620 2b20 345d 290a  off : off + 4]).
+00018b80: 0a20 2020 2020 2020 2069 6620 636f 6c74  .        if colt
+00018b90: 7970 6520 3d3d 2054 7970 6543 6f64 6573  ype == TypeCodes
+00018ba0: 2e54 494d 4553 5441 4d50 5f4e 414e 4f53  .TIMESTAMP_NANOS
+00018bb0: 3a0a 2020 2020 2020 2020 2020 2020 7469  :.            ti
+00018bc0: 6d65 7374 616d 7020 3d20 7365 6c66 2e5f  mestamp = self._
+00018bd0: 6765 745f 6c6f 6e67 2829 202f 2031 3030  get_long() / 100
+00018be0: 3030 3030 3030 302e 300a 2020 2020 2020  0000000.0.      
+00018bf0: 2020 2020 2020 7265 7475 726e 2064 6174        return dat
+00018c00: 6574 696d 652e 6461 7465 7469 6d65 2e75  etime.datetime.u
+00018c10: 7463 6672 6f6d 7469 6d65 7374 616d 7028  tcfromtimestamp(
+00018c20: 7469 6d65 7374 616d 7029 0a0a 2020 2020  timestamp)..    
+00018c30: 2020 2020 6966 2063 6f6c 7479 7065 203d      if coltype =
+00018c40: 3d20 5479 7065 436f 6465 732e 5449 4d45  = TypeCodes.TIME
+00018c50: 5f4e 414e 4f53 3a0a 2020 2020 2020 2020  _NANOS:.        
+00018c60: 2020 2020 6e61 6e6f 7320 3d20 7365 6c66      nanos = self
+00018c70: 2e5f 6765 745f 6c6f 6e67 2829 0a20 2020  ._get_long().   
+00018c80: 2020 2020 2020 2020 206d 6963 726f 7320           micros 
+00018c90: 3d20 696e 7428 286e 616e 6f73 202f 2031  = int((nanos / 1
+00018ca0: 3030 3029 2025 2031 3030 3030 3030 290a  000) % 1000000).
+00018cb0: 2020 2020 2020 2020 2020 2020 666c 6f61              floa
+00018cc0: 745f 7365 636f 6e64 7320 3d20 6e61 6e6f  t_seconds = nano
+00018cd0: 7320 2f20 3130 3030 3030 3030 3030 0a20  s / 1000000000. 
+00018ce0: 2020 2020 2020 2020 2020 2073 6563 6f6e             secon
+00018cf0: 6420 3d20 696e 7428 666c 6f61 745f 7365  d = int(float_se
+00018d00: 636f 6e64 7320 2520 3630 290a 2020 2020  conds % 60).    
+00018d10: 2020 2020 2020 2020 6d69 6e75 7465 7320          minutes 
+00018d20: 3d20 666c 6f61 745f 7365 636f 6e64 7320  = float_seconds 
+00018d30: 2f20 3630 0a20 2020 2020 2020 2020 2020  / 60.           
+00018d40: 206d 696e 7574 6520 3d20 696e 7428 6d69   minute = int(mi
+00018d50: 6e75 7465 7320 2520 3630 290a 2020 2020  nutes % 60).    
+00018d60: 2020 2020 2020 2020 686f 7572 7320 3d20          hours = 
+00018d70: 6d69 6e75 7465 7320 2f20 3630 0a20 2020  minutes / 60.   
+00018d80: 2020 2020 2020 2020 2068 6f75 7220 3d20           hour = 
+00018d90: 696e 7428 686f 7572 7320 2520 3234 290a  int(hours % 24).
+00018da0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00018db0: 7572 6e20 6461 7465 7469 6d65 2e74 696d  urn datetime.tim
+00018dc0: 6528 686f 7572 2c20 6d69 6e75 7465 2c20  e(hour, minute, 
+00018dd0: 7365 636f 6e64 2c20 6d69 6372 6f73 290a  second, micros).
+00018de0: 0a20 2020 2020 2020 2069 6620 636f 6c74  .        if colt
+00018df0: 7970 6520 3d3d 2054 7970 6543 6f64 6573  ype == TypeCodes
+00018e00: 2e54 5550 4c45 3a0a 2020 2020 2020 2020  .TUPLE:.        
+00018e10: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00018e20: 5f67 6574 5f74 7570 6c65 2829 0a0a 2020  _get_tuple()..  
+00018e30: 2020 2020 2020 6966 2063 6f6c 7479 7065        if coltype
+00018e40: 203d 3d20 5479 7065 436f 6465 732e 5354   == TypeCodes.ST
+00018e50: 5f4c 494e 4553 5452 494e 473a 0a20 2020  _LINESTRING:.   
+00018e60: 2020 2020 2020 2020 2070 6f69 6e74 7320           points 
+00018e70: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
+00018e80: 206e 756d 5f65 6c65 6d65 6e74 7320 3d20   num_elements = 
+00018e90: 7365 6c66 2e5f 6765 745f 696e 7428 290a  self._get_int().
+00018ea0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00018eb0: 6920 696e 2072 616e 6765 286e 756d 5f65  i in range(num_e
+00018ec0: 6c65 6d65 6e74 7329 3a0a 2020 2020 2020  lements):.      
+00018ed0: 2020 2020 2020 2020 2020 6c6f 6e67 203d            long =
+00018ee0: 2073 656c 662e 5f67 6574 5f64 6f75 626c   self._get_doubl
+00018ef0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+00018f00: 2020 2020 6c61 7420 3d20 7365 6c66 2e5f      lat = self._
+00018f10: 6765 745f 646f 7562 6c65 2829 0a20 2020  get_double().   
+00018f20: 2020 2020 2020 2020 2020 2020 2070 6f69               poi
+00018f30: 6e74 732e 6170 7065 6e64 285f 5354 506f  nts.append(_STPo
+00018f40: 696e 7428 6c6f 6e67 2c20 6c61 7429 290a  int(long, lat)).
+00018f50: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00018f60: 726e 205f 5354 4c69 6e65 7374 7269 6e67  rn _STLinestring
+00018f70: 2870 6f69 6e74 7329 0a0a 2020 2020 2020  (points)..      
+00018f80: 2020 6966 2063 6f6c 7479 7065 203d 3d20    if coltype == 
+00018f90: 5479 7065 436f 6465 732e 5354 5f50 4f4c  TypeCodes.ST_POL
+00018fa0: 5947 4f4e 3a0a 2020 2020 2020 2020 2020  YGON:.          
+00018fb0: 2020 6578 7465 7269 6f72 203d 205b 5d0a    exterior = [].
+00018fc0: 2020 2020 2020 2020 2020 2020 6e75 6d5f              num_
+00018fd0: 656c 656d 656e 7473 203d 2073 656c 662e  elements = self.
+00018fe0: 5f67 6574 5f69 6e74 2829 0a20 2020 2020  _get_int().     
+00018ff0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00019000: 7261 6e67 6528 6e75 6d5f 656c 656d 656e  range(num_elemen
+00019010: 7473 293a 0a20 2020 2020 2020 2020 2020  ts):.           
+00019020: 2020 2020 206c 6f6e 6720 3d20 7365 6c66       long = self
+00019030: 2e5f 6765 745f 646f 7562 6c65 2829 0a20  ._get_double(). 
+00019040: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00019050: 6174 203d 2073 656c 662e 5f67 6574 5f64  at = self._get_d
+00019060: 6f75 626c 6528 290a 2020 2020 2020 2020  ouble().        
+00019070: 2020 2020 2020 2020 6578 7465 7269 6f72          exterior
+00019080: 2e61 7070 656e 6428 5f53 5450 6f69 6e74  .append(_STPoint
+00019090: 286c 6f6e 672c 206c 6174 2929 0a20 2020  (long, lat)).   
+000190a0: 2020 2020 2020 2020 2068 6f6c 6573 203d           holes =
+000190b0: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
+000190c0: 6e75 6d5f 7269 6e67 7320 3d20 7365 6c66  num_rings = self
+000190d0: 2e5f 6765 745f 696e 7428 290a 2020 2020  ._get_int().    
+000190e0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+000190f0: 2072 616e 6765 286e 756d 5f72 696e 6773   range(num_rings
+00019100: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00019110: 2020 206e 756d 5f65 6c65 6d65 6e74 7320     num_elements 
+00019120: 3d20 7365 6c66 2e5f 6765 745f 696e 7428  = self._get_int(
+00019130: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00019140: 2020 7269 6e67 203d 205b 5d0a 2020 2020    ring = [].    
+00019150: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00019160: 6a20 696e 2072 616e 6765 286e 756d 5f65  j in range(num_e
+00019170: 6c65 6d65 6e74 7329 3a0a 2020 2020 2020  lements):.      
+00019180: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00019190: 6e67 203d 2073 656c 662e 5f67 6574 5f64  ng = self._get_d
+000191a0: 6f75 626c 6528 290a 2020 2020 2020 2020  ouble().        
+000191b0: 2020 2020 2020 2020 2020 2020 6c61 7420              lat 
+000191c0: 3d20 7365 6c66 2e5f 6765 745f 646f 7562  = self._get_doub
+000191d0: 6c65 2829 0a20 2020 2020 2020 2020 2020  le().           
+000191e0: 2020 2020 2020 2020 2072 696e 672e 6170           ring.ap
+000191f0: 7065 6e64 285f 5354 506f 696e 7428 6c6f  pend(_STPoint(lo
+00019200: 6e67 2c20 6c61 7429 290a 2020 2020 2020  ng, lat)).      
+00019210: 2020 2020 2020 2020 2020 686f 6c65 732e            holes.
+00019220: 6170 7065 6e64 2872 696e 6729 0a20 2020  append(ring).   
+00019230: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00019240: 5f53 5450 6f6c 7967 6f6e 2865 7874 6572  _STPolygon(exter
+00019250: 696f 722c 2068 6f6c 6573 290a 0a20 2020  ior, holes)..   
+00019260: 2020 2020 2073 656c 662e 656e 645f 6f66       self.end_of
+00019270: 5f64 6174 6120 3d20 5472 7565 0a20 2020  _data = True.   
+00019280: 2020 2020 2072 6169 7365 2045 7272 6f72       raise Error
+00019290: 2872 6561 736f 6e3d 6622 556e 6b6e 6f77  (reason=f"Unknow
+000192a0: 6e20 636f 6c75 6d6e 2074 7970 6520 7b63  n column type {c
+000192b0: 6f6c 7479 7065 7d22 290a 0a20 2020 2064  oltype}")..    d
+000192c0: 6566 205f 6765 745f 6279 7465 2873 656c  ef _get_byte(sel
+000192d0: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
+000192e0: 2020 206f 6666 7365 7420 3d20 7365 6c66     offset = self
+000192f0: 2e5f 6f66 6673 6574 0a20 2020 2020 2020  ._offset.       
+00019300: 2073 656c 662e 5f6f 6666 7365 7420 2b3d   self._offset +=
+00019310: 2031 0a20 2020 2020 2020 2072 6574 7572   1.        retur
+00019320: 6e20 7365 6c66 2e5f 6275 6628 295b 6f66  n self._buf()[of
+00019330: 6673 6574 5d0a 0a20 2020 2064 6566 205f  fset]..    def _
+00019340: 6765 745f 696e 7428 7365 6c66 2920 2d3e  get_int(self) ->
+00019350: 2069 6e74 3a0a 2020 2020 2020 2020 6f66   int:.        of
+00019360: 6673 6574 203d 2073 656c 662e 5f6f 6666  fset = self._off
+00019370: 7365 740a 2020 2020 2020 2020 7365 6c66  set.        self
+00019380: 2e5f 6f66 6673 6574 202b 3d20 340a 2020  ._offset += 4.  
+00019390: 2020 2020 2020 7220 3d20 5f75 6e70 6163        r = _unpac
+000193a0: 6b5f 696e 7428 7365 6c66 2e5f 6275 6628  k_int(self._buf(
+000193b0: 292c 206f 6666 7365 7429 5b30 5d0a 2020  ), offset)[0].  
+000193c0: 2020 2020 2020 6173 7365 7274 2069 7369        assert isi
+000193d0: 6e73 7461 6e63 6528 722c 2069 6e74 290a  nstance(r, int).
+000193e0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+000193f0: 0a0a 2020 2020 6465 6620 5f67 6574 5f6c  ..    def _get_l
+00019400: 6f6e 6728 7365 6c66 2920 2d3e 2069 6e74  ong(self) -> int
+00019410: 3a0a 2020 2020 2020 2020 6f66 6673 6574  :.        offset
+00019420: 203d 2073 656c 662e 5f6f 6666 7365 740a   = self._offset.
+00019430: 2020 2020 2020 2020 7365 6c66 2e5f 6f66          self._of
+00019440: 6673 6574 202b 3d20 380a 2020 2020 2020  fset += 8.      
+00019450: 2020 7220 3d20 5f75 6e70 6163 6b5f 6c6f    r = _unpack_lo
+00019460: 6e67 2873 656c 662e 5f62 7566 2829 2c20  ng(self._buf(), 
+00019470: 6f66 6673 6574 295b 305d 0a20 2020 2020  offset)[0].     
+00019480: 2020 2061 7373 6572 7420 6973 696e 7374     assert isinst
+00019490: 616e 6365 2872 2c20 696e 7429 0a20 2020  ance(r, int).   
+000194a0: 2020 2020 2072 6574 7572 6e20 720a 0a20       return r.. 
+000194b0: 2020 2064 6566 205f 6765 745f 646f 7562     def _get_doub
+000194c0: 6c65 2873 656c 6629 202d 3e20 666c 6f61  le(self) -> floa
+000194d0: 743a 0a20 2020 2020 2020 206f 6666 7365  t:.        offse
+000194e0: 7420 3d20 7365 6c66 2e5f 6f66 6673 6574  t = self._offset
+000194f0: 0a20 2020 2020 2020 2073 656c 662e 5f6f  .        self._o
+00019500: 6666 7365 7420 2b3d 2038 0a20 2020 2020  ffset += 8.     
+00019510: 2020 2072 203d 205f 756e 7061 636b 5f64     r = _unpack_d
+00019520: 6f75 626c 6528 7365 6c66 2e5f 6275 6628  ouble(self._buf(
+00019530: 292c 206f 6666 7365 7429 5b30 5d0a 2020  ), offset)[0].  
+00019540: 2020 2020 2020 6173 7365 7274 2069 7369        assert isi
+00019550: 6e73 7461 6e63 6528 722c 2066 6c6f 6174  nstance(r, float
+00019560: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00019570: 2072 0a0a 2020 2020 6465 6620 5f67 6574   r..    def _get
+00019580: 5f74 7970 6528 7365 6c66 2c20 6461 7461  _type(self, data
+00019590: 6c65 6e3a 2069 6e74 2c20 756e 7061 636b  len: int, unpack
+000195a0: 6572 3a20 4361 6c6c 6162 6c65 5b5b 6279  er: Callable[[by
+000195b0: 7465 732c 2069 6e74 5d2c 2054 7570 6c65  tes, int], Tuple
+000195c0: 5b5f 542c 202e 2e2e 5d5d 2920 2d3e 205f  [_T, ...]]) -> _
+000195d0: 543a 0a20 2020 2020 2020 206f 6666 7365  T:.        offse
+000195e0: 7420 3d20 7365 6c66 2e5f 6f66 6673 6574  t = self._offset
+000195f0: 0a20 2020 2020 2020 2073 656c 662e 5f6f  .        self._o
+00019600: 6666 7365 7420 2b3d 2064 6174 616c 656e  ffset += datalen
+00019610: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00019620: 756e 7061 636b 6572 2873 656c 662e 5f62  unpacker(self._b
+00019630: 7566 2829 2c20 6f66 6673 6574 295b 305d  uf(), offset)[0]
+00019640: 0a0a 2020 2020 6465 6620 5f67 6574 5f61  ..    def _get_a
+00019650: 7272 6179 2873 656c 662c 206c 6576 656c  rray(self, level
+00019660: 3a20 696e 7429 202d 3e20 4c69 7374 5b6f  : int) -> List[o
+00019670: 626a 6563 745d 3a0a 2020 2020 2020 2020  bject]:.        
+00019680: 6172 7261 793a 204c 6973 745b 6f62 6a65  array: List[obje
+00019690: 6374 5d20 3d20 5b5d 0a0a 2020 2020 2020  ct] = []..      
+000196a0: 2020 6e75 6d5f 656c 656d 656e 7473 203d    num_elements =
+000196b0: 2073 656c 662e 5f67 6574 5f69 6e74 2829   self._get_int()
+000196c0: 0a0a 2020 2020 2020 2020 616c 6c5f 6e75  ..        all_nu
+000196d0: 6c6c 203d 2073 656c 662e 5f67 6574 5f62  ll = self._get_b
+000196e0: 7974 6528 290a 0a20 2020 2020 2020 2069  yte()..        i
+000196f0: 6620 616c 6c5f 6e75 6c6c 2021 3d20 303a  f all_null != 0:
+00019700: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00019710: 7572 6e20 5b5d 0a0a 2020 2020 2020 2020  urn []..        
+00019720: 666f 7220 5f20 696e 2072 616e 6765 286e  for _ in range(n
+00019730: 756d 5f65 6c65 6d65 6e74 7329 3a0a 2020  um_elements):.  
+00019740: 2020 2020 2020 2020 2020 6966 206c 6576            if lev
+00019750: 656c 203e 2030 3a0a 2020 2020 2020 2020  el > 0:.        
+00019760: 2020 2020 2020 2020 6172 7261 792e 6170          array.ap
+00019770: 7065 6e64 2873 656c 662e 5f67 6574 5f61  pend(self._get_a
+00019780: 7272 6179 286c 6576 656c 202d 2031 2929  rray(level - 1))
+00019790: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+000197a0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000197b0: 2020 2061 7272 6179 2e61 7070 656e 6428     array.append(
+000197c0: 7365 6c66 2e5f 6465 636f 6465 5f65 6e74  self._decode_ent
+000197d0: 7279 2829 290a 0a20 2020 2020 2020 2072  ry())..        r
+000197e0: 6574 7572 6e20 6172 7261 790a 0a20 2020  eturn array..   
+000197f0: 2064 6566 205f 636c 6f73 655f 7265 7375   def _close_resu
+00019800: 6c74 7365 7428 7365 6c66 2920 2d3e 204e  ltset(self) -> N
+00019810: 6f6e 653a 0a20 2020 2020 2020 2072 6571  one:.        req
+00019820: 203d 2070 726f 746f 2e52 6571 7565 7374   = proto.Request
+00019830: 2829 0a20 2020 2020 2020 2072 6571 2e74  ().        req.t
+00019840: 7970 6520 3d20 7072 6f74 6f2e 5265 7175  ype = proto.Requ
+00019850: 6573 742e 5265 7175 6573 7454 7970 652e  est.RequestType.
+00019860: 5661 6c75 6528 2243 4c4f 5345 5f52 4553  Value("CLOSE_RES
+00019870: 554c 545f 5345 5422 2920 2023 2074 7970  ULT_SET")  # typ
+00019880: 653a 2069 676e 6f72 6520 2320 6874 7470  e: ignore # http
+00019890: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
+000198a0: 726f 746f 636f 6c62 7566 6665 7273 2f70  rotocolbuffers/p
+000198b0: 726f 746f 6275 662f 6973 7375 6573 2f31  rotobuf/issues/1
+000198c0: 3032 3430 0a0a 2020 2020 2020 2020 5f73  0240..        _s
+000198d0: 656e 645f 6d73 6728 7365 6c66 2e63 6f6e  end_msg(self.con
+000198e0: 6e65 6374 696f 6e2c 2072 6571 290a 0a20  nection, req).. 
+000198f0: 2020 2020 2020 2072 7370 203d 205f 7265         rsp = _re
+00019900: 6376 5f6d 7367 2873 656c 662e 636f 6e6e  cv_msg(self.conn
+00019910: 6563 7469 6f6e 2c20 7072 6f74 6f2e 436f  ection, proto.Co
+00019920: 6e66 6972 6d61 7469 6f6e 5265 7370 6f6e  nfirmationRespon
+00019930: 7365 2829 290a 0a20 2020 2020 2020 2069  se())..        i
+00019940: 6620 7273 702e 7479 7065 203d 3d20 7072  f rsp.type == pr
+00019950: 6f74 6f2e 436f 6e66 6972 6d61 7469 6f6e  oto.Confirmation
+00019960: 5265 7370 6f6e 7365 2e52 4553 504f 4e53  Response.RESPONS
+00019970: 455f 5741 524e 3a0a 2020 2020 2020 2020  E_WARN:.        
+00019980: 2020 2020 7761 726e 2872 7370 2e72 6561      warn(rsp.rea
+00019990: 736f 6e29 0a20 2020 2020 2020 2065 6c69  son).        eli
+000199a0: 6620 6e6f 7420 7273 702e 7479 7065 203d  f not rsp.type =
+000199b0: 3d20 7072 6f74 6f2e 436f 6e66 6972 6d61  = proto.Confirma
+000199c0: 7469 6f6e 5265 7370 6f6e 7365 2e52 4553  tionResponse.RES
+000199d0: 504f 4e53 455f 4f4b 3a0a 2020 2020 2020  PONSE_OK:.      
+000199e0: 2020 2020 2020 7261 6973 6520 5f63 6f6e        raise _con
+000199f0: 7665 7274 5f65 7863 6570 7469 6f6e 2872  vert_exception(r
+00019a00: 7370 290a 0a20 2020 2064 6566 205f 6765  sp)..    def _ge
+00019a10: 745f 7475 706c 6528 7365 6c66 2920 2d3e  t_tuple(self) ->
+00019a20: 2054 7570 6c65 5b6f 626a 6563 742c 202e   Tuple[object, .
+00019a30: 2e2e 5d3a 0a20 2020 2020 2020 206e 756d  ..]:.        num
+00019a40: 5f65 6c65 6d65 6e74 7320 3d20 7365 6c66  _elements = self
+00019a50: 2e5f 6765 745f 696e 7428 290a 2020 2020  ._get_int().    
+00019a60: 2020 2020 7265 7374 7570 6c65 3a20 5475      restuple: Tu
+00019a70: 706c 655b 6f62 6a65 6374 2c20 2e2e 2e5d  ple[object, ...]
+00019a80: 203d 2028 290a 2020 2020 2020 2020 666f   = ().        fo
+00019a90: 7220 5f20 696e 2072 616e 6765 286e 756d  r _ in range(num
+00019aa0: 5f65 6c65 6d65 6e74 7329 3a0a 2020 2020  _elements):.    
+00019ab0: 2020 2020 2020 2020 7265 7374 7570 6c65          restuple
+00019ac0: 202b 3d20 2873 656c 662e 5f64 6563 6f64   += (self._decod
+00019ad0: 655f 656e 7472 7928 292c 290a 2020 2020  e_entry(),).    
+00019ae0: 2020 2020 7265 7475 726e 2072 6573 7475      return restu
+00019af0: 706c 650a 0a0a 6465 6620 636f 6e6e 6563  ple...def connec
+00019b00: 7428 0a20 2020 2064 736e 3a20 4f70 7469  t(.    dsn: Opti
+00019b10: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00019b20: 2c0a 2020 2020 7573 6572 3a20 4f70 7469  ,.    user: Opti
+00019b30: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00019b40: 2c0a 2020 2020 7061 7373 776f 7264 3a20  ,.    password: 
+00019b50: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00019b60: 4e6f 6e65 2c0a 2020 2020 686f 7374 3a20  None,.    host: 
+00019b70: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00019b80: 4e6f 6e65 2c0a 2020 2020 6461 7461 6261  None,.    databa
+00019b90: 7365 3a20 4f70 7469 6f6e 616c 5b73 7472  se: Optional[str
+00019ba0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 746c  ] = None,.    tl
+00019bb0: 733a 204f 7074 696f 6e61 6c5b 556e 696f  s: Optional[Unio
+00019bc0: 6e5b 696e 742c 2073 7472 5d5d 203d 204e  n[int, str]] = N
+00019bd0: 6f6e 652c 0a20 2020 2066 6f72 6365 3a20  one,.    force: 
+00019be0: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
+00019bf0: 204e 6f6e 652c 0a20 2020 2068 616e 6473   None,.    hands
+00019c00: 6861 6b65 3a20 4f70 7469 6f6e 616c 5b55  hake: Optional[U
+00019c10: 6e69 6f6e 5b69 6e74 2c20 7374 725d 5d20  nion[int, str]] 
+00019c20: 3d20 2267 636d 222c 0a20 2020 2063 6f6e  = "gcm",.    con
+00019c30: 6669 6766 696c 653a 204f 7074 696f 6e61  figfile: Optiona
+00019c40: 6c5b 7374 725d 203d 204e 6f6e 652c 0a29  l[str] = None,.)
+00019c50: 202d 3e20 436f 6e6e 6563 7469 6f6e 3a0a   -> Connection:.
+00019c60: 2020 2020 2320 7079 6c69 6e74 3a20 6469      # pylint: di
+00019c70: 7361 626c 653d 746f 6f2d 6d61 6e79 2d61  sable=too-many-a
+00019c80: 7267 756d 656e 7473 0a20 2020 2022 2222  rguments.    """
+00019c90: 4372 6561 7465 2061 206e 6577 2064 6174  Create a new dat
+00019ca0: 6162 6173 6520 636f 6e6e 6563 7469 6f6e  abase connection
+00019cb0: 2e0a 0a20 2020 2054 6865 2063 6f6e 6e65  ...    The conne
+00019cc0: 6374 696f 6e20 7061 7261 6d65 7465 7273  ction parameters
+00019cd0: 2063 616e 2062 6520 7370 6563 6966 6965   can be specifie
+00019ce0: 6420 6173 2070 6172 7420 6f66 2074 6865  d as part of the
+00019cf0: 2064 736e 2c0a 2020 2020 7573 696e 6720   dsn,.    using 
+00019d00: 6b65 7977 6f72 6420 6172 6775 6d65 6e74  keyword argument
+00019d10: 7320 6f72 2062 6f74 682e 2020 4966 2062  s or both.  If b
+00019d20: 6f74 6820 6172 6520 7370 6563 6966 6965  oth are specifie
+00019d30: 642c 2074 6865 206b 6579 776f 7264 0a20  d, the keyword. 
+00019d40: 2020 2070 6172 616d 6574 6572 206f 7665     parameter ove
+00019d50: 7272 6964 6573 2074 6865 2076 616c 7565  rrides the value
+00019d60: 2069 6e20 7468 6520 6473 6e2e 0a0a 2020   in the dsn...  
+00019d70: 2020 5468 6520 4f63 6965 6e74 2044 534e    The Ocient DSN
+00019d80: 2069 7320 6f66 2074 6865 2066 6f72 6d61   is of the forma
+00019d90: 743a 0a20 2020 2060 6f63 6965 6e74 3a2f  t:.    `ocient:/
+00019da0: 2f75 7365 723a 7061 7373 776f 7264 405b  /user:password@[
+00019db0: 686f 7374 5d5b 3a70 6f72 745d 5b2f 6461  host][:port][/da
+00019dc0: 7461 6261 7365 5d5b 3f70 6172 616d 313d  tabase][?param1=
+00019dd0: 7661 6c75 6531 262e 2e2e 5d60 0a0a 2020  value1&...]`..  
+00019de0: 2020 6075 7365 7260 2061 6e64 2060 7061    `user` and `pa
+00019df0: 7373 776f 7264 6020 6d75 7374 2062 6520  ssword` must be 
+00019e00: 7375 7070 6c69 6564 2e20 2060 686f 7374  supplied.  `host
+00019e10: 6020 6465 6661 756c 7473 2074 6f20 6c6f  ` defaults to lo
+00019e20: 6361 6c68 6f73 742c 0a20 2020 2070 6f72  calhost,.    por
+00019e30: 7420 6465 6661 756c 7473 2074 6f20 3430  t defaults to 40
+00019e40: 3530 2c20 6461 7461 6261 7365 2064 6566  50, database def
+00019e50: 6175 6c74 7320 746f 2060 7379 7374 656d  aults to `system
+00019e60: 6020 616e 6420 6074 6c73 6020 6465 6661  ` and `tls` defa
+00019e70: 756c 7473 0a20 2020 2074 6f20 6075 6e76  ults.    to `unv
+00019e80: 6572 6966 6965 6460 2e0a 0a20 2020 204d  erified`...    M
+00019e90: 756c 7469 706c 6520 686f 7374 7320 6d61  ultiple hosts ma
+00019ea0: 7920 6265 2073 7065 6369 6669 6564 2c20  y be specified, 
+00019eb0: 7365 7061 7261 7465 6420 6279 2061 2063  separated by a c
+00019ec0: 6f6d 6d61 2c20 696e 2077 6869 6368 2063  omma, in which c
+00019ed0: 6173 6520 7468 650a 2020 2020 686f 7374  ase the.    host
+00019ee0: 7320 7769 6c6c 2062 6520 7472 6965 6420  s will be tried 
+00019ef0: 696e 206f 7264 6572 2020 5468 7573 2061  in order  Thus a
+00019f00: 6e20 6578 616d 706c 6520 4453 4e20 6d69  n example DSN mi
+00019f10: 6768 7420 6265 0a20 2020 2060 6f63 6965  ght be.    `ocie
+00019f20: 6e74 3a2f 2f73 6f6d 656f 6e65 3a73 6f6d  nt://someone:som
+00019f30: 6570 6173 7377 6f72 6440 686f 7374 312c  epassword@host1,
+00019f40: 686f 7374 323a 3430 3531 2f6d 7964 6260  host2:4051/mydb`
+00019f50: 0a0a 2020 2020 636f 6e66 6967 6669 6c65  ..    configfile
+00019f60: 2073 7065 6369 6669 6573 2074 6865 206e   specifies the n
+00019f70: 616d 6520 6f66 2061 2063 6f6e 6669 6775  ame of a configu
+00019f80: 7261 7469 6f6e 2066 696c 6520 696e 2049  ration file in I
+00019f90: 4e49 2066 6f72 6d61 742e 2053 6565 0a20  NI format. See. 
+00019fa0: 2020 2074 6865 2043 6f6e 6e65 6374 696f     the Connectio
+00019fb0: 6e20 636c 6173 7320 666f 7220 6d6f 7265  n class for more
+00019fc0: 2064 6574 6169 6c65 6420 646f 6375 6d65   detailed docume
+00019fd0: 6e74 6174 696f 6e2e 0a0a 2020 2020 4375  ntation...    Cu
+00019fe0: 7272 656e 746c 7920 7375 7070 6f72 7465  rrently supporte
+00019ff0: 6420 7061 7261 6d65 7465 7273 2061 7265  d parameters are
+0001a000: 3a0a 0a20 2020 202d 2074 6c73 3a20 5768  :..    - tls: Wh
+0001a010: 6963 6820 6361 6e20 6861 7665 2074 6865  ich can have the
+0001a020: 2076 616c 7565 7320 226f 6666 222c 2022   values "off", "
+0001a030: 756e 7665 7269 6669 6564 222c 206f 7220  unverified", or 
+0001a040: 226f 6e22 2069 6e20 7468 6520 6473 6e2c  "on" in the dsn,
+0001a050: 0a20 2020 2020 2020 2020 6f72 2043 6f6e  .         or Con
+0001a060: 6e65 6374 696f 6e2e 544c 535f 4e4f 4e45  nection.TLS_NONE
+0001a070: 2c20 436f 6e6e 6563 7469 6f6e 2e54 4c53  , Connection.TLS
+0001a080: 5f55 4e56 4552 4946 4945 442c 206f 720a  _UNVERIFIED, or.
+0001a090: 2020 2020 2020 2020 2043 6f6e 6e65 6374           Connect
+0001a0a0: 696f 6e2e 544c 535f 4f4e 2061 7320 6120  ion.TLS_ON as a 
+0001a0b0: 6b65 7977 6f72 6420 7061 7261 6d65 7465  keyword paramete
+0001a0c0: 722e 0a20 2020 202d 2068 616e 6473 6861  r..    - handsha
+0001a0d0: 6b65 3a20 2243 4243 222c 2022 4743 4d22  ke: "CBC", "GCM"
+0001a0e0: 2c20 6f72 2022 5353 4f22 2e20 2247 434d  , or "SSO". "GCM
+0001a0f0: 2220 2847 616c 6f69 7320 436f 756e 7465  " (Galois Counte
+0001a100: 7220 4d6f 6465 2920 7368 6f75 6c64 2062  r Mode) should b
+0001a110: 6520 7573 6564 206f 7665 7220 2243 4243  e used over "CBC
+0001a120: 2220 2843 6970 6865 7220 426c 6f63 6b20  " (Cipher Block 
+0001a130: 4368 6169 6e69 6e67 2920 666f 7220 7061  Chaining) for pa
+0001a140: 7373 776f 7264 2065 6e63 7279 7074 696f  ssword encryptio
+0001a150: 6e2e 2022 5353 4f22 2066 6f72 2073 696e  n. "SSO" for sin
+0001a160: 676c 6520 7369 676e 206f 6e2e 0a20 2020  gle sign on..   
+0001a170: 202d 2066 6f72 6365 3a20 666f 7263 6520   - force: force 
+0001a180: 7468 6520 636f 6e6e 6563 7469 6f6e 2074  the connection t
+0001a190: 6f20 7265 6d61 696e 206f 6e20 7468 6973  o remain on this
+0001a1a0: 2068 6f73 740a 2020 2020 2222 220a 2020   host.    """.  
+0001a1b0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+0001a1c0: 6861 6e64 7368 616b 652c 2073 7472 293a  handshake, str):
+0001a1d0: 0a20 2020 2020 2020 2069 6620 6861 6e64  .        if hand
+0001a1e0: 7368 616b 652e 6c6f 7765 7228 2920 3d3d  shake.lower() ==
+0001a1f0: 2022 6763 6d22 3a0a 2020 2020 2020 2020   "gcm":.        
+0001a200: 2020 2020 6861 6e64 7368 616b 6520 3d20      handshake = 
+0001a210: 436f 6e6e 6563 7469 6f6e 2e48 414e 4453  Connection.HANDS
+0001a220: 4841 4b45 5f47 434d 0a20 2020 2020 2020  HAKE_GCM.       
+0001a230: 2065 6c69 6620 6861 6e64 7368 616b 652e   elif handshake.
+0001a240: 6c6f 7765 7228 2920 3d3d 2022 6362 6322  lower() == "cbc"
+0001a250: 3a0a 2020 2020 2020 2020 2020 2020 6861  :.            ha
+0001a260: 6e64 7368 616b 6520 3d20 436f 6e6e 6563  ndshake = Connec
+0001a270: 7469 6f6e 2e48 414e 4453 4841 4b45 5f43  tion.HANDSHAKE_C
+0001a280: 4243 0a20 2020 2020 2020 2065 6c69 6620  BC.        elif 
+0001a290: 6861 6e64 7368 616b 652e 6c6f 7765 7228  handshake.lower(
+0001a2a0: 2920 3d3d 2022 7373 6f22 3a0a 2020 2020  ) == "sso":.    
+0001a2b0: 2020 2020 2020 2020 6861 6e64 7368 616b          handshak
+0001a2c0: 6520 3d20 436f 6e6e 6563 7469 6f6e 2e48  e = Connection.H
+0001a2d0: 414e 4453 4841 4b45 5f53 534f 0a20 2020  ANDSHAKE_SSO.   
+0001a2e0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0001a2f0: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
+0001a300: 7469 6d65 4572 726f 7228 6622 556e 6b6e  timeError(f"Unkn
+0001a310: 6f77 6e20 4861 6e64 7368 616b 6520 6d65  own Handshake me
+0001a320: 7468 6f64 207b 6861 6e64 7368 616b 657d  thod {handshake}
+0001a330: 2229 0a0a 2020 2020 6966 2069 7369 6e73  ")..    if isins
+0001a340: 7461 6e63 6528 746c 732c 2073 7472 293a  tance(tls, str):
+0001a350: 0a20 2020 2020 2020 2069 6620 746c 732e  .        if tls.
+0001a360: 6c6f 7765 7228 2920 3d3d 2022 6f6e 223a  lower() == "on":
+0001a370: 0a20 2020 2020 2020 2020 2020 2074 6c73  .            tls
+0001a380: 203d 2043 6f6e 6e65 6374 696f 6e2e 544c   = Connection.TL
+0001a390: 535f 4f4e 0a20 2020 2020 2020 2065 6c69  S_ON.        eli
+0001a3a0: 6620 746c 732e 6c6f 7765 7228 2920 3d3d  f tls.lower() ==
+0001a3b0: 2022 756e 7665 7269 6669 6564 223a 0a20   "unverified":. 
+0001a3c0: 2020 2020 2020 2020 2020 2074 6c73 203d             tls =
+0001a3d0: 2043 6f6e 6e65 6374 696f 6e2e 544c 535f   Connection.TLS_
+0001a3e0: 554e 5645 5249 4649 4544 0a20 2020 2020  UNVERIFIED.     
+0001a3f0: 2020 2065 6c69 6620 746c 732e 6c6f 7765     elif tls.lowe
+0001a400: 7228 2920 3d3d 2022 6f66 6622 3a0a 2020  r() == "off":.  
+0001a410: 2020 2020 2020 2020 2020 746c 7320 3d20            tls = 
+0001a420: 436f 6e6e 6563 7469 6f6e 2e54 4c53 5f4e  Connection.TLS_N
+0001a430: 4f4e 450a 2020 2020 2020 2020 656c 7365  ONE.        else
+0001a440: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+0001a450: 6973 6520 5275 6e74 696d 6545 7272 6f72  ise RuntimeError
+0001a460: 2866 2255 6e6b 6e6f 776e 2054 4c53 206d  (f"Unknown TLS m
+0001a470: 6f64 6520 7b74 6c73 7d22 290a 0a20 2020  ode {tls}")..   
+0001a480: 2070 6172 616d 7320 3d20 7b0a 2020 2020   params = {.    
+0001a490: 2020 2020 2275 7365 7222 3a20 7573 6572      "user": user
+0001a4a0: 2c0a 2020 2020 2020 2020 2270 6173 7377  ,.        "passw
+0001a4b0: 6f72 6422 3a20 222a 2a2a 2a2a 222c 0a20  ord": "*****",. 
+0001a4c0: 2020 2020 2020 2022 686f 7374 223a 2068         "host": h
+0001a4d0: 6f73 742c 0a20 2020 2020 2020 2022 6461  ost,.        "da
+0001a4e0: 7461 6261 7365 223a 2064 6174 6162 6173  tabase": databas
+0001a4f0: 652c 0a20 2020 2020 2020 2022 746c 7322  e,.        "tls"
+0001a500: 3a20 746c 732c 0a20 2020 2020 2020 2022  : tls,.        "
+0001a510: 6861 6e64 7368 616b 6522 3a20 6861 6e64  handshake": hand
+0001a520: 7368 616b 652c 0a20 2020 207d 0a0a 2020  shake,.    }..  
+0001a530: 2020 6c6f 6767 6572 2e64 6562 7567 2866    logger.debug(f
+0001a540: 2243 6f6e 6e65 6374 207b 7061 7261 6d73  "Connect {params
+0001a550: 7d22 290a 0a20 2020 2072 6574 7572 6e20  }")..    return 
+0001a560: 436f 6e6e 6563 7469 6f6e 2864 736e 2c20  Connection(dsn, 
+0001a570: 7573 6572 2c20 7061 7373 776f 7264 2c20  user, password, 
+0001a580: 686f 7374 2c20 6461 7461 6261 7365 2c20  host, database, 
+0001a590: 746c 732c 2068 616e 6473 6861 6b65 2c20  tls, handshake, 
+0001a5a0: 666f 7263 652c 2063 6f6e 6669 6766 696c  force, configfil
+0001a5b0: 6529 0a                                  e).
```

### Comparing `pyocient-1.0.9/setup.py` & `pyocient-2.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Ocient Database Python API
 """
 
-from setuptools import setup
-from setuptools.command.build_py import build_py
-import pathlib
-import subprocess
 import os
+import pathlib
+from typing import Dict
+
+from setuptools import setup
 
 here = pathlib.Path(__file__).parent.absolute()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
-version = {}
-with open(os.path.join(here, "version.py")) as version_file:
-    exec(version_file.read(), version)
-    version = version["__version__"]
+with open(os.path.join(here, "pyocient", "pkg_version.py")) as version_file:
+    globals: Dict[str, str] = {}
+    exec(version_file.read(), globals)
+    version = globals["__version__"]
 
 setup(
     name="pyocient",
     version=version,
     description="Ocient Database Python API",
     author="Ocient Inc",
     author_email="info@ocient.com",
@@ -36,31 +36,31 @@
         # Indicate who your project is intended for
         "Topic :: Database",
         "Topic :: Database :: Front-Ends",
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
+        "Typing :: Typed",
     ],
     keywords="database, sql, development",
     setup_requires=[
         "wheel",
     ],
     install_requires=[
-        "dsnparse",
+        "dsnparse<=0.1.15",
         "prompt-toolkit",
         "pygments",
         "tabulate",
-        "cryptography<=36.0",
-        "cffi<=1.15.0",
-        "google-auth<=2.6",  # because google-api-python-client doesn't provide an upper bound for this dep
-        "protobuf<=3.19.1",  # because google-api-python-client doesn't provide an upper bound for this dep
-        "google-api-python-client",
+        "cryptography",
+        "protobuf>=3.20.0,<=4.22.0",
     ],
-    py_modules=["pyocient", "version", "ClientWireProtocol_pb2"],
+    packages=["pyocient"],
+    package_data={"pyocient": ["py.typed"]},
     entry_points={
         "console_scripts": [
-            "pyocient=pyocient:main",
+            "pyocient=pyocient.cli:main",
         ],
     },
-    python_requires=">=3.5, <4",
+    python_requires=">=3.7, <4",
+    options={"bdist_wheel": {"universal": "1"}},
 )
```

