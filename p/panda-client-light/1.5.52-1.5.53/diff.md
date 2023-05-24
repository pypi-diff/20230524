# Comparing `tmp/panda_client_light-1.5.52-py2.py3-none-any.whl.zip` & `tmp/panda_client_light-1.5.53-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 155939 bytes, number of entries: 36
+Zip file size: 155998 bytes, number of entries: 36
 -rw-r--r--  2.0 unx    63390 b- defN 20-Feb-02 00:00 pandaclient/AthenaUtils.py
 -rw-r--r--  2.0 unx     2276 b- defN 20-Feb-02 00:00 pandaclient/BookConfig.py
 -rwxr-xr-x  2.0 unx    32382 b- defN 20-Feb-02 00:00 pandaclient/BookGUI.py
 -rwxr-xr-x  2.0 unx    62375 b- defN 20-Feb-02 00:00 pandaclient/Client.py
 -rwxr-xr-x  2.0 unx     3118 b- defN 20-Feb-02 00:00 pandaclient/FileSpec.py
 -rw-r--r--  2.0 unx     3468 b- defN 20-Feb-02 00:00 pandaclient/Group_argparse.py
 -rwxr-xr-x  2.0 unx    27030 b- defN 20-Feb-02 00:00 pandaclient/JobSpec.py
@@ -16,23 +16,23 @@
 -rw-r--r--  2.0 unx       27 b- defN 20-Feb-02 00:00 pandaclient/PandaToolsPkgInfo.py
 -rw-r--r--  2.0 unx    15441 b- defN 20-Feb-02 00:00 pandaclient/ParseJobXML.py
 -rw-r--r--  2.0 unx   104912 b- defN 20-Feb-02 00:00 pandaclient/PathenaScript.py
 -rw-r--r--  2.0 unx    11704 b- defN 20-Feb-02 00:00 pandaclient/PchainScript.py
 -rwxr-xr-x  2.0 unx      247 b- defN 20-Feb-02 00:00 pandaclient/PcontainerScript.py
 -rw-r--r--  2.0 unx    24834 b- defN 20-Feb-02 00:00 pandaclient/PdbUtils.py
 -rw-r--r--  2.0 unx    27474 b- defN 20-Feb-02 00:00 pandaclient/PhpoScript.py
--rw-r--r--  2.0 unx   104361 b- defN 20-Feb-02 00:00 pandaclient/PrunScript.py
+-rw-r--r--  2.0 unx   104663 b- defN 20-Feb-02 00:00 pandaclient/PrunScript.py
 -rw-r--r--  2.0 unx    32754 b- defN 20-Feb-02 00:00 pandaclient/PsubUtils.py
 -rwxr-xr-x  2.0 unx        0 b- defN 20-Feb-02 00:00 pandaclient/__init__.py
 -rw-r--r--  2.0 unx     1862 b- defN 20-Feb-02 00:00 pandaclient/example_task.py
 -rw-r--r--  2.0 unx     2055 b- defN 20-Feb-02 00:00 pandaclient/idds_api.py
 -rw-r--r--  2.0 unx     4163 b- defN 20-Feb-02 00:00 pandaclient/localSpecs.py
 -rw-r--r--  2.0 unx    10226 b- defN 20-Feb-02 00:00 pandaclient/openidc_utils.py
 -rw-r--r--  2.0 unx    10528 b- defN 20-Feb-02 00:00 pandaclient/panda_api.py
 -rw-r--r--  2.0 unx     4975 b- defN 20-Feb-02 00:00 pandaclient/panda_gui.py
 -rw-r--r--  2.0 unx     4025 b- defN 20-Feb-02 00:00 pandaclient/panda_jupyter.py
 -rw-r--r--  2.0 unx     7280 b- defN 20-Feb-02 00:00 pandaclient/pcontainer_core.py
 -rw-r--r--  2.0 unx     4281 b- defN 20-Feb-02 00:00 pandaclient/queryPandaMonUtils.py
-?rw-r--r--  2.0 unx     1758 b- defN 20-Feb-02 00:00 panda_client_light-1.5.52.dist-info/METADATA
-?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 panda_client_light-1.5.52.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2992 b- defN 20-Feb-02 00:00 panda_client_light-1.5.52.dist-info/RECORD
-36 files, 657974 bytes uncompressed, 151219 bytes compressed:  77.0%
+?rw-r--r--  2.0 unx     1758 b- defN 20-Feb-02 00:00 panda_client_light-1.5.53.dist-info/METADATA
+?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 panda_client_light-1.5.53.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2992 b- defN 20-Feb-02 00:00 panda_client_light-1.5.53.dist-info/RECORD
+36 files, 658276 bytes uncompressed, 151278 bytes compressed:  77.0%
```

## zipnote {}

```diff
@@ -93,17 +93,17 @@
 
 Filename: pandaclient/pcontainer_core.py
 Comment: 
 
 Filename: pandaclient/queryPandaMonUtils.py
 Comment: 
 
-Filename: panda_client_light-1.5.52.dist-info/METADATA
+Filename: panda_client_light-1.5.53.dist-info/METADATA
 Comment: 
 
-Filename: panda_client_light-1.5.52.dist-info/WHEEL
+Filename: panda_client_light-1.5.53.dist-info/WHEEL
 Comment: 
 
-Filename: panda_client_light-1.5.52.dist-info/RECORD
+Filename: panda_client_light-1.5.53.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pandaclient/PandaToolsPkgInfo.py

```diff
@@ -1 +1 @@
-release_version = "1.5.52"
+release_version = "1.5.53"
```

## pandaclient/PrunScript.py

```diff
@@ -1487,38 +1487,46 @@
                  'value': '-l ${LIB}',
                  },
                 ]
     # output
     if options.outputs != '':
         outMap = {}
         dsSuffix = []
+        dsIndex = 0
         for tmpLFN in options.outputs.split(','):
             tmpDsSuffix = ''
             if ':' in tmpLFN:
-                tmpDsSuffix,tmpLFN = tmpLFN.split(':')
+                tmpDsSuffix, tmpLFN = tmpLFN.split(':')
                 if tmpDsSuffix in dsSuffix:
-                    tmpErrMsg  = "dataset name suffix '%s' is used for multiple files in --outputs. " % tmpDsSuffix
+                    tmpErrMsg = "dataset name suffix '%s' is used for multiple files in --outputs. " % tmpDsSuffix
                     tmpErrMsg += 'each output must have a unique suffix.'
                     tmpLog.error(tmpErrMsg)
                     sys.exit(EC_Config)
                 dsSuffix.append(tmpDsSuffix)
-            tmpNewLFN = tmpLFN
-            # change * to XYZ and add .tgz
-            if '*' in tmpNewLFN:
-                tmpNewLFN = tmpNewLFN.replace('*','XYZ')
-                tmpNewLFN += '.tgz'
-            if len(outDatasetName.split('.')) > 2:
-                lfn = '{0}.{1}'.format(*outDatasetName.split('.')[:2])
+            if tmpLFN.startswith('regex|'):
+                # regex
+                lfn = tmpLFN
+                if not tmpDsSuffix:
+                    tmpDsSuffix = dsIndex
+                    dsIndex += 1
             else:
-                lfn = outDatasetName[:-1]
-            if options.addNthFieldOfInDSToLFN != '' or options.addNthFieldOfInFileToLFN != '':
-                lfn += '${MIDDLENAME}'
-            lfn += '.$JEDITASKID._${{SN/P}}.{0}'.format(tmpNewLFN)
-            if tmpDsSuffix == '':
-                tmpDsSuffix = tmpNewLFN
+                tmpNewLFN = tmpLFN
+                # change * to XYZ and add .tgz
+                if '*' in tmpNewLFN:
+                    tmpNewLFN = tmpNewLFN.replace('*','XYZ')
+                    tmpNewLFN += '.tgz'
+                if len(outDatasetName.split('.')) > 2:
+                    lfn = '{0}.{1}'.format(*outDatasetName.split('.')[:2])
+                else:
+                    lfn = outDatasetName[:-1]
+                if options.addNthFieldOfInDSToLFN != '' or options.addNthFieldOfInFileToLFN != '':
+                    lfn += '${MIDDLENAME}'
+                lfn += '.$JEDITASKID._${{SN/P}}.{0}'.format(tmpNewLFN)
+                if tmpDsSuffix == '':
+                    tmpDsSuffix = tmpNewLFN
             dataset = '{0}_{1}/'.format(outDatasetName[:-1],tmpDsSuffix)
             taskParamMap['jobParameters'] += MiscUtils.makeJediJobParam(lfn,dataset,'output',hidden=True,
                                                                         destination=options.destSE,
                                                                         token=options.spaceToken,
                                                                         allowNoOutput=options.allowNoOutput)
             outMap[tmpLFN] = lfn
         if options.loadXML:
```

## Comparing `panda_client_light-1.5.52.dist-info/METADATA` & `panda_client_light-1.5.53.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda-client-light
-Version: 1.5.52
+Version: 1.5.53
 Summary: PanDA Client Package installed on PanDA server
 Project-URL: Homepage, https://panda-wms.readthedocs.io/en/latest/
 Author-email: PanDA Team <atlas-adc-panda@cern.ch>
 License-Expression: Apache-2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

## Comparing `panda_client_light-1.5.52.dist-info/RECORD` & `panda_client_light-1.5.53.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 pandaclient/LocalJobSpec.py,sha256=rVMgk4KVhMY1hjWnsaIL9cWVAZMEKVOnE4vQqz7cHWU,13691
 pandaclient/LocalJobsetSpec.py,sha256=nYQMhKrbCtzm68ZWnEXCs_-mWvATm9XClm514aJ-7cU,11007
 pandaclient/MiscUtils.py,sha256=EsYggBpqtszpTKtp4Erc9Xe6Dr42VvqloFc7_T-U1KY,9856
 pandaclient/MyproxyUtils.py,sha256=7eNIdr6Vt8phcW5FVbt5mZ10I4tZH0n-xAuKBk-GcQI,15025
 pandaclient/PBookCore.py,sha256=134Ubc_RG2SMjmgeNs6s_op-3zpyFFOcNLMqd89f8bs,17679
 pandaclient/PBookScript.py,sha256=zgH4LHQeXkyeM1rxtQ64KN0lFDM3wAqpsRf5QVYzp_I,19506
 pandaclient/PLogger.py,sha256=1R0xMlWsHLdptyb-ewt_o6NVveK07ENmKBoE-NKtyJw,1167
-pandaclient/PandaToolsPkgInfo.py,sha256=cZ5KnFHi6CYeZ7YFoEevFbfF-qMhKA6gZ4I1629WIyU,27
+pandaclient/PandaToolsPkgInfo.py,sha256=lk3O1j4TmGnWuqEsTuHGncC6Njj5Wf2J5rax7S6lQMA,27
 pandaclient/ParseJobXML.py,sha256=GWdiTXhRZOVIqxUT4laZZ13WQ5HZs4V2PgichtyQ4Ec,15441
 pandaclient/PathenaScript.py,sha256=2KCZMps7gDhkFFJA0vE1f1eS5XBLQl42UwXciIphu3A,104912
 pandaclient/PchainScript.py,sha256=JuDJoegkS82Yggo7_szQVEuePgYp5NHp-_vmxOPovW8,11704
 pandaclient/PcontainerScript.py,sha256=J7EiyUfBmMPHXvdwbPE7t9redP6JhdWmCZa3Yg27fRQ,247
 pandaclient/PdbUtils.py,sha256=TNsmCb___D1JevvocLWMUUKajA10Zo62VjdqDx4-Law,24834
 pandaclient/PhpoScript.py,sha256=SgAFlX4VJSx24A4z4fH6sTwka1CJD2_CAbOxrgVXrwU,27474
-pandaclient/PrunScript.py,sha256=4Puim5IHHs7ByVJq7t-dYQ6E2uFahXcHIHryXbz9gw4,104361
+pandaclient/PrunScript.py,sha256=lRGKiskp0USbXv9q4-z3BXLplOnzp4UXjW95QQs9xwU,104663
 pandaclient/PsubUtils.py,sha256=uZ1AZUWDGMOGOPGkUmhyH_hTlmKZO593djgsSYwQrJQ,32754
 pandaclient/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pandaclient/example_task.py,sha256=8bMua7YPKI8Eh-UgyZJVDUT3Hhv35FDyQ_eo7KW2PRk,1862
 pandaclient/idds_api.py,sha256=2khWVag3GDHQEkfqZvnuq0Qcc_hGsOCknglHSS9mudY,2055
 pandaclient/localSpecs.py,sha256=Cx9ZNTaOvFIWbk_u9f7Xg9s_4zJdhyksAeMWNwHKbt0,4163
 pandaclient/openidc_utils.py,sha256=nV4cq1n9jDgGXn8FqoERBDHDnFEJMTYuZ7HqIbWKqaU,10226
 pandaclient/panda_api.py,sha256=eNLVvzBiqjANFbqED_AX-K3UI7tASl0fHml8SAMuIkw,10528
 pandaclient/panda_gui.py,sha256=5nW5RsYaXuDcgsxj8SCXvnrZrC117bg70OBZRXqjIvY,4975
 pandaclient/panda_jupyter.py,sha256=buiC8kGSA_KCaZ9TF6XLbfi0hwHi9d6_npDXitRlkCA,4025
 pandaclient/pcontainer_core.py,sha256=k_HjWhLtGPVtnRgK1yaMzEY0XgiBz3XHZt-rVoLf04c,7280
 pandaclient/queryPandaMonUtils.py,sha256=7NqvwjMAgpJC9re4qKe7W6Zn9E7CRzyL1yHmp9yndsg,4281
-panda_client_light-1.5.52.dist-info/METADATA,sha256=WqszqjijGuSGYquRVegP-TkQb4n4PptDKjjoOeXRSMQ,1758
-panda_client_light-1.5.52.dist-info/WHEEL,sha256=BnTM96A0yHS39SE-waRX_LK6xllJtQJhpP4G4cCnPIA,105
-panda_client_light-1.5.52.dist-info/RECORD,,
+panda_client_light-1.5.53.dist-info/METADATA,sha256=HD4aDfZn0WVb9CnQBFXUAHt3V_gxyHzXD1C-hNCnyDE,1758
+panda_client_light-1.5.53.dist-info/WHEEL,sha256=BnTM96A0yHS39SE-waRX_LK6xllJtQJhpP4G4cCnPIA,105
+panda_client_light-1.5.53.dist-info/RECORD,,
```

