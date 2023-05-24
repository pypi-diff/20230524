# Comparing `tmp/PyFixedReps-andnp-4.0.0.tar.gz` & `tmp/PyFixedReps-andnp-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFixedReps-andnp-4.0.0.tar", last modified: Tue May 23 03:16:48 2023, max compression
+gzip compressed data, was "PyFixedReps-andnp-4.0.1.tar", last modified: Wed May 24 03:45:34 2023, max compression
```

## Comparing `PyFixedReps-andnp-4.0.0.tar` & `PyFixedReps-andnp-4.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      181 2023-05-23 03:16:13.550581 PyFixedReps-andnp-4.0.0/PyFixedReps/BaseRepresentation.py
--rw-r--r--   0        0        0      751 2023-05-23 03:16:13.550581 PyFixedReps-andnp-4.0.0/PyFixedReps/RBF.py
--rw-r--r--   0        0        0     2856 2023-05-23 03:16:13.550581 PyFixedReps-andnp-4.0.0/PyFixedReps/TileCoder.py
--rw-r--r--   0        0        0      220 2023-05-23 03:16:13.550581 PyFixedReps-andnp-4.0.0/PyFixedReps/__init__.py
--rw-r--r--   0        0        0      477 2023-05-23 03:16:13.550581 PyFixedReps-andnp-4.0.0/PyFixedReps/_jit.py
--rw-r--r--   0        0        0     2931 2023-05-23 03:16:46.383080 PyFixedReps-andnp-4.0.0/README.md
--rw-r--r--   0        0        0      942 2023-05-23 03:16:46.395080 PyFixedReps-andnp-4.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-23 03:16:13.550581 PyFixedReps-andnp-4.0.0/tests/__init__.py
--rw-r--r--   0        0        0      437 2023-05-23 03:16:13.550581 PyFixedReps-andnp-4.0.0/tests/test_RBF.py
--rw-r--r--   0        0        0     3907 2023-05-23 03:16:13.550581 PyFixedReps-andnp-4.0.0/tests/test_TileCoder.py
--rw-r--r--   0        0        0     3126 1970-01-01 00:00:00.000000 PyFixedReps-andnp-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0      181 2023-05-24 03:44:52.497887 PyFixedReps-andnp-4.0.1/PyFixedReps/BaseRepresentation.py
+-rw-r--r--   0        0        0      751 2023-05-24 03:44:52.497887 PyFixedReps-andnp-4.0.1/PyFixedReps/RBF.py
+-rw-r--r--   0        0        0     2869 2023-05-24 03:44:52.497887 PyFixedReps-andnp-4.0.1/PyFixedReps/TileCoder.py
+-rw-r--r--   0        0        0      220 2023-05-24 03:44:52.497887 PyFixedReps-andnp-4.0.1/PyFixedReps/__init__.py
+-rw-r--r--   0        0        0      477 2023-05-24 03:44:52.497887 PyFixedReps-andnp-4.0.1/PyFixedReps/_jit.py
+-rw-r--r--   0        0        0     2931 2023-05-24 03:45:32.829988 PyFixedReps-andnp-4.0.1/README.md
+-rw-r--r--   0        0        0      945 2023-05-24 03:45:32.833988 PyFixedReps-andnp-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 03:44:52.501887 PyFixedReps-andnp-4.0.1/tests/__init__.py
+-rw-r--r--   0        0        0      437 2023-05-24 03:44:52.501887 PyFixedReps-andnp-4.0.1/tests/test_RBF.py
+-rw-r--r--   0        0        0     3907 2023-05-24 03:44:52.501887 PyFixedReps-andnp-4.0.1/tests/test_TileCoder.py
+-rw-r--r--   0        0        0     3126 1970-01-01 00:00:00.000000 PyFixedReps-andnp-4.0.1/PKG-INFO
```

### Comparing `PyFixedReps-andnp-4.0.0/PyFixedReps/RBF.py` & `PyFixedReps-andnp-4.0.1/PyFixedReps/RBF.py`

 * *Files identical despite different names*

### Comparing `PyFixedReps-andnp-4.0.0/PyFixedReps/TileCoder.py` & `PyFixedReps-andnp-4.0.1/PyFixedReps/TileCoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import numpy.typing as npt
 from dataclasses import dataclass
-from tile_coder import get_tc_indices
-from typing import Iterable, List, Optional, Sequence, Tuple
+from tile_coder_rs import get_tc_indices
+from typing import Any, Iterable, List, Optional, Sequence, Tuple
 from PyFixedReps.BaseRepresentation import Array, BaseRepresentation
 
 Range = Tuple[float, float]
 RandomState = np.random.RandomState
 
 @dataclass
 class TileCoderConfig:
@@ -25,15 +25,15 @@
         self._c = c = config
 
         ranges: Sequence[Range | None] = [None] * c.dims
         if c.input_ranges is not None:
             assert len(c.input_ranges) == c.dims
             ranges = c.input_ranges
 
-        self._tiles = _normalize_tiles(c.tiles, c.dims)
+        self._tiles: Any = _normalize_tiles(c.tiles, c.dims)
         self._input_ranges = _normalize_scalars(ranges)
         self._tiling_offsets: Array = np.array([ self._build_offset(ntl) for ntl in range(c.tilings) ])
         self._total_tiles = int(c.tilings * self._tiles.prod())
 
     # construct tiling offsets
     # defaults to evenly spaced tilings
     def _build_offset(self, n: int):
```

### Comparing `PyFixedReps-andnp-4.0.0/README.md` & `PyFixedReps-andnp-4.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # PyFixedReps
 Short for: Python Fixed Representations.
 This is a collection of unit tested implementations of common fixed representations commonly used with linear (in features) RL systems.
 
 ## Installing
 Can be installed using `pip` by including this in your `requirements.txt`:
 ```
-pip install PyFixedReps-andnp==4.0.0
+pip install PyFixedReps-andnp==4.0.1
 ```
 I highly recommend specifying the version number when installing in order to ensure reproducibility of experiments.
 This library is fairly stable, so does not change often and there is little risk of missing an important change.
 
 ## Tile-coder
 ```python
 from PyFixedReps import TileCoder
```

### Comparing `PyFixedReps-andnp-4.0.0/pyproject.toml` & `PyFixedReps-andnp-4.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "4.0.0"
+version = "4.0.1"
 tag_format = "$version"
 version_files = [
     "pyproject.toml",
     "README.md",
 ]
 
 [tool.pdm]
@@ -24,23 +24,23 @@
 ]
 
 [tool.mypy]
 mypy_path = "typings"
 
 [project]
 name = "PyFixedReps-andnp"
-version = "4.0.0"
+version = "4.0.1"
 description = ""
 authors = [
     { name = "Andy Patterson", email = "andnpatterson@gmail.com" },
 ]
 dependencies = [
     "numpy>=1.23.5",
     "numba>=0.56.4",
-    "tile-coder==0.1.0",
+    "tile-coder-rs==0.1.0",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `PyFixedReps-andnp-4.0.0/tests/test_TileCoder.py` & `PyFixedReps-andnp-4.0.1/tests/test_TileCoder.py`

 * *Files identical despite different names*

### Comparing `PyFixedReps-andnp-4.0.0/PKG-INFO` & `PyFixedReps-andnp-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: PyFixedReps-andnp
-Version: 4.0.0
+Version: 4.0.1
 License: MIT
 Author-email: Andy Patterson <andnpatterson@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # PyFixedReps
 Short for: Python Fixed Representations.
 This is a collection of unit tested implementations of common fixed representations commonly used with linear (in features) RL systems.
 
 ## Installing
 Can be installed using `pip` by including this in your `requirements.txt`:
 ```
-pip install PyFixedReps-andnp==4.0.0
+pip install PyFixedReps-andnp==4.0.1
 ```
 I highly recommend specifying the version number when installing in order to ensure reproducibility of experiments.
 This library is fairly stable, so does not change often and there is little risk of missing an important change.
 
 ## Tile-coder
 ```python
 from PyFixedReps import TileCoder
```

