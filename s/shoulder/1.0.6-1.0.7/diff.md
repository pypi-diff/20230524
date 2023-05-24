# Comparing `tmp/shoulder-1.0.6.tar.gz` & `tmp/shoulder-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shoulder-1.0.6.tar", max compression
+gzip compressed data, was "shoulder-1.0.7.tar", max compression
```

## Comparing `shoulder-1.0.6.tar` & `shoulder-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1097 2023-05-12 01:39:37.059210 shoulder-1.0.6/LICENSE.md
--rw-r--r--   0        0        0     1867 2023-05-12 20:38:29.614149 shoulder-1.0.6/README.md
--rw-r--r--   0        0        0      824 2023-05-12 20:49:48.004324 shoulder-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      109 2023-05-12 01:39:37.059210 shoulder-1.0.6/src/shoulder/__init__.py
--rw-r--r--   0        0        0     1293 2023-05-12 01:39:37.059210 shoulder-1.0.6/src/shoulder/base.py
--rw-r--r--   0        0        0     2718 2023-05-12 20:49:23.696116 shoulder-1.0.6/src/shoulder/bone.py
--rw-r--r--   0        0        0        0 2023-05-12 01:39:37.059210 shoulder-1.0.6/src/shoulder/glenoid/__init__.py
--rw-r--r--   0        0        0        1 2023-05-12 01:39:37.059210 shoulder-1.0.6/src/shoulder/humerus/__init__.py
--rw-r--r--   0        0        0    18093 2023-05-12 20:29:51.032233 shoulder-1.0.6/src/shoulder/humerus/anatomic_neck.py
--rw-r--r--   0        0        0     3297 2023-05-12 01:39:37.059210 shoulder-1.0.6/src/shoulder/humerus/angles.py
--rw-r--r--   0        0        0    11404 2023-05-12 18:05:39.879225 shoulder-1.0.6/src/shoulder/humerus/bicipital_groove.py
--rw-r--r--   0        0        0     6756 2023-05-12 18:50:36.369783 shoulder-1.0.6/src/shoulder/humerus/canal.py
--rw-r--r--   0        0        0     5267 2023-05-12 18:56:35.104991 shoulder-1.0.6/src/shoulder/humerus/epicondyle.py
--rw-r--r--   0        0        0     7262 2023-05-12 04:24:24.053927 shoulder-1.0.6/src/shoulder/humerus/mesh.py
--rw-r--r--   0        0        0     2803 2023-05-12 01:39:37.059210 shoulder-1.0.6/src/shoulder/plotting.py
--rw-r--r--   0        0        0     6681 2023-05-12 01:39:37.059210 shoulder-1.0.6/src/shoulder/utils.py
--rw-r--r--   0        0        0     2845 1970-01-01 00:00:00.000000 shoulder-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-05-12 01:39:37.059210 shoulder-1.0.7/LICENSE.md
+-rw-r--r--   0        0        0     1867 2023-05-12 20:38:29.614149 shoulder-1.0.7/README.md
+-rw-r--r--   0        0        0      889 2023-05-17 15:29:24.360609 shoulder-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-05-12 01:39:37.059210 shoulder-1.0.7/src/shoulder/__init__.py
+-rw-r--r--   0        0        0     1293 2023-05-12 01:39:37.059210 shoulder-1.0.7/src/shoulder/base.py
+-rw-r--r--   0        0        0     2838 2023-05-15 14:44:39.754454 shoulder-1.0.7/src/shoulder/bone.py
+-rw-r--r--   0        0        0        0 2023-05-12 01:39:37.059210 shoulder-1.0.7/src/shoulder/glenoid/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-12 01:39:37.059210 shoulder-1.0.7/src/shoulder/humerus/__init__.py
+-rw-r--r--   0        0        0    18172 2023-05-15 16:33:59.811699 shoulder-1.0.7/src/shoulder/humerus/anatomic_neck.py
+-rw-r--r--   0        0        0     3297 2023-05-12 01:39:37.059210 shoulder-1.0.7/src/shoulder/humerus/angles.py
+-rw-r--r--   0        0        0    14931 2023-05-15 19:15:58.722698 shoulder-1.0.7/src/shoulder/humerus/bicipital_groove.py
+-rw-r--r--   0        0        0     6628 2023-05-14 03:39:04.887022 shoulder-1.0.7/src/shoulder/humerus/canal.py
+-rw-r--r--   0        0        0     5267 2023-05-12 18:56:35.104991 shoulder-1.0.7/src/shoulder/humerus/epicondyle.py
+-rw-r--r--   0        0        0     7262 2023-05-15 16:47:18.014441 shoulder-1.0.7/src/shoulder/humerus/mesh.py
+-rw-r--r--   0        0        0     2803 2023-05-12 01:39:37.059210 shoulder-1.0.7/src/shoulder/plotting.py
+-rw-r--r--   0        0        0     6681 2023-05-12 01:39:37.059210 shoulder-1.0.7/src/shoulder/utils.py
+-rw-r--r--   0        0        0     2886 1970-01-01 00:00:00.000000 shoulder-1.0.7/PKG-INFO
```

### Comparing `shoulder-1.0.6/LICENSE.md` & `shoulder-1.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.6/README.md` & `shoulder-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.6/pyproject.toml` & `shoulder-1.0.7/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shoulder"
-version = "1.0.6"
+version = "1.0.7"
 description = "patient specific anatomic coordinate system generation for shoulder bones"
 authors = ["Gregory W Spangenberg <gspangen@westerneng.ca>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gregspangenberg/shoulder"
 
 [tool.poetry.dependencies]
@@ -15,20 +15,23 @@
 shapely = "^1.8.4"
 rtree = "^1.0.0"
 plotly = "^5.10.0"
 scikit-spatial = "^6.5.0"
 numpy-stl = "^2.17.1"
 circle-fit = "^0.1.3"
 scikit-learn = "^1.1.2"
+ruptures = "^1.1.7"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.8.0"
 ipykernel = "^6.15.2"
 nbformat = "^5.7.0"
 pwlf = "^2.2.1"
 pyglet = "~1.5"
 ipywidgets = "^7"
+pandas = "^2.0.1"
+statsmodels = "^0.14.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `shoulder-1.0.6/src/shoulder/base.py` & `shoulder-1.0.7/src/shoulder/base.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.6/src/shoulder/bone.py` & `shoulder-1.0.7/src/shoulder/bone.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 
 class Humerus(Bone):
     def __init__(self, stl_file):
         self.stl_file = stl_file
         self.transform = np.identity(4)
         msh = mesh.FullObb(stl_file)
+        self._mesh = msh
 
         self.canal = canal.Canal(msh)
         self.trans_epiconylar = epicondyle.TransEpicondylar(msh)
         self.anatomic_neck = anatomic_neck.AnatomicNeck(msh, self.trans_epiconylar)
         self.bicipital_groove = bicipital_groove.DeepGroove(msh)
 
     def apply_csys_canal_transepiconylar(self) -> np.ndarray:
@@ -37,15 +38,18 @@
 
 class ProximalHumerus(Bone):
     def __init__(self, stl_file):
         self.stl_file = stl_file
         self.transform = np.identity(4)
 
         msh = mesh.ProxObb(stl_file)
+        self._mesh = msh
+
         self.canal = canal.Canal(msh)
+        self.bicipital_groove = bicipital_groove.DeepGroove(msh)
 
     def apply_csys_canal_articular(self, articular) -> np.ndarray:
         self.transform = construct_csys(self.canal._axis, articular)
         self._update_landmark_data(self.transform)
         return self.transform
```

### Comparing `shoulder-1.0.6/src/shoulder/humerus/anatomic_neck.py` & `shoulder-1.0.7/src/shoulder/humerus/anatomic_neck.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,17 +132,20 @@
             self._control_points_ct = fit_plane_pts_ct
             self._control_points = fit_plane_pts_ct
             self._points_ct = plane_pts_ct
             self._points = plane_pts_ct
         return self._points
 
     def transform_landmark(self, transform) -> None:
-        # self._axis = utils.transform_pts(self._axis_ct, transform)
-        self._points = utils.transform_pts(self._points_ct, transform)
-        self._control_points = utils.transform_pts(self._control_points_ct, transform)
+        if self._points is not None:
+            # self._axis = utils.transform_pts(self._axis_ct, transform)
+            self._points = utils.transform_pts(self._points_ct, transform)
+            self._control_points = utils.transform_pts(
+                self._control_points_ct, transform
+            )
 
     def _graph_obj(self):
         if self._points is None:
             return None
         else:
             plot = [
                 go.Mesh3d(
```

### Comparing `shoulder-1.0.6/src/shoulder/humerus/angles.py` & `shoulder-1.0.7/src/shoulder/humerus/angles.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.6/src/shoulder/humerus/bicipital_groove.py` & `shoulder-1.0.7/src/shoulder/humerus/bicipital_groove.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,51 @@
 from shoulder import utils
 from shoulder.base import Landmark
 
-
+import ruptures
 import numpy as np
 import scipy.signal
 import skspatial.objects
 import plotly.graph_objects as go
+from functools import cached_property
 import matplotlib.pyplot as plt
 
 
 class DeepGroove(Landmark):
     def __init__(self, obb):
         self._mesh_oriented_uobb = obb.mesh
         self._transform_uobb = obb.transform
+        self._obb_cutoff_pcts = obb.cutoff_pcts
         self._points_ct = None
         self._points = None
         self._axis_ct = None
         self._axis = None
 
-    def axis(self, cutoff_pcts=[0.75, 0.92], slice_num=35, interp_num=250):
+    def axis(self, cutoff_pcts=[0.35, 0.85], slice_num=35, interp_num=250):
         if self._axis is None:
+            proximal_cutoff, distal_cutoff = self._surgical_neck_cutoff_zs(*cutoff_pcts)
             # slice_num  must use odd soo add 1 if even
             if (slice_num % 2) == 0:
                 slice_num += 1
 
             # find z interval to calculate bicipital groove upon
-            cutoff_pcts.sort()
-            z_max = np.max(self._mesh_oriented_uobb.bounds[:, -1])
-            zs = np.linspace(
-                cutoff_pcts[1] * z_max, cutoff_pcts[0] * z_max, num=slice_num
-            ).flatten()
+            # self.cutoff_pcts.sort()
+            # get length of the bone
+            # z_max = np.max(self._mesh_oriented_uobb.bounds[:, -1])
+            # z_min = np.min(self._mesh_oriented_uobb.bounds[:, -1])
+            # z_length = abs(z_max) + abs(z_min)
+
+            # # find distance that the cutoff percentages are at
+            # # cutoff_pcts.sort()  # ensure bottom slice pct is first
+            # distal_cutoff = self.cutoff_pcts[0] * z_length + z_min
+            # proximal_cutoff = self.cutoff_pcts[1] * z_length + z_min
+
+            zs = np.linspace(distal_cutoff, proximal_cutoff, num=slice_num).flatten()
 
+            # preallocate variables
             xy = np.zeros((interp_num, 2, slice_num))
             polar = np.zeros((interp_num, 2, slice_num))
             weights = np.zeros((interp_num, 2, slice_num))
             to_3Ds = np.zeros((4, 4, slice_num))
 
             for i, z in enumerate(zs):
                 # grab the polygon of the slice
@@ -112,20 +123,36 @@
             bg_peak = list(set(deg_peaks) - set(non_bg_peaks))[0]
 
             # get local minima by specifying serach window for
             # search up to 15 degrees away on each side
             deg_variance = int(round(360 / interp_num) * 15)
             bg_xyz = np.zeros((1, 3, len(zs)))
             for i, z in enumerate(zs):
+                # print(polar_0)
                 bg_idx_near = _find_nearest_idx(
                     polar_0[:, 0, i].flatten(), np.deg2rad(bg_peak)
                 )
-                bg_range = polar_0[
-                    (bg_idx_near - deg_variance) : (bg_idx_near + deg_variance), :, i
-                ]
+                # sometimes the degree variance will be higher than than the index bg is found at
+                # when this occurs the indexing will start with a negative numebr causing it to fail
+                # basically a wrap around problem
+
+                if deg_variance > bg_idx_near:
+                    bg_range = np.concatenate(
+                        (
+                            polar_0[(bg_idx_near - deg_variance) :, :, i],
+                            polar_0[: (bg_idx_near + deg_variance), :, i],
+                        ),
+                        axis=0,
+                    )
+                else:
+                    bg_range = polar_0[
+                        (bg_idx_near - deg_variance) : (bg_idx_near + deg_variance),
+                        :,
+                        i,
+                    ]
                 bg_local_i = np.argmin(bg_range[:, 1])
 
                 # transform back to radial coordinates
                 bg_i = bg_local_i + (bg_idx_near - deg_variance)  # put back in context
                 _bg_xy = _pol2cart(polar[bg_i, :, i].reshape(1, 2))
 
                 # i think to_3D is perhaps fully broken, doesn't seem to work
@@ -145,30 +172,83 @@
             self._axis = line_ends
             self._points_ct = bg_xyz
             self._points = bg_xyz
 
         return self._axis
 
     def transform_landmark(self, transform) -> None:
-        self._points = utils.transform_pts(self._points_ct, transform)
-        self._axis = utils.transform_pts(self._axis_ct, transform)
+        if self._axis is not None:
+            self._points = utils.transform_pts(self._points_ct, transform)
+            self._axis = utils.transform_pts(self._axis_ct, transform)
 
     def _graph_obj(self):
         if self._points is None:
             return None
 
         else:
             plot = go.Scatter3d(
                 x=self._points[:, 0],
                 y=self._points[:, 1],
                 z=self._points[:, 2],
                 name="Bicipital Groove",
             )
             return plot
 
+    def _surgical_neck_cutoff_zs(self, bottom_pct=0.35, top_pct=0.85):
+        """given cutoff perccentages with 0 being the surgical neck and 1 being the
+        top of the head return the z coordaintes
+        """
+        # this basically calcuates where the surgical neck is
+        z_max = np.max(self._mesh_oriented_uobb.bounds[:, -1])
+        z_min = np.min(self._mesh_oriented_uobb.bounds[:, -1])
+        z_length = abs(z_max) + abs(z_min)
+
+        z_low_pct = self._obb_cutoff_pcts[0]
+        z_high_pct = self._obb_cutoff_pcts[1]
+        distal_cutoff = z_low_pct * z_length + z_min
+        proximal_cutoff = z_high_pct * z_length + z_min
+        # print(distal_cutoff)
+
+        z_intervals = np.linspace(distal_cutoff, 0.99 * z_max, 100)
+
+        z_area = np.zeros(len(z_intervals))
+        for i, z in enumerate(z_intervals):
+            slice = self._mesh_oriented_uobb.section(
+                plane_origin=[0, 0, z], plane_normal=[0, 0, 1]
+            )
+            slice, to_3d = slice.to_planar()
+            # big_poly = slice.polygons_closed[
+            #     np.argmax([p.area for p in slice.polygons_closed])
+            # ]
+            z_area[i,] = slice.area
+
+        algo = ruptures.KernelCPD(kernel="rbf")
+        algo.fit(z_area)
+        bkp = algo.predict(n_bkps=1)
+
+        surgical_neck_z = z_intervals[bkp[0]]
+        surgical_neck_top_head = z_max - surgical_neck_z
+        bottom = surgical_neck_z + (surgical_neck_top_head * bottom_pct)
+        top = surgical_neck_z + (surgical_neck_top_head * top_pct)
+
+        # interval on which to calcaulte bicipital groove
+        return [bottom, top]
+
+    def _apply_cutoff_pcts(self, cutoff_pcts):
+        z_max = np.max(self._mesh_oriented_uobb.bounds[:, -1])
+        z_min = np.min(self._mesh_oriented_uobb.bounds[:, -1])
+        z_length = abs(z_max) + abs(z_min)
+
+        # find distance that the cutoff percentages are at
+        # cutoff_pcts.sort()  # ensure bottom slice pct is first
+        distal_cutoff = self.cutoff_pcts[0] * z_length + z_min
+        proximal_cutoff = self.cutoff_pcts[1] * z_length + z_min
+
+        return [distal_cutoff, proximal_cutoff]
+
 
 def _find_nearest_idx(array, value):
     idx = np.searchsorted(array, value, side="left")
     if idx > 0 and (
         idx == len(array) or np.abs(value - array[idx - 1]) < np.abs(value - array[idx])
     ):
         return idx - 1
```

### Comparing `shoulder-1.0.6/src/shoulder/humerus/canal.py` & `shoulder-1.0.7/src/shoulder/humerus/canal.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 
 class Canal(Landmark):
     def __init__(self, obb: mesh.Obb):
         """Calculates the centerline of the humeral canal"""
         self._mesh_oriented_uobb = obb.mesh
         self._transform_uobb = obb.transform
+        self.cutoff_pcts = obb.cutoff_pcts
         self._points_ct = None
         self._points = None
         self._axis_ct = None
         self._axis = None
-        self.cutoff_pcts = obb.cutoff_pcts
 
     def axis(self, cutoff_pcts: list = None, num_slices: int = 50) -> np.ndarray:
         """calculates the centerline in region of humerus
 
         Args:
             cutoff_pcts (list): cutoff for where centerline is to be fit between i.e [0.2,0.8] -> middle 60% of the bone
 
@@ -41,24 +41,22 @@
 
             Returns:
                 centroids (np.array): array of xyz points for centroids along length
                 cutoff_length (float): length between the cutoff percentages on the bone
             """
 
             # get length of the bone
-            y_length = 2 * (
-                abs(msh_o.bounds[0][-1])
-            )  # mesh centered at 0, multiply by 2 to get full length along humeral canal
+            z_max = np.max(msh_o.bounds[:, -1])
+            z_min = np.min(msh_o.bounds[:, -1])
+            z_length = abs(z_max) + abs(z_min)
 
             # find distance that the cutoff percentages are at
             cutoff_pcts.sort()  # ensure bottom slice pct is first
-            distal_cutoff = cutoff_pcts[0] * y_length - (
-                y_length / 2
-            )  # pct of total y-length then subtract to return center to 0
-            proximal_cutoff = cutoff_pcts[1] * y_length - (y_length / 2)
+            distal_cutoff = cutoff_pcts[0] * z_length + z_min
+            proximal_cutoff = cutoff_pcts[1] * z_length + z_min
             # length between cutoff pts
             cutoff_length = abs(proximal_cutoff - distal_cutoff)
 
             # spacing of cuts
             cuts = np.linspace(
                 distal_cutoff, proximal_cutoff, num=num_centroids
             ).flatten()
```

### Comparing `shoulder-1.0.6/src/shoulder/humerus/epicondyle.py` & `shoulder-1.0.7/src/shoulder/humerus/epicondyle.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.6/src/shoulder/humerus/mesh.py` & `shoulder-1.0.7/src/shoulder/humerus/mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
     @property
     def transform(self) -> np.ndarray:
         return self._obb[1]
 
     @property
     def cutoff_pcts(self):
-        return [0.4, 0.8]
+        return [0.5, 0.8]
 
     @cached_property
     def _obb(self):
         """rotates the humerus so the humeral head faces up (+ y-axis)
 
         Args:
             mesh (trimesh.mesh): mesh to rotate up
```

### Comparing `shoulder-1.0.6/src/shoulder/plotting.py` & `shoulder-1.0.7/src/shoulder/plotting.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.6/src/shoulder/utils.py` & `shoulder-1.0.7/src/shoulder/utils.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.6/PKG-INFO` & `shoulder-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shoulder
-Version: 1.0.6
+Version: 1.0.7
 Summary: patient specific anatomic coordinate system generation for shoulder bones
 Home-page: https://github.com/gregspangenberg/shoulder
 License: MIT
 Author: Gregory W Spangenberg
 Author-email: gspangen@westerneng.ca
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: circle-fit (>=0.1.3,<0.2.0)
 Requires-Dist: networkx (>=2.8.6,<3.0.0)
 Requires-Dist: numpy-stl (>=2.17.1,<3.0.0)
 Requires-Dist: plotly (>=5.10.0,<6.0.0)
 Requires-Dist: rtree (>=1.0.0,<2.0.0)
+Requires-Dist: ruptures (>=1.1.7,<2.0.0)
 Requires-Dist: scikit-learn (>=1.1.2,<2.0.0)
 Requires-Dist: scikit-spatial (>=6.5.0,<7.0.0)
 Requires-Dist: scipy (>=1.9.1,<2.0.0)
 Requires-Dist: shapely (>=1.8.4,<2.0.0)
 Requires-Dist: trimesh (>=3.14.1,<4.0.0)
 Project-URL: Repository, https://github.com/gregspangenberg/shoulder
 Description-Content-Type: text/markdown
```

