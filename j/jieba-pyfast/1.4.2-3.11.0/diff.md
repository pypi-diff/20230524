# Comparing `tmp/jieba_pyfast-1.4.2-cp311-cp311-macosx_12_0_x86_64.whl.zip` & `tmp/jieba_pyfast-3.11.0-cp311-cp311-macosx_12_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5099395 bytes, number of entries: 30
+Zip file size: 5099403 bytes, number of entries: 30
 -rwxr-xr-x  2.0 unx    42680 b- defN 80-Jan-01 00:00 _jieba_fast_functions_py3.cpython-311-darwin.so
 -rwxr-xr-x  2.0 unx    19276 b- defN 80-Jan-01 00:00 jieba_pyfast/__init__.py
 -rw-r--r--  2.0 unx     3921 b- defN 80-Jan-01 00:00 jieba_pyfast/jieba_fast_functions_py3.py
 -rwxr-xr-x  2.0 unx      920 b- defN 80-Jan-01 00:00 jieba_pyfast/_compat.py
 -rwxr-xr-x  2.0 unx  5071852 b- defN 80-Jan-01 00:00 jieba_pyfast/dict.txt
 -rw-r--r--  2.0 unx     9734 b- defN 80-Jan-01 00:00 jieba_pyfast/source/jieba_fast_functions_wrap_py3.i
 -rw-r--r--  2.0 unx     3921 b- defN 80-Jan-01 00:00 jieba_pyfast/source/jieba_fast_functions_py3.py
@@ -21,12 +21,12 @@
 -rwxr-xr-x  2.0 unx  1275441 b- defN 80-Jan-01 00:00 jieba_pyfast/finalseg/prob_emit.p
 -rwxr-xr-x  2.0 unx      259 b- defN 80-Jan-01 00:00 jieba_pyfast/finalseg/prob_trans.py
 -rwxr-xr-x  2.0 unx  1356989 b- defN 80-Jan-01 00:00 jieba_pyfast/finalseg/prob_emit.py
 -rwxr-xr-x  2.0 unx     2922 b- defN 80-Jan-01 00:00 jieba_pyfast/finalseg/__init__.py
 -rwxr-xr-x  2.0 unx      260 b- defN 80-Jan-01 00:00 jieba_pyfast/finalseg/prob_trans.p
 -rw-r--r--  2.0 unx     3921 b- defN 80-Jan-01 00:00 jieba_pyfast/finalseg/jieba_fast_functions_py3.py
 -rwxr-xr-x  2.0 unx      109 b- defN 80-Jan-01 00:00 jieba_pyfast/finalseg/prob_start.py
--rw-r--r--  2.0 unx     2773 b- defN 23-May-24 09:16 jieba_pyfast-1.4.2.dist-info/RECORD
--rwxr-xr-x  2.0 unx     1075 b- defN 80-Jan-01 00:00 jieba_pyfast-1.4.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      107 b- defN 80-Jan-01 00:00 jieba_pyfast-1.4.2.dist-info/WHEEL
--rw-r--r--  2.0 unx      809 b- defN 80-Jan-01 00:00 jieba_pyfast-1.4.2.dist-info/METADATA
-30 files, 18480795 bytes uncompressed, 5094963 bytes compressed:  72.4%
+-rw-r--r--  2.0 unx     2777 b- defN 23-May-24 09:17 jieba_pyfast-3.11.0.dist-info/RECORD
+-rwxr-xr-x  2.0 unx     1075 b- defN 80-Jan-01 00:00 jieba_pyfast-3.11.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      107 b- defN 80-Jan-01 00:00 jieba_pyfast-3.11.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      810 b- defN 80-Jan-01 00:00 jieba_pyfast-3.11.0.dist-info/METADATA
+30 files, 18480800 bytes uncompressed, 5094963 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -72,20 +72,20 @@
 
 Filename: jieba_pyfast/finalseg/jieba_fast_functions_py3.py
 Comment: 
 
 Filename: jieba_pyfast/finalseg/prob_start.py
 Comment: 
 
-Filename: jieba_pyfast-1.4.2.dist-info/RECORD
+Filename: jieba_pyfast-3.11.0.dist-info/RECORD
 Comment: 
 
-Filename: jieba_pyfast-1.4.2.dist-info/LICENSE
+Filename: jieba_pyfast-3.11.0.dist-info/LICENSE
 Comment: 
 
-Filename: jieba_pyfast-1.4.2.dist-info/WHEEL
+Filename: jieba_pyfast-3.11.0.dist-info/WHEEL
 Comment: 
 
-Filename: jieba_pyfast-1.4.2.dist-info/METADATA
+Filename: jieba_pyfast-3.11.0.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## _jieba_fast_functions_py3.cpython-311-darwin.so

### llvm-readobj --symbols {}

```diff
@@ -402,15 +402,15 @@
   Symbol {
     Name: /Users/runner/work/jieba_pyfast/jieba_pyfast/build/temp.macosx-10.9-x86_64-cpython-311/jieba_pyfast/source/jieba_fast_functions_wrap_py3_wrap.o (2296)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x646DD5CC
+    Value: 0x646DD615
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
```

### x86_64

 * *Format-specific differences are supported for this file format but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Mach-O 64-bit x86_64 bundle, flags:<NOUNDEFS|DYLDLINK|TWOLEVEL>*

```diff
@@ -2202,15 +2202,15 @@
 00008990: 604b 0000 0000 0000 2f08 0000 0e0c 0000  `K....../.......
 000089a0: 684b 0000 0000 0000 4708 0000 0e0c 0000  hK......G.......
 000089b0: 704b 0000 0000 0000 7008 0000 0e0c 0000  pK......p.......
 000089c0: 084d 0000 0000 0000 0100 0000 6401 0000  .M..........d...
 000089d0: 0000 0000 0000 0000 9108 0000 6400 0000  ............d...
 000089e0: 0000 0000 0000 0000 d308 0000 6400 0000  ............d...
 000089f0: 0000 0000 0000 0000 f808 0000 6603 0100  ............f...
-00008a00: ccd5 6d64 0000 0000 0100 0000 2e01 0000  ..md............
+00008a00: 15d6 6d64 0000 0000 0100 0000 2e01 0000  ..md............
 00008a10: e00b 0000 0000 0000 8809 0000 2401 0000  ............$...
 00008a20: e00b 0000 0000 0000 8f09 0000 8400 0000  ................
 00008a30: 0000 0000 0000 0000 0100 0000 2400 0000  ............$...
 00008a40: 5002 0000 0000 0000 0100 0000 4e01 0000  P...........N...
 00008a50: e00b 0000 0000 0000 0100 0000 2e01 0000  ................
 00008a60: 300e 0000 0000 0000 c809 0000 2401 0000  0...........$...
 00008a70: 300e 0000 0000 0000 0100 0000 2400 0000  0...........$...
```

## Comparing `jieba_pyfast-1.4.2.dist-info/RECORD` & `jieba_pyfast-3.11.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-_jieba_fast_functions_py3.cpython-311-darwin.so,sha256=Oz7qHDTsEscjFO3iY2xH7mdMvF24o3BwaezStnMNpTk,42680
+_jieba_fast_functions_py3.cpython-311-darwin.so,sha256=bZoZZEfbs-Xyh-FUDtYHYXJ2_-RAeIihUmhAjTb_QBk,42680
 jieba_pyfast/__init__.py,sha256=47Yfo_TIAC_1cJTkUNBn6c0H8aJYOT3nW4TyE1o85_w,19276
 jieba_pyfast/jieba_fast_functions_py3.py,sha256=NqE0vCLDZ-SVtyymCwg_So57k5zdY0yNtLEvfDeVGX8,3921
 jieba_pyfast/_compat.py,sha256=oCmqNk4iWEKbEdljCYWwkITuSaYKNcSvZWEK9tXMLQ8,920
 jieba_pyfast/dict.txt,sha256=cZfDIR3dmJYrA2zfQDJNHqK_qhK9Ao5o-qcBEaiOEqg,5071852
 jieba_pyfast/source/jieba_fast_functions_wrap_py3.i,sha256=t8Yh97xh7UiDBnE2KoLpID7f5sTLz_Qfs9I1NJgKzAw,9734
 jieba_pyfast/source/jieba_fast_functions_py3.py,sha256=NqE0vCLDZ-SVtyymCwg_So57k5zdY0yNtLEvfDeVGX8,3921
 jieba_pyfast/source/jieba_fast_functions_wrap_py3_wrap.c,sha256=h6ljTWP5Bg2_a_os_8L29MrbKbaMCt3Z3xqB6NGG14w,124414
@@ -20,11 +20,11 @@
 jieba_pyfast/finalseg/prob_emit.p,sha256=Hh0dg1sMd9I0rKpq-iOhP_zll6KVvg16Hs5qDUQNzwg,1275441
 jieba_pyfast/finalseg/prob_trans.py,sha256=1SuLCLa4mvt5Uhy86ujw3K_2EO65YTosY9K8C1piKzQ,259
 jieba_pyfast/finalseg/prob_emit.py,sha256=OPXlKBwRcLdL7CuMnqbFb_Uvavk59BeoKDCHtldUIDg,1356989
 jieba_pyfast/finalseg/__init__.py,sha256=zIUsscOvj6ZYW32oxHtF6bVbIx5Aw1kS13lK4KC5-yw,2922
 jieba_pyfast/finalseg/prob_trans.p,sha256=6n9QFi_6AdtJc8eoEgs8AjP7xYGfwNYXUTU18fLH_tw,260
 jieba_pyfast/finalseg/jieba_fast_functions_py3.py,sha256=NqE0vCLDZ-SVtyymCwg_So57k5zdY0yNtLEvfDeVGX8,3921
 jieba_pyfast/finalseg/prob_start.py,sha256=raVrh2nR6DDJZPJ485karIGFjA7fpxo8iRhvFX74YRg,109
-jieba_pyfast-1.4.2.dist-info/RECORD,,
-jieba_pyfast-1.4.2.dist-info/LICENSE,sha256=GLoJhIOfhYU7Kfra-ZL326j9DKD76uNN4rhzUiLcejc,1075
-jieba_pyfast-1.4.2.dist-info/WHEEL,sha256=L9j5kZliY_RmhQpA0BNpxXPfCg-0_bW_DSgAkuvMplg,107
-jieba_pyfast-1.4.2.dist-info/METADATA,sha256=_CNR-CRSQEChPW5Gm48iwIn-iO0QoKa_dN3uEC1bmGs,809
+jieba_pyfast-3.11.0.dist-info/RECORD,,
+jieba_pyfast-3.11.0.dist-info/LICENSE,sha256=GLoJhIOfhYU7Kfra-ZL326j9DKD76uNN4rhzUiLcejc,1075
+jieba_pyfast-3.11.0.dist-info/WHEEL,sha256=L9j5kZliY_RmhQpA0BNpxXPfCg-0_bW_DSgAkuvMplg,107
+jieba_pyfast-3.11.0.dist-info/METADATA,sha256=DOTmMoiFIHhcnvAnCPSEc-QUs1gSVBYVAWLibjfR2Ng,810
```

## Comparing `jieba_pyfast-1.4.2.dist-info/LICENSE` & `jieba_pyfast-3.11.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jieba_pyfast-1.4.2.dist-info/METADATA` & `jieba_pyfast-3.11.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jieba-pyfast
-Version: 1.4.2
+Version: 3.11.0
 Summary: Tokenize Chinese characters
 License: MIT
 Author: snapADDY GmbH
 Author-email: info@snapaddy.com
 Requires-Python: ==3.11.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

