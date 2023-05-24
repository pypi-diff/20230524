# Comparing `tmp/NuMeTriS-0.0.8.tar.gz` & `tmp/NuMeTriS-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NuMeTriS-0.0.8.tar", last modified: Tue May 23 08:25:10 2023, max compression
+gzip compressed data, was "NuMeTriS-0.0.9.tar", last modified: Wed May 24 16:25:05 2023, max compression
```

## Comparing `NuMeTriS-0.0.8.tar` & `NuMeTriS-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 08:25:10.046504 NuMeTriS-0.0.8/
--rw-rw-r--   0 mars      (1000) mars      (1000)    35149 2023-05-23 08:23:41.000000 NuMeTriS-0.0.8/LICENSE
--rw-rw-r--   0 mars      (1000) mars      (1000)     9563 2023-05-23 08:25:10.046504 NuMeTriS-0.0.8/PKG-INFO
--rw-rw-r--   0 mars      (1000) mars      (1000)     8577 2023-05-23 08:23:41.000000 NuMeTriS-0.0.8/README.md
--rw-rw-r--   0 mars      (1000) mars      (1000)     1380 2023-05-23 08:23:41.000000 NuMeTriS-0.0.8/pyproject.toml
--rw-rw-r--   0 mars      (1000) mars      (1000)       38 2023-05-23 08:25:10.046504 NuMeTriS-0.0.8/setup.cfg
--rw-rw-r--   0 mars      (1000) mars      (1000)      136 2023-05-23 08:23:41.000000 NuMeTriS-0.0.8/setup.py
-drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 08:25:10.042504 NuMeTriS-0.0.8/src/
-drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 08:25:10.042504 NuMeTriS-0.0.8/src/NuMeTriS/
--rw-rw-r--   0 mars      (1000) mars      (1000)    23127 2023-05-23 08:23:41.000000 NuMeTriS-0.0.8/src/NuMeTriS/Graph_Class.py
--rw-rw-r--   0 mars      (1000) mars      (1000)    69485 2023-05-23 08:23:41.000000 NuMeTriS-0.0.8/src/NuMeTriS/Utility_Functions.py
--rw-rw-r--   0 mars      (1000) mars      (1000)      183 2023-05-23 08:23:41.000000 NuMeTriS-0.0.8/src/NuMeTriS/__init__.py
-drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 08:25:10.042504 NuMeTriS-0.0.8/src/NuMeTriS.egg-info/
--rw-rw-r--   0 mars      (1000) mars      (1000)     9563 2023-05-23 08:25:10.000000 NuMeTriS-0.0.8/src/NuMeTriS.egg-info/PKG-INFO
--rw-rw-r--   0 mars      (1000) mars      (1000)      395 2023-05-23 08:25:10.000000 NuMeTriS-0.0.8/src/NuMeTriS.egg-info/SOURCES.txt
--rw-rw-r--   0 mars      (1000) mars      (1000)        1 2023-05-23 08:25:10.000000 NuMeTriS-0.0.8/src/NuMeTriS.egg-info/dependency_links.txt
--rw-rw-r--   0 mars      (1000) mars      (1000)       94 2023-05-23 08:25:10.000000 NuMeTriS-0.0.8/src/NuMeTriS.egg-info/requires.txt
--rw-rw-r--   0 mars      (1000) mars      (1000)        9 2023-05-23 08:25:10.000000 NuMeTriS-0.0.8/src/NuMeTriS.egg-info/top_level.txt
-drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-23 08:25:10.046504 NuMeTriS-0.0.8/tests/
--rw-rw-r--   0 mars      (1000) mars      (1000)      693 2023-05-23 08:23:41.000000 NuMeTriS-0.0.8/tests/test_DBCM.py
--rw-rw-r--   0 mars      (1000) mars      (1000)      703 2023-05-23 08:23:41.000000 NuMeTriS-0.0.8/tests/test_DBCM_CReMa.py
--rw-rw-r--   0 mars      (1000) mars      (1000)      693 2023-05-23 08:23:41.000000 NuMeTriS-0.0.8/tests/test_RBCM.py
--rw-rw-r--   0 mars      (1000) mars      (1000)      703 2023-05-23 08:23:41.000000 NuMeTriS-0.0.8/tests/test_RBCM_CRWCM.py
+drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-24 16:25:05.543990 NuMeTriS-0.0.9/
+-rw-rw-r--   0 mars      (1000) mars      (1000)    35149 2023-05-24 16:21:13.000000 NuMeTriS-0.0.9/LICENSE
+-rw-rw-r--   0 mars      (1000) mars      (1000)     9922 2023-05-24 16:25:05.543990 NuMeTriS-0.0.9/PKG-INFO
+-rw-rw-r--   0 mars      (1000) mars      (1000)     8936 2023-05-24 16:21:13.000000 NuMeTriS-0.0.9/README.md
+-rw-rw-r--   0 mars      (1000) mars      (1000)     1380 2023-05-24 16:21:13.000000 NuMeTriS-0.0.9/pyproject.toml
+-rw-rw-r--   0 mars      (1000) mars      (1000)       38 2023-05-24 16:25:05.543990 NuMeTriS-0.0.9/setup.cfg
+-rw-rw-r--   0 mars      (1000) mars      (1000)      136 2023-05-24 16:21:13.000000 NuMeTriS-0.0.9/setup.py
+drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-24 16:25:05.539988 NuMeTriS-0.0.9/src/
+drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-24 16:25:05.539988 NuMeTriS-0.0.9/src/NuMeTriS/
+-rw-rw-r--   0 mars      (1000) mars      (1000)    23127 2023-05-24 16:21:13.000000 NuMeTriS-0.0.9/src/NuMeTriS/Graph_Class.py
+-rw-rw-r--   0 mars      (1000) mars      (1000)    69485 2023-05-24 16:21:13.000000 NuMeTriS-0.0.9/src/NuMeTriS/Utility_Functions.py
+-rw-rw-r--   0 mars      (1000) mars      (1000)      183 2023-05-24 16:21:13.000000 NuMeTriS-0.0.9/src/NuMeTriS/__init__.py
+drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-24 16:25:05.543990 NuMeTriS-0.0.9/src/NuMeTriS.egg-info/
+-rw-rw-r--   0 mars      (1000) mars      (1000)     9922 2023-05-24 16:25:05.000000 NuMeTriS-0.0.9/src/NuMeTriS.egg-info/PKG-INFO
+-rw-rw-r--   0 mars      (1000) mars      (1000)      395 2023-05-24 16:25:05.000000 NuMeTriS-0.0.9/src/NuMeTriS.egg-info/SOURCES.txt
+-rw-rw-r--   0 mars      (1000) mars      (1000)        1 2023-05-24 16:25:05.000000 NuMeTriS-0.0.9/src/NuMeTriS.egg-info/dependency_links.txt
+-rw-rw-r--   0 mars      (1000) mars      (1000)       94 2023-05-24 16:25:05.000000 NuMeTriS-0.0.9/src/NuMeTriS.egg-info/requires.txt
+-rw-rw-r--   0 mars      (1000) mars      (1000)        9 2023-05-24 16:25:05.000000 NuMeTriS-0.0.9/src/NuMeTriS.egg-info/top_level.txt
+drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-24 16:25:05.543990 NuMeTriS-0.0.9/tests/
+-rw-rw-r--   0 mars      (1000) mars      (1000)      693 2023-05-24 16:21:13.000000 NuMeTriS-0.0.9/tests/test_DBCM.py
+-rw-rw-r--   0 mars      (1000) mars      (1000)      703 2023-05-24 16:21:13.000000 NuMeTriS-0.0.9/tests/test_DBCM_CReMa.py
+-rw-rw-r--   0 mars      (1000) mars      (1000)      693 2023-05-24 16:21:13.000000 NuMeTriS-0.0.9/tests/test_RBCM.py
+-rw-rw-r--   0 mars      (1000) mars      (1000)      703 2023-05-24 16:21:13.000000 NuMeTriS-0.0.9/tests/test_RBCM_CRWCM.py
```

### Comparing `NuMeTriS-0.0.8/LICENSE` & `NuMeTriS-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `NuMeTriS-0.0.8/PKG-INFO` & `NuMeTriS-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NuMeTriS
-Version: 0.0.8
+Version: 0.0.9
 Summary: NuMeTris is a package for Maximum-Entropy models for triadic pattern detection. It contains known models such as DBCM and RBCM for binary motif analysis, and contain mixture models such as DBCM+CReMa and RBCM+CRWCM for weighted triadic motif analysis. The models are solved and routine are present for numeric ensemble generation and the computation of the triadic z-scores for triadic sub-graph occurrence, average flux and intensity.
 Author-email: Marzio Di Vece <marzio.divece@imtlucca.it>
 Project-URL: Homepage, https://github.com/MarsMDK/NuMeTriS
 Keywords: maximum entropy methods,network motifs,pattern detection,graph,network,entropy
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -177,9 +177,9 @@
 
 *Author*:
 
 [Marzio Di Vece](https://www.imtlucca.it/it/marzio.divece) (a.k.a. [MarsMDK](https://github.com/MarsMDK))
 
 *Acknowledgments*:
 The module was developed under the supervision of [Diego Garlaschelli](https://www.imtlucca.it/en/diego.garlaschelli) and [Frank P. Pijpers](https://www.uva.nl/profiel/p/i/f.p.pijpers/f.p.pijpers.html).
-It was developed at [IMT School for Advanced Studies Lucca](https://www.imtlucca.it/en) and [Statistics Netherlands](https://www.cbs.nl/en-gb) and
-supported by the Italian ‘Programma di Attività Integrata’ (PAI) project ‘Prosociality, Cognition and Peer Effects’ (Pro.Co.P.E.), funded by IMT School for Advanced Studies.
+It was developed at [IMT School for Advanced Studies Lucca](https://www.imtlucca.it/en) and [Statistics Netherlands](https://www.cbs.nl/en-gb).
+This work is supported by the European Union - Horizon 2020 Program under the scheme “INFRAIA-01-2018-2019 – Integrating Activities for Advanced Communities”, Grant Agreement n. 871042, ‘SoBigData++: European Integrated Infrastructure for Social Mining and Big Data Analytics’ [(http://www.sobigdata.eu)](http://www.sobigdata.eu). This module was also supported by the Italian ‘Programma di Attività Integrata’ (PAI) project ‘Prosociality, Cognition and Peer Effects’ (Pro.Co.P.E.), funded by IMT School for Advanced Studies.
```

### Comparing `NuMeTriS-0.0.8/README.md` & `NuMeTriS-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -162,9 +162,9 @@
 
 *Author*:
 
 [Marzio Di Vece](https://www.imtlucca.it/it/marzio.divece) (a.k.a. [MarsMDK](https://github.com/MarsMDK))
 
 *Acknowledgments*:
 The module was developed under the supervision of [Diego Garlaschelli](https://www.imtlucca.it/en/diego.garlaschelli) and [Frank P. Pijpers](https://www.uva.nl/profiel/p/i/f.p.pijpers/f.p.pijpers.html).
-It was developed at [IMT School for Advanced Studies Lucca](https://www.imtlucca.it/en) and [Statistics Netherlands](https://www.cbs.nl/en-gb) and
-supported by the Italian ‘Programma di Attività Integrata’ (PAI) project ‘Prosociality, Cognition and Peer Effects’ (Pro.Co.P.E.), funded by IMT School for Advanced Studies.
+It was developed at [IMT School for Advanced Studies Lucca](https://www.imtlucca.it/en) and [Statistics Netherlands](https://www.cbs.nl/en-gb).
+This work is supported by the European Union - Horizon 2020 Program under the scheme “INFRAIA-01-2018-2019 – Integrating Activities for Advanced Communities”, Grant Agreement n. 871042, ‘SoBigData++: European Integrated Infrastructure for Social Mining and Big Data Analytics’ [(http://www.sobigdata.eu)](http://www.sobigdata.eu). This module was also supported by the Italian ‘Programma di Attività Integrata’ (PAI) project ‘Prosociality, Cognition and Peer Effects’ (Pro.Co.P.E.), funded by IMT School for Advanced Studies.
```

### Comparing `NuMeTriS-0.0.8/pyproject.toml` & `NuMeTriS-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NuMeTriS"
-version = "0.0.8"
+version = "0.0.9"
 description = "NuMeTris is a package for Maximum-Entropy models for triadic pattern detection. It contains known models such as DBCM and RBCM for binary motif analysis, and contain mixture models such as DBCM+CReMa and RBCM+CRWCM for weighted triadic motif analysis. The models are solved and routine are present for numeric ensemble generation and the computation of the triadic z-scores for triadic sub-graph occurrence, average flux and intensity."
 readme = "README.md"
 license = {file = "GNU General Public License v3"}
 authors = [{ name = "Marzio Di Vece", email = "marzio.divece@imtlucca.it" }]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3.9",
```

### Comparing `NuMeTriS-0.0.8/src/NuMeTriS/Graph_Class.py` & `NuMeTriS-0.0.9/src/NuMeTriS/Graph_Class.py`

 * *Files identical despite different names*

### Comparing `NuMeTriS-0.0.8/src/NuMeTriS/Utility_Functions.py` & `NuMeTriS-0.0.9/src/NuMeTriS/Utility_Functions.py`

 * *Files identical despite different names*

### Comparing `NuMeTriS-0.0.8/src/NuMeTriS.egg-info/PKG-INFO` & `NuMeTriS-0.0.9/src/NuMeTriS.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NuMeTriS
-Version: 0.0.8
+Version: 0.0.9
 Summary: NuMeTris is a package for Maximum-Entropy models for triadic pattern detection. It contains known models such as DBCM and RBCM for binary motif analysis, and contain mixture models such as DBCM+CReMa and RBCM+CRWCM for weighted triadic motif analysis. The models are solved and routine are present for numeric ensemble generation and the computation of the triadic z-scores for triadic sub-graph occurrence, average flux and intensity.
 Author-email: Marzio Di Vece <marzio.divece@imtlucca.it>
 Project-URL: Homepage, https://github.com/MarsMDK/NuMeTriS
 Keywords: maximum entropy methods,network motifs,pattern detection,graph,network,entropy
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -177,9 +177,9 @@
 
 *Author*:
 
 [Marzio Di Vece](https://www.imtlucca.it/it/marzio.divece) (a.k.a. [MarsMDK](https://github.com/MarsMDK))
 
 *Acknowledgments*:
 The module was developed under the supervision of [Diego Garlaschelli](https://www.imtlucca.it/en/diego.garlaschelli) and [Frank P. Pijpers](https://www.uva.nl/profiel/p/i/f.p.pijpers/f.p.pijpers.html).
-It was developed at [IMT School for Advanced Studies Lucca](https://www.imtlucca.it/en) and [Statistics Netherlands](https://www.cbs.nl/en-gb) and
-supported by the Italian ‘Programma di Attività Integrata’ (PAI) project ‘Prosociality, Cognition and Peer Effects’ (Pro.Co.P.E.), funded by IMT School for Advanced Studies.
+It was developed at [IMT School for Advanced Studies Lucca](https://www.imtlucca.it/en) and [Statistics Netherlands](https://www.cbs.nl/en-gb).
+This work is supported by the European Union - Horizon 2020 Program under the scheme “INFRAIA-01-2018-2019 – Integrating Activities for Advanced Communities”, Grant Agreement n. 871042, ‘SoBigData++: European Integrated Infrastructure for Social Mining and Big Data Analytics’ [(http://www.sobigdata.eu)](http://www.sobigdata.eu). This module was also supported by the Italian ‘Programma di Attività Integrata’ (PAI) project ‘Prosociality, Cognition and Peer Effects’ (Pro.Co.P.E.), funded by IMT School for Advanced Studies.
```

### Comparing `NuMeTriS-0.0.8/tests/test_DBCM.py` & `NuMeTriS-0.0.9/tests/test_DBCM.py`

 * *Files identical despite different names*

### Comparing `NuMeTriS-0.0.8/tests/test_DBCM_CReMa.py` & `NuMeTriS-0.0.9/tests/test_DBCM_CReMa.py`

 * *Files identical despite different names*

### Comparing `NuMeTriS-0.0.8/tests/test_RBCM.py` & `NuMeTriS-0.0.9/tests/test_RBCM.py`

 * *Files identical despite different names*

### Comparing `NuMeTriS-0.0.8/tests/test_RBCM_CRWCM.py` & `NuMeTriS-0.0.9/tests/test_RBCM_CRWCM.py`

 * *Files identical despite different names*

