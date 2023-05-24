# Comparing `tmp/greedyFAS-1.9.0.tar.gz` & `tmp/greedyFAS-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greedyFAS-1.9.0.tar", last modified: Fri May 28 15:36:26 2021, max compression
+gzip compressed data, was "greedyFAS-1.9.1.tar", last modified: Fri May 28 18:38:17 2021, max compression
```

## Comparing `greedyFAS-1.9.0.tar` & `greedyFAS-1.9.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 15:36:26.579767 greedyFAS-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       31 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7024 2021-05-28 15:36:26.579767 greedyFAS-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5609 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 15:36:26.575767 greedyFAS-1.9.0/greedyFAS/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/greedyFAS/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 15:36:26.575767 greedyFAS-1.9.0/greedyFAS/annoFAS/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/greedyFAS/annoFAS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8521 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/greedyFAS/annoFAS/annoFAS.py
--rw-r--r--   0 runner    (1001) docker     (121)    19671 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/greedyFAS/annoFAS/annoModules.py
--rw-r--r--   0 runner    (1001) docker     (121)     6398 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/greedyFAS/annoFAS/annoParserFAS.py
--rw-r--r--   0 runner    (1001) docker     (121)     5687 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/greedyFAS/annoFAS/checkAnno.py
--rw-r--r--   0 runner    (1001) docker     (121)     3436 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/greedyFAS/annoFAS/getProtByAnno.py
--rw-r--r--   0 runner    (1001) docker     (121)     3320 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/greedyFAS/annoFAS/test_annofas.fa
--rw-r--r--   0 runner    (1001) docker     (121)    16675 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/greedyFAS/calcFAS.py
--rw-r--r--   0 runner    (1001) docker     (121)     5655 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/greedyFAS/complexityFAS.py
--rw-r--r--   0 runner    (1001) docker     (121)     4112 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/greedyFAS/domainFAS.py
--rw-r--r--   0 runner    (1001) docker     (121)     3641 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/greedyFAS/extractAnnoFAS.py
--rw-r--r--   0 runner    (1001) docker     (121)    12755 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/greedyFAS/fdogFAS.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 15:36:26.579767 greedyFAS-1.9.0/greedyFAS/mainFAS/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/greedyFAS/mainFAS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3024 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/greedyFAS/mainFAS/fasInput.py
--rw-r--r--   0 runner    (1001) docker     (121)     7407 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/greedyFAS/mainFAS/fasOutput.py
--rw-r--r--   0 runner    (1001) docker     (121)     3094 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/greedyFAS/mainFAS/fasPathing.py
--rw-r--r--   0 runner    (1001) docker     (121)    17011 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/greedyFAS/mainFAS/fasScoring.py
--rw-r--r--   0 runner    (1001) docker     (121)     8524 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/greedyFAS/mainFAS/fasWeighting.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    51190 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/greedyFAS/mainFAS/greedyFAS.py
--rw-r--r--   0 runner    (1001) docker     (121)    21729 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/greedyFAS/setupFAS.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 15:36:26.575767 greedyFAS-1.9.0/greedyFAS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7024 2021-05-28 15:36:26.000000 greedyFAS-1.9.0/greedyFAS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      849 2021-05-28 15:36:26.000000 greedyFAS-1.9.0/greedyFAS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-28 15:36:26.000000 greedyFAS-1.9.0/greedyFAS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      444 2021-05-28 15:36:26.000000 greedyFAS-1.9.0/greedyFAS.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-05-28 15:36:26.000000 greedyFAS-1.9.0/greedyFAS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-05-28 15:36:26.000000 greedyFAS-1.9.0/greedyFAS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-28 15:36:26.579767 greedyFAS-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2602 2021-05-28 15:32:23.000000 greedyFAS-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 18:38:17.515579 greedyFAS-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)    35147 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     7024 2021-05-28 18:38:17.515579 greedyFAS-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5609 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 18:38:17.511579 greedyFAS-1.9.1/greedyFAS/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/greedyFAS/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 18:38:17.511579 greedyFAS-1.9.1/greedyFAS/annoFAS/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/greedyFAS/annoFAS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8521 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/greedyFAS/annoFAS/annoFAS.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19671 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/greedyFAS/annoFAS/annoModules.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6398 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/greedyFAS/annoFAS/annoParserFAS.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5687 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/greedyFAS/annoFAS/checkAnno.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4057 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/greedyFAS/annoFAS/getProtByAnno.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3320 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/greedyFAS/annoFAS/test_annofas.fa
+-rw-r--r--   0 runner    (1001) docker     (121)    16675 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/greedyFAS/calcFAS.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5655 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/greedyFAS/complexityFAS.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4112 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/greedyFAS/domainFAS.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3641 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/greedyFAS/extractAnnoFAS.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12755 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/greedyFAS/fdogFAS.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 18:38:17.515579 greedyFAS-1.9.1/greedyFAS/mainFAS/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/greedyFAS/mainFAS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3024 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/greedyFAS/mainFAS/fasInput.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7407 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/greedyFAS/mainFAS/fasOutput.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3094 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/greedyFAS/mainFAS/fasPathing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17011 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/greedyFAS/mainFAS/fasScoring.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8524 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/greedyFAS/mainFAS/fasWeighting.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    51190 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/greedyFAS/mainFAS/greedyFAS.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21729 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/greedyFAS/setupFAS.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 18:38:17.511579 greedyFAS-1.9.1/greedyFAS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7024 2021-05-28 18:38:17.000000 greedyFAS-1.9.1/greedyFAS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      849 2021-05-28 18:38:17.000000 greedyFAS-1.9.1/greedyFAS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-28 18:38:17.000000 greedyFAS-1.9.1/greedyFAS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      444 2021-05-28 18:38:17.000000 greedyFAS-1.9.1/greedyFAS.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2021-05-28 18:38:17.000000 greedyFAS-1.9.1/greedyFAS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2021-05-28 18:38:17.000000 greedyFAS-1.9.1/greedyFAS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-28 18:38:17.515579 greedyFAS-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2602 2021-05-28 18:36:45.000000 greedyFAS-1.9.1/setup.py
```

### Comparing `greedyFAS-1.9.0/LICENSE` & `greedyFAS-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `greedyFAS-1.9.0/PKG-INFO` & `greedyFAS-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greedyFAS
-Version: 1.9.0
+Version: 1.9.1
 Summary: A tool to compare protein feature architectures
 Home-page: https://github.com/BIONF/FAS
 Author: Julian Dosch
 Author-email: Dosch@bio.uni-frankfurt.de
 License: GPL-3.0
 Description: # FAS - Feature Architecture Similarity
         [![PyPI version](https://badge.fury.io/py/greedyFAS.svg)](https://badge.fury.io/py/greedyFAS)
```

### Comparing `greedyFAS-1.9.0/README.md` & `greedyFAS-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `greedyFAS-1.9.0/greedyFAS/annoFAS/annoFAS.py` & `greedyFAS-1.9.1/greedyFAS/annoFAS/annoFAS.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             annoModules.save2json(annoDict, outName, outPath)
             pool.close()
         else:
             print(outFile + ' already exists!')
 
 
 def main():
-    version = '1.9.0'
+    version = '1.9.1'
     parser = argparse.ArgumentParser(description='You are running FAS version ' + str(version) + '.',
                                      epilog="For more information on certain options, please refer to the wiki pages "
                                             "on github: https://github.com/BIONF/FAS/wiki")
     required = parser.add_argument_group('required arguments')
     optional = parser.add_argument_group('optional arguments')
     required.add_argument('-i', '--fasta', help='Input sequence(s) in fasta format', action='store', default='',
                           required=True)
```

### Comparing `greedyFAS-1.9.0/greedyFAS/annoFAS/annoModules.py` & `greedyFAS-1.9.1/greedyFAS/annoFAS/annoModules.py`

 * *Files identical despite different names*

### Comparing `greedyFAS-1.9.0/greedyFAS/annoFAS/annoParserFAS.py` & `greedyFAS-1.9.1/greedyFAS/annoFAS/annoParserFAS.py`

 * *Files identical despite different names*

### Comparing `greedyFAS-1.9.0/greedyFAS/annoFAS/checkAnno.py` & `greedyFAS-1.9.1/greedyFAS/annoFAS/checkAnno.py`

 * *Files identical despite different names*

### Comparing `greedyFAS-1.9.0/greedyFAS/annoFAS/getProtByAnno.py` & `greedyFAS-1.9.1/greedyFAS/annoFAS/getProtByAnno.py`

 * *Files 27% similar despite different names*

```diff
@@ -23,57 +23,65 @@
 import sys
 import os
 import argparse
 from pathlib import Path
 import json
 import re
 
-def checkCompleteAnno(featureList, jsonFile):
+def checkCompleteAnno(featureList, jsonFile, condition):
     with open(jsonFile) as jf:
         dt = json.load(jf)
         # get list of proteins that contain selected features
         protList = []
         for prot in list(dt['feature'].keys()):
             for item in dt['feature'][prot]:
                 if isinstance(dt['feature'][prot][item], dict):
-                    if any(re.search(feat+';', ';'.join(list(dt['feature'][prot][item].keys()))+';', re.I)
-                        for feat in featureList):
-                        protList.append(prot)
+                    if condition == "ANY" or condition == "any":
+                        if any(re.search(feat+';', ';'.join(list(dt['feature'][prot][item].keys()))+';', re.I)
+                            for feat in featureList):
+                            protList.append(prot)
+                    elif condition == "ALL" or condition == "all":
+                        if all(re.search(feat+';', ';'.join(list(dt['feature'][prot][item].keys()))+';', re.I)
+                            for feat in featureList):
+                            protList.append(prot)
         # get all features for found proteins
         out = {}
         for prot in protList:
             out[prot] = []
             for item in dt['feature'][prot]:
                 if isinstance(dt['feature'][prot][item], dict):
                     features = list(dt['feature'][prot][item].keys())
                     if len(features) > 0:
                         out[prot].append(';'.join(features))
         return(out)
 
 def main():
-    version = '0.0.1'
+    version = '0.0.2'
     parser = argparse.ArgumentParser(description='You are running getProtByAnno version ' + str(version) + '.',
                                      epilog="For more information on certain options, please refer to the wiki pages "
                                             "on github: https://github.com/BIONF/FAS/wiki")
     required = parser.add_argument_group('required arguments')
     optional = parser.add_argument_group('optional arguments')
     required.add_argument('-a', '--annoFile', help='Input annotation file in json format', action='store', default='',
                           required=True)
     required.add_argument('-f', '--features', help='List of features of interest, separated by comma. E.g. pfam_ig,pfam_TMA7', action='store', default='',
                           required=True)
     optional.add_argument('-i', '--idOnly', help='Get only protein IDs', action='store_true')
+    optional.add_argument('-c','--condition', help='Choose to query based on ALL or ANY features. Default: ANY',
+                            choices=['ALL', 'all', 'ANY', 'any'], action='store', default='ANY', type=str)
 
     args = parser.parse_args()
     featureList = str(args.features).split(",")
     if len(featureList) == 0:
         sys.exit('No feature given! Please specify feature of interest using --features option!')
     jsonFile = os.path.abspath(args.annoFile)
     if not os.path.exists(jsonFile):
         sys.exit('%s not found!' % jsonFile)
     idOnly = args.idOnly
+    condition = args.condition
 
     out = checkCompleteAnno(featureList, jsonFile)
     if not idOnly:
         for prot in out:
             print('%s\t%s' % (prot, ';'.join(out[prot])))
     else:
         print('\n'.join(out))
```

### Comparing `greedyFAS-1.9.0/greedyFAS/annoFAS/test_annofas.fa` & `greedyFAS-1.9.1/greedyFAS/annoFAS/test_annofas.fa`

 * *Files identical despite different names*

### Comparing `greedyFAS-1.9.0/greedyFAS/calcFAS.py` & `greedyFAS-1.9.1/greedyFAS/calcFAS.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import multiprocessing as mp
 from greedyFAS.annoFAS import annoFAS
 from greedyFAS.annoFAS import annoModules
 from greedyFAS.mainFAS import fasInput, greedyFAS
 
 
 def get_options():
-    version = '1.9.0'
+    version = '1.9.1'
     parser = argparse.ArgumentParser(description='You are running FAS version ' + str(version) + '.',
                                      epilog="For more information on certain options, please refer to the wiki pages "
                                             "on github: https://github.com/BIONF/FAS/wiki")
     required = parser.add_argument_group('required arguments')
     general = parser.add_argument_group('general arguments')
     inargs = parser.add_argument_group('input arguments')
     outargs = parser.add_argument_group('output arguments')
```

### Comparing `greedyFAS-1.9.0/greedyFAS/complexityFAS.py` & `greedyFAS-1.9.1/greedyFAS/complexityFAS.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     pass
 from greedyFAS.mainFAS import fasPathing
 from greedyFAS.mainFAS import fasInput
 from greedyFAS.mainFAS import greedyFAS
 
 
 def get_options():
-    version = '1.9.0'
+    version = '1.9.1'
     parser = argparse.ArgumentParser(description='You are running FAS version ' + str(version) + '.',
                                      epilog="This script allows you to assess the complexity (number of paths) of the "
                                             "feature architecture for linearization.")
     required = parser.add_argument_group('required arguments')
     optional = parser.add_argument_group('optional arguments')
     parser.add_argument('--version', action='version', version=str(version))
     required.add_argument("-i", "--input", default=None, type=str, required=True,
```

### Comparing `greedyFAS-1.9.0/greedyFAS/domainFAS.py` & `greedyFAS-1.9.1/greedyFAS/domainFAS.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 from greedyFAS.mainFAS import fasInput
 import argparse
 import os
 
 
 def get_options():
-    version = '1.9.0'
+    version = '1.9.1'
     parser = argparse.ArgumentParser(description='You are running FAS version ' + str(version) + '.',
                                      epilog="This script allows you to create domain input files for phyloprofile "
                                             "without doing a FAS calculation.")
     required = parser.add_argument_group('required arguments')
     optional = parser.add_argument_group('optional arguments')
     parser.add_argument('--version', action='version', version=str(version))
     required.add_argument("-j", "--json", default=None, type=str, required=True,
```

### Comparing `greedyFAS-1.9.0/greedyFAS/extractAnnoFAS.py` & `greedyFAS-1.9.1/greedyFAS/extractAnnoFAS.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import json
 from tqdm import tqdm
 from time import sleep
 from greedyFAS.mainFAS.fasInput import read_json
 
 
 def get_options():
-    version = '1.9.0'
+    version = '1.9.1'
     parser = argparse.ArgumentParser(description='You are running FAS version ' + str(version) + '.',
                                      epilog="For more information on certain options, please refer to the wiki pages "
                                             "on github: https://github.com/BIONF/FAS/wiki")
     required = parser.add_argument_group('required arguments')
     parser.add_argument('--version', action='version', version=str(version))
     required.add_argument("-x", "--extract_ids", default=None, type=str, required=True,
                           help="path to file, which contains a list of ids that should be extracted")
```

### Comparing `greedyFAS-1.9.0/greedyFAS/fdogFAS.py` & `greedyFAS-1.9.1/greedyFAS/fdogFAS.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
                     out.write(seed + "\tncbi" + ncbi + "\t" + seed + "|" + spec + "|" + pair[1] + "|" +
                               groupdict[pair[0]][seed][pair[1]] + "\t" + str(result[0][pair][0]) + "\t" +
                               str(result[0][pair][1]) + "\n")
     out.close()
 
 
 def get_options():
-    version = '1.9.0'
+    version = '1.9.1'
     parser = argparse.ArgumentParser(description='You are running FAS version ' + str(version) + '.',
                                      epilog="For more information on certain options, please refer to the wiki pages "
                                             "on github: https://github.com/BIONF/FAS/wiki")
     required = parser.add_argument_group('required arguments')
     optional = parser.add_argument_group('optional arguments')
     parser.add_argument('--version', action='version', version=str(version))
     required.add_argument("-i", "--extended_fa", default=None, type=str, required=True,
```

### Comparing `greedyFAS-1.9.0/greedyFAS/mainFAS/fasInput.py` & `greedyFAS-1.9.1/greedyFAS/mainFAS/fasInput.py`

 * *Files identical despite different names*

### Comparing `greedyFAS-1.9.0/greedyFAS/mainFAS/fasOutput.py` & `greedyFAS-1.9.1/greedyFAS/mainFAS/fasOutput.py`

 * *Files identical despite different names*

### Comparing `greedyFAS-1.9.0/greedyFAS/mainFAS/fasPathing.py` & `greedyFAS-1.9.1/greedyFAS/mainFAS/fasPathing.py`

 * *Files identical despite different names*

### Comparing `greedyFAS-1.9.0/greedyFAS/mainFAS/fasScoring.py` & `greedyFAS-1.9.1/greedyFAS/mainFAS/fasScoring.py`

 * *Files identical despite different names*

### Comparing `greedyFAS-1.9.0/greedyFAS/mainFAS/fasWeighting.py` & `greedyFAS-1.9.1/greedyFAS/mainFAS/fasWeighting.py`

 * *Files identical despite different names*

### Comparing `greedyFAS-1.9.0/greedyFAS/mainFAS/greedyFAS.py` & `greedyFAS-1.9.1/greedyFAS/mainFAS/greedyFAS.py`

 * *Files identical despite different names*

### Comparing `greedyFAS-1.9.0/greedyFAS/setupFAS.py` & `greedyFAS-1.9.1/greedyFAS/setupFAS.py`

 * *Files 0% similar despite different names*

```diff
@@ -448,15 +448,15 @@
         print('annoFAS -i test_annofas.fa -o testFas_output')
         sys.exit()
     else:
         sys.exit('Some errors occur with annotation tools. Please check if they can be excuted at %s' % anno_path)
 
 
 def main():
-    version = '1.9.0'
+    version = '1.9.1'
     parser = argparse.ArgumentParser(description='You are running setupFAS version ' + str(version) + '.')
     required = parser.add_argument_group('required arguments')
     optional = parser.add_argument_group('optional arguments')
     required.add_argument('-t', '--toolPath', help='Set path to save annotation tools', action='store', default='',
                           required=True)
     optional.add_argument('-d', '--dtuPath', help='Set path to DTU tools (SignalP and TMHMM)', action='store',
                           default='')
```

### Comparing `greedyFAS-1.9.0/greedyFAS.egg-info/PKG-INFO` & `greedyFAS-1.9.1/greedyFAS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greedyFAS
-Version: 1.9.0
+Version: 1.9.1
 Summary: A tool to compare protein feature architectures
 Home-page: https://github.com/BIONF/FAS
 Author: Julian Dosch
 Author-email: Dosch@bio.uni-frankfurt.de
 License: GPL-3.0
 Description: # FAS - Feature Architecture Similarity
         [![PyPI version](https://badge.fury.io/py/greedyFAS.svg)](https://badge.fury.io/py/greedyFAS)
```

### Comparing `greedyFAS-1.9.0/greedyFAS.egg-info/SOURCES.txt` & `greedyFAS-1.9.1/greedyFAS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `greedyFAS-1.9.0/setup.py` & `greedyFAS-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as input:
     long_description = input.read()
 
 setup(
     name="greedyFAS",
-    version="1.9.0",
+    version="1.9.1",
     python_requires='>=3.7.0',
     description="A tool to compare protein feature architectures",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Julian Dosch",
     author_email="Dosch@bio.uni-frankfurt.de",
     url="https://github.com/BIONF/FAS",
```

