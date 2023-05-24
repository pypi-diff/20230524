# Comparing `tmp/ssh_certificate_parser-1.3.3.tar.gz` & `tmp/ssh_certificate_parser-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_certificate_parser-1.3.3.tar", last modified: Mon Aug 16 18:37:09 2021, max compression
+gzip compressed data, was "ssh_certificate_parser-1.4.0.tar", last modified: Tue Mar 14 17:11:33 2023, max compression
```

## Comparing `ssh_certificate_parser-1.3.3.tar` & `ssh_certificate_parser-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 jbrown     (501) staff       (20)        0 2021-08-16 18:37:09.824585 ssh_certificate_parser-1.3.3/
--rw-r--r--   0 jbrown     (501) staff       (20)      919 2021-08-16 18:36:08.000000 ssh_certificate_parser-1.3.3/CHANGES.md
--rw-r--r--   0 jbrown     (501) staff       (20)      754 2021-08-16 18:26:11.000000 ssh_certificate_parser-1.3.3/LICENSE.txt
--rw-r--r--   0 jbrown     (501) staff       (20)       27 2021-01-05 00:06:46.000000 ssh_certificate_parser-1.3.3/MANIFEST.in
--rw-r--r--   0 jbrown     (501) staff       (20)     2207 2021-08-16 18:37:09.824371 ssh_certificate_parser-1.3.3/PKG-INFO
--rw-r--r--   0 jbrown     (501) staff       (20)     1179 2021-08-16 18:36:45.000000 ssh_certificate_parser-1.3.3/README.md
--rw-r--r--   0 jbrown     (501) staff       (20)       38 2021-08-16 18:37:09.824662 ssh_certificate_parser-1.3.3/setup.cfg
--rwxr-xr-x   0 jbrown     (501) staff       (20)     1278 2021-08-16 18:35:53.000000 ssh_certificate_parser-1.3.3/setup.py
-drwxr-xr-x   0 jbrown     (501) staff       (20)        0 2021-08-16 18:37:09.822754 ssh_certificate_parser-1.3.3/ssh_certificate_parser/
--rw-r--r--   0 jbrown     (501) staff       (20)     6382 2021-08-16 18:36:00.000000 ssh_certificate_parser-1.3.3/ssh_certificate_parser/__init__.py
--rw-r--r--   0 jbrown     (501) staff       (20)      335 2021-01-05 00:06:46.000000 ssh_certificate_parser-1.3.3/ssh_certificate_parser/__main__.py
--rw-r--r--   0 jbrown     (501) staff       (20)      548 2021-01-05 00:32:18.000000 ssh_certificate_parser-1.3.3/ssh_certificate_parser/errors.py
--rw-r--r--   0 jbrown     (501) staff       (20)      946 2021-08-13 19:50:04.000000 ssh_certificate_parser-1.3.3/ssh_certificate_parser/parser_helpers.py
-drwxr-xr-x   0 jbrown     (501) staff       (20)        0 2021-08-16 18:37:09.824055 ssh_certificate_parser-1.3.3/ssh_certificate_parser.egg-info/
--rw-r--r--   0 jbrown     (501) staff       (20)     2207 2021-08-16 18:37:09.000000 ssh_certificate_parser-1.3.3/ssh_certificate_parser.egg-info/PKG-INFO
--rw-r--r--   0 jbrown     (501) staff       (20)      448 2021-08-16 18:37:09.000000 ssh_certificate_parser-1.3.3/ssh_certificate_parser.egg-info/SOURCES.txt
--rw-r--r--   0 jbrown     (501) staff       (20)        1 2021-08-16 18:37:09.000000 ssh_certificate_parser-1.3.3/ssh_certificate_parser.egg-info/dependency_links.txt
--rw-r--r--   0 jbrown     (501) staff       (20)       10 2021-08-16 18:37:09.000000 ssh_certificate_parser-1.3.3/ssh_certificate_parser.egg-info/requires.txt
--rw-r--r--   0 jbrown     (501) staff       (20)       23 2021-08-16 18:37:09.000000 ssh_certificate_parser-1.3.3/ssh_certificate_parser.egg-info/top_level.txt
--rw-r--r--   0 jbrown     (501) staff       (20)       59 2021-01-05 00:32:18.000000 ssh_certificate_parser-1.3.3/test_requirements.txt
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-03-14 17:11:33.820502 ssh_certificate_parser-1.4.0/
+-rw-r--r--   0 jhammond   (502) staff       (20)      987 2023-03-14 17:09:46.000000 ssh_certificate_parser-1.4.0/CHANGES.md
+-rw-r--r--   0 jhammond   (502) staff       (20)      754 2023-03-14 16:41:07.000000 ssh_certificate_parser-1.4.0/LICENSE.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)       27 2023-03-14 16:41:07.000000 ssh_certificate_parser-1.4.0/MANIFEST.in
+-rw-r--r--   0 jhammond   (502) staff       (20)     2289 2023-03-14 17:11:33.820362 ssh_certificate_parser-1.4.0/PKG-INFO
+-rw-r--r--   0 jhammond   (502) staff       (20)     1179 2023-03-14 16:41:07.000000 ssh_certificate_parser-1.4.0/README.md
+-rw-r--r--   0 jhammond   (502) staff       (20)       38 2023-03-14 17:11:33.820536 ssh_certificate_parser-1.4.0/setup.cfg
+-rwxr-xr-x   0 jhammond   (502) staff       (20)     1378 2023-03-14 17:09:46.000000 ssh_certificate_parser-1.4.0/setup.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-03-14 17:11:33.819331 ssh_certificate_parser-1.4.0/ssh_certificate_parser/
+-rw-r--r--   0 jhammond   (502) staff       (20)     6327 2023-03-14 17:09:46.000000 ssh_certificate_parser-1.4.0/ssh_certificate_parser/__init__.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      335 2023-03-14 16:41:07.000000 ssh_certificate_parser-1.4.0/ssh_certificate_parser/__main__.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      548 2023-03-14 16:41:07.000000 ssh_certificate_parser-1.4.0/ssh_certificate_parser/errors.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      946 2023-03-14 16:41:07.000000 ssh_certificate_parser-1.4.0/ssh_certificate_parser/parser_helpers.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-03-14 17:11:33.819952 ssh_certificate_parser-1.4.0/ssh_certificate_parser.egg-info/
+-rw-r--r--   0 jhammond   (502) staff       (20)     2289 2023-03-14 17:11:33.000000 ssh_certificate_parser-1.4.0/ssh_certificate_parser.egg-info/PKG-INFO
+-rw-r--r--   0 jhammond   (502) staff       (20)      499 2023-03-14 17:11:33.000000 ssh_certificate_parser-1.4.0/ssh_certificate_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)        1 2023-03-14 17:11:33.000000 ssh_certificate_parser-1.4.0/ssh_certificate_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)       10 2023-03-14 17:11:33.000000 ssh_certificate_parser-1.4.0/ssh_certificate_parser.egg-info/requires.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)       23 2023-03-14 17:11:33.000000 ssh_certificate_parser-1.4.0/ssh_certificate_parser.egg-info/top_level.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)       80 2023-03-14 17:09:46.000000 ssh_certificate_parser-1.4.0/test_requirements.txt
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-03-14 17:11:33.820195 ssh_certificate_parser-1.4.0/tests/
+-rw-r--r--   0 jhammond   (502) staff       (20)     3943 2023-03-14 16:41:07.000000 ssh_certificate_parser-1.4.0/tests/test_basic.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1540 2023-03-14 16:41:07.000000 ssh_certificate_parser-1.4.0/tests/test_parser_functions.py
```

### Comparing `ssh_certificate_parser-1.3.3/CHANGES.md` & `ssh_certificate_parser-1.4.0/CHANGES.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 ChangeLog
 =========
 
+1.4.0
+-----
+
+- Adds proper support for `ecdsa-sha2-nistp384`
+
 1.3.3
 -----
+
 - Fix RtD link issue
 
 1.3.2
 -----
+
 - Fix PyPI project URLs
 
 1.3.1
 -----
+
 - Fix `setup.py` issues
 
 1.3.0
 -----
+
 - Can now parse ECDSA keys (if they're signed with an RSA CA)
 - Add `.from_file` constructor on `SSHCertificate`
 - Add a bunch of type hints
 - Improve documentation a bit
 
 1.2.0
 -----
+
 - Can now parse DSA and Ed25519 keys (although they still have to have been signed by an RSA CA)
 - Unit tests
 - `key_type` is now in the `SSHCertificate` object
 - `pubkey_parts` is a dictionary containing the appropriate parts for that key (e.g., `n` and `e` for RSA)
 - Now raises subclasses of `ssh_certificate_parser.errors.SSHCertificateParserError` instead of just `ValueError` with a string description
 
 1.1.0
 -----
+
 - CA certificate fingerprint (equivalent to `ssh-keygen -l -f /path/to/key.pub`) is now parsed for ssh-rsa CAs. I don't have any ECDSA/Ed25519 CAs so I haven't tested them!
```

### Comparing `ssh_certificate_parser-1.3.3/LICENSE.txt` & `ssh_certificate_parser-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssh_certificate_parser-1.3.3/PKG-INFO` & `ssh_certificate_parser-1.4.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: ssh_certificate_parser
-Version: 1.3.3
+Version: 1.4.0
 Summary: Python library for interacting with OpenSSH Certificates
 Home-page: https://github.com/easypost/ssh_certificate_parser
 Author: James Brown
 Author-email: jbrown@easypost.com
 License: ISC
 Project-URL: Docs, https://ssh-certificate-parser.readthedocs.io/
 Project-URL: Tracker, https://github.com/EasyPost/ssh_certificate_parser/issues
 Project-URL: Source, https://github.com/EasyPost/ssh_certificate_parser
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 `ssh_certificate_parser` is a small library for interacting with [OpenSSH host/user certificates](https://cvsweb.openbsd.org/cgi-bin/cvsweb/~checkout~/src/usr.bin/ssh/PROTOCOL.certkeys?rev=1.15&content-type=text/plain). Specifically, it supports RSA, DSA, and Ed25519 keys signed by an RSA certificate authority. It does not currently validate the CA signature, but merely parses out some fields.
@@ -39,9 +40,7 @@
 
 cert = SSHCertificate.from_file('/etc/ssh/ssh_host_rsa_key-cert.pub')
 
 remaining_seconds_of_validity = cert.remaining_validity
 ```
 
 Full documentation is at <https://ssh-certificate-parser.readthedocs.io/en/latest/>.
-
-
```

### Comparing `ssh_certificate_parser-1.3.3/README.md` & `ssh_certificate_parser-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ssh_certificate_parser-1.3.3/setup.py` & `ssh_certificate_parser-1.4.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 #!/usr/bin/env python
 
-from setuptools import setup, find_packages
-
+from setuptools import find_packages, setup
 
 setup(
     name="ssh_certificate_parser",
-    version="1.3.3",
+    version="1.4.0",
     author="James Brown",
     author_email="jbrown@easypost.com",
     url="https://github.com/easypost/ssh_certificate_parser",
     license="ISC",
-    packages=find_packages(exclude=['tests']),
+    packages=find_packages(exclude=["tests"]),
     description="Python library for interacting with OpenSSH Certificates",
-    long_description=open('README.md', 'r').read(),
-    long_description_content_type='text/markdown',
+    long_description=open("README.md", "r").read(),
+    long_description_content_type="text/markdown",
     install_requires=[
-        'attrs>=16',
+        "attrs>=16",
     ],
     project_urls={
-        'Docs': 'https://ssh-certificate-parser.readthedocs.io/',
-        'Tracker': 'https://github.com/EasyPost/ssh_certificate_parser/issues',
-        'Source': 'https://github.com/EasyPost/ssh_certificate_parser',
+        "Docs": "https://ssh-certificate-parser.readthedocs.io/",
+        "Tracker": "https://github.com/EasyPost/ssh_certificate_parser/issues",
+        "Source": "https://github.com/EasyPost/ssh_certificate_parser",
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Console",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: POSIX",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: ISC License (ISCL)",
-    ]
+    ],
 )
```

### Comparing `ssh_certificate_parser-1.3.3/ssh_certificate_parser/__init__.py` & `ssh_certificate_parser-1.4.0/ssh_certificate_parser/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import base64
-import hashlib
-import enum
 import datetime
-from typing import List
+import enum
+import hashlib
 from pathlib import Path
+from typing import List
 
 import attr
 
-from .errors import UnsupportedKeyTypeError
-from .errors import UnsupportedCertificateTypeError
-from .parser_helpers import take_u32
-from .parser_helpers import take_u64
-from .parser_helpers import take_pascal_bytestring
-from .parser_helpers import take_pascal_string
-from .parser_helpers import take_list
+from .errors import UnsupportedCertificateTypeError, UnsupportedKeyTypeError
+from .parser_helpers import (take_list, take_pascal_bytestring,
+                             take_pascal_string, take_u32, take_u64)
 
 __author__ = 'EasyPost <oss@easypost.com>'
-version_info = (1, 3, 3)
+version_info = (1, 4, 0)
 __version__ = '.'.join(str(s) for s in version_info)
 
 
 class CertType(enum.Enum):
     SSH2_CERT_TYPE_USER = 1
     SSH2_CERT_TYPE_HOST = 2
 
@@ -150,15 +146,15 @@
         valid_before, blob = take_u64(blob)
         valid_before = datetime.datetime.utcfromtimestamp(valid_before)
         crits, blob = take_list(blob, take_pascal_string)
         exts, blob = take_list(blob, take_pascal_string)
         unknown, blob = take_pascal_bytestring(blob)
         raw_ca, blob = take_pascal_bytestring(blob)
         ca_cert_type, raw_ca_rest = take_pascal_string(raw_ca)
-        if ca_cert_type == 'ssh-rsa':
+        if ca_cert_type == 'ssh-rsa' or ca_cert_type == 'ecdsa-sha2-nistp384':
             ca_cert = take_rsa_cert(raw_ca, raw_ca_rest)
         else:
             raise UnsupportedCertificateTypeError(ca_cert_type)
         signature = blob
         return SSHCertificate(
             serial, cert_type, key_id, principals, valid_after, valid_before,
             crits, exts, ca_cert, signature, key_type, pubkey_parts
```

### Comparing `ssh_certificate_parser-1.3.3/ssh_certificate_parser/errors.py` & `ssh_certificate_parser-1.4.0/ssh_certificate_parser/errors.py`

 * *Files identical despite different names*

### Comparing `ssh_certificate_parser-1.3.3/ssh_certificate_parser/parser_helpers.py` & `ssh_certificate_parser-1.4.0/ssh_certificate_parser/parser_helpers.py`

 * *Files identical despite different names*

### Comparing `ssh_certificate_parser-1.3.3/ssh_certificate_parser.egg-info/PKG-INFO` & `ssh_certificate_parser-1.4.0/ssh_certificate_parser.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: ssh-certificate-parser
-Version: 1.3.3
+Version: 1.4.0
 Summary: Python library for interacting with OpenSSH Certificates
 Home-page: https://github.com/easypost/ssh_certificate_parser
 Author: James Brown
 Author-email: jbrown@easypost.com
 License: ISC
 Project-URL: Docs, https://ssh-certificate-parser.readthedocs.io/
 Project-URL: Tracker, https://github.com/EasyPost/ssh_certificate_parser/issues
 Project-URL: Source, https://github.com/EasyPost/ssh_certificate_parser
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 `ssh_certificate_parser` is a small library for interacting with [OpenSSH host/user certificates](https://cvsweb.openbsd.org/cgi-bin/cvsweb/~checkout~/src/usr.bin/ssh/PROTOCOL.certkeys?rev=1.15&content-type=text/plain). Specifically, it supports RSA, DSA, and Ed25519 keys signed by an RSA certificate authority. It does not currently validate the CA signature, but merely parses out some fields.
@@ -39,9 +40,7 @@
 
 cert = SSHCertificate.from_file('/etc/ssh/ssh_host_rsa_key-cert.pub')
 
 remaining_seconds_of_validity = cert.remaining_validity
 ```
 
 Full documentation is at <https://ssh-certificate-parser.readthedocs.io/en/latest/>.
-
-
```

