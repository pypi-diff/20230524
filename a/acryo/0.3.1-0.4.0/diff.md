# Comparing `tmp/acryo-0.3.1.tar.gz` & `tmp/acryo-0.4.0.tar.gz`

## Comparing `acryo-0.3.1.tar` & `acryo-0.4.0.tar`

### file list

```diff
@@ -1,46 +1,51 @@
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/__init__.py
--rw-r--r--   0        0        0    11824 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/_correlation.py
--rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/_dask.py
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/_reader.py
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/_rotation.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/_typed_scipy.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/_types.py
--rw-r--r--   0        0        0    11797 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/_utils.py
--rw-r--r--   0        0        0    20882 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/simulator.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/alignment/__init__.py
--rw-r--r--   0        0        0    28969 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/alignment/_base.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/alignment/_bound.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/alignment/_concrete.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/classification/__init__.py
--rw-r--r--   0        0        0    18578 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/classification/_dask_pca.py
--rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/classification/pca.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/loader/__init__.py
--rw-r--r--   0        0        0    37276 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/loader/_base.py
--rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/loader/_batch.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/loader/_cache.py
--rw-r--r--   0        0        0    18998 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/loader/_group.py
--rw-r--r--   0        0        0     9586 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/loader/_loader.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/loader/_misc.py
--rw-r--r--   0        0        0    10259 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/loader/_mock.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/molecules/__init__.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/molecules/_cut.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/molecules/_group.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/molecules/_rotation.py
--rw-r--r--   0        0        0    33963 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/molecules/core.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/pick/__init__.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/pick/_base.py
--rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/pick/_concrete.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/pipe/__init__.py
--rw-r--r--   0        0        0    12912 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/pipe/_classes.py
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/pipe/_curry.py
--rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/pipe/_imread.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/pipe/_masking.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/pipe/_transform.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/testing/__init__.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/testing/_templates.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 acryo-0.3.1/acryo/testing/core.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 acryo-0.3.1/.gitignore
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 acryo-0.3.1/LICENSE
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 acryo-0.3.1/README.md
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 acryo-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 acryo-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/__init__.py
+-rw-r--r--   0        0        0     6201 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/_dask.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/_reader.py
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/_rotation.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/_typed_scipy.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/_types.py
+-rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/_utils.py
+-rw-r--r--   0        0        0    20882 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/simulator.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/alignment/__init__.py
+-rw-r--r--   0        0        0    32102 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/alignment/_base.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/alignment/_bound.py
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/alignment/_concrete.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/backend/__init__.py
+-rw-r--r--   0        0        0    17080 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/backend/_api.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/backend/_bandpass.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/backend/_missing_wedge.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/backend/_pcc.py
+-rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/backend/_zncc.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/classification/__init__.py
+-rw-r--r--   0        0        0    18578 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/classification/_dask_pca.py
+-rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/classification/pca.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/loader/__init__.py
+-rw-r--r--   0        0        0    37929 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/loader/_base.py
+-rw-r--r--   0        0        0     8085 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/loader/_batch.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/loader/_cache.py
+-rw-r--r--   0        0        0    19585 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/loader/_group.py
+-rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/loader/_loader.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/loader/_misc.py
+-rw-r--r--   0        0        0    10507 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/loader/_mock.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/molecules/__init__.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/molecules/_cut.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/molecules/_group.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/molecules/_rotation.py
+-rw-r--r--   0        0        0    33963 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/molecules/core.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/pick/__init__.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/pick/_base.py
+-rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/pick/_concrete.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/pipe/__init__.py
+-rw-r--r--   0        0        0    12912 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/pipe/_classes.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/pipe/_curry.py
+-rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/pipe/_imread.py
+-rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/pipe/_masking.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/pipe/_transform.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/testing/__init__.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/testing/_templates.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/testing/core.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 acryo-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 acryo-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 acryo-0.4.0/README.md
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 acryo-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 acryo-0.4.0/PKG-INFO
```

### Comparing `acryo-0.3.1/acryo/_dask.py` & `acryo-0.4.0/acryo/_dask.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,19 @@
         *args: _P.args,
         **kwargs: _P.kwargs,
     ) -> DaskTaskPool[[da.Array], _R]:
         pool = DaskTaskPool.from_func(func)
         [pool.add_task(s, *args, **kwargs) for s in self]
         return pool
 
+    def map_blocks(self, func, *args, **kwargs):
+        return DaskArrayList(
+            [a.map_blocks(func, *args, **kwargs) for a in self._arrays]
+        )
+
     def enumerate(self) -> Iterator[tuple[int, da.Array]]:
         return enumerate(self)
 
 
 _R1 = TypeVar("_R1")
 _R2 = TypeVar("_R2")
```

### Comparing `acryo-0.3.1/acryo/_reader.py` & `acryo-0.4.0/acryo/_reader.py`

 * *Files identical despite different names*

### Comparing `acryo-0.3.1/acryo/_rotation.py` & `acryo-0.4.0/acryo/_rotation.py`

 * *Files identical despite different names*

### Comparing `acryo-0.3.1/acryo/_typed_scipy.py` & `acryo-0.4.0/acryo/_typed_scipy.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,25 +5,33 @@
 from numpy.typing import NDArray
 
 # scipy is not well typed. Make patches here.
 if TYPE_CHECKING:
     Mode = Literal["constant", "nearest", "mirror", "wrap", "reflect"]
 
     def fftn(
-        img: NDArray[np.float32] | NDArray[np.complex64], axes=None
+        img: NDArray[np.float32] | NDArray[np.complex64], s=None, axes=None
     ) -> NDArray[np.complex64]:
         ...
 
-    def ifftn(img: NDArray[np.complex64], axes=None) -> NDArray[np.complex64]:
+    def ifftn(img: NDArray[np.complex64], s=None, axes=None) -> NDArray[np.complex64]:
         ...
 
-    def rfftn(img: NDArray[np.float32]) -> NDArray[np.complex64]:
+    def rfftn(img: NDArray[np.float32], s=None, axes=None) -> NDArray[np.complex64]:
         ...
 
-    def irfftn(img: NDArray[np.complex64]) -> NDArray[np.float32]:
+    def irfftn(img: NDArray[np.complex64], s=None, axes=None) -> NDArray[np.float32]:
+        ...
+
+    def convolve(
+        in1: NDArray[np.float32],
+        in2: NDArray[np.float32],
+        mode: Literal["full", "valid", "same"] = "full",
+        method: Literal["auto", "fft", "direct"] = "auto",
+    ) -> NDArray[np.float32]:
         ...
 
     def spline_filter(
         input: NDArray[np.float32],
         order: int = 3,
         output: Any = np.float64,
         mode: Mode = "mirror",
@@ -39,31 +47,45 @@
         order: int = 3,
         mode: Mode = "constant",
         cval: float = 0.0,
         prefilter: bool = True,
     ) -> NDArray[np.float32]:
         ...
 
+    def shift(
+        input: NDArray[np.float32],
+        shift: tuple[float, ...] | NDArray[np.float32],
+        output: NDArray[np.float32] | None = None,
+        order: int = 3,
+        mode: Mode = "constant",
+        cval: float = 0.0,
+        prefilter: bool = True,
+    ) -> NDArray[np.float32]:
+        ...
+
     def map_coordinates(
         input: NDArray[np.float32],
         coordinates: NDArray[np.float32],
         output: NDArray[np.float32] | None = None,
         order: int = 3,
         mode: Mode = "constant",
         cval: float = 0.0,
         prefilter: bool = True,
     ) -> NDArray[np.float32]:
         ...
 
 else:
     from scipy.fft import rfftn, irfftn, fftn, ifftn
-    from scipy.ndimage import spline_filter, affine_transform, map_coordinates
+    from scipy.ndimage import spline_filter, affine_transform, map_coordinates, shift
+    from scipy.signal import convolve
 
 __all__ = [
     "fftn",
     "ifftn",
     "rfftn",
     "irfftn",
     "spline_filter",
     "affine_transform",
+    "shift",
     "map_coordinates",
+    "convolve",
 ]
```

### Comparing `acryo-0.3.1/acryo/_utils.py` & `acryo-0.4.0/acryo/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import warnings
 from typing import Callable, Sequence, TYPE_CHECKING, TypeVar
 from functools import lru_cache, reduce, wraps
 
 import numpy as np
 from numpy.typing import NDArray
 from dask import array as da
-from dask.delayed import delayed
 from scipy import ndimage as ndi
 from scipy.spatial.transform import Rotation
 from acryo._typed_scipy import fftn, rfftn, irfftn
 
 if TYPE_CHECKING:
     from acryo._types import degree
 
@@ -74,15 +73,15 @@
             [0.0, 0.0, 0.0, 1.0],
         ],
         dtype=np.float32,
     )
 
     matrices: list[np.ndarray] = []
     for rot in rotators:
-        e_ = np.eye(4)
+        e_ = np.eye(4, dtype=np.float32)
         e_[:3, :3] = rot.as_matrix()
         matrices.append(translation_0 @ e_ @ translation_1)
     return matrices
 
 
 def fourier_shell_correlation(
     img0: np.ndarray,
@@ -131,27 +130,27 @@
     pw0 = f0.real**2 + f0.imag**2
     pw1 = f1.real**2 + f1.imag**2
     out = radial_sum(cov) / np.sqrt(radial_sum(pw0) * radial_sum(pw1))
     freq = (np.arange(len(out)) + 0.5) * dfreq
     return freq, out
 
 
-def bin_image(img: np.ndarray | da.Array, binsize: int) -> np.ndarray:
+def bin_image(img: np.ndarray | da.Array, binsize: int):
     """Bin an image."""
     _slices: list[slice] = []
     _shapes: list[int] = []
     for s in img.shape:
         npix, res = divmod(s, binsize)
         _slices.append(slice(None, s - res))
         _shapes.extend([npix, binsize])
     slices = tuple(_slices)
     shapes = tuple(_shapes)
-    img_reshaped = np.reshape(img[slices], shapes)
+    img_reshaped = img[slices].reshape(shapes)
     axis = tuple(i * 2 + 1 for i in range(img.ndim))
-    return np.sum(img_reshaped, axis=axis)
+    return img_reshaped.sum(axis=axis)
 
 
 def prepare_affine(
     img: da.Array,
     center: Sequence[float],
     output_shape: Sequence[int],
     rot: Rotation,
@@ -208,31 +207,14 @@
         input = da.pad(img0, pads, mode="mean")
     else:
         input = img0
     mtx = compose_matrices(new_center, [rot], output_center=output_center)[0]
     return input, mtx
 
 
-_delayed_affine_transform = delayed(ndi.affine_transform)
-
-
-def delayed_affine(
-    input: np.ndarray,
-    matrix: np.ndarray,
-    order: int = 3,
-    mode: str = "constant",
-    cval: float = 0.0,
-    prefilter: bool = True,
-) -> da.Array:
-    out = _delayed_affine_transform(
-        input, matrix, order=order, mode=mode, cval=cval, prefilter=prefilter
-    )
-    return da.from_delayed(out, shape=input.shape, dtype=input.dtype)  # type: ignore
-
-
 def missing_wedge_mask(
     rotator: Rotation,
     tilt_range: tuple[degree, degree],
     shape: tuple[int, int, int],
 ) -> NDArray[np.float32]:
     """
     Create a binary mask that covers tomographical missing wedge.
@@ -285,37 +267,38 @@
     for ind, s in zip(inds, shape):
         # Note that the shifts in indices must resemble the shifts in fftshift.
         ind -= np.ceil(s / 2)
     return np.fft.fftshift(np.stack(list(inds), axis=-1), axes=(0, 1, 2))
 
 
 # lowpass filter
-# Modified from skimage.filters._fft_based
+
+
 def lowpass_filter_ft(
     img: NDArray[np.float32], cutoff: float, order: int = 2
 ) -> NDArray[np.complex64]:
     """Apply a low-pass filter and return the result in Fourier space."""
     if cutoff >= 0.5 * np.sqrt(img.ndim) or cutoff <= 0:
         return fftn(img)
-    weight = _get_ND_butterworth_filter(
+    weight = nd_butterworth_weight(
         img.shape,
         cutoff,
         order,
         real=False,
     )
     return weight * fftn(img)
 
 
 def lowpass_filter(
     img: NDArray[np.float32], cutoff: float, order: int = 2
 ) -> NDArray[np.float32]:
     """Apply a low-pass filter and return the result in real space."""
     if cutoff >= 0.5 * np.sqrt(img.ndim) or cutoff <= 0:
         return img
-    weight = _get_ND_butterworth_filter(
+    weight = nd_butterworth_weight(
         img.shape,
         cutoff,
         order,
         real=True,
     )
     out = irfftn(weight * rfftn(img))
     return out.real
@@ -323,41 +306,42 @@
 
 def highpass_filter_ft(
     img: NDArray[np.float32], cutoff: float, order: int = 2
 ) -> NDArray[np.complex64]:
     """Apply a high-pass filter and return the result in Fourier space."""
     if cutoff >= 0.5 * np.sqrt(img.ndim) or cutoff <= 0:
         return np.zeros_like(img)
-    weight = 1 - _get_ND_butterworth_filter(
+    weight = 1 - nd_butterworth_weight(
         img.shape,
         cutoff,
         order,
         real=False,
     )
     return weight * fftn(img)
 
 
 def highpass_filter(
     img: NDArray[np.float32], cutoff: float, order: int = 2
 ) -> NDArray[np.float32]:
     """Apply a high-pass filter and return the result in real space."""
     if cutoff >= 0.5 * np.sqrt(img.ndim) or cutoff <= 0:
         return np.zeros_like(img)
-    weight = 1 - _get_ND_butterworth_filter(
+    weight = 1 - nd_butterworth_weight(
         img.shape,
         cutoff,
         order,
         real=True,
     )
     out = irfftn(weight * rfftn(img))
     return out.real
 
 
+# Modified from skimage.filters._fft_based
 @lru_cache(maxsize=4)
-def _get_ND_butterworth_filter(
+def nd_butterworth_weight(
     shape: tuple[int, ...],
     cutoff: float,
     order: int,
     real: bool,
 ) -> NDArray[np.float32]:
     ranges = []
     for d in shape:
```

### Comparing `acryo-0.3.1/acryo/simulator.py` & `acryo-0.4.0/acryo/simulator.py`

 * *Files identical despite different names*

### Comparing `acryo-0.3.1/acryo/alignment/_base.py` & `acryo-0.4.0/acryo/alignment/_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,46 +4,39 @@
 from abc import ABC, abstractmethod
 from functools import lru_cache
 from typing import (
     Callable,
     Iterable,
     NamedTuple,
     Sequence,
-    TYPE_CHECKING,
     Union,
 )
 from typing_extensions import Self
-import warnings
 
 import numpy as np
 from numpy.typing import NDArray
 from scipy.spatial.transform import Rotation
 
 from acryo._rotation import normalize_rotations
 from acryo._types import Ranges, subpixel, degree
-from acryo._utils import (
-    compose_matrices,
-    missing_wedge_mask,
-    lowpass_filter_ft,
-)
-from acryo._typed_scipy import ifftn, spline_filter, affine_transform, map_coordinates
+from acryo._utils import compose_matrices
 from acryo._dask import DaskTaskPool, compute
-from ._bound import ParametrizedModel
-
-if TYPE_CHECKING:
-    pass
+from acryo.backend import Backend, AnyArray, NUMPY_BACKEND
+from acryo.alignment._bound import ParametrizedModel
 
 
 TemplateType = Union[NDArray[np.float32], Sequence[NDArray[np.float32]]]
 MaskType = Union[
     NDArray[np.float32],
     Callable[[NDArray[np.float32]], NDArray[np.float32]],
     None,
 ]
 AlignmentFactory = Callable[[TemplateType, MaskType], "BaseAlignmentModel"]
+_Template = AnyArray[np.complex64]
+_Mask = AnyArray[np.float32]
 
 
 class AlignmentResult(NamedTuple):
     """The optimal alignment result."""
 
     label: int
     shift: NDArray[np.float32]
@@ -55,14 +48,32 @@
         rotator = Rotation.from_quat(self.quat)
         shift_matrix = np.eye(4, dtype=np.float32)
         shift_matrix[:3, 3] = self.shift
         rot_matrix = compose_matrices(np.array(shape) / 2 - 0.5, [rotator])[0]
         return shift_matrix @ rot_matrix
 
 
+class TemplateMaskCache:
+    _dict: dict[Backend, tuple[_Template, _Mask]]
+
+    def __init__(self):
+        self._dict = {}
+
+    def get(self, backend: Backend) -> tuple[_Template, _Mask] | None:
+        if out := self._dict.get(backend):
+            return out
+        if val := next(iter(self._dict.values()), None):
+            self._dict[backend] = out = backend.asarray(val[0]), backend.asarray(val[1])
+            return out
+        return None
+
+    def set(self, backend: Backend, template: _Template, mask: _Mask):
+        self._dict[backend] = template, mask
+
+
 class BaseAlignmentModel(ABC):
     """
     The base class to implement alignment method.
 
     This class supports subvolume masking, pre-transformation of subvolumes and
     template, optimization of spatial transformation.
 
@@ -77,17 +88,17 @@
         +-----+------+
               |
               v
          (alignment)
 
     Abstract Methods
     ----------------
-    >>> def optimize(self, template, reference, max_shifts, quaternion):
+    >>> def optimize(self, template, reference, max_shifts, quaternion, pos, backend):
     >>>     ...
-    >>> def pre_transform(self, image):
+    >>> def pre_transform(self, image, backend):
     >>>     ...
 
     """
 
     _DUMMY_POS = np.array([0.0, 0.0, 0.0], dtype=np.float32)
     _DUMMY_QUAT = np.array([0.0, 0.0, 0.0, 1.0], dtype=np.float32)
 
@@ -126,15 +137,16 @@
                     "Shape mismatch in between template image "
                     f"{self._template.shape[-self._ndim :]} and mask image {mask.shape})."
                 )
             if mask.dtype not in (np.float32, np.bool_):
                 mask = mask.astype(np.float32)
             self._mask = mask
 
-        self._template_input, self._mask_input = self._get_template_and_mask_input()
+        self._template_mask_cache = TemplateMaskCache()
+        self._get_template_and_mask_input(Backend())  # cache the template and mask
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(shape={self._template.shape})"
 
     @property
     def template(self) -> NDArray[np.float32]:
         """The template image."""
@@ -162,19 +174,20 @@
     ):
         """Create a BaseAlignmentModel instance with parameters."""
         return ParametrizedModel(cls, **params)
 
     @abstractmethod
     def _optimize(
         self,
-        subvolume: NDArray[np.complex64],
-        template: NDArray[np.complex64],
+        subvolume: AnyArray[np.complex64],
+        template: _Template,
         max_shifts: tuple[float, ...],
         quaternion: NDArray[np.float32],
         pos: NDArray[np.float32],
+        backend: Backend,
     ) -> tuple[NDArray[np.float32], NDArray[np.float32], float]:
         """
         Optimization of shift and rotation of subvolume.
 
         This method uses a subvolume and a template image to find the optimal
         shift/rotation to fit subvolume to template under the restriction of
         maximum shifts.
@@ -199,33 +212,39 @@
             - rotation ... Rotation in quaternion. If this cannot be optimized by the
               implemented algorithm, this value can be ``[0., 0., 0., 0.]``.
             - score ... This value Must be a float and larger value should represent
               better results.
         """
 
     @abstractmethod
-    def pre_transform(self, image: NDArray[np.float32]) -> NDArray[np.complex64]:
+    def pre_transform(
+        self,
+        image: AnyArray[np.float32],
+        backend: Backend,
+    ) -> AnyArray[np.complex64]:
         """Pre-transformation applied to input images (including template)."""
 
     def _landscape(
         self,
-        subvolume: NDArray[np.complex64],
-        template: NDArray[np.complex64],
+        subvolume: AnyArray[np.complex64],
+        template: _Template,
         max_shifts: tuple[float, ...],
         quaternion: NDArray[np.float32],
         pos: NDArray[np.float32],
-    ) -> NDArray[np.float32]:
+        backend: Backend,
+    ) -> AnyArray[np.float32]:
         """Return the landscape of the subvolume."""
         raise NotImplementedError(
             f"_landscape method is not implemented for {type(self).__name__}."
         )
 
     def _get_template_and_mask_input(
         self,
-    ) -> tuple[NDArray[np.complex64], NDArray[np.float32]]:
+        backend: Backend | None = None,
+    ) -> tuple[_Template, AnyArray[np.float32]]:
         """
         Returns proper template and mask images for alignment.
 
         Template dimensionality will be dispatched according to the input
         parameters. Returned template should be used in line of the
         :func:`get_alignment_function`.
 
@@ -233,29 +252,39 @@
         -------
         array
             Template image(s) and mask image(s). Its axes varies depending on the input.
 
             - single template image ... 3D
             - many template images ... 4D
         """
+        xp = backend or Backend()
+        if out := self._template_mask_cache.get(xp):
+            return out
+        mask = xp.asarray(self._mask)
         if self._n_templates > 1:
-            template_input = np.stack(
-                [self.pre_transform(tmp * self._mask) for tmp in self._template],
+            template_input = xp.stack(
+                [
+                    self.pre_transform(xp.asarray(tmp) * mask, xp)
+                    for tmp in self._template
+                ],
                 axis=0,
             )
         else:
-            template_input = self.pre_transform(self._template * self._mask)
-        return template_input, self._mask
+            template_masked = xp.asarray(self._template * self._mask)
+            template_input = self.pre_transform(template_masked, xp)
+        self._template_mask_cache.set(xp, template_input, mask)
+        return template_input, mask
 
     def align(
         self,
-        img: NDArray[np.float32],
+        img: NDArray[np.float32] | AnyArray[np.float32],
         max_shifts: tuple[float, float, float],
         quaternion: NDArray[np.float32] | None = None,
         pos: NDArray[np.float32] | None = None,
+        backend: Backend | None = None,
     ) -> AlignmentResult:
         """
         Align an image using current alignment parameters.
 
         Parameters
         ----------
         img : np.ndarray
@@ -264,41 +293,45 @@
             Maximum shifts along z, y, x axis in pixel.
 
         Returns
         -------
         AlignmentResult
             Result of alignment.
         """
+        xp = backend or Backend()
         if quaternion is None:
             _quat = self._DUMMY_QUAT
         else:
             _quat = quaternion
         if pos is None:
             _pos = self._DUMMY_POS
         else:
             _pos = pos
 
         if self._is_multiple():
             _align_fn = self._optimize_multiple
         else:
             _align_fn = self._optimize_single
+        _template, _mask = self._get_template_and_mask_input(backend=xp)
         return _align_fn(
-            img,
-            self._template_input,
-            self._mask_input,
+            xp.asarray(img),
+            _template,
+            _mask,
             max_shifts,
             _quat,
             _pos,
+            xp,
         )
 
     def fit(
         self,
         img: NDArray[np.float32],
         max_shifts: tuple[float, float, float],
         cval: float | None = None,
+        backend: Backend | None = None,
     ) -> tuple[NDArray[np.float32], AlignmentResult]:
         """
         Fit image to template based on the alignment model.
 
         Parameters
         ----------
         img : np.ndarray
@@ -309,27 +342,32 @@
             Constant value for padding.
 
         Returns
         -------
         np.ndarray, AlignmentResult
             Transformed input image and the alignment result.
         """
-        result = self.align(img, max_shifts=max_shifts, quaternion=None, pos=None)
-        mtx = result.affine_matrix(img.shape)
-        _cval = _normalize_cval(cval, img)
-        img_trans = affine_transform(img, mtx, cval=_cval)
-        return img_trans, result
+        xp = backend or Backend()
+        img_input = xp.asarray(img)
+        result = self.align(
+            img_input, max_shifts=max_shifts, quaternion=None, pos=None, backend=xp
+        )
+        mtx = result.affine_matrix(img_input.shape)
+        _cval = _normalize_cval(cval, img_input, xp)
+        img_trans = xp.affine_transform(img_input, mtx, cval=_cval)
+        return xp.asnumpy(img_trans), result
 
     def landscape(
         self,
         img: NDArray[np.float32],
         max_shifts: tuple[float, float, float],
         quaternion: NDArray[np.float32] | None = None,
         pos: NDArray[np.float32] | None = None,
         upsample: int = 1,
+        backend: Backend | None = None,
     ) -> NDArray[np.float32]:
         """
         Calculate correlation landscape of the input image.
 
         Parameters
         ----------
         img : np.ndarray
@@ -339,130 +377,141 @@
 
         Returns
         -------
         np.ndarray
             N (if single template) or N+1 (if multi-template) dimensional array of
             correlation landscape.
         """
+        xp = backend or Backend()
         if quaternion is None:
             _quat = self._DUMMY_QUAT
         else:
             _quat = quaternion
         if pos is None:
             _pos = self._DUMMY_POS
         else:
             _pos = pos
         if self._is_multiple():
             fn = self._landscape_multiple
         else:
             fn = self._landscape_single
 
+        _template, _mask = self._get_template_and_mask_input(backend=xp)
         # calculate the landscape
         lds = fn(
-            img,
-            self._template_input,
-            self._mask_input,
+            xp.asarray(img),
+            _template,
+            _mask,
             max_shifts,
             _quat,
             _pos,
+            xp,
         )
 
         if upsample > 1:
             if not self._is_multiple():
-                coords = _create_mesh_for_landscape(lds.shape, max_shifts, upsample)
-                lds_upsampled = map_coordinates(
+                coords = _build_mesh(lds.shape, max_shifts, upsample, xp)
+                lds_upsampled = xp.map_coordinates(
                     lds, coords, order=3, mode="constant", cval=0.0, prefilter=True
                 )
             else:
-                coords = _create_mesh_for_landscape(lds.shape[1:], max_shifts, upsample)
+                coords = _build_mesh(lds.shape[1:], max_shifts, upsample, xp)
                 all_lds = [
-                    map_coordinates(
+                    xp.map_coordinates(
                         l, coords, order=3, mode="constant", cval=0.0, prefilter=True
                     )
                     for l in lds
                 ]
-                lds_upsampled = np.stack(all_lds, axis=0)
-            return lds_upsampled
-        return lds
+                lds_upsampled = xp.stack(all_lds, axis=0)
+            return xp.asnumpy(lds_upsampled)
+        return xp.asnumpy(lds)
 
     def _landscape_single(
         self,
-        subvolume: NDArray[np.float32],
-        template: NDArray[np.complex64],
-        mask: NDArray[np.float32],
+        subvolume: AnyArray[np.float32],
+        template: _Template,
+        mask: AnyArray[np.float32],
         max_shifts: tuple[float, ...],
         quaternion: NDArray[np.float32],
         pos: NDArray[np.float32],
+        backend: Backend,
     ):
         return self._landscape(
-            self.pre_transform(subvolume * mask),
+            self.pre_transform(subvolume * mask, backend),
             template,
             max_shifts=max_shifts,
             quaternion=quaternion,
             pos=pos,
+            backend=backend,
         )
 
     def _landscape_multiple(
         self,
-        subvolume: NDArray[np.float32],
-        template_list: Iterable[NDArray[np.complex64]],
-        mask_list: Iterable[NDArray[np.float32]],
+        subvolume: AnyArray[np.float32],
+        template_list: _Template,
+        mask_list: Iterable[AnyArray[np.float32]],
         max_shifts: tuple[float, float, float],
         quaternion: NDArray[np.float32],
         pos: NDArray[np.float32],
-    ):
-        out: list[NDArray[np.float32]] = []
+        backend: Backend,
+    ) -> AnyArray[np.float32]:
+        out: list[AnyArray[np.float32]] = []
         for template, mask in zip(template_list, mask_list):
             lnd = self._landscape(
-                self.pre_transform(subvolume * mask),
+                self.pre_transform(subvolume * mask, backend),
                 template,
                 max_shifts=max_shifts,
                 quaternion=quaternion,
                 pos=pos,
+                backend=backend,
             )
             out.append(lnd)
-        return np.stack(out, axis=0)
+        return backend.stack(out, axis=0)
 
     def _optimize_single(
         self,
-        subvolume: NDArray[np.float32],
-        template: NDArray[np.complex64],
-        mask: NDArray[np.float32],
+        subvolume: AnyArray[np.float32],
+        template: _Template,
+        mask: AnyArray[np.float32],
         max_shifts: tuple[float, float, float],
         quaternion: NDArray[np.float32],
         pos: NDArray[np.float32],
+        backend: Backend,
     ) -> AlignmentResult:
         out = self._optimize(
-            self.pre_transform(subvolume * mask),
+            self.pre_transform(subvolume * mask, backend),
             template,
             max_shifts=max_shifts,
             quaternion=quaternion,
             pos=pos,
+            backend=backend,
         )
         return AlignmentResult(0, *out)
 
     def _optimize_multiple(
         self,
-        subvolume: NDArray[np.float32],
-        template_list: Iterable[NDArray[np.complex64]],
-        mask_list: Iterable[NDArray[np.float32]],
+        subvolume: AnyArray[np.float32],
+        template_list: _Template,
+        mask_list: AnyArray[np.float32],
         max_shifts: tuple[float, float, float],
         quaternion: NDArray[np.float32],
         pos: NDArray[np.float32],
+        backend: Backend,
     ) -> AlignmentResult:
         all_shifts: list[np.ndarray] = []
         all_quat: list[np.ndarray] = []
         all_score: list[float] = []
         for template, mask in zip(template_list, mask_list):
             shift, quat, score = self._optimize(
-                self.pre_transform(subvolume * mask),
+                self.pre_transform(subvolume * mask, backend),
                 template,
                 max_shifts=max_shifts,
                 quaternion=quaternion,
                 pos=pos,
+                backend=backend,
             )
             all_shifts.append(shift)
             all_quat.append(quat)
             all_score.append(score)
 
         iopt = int(np.argmax(all_score))
         return AlignmentResult(iopt, all_shifts[iopt], all_quat[iopt], all_score[iopt])
@@ -480,22 +529,14 @@
 
     @property
     def niter(self) -> int:
         """Number of templates."""
         return self._n_templates
 
 
-# deprecated
-def optimize(self: BaseAlignmentModel, *args, **kwargs):
-    warnings.warn(
-        "`optimize` is deprecated. It is now a private method.", DeprecationWarning
-    )
-    return self._optimize(*args, **kwargs)
-
-
 class RotationImplemented(BaseAlignmentModel):
     """
     An alignment model implemented with default rotation optimizer.
 
     If ``optimize`` does not support rotation optimization, this class implements
     simple parameter searching algorithm to it. Thus, ``optimize`` only has to
     optimize shift of images.
@@ -527,14 +568,15 @@
 
     def align(
         self,
         img: NDArray[np.float32],
         max_shifts: tuple[subpixel, subpixel, subpixel],
         quaternion: NDArray[np.float32] | None,
         pos: NDArray[np.float32] | None,
+        backend: Backend | None = None,
     ) -> AlignmentResult:
         """
         Align an image using current alignment parameters.
 
         Parameters
         ----------
         img : np.ndarray
@@ -543,23 +585,24 @@
             Maximum shifts along z, y, x axis in pixel.
 
         Returns
         -------
         AlignmentResult
             Result of alignment.
         """
-        iopt, shift, _, corr = super().align(img, max_shifts, quaternion, pos)
+        iopt, shift, _, corr = super().align(img, max_shifts, quaternion, pos, backend)
         quat = self.quaternions[iopt % self._n_rotations]
         return AlignmentResult(label=iopt, shift=shift, quat=quat, score=corr)
 
     def fit(
         self,
         img: NDArray[np.float32],
         max_shifts: tuple[subpixel, subpixel, subpixel],
         cval: float | None = None,
+        backend: Backend | None = None,
     ) -> tuple[NDArray[np.float32], AlignmentResult]:
         """
         Fit image to template based on the alignment model.
 
         Unlike ``BaseAlignmentModel``, rotation optimization is executed in
         parallel to boost calculation.
 
@@ -573,61 +616,63 @@
             Constant value for padding.
 
         Returns
         -------
         np.ndarray, AlignmentResult
             Transformed input image and the alignment result.
         """
+        xp = backend or Backend()
         pool = DaskTaskPool.from_func(self._optimize)
         pos = np.zeros(3, dtype=np.float32)
-        for quat, tmp, mask in zip(
-            self.quaternions, self._template_input, self._mask_input
-        ):
+        img_input = xp.asarray(img)
+        _template, _mask = self._get_template_and_mask_input(backend=xp)
+        for quat, tmp, mask in zip(self.quaternions, _template, _mask):
             pool.add_task(
-                self.pre_transform(img * mask),
+                self.pre_transform(img_input * mask, xp),
                 tmp,
                 max_shifts,
                 quat,
                 pos=pos,
+                backend=xp,
             )
         results = pool.compute()
         scores = [x[2] for x in results]
         iopt = np.argmax(scores)
         opt_result = results[iopt]
         result = AlignmentResult(
             label=0,
             shift=opt_result[0],
             quat=self.quaternions[iopt],
             score=opt_result[2],
         )
 
-        mtx = result.affine_matrix(img.shape)
-        _img_cval = _normalize_cval(cval, img)
-        img_trans = affine_transform(img, mtx, cval=_img_cval)
-        return img_trans, result
+        mtx = result.affine_matrix(img_input.shape)
+        _img_cval = _normalize_cval(cval, img_input, xp)
+        img_trans = xp.affine_transform(img_input, mtx, cval=_img_cval)
+        return xp.asnumpy(img_trans), result
 
     def _transform_template(
         self,
-        temp: NDArray[np.float32],
+        temp: AnyArray[np.float32],
         matrix: NDArray[np.float32],
         cval: float | None = None,
         order: int = 3,
         prefilter: bool = True,
-    ) -> NDArray[np.complex64]:
-        _cval = _normalize_cval(cval, temp)
-
-        return self.pre_transform(
-            affine_transform(
-                temp, matrix=matrix, cval=_cval, order=order, prefilter=prefilter
-            )
+        backend: Backend = NUMPY_BACKEND,
+    ) -> _Template:
+        _cval = _normalize_cval(cval, temp, backend)
+        temp_transformed = backend.affine_transform(
+            temp, matrix=matrix, cval=_cval, order=order, prefilter=prefilter
         )
+        return self.pre_transform(temp_transformed, backend)
 
     def _get_template_and_mask_input(
         self,
-    ) -> tuple[NDArray[np.complex64], NDArray[np.float32]]:
+        backend: Backend | None = None,
+    ) -> tuple[_Template, NDArray[np.float32]]:
         """
         Returns proper template image for alignment.
 
         Template dimensionality will be dispatched according to the input
         parameters. Returned template should be used in line of the
         :func:`get_alignment_function`.
 
@@ -639,79 +684,94 @@
             - no rotation, single template image ... 3D
             - has rotation, single template image ... 4D
             - no rotation, many template images ... 4D
             - has rotation, many template images ... 4D and when iterated over
               the first axis yielded images will be (rot0, temp0),
               (rot0, temp1), ...
         """
+        xp = backend or Backend()
         if self._n_rotations > 1:
             rotators = [Rotation.from_quat(r).inv() for r in self.quaternions]
             matrices = compose_matrices(
                 np.array(self._template.shape[-3:]) / 2 - 0.5, rotators
             )
             cval = float(np.percentile(self._template, 1))
             if self._n_templates > 1:
-                inputs_templates: list[NDArray[np.float32]] = [
-                    spline_filter(
+                inputs_templates = [
+                    xp.spline_filter(
                         tmp * self._mask,
                         order=3,
                         mode="constant",
                         output=np.float32,
                     )
                     for tmp in self._template
                 ]
                 pool_template = DaskTaskPool.from_func(self._transform_template)
-                pool_mask = DaskTaskPool.from_func(affine_transform)
+                pool_mask = DaskTaskPool.from_func(xp.affine_transform)
                 ntmp = len(inputs_templates)
                 for mat in matrices:
                     for tmp in inputs_templates:
                         pool_template.add_task(
-                            tmp, mat, order=3, cval=cval, prefilter=False
+                            tmp,
+                            mat,
+                            order=3,
+                            cval=cval,
+                            prefilter=False,
+                            backend=xp,
                         )
                     pool_mask.add_tasks(
                         ntmp, self._mask, mat, order=3, mode="nearest", prefilter=False
                     )
             else:
-                template_masked = spline_filter(
+                template_masked = xp.spline_filter(
                     self._template * self._mask,
                     order=3,
                     output=np.float32,
                     mode="constant",
                 )
                 pool_template = DaskTaskPool.from_func(self._transform_template)
-                pool_mask = DaskTaskPool.from_func(affine_transform)
+                pool_mask = DaskTaskPool.from_func(xp.affine_transform)
                 for mat in matrices:
                     pool_template.add_task(
-                        template_masked, mat, order=3, cval=cval, prefilter=False
+                        template_masked,
+                        mat,
+                        order=3,
+                        cval=cval,
+                        prefilter=False,
+                        backend=xp,
                     )
                     pool_mask.add_task(
                         self._mask, mat, order=3, mode="nearest", prefilter=False
                     )
 
             _templates, _masks = compute(
                 (
                     pool_template.asarrays(self.input_shape, dtype=np.complex64),
                     pool_mask.asarrays(self.input_shape, dtype=np.float32),
                 )
             )
-            template_input = np.stack(_templates, axis=0)
-            mask_input = np.stack(_masks, axis=0)
+            template_input = xp.stack(_templates, axis=0)
+            mask_input = xp.stack(_masks, axis=0)
         else:
             pool = DaskTaskPool.from_func(self.pre_transform)
             if self._n_templates > 1:
                 for tmp in self._template:
-                    pool.add_task(tmp * self._mask)
-                template_input = np.stack(pool.compute(), axis=0)
-                mask_input = np.stack([self._mask] * len(self._template), axis=0)
+                    pool.add_task(tmp * self._mask, xp)
+                template_input = xp.stack(pool.compute(), axis=0)
+                mask_input = xp.stack(
+                    [xp.asarray(self._mask)] * self._n_templates, axis=0
+                )
 
             else:
                 # NOTE: dask.compute is always called once inside this method.
-                template_input = pool.add_task(self._template * self._mask).compute()[0]
-                mask_input = self._mask
+                template_masked = xp.asarray(self._template * self._mask)
+                template_input = pool.add_task(template_masked, xp).compute()[0]
+                mask_input = xp.asarray(self._mask)
 
+        self._template_mask_cache.set(xp, template_input, mask_input)
         return template_input, mask_input
 
     def _is_multiple(self) -> bool:
         return self._n_templates * self._n_rotations > 1
 
     @property
     def niter(self) -> int:
@@ -756,22 +816,25 @@
         return ParametrizedModel(
             cls,
             rotations=rotations,
             cutoff=cutoff,
             tilt_range=tilt_range,
         )
 
-    def pre_transform(self, image: NDArray[np.float32]) -> NDArray[np.complex64]:
+    def pre_transform(
+        self, image: AnyArray[np.float32], backend: Backend
+    ) -> AnyArray[np.complex64]:
         """Apply low-pass filter without IFFT."""
-        return lowpass_filter_ft(image, cutoff=self._cutoff)
+        return backend.lowpass_filter_ft(image, cutoff=self._cutoff)
 
     def masked_difference(
         self,
         image: NDArray[np.float32],
         quaternion: NDArray[np.float32],
+        backend: Backend | None = None,
     ) -> NDArray[np.float32]:
         """
         Difference between an image and the template, considering the missing wedge.
 
         Parameters
         ----------
         image : 3D array
@@ -785,70 +848,87 @@
         3D array
             Difference map.
         """
         if self._n_templates > 1:
             raise NotImplementedError(
                 "Masked difference is not implemented for multi-template."
             )
-        mw = self._get_missing_wedge_mask(quaternion)
-        ft = self._template_input  # NOTE: ft.ndim == 3
-        template_masked = np.real(ifftn(ft * mw))
-        img_input = np.real(ifftn(self.pre_transform(image * self._mask) * mw))
-        return img_input - template_masked
+        xp = backend or Backend()
+        _template, _mask = self._get_template_and_mask_input(xp)
+        image_input = self.pre_transform(xp.asarray(image) * _mask, xp)
+        mw = self._get_missing_wedge_mask(quaternion, xp)
+        template_masked = xp.ifftn(_template * mw).real
+        img_input = xp.ifftn(image_input * mw).real
+        return xp.asnumpy(img_input - template_masked)
 
     def mask_missing_wedge(
         self,
         image: NDArray[np.complex64],
         quaternion: NDArray[np.float32],
+        backend: Backend | None = None,
     ) -> NDArray[np.complex64]:
         """Apply missing wedge mask in the frequency domain."""
-        return image * self._get_missing_wedge_mask(quaternion)
+        xp = backend or Backend()
+        mask = self._get_missing_wedge_mask(quaternion, xp)
+        return xp.asnumpy(xp.asarray(image) * mask)
 
-    def _get_missing_wedge_mask(
-        self, quat: NDArray[np.float32]
-    ) -> NDArray[np.float32] | int:
+    def get_missing_wedge_mask(
+        self, quat: NDArray[np.float32], backend: Backend | None = None
+    ):
         """
-        Create a binary mask that covers tomographical missing wedge.
+        Create a mask that covers tomographical missing wedge.
 
         Parameters
         ----------
         quat : (4,) array
             Quaternion representation of the orientation of the subvolume.
 
         Returns
         -------
-        np.ndarray or float
-            Missing wedge mask. If ``tilt_range`` is None, 1 will be returned.
+        np.ndarray or 1
+            Missing wedge mask array.
         """
+        xp = backend or Backend()
+        return self._get_missing_wedge_mask(quat, xp)
+
+    def _get_missing_wedge_mask(
+        self,
+        quat: NDArray[np.float32],
+        backend: Backend,
+    ) -> AnyArray[np.float32] | int:
+        """Create a mask that covers tomographical missing wedge."""
         if self._tilt_range is None:
             return 1
-        return missing_wedge_mask(
+        return backend.missing_wedge_mask(
             rotator=Rotation.from_quat(quat),
             tilt_range=self._tilt_range,
             shape=self.input_shape,
         )
 
 
-def _normalize_cval(cval: float | None, img: np.ndarray) -> float:
+def _normalize_cval(
+    cval: float | None, img: AnyArray[np.float32], backend: Backend
+) -> float:
     if cval is None:
-        _cval = float(np.percentile(img, 1))
+        _cval = float(backend.percentile(img, 1))
     else:
         _cval = cval
     return _cval
 
 
 @lru_cache(maxsize=2)
-def _create_mesh_for_landscape(
+def _build_mesh(
     shape: tuple[int, int, int],
     max_shifts: tuple[float, float, float],
     upsample: int,
-) -> NDArray[np.float32]:
+    backend: Backend,
+) -> AnyArray[np.float32]:
     upsampled_max_shifts = (np.asarray(max_shifts) * upsample).astype(np.int32)
     center = np.array(shape) / 2 - 0.5
-    mesh = np.meshgrid(
+    mesh = backend.meshgrid(
         *[
-            np.arange(-width, width + 1) / upsample + c
+            backend.arange(-width, width + 1) / upsample + c
             for c, width in zip(center, upsampled_max_shifts)
         ],
         indexing="ij",
     )
-    return np.stack(mesh, axis=0)
+    return backend.stack(mesh, axis=0)
```

### Comparing `acryo-0.3.1/acryo/alignment/_bound.py` & `acryo-0.4.0/acryo/alignment/_bound.py`

 * *Files identical despite different names*

### Comparing `acryo-0.3.1/acryo/classification/_dask_pca.py` & `acryo-0.4.0/acryo/classification/_dask_pca.py`

 * *Files identical despite different names*

### Comparing `acryo-0.3.1/acryo/classification/pca.py` & `acryo-0.4.0/acryo/classification/pca.py`

 * *Files identical despite different names*

### Comparing `acryo-0.3.1/acryo/loader/_base.py` & `acryo-0.4.0/acryo/loader/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     ZNCCAlignment,
     RotationImplemented,
     AlignmentFactory,
     AlignmentResult,
 )
 from acryo import _utils
 from acryo._types import nm, pixel
+from acryo.backend import Backend
 from acryo._dask import DaskArrayList, DaskTaskList, DaskTaskIterator, compute
 from acryo.molecules import Molecules
 from acryo.loader import _misc
 from acryo.loader._group import LoaderGroup
 from acryo.loader._cache import SubtomogramCache
 from acryo.pipe._classes import ImageProvider, ImageConverter
 
@@ -109,41 +110,48 @@
 
     @property
     def corner_safe(self) -> bool:
         """Whether rotation is corner-safe."""
         return self._corner_safe
 
     @abstractmethod
-    def construct_loading_tasks(self, output_shape: _ShapeType = None) -> DaskArrayList:
+    def construct_loading_tasks(
+        self,
+        output_shape: _ShapeType = None,
+        backend: Backend | None = None,
+    ) -> DaskArrayList:
         ...
 
-    def _get_cached_array(self, shape: tuple[int, int, int] | None) -> da.Array | None:
-        return CACHE.get_cache(id(self), shape)
+    def _get_cached_array(
+        self, shape: tuple[int, int, int] | None, backend: Backend | None
+    ) -> da.Array | None:
+        return CACHE.get_cache(id(self), shape, backend)
 
     def construct_dask(
         self,
         output_shape: pixel | tuple[pixel, ...] | None = None,
+        backend: Backend | None = None,
     ) -> da.Array:
         """
         Construct a dask array of subtomograms.
 
         This function is always needed before parallel processing. If subtomograms
         are cached in a memory-map it will be used instead.
 
         Returns
         -------
         da.Array
             An 4-D array which ``arr[i]`` corresponds to the ``i``-th subtomogram.
         """
         output_shape = self._get_output_shape(output_shape)
-
-        if (cached := self._get_cached_array(output_shape)) is not None:
+        xp = backend or Backend()
+        if (cached := self._get_cached_array(output_shape, xp)) is not None:
             return cached
 
-        tasks = self.construct_loading_tasks(output_shape=output_shape)
+        tasks = self.construct_loading_tasks(output_shape, xp)
         out = da.stack(tasks, axis=0)
         return out
 
     @abstractmethod
     def replace(
         self,
         molecules: Molecules | None = None,
@@ -246,17 +254,18 @@
 
         Returns
         -------
         da.Array
             A lazy-loading array that uses the memory-mapped array.
         """
         output_shape = self._get_output_shape(output_shape)
-        if (cached := self._get_cached_array(output_shape)) is not None:
+        backend = Backend()
+        if (cached := self._get_cached_array(output_shape, backend)) is not None:
             return cached
-        dsk = self.construct_dask(output_shape=output_shape)
+        dsk = self.construct_dask(output_shape=output_shape, backend=backend)
         return CACHE.cache_array(dsk, id(self))
 
     @contextmanager
     def cached(self, output_shape: _ShapeType = None) -> Iterator[da.Array]:
         """
         Context manager for caching subtomograms of give shape.
 
@@ -316,30 +325,33 @@
         3D array
             Subtomogram
         """
         tasks = self.construct_loading_tasks(output_shape=output_shape)
         for task in tasks:
             yield task.compute()
 
-    def average(self, output_shape: _ShapeType = None) -> NDArray[np.float32]:
+    def average(
+        self, output_shape: _ShapeType = None, *, backend: Backend | None = None
+    ) -> NDArray[np.float32]:
         """
         Calculate the average of subtomograms.
 
         This function execute so-called "subtomogram averaging". The size of
         subtomograms is determined by the ``self.output_shape`` attribute.
 
         Returns
         -------
         np.ndarray
             Averaged image
         """
+        xp = backend or Backend()
         output_shape = self._get_output_shape(output_shape)
-        dsk = self.construct_dask(output_shape=output_shape)
+        dsk = self.construct_dask(output_shape=output_shape, backend=xp)
         dsk = dsk.rechunk(("auto",) + output_shape)  # type: ignore
-        return da.compute(da.mean(dsk, axis=0))[0]
+        return xp.asnumpy(dsk.mean(axis=0).compute())
 
     def average_split(
         self,
         n_set: int = 1,
         seed: int | None = 0,
         squeeze: bool = True,
         output_shape: _ShapeType = None,
@@ -364,44 +376,46 @@
             shape of the loader object will be used.
 
         Returns
         -------
         np.ndarray
             Averaged images. The shape of the array is (n_set, 2, *output_shape).
         """
+        backend = Backend()
         output_shape = self._get_output_shape(output_shape)
         rng = np.random.default_rng(seed=seed)
 
         tasks: list[da.Array] = []
         dsk = self.construct_dask(output_shape=output_shape)
         nmole = dsk.shape[0]
         for _ in range(n_set):
             ind0, ind1 = _misc.random_splitter(rng, nmole)
             _stack = da.stack(
                 [
-                    da.mean(dsk[ind0].rechunk(("auto",) + output_shape), axis=0),  # type: ignore
-                    da.mean(dsk[ind1].rechunk(("auto",) + output_shape), axis=0),  # type: ignore
+                    dsk[ind0].rechunk(("auto",) + output_shape).mean(axis=0),  # type: ignore
+                    dsk[ind1].rechunk(("auto",) + output_shape).mean(axis=0),  # type: ignore
                 ],
                 axis=0,
             )
             tasks.append(_stack)
 
         out = da.compute(tasks)[0]
-        stack = np.stack(out, axis=0)
+        stack = np.stack([backend.asnumpy(a) for a in out], axis=0)
         if squeeze and n_set == 1:
             stack = stack[0]
         return stack
 
     def align(
         self,
         template: TemplateInputType,
         *,
         mask: MaskInputType = None,
         max_shifts: nm | tuple[nm, nm, nm] = 1.0,
         alignment_model: type[BaseAlignmentModel] | AlignmentFactory = ZNCCAlignment,
+        backend: Backend | None = None,
         **align_kwargs,
     ) -> Self:
         """
         Align subtomograms to the template image.
 
         This method conduct so called "subtomogram alignment". Only shifts and rotations
         are calculated in this method. To get averaged image, you'll have to run "average"
@@ -423,26 +437,28 @@
             Additional keyword arguments passed to the input alignment model.
 
         Returns
         -------
         subtomogram loader object
             A loader instance of the same type with updated molecules.
         """
+        _backend = backend or Backend()
         max_shifts = _normalize_max_shifts(max_shifts)
         _max_shifts_px = np.asarray(max_shifts) / self.scale
 
         model = alignment_model(
             self.normalize_template(template),
             self.normalize_mask(mask),
             **align_kwargs,
         )
         tasks = self.construct_mapping_tasks(
             model.align,
             max_shifts=_max_shifts_px,
             output_shape=model.input_shape,
+            backend=_backend,
             var_kwarg=dict(
                 quaternion=self.molecules.quaternion(),
                 pos=self.molecules.pos / self.scale,
             ),
         )
         all_results = tasks.compute()
         return self._post_align(all_results, model.input_shape)
@@ -500,21 +516,23 @@
         Returns
         -------
         subtomogram loader object
             A loader instance of the same type with updated molecules.
         """
         if output_shape is None and isinstance(mask, np.ndarray):
             output_shape = mask.shape
+        backend = Backend()
         with self.cached(output_shape=output_shape):
-            template = self.average(output_shape=output_shape)
+            template = self.average(output_shape=output_shape, backend=backend)
             out = self.align(
                 template,
                 mask=mask,
                 max_shifts=max_shifts,
                 alignment_model=alignment_model,
+                backend=backend,
                 **align_kwargs,
             )
         return out
 
     def align_multi_templates(
         self,
         templates: list[TemplateInputType],
@@ -560,14 +578,15 @@
             mask=self.normalize_mask(mask),
             **align_kwargs,
         )
         tasks = self.construct_mapping_tasks(
             model.align,
             max_shifts=_max_shifts_px,
             output_shape=model.input_shape,
+            backend=Backend(),
             var_kwarg=dict(
                 quaternion=self.molecules.quaternion(),
                 pos=self.molecules.pos / self.scale,
             ),
         )
         all_results = tasks.compute()
         if isinstance(model, RotationImplemented) and model._n_rotations > 1:
@@ -916,15 +935,15 @@
 
     def filter(
         self,
         predicate: pl.Expr | str | pl.Series | list[bool] | np.ndarray,
     ) -> Self:
         """Return a new loader with filtered molecules."""
         out = self.replace(molecules=self.molecules.filter(predicate))
-        if (cached := self._get_cached_array(shape=None)) is not None:
+        if (cached := self._get_cached_array(None, None)) is not None:
             if isinstance(predicate, (str, pl.Expr)):
                 sl = self.molecules.features.select(predicate).to_numpy().ravel()
             else:
                 sl = np.asarray(predicate)
             CACHE.cache_array(cached[sl], id(out))
         return out
```

### Comparing `acryo-0.3.1/acryo/loader/_batch.py` & `acryo-0.4.0/acryo/loader/_batch.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import numpy as np
 import polars as pl
 
 from dask import array as da
 
 from acryo import _utils
 from acryo.molecules import Molecules
+from acryo.backend import Backend
 from acryo._types import nm, pixel
 from acryo._dask import DaskArrayList
 from acryo.loader._base import LoaderBase
 from acryo.loader._loader import SubtomogramLoader, Unset
 
 if TYPE_CHECKING:
     from numpy.typing import NDArray
@@ -56,17 +57,32 @@
         """All the images in the collection."""
         return MappingProxyType(self._images)
 
     def add_tomogram(
         self,
         image: np.ndarray | da.Array,
         molecules: Molecules,
-        image_id: Hashable = None,
+        image_id: Hashable | None = None,
     ) -> Self:
-        """Add a tomogram and its molecules to the collection."""
+        """
+        Add a tomogram and its molecules to the collection.
+
+        Parameters
+        ----------
+        image : np.ndarray or da.Array
+            Tomogram image. This argument is passed directly to the `SubtomogramLoader`
+            constructor.
+        molecules : Molecules
+            Molecules in the tomogram (corresponding to the ``image`` argument). This
+            argument is passed directly to the `SubtomogramLoader` constructor.
+        image_id : Hashable, optional
+            Identifier for the tomogram. If not provided, a unique identifier will be
+            generated. This identifier is used to tag molecules with the tomogram they
+            reside in.
+        """
         if image_id is None:
             image_id = len(self._images)
             while image_id in self._images:
                 image_id += 1
         molecules = molecules.copy()
         molecules.features = molecules.features.with_columns(
             pl.Series(IMAGE_ID_LABEL, np.full((len(molecules)), image_id))
@@ -161,17 +177,22 @@
         out = self.replace(
             molecules=molecules,
             scale=self.scale * binsize,
         )
         out._images = _images
         return out
 
-    def construct_loading_tasks(self, output_shape: _ShapeType = None) -> DaskArrayList:
+    def construct_loading_tasks(
+        self,
+        output_shape: _ShapeType = None,
+        backend: Backend | None = None,
+    ) -> DaskArrayList:
+        _backend = backend or Backend()
         return DaskArrayList.concat(
-            loader.construct_loading_tasks(output_shape=output_shape)
+            loader.construct_loading_tasks(output_shape=output_shape, backend=_backend)
             for loader in self.loaders
         )
 
 
 class LoaderAccessor:
     def __init__(self, collection: BatchLoader):
         self._loader = weakref.ref(collection)
```

### Comparing `acryo-0.3.1/acryo/loader/_cache.py` & `acryo-0.4.0/acryo/loader/_cache.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 from __future__ import annotations
 
 from typing import NamedTuple, Mapping
 import tempfile
 from contextlib import contextmanager
 import numpy as np
 from dask import array as da
+from acryo.backend import Backend
 
 
 class _Subtomogram(NamedTuple):
     array: da.Array
+    backend: str
 
 
 class SubtomogramCache(Mapping[int, _Subtomogram]):
     def __init__(self, dir=None) -> None:
         self._dict: dict[int, _Subtomogram] = {}
         self._cache_dir = dir
 
@@ -22,36 +24,48 @@
 
     def __len__(self) -> int:
         return len(self._dict)
 
     def __iter__(self):
         return iter(self._dict)
 
-    def cache_array(self, dsk: da.Array, id_) -> da.Array:
+    def cache_array(self, dsk: da.Array, id_: int) -> da.Array:
         shape = dsk.shape
         with tempfile.NamedTemporaryFile(dir=self._cache_dir) as ntf:
             mmap = np.memmap(ntf, dtype=np.float32, mode="w+", shape=shape)
 
+        component = dsk[(0,) * dsk.ndim].compute()
+        _is_cupy = type(component).__module__.startswith("cupy")
+        if _is_cupy:
+            dsk = dsk.map_blocks(lambda x: x.get(), dtype=dsk.dtype)  # type: ignore
         da.store(dsk, mmap, compute=True)
 
         darr = da.from_array(
             mmap,
             chunks=("auto",) + shape[1:],  # type: ignore
             meta=np.array([], dtype=np.float32),
         )
-        self._dict[id_] = _Subtomogram(darr)
+        self._dict[id_] = _Subtomogram(darr, "cupy" if _is_cupy else "numpy")
         return darr
 
     def get_cache(
-        self, id_: int, shape: tuple[int, int, int] | None = None
+        self,
+        id_: int,
+        shape: tuple[int, int, int] | None,
+        backend: Backend | None = None,
     ) -> da.Array | None:
         if id_ in self._dict:
-            dsk = self._dict[id_].array
+            cache = self._dict[id_]
+            dsk = cache.array
             if shape is None or dsk.shape[1:] == shape:
-                return dsk
+                if backend is None:
+                    return dsk
+                elif cache.backend == "cupy" and backend.name == "numpy":
+                    return dsk.map_blocks(backend.asnumpy, dtype=dsk.dtype)  # type: ignore
+                return dsk.map_blocks(backend.asarray, dtype=dsk.dtype)  # type: ignore
         return None
 
     def delete_cache(self, id_):
         self._dict.pop(id_, None)
 
     @contextmanager
     def temporal(self):
```

### Comparing `acryo-0.3.1/acryo/loader/_group.py` & `acryo-0.4.0/acryo/loader/_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     AlignmentResult,
 )
 
 from acryo import _utils
 from acryo._types import nm
 from acryo._dask import compute, DaskTaskList
 from acryo.loader import _misc
+from acryo.backend import Backend, AnyArray
 
 if TYPE_CHECKING:
     from dask.delayed import Delayed
     from numpy.typing import NDArray
     from acryo.loader._base import (
         LoaderBase,
         Unset,
@@ -86,34 +87,40 @@
             )
         )
 
     def __iter__(self) -> Iterator[tuple[_K, _L]]:
         yield from self._it
 
     def average(
-        self, output_shape: _ShapeType | None = None
+        self,
+        output_shape: _ShapeType = None,
+        *,
+        backend: Backend | None = None,
     ) -> dict[_K, NDArray[np.float32]]:
         """Calculate average images."""
+        xp = backend or Backend()
         tasks = []
         keys: list[_K] = []
         for key, loader in self:
             keys.append(key)
             _output_shape = loader._get_output_shape(output_shape)
-            dsk = loader.construct_dask(_output_shape)
+            dsk = loader.construct_dask(_output_shape, backend=xp)
             tasks.append(da.mean(dsk, axis=0))
 
-        out: list[NDArray[np.float32]] = da.compute(tasks)[0]
-        return {key: img for key, img in zip(keys, out)}
+        out: list[AnyArray[np.float32]] = da.compute(tasks)[0]
+        return {key: xp.asnumpy(img) for key, img in zip(keys, out)}
 
     def average_split(
         self,
         n_set: int = 1,
         seed: int | None = 0,
         squeeze: bool = True,
         output_shape: _ShapeType = None,
+        *,
+        backend: Backend | None = None,
     ) -> dict[_K, NDArray[np.float32]]:
         """
         Split subtomograms into two set and average separately.
 
         This method executes pairwise subtomogram averaging using randomly
         selected molecules, which is useful for calculation of such as Fourier
         shell correlation.
@@ -131,20 +138,21 @@
             shape of the loader objects will be used.
 
         Returns
         -------
         dict of np.ndarray
             Averaged images with keys of the group keys.
         """
+        xp = backend or Backend()
         rng = np.random.default_rng(seed=seed)
 
         all_tasks: list[list[da.Array]] = []
         for key, loader in self:
             output_shape = loader._get_output_shape(output_shape)
-            dask_array = loader.construct_dask(output_shape=output_shape)
+            dask_array = loader.construct_dask(output_shape=output_shape, backend=xp)
             nmole = dask_array.shape[0]
             tasks: list[da.Array] = []
             for _ in range(n_set):
                 ind0, ind1 = _misc.random_splitter(rng, nmole)
                 _stack = da.stack(
                     [
                         da.mean(dask_array[ind0], axis=0),
@@ -154,27 +162,28 @@
                 )
                 tasks.append(_stack)
             all_tasks.append(tasks)
 
         computed = da.compute(all_tasks)[0]
         out: dict[_K, NDArray[np.float32]] = {}
         for (key, loader), stack in zip(self, computed):
-            stack = np.stack(stack, axis=0)
+            stack = xp.asnumpy(xp.stack(stack, axis=0))
             if squeeze and n_set == 1:
                 stack = stack[0]
             out[key] = stack
         return out
 
     def align(
         self,
         template: TemplateInputType | Mapping[_K, TemplateInputType],
         *,
         mask: MaskInputType = None,
         max_shifts: nm | tuple[nm, nm, nm] = 1.0,
         alignment_model: type[BaseAlignmentModel] | AlignmentFactory = ZNCCAlignment,
+        backend: Backend | None = None,
         **align_kwargs,
     ) -> LoaderGroup[_K, _L]:
         """
         Align subtomograms to the template image.
 
         This method conduct so called "subtomogram alignment". Only shifts and rotations
         are calculated in this method. To get averaged image, you'll have to run "average"
@@ -209,14 +218,15 @@
                 **align_kwargs,
             )
             _max_shifts_px = np.asarray(max_shifts) / loader.scale
             tasks = loader.construct_mapping_tasks(
                 model.align,
                 max_shifts=_max_shifts_px,
                 output_shape=model.input_shape,
+                backend=backend,
                 var_kwarg=dict(
                     quaternion=loader.molecules.quaternion(),
                     pos=loader.molecules.pos / loader.scale,
                 ),
             )
             all_tasks.append(tasks)
             input_shape = model.input_shape
@@ -234,14 +244,15 @@
     def align_no_template(
         self,
         *,
         mask: MaskInputType = None,
         max_shifts: nm | tuple[nm, nm, nm] = 1.0,
         output_shape: _ShapeType = None,
         alignment_model: type[BaseAlignmentModel] = ZNCCAlignment,
+        backend: Backend | None = None,
         **align_kwargs,
     ) -> LoaderGroup[_K, _L]:
         """
         Align subtomograms without template image.
 
         A template-free version of :func:`align`. This method first
         calculates averaged image and uses it for the alignment template. To
@@ -261,20 +272,22 @@
             Additional keyword arguments passed to the input alignment model.
 
         Returns
         -------
         LoaderGroup
             A loader group with updated molecules.
         """
-        avg = self.average(output_shape=output_shape)
+        xp = backend or Backend()
+        avg = self.average(output_shape=output_shape, backend=xp)
         return self.align(
             avg,
             mask=mask,
             max_shifts=max_shifts,
             alignment_model=alignment_model,
+            backend=xp,
             **align_kwargs,
         )
 
     def align_multi_templates(
         self,
         templates: list[TemplateInputType] | Mapping[_K, list[TemplateInputType]],
         *,
@@ -381,21 +394,25 @@
         else:
             _funcs = funcs
         if schema is None:
             schema = [fn.__name__ for fn in _funcs]
         if len(set(schema)) != len(schema):
             raise ValueError("Schema names must be unique.")
         keys: list[_K] = []
+        xp = Backend()
         for key, loader in self:
             output_shape = loader.output_shape
             if not isinstance(output_shape, tuple):
                 raise ValueError("LoaderGroup has no output shape.")
             taskset = []
             for fn in _funcs:
-                tasks = loader.construct_mapping_tasks(fn, output_shape=output_shape)
+                f_as_np = lambda ar: fn(xp.asnumpy(ar))
+                tasks = loader.construct_mapping_tasks(
+                    f_as_np, output_shape=output_shape
+                )
                 taskset.append(list(tasks))
             all_tasks.append(taskset)
             keys.append(key)
         all_results = da.compute(all_tasks)[0]
         out: dict[_K, pl.DataFrame] = {}
         for key, result in zip(keys, all_results):
             out[key] = pl.DataFrame(np.array(result), schema=schema)
@@ -503,15 +520,15 @@
         self._order = order
         self._scale = scale
         self._output_shape = output_shape
         self._corner_safe = corner_safe
 
     def __iter__(self) -> Iterator[tuple[_K, _L]]:
         loader = self._loader
-        cached = loader._get_cached_array(shape=None)
+        cached = loader._get_cached_array(None, None)
         index_col_name = "__index"
         if index_col_name in loader.molecules.features:
             index_col_name += "_"
         index = pl.Series(index_col_name, np.arange(loader.count()))
         for key, mole in loader.molecules.with_features(index).groupby(self._by):
             _loader = loader.replace(
                 molecules=mole.drop_features(index_col_name),
```

### Comparing `acryo-0.3.1/acryo/loader/_loader.py` & `acryo-0.4.0/acryo/loader/_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # pyright: reportPrivateImportUsage=false
 
 from __future__ import annotations
 from typing import (
     TYPE_CHECKING,
-    Callable,
     NamedTuple,
     Any,
 )
 import numpy as np
-from scipy import ndimage as ndi
 from dask import array as da
 
 from acryo._types import nm, pixel
 from acryo._reader import imread
 from acryo.molecules import Molecules
+from acryo.backend import Backend
 from acryo import _utils
 from acryo.loader import _misc
 from acryo.loader._base import LoaderBase, Unset, _ShapeType
 from acryo._dask import DaskTaskPool, DaskArrayList
 
 if TYPE_CHECKING:
     from typing_extensions import Self
@@ -197,51 +196,52 @@
 
         out._image = binned_image
         return out
 
     def construct_loading_tasks(
         self,
         output_shape: _ShapeType = None,
+        backend: Backend | None = None,
     ) -> DaskArrayList:
         """
         Construct a list of subtomogram lazy loader.
 
         Returns
         -------
         list of Delayed object
             Each object returns a subtomogram on execution by ``da.compute``.
         """
         output_shape = self._get_output_shape(output_shape)
-        if (cached := self._get_cached_array(output_shape)) is not None:
+        xp = backend or Backend()
+        if (cached := self._get_cached_array(output_shape, xp)) is not None:
             return DaskArrayList(cached[i] for i in range(len(self)))
 
         image = self.image
         scale = self.scale
         if isinstance(image, np.ndarray):
-            image = da.from_array(image)
+            image = da.from_array(image, asarray=xp.asarray)
 
         if self.corner_safe:
             _prep = _utils.prepare_affine_cornersafe
         else:
             _prep = _utils.prepare_affine
-        pool = DaskTaskPool.from_func(_rotated_crop)
+        pool = DaskTaskPool.from_func(xp.rotated_crop)
         for i in range(len(self)):
             subvol, mtx = _prep(
                 image,
                 center=self.molecules.pos[i] / scale,
                 output_shape=output_shape,
                 rot=self.molecules.rotator[i],
             )
             pool.add_task(
                 subvol,
                 mtx,
                 shape=output_shape,
                 order=self.order,
-                mode="constant",
-                cval=np.mean,
+                cval=xp.mean,
             )
 
         return pool.asarrays(shape=output_shape, dtype=np.float32)
 
 
 class ClassificationResult(NamedTuple):
     """Tuple of classification results."""
@@ -272,30 +272,7 @@
     # check scale
     _scale = float(scale)
     if _scale <= 0:
         raise ValueError("Negative scale is not allowed.")
 
     _corner_safe = bool(corner_safe)
     return order, _output_shape, _scale, _corner_safe
-
-
-def _rotated_crop(
-    subimg,
-    mtx: NDArray[np.float32],
-    shape: tuple[int, int, int],
-    order: int,
-    mode: str,
-    cval: float | Callable[[NDArray[np.float32]], float],
-) -> NDArray[np.float32]:
-    if callable(cval):
-        cval = cval(subimg)
-
-    out = ndi.affine_transform(
-        subimg,
-        matrix=mtx,
-        output_shape=shape,
-        order=order,
-        prefilter=order > 1,
-        mode=mode,
-        cval=cval,
-    )
-    return out  # type: ignore
```

### Comparing `acryo-0.3.1/acryo/loader/_misc.py` & `acryo-0.4.0/acryo/loader/_misc.py`

 * *Files identical despite different names*

### Comparing `acryo-0.3.1/acryo/loader/_mock.py` & `acryo-0.4.0/acryo/loader/_mock.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 from numpy.typing import NDArray
 from dask import array as da, delayed
 from scipy import ndimage as ndi
 from scipy.spatial.transform import Rotation
 
 from acryo import _utils
 from acryo._types import nm
-from acryo._typed_scipy import fftn, ifftn, spline_filter, affine_transform
+from acryo._typed_scipy import fftn, ifftn, spline_filter
 from acryo._dask import DaskArrayList, DaskTaskPool
 from acryo.molecules import Molecules
+from acryo.backend import Backend
 from acryo.pipe._classes import ImageProvider
 
 if TYPE_CHECKING:
     from typing_extensions import Self
     from ._base import _ShapeType
 
 
@@ -83,19 +84,26 @@
             raise ValueError("Template must be 3D.")
 
     @property
     def molecules(self) -> Molecules:
         """All the molecules"""
         return self._molecules
 
-    def construct_loading_tasks(self, output_shape: _ShapeType = None) -> DaskArrayList:
+    def construct_loading_tasks(
+        self,
+        output_shape: _ShapeType = None,
+        backend: Backend | None = None,
+    ) -> DaskArrayList:
         # TODO: this implementation is not efficent. Radon transformation is not
         # actually needed. Apply missing wedge mask directly to the template, and
         # apply inverse-Radon only to the noise. The linearity of Radon
         # transformation guarantees that the result is correct.
+        _backend = backend or Backend()
+        if _backend.name == "cupy":
+            raise NotImplementedError("Cupy backend is not supported yet.")
         if isinstance(self._template, ImageProvider):
             template = self._template(self.scale)
         else:
             template = self._template
         if output_shape is None:
             output_shape = template.shape
         elif output_shape != template.shape:
@@ -109,15 +117,15 @@
             template = spline_filter(
                 template, order=self.order, mode="constant", output=np.float32
             )
         center = np.array(template.shape) / 2 - 0.5
         matrices = self.molecules.affine_matrix(
             center, center + self.molecules.pos / self.scale
         )
-        pool = DaskTaskPool.from_func(affine_transform)
+        pool = DaskTaskPool.from_func(_backend.affine_transform)
         for mtx in matrices:
             pool.add_task(template, mtx, order=self.order, prefilter=False)
         task_list = pool.asarrays(shape=template.shape, dtype=np.float32)
         if self._degrees is not None:
             task_list = DaskArrayList(
                 simulate_noise(
                     task,
```

### Comparing `acryo-0.3.1/acryo/molecules/_cut.py` & `acryo-0.4.0/acryo/molecules/_cut.py`

 * *Files identical despite different names*

### Comparing `acryo-0.3.1/acryo/molecules/_group.py` & `acryo-0.4.0/acryo/molecules/_group.py`

 * *Files identical despite different names*

### Comparing `acryo-0.3.1/acryo/molecules/_rotation.py` & `acryo-0.4.0/acryo/molecules/_rotation.py`

 * *Files identical despite different names*

### Comparing `acryo-0.3.1/acryo/molecules/core.py` & `acryo-0.4.0/acryo/molecules/core.py`

 * *Files identical despite different names*

### Comparing `acryo-0.3.1/acryo/pick/_base.py` & `acryo-0.4.0/acryo/pick/_base.py`

 * *Files identical despite different names*

### Comparing `acryo-0.3.1/acryo/pick/_concrete.py` & `acryo-0.4.0/acryo/pick/_concrete.py`

 * *Files identical despite different names*

### Comparing `acryo-0.3.1/acryo/pipe/__init__.py` & `acryo-0.4.0/acryo/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `acryo-0.3.1/acryo/pipe/_classes.py` & `acryo-0.4.0/acryo/pipe/_classes.py`

 * *Files identical despite different names*

### Comparing `acryo-0.3.1/acryo/pipe/_curry.py` & `acryo-0.4.0/acryo/pipe/_curry.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from __future__ import annotations
 
-from typing import Callable, TypeVar, Any
+from typing import Callable, Any
 from typing_extensions import ParamSpec, Concatenate
 import inspect
 import numpy as np
 from acryo.pipe._classes import ImageProvider, ImageConverter
 from acryo._types import nm
 
 _P = ParamSpec("_P")
-_R = TypeVar("_R")
 
 
 def provider_function(
     fn: Callable[Concatenate[nm | float, _P], np.ndarray]
 ) -> Callable[_P, ImageProvider]:
     """
     Convert a function into a curried function that returns a image provider.
@@ -23,15 +22,15 @@
     ... def provide_random_image(scale, shape):
     ...     return np.random.random(shape)
     >>> provider = provide_random_image((10, 20, 30))
     >>> provider(0.18)  # return a (10, 20, 30) array
 
     """
 
-    def inner(*args, **kwargs):
+    def inner(*args: _P.args, **kwargs: _P.kwargs):
         _fn = _assert_1_arg(fn)
         return ImageProvider(lambda scale: _fn(scale, *args, **kwargs)).with_name(
             _format_args(fn, *args, **kwargs)
         )
 
     _update_wrapper(inner, fn, npop=1)
     return inner
@@ -52,15 +51,15 @@
     ... def gaussian_filter(img, scale, sigma):
     ...     return ndi.gaussian_filter(img, sigma / scale)
     >>> converter = gaussian_filter(1.5)
     >>> converter(arr)  # return a Gaussian filtered `arr`
 
     """
 
-    def inner(*args, **kwargs):
+    def inner(*args: _P.args, **kwargs: _P.kwargs):
         _fn = _assert_2_args(fn)
         return ImageConverter(
             lambda img, scale: _fn(img, scale, *args, **kwargs)
         ).with_name(_format_args(fn, *args, **kwargs))
 
     _update_wrapper(inner, fn, npop=2)
     return inner
@@ -87,14 +86,15 @@
         1
         for p in inspect.signature(func).parameters.values()
         if p.kind in (p.POSITIONAL_ONLY, p.POSITIONAL_OR_KEYWORD)
     )
     if nargs == 0:
         out = lambda x: func()
         _update_attr(out, func)
+        return out
     else:
         return func
 
 
 def _assert_2_args(func: Callable) -> Callable[[Any, Any], Any]:
     nargs = sum(
         1
```

### Comparing `acryo-0.3.1/acryo/pipe/_imread.py` & `acryo-0.4.0/acryo/pipe/_imread.py`

 * *Files identical despite different names*

### Comparing `acryo-0.3.1/acryo/pipe/_masking.py` & `acryo-0.4.0/acryo/pipe/_masking.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     size = 2 * r + 1
     zz, yy, xx = np.indices((size,) * 3)
     structure = (xx - r) ** 2 + (yy - r) ** 2 + (zz - r) ** 2 <= r**2
     if radius < 0:
         out = ndi.binary_erosion(img, structure=structure, border_value=False)
     elif radius > 0:
         out = ndi.binary_dilation(img, structure=structure, border_value=False)
-    return out
+    return out  # type: ignore
 
 
 @converter_function
 def gaussian_smooth(
     img: NDArray[np.bool_], scale: nm, sigma: nm
 ) -> NDArray[np.float32]:
     """
@@ -77,15 +77,15 @@
     ----------
     sigma : float
         Standard deviation of the Gaussian kernel.
     """
     if sigma == 0:
         return img.astype(np.float32)
     img = ~img
-    dist = ndi.distance_transform_edt(img)
+    dist: NDArray[np.float32] = ndi.distance_transform_edt(img)  # type: ignore
     blurred_mask = np.exp(-(dist**2) / 2 / (sigma / scale) ** 2, dtype=np.float32)
     return blurred_mask
 
 
 def soft_otsu(sigma: nm = 1.0, radius: nm = 1.0, bins: int = 256):
     """
     Pipe operation of soft Otsu thresholding.
```

### Comparing `acryo-0.3.1/acryo/pipe/_transform.py` & `acryo-0.4.0/acryo/pipe/_transform.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from __future__ import annotations
 import numpy as np
 from numpy.typing import NDArray
 from scipy import ndimage as ndi
 from acryo import _utils
 from acryo._types import nm
+from acryo._typed_scipy import shift as ndi_shift
 from acryo.pipe._curry import converter_function
 
 
 @converter_function
 def center_by_mass(
     img: NDArray[np.float32], scale: nm, *, order: int = 3
 ) -> NDArray[np.float32]:
     """Centering an image by its center of mass."""
     shift = np.array(ndi.center_of_mass(img)) - np.array(img.shape) / 2
-    return ndi.shift(img, -shift, order=order, prefilter=order > 1, mode="nearest")  # type: ignore
+    return ndi_shift(img, -shift, order=order, prefilter=order > 1, mode="nearest")
 
 
 @converter_function
 def gaussian_filter(
     img: NDArray[np.float32], scale: nm, *, sigma: nm, mode="reflect", cval: float = 0.0
 ) -> NDArray[np.float32]:
     """Gaussian filtering an image."""
```

### Comparing `acryo-0.3.1/acryo/testing/_templates.py` & `acryo-0.4.0/acryo/testing/_templates.py`

 * *Files identical despite different names*

### Comparing `acryo-0.3.1/acryo/testing/core.py` & `acryo-0.4.0/acryo/testing/core.py`

 * *Files identical despite different names*

### Comparing `acryo-0.3.1/.gitignore` & `acryo-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `acryo-0.3.1/LICENSE` & `acryo-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `acryo-0.3.1/README.md` & `acryo-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `acryo-0.3.1/pyproject.toml` & `acryo-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `acryo-0.3.1/PKG-INFO` & `acryo-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acryo
-Version: 0.3.1
+Version: 0.4.0
 Summary: An extensible cryo-EM/ET toolkit for Python.
 Author-email: Hanjin Liu <liuhanjin-sc@g.ecc.u-tokyo.ac.jp>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Hanjin Liu
         All rights reserved.
```

