# Comparing `tmp/seislib-0.6.8.tar.gz` & `tmp/seislib-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seislib-0.6.8.tar", last modified: Tue Apr  4 23:59:17 2023, max compression
+gzip compressed data, was "seislib-0.6.9.tar", last modified: Thu Apr  6 05:40:56 2023, max compression
```

## Comparing `seislib-0.6.8.tar` & `seislib-0.6.9.tar`

### file list

```diff
@@ -1,439 +1,439 @@
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.833682 seislib-0.6.8/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1073 2023-04-03 03:52:42.000000 seislib-0.6.8/LICENSE.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      457 2023-04-03 03:52:42.000000 seislib-0.6.8/MANIFEST.in
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5278 2023-04-04 23:59:17.833682 seislib-0.6.8/PKG-INFO
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     4724 2023-04-03 03:52:42.000000 seislib-0.6.8/README.md
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.813682 seislib-0.6.8/seislib/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      373 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      258 2023-04-04 23:54:01.000000 seislib-0.6.8/seislib/__version__.py
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.813682 seislib-0.6.8/seislib/an/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3210 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/an/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    84409 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/an/an_attenuation.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    39923 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/an/an_downloader.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    67691 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/an/an_processing.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    37165 2023-04-04 23:48:09.000000 seislib-0.6.8/seislib/an/an_velocity.py
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.817682 seislib-0.6.8/seislib/colormaps/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)   115362 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/+LICENCE.pdf
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)   876959 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/+README_ScientificColourMaps-6.pdf
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)   324037 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/+ScientificColourMapsGuideline_Crameri_EtAl2020.pdf
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1348 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/__init__.py
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.817682 seislib-0.6.8/seislib/colormaps/acton/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.817682 seislib-0.6.8/seislib/colormaps/acton/CategoricalPalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5289 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/acton/CategoricalPalettes/actonS.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/acton/CategoricalPalettes/actonS.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3026 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/acton/CategoricalPalettes/actonS_HEX.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.817682 seislib-0.6.8/seislib/colormaps/acton/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      355 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/acton/DiscretePalettes/acton10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3018 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/acton/DiscretePalettes/acton100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      799 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/acton/DiscretePalettes/acton25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1539 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/acton/DiscretePalettes/acton50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/acton/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12422 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/acton/acton.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/acton/acton.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.817682 seislib-0.6.8/seislib/colormaps/bam/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.817682 seislib-0.6.8/seislib/colormaps/bam/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      333 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bam/DiscretePalettes/bam10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2816 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bam/DiscretePalettes/bam100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      747 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bam/DiscretePalettes/bam25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1437 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bam/DiscretePalettes/bam50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bam/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12399 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bam/bam.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bam/bam.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.817682 seislib-0.6.8/seislib/colormaps/bamO/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.817682 seislib-0.6.8/seislib/colormaps/bamO/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      344 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bamO/DiscretePalettes/bamO10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2917 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bamO/DiscretePalettes/bamO100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      773 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bamO/DiscretePalettes/bamO25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1488 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bamO/DiscretePalettes/bamO50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bamO/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12400 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bamO/bamO.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bamO/bamO.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.817682 seislib-0.6.8/seislib/colormaps/bamako/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.817682 seislib-0.6.8/seislib/colormaps/bamako/CategoricalPalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5337 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bamako/CategoricalPalettes/bamakoS.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bamako/CategoricalPalettes/bamakoS.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3130 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bamako/CategoricalPalettes/bamakoS_HEX.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.817682 seislib-0.6.8/seislib/colormaps/bamako/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      366 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bamako/DiscretePalettes/bamako10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3119 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bamako/DiscretePalettes/bamako100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      825 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bamako/DiscretePalettes/bamako25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1590 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bamako/DiscretePalettes/bamako50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bamako/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12513 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bamako/bamako.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bamako/bamako.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.817682 seislib-0.6.8/seislib/colormaps/batlow/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.817682 seislib-0.6.8/seislib/colormaps/batlow/CategoricalPalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5318 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlow/CategoricalPalettes/batlowS.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlow/CategoricalPalettes/batlowS.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3129 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlow/CategoricalPalettes/batlowS_HEX.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.817682 seislib-0.6.8/seislib/colormaps/batlow/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      366 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlow/DiscretePalettes/batlow10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3119 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlow/DiscretePalettes/batlow100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      825 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlow/DiscretePalettes/batlow25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1590 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlow/DiscretePalettes/batlow50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlow/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12463 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlow/batlow.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlow/batlow.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.817682 seislib-0.6.8/seislib/colormaps/batlowK/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.817682 seislib-0.6.8/seislib/colormaps/batlowK/CategoricalPalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5309 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlowK/CategoricalPalettes/batlowKS.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlowK/CategoricalPalettes/batlowKS.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3230 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlowK/CategoricalPalettes/batlowKS_HEX.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.817682 seislib-0.6.8/seislib/colormaps/batlowK/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      377 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlowK/DiscretePalettes/batlowK10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3220 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlowK/DiscretePalettes/batlowK100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      851 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlowK/DiscretePalettes/batlowK25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1641 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlowK/DiscretePalettes/batlowK50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlowK/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12462 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlowK/batlowK.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlowK/batlowK.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.817682 seislib-0.6.8/seislib/colormaps/batlowW/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.817682 seislib-0.6.8/seislib/colormaps/batlowW/CategoricalPalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5282 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlowW/CategoricalPalettes/batlowWS.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlowW/CategoricalPalettes/batlowWS.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3235 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlowW/CategoricalPalettes/batlowWS_HEX.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.817682 seislib-0.6.8/seislib/colormaps/batlowW/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      377 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlowW/DiscretePalettes/batlowW10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3220 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlowW/DiscretePalettes/batlowW100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      851 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlowW/DiscretePalettes/batlowW25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1641 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlowW/DiscretePalettes/batlowW50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlowW/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12363 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlowW/batlowW.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/batlowW/batlowW.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/berlin/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/berlin/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      366 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/berlin/DiscretePalettes/berlin10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3119 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/berlin/DiscretePalettes/berlin100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      825 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/berlin/DiscretePalettes/berlin25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1590 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/berlin/DiscretePalettes/berlin50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/berlin/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12620 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/berlin/berlin.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/berlin/berlin.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/bilbao/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/bilbao/CategoricalPalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5312 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bilbao/CategoricalPalettes/bilbaoS.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bilbao/CategoricalPalettes/bilbaoS.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3128 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bilbao/CategoricalPalettes/bilbaoS_HEX.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/bilbao/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      366 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bilbao/DiscretePalettes/bilbao10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3119 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bilbao/DiscretePalettes/bilbao100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      825 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bilbao/DiscretePalettes/bilbao25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1590 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bilbao/DiscretePalettes/bilbao50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bilbao/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12446 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bilbao/bilbao.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bilbao/bilbao.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/broc/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/broc/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      344 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/broc/DiscretePalettes/broc10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2917 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/broc/DiscretePalettes/broc100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      773 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/broc/DiscretePalettes/broc25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1488 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/broc/DiscretePalettes/broc50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/broc/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12423 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/broc/broc.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/broc/broc.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/brocO/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/brocO/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      355 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/brocO/DiscretePalettes/brocO10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3018 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/brocO/DiscretePalettes/brocO100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      799 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/brocO/DiscretePalettes/brocO25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1539 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/brocO/DiscretePalettes/brocO50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/brocO/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12412 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/brocO/brocO.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/brocO/brocO.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/buda/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/buda/CategoricalPalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5266 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/buda/CategoricalPalettes/budaS.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/buda/CategoricalPalettes/budaS.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2928 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/buda/CategoricalPalettes/budaS_HEX.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/buda/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      344 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/buda/DiscretePalettes/buda10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2917 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/buda/DiscretePalettes/buda100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      773 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/buda/DiscretePalettes/buda25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1488 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/buda/DiscretePalettes/buda50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/buda/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12387 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/buda/buda.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/buda/buda.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/bukavu/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/bukavu/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      366 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bukavu/DiscretePalettes/bukavu10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3119 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bukavu/DiscretePalettes/bukavu100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      825 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bukavu/DiscretePalettes/bukavu25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1590 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bukavu/DiscretePalettes/bukavu50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bukavu/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12451 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bukavu/bukavu.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/bukavu/bukavu.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/cork/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/cork/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      344 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/cork/DiscretePalettes/cork10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2917 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/cork/DiscretePalettes/cork100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      773 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/cork/DiscretePalettes/cork25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1488 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/cork/DiscretePalettes/cork50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/cork/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12461 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/cork/cork.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/cork/cork.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/corkO/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/corkO/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      355 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/corkO/DiscretePalettes/corkO10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3018 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/corkO/DiscretePalettes/corkO100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      799 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/corkO/DiscretePalettes/corkO25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1539 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/corkO/DiscretePalettes/corkO50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/corkO/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12414 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/corkO/corkO.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/corkO/corkO.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/davos/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/davos/CategoricalPalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5296 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/davos/CategoricalPalettes/davosS.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/davos/CategoricalPalettes/davosS.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3027 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/davos/CategoricalPalettes/davosS_HEX.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/davos/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      355 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/davos/DiscretePalettes/davos10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3018 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/davos/DiscretePalettes/davos100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      799 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/davos/DiscretePalettes/davos25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1539 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/davos/DiscretePalettes/davos50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/davos/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12454 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/davos/davos.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/davos/davos.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/devon/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/devon/CategoricalPalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5285 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/devon/CategoricalPalettes/devonS.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/devon/CategoricalPalettes/devonS.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3026 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/devon/CategoricalPalettes/devonS_HEX.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/devon/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      355 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/devon/DiscretePalettes/devon10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3018 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/devon/DiscretePalettes/devon100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      799 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/devon/DiscretePalettes/devon25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1539 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/devon/DiscretePalettes/devon50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/devon/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12414 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/devon/devon.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/devon/devon.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/fes/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.821682 seislib-0.6.8/seislib/colormaps/fes/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      333 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/fes/DiscretePalettes/fes10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2816 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/fes/DiscretePalettes/fes100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      747 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/fes/DiscretePalettes/fes25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1437 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/fes/DiscretePalettes/fes50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/fes/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12412 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/fes/fes.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/fes/fes.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/grayC/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/grayC/CategoricalPalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5318 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/grayC/CategoricalPalettes/grayCS.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/grayC/CategoricalPalettes/grayCS.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3027 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/grayC/CategoricalPalettes/grayCS_HEX.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/grayC/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      355 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/grayC/DiscretePalettes/grayC10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3018 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/grayC/DiscretePalettes/grayC100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      799 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/grayC/DiscretePalettes/grayC25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1539 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/grayC/DiscretePalettes/grayC50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/grayC/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12470 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/grayC/grayC.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/grayC/grayC.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/hawaii/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/hawaii/CategoricalPalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5309 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/hawaii/CategoricalPalettes/hawaiiS.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/hawaii/CategoricalPalettes/hawaiiS.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3130 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/hawaii/CategoricalPalettes/hawaiiS_HEX.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/hawaii/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      366 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/hawaii/DiscretePalettes/hawaii10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3119 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/hawaii/DiscretePalettes/hawaii100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      825 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/hawaii/DiscretePalettes/hawaii25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1590 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/hawaii/DiscretePalettes/hawaii50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/hawaii/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12436 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/hawaii/hawaii.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/hawaii/hawaii.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/imola/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/imola/CategoricalPalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5273 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/imola/CategoricalPalettes/imolaS.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/imola/CategoricalPalettes/imolaS.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3028 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/imola/CategoricalPalettes/imolaS_HEX.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/imola/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      355 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/imola/DiscretePalettes/imola10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3018 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/imola/DiscretePalettes/imola100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      799 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/imola/DiscretePalettes/imola25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1539 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/imola/DiscretePalettes/imola50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/imola/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12391 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/imola/imola.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/imola/imola.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/lajolla/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/lajolla/CategoricalPalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5307 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lajolla/CategoricalPalettes/lajollaS.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lajolla/CategoricalPalettes/lajollaS.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3231 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lajolla/CategoricalPalettes/lajollaS_HEX.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/lajolla/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      377 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lajolla/DiscretePalettes/lajolla10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3220 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lajolla/DiscretePalettes/lajolla100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      851 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lajolla/DiscretePalettes/lajolla25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1641 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lajolla/DiscretePalettes/lajolla50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lajolla/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12437 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lajolla/lajolla.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lajolla/lajolla.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/lapaz/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/lapaz/CategoricalPalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5283 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lapaz/CategoricalPalettes/lapazS.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lapaz/CategoricalPalettes/lapazS.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3026 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lapaz/CategoricalPalettes/lapazS_HEX.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/lapaz/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      355 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lapaz/DiscretePalettes/lapaz10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3018 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lapaz/DiscretePalettes/lapaz100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      799 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lapaz/DiscretePalettes/lapaz25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1539 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lapaz/DiscretePalettes/lapaz50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lapaz/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12425 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lapaz/lapaz.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lapaz/lapaz.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/lisbon/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/lisbon/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      366 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lisbon/DiscretePalettes/lisbon10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3119 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lisbon/DiscretePalettes/lisbon100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      825 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lisbon/DiscretePalettes/lisbon25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1590 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lisbon/DiscretePalettes/lisbon50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lisbon/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12462 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lisbon/lisbon.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/lisbon/lisbon.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/nuuk/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/nuuk/CategoricalPalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5281 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/nuuk/CategoricalPalettes/nuukS.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/nuuk/CategoricalPalettes/nuukS.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2927 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/nuuk/CategoricalPalettes/nuukS_HEX.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/nuuk/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      344 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/nuuk/DiscretePalettes/nuuk10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2917 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/nuuk/DiscretePalettes/nuuk100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      773 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/nuuk/DiscretePalettes/nuuk25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1488 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/nuuk/DiscretePalettes/nuuk50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/nuuk/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12417 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/nuuk/nuuk.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/nuuk/nuuk.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/oleron/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/oleron/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      366 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/oleron/DiscretePalettes/oleron10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3119 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/oleron/DiscretePalettes/oleron100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      825 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/oleron/DiscretePalettes/oleron25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1590 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/oleron/DiscretePalettes/oleron50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/oleron/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12477 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/oleron/oleron.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/oleron/oleron.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/oslo/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/oslo/CategoricalPalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5319 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/oslo/CategoricalPalettes/osloS.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/oslo/CategoricalPalettes/osloS.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2927 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/oslo/CategoricalPalettes/osloS_HEX.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/oslo/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      344 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/oslo/DiscretePalettes/oslo10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2917 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/oslo/DiscretePalettes/oslo100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      773 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/oslo/DiscretePalettes/oslo25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1488 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/oslo/DiscretePalettes/oslo50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/oslo/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12521 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/oslo/oslo.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/oslo/oslo.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/roma/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.825682 seislib-0.6.8/seislib/colormaps/roma/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      344 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/roma/DiscretePalettes/roma10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2917 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/roma/DiscretePalettes/roma100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      773 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/roma/DiscretePalettes/roma25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1488 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/roma/DiscretePalettes/roma50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/roma/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12459 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/roma/roma.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/roma/roma.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.829682 seislib-0.6.8/seislib/colormaps/romaO/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.829682 seislib-0.6.8/seislib/colormaps/romaO/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      355 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/romaO/DiscretePalettes/romaO10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3018 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/romaO/DiscretePalettes/romaO100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      799 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/romaO/DiscretePalettes/romaO25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1539 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/romaO/DiscretePalettes/romaO50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/romaO/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12422 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/romaO/romaO.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/romaO/romaO.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.829682 seislib-0.6.8/seislib/colormaps/tofino/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.829682 seislib-0.6.8/seislib/colormaps/tofino/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      366 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/tofino/DiscretePalettes/tofino10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3119 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/tofino/DiscretePalettes/tofino100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      825 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/tofino/DiscretePalettes/tofino25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1590 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/tofino/DiscretePalettes/tofino50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/tofino/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12522 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/tofino/tofino.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/tofino/tofino.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.829682 seislib-0.6.8/seislib/colormaps/tokyo/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.829682 seislib-0.6.8/seislib/colormaps/tokyo/CategoricalPalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5299 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/tokyo/CategoricalPalettes/tokyoS.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/tokyo/CategoricalPalettes/tokyoS.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3030 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/tokyo/CategoricalPalettes/tokyoS_HEX.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.829682 seislib-0.6.8/seislib/colormaps/tokyo/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      355 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/tokyo/DiscretePalettes/tokyo10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3018 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/tokyo/DiscretePalettes/tokyo100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      799 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/tokyo/DiscretePalettes/tokyo25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1539 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/tokyo/DiscretePalettes/tokyo50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/tokyo/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12421 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/tokyo/tokyo.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/tokyo/tokyo.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.829682 seislib-0.6.8/seislib/colormaps/turku/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.829682 seislib-0.6.8/seislib/colormaps/turku/CategoricalPalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5298 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/turku/CategoricalPalettes/turkuS.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/turku/CategoricalPalettes/turkuS.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3028 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/turku/CategoricalPalettes/turkuS_HEX.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.829682 seislib-0.6.8/seislib/colormaps/turku/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      355 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/turku/DiscretePalettes/turku10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3018 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/turku/DiscretePalettes/turku100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      799 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/turku/DiscretePalettes/turku25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1539 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/turku/DiscretePalettes/turku50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/turku/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12433 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/turku/turku.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/turku/turku.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.829682 seislib-0.6.8/seislib/colormaps/vanimo/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.829682 seislib-0.6.8/seislib/colormaps/vanimo/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      366 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/vanimo/DiscretePalettes/vanimo10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3119 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/vanimo/DiscretePalettes/vanimo100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      825 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/vanimo/DiscretePalettes/vanimo25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1590 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/vanimo/DiscretePalettes/vanimo50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/vanimo/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12515 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/vanimo/vanimo.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/vanimo/vanimo.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.829682 seislib-0.6.8/seislib/colormaps/vik/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.829682 seislib-0.6.8/seislib/colormaps/vik/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      333 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/vik/DiscretePalettes/vik10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2816 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/vik/DiscretePalettes/vik100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      747 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/vik/DiscretePalettes/vik25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1437 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/vik/DiscretePalettes/vik50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/vik/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12548 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/vik/vik.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/vik/vik.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.829682 seislib-0.6.8/seislib/colormaps/vikO/
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.829682 seislib-0.6.8/seislib/colormaps/vikO/DiscretePalettes/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      344 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/vikO/DiscretePalettes/vikO10.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2917 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/vikO/DiscretePalettes/vikO100.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      773 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/vikO/DiscretePalettes/vikO25.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1488 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/vikO/DiscretePalettes/vikO50.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/vikO/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12427 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/vikO/vikO.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/colormaps/vikO/vikO.txt
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.833682 seislib-0.6.8/seislib/eq/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2147 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/eq/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    39847 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/eq/eq_downloader.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)   101133 2023-04-04 23:50:46.000000 seislib-0.6.8/seislib/eq/eq_velocity.py
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.833682 seislib-0.6.8/seislib/exceptions/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       28 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/exceptions/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1463 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/exceptions/exceptions.py
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.833682 seislib-0.6.8/seislib/plotting/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      965 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/plotting/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    42784 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/plotting/plotting.py
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.833682 seislib-0.6.8/seislib/tomography/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1417 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/tomography/__init__.py
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.833682 seislib-0.6.8/seislib/tomography/_ray_theory/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/tomography/_ray_theory/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      153 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/tomography/_ray_theory/_math.pxd
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      809 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/tomography/_ray_theory/_math.pyx
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      462 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/tomography/_ray_theory/_spherical_geometry.pxd
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     4528 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/tomography/_ray_theory/_spherical_geometry.pyx
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    24406 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/tomography/_ray_theory/_tomography.pyx
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1703 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/tomography/_ray_theory/setup_all.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    36472 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/tomography/grid.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    72055 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/tomography/tomography.py
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.833682 seislib-0.6.8/seislib/utils/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1054 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/utils/__init__.py
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    17570 2023-04-03 03:52:42.000000 seislib-0.6.8/seislib/utils/utils.py
-drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-04 23:59:17.813682 seislib-0.6.8/seislib.egg-info/
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5278 2023-04-04 23:59:17.000000 seislib-0.6.8/seislib.egg-info/PKG-INFO
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    15384 2023-04-04 23:59:17.000000 seislib-0.6.8/seislib.egg-info/SOURCES.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)        1 2023-04-04 23:59:17.000000 seislib-0.6.8/seislib.egg-info/dependency_links.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       87 2023-04-04 23:59:17.000000 seislib-0.6.8/seislib.egg-info/requires.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)        8 2023-04-04 23:59:17.000000 seislib-0.6.8/seislib.egg-info/top_level.txt
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       79 2023-04-04 23:59:17.833682 seislib-0.6.8/setup.cfg
--rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3340 2023-04-03 03:52:42.000000 seislib-0.6.8/setup.py
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.757315 seislib-0.6.9/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1073 2023-04-03 03:52:42.000000 seislib-0.6.9/LICENSE.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      457 2023-04-03 03:52:42.000000 seislib-0.6.9/MANIFEST.in
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5278 2023-04-06 05:40:56.757315 seislib-0.6.9/PKG-INFO
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     4724 2023-04-03 03:52:42.000000 seislib-0.6.9/README.md
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.741315 seislib-0.6.9/seislib/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      373 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      258 2023-04-06 05:40:13.000000 seislib-0.6.9/seislib/__version__.py
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.741315 seislib-0.6.9/seislib/an/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3210 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/an/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    84409 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/an/an_attenuation.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    39923 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/an/an_downloader.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    67691 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/an/an_processing.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    37179 2023-04-06 05:38:34.000000 seislib-0.6.9/seislib/an/an_velocity.py
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)   115362 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/+LICENCE.pdf
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)   876959 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/+README_ScientificColourMaps-6.pdf
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)   324037 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/+ScientificColourMapsGuideline_Crameri_EtAl2020.pdf
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1348 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/__init__.py
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/acton/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/acton/CategoricalPalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5289 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/acton/CategoricalPalettes/actonS.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/acton/CategoricalPalettes/actonS.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3026 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/acton/CategoricalPalettes/actonS_HEX.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/acton/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      355 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/acton/DiscretePalettes/acton10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3018 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/acton/DiscretePalettes/acton100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      799 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/acton/DiscretePalettes/acton25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1539 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/acton/DiscretePalettes/acton50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/acton/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12422 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/acton/acton.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/acton/acton.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/bam/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/bam/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      333 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bam/DiscretePalettes/bam10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2816 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bam/DiscretePalettes/bam100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      747 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bam/DiscretePalettes/bam25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1437 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bam/DiscretePalettes/bam50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bam/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12399 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bam/bam.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bam/bam.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/bamO/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/bamO/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      344 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bamO/DiscretePalettes/bamO10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2917 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bamO/DiscretePalettes/bamO100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      773 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bamO/DiscretePalettes/bamO25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1488 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bamO/DiscretePalettes/bamO50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bamO/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12400 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bamO/bamO.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bamO/bamO.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/bamako/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/bamako/CategoricalPalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5337 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bamako/CategoricalPalettes/bamakoS.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bamako/CategoricalPalettes/bamakoS.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3130 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bamako/CategoricalPalettes/bamakoS_HEX.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/bamako/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      366 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bamako/DiscretePalettes/bamako10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3119 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bamako/DiscretePalettes/bamako100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      825 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bamako/DiscretePalettes/bamako25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1590 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bamako/DiscretePalettes/bamako50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bamako/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12513 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bamako/bamako.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bamako/bamako.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/batlow/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/batlow/CategoricalPalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5318 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlow/CategoricalPalettes/batlowS.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlow/CategoricalPalettes/batlowS.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3129 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlow/CategoricalPalettes/batlowS_HEX.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/batlow/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      366 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlow/DiscretePalettes/batlow10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3119 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlow/DiscretePalettes/batlow100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      825 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlow/DiscretePalettes/batlow25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1590 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlow/DiscretePalettes/batlow50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlow/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12463 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlow/batlow.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlow/batlow.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/batlowK/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/batlowK/CategoricalPalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5309 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlowK/CategoricalPalettes/batlowKS.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlowK/CategoricalPalettes/batlowKS.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3230 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlowK/CategoricalPalettes/batlowKS_HEX.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/batlowK/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      377 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlowK/DiscretePalettes/batlowK10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3220 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlowK/DiscretePalettes/batlowK100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      851 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlowK/DiscretePalettes/batlowK25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1641 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlowK/DiscretePalettes/batlowK50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlowK/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12462 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlowK/batlowK.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlowK/batlowK.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/batlowW/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/batlowW/CategoricalPalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5282 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlowW/CategoricalPalettes/batlowWS.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlowW/CategoricalPalettes/batlowWS.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3235 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlowW/CategoricalPalettes/batlowWS_HEX.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/batlowW/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      377 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlowW/DiscretePalettes/batlowW10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3220 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlowW/DiscretePalettes/batlowW100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      851 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlowW/DiscretePalettes/batlowW25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1641 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlowW/DiscretePalettes/batlowW50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlowW/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12363 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlowW/batlowW.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/batlowW/batlowW.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/berlin/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/berlin/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      366 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/berlin/DiscretePalettes/berlin10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3119 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/berlin/DiscretePalettes/berlin100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      825 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/berlin/DiscretePalettes/berlin25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1590 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/berlin/DiscretePalettes/berlin50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/berlin/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12620 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/berlin/berlin.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/berlin/berlin.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/bilbao/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/bilbao/CategoricalPalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5312 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bilbao/CategoricalPalettes/bilbaoS.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bilbao/CategoricalPalettes/bilbaoS.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3128 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bilbao/CategoricalPalettes/bilbaoS_HEX.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/bilbao/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      366 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bilbao/DiscretePalettes/bilbao10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3119 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bilbao/DiscretePalettes/bilbao100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      825 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bilbao/DiscretePalettes/bilbao25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1590 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bilbao/DiscretePalettes/bilbao50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bilbao/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12446 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bilbao/bilbao.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bilbao/bilbao.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.745315 seislib-0.6.9/seislib/colormaps/broc/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/broc/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      344 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/broc/DiscretePalettes/broc10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2917 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/broc/DiscretePalettes/broc100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      773 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/broc/DiscretePalettes/broc25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1488 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/broc/DiscretePalettes/broc50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/broc/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12423 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/broc/broc.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/broc/broc.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/brocO/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/brocO/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      355 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/brocO/DiscretePalettes/brocO10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3018 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/brocO/DiscretePalettes/brocO100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      799 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/brocO/DiscretePalettes/brocO25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1539 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/brocO/DiscretePalettes/brocO50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/brocO/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12412 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/brocO/brocO.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/brocO/brocO.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/buda/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/buda/CategoricalPalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5266 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/buda/CategoricalPalettes/budaS.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/buda/CategoricalPalettes/budaS.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2928 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/buda/CategoricalPalettes/budaS_HEX.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/buda/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      344 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/buda/DiscretePalettes/buda10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2917 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/buda/DiscretePalettes/buda100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      773 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/buda/DiscretePalettes/buda25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1488 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/buda/DiscretePalettes/buda50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/buda/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12387 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/buda/buda.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/buda/buda.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/bukavu/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/bukavu/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      366 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bukavu/DiscretePalettes/bukavu10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3119 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bukavu/DiscretePalettes/bukavu100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      825 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bukavu/DiscretePalettes/bukavu25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1590 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bukavu/DiscretePalettes/bukavu50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bukavu/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12451 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bukavu/bukavu.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/bukavu/bukavu.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/cork/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/cork/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      344 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/cork/DiscretePalettes/cork10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2917 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/cork/DiscretePalettes/cork100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      773 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/cork/DiscretePalettes/cork25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1488 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/cork/DiscretePalettes/cork50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/cork/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12461 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/cork/cork.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/cork/cork.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/corkO/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/corkO/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      355 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/corkO/DiscretePalettes/corkO10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3018 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/corkO/DiscretePalettes/corkO100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      799 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/corkO/DiscretePalettes/corkO25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1539 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/corkO/DiscretePalettes/corkO50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/corkO/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12414 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/corkO/corkO.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/corkO/corkO.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/davos/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/davos/CategoricalPalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5296 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/davos/CategoricalPalettes/davosS.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/davos/CategoricalPalettes/davosS.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3027 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/davos/CategoricalPalettes/davosS_HEX.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/davos/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      355 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/davos/DiscretePalettes/davos10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3018 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/davos/DiscretePalettes/davos100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      799 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/davos/DiscretePalettes/davos25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1539 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/davos/DiscretePalettes/davos50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/davos/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12454 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/davos/davos.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/davos/davos.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/devon/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/devon/CategoricalPalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5285 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/devon/CategoricalPalettes/devonS.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/devon/CategoricalPalettes/devonS.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3026 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/devon/CategoricalPalettes/devonS_HEX.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/devon/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      355 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/devon/DiscretePalettes/devon10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3018 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/devon/DiscretePalettes/devon100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      799 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/devon/DiscretePalettes/devon25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1539 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/devon/DiscretePalettes/devon50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/devon/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12414 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/devon/devon.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/devon/devon.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/fes/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/fes/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      333 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/fes/DiscretePalettes/fes10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2816 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/fes/DiscretePalettes/fes100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      747 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/fes/DiscretePalettes/fes25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1437 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/fes/DiscretePalettes/fes50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/fes/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12412 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/fes/fes.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/fes/fes.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/grayC/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/grayC/CategoricalPalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5318 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/grayC/CategoricalPalettes/grayCS.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/grayC/CategoricalPalettes/grayCS.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3027 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/grayC/CategoricalPalettes/grayCS_HEX.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/grayC/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      355 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/grayC/DiscretePalettes/grayC10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3018 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/grayC/DiscretePalettes/grayC100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      799 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/grayC/DiscretePalettes/grayC25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1539 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/grayC/DiscretePalettes/grayC50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/grayC/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12470 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/grayC/grayC.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/grayC/grayC.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/hawaii/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/hawaii/CategoricalPalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5309 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/hawaii/CategoricalPalettes/hawaiiS.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/hawaii/CategoricalPalettes/hawaiiS.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3130 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/hawaii/CategoricalPalettes/hawaiiS_HEX.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.749315 seislib-0.6.9/seislib/colormaps/hawaii/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      366 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/hawaii/DiscretePalettes/hawaii10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3119 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/hawaii/DiscretePalettes/hawaii100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      825 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/hawaii/DiscretePalettes/hawaii25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1590 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/hawaii/DiscretePalettes/hawaii50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/hawaii/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12436 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/hawaii/hawaii.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/hawaii/hawaii.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/imola/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/imola/CategoricalPalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5273 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/imola/CategoricalPalettes/imolaS.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/imola/CategoricalPalettes/imolaS.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3028 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/imola/CategoricalPalettes/imolaS_HEX.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/imola/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      355 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/imola/DiscretePalettes/imola10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3018 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/imola/DiscretePalettes/imola100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      799 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/imola/DiscretePalettes/imola25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1539 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/imola/DiscretePalettes/imola50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/imola/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12391 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/imola/imola.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/imola/imola.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/lajolla/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/lajolla/CategoricalPalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5307 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lajolla/CategoricalPalettes/lajollaS.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lajolla/CategoricalPalettes/lajollaS.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3231 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lajolla/CategoricalPalettes/lajollaS_HEX.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/lajolla/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      377 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lajolla/DiscretePalettes/lajolla10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3220 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lajolla/DiscretePalettes/lajolla100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      851 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lajolla/DiscretePalettes/lajolla25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1641 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lajolla/DiscretePalettes/lajolla50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lajolla/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12437 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lajolla/lajolla.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lajolla/lajolla.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/lapaz/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/lapaz/CategoricalPalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5283 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lapaz/CategoricalPalettes/lapazS.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lapaz/CategoricalPalettes/lapazS.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3026 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lapaz/CategoricalPalettes/lapazS_HEX.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/lapaz/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      355 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lapaz/DiscretePalettes/lapaz10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3018 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lapaz/DiscretePalettes/lapaz100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      799 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lapaz/DiscretePalettes/lapaz25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1539 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lapaz/DiscretePalettes/lapaz50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lapaz/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12425 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lapaz/lapaz.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lapaz/lapaz.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/lisbon/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/lisbon/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      366 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lisbon/DiscretePalettes/lisbon10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3119 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lisbon/DiscretePalettes/lisbon100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      825 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lisbon/DiscretePalettes/lisbon25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1590 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lisbon/DiscretePalettes/lisbon50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lisbon/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12462 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lisbon/lisbon.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/lisbon/lisbon.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/nuuk/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/nuuk/CategoricalPalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5281 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/nuuk/CategoricalPalettes/nuukS.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/nuuk/CategoricalPalettes/nuukS.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2927 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/nuuk/CategoricalPalettes/nuukS_HEX.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/nuuk/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      344 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/nuuk/DiscretePalettes/nuuk10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2917 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/nuuk/DiscretePalettes/nuuk100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      773 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/nuuk/DiscretePalettes/nuuk25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1488 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/nuuk/DiscretePalettes/nuuk50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/nuuk/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12417 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/nuuk/nuuk.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/nuuk/nuuk.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/oleron/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/oleron/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      366 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/oleron/DiscretePalettes/oleron10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3119 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/oleron/DiscretePalettes/oleron100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      825 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/oleron/DiscretePalettes/oleron25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1590 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/oleron/DiscretePalettes/oleron50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/oleron/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12477 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/oleron/oleron.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/oleron/oleron.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/oslo/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/oslo/CategoricalPalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5319 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/oslo/CategoricalPalettes/osloS.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/oslo/CategoricalPalettes/osloS.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2927 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/oslo/CategoricalPalettes/osloS_HEX.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/oslo/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      344 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/oslo/DiscretePalettes/oslo10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2917 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/oslo/DiscretePalettes/oslo100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      773 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/oslo/DiscretePalettes/oslo25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1488 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/oslo/DiscretePalettes/oslo50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/oslo/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12521 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/oslo/oslo.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/oslo/oslo.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/roma/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/roma/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      344 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/roma/DiscretePalettes/roma10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2917 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/roma/DiscretePalettes/roma100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      773 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/roma/DiscretePalettes/roma25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1488 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/roma/DiscretePalettes/roma50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/roma/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12459 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/roma/roma.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/roma/roma.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/romaO/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/romaO/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      355 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/romaO/DiscretePalettes/romaO10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3018 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/romaO/DiscretePalettes/romaO100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      799 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/romaO/DiscretePalettes/romaO25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1539 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/romaO/DiscretePalettes/romaO50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/romaO/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12422 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/romaO/romaO.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/romaO/romaO.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/tofino/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/tofino/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      366 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/tofino/DiscretePalettes/tofino10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3119 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/tofino/DiscretePalettes/tofino100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      825 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/tofino/DiscretePalettes/tofino25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1590 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/tofino/DiscretePalettes/tofino50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/tofino/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12522 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/tofino/tofino.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/tofino/tofino.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.753315 seislib-0.6.9/seislib/colormaps/tokyo/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.757315 seislib-0.6.9/seislib/colormaps/tokyo/CategoricalPalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5299 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/tokyo/CategoricalPalettes/tokyoS.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/tokyo/CategoricalPalettes/tokyoS.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3030 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/tokyo/CategoricalPalettes/tokyoS_HEX.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.757315 seislib-0.6.9/seislib/colormaps/tokyo/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      355 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/tokyo/DiscretePalettes/tokyo10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3018 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/tokyo/DiscretePalettes/tokyo100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      799 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/tokyo/DiscretePalettes/tokyo25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1539 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/tokyo/DiscretePalettes/tokyo50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/tokyo/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12421 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/tokyo/tokyo.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/tokyo/tokyo.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.757315 seislib-0.6.9/seislib/colormaps/turku/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.757315 seislib-0.6.9/seislib/colormaps/turku/CategoricalPalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5298 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/turku/CategoricalPalettes/turkuS.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2700 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/turku/CategoricalPalettes/turkuS.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3028 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/turku/CategoricalPalettes/turkuS_HEX.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.757315 seislib-0.6.9/seislib/colormaps/turku/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      355 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/turku/DiscretePalettes/turku10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3018 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/turku/DiscretePalettes/turku100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      799 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/turku/DiscretePalettes/turku25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1539 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/turku/DiscretePalettes/turku50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/turku/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12433 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/turku/turku.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/turku/turku.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.757315 seislib-0.6.9/seislib/colormaps/vanimo/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.757315 seislib-0.6.9/seislib/colormaps/vanimo/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      366 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/vanimo/DiscretePalettes/vanimo10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3119 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/vanimo/DiscretePalettes/vanimo100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      825 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/vanimo/DiscretePalettes/vanimo25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1590 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/vanimo/DiscretePalettes/vanimo50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/vanimo/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12515 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/vanimo/vanimo.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/vanimo/vanimo.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.757315 seislib-0.6.9/seislib/colormaps/vik/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.757315 seislib-0.6.9/seislib/colormaps/vik/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      333 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/vik/DiscretePalettes/vik10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2816 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/vik/DiscretePalettes/vik100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      747 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/vik/DiscretePalettes/vik25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1437 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/vik/DiscretePalettes/vik50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/vik/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12548 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/vik/vik.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/vik/vik.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.757315 seislib-0.6.9/seislib/colormaps/vikO/
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.757315 seislib-0.6.9/seislib/colormaps/vikO/DiscretePalettes/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      344 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/vikO/DiscretePalettes/vikO10.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2917 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/vikO/DiscretePalettes/vikO100.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      773 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/vikO/DiscretePalettes/vikO25.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1488 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/vikO/DiscretePalettes/vikO50.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       48 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/vikO/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    12427 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/vikO/vikO.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     6912 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/colormaps/vikO/vikO.txt
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.757315 seislib-0.6.9/seislib/eq/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     2147 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/eq/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    39847 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/eq/eq_downloader.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)   101147 2023-04-06 05:39:08.000000 seislib-0.6.9/seislib/eq/eq_velocity.py
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.757315 seislib-0.6.9/seislib/exceptions/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       28 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/exceptions/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1463 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/exceptions/exceptions.py
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.757315 seislib-0.6.9/seislib/plotting/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      965 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/plotting/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    42784 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/plotting/plotting.py
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.757315 seislib-0.6.9/seislib/tomography/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1417 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/tomography/__init__.py
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.757315 seislib-0.6.9/seislib/tomography/_ray_theory/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/tomography/_ray_theory/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      153 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/tomography/_ray_theory/_math.pxd
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      809 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/tomography/_ray_theory/_math.pyx
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)      462 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/tomography/_ray_theory/_spherical_geometry.pxd
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     4528 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/tomography/_ray_theory/_spherical_geometry.pyx
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    24406 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/tomography/_ray_theory/_tomography.pyx
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1703 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/tomography/_ray_theory/setup_all.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    36472 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/tomography/grid.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    72055 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/tomography/tomography.py
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.757315 seislib-0.6.9/seislib/utils/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     1054 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/utils/__init__.py
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    17570 2023-04-03 03:52:42.000000 seislib-0.6.9/seislib/utils/utils.py
+drwxrwxr-x   0 fabrizio  (1000) fabrizio  (1000)        0 2023-04-06 05:40:56.741315 seislib-0.6.9/seislib.egg-info/
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     5278 2023-04-06 05:40:56.000000 seislib-0.6.9/seislib.egg-info/PKG-INFO
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)    15384 2023-04-06 05:40:56.000000 seislib-0.6.9/seislib.egg-info/SOURCES.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)        1 2023-04-06 05:40:56.000000 seislib-0.6.9/seislib.egg-info/dependency_links.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       87 2023-04-06 05:40:56.000000 seislib-0.6.9/seislib.egg-info/requires.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)        8 2023-04-06 05:40:56.000000 seislib-0.6.9/seislib.egg-info/top_level.txt
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)       79 2023-04-06 05:40:56.757315 seislib-0.6.9/setup.cfg
+-rw-rw-r--   0 fabrizio  (1000) fabrizio  (1000)     3340 2023-04-03 03:52:42.000000 seislib-0.6.9/setup.py
```

### Comparing `seislib-0.6.8/LICENSE.txt` & `seislib-0.6.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/PKG-INFO` & `seislib-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seislib
-Version: 0.6.8
+Version: 0.6.9
 Summary: Multi-scale Seismic Imaging
 Home-page: https://github.com/fmagrini/seislib
 Author: Fabrizio Magrini
 Author-email: fabrizio.magrini90@gmail.com
 License: MIT
 Keywords: Seismic Imaging,Surface Waves,Seismic Ambient Noise,Earthquake Seismology,Tomographic Inversion
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `seislib-0.6.8/README.md` & `seislib-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/an/__init__.py` & `seislib-0.6.9/seislib/an/__init__.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/an/an_attenuation.py` & `seislib-0.6.9/seislib/an/an_attenuation.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/an/an_downloader.py` & `seislib-0.6.9/seislib/an/an_downloader.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/an/an_processing.py` & `seislib-0.6.9/seislib/an/an_processing.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/an/an_velocity.py` & `seislib-0.6.9/seislib/an/an_velocity.py`

 * *Files 0% similar despite different names*

```diff
@@ -706,15 +706,15 @@
             an.prepare_input_tomography(savedir=savedir,
                                         period=periods)
 
         The above will save one txt file for each specified period.
         """
         os.makedirs(savedir, exist_ok=True)
         period = np.array([period]) if np.isscalar(period) else np.array(period)
-        coords, velocity = self.interpolate_dispcurves(1/period)
+        codes, coords, velocity = self.interpolate_dispcurves(1/period)
         dist = SeismicTomography.gc_distance(*coords.T)
         wavelength = velocity * period
         ratios = dist.reshape(-1, 1) / wavelength
         velocity_final = np.where(ratios>min_no_wavelengths, velocity, np.nan)
 
         for iperiod, p in enumerate(period):
             save = os.path.join(savedir, outfile%p)
@@ -765,15 +765,15 @@
             an.prepare_data()
 
         Even if the computation of the dispersion curves is not yet 
         finished, you can use the above instance to interpolate all the
         available dispersion curves as follows::
 
             frequency = [1/30, 1/20, 1/10, 1/5]
-            coords, measurements = an.interpolate_dispcurves(frequency)        
+            codes, coords, measurements = an.interpolate_dispcurves(frequency)        
         """
         def display_progress(no_files, done, verbose=False):
             if verbose and not done % int(0.05*no_files + 1):
                 print('FILES PROCESSED: %d/%d'%(done, no_files))
                     
         src = os.path.join(self.savedir, 'dispcurves')
         files = [i for i in sorted(os.listdir(src)) if i.endswith('npy')]
```

### Comparing `seislib-0.6.8/seislib/colormaps/+LICENCE.pdf` & `seislib-0.6.9/seislib/colormaps/+LICENCE.pdf`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/+README_ScientificColourMaps-6.pdf` & `seislib-0.6.9/seislib/colormaps/+README_ScientificColourMaps-6.pdf`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/+ScientificColourMapsGuideline_Crameri_EtAl2020.pdf` & `seislib-0.6.9/seislib/colormaps/+ScientificColourMapsGuideline_Crameri_EtAl2020.pdf`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/__init__.py` & `seislib-0.6.9/seislib/colormaps/__init__.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/acton/CategoricalPalettes/actonS.py` & `seislib-0.6.9/seislib/colormaps/acton/CategoricalPalettes/actonS.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/acton/CategoricalPalettes/actonS.txt` & `seislib-0.6.9/seislib/colormaps/acton/CategoricalPalettes/actonS.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/acton/CategoricalPalettes/actonS_HEX.txt` & `seislib-0.6.9/seislib/colormaps/acton/CategoricalPalettes/actonS_HEX.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/acton/DiscretePalettes/acton100.txt` & `seislib-0.6.9/seislib/colormaps/acton/DiscretePalettes/acton100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/acton/DiscretePalettes/acton25.txt` & `seislib-0.6.9/seislib/colormaps/acton/DiscretePalettes/acton25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/acton/DiscretePalettes/acton50.txt` & `seislib-0.6.9/seislib/colormaps/acton/DiscretePalettes/acton50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/acton/acton.py` & `seislib-0.6.9/seislib/colormaps/acton/acton.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/acton/acton.txt` & `seislib-0.6.9/seislib/colormaps/acton/acton.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bam/DiscretePalettes/bam100.txt` & `seislib-0.6.9/seislib/colormaps/bam/DiscretePalettes/bam100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bam/DiscretePalettes/bam25.txt` & `seislib-0.6.9/seislib/colormaps/bam/DiscretePalettes/bam25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bam/DiscretePalettes/bam50.txt` & `seislib-0.6.9/seislib/colormaps/bam/DiscretePalettes/bam50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bam/bam.py` & `seislib-0.6.9/seislib/colormaps/bam/bam.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bam/bam.txt` & `seislib-0.6.9/seislib/colormaps/bam/bam.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bamO/DiscretePalettes/bamO100.txt` & `seislib-0.6.9/seislib/colormaps/bamO/DiscretePalettes/bamO100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bamO/DiscretePalettes/bamO25.txt` & `seislib-0.6.9/seislib/colormaps/bamO/DiscretePalettes/bamO25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bamO/DiscretePalettes/bamO50.txt` & `seislib-0.6.9/seislib/colormaps/bamO/DiscretePalettes/bamO50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bamO/bamO.py` & `seislib-0.6.9/seislib/colormaps/bamO/bamO.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bamO/bamO.txt` & `seislib-0.6.9/seislib/colormaps/bamO/bamO.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bamako/CategoricalPalettes/bamakoS.py` & `seislib-0.6.9/seislib/colormaps/bamako/CategoricalPalettes/bamakoS.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bamako/CategoricalPalettes/bamakoS.txt` & `seislib-0.6.9/seislib/colormaps/bamako/CategoricalPalettes/bamakoS.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bamako/CategoricalPalettes/bamakoS_HEX.txt` & `seislib-0.6.9/seislib/colormaps/bamako/CategoricalPalettes/bamakoS_HEX.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bamako/DiscretePalettes/bamako100.txt` & `seislib-0.6.9/seislib/colormaps/bamako/DiscretePalettes/bamako100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bamako/DiscretePalettes/bamako25.txt` & `seislib-0.6.9/seislib/colormaps/bamako/DiscretePalettes/bamako25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bamako/DiscretePalettes/bamako50.txt` & `seislib-0.6.9/seislib/colormaps/bamako/DiscretePalettes/bamako50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bamako/bamako.py` & `seislib-0.6.9/seislib/colormaps/bamako/bamako.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bamako/bamako.txt` & `seislib-0.6.9/seislib/colormaps/bamako/bamako.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/batlow/CategoricalPalettes/batlowS.py` & `seislib-0.6.9/seislib/colormaps/batlow/CategoricalPalettes/batlowS.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/batlow/CategoricalPalettes/batlowS.txt` & `seislib-0.6.9/seislib/colormaps/batlow/CategoricalPalettes/batlowS.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/batlow/CategoricalPalettes/batlowS_HEX.txt` & `seislib-0.6.9/seislib/colormaps/batlow/CategoricalPalettes/batlowS_HEX.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/batlow/DiscretePalettes/batlow100.txt` & `seislib-0.6.9/seislib/colormaps/batlow/DiscretePalettes/batlow100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/batlow/DiscretePalettes/batlow25.txt` & `seislib-0.6.9/seislib/colormaps/batlow/DiscretePalettes/batlow25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/batlow/DiscretePalettes/batlow50.txt` & `seislib-0.6.9/seislib/colormaps/batlow/DiscretePalettes/batlow50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/batlow/batlow.py` & `seislib-0.6.9/seislib/colormaps/batlow/batlow.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/batlow/batlow.txt` & `seislib-0.6.9/seislib/colormaps/batlow/batlow.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/batlowK/CategoricalPalettes/batlowKS.py` & `seislib-0.6.9/seislib/colormaps/batlowK/CategoricalPalettes/batlowKS.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/batlowK/CategoricalPalettes/batlowKS.txt` & `seislib-0.6.9/seislib/colormaps/batlowK/CategoricalPalettes/batlowKS.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/batlowK/CategoricalPalettes/batlowKS_HEX.txt` & `seislib-0.6.9/seislib/colormaps/batlowK/CategoricalPalettes/batlowKS_HEX.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/batlowK/DiscretePalettes/batlowK100.txt` & `seislib-0.6.9/seislib/colormaps/batlowK/DiscretePalettes/batlowK100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/batlowK/DiscretePalettes/batlowK25.txt` & `seislib-0.6.9/seislib/colormaps/batlowK/DiscretePalettes/batlowK25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/batlowK/DiscretePalettes/batlowK50.txt` & `seislib-0.6.9/seislib/colormaps/batlowK/DiscretePalettes/batlowK50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/batlowK/batlowK.py` & `seislib-0.6.9/seislib/colormaps/batlowK/batlowK.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/batlowK/batlowK.txt` & `seislib-0.6.9/seislib/colormaps/batlowK/batlowK.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/batlowW/CategoricalPalettes/batlowWS.py` & `seislib-0.6.9/seislib/colormaps/batlowW/CategoricalPalettes/batlowWS.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/batlowW/CategoricalPalettes/batlowWS.txt` & `seislib-0.6.9/seislib/colormaps/batlowW/CategoricalPalettes/batlowWS.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/batlowW/CategoricalPalettes/batlowWS_HEX.txt` & `seislib-0.6.9/seislib/colormaps/batlowW/CategoricalPalettes/batlowWS_HEX.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/batlowW/DiscretePalettes/batlowW100.txt` & `seislib-0.6.9/seislib/colormaps/batlowW/DiscretePalettes/batlowW100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/batlowW/DiscretePalettes/batlowW25.txt` & `seislib-0.6.9/seislib/colormaps/batlowW/DiscretePalettes/batlowW25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/batlowW/DiscretePalettes/batlowW50.txt` & `seislib-0.6.9/seislib/colormaps/batlowW/DiscretePalettes/batlowW50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/batlowW/batlowW.py` & `seislib-0.6.9/seislib/colormaps/batlowW/batlowW.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/batlowW/batlowW.txt` & `seislib-0.6.9/seislib/colormaps/batlowW/batlowW.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/berlin/DiscretePalettes/berlin100.txt` & `seislib-0.6.9/seislib/colormaps/berlin/DiscretePalettes/berlin100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/berlin/DiscretePalettes/berlin25.txt` & `seislib-0.6.9/seislib/colormaps/berlin/DiscretePalettes/berlin25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/berlin/DiscretePalettes/berlin50.txt` & `seislib-0.6.9/seislib/colormaps/berlin/DiscretePalettes/berlin50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/berlin/berlin.py` & `seislib-0.6.9/seislib/colormaps/berlin/berlin.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/berlin/berlin.txt` & `seislib-0.6.9/seislib/colormaps/berlin/berlin.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bilbao/CategoricalPalettes/bilbaoS.py` & `seislib-0.6.9/seislib/colormaps/bilbao/CategoricalPalettes/bilbaoS.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bilbao/CategoricalPalettes/bilbaoS.txt` & `seislib-0.6.9/seislib/colormaps/bilbao/CategoricalPalettes/bilbaoS.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bilbao/CategoricalPalettes/bilbaoS_HEX.txt` & `seislib-0.6.9/seislib/colormaps/bilbao/CategoricalPalettes/bilbaoS_HEX.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bilbao/DiscretePalettes/bilbao100.txt` & `seislib-0.6.9/seislib/colormaps/bilbao/DiscretePalettes/bilbao100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bilbao/DiscretePalettes/bilbao25.txt` & `seislib-0.6.9/seislib/colormaps/bilbao/DiscretePalettes/bilbao25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bilbao/DiscretePalettes/bilbao50.txt` & `seislib-0.6.9/seislib/colormaps/bilbao/DiscretePalettes/bilbao50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bilbao/bilbao.py` & `seislib-0.6.9/seislib/colormaps/bilbao/bilbao.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bilbao/bilbao.txt` & `seislib-0.6.9/seislib/colormaps/bilbao/bilbao.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/broc/DiscretePalettes/broc100.txt` & `seislib-0.6.9/seislib/colormaps/broc/DiscretePalettes/broc100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/broc/DiscretePalettes/broc25.txt` & `seislib-0.6.9/seislib/colormaps/broc/DiscretePalettes/broc25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/broc/DiscretePalettes/broc50.txt` & `seislib-0.6.9/seislib/colormaps/broc/DiscretePalettes/broc50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/broc/broc.py` & `seislib-0.6.9/seislib/colormaps/broc/broc.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/broc/broc.txt` & `seislib-0.6.9/seislib/colormaps/broc/broc.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/brocO/DiscretePalettes/brocO100.txt` & `seislib-0.6.9/seislib/colormaps/brocO/DiscretePalettes/brocO100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/brocO/DiscretePalettes/brocO25.txt` & `seislib-0.6.9/seislib/colormaps/brocO/DiscretePalettes/brocO25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/brocO/DiscretePalettes/brocO50.txt` & `seislib-0.6.9/seislib/colormaps/brocO/DiscretePalettes/brocO50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/brocO/brocO.py` & `seislib-0.6.9/seislib/colormaps/brocO/brocO.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/brocO/brocO.txt` & `seislib-0.6.9/seislib/colormaps/brocO/brocO.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/buda/CategoricalPalettes/budaS.py` & `seislib-0.6.9/seislib/colormaps/buda/CategoricalPalettes/budaS.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/buda/CategoricalPalettes/budaS.txt` & `seislib-0.6.9/seislib/colormaps/buda/CategoricalPalettes/budaS.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/buda/CategoricalPalettes/budaS_HEX.txt` & `seislib-0.6.9/seislib/colormaps/buda/CategoricalPalettes/budaS_HEX.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/buda/DiscretePalettes/buda100.txt` & `seislib-0.6.9/seislib/colormaps/buda/DiscretePalettes/buda100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/buda/DiscretePalettes/buda25.txt` & `seislib-0.6.9/seislib/colormaps/buda/DiscretePalettes/buda25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/buda/DiscretePalettes/buda50.txt` & `seislib-0.6.9/seislib/colormaps/buda/DiscretePalettes/buda50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/buda/buda.py` & `seislib-0.6.9/seislib/colormaps/buda/buda.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/buda/buda.txt` & `seislib-0.6.9/seislib/colormaps/buda/buda.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bukavu/DiscretePalettes/bukavu100.txt` & `seislib-0.6.9/seislib/colormaps/bukavu/DiscretePalettes/bukavu100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bukavu/DiscretePalettes/bukavu25.txt` & `seislib-0.6.9/seislib/colormaps/bukavu/DiscretePalettes/bukavu25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bukavu/DiscretePalettes/bukavu50.txt` & `seislib-0.6.9/seislib/colormaps/bukavu/DiscretePalettes/bukavu50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bukavu/bukavu.py` & `seislib-0.6.9/seislib/colormaps/bukavu/bukavu.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/bukavu/bukavu.txt` & `seislib-0.6.9/seislib/colormaps/bukavu/bukavu.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/cork/DiscretePalettes/cork100.txt` & `seislib-0.6.9/seislib/colormaps/cork/DiscretePalettes/cork100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/cork/DiscretePalettes/cork25.txt` & `seislib-0.6.9/seislib/colormaps/cork/DiscretePalettes/cork25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/cork/DiscretePalettes/cork50.txt` & `seislib-0.6.9/seislib/colormaps/cork/DiscretePalettes/cork50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/cork/cork.py` & `seislib-0.6.9/seislib/colormaps/cork/cork.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/cork/cork.txt` & `seislib-0.6.9/seislib/colormaps/cork/cork.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/corkO/DiscretePalettes/corkO100.txt` & `seislib-0.6.9/seislib/colormaps/corkO/DiscretePalettes/corkO100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/corkO/DiscretePalettes/corkO25.txt` & `seislib-0.6.9/seislib/colormaps/corkO/DiscretePalettes/corkO25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/corkO/DiscretePalettes/corkO50.txt` & `seislib-0.6.9/seislib/colormaps/corkO/DiscretePalettes/corkO50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/corkO/corkO.py` & `seislib-0.6.9/seislib/colormaps/corkO/corkO.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/corkO/corkO.txt` & `seislib-0.6.9/seislib/colormaps/corkO/corkO.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/davos/CategoricalPalettes/davosS.py` & `seislib-0.6.9/seislib/colormaps/davos/CategoricalPalettes/davosS.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/davos/CategoricalPalettes/davosS.txt` & `seislib-0.6.9/seislib/colormaps/davos/CategoricalPalettes/davosS.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/davos/CategoricalPalettes/davosS_HEX.txt` & `seislib-0.6.9/seislib/colormaps/davos/CategoricalPalettes/davosS_HEX.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/davos/DiscretePalettes/davos100.txt` & `seislib-0.6.9/seislib/colormaps/davos/DiscretePalettes/davos100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/davos/DiscretePalettes/davos25.txt` & `seislib-0.6.9/seislib/colormaps/davos/DiscretePalettes/davos25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/davos/DiscretePalettes/davos50.txt` & `seislib-0.6.9/seislib/colormaps/davos/DiscretePalettes/davos50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/davos/davos.py` & `seislib-0.6.9/seislib/colormaps/davos/davos.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/davos/davos.txt` & `seislib-0.6.9/seislib/colormaps/davos/davos.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/devon/CategoricalPalettes/devonS.py` & `seislib-0.6.9/seislib/colormaps/devon/CategoricalPalettes/devonS.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/devon/CategoricalPalettes/devonS.txt` & `seislib-0.6.9/seislib/colormaps/devon/CategoricalPalettes/devonS.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/devon/CategoricalPalettes/devonS_HEX.txt` & `seislib-0.6.9/seislib/colormaps/devon/CategoricalPalettes/devonS_HEX.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/devon/DiscretePalettes/devon100.txt` & `seislib-0.6.9/seislib/colormaps/devon/DiscretePalettes/devon100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/devon/DiscretePalettes/devon25.txt` & `seislib-0.6.9/seislib/colormaps/devon/DiscretePalettes/devon25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/devon/DiscretePalettes/devon50.txt` & `seislib-0.6.9/seislib/colormaps/devon/DiscretePalettes/devon50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/devon/devon.py` & `seislib-0.6.9/seislib/colormaps/devon/devon.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/devon/devon.txt` & `seislib-0.6.9/seislib/colormaps/devon/devon.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/fes/DiscretePalettes/fes100.txt` & `seislib-0.6.9/seislib/colormaps/fes/DiscretePalettes/fes100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/fes/DiscretePalettes/fes25.txt` & `seislib-0.6.9/seislib/colormaps/fes/DiscretePalettes/fes25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/fes/DiscretePalettes/fes50.txt` & `seislib-0.6.9/seislib/colormaps/fes/DiscretePalettes/fes50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/fes/fes.py` & `seislib-0.6.9/seislib/colormaps/fes/fes.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/fes/fes.txt` & `seislib-0.6.9/seislib/colormaps/fes/fes.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/grayC/CategoricalPalettes/grayCS.py` & `seislib-0.6.9/seislib/colormaps/grayC/CategoricalPalettes/grayCS.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/grayC/CategoricalPalettes/grayCS.txt` & `seislib-0.6.9/seislib/colormaps/grayC/CategoricalPalettes/grayCS.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/grayC/CategoricalPalettes/grayCS_HEX.txt` & `seislib-0.6.9/seislib/colormaps/grayC/CategoricalPalettes/grayCS_HEX.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/grayC/DiscretePalettes/grayC100.txt` & `seislib-0.6.9/seislib/colormaps/grayC/DiscretePalettes/grayC100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/grayC/DiscretePalettes/grayC25.txt` & `seislib-0.6.9/seislib/colormaps/grayC/DiscretePalettes/grayC25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/grayC/DiscretePalettes/grayC50.txt` & `seislib-0.6.9/seislib/colormaps/grayC/DiscretePalettes/grayC50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/grayC/grayC.py` & `seislib-0.6.9/seislib/colormaps/grayC/grayC.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/grayC/grayC.txt` & `seislib-0.6.9/seislib/colormaps/grayC/grayC.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/hawaii/CategoricalPalettes/hawaiiS.py` & `seislib-0.6.9/seislib/colormaps/hawaii/CategoricalPalettes/hawaiiS.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/hawaii/CategoricalPalettes/hawaiiS.txt` & `seislib-0.6.9/seislib/colormaps/hawaii/CategoricalPalettes/hawaiiS.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/hawaii/CategoricalPalettes/hawaiiS_HEX.txt` & `seislib-0.6.9/seislib/colormaps/hawaii/CategoricalPalettes/hawaiiS_HEX.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/hawaii/DiscretePalettes/hawaii100.txt` & `seislib-0.6.9/seislib/colormaps/hawaii/DiscretePalettes/hawaii100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/hawaii/DiscretePalettes/hawaii25.txt` & `seislib-0.6.9/seislib/colormaps/hawaii/DiscretePalettes/hawaii25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/hawaii/DiscretePalettes/hawaii50.txt` & `seislib-0.6.9/seislib/colormaps/hawaii/DiscretePalettes/hawaii50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/hawaii/hawaii.py` & `seislib-0.6.9/seislib/colormaps/hawaii/hawaii.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/hawaii/hawaii.txt` & `seislib-0.6.9/seislib/colormaps/hawaii/hawaii.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/imola/CategoricalPalettes/imolaS.py` & `seislib-0.6.9/seislib/colormaps/imola/CategoricalPalettes/imolaS.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/imola/CategoricalPalettes/imolaS.txt` & `seislib-0.6.9/seislib/colormaps/imola/CategoricalPalettes/imolaS.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/imola/CategoricalPalettes/imolaS_HEX.txt` & `seislib-0.6.9/seislib/colormaps/imola/CategoricalPalettes/imolaS_HEX.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/imola/DiscretePalettes/imola100.txt` & `seislib-0.6.9/seislib/colormaps/imola/DiscretePalettes/imola100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/imola/DiscretePalettes/imola25.txt` & `seislib-0.6.9/seislib/colormaps/imola/DiscretePalettes/imola25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/imola/DiscretePalettes/imola50.txt` & `seislib-0.6.9/seislib/colormaps/imola/DiscretePalettes/imola50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/imola/imola.py` & `seislib-0.6.9/seislib/colormaps/imola/imola.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/imola/imola.txt` & `seislib-0.6.9/seislib/colormaps/imola/imola.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/lajolla/CategoricalPalettes/lajollaS.py` & `seislib-0.6.9/seislib/colormaps/lajolla/CategoricalPalettes/lajollaS.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/lajolla/CategoricalPalettes/lajollaS.txt` & `seislib-0.6.9/seislib/colormaps/lajolla/CategoricalPalettes/lajollaS.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/lajolla/CategoricalPalettes/lajollaS_HEX.txt` & `seislib-0.6.9/seislib/colormaps/lajolla/CategoricalPalettes/lajollaS_HEX.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/lajolla/DiscretePalettes/lajolla100.txt` & `seislib-0.6.9/seislib/colormaps/lajolla/DiscretePalettes/lajolla100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/lajolla/DiscretePalettes/lajolla25.txt` & `seislib-0.6.9/seislib/colormaps/lajolla/DiscretePalettes/lajolla25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/lajolla/DiscretePalettes/lajolla50.txt` & `seislib-0.6.9/seislib/colormaps/lajolla/DiscretePalettes/lajolla50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/lajolla/lajolla.py` & `seislib-0.6.9/seislib/colormaps/lajolla/lajolla.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/lajolla/lajolla.txt` & `seislib-0.6.9/seislib/colormaps/lajolla/lajolla.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/lapaz/CategoricalPalettes/lapazS.py` & `seislib-0.6.9/seislib/colormaps/lapaz/CategoricalPalettes/lapazS.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/lapaz/CategoricalPalettes/lapazS.txt` & `seislib-0.6.9/seislib/colormaps/lapaz/CategoricalPalettes/lapazS.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/lapaz/CategoricalPalettes/lapazS_HEX.txt` & `seislib-0.6.9/seislib/colormaps/lapaz/CategoricalPalettes/lapazS_HEX.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/lapaz/DiscretePalettes/lapaz100.txt` & `seislib-0.6.9/seislib/colormaps/lapaz/DiscretePalettes/lapaz100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/lapaz/DiscretePalettes/lapaz25.txt` & `seislib-0.6.9/seislib/colormaps/lapaz/DiscretePalettes/lapaz25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/lapaz/DiscretePalettes/lapaz50.txt` & `seislib-0.6.9/seislib/colormaps/lapaz/DiscretePalettes/lapaz50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/lapaz/lapaz.py` & `seislib-0.6.9/seislib/colormaps/lapaz/lapaz.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/lapaz/lapaz.txt` & `seislib-0.6.9/seislib/colormaps/lapaz/lapaz.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/lisbon/DiscretePalettes/lisbon100.txt` & `seislib-0.6.9/seislib/colormaps/lisbon/DiscretePalettes/lisbon100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/lisbon/DiscretePalettes/lisbon25.txt` & `seislib-0.6.9/seislib/colormaps/lisbon/DiscretePalettes/lisbon25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/lisbon/DiscretePalettes/lisbon50.txt` & `seislib-0.6.9/seislib/colormaps/lisbon/DiscretePalettes/lisbon50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/lisbon/lisbon.py` & `seislib-0.6.9/seislib/colormaps/lisbon/lisbon.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/lisbon/lisbon.txt` & `seislib-0.6.9/seislib/colormaps/lisbon/lisbon.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/nuuk/CategoricalPalettes/nuukS.py` & `seislib-0.6.9/seislib/colormaps/nuuk/CategoricalPalettes/nuukS.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/nuuk/CategoricalPalettes/nuukS.txt` & `seislib-0.6.9/seislib/colormaps/nuuk/CategoricalPalettes/nuukS.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/nuuk/CategoricalPalettes/nuukS_HEX.txt` & `seislib-0.6.9/seislib/colormaps/nuuk/CategoricalPalettes/nuukS_HEX.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/nuuk/DiscretePalettes/nuuk100.txt` & `seislib-0.6.9/seislib/colormaps/nuuk/DiscretePalettes/nuuk100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/nuuk/DiscretePalettes/nuuk25.txt` & `seislib-0.6.9/seislib/colormaps/nuuk/DiscretePalettes/nuuk25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/nuuk/DiscretePalettes/nuuk50.txt` & `seislib-0.6.9/seislib/colormaps/nuuk/DiscretePalettes/nuuk50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/nuuk/nuuk.py` & `seislib-0.6.9/seislib/colormaps/nuuk/nuuk.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/nuuk/nuuk.txt` & `seislib-0.6.9/seislib/colormaps/nuuk/nuuk.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/oleron/DiscretePalettes/oleron100.txt` & `seislib-0.6.9/seislib/colormaps/oleron/DiscretePalettes/oleron100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/oleron/DiscretePalettes/oleron25.txt` & `seislib-0.6.9/seislib/colormaps/oleron/DiscretePalettes/oleron25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/oleron/DiscretePalettes/oleron50.txt` & `seislib-0.6.9/seislib/colormaps/oleron/DiscretePalettes/oleron50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/oleron/oleron.py` & `seislib-0.6.9/seislib/colormaps/oleron/oleron.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/oleron/oleron.txt` & `seislib-0.6.9/seislib/colormaps/oleron/oleron.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/oslo/CategoricalPalettes/osloS.py` & `seislib-0.6.9/seislib/colormaps/oslo/CategoricalPalettes/osloS.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/oslo/CategoricalPalettes/osloS.txt` & `seislib-0.6.9/seislib/colormaps/oslo/CategoricalPalettes/osloS.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/oslo/CategoricalPalettes/osloS_HEX.txt` & `seislib-0.6.9/seislib/colormaps/oslo/CategoricalPalettes/osloS_HEX.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/oslo/DiscretePalettes/oslo100.txt` & `seislib-0.6.9/seislib/colormaps/oslo/DiscretePalettes/oslo100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/oslo/DiscretePalettes/oslo25.txt` & `seislib-0.6.9/seislib/colormaps/oslo/DiscretePalettes/oslo25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/oslo/DiscretePalettes/oslo50.txt` & `seislib-0.6.9/seislib/colormaps/oslo/DiscretePalettes/oslo50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/oslo/oslo.py` & `seislib-0.6.9/seislib/colormaps/oslo/oslo.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/oslo/oslo.txt` & `seislib-0.6.9/seislib/colormaps/oslo/oslo.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/roma/DiscretePalettes/roma100.txt` & `seislib-0.6.9/seislib/colormaps/roma/DiscretePalettes/roma100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/roma/DiscretePalettes/roma25.txt` & `seislib-0.6.9/seislib/colormaps/roma/DiscretePalettes/roma25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/roma/DiscretePalettes/roma50.txt` & `seislib-0.6.9/seislib/colormaps/roma/DiscretePalettes/roma50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/roma/roma.py` & `seislib-0.6.9/seislib/colormaps/roma/roma.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/roma/roma.txt` & `seislib-0.6.9/seislib/colormaps/roma/roma.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/romaO/DiscretePalettes/romaO100.txt` & `seislib-0.6.9/seislib/colormaps/romaO/DiscretePalettes/romaO100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/romaO/DiscretePalettes/romaO25.txt` & `seislib-0.6.9/seislib/colormaps/romaO/DiscretePalettes/romaO25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/romaO/DiscretePalettes/romaO50.txt` & `seislib-0.6.9/seislib/colormaps/romaO/DiscretePalettes/romaO50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/romaO/romaO.py` & `seislib-0.6.9/seislib/colormaps/romaO/romaO.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/romaO/romaO.txt` & `seislib-0.6.9/seislib/colormaps/romaO/romaO.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/tofino/DiscretePalettes/tofino100.txt` & `seislib-0.6.9/seislib/colormaps/tofino/DiscretePalettes/tofino100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/tofino/DiscretePalettes/tofino25.txt` & `seislib-0.6.9/seislib/colormaps/tofino/DiscretePalettes/tofino25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/tofino/DiscretePalettes/tofino50.txt` & `seislib-0.6.9/seislib/colormaps/tofino/DiscretePalettes/tofino50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/tofino/tofino.py` & `seislib-0.6.9/seislib/colormaps/tofino/tofino.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/tofino/tofino.txt` & `seislib-0.6.9/seislib/colormaps/tofino/tofino.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/tokyo/CategoricalPalettes/tokyoS.py` & `seislib-0.6.9/seislib/colormaps/tokyo/CategoricalPalettes/tokyoS.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/tokyo/CategoricalPalettes/tokyoS.txt` & `seislib-0.6.9/seislib/colormaps/tokyo/CategoricalPalettes/tokyoS.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/tokyo/CategoricalPalettes/tokyoS_HEX.txt` & `seislib-0.6.9/seislib/colormaps/tokyo/CategoricalPalettes/tokyoS_HEX.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/tokyo/DiscretePalettes/tokyo100.txt` & `seislib-0.6.9/seislib/colormaps/tokyo/DiscretePalettes/tokyo100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/tokyo/DiscretePalettes/tokyo25.txt` & `seislib-0.6.9/seislib/colormaps/tokyo/DiscretePalettes/tokyo25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/tokyo/DiscretePalettes/tokyo50.txt` & `seislib-0.6.9/seislib/colormaps/tokyo/DiscretePalettes/tokyo50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/tokyo/tokyo.py` & `seislib-0.6.9/seislib/colormaps/tokyo/tokyo.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/tokyo/tokyo.txt` & `seislib-0.6.9/seislib/colormaps/tokyo/tokyo.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/turku/CategoricalPalettes/turkuS.py` & `seislib-0.6.9/seislib/colormaps/turku/CategoricalPalettes/turkuS.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/turku/CategoricalPalettes/turkuS.txt` & `seislib-0.6.9/seislib/colormaps/turku/CategoricalPalettes/turkuS.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/turku/CategoricalPalettes/turkuS_HEX.txt` & `seislib-0.6.9/seislib/colormaps/turku/CategoricalPalettes/turkuS_HEX.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/turku/DiscretePalettes/turku100.txt` & `seislib-0.6.9/seislib/colormaps/turku/DiscretePalettes/turku100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/turku/DiscretePalettes/turku25.txt` & `seislib-0.6.9/seislib/colormaps/turku/DiscretePalettes/turku25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/turku/DiscretePalettes/turku50.txt` & `seislib-0.6.9/seislib/colormaps/turku/DiscretePalettes/turku50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/turku/turku.py` & `seislib-0.6.9/seislib/colormaps/turku/turku.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/turku/turku.txt` & `seislib-0.6.9/seislib/colormaps/turku/turku.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/vanimo/DiscretePalettes/vanimo100.txt` & `seislib-0.6.9/seislib/colormaps/vanimo/DiscretePalettes/vanimo100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/vanimo/DiscretePalettes/vanimo25.txt` & `seislib-0.6.9/seislib/colormaps/vanimo/DiscretePalettes/vanimo25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/vanimo/DiscretePalettes/vanimo50.txt` & `seislib-0.6.9/seislib/colormaps/vanimo/DiscretePalettes/vanimo50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/vanimo/vanimo.py` & `seislib-0.6.9/seislib/colormaps/vanimo/vanimo.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/vanimo/vanimo.txt` & `seislib-0.6.9/seislib/colormaps/vanimo/vanimo.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/vik/DiscretePalettes/vik100.txt` & `seislib-0.6.9/seislib/colormaps/vik/DiscretePalettes/vik100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/vik/DiscretePalettes/vik25.txt` & `seislib-0.6.9/seislib/colormaps/vik/DiscretePalettes/vik25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/vik/DiscretePalettes/vik50.txt` & `seislib-0.6.9/seislib/colormaps/vik/DiscretePalettes/vik50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/vik/vik.py` & `seislib-0.6.9/seislib/colormaps/vik/vik.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/vik/vik.txt` & `seislib-0.6.9/seislib/colormaps/vik/vik.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/vikO/DiscretePalettes/vikO100.txt` & `seislib-0.6.9/seislib/colormaps/vikO/DiscretePalettes/vikO100.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/vikO/DiscretePalettes/vikO25.txt` & `seislib-0.6.9/seislib/colormaps/vikO/DiscretePalettes/vikO25.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/vikO/DiscretePalettes/vikO50.txt` & `seislib-0.6.9/seislib/colormaps/vikO/DiscretePalettes/vikO50.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/vikO/vikO.py` & `seislib-0.6.9/seislib/colormaps/vikO/vikO.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/colormaps/vikO/vikO.txt` & `seislib-0.6.9/seislib/colormaps/vikO/vikO.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/eq/__init__.py` & `seislib-0.6.9/seislib/eq/__init__.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/eq/eq_downloader.py` & `seislib-0.6.9/seislib/eq/eq_downloader.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/eq/eq_velocity.py` & `seislib-0.6.9/seislib/eq/eq_velocity.py`

 * *Files 0% similar despite different names*

```diff
@@ -872,15 +872,15 @@
             eq.prepare_input_tomography(savedir=savedir,
                                         period=periods)
 
         The above will save one txt file for each specified period.
         """
         os.makedirs(savedir, exist_ok=True)
         period = np.array([period]) if np.isscalar(period) else np.array(period)
-        coords, velocity = self.interpolate_dispcurves(period)
+        codes, coords, velocity = self.interpolate_dispcurves(period)
         dist = SeismicTomography.gc_distance(*coords.T)
         wavelength = velocity * period
         ratios = dist.reshape(-1, 1) / wavelength
         velocity_final = np.where(ratios>min_no_wavelengths, velocity, np.nan)
         for iperiod, p in enumerate(period):
             save = os.path.join(savedir, outfile%p)
             vel = velocity_final[:, iperiod]
@@ -934,15 +934,15 @@
                             min_no_events=8)
 
         Even if the computation of the dispersion curves is not yet 
         finished, you can use the above instance to interpolate all the
         available dispersion curves as follows::
 
             period = [20, 30, 40, 50]
-            coords, measurements = eq.interpolate_dispcurves(period)  
+            codes, coords, measurements = eq.interpolate_dispcurves(period)  
         """   
         def display_progress(no_files, done, verbose=False):
             if verbose and not done % int(0.05*no_files + 1):
                 print('FILES PROCESSED: %d/%d'%(done, no_files))
 
         src = os.path.join(self.savedir, 'dispcurves')
         files = [i for i in sorted(os.listdir(src)) if i.endswith('npy')]
```

### Comparing `seislib-0.6.8/seislib/exceptions/exceptions.py` & `seislib-0.6.9/seislib/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/plotting/__init__.py` & `seislib-0.6.9/seislib/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/plotting/plotting.py` & `seislib-0.6.9/seislib/plotting/plotting.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/tomography/__init__.py` & `seislib-0.6.9/seislib/tomography/__init__.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/tomography/_ray_theory/_math.pyx` & `seislib-0.6.9/seislib/tomography/_ray_theory/_math.pyx`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/tomography/_ray_theory/_spherical_geometry.pyx` & `seislib-0.6.9/seislib/tomography/_ray_theory/_spherical_geometry.pyx`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/tomography/_ray_theory/_tomography.pyx` & `seislib-0.6.9/seislib/tomography/_ray_theory/_tomography.pyx`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/tomography/_ray_theory/setup_all.py` & `seislib-0.6.9/seislib/tomography/_ray_theory/setup_all.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/tomography/grid.py` & `seislib-0.6.9/seislib/tomography/grid.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/tomography/tomography.py` & `seislib-0.6.9/seislib/tomography/tomography.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/utils/__init__.py` & `seislib-0.6.9/seislib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib/utils/utils.py` & `seislib-0.6.9/seislib/utils/utils.py`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/seislib.egg-info/PKG-INFO` & `seislib-0.6.9/seislib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seislib
-Version: 0.6.8
+Version: 0.6.9
 Summary: Multi-scale Seismic Imaging
 Home-page: https://github.com/fmagrini/seislib
 Author: Fabrizio Magrini
 Author-email: fabrizio.magrini90@gmail.com
 License: MIT
 Keywords: Seismic Imaging,Surface Waves,Seismic Ambient Noise,Earthquake Seismology,Tomographic Inversion
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `seislib-0.6.8/seislib.egg-info/SOURCES.txt` & `seislib-0.6.9/seislib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seislib-0.6.8/setup.py` & `seislib-0.6.9/setup.py`

 * *Files identical despite different names*

