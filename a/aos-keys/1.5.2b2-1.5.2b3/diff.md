# Comparing `tmp/aos_keys-1.5.2b2-py3-none-any.whl.zip` & `tmp/aos_keys-1.5.2b3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 17029 bytes, number of entries: 16
+Zip file size: 17116 bytes, number of entries: 16
 -rw-rw-r--  2.0 unx      117 b- defN 22-Jun-30 08:41 aos_keys/__init__.py
--rw-rw-r--  2.0 unx     6733 b- defN 23-May-22 11:35 aos_keys/actions.py
+-rw-rw-r--  2.0 unx     6745 b- defN 23-May-23 08:41 aos_keys/actions.py
 -rw-rw-r--  2.0 unx    10184 b- defN 23-Apr-04 10:59 aos_keys/certificate_manager.py
 -rw-rw-r--  2.0 unx     3004 b- defN 23-Apr-04 11:14 aos_keys/cloud_api.py
 -rw-rw-r--  2.0 unx     3789 b- defN 22-Sep-23 09:10 aos_keys/common.py
 -rw-rw-r--  2.0 unx     4547 b- defN 23-Apr-04 10:59 aos_keys/crypto_container.py
--rw-rw-r--  2.0 unx     5970 b- defN 23-Apr-04 10:59 aos_keys/key_manager.py
--rw-rw-r--  2.0 unx     8397 b- defN 23-May-22 11:54 aos_keys/main.py
+-rw-rw-r--  2.0 unx     6210 b- defN 23-May-24 06:03 aos_keys/key_manager.py
+-rw-rw-r--  2.0 unx     8397 b- defN 23-May-23 08:09 aos_keys/main.py
 -rw-rw-r--  2.0 unx     1452 b- defN 22-Sep-23 09:10 aos_keys/files/1rootCA.crt
 -rw-rw-r--  2.0 unx      113 b- defN 22-Jun-30 08:41 aos_keys/files/__init__.py
--rw-rw-r--  2.0 unx     2565 b- defN 23-May-22 15:57 aos_keys-1.5.2b2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-22 15:57 aos_keys-1.5.2b2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       48 b- defN 23-May-22 15:57 aos_keys-1.5.2b2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-May-22 15:57 aos_keys-1.5.2b2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Apr-04 09:57 aos_keys-1.5.2b2.dist-info/zip-safe
-?rw-rw-r--  2.0 unx     1293 b- defN 23-May-22 15:57 aos_keys-1.5.2b2.dist-info/RECORD
-16 files, 48314 bytes uncompressed, 14899 bytes compressed:  69.2%
+-rw-rw-r--  2.0 unx     2565 b- defN 23-May-24 06:04 aos_keys-1.5.2b3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-24 06:04 aos_keys-1.5.2b3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       48 b- defN 23-May-24 06:04 aos_keys-1.5.2b3.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-24 06:04 aos_keys-1.5.2b3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-23 08:16 aos_keys-1.5.2b3.dist-info/zip-safe
+?rw-rw-r--  2.0 unx     1293 b- defN 23-May-24 06:04 aos_keys-1.5.2b3.dist-info/RECORD
+16 files, 48566 bytes uncompressed, 14986 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -24,26 +24,26 @@
 
 Filename: aos_keys/files/1rootCA.crt
 Comment: 
 
 Filename: aos_keys/files/__init__.py
 Comment: 
 
-Filename: aos_keys-1.5.2b2.dist-info/METADATA
+Filename: aos_keys-1.5.2b3.dist-info/METADATA
 Comment: 
 
-Filename: aos_keys-1.5.2b2.dist-info/WHEEL
+Filename: aos_keys-1.5.2b3.dist-info/WHEEL
 Comment: 
 
-Filename: aos_keys-1.5.2b2.dist-info/entry_points.txt
+Filename: aos_keys-1.5.2b3.dist-info/entry_points.txt
 Comment: 
 
-Filename: aos_keys-1.5.2b2.dist-info/top_level.txt
+Filename: aos_keys-1.5.2b3.dist-info/top_level.txt
 Comment: 
 
-Filename: aos_keys-1.5.2b2.dist-info/zip-safe
+Filename: aos_keys-1.5.2b3.dist-info/zip-safe
 Comment: 
 
-Filename: aos_keys-1.5.2b2.dist-info/RECORD
+Filename: aos_keys-1.5.2b3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aos_keys/actions.py

```diff
@@ -176,20 +176,20 @@
         'User name: ': user_info.get('username'),
         'email: ': user_info.get('email'),
         'role: ': user_role,
     }
 
     if user_role in ('oem', 'fleet owner'):
         print_info['OEM Title:'] = user_info.get('oem').get('title')
-        print_info['Fleets:'] = '\n'.join(fleet['title'] for fleet in user_info.get('fleets'))
+        print_info['Fleets:'] = '\n'.join(fleet['title'] for fleet in user_info.get('fleets', []))
     elif user_role == 'service provider':
         print_info['SP Title:'] = user_info.get('service_provider').get('title')
 
-    print_info['Permission groups: '] = '\n'.join(user_info.get('permission_groups'))
-    print_info['Standalone permissions: '] = '\n'.join(user_info.get('permissions'))
+    print_info['Permission groups: '] = '\n'.join(user_info.get('permission_groups', []))
+    print_info['Standalone permissions: '] = '\n'.join(user_info.get('permissions', []))
 
     table = Table(padding=0, title='Cloud user info', show_header=False)
     table.add_column('', no_wrap=True, justify='left', style='')
     table.add_column('')
     for head in print_info:
         table.add_row(head, str(print_info[head]))
```

## aos_keys/key_manager.py

```diff
@@ -1,20 +1,20 @@
 #
 #  Copyright (c) 2018-2022 Renesas Inc.
 #  Copyright (c) 2018-2022 EPAM Systems Inc.
 #
 """aos-keys certificates manager module."""
-
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.asymmetric import ec, rsa
 from cryptography.hazmat.primitives.hashes import SHA256
 from cryptography.hazmat.primitives.serialization import load_pem_private_key, NoEncryption, Encoding, PrivateFormat
 from cryptography.hazmat.primitives.serialization.pkcs12 import serialize_key_and_certificates, load_pkcs12
 from cryptography.x509 import load_pem_x509_certificate, Name, CertificateSigningRequestBuilder
 from cryptography.x509.oid import NameOID
+from datetime import datetime
 from rich.table import Table
 
 from aos_keys.common import console, AosKeysError
 
 _CERTIFICATE_START = b'-----BEGIN CERTIFICATE-----'
 
 
@@ -92,14 +92,19 @@
         certificate = load_pkcs12(cert.read(), password=None).cert.certificate
         org_list = certificate.subject.get_attributes_for_oid(NameOID.ORGANIZATION_NAME)
         if org_list:
             return org_list[0].value
         return 'aoscloud.io'
 
 
+def datetime_from_utc_to_local(utc_datetime):
+    now_aware = datetime.now().astimezone()
+    return utc_datetime.astimezone().isoformat(' ', 'seconds')
+
+
 def print_cert_info(cert_file_path: str) -> None:
     """
     Print information about user certificate.
 
     Args:
         cert_file_path: path to user certificate.
 
@@ -117,16 +122,16 @@
     table.add_column('', style='bold')
     table.add_row('File: ', cert_file_path)
     _print_cert_field(table, 'Aos base domain: ', certificate, NameOID.ORGANIZATION_NAME)
     table.add_row('Serial number: ', f'{certificate.serial_number:X}')
     _print_cert_field(table, 'User: ', certificate, NameOID.COMMON_NAME)
     _print_cert_field(table, 'e-mail: ', certificate, NameOID.EMAIL_ADDRESS)
     _print_cert_field(table, 'Company name: ', certificate, NameOID.ORGANIZATIONAL_UNIT_NAME)
-    table.add_row('Valid not before: ', str(certificate.not_valid_before))
-    table.add_row('Valid not after: ', str(certificate.not_valid_after))
+    table.add_row('Valid not before: ', str(datetime_from_utc_to_local(certificate.not_valid_before)))
+    table.add_row('Valid not after: ', str(datetime_from_utc_to_local(certificate.not_valid_after)))
     console.print(table)
 
 
 def pem_to_pkcs12_bytes(private_key_pem: bytes, certificate_pem: bytes, friendly_name: str) -> bytes:
     """
     Create pkcs12 container from private key and certificate.
```

## Comparing `aos_keys-1.5.2b2.dist-info/METADATA` & `aos_keys-1.5.2b3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aos-keys
-Version: 1.5.2b2
+Version: 1.5.2b3
 Summary: AosEdge private keys and certificate manager
 Author: EPAM Systems
 Author-email: support@aoscloud.io
 License: Apache License 2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

