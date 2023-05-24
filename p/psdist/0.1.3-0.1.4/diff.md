# Comparing `tmp/psdist-0.1.3.tar.gz` & `tmp/psdist-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psdist-0.1.3.tar", last modified: Thu Apr 20 17:37:57 2023, max compression
+gzip compressed data, was "psdist-0.1.4.tar", last modified: Wed May 24 17:51:17 2023, max compression
```

## Comparing `psdist-0.1.3.tar` & `psdist-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-04-20 17:37:57.390984 psdist-0.1.3/
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1070 2022-11-29 16:42:20.000000 psdist-0.1.3/LICENSE
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1160 2023-04-20 17:37:57.390861 psdist-0.1.3/PKG-INFO
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      702 2023-03-07 19:34:27.000000 psdist-0.1.3/README.md
-drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-04-20 17:37:57.389092 psdist-0.1.3/psdist/
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       95 2023-03-02 16:46:32.000000 psdist-0.1.3/psdist/__init__.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     4925 2023-01-17 23:20:27.000000 psdist-0.1.3/psdist/ap.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    12559 2023-04-20 15:24:28.000000 psdist-0.1.3/psdist/cloud.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1247 2023-01-17 19:53:50.000000 psdist-0.1.3/psdist/data.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    17797 2023-04-19 23:33:18.000000 psdist-0.1.3/psdist/image.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1344 2023-03-02 16:46:32.000000 psdist-0.1.3/psdist/utils.py
-drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-04-20 17:37:57.390707 psdist-0.1.3/psdist/visualization/
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      156 2023-03-02 16:46:32.000000 psdist-0.1.3/psdist/visualization/__init__.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    14884 2023-03-02 16:46:32.000000 psdist-0.1.3/psdist/visualization/cloud.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    36292 2023-04-20 17:16:20.000000 psdist-0.1.3/psdist/visualization/grid.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    22274 2023-03-02 16:46:32.000000 psdist-0.1.3/psdist/visualization/image.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     4152 2023-03-02 16:46:32.000000 psdist-0.1.3/psdist/visualization/visualization.py
-drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-04-20 17:37:57.389774 psdist-0.1.3/psdist.egg-info/
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1160 2023-04-20 17:37:57.000000 psdist-0.1.3/psdist.egg-info/PKG-INFO
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      436 2023-04-20 17:37:57.000000 psdist-0.1.3/psdist.egg-info/SOURCES.txt
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)        1 2023-04-20 17:37:57.000000 psdist-0.1.3/psdist.egg-info/dependency_links.txt
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      110 2023-04-20 17:37:57.000000 psdist-0.1.3/psdist.egg-info/requires.txt
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)        7 2023-04-20 17:37:57.000000 psdist-0.1.3/psdist.egg-info/top_level.txt
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      716 2023-04-20 17:36:13.000000 psdist-0.1.3/pyproject.toml
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       38 2023-04-20 17:37:57.391022 psdist-0.1.3/setup.cfg
+drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-05-24 17:51:17.387772 psdist-0.1.4/
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1070 2022-11-29 16:42:20.000000 psdist-0.1.4/LICENSE
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1160 2023-05-24 17:51:17.387656 psdist-0.1.4/PKG-INFO
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      702 2023-03-07 19:34:27.000000 psdist-0.1.4/README.md
+drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-05-24 17:51:17.385944 psdist-0.1.4/psdist/
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       95 2023-03-02 16:46:32.000000 psdist-0.1.4/psdist/__init__.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     4925 2023-01-17 23:20:27.000000 psdist-0.1.4/psdist/ap.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    12828 2023-05-24 15:50:44.000000 psdist-0.1.4/psdist/cloud.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1247 2023-01-17 19:53:50.000000 psdist-0.1.4/psdist/data.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    17668 2023-05-24 15:50:44.000000 psdist-0.1.4/psdist/image.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       53 2023-05-24 15:51:53.000000 psdist-0.1.4/psdist/sampling.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1344 2023-03-02 16:46:32.000000 psdist-0.1.4/psdist/utils.py
+drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-05-24 17:51:17.387468 psdist-0.1.4/psdist/visualization/
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      156 2023-03-02 16:46:32.000000 psdist-0.1.4/psdist/visualization/__init__.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    14912 2023-05-24 17:16:25.000000 psdist-0.1.4/psdist/visualization/cloud.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    36316 2023-05-24 15:50:44.000000 psdist-0.1.4/psdist/visualization/grid.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    22492 2023-05-24 15:50:44.000000 psdist-0.1.4/psdist/visualization/image.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     4152 2023-03-02 16:46:32.000000 psdist-0.1.4/psdist/visualization/visualization.py
+drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-05-24 17:51:17.386656 psdist-0.1.4/psdist.egg-info/
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1160 2023-05-24 17:51:17.000000 psdist-0.1.4/psdist.egg-info/PKG-INFO
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      455 2023-05-24 17:51:17.000000 psdist-0.1.4/psdist.egg-info/SOURCES.txt
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)        1 2023-05-24 17:51:17.000000 psdist-0.1.4/psdist.egg-info/dependency_links.txt
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      110 2023-05-24 17:51:17.000000 psdist-0.1.4/psdist.egg-info/requires.txt
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)        7 2023-05-24 17:51:17.000000 psdist-0.1.4/psdist.egg-info/top_level.txt
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      716 2023-05-24 17:50:13.000000 psdist-0.1.4/pyproject.toml
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       38 2023-05-24 17:51:17.387809 psdist-0.1.4/setup.cfg
```

### Comparing `psdist-0.1.3/LICENSE` & `psdist-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `psdist-0.1.3/PKG-INFO` & `psdist-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psdist
-Version: 0.1.3
+Version: 0.1.4
 Summary: Analysis/visualization of phase space distributions
 Author-email: Austin Hoover <ahoover1218@gmail.com>
 Project-URL: homepage, https://github.com/austin-hoover/psdist
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `psdist-0.1.3/README.md` & `psdist-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `psdist-0.1.3/psdist/ap.py` & `psdist-0.1.4/psdist/ap.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.3/psdist/cloud.py` & `psdist-0.1.4/psdist/cloud.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Functions for n-dimensional point clouds."""
+"""Functions for point clouds."""
 import numpy as np
 import scipy.interpolate
 import scipy.stats
 
 from psdist import ap
 from psdist.utils import array_like
 from psdist.utils import centers_from_edges
@@ -13,52 +13,52 @@
 # Analysis
 # ------------------------------------------------------------------------------
 def mean(X):
     """Compute mean (centroid).
 
     Parameters
     ----------
-    X : ndarray, shape (k, n)
-        Coordinates of k points in n-dimensional space.
+    X : ndarray, shape (n, d)
+        Coordinates of n points in d-dimensional space.
 
     Returns
     -------
-    ndarray, shape (n,)
+    ndarray, shape (d,)
         The centroid coordinates.
     """
     return np.mean(X, axis=0)
 
 
 def cov(X):
     """Compute covariance matrix.
 
     Parameters
     ----------
-    X : ndarray, shape (k, n)
-        Coordinates of k points in n-dimensional space.
+    X : ndarray, shape (n, d)
+        Coordinates of n points in d-dimensional space.
 
     Returns
     -------
-    ndarray, shape (n, n)
+    ndarray, shape (d, d)
         The covariance matrix of second-order moments.
     """
     return np.cov(X.T)
 
 
 def corr(X):
     """Compute correlation matrix.
 
     Parameters
     ----------
-    X : ndarray, shape (k, n)
-        Coordinates of k points in n-dimensional space.
+    X : ndarray, shape (n, d)
+        Coordinates of n points in d-dimensional space.
 
     Returns
     -------
-    ndarray, shape (n, n)
+    ndarray, shape (d, d)
         The correlation matrix.
     """
     return cov2corr(np.cov(X.T))
 
 
 def get_radii(X):
     return np.linalg.norm(X, axis=1)
@@ -71,16 +71,16 @@
 
 
 def enclosing_sphere(X, axis=None, fraction=1.0):
     """Scales sphere until it contains some fraction of points.
 
     Parameters
     ----------
-    X : ndarray, shape (k, n)
-        Coordinates of k points in n-dimensional space.
+    X : ndarray, shape (n, d)
+        Coordinates of n points in d-dimensional space.
     axis : tuple
         The distribution is projected onto this axis before proceeding. The
         ellipsoid is defined in this subspace.
     fraction : float
         Fraction of points in sphere.
 
     Returns
@@ -94,16 +94,16 @@
 
 
 def enclosing_ellipsoid(X, axis=None, fraction=1.0):
     """Scale the rms ellipsoid until it contains some fraction of points.
 
     Parameters
     ----------
-    X : ndarray, shape (k, n)
-        Coordinates of k points in n-dimensional space.
+    X : ndarray, shape (n, d)
+        Coordinates of n points in d-dimensional space.
     axis : tuple
         The distribution is projected onto this axis before proceeding. The
         ellipsoid is defined in this subspace.
     fraction : float
         Fraction of points enclosed.
 
     Returns
@@ -125,22 +125,22 @@
 
 
 def project(X, axis=None):
     """Axis-aligned projection. (Just calls `X[:, axis]`.)
 
     Parameters
     ----------
-    X : ndarray, shape (k, n)
-        Coordinates of k points in n-dimensional space.
+    X : ndarray, shape (n, d)
+        Coordinates of n points in d-dimensional space.
     axis : tuple[int], length l
         The axis on which to project the points.
 
     Returns
     -------
-    ndarray, shape (k, l)
+    ndarray, shape (n, l)
         The points projected onto the specified axis.
     """
     if axis is None:
         axis = tuple(np.arange(X.shape[1]))
     if array_like(axis) and len(axis) > X.shape[1]:
         raise ValueError("Invalid projection axis.")
     return X[:, axis]
@@ -149,113 +149,119 @@
 def transform(X, func=None, **kws):
     """Apply a nonlinear transformation.
 
     This function just calls `np.apply_along_axis`.
 
     Parameters
     ----------
-    X : ndarray, shape (k, n)
-        Coordinates of k points in n-dimensional space.
+    X : ndarray, shape (n, d)
+        Coordinates of n points in d-dimensional space.
     function : callable
         Function applied to each point in X. Call signature is
         `function(point, **kws)` where `point` is an n-dimensional
         point given by one row of `X`.
     **kws
         Key word arguments for
 
     Returns
     -------
-    ndarray, shape (k, n)
+    ndarray, shape (n, d)
         The transformed distribution.
     """
     return np.apply_along_axis(lambda point: func(point, **kws), 1, X)
 
 
 def transform_linear(X, M):
     """Apply a linear transformation.
 
     This function just calls `np.apply_along_axis`.
 
     Parameters
     ----------
-    X : ndarray, shape (k, n)
-        Coordinates of k points in n-dimensional space.
-    M : ndarray, shape (n, n)
+    X : ndarray, shape (n, d)
+        Coordinates of n points in d-dimensional space.
+    M : ndarray, shape (d, d)
         A linear transfer matrix.
 
     Returns
     -------
-    ndarray, shape (k, n)
+    ndarray, shape (n, d)
         The transformed distribution.
     """
     func = lambda point: np.matmul(M, point)
     return transform(X, lambda point: np.matmul(M, point))
 
 
 def shift(X, delta=0.0):
     return X + delta
 
 
 def scale(X, factor=1.0):
     return X * factor
 
 
-def slice_planar(X, axis=None, center=None, width=None):
+def slice_planar(X, axis=None, center=None, width=None, limits=None):
     """Return points within a planar slice.
 
     Parameters
     ----------
-    X : ndarray, shape (k, n)
-        Coordinates of k points in n-dimensional space.
+    X : ndarray, shape (n, d)
+        Coordinates of n points in d-dimensional space.
     axis : tuple
         Slice axes. For example, (0, 1) will slice along the first and
         second axes of the array.
     center : ndarray, shape (n,)
         The center of the box.
-    width : ndarray, shape (n,)
+    width : ndarray, shape (d,)
         The width of the box along each axis.
+    limits : ndarray, shape (d, 2)
+        The (min, max) along each axis. Overrides `center` and `edges` if provided.
 
     Returns
     -------
     ndarray, shape (?, n)
         The points within the box.
     """
-    k, n = X.shape
-    if type(axis) is int:
+    n, d = X.shape
+    if not array_like(axis):
         axis = (axis,)
-    if type(center) in [int, float]:
-        center = np.full(n, center)
-    if type(width) in [int, float]:
-        width = np.full(n, width)
-    center = np.array(center)
-    width = np.array(width)
-    limits = list(zip(center - 0.5 * width, center + 0.5 * width))
+    if limits is None:
+        if not array_like(center):
+            center = np.full(d, center)
+        if not array_like(width):
+            width = np.full(d, width)
+        center = np.array(center)
+        width = np.array(width)
+        limits = list(zip(center - 0.5 * width, center + 0.5 * width))  
+    limits = np.array(limits)
+    if limits.ndim == 0:
+        limits = limits[None, :]
     conditions = []
     for j, (umin, umax) in zip(axis, limits):
         conditions.append(X[:, j] > umin)
         conditions.append(X[:, j] < umax)
     idx = np.logical_and.reduce(conditions)
     return X[idx, :]
 
 
 def slice_sphere(X, axis=None, rmin=0.0, rmax=None):
     """Return points within a spherical shell slice.
 
     Parameters
     ----------
-    X : ndarray, shape (k, n)
-        Coordinates of k points in n-dimensional space.
+    X : ndarray, shape (n, d)
+        Coordinates of n points in d-dimensional space.
     axis : tuple
         The subspace in which to define the sphere.
     rmin, rmax : float
         Inner/outer radius of spherical shell.
 
     Returns
     -------
-    ndarray, shape (?, n)
+    ndarray, shape (?, d)
         The points within the sphere.
     """
     if rmax is None:
         rmax = np.inf
     radii = get_radii(project(X, axis))
     idx = np.logical_and(radii > rmin, radii < rmax)
     return X[idx, :]
@@ -265,24 +271,24 @@
     """Return points within an ellipsoidal shell slice.
 
     The ellipsoid is defined by the covariance matrix of the
     distribution.
 
     Parameters
     ----------
-    X : ndarray, shape (k, n)
-        Coordinates of k points in n-dimensional space.
+    X : ndarray, shape (n, d)
+        Coordinates of n points in d-dimensional space.
     axis : tuple
         The subspace in which to define the ellipsoid.
     rmin, rmax : list[float]
         Min/max "radius" (x^T Sigma^-1 x). relative to covariance matrix.
 
     Returns
     -------
-    ndarray, shape (?, n)
+    ndarray, shape (?, d)
         Points within the shell.
     """
     if rmax is None:
         rmax = np.inf
     radii = get_ellipsoid_radii(project(X, axis))
     idx = np.logical_and(rmin < radii, radii < rmax)
     return X[idx, :]
@@ -292,31 +298,31 @@
     """Return points within a contour shell slice.
 
     The slice is defined by the density contours in the subspace defined by
     `axis`.
 
     Parameters
     ----------
-    X : ndarray, shape (k, n)
-        Coordinates of k points in n-dimensional space.
+    X : ndarray, shape (n, d)
+        Coordinates of n points in d-dimensional space.
     axis : tuple
         The subspace in which to define the density contours.
     lmin, lmax : list[float]
         If `f` is the density in the subspace defined by `axis`, then we select
         points where lmin <= f / max(f) <= lmax.
     interp : bool
         If True, compute the histogram, then interpolate and evaluate the
         resulting function at each point in `X`. Otherwise we keep track
         of the indices in which each point lands when it is binned,
         and accept the point if it's bin has a value within fmin and fmax.
         The latter is a lot slower.
 
     Returns
     -------
-    ndarray, shape (?, n)
+    ndarray, shape (?, d)
         Points within the shell.
     """
     _X = project(X, axis)
     hist, edges = histogram(_X, **hist_kws)
     hist = hist / np.max(hist)
     centers = [0.5 * (e[:-1] + e[1:]) for e in edges]
     if interp:
@@ -344,22 +350,22 @@
 
 
 def norm_xxp_yyp_zzp(X, scale_emittance=False):
     """Normalize x-px, y-py, z-pz, ...
 
     Parameters
     ----------
-    X : ndarray, shape (k, 2n)
-        Coordinates of k points in 2n-dimensional phase space.
+    X : ndarray, shape (n, d)
+        Coordinates of n points in d-dimensional phase space (d is even).
     scale_emittance : bool
         Whether to divide the coordinates by the square root of the rms emittance.
 
     Returns
     -------
-    Xn : ndarray, shape (N, 6)
+    Xn : ndarray, shape (n, d)
         Normalized phase space coordinate array.
     """
     if X.shape[1] % 2 != 0:
         raise ValueError("X must have an even number of columns.")
     Sigma = np.cov(X.T)
     Xn = np.zeros(X.shape)
     for i in range(0, X.shape[1], 2):
@@ -374,20 +380,20 @@
 
 
 def decorrelate(X):
     """Remove cross-plane correlations by permuting (x, x'), (y, y'), (z, z') pairs.
 
     Parameters
     ----------
-    X : ndarray, shape (k, 2n)
-        Coordinates of k points in 2n-dimensional space.
+    X : ndarray, shape (n, d)
+        Coordinates of k points in d-dimensional space (d is even).
 
     Returns
     -------
-    ndarray, shape (k, 2n)
+    ndarray, shape (n, d)
         The decorrelated coordinates.
     """
     if X.shape[1] % 2 != 0:
         raise ValueError("X must have even number of columns.")
     for i in range(0, X.shape[1], 2):
         idx = np.random.permutation(np.arange(X.shape[0]))
         X[:, i : i + 2] = X[idx, i : i + 2]
@@ -395,23 +401,23 @@
 
 
 def downsample(X, samples):
     """Select a random subset of points.
 
     Parameters
     ----------
-    X : ndarray, shape (k, n)
-        Coordinates of k points in n-dimensional space.
+    X : ndarray, shape (n, d)
+        Coordinates of n points in d-dimensional space.
     samples : int or float
         The number of samples to keep If less than 1, specifies
         the fraction of points.
 
     Returns
     -------
-    ndarray, shape (<= k, n)
+    ndarray, shape (<= n, d)
         The downsampled coordinate array.
     """
     samples = min(samples, X.shape[0])
     idx = random_selection(np.arange(X.shape[0]), samples)
     return X[idx, :]
 
 
@@ -444,16 +450,16 @@
 def gaussian_kde(X, **kws):
     """Gaussian kernel density estimation (KDE).
 
     This function just calls `scipy.stats.gaussian_kde`.
 
     Parameters
     ----------
-    X : ndarray, shape (k, n)
-        Coordinates of k points in n-dimensional space.
+    X : ndarray, shape (n, d)
+        Coordinates of n points in d-dimensional space.
     **kws
         Key word arguments
 
     Returns
     -------
     estimator : scipy.stats.gaussian_kde
         The density estimator.
```

### Comparing `psdist-0.1.3/psdist/data.py` & `psdist-0.1.4/psdist/data.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.3/psdist/image.py` & `psdist-0.1.4/psdist/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-"""Functions for n-dimensional images."""
+"""Functions for multi-dimensional images."""
 import numpy as np
 from tqdm import tqdm
 from scipy import ndimage
 
+from psdist.utils import array_like
 from psdist.utils import cov2corr
 from psdist.utils import edges_from_centers
 from psdist.utils import centers_from_edges
 
 
 # Analysis
 # ------------------------------------------------------------------------------
 
 
 def get_grid_coords(*coords):
     """Return list of grid coordinates from coordinate arrays along each axis.
 
     Parameters
     ----------
-    coords : list of 1D arrays
+    coords : list[ndarray]
         Coordinates along each axis of regular grid. Example: [[1, 2, 3], [0, 1, 2]].
 
     Returns
     -------
     ndarray, shape (K, len(coords))
         Coordinate array for all points in the grid. The total number of grid
         points is `K = np.prod([len(c) for c in coords])`.
@@ -33,21 +34,21 @@
     """Return the indices of the maximum element of `f`."""
     return np.unravel_index(np.argmax(f), f.shape)
 
 
 def get_radii(coords, Sigma):
     """Return "radii" (x^T Sigma^-1^T x) from grid coordinates and covariance matrix.
 
-    This is quite slow when n > 4 due to creating a mesh grid.
+    This is quite slow when d > 4 due to creating a mesh grid.
 
     Parameters
     ----------
-    coords : list[ndarray], length n
+    coords : list[ndarray], length d
         Coordinate array for each dimension of the regular grid.
-    Sigma : ndarray, shape (n, n)
+    Sigma : ndarray, shape (d, d)
         Covariance matrix of some distribution on the grid.
 
     Returns
     -------
     R : ndarray
         "Radius" x^T Sigma^-1^T x at each point in grid.
     """
@@ -63,15 +64,15 @@
 
 def radial_density(f, R, radii, dr=None):
     """Return average density within ellipsoidal shells.
 
     Parameters
     ----------
     f : ndarray
-        An n-dimensional image.
+        A d-dimensional image.
     R : ndarray, same shape as `f`.
         Gives the "radius" at each pixel in f.
     radii : ndarray, shape (k,)
         Radii at which to evaluate the density.
     dr : float
         The shell width.
 
@@ -87,48 +88,48 @@
         f_masked = np.ma.masked_where(np.logical_or(R < r, R > r + dr), f)
         # mean density within this shell...
         fr.append(np.mean(f_masked))
     return np.array(fr)
 
 
 def mean(f, coords=None):
-    """Compute the n-dimensional mean.
+    """Compute the d-dimensional mean.
 
     Parameters
     ----------
     f : ndarray
-        An n-dimensional image.
+        A d-dimensional image.
     coords : list[ndarray]
         Coordinates along each axis of the image.
 
     Returns
     -------
-    ndarray, shape (n,)
-        The n-dimensional mean.
+    ndarray, shape (d,)
+        The d-dimensional mean.
     """
     if coords is None:
         coords = [np.arange(f.shape[k]) for k in range(f.ndim)]
     return np.array(
         [np.average(C, weights=f) for C in np.meshgrid(*coords, indexing="ij")]
     )
 
 
 def cov(f, coords=None):
-    """Compute the n x n covariance matrix.
+    """Compute the d x d covariance matrix.
 
     Parameters
     ----------
     f : ndarray
-        An n-dimensional image.
+        A d-dimensional image.
     coords : list[ndarray]
         Coordinates along each axis of the image.
 
     Returns
     -------
-    ndarray, shape (n, n)
+    ndarray, shape (d, d)
         The covariance matrix.
     """
 
     def cov_2x2(_f, _coords):
         COORDS = np.meshgrid(*_coords, indexing="ij")
         Sigma = np.zeros((_f.ndim, _f.ndim))
         _f_sum = np.sum(_f)
@@ -143,20 +144,19 @@
                     EXY = np.sum(_f * X * Y) / _f_sum
                     Sigma[i, j] = Sigma[j, i] = EXY - EX * EY
         return Sigma
 
     if coords is None:
         coords = [np.arange(f.shape[k]) for k in range(f.ndim)]
 
-    n = f.ndim
-    if n < 3:
+    if f.ndim < 3:
         return cov_2x2(f, coords)
 
-    Sigma = np.zeros((n, n))
-    for i in range(n):
+    Sigma = np.zeros((f.ndim, f.ndim))
+    for i in range(f.ndim):
         for j in range(i):
             axis = (i, j)
             _image = project(f, axis=axis)
             _coords = [coords[k] for k in axis]
             # Compute 2 x 2 covariance matrix from this projection.
             _sigma = cov_2x2(_image, _coords)
             # Update elements of n x n covariance matrix. This will update
@@ -164,41 +164,41 @@
             Sigma[i, i] = _sigma[0, 0]
             Sigma[j, j] = _sigma[1, 1]
             Sigma[i, j] = Sigma[j, i] = _sigma[0, 1]
     return Sigma
 
 
 def corr(f, coords=None):
-    """Compute the n x n correlation matrix.
+    """Compute the d x d correlation matrix.
 
     Parameters
     ----------
     f : ndarray
-        An n-dimensional image.
+        A d-dimensional image.
     coords : list[ndarray]
         Coordinates along each axis of the image.
 
     Returns
     -------
-    ndarray, shape (n, n)
+    ndarray, shape (d, d)
         The correlation matrix.
     """
     return cov2corr(cov(f, coords))
 
 
 # Transformation
 # ------------------------------------------------------------------------------
 
 
-def slice_idx(n=1, axis=0, ind=0):
+def slice_idx(d=1, axis=0, ind=0):
     """Return planar slice index array.
 
     Parameters
     ----------
-    n : int
+    d : int
         The number of elements in the slice index array. (The number of dimensions
         in the array to be sliced.)
     axis : list[int]
         The sliced axes.
     ind : list[int] or list[tuple]
         The indices along the sliced axes. If a tuple is provided, this
         defines the (min, max) index.
@@ -216,15 +216,15 @@
         # selects a range along that axis.
         if type(ind) is tuple:
             ind = [ind]
     # Make list if only one ind provided.
     if type(ind) is int:
         ind = [ind]
     # Initialize the slice index to select all elements.
-    idx = n * [slice(None)]
+    idx = d * [slice(None)]
     # If any indices were provided, add them to `idx`.
     for k, item in zip(axis, ind):
         if item is None:
             continue
         elif type(item) is tuple and len(item) == 2:
             idx[k] = slice(item[0], item[1])
         else:
@@ -237,15 +237,15 @@
     """Compute an ellipsoid slice.
 
     Ellipsoid is computed from the covariance matrix of `f`.
 
     Parameters
     ----------
     f : ndarray
-        An n-dimensional image.
+        A d-dimensional image.
     axis : list[int]
         Specificies the subspace in which the ellipsoid slices are computed.
         Example: in x-y-z space, we may define a circle in x-y. This could
         select points within a cylinder in x-y-z.
     rmin, rmax : float
         We select the region between two nested ellipsoids with "radius"
         rmin and rmax. The radius is r = x^T Sigma^-1 x, where Sigma is
@@ -264,15 +264,15 @@
 
 def slice_idx_contour(f, axis=None, lmin=0.0, lmax=1.0):
     """Compute a contour slice.
 
     Parameters
     ----------
     f : ndarray
-        An n-dimensional image.
+        A d-dimensional image.
     axis : list[int]
         Specificies the subspace in which the contours are computed. (See
         `slice_idx_ellipsoid`.)
     lmin, lmax : float
         `f`is projected onto `axis` and the projection `fpr` is normalized to
         the range [0, 1]. Then, we find the points in this subspace such that
         `fpr` is within the range [lmin, lmax].
@@ -303,89 +303,87 @@
 
 def project(f, axis=0):
     """Project along one or more axes.
 
     Parameters
     ----------
     f : ndarray
-        An n-dimensional image.
+        A d-dimensional image.
     axis : list[int]
         The axes onto which the image is projected, i.e., the
         axes which are not summed over. Can be an int or list
         of ints. Array axes are swapped as required.
 
     Returns
     -------
     proj : ndarray
         The projection of `image` onto the specified axis.
     """
     # Sum over specified axes.
-    n = f.ndim
     if type(axis) is int:
         axis = [axis]
     axis = tuple(axis)
     axis_sum = tuple([i for i in range(f.ndim) if i not in axis])
     proj = np.sum(f, axis_sum)
 
     # Order the remaining axes.
-    n = proj.ndim
-    loc = list(range(n))
-    destination = np.zeros(n, dtype=int)
+    loc = list(range(proj.ndim))
+    destination = np.zeros(proj.ndim, dtype=int)
     for i, index in enumerate(np.argsort(axis)):
         destination[index] = i
-    for i in range(n):
+    for i in range(proj.ndim):
         if loc[i] != destination[i]:
             j = loc.index(destination[i])
             proj = np.swapaxes(proj, i, j)
             loc[i], loc[j] = loc[j], loc[i]
     return proj
 
 
 def project1d_contour(f, axis=0, lmin=0.0, lmax=1.0, fpr=None):
-    """Apply contour slice in n-1 dimensions, then project onto the remaining dimension.
+    """Apply contour slice in d - 1 dimensions, then project onto the remaining dimension.
 
     Parameters
     ----------
     f : ndarray
-        An n-dimensional image.
+        A d-dimensional image.
     axis : int
-        The 1D projection axis.
+        The projection axis.
     lmin, lmax : float
-        Min and max contour levels of the (n-1)-dimensional projection of `f`,
+        Min and max contour levels of the (d-1)-dimensional projection of `f`,
         normalized the the range [0, 1].
     fpr : ndarray, shape [f.shape[i] for i in range(f.ndim) if i != axis]
-        The (n-1)-dimensional projection of `f` onto all dimensions other than `axis`.
+        The (d-1)-dimensional projection of `f` onto all dimensions other than `axis`.
         (If not provided, it will be computed within the function.)
 
     Returns
     -------
     ndarray, shape (f.shape[axis],)
-        The 1D projection of the slice.
+        The projection of the slice.
     """
     axis_proj = [i for i in range(f.ndim) if i != axis]
     if fpr is None:
         fpr = project(f, axis=axis_proj)
     fpr = fpr / np.max(fpr)
     idx = slice_idx(
-        n=f.ndim,
+        d=f.ndim,
         axis=axis_proj,
         ind=np.where(np.logical_and(fpr >= lmin, fpr <= lmax)),
     )
     # `f[idx]` will give a two-dimensional array. Normally we need to sum over
     # the first axis. If `axis == 0`, we need to sum over the second axis.
     return np.sum(f[idx], axis=int(axis == 0))
 
 
 def project2d_contour(f, axis=(0, 1), lmin=0.0, lmax=1.0, fpr=None):
-    """Apply contour slice in n-2 dimensions, then project onto the remaining two dimensions.
+    """Apply contour slice in d - 2 dimensions, then project onto the remaining two dimensions.
 
     Parameters
     ----------
     f : ndarray
-        An n-dimensional image.
+        A d-dimensional image.
     axis : tuple
         The 2D projection axis.
     lmin, lmax : float
         Min and max contour levels of the (n-2)-dimensional projection of `f`,
         normalized the the range [0, 1].
     fpr : ndarray, shape [f.shape[i] for i in range(f.ndim) if i != axis]
         The (n-1)-dimensional projection of `f` onto all dimensions other than `axis`.
@@ -409,43 +407,41 @@
     _axis_proj = (1, 2)
     if axis == (0, 1):
         _axis_proj = (0, 1)
     elif axis == (0, f.ndim - 1):
         _axis_proj = (0, 2)
     # Two elements of `idx` will be `slice(None)`; these are the elements in `axis`.
     # These will always be in order. So, if `axis[0] > axis[1]`, we need to flip
-    # `axis_proj`. Need a way to handle this automatically, especially if we
-    # are going to consider m-dimensional projections after applying a contour
-    # slice in (n-m) dimensions.
+    # `axis_proj`. Need a way to handle this automatically.
     if axis[0] > axis[1]:
         _axis_proj = tuple(reversed(_axis_proj))
     return project(f[idx], axis=_axis_proj)
 
 
 def copy_into_new_dim(f, shape=None, axis=-1, method="broadcast", copy=False):
     """Copy image into one or more new dimensions.
 
     See 'https://stackoverflow.com/questions/32171917/how-to-copy-a-2d-array-into-a-3rd-dimension-n-times'
 
     Parameters
     ----------
     f : ndarray
-        An n-dimensional image.
-    shape : n-tuple of ints
+        A d-dimensional image.
+    shape : d-tuple of ints
         The shape of the new dimensions.
     axis : int (0 or -1)
         If 0, the new dimensions will be inserted before the first axis. If -1,
         the new dimensions will be inserted after the last axis. I think
         values other than 0 or -1 should work; this does not currently
         work, at least for `method='broadcast'`, last I checked.
     method : {'repeat', 'broadcast'}
         Whether to use `np.repeat` or `np.expand_dims` and `np.broadcast_to`. The
         'broadcast' method is faster.
     """
-    if type(shape) in [int, np.int32, np.int64]:
+    if not array_like(shape):
         shape = (shape,)
     if method == "repeat":
         for i in range(len(shape)):
             f = np.repeat(np.expand_dims(f, axis), shape[i], axis=axis)
         return f
     elif method == "broadcast":
         if axis == 0:
@@ -549,23 +545,23 @@
 
 def sample_grid(f, coords=None, samples=1):
     """Sample from histogram.
 
     Parameters
     ----------
     f : ndarray
-        An n-dimensional histogram.
+        A d-dimensional histogram.
     coords : list[ndarray]
         Coordinates along each axis of the image.
     samples : int
         The number of samples to draw.
 
     Returns
     -------
-    ndarray, shape (samples, n)
+    ndarray, shape (samples, d)
         Samples drawn from the distribution.
     """
     if coords is None:
         coords = [np.arange(f.shape[k]) for k in range(f.ndim)]
     elif f.ndim == 1:
         coords = [coords]
     edges = [edges_from_centers(c) for c in coords]
```

### Comparing `psdist-0.1.3/psdist/utils.py` & `psdist-0.1.4/psdist/utils.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.3/psdist/visualization/cloud.py` & `psdist-0.1.4/psdist/visualization/cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Plotting routines for discrete sets of points in 2n-dimensional phase space."""
+"""Plotting routines for point clouds."""
 from ipywidgets import interactive
 from ipywidgets import widgets
 from matplotlib import pyplot as plt
 import numpy as np
 import proplot as pplt
 
 import psdist.cloud
@@ -12,16 +12,16 @@
 
 
 def auto_limits(X, sigma=None, pad=0.0, zero_center=False, share_xy=False):
     """Determine axis limits from coordinate array.
 
     Parametersv
     ----------
-    X : ndarray, shape (k, n)
-        Coordinate array for k points in n-dimensional space.
+    X : ndarray, shape (n, d)
+        Coordinate array for n points in d-dimensional space.
     sigma : float
         If a number is provided, it is used to set the limits relative to
         the standard deviation of the distribution.
     pad : float
         Fractional padding to apply to the limits.
     zero_center : bool
         Whether to center the limits on zero.
@@ -63,16 +63,16 @@
 
 
 def plot_rms_ellipse(X, ax=None, level=1.0, center_at_mean=True, **ellipse_kws):
     """Compute and plot RMS ellipse from bunch coordinates.
 
     Parameters
     ----------
-    X : ndarray, shape (k, 2)
-        Coordinate array for k points in 2-dimensional space.
+    X : ndarray, shape (n, 2)
+        Coordinate array for n points in 2-dimensional space.
     ax : Axes
         The axis on which to plot.
     level : number of list of numbers
         If a number, plot the rms ellipse inflated by the number. If a list
         of numbers, repeat for each number.
     center_at_mean : bool
         Whether to center the ellipse at the image centroid.
@@ -85,16 +85,16 @@
 
 
 def scatter(X, ax=None, samples=None, **kws):
     """Convenience function for 2D scatter plot.
 
     Parameters
     ----------
-    X : ndarray, shape (k, n)
-        Coordinate array for k points in n-dimensional space.
+    X : ndarray, shape (n, d)
+        Coordinate array for n points in d-dimensional space.
     ax : Axes
         The axis on which to plot.
     samples : int
         Plot this many random samples.
     **kws
         Key word arguments passed to `ax.scatter`.
     """
@@ -115,16 +115,16 @@
 def hist(X, ax=None, bins="auto", limits=None, **kws):
     """Convenience function for 2D histogram with auto-binning.
 
     For more options, I recommend seaborn.histplot.
 
     Parameters
     ----------
-    X : ndarray, shape (k, 2)
-        Coordinate array for k points in 2-dimensional space.
+    X : ndarray, shape (n, 2)
+        Coordinate array for n points in 2-dimensional space.
     ax : Axes
         The axis on which to plot.
     limits, bins : see `psdist.bunch.histogram`.
     **kws
         Key word arguments passed to `plotting.image`.
     """
     f, coords = psdist.cloud.histogram(X, bins=bins, limits=limits, centers=True)
@@ -132,16 +132,16 @@
 
 
 def kde(X, ax=None, coords=None, res=100, kde_kws=None, **kws):
     """Plot kernel density estimation (KDE).
 
     Parameters
     ----------
-    X : ndarray, shape (k, 2)
-        Coordinate array for k points in 2-dimensional space.
+    X : ndarray, shape (n, 2)
+        Coordinate array for n points in 2-dimensional space.
     ax : Axes
         The axis on which to plot.
     coords : [xcoords, ycoords]
         Coordinates along each axis of a two-dimensional regular grid on which to
         evaluate the density.
     res : int
         If coords is not provided, determines the evaluation grid resolution.
@@ -163,16 +163,16 @@
 
 
 def plot2d(X, kind="hist", rms_ellipse=False, rms_ellipse_kws=None, ax=None, **kws):
     """Plot
 
     Parameters
     ----------
-    X : ndarray, shape (k, n)
-        Coordinate array for k points in n-dimensional space.
+    X : ndarray, shape (n, d)
+        Coordinate array for n points in d-dimensional space.
     kind : {'hist', 'contour', 'contourf', 'scatter', 'kde'}
         The kind of plot.
     rms_ellipse : bool
         Whether to plot the RMS ellipse.
     rms_ellipse_kws : dict
         Key word arguments passed to `visualization.cloud.plot_rms_ellipse`.
     ax : Axes
@@ -204,16 +204,16 @@
 def joint(X, grid_kws=None, marg_hist_kws=None, marg_kws=None, **kws):
     """Joint plot.
 
     This is a convenience function; see `psdist.visualization.grid.JointGrid`.
 
     Parameters
     ----------
-    X : ndarray, shape (k, 2)
-        Coordinates of k points in 2-dimensional space.
+    X : ndarray, shape (n, 2)
+        Coordinates of n points in 2-dimensional space.
     grid_kws : dict
         Key word arguments passed to `JointGrid`.
     marg_hist_kws : dict
         Key word arguments passed to `np.histogram` for 1D histograms.
     marg_kws : dict
         Key word arguments passed to `visualization.plot1d`.
     **kws
@@ -244,16 +244,16 @@
 ):
     """Corner plot (scatter plot matrix).
 
     This is a convenience function; see `psdist.visualization.grid.CornerGrid`.
 
     Parameters
     ----------
-    X : ndarray, shape (k, n)
-        Coordinates of k points in n-dimensional space.
+    X : ndarray, shape (n, d)
+        Coordinates of n points in d-dimensional space.
     limits : list[tuple], length n
         The (min, max) plot limits for each axis.
     labels : list[str], length n
         The axis labels.
     prof_edge_only : bool
         If plotting profiles on top of images (on off-diagonal subplots), whether
         to plot x profiles only in bottom row and y profiles only in left column.
@@ -268,27 +268,27 @@
     -------
     psdist.visualization.grid.CornerGrid
         The `CornerGrid` on which the plot was drawn.
     """
     from psdist.visualization.grid import CornerGrid
     if grid_kws is None:
         grid_kws = dict()
-    cgrid = CornerGrid(n=X.shape[1], **grid_kws)
+    grid = CornerGrid(d=X.shape[1], **grid_kws)
     if labels is not None:
         cgrid.set_labels(labels)
-    cgrid.plot_cloud(
+    grid.plot_cloud(
         X,
         limits=limits,
         autolim_kws=autolim_kws,
         prof_edge_only=prof_edge_only,
         update_limits=update_limits,
         diag_kws=diag_kws,
         **kws,
     )
-    return cgrid
+    return grid
 
 
 def proj2d_interactive_slice(
     X,
     limits=None,
     nbins=30,
     default_ind=(0, 1),
@@ -297,16 +297,16 @@
     units=None,
     **plot_kws,
 ):
     """2D partial projection of bunch with interactive slicing.
 
     Parameters
     ----------
-    X : ndarray, shape (k, n)
-        Coordinates of k points in n-dimensional space.
+    X : ndarray, shape (n, d)
+        Coordinates of n points in d-dimensional space.
     limits : list[(min, max)]
         Limits along each axis.
     nbins : int
         Default number of bins for slicing/viewing. Both can be changed with
         sliders.
     default_ind : (i, j)
         Default view axis.
@@ -314,22 +314,20 @@
         Whether to slice one index along the axis or a range of indices.
     dims, units : list[str], shape (n,)
         Dimension names and units.
     **plot_kws
         Key word arguments passed to `plot2d`.
     """
     plot_kws.setdefault("kind", "hist")
-
-    n = X.shape[1]
     if limits is None:
-        limits = [(np.min(X[:, i]), np.max(X[:, i])) for i in range(n)]
+        limits = [(np.min(X[:, i]), np.max(X[:, i])) for i in range(X.shape[1])]
     if dims is None:
-        dims = [f"x{i + 1}" for i in range(n)]
+        dims = [f"x{i + 1}" for i in range(X.shape[1])]
     if units is None:
-        units = n * [""]
+        units = X.shape[1] * [""]
     dims_units = []
     for dim, unit in zip(dims, units):
         dims_units.append(f"{dim}" + f" [{unit}]" if unit != "" else dim)
 
     # Widgets
     nbins_default = nbins
     dim1 = widgets.Dropdown(options=dims, index=default_ind[0], description="dim 1")
@@ -339,15 +337,15 @@
     )
     nbins_plot = widgets.IntSlider(
         min=2, max=200, value=nbins_default, description="plot res"
     )
     autobin = widgets.Checkbox(description="auto plot res", value=False)
     log = widgets.Checkbox(description="log", value=False)
     sliders, checks = [], []
-    for k in range(n):
+    for k in range(X.shape[1]):
         if slice_type == "int":
             slider = widgets.IntSlider(
                 min=0,
                 max=100,
                 value=0,
                 description=dims[k],
                 continuous_update=True,
@@ -364,15 +362,15 @@
             raise ValueError("Invalid `slice_type`.")
         slider.layout.display = "none"
         sliders.append(slider)
         checks.append(widgets.Checkbox(description=f"slice {dims[k]}"))
 
     def hide(button):
         """Hide inactive sliders."""
-        for k in range(n):
+        for k in range(X.shape[1]):
             # Hide elements for dimensions being plotted.
             valid = dims[k] not in (dim1.value, dim2.value)
             disp = None if valid else "none"
             for element in [sliders[k], checks[k]]:
                 element.layout.display = disp
             # Uncheck boxes for dimensions being plotted.
             if not valid and checks[k].value:
@@ -384,15 +382,15 @@
 
     # Make slider visiblity depend on checkmarks.
     for element in (dim1, dim2, *checks, autobin):
         element.observe(hide, names="value")
 
     # Initial hide
     nbins_plot.layout.display = "none"
-    for k in range(n):
+    for k in range(X.shape[1]):
         if k in default_ind:
             checks[k].layout.display = "none"
             sliders[k].layout.display = "none"
 
     def update(**kws):
         dim1 = kws["dim1"]
         dim2 = kws["dim2"]
@@ -436,15 +434,15 @@
             _X = X[:, :]
         if _X.shape[0] == 0:
             return
 
         # Update plotting key word arguments.
         if plot_kws["kind"] != "scatter":
             plot_kws["bins"] = "auto" if autobin else nbins_plot
-            plot_kws["limits"] = limits
+            plot_kws["limits"] = [limits[axis_view[0]], limits[axis_view[1]]]
             plot_kws["norm"] = "log" if kws["log"] else None
 
         # Plot the selected points.
         fig, ax = pplt.subplots()
         plot2d(_X[:, axis_view], ax=ax, **plot_kws)
         ax.format(xlabel=dims_units[axis_view[0]], ylabel=dims_units[axis_view[1]])
         plt.show()
```

### Comparing `psdist-0.1.3/psdist/visualization/grid.py` & `psdist-0.1.4/psdist/visualization/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
     def plot_image(self, f, coords=None, marg_kws=None, **kws):
         """Plot a 2D image.
 
         Parameters
         ----------
         f : ndarray
-            An n-dimensional image.
+            A d-dimensional image.
         coords : list[ndarray]
             Coordinates along each dimension of `f`.
         marg_kws : dict
             Key word arguments passed to `visualization.plot1d`.
         **kws
             Key word arguments passed to `visualization.image.plot2d.`
         """
@@ -161,28 +161,28 @@
         The index of the dimension plotted on each diagonal subplot.
     offdiag_indices : list[2-tuple of int]
         Indices of the dimensions plotted on each off-diagonal subplot.
     """
     
     def __init__(
         self, 
-        n=4, 
+        d=4, 
         diag=True, 
         diag_norm="max",
         diag_scale=0.65,
         diag_rspine=False,
         limits=None, 
         labels=None, 
         corner=True,
         **fig_kws
     ):
         """
         Parameters
         ----------
-        n : int
+        d : int
             The number of rows/columns.
         diag : bool
             Whether to include diagonal subplots (univariate plots). If False,
             we have an (n - 1) x (n - 1) grid instead of an n x n grid.
         diag_norm : {"max", "area"}
             Normalize 1D histograms max value or the area under the curve.
         diag_scale : float
@@ -196,21 +196,20 @@
         corner : bool
             Whether to hide the upper-triangular subplots.
         **fig_kws
             Key word arguments passed to `pplt.subplots()`.
         """
         # Create figure.
         self.new = True
-        self.n = n
+        self.d = self.nrows = self.ncols = d
         self.corner = corner
         self.diag = diag
         self.diag_norm = diag_norm
         self.diag_scale = diag_scale
         self.diag_rspine = diag_rspine
-        self.nrows = self.ncols = self.n
         if not self.diag:
             self.nrows = self.nrows - 1
             self.ncols = self.ncols - 1
         self.fig_kws = fig_kws
         self.fig_kws.setdefault("figwidth", 1.5 * self.nrows)
         self.fig_kws.setdefault("aligny", True)
         self.fig, self.axs = pplt.subplots(
@@ -226,25 +225,25 @@
         self.diag_axs = []
         self.offdiag_axs = []
         self.offdiag_axs_u = []
         self.diag_indices = []
         self.offdiag_indices = []
         self.offdiag_indices_u = []
         if self.diag:
-            for i in range(self.n):
+            for i in range(self.d):
                 self.diag_axs.append(self.axs[i, i])
                 self.diag_indices.append(i)
-            for i in range(1, self.n):
+            for i in range(1, self.d):
                 for j in range(i):
                     self.offdiag_axs.append(self.axs[i, j])
                     self.offdiag_axs_u.append(self.axs[j, i])
                     self.offdiag_indices.append((j, i))
                     self.offdiag_indices_u.append((i, j))
         else:
-            for i in range(self.n - 1):
+            for i in range(self.d - 1):
                 for j in range(i + 1):
                     self.offdiag_axs.append(self.axs[i, j])
                     self.offdiag_indices.append((j, i + 1))
 
         # Set limits and labels.
         self.limits = limits
         if limits is not None:
@@ -292,15 +291,15 @@
         self._fake_diag_yticks()
 
     def get_labels(self):
         """Return the dimension labels."""
         if self.diag:
             labels = [ax.get_xlabel() for ax in self.diag_axs]
         else:
-            labels = [self.axs[-1, i].get_xlabel() for i in range(self.n - 1)]
+            labels = [self.axs[-1, i].get_xlabel() for i in range(self.d - 1)]
             labels = labels + [self.axs[-1, 0].get_ylabel()]
         return labels
 
     def set_labels(self, labels):
         """Set the dimension labels."""
         for ax, label in zip(self.axs[-1, :], labels):
             ax.format(xlabel=label)
@@ -311,15 +310,15 @@
         self.labels = labels
 
     def get_limits(self):
         """Return the plot limits."""
         if self.diag:
             limits = [ax.get_xlim() for ax in self.diag_axs]
         else:
-            limits = [self.axs[-1, i].get_xlim() for i in range(self.n - 1)]
+            limits = [self.axs[-1, i].get_xlim() for i in range(self.d - 1)]
             limits = limits + [self.axs[-1, 0].get_ylim()]
         return limits
 
     def set_limits(self, limits=None, expand=False):
         """Set the plot limits.
 
         Parameters
@@ -385,20 +384,20 @@
         prof_edge_only=False,
         lower=True,
         upper=True,
         update_limits=True,
         diag_kws=None,
         **kws,
     ):
-        """Plot an n-dimensional image.
+        """Plot an image.
 
         Parameters
         ----------
         f : ndarray
-            An n-dimensional image.
+            A d-dimensional image.
         coords : list[ndarray]
             Coordinates along each axis of the grid (if `data` is an image).
         prof_edge_only : bool
             If plotting profiles on top of images (on off-diagonal subplots), whether
             to plot x profiles only in bottom row and y profiles only in left column.
         lower, upper, bool
             Whether to plot on the lower or upper triangular subplots (or both).
@@ -434,15 +433,15 @@
 
         # Bivariate plots.
         profx, profy = [kws.pop(key) for key in ("profx", "profy")]
         if lower:
             for ax, axis in zip(self.offdiag_axs, self.offdiag_indices):
                 if prof_edge_only:
                     if profx:
-                        kws["profx"] = axis[1] == self.n - 1
+                        kws["profx"] = axis[1] == self.d - 1
                     if profy:
                         kws["profy"] = axis[0] == 0
                 _f = psdist.image.project(f, axis=axis)
                 _f = _f / np.max(_f)
                 _coords = [coords[k] for k in axis]
                 vis_image.plot2d(_f, coords=_coords, ax=ax, **kws)
         if not self.corner and upper:
@@ -462,21 +461,21 @@
         prof_edge_only=False,
         lower=True,
         upper=True,
         update_limits=True,
         diag_kws=None,
         **kws,
     ):
-        """Plot an n-dimensional point cloud.
+        """Plot a point cloud.
 
         Parameters
         ----------
-        X : ndarray, shape (k, n)
-            Coordinates of k points in n-dimensional space.
-        limits : list[tuple], length n
+        X : ndarray, shape (n, d)
+            Coordinates of n points in d-dimensional space.
+        limits : list[tuple], length d
             The (min, max) axis limits.
         bins : 'auto', int, list[int]
             The number of bins along each dimension (if plot type requires histogram
             computation). If int or 'auto', applies to all dimensions. Currently
             the histogram is computed with limits based on the data min/max, not
             the plot limits.
         prof_edge_only : bool
@@ -487,15 +486,14 @@
         update_limits : bool
             Whether to extend the existing plot limits.
         diag_kws : dict
             Key word argument passed to `visualization.plot1d`.
         **kws
             Key word arguments pass to `visualization.cloud.plot2d`
         """
-        n = X.shape[1]
         if diag_kws is None:
             diag_kws = dict()
         diag_kws.setdefault("color", "black")
         diag_kws.setdefault("lw", 1.0)
         diag_kws.setdefault("kind", "step")
         kws.setdefault("kind", "hist")
         kws.setdefault("profx", False)
@@ -508,19 +506,19 @@
             limits = vis_cloud.auto_limits(X, **autolim_kws)
         if update_limits:
             self.set_limits(limits, expand=(not self.new))
         limits = self.get_limits()
         self.new = False
         
         if not psdist.utils.array_like(bins):
-            bins = n * [bins]
+            bins = X.shape[1] * [bins]
 
         # Univariate plots. Remember histogram bins and use them for 2D histograms.
         edges = []
-        for axis in range(self.n):
+        for axis in range(self.d):
             if psdist.utils.array_like(bins[axis]):
                 _edges = bins[axis]
             else:
                 _edges = np.histogram_bin_edges(X[:, axis], bins[axis], limits[axis])
             edges.append(_edges)
             if self.diag:
                 heights, _ = np.histogram(X[:, axis], _edges)
@@ -529,15 +527,15 @@
 
         # Bivariate plots:
         profx, profy = [kws.pop(key) for key in ("profx", "profy")]
         if lower:
             for ax, axis in zip(self.offdiag_axs, self.offdiag_indices):
                 if prof_edge_only:
                     if profx:
-                        kws["profx"] = axis[1] == self.n - 1
+                        kws["profx"] = axis[1] == self.d - 1
                     if profy:
                         kws["profy"] = axis[0] == 0
                 if kws["kind"] in ["hist", "contour", "contourf"]:
                     kws["bins"] = [edges[axis[0]], edges[axis[1]]]
                 vis_cloud.plot2d(X[:, axis], ax=ax, **kws)
         if upper and not self.corner:
             for ax, axis in zip(self.offdiag_axs_u, self.offdiag_indices_u):
@@ -732,20 +730,20 @@
         labels=None,
         axis_view=(0, 1),
         axis_slice=(2, 3),
         pad=0.0,
         debug=False,
         **kws,
     ):
-        """Plot an n-dimensional image.
+        """Plot a d-dimensional image.
 
         Parameters
         ----------
         f : ndarray
-            An n-dimensional image.
+            An d-dimensional image.
         coords : list[ndarray]
             Coordinates along each axis of the grid (if `data` is an image).
         labels : list[str], length n
             Label for each dimension.
         axis_view, axis_slice : 2-tuple of int
             The axis to view (plot) and to slice.
         pad : int, float, list
@@ -779,20 +777,22 @@
         if labels is not None:
             _labels = [labels[i] for i in axis_view + axis_slice]
 
         # Select slice indices.
         if type(pad) in [float, int]:
             pad = len(axis_slice) * [pad]
         ind_slice = []
-        for i, steps, _pad in zip(axis_slice, [self.nrows, self.ncols], pad):
+        for i, nsteps, _pad in zip(axis_slice, [self.nrows, self.ncols], pad):
             start = int(_pad * f.shape[i])
             stop = f.shape[i] - 1 - start
-            if (stop - start) < steps:
+            if stop - start == nsteps - 1:
+                ind_slice.append(np.arange(nsteps))
+            elif (stop - start) < nsteps:
                 raise ValueError(f"f.shape[{i}] < number of slice indices requested.")
-            ind_slice.append(np.linspace(start, stop, steps).astype(int))
+            ind_slice.append(np.linspace(start, stop, nsteps).astype(int))
         ind_slice = tuple(ind_slice)
         self.ind_slice = ind_slice
 
         if debug:
             print("Slice indices:")
             for ind in ind_slice:
                 print(ind)
@@ -883,24 +883,24 @@
         axis_view=(0, 1),
         axis_slice=(2, 3),
         pad=0.0,
         debug=False,
         autolim_kws=None,
         **kws,
     ):
-        """Plot an n-dimensional point cloud.
+        """Plot a point cloud.
 
         NOTE: this is not currently working... for the time being, it is recommended
         to generate a 4D histogram and then call `plot_image`.
 
         Parameters
         ----------
-        X : ndarray, shape (k, n)
-            Coordinates of k points in n-dimensional space.
-        labels : list[str], length n
+        X : ndarray, shape (n, d)
+            Coordinates of n points in d-dimensional space.
+        labels : list[str], length d
             Label for each dimension.
         bins_slice : int, list[int], list[ndarray]
             Specifies the bins used for slicing in `axis_slice`. The bin range
             is determined by the min/max point in `X`.
         axis_view, axis_slice : 2-tuple of int
             The axis to view (plot) and to slice.
         pad : int, float, list
```

### Comparing `psdist-0.1.3/psdist/visualization/image.py` & `psdist-0.1.4/psdist/visualization/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Plotting routines for 2n-dimensional phase space images."""
+"""Plotting routines for multi-dimensional images."""
 from ipywidgets import interactive
 from ipywidgets import widgets
 from matplotlib import pyplot as plt
 import numpy as np
 import proplot as pplt
 
 import psdist.image
@@ -99,14 +99,15 @@
     ax=None,
     kind="pcolor",
     profx=False,
     profy=False,
     prof_kws=None,
     process_kws=None,
     offset=None,
+    offset_type="relative",
     mask=False,
     rms_ellipse=False,
     rms_ellipse_kws=None,
     return_mesh=False,
     **kws,
 ):
     """Plot a two-dimensional image.
@@ -129,17 +130,18 @@
         Whether to plot rms ellipse.
     rms_ellipse_kws : dict
         Key word arguments for `image_rms_ellipse`.
     return_mesh : bool
         Whether to return a mesh from `ax.pcolormesh`.
     process_kws : dict
         Key word arguments passed to `psdist.image.process`.
-    offset : float
-        Adds `min(f) * offset` to the image. Helpful to get rid of zeros for
-        logarithmic color scales.
+    offset, offset_type : float, {"relative", "absolute"}
+        Adds offset to the image (helpful to get rid of zeros for logarithmic 
+        color scales. If offset_type is 'relative' add `min(f) * offset` to
+        the image. Otherwise add `offset`.
     mask : bool
         Whether to plot pixels at or below zero.
     **kws
         Key word arguments passed to plotting function.
     """
     if coords is None:
         coords = [np.arange(f.shape[k]) for k in range(f.ndim)]
@@ -167,17 +169,19 @@
     kws.setdefault("colorbar", False)
     kws.setdefault("colorbar_kw", dict())
 
     # Process the image.
     f = f.copy()
     f = psdist.image.process(f, **process_kws)
     if offset is not None:
-        if np.count_nonzero(f):
+        if offset_type == "relative" and np.count_nonzero(f):
             offset = offset * np.min(f[f > 0])
         f = f + offset
+    else:
+        offset = 0.0
 
     # Make sure there are no more zero elements if norm='log'.
     log = "norm" in kws and kws["norm"] == "log"
     if log:
         kws["colorbar_kw"]["formatter"] = "log"
     if mask or log:
         f = np.ma.masked_less_equal(f, 0)
@@ -195,30 +199,30 @@
             rms_ellipse_kws = dict()
         plot_rms_ellipse(f, coords=coords, ax=ax, **rms_ellipse_kws)
     if profx or profy:
         if prof_kws is None:
             prof_kws = dict()
         if kind == "contourf":
             prof_kws.setdefault("start", "center")
-        plot_profiles(f, coords=coords, ax=ax, profx=profx, profy=profy, **prof_kws)
+        plot_profiles(f - offset, coords=coords, ax=ax, profx=profx, profy=profy, **prof_kws)
     if return_mesh:
         return ax, mesh
     else:
         return ax
 
 
 def joint(f, coords=None, grid_kws=None, marg_kws=None, **kws):
     """Joint plot.
 
     This is a convenience function; see `psdist.visualization.grid.JointGrid`.
 
     Parameters
     ----------
     f : ndarray
-        An 2-dimensional image.
+        A 2-dimensional image.
     coords : list[ndarray]
         Coordinates along each dimension of `f`.
     grid_kws : dict
         Key word arguments passed to `JointGrid`.
     marg_kws : dict
         Key word arguments passed to `visualization.plot1d`.
     **kws
@@ -249,15 +253,15 @@
     """Corner plot (scatter plot matrix).
 
     This is a convenience function; see `psdist.visualization.grid.CornerGrid`.
 
     Parameters
     ----------
     f : ndarray
-        An n-dimensional image.
+        A d-dimensional image.
     coords : list[ndarray]
         Coordinates along each dimension of `f`.
     labels : list[str], length n
         Label for each dimension.
     axis_view, axis_slice : 2-tuple of int
         The axis to view (plot) and to slice.
     pad : int, float, list
@@ -274,15 +278,15 @@
     -------
     psdist.visualization.grid.CornerGrid
         The `CornerGrid` on which the plot was drawn.
     """
     from psdist.visualization.grid import CornerGrid
     if grid_kws is None:
         grid_kws = dict()
-    grid = CornerGrid(n=f.ndim, **grid_kws)
+    grid = CornerGrid(d=f.ndim, **grid_kws)
     if labels is not None:
         grid.set_labels(labels)
     grid.plot_image(
         f,
         coords=coords,
         prof_edge_only=prof_edge_only,
         update_limits=True,
@@ -306,15 +310,15 @@
     """Slice matrix plot.
 
     This is a convenience function; see `psdist.visualization.grid.SliceGrid`.
 
     Parameters
     ----------
     f : ndarray
-        An n-dimensional image.
+        A d-dimensional image.
     coords : list[ndarray]
         Coordinates along each axis of the grid (if `data` is an image).
     labels : list[str], length n
         Label for each dimension.
     axis_view, axis_slice : 2-tuple of int
         The axis to view (plot) and to slice.
     pad : int, float, list
@@ -365,23 +369,23 @@
     dims=None,
     units=None,
     cmaps=None,
     thresh_slider=False,
     profiles_checkbox=False,
     **plot_kws,
 ):
-    """2D partial projection of image with interactive slicing.
+    """2D partial projection with interactive slicing.
 
     The distribution is projected onto the specified axes. Sliders provide the
     option to slice the distribution before projecting.
 
     Parameters
     ----------
     f : ndarray
-        An n-dimensional image.
+        A d-dimensional image.
     coords : list[ndarray]
         Coordinate arrays along each dimension. A square grid is assumed.
     default_ind : (i, j)
         Default x and y index to plot.
     slice_type : {'int', 'range'}
         Whether to slice one index along the axis or a range of indices.
     dims, units : list[str], shape (n,)
@@ -396,21 +400,20 @@
         Key word arguments for `visualization.image.plot2d`.
 
     Returns
     -------
     ipywidgets.widgets.interaction.interactive
         This widget can be displayed by calling `IPython.display.display(gui)`.
     """
-    n = f.ndim
     if coords is None:
-        coords = [np.arange(f.shape[k]) for k in range(n)]
+        coords = [np.arange(f.shape[k]) for k in range(f.ndim)]
     if dims is None:
-        dims = [f"x{i + 1}" for i in range(n)]
+        dims = [f"x{i + 1}" for i in range(f.ndim)]
     if units is None:
-        units = n * [""]
+        units = f.ndim * [""]
     dims_units = []
     for dim, unit in zip(dims, units):
         dims_units.append(f"{dim}" + f" [{unit}]" if unit != "" else dim)
     plot_kws.setdefault("colorbar", True)
     plot_kws["process_kws"] = dict(thresh_type="frac")
 
     # Widgets
@@ -435,15 +438,15 @@
     dim1 = widgets.Dropdown(options=dims, index=default_ind[0], description="dim 1")
     dim2 = widgets.Dropdown(options=dims, index=default_ind[1], description="dim 2")
 
     # Sliders and checkboxes (for slicing). Each unplotted dimension has a
     # checkbox which determine if that dimension is sliced. The slice
     # indices are determined by the slider.
     sliders, checks = [], []
-    for k in range(n):
+    for k in range(f.ndim):
         if slice_type == "int":
             slider = widgets.IntSlider(
                 min=0,
                 max=f.shape[k],
                 value=(f.shape[k] // 2),
                 description=dims[k],
                 continuous_update=True,
@@ -460,15 +463,15 @@
             raise ValueError("`slice_type` must be 'int' or 'range'.")
         slider.layout.display = "none"
         sliders.append(slider)
         checks.append(widgets.Checkbox(description=f"slice {dims[k]}"))
 
     def hide(button):
         """Hide/show sliders."""
-        for k in range(n):
+        for k in range(f.ndim):
             # Hide elements for dimensions being plotted.
             valid = dims[k] not in (dim1.value, dim2.value)
             disp = None if valid else "none"
             for element in [sliders[k], checks[k]]:
                 element.layout.display = disp
             # Uncheck boxes for dimensions being plotted.
             if not valid and checks[k].value:
@@ -477,15 +480,15 @@
             if not checks[k].value:
                 sliders[k].layout.display = "none"
 
     # Update the slider list automatically.
     for element in (dim1, dim2, *checks):
         element.observe(hide, names="value")
     # Initial hide
-    for k in range(n):
+    for k in range(f.ndim):
         if k in default_ind:
             checks[k].layout.display = "none"
             sliders[k].layout.display = "none"
 
     def update(**kws):
         """Update the figure."""
         dim1, dim2 = kws["dim1"], kws["dim2"]
@@ -500,15 +503,15 @@
             if check and dim in (dim1, dim2):
                 return
         if dim1 == dim2:
             return
         # Slice and project the distribution.
         axis_view = [dims.index(dim) for dim in (dim1, dim2)]
         axis_slice = [dims.index(dim) for dim, check in zip(dims, checks) if check]
-        for k in range(n):
+        for k in range(f.ndim):
             if type(ind[k]) is int:
                 ind[k] = (ind[k], ind[k] + 1)
         ind = [ind[k] for k in axis_slice]
         idx = psdist.image.slice_idx(f.ndim, axis_slice, ind)
         _f = psdist.image.project(f[idx], axis_view)
         # Update plotting key word arguments.
         if "cmap" in kws:
@@ -553,20 +556,20 @@
     default_ind=0,
     slice_type="int",
     dims=None,
     units=None,
     fig_kws=None,
     **plot_kws,
 ):
-    """1D partial projection of n-dimensional image with interactive slicing.
+    """1D partial projection with interactive slicing.
 
     Parameters
     ----------
     f : ndarray
-        An n-dimensional image.
+        A d-dimensional image.
     coords : list[ndarray]
         Grid coordinates for each dimension.
     default_ind : int
         Default index to plot.
     slice_type : {'int', 'range'}
         Whether to slice one index along the axis or a range of indices.
     dims, units : list[str], shape (n,)
@@ -579,36 +582,35 @@
         Key word arguments passed to 1D plotting function.
 
     Returns
     -------
     gui : ipywidgets.widgets.interaction.interactive
         This widget can be displayed by calling `IPython.display.display(gui)`.
     """
-    n = f.ndim
     if coords is None:
-        coords = [np.arange(f.shape[k]) for k in range(n)]
+        coords = [np.arange(f.shape[k]) for k in range(f.ndim)]
     if dims is None:
-        dims = [f"x{i + 1}" for i in range(n)]
+        dims = [f"x{i + 1}" for i in range(f.ndim)]
     if units is None:
-        units = n * [""]
+        units = f.ndim * [""]
     dims_units = []
     for dim, unit in zip(dims, units):
         dims_units.append(f"{dim}" + f" [{unit}]" if unit != "" else dim)
     if fig_kws is None:
         fig_kws = dict()
     fig_kws.setdefault("figsize", (4.5, 1.5))
     plot_kws.setdefault("color", "black")
     plot_kws.setdefault("kind", "stepfilled")
 
     # Widgets
     dim1 = widgets.Dropdown(options=dims, index=default_ind, description="dim")
 
     # Sliders
     sliders, checks = [], []
-    for k in range(n):
+    for k in range(f.ndim):
         if slice_type == "int":
             slider = widgets.IntSlider(
                 min=0,
                 max=f.shape[k],
                 value=f.shape[k] // 2,
                 description=dims[k],
                 continuous_update=True,
@@ -625,15 +627,15 @@
             raise ValueError("Invalid `slice_type`.")
         slider.layout.display = "none"
         sliders.append(slider)
         checks.append(widgets.Checkbox(description=f"slice {dims[k]}"))
 
     def hide(button):
         """Hide/show sliders based on checkboxes."""
-        for k in range(n):
+        for k in range(f.ndim):
             # Hide elements for dimensions being plotted.
             valid = dims[k] != dim1.value
             disp = None if valid else "none"
             for element in [sliders[k], checks[k]]:
                 element.layout.display = disp
             # Uncheck boxes for dimensions being plotted.
             if not valid and checks[k].value:
@@ -642,15 +644,15 @@
             if not checks[k].value:
                 sliders[k].layout.display = "none"
 
     # Update the slider list automatically.
     for element in (dim1, *checks):
         element.observe(hide, names="value")
     # Initial hide
-    for k in range(n):
+    for k in range(f.ndim):
         if k == default_ind:
             checks[k].layout.display = "none"
             sliders[k].layout.display = "none"
 
     def update(**kws):
         """Update the figure."""
         dim1 = kws["dim1"]
@@ -663,15 +665,15 @@
         # Return nothing if input does not make sense.
         for dim, check in zip(dims, checks):
             if check and dim == dim1:
                 return
         # Slice, then project onto the specified axis.
         axis_view = dims.index(dim1)
         axis_slice = [dims.index(dim) for dim, check in zip(dims, checks) if check]
-        for k in range(n):
+        for k in range(f.ndim):
             if type(ind[k]) is int:
                 ind[k] = (ind[k], ind[k] + 1)
         ind = [ind[k] for k in axis_slice]
         idx = psdist.image.slice_idx(f.ndim, axis_slice, ind)
         profile = psdist.image.project(f[idx], axis_view)
         if np.max(profile) > 0:
             profile = profile / np.sum(profile)
```

### Comparing `psdist-0.1.3/psdist/visualization/visualization.py` & `psdist-0.1.4/psdist/visualization/visualization.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.3/psdist.egg-info/PKG-INFO` & `psdist-0.1.4/psdist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psdist
-Version: 0.1.3
+Version: 0.1.4
 Summary: Analysis/visualization of phase space distributions
 Author-email: Austin Hoover <ahoover1218@gmail.com>
 Project-URL: homepage, https://github.com/austin-hoover/psdist
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `psdist-0.1.3/pyproject.toml` & `psdist-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "psdist"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Austin Hoover", email="ahoover1218@gmail.com" },
 ]
 description = "Analysis/visualization of phase space distributions"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

