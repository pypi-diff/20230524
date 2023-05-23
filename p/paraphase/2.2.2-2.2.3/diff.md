# Comparing `tmp/paraphase-2.2.2.tar.gz` & `tmp/paraphase-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paraphase-2.2.2.tar", last modified: Mon May  1 19:34:36 2023, max compression
+gzip compressed data, was "paraphase-2.2.3.tar", last modified: Tue May 23 23:09:42 2023, max compression
```

## Comparing `paraphase-2.2.2.tar` & `paraphase-2.2.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-05-01 19:34:36.061583 paraphase-2.2.2/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     1675 2022-10-20 20:09:26.000000 paraphase-2.2.2/LICENSE
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     7304 2023-05-01 19:34:36.060574 paraphase-2.2.2/PKG-INFO
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     6974 2023-04-29 00:59:55.000000 paraphase-2.2.2/README.md
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-05-01 19:34:35.658566 paraphase-2.2.2/paraphase/
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)       22 2023-05-01 19:10:23.000000 paraphase-2.2.2/paraphase/__init__.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)      123 2023-05-01 16:34:08.000000 paraphase-2.2.2/paraphase/__main__.py
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-05-01 19:34:35.701833 paraphase-2.2.2/paraphase/data/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     3457 2023-05-01 19:05:53.000000 paraphase-2.2.2/paraphase/data/config.yaml
--rw-r--r--   0 xchen    (71795) Domain Users (10513)      104 2023-05-01 19:05:53.000000 paraphase-2.2.2/paraphase/data/genes.yaml
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     2352 2022-10-20 17:37:49.000000 paraphase-2.2.2/paraphase/data/genome_region.bed
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-05-01 19:34:35.704834 paraphase-2.2.2/paraphase/data/rccx/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)      256 2023-03-11 03:44:27.000000 paraphase-2.2.2/paraphase/data/rccx/cyp21_diff_sites.txt
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-05-01 19:34:35.729842 paraphase-2.2.2/paraphase/data/smn1/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)   665935 2023-04-29 00:59:55.000000 paraphase-2.2.2/paraphase/data/smn1/known_haplotypes.json
--rw-r--r--   0 xchen    (71795) Domain Users (10513)    48846 2023-03-11 03:44:27.000000 paraphase-2.2.2/paraphase/data/smn1/ref_smn2.fa
--rw-r--r--   0 xchen    (71795) Domain Users (10513)       38 2023-03-11 03:44:27.000000 paraphase-2.2.2/paraphase/data/smn1/ref_smn2.fa.fai
--rw-r--r--   0 xchen    (71795) Domain Users (10513)  1584900 2022-10-20 17:37:49.000000 paraphase-2.2.2/paraphase/data/smn1/smn_matching_pos.txt
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-05-01 19:34:35.956567 paraphase-2.2.2/paraphase/genes/
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)      320 2023-05-01 19:05:53.000000 paraphase-2.2.2/paraphase/genes/__init__.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     2719 2023-04-29 00:59:55.000000 paraphase-2.2.2/paraphase/genes/cfc1_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     6307 2023-04-29 00:59:55.000000 paraphase-2.2.2/paraphase/genes/f8_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     6693 2023-04-29 00:59:55.000000 paraphase-2.2.2/paraphase/genes/ikbkg_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     4435 2023-04-29 00:59:55.000000 paraphase-2.2.2/paraphase/genes/ncf1_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     5462 2023-04-29 00:59:55.000000 paraphase-2.2.2/paraphase/genes/neb_phaser.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     2887 2023-04-29 00:59:55.000000 paraphase-2.2.2/paraphase/genes/pms2_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)    23326 2023-04-29 00:59:55.000000 paraphase-2.2.2/paraphase/genes/rccx_phaser.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    25529 2023-04-29 00:59:55.000000 paraphase-2.2.2/paraphase/genes/smn1_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     5590 2023-04-29 00:59:55.000000 paraphase-2.2.2/paraphase/genes/strc_phaser.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     1836 2023-04-29 00:59:55.000000 paraphase-2.2.2/paraphase/genome_depth.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    47878 2023-04-29 00:59:55.000000 paraphase-2.2.2/paraphase/haplotype_assembler.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    18442 2023-05-01 19:09:17.000000 paraphase-2.2.2/paraphase/paraphase.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    55195 2023-05-01 16:34:08.000000 paraphase-2.2.2/paraphase/phaser.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    30069 2023-05-01 19:08:38.000000 paraphase-2.2.2/paraphase/prepare_bam_and_vcf.py
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-05-01 19:34:35.687569 paraphase-2.2.2/paraphase.egg-info/
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     7304 2023-05-01 19:34:33.000000 paraphase-2.2.2/paraphase.egg-info/PKG-INFO
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     1153 2023-05-01 19:34:33.000000 paraphase-2.2.2/paraphase.egg-info/SOURCES.txt
--rw-r--r--   0 xchen    (71795) Domain Users (10513)        1 2023-05-01 19:34:33.000000 paraphase-2.2.2/paraphase.egg-info/dependency_links.txt
--rw-r--r--   0 xchen    (71795) Domain Users (10513)       54 2023-05-01 19:34:33.000000 paraphase-2.2.2/paraphase.egg-info/entry_points.txt
--rw-r--r--   0 xchen    (71795) Domain Users (10513)       45 2023-05-01 19:34:33.000000 paraphase-2.2.2/paraphase.egg-info/requires.txt
--rw-r--r--   0 xchen    (71795) Domain Users (10513)       10 2023-05-01 19:34:33.000000 paraphase-2.2.2/paraphase.egg-info/top_level.txt
--rw-r--r--   0 xchen    (71795) Domain Users (10513)       38 2023-05-01 19:34:36.062567 paraphase-2.2.2/setup.cfg
--rw-r--r--   0 xchen    (71795) Domain Users (10513)      846 2023-05-01 19:31:14.000000 paraphase-2.2.2/setup.py
-drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-05-01 19:34:36.056576 paraphase-2.2.2/tests/
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    16147 2023-03-11 01:37:24.000000 paraphase-2.2.2/tests/test_haplotype_assembler.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     1501 2023-04-29 00:59:55.000000 paraphase-2.2.2/tests/test_paraphase.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     8332 2023-04-29 00:59:55.000000 paraphase-2.2.2/tests/test_phaser.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     1793 2023-04-29 00:59:55.000000 paraphase-2.2.2/tests/test_prepare_bam_and_vcf.py
--rw-r--r--   0 xchen    (71795) Domain Users (10513)     4316 2023-04-29 00:59:55.000000 paraphase-2.2.2/tests/test_rccx_phaser.py
--rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     8582 2023-04-29 00:59:55.000000 paraphase-2.2.2/tests/test_smn1_phaser.py
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-05-23 23:09:42.950712 paraphase-2.2.3/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     1675 2022-10-20 20:09:26.000000 paraphase-2.2.3/LICENSE
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     7304 2023-05-23 23:09:42.949717 paraphase-2.2.3/PKG-INFO
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     6974 2023-05-11 22:15:57.000000 paraphase-2.2.3/README.md
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-05-23 23:09:42.754719 paraphase-2.2.3/paraphase/
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)       22 2023-05-22 17:45:55.000000 paraphase-2.2.3/paraphase/__init__.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)      123 2023-05-11 22:15:57.000000 paraphase-2.2.3/paraphase/__main__.py
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-05-23 23:09:42.830709 paraphase-2.2.3/paraphase/data/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     3457 2023-05-22 17:38:53.000000 paraphase-2.2.3/paraphase/data/config.yaml
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)      104 2023-05-22 17:38:53.000000 paraphase-2.2.3/paraphase/data/genes.yaml
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     2352 2022-10-20 17:37:49.000000 paraphase-2.2.3/paraphase/data/genome_region.bed
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-05-23 23:09:42.834716 paraphase-2.2.3/paraphase/data/rccx/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)      256 2023-05-11 22:15:57.000000 paraphase-2.2.3/paraphase/data/rccx/cyp21_diff_sites.txt
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-05-23 23:09:42.854408 paraphase-2.2.3/paraphase/data/smn1/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)   665935 2023-05-11 22:15:58.000000 paraphase-2.2.3/paraphase/data/smn1/known_haplotypes.json
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)    48846 2023-05-11 22:15:58.000000 paraphase-2.2.3/paraphase/data/smn1/ref_smn2.fa
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)       38 2023-05-11 22:15:58.000000 paraphase-2.2.3/paraphase/data/smn1/ref_smn2.fa.fai
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)  1584900 2022-10-20 17:37:49.000000 paraphase-2.2.3/paraphase/data/smn1/smn_matching_pos.txt
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-05-23 23:09:42.912711 paraphase-2.2.3/paraphase/genes/
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)      320 2023-05-22 17:38:53.000000 paraphase-2.2.3/paraphase/genes/__init__.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     2719 2023-05-11 22:15:58.000000 paraphase-2.2.3/paraphase/genes/cfc1_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     6240 2023-05-23 22:35:18.000000 paraphase-2.2.3/paraphase/genes/f8_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     6693 2023-05-11 22:15:58.000000 paraphase-2.2.3/paraphase/genes/ikbkg_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     4435 2023-05-11 22:15:58.000000 paraphase-2.2.3/paraphase/genes/ncf1_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     5462 2023-05-11 22:15:58.000000 paraphase-2.2.3/paraphase/genes/neb_phaser.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     2887 2023-05-11 22:15:58.000000 paraphase-2.2.3/paraphase/genes/pms2_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)    23326 2023-05-12 17:09:18.000000 paraphase-2.2.3/paraphase/genes/rccx_phaser.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    25529 2023-05-11 22:15:58.000000 paraphase-2.2.3/paraphase/genes/smn1_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     5590 2023-05-11 22:15:58.000000 paraphase-2.2.3/paraphase/genes/strc_phaser.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     1836 2023-05-11 22:15:58.000000 paraphase-2.2.3/paraphase/genome_depth.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    48123 2023-05-23 22:35:15.000000 paraphase-2.2.3/paraphase/haplotype_assembler.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    20859 2023-05-23 23:06:17.000000 paraphase-2.2.3/paraphase/paraphase.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    55387 2023-05-23 22:44:34.000000 paraphase-2.2.3/paraphase/phaser.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    30953 2023-05-23 22:35:35.000000 paraphase-2.2.3/paraphase/prepare_bam_and_vcf.py
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-05-23 23:09:42.798709 paraphase-2.2.3/paraphase.egg-info/
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     7304 2023-05-23 23:09:41.000000 paraphase-2.2.3/paraphase.egg-info/PKG-INFO
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     1153 2023-05-23 23:09:41.000000 paraphase-2.2.3/paraphase.egg-info/SOURCES.txt
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)        1 2023-05-23 23:09:41.000000 paraphase-2.2.3/paraphase.egg-info/dependency_links.txt
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)       54 2023-05-23 23:09:41.000000 paraphase-2.2.3/paraphase.egg-info/entry_points.txt
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)       45 2023-05-23 23:09:41.000000 paraphase-2.2.3/paraphase.egg-info/requires.txt
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)       10 2023-05-23 23:09:41.000000 paraphase-2.2.3/paraphase.egg-info/top_level.txt
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)       38 2023-05-23 23:09:42.952741 paraphase-2.2.3/setup.cfg
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)      846 2023-05-11 22:15:58.000000 paraphase-2.2.3/setup.py
+drwxr-xr-x   0 xchen    (71795) Domain Users (10513)        0 2023-05-23 23:09:42.945711 paraphase-2.2.3/tests/
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)    16147 2023-05-11 22:15:58.000000 paraphase-2.2.3/tests/test_haplotype_assembler.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     1501 2023-05-11 22:15:58.000000 paraphase-2.2.3/tests/test_paraphase.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     8332 2023-05-11 22:15:58.000000 paraphase-2.2.3/tests/test_phaser.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     1793 2023-05-11 22:15:58.000000 paraphase-2.2.3/tests/test_prepare_bam_and_vcf.py
+-rw-r--r--   0 xchen    (71795) Domain Users (10513)     4316 2023-05-11 22:15:58.000000 paraphase-2.2.3/tests/test_rccx_phaser.py
+-rwxr-xr-x   0 xchen    (71795) Domain Users (10513)     8582 2023-05-11 22:15:58.000000 paraphase-2.2.3/tests/test_smn1_phaser.py
```

### Comparing `paraphase-2.2.2/LICENSE` & `paraphase-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.2/PKG-INFO` & `paraphase-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paraphase
-Version: 2.2.2
+Version: 2.2.3
 Summary: paraphase: HiFi-based caller for highly homologous genes
 Home-page: https://github.com/PacificBiosciences/paraphase
 Author: Xiao Chen
 Author-email: xchen@pacificbiosciences.com
 License: BSD-3-Clause-Clear
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `paraphase-2.2.2/README.md` & `paraphase-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.2/paraphase/data/config.yaml` & `paraphase-2.2.3/paraphase/data/config.yaml`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.2/paraphase/data/genome_region.bed` & `paraphase-2.2.3/paraphase/data/genome_region.bed`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.2/paraphase/data/smn1/known_haplotypes.json` & `paraphase-2.2.3/paraphase/data/smn1/known_haplotypes.json`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.2/paraphase/data/smn1/ref_smn2.fa` & `paraphase-2.2.3/paraphase/data/smn1/ref_smn2.fa`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.2/paraphase/data/smn1/smn_matching_pos.txt` & `paraphase-2.2.3/paraphase/data/smn1/smn_matching_pos.txt`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.2/paraphase/genes/cfc1_phaser.py` & `paraphase-2.2.3/paraphase/genes/cfc1_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.2/paraphase/genes/f8_phaser.py` & `paraphase-2.2.3/paraphase/genes/f8_phaser.py`

 * *Files 5% similar despite different names*

```diff
@@ -145,21 +145,20 @@
             hap_name = ass_haps[hap]
             p5region = list(set(regions[0]))
             p3region = list(set(regions[1]))
             flanking_sum.setdefault(
                 hap_name, "-".join(["/".join(p5region), "/".join(p3region)])
             )
         for hap, links in flanking_sum.items():
-            if "region1" in links and links != "region1-region1":
-                if links == "region1-region2":
-                    sv_hap.setdefault(hap_name, "deletion")
-                elif links == "region2-region1":
-                    sv_hap.setdefault(hap_name, "duplication")
-                elif "region3" in links:
-                    sv_hap.setdefault(hap_name, "inversion")
+            if links == "region1-region2":
+                sv_hap.setdefault(hap, "deletion")
+            elif links == "region2-region1":
+                sv_hap.setdefault(hap, "duplication")
+            elif links == "region3-region1" or links == "region1-region3":
+                sv_hap.setdefault(hap, "inversion")
 
         self.close_handle()
 
         return self.GeneCall(
             total_cn,
             ass_haps,
             [],
```

### Comparing `paraphase-2.2.2/paraphase/genes/ikbkg_phaser.py` & `paraphase-2.2.3/paraphase/genes/ikbkg_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.2/paraphase/genes/ncf1_phaser.py` & `paraphase-2.2.3/paraphase/genes/ncf1_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.2/paraphase/genes/neb_phaser.py` & `paraphase-2.2.3/paraphase/genes/neb_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.2/paraphase/genes/pms2_phaser.py` & `paraphase-2.2.3/paraphase/genes/pms2_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.2/paraphase/genes/rccx_phaser.py` & `paraphase-2.2.3/paraphase/genes/rccx_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.2/paraphase/genes/smn1_phaser.py` & `paraphase-2.2.3/paraphase/genes/smn1_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.2/paraphase/genes/strc_phaser.py` & `paraphase-2.2.3/paraphase/genes/strc_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.2/paraphase/genome_depth.py` & `paraphase-2.2.3/paraphase/genome_depth.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.2/paraphase/haplotype_assembler.py` & `paraphase-2.2.3/paraphase/haplotype_assembler.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,30 +255,30 @@
             # when variants are inside a deletion region
             has_sv = True in [
                 at[0].split("-")[0] not in ["1", "2"]
                 or at[1].split("-")[0] not in ["1", "2"]
                 for at in self.edge_per_position[pos]
             ]
             thres = self.get_thres(num_reads)
-            for (node1, node2, n) in self.edge_per_position[pos]:
+            for node1, node2, n in self.edge_per_position[pos]:
                 if (
                     len(self.next_per_node[node1]) > 1
                     and len(self.previous_per_node[node2]) > 1
                     and n <= thres
                 ) or (
                     has_sv
                     and n == 1
                     and len(self.next_per_node[node1]) > 1
                     and len(self.previous_per_node[node2]) > 1
                 ):
                     edges_removed.append((node1, node2, n))
                 else:
                     new_edge_per_position.setdefault(pos, []).append((node1, node2, n))
         self.edge_per_position = new_edge_per_position
-        for (node1, node2, n) in edges_removed:
+        for node1, node2, n in edges_removed:
             if debug:
                 print("removing", node1, node2, n)
             self.next_per_node[node1].remove(node2)
             self.previous_per_node[node2].remove(node1)
         for pos in self.edge_per_position:
             num_reads = [at[2] for at in self.edge_per_position[pos]]
             self.edge_info.setdefault(pos, num_reads)
@@ -787,26 +787,26 @@
             for node1, node2, _ in self.edge_per_position[pos]:
                 self.add_edge(node1, node2)
                 if node1 not in self.nodes:
                     self.nodes.append(node1)
                 if node2 not in self.nodes:
                     self.nodes.append(node2)
 
-        for i in [1, 2]:
+        for i in range(5):
             for j in range(self.nvar):
                 node = f"{i}-{j}"
                 if node not in self.nodes:
                     hap = "x" * j + str(i) + "x" * (self.nvar - j - 1)
                     read_support = self.match_reads_and_haplotypes(
                         self.reads_original, [hap]
                     )
                     if hap in read_support.unique and len(read_support.unique[hap]) > 1:
                         self.nodes.append(node)
 
-        for (node1, node2) in self.edges:
+        for node1, node2 in self.edges:
             for n in (node1, node2):
                 if n not in self.nodes:
                     self.nodes.append(n)
         self.get_positions()
         if debug:
             pprint(self.edge_per_position)
 
@@ -1133,35 +1133,40 @@
         highest_cn, main_haps_candidates = self.get_highest_cn(final_haps)
 
         # extend all possible haps
         extended_main_hap_candidates = []
         for main_haps_candidate in main_haps_candidates:
             extended = self.extend_pivot_blocks(main_haps_candidate, debug=debug)
             extended_main_hap_candidates.append(extended)
-        scores = []
-        for extended_main_hap_candidate in extended_main_hap_candidates:
-            pivot_ones = [
-                a for a in extended_main_hap_candidate if a[self.pivot_pos] != "x"
-            ]
-            nhap = len(pivot_ones)
-            total_length = sum([len(a.strip("x")) for a in pivot_ones])
-
-            represented_haps = []
-            for hap1 in final_haps:
-                mismatches = []
-                for hap2 in pivot_ones:
-                    match, mismatch, extend = VariantGraph.compare_two_haps(hap1, hap2)
-                    mismatches.append(mismatch)
-                if 0 in mismatches:
-                    represented_haps.append(hap1)
-            num_represented_haps = len(represented_haps)
-
-            scores.append(((nhap, num_represented_haps, total_length), pivot_ones))
-        sort_candidates = sorted(
-            scores,
-            key=lambda x: x[0],
-            reverse=True,
-        )
-        main_haps = sort_candidates[0][1]
+        if self.pivot_pos != -1:
+            scores = []
+            for extended_main_hap_candidate in extended_main_hap_candidates:
+                pivot_ones = [
+                    a for a in extended_main_hap_candidate if a[self.pivot_pos] != "x"
+                ]
+                nhap = len(pivot_ones)
+                total_length = sum([len(a.strip("x")) for a in pivot_ones])
+
+                represented_haps = []
+                for hap1 in final_haps:
+                    mismatches = []
+                    for hap2 in pivot_ones:
+                        match, mismatch, extend = VariantGraph.compare_two_haps(
+                            hap1, hap2
+                        )
+                        mismatches.append(mismatch)
+                    if 0 in mismatches:
+                        represented_haps.append(hap1)
+                num_represented_haps = len(represented_haps)
+
+                scores.append(((nhap, num_represented_haps, total_length), pivot_ones))
+            sort_candidates = sorted(
+                scores,
+                key=lambda x: x[0],
+                reverse=True,
+            )
+            main_haps = sort_candidates[0][1]
+        else:
+            main_haps = extended_main_hap_candidates[0]
         if main_haps == []:
             main_haps = final_haps
         return main_haps, final_haps, highest_cn
```

### Comparing `paraphase-2.2.2/paraphase/paraphase.py` & `paraphase-2.2.3/paraphase/paraphase.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # paraphase
 # Author: Xiao Chen <xchen@pacificbiosciences.com>
 
 
 import os
+import sys
 import argparse
 import json
 import yaml
 import logging
 import datetime
 import shutil
 import pysam
@@ -18,33 +19,26 @@
 from paraphase.genome_depth import GenomeDepth
 from paraphase.prepare_bam_and_vcf import (
     BamRealigner,
     BamTagger,
     VcfGenerater,
     TwoGeneVcfGenerater,
 )
+import paraphase
 from paraphase import genes
 from .phaser import Phaser
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 class Paraphase:
     def __init__(self):
         self.samtools = None
         self.minimap2 = None
 
-    @staticmethod
-    def get_version():
-        with open(os.path.join(os.path.dirname(__file__), "__init__.py")) as f:
-            for line in f:
-                if "version" in line:
-                    return line.split('"')[1]
-        return None
-
     def parse_configs(self, region_config=None):
         """
         Parse config files
         region_config: parameters for each region of interest
         gene_config: specifies some additional analyses triggered with some genes
         """
         data_path = os.path.join(os.path.dirname(__file__), "data")
@@ -58,126 +52,207 @@
         with open(gene_config, "r") as f:
             gene_config_parsed = yaml.safe_load(f)
         self.genes_to_call = gene_config_parsed.get("genes_to_call")
         self.genome_depth_genes = gene_config_parsed.get("genome_depth_genes")
         self.no_vcf_genes = gene_config_parsed.get("no_vcf_genes")
         self.check_sex_genes = gene_config_parsed.get("check_sex_genes")
 
-    def process_sample(self, bamlist, outdir, configs, tmpdir, dcov={}, novcf=False):
+    def process_gene(
+        self,
+        gene_list,
+        configs,
+        outdir,
+        tmpdir,
+        gdepth,
+        bam,
+        sample_sex,
+        novcf,
+        prog_cmd,
+    ):
+        """Workflow for each region"""
+        phaser_calls = {}
+        for gene in gene_list:
+            try:
+                sample_id = bam.split("/")[-1].split(".")[0]
+                if gene == "smn1":
+                    phaser = genes.Smn1Phaser(
+                        sample_id, tmpdir, gdepth, bam, sample_sex
+                    )
+                elif gene == "rccx":
+                    phaser = genes.RccxPhaser(
+                        sample_id, tmpdir, gdepth, bam, sample_sex
+                    )
+                elif gene == "pms2":
+                    phaser = genes.Pms2Phaser(
+                        sample_id, tmpdir, gdepth, bam, sample_sex
+                    )
+                elif gene == "strc":
+                    phaser = genes.StrcPhaser(
+                        sample_id, tmpdir, gdepth, bam, sample_sex
+                    )
+                elif gene == "ncf1":
+                    phaser = genes.Ncf1Phaser(
+                        sample_id, tmpdir, gdepth, bam, sample_sex
+                    )
+                elif gene == "cfc1":
+                    phaser = genes.Cfc1Phaser(
+                        sample_id, tmpdir, gdepth, bam, sample_sex
+                    )
+                elif gene == "neb":
+                    phaser = genes.NebPhaser(sample_id, tmpdir, gdepth, bam, sample_sex)
+                elif gene == "ikbkg":
+                    phaser = genes.IkbkgPhaser(
+                        sample_id, tmpdir, gdepth, bam, sample_sex
+                    )
+                elif gene == "f8":
+                    phaser = genes.F8Phaser(sample_id, tmpdir, gdepth, bam, sample_sex)
+                else:
+                    phaser = Phaser(sample_id, tmpdir)
+
+                config = configs[gene]
+                logging.info(
+                    f"Running analysis for {gene} for sample {sample_id} at {datetime.datetime.now()}..."
+                )
+                logging.info(
+                    f"Realigning reads for {gene} for sample {sample_id} at {datetime.datetime.now()}..."
+                )
+                bam_realigner = BamRealigner(bam, tmpdir, config, prog_cmd)
+                bam_realigner.write_realign_bam()
+
+                logging.info(
+                    f"Phasing haplotypes for {gene} for sample {sample_id} at {datetime.datetime.now()}..."
+                )
+
+                phaser.set_parameter(config)
+                phaser_call = phaser.call()._asdict()
+                phaser_calls.setdefault(gene, phaser_call)
+
+                logging.info(
+                    f"Tagging reads for {gene} for sample {sample_id} at {datetime.datetime.now()}..."
+                )
+                bam_tagger = BamTagger(sample_id, tmpdir, config, phaser_call)
+                bam_tagger.write_bam(random_assign=True)
+
+                if novcf is False and gene not in self.no_vcf_genes:
+                    logging.info(
+                        f"Generating VCFs for {gene} for sample {sample_id} at {datetime.datetime.now()}..."
+                    )
+                    if gene == "smn1":
+                        vcf_generater = TwoGeneVcfGenerater(
+                            sample_id,
+                            outdir,
+                            phaser_call,
+                        )
+                        vcf_generater.set_parameter(
+                            config, tmpdir=tmpdir, prog_cmd=prog_cmd
+                        )
+                        vcf_generater.run()
+                    else:
+                        vcf_generater = VcfGenerater(
+                            sample_id,
+                            outdir,
+                            phaser_call,
+                        )
+                        vcf_generater.set_parameter(
+                            config, tmpdir=tmpdir, prog_cmd=prog_cmd
+                        )
+                        vcf_generater.run_without_realign()
+            except Exception:
+                logging.error(
+                    f"Error running {gene} for sample {sample_id}...See error message below"
+                )
+                traceback.print_exc()
+                phaser_calls.setdefault(gene, None)
+        return phaser_calls
+
+    def process_sample(
+        self,
+        bamlist,
+        outdir,
+        configs,
+        tmpdir,
+        prog_cmd,
+        num_threads=1,
+        dcov={},
+        novcf=False,
+    ):
         """Main workflow"""
         for bam in bamlist:
             try:
                 sample_id = bam.split("/")[-1].split(".")[0]
                 logging.info(
                     f"Processing sample {sample_id} at {datetime.datetime.now()}..."
                 )
                 sample_out = {}
                 gdepth = None
                 sample_sex = None
-                query_genes = set(configs.keys())
-                if query_genes.intersection(set(self.genome_depth_genes)) != set():
+                query_genes = list(configs.keys())
+                if set(query_genes).intersection(set(self.genome_depth_genes)) != set():
                     logging.info(
-                        f"Getting genome depth at {datetime.datetime.now()}..."
+                        f"Getting genome depth for sample {sample_id} at {datetime.datetime.now()}..."
                     )
                     if sample_id in dcov:
                         gdepth = dcov[sample_id]
                     if gdepth is None:
                         depth = GenomeDepth(
                             bam,
                             os.path.join(
                                 os.path.dirname(__file__), "data", "genome_region.bed"
                             ),
                         )
                         gdepth, gmad = depth.call()
                         if gdepth < 10 or gmad > 0.25:
                             logging.warning(
-                                "Due to low or highly variable genome coverage, genome coverage is not used for depth correction."
+                                f"For sample {sample_id}, due to low or highly variable genome coverage, genome coverage is not used for depth correction."
                             )
                             gdepth = None
 
-                phasers = {
-                    "smn1": genes.Smn1Phaser(
-                        sample_id, tmpdir, gdepth, bam, sample_sex
-                    ),
-                    "rccx": genes.RccxPhaser(
-                        sample_id, tmpdir, gdepth, bam, sample_sex
-                    ),
-                    "pms2": genes.Pms2Phaser(
-                        sample_id, tmpdir, gdepth, bam, sample_sex
-                    ),
-                    "strc": genes.StrcPhaser(
-                        sample_id, tmpdir, gdepth, bam, sample_sex
-                    ),
-                    "ncf1": genes.Ncf1Phaser(
-                        sample_id, tmpdir, gdepth, bam, sample_sex
-                    ),
-                    "cfc1": genes.Cfc1Phaser(
-                        sample_id, tmpdir, gdepth, bam, sample_sex
-                    ),
-                    "neb": genes.NebPhaser(sample_id, tmpdir, gdepth, bam, sample_sex),
-                    "ikbkg": genes.IkbkgPhaser(
-                        sample_id, tmpdir, gdepth, bam, sample_sex
-                    ),
-                    "f8": genes.F8Phaser(sample_id, tmpdir, gdepth, bam, sample_sex),
-                }
-                for gene in configs:
-                    config = configs[gene]
-                    logging.info(
-                        f"Running analysis for {gene} at {datetime.datetime.now()}..."
-                    )
-                    logging.info(
-                        f"Realigning reads for {gene} at {datetime.datetime.now()}..."
-                    )
-                    bam_realigner = BamRealigner(bam, tmpdir, config)
-                    bam_realigner.write_realign_bam()
-
-                    logging.info(
-                        f"Phasing haplotypes for {gene} at {datetime.datetime.now()}..."
+                if num_threads == 1:
+                    sample_out = self.process_gene(
+                        query_genes,
+                        configs,
+                        outdir,
+                        tmpdir,
+                        gdepth,
+                        bam,
+                        sample_sex,
+                        novcf,
+                        prog_cmd,
                     )
-
-                    phaser = phasers.get(gene)
-                    # use default phaser for other genes
-                    if phaser is None:
-                        phaser = Phaser(sample_id, tmpdir)
-                    phaser.set_parameter(config)
-                    phaser_call = phaser.call()._asdict()
-
-                    logging.info(
-                        f"Tagging reads for {gene} at {datetime.datetime.now()}..."
+                else:
+                    process_gene_partial = partial(
+                        self.process_gene,
+                        configs=configs,
+                        outdir=outdir,
+                        tmpdir=tmpdir,
+                        gdepth=gdepth,
+                        bam=bam,
+                        sample_sex=sample_sex,
+                        novcf=novcf,
+                        prog_cmd=prog_cmd,
                     )
-                    bam_tagger = BamTagger(sample_id, tmpdir, config, phaser_call)
-                    bam_tagger.write_bam(random_assign=True)
-
-                    if novcf is False and gene not in self.no_vcf_genes:
-                        logging.info(
-                            f"Generating VCFs for {gene} at {datetime.datetime.now()}..."
-                        )
-                        if gene == "smn1":
-                            vcf_generater = TwoGeneVcfGenerater(
-                                sample_id,
-                                outdir,
-                                phaser_call,
-                            )
-                            vcf_generater.set_parameter(config, tmpdir=tmpdir)
-                            vcf_generater.run()
-                        else:
-                            vcf_generater = VcfGenerater(
-                                sample_id,
-                                outdir,
-                                phaser_call,
-                            )
-                            vcf_generater.set_parameter(config, tmpdir=tmpdir)
-                            vcf_generater.run_without_realign()
-
-                    sample_out.setdefault(gene, phaser_call)
+                    gene_groups = [
+                        query_genes[i::num_threads] for i in range(num_threads)
+                    ]
+                    pool = mp.Pool(num_threads)
+                    phaser_calls = pool.map(process_gene_partial, gene_groups)
+                    pool.close()
+                    pool.join()
+                    for phaser_call_set in phaser_calls:
+                        sample_out.update(phaser_call_set)
+                sample_out = dict(sorted(sample_out.items()))
 
-                logging.info(f"Merging all bams at {datetime.datetime.now()}...")
+                logging.info(
+                    f"Merging all bams for sample {sample_id} at {datetime.datetime.now()}..."
+                )
                 self.merge_bams(query_genes, outdir, tmpdir, sample_id)
 
-                logging.info(f"Writing to json at {datetime.datetime.now()}...")
+                logging.info(
+                    f"Writing to json for sample {sample_id} at {datetime.datetime.now()}..."
+                )
                 out_json = os.path.join(outdir, sample_id + ".json")
                 with open(out_json, "w") as json_output:
                     json.dump(sample_out, json_output, indent=4)
             except Exception:
                 logging.error(
                     f"Error running sample {sample_id}...See error message below"
                 )
@@ -198,19 +273,14 @@
             for bam in bams:
                 fout.write(bam + "\n")
         merged_bam = os.path.join(outdir, f"{sample_id}_realigned_tagged.bam")
         tmp_bam = os.path.join(tmpdir, f"{sample_id}_merged.bam")
         pysam.merge("-f", "-o", tmp_bam, "-b", bam_list_file)
         pysam.sort("-o", merged_bam, tmp_bam)
         pysam.index(merged_bam)
-        os.remove(tmp_bam)
-        os.remove(bam_list_file)
-        for bam in bams:
-            os.remove(bam)
-            os.remove(bam + ".bai")
 
     def get_samtools_minimap2_path(self, args):
         """Get and check path to third-party tools"""
         samtools_check = [
             a for a in [args.samtools, shutil.which("samtools")] if a is not None
         ]
         samtools_check2 = [a for a in samtools_check if os.path.exists(a)]
@@ -348,15 +418,15 @@
             "--depth",
             help="Optional path to a file listing average depth for each sample",
             required=False,
         )
         parser.add_argument(
             "-t",
             "--threads",
-            help="Optional number of threads. Only used together with -l",
+            help="Optional number of threads",
             required=False,
             type=int,
             default=1,
         )
         parser.add_argument(
             "--novcf",
             help="Optional. If specified, paraphase will not write vcfs",
@@ -370,30 +440,31 @@
         )
         parser.add_argument(
             "--minimap2",
             help="Optional path to minimap2",
             required=False,
         )
         parser.add_argument(
-            "-v", "--version", action="version", version=f"{self.get_version()}"
+            "-v", "--version", action="version", version=f"{paraphase.__version__}"
         )
         return parser
 
     def run(self):
         parser = self.load_parameters()
         args = parser.parse_args()
+        num_threads = args.threads
         outdir = args.out
-        if os.path.exists(outdir) is False:
-            os.makedirs(outdir)
+        os.makedirs(outdir, exist_ok=True)
         tmpdir = os.path.join(
             outdir, f"tmp_{datetime.datetime.now().strftime('%Y-%m-%d-%H-%M-%S-%f')}"
         )
-        os.makedirs(tmpdir)
+        os.makedirs(tmpdir, exist_ok=True)
 
         try:
+            prog_cmd = " ".join(sys.argv[1:])
             self.parse_configs(region_config=args.config)
             self.get_samtools_minimap2_path(args)
             gene_list = self.get_gene_list(args.gene)
             if gene_list == []:
                 all_genes_joined = ",".join(self.accepted_genes)
                 raise Exception(
                     f"Please provide valid gene name(s). Accepted genes are {all_genes_joined}."
@@ -406,42 +477,46 @@
                 with open(args.depth) as f:
                     for line in f:
                         split_line = line.split()
                         dcov.setdefault(split_line[0], float(split_line[-1]))
 
             # process sample(s)
             bamlist = []
+            # one bam, multiprocess by gene
             if args.bam is not None:
                 if os.path.exists(args.bam) and os.path.exists(args.bam + ".bai"):
                     bamlist = [args.bam]
                     self.process_sample(
                         bamlist,
                         outdir,
                         configs,
                         tmpdir,
+                        prog_cmd,
+                        num_threads,
                         dcov,
                         args.novcf,
                     )
                 else:
                     logging.warning(f"{args.bam} bam or bai file doesn't exist")
+            # multiple bams, multiprocess by sample
             elif args.list is not None:
                 with open(args.list) as f:
                     for line in f:
                         bam = line[:-1]
                         if os.path.exists(bam) and os.path.exists(bam + ".bai"):
                             bamlist.append(bam)
                         else:
                             logging.warning(f"{bam} bam or bai file doesn't exist")
 
-                num_threads = args.threads
                 process_sample_partial = partial(
                     self.process_sample,
                     outdir=outdir,
                     configs=configs,
                     tmpdir=tmpdir,
+                    prog_cmd=prog_cmd,
                     dcov=dcov,
                     novcf=args.novcf,
                 )
                 bam_groups = [bamlist[i::num_threads] for i in range(num_threads)]
                 pool = mp.Pool(num_threads)
                 pool.map(process_sample_partial, bam_groups)
                 pool.close()
@@ -449,11 +524,12 @@
             else:
                 raise Exception("No input file is given")
         except Exception:
             logging.error("Error running the program...See error message below")
             traceback.print_exc()
         finally:
             # remove temp dir
-            shutil.rmtree(tmpdir)
+            if os.path.exists(tmpdir):
+                shutil.rmtree(tmpdir)
             logging.info(
                 f"Completed Paraphase analysis at {datetime.datetime.now()}..."
             )
```

### Comparing `paraphase-2.2.2/paraphase/phaser.py` & `paraphase-2.2.3/paraphase/phaser.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import logging
 from scipy.stats import poisson
 from collections import namedtuple
 from .haplotype_assembler import VariantGraph
 
 
 class Phaser:
-
     clip_5p = r"^\d+S|^\d+H"
     clip_3p = r"\d+S$|\d+H$"
     deletion = r"\d+D"
     fields = [
         "total_cn",
         "gene_cn",
         "final_haplotypes",
@@ -421,19 +420,20 @@
             bases = bases_per_site[pos]
             bases_x = bases.count("x")
             bases_ref = bases.count("1")
             bases_alt = bases.count("2")
             this_var = self.het_sites[pos]
             if bases_x == len(bases):
                 sites_to_remove.append(this_var)
-            if bases_ref + bases_alt == len(bases) - bases_x and bases_alt <= 3:
+            elif bases_ref + bases_alt == len(bases) - bases_x and bases_alt <= 3:
                 if this_var not in kept_sites:
                     sites_to_remove.append(this_var)
         for var in sites_to_remove:
-            self.het_sites.remove(var)
+            if var in self.het_sites:
+                self.het_sites.remove(var)
 
     def allow_del_bases(self, pos):
         return False
 
     def process_indel(self, pos, ref_seq, var_seq):
         """Translate pysam indel seq into real sequence"""
         if "+" in var_seq:
@@ -1274,16 +1274,17 @@
             uniquely_supporting_reads,
             nonuniquely_supporting_reads,
             raw_read_haps,
             read_counts,
         ) = self.phase_haps(raw_read_haps)
 
         tmp = {}
+        mod_gene_name = ",".join(self.gene.split("-"))
         for i, hap in enumerate(ass_haps):
-            tmp.setdefault(hap, f"hap{i+1}")
+            tmp.setdefault(hap, f"{mod_gene_name}_hap{i+1}")
         ass_haps = tmp
 
         haplotypes = None
         dvar = None
         if ass_haps != {}:
             haplotypes, dvar = self.output_variants_in_haplotypes(
                 ass_haps,
@@ -1294,15 +1295,20 @@
         two_cp_haps = self.compare_depth(haplotypes)
         total_cn = len(ass_haps) + len(two_cp_haps)
 
         # phase
         alleles = []
         hap_links = {}
         if self.to_phase is True:
-            (alleles, hap_links, _, _,) = self.phase_alleles(
+            (
+                alleles,
+                hap_links,
+                _,
+                _,
+            ) = self.phase_alleles(
                 uniquely_supporting_reads,
                 nonuniquely_supporting_reads,
                 raw_read_haps,
                 ass_haps,
                 reverse=self.is_reverse,
             )
         self.close_handle()
```

### Comparing `paraphase-2.2.2/paraphase/prepare_bam_and_vcf.py` & `paraphase-2.2.3/paraphase/prepare_bam_and_vcf.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,29 +5,31 @@
 import os
 import pysam
 import subprocess
 import random
 import re
 from collections import Counter
 from .haplotype_assembler import VariantGraph
+import paraphase
 
 
 class BamRealigner:
     """
     Extract and realign reads to region of interest
     """
 
     min_mapq = 50
     min_aln = 800
     deletion = r"\d+D"
     insertion = r"\d+I"
 
-    def __init__(self, bam, outdir, config):
+    def __init__(self, bam, outdir, config, prog_cmd):
         self.bam = bam
         self.outdir = outdir
+        self.prog_cmd = prog_cmd
         self.gene = config["gene"]
         self.ref = config["data"]["reference"]
         self.nchr_old = config["nchr_old"]
         self.nchr = config["nchr"]
         self.offset = int(self.nchr_old.split("_")[1]) - 1
         self.nchr_length = config["nchr_length"]
         self.extract_regions = config["extract_regions"]
@@ -57,28 +59,47 @@
     def write_realign_bam(self):
         """
         Realign reads to region of interest and output a tagged bam for visualization
         """
         realign_cmd = (
             f"{self.samtools} view -F 0x100 -F 0x200 -F 0x800 {self.bam} {self.extract_regions} | sort | uniq | "
             + f'awk \'BEGIN {{FS="\\t"}} {{print "@" $1 "\\n" $10 "\\n+\\n" $11}}\''
-            + f" | {self.minimap2} -a -x map-pb {self.ref} - | {self.samtools} view -b | {self.samtools} sort > {self.realign_bam}"
+            + f" | {self.minimap2} -a -x map-pb {self.ref} - | {self.samtools} view -bh | {self.samtools} sort > {self.realign_bam}"
         )
         result = subprocess.run(realign_cmd, capture_output=True, text=True, shell=True)
         result.check_returncode()
         if os.path.exists(self.realign_bam) is False:
             raise Exception("Realigned bam does not exist.")
 
         pysam.index(self.realign_bam)
         realign_bamh = pysam.AlignmentFile(self.realign_bam, "rb")
+        realign_bamh_header = realign_bamh.header
+        realign_bamh_header = realign_bamh_header.to_dict()
+        pg_lines = []
+        pg_lines_original = realign_bamh_header.get("PG")
+        if pg_lines_original is not None:
+            pg_lines = [
+                a for a in pg_lines_original if "ID" in a and a["ID"] == "minimap2"
+            ]
+        pg_lines.append(
+            {
+                "PN": "paraphase",
+                "ID": "paraphase",
+                "VN": paraphase.__version__,
+                "CL": f"paraphase {self.prog_cmd}",
+            }
+        )
+        new_header = {
+            "SQ": [{"SN": self.nchr, "LN": self.nchr_length}],
+            "PG": pg_lines,
+        }
         realign_out_bamh = pysam.AlignmentFile(
             self.realign_out_bam,
             "wb",
-            reference_names=[self.nchr],
-            reference_lengths=[self.nchr_length],
+            header=new_header,
         )
         for read in realign_bamh.fetch(self.nchr_old):
             num_mismatch = self.get_nm(read)
             if (
                 read.mapping_quality >= self.min_mapq
                 and read.query_alignment_length >= self.min_aln
                 and num_mismatch < read.reference_length * self.max_mismatch
@@ -260,36 +281,36 @@
 
     def __init__(self, sample_id, outdir, call_sum):
         self.sample_id = sample_id
         self.outdir = outdir
         self.call_sum = call_sum
         self.match = {}
 
-    def set_parameter(self, config, tmpdir=None):
+    def set_parameter(self, config, tmpdir=None, prog_cmd=None):
         self.gene = config["gene"]
         self.nchr = config["nchr"]
         self.nchr_old = config["nchr_old"]
         self.offset = int(self.nchr_old.split("_")[1]) - 1
         self.nchr_length = config["nchr_length"]
         self.ref = config["data"]["reference"]
         self.samtools = config["tools"]["samtools"]
         self.minimap2 = config["tools"]["minimap2"]
         self.use_supplementary = False
         if "use_supplementary" in config:
             self.use_supplementary = config["use_supplementary"]
 
+        self.prog_cmd = prog_cmd
         self.tmpdir = tmpdir
         if self.tmpdir is None:
             self.tmpdir = self.outdir
         self.bam = os.path.join(
             tmpdir, self.sample_id + f"_{self.gene}_realigned_tagged.bam"
         )
         self.vcf_dir = os.path.join(self.outdir, f"{self.sample_id}_vcfs")
-        if os.path.exists(self.vcf_dir) is False:
-            os.makedirs(self.vcf_dir)
+        os.makedirs(self.vcf_dir, exist_ok=True)
 
     def get_range_in_other_gene(self, pos):
         """
         Find the correponding coordinates in the other gene
         """
         if pos in self.match:
             return self.match[pos]
@@ -305,14 +326,16 @@
         fout.write('##FILTER=<ID=PASS,Description="All filters passed">\n')
         fout.write('##FORMAT=<ID=GT,Number=1,Type=String,Description="Genotype">\n')
         fout.write('##FORMAT=<ID=DP,Number=1,Type=Integer,Description="Read depth">\n')
         fout.write(
             '##FORMAT=<ID=AD,Number=R,Type=Integer,Description="Read depth for each allele">\n'
         )
         fout.write(f"##contig=<ID={self.nchr},length={self.nchr_length}>\n")
+        fout.write(f"##paraphase_version={paraphase.__version__}\n")
+        fout.write(f"##paraphase_command=paraphase {self.prog_cmd}\n")
         header = [
             "#CHROM",
             "POS",
             "ID",
             "REF",
             "ALT",
             "QUAL",
@@ -765,16 +788,16 @@
     """
     Make vcf for two-gene scenario
     """
 
     def __init__(self, sample_id, outdir, call_sum):
         VcfGenerater.__init__(self, sample_id, outdir, call_sum)
 
-    def set_parameter(self, config, tmpdir=None):
-        super().set_parameter(config, tmpdir)
+    def set_parameter(self, config, tmpdir=None, prog_cmd=None):
+        super().set_parameter(config, tmpdir, prog_cmd)
         self.nchr_old_gene2 = config["nchr_old_smn2"]
         self.offset_gene2 = int(self.nchr_old_gene2.split("_")[1]) - 1
         self.ref_gene2 = config["data"]["reference_smn2"]
         self.position_match = config["data"]["smn_match"]
         with open(self.position_match) as f:
             for line in f:
                 at = line.split()
```

### Comparing `paraphase-2.2.2/paraphase.egg-info/PKG-INFO` & `paraphase-2.2.3/paraphase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paraphase
-Version: 2.2.2
+Version: 2.2.3
 Summary: paraphase: HiFi-based caller for highly homologous genes
 Home-page: https://github.com/PacificBiosciences/paraphase
 Author: Xiao Chen
 Author-email: xchen@pacificbiosciences.com
 License: BSD-3-Clause-Clear
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `paraphase-2.2.2/paraphase.egg-info/SOURCES.txt` & `paraphase-2.2.3/paraphase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.2/setup.py` & `paraphase-2.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.2/tests/test_haplotype_assembler.py` & `paraphase-2.2.3/tests/test_haplotype_assembler.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.2/tests/test_paraphase.py` & `paraphase-2.2.3/tests/test_paraphase.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.2/tests/test_phaser.py` & `paraphase-2.2.3/tests/test_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.2/tests/test_prepare_bam_and_vcf.py` & `paraphase-2.2.3/tests/test_prepare_bam_and_vcf.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.2/tests/test_rccx_phaser.py` & `paraphase-2.2.3/tests/test_rccx_phaser.py`

 * *Files identical despite different names*

### Comparing `paraphase-2.2.2/tests/test_smn1_phaser.py` & `paraphase-2.2.3/tests/test_smn1_phaser.py`

 * *Files identical despite different names*

