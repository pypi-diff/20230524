# Comparing `tmp/jieba_pyfast-1.4.1-cp311-cp311-macosx_12_0_x86_64.whl.zip` & `tmp/jieba_pyfast-1.4.2-cp311-cp311-macosx_12_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5099402 bytes, number of entries: 30
+Zip file size: 5099395 bytes, number of entries: 30
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
--rw-r--r--  2.0 unx     2773 b- defN 22-Dec-19 13:09 jieba_pyfast-1.4.1.dist-info/RECORD
--rwxr-xr-x  2.0 unx     1075 b- defN 80-Jan-01 00:00 jieba_pyfast-1.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      107 b- defN 80-Jan-01 00:00 jieba_pyfast-1.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx      817 b- defN 80-Jan-01 00:00 jieba_pyfast-1.4.1.dist-info/METADATA
-30 files, 18480803 bytes uncompressed, 5094970 bytes compressed:  72.4%
+-rw-r--r--  2.0 unx     2773 b- defN 23-May-24 09:16 jieba_pyfast-1.4.2.dist-info/RECORD
+-rwxr-xr-x  2.0 unx     1075 b- defN 80-Jan-01 00:00 jieba_pyfast-1.4.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      107 b- defN 80-Jan-01 00:00 jieba_pyfast-1.4.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      809 b- defN 80-Jan-01 00:00 jieba_pyfast-1.4.2.dist-info/METADATA
+30 files, 18480795 bytes uncompressed, 5094963 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -72,20 +72,20 @@
 
 Filename: jieba_pyfast/finalseg/jieba_fast_functions_py3.py
 Comment: 
 
 Filename: jieba_pyfast/finalseg/prob_start.py
 Comment: 
 
-Filename: jieba_pyfast-1.4.1.dist-info/RECORD
+Filename: jieba_pyfast-1.4.2.dist-info/RECORD
 Comment: 
 
-Filename: jieba_pyfast-1.4.1.dist-info/LICENSE
+Filename: jieba_pyfast-1.4.2.dist-info/LICENSE
 Comment: 
 
-Filename: jieba_pyfast-1.4.1.dist-info/WHEEL
+Filename: jieba_pyfast-1.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: jieba_pyfast-1.4.1.dist-info/METADATA
+Filename: jieba_pyfast-1.4.2.dist-info/METADATA
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
-    Value: 0x63A06286
+    Value: 0x646DD5CC
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
@@ -79,19 +79,19 @@
 000004e0: 9886 0000 7000 0000 0200 0000 1800 0000  ....p...........
 000004f0: 3887 0000 f000 0000 4898 0000 700e 0000  8.......H...p...
 00000500: 0b00 0000 5000 0000 0000 0000 a600 0000  ....P...........
 00000510: a600 0000 0500 0000 ab00 0000 4500 0000  ............E...
 00000520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000530: 0000 0000 0000 0000 3896 0000 8300 0000  ........8.......
 00000540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000550: 1b00 0000 1800 0000 c151 434d c7f8 3830  .........QCM..80
-00000560: 8506 d062 3ab5 add6 2400 0000 1000 0000  ...b:...$.......
-00000570: 0009 0a00 0003 0c00 2a00 0000 1000 0000  ........*.......
+00000550: 1b00 0000 1800 0000 1b1a 6df4 a9a5 398c  ..........m...9.
+00000560: 8f05 00f6 2900 fc0c 2400 0000 1000 0000  ....)...$.......
+00000570: 0009 0a00 0001 0d00 2a00 0000 1000 0000  ........*.......
 00000580: 0000 0000 0000 0000 0c00 0000 3800 0000  ............8...
-00000590: 1800 0000 0200 0000 0364 1f05 0000 0100  .........d......
+00000590: 1800 0000 0200 0000 0000 2705 0000 0100  ..........'.....
 000005a0: 2f75 7372 2f6c 6962 2f6c 6962 5379 7374  /usr/lib/libSyst
 000005b0: 656d 2e42 2e64 796c 6962 0000 0000 0000  em.B.dylib......
 000005c0: 2600 0000 1000 0000 0887 0000 3000 0000  &...........0...
 000005d0: 2900 0000 1000 0000 3887 0000 0000 0000  ).......8.......
 000005e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000005f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -2202,15 +2202,15 @@
 00008990: 604b 0000 0000 0000 2f08 0000 0e0c 0000  `K....../.......
 000089a0: 684b 0000 0000 0000 4708 0000 0e0c 0000  hK......G.......
 000089b0: 704b 0000 0000 0000 7008 0000 0e0c 0000  pK......p.......
 000089c0: 084d 0000 0000 0000 0100 0000 6401 0000  .M..........d...
 000089d0: 0000 0000 0000 0000 9108 0000 6400 0000  ............d...
 000089e0: 0000 0000 0000 0000 d308 0000 6400 0000  ............d...
 000089f0: 0000 0000 0000 0000 f808 0000 6603 0100  ............f...
-00008a00: 8662 a063 0000 0000 0100 0000 2e01 0000  .b.c............
+00008a00: ccd5 6d64 0000 0000 0100 0000 2e01 0000  ..md............
 00008a10: e00b 0000 0000 0000 8809 0000 2401 0000  ............$...
 00008a20: e00b 0000 0000 0000 8f09 0000 8400 0000  ................
 00008a30: 0000 0000 0000 0000 0100 0000 2400 0000  ............$...
 00008a40: 5002 0000 0000 0000 0100 0000 4e01 0000  P...........N...
 00008a50: e00b 0000 0000 0000 0100 0000 2e01 0000  ................
 00008a60: 300e 0000 0000 0000 c809 0000 2401 0000  0...........$...
 00008a70: 300e 0000 0000 0000 0100 0000 2400 0000  0...........$...
```

## Comparing `jieba_pyfast-1.4.1.dist-info/RECORD` & `jieba_pyfast-1.4.2.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-_jieba_fast_functions_py3.cpython-311-darwin.so,sha256=I_C2H7Nx6oC8cY6-kZA_M3zW-wue0IQLNkkoZ3rkboM,42680
+_jieba_fast_functions_py3.cpython-311-darwin.so,sha256=Oz7qHDTsEscjFO3iY2xH7mdMvF24o3BwaezStnMNpTk,42680
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
-jieba_pyfast-1.4.1.dist-info/RECORD,,
-jieba_pyfast-1.4.1.dist-info/LICENSE,sha256=GLoJhIOfhYU7Kfra-ZL326j9DKD76uNN4rhzUiLcejc,1075
-jieba_pyfast-1.4.1.dist-info/WHEEL,sha256=4a4lBwQjT6ajNeDmbLTNi-NImv6J2GMoDZJ4F8RWc3o,107
-jieba_pyfast-1.4.1.dist-info/METADATA,sha256=kIitpA-nfgiCAdvKfHs_2jxKwhTrIOecM6wDv6TYp4c,817
+jieba_pyfast-1.4.2.dist-info/RECORD,,
+jieba_pyfast-1.4.2.dist-info/LICENSE,sha256=GLoJhIOfhYU7Kfra-ZL326j9DKD76uNN4rhzUiLcejc,1075
+jieba_pyfast-1.4.2.dist-info/WHEEL,sha256=L9j5kZliY_RmhQpA0BNpxXPfCg-0_bW_DSgAkuvMplg,107
+jieba_pyfast-1.4.2.dist-info/METADATA,sha256=_CNR-CRSQEChPW5Gm48iwIn-iO0QoKa_dN3uEC1bmGs,809
```

## Comparing `jieba_pyfast-1.4.1.dist-info/LICENSE` & `jieba_pyfast-1.4.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jieba_pyfast-1.4.1.dist-info/METADATA` & `jieba_pyfast-1.4.2.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: jieba-pyfast
-Version: 1.4.1
+Version: 1.4.2
 Summary: Tokenize Chinese characters
 License: MIT
 Author: snapADDY GmbH
 Author-email: info@snapaddy.com
-Requires-Python: >=3.11.0,<3.12.0
+Requires-Python: ==3.11.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # jieba_pyfast
```

