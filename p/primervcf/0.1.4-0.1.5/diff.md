# Comparing `tmp/primervcf-0.1.4-py3-none-any.whl.zip` & `tmp/primervcf-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 17326 bytes, number of entries: 17
+Zip file size: 17328 bytes, number of entries: 17
 -rw-rw-r--  2.0 unx      519 b- defN 22-Dec-03 14:54 main.py
 -rw-rw-r--  2.0 unx     5107 b- defN 22-Oct-28 09:04 primer_indel.py
 -rw-rw-r--  2.0 unx     1432 b- defN 22-Dec-12 08:40 bin/fq2vcf.py
 -rw-rw-r--  2.0 unx     3096 b- defN 22-Dec-22 01:42 bin/primerdesign_vcf.py
 -rw-rw-r--  2.0 unx     1049 b- defN 22-Dec-22 01:42 bin/vcf2del.py
--rw-rw-r--  2.0 unx      145 b- defN 23-Apr-28 02:49 primervcf/__init__.py
+-rw-rw-r--  2.0 unx      145 b- defN 23-May-24 08:50 primervcf/__init__.py
 -rw-rw-r--  2.0 unx     2867 b- defN 22-Dec-12 06:31 primervcf/map2vcf.py
 -rw-rw-r--  2.0 unx     6077 b- defN 23-Apr-28 02:46 primervcf/primer_indel.py
 -rw-rw-r--  2.0 unx     1795 b- defN 22-Dec-05 00:32 primervcf/utils.py
 -rw-rw-r--  2.0 unx     2923 b- defN 22-Dec-22 02:50 primervcf/vcfparser.py
--rwxrwxr-x  2.0 unx     1419 b- defN 23-Apr-28 02:54 primervcf-0.1.4.data/scripts/fq2vcf.py
--rwxrwxr-x  2.0 unx     3083 b- defN 23-Apr-28 02:54 primervcf-0.1.4.data/scripts/primerdesign_vcf.py
--rwxrwxr-x  2.0 unx     1036 b- defN 23-Apr-28 02:54 primervcf-0.1.4.data/scripts/vcf2del.py
--rw-rw-r--  2.0 unx     6821 b- defN 23-Apr-28 02:54 primervcf-0.1.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-28 02:54 primervcf-0.1.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Apr-28 02:54 primervcf-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1348 b- defN 23-Apr-28 02:54 primervcf-0.1.4.dist-info/RECORD
-17 files, 38824 bytes uncompressed, 15134 bytes compressed:  61.0%
+-rwxrwxr-x  2.0 unx     1419 b- defN 23-May-24 08:52 primervcf-0.1.5.data/scripts/fq2vcf.py
+-rwxrwxr-x  2.0 unx     3083 b- defN 23-May-24 08:52 primervcf-0.1.5.data/scripts/primerdesign_vcf.py
+-rwxrwxr-x  2.0 unx     1036 b- defN 23-May-24 08:52 primervcf-0.1.5.data/scripts/vcf2del.py
+-rw-rw-r--  2.0 unx     6821 b- defN 23-May-24 08:52 primervcf-0.1.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-24 08:52 primervcf-0.1.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-May-24 08:52 primervcf-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1348 b- defN 23-May-24 08:52 primervcf-0.1.5.dist-info/RECORD
+17 files, 38824 bytes uncompressed, 15136 bytes compressed:  61.0%
```

## zipnote {}

```diff
@@ -24,29 +24,29 @@
 
 Filename: primervcf/utils.py
 Comment: 
 
 Filename: primervcf/vcfparser.py
 Comment: 
 
-Filename: primervcf-0.1.4.data/scripts/fq2vcf.py
+Filename: primervcf-0.1.5.data/scripts/fq2vcf.py
 Comment: 
 
-Filename: primervcf-0.1.4.data/scripts/primerdesign_vcf.py
+Filename: primervcf-0.1.5.data/scripts/primerdesign_vcf.py
 Comment: 
 
-Filename: primervcf-0.1.4.data/scripts/vcf2del.py
+Filename: primervcf-0.1.5.data/scripts/vcf2del.py
 Comment: 
 
-Filename: primervcf-0.1.4.dist-info/METADATA
+Filename: primervcf-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: primervcf-0.1.4.dist-info/WHEEL
+Filename: primervcf-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: primervcf-0.1.4.dist-info/top_level.txt
+Filename: primervcf-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: primervcf-0.1.4.dist-info/RECORD
+Filename: primervcf-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## primervcf/__init__.py

```diff
@@ -1,7 +1,7 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # @Time    : 5/12/2022 12:40 PM
 # @Author  : Runsheng
 # @File    : __init__.py
 
-__version__="0.1.4"
+__version__="0.1.5"
```

## Comparing `primervcf-0.1.4.data/scripts/fq2vcf.py` & `primervcf-0.1.5.data/scripts/fq2vcf.py`

 * *Files identical despite different names*

## Comparing `primervcf-0.1.4.data/scripts/primerdesign_vcf.py` & `primervcf-0.1.5.data/scripts/primerdesign_vcf.py`

 * *Files identical despite different names*

## Comparing `primervcf-0.1.4.data/scripts/vcf2del.py` & `primervcf-0.1.5.data/scripts/vcf2del.py`

 * *Files identical despite different names*

## Comparing `primervcf-0.1.4.dist-info/METADATA` & `primervcf-0.1.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primervcf
-Version: 0.1.4
+Version: 0.1.5
 Summary: primer design for haplotype genotyping using indel information
 Home-page: https://github.com/Runsheng/primervcf
 Author: runsheng
 Author-email: runsheng.lee@gmail.com
 License: GPL-2
 Description-Content-Type: text/markdown
 Requires-Dist: primer3-py (>=0.6.1)
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: primervcf Version: 0.1.4 Summary: primer design for
+Metadata-Version: 2.1 Name: primervcf Version: 0.1.5 Summary: primer design for
 haplotype genotyping using indel information Home-page: https://github.com/
 Runsheng/primervcf Author: runsheng Author-email: runsheng.lee@gmail.com
 License: GPL-2 Description-Content-Type: text/markdown Requires-Dist: primer3-
 py (>=0.6.1) Requires-Dist: biopython (>=1.78) Requires-Dist: primerdiffer
 (>=0.1.4) Requires-Dist: pyssw (>=0.1.4) Requires-Dist: PyVCF3 (>=1.0.3) #
 **primervcf** package ![PyPI](https://img.shields.io/pypi/v/
 primervcf?color=green) ![License](https://img.shields.io/pypi/l/
```

## Comparing `primervcf-0.1.4.dist-info/RECORD` & `primervcf-0.1.5.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 main.py,sha256=vsawfI3E9cyppEtNHqAB60vcFBqPJYkpqBUZtgCQXqA,519
 primer_indel.py,sha256=RHifOKujT-tcVYXXIWlbMh-FTWvVg8IAk_hhPHFP-Qs,5107
 bin/fq2vcf.py,sha256=vdxCnrkmoeBTB8bM_b00eh6TtGqpO8kobxkw3U0G6jc,1432
 bin/primerdesign_vcf.py,sha256=xFirCI2TPz2w1HbzG-rlpAGK3Ynqsdu6yqYWDjJZP8s,3096
 bin/vcf2del.py,sha256=mwftS3UOPu8RdPXzBP9zKQwCZ1cjpYHLWy2FnD40NzE,1049
-primervcf/__init__.py,sha256=4ccvFnkNzWJaU-WVv1fVjUdzMirEwAPRrjl0NEnZRM0,145
+primervcf/__init__.py,sha256=HTKsFLkPt_Jf2IBV0PInDpcLRiXQ1LilM7_EMCryp8w,145
 primervcf/map2vcf.py,sha256=fZBW4eu2LZGqPxskMl48Ai--4HEc13LluMx1OLffqX8,2867
 primervcf/primer_indel.py,sha256=S1bvSA9wgs2au89v9F8lJhlwtWkLPA-LMvmWke8AGf8,6077
 primervcf/utils.py,sha256=-pMtELpo5NE4pwbJwHtavOuvBN2Y1_xKhaTUFju8zj4,1795
 primervcf/vcfparser.py,sha256=dEicz6bCUZWdhxSCrdCm2mejcVeeDI33KHrRIobSp7c,2923
-primervcf-0.1.4.data/scripts/fq2vcf.py,sha256=WvZz8BWVLtVvs3WRvqzwJ00knbrW0KJNbUguNHETatU,1419
-primervcf-0.1.4.data/scripts/primerdesign_vcf.py,sha256=KxvCDsq-3z9VyITqoaSljhsiSQI-0N5UMTcVCXDNatY,3083
-primervcf-0.1.4.data/scripts/vcf2del.py,sha256=iprjY1DOsko1W9OKXhPzOx8bfOqURKEEzWid-wPbhT8,1036
-primervcf-0.1.4.dist-info/METADATA,sha256=KpTUHGl0csILcKW16jDe2kFrXxfAUwCF-DG8JZWIy6w,6821
-primervcf-0.1.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-primervcf-0.1.4.dist-info/top_level.txt,sha256=blIj4ylPX158RvqoDhQAdf--tR3HfLNsH6Mo5xMPJ7U,15
-primervcf-0.1.4.dist-info/RECORD,,
+primervcf-0.1.5.data/scripts/fq2vcf.py,sha256=WvZz8BWVLtVvs3WRvqzwJ00knbrW0KJNbUguNHETatU,1419
+primervcf-0.1.5.data/scripts/primerdesign_vcf.py,sha256=KxvCDsq-3z9VyITqoaSljhsiSQI-0N5UMTcVCXDNatY,3083
+primervcf-0.1.5.data/scripts/vcf2del.py,sha256=iprjY1DOsko1W9OKXhPzOx8bfOqURKEEzWid-wPbhT8,1036
+primervcf-0.1.5.dist-info/METADATA,sha256=fjj-7DEjJUbkN45c3agQ4iLEoSigeSrucz7pJSfE-2Y,6821
+primervcf-0.1.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+primervcf-0.1.5.dist-info/top_level.txt,sha256=blIj4ylPX158RvqoDhQAdf--tR3HfLNsH6Mo5xMPJ7U,15
+primervcf-0.1.5.dist-info/RECORD,,
```

