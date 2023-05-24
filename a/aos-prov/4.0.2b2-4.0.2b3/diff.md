# Comparing `tmp/aos_prov-4.0.2b2-py3-none-any.whl.zip` & `tmp/aos_prov-4.0.2b3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,13 @@
-Zip file size: 68479 bytes, number of entries: 59
+Zip file size: 64410 bytes, number of entries: 56
 -rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/__init__.py
 -rw-rw-r--  2.0 unx     2842 b- defN 23-Apr-04 10:59 aos_prov/actions.py
--rw-rw-r--  2.0 unx     7271 b- defN 23-May-22 11:54 aos_prov/main.py
+-rw-rw-r--  2.0 unx     7325 b- defN 23-May-23 08:08 aos_prov/main.py
 -rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/commands/__init__.py
 -rw-rw-r--  2.0 unx     7501 b- defN 23-Apr-04 10:59 aos_prov/commands/command_provision.py
--rw-rw-r--  2.0 unx     4883 b- defN 23-Jan-19 09:24 aos_prov/commands/command_vm.py
--rw-rw-r--  2.0 unx     2326 b- defN 22-Dec-16 09:22 aos_prov/commands/command_vm_libvirt.py
 -rw-rw-r--  2.0 unx     9689 b- defN 23-Apr-04 10:59 aos_prov/commands/command_vm_multi_node_manage.py
 -rw-rw-r--  2.0 unx     3799 b- defN 23-Apr-04 10:59 aos_prov/commands/download.py
 -rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/communication/__init__.py
 -rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/communication/cloud/__init__.py
 -rw-rw-r--  2.0 unx     8552 b- defN 23-Apr-04 10:59 aos_prov/communication/cloud/cloud_api.py
 -rw-rw-r--  2.0 unx       89 b- defN 22-Apr-10 14:06 aos_prov/communication/unit/__init__.py
 -rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v0/__init__.py
@@ -37,25 +35,24 @@
 -rw-rw-r--  2.0 unx    12904 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2_grpc.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Dec-01 17:44 aos_prov/communication/unit/v4/__init__.py
 -rw-rw-r--  2.0 unx     9592 b- defN 23-Apr-04 10:59 aos_prov/communication/unit/v4/unit_communication_v4.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Dec-01 17:44 aos_prov/communication/unit/v4/generated/__init__.py
 -rw-rw-r--  2.0 unx    18433 b- defN 22-Dec-01 17:44 aos_prov/communication/unit/v4/generated/iamanager_pb2.py
 -rw-rw-r--  2.0 unx    33405 b- defN 22-Dec-01 17:44 aos_prov/communication/unit/v4/generated/iamanager_pb2_grpc.py
 -rw-rw-r--  2.0 unx     2705 b- defN 22-Apr-10 14:06 aos_prov/files/1rootCA.crt
--rw-rw-r--  2.0 unx     2690 b- defN 22-Nov-13 13:27 aos_prov/files/vm.xml
 -rw-rw-r--  2.0 unx      748 b- defN 22-Nov-13 13:27 aos_prov/utils/__init__.py
 -rw-rw-r--  2.0 unx     1649 b- defN 23-Apr-04 10:59 aos_prov/utils/common.py
 -rw-rw-r--  2.0 unx     2591 b- defN 22-Dec-01 17:44 aos_prov/utils/config.py
 -rw-rw-r--  2.0 unx      501 b- defN 22-Nov-13 13:27 aos_prov/utils/errors.py
 -rw-rw-r--  2.0 unx     1176 b- defN 22-Dec-01 17:44 aos_prov/utils/unit_certificate.py
 -rw-rw-r--  2.0 unx     7475 b- defN 23-Apr-04 10:59 aos_prov/utils/user_credentials.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-13 13:27 test/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-13 13:27 test/utils/__init__.py
 -rw-rw-r--  2.0 unx      642 b- defN 22-Dec-01 17:44 test/utils/test_config.py
 -rw-rw-r--  2.0 unx      632 b- defN 22-Dec-01 17:44 test/utils/test_unit_certificate.py
 -rw-rw-r--  2.0 unx      439 b- defN 22-Nov-13 13:27 test/utils/test_user_credentials.py
--rw-rw-r--  2.0 unx     2484 b- defN 23-May-22 15:57 aos_prov-4.0.2b2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-22 15:57 aos_prov-4.0.2b2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       48 b- defN 23-May-22 15:57 aos_prov-4.0.2b2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       14 b- defN 23-May-22 15:57 aos_prov-4.0.2b2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5880 b- defN 23-May-22 15:57 aos_prov-4.0.2b2.dist-info/RECORD
-59 files, 356114 bytes uncompressed, 58753 bytes compressed:  83.5%
+-rw-rw-r--  2.0 unx     2484 b- defN 23-May-23 16:49 aos_prov-4.0.2b3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-23 16:49 aos_prov-4.0.2b3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       48 b- defN 23-May-23 16:49 aos_prov-4.0.2b3.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       14 b- defN 23-May-23 16:49 aos_prov-4.0.2b3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5618 b- defN 23-May-23 16:49 aos_prov-4.0.2b3.dist-info/RECORD
+56 files, 346007 bytes uncompressed, 55094 bytes compressed:  84.1%
```

## zipnote {}

```diff
@@ -9,20 +9,14 @@
 
 Filename: aos_prov/commands/__init__.py
 Comment: 
 
 Filename: aos_prov/commands/command_provision.py
 Comment: 
 
-Filename: aos_prov/commands/command_vm.py
-Comment: 
-
-Filename: aos_prov/commands/command_vm_libvirt.py
-Comment: 
-
 Filename: aos_prov/commands/command_vm_multi_node_manage.py
 Comment: 
 
 Filename: aos_prov/commands/download.py
 Comment: 
 
 Filename: aos_prov/communication/__init__.py
@@ -120,17 +114,14 @@
 
 Filename: aos_prov/communication/unit/v4/generated/iamanager_pb2_grpc.py
 Comment: 
 
 Filename: aos_prov/files/1rootCA.crt
 Comment: 
 
-Filename: aos_prov/files/vm.xml
-Comment: 
-
 Filename: aos_prov/utils/__init__.py
 Comment: 
 
 Filename: aos_prov/utils/common.py
 Comment: 
 
 Filename: aos_prov/utils/config.py
@@ -156,23 +147,23 @@
 
 Filename: test/utils/test_unit_certificate.py
 Comment: 
 
 Filename: test/utils/test_user_credentials.py
 Comment: 
 
-Filename: aos_prov-4.0.2b2.dist-info/METADATA
+Filename: aos_prov-4.0.2b3.dist-info/METADATA
 Comment: 
 
-Filename: aos_prov-4.0.2b2.dist-info/WHEEL
+Filename: aos_prov-4.0.2b3.dist-info/WHEEL
 Comment: 
 
-Filename: aos_prov-4.0.2b2.dist-info/entry_points.txt
+Filename: aos_prov-4.0.2b3.dist-info/entry_points.txt
 Comment: 
 
-Filename: aos_prov-4.0.2b2.dist-info/top_level.txt
+Filename: aos_prov-4.0.2b3.dist-info/top_level.txt
 Comment: 
 
-Filename: aos_prov-4.0.2b2.dist-info/RECORD
+Filename: aos_prov-4.0.2b3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aos_prov/main.py

```diff
@@ -32,14 +32,15 @@
 _DEFAULT_USER_CERTIFICATE = str(Path.home() / '.aos' / 'security' / 'aos-user-oem.p12')
 
 logger = logging.getLogger(__name__)
 
 
 def _parse_args():
     parser = argparse.ArgumentParser(
+        prog='aos-prov',
         description="The board provisioning tool using gRPC protocol",
         epilog="Run 'aos-prov --help' for more information about commands, "
                "or 'aos-prov COMMAND --help' to see info about command about desired command")
 
     parser.add_argument(
         '-u',
         '--unit',
@@ -162,15 +163,16 @@
         default=_DEFAULT_USER_CERTIFICATE,
     )
 
     parser.add_argument(
         '-V',
         '--version',
         action='version',
-        version=f"%(prog)s {version('aos-prov')}")
+        version=f'%(prog)s {version("aos-prov")}',  # noqa: WPS323,WPS237
+    )
 
     download_command = sub_parser.add_parser(_COMMAND_DOWNLOAD, help='Download image')
     download_command.set_defaults(which=_COMMAND_DOWNLOAD)
     download_command.add_argument(
         '-a',
         '--address',
         dest='download_address',
```

## Comparing `aos_prov-4.0.2b2.dist-info/METADATA` & `aos_prov-4.0.2b3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aos-prov
-Version: 4.0.2b2
+Version: 4.0.2b3
 Summary: AosEdge Unit provisioning tool
 Author: EPAM Systems
 Author-email: support@aoscloud.io
 License: Apache License 2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

## Comparing `aos_prov-4.0.2b2.dist-info/RECORD` & `aos_prov-4.0.2b3.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 aos_prov/__init__.py,sha256=GG0w5d4OL0uOtGiHjbqIxaTR64BEYWYw1CULBI3cz-8,89
 aos_prov/actions.py,sha256=nFG7HDWRs9v8kpuztVyM3zXnYH6fVYi5qFmnb8QLBcQ,2842
-aos_prov/main.py,sha256=4z6XrPUXlc9UO_Pk-Gz0mhK7NhyMueAKWrWnvLRC4M8,7271
+aos_prov/main.py,sha256=T3Nbt8zmyro110-h9LmLP2Ji8z9MYB1FWZFoOzsSNmo,7325
 aos_prov/commands/__init__.py,sha256=GG0w5d4OL0uOtGiHjbqIxaTR64BEYWYw1CULBI3cz-8,89
 aos_prov/commands/command_provision.py,sha256=_q0hdHIntYiky7RIvG0rVIHqajzqD45nTriAnXLZpko,7501
-aos_prov/commands/command_vm.py,sha256=ASTlpDw95_4TqF5Lhi75SP03AAHLGy-gS86YZn1L3B8,4883
-aos_prov/commands/command_vm_libvirt.py,sha256=tynTeJIybqWNRjWYYJYnB-0HGyS4-KPZj_km3-JML3k,2326
 aos_prov/commands/command_vm_multi_node_manage.py,sha256=-_rjolNtBlVAu4UgA8VhX8U3vVA6PKIqeC2K_ofRq0w,9689
 aos_prov/commands/download.py,sha256=IltafRwLmlXz5JsCCTOpIFUTwP-g4KXZlPTJXTdR9kg,3799
 aos_prov/communication/__init__.py,sha256=g_G31XwUu8TLcWqYs29k7BIMKlsnQ_NS49zwy4o8ZPg,89
 aos_prov/communication/cloud/__init__.py,sha256=GG0w5d4OL0uOtGiHjbqIxaTR64BEYWYw1CULBI3cz-8,89
 aos_prov/communication/cloud/cloud_api.py,sha256=hvCKoqQzdJ3RIw1uYYWoeaADWFM6W3BCU7nDKF9nLA0,8552
 aos_prov/communication/unit/__init__.py,sha256=g_G31XwUu8TLcWqYs29k7BIMKlsnQ_NS49zwy4o8ZPg,89
 aos_prov/communication/unit/v0/__init__.py,sha256=g_G31XwUu8TLcWqYs29k7BIMKlsnQ_NS49zwy4o8ZPg,89
@@ -36,24 +34,23 @@
 aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2_grpc.py,sha256=lW-qgXE-T05_Xgiu-ejHdh-08ushwoCGExYYwp-5iC0,12904
 aos_prov/communication/unit/v4/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aos_prov/communication/unit/v4/unit_communication_v4.py,sha256=jSwFMEv2JbnIG_rcwU4Rbz1I9viGB1VfvaxSZ3o_AAo,9592
 aos_prov/communication/unit/v4/generated/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aos_prov/communication/unit/v4/generated/iamanager_pb2.py,sha256=VNNHm-5L2JX8rQkv-Sidgzlu_wus98Tjw1v44JrEzq8,18433
 aos_prov/communication/unit/v4/generated/iamanager_pb2_grpc.py,sha256=pOin6Yl556SQgo1J_l-lTmypm8TeMx__U5kArMyum9A,33405
 aos_prov/files/1rootCA.crt,sha256=ToJxPHzLkJQmYdXNPVJA3ACBf7uv0THJK8ypR18etws,2705
-aos_prov/files/vm.xml,sha256=QMguS8KGVurCJgQmkjCIyZfU4CPs8-rmIlX-xwVEWYI,2690
 aos_prov/utils/__init__.py,sha256=FXJpTks2FyzbRUI3vSk-bRK1EPpQfyc2mC1OCMmPnw4,748
 aos_prov/utils/common.py,sha256=XFuewA2HYRo0MzFkZrs0j-Jcs3HUiSWLgQhUf1uB-u4,1649
 aos_prov/utils/config.py,sha256=agWFGFFBj2Y0icjCVKLCVR2KsFxgKaHVl0ZPLoJjDZM,2591
 aos_prov/utils/errors.py,sha256=0pAtbvFDd6cBKbaqexXmP0IfJu8rrY-i-bmv32ogtZI,501
 aos_prov/utils/unit_certificate.py,sha256=WYhSiQOuK7OmAK4aTWpaQRxjufJ3WKdHXpmNJSRwhkY,1176
 aos_prov/utils/user_credentials.py,sha256=4916YJfDQLkOIs3hynjftlf2c10L47jToLkkSH3iyhg,7475
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/utils/test_config.py,sha256=696gxCTKBDuXMe3aKd3ucGsx8qZItMGNlp53NgczEOI,642
 test/utils/test_unit_certificate.py,sha256=hh6fN3qCeZbizfgzF1V5DEYUSuCxzSNDq1qI7YrpZqs,632
 test/utils/test_user_credentials.py,sha256=CGjW9zhm3NxGP3JXTMI8p1gupqSWozbWHUCou7EUUw0,439
-aos_prov-4.0.2b2.dist-info/METADATA,sha256=JxVQNo2lC3TywdL5shNv8AYN5WhuAR1qaPuH7b2jfbk,2484
-aos_prov-4.0.2b2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-aos_prov-4.0.2b2.dist-info/entry_points.txt,sha256=fkaEe75Sm0Z8TQtunDs5iah-ilcOouPDsCnNyQaZg18,48
-aos_prov-4.0.2b2.dist-info/top_level.txt,sha256=2vX7skeG9R6AfX6SK6xeAwN_SW1w1Jub2V2W_3u8Prc,14
-aos_prov-4.0.2b2.dist-info/RECORD,,
+aos_prov-4.0.2b3.dist-info/METADATA,sha256=S16lPHS-92Bpg16plXCT_SGFua7Vq4fg2vGwh9R5DLY,2484
+aos_prov-4.0.2b3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+aos_prov-4.0.2b3.dist-info/entry_points.txt,sha256=fkaEe75Sm0Z8TQtunDs5iah-ilcOouPDsCnNyQaZg18,48
+aos_prov-4.0.2b3.dist-info/top_level.txt,sha256=2vX7skeG9R6AfX6SK6xeAwN_SW1w1Jub2V2W_3u8Prc,14
+aos_prov-4.0.2b3.dist-info/RECORD,,
```

