# Comparing `tmp/pytransform3d-3.1.0.tar.gz` & `tmp/pytransform3d-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytransform3d-3.1.0.tar", last modified: Fri Apr 14 18:51:49 2023, max compression
+gzip compressed data, was "pytransform3d-3.2.0.tar", last modified: Wed May 24 12:11:41 2023, max compression
```

## Comparing `pytransform3d-3.1.0.tar` & `pytransform3d-3.2.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-04-14 18:51:49.704778 pytransform3d-3.1.0/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1653 2023-01-12 22:48:31.000000 pytransform3d-3.1.0/LICENSE
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)       58 2023-04-14 18:46:22.000000 pytransform3d-3.1.0/MANIFEST.in
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     9557 2023-04-14 18:51:49.704778 pytransform3d-3.1.0/PKG-INFO
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     8884 2023-04-14 18:46:22.000000 pytransform3d-3.1.0/README.md
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-04-14 18:51:49.696778 pytransform3d-3.1.0/pytransform3d/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)       61 2023-04-14 18:46:28.000000 pytransform3d-3.1.0/pytransform3d/__init__.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    21369 2022-09-17 15:37:15.000000 pytransform3d-3.1.0/pytransform3d/batch_rotations.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2257 2022-03-23 10:33:20.000000 pytransform3d-3.1.0/pytransform3d/batch_rotations.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    11534 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/camera.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1268 2021-05-11 07:46:15.000000 pytransform3d-3.1.0/pytransform3d/camera.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3898 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/coordinates.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      462 2021-08-07 17:17:14.000000 pytransform3d-3.1.0/pytransform3d/coordinates.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    13372 2022-02-11 10:41:03.000000 pytransform3d-3.1.0/pytransform3d/editor.py
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-04-14 18:51:49.700778 pytransform3d-3.1.0/pytransform3d/plot_utils/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      829 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/plot_utils/__init__.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    10111 2022-12-22 19:37:52.000000 pytransform3d-3.1.0/pytransform3d/plot_utils/_artists.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1692 2021-05-11 07:46:15.000000 pytransform3d-3.1.0/pytransform3d/plot_utils/_artists.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2606 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/plot_utils/_layout.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      373 2021-05-11 07:46:15.000000 pytransform3d-3.1.0/pytransform3d/plot_utils/_layout.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    21851 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/plot_utils/_plot_functions.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2656 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/plot_utils/_plot_functions.pyi
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-04-14 18:51:49.700778 pytransform3d-3.1.0/pytransform3d/rotations/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     9185 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/rotations/__init__.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      407 2022-09-17 15:37:15.000000 pytransform3d-3.1.0/pytransform3d/rotations/_constants.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    62000 2023-04-14 18:46:22.000000 pytransform3d-3.1.0/pytransform3d/rotations/_conversions.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     7054 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/rotations/_conversions.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3444 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/rotations/_jacobians.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      356 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/rotations/_jacobians.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     8686 2022-02-11 10:43:44.000000 pytransform3d-3.1.0/pytransform3d/rotations/_plot.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      683 2021-06-06 09:06:24.000000 pytransform3d-3.1.0/pytransform3d/rotations/_plot.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     7380 2023-01-12 22:48:31.000000 pytransform3d-3.1.0/pytransform3d/rotations/_quaternion_operations.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      718 2023-01-12 22:48:31.000000 pytransform3d-3.1.0/pytransform3d/rotations/_quaternion_operations.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5201 2022-02-11 10:41:03.000000 pytransform3d-3.1.0/pytransform3d/rotations/_rotors.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      748 2021-06-06 09:06:24.000000 pytransform3d-3.1.0/pytransform3d/rotations/_rotors.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5045 2022-03-23 10:33:20.000000 pytransform3d-3.1.0/pytransform3d/rotations/_slerp.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      688 2022-03-23 10:33:20.000000 pytransform3d-3.1.0/pytransform3d/rotations/_slerp.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     4236 2022-09-17 15:37:15.000000 pytransform3d-3.1.0/pytransform3d/rotations/_testing.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      393 2022-09-17 15:37:15.000000 pytransform3d-3.1.0/pytransform3d/rotations/_testing.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    16625 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/rotations/_utils.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1736 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/rotations/_utils.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    19380 2022-03-23 10:33:20.000000 pytransform3d-3.1.0/pytransform3d/trajectories.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1618 2022-03-23 10:33:20.000000 pytransform3d-3.1.0/pytransform3d/trajectories.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    19804 2023-02-25 22:06:43.000000 pytransform3d-3.1.0/pytransform3d/transform_manager.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2213 2023-02-11 16:37:10.000000 pytransform3d-3.1.0/pytransform3d/transform_manager.pyi
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-04-14 18:51:49.704778 pytransform3d-3.1.0/pytransform3d/transformations/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3834 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/transformations/__init__.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    32766 2023-04-14 18:46:22.000000 pytransform3d-3.1.0/pytransform3d/transformations/_conversions.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2892 2021-05-23 13:02:30.000000 pytransform3d-3.1.0/pytransform3d/transformations/_conversions.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5298 2022-03-15 09:35:04.000000 pytransform3d-3.1.0/pytransform3d/transformations/_dual_quaternion_operations.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      517 2021-05-11 07:46:15.000000 pytransform3d-3.1.0/pytransform3d/transformations/_dual_quaternion_operations.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     6006 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/transformations/_jacobians.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      360 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/transformations/_jacobians.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5945 2021-05-06 20:16:10.000000 pytransform3d-3.1.0/pytransform3d/transformations/_plot.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      632 2021-05-11 07:46:15.000000 pytransform3d-3.1.0/pytransform3d/transformations/_plot.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3489 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/transformations/_random.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      406 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/transformations/_random.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     6100 2023-02-11 16:37:10.000000 pytransform3d-3.1.0/pytransform3d/transformations/_testing.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      509 2021-05-11 07:46:15.000000 pytransform3d-3.1.0/pytransform3d/transformations/_testing.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     7271 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/transformations/_transform_operations.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      952 2021-05-11 07:46:15.000000 pytransform3d-3.1.0/pytransform3d/transformations/_transform_operations.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    13510 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/transformations/_utils.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      888 2021-05-11 07:46:15.000000 pytransform3d-3.1.0/pytransform3d/transformations/_utils.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    17158 2023-04-14 18:46:22.000000 pytransform3d-3.1.0/pytransform3d/uncertainty.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1320 2023-04-14 18:46:22.000000 pytransform3d-3.1.0/pytransform3d/uncertainty.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    28330 2022-12-22 19:37:52.000000 pytransform3d-3.1.0/pytransform3d/urdf.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3345 2023-02-11 16:37:10.000000 pytransform3d-3.1.0/pytransform3d/urdf.pyi
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-04-14 18:51:49.704778 pytransform3d-3.1.0/pytransform3d/visualizer/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      708 2023-02-11 17:57:50.000000 pytransform3d-3.1.0/pytransform3d/visualizer/__init__.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    37882 2022-12-22 19:37:52.000000 pytransform3d-3.1.0/pytransform3d/visualizer/_artists.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5704 2023-02-11 17:57:50.000000 pytransform3d-3.1.0/pytransform3d/visualizer/_artists.pyi
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    23163 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/visualizer/_figure.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     4235 2023-02-11 17:57:50.000000 pytransform3d-3.1.0/pytransform3d/visualizer/_figure.pyi
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-04-14 18:51:49.700778 pytransform3d-3.1.0/pytransform3d.egg-info/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     9557 2023-04-14 18:51:49.000000 pytransform3d-3.1.0/pytransform3d.egg-info/PKG-INFO
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2620 2023-04-14 18:51:49.000000 pytransform3d-3.1.0/pytransform3d.egg-info/SOURCES.txt
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)        1 2023-04-14 18:51:49.000000 pytransform3d-3.1.0/pytransform3d.egg-info/dependency_links.txt
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      158 2023-04-14 18:51:49.000000 pytransform3d-3.1.0/pytransform3d.egg-info/requires.txt
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)       14 2023-04-14 18:51:49.000000 pytransform3d-3.1.0/pytransform3d.egg-info/top_level.txt
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      272 2023-04-14 18:51:49.704778 pytransform3d-3.1.0/setup.cfg
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1399 2023-02-11 16:37:10.000000 pytransform3d-3.1.0/setup.py
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-05-24 12:11:41.801366 pytransform3d-3.2.0/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1653 2023-01-12 22:48:31.000000 pytransform3d-3.2.0/LICENSE
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)       58 2023-04-14 18:46:22.000000 pytransform3d-3.2.0/MANIFEST.in
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     9557 2023-05-24 12:11:41.801366 pytransform3d-3.2.0/PKG-INFO
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     8884 2023-04-14 18:46:22.000000 pytransform3d-3.2.0/README.md
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-05-24 12:11:41.793366 pytransform3d-3.2.0/pytransform3d/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)       61 2023-05-24 12:06:02.000000 pytransform3d-3.2.0/pytransform3d/__init__.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    21369 2022-09-17 15:37:15.000000 pytransform3d-3.2.0/pytransform3d/batch_rotations.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2257 2022-03-23 10:33:20.000000 pytransform3d-3.2.0/pytransform3d/batch_rotations.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    11534 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/camera.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1268 2021-05-11 07:46:15.000000 pytransform3d-3.2.0/pytransform3d/camera.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3898 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/coordinates.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      462 2021-08-07 17:17:14.000000 pytransform3d-3.2.0/pytransform3d/coordinates.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    13372 2022-02-11 10:41:03.000000 pytransform3d-3.2.0/pytransform3d/editor.py
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-05-24 12:11:41.797366 pytransform3d-3.2.0/pytransform3d/plot_utils/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      829 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/plot_utils/__init__.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    10111 2022-12-22 19:37:52.000000 pytransform3d-3.2.0/pytransform3d/plot_utils/_artists.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1692 2021-05-11 07:46:15.000000 pytransform3d-3.2.0/pytransform3d/plot_utils/_artists.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2606 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/plot_utils/_layout.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      373 2021-05-11 07:46:15.000000 pytransform3d-3.2.0/pytransform3d/plot_utils/_layout.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    21851 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/plot_utils/_plot_functions.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2656 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/plot_utils/_plot_functions.pyi
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-05-24 12:11:41.797366 pytransform3d-3.2.0/pytransform3d/rotations/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     9185 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/rotations/__init__.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      407 2022-09-17 15:37:15.000000 pytransform3d-3.2.0/pytransform3d/rotations/_constants.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    62106 2023-05-22 14:55:27.000000 pytransform3d-3.2.0/pytransform3d/rotations/_conversions.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     7054 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/rotations/_conversions.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3444 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/rotations/_jacobians.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      356 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/rotations/_jacobians.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     8686 2022-02-11 10:43:44.000000 pytransform3d-3.2.0/pytransform3d/rotations/_plot.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      683 2021-06-06 09:06:24.000000 pytransform3d-3.2.0/pytransform3d/rotations/_plot.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     7689 2023-05-22 14:55:27.000000 pytransform3d-3.2.0/pytransform3d/rotations/_quaternion_operations.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      718 2023-01-12 22:48:31.000000 pytransform3d-3.2.0/pytransform3d/rotations/_quaternion_operations.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5201 2022-02-11 10:41:03.000000 pytransform3d-3.2.0/pytransform3d/rotations/_rotors.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      748 2021-06-06 09:06:24.000000 pytransform3d-3.2.0/pytransform3d/rotations/_rotors.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5045 2022-03-23 10:33:20.000000 pytransform3d-3.2.0/pytransform3d/rotations/_slerp.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      688 2022-03-23 10:33:20.000000 pytransform3d-3.2.0/pytransform3d/rotations/_slerp.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     4236 2022-09-17 15:37:15.000000 pytransform3d-3.2.0/pytransform3d/rotations/_testing.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      393 2022-09-17 15:37:15.000000 pytransform3d-3.2.0/pytransform3d/rotations/_testing.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    16625 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/rotations/_utils.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1736 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/rotations/_utils.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    19380 2022-03-23 10:33:20.000000 pytransform3d-3.2.0/pytransform3d/trajectories.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1618 2022-03-23 10:33:20.000000 pytransform3d-3.2.0/pytransform3d/trajectories.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    19965 2023-05-24 12:05:13.000000 pytransform3d-3.2.0/pytransform3d/transform_manager.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2213 2023-02-11 16:37:10.000000 pytransform3d-3.2.0/pytransform3d/transform_manager.pyi
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-05-24 12:11:41.801366 pytransform3d-3.2.0/pytransform3d/transformations/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3834 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/transformations/__init__.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    32766 2023-04-14 18:46:22.000000 pytransform3d-3.2.0/pytransform3d/transformations/_conversions.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2892 2021-05-23 13:02:30.000000 pytransform3d-3.2.0/pytransform3d/transformations/_conversions.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5540 2023-05-22 14:55:27.000000 pytransform3d-3.2.0/pytransform3d/transformations/_dual_quaternion_operations.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      517 2021-05-11 07:46:15.000000 pytransform3d-3.2.0/pytransform3d/transformations/_dual_quaternion_operations.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     6006 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/transformations/_jacobians.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      360 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/transformations/_jacobians.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5945 2021-05-06 20:16:10.000000 pytransform3d-3.2.0/pytransform3d/transformations/_plot.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      632 2021-05-11 07:46:15.000000 pytransform3d-3.2.0/pytransform3d/transformations/_plot.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3489 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/transformations/_random.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      406 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/transformations/_random.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     6100 2023-02-11 16:37:10.000000 pytransform3d-3.2.0/pytransform3d/transformations/_testing.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      509 2021-05-11 07:46:15.000000 pytransform3d-3.2.0/pytransform3d/transformations/_testing.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     7271 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/transformations/_transform_operations.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      952 2021-05-11 07:46:15.000000 pytransform3d-3.2.0/pytransform3d/transformations/_transform_operations.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    13510 2023-04-03 19:11:52.000000 pytransform3d-3.2.0/pytransform3d/transformations/_utils.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      888 2021-05-11 07:46:15.000000 pytransform3d-3.2.0/pytransform3d/transformations/_utils.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    17158 2023-04-14 18:46:22.000000 pytransform3d-3.2.0/pytransform3d/uncertainty.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1320 2023-04-14 18:46:22.000000 pytransform3d-3.2.0/pytransform3d/uncertainty.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    28330 2022-12-22 19:37:52.000000 pytransform3d-3.2.0/pytransform3d/urdf.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3345 2023-02-11 16:37:10.000000 pytransform3d-3.2.0/pytransform3d/urdf.pyi
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-05-24 12:11:41.801366 pytransform3d-3.2.0/pytransform3d/visualizer/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      708 2023-02-11 17:57:50.000000 pytransform3d-3.2.0/pytransform3d/visualizer/__init__.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    37882 2023-04-15 17:56:14.000000 pytransform3d-3.2.0/pytransform3d/visualizer/_artists.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5704 2023-04-15 17:56:14.000000 pytransform3d-3.2.0/pytransform3d/visualizer/_artists.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    23163 2023-04-15 17:56:14.000000 pytransform3d-3.2.0/pytransform3d/visualizer/_figure.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     4235 2023-04-15 17:56:14.000000 pytransform3d-3.2.0/pytransform3d/visualizer/_figure.pyi
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-05-24 12:11:41.793366 pytransform3d-3.2.0/pytransform3d.egg-info/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     9557 2023-05-24 12:11:41.000000 pytransform3d-3.2.0/pytransform3d.egg-info/PKG-INFO
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2620 2023-05-24 12:11:41.000000 pytransform3d-3.2.0/pytransform3d.egg-info/SOURCES.txt
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)        1 2023-05-24 12:11:41.000000 pytransform3d-3.2.0/pytransform3d.egg-info/dependency_links.txt
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      158 2023-05-24 12:11:41.000000 pytransform3d-3.2.0/pytransform3d.egg-info/requires.txt
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)       14 2023-05-24 12:11:41.000000 pytransform3d-3.2.0/pytransform3d.egg-info/top_level.txt
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      272 2023-05-24 12:11:41.801366 pytransform3d-3.2.0/setup.cfg
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1399 2023-02-11 16:37:10.000000 pytransform3d-3.2.0/setup.py
```

### Comparing `pytransform3d-3.1.0/LICENSE` & `pytransform3d-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/PKG-INFO` & `pytransform3d-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytransform3d
-Version: 3.1.0
+Version: 3.2.0
 Summary: 3D transformations for Python
 Home-page: https://github.com/dfki-ric/pytransform3d
 Author: Alexander Fabisch
 Author-email: afabisch@googlemail.com
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytransform3d-3.1.0/README.md` & `pytransform3d-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/batch_rotations.py` & `pytransform3d-3.2.0/pytransform3d/batch_rotations.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/batch_rotations.pyi` & `pytransform3d-3.2.0/pytransform3d/batch_rotations.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/camera.py` & `pytransform3d-3.2.0/pytransform3d/camera.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/camera.pyi` & `pytransform3d-3.2.0/pytransform3d/camera.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/coordinates.py` & `pytransform3d-3.2.0/pytransform3d/coordinates.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/editor.py` & `pytransform3d-3.2.0/pytransform3d/editor.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/plot_utils/__init__.py` & `pytransform3d-3.2.0/pytransform3d/plot_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/plot_utils/_artists.py` & `pytransform3d-3.2.0/pytransform3d/plot_utils/_artists.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/plot_utils/_artists.pyi` & `pytransform3d-3.2.0/pytransform3d/plot_utils/_artists.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/plot_utils/_layout.py` & `pytransform3d-3.2.0/pytransform3d/plot_utils/_layout.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/plot_utils/_plot_functions.py` & `pytransform3d-3.2.0/pytransform3d/plot_utils/_plot_functions.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/plot_utils/_plot_functions.pyi` & `pytransform3d-3.2.0/pytransform3d/plot_utils/_plot_functions.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/rotations/__init__.py` & `pytransform3d-3.2.0/pytransform3d/rotations/__init__.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/rotations/_conversions.py` & `pytransform3d-3.2.0/pytransform3d/rotations/_conversions.py`

 * *Files 0% similar despite different names*

```diff
@@ -987,16 +987,18 @@
 
     # Step 3
     # - Equation 8
     CDCT = np.dot(np.dot(C, D), C.T)
     O = np.dot(CDCT, active_matrix_from_angle(0, lmbda).T)
 
     # Step 4
+    # Fix numerical issue if O_22 is slightly out of range of arccos
+    O_22 = max(min(O[2, 2], 1.0), -1.0)
     # - Equation 10a
-    beta = lmbda + np.arccos(O[2, 2])
+    beta = lmbda + np.arccos(O_22)
 
     safe1 = abs(beta - lmbda) >= np.finfo(float).eps
     safe2 = abs(beta - lmbda - np.pi) >= np.finfo(float).eps
     if safe1 and safe2:  # Default case, no gimbal lock
         # Step 5
         # - Equation 10b
         alpha = np.arctan2(O[0, 2], -O[1, 2])
```

### Comparing `pytransform3d-3.1.0/pytransform3d/rotations/_conversions.pyi` & `pytransform3d-3.2.0/pytransform3d/rotations/_conversions.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/rotations/_jacobians.py` & `pytransform3d-3.2.0/pytransform3d/rotations/_jacobians.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/rotations/_plot.py` & `pytransform3d-3.2.0/pytransform3d/rotations/_plot.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/rotations/_plot.pyi` & `pytransform3d-3.2.0/pytransform3d/rotations/_plot.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/rotations/_quaternion_operations.py` & `pytransform3d-3.2.0/pytransform3d/rotations/_quaternion_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,25 @@
     quaternion_from_compact_axis_angle, compact_axis_angle_from_quaternion,
     axis_angle_from_quaternion, quaternion_from_angle, check_axis_index)
 
 
 def quaternion_integrate(Qd, q0=np.array([1.0, 0.0, 0.0, 0.0]), dt=1.0):
     """Integrate angular velocities to quaternions.
 
+     Angular velocities are given in global frame and will be left-multiplied
+     to the initial or previous orientation respectively.
+
     Parameters
     ----------
     Qd : array-like, shape (n_steps, 3)
         Angular velocities in a compact axis-angle representation. Each angular
         velocity represents the rotational offset after one unit of time.
 
     q0 : array-like, shape (4,), optional (default: [1, 0, 0, 0])
-        Unit quaternion to represent initial rotation: (w, x, y, z)
+        Unit quaternion to represent initial orientation: (w, x, y, z)
 
     dt : float, optional (default: 1)
         Time interval between steps.
 
     Returns
     -------
     Q : array-like, shape (n_steps, 4)
@@ -57,14 +60,17 @@
         interval afterwards.
 
     Returns
     -------
     A : array-like, shape (n_steps, 3)
         Angular velocities in a compact axis-angle representation. Each angular
         velocity represents the rotational offset after one unit of time.
+        Angular velocities are given in global frame and will be
+        left-multiplied during integration to the initial or previous
+        orientation respectively.
     """
     Q = check_quaternions(Q)
     Qd = np.empty((len(Q), 3))
     Qd[0] = compact_axis_angle_from_quaternion(
         concatenate_quaternions(Q[1], q_conj(Q[0]))) / dt
     for t in range(1, len(Q) - 1):
         # divided by two because of central differences
```

### Comparing `pytransform3d-3.1.0/pytransform3d/rotations/_quaternion_operations.pyi` & `pytransform3d-3.2.0/pytransform3d/rotations/_quaternion_operations.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/rotations/_rotors.py` & `pytransform3d-3.2.0/pytransform3d/rotations/_rotors.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/rotations/_rotors.pyi` & `pytransform3d-3.2.0/pytransform3d/rotations/_rotors.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/rotations/_slerp.py` & `pytransform3d-3.2.0/pytransform3d/rotations/_slerp.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/rotations/_slerp.pyi` & `pytransform3d-3.2.0/pytransform3d/rotations/_slerp.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/rotations/_testing.py` & `pytransform3d-3.2.0/pytransform3d/rotations/_testing.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/rotations/_utils.py` & `pytransform3d-3.2.0/pytransform3d/rotations/_utils.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/rotations/_utils.pyi` & `pytransform3d-3.2.0/pytransform3d/rotations/_utils.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/trajectories.py` & `pytransform3d-3.2.0/pytransform3d/trajectories.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/trajectories.pyi` & `pytransform3d-3.2.0/pytransform3d/trajectories.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/transform_manager.py` & `pytransform3d-3.2.0/pytransform3d/transform_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,17 @@
             This object for chaining
         """
         transform_key = (from_frame, to_frame)
         if transform_key in self.transforms:
             del self.transforms[transform_key]
             ij_index = self.transform_to_ij_index[transform_key]
             del self.transform_to_ij_index[transform_key]
+            self.transform_to_ij_index = dict(
+                (k, v if v < ij_index else v - 1)
+                for k, v in self.transform_to_ij_index.items())
             del self.i[ij_index]
             del self.j[ij_index]
             self._recompute_shortest_path()
         return self
 
     def _recompute_shortest_path(self):
         n_nodes = len(self.nodes)
```

### Comparing `pytransform3d-3.1.0/pytransform3d/transform_manager.pyi` & `pytransform3d-3.2.0/pytransform3d/transform_manager.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/transformations/__init__.py` & `pytransform3d-3.2.0/pytransform3d/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/transformations/_conversions.py` & `pytransform3d-3.2.0/pytransform3d/transformations/_conversions.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/transformations/_conversions.pyi` & `pytransform3d-3.2.0/pytransform3d/transformations/_conversions.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/transformations/_dual_quaternion_operations.py` & `pytransform3d-3.2.0/pytransform3d/transformations/_dual_quaternion_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -137,14 +137,20 @@
     t : float in [0, 1]
         Position between start and goal
 
     Returns
     -------
     a : array, shape (8,)
         Interpolated unit dual quaternion: (pw, px, py, pz, qw, qx, qy, qz)
+
+    References
+    ----------
+    Kavan, Collins, O'Sullivan, Zara: Dual Quaternions for Rigid Transformation
+    Blending (2006), Technical report, Trinity College Dublin,
+    https://users.cs.utah.edu/~ladislav/kavan06dual/kavan06dual.pdf
     """
     start = check_dual_quaternion(start)
     end = check_dual_quaternion(end)
     diff = concatenate_dual_quaternions(dq_q_conj(start), end)
     return concatenate_dual_quaternions(start, dual_quaternion_power(diff, t))
```

### Comparing `pytransform3d-3.1.0/pytransform3d/transformations/_dual_quaternion_operations.pyi` & `pytransform3d-3.2.0/pytransform3d/transformations/_dual_quaternion_operations.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/transformations/_jacobians.py` & `pytransform3d-3.2.0/pytransform3d/transformations/_jacobians.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/transformations/_plot.py` & `pytransform3d-3.2.0/pytransform3d/transformations/_plot.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/transformations/_plot.pyi` & `pytransform3d-3.2.0/pytransform3d/transformations/_plot.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/transformations/_random.py` & `pytransform3d-3.2.0/pytransform3d/transformations/_random.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/transformations/_testing.py` & `pytransform3d-3.2.0/pytransform3d/transformations/_testing.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/transformations/_transform_operations.py` & `pytransform3d-3.2.0/pytransform3d/transformations/_transform_operations.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/transformations/_transform_operations.pyi` & `pytransform3d-3.2.0/pytransform3d/transformations/_transform_operations.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/transformations/_utils.py` & `pytransform3d-3.2.0/pytransform3d/transformations/_utils.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/transformations/_utils.pyi` & `pytransform3d-3.2.0/pytransform3d/transformations/_utils.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/uncertainty.py` & `pytransform3d-3.2.0/pytransform3d/uncertainty.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/uncertainty.pyi` & `pytransform3d-3.2.0/pytransform3d/uncertainty.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/urdf.py` & `pytransform3d-3.2.0/pytransform3d/urdf.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/urdf.pyi` & `pytransform3d-3.2.0/pytransform3d/urdf.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/visualizer/__init__.py` & `pytransform3d-3.2.0/pytransform3d/visualizer/__init__.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/visualizer/_artists.py` & `pytransform3d-3.2.0/pytransform3d/visualizer/_artists.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/visualizer/_artists.pyi` & `pytransform3d-3.2.0/pytransform3d/visualizer/_artists.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/visualizer/_figure.py` & `pytransform3d-3.2.0/pytransform3d/visualizer/_figure.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d/visualizer/_figure.pyi` & `pytransform3d-3.2.0/pytransform3d/visualizer/_figure.pyi`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/pytransform3d.egg-info/PKG-INFO` & `pytransform3d-3.2.0/pytransform3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytransform3d
-Version: 3.1.0
+Version: 3.2.0
 Summary: 3D transformations for Python
 Home-page: https://github.com/dfki-ric/pytransform3d
 Author: Alexander Fabisch
 Author-email: afabisch@googlemail.com
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytransform3d-3.1.0/pytransform3d.egg-info/SOURCES.txt` & `pytransform3d-3.2.0/pytransform3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.1.0/setup.py` & `pytransform3d-3.2.0/setup.py`

 * *Files identical despite different names*

