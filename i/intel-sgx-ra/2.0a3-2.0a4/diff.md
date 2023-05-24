# Comparing `tmp/intel_sgx_ra-2.0a3.tar.gz` & `tmp/intel_sgx_ra-2.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intel_sgx_ra-2.0a3.tar", last modified: Wed May 17 13:01:32 2023, max compression
+gzip compressed data, was "intel_sgx_ra-2.0a4.tar", last modified: Wed May 24 14:32:20 2023, max compression
```

## Comparing `intel_sgx_ra-2.0a3.tar` & `intel_sgx_ra-2.0a4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:32.751222 intel_sgx_ra-2.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-17 13:01:32.751222 intel_sgx_ra-2.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-17 13:01:32.751222 intel_sgx_ra-2.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:32.743221 intel_sgx_ra-2.0a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:32.747221 intel_sgx_ra-2.0a3/src/intel_sgx_ra/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/attest.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/base64url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:32.747221 intel_sgx_ra-2.0a3/src/intel_sgx_ra/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/cli/verify.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/error.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/globs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/pccs.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/ratls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra/signer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:32.747221 intel_sgx_ra-2.0a3/src/intel_sgx_ra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-17 13:01:32.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-17 13:01:32.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:01:32.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-17 13:01:32.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:01:32.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-17 13:01:32.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 13:01:32.000000 intel_sgx_ra-2.0a3/src/intel_sgx_ra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:01:32.751222 intel_sgx_ra-2.0a3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/tests/test_pccs.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/tests/test_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-17 13:00:47.000000 intel_sgx_ra-2.0a3/tests/test_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:32:20.190170 intel_sgx_ra-2.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-24 14:32:20.190170 intel_sgx_ra-2.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-24 14:32:20.190170 intel_sgx_ra-2.0a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:32:20.186170 intel_sgx_ra-2.0a4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:32:20.186170 intel_sgx_ra-2.0a4/src/intel_sgx_ra/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/attest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/base64url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:32:20.186170 intel_sgx_ra-2.0a4/src/intel_sgx_ra/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/cli/verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/globs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/pccs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/ratls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/signer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:32:20.186170 intel_sgx_ra-2.0a4/src/intel_sgx_ra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-24 14:32:20.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-24 14:32:20.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:32:20.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-24 14:32:20.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:32:20.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-24 14:32:20.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-24 14:32:20.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:32:20.186170 intel_sgx_ra-2.0a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/tests/test_pccs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/tests/test_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/tests/test_regex.py
```

### Comparing `intel_sgx_ra-2.0a3/PKG-INFO` & `intel_sgx_ra-2.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intel_sgx_ra
-Version: 2.0a3
+Version: 2.0a4
 Summary: Intel SGX Remote Attestation verification library
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `intel_sgx_ra-2.0a3/README.md` & `intel_sgx_ra-2.0a4/README.md`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a3/setup.py` & `intel_sgx_ra-2.0a4/setup.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a3/src/intel_sgx_ra/attest.py` & `intel_sgx_ra-2.0a4/src/intel_sgx_ra/attest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """intel_ra_sgx.attest module."""
 
 import logging
 from datetime import datetime
 from hashlib import sha256
-from typing import Union, cast
+from typing import Literal, Optional, Tuple, Union, cast
 
 import cryptography.exceptions
 from cryptography import x509
 from cryptography.hazmat.primitives.asymmetric import ec
 from cryptography.hazmat.primitives.asymmetric.utils import encode_dss_signature
 from cryptography.hazmat.primitives.hashes import SHA256, HashAlgorithm
 
 from intel_sgx_ra import globs
 from intel_sgx_ra.error import (
     CertificateError,
     CertificateRevokedError,
+    CollateralsError,
     SGXDebugModeError,
     SGXVerificationError,
 )
 from intel_sgx_ra.pccs import get_pck_cert_crl, get_root_ca_crl
 from intel_sgx_ra.quote import Quote
 
 # define SGX_FLAGS_DEBUG 0x0000000000000002ULL
@@ -93,15 +94,31 @@
         raise exc
 
     logging.info("%s Certification chain", globs.OK)
 
     return True
 
 
-def verify_quote(quote: Union[Quote, bytes], pccs_url: str):
+def retrieve_collaterals(
+    pccs_url: str, ca: Literal["processor", "platform"]
+) -> Tuple[x509.CertificateRevocationList, x509.CertificateRevocationList]:
+    """Retrive collaterals from PCCS URL and PCK CA type."""
+    root_ca_crl: x509.CertificateRevocationList = get_root_ca_crl(pccs_url)
+    pck_ca_crl: x509.CertificateRevocationList = get_pck_cert_crl(pccs_url, ca)
+
+    return root_ca_crl, pck_ca_crl
+
+
+def verify_quote(
+    quote: Union[Quote, bytes],
+    collaterals: Optional[
+        Tuple[x509.CertificateRevocationList, x509.CertificateRevocationList]
+    ] = None,
+    pccs_url: Optional[str] = None,
+):
     """Process DCAP remote attestation with `quote`."""
     quote = cast(Quote, Quote.from_bytes(quote) if isinstance(quote, bytes) else quote)
 
     # If set, then the enclave is in debug mode
     debug: bool = bool(quote.report_body.flags & SGX_FLAGS_DEBUG)
 
     logging.info("%s No SGX debug mode", globs.FAIL if debug else globs.OK)
@@ -109,25 +126,30 @@
     if debug:
         raise SGXDebugModeError
 
     pck_cert, pck_ca_cert, root_ca_cert = [
         x509.load_pem_x509_certificate(raw_cert) for raw_cert in quote.certs()
     ]  # type: x509.Certificate, x509.Certificate, x509.Certificate
 
-    root_ca_crl: x509.CertificateRevocationList = get_root_ca_crl(pccs_url)
-    common_name, *_ = pck_ca_cert.subject.get_attributes_for_oid(
-        x509.NameOID.COMMON_NAME
-    )
+    root_ca_crl: x509.CertificateRevocationList
     pck_ca_crl: x509.CertificateRevocationList
-    if common_name.value == "Intel SGX PCK Platform CA":
-        pck_ca_crl = get_pck_cert_crl(pccs_url, "platform")
-    elif common_name.value == "Intel SGX PCK Processor CA":
-        pck_ca_crl = get_pck_cert_crl(pccs_url, "processor")
+    if pccs_url is not None:
+        common_name, *_ = pck_ca_cert.subject.get_attributes_for_oid(
+            x509.NameOID.COMMON_NAME
+        )
+        if common_name.value == "Intel SGX PCK Platform CA":
+            root_ca_crl, pck_ca_crl = retrieve_collaterals(pccs_url, "platform")
+        elif common_name.value == "Intel SGX PCK Processor CA":
+            root_ca_crl, pck_ca_crl = retrieve_collaterals(pccs_url, "processor")
+        else:
+            raise CertificateError("Unknown CN in Intel SGX PCK Platform/Processor CA")
+    elif collaterals is not None:
+        root_ca_crl, pck_ca_crl = collaterals
     else:
-        raise CertificateError("Unknown CN in Intel SGX PCK Platform/Processor CA")
+        raise CollateralsError("Collaterals or PCCS URL missing")
 
     assert verify_pck_chain(
         root_ca_cert, pck_ca_cert, pck_cert, root_ca_crl, pck_ca_crl
     )
 
     ecdsa_attestation_pk = ec.EllipticCurvePublicNumbers(
         curve=ec.SECP256R1(),
```

### Comparing `intel_sgx_ra-2.0a3/src/intel_sgx_ra/base64url.py` & `intel_sgx_ra-2.0a4/src/intel_sgx_ra/base64url.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a3/src/intel_sgx_ra/cli/utils.py` & `intel_sgx_ra-2.0a4/src/intel_sgx_ra/cli/utils.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a3/src/intel_sgx_ra/cli/verify.py` & `intel_sgx_ra-2.0a4/src/intel_sgx_ra/cli/verify.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a3/src/intel_sgx_ra/pccs.py` & `intel_sgx_ra-2.0a4/src/intel_sgx_ra/pccs.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a3/src/intel_sgx_ra/quote.py` & `intel_sgx_ra-2.0a4/src/intel_sgx_ra/quote.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a3/src/intel_sgx_ra/ratls.py` & `intel_sgx_ra-2.0a4/src/intel_sgx_ra/ratls.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a3/src/intel_sgx_ra/signer.py` & `intel_sgx_ra-2.0a4/src/intel_sgx_ra/signer.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a3/src/intel_sgx_ra.egg-info/PKG-INFO` & `intel_sgx_ra-2.0a4/src/intel_sgx_ra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intel-sgx-ra
-Version: 2.0a3
+Version: 2.0a4
 Summary: Intel SGX Remote Attestation verification library
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `intel_sgx_ra-2.0a3/src/intel_sgx_ra.egg-info/SOURCES.txt` & `intel_sgx_ra-2.0a4/src/intel_sgx_ra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a3/tests/test_pccs.py` & `intel_sgx_ra-2.0a4/tests/test_pccs.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a3/tests/test_quote.py` & `intel_sgx_ra-2.0a4/tests/test_quote.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a3/tests/test_regex.py` & `intel_sgx_ra-2.0a4/tests/test_regex.py`

 * *Files identical despite different names*

