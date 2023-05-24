# Comparing `tmp/fluidsim-core-0.7.2.tar.gz` & `tmp/fluidsim-core-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluidsim-core-0.7.2.tar", last modified: Thu Jan  5 14:33:30 2023, max compression
+gzip compressed data, was "fluidsim-core-0.7.3.tar", last modified: Wed May 24 11:13:06 2023, max compression
```

## Comparing `fluidsim-core-0.7.2.tar` & `fluidsim-core-0.7.3.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:33:30.163074 fluidsim-core-0.7.2/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    21781 2021-01-08 06:29:50.000000 fluidsim-core-0.7.2/LICENSE.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1181 2023-01-05 14:33:30.163074 fluidsim-core-0.7.2/PKG-INFO
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      296 2021-01-08 06:29:50.000000 fluidsim-core-0.7.2/README.rst
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:33:30.159074 fluidsim-core-0.7.2/fluidsim_core/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      301 2022-11-16 08:52:07.000000 fluidsim-core-0.7.2/fluidsim_core/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       22 2023-01-05 13:54:22.000000 fluidsim-core-0.7.2/fluidsim_core/_version.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3647 2022-03-03 16:23:16.000000 fluidsim-core-0.7.2/fluidsim_core/extend_simul.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    17312 2022-11-15 15:16:22.000000 fluidsim-core-0.7.2/fluidsim_core/hexa_files.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3857 2022-09-02 13:06:20.000000 fluidsim-core-0.7.2/fluidsim_core/info.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1868 2022-03-03 16:23:16.000000 fluidsim-core-0.7.2/fluidsim_core/loader.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2568 2021-01-11 13:59:58.000000 fluidsim-core-0.7.2/fluidsim_core/magic.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:33:30.159074 fluidsim-core-0.7.2/fluidsim_core/output/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      223 2023-01-05 13:50:09.000000 fluidsim-core-0.7.2/fluidsim_core/output/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    12347 2022-10-12 12:45:59.000000 fluidsim-core-0.7.2/fluidsim_core/output/base.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    27397 2022-11-15 15:16:22.000000 fluidsim-core-0.7.2/fluidsim_core/output/movies.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6482 2022-10-28 07:09:48.000000 fluidsim-core-0.7.2/fluidsim_core/output/phys_fields.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3039 2022-11-14 21:15:10.000000 fluidsim-core-0.7.2/fluidsim_core/output/phys_fields_snek5000.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2614 2023-01-05 13:53:24.000000 fluidsim-core-0.7.2/fluidsim_core/output/remaining_clock_time.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6526 2022-09-02 13:06:20.000000 fluidsim-core-0.7.2/fluidsim_core/params.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:33:30.159074 fluidsim-core-0.7.2/fluidsim_core/scripts/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      393 2022-11-16 08:52:25.000000 fluidsim-core-0.7.2/fluidsim_core/scripts/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4382 2022-11-29 20:38:00.000000 fluidsim-core-0.7.2/fluidsim_core/scripts/restart.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2311 2022-03-25 09:19:22.000000 fluidsim-core-0.7.2/fluidsim_core/solver.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:33:30.163074 fluidsim-core-0.7.2/fluidsim_core/tests/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        0 2021-01-08 06:29:50.000000 fluidsim-core-0.7.2/fluidsim_core/tests/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1792 2022-11-14 20:40:29.000000 fluidsim-core-0.7.2/fluidsim_core/tests/conftest.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      814 2022-03-03 16:23:16.000000 fluidsim-core-0.7.2/fluidsim_core/tests/solver.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1456 2022-11-14 21:07:29.000000 fluidsim-core-0.7.2/fluidsim_core/tests/test_hexa_files.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      218 2022-03-03 16:23:16.000000 fluidsim-core-0.7.2/fluidsim_core/tests/test_loader.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      474 2022-10-28 07:09:48.000000 fluidsim-core-0.7.2/fluidsim_core/tests/test_output_movies.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      227 2022-03-03 16:23:16.000000 fluidsim-core-0.7.2/fluidsim_core/tests/test_solver.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4174 2022-07-22 08:03:03.000000 fluidsim-core-0.7.2/fluidsim_core/tests/test_solver_with_output.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:33:30.159074 fluidsim-core-0.7.2/fluidsim_core.egg-info/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1181 2023-01-05 14:33:30.000000 fluidsim-core-0.7.2/fluidsim_core.egg-info/PKG-INFO
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1085 2023-01-05 14:33:30.000000 fluidsim-core-0.7.2/fluidsim_core.egg-info/SOURCES.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        1 2023-01-05 14:33:30.000000 fluidsim-core-0.7.2/fluidsim_core.egg-info/dependency_links.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       56 2023-01-05 14:33:30.000000 fluidsim-core-0.7.2/fluidsim_core.egg-info/entry_points.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       70 2023-01-05 14:33:30.000000 fluidsim-core-0.7.2/fluidsim_core.egg-info/requires.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       14 2023-01-05 14:33:30.000000 fluidsim-core-0.7.2/fluidsim_core.egg-info/top_level.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       98 2021-01-08 06:29:50.000000 fluidsim-core-0.7.2/pyproject.toml
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1151 2023-01-05 14:33:30.163074 fluidsim-core-0.7.2/setup.cfg
--rw-rw-r--   0 pierre    (1000) pierre    (1000)       39 2021-01-08 06:29:50.000000 fluidsim-core-0.7.2/setup.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:13:06.664693 fluidsim-core-0.7.3/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    21781 2022-01-14 09:58:02.000000 fluidsim-core-0.7.3/LICENSE.txt
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1181 2023-05-24 11:13:06.664693 fluidsim-core-0.7.3/PKG-INFO
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      296 2022-01-14 09:58:02.000000 fluidsim-core-0.7.3/README.rst
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:13:06.660693 fluidsim-core-0.7.3/fluidsim_core/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      310 2023-05-24 08:58:12.000000 fluidsim-core-0.7.3/fluidsim_core/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)       22 2023-05-24 09:29:00.000000 fluidsim-core-0.7.3/fluidsim_core/_version.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     3647 2022-11-24 10:48:01.000000 fluidsim-core-0.7.3/fluidsim_core/extend_simul.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    17303 2023-05-24 07:56:46.000000 fluidsim-core-0.7.3/fluidsim_core/hexa_files.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     3855 2023-05-24 07:56:46.000000 fluidsim-core-0.7.3/fluidsim_core/info.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      714 2023-05-24 08:58:12.000000 fluidsim-core-0.7.3/fluidsim_core/ipy_load.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1868 2022-11-24 10:48:01.000000 fluidsim-core-0.7.3/fluidsim_core/loader.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2568 2022-01-14 09:58:02.000000 fluidsim-core-0.7.3/fluidsim_core/magic.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:13:06.664693 fluidsim-core-0.7.3/fluidsim_core/output/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      223 2023-01-16 10:43:32.000000 fluidsim-core-0.7.3/fluidsim_core/output/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    12347 2022-11-24 10:48:01.000000 fluidsim-core-0.7.3/fluidsim_core/output/base.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     4368 2023-05-24 07:56:46.000000 fluidsim-core-0.7.3/fluidsim_core/output/dataframe_from_paths.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    27397 2022-11-24 10:48:01.000000 fluidsim-core-0.7.3/fluidsim_core/output/movies.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     6480 2023-05-24 07:56:46.000000 fluidsim-core-0.7.3/fluidsim_core/output/phys_fields.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     3036 2023-05-24 07:56:46.000000 fluidsim-core-0.7.3/fluidsim_core/output/phys_fields_snek5000.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2773 2023-05-10 14:43:49.000000 fluidsim-core-0.7.3/fluidsim_core/output/remaining_clock_time.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     6526 2022-11-24 10:48:01.000000 fluidsim-core-0.7.3/fluidsim_core/params.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      945 2023-05-24 08:58:12.000000 fluidsim-core-0.7.3/fluidsim_core/paths.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:13:06.664693 fluidsim-core-0.7.3/fluidsim_core/scripts/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      393 2022-11-24 10:48:01.000000 fluidsim-core-0.7.3/fluidsim_core/scripts/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     4381 2023-05-24 07:56:46.000000 fluidsim-core-0.7.3/fluidsim_core/scripts/restart.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2277 2023-05-24 08:58:12.000000 fluidsim-core-0.7.3/fluidsim_core/solver.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:13:06.664693 fluidsim-core-0.7.3/fluidsim_core/tests/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)        0 2022-01-14 09:58:02.000000 fluidsim-core-0.7.3/fluidsim_core/tests/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1791 2023-05-24 07:56:46.000000 fluidsim-core-0.7.3/fluidsim_core/tests/conftest.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      814 2022-11-24 10:48:01.000000 fluidsim-core-0.7.3/fluidsim_core/tests/solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1455 2023-05-24 07:56:46.000000 fluidsim-core-0.7.3/fluidsim_core/tests/test_hexa_files.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      218 2022-11-24 10:48:01.000000 fluidsim-core-0.7.3/fluidsim_core/tests/test_loader.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      474 2022-11-24 10:48:01.000000 fluidsim-core-0.7.3/fluidsim_core/tests/test_output_movies.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      227 2022-11-24 10:48:01.000000 fluidsim-core-0.7.3/fluidsim_core/tests/test_solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     4174 2022-11-24 10:48:01.000000 fluidsim-core-0.7.3/fluidsim_core/tests/test_solver_with_output.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:13:06.660693 fluidsim-core-0.7.3/fluidsim_core.egg-info/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1181 2023-05-24 11:13:06.000000 fluidsim-core-0.7.3/fluidsim_core.egg-info/PKG-INFO
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1179 2023-05-24 11:13:06.000000 fluidsim-core-0.7.3/fluidsim_core.egg-info/SOURCES.txt
+-rw-r--r--   0 augier3pi (23665) all-users   (513)        1 2023-05-24 11:13:06.000000 fluidsim-core-0.7.3/fluidsim_core.egg-info/dependency_links.txt
+-rw-r--r--   0 augier3pi (23665) all-users   (513)       56 2023-05-24 11:13:06.000000 fluidsim-core-0.7.3/fluidsim_core.egg-info/entry_points.txt
+-rw-r--r--   0 augier3pi (23665) all-users   (513)       70 2023-05-24 11:13:06.000000 fluidsim-core-0.7.3/fluidsim_core.egg-info/requires.txt
+-rw-r--r--   0 augier3pi (23665) all-users   (513)       14 2023-05-24 11:13:06.000000 fluidsim-core-0.7.3/fluidsim_core.egg-info/top_level.txt
+-rw-r--r--   0 augier3pi (23665) all-users   (513)       98 2022-01-14 09:58:02.000000 fluidsim-core-0.7.3/pyproject.toml
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1151 2023-05-24 11:13:06.664693 fluidsim-core-0.7.3/setup.cfg
+-rw-r--r--   0 augier3pi (23665) all-users   (513)       39 2022-10-27 08:52:15.000000 fluidsim-core-0.7.3/setup.py
```

### Comparing `fluidsim-core-0.7.2/LICENSE.txt` & `fluidsim-core-0.7.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fluidsim-core-0.7.2/PKG-INFO` & `fluidsim-core-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluidsim-core
-Version: 0.7.2
+Version: 0.7.3
 Summary: Pure-Python core library for FluidSim framework
 Home-page: https://foss.heptapod.net/fluiddyn/fluidsim/-/tree/branch/default/lib
 Author: FluidDyn project
 Author-email: fluiddyn@freelists.org
 License: CeCILL License
 Project-URL: Bug Tracker, https://foss.heptapod.net/fluiddyn/fluidsim/-/issues
 Project-URL: Documentation, https://fluidsim.readthedocs.io/en/latest/generated/fluidsim_core.html
```

### Comparing `fluidsim-core-0.7.2/fluidsim_core/extend_simul.py` & `fluidsim-core-0.7.3/fluidsim_core/extend_simul.py`

 * *Files identical despite different names*

### Comparing `fluidsim-core-0.7.2/fluidsim_core/hexa_files.py` & `fluidsim-core-0.7.3/fluidsim_core/hexa_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,14 @@
             time=self.time,
             equation=self.equation,
         )
 
     __rmul__ = __mul__
 
     def __add__(self, arg):
-
         return self.__class__(
             self.key,
             arrays=[arr0 + arr1 for arr0, arr1 in zip(arg.arrays, self.arrays)],
             time=(self.time + arg.time) / 2,
             equation=self.equation,
         )
 
@@ -249,27 +248,25 @@
         hexa_data = self._read_hexadata_from_path(path_file, skip_vars=skip_vars)
         hexa_field = HexaField(key, hexa_data, equation=equation)
         return hexa_field, float(hexa_data.time)
 
     def init_hexa_pcolormesh(
         self, ax, hexa_color, hexa_x, hexa_y, vmin=None, vmax=None, **kwargs
     ):
-
         images = []
 
         if vmax is None:
             vmax = hexa_color.max()
 
         if vmin is None:
             vmin = hexa_color.min()
 
-        for (arr, elem_x, elem_y) in zip(
+        for arr, elem_x, elem_y in zip(
             hexa_color.arrays, hexa_x.elements, hexa_y.elements
         ):
-
             x_edges = elem_x["edges"]
             y_edges = elem_y["edges"]
 
             image = ax.pcolormesh(
                 x_edges,
                 y_edges,
                 arr,
@@ -288,15 +285,15 @@
         def on_move(event):
             if event.inaxes is not None and event.inaxes == ax:
                 x = event.xdata
                 y = event.ydata
 
                 elements_possibly_touched = []
 
-                for (image, elem_x, elem_y) in zip(
+                for image, elem_x, elem_y in zip(
                     images, hexa_x.elements, hexa_y.elements
                 ):
                     xmin, xmax = elem_x["lims"]
                     ymin, ymax = elem_y["lims"]
 
                     x_2d = elem_x["array"]
                     y_2d = elem_y["array"]
@@ -331,15 +328,14 @@
         fig.canvas.mpl_connect("motion_notify_event", on_move)
         # to be able to test this callback
         fig._on_move_hexa = on_move
 
         return images, cbar
 
     def init_quiver_1st_step(self, hexa_x, hexa_y, percentage_dx_quiver=4.0):
-
         xmin = hexa_x.min()
         xmax = hexa_x.max()
 
         ymin = hexa_y.min()
         ymax = hexa_y.max()
 
         dx_quiver = percentage_dx_quiver / 100 * (xmax - xmin)
@@ -399,15 +395,14 @@
         vx_quiver = []
         vy_quiver = []
         vmax = -np.inf
 
         for indices_vectors_in_elem, arr_vx, arr_vy in zip(
             indices_vectors_in_elems, hexa_vx.arrays, hexa_vy.arrays
         ):
-
             vmax_elem = np.max(np.sqrt(arr_vx**2 + arr_vy**2))
             if vmax_elem > vmax:
                 vmax = vmax_elem
 
             for iy, ix in indices_vectors_in_elem:
                 vx_quiver.append(arr_vx[iy, ix])
                 vy_quiver.append(arr_vy[iy, ix])
```

### Comparing `fluidsim-core-0.7.2/fluidsim_core/info.py` & `fluidsim-core-0.7.3/fluidsim_core/info.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     _extenders: list
 
       List of extenders (see :mod:`fluidsim_core.extend_simul`).
 
     """
 
     def __init__(self, only_root=False, **kargs):
-
         if len(kargs) == 0 or ("path_file" in kargs and "tag" not in kargs):
             kargs["tag"] = "solver"
 
         super().__init__(**kargs)
 
         if (
             "tag" in kargs
@@ -71,15 +70,14 @@
                         [
                             f"{extender._module_name}.{extender.__name__}"
                             for extender in self._extenders
                         ],
                     )
 
     def _init_root(self):
-
         self._set_attribs(
             {
                 "module_name": "fluidsim_core.solver",
                 "class_name": "SimulCore",
                 "short_name": "Core",
             }
         )
```

### Comparing `fluidsim-core-0.7.2/fluidsim_core/loader.py` & `fluidsim-core-0.7.3/fluidsim_core/loader.py`

 * *Files identical despite different names*

### Comparing `fluidsim-core-0.7.2/fluidsim_core/magic.py` & `fluidsim-core-0.7.3/fluidsim_core/magic.py`

 * *Files identical despite different names*

### Comparing `fluidsim-core-0.7.2/fluidsim_core/output/base.py` & `fluidsim-core-0.7.3/fluidsim_core/output/base.py`

 * *Files identical despite different names*

### Comparing `fluidsim-core-0.7.2/fluidsim_core/output/movies.py` & `fluidsim-core-0.7.3/fluidsim_core/output/movies.py`

 * *Files identical despite different names*

### Comparing `fluidsim-core-0.7.2/fluidsim_core/output/phys_fields.py` & `fluidsim-core-0.7.3/fluidsim_core/output/phys_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,14 @@
         time=None,
         idx_time=None,
         key=None,
         equation=None,
         interpolate_time=True,
         skip_vars=(),
     ):
-
         if time is None and idx_time is None:
             self.update_times()
             time = self.times[-1]
 
         # Assert files are available
         if self.times.size == 0:
             raise FileNotFoundError(
@@ -170,15 +169,14 @@
         if not interpolate_time and time is not None:
             idx, time_closest = self.get_closest_time_file(time)
             return self.get_field_to_plot(
                 idx_time=idx, key=key, equation=equation, skip_vars=skip_vars
             )
 
         if interpolate_time and time is not None:
-
             idx_closest, time_closest = self.get_closest_time_file(time)
 
             if math.isclose(time, time_closest) or self.times.size == 1:
                 return self.get_field_to_plot(
                     idx_time=idx_closest,
                     key=key,
                     equation=equation,
```

### Comparing `fluidsim-core-0.7.2/fluidsim_core/output/phys_fields_snek5000.py` & `fluidsim-core-0.7.3/fluidsim_core/output/phys_fields_snek5000.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,20 +11,18 @@
 
 from fluidsim_core.output.phys_fields import PhysFieldsABC
 from fluidsim_core.output.movies import MoviesBasePhysFieldsHexa
 from fluidsim_core.hexa_files import SetOfPhysFieldFiles
 
 
 class PhysFields4Snek5000(PhysFieldsABC):
-
     _cls_movies = MoviesBasePhysFieldsHexa
     _cls_set_of_files = SetOfPhysFieldFiles
 
     def __init__(self, output=None):
-
         self.output = output
         self.params = output.params
 
         self.set_of_phys_files = self._cls_set_of_files(output=output)
         self.plot_hexa = self.set_of_phys_files.plot_hexa
         self.plot_hexa_stat = partial(
             self.set_of_phys_files.plot_hexa, prefix="sts"
@@ -81,15 +79,14 @@
             raise ValueError("cannot get anything from the state for this solver")
         return self.set_of_phys_files.get_vector_for_plot(
             time, self._equation, skip_vars=skip_vars
         )
 
     @lru_cache(maxsize=None)
     def _get_axis_data(self, equation):
-
         (
             letter_x_axis,
             letter_y_axis,
         ) = self.set_of_phys_files.get_letters_axes_from_equation(equation)
 
         hexa_x, _ = self.get_field_to_plot(
             idx_time=0, key=letter_x_axis, equation=equation
```

### Comparing `fluidsim-core-0.7.2/fluidsim_core/output/remaining_clock_time.py` & `fluidsim-core-0.7.3/fluidsim_core/output/remaining_clock_time.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,23 @@
 import numpy as np
 import matplotlib.pyplot as plt
 
 
 class RemainingClockTime(metaclass=ABCMeta):
     @abstractmethod
     def _load_times(self):
-        """Load remaining time data."""
+        """Load remaining time data.
+
+        - equation_times
+        - remaining_clock_times
+        - clock_times_per_timestep
+        - equation_time_start
+        - full_clock_time
+
+        """
 
     def plot_clock_times(self):
         """Plot the estimated full clock time and clock time per time step."""
 
         results = self._load_times()
         equation_times = results["equation_times"]
```

### Comparing `fluidsim-core-0.7.2/fluidsim_core/params.py` & `fluidsim-core-0.7.3/fluidsim_core/params.py`

 * *Files identical despite different names*

### Comparing `fluidsim-core-0.7.2/fluidsim_core/scripts/restart.py` & `fluidsim-core-0.7.3/fluidsim_core/scripts/restart.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,14 @@
         return path_file
 
     def main(self):
         """Entry point fluidsim-restart"""
         params, sim = self.restart()
 
         if sim is not None and sim.time_stepping._has_to_stop:
-
             if mpi.rank == 0:
                 # processes with rank 0 exits early with exit code 99 or 0
                 exit_code = 99
                 if (
                     Path(sim.output.path_run) / "IDEMPOTENT_NO_RELAUNCH"
                 ).exists():
                     exit_code = 0
```

### Comparing `fluidsim-core-0.7.2/fluidsim_core/solver.py` & `fluidsim-core-0.7.3/fluidsim_core/solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """The Simulation class API.
 
 .. autoclass:: SimulCore
    :members: _complete_params_with_default, create_default_params, __init__
 
 """
 from abc import ABC, abstractclassmethod, abstractmethod, abstractstaticmethod
-from warnings import warn
 
 from .info import InfoSolverCore, create_info_simul
 from .params import Parameters
 
 
 __all__ = ["SimulCore"]
 
@@ -26,15 +25,15 @@
     @abstractstaticmethod
     def _complete_params_with_default(params):
         """A static method used to complete the *params* container."""
         attribs = {}
         params._set_attribs(attribs)
         #  params._set_doc("""Describe docstrings for params here.""")
 
-    @abstractclassmethod
+    @classmethod
     def create_default_params(cls):
         """Sets an ``info_solver`` instance as a class attribute and returns a
         *params* container populated with default values.
 
         """
         cls.info_solver = cls.InfoSolver()
         return cls.Parameters._create_params(cls.info_solver)
```

### Comparing `fluidsim-core-0.7.2/fluidsim_core/tests/conftest.py` & `fluidsim-core-0.7.3/fluidsim_core/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import pymech
 
 name_solver = "testing"
 
 
 @pytest.fixture
 def path_sim(tmp_path):
-
     path_dir = tmp_path / "session_00"
     path_dir.mkdir(exist_ok=True, parents=True)
 
     nx = 2
     ny = 4
     nz = 6
     nx_elem = ny_elem = nz_elem = 2
```

### Comparing `fluidsim-core-0.7.2/fluidsim_core/tests/solver.py` & `fluidsim-core-0.7.3/fluidsim_core/tests/solver.py`

 * *Files identical despite different names*

### Comparing `fluidsim-core-0.7.2/fluidsim_core/tests/test_hexa_files.py` & `fluidsim-core-0.7.3/fluidsim_core/tests/test_hexa_files.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 class MockEvent:
     inaxes: object
     xdata: float
     ydata: float
 
 
 def test_setoffiles(false_output):
-
     output = false_output
     assert output.path_run.exists()
 
     hexa_data_loaded = pymech.readnek(
         output.path_run / f"session_00/{output.name_solver}0.f{1:05d}"
     )
```

### Comparing `fluidsim-core-0.7.2/fluidsim_core/tests/test_solver_with_output.py` & `fluidsim-core-0.7.3/fluidsim_core/tests/test_solver_with_output.py`

 * *Files identical despite different names*

### Comparing `fluidsim-core-0.7.2/fluidsim_core.egg-info/PKG-INFO` & `fluidsim-core-0.7.3/fluidsim_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluidsim-core
-Version: 0.7.2
+Version: 0.7.3
 Summary: Pure-Python core library for FluidSim framework
 Home-page: https://foss.heptapod.net/fluiddyn/fluidsim/-/tree/branch/default/lib
 Author: FluidDyn project
 Author-email: fluiddyn@freelists.org
 License: CeCILL License
 Project-URL: Bug Tracker, https://foss.heptapod.net/fluiddyn/fluidsim/-/issues
 Project-URL: Documentation, https://fluidsim.readthedocs.io/en/latest/generated/fluidsim_core.html
```

### Comparing `fluidsim-core-0.7.2/fluidsim_core.egg-info/SOURCES.txt` & `fluidsim-core-0.7.3/fluidsim_core.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,29 @@
 setup.cfg
 setup.py
 fluidsim_core/__init__.py
 fluidsim_core/_version.py
 fluidsim_core/extend_simul.py
 fluidsim_core/hexa_files.py
 fluidsim_core/info.py
+fluidsim_core/ipy_load.py
 fluidsim_core/loader.py
 fluidsim_core/magic.py
 fluidsim_core/params.py
+fluidsim_core/paths.py
 fluidsim_core/solver.py
 fluidsim_core.egg-info/PKG-INFO
 fluidsim_core.egg-info/SOURCES.txt
 fluidsim_core.egg-info/dependency_links.txt
 fluidsim_core.egg-info/entry_points.txt
 fluidsim_core.egg-info/requires.txt
 fluidsim_core.egg-info/top_level.txt
 fluidsim_core/output/__init__.py
 fluidsim_core/output/base.py
+fluidsim_core/output/dataframe_from_paths.py
 fluidsim_core/output/movies.py
 fluidsim_core/output/phys_fields.py
 fluidsim_core/output/phys_fields_snek5000.py
 fluidsim_core/output/remaining_clock_time.py
 fluidsim_core/scripts/__init__.py
 fluidsim_core/scripts/restart.py
 fluidsim_core/tests/__init__.py
```

### Comparing `fluidsim-core-0.7.2/setup.cfg` & `fluidsim-core-0.7.3/setup.cfg`

 * *Files identical despite different names*

