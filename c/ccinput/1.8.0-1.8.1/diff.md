# Comparing `tmp/ccinput-1.8.0.tar.gz` & `tmp/ccinput-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccinput-1.8.0.tar", last modified: Sun Apr 23 15:50:23 2023, max compression
+gzip compressed data, was "ccinput-1.8.1.tar", last modified: Wed May 24 15:34:38 2023, max compression
```

## Comparing `ccinput-1.8.0.tar` & `ccinput-1.8.1.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:50:23.621481 ccinput-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-23 15:49:46.000000 ccinput-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-23 15:49:46.000000 ccinput-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-23 15:50:23.621481 ccinput-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-23 15:49:46.000000 ccinput-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:50:23.621481 ccinput-1.8.0/ccinput/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-23 15:50:23.621481 ccinput-1.8.0/ccinput/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/calculation.py
--rw-r--r--   0 runner    (1001) docker     (123)    76266 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/documentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:50:23.621481 ccinput-1.8.0/ccinput/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/drivers/pysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:50:23.621481 ccinput-1.8.0/ccinput/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/packages/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/packages/nwchem.py
--rw-r--r--   0 runner    (1001) docker     (123)    15963 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/packages/orca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/packages/psi4.py
--rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/packages/qchem.py
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/packages/xtb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/presets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:50:23.621481 ccinput-1.8.0/ccinput/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/tests/test_calculation.py
--rw-r--r--   0 runner    (1001) docker     (123)    38742 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)   111131 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/tests/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)    57036 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/tests/test_orca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/tests/test_psi4.py
--rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/tests/test_pysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    47385 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/tests/test_qchem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/tests/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)    22171 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/tests/test_xtb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/tests/testing_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    15174 2023-04-23 15:49:46.000000 ccinput-1.8.0/ccinput/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:50:23.617481 ccinput-1.8.0/ccinput.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-23 15:50:23.000000 ccinput-1.8.0/ccinput.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-23 15:50:23.000000 ccinput-1.8.0/ccinput.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 15:50:23.000000 ccinput-1.8.0/ccinput.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-23 15:50:23.000000 ccinput-1.8.0/ccinput.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 15:50:23.000000 ccinput-1.8.0/ccinput.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-23 15:50:23.000000 ccinput-1.8.0/ccinput.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 15:50:23.000000 ccinput-1.8.0/ccinput.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-23 15:49:46.000000 ccinput-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-23 15:50:23.621481 ccinput-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-23 15:49:46.000000 ccinput-1.8.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-23 15:49:46.000000 ccinput-1.8.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:34:38.119289 ccinput-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-24 15:33:49.000000 ccinput-1.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 15:33:49.000000 ccinput-1.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-24 15:34:38.119289 ccinput-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-05-24 15:33:49.000000 ccinput-1.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:34:38.119289 ccinput-1.8.1/ccinput/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-24 15:34:38.119289 ccinput-1.8.1/ccinput/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76266 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/documentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:34:38.115289 ccinput-1.8.1/ccinput/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/drivers/pysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:34:38.115289 ccinput-1.8.1/ccinput/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/packages/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/packages/nwchem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15963 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/packages/orca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/packages/psi4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/packages/qchem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/packages/xtb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/presets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:34:38.119289 ccinput-1.8.1/ccinput/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/tests/test_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38742 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)   111131 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/tests/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59121 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/tests/test_orca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/tests/test_psi4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/tests/test_pysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47385 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/tests/test_qchem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/tests/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22171 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/tests/test_xtb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/tests/testing_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18972 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/verify_sanity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15174 2023-05-24 15:33:49.000000 ccinput-1.8.1/ccinput/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:34:38.115289 ccinput-1.8.1/ccinput.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-24 15:34:38.000000 ccinput-1.8.1/ccinput.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-24 15:34:38.000000 ccinput-1.8.1/ccinput.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:34:38.000000 ccinput-1.8.1/ccinput.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-24 15:34:38.000000 ccinput-1.8.1/ccinput.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:34:38.000000 ccinput-1.8.1/ccinput.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 15:34:38.000000 ccinput-1.8.1/ccinput.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 15:34:38.000000 ccinput-1.8.1/ccinput.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-24 15:33:49.000000 ccinput-1.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-24 15:34:38.119289 ccinput-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-24 15:33:49.000000 ccinput-1.8.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-05-24 15:33:49.000000 ccinput-1.8.1/versioneer.py
```

### Comparing `ccinput-1.8.0/LICENSE` & `ccinput-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.0/PKG-INFO` & `ccinput-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccinput
-Version: 1.8.0
+Version: 1.8.1
 Summary: Computational Chemistry Input Generator
 Home-page: http://github.com/cyllab/ccinput
 Author: Raphaël Robidas
 Author-email: Raphael.Robidas@USherbrooke.ca
 License: BSD 3-Clause
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ccinput-1.8.0/README.md` & `ccinput-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.0/ccinput/calculation.py` & `ccinput-1.8.1/ccinput/calculation.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.0/ccinput/constants.py` & `ccinput-1.8.1/ccinput/constants.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.0/ccinput/documentation.py` & `ccinput-1.8.1/ccinput/documentation.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.0/ccinput/drivers/pysis.py` & `ccinput-1.8.1/ccinput/drivers/pysis.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.0/ccinput/packages/gaussian.py` & `ccinput-1.8.1/ccinput/packages/gaussian.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.0/ccinput/packages/nwchem.py` & `ccinput-1.8.1/ccinput/packages/nwchem.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.0/ccinput/packages/orca.py` & `ccinput-1.8.1/ccinput/packages/orca.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,15 @@
                         success = True
                 else:
                     success = True
 
                 # TODO: handle auxiliary basis sets
 
             if success:
-                custom_bs += _custom_bs.strip()
+                custom_bs += _custom_bs
             else:
                 bs = bse.get_basis(
                     bs_keyword, fmt="ORCA", elements=[el_num], header=False
                 ).strip()
                 sbs = bs.split("\n")
                 if bs.find("ECP") != -1:
                     clean_bs = "\n".join(sbs[3:]).strip() + "\n"
@@ -330,15 +330,15 @@
                 else:
                     clean_bs = "\n".join(sbs[3:-1]).strip() + "\n"
                     custom_bs += f"newgto {el}\n"
                     custom_bs += clean_bs.strip()
                     custom_bs += "end"
 
         if custom_bs != "":
-            self.blocks.append(BS_TEMPLATE.format(custom_bs))
+            self.blocks.append(BS_TEMPLATE.format(custom_bs.strip()))
 
     def handle_xyz(self):
         lines = [i + "\n" for i in clean_xyz(self.calc.xyz).split("\n") if i != ""]
         self.xyz_structure = "".join(lines)
 
     def handle_pal_mem(self):
         if self.calc.parameters.theory_level == "semiempirical":
```

### Comparing `ccinput-1.8.0/ccinput/packages/psi4.py` & `ccinput-1.8.1/ccinput/packages/psi4.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.0/ccinput/packages/qchem.py` & `ccinput-1.8.1/ccinput/packages/qchem.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.0/ccinput/packages/xtb.py` & `ccinput-1.8.1/ccinput/packages/xtb.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.0/ccinput/presets.py` & `ccinput-1.8.1/ccinput/presets.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.0/ccinput/tests/test_calculation.py` & `ccinput-1.8.1/ccinput/tests/test_calculation.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.0/ccinput/tests/test_cli.py` & `ccinput-1.8.1/ccinput/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -704,15 +704,15 @@
         distance: 1, 3, auto
         atoms: 1,3
         $metadyn
         atoms: 2,4-9"""
 
         self.assertTrue(self.is_equivalent(INPUT_REF, objs[0].input_file))
         self.assertEqual(
-            objs[0].command, "crest ethanol.xyz -cinp input -rthr 0.6 -ewin 6"
+            objs[0].command, "crest ethanol.xyz -cinp input -rthr 2.0 -ewin 6"
         )
 
     @patch("ccinput.utilities.warn")
     def test_warn_unknown(self, warn_fn):
         warn_fn.side_effect = self.get_warn
         line = 'Gaussian sp abcd -bs cc-pvdz --xyz "Cl 0 0 0" -c -1'
         parser = get_parser()
```

### Comparing `ccinput-1.8.0/ccinput/tests/test_gaussian.py` & `ccinput-1.8.1/ccinput/tests/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.0/ccinput/tests/test_orca.py` & `ccinput-1.8.1/ccinput/tests/test_orca.py`

 * *Files 2% similar despite different names*

```diff
@@ -1414,14 +1414,68 @@
         %pal
         nprocs 8
         end
         """
 
         self.assertTrue(self.is_equivalent(REF, inp.input_file))
 
+    def test_opt_DFT_two_custom_bs_ecp(self):
+        params = {
+            "nproc": 8,
+            "type": "Geometrical Optimisation",
+            "file": "Ph2I_cation.xyz",
+            "software": "ORCA",
+            "charge": "+1",
+            "method": "B3LYP",
+            "basis_set": "6-31+G(d,p)",
+            "custom_basis_sets": "I=Def2-TZVPD;H=Def2-TZVP",
+        }
+
+        inp = self.generate_calculation(**params)
+
+        REF = """
+        !OPT B3LYP 6-31+G(d,p)
+        *xyz 1 1
+        C         -3.06870       -2.28540        0.00000
+        C         -1.67350       -2.28540        0.00000
+        C         -0.97600       -1.07770        0.00000
+        C         -1.67360        0.13090       -0.00120
+        C         -3.06850        0.13080       -0.00170
+        C         -3.76610       -1.07740       -0.00070
+        H         -3.61840       -3.23770        0.00040
+        H         -1.12400       -3.23790        0.00130
+        H          0.12370       -1.07760        0.00060
+        H         -1.12340        1.08300       -0.00130
+        H         -4.86570       -1.07720       -0.00090
+        I         -4.11890        1.94920       -0.00350
+        C         -4.64360        2.85690       -1.82310
+        C         -3.77180        3.76300       -2.42740
+        C         -5.86360        2.55380       -2.42750
+        C         -4.12020        4.36650       -3.63560
+        H         -2.81040        4.00240       -1.95030
+        C         -6.21180        3.15650       -3.63650
+        H         -6.55070        1.83950       -1.95140
+        C         -5.34050        4.06290       -4.24060
+        H         -3.43340        5.08120       -4.11170
+        H         -7.17360        2.91710       -4.11310
+        H         -5.61500        4.53870       -5.19320
+        *
+        %basis
+        NewGTO I "Def2-TZVPD" end
+        NewECP I "def2-ECP" end
+        NewGTO H "Def2-TZVP" end
+        end
+        %MaxCore 125
+        %pal
+        nprocs 8
+        end
+        """
+
+        self.assertTrue(self.is_equivalent(REF, inp.input_file))
+
     def test_opt_DFT_custom_bs_ecp_synonym(self):
         params = {
             "nproc": 8,
             "type": "Geometrical Optimisation",
             "file": "Ph2I_cation.xyz",
             "software": "ORCA",
             "charge": "+1",
```

### Comparing `ccinput-1.8.0/ccinput/tests/test_psi4.py` & `ccinput-1.8.1/ccinput/tests/test_psi4.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.0/ccinput/tests/test_pysis.py` & `ccinput-1.8.1/ccinput/tests/test_pysis.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.0/ccinput/tests/test_qchem.py` & `ccinput-1.8.1/ccinput/tests/test_qchem.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.0/ccinput/tests/test_structures.py` & `ccinput-1.8.1/ccinput/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.0/ccinput/tests/test_xtb.py` & `ccinput-1.8.1/ccinput/tests/test_xtb.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,15 +356,15 @@
             "type": "Conformational Search",
             "file": "ethanol.xyz",
             "software": "xtb",
         }
 
         xtb = self.generate_calculation(**params)
 
-        REF = "crest ethanol.xyz -rthr 0.6 -ewin 6"
+        REF = "crest ethanol.xyz -rthr 2.0 -ewin 6"
 
         self.assertTrue(self.is_equivalent(REF, xtb.command))
 
         self.assertEqual("", xtb.input_file)
 
     def test_conformational_search_specs(self):
         params = {
@@ -404,15 +404,15 @@
             "file": "ethanol.xyz",
             "software": "xtb",
             "constraints": "Freeze/1_2;",
         }
 
         xtb = self.generate_calculation(**params)
 
-        REF = "crest ethanol.xyz -cinp input -rthr 0.6 -ewin 6"
+        REF = "crest ethanol.xyz -cinp input -rthr 2.0 -ewin 6"
         self.assertTrue(self.is_equivalent(REF, xtb.command))
 
         INPUT = """$constrain
         force constant=1.0
         reference=ethanol.xyz
         distance: 1, 2, auto
         atoms: 1-2
@@ -427,15 +427,15 @@
             "file": "ethanol.xyz",
             "software": "xtb",
             "constraints": "Freeze/1_4;Freeze/6_8;",
         }
 
         xtb = self.generate_calculation(**params)
 
-        REF = "crest ethanol.xyz -cinp input -rthr 0.6 -ewin 6"
+        REF = "crest ethanol.xyz -cinp input -rthr 2.0 -ewin 6"
         self.assertTrue(self.is_equivalent(REF, xtb.command))
 
         INPUT = """$constrain
         force constant=1.0
         reference=ethanol.xyz
         distance: 1, 4, auto
         distance: 6, 8, auto
@@ -451,15 +451,15 @@
             "file": "ethanol.xyz",
             "software": "xtb",
             "constraints": "Freeze/2_3;",
         }
 
         xtb = self.generate_calculation(**params)
 
-        REF = "crest ethanol.xyz -cinp input -rthr 0.6 -ewin 6"
+        REF = "crest ethanol.xyz -cinp input -rthr 2.0 -ewin 6"
         self.assertTrue(self.is_equivalent(REF, xtb.command))
 
         INPUT = """$constrain
         force constant=1.0
         reference=ethanol.xyz
         distance: 2, 3, auto
         atoms: 2-3
@@ -475,15 +475,15 @@
             "software": "xtb",
             "constraints": "Freeze/2_3;",
             "specifications": "--force_constant 2.0",
         }
 
         xtb = self.generate_calculation(**params)
 
-        REF = "crest ethanol.xyz -cinp input -rthr 0.6 -ewin 6"
+        REF = "crest ethanol.xyz -cinp input -rthr 2.0 -ewin 6"
         self.assertTrue(self.is_equivalent(REF, xtb.command))
 
         INPUT = """$constrain
         force constant=2.0
         reference=ethanol.xyz
         distance: 2, 3, auto
         atoms: 2-3
@@ -499,15 +499,15 @@
             "software": "xtb",
             "constraints": "Freeze/2_3;Freeze/3_4;",
             "specifications": "--force_constant 2.0",
         }
 
         xtb = self.generate_calculation(**params)
 
-        REF = "crest ethanol.xyz -cinp input -rthr 0.6 -ewin 6"
+        REF = "crest ethanol.xyz -cinp input -rthr 2.0 -ewin 6"
         self.assertTrue(self.is_equivalent(REF, xtb.command))
 
         INPUT = """$constrain
         force constant=2.0
         reference=ethanol.xyz
         distance: 2, 3, auto
         distance: 3, 4, auto
@@ -524,15 +524,15 @@
             "software": "xtb",
             "constraints": "Freeze/1_2;",
             "output": "inp",
         }
 
         xtb = self.generate_calculation(**params)
 
-        REF = "crest ethanol.xyz -cinp inp -rthr 0.6 -ewin 6"
+        REF = "crest ethanol.xyz -cinp inp -rthr 2.0 -ewin 6"
         self.assertTrue(self.is_equivalent(REF, xtb.command))
 
         INPUT = """$constrain
         force constant=1.0
         reference=ethanol.xyz
         distance: 1, 2, auto
         atoms: 1-2
@@ -559,15 +559,15 @@
             "software": "xtb",
             "constraints": "Freeze/2_3;",
             "specifications": "--force_constant=2.0",
         }
 
         xtb = self.generate_calculation(**params)
 
-        REF = "crest ethanol.xyz -cinp input -rthr 0.6 -ewin 6"
+        REF = "crest ethanol.xyz -cinp input -rthr 2.0 -ewin 6"
         self.assertTrue(self.is_equivalent(REF, xtb.command))
 
         INPUT = """$constrain
         force constant=2.0
         reference=ethanol.xyz
         distance: 2, 3, auto
         atoms: 2-3
```

### Comparing `ccinput-1.8.0/ccinput/utilities.py` & `ccinput-1.8.1/ccinput/utilities.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.0/ccinput/wrapper.py` & `ccinput-1.8.1/ccinput/wrapper.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.0/ccinput.egg-info/PKG-INFO` & `ccinput-1.8.1/ccinput.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccinput
-Version: 1.8.0
+Version: 1.8.1
 Summary: Computational Chemistry Input Generator
 Home-page: http://github.com/cyllab/ccinput
 Author: Raphaël Robidas
 Author-email: Raphael.Robidas@USherbrooke.ca
 License: BSD 3-Clause
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ccinput-1.8.0/ccinput.egg-info/SOURCES.txt` & `ccinput-1.8.1/ccinput.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ccinput/_version.py
 ccinput/calculation.py
 ccinput/constants.py
 ccinput/documentation.py
 ccinput/exceptions.py
 ccinput/presets.py
 ccinput/utilities.py
+ccinput/verify_sanity.py
 ccinput/wrapper.py
 ccinput.egg-info/PKG-INFO
 ccinput.egg-info/SOURCES.txt
 ccinput.egg-info/dependency_links.txt
 ccinput.egg-info/entry_points.txt
 ccinput.egg-info/not-zip-safe
 ccinput.egg-info/requires.txt
```

### Comparing `ccinput-1.8.0/setup.py` & `ccinput-1.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.8.0/versioneer.py` & `ccinput-1.8.1/versioneer.py`

 * *Files identical despite different names*

