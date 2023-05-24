# Comparing `tmp/ifiscripts-2023.1.9.1.tar.gz` & `tmp/ifiscripts-2023.5.10.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifiscripts-2023.1.9.1.tar", last modified: Mon Jan  9 12:57:50 2023, max compression
+gzip compressed data, was "ifiscripts-2023.5.10.1.tar", last modified: Wed May 10 11:36:58 2023, max compression
```

## Comparing `ifiscripts-2023.1.9.1.tar` & `ifiscripts-2023.5.10.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-01-09 12:57:50.133765 ifiscripts-2023.1.9.1/
--rw-rw-rw-   0        0        0   970313 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/26_XYZ-22_Rec709.cube
--rw-rw-rw-   0        0        0     1116 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/LICENSE.txt
--rw-rw-rw-   0        0        0       70 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1129 2023-01-09 12:57:50.133765 ifiscripts-2023.1.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     4611 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/README.rst
--rw-rw-rw-   0        0        0     5029 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/film_scan_aip_documentation.txt
-drwxrwxrwx   0        0        0        0 2023-01-09 12:57:49.856290 ifiscripts-2023.1.9.1/ifiscripts.egg-info/
--rw-rw-rw-   0        0        0     1129 2023-01-09 12:57:49.000000 ifiscripts-2023.1.9.1/ifiscripts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1666 2023-01-09 12:57:49.000000 ifiscripts-2023.1.9.1/ifiscripts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-09 12:57:49.000000 ifiscripts-2023.1.9.1/ifiscripts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-01-09 12:57:49.000000 ifiscripts-2023.1.9.1/ifiscripts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-01-09 12:57:49.000000 ifiscripts-2023.1.9.1/ifiscripts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-09 12:57:49.929840 ifiscripts-2023.1.9.1/legacy_scripts/
--rw-rw-rw-   0        0        0     2872 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/legacy_scripts/batchfixity.py
--rw-rw-rw-   0        0        0     1599 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/legacy_scripts/db_cleaning.py
--rw-rw-rw-   0        0        0    11222 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/legacy_scripts/dpxonly.py
--rw-rw-rw-   0        0        0     5019 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/legacy_scripts/dvsip.py
--rw-rw-rw-   0        0        0     1004 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/legacy_scripts/giffer.py
--rw-rw-rw-   0        0        0      989 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/legacy_scripts/loopline.py
--rw-rw-rw-   0        0        0    11528 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/legacy_scripts/makedpx.py
--rw-rw-rw-   0        0        0      851 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/legacy_scripts/mezzaninecheck.py
--rw-rw-rw-   0        0        0     1720 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/legacy_scripts/oeremove.py
--rw-rw-rw-   0        0        0     3803 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/legacy_scripts/pg.py
--rw-rw-rw-   0        0        0     3065 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/legacy_scripts/playerseq.py
--rw-rw-rw-   0        0        0    21971 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/legacy_scripts/premisgui.py
--rw-rw-rw-   0        0        0     2658 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/legacy_scripts/qctools.py
--rw-rw-rw-   0        0        0    15738 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/legacy_scripts/rawbatch.py
--rw-rw-rw-   0        0        0      421 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/legacy_scripts/renumber.py
--rw-rw-rw-   0        0        0    67554 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/legacy_scripts/revtmd.py
--rw-rw-rw-   0        0        0     1316 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/legacy_scripts/sha512deep.py
-drwxrwxrwx   0        0        0        0 2023-01-09 12:57:50.133765 ifiscripts-2023.1.9.1/scripts/
--rw-rw-rw-   0        0        0   123258 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/Objects.py
--rw-rw-rw-   0        0        0    12189 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/accession.py
--rw-rw-rw-   0        0        0     3710 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/accession_register.py
--rw-rw-rw-   0        0        0     8952 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/as11fixity.py
--rw-rw-rw-   0        0        0    16639 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/batchaccession.py
--rw-rw-rw-   0        0        0     2582 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/batchmakeshell.py
--rw-rw-rw-   0        0        0     6005 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/batchsipcreator.py
--rw-rw-rw-   0        0        0     9396 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/bitc.py
--rw-rw-rw-   0        0        0    10479 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/concat.py
--rw-rw-rw-   0        0        0    32639 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/copyit.py
--rw-rw-rw-   0        0        0    23142 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/dcpaccess.py
--rw-rw-rw-   0        0        0    13705 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/dcpfixity.py
--rw-rw-rw-   0        0        0     4813 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/deletefiles.py
--rw-rw-rw-   0        0        0    68625 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/dfxml.py
--rw-rw-rw-   0        0        0      804 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/durationcheck.py
--rw-rw-rw-   0        0        0     7327 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/ffv1mkvvalidate.py
--rw-rw-rw-   0        0        0     1903 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/framemd5.py
--rw-rw-rw-   0        0        0    78362 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/ififuncs.py
--rw-rw-rw-   0        0        0    12437 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/loopline_repackage.py
--rw-rw-rw-   0        0        0     3668 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/make_mediaconch.py
--rw-rw-rw-   0        0        0     1628 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/makedfxml.py
--rw-rw-rw-   0        0        0     3680 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/makedip.py
--rw-rw-rw-   0        0        0    12126 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/makeffv1.py
--rw-rw-rw-   0        0        0    32173 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/makepbcore.py
--rw-rw-rw-   0        0        0      300 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/makeuuid.py
--rw-rw-rw-   0        0        0     3414 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/makezip.py
--rw-rw-rw-   0        0        0     6947 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/manifest.py
--rw-rw-rw-   0        0        0     5708 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/masscopy.py
--rw-rw-rw-   0        0        0      971 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/massqc.py
--rw-rw-rw-   0        0        0      755 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/mergepbcore.py
--rw-rw-rw-   0        0        0     1983 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/multicopy.py
--rw-rw-rw-   0        0        0    10584 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/normalise.py
--rw-rw-rw-   0        0        0     2695 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/order.py
--rw-rw-rw-   0        0        0     6649 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/package_update.py
--rw-rw-rw-   0        0        0     3853 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/packagecheck.py
--rw-rw-rw-   0        0        0     4846 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/prores.py
--rw-rw-rw-   0        0        0    15379 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/seq2ffv1.py
--rw-rw-rw-   0        0        0    26699 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/sipcreator.py
--rw-rw-rw-   0        0        0     4440 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/strongbox_fixity.py
--rw-rw-rw-   0        0        0     2682 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/subfolders.py
--rw-rw-rw-   0        0        0     3927 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/testfiles.py
--rw-rw-rw-   0        0        0     9842 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/validate.py
--rw-rw-rw-   0        0        0     7154 2023-01-09 12:53:28.000000 ifiscripts-2023.1.9.1/scripts/walk_to_dfxml.py
--rw-rw-rw-   0        0        0       42 2023-01-09 12:57:50.133765 ifiscripts-2023.1.9.1/setup.cfg
--rw-rw-rw-   0        0        0     3040 2023-01-09 12:57:46.000000 ifiscripts-2023.1.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:36:58.882762 ifiscripts-2023.5.10.1/
+-rw-rw-rw-   0        0        0   970313 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/26_XYZ-22_Rec709.cube
+-rw-rw-rw-   0        0        0     1116 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       70 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1130 2023-05-10 11:36:58.882762 ifiscripts-2023.5.10.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4611 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/README.rst
+-rw-rw-rw-   0        0        0     5029 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/film_scan_aip_documentation.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 11:36:58.797292 ifiscripts-2023.5.10.1/ifiscripts.egg-info/
+-rw-rw-rw-   0        0        0     1130 2023-05-10 11:36:58.000000 ifiscripts-2023.5.10.1/ifiscripts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1666 2023-05-10 11:36:58.000000 ifiscripts-2023.5.10.1/ifiscripts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 11:36:58.000000 ifiscripts-2023.5.10.1/ifiscripts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-10 11:36:58.000000 ifiscripts-2023.5.10.1/ifiscripts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-10 11:36:58.000000 ifiscripts-2023.5.10.1/ifiscripts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 11:36:58.821919 ifiscripts-2023.5.10.1/legacy_scripts/
+-rw-rw-rw-   0        0        0     2872 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/legacy_scripts/batchfixity.py
+-rw-rw-rw-   0        0        0     1599 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/legacy_scripts/db_cleaning.py
+-rw-rw-rw-   0        0        0    11222 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/legacy_scripts/dpxonly.py
+-rw-rw-rw-   0        0        0     5019 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/legacy_scripts/dvsip.py
+-rw-rw-rw-   0        0        0     1004 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/legacy_scripts/giffer.py
+-rw-rw-rw-   0        0        0      989 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/legacy_scripts/loopline.py
+-rw-rw-rw-   0        0        0    11528 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/legacy_scripts/makedpx.py
+-rw-rw-rw-   0        0        0      851 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/legacy_scripts/mezzaninecheck.py
+-rw-rw-rw-   0        0        0     1720 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/legacy_scripts/oeremove.py
+-rw-rw-rw-   0        0        0     3803 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/legacy_scripts/pg.py
+-rw-rw-rw-   0        0        0     3065 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/legacy_scripts/playerseq.py
+-rw-rw-rw-   0        0        0    21971 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/legacy_scripts/premisgui.py
+-rw-rw-rw-   0        0        0     2658 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/legacy_scripts/qctools.py
+-rw-rw-rw-   0        0        0    15738 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/legacy_scripts/rawbatch.py
+-rw-rw-rw-   0        0        0      421 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/legacy_scripts/renumber.py
+-rw-rw-rw-   0        0        0    67554 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/legacy_scripts/revtmd.py
+-rw-rw-rw-   0        0        0     1316 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/legacy_scripts/sha512deep.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:36:58.880762 ifiscripts-2023.5.10.1/scripts/
+-rw-rw-rw-   0        0        0   123258 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/Objects.py
+-rw-rw-rw-   0        0        0    12189 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/accession.py
+-rw-rw-rw-   0        0        0     3710 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/accession_register.py
+-rw-rw-rw-   0        0        0     8952 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/as11fixity.py
+-rw-rw-rw-   0        0        0    16639 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/batchaccession.py
+-rw-rw-rw-   0        0        0     2582 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/batchmakeshell.py
+-rw-rw-rw-   0        0        0     6005 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/batchsipcreator.py
+-rw-rw-rw-   0        0        0     9396 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/bitc.py
+-rw-rw-rw-   0        0        0    10479 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/concat.py
+-rw-rw-rw-   0        0        0    32639 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/copyit.py
+-rw-rw-rw-   0        0        0    23142 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/dcpaccess.py
+-rw-rw-rw-   0        0        0    13705 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/dcpfixity.py
+-rw-rw-rw-   0        0        0     4813 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/deletefiles.py
+-rw-rw-rw-   0        0        0    68625 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/dfxml.py
+-rw-rw-rw-   0        0        0      804 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/durationcheck.py
+-rw-rw-rw-   0        0        0     7327 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/ffv1mkvvalidate.py
+-rw-rw-rw-   0        0        0     1903 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/framemd5.py
+-rw-rw-rw-   0        0        0    77782 2023-05-10 11:12:55.000000 ifiscripts-2023.5.10.1/scripts/ififuncs.py
+-rw-rw-rw-   0        0        0    12437 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/loopline_repackage.py
+-rw-rw-rw-   0        0        0     3668 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/make_mediaconch.py
+-rw-rw-rw-   0        0        0     1628 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/makedfxml.py
+-rw-rw-rw-   0        0        0     3680 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/makedip.py
+-rw-rw-rw-   0        0        0    12126 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/makeffv1.py
+-rw-rw-rw-   0        0        0    32173 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/makepbcore.py
+-rw-rw-rw-   0        0        0      300 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/makeuuid.py
+-rw-rw-rw-   0        0        0     3414 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/makezip.py
+-rw-rw-rw-   0        0        0     6947 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/manifest.py
+-rw-rw-rw-   0        0        0     5708 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/masscopy.py
+-rw-rw-rw-   0        0        0      971 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/massqc.py
+-rw-rw-rw-   0        0        0      755 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/mergepbcore.py
+-rw-rw-rw-   0        0        0     1983 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/multicopy.py
+-rw-rw-rw-   0        0        0    10584 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/normalise.py
+-rw-rw-rw-   0        0        0     2695 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/order.py
+-rw-rw-rw-   0        0        0     6649 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/package_update.py
+-rw-rw-rw-   0        0        0     3853 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/packagecheck.py
+-rw-rw-rw-   0        0        0     4935 2023-02-09 14:21:08.000000 ifiscripts-2023.5.10.1/scripts/prores.py
+-rw-rw-rw-   0        0        0    15379 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/seq2ffv1.py
+-rw-rw-rw-   0        0        0    26699 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/sipcreator.py
+-rw-rw-rw-   0        0        0     4440 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/strongbox_fixity.py
+-rw-rw-rw-   0        0        0     2682 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/subfolders.py
+-rw-rw-rw-   0        0        0     3927 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/testfiles.py
+-rw-rw-rw-   0        0        0     9842 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/validate.py
+-rw-rw-rw-   0        0        0     7154 2023-01-09 12:53:28.000000 ifiscripts-2023.5.10.1/scripts/walk_to_dfxml.py
+-rw-rw-rw-   0        0        0       42 2023-05-10 11:36:58.882762 ifiscripts-2023.5.10.1/setup.cfg
+-rw-rw-rw-   0        0        0     3040 2023-05-10 11:14:52.000000 ifiscripts-2023.5.10.1/setup.py
```

### Comparing `ifiscripts-2023.1.9.1/26_XYZ-22_Rec709.cube` & `ifiscripts-2023.5.10.1/26_XYZ-22_Rec709.cube`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/LICENSE.txt` & `ifiscripts-2023.5.10.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/PKG-INFO` & `ifiscripts-2023.5.10.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifiscripts
-Version: 2023.1.9.1
+Version: 2023.5.10.1
 Summary: Scripts for processing moving image material in the Irish Film Institute/Irish Film Archive
 Author: Kieran O'Leary
 Author-email: kieran.o.leary@gmail.com
 License: MIT
 Requires-Python: >=3.8
 License-File: LICENSE.txt
```

### Comparing `ifiscripts-2023.1.9.1/README.rst` & `ifiscripts-2023.5.10.1/README.rst`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/film_scan_aip_documentation.txt` & `ifiscripts-2023.5.10.1/film_scan_aip_documentation.txt`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/ifiscripts.egg-info/PKG-INFO` & `ifiscripts-2023.5.10.1/ifiscripts.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifiscripts
-Version: 2023.1.9.1
+Version: 2023.5.10.1
 Summary: Scripts for processing moving image material in the Irish Film Institute/Irish Film Archive
 Author: Kieran O'Leary
 Author-email: kieran.o.leary@gmail.com
 License: MIT
 Requires-Python: >=3.8
 License-File: LICENSE.txt
```

### Comparing `ifiscripts-2023.1.9.1/ifiscripts.egg-info/SOURCES.txt` & `ifiscripts-2023.5.10.1/ifiscripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/legacy_scripts/batchfixity.py` & `ifiscripts-2023.5.10.1/legacy_scripts/batchfixity.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/legacy_scripts/db_cleaning.py` & `ifiscripts-2023.5.10.1/legacy_scripts/db_cleaning.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/legacy_scripts/dpxonly.py` & `ifiscripts-2023.5.10.1/legacy_scripts/dpxonly.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/legacy_scripts/dvsip.py` & `ifiscripts-2023.5.10.1/legacy_scripts/dvsip.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/legacy_scripts/giffer.py` & `ifiscripts-2023.5.10.1/legacy_scripts/giffer.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/legacy_scripts/loopline.py` & `ifiscripts-2023.5.10.1/legacy_scripts/loopline.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/legacy_scripts/makedpx.py` & `ifiscripts-2023.5.10.1/legacy_scripts/makedpx.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/legacy_scripts/mezzaninecheck.py` & `ifiscripts-2023.5.10.1/legacy_scripts/mezzaninecheck.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/legacy_scripts/oeremove.py` & `ifiscripts-2023.5.10.1/legacy_scripts/oeremove.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/legacy_scripts/pg.py` & `ifiscripts-2023.5.10.1/legacy_scripts/pg.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/legacy_scripts/playerseq.py` & `ifiscripts-2023.5.10.1/legacy_scripts/playerseq.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/legacy_scripts/premisgui.py` & `ifiscripts-2023.5.10.1/legacy_scripts/premisgui.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/legacy_scripts/qctools.py` & `ifiscripts-2023.5.10.1/legacy_scripts/qctools.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/legacy_scripts/rawbatch.py` & `ifiscripts-2023.5.10.1/legacy_scripts/rawbatch.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/legacy_scripts/revtmd.py` & `ifiscripts-2023.5.10.1/legacy_scripts/revtmd.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/legacy_scripts/sha512deep.py` & `ifiscripts-2023.5.10.1/legacy_scripts/sha512deep.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/Objects.py` & `ifiscripts-2023.5.10.1/scripts/Objects.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/accession.py` & `ifiscripts-2023.5.10.1/scripts/accession.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/accession_register.py` & `ifiscripts-2023.5.10.1/scripts/accession_register.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/as11fixity.py` & `ifiscripts-2023.5.10.1/scripts/as11fixity.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/batchaccession.py` & `ifiscripts-2023.5.10.1/scripts/batchaccession.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/batchmakeshell.py` & `ifiscripts-2023.5.10.1/scripts/batchmakeshell.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/batchsipcreator.py` & `ifiscripts-2023.5.10.1/scripts/batchsipcreator.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/bitc.py` & `ifiscripts-2023.5.10.1/scripts/bitc.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/concat.py` & `ifiscripts-2023.5.10.1/scripts/concat.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/copyit.py` & `ifiscripts-2023.5.10.1/scripts/copyit.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/dcpaccess.py` & `ifiscripts-2023.5.10.1/scripts/dcpaccess.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/dcpfixity.py` & `ifiscripts-2023.5.10.1/scripts/dcpfixity.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/deletefiles.py` & `ifiscripts-2023.5.10.1/scripts/deletefiles.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/dfxml.py` & `ifiscripts-2023.5.10.1/scripts/dfxml.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/durationcheck.py` & `ifiscripts-2023.5.10.1/scripts/durationcheck.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/ffv1mkvvalidate.py` & `ifiscripts-2023.5.10.1/scripts/ffv1mkvvalidate.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/framemd5.py` & `ifiscripts-2023.5.10.1/scripts/framemd5.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/ififuncs.py` & `ifiscripts-2023.5.10.1/scripts/ififuncs.py`

 * *Files 2% similar despite different names*

```diff
@@ -721,70 +721,55 @@
     log_dir = "%s/logs" % path
     data_dir = "%s/objects" % path
     # Actually create the directories.
     os.makedirs(metadata_dir)
     os.makedirs(data_dir)
     os.makedirs(log_dir)
 
-
+    
 def get_user():
     '''
     Asks user who they are. Returns a string with their name
     '''
     user = ''
-    if user not in ('1', '2', '3', '4', '5', '6', '7', '8', '9', '10', '11', '12', '13', '14'):
+    if user not in ('1', '2', '3', '4', '5', '6', '7', '8', '9'):
         user = input(
-            '\n\n**** Who are you?\nPress 1,2,3,4,5,6,7,8,9,10,11,12,13,14\n\n1.\tKieran O\'Leary\n2.\tRaelene Casey\n3.\tAoife Fitzmaurice\n4.\tYujing Huang\n5.\tNoelia Romero\n6.\tAna Truchanova\n7.\tEoin O\'Donohoe\n8.\tGavin Martin\n9.\tNiamh Murphy\n10.\tRaven Cooke\n11.\tNiall Anderson\n12.\tYazhou He\n13.\tCaroline Crowther\n14.\tMark Keleghan\n'
+            '\n\n**** Who are you?\nPress 1,2,3,4,5,6,7,8,9,10\n\n1.\tCaroline Crowther\n2.\tEmma Battlebury\n3.\tGavin Martin\n4.\tMark Keleghan\n5.\tNiall Anderson\n6.\tNoelia Romero\n7.\tRaelene Casey\n8.\tRaven Cooke\n9.\tYazhou He\n\n(User list was last updated on 2023-05-10)\n'
         )
-        while user not in ('1', '2', '3', '4', '5', '6', '7', '8', '9', '10', '11', '12', '13', '14'):
+        while user not in ('1', '2', '3', '4', '5', '6', '7', '8', '9'):
             user = input(
-                '\n\n**** Who are you?\nPress 1,2,3,4,5,6,7,8,9,10,11,12,13,14\n\n1.\tKieran O\'Leary\n2.\tRaelene Casey\n3.\tAoife Fitzmaurice\n4.\tYujing Huang\n5.\tNoelia Romero\n6.\tAna Truchanova\n7.\tEoin O\'Donohoe\n8.\tGavin Martin\n9.\tNiamh Murphy\n10.\tRaven Cooke\n11.\tNiall Anderson\n12.\tYazhou He\n13.\tCaroline Crowther\n14.\tMark Keleghan\n'
+            '\n\n**** Who are you?\nPress 1,2,3,4,5,6,7,8,9,10\n\n1.\tCaroline Crowther\n2.\tEmma Battlebury\n3.\tGavin Martin\n4.\tMark Keleghan\n5.\tNiall Anderson\n6.\tNoelia Romero\n7.\tRaelene Casey\n8.\tRaven Cooke\n9.\tYazhou He\n\n(User list was last updated on 2023-05-10)\n'
             )
     if user == '1':
-        user = 'Kieran O\'Leary'
+        user = 'Caroline Crowther'
         time.sleep(1)
     elif user == '2':
-        user = 'Raelene Casey'
+        user = 'Emma Battlebury'
         time.sleep(1)
     elif user == '3':
-        user = 'Aoife Fitzmaurice'
+        user = 'Gavin Martin'
         time.sleep(1)
     elif user == '4':
-        user = 'Yujing Huang'
+        user = 'Mark Keleghan'
         time.sleep(1)
     elif user == '5':
-        user = 'Noelia Romero'
+        user = 'Niall Anderson'
         time.sleep(1)
     elif user == '6':
-        user = 'Ana Truchanova'
+        user = 'Noelia Romero'
         time.sleep(1)
     elif user == '7':
-        user = 'Eoin O\'Donohoe'
+        user = 'Raelene Casey'
         time.sleep(1)
     elif user == '8':
-        user = 'Gavin Martin'
-        time.sleep(1)
-    elif user == '9':
-        user = 'Niamh Murphy'
-        time.sleep(1)
-    elif user == '10':
         user = 'Raven Cooke'
         time.sleep(1)
-    elif user == '11':
-        user = 'Niall Anderson'
-        time.sleep(1)
-    elif user == '12':
+    elif user == '9':
         user = 'Yazhou He'
         time.sleep(1)
-    elif user == '13':
-        user = 'Caroline Crowther'
-        time.sleep(1)
-    elif user == '14':
-        user = 'Mark Keleghan'
-        time.sleep(1)
     return user
 
 
 def determine_user(args):
     '''
     Determine who is the user.
     UNITTEST - check if user is a string. Use mock to simulate input.
@@ -1470,15 +1455,15 @@
 def recursive_file_list(video_files):
     '''
     Recursively searches through directories for AV files and adds to a list.
     '''
     recursive_list = []
     for root, _, filenames in os.walk(video_files):
         for filename in filenames:
-            if filename.endswith(('.MP4', '.mp4', '.MOV', '.mov', '.mkv', '.mxf', '.MXF', '.WAV', '.wav', '.aiff', '.AIFF', 'mp3', 'MP3', 'm2t', '.dv', '.DV', '.iso', '.ISO')):
+            if filename.endswith(('.MP4', '.mp4', '.MOV', '.mov', '.mkv', '.mxf', '.MXF', '.WAV', '.wav', '.aiff', '.AIFF', 'mp3', 'MP3', 'm2t', 'MTS', '.dv', '.DV', '.iso', '.ISO')):
                 recursive_list.append(os.path.join(root, filename))
     return recursive_list
 
 
 def get_video_files(source):
     '''
     Generates a list of video files.
```

### Comparing `ifiscripts-2023.1.9.1/scripts/loopline_repackage.py` & `ifiscripts-2023.5.10.1/scripts/loopline_repackage.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/make_mediaconch.py` & `ifiscripts-2023.5.10.1/scripts/make_mediaconch.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/makedfxml.py` & `ifiscripts-2023.5.10.1/scripts/makedfxml.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/makedip.py` & `ifiscripts-2023.5.10.1/scripts/makedip.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/makeffv1.py` & `ifiscripts-2023.5.10.1/scripts/makeffv1.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/makepbcore.py` & `ifiscripts-2023.5.10.1/scripts/makepbcore.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/makezip.py` & `ifiscripts-2023.5.10.1/scripts/makezip.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/manifest.py` & `ifiscripts-2023.5.10.1/scripts/manifest.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/masscopy.py` & `ifiscripts-2023.5.10.1/scripts/masscopy.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/massqc.py` & `ifiscripts-2023.5.10.1/scripts/massqc.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/mergepbcore.py` & `ifiscripts-2023.5.10.1/scripts/mergepbcore.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/multicopy.py` & `ifiscripts-2023.5.10.1/scripts/multicopy.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/normalise.py` & `ifiscripts-2023.5.10.1/scripts/normalise.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/order.py` & `ifiscripts-2023.5.10.1/scripts/order.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/package_update.py` & `ifiscripts-2023.5.10.1/scripts/package_update.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/packagecheck.py` & `ifiscripts-2023.5.10.1/scripts/packagecheck.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/prores.py` & `ifiscripts-2023.5.10.1/scripts/prores.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,14 +119,16 @@
             ffmpeg_args.append('0:a?')
             ffmpeg_args.append('-map')
             ffmpeg_args.append('0:v')
                 
         if args.hq:
             ffmpeg_args.append('-profile:v')
             ffmpeg_args.append('3')
+            ffmpeg_args.append('-pix_fmt')
+            ffmpeg_args.append('yuv422p10le')
         if args.wide:
             ffmpeg_args.append('-aspect')
             ffmpeg_args.append('16:9')
         if args.yadif or args.scale:
         
             filter_options = '-vf'
```

### Comparing `ifiscripts-2023.1.9.1/scripts/seq2ffv1.py` & `ifiscripts-2023.5.10.1/scripts/seq2ffv1.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/sipcreator.py` & `ifiscripts-2023.5.10.1/scripts/sipcreator.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/strongbox_fixity.py` & `ifiscripts-2023.5.10.1/scripts/strongbox_fixity.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/subfolders.py` & `ifiscripts-2023.5.10.1/scripts/subfolders.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/testfiles.py` & `ifiscripts-2023.5.10.1/scripts/testfiles.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/validate.py` & `ifiscripts-2023.5.10.1/scripts/validate.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/scripts/walk_to_dfxml.py` & `ifiscripts-2023.5.10.1/scripts/walk_to_dfxml.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.1.9.1/setup.py` & `ifiscripts-2023.5.10.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,10 +71,10 @@
         'dicttoxml',
         'future',
         'clairmeta'
     ],
     data_files=[('', ['film_scan_aip_documentation.txt', '26_XYZ-22_Rec709.cube'])],
     include_package_data=True,
     name='ifiscripts',
-    version='2023.01.09.1',
+    version='2023.05.10.1',
     python_requires='>=3.8'
 )
```

