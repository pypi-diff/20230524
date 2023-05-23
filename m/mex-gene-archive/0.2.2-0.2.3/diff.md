# Comparing `tmp/mex_gene_archive-0.2.2.tar.gz` & `tmp/mex_gene_archive-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mex_gene_archive-0.2.2.tar", last modified: Thu May  4 20:46:26 2023, max compression
+gzip compressed data, was "mex_gene_archive-0.2.3.tar", last modified: Tue May 23 23:28:07 2023, max compression
```

## Comparing `mex_gene_archive-0.2.2.tar` & `mex_gene_archive-0.2.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-04 20:46:26.622010 mex_gene_archive-0.2.2/
-drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-04 20:46:26.606010 mex_gene_archive-0.2.2/.github/
-drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-04 20:46:26.614010 mex_gene_archive-0.2.2/.github/workflows/
--rw-r--r--   0 diane     (1000) diane     (1000)      654 2021-10-26 21:45:01.000000 mex_gene_archive-0.2.2/.github/workflows/ci-test.yml
--rw-r--r--   0 diane     (1000) diane     (1000)      129 2023-05-04 18:43:03.000000 mex_gene_archive-0.2.2/.gitignore
--rw-r--r--   0 diane     (1000) diane     (1000)     1255 2023-05-04 18:43:03.000000 mex_gene_archive-0.2.2/Changelog.rst
--rw-r--r--   0 diane     (1000) diane     (1000)     1547 2021-10-26 17:27:08.000000 mex_gene_archive-0.2.2/LICENSE.txt
--rw-r--r--   0 diane     (1000) diane     (1000)     2809 2023-05-04 20:46:26.622010 mex_gene_archive-0.2.2/PKG-INFO
--rw-r--r--   0 diane     (1000) diane     (1000)     2337 2023-04-28 17:46:50.000000 mex_gene_archive-0.2.2/README.rst
-drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-04 20:46:26.618010 mex_gene_archive-0.2.2/mex_gene_archive/
--rw-r--r--   0 diane     (1000) diane     (1000)        0 2021-10-26 17:27:08.000000 mex_gene_archive-0.2.2/mex_gene_archive/__init__.py
--rw-r--r--   0 diane     (1000) diane     (1000)      160 2023-05-04 20:46:26.000000 mex_gene_archive-0.2.2/mex_gene_archive/_version.py
--rw-r--r--   0 diane     (1000) diane     (1000)     5199 2023-04-29 06:07:52.000000 mex_gene_archive-0.2.2/mex_gene_archive/anndata.py
--rw-r--r--   0 diane     (1000) diane     (1000)     5312 2022-01-13 20:01:28.000000 mex_gene_archive-0.2.2/mex_gene_archive/filter.py
--rw-r--r--   0 diane     (1000) diane     (1000)     4291 2023-05-01 19:12:18.000000 mex_gene_archive-0.2.2/mex_gene_archive/manifest.py
--rw-r--r--   0 diane     (1000) diane     (1000)     5051 2023-04-29 00:36:47.000000 mex_gene_archive-0.2.2/mex_gene_archive/reader.py
--rw-r--r--   0 diane     (1000) diane     (1000)     7338 2023-05-04 18:43:03.000000 mex_gene_archive-0.2.2/mex_gene_archive/starsolo.py
-drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-04 20:46:26.618010 mex_gene_archive-0.2.2/mex_gene_archive.egg-info/
--rw-r--r--   0 diane     (1000) diane     (1000)     2809 2023-05-04 20:46:26.000000 mex_gene_archive-0.2.2/mex_gene_archive.egg-info/PKG-INFO
--rw-r--r--   0 diane     (1000) diane     (1000)      635 2023-05-04 20:46:26.000000 mex_gene_archive-0.2.2/mex_gene_archive.egg-info/SOURCES.txt
--rw-r--r--   0 diane     (1000) diane     (1000)        1 2023-05-04 20:46:26.000000 mex_gene_archive-0.2.2/mex_gene_archive.egg-info/dependency_links.txt
--rw-r--r--   0 diane     (1000) diane     (1000)       29 2023-05-04 20:46:26.000000 mex_gene_archive-0.2.2/mex_gene_archive.egg-info/requires.txt
--rw-r--r--   0 diane     (1000) diane     (1000)       23 2023-05-04 20:46:26.000000 mex_gene_archive-0.2.2/mex_gene_archive.egg-info/top_level.txt
--rw-r--r--   0 diane     (1000) diane     (1000)      396 2023-04-28 21:37:26.000000 mex_gene_archive-0.2.2/pyproject.toml
--rw-r--r--   0 diane     (1000) diane     (1000)      624 2023-05-04 20:46:26.622010 mex_gene_archive-0.2.2/setup.cfg
--rw-r--r--   0 diane     (1000) diane     (1000)       69 2021-10-26 17:27:08.000000 mex_gene_archive-0.2.2/setup.py
-drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-04 20:46:26.622010 mex_gene_archive-0.2.2/tests/
--rw-r--r--   0 diane     (1000) diane     (1000)        0 2021-10-26 17:27:08.000000 mex_gene_archive-0.2.2/tests/__init__.py
--rw-r--r--   0 diane     (1000) diane     (1000)    31823 2023-05-04 18:43:03.000000 mex_gene_archive-0.2.2/tests/stage_data.py
--rw-r--r--   0 diane     (1000) diane     (1000)     3327 2023-05-04 18:43:03.000000 mex_gene_archive-0.2.2/tests/test_anndata.py
--rw-r--r--   0 diane     (1000) diane     (1000)     2431 2021-10-26 17:27:08.000000 mex_gene_archive-0.2.2/tests/test_filter.py
--rw-r--r--   0 diane     (1000) diane     (1000)     3754 2023-05-01 19:15:57.000000 mex_gene_archive-0.2.2/tests/test_manifest.py
--rw-r--r--   0 diane     (1000) diane     (1000)    12358 2023-05-04 18:43:03.000000 mex_gene_archive-0.2.2/tests/test_starsolo.py
+drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-23 23:28:07.979447 mex_gene_archive-0.2.3/
+drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-23 23:28:07.975447 mex_gene_archive-0.2.3/.github/
+drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-23 23:28:07.975447 mex_gene_archive-0.2.3/.github/workflows/
+-rw-r--r--   0 diane     (1000) diane     (1000)      654 2021-10-26 21:45:01.000000 mex_gene_archive-0.2.3/.github/workflows/ci-test.yml
+-rw-r--r--   0 diane     (1000) diane     (1000)      129 2023-05-04 18:43:03.000000 mex_gene_archive-0.2.3/.gitignore
+-rw-r--r--   0 diane     (1000) diane     (1000)     1477 2023-05-23 23:20:13.000000 mex_gene_archive-0.2.3/Changelog.rst
+-rw-r--r--   0 diane     (1000) diane     (1000)     1547 2021-10-26 17:27:08.000000 mex_gene_archive-0.2.3/LICENSE.txt
+-rw-r--r--   0 diane     (1000) diane     (1000)     2809 2023-05-23 23:28:07.979447 mex_gene_archive-0.2.3/PKG-INFO
+-rw-r--r--   0 diane     (1000) diane     (1000)     2337 2023-04-28 17:46:50.000000 mex_gene_archive-0.2.3/README.rst
+drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-23 23:28:07.979447 mex_gene_archive-0.2.3/mex_gene_archive/
+-rw-r--r--   0 diane     (1000) diane     (1000)        0 2021-10-26 17:27:08.000000 mex_gene_archive-0.2.3/mex_gene_archive/__init__.py
+-rw-r--r--   0 diane     (1000) diane     (1000)      160 2023-05-23 23:28:07.000000 mex_gene_archive-0.2.3/mex_gene_archive/_version.py
+-rw-r--r--   0 diane     (1000) diane     (1000)     5211 2023-05-23 22:59:18.000000 mex_gene_archive-0.2.3/mex_gene_archive/anndata.py
+-rw-r--r--   0 diane     (1000) diane     (1000)     5312 2022-01-13 20:01:28.000000 mex_gene_archive-0.2.3/mex_gene_archive/filter.py
+-rw-r--r--   0 diane     (1000) diane     (1000)     4291 2023-05-01 19:12:18.000000 mex_gene_archive-0.2.3/mex_gene_archive/manifest.py
+-rw-r--r--   0 diane     (1000) diane     (1000)     5051 2023-04-29 00:36:47.000000 mex_gene_archive-0.2.3/mex_gene_archive/reader.py
+-rw-r--r--   0 diane     (1000) diane     (1000)     7338 2023-05-04 18:43:03.000000 mex_gene_archive-0.2.3/mex_gene_archive/starsolo.py
+drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-23 23:28:07.979447 mex_gene_archive-0.2.3/mex_gene_archive.egg-info/
+-rw-r--r--   0 diane     (1000) diane     (1000)     2809 2023-05-23 23:28:07.000000 mex_gene_archive-0.2.3/mex_gene_archive.egg-info/PKG-INFO
+-rw-r--r--   0 diane     (1000) diane     (1000)      635 2023-05-23 23:28:07.000000 mex_gene_archive-0.2.3/mex_gene_archive.egg-info/SOURCES.txt
+-rw-r--r--   0 diane     (1000) diane     (1000)        1 2023-05-23 23:28:07.000000 mex_gene_archive-0.2.3/mex_gene_archive.egg-info/dependency_links.txt
+-rw-r--r--   0 diane     (1000) diane     (1000)       29 2023-05-23 23:28:07.000000 mex_gene_archive-0.2.3/mex_gene_archive.egg-info/requires.txt
+-rw-r--r--   0 diane     (1000) diane     (1000)       23 2023-05-23 23:28:07.000000 mex_gene_archive-0.2.3/mex_gene_archive.egg-info/top_level.txt
+-rw-r--r--   0 diane     (1000) diane     (1000)      396 2023-04-28 21:37:26.000000 mex_gene_archive-0.2.3/pyproject.toml
+-rw-r--r--   0 diane     (1000) diane     (1000)      624 2023-05-23 23:28:07.983447 mex_gene_archive-0.2.3/setup.cfg
+-rw-r--r--   0 diane     (1000) diane     (1000)       69 2021-10-26 17:27:08.000000 mex_gene_archive-0.2.3/setup.py
+drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-23 23:28:07.979447 mex_gene_archive-0.2.3/tests/
+-rw-r--r--   0 diane     (1000) diane     (1000)        0 2021-10-26 17:27:08.000000 mex_gene_archive-0.2.3/tests/__init__.py
+-rw-r--r--   0 diane     (1000) diane     (1000)    31823 2023-05-04 18:43:03.000000 mex_gene_archive-0.2.3/tests/stage_data.py
+-rw-r--r--   0 diane     (1000) diane     (1000)     4564 2023-05-23 22:59:38.000000 mex_gene_archive-0.2.3/tests/test_anndata.py
+-rw-r--r--   0 diane     (1000) diane     (1000)     2431 2021-10-26 17:27:08.000000 mex_gene_archive-0.2.3/tests/test_filter.py
+-rw-r--r--   0 diane     (1000) diane     (1000)     3754 2023-05-01 19:15:57.000000 mex_gene_archive-0.2.3/tests/test_manifest.py
+-rw-r--r--   0 diane     (1000) diane     (1000)    12358 2023-05-04 18:43:03.000000 mex_gene_archive-0.2.3/tests/test_starsolo.py
```

### Comparing `mex_gene_archive-0.2.2/.github/workflows/ci-test.yml` & `mex_gene_archive-0.2.3/.github/workflows/ci-test.yml`

 * *Files identical despite different names*

### Comparing `mex_gene_archive-0.2.2/Changelog.rst` & `mex_gene_archive-0.2.3/Changelog.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 
 Changelog
 =========
 
+Release 0.2.3
+-------------
+
+The code to generate the md5sums for the merged matrix file didn't
+call .hexdigest() so the md5sum for the merged sparse matrix file was
+the string rerepresentation of the python md5 object.
+
+
 Release 0.2.2
 -------------
 
 Add function to write an AnnData archive to a mex_gene_archive file.
 
 def write_anndata_as_mex_archive(
     adata,
```

### Comparing `mex_gene_archive-0.2.2/LICENSE.txt` & `mex_gene_archive-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mex_gene_archive-0.2.2/PKG-INFO` & `mex_gene_archive-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mex_gene_archive
-Version: 0.2.2
+Version: 0.2.3
 Summary: matrix market tar archive access utilities
 Home-page: https://github.com/detrout/mex_gene_archive
 Author: Diane Trout
 Author-email: diane@caltech.edu
 License: BSD-3
 Project-URL: Source, https://github.com/detrout/mex_gene_archive
 Project-URL: Tracker, https://github.com/detrout/mex_gene_archive/issues
```

### Comparing `mex_gene_archive-0.2.2/README.rst` & `mex_gene_archive-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `mex_gene_archive-0.2.2/mex_gene_archive/anndata.py` & `mex_gene_archive-0.2.3/mex_gene_archive/anndata.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     )
     if destination is not None:
         tar_name = Path(destination) / tar_name
 
     md5s = [
         (barcode_filename, compute_byte_md5sum(generate_barcode_bytes(adata))),
         (features_filename, compute_byte_md5sum(generate_features_bytes(adata))),
-        (matrix_filename, hashlib.md5(get_matrix_buffer(adata))),
+        (matrix_filename, hashlib.md5(get_matrix_buffer(adata)).hexdigest()),
     ]
     manifest = create_metadata(adata.uns, md5s)
 
     manifest_buffer = BytesIO(
         write_manifest(StringIO(), manifest).getvalue().encode("ascii")
     )
```

### Comparing `mex_gene_archive-0.2.2/mex_gene_archive/filter.py` & `mex_gene_archive-0.2.3/mex_gene_archive/filter.py`

 * *Files identical despite different names*

### Comparing `mex_gene_archive-0.2.2/mex_gene_archive/manifest.py` & `mex_gene_archive-0.2.3/mex_gene_archive/manifest.py`

 * *Files identical despite different names*

### Comparing `mex_gene_archive-0.2.2/mex_gene_archive/reader.py` & `mex_gene_archive-0.2.3/mex_gene_archive/reader.py`

 * *Files identical despite different names*

### Comparing `mex_gene_archive-0.2.2/mex_gene_archive/starsolo.py` & `mex_gene_archive-0.2.3/mex_gene_archive/starsolo.py`

 * *Files identical despite different names*

### Comparing `mex_gene_archive-0.2.2/mex_gene_archive.egg-info/PKG-INFO` & `mex_gene_archive-0.2.3/mex_gene_archive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mex-gene-archive
-Version: 0.2.2
+Version: 0.2.3
 Summary: matrix market tar archive access utilities
 Home-page: https://github.com/detrout/mex_gene_archive
 Author: Diane Trout
 Author-email: diane@caltech.edu
 License: BSD-3
 Project-URL: Source, https://github.com/detrout/mex_gene_archive
 Project-URL: Tracker, https://github.com/detrout/mex_gene_archive/issues
```

### Comparing `mex_gene_archive-0.2.2/mex_gene_archive.egg-info/SOURCES.txt` & `mex_gene_archive-0.2.3/mex_gene_archive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mex_gene_archive-0.2.2/setup.cfg` & `mex_gene_archive-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `mex_gene_archive-0.2.2/tests/stage_data.py` & `mex_gene_archive-0.2.3/tests/stage_data.py`

 * *Files identical despite different names*

### Comparing `mex_gene_archive-0.2.2/tests/test_anndata.py` & `mex_gene_archive-0.2.3/tests/test_anndata.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from anndata import AnnData
-from io import BytesIO
+from io import BytesIO, TextIOWrapper
 import numpy
 from pathlib import Path
 import pandas
 from scipy.io import mmread
+import tarfile
 import tempfile
 from unittest import TestCase
 
 from mex_gene_archive.anndata import (
     generate_barcode_bytes,
     generate_features_bytes,
     get_matrix_buffer,
     write_anndata_as_mex_archive,
 )
 from mex_gene_archive.manifest import ConfigError
 from mex_gene_archive.reader import read_mex_archive_as_anndata
+from mex_gene_archive.starsolo import MULTIREAD_NAME
 
 from .stage_data import (
     generate_barcodes,
     generate_count_matrix,
     generate_features,
 )
 
@@ -72,36 +74,65 @@
 
     def test_write_and_read(self):
         adata = make_adata()
 
         quantification = "Gene"
         multiread = "Unique"
         matrix = "raw"
+
+        expected_manifest = {
+            "experiment_accession": "test_experiment",
+            "description": "sample data generated for testing",
+            "library_accession": "test_library",
+        }
+
         with tempfile.TemporaryDirectory() as tmp_dir:
             tmp_dir = Path(tmp_dir)
             self.assertRaises(
                 ConfigError,
                 write_anndata_as_mex_archive,
                 adata,
                 quantification,
                 multiread,
                 matrix,
                 destination=tmp_dir,
             )
 
-            adata.uns["experiment_accession"] = "test_experiment"
-            adata.uns["description"] = "sample data generated for testing"
-            adata.uns["library_accession"] = "test_library"
+            for key in expected_manifest:
+                adata.uns[key] = expected_manifest[key]
 
             write_anndata_as_mex_archive(
                 adata, quantification, multiread, matrix, destination=tmp_dir
             )
             filename = tmp_dir / "{}_{}_{}.tar.gz".format(
                 quantification, multiread, matrix
             )
             self.assertTrue(filename.exists())
 
             read = read_mex_archive_as_anndata(filename)
 
+            with tarfile.open(name=filename, mode="r:*") as archive:
+                for member in archive:
+                    member_path = Path(member.name)
+                    text_stream = TextIOWrapper(archive.extractfile(member), encoding="utf-8")
+                    if member_path.name == "manifest.tsv":
+                        metadata = pandas.read_csv(
+                            text_stream, sep="\t", index_col="name")
+                        break
+
         self.assertTrue(numpy.all(adata.var_names == read.var_names))
         self.assertTrue(numpy.all(adata.obs_names == read.obs_names))
         self.assertTrue(numpy.all(adata.X == read.X))
+
+        for key in expected_manifest:
+            self.assertEqual(adata.uns[key], expected_manifest[key])
+
+        base = "{}/{}/".format(
+            quantification, matrix
+        )
+        expected_md5s = {
+            base + "barcodes.tsv": "md5sum:5c34cff881503b2434f6119bc223f3f6",
+            base + "features.tsv": "md5sum:6f186211712a1568b0a58e44c9696ff3",
+            base + MULTIREAD_NAME[multiread]: "md5sum:6dd76439cba2587e74ff7ba0b814fb6c",
+        }
+        for name in expected_md5s:
+            self.assertEqual(metadata.loc[name, "value"], expected_md5s[name])
```

### Comparing `mex_gene_archive-0.2.2/tests/test_filter.py` & `mex_gene_archive-0.2.3/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `mex_gene_archive-0.2.2/tests/test_manifest.py` & `mex_gene_archive-0.2.3/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `mex_gene_archive-0.2.2/tests/test_starsolo.py` & `mex_gene_archive-0.2.3/tests/test_starsolo.py`

 * *Files identical despite different names*

