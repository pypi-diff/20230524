# Comparing `tmp/range_compression-0.2.1.tar.gz` & `tmp/range_compression-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "range_compression-0.2.1.tar", max compression
+gzip compressed data, was "range_compression-0.2.2.tar", max compression
```

## Comparing `range_compression-0.2.1.tar` & `range_compression-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      488 2023-05-19 02:23:35.360031 range_compression-0.2.1/README.md
--rw-r--r--   0        0        0      622 2023-05-24 08:52:17.551216 range_compression-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       86 2023-05-19 02:26:56.109857 range_compression-0.2.1/range_compression/__init__.py
--rw-r--r--   0        0        0     6751 2023-05-24 08:52:09.114507 range_compression-0.2.1/range_compression/range_compression.py
--rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 range_compression-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      488 2023-05-19 02:23:35.360031 range_compression-0.2.2/README.md
+-rw-r--r--   0        0        0      622 2023-05-24 08:58:16.319690 range_compression-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       90 2023-05-24 08:58:09.212988 range_compression-0.2.2/range_compression/__init__.py
+-rw-r--r--   0        0        0     7216 2023-05-24 08:58:01.719617 range_compression-0.2.2/range_compression/range_compression.py
+-rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 range_compression-0.2.2/PKG-INFO
```

### Comparing `range_compression-0.2.1/pyproject.toml` & `range_compression-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "range-compression"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["myuan <zhengmy@ion.ac.cn>"]
 license = "LGPL"
 readme = "README.md"
 packages = [{include = "range_compression"}]
 repository = "https://github.com/myuanz/matrix-range-compression"
```

### Comparing `range_compression-0.2.1/range_compression/range_compression.py` & `range_compression-0.2.2/range_compression/range_compression.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,16 +85,27 @@
         return base
 
     def find_index(
         self, 
         X: np.ndarray, Y: np.ndarray, 
         binary_search=False
     ):
-        return find_index(self, X, Y, binary_search=binary_search)
-
+        if self.encodings.shape[1] == 4:
+            import warnings
+            warnings.warn(f'`row_indexes` has 4 columns.')
+        if not isinstance(X, np.ndarray):
+            X = np.array(X)
+        if not isinstance(Y, np.ndarray):
+            Y = np.array(Y)
+
+        args = (self.row_indexes, self.encodings, X, Y)
+        if binary_search:
+            return _find_index_binary(*args)
+        else:
+            return _find_index(*args)
 
 @nb.njit
 def _mask_encode(mask):
     n_rows, n_cols = mask.shape
 
     encodings = []
     row_indexes = []
@@ -221,7 +232,10 @@
         Y = np.array(Y)
 
     args = (mask_encoding_result.row_indexes, mask_encoding_result.encodings, X, Y)
     if binary_search:
         return _find_index_binary(*args)
     else:
         return _find_index(*args)
+
+rcm_load = RangeCompressedMask.load
+rcm_find_index = RangeCompressedMask.find_index
```

### Comparing `range_compression-0.2.1/PKG-INFO` & `range_compression-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: range-compression
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Home-page: https://github.com/myuanz/matrix-range-compression
 License: LGPL
 Author: myuan
 Author-email: zhengmy@ion.ac.cn
 Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
```

