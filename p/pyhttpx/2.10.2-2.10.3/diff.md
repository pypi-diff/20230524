# Comparing `tmp/pyhttpx-2.10.2.tar.gz` & `tmp/pyhttpx-2.10.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyhttpx-2.10.2.tar", last modified: Tue May 23 13:58:41 2023, max compression
+gzip compressed data, was "dist\pyhttpx-2.10.3.tar", last modified: Wed May 24 03:33:25 2023, max compression
```

## Comparing `pyhttpx-2.10.2.tar` & `pyhttpx-2.10.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/
--rw-rw-rw-   0        0        0     1086 2022-08-12 14:37:21.000000 pyhttpx-2.10.2/LICENSE
--rw-rw-rw-   0        0        0       24 2022-08-15 03:00:31.000000 pyhttpx-2.10.2/MANIFEST.in
--rw-rw-rw-   0        0        0      339 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/PKG-INFO
--rw-rw-rw-   0        0        0     3197 2023-05-23 13:16:49.000000 pyhttpx-2.10.2/README.md
--rw-rw-rw-   0        0        0        0 2022-08-15 02:16:12.000000 pyhttpx-2.10.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/pyhttpx/
--rw-rw-rw-   0        0        0       81 2022-12-05 09:21:49.000000 pyhttpx-2.10.2/pyhttpx/__init__.py
--rw-rw-rw-   0        0        0      262 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/__version__.py
--rw-rw-rw-   0        0        0      106 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/compat.py
--rw-rw-rw-   0        0        0     1107 2022-12-05 07:47:21.000000 pyhttpx-2.10.2/pyhttpx/exception.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/pyhttpx/layers/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/__init__.py
--rw-rw-rw-   0        0        0     2308 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/aes.py
--rw-rw-rw-   0        0        0     1114 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/chacha20_poly1305.py
--rw-rw-rw-   0        0        0     4618 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/cipher_aead.py
--rw-rw-rw-   0        0        0     3910 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/cipher_block.py
--rw-rw-rw-   0        0        0      266 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/ciphers.py
--rw-rw-rw-   0        0        0     4293 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/ecc.py
--rw-rw-rw-   0        0        0     6180 2023-01-31 06:58:53.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/hkdf.py
--rw-rw-rw-   0        0        0      947 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/kx_algs.py
--rw-rw-rw-   0        0        0     1771 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/prf.py
--rw-rw-rw-   0        0        0     8016 2023-05-23 13:46:40.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/extensions.py
--rw-rw-rw-   0        0        0      123 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/fields.py
--rw-rw-rw-   0        0        0     1232 2022-10-27 08:35:29.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/handshake.py
--rw-rw-rw-   0        0        0     6750 2023-04-03 08:04:05.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/keyexchange.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/linux/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/linux/__init__.py
--rw-rw-rw-   0        0        0    10488 2023-05-23 13:31:03.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/pyaiossl.py
--rw-rw-rw-   0        0        0    19396 2023-05-23 13:31:03.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/pyssl.py
--rw-rw-rw-   0        0        0     2357 2023-05-17 03:53:54.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/socks.py
--rw-rw-rw-   0        0        0     4513 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/suites.py
--rw-rw-rw-   0        0        0    19146 2023-05-20 08:13:11.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/tls_context.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/window/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/window/__init__.py
--rw-rw-rw-   0        0        0     9302 2023-03-08 03:35:13.000000 pyhttpx-2.10.2/pyhttpx/models.py
--rw-rw-rw-   0        0        0    16938 2023-05-23 13:12:16.000000 pyhttpx-2.10.2/pyhttpx/session.py
--rw-rw-rw-   0        0        0     1991 2023-05-23 12:56:47.000000 pyhttpx-2.10.2/pyhttpx/utils.py
--rw-rw-rw-   0        0        0     8230 2023-05-23 13:39:01.000000 pyhttpx-2.10.2/pyhttpx/websocket.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/pyhttpx.egg-info/
--rw-rw-rw-   0        0        0      339 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/pyhttpx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1248 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/pyhttpx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/pyhttpx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-08-15 06:28:23.000000 pyhttpx-2.10.2/pyhttpx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       68 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/pyhttpx.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/pyhttpx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/setup.cfg
--rw-rw-rw-   0        0        0     1576 2023-05-23 13:58:30.000000 pyhttpx-2.10.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/tests/
--rw-rw-rw-   0        0        0        0 2022-08-15 03:02:17.000000 pyhttpx-2.10.2/tests/__init__.py
--rw-rw-rw-   0        0        0     1197 2023-05-23 13:57:49.000000 pyhttpx-2.10.2/tests/requestTest.py
--rw-rw-rw-   0        0        0     1931 2023-05-23 13:43:36.000000 pyhttpx-2.10.2/tests/websocketTest.py
+drwxrwxrwx   0        0        0        0 2023-05-24 03:33:25.000000 pyhttpx-2.10.3/
+-rw-rw-rw-   0        0        0     1086 2022-08-12 14:37:21.000000 pyhttpx-2.10.3/LICENSE
+-rw-rw-rw-   0        0        0       24 2022-08-15 03:00:31.000000 pyhttpx-2.10.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      339 2023-05-24 03:33:25.000000 pyhttpx-2.10.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3197 2023-05-23 13:16:49.000000 pyhttpx-2.10.3/README.md
+-rw-rw-rw-   0        0        0        0 2022-08-15 02:16:12.000000 pyhttpx-2.10.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-24 03:33:25.000000 pyhttpx-2.10.3/pyhttpx/
+-rw-rw-rw-   0        0        0       81 2022-12-05 09:21:49.000000 pyhttpx-2.10.3/pyhttpx/__init__.py
+-rw-rw-rw-   0        0        0      262 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/__version__.py
+-rw-rw-rw-   0        0        0      106 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/compat.py
+-rw-rw-rw-   0        0        0     1107 2022-12-05 07:47:21.000000 pyhttpx-2.10.3/pyhttpx/exception.py
+drwxrwxrwx   0        0        0        0 2023-05-24 03:33:25.000000 pyhttpx-2.10.3/pyhttpx/layers/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 03:33:25.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 03:33:25.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/__init__.py
+-rw-rw-rw-   0        0        0     2308 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/aes.py
+-rw-rw-rw-   0        0        0     1114 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/chacha20_poly1305.py
+-rw-rw-rw-   0        0        0     4618 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/cipher_aead.py
+-rw-rw-rw-   0        0        0     3910 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/cipher_block.py
+-rw-rw-rw-   0        0        0      266 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/ciphers.py
+-rw-rw-rw-   0        0        0     4293 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/ecc.py
+-rw-rw-rw-   0        0        0     6180 2023-01-31 06:58:53.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/hkdf.py
+-rw-rw-rw-   0        0        0      947 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/kx_algs.py
+-rw-rw-rw-   0        0        0     1771 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/prf.py
+-rw-rw-rw-   0        0        0     8016 2023-05-23 13:46:40.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/extensions.py
+-rw-rw-rw-   0        0        0      123 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/fields.py
+-rw-rw-rw-   0        0        0     1232 2022-10-27 08:35:29.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/handshake.py
+-rw-rw-rw-   0        0        0     6750 2023-04-03 08:04:05.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/keyexchange.py
+drwxrwxrwx   0        0        0        0 2023-05-24 03:33:25.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/linux/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/linux/__init__.py
+-rw-rw-rw-   0        0        0    10488 2023-05-23 13:31:03.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/pyaiossl.py
+-rw-rw-rw-   0        0        0    19396 2023-05-23 13:31:03.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/pyssl.py
+-rw-rw-rw-   0        0        0     2357 2023-05-17 03:53:54.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/socks.py
+-rw-rw-rw-   0        0        0     4513 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/suites.py
+-rw-rw-rw-   0        0        0    19146 2023-05-20 08:13:11.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/tls_context.py
+drwxrwxrwx   0        0        0        0 2023-05-24 03:33:25.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/window/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/window/__init__.py
+-rw-rw-rw-   0        0        0     9302 2023-03-08 03:35:13.000000 pyhttpx-2.10.3/pyhttpx/models.py
+-rw-rw-rw-   0        0        0    16930 2023-05-24 03:33:07.000000 pyhttpx-2.10.3/pyhttpx/session.py
+-rw-rw-rw-   0        0        0     1991 2023-05-23 12:56:47.000000 pyhttpx-2.10.3/pyhttpx/utils.py
+-rw-rw-rw-   0        0        0     8230 2023-05-23 13:39:01.000000 pyhttpx-2.10.3/pyhttpx/websocket.py
+drwxrwxrwx   0        0        0        0 2023-05-24 03:33:25.000000 pyhttpx-2.10.3/pyhttpx.egg-info/
+-rw-rw-rw-   0        0        0      339 2023-05-24 03:33:24.000000 pyhttpx-2.10.3/pyhttpx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1248 2023-05-24 03:33:24.000000 pyhttpx-2.10.3/pyhttpx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 03:33:24.000000 pyhttpx-2.10.3/pyhttpx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-08-15 06:28:23.000000 pyhttpx-2.10.3/pyhttpx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       68 2023-05-24 03:33:24.000000 pyhttpx-2.10.3/pyhttpx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-24 03:33:24.000000 pyhttpx-2.10.3/pyhttpx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 03:33:25.000000 pyhttpx-2.10.3/setup.cfg
+-rw-rw-rw-   0        0        0     1576 2023-05-24 03:33:22.000000 pyhttpx-2.10.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 03:33:25.000000 pyhttpx-2.10.3/tests/
+-rw-rw-rw-   0        0        0        0 2022-08-15 03:02:17.000000 pyhttpx-2.10.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     1197 2023-05-23 13:57:49.000000 pyhttpx-2.10.3/tests/requestTest.py
+-rw-rw-rw-   0        0        0     1931 2023-05-23 13:43:36.000000 pyhttpx-2.10.3/tests/websocketTest.py
```

### Comparing `pyhttpx-2.10.2/LICENSE` & `pyhttpx-2.10.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.2/README.md` & `pyhttpx-2.10.3/README.md`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.2/pyhttpx/exception.py` & `pyhttpx-2.10.3/pyhttpx/exception.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/aes.py` & `pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/chacha20_poly1305.py` & `pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/chacha20_poly1305.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/cipher_aead.py` & `pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/cipher_aead.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/cipher_block.py` & `pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/cipher_block.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/ecc.py` & `pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/ecc.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/hkdf.py` & `pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/hkdf.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/kx_algs.py` & `pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/kx_algs.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/prf.py` & `pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/prf.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.2/pyhttpx/layers/tls/extensions.py` & `pyhttpx-2.10.3/pyhttpx/layers/tls/extensions.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.2/pyhttpx/layers/tls/handshake.py` & `pyhttpx-2.10.3/pyhttpx/layers/tls/handshake.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.2/pyhttpx/layers/tls/keyexchange.py` & `pyhttpx-2.10.3/pyhttpx/layers/tls/keyexchange.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.2/pyhttpx/layers/tls/pyaiossl.py` & `pyhttpx-2.10.3/pyhttpx/layers/tls/pyaiossl.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.2/pyhttpx/layers/tls/pyssl.py` & `pyhttpx-2.10.3/pyhttpx/layers/tls/pyssl.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.2/pyhttpx/layers/tls/socks.py` & `pyhttpx-2.10.3/pyhttpx/layers/tls/socks.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.2/pyhttpx/layers/tls/suites.py` & `pyhttpx-2.10.3/pyhttpx/layers/tls/suites.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.2/pyhttpx/layers/tls/tls_context.py` & `pyhttpx-2.10.3/pyhttpx/layers/tls/tls_context.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.2/pyhttpx/models.py` & `pyhttpx-2.10.3/pyhttpx/models.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.2/pyhttpx/session.py` & `pyhttpx-2.10.3/pyhttpx/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,15 @@
 
         msg = b'%s %s HTTP/1.1\r\n' % (req.method.encode('latin1'), req.path.encode('latin1'))
         dh = copy.deepcopy(req.headers) or default_headers()
         dh.update(send_kw)
         dh['Host'] = req.host
         dh=dict((k, v) for k, v in dh.items())
         req_body = ''
-        
+
         if req.method == 'POST':
             if req.data:
                 if isinstance(req.data, str):
                     req_body = req.data
 
                 elif isinstance(req.data, dict):
                     req_body = urlencode(req.data)
@@ -353,15 +353,15 @@
         }
         headers = copy.deepcopy(req.headers) or default_headers()
 
         for k,v in headers.items():
             k = k.lower()
             dh[k] = v
         if req.method == 'POST':
-            dh['Content-Length'] = len(req_body)
+            dh['content-length'] = len(req_body)
 
         head_block = []
         for k,v in dh.items():
             if not k in ['connection','host']:
                 head_block.append((k,v))
 
         _cookies = self.cookie_manger.get(get_top_domain(self.req.host))
```

### Comparing `pyhttpx-2.10.2/pyhttpx/utils.py` & `pyhttpx-2.10.3/pyhttpx/utils.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.2/pyhttpx/websocket.py` & `pyhttpx-2.10.3/pyhttpx/websocket.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.2/pyhttpx.egg-info/SOURCES.txt` & `pyhttpx-2.10.3/pyhttpx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.2/setup.py` & `pyhttpx-2.10.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         sys.exit(errno)
 
 
 
 packages = find_packages()
 setup(
     name = "pyhttpx",
-    version = "2.10.2",
+    version = "2.10.3",
     keywords = ["pip", "pyhttpx"],
     description = "HTTP library.",
     long_description = "HTTP library, TLS supported version：tls1.2/tls1.3, HTTP supported version: http1.1/http2",
     license = "MIT Licence",
 
     url = "https://github.com/zero3301/pyhttpx",
     author = "3301",
```

### Comparing `pyhttpx-2.10.2/tests/requestTest.py` & `pyhttpx-2.10.3/tests/requestTest.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.2/tests/websocketTest.py` & `pyhttpx-2.10.3/tests/websocketTest.py`

 * *Files identical despite different names*

