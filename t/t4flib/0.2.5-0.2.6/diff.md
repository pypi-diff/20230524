# Comparing `tmp/t4flib-0.2.5-py2.py3-none-any.whl.zip` & `tmp/t4flib-0.2.6-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 11061 bytes, number of entries: 12
+Zip file size: 11060 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-11 18:20 t4flib/__init__.py
 -rw-rw-r--  2.0 unx      892 b- defN 23-May-17 17:25 t4flib/config.py
 -rw-rw-r--  2.0 unx      971 b- defN 23-May-17 15:49 t4flib/data_helper.py
 -rw-rw-r--  2.0 unx     6145 b- defN 23-May-17 15:49 t4flib/file_helper.py
--rw-rw-r--  2.0 unx     5700 b- defN 23-May-22 13:49 t4flib/filetransfer_helper.py
+-rw-rw-r--  2.0 unx     5621 b- defN 23-May-22 15:34 t4flib/filetransfer_helper.py
 -rw-rw-r--  2.0 unx     7420 b- defN 23-May-17 15:49 t4flib/functional_helper.py
 -rw-rw-r--  2.0 unx     3235 b- defN 23-May-17 15:49 t4flib/gcloud_helper.py
 -rw-rw-r--  2.0 unx      876 b- defN 23-May-17 15:14 t4flib/log_helper.py
--rw-rw-r--  2.0 unx     1747 b- defN 23-May-22 14:02 t4flib-0.2.5.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-May-22 14:02 t4flib-0.2.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-May-22 14:02 t4flib-0.2.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      919 b- defN 23-May-22 14:02 t4flib-0.2.5.dist-info/RECORD
-12 files, 28022 bytes uncompressed, 9529 bytes compressed:  66.0%
+-rw-rw-r--  2.0 unx     1747 b- defN 23-May-22 15:47 t4flib-0.2.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-May-22 15:47 t4flib-0.2.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-22 15:47 t4flib-0.2.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      919 b- defN 23-May-22 15:47 t4flib-0.2.6.dist-info/RECORD
+12 files, 27943 bytes uncompressed, 9528 bytes compressed:  65.9%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: t4flib/gcloud_helper.py
 Comment: 
 
 Filename: t4flib/log_helper.py
 Comment: 
 
-Filename: t4flib-0.2.5.dist-info/METADATA
+Filename: t4flib-0.2.6.dist-info/METADATA
 Comment: 
 
-Filename: t4flib-0.2.5.dist-info/WHEEL
+Filename: t4flib-0.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: t4flib-0.2.5.dist-info/top_level.txt
+Filename: t4flib-0.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: t4flib-0.2.5.dist-info/RECORD
+Filename: t4flib-0.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## t4flib/filetransfer_helper.py

```diff
@@ -114,15 +114,15 @@
             log_f.debug(f'{ft_flow_to_send.path_to_get_file}/{ft_flow_to_send.filemask}')
 
             files = get_all_file_by_filemask(ft_flow_to_send.path_to_get_file, ft_flow_to_send.filemask)
             if len(files) == 0:
                 log_f.warning('Pas de fichier trouvé')
                 continue
 
-            for file in get_all_file_by_filemask(ft_flow_to_send.path_to_get_file, ft_flow_to_send.filemask):
+            for file in files:
 
                 shutil.copy(str(file.absolute()), ft_flow_to_send.path_out)
 
                 body_request = json.dumps({
                     "flow": ft_flow_to_send.flow_name,
                     "userId": ft_flow_to_send.server,
                     "authKey": ft_flow_to_send.ft_key,
```

## Comparing `t4flib-0.2.5.dist-info/METADATA` & `t4flib-0.2.6.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t4flib
-Version: 0.2.5
+Version: 0.2.6
 Summary: Librairie de fonction utiles pour T4F
 Home-page: http://gitlab.dev.fr.auchan.com/tech4finance/t4flib.git
 Author: Corentin DEVROUETE
 Author-email: cdevrouete@advanced-schema.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `t4flib-0.2.5.dist-info/RECORD` & `t4flib-0.2.6.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 t4flib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 t4flib/config.py,sha256=fHt2THXtajPzzV_gnHPZNVmez09ODLfIFrt4cTXgZsE,892
 t4flib/data_helper.py,sha256=SdKdv2U1EXtHJcfEff_I8zIlMWv56-xLZqczAw4kOUU,971
 t4flib/file_helper.py,sha256=NYIgOrA1iJBUcodtaRlDIsIHoivonLme4PmFZB1nQLw,6145
-t4flib/filetransfer_helper.py,sha256=8dL9dqJ_Kgory2nQ2Hoexv2Xw1IqBFFneEr-I7tS714,5700
+t4flib/filetransfer_helper.py,sha256=CkWlCJe5E_G0iovU2Jvm5ixB94RYl-lmAid4gEiDAe0,5621
 t4flib/functional_helper.py,sha256=CfbwrMufVRwCQNg9us9tujS3oeCmxql18vmo7B5lUAI,7420
 t4flib/gcloud_helper.py,sha256=sy5EpA2iVlcNlveP77N3iUCERNZXabSVOOcz8rifO6I,3235
 t4flib/log_helper.py,sha256=pu_y3m7iHWpkgYnxLYAlQjWjqknMGDcCDjHV6w4YYDc,876
-t4flib-0.2.5.dist-info/METADATA,sha256=pPB8jH81zrCNkX0-KH_B0pgQttcePVNTY4YWp517uH8,1747
-t4flib-0.2.5.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-t4flib-0.2.5.dist-info/top_level.txt,sha256=-05r3tdNDBMHneiATbWVqDQI7djLF9N83J6mAMcxbp8,7
-t4flib-0.2.5.dist-info/RECORD,,
+t4flib-0.2.6.dist-info/METADATA,sha256=JEZAnuuYOV-2vEEmbCJFRxRtEpViBYDTxJVsCMADfjU,1747
+t4flib-0.2.6.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+t4flib-0.2.6.dist-info/top_level.txt,sha256=-05r3tdNDBMHneiATbWVqDQI7djLF9N83J6mAMcxbp8,7
+t4flib-0.2.6.dist-info/RECORD,,
```

