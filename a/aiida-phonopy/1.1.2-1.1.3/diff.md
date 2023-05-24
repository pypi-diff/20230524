# Comparing `tmp/aiida_phonopy-1.1.2.tar.gz` & `tmp/aiida_phonopy-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_phonopy-1.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiida_phonopy-1.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida_phonopy-1.1.2.tar` & `aiida_phonopy-1.1.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     6148 2023-05-22 14:56:26.138166 aiida_phonopy-1.1.2/.DS_Store
--rw-r--r--   0        0        0     3763 2023-05-22 14:56:26.138166 aiida_phonopy-1.1.2/.github/workflows/cd.yml
--rw-r--r--   0        0        0     2397 2023-05-22 14:56:26.138166 aiida_phonopy-1.1.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1512 2023-05-22 14:56:26.138166 aiida_phonopy-1.1.2/.github/workflows/validate_release_tag.py
--rw-r--r--   0        0        0      501 2023-05-22 14:56:26.138166 aiida_phonopy-1.1.2/.gitignore
--rw-r--r--   0        0        0     1034 2023-05-22 14:56:26.138166 aiida_phonopy-1.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      300 2023-05-22 14:56:26.138166 aiida_phonopy-1.1.2/.readthedocs.yml
--rw-r--r--   0        0        0     4299 2023-05-22 14:56:26.138166 aiida_phonopy-1.1.2/CHANGELOG.md
--rw-r--r--   0        0        0     1085 2023-05-22 14:56:26.138166 aiida_phonopy-1.1.2/LICENSE.txt
--rw-r--r--   0        0        0     1816 2023-05-22 14:56:26.138166 aiida_phonopy-1.1.2/README.md
--rw-r--r--   0        0        0      155 2023-05-22 14:56:26.138166 aiida_phonopy-1.1.2/docker-compose.yml
--rw-r--r--   0        0        0      455 2023-05-22 14:56:26.154166 aiida_phonopy-1.1.2/environment.yml
--rw-r--r--   0        0        0    52380 2023-05-22 14:56:26.154166 aiida_phonopy-1.1.2/examples/BaTiO3/FORCE_SETS
--rw-r--r--   0        0        0    21945 2023-05-22 14:56:26.154166 aiida_phonopy-1.1.2/examples/BaTiO3/phonopy.yaml
--rw-r--r--   0        0        0    52380 2023-05-22 14:56:26.154166 aiida_phonopy-1.1.2/examples/BaTiO3/ref_out/FORCE_SETS
--rw-r--r--   0        0        0       41 2023-05-22 14:56:26.154166 aiida_phonopy-1.1.2/examples/BaTiO3/ref_out/aiida.in
--rw-r--r--   0        0        0     1538 2023-05-22 14:56:26.154166 aiida_phonopy-1.1.2/examples/BaTiO3/ref_out/aiida.out
--rw-r--r--   0        0        0    58620 2023-05-22 14:56:26.154166 aiida_phonopy-1.1.2/examples/BaTiO3/ref_out/band.hdf5
--rw-r--r--   0        0        0    43797 2023-05-22 14:56:26.154166 aiida_phonopy-1.1.2/examples/BaTiO3/ref_out/force_constants.hdf5
--rw-r--r--   0        0        0     2445 2023-05-22 14:56:26.154166 aiida_phonopy-1.1.2/examples/BaTiO3/ref_out/irreps.yaml
--rw-r--r--   0        0        0    39220 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/examples/BaTiO3/ref_out/mesh.hdf5
--rw-r--r--   0        0        0    21837 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/examples/BaTiO3/ref_out/phonopy.yaml
--rw-r--r--   0        0        0     2336 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/examples/BaTiO3/ref_out/qpoints.hdf5
--rw-r--r--   0        0        0    33644 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/examples/BaTiO3/ref_out/thermal_properties.yaml
--rw-r--r--   0        0        0     1254 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/examples/BaTiO3/script.py
--rw-r--r--   0        0        0    49210 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/examples/Si/preprocess.ipynb
--rw-r--r--   0        0        0     3514 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/pyproject.toml
--rw-r--r--   0        0        0       91 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/src/aiida_phonopy/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/src/aiida_phonopy/calculations/__init__.py
--rw-r--r--   0        0        0       62 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/src/aiida_phonopy/calculations/functions/__init__.py
--rw-r--r--   0        0        0    10711 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/src/aiida_phonopy/calculations/functions/data_utils.py
--rw-r--r--   0        0        0     4037 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/src/aiida_phonopy/calculations/functions/link_structures.py
--rw-r--r--   0        0        0    18253 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/src/aiida_phonopy/calculations/phonopy.py
--rw-r--r--   0        0        0      271 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/src/aiida_phonopy/data/__init__.py
--rw-r--r--   0        0        0     4298 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/src/aiida_phonopy/data/force_constants.py
--rw-r--r--   0        0        0    10128 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/src/aiida_phonopy/data/phonopy.py
--rw-r--r--   0        0        0    13397 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/src/aiida_phonopy/data/preprocess.py
--rw-r--r--   0        0        0    21571 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/src/aiida_phonopy/data/raw.py
--rw-r--r--   0        0        0       65 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/src/aiida_phonopy/parsers/__init__.py
--rw-r--r--   0        0        0     2450 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/src/aiida_phonopy/parsers/base.py
--rw-r--r--   0        0        0    18608 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/src/aiida_phonopy/parsers/phonopy.py
--rw-r--r--   0        0        0        0 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/src/aiida_phonopy/parsers/raw_parsers/__init__.py
--rw-r--r--   0        0        0     1080 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/src/aiida_phonopy/parsers/raw_parsers/phonopy.py
--rw-r--r--   0        0        0        0 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/src/aiida_phonopy/utils/__init__.py
--rw-r--r--   0        0        0     2138 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/src/aiida_phonopy/utils/mapping.py
--rw-r--r--   0        0        0      688 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/src/aiida_phonopy/utils/resources.py
--rw-r--r--   0        0        0        0 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/src/aiida_phonopy/workflows/__init__.py
--rw-r--r--   0        0        0    15542 2023-05-22 14:56:26.158166 aiida_phonopy-1.1.2/src/aiida_phonopy/workflows/phonopy.py
--rw-r--r--   0        0        0     3647 1970-01-01 00:00:00.000000 aiida_phonopy-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2023-05-24 20:30:19.245475 aiida_phonopy-1.1.3/.DS_Store
+-rw-r--r--   0        0        0     3763 2023-05-24 20:30:19.245475 aiida_phonopy-1.1.3/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     2397 2023-05-24 20:30:19.245475 aiida_phonopy-1.1.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1512 2023-05-24 20:30:19.245475 aiida_phonopy-1.1.3/.github/workflows/validate_release_tag.py
+-rw-r--r--   0        0        0      501 2023-05-24 20:30:19.245475 aiida_phonopy-1.1.3/.gitignore
+-rw-r--r--   0        0        0     1034 2023-05-24 20:30:19.245475 aiida_phonopy-1.1.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      300 2023-05-24 20:30:19.245475 aiida_phonopy-1.1.3/.readthedocs.yml
+-rw-r--r--   0        0        0     4299 2023-05-24 20:30:19.245475 aiida_phonopy-1.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1085 2023-05-24 20:30:19.245475 aiida_phonopy-1.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     1816 2023-05-24 20:30:19.245475 aiida_phonopy-1.1.3/README.md
+-rw-r--r--   0        0        0      155 2023-05-24 20:30:19.245475 aiida_phonopy-1.1.3/docker-compose.yml
+-rw-r--r--   0        0        0      455 2023-05-24 20:30:19.261475 aiida_phonopy-1.1.3/environment.yml
+-rw-r--r--   0        0        0    52380 2023-05-24 20:30:19.261475 aiida_phonopy-1.1.3/examples/BaTiO3/FORCE_SETS
+-rw-r--r--   0        0        0    21945 2023-05-24 20:30:19.261475 aiida_phonopy-1.1.3/examples/BaTiO3/phonopy.yaml
+-rw-r--r--   0        0        0    52380 2023-05-24 20:30:19.261475 aiida_phonopy-1.1.3/examples/BaTiO3/ref_out/FORCE_SETS
+-rw-r--r--   0        0        0       41 2023-05-24 20:30:19.261475 aiida_phonopy-1.1.3/examples/BaTiO3/ref_out/aiida.in
+-rw-r--r--   0        0        0     1538 2023-05-24 20:30:19.261475 aiida_phonopy-1.1.3/examples/BaTiO3/ref_out/aiida.out
+-rw-r--r--   0        0        0    58620 2023-05-24 20:30:19.261475 aiida_phonopy-1.1.3/examples/BaTiO3/ref_out/band.hdf5
+-rw-r--r--   0        0        0    43797 2023-05-24 20:30:19.261475 aiida_phonopy-1.1.3/examples/BaTiO3/ref_out/force_constants.hdf5
+-rw-r--r--   0        0        0     2445 2023-05-24 20:30:19.261475 aiida_phonopy-1.1.3/examples/BaTiO3/ref_out/irreps.yaml
+-rw-r--r--   0        0        0    39220 2023-05-24 20:30:19.261475 aiida_phonopy-1.1.3/examples/BaTiO3/ref_out/mesh.hdf5
+-rw-r--r--   0        0        0    21837 2023-05-24 20:30:19.261475 aiida_phonopy-1.1.3/examples/BaTiO3/ref_out/phonopy.yaml
+-rw-r--r--   0        0        0     2336 2023-05-24 20:30:19.261475 aiida_phonopy-1.1.3/examples/BaTiO3/ref_out/qpoints.hdf5
+-rw-r--r--   0        0        0    33644 2023-05-24 20:30:19.261475 aiida_phonopy-1.1.3/examples/BaTiO3/ref_out/thermal_properties.yaml
+-rw-r--r--   0        0        0     1254 2023-05-24 20:30:19.261475 aiida_phonopy-1.1.3/examples/BaTiO3/script.py
+-rw-r--r--   0        0        0    49210 2023-05-24 20:30:19.261475 aiida_phonopy-1.1.3/examples/Si/preprocess.ipynb
+-rw-r--r--   0        0        0     3514 2023-05-24 20:30:19.261475 aiida_phonopy-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0       91 2023-05-24 20:30:19.261475 aiida_phonopy-1.1.3/src/aiida_phonopy/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 20:30:19.265475 aiida_phonopy-1.1.3/src/aiida_phonopy/calculations/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-24 20:30:19.265475 aiida_phonopy-1.1.3/src/aiida_phonopy/calculations/functions/__init__.py
+-rw-r--r--   0        0        0    10710 2023-05-24 20:30:19.265475 aiida_phonopy-1.1.3/src/aiida_phonopy/calculations/functions/data_utils.py
+-rw-r--r--   0        0        0     4037 2023-05-24 20:30:19.265475 aiida_phonopy-1.1.3/src/aiida_phonopy/calculations/functions/link_structures.py
+-rw-r--r--   0        0        0    18253 2023-05-24 20:30:19.265475 aiida_phonopy-1.1.3/src/aiida_phonopy/calculations/phonopy.py
+-rw-r--r--   0        0        0      271 2023-05-24 20:30:19.265475 aiida_phonopy-1.1.3/src/aiida_phonopy/data/__init__.py
+-rw-r--r--   0        0        0     4298 2023-05-24 20:30:19.265475 aiida_phonopy-1.1.3/src/aiida_phonopy/data/force_constants.py
+-rw-r--r--   0        0        0    10128 2023-05-24 20:30:19.265475 aiida_phonopy-1.1.3/src/aiida_phonopy/data/phonopy.py
+-rw-r--r--   0        0        0    13397 2023-05-24 20:30:19.265475 aiida_phonopy-1.1.3/src/aiida_phonopy/data/preprocess.py
+-rw-r--r--   0        0        0    21571 2023-05-24 20:30:19.265475 aiida_phonopy-1.1.3/src/aiida_phonopy/data/raw.py
+-rw-r--r--   0        0        0       65 2023-05-24 20:30:19.265475 aiida_phonopy-1.1.3/src/aiida_phonopy/parsers/__init__.py
+-rw-r--r--   0        0        0     2450 2023-05-24 20:30:19.265475 aiida_phonopy-1.1.3/src/aiida_phonopy/parsers/base.py
+-rw-r--r--   0        0        0    18608 2023-05-24 20:30:19.265475 aiida_phonopy-1.1.3/src/aiida_phonopy/parsers/phonopy.py
+-rw-r--r--   0        0        0        0 2023-05-24 20:30:19.265475 aiida_phonopy-1.1.3/src/aiida_phonopy/parsers/raw_parsers/__init__.py
+-rw-r--r--   0        0        0     1080 2023-05-24 20:30:19.265475 aiida_phonopy-1.1.3/src/aiida_phonopy/parsers/raw_parsers/phonopy.py
+-rw-r--r--   0        0        0        0 2023-05-24 20:30:19.265475 aiida_phonopy-1.1.3/src/aiida_phonopy/utils/__init__.py
+-rw-r--r--   0        0        0     2138 2023-05-24 20:30:19.265475 aiida_phonopy-1.1.3/src/aiida_phonopy/utils/mapping.py
+-rw-r--r--   0        0        0      688 2023-05-24 20:30:19.265475 aiida_phonopy-1.1.3/src/aiida_phonopy/utils/resources.py
+-rw-r--r--   0        0        0        0 2023-05-24 20:30:19.265475 aiida_phonopy-1.1.3/src/aiida_phonopy/workflows/__init__.py
+-rw-r--r--   0        0        0    15542 2023-05-24 20:30:19.265475 aiida_phonopy-1.1.3/src/aiida_phonopy/workflows/phonopy.py
+-rw-r--r--   0        0        0     3647 1970-01-01 00:00:00.000000 aiida_phonopy-1.1.3/PKG-INFO
```

### Comparing `aiida_phonopy-1.1.2/.DS_Store` & `aiida_phonopy-1.1.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/.github/workflows/cd.yml` & `aiida_phonopy-1.1.3/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/.github/workflows/ci.yml` & `aiida_phonopy-1.1.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/.github/workflows/validate_release_tag.py` & `aiida_phonopy-1.1.3/.github/workflows/validate_release_tag.py`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/.pre-commit-config.yaml` & `aiida_phonopy-1.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/CHANGELOG.md` & `aiida_phonopy-1.1.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/LICENSE.txt` & `aiida_phonopy-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/README.md` & `aiida_phonopy-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/examples/BaTiO3/FORCE_SETS` & `aiida_phonopy-1.1.3/examples/BaTiO3/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/examples/BaTiO3/phonopy.yaml` & `aiida_phonopy-1.1.3/examples/BaTiO3/phonopy.yaml`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/examples/BaTiO3/ref_out/FORCE_SETS` & `aiida_phonopy-1.1.3/examples/BaTiO3/ref_out/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/examples/BaTiO3/ref_out/aiida.out` & `aiida_phonopy-1.1.3/examples/BaTiO3/ref_out/aiida.out`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/examples/BaTiO3/ref_out/band.hdf5` & `aiida_phonopy-1.1.3/examples/BaTiO3/ref_out/band.hdf5`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/examples/BaTiO3/ref_out/force_constants.hdf5` & `aiida_phonopy-1.1.3/examples/BaTiO3/ref_out/force_constants.hdf5`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/examples/BaTiO3/ref_out/irreps.yaml` & `aiida_phonopy-1.1.3/examples/BaTiO3/ref_out/irreps.yaml`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/examples/BaTiO3/ref_out/mesh.hdf5` & `aiida_phonopy-1.1.3/examples/BaTiO3/ref_out/mesh.hdf5`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/examples/BaTiO3/ref_out/phonopy.yaml` & `aiida_phonopy-1.1.3/examples/BaTiO3/ref_out/phonopy.yaml`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/examples/BaTiO3/ref_out/qpoints.hdf5` & `aiida_phonopy-1.1.3/examples/BaTiO3/ref_out/qpoints.hdf5`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/examples/BaTiO3/ref_out/thermal_properties.yaml` & `aiida_phonopy-1.1.3/examples/BaTiO3/ref_out/thermal_properties.yaml`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/examples/BaTiO3/script.py` & `aiida_phonopy-1.1.3/examples/BaTiO3/script.py`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/examples/Si/preprocess.ipynb` & `aiida_phonopy-1.1.3/examples/Si/preprocess.ipynb`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/pyproject.toml` & `aiida_phonopy-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/src/aiida_phonopy/calculations/functions/data_utils.py` & `aiida_phonopy-1.1.3/src/aiida_phonopy/calculations/functions/data_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 @calcfunction
 def generate_preprocess_data(
     structure: orm.StructureData,
     displacement_generator: orm.Dict | None = None,
     supercell_matrix: orm.List | None = None,
     primitive_matrix: orm.List | None = None,
     symprec: orm.Float | None = None,
-    is_symmetry: orm.Float | None = None,
+    is_symmetry: orm.Bool | None = None,
     distinguish_kinds: orm.Bool | None = None,
 ):
     """Return a complete stored PreProcessData node.
 
     :param structure: structure data node representing the unitcell
     :type structure: :class:`~aiida.orm.StructureData`
     :param displacement_generator: dictionary containing the info for generating the displacements
```

### Comparing `aiida_phonopy-1.1.2/src/aiida_phonopy/calculations/functions/link_structures.py` & `aiida_phonopy-1.1.3/src/aiida_phonopy/calculations/functions/link_structures.py`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/src/aiida_phonopy/calculations/phonopy.py` & `aiida_phonopy-1.1.3/src/aiida_phonopy/calculations/phonopy.py`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/src/aiida_phonopy/data/force_constants.py` & `aiida_phonopy-1.1.3/src/aiida_phonopy/data/force_constants.py`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/src/aiida_phonopy/data/phonopy.py` & `aiida_phonopy-1.1.3/src/aiida_phonopy/data/phonopy.py`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/src/aiida_phonopy/data/preprocess.py` & `aiida_phonopy-1.1.3/src/aiida_phonopy/data/preprocess.py`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/src/aiida_phonopy/data/raw.py` & `aiida_phonopy-1.1.3/src/aiida_phonopy/data/raw.py`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/src/aiida_phonopy/parsers/base.py` & `aiida_phonopy-1.1.3/src/aiida_phonopy/parsers/base.py`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/src/aiida_phonopy/parsers/phonopy.py` & `aiida_phonopy-1.1.3/src/aiida_phonopy/parsers/phonopy.py`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/src/aiida_phonopy/parsers/raw_parsers/phonopy.py` & `aiida_phonopy-1.1.3/src/aiida_phonopy/parsers/raw_parsers/phonopy.py`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/src/aiida_phonopy/utils/mapping.py` & `aiida_phonopy-1.1.3/src/aiida_phonopy/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/src/aiida_phonopy/utils/resources.py` & `aiida_phonopy-1.1.3/src/aiida_phonopy/utils/resources.py`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/src/aiida_phonopy/workflows/phonopy.py` & `aiida_phonopy-1.1.3/src/aiida_phonopy/workflows/phonopy.py`

 * *Files identical despite different names*

### Comparing `aiida_phonopy-1.1.2/PKG-INFO` & `aiida_phonopy-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-phonopy
-Version: 1.1.2
+Version: 1.1.3
 Summary: The official AiiDA plugin for Phonopy
 Keywords: aiida,phonopy,workflows
 Author-email: Lorenzo Bastonero <bastonero.lorenzo@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
```

