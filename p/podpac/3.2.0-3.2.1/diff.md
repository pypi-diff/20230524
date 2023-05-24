# Comparing `tmp/podpac-3.2.0.tar.gz` & `tmp/podpac-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podpac-3.2.0.tar", last modified: Wed Dec 28 13:37:33 2022, max compression
+gzip compressed data, was "podpac-3.2.1.tar", last modified: Wed May 24 15:51:49 2023, max compression
```

## Comparing `podpac-3.2.0.tar` & `podpac-3.2.1.tar`

### file list

```diff
@@ -1,152 +1,153 @@
-drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2022-12-28 13:37:34.222326 podpac-3.2.0/
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)    10316 2019-01-26 02:28:54.000000 podpac-3.2.0/LICENSE
--rw-r--r--   0 mpu       (1000) mpu       (1000)     2666 2022-12-28 13:37:34.223325 podpac-3.2.0/PKG-INFO
-drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2022-12-28 13:37:31.211573 podpac-3.2.0/podpac/
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     1568 2020-04-23 02:49:53.000000 podpac-3.2.0/podpac/__init__.py
-drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2022-12-28 13:37:31.345222 podpac-3.2.0/podpac/alglib/
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)      168 2020-04-23 02:49:53.000000 podpac-3.2.0/podpac/alglib/__init__.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     2008 2021-03-16 17:05:15.000000 podpac-3.2.0/podpac/alglib/climatology.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)      824 2022-12-28 12:55:34.000000 podpac-3.2.0/podpac/algorithm.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)      228 2022-12-28 12:55:34.000000 podpac-3.2.0/podpac/authentication.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)      278 2021-04-14 18:01:36.000000 podpac-3.2.0/podpac/compositor.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     1587 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/conftest.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)      505 2022-12-28 12:55:34.000000 podpac-3.2.0/podpac/coordinates.py
-drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2022-12-28 13:37:31.523946 podpac-3.2.0/podpac/core/
--rw-r--r--   0 mpu       (1000) mpu       (1000)      874 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/__init__.py
-drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2022-12-28 13:37:31.732850 podpac-3.2.0/podpac/core/algorithm/
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)        0 2018-03-13 14:02:47.000000 podpac-3.2.0/podpac/core/algorithm/__init__.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     6079 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/algorithm/algorithm.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    12126 2022-12-28 12:55:34.000000 podpac-3.2.0/podpac/core/algorithm/coord_select.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    10228 2022-12-28 12:55:34.000000 podpac-3.2.0/podpac/core/algorithm/generic.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     4443 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/algorithm/reprojection.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    10748 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/algorithm/signal.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    34643 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/algorithm/stats.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     3411 2022-12-28 12:55:34.000000 podpac-3.2.0/podpac/core/algorithm/utility.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     7483 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/authentication.py
-drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2022-12-28 13:37:31.943723 podpac-3.2.0/podpac/core/cache/
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)      351 2021-03-16 17:05:15.000000 podpac-3.2.0/podpac/core/cache/__init__.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    10631 2022-12-28 12:55:34.000000 podpac-3.2.0/podpac/core/cache/cache_ctrl.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     3726 2022-12-28 12:55:34.000000 podpac-3.2.0/podpac/core/cache/cache_store.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     5597 2022-12-28 12:55:34.000000 podpac-3.2.0/podpac/core/cache/disk_cache_store.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    11976 2022-12-28 12:55:34.000000 podpac-3.2.0/podpac/core/cache/file_cache_store.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     8237 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/cache/ram_cache_store.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     9032 2022-12-28 12:55:34.000000 podpac-3.2.0/podpac/core/cache/s3_cache_store.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     2015 2021-03-16 17:05:15.000000 podpac-3.2.0/podpac/core/cache/utils.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     7817 2021-03-16 17:05:15.000000 podpac-3.2.0/podpac/core/common_test_utils.py
-drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2022-12-28 13:37:32.050822 podpac-3.2.0/podpac/core/compositor/
--rw-r--r--   0 mpu       (1000) mpu       (1000)      133 2022-12-28 12:55:34.000000 podpac-3.2.0/podpac/core/compositor/__init__.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    10049 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/compositor/compositor.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     3122 2021-06-02 02:30:11.000000 podpac-3.2.0/podpac/core/compositor/ordered_compositor.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     3770 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/compositor/tile_compositor.py
-drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2022-12-28 13:37:32.354877 podpac-3.2.0/podpac/core/coordinates/
--rw-r--r--   0 mpu       (1000) mpu       (1000)     1065 2022-12-28 12:55:34.000000 podpac-3.2.0/podpac/core/coordinates/__init__.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    12895 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/coordinates/affine_coordinates.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    12944 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/coordinates/array_coordinates1d.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     3386 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/coordinates/base_coordinates.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     2975 2021-03-16 17:05:16.000000 podpac-3.2.0/podpac/core/coordinates/cfunctions.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    59801 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/coordinates/coordinates.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    14280 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/coordinates/coordinates1d.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     6943 2022-12-28 12:55:34.000000 podpac-3.2.0/podpac/core/coordinates/group_coordinates.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     8186 2021-04-14 18:01:37.000000 podpac-3.2.0/podpac/core/coordinates/polar_coordinates.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    24180 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/coordinates/stacked_coordinates.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    18949 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/coordinates/uniform_coordinates1d.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)    16775 2021-04-14 18:01:37.000000 podpac-3.2.0/podpac/core/coordinates/utils.py
-drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2022-12-28 13:37:32.664942 podpac-3.2.0/podpac/core/data/
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)        0 2018-03-13 14:02:47.000000 podpac-3.2.0/podpac/core/data/__init__.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     3300 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/data/array_source.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     5969 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/data/csv_source.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     3742 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/data/dataset_source.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    23415 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/data/datasource.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     8765 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/data/file_source.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     4330 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/data/h5py_source.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    16950 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/data/ogc.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     5249 2022-12-28 12:55:34.000000 podpac-3.2.0/podpac/core/data/ogr.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     4835 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/data/pydap_source.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    12782 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/data/rasterio_source.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     4220 2022-12-28 12:55:34.000000 podpac-3.2.0/podpac/core/data/reprojection.py
-drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2022-12-28 13:37:33.065811 podpac-3.2.0/podpac/core/data/test/
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)        0 2018-11-06 18:52:41.000000 podpac-3.2.0/podpac/core/data/test/__init__.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     2409 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/data/test/test_array.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)    11335 2021-04-14 18:01:37.000000 podpac-3.2.0/podpac/core/data/test/test_csv.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     4765 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/data/test/test_dataset.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    25785 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/data/test/test_datasource.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     9898 2021-03-16 17:05:16.000000 podpac-3.2.0/podpac/core/data/test/test_file_source.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     2920 2020-04-23 02:49:53.000000 podpac-3.2.0/podpac/core/data/test/test_h5py.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     3884 2021-06-02 02:30:11.000000 podpac-3.2.0/podpac/core/data/test/test_ogr.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     2950 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/data/test/test_pydap.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     2373 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/data/test/test_rasterio.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     5634 2021-04-14 18:01:37.000000 podpac-3.2.0/podpac/core/data/test/test_reprojected_source.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    25113 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/data/test/test_wcs.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     2797 2022-12-28 12:55:34.000000 podpac-3.2.0/podpac/core/data/test/test_zarr.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     6989 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/data/zarr_source.py
-drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2022-12-28 13:37:33.331069 podpac-3.2.0/podpac/core/interpolation/
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)       69 2021-04-14 18:01:37.000000 podpac-3.2.0/podpac/core/interpolation/__init__.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    12799 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/interpolation/interpolation.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    29770 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/interpolation/interpolation_manager.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)    14366 2021-06-02 02:30:11.000000 podpac-3.2.0/podpac/core/interpolation/interpolator.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    19690 2022-12-28 12:55:35.000000 podpac-3.2.0/podpac/core/interpolation/nearest_neighbor_interpolator.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     2276 2022-12-28 12:55:35.000000 podpac-3.2.0/podpac/core/interpolation/none_interpolator.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     4214 2021-04-14 18:01:37.000000 podpac-3.2.0/podpac/core/interpolation/rasterio_interpolator.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     9837 2021-04-14 18:01:37.000000 podpac-3.2.0/podpac/core/interpolation/scipy_interpolator.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    10184 2022-12-28 12:55:35.000000 podpac-3.2.0/podpac/core/interpolation/selector.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     5504 2022-12-28 13:29:54.000000 podpac-3.2.0/podpac/core/interpolation/xarray_interpolator.py
-drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2022-12-28 13:37:33.457663 podpac-3.2.0/podpac/core/managers/
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)        0 2018-11-06 18:52:41.000000 podpac-3.2.0/podpac/core/managers/__init__.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)   103854 2022-12-28 13:29:55.000000 podpac-3.2.0/podpac/core/managers/aws.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     2272 2021-04-14 18:01:37.000000 podpac-3.2.0/podpac/core/managers/multi_process.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     2906 2021-03-16 17:05:16.000000 podpac-3.2.0/podpac/core/managers/multi_threading.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    18226 2022-12-28 12:55:35.000000 podpac-3.2.0/podpac/core/managers/parallel.py
-drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2022-12-28 13:37:33.617995 podpac-3.2.0/podpac/core/managers/test/
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)        0 2020-04-21 19:09:56.000000 podpac-3.2.0/podpac/core/managers/test/__init__.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)       64 2020-04-23 02:49:53.000000 podpac-3.2.0/podpac/core/managers/test/test_aws.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     1642 2021-04-14 18:01:37.000000 podpac-3.2.0/podpac/core/managers/test/test_multiprocess.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     2818 2020-04-23 02:49:53.000000 podpac-3.2.0/podpac/core/managers/test/test_multithreading.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     5209 2021-04-14 18:01:37.000000 podpac-3.2.0/podpac/core/managers/test/test_parallel.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    46616 2022-12-28 13:29:55.000000 podpac-3.2.0/podpac/core/node.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)    15492 2021-06-04 18:04:45.000000 podpac-3.2.0/podpac/core/settings.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     6870 2022-12-28 13:29:55.000000 podpac-3.2.0/podpac/core/style.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    26263 2022-12-28 12:55:35.000000 podpac-3.2.0/podpac/core/units.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    20537 2022-12-28 13:29:55.000000 podpac-3.2.0/podpac/core/utils.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)      720 2021-06-02 02:30:11.000000 podpac-3.2.0/podpac/data.py
-drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2022-12-28 13:37:33.936693 podpac-3.2.0/podpac/datalib/
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)      813 2021-09-09 12:57:17.000000 podpac-3.2.0/podpac/datalib/__init__.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    15156 2022-12-28 13:29:55.000000 podpac-3.2.0/podpac/datalib/cosmos_stations.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     3906 2022-12-28 13:29:55.000000 podpac-3.2.0/podpac/datalib/drought_monitor.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    21487 2022-12-28 12:55:35.000000 podpac-3.2.0/podpac/datalib/egi.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     4061 2022-12-28 13:29:55.000000 podpac-3.2.0/podpac/datalib/gfs.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     7275 2022-12-28 12:55:35.000000 podpac-3.2.0/podpac/datalib/intake_catalog.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    13517 2022-12-28 13:29:55.000000 podpac-3.2.0/podpac/datalib/modis_pds.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     5540 2021-09-09 12:57:17.000000 podpac-3.2.0/podpac/datalib/nasaCMR.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    12177 2022-12-28 13:29:55.000000 podpac-3.2.0/podpac/datalib/satutils.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    10444 2022-12-28 13:29:55.000000 podpac-3.2.0/podpac/datalib/smap_egi.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     2732 2022-12-28 13:29:55.000000 podpac-3.2.0/podpac/datalib/soilgrids.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)    22144 2021-09-09 12:57:17.000000 podpac-3.2.0/podpac/datalib/soilscape.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    15658 2022-12-28 13:29:55.000000 podpac-3.2.0/podpac/datalib/terraintiles.py
-drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2022-12-28 13:37:34.204319 podpac-3.2.0/podpac/datalib/test/
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)        0 2021-04-14 18:01:37.000000 podpac-3.2.0/podpac/datalib/test/__init__.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     1677 2021-04-14 18:01:37.000000 podpac-3.2.0/podpac/datalib/test/coordinates_for_tests.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     1232 2021-04-14 18:01:37.000000 podpac-3.2.0/podpac/datalib/test/test_cosmos.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     2235 2021-06-02 02:30:11.000000 podpac-3.2.0/podpac/datalib/test/test_gfs.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)      504 2021-04-14 18:01:37.000000 podpac-3.2.0/podpac/datalib/test/test_modis.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     1215 2021-04-14 18:01:37.000000 podpac-3.2.0/podpac/datalib/test/test_satutils.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)      532 2021-04-14 18:01:37.000000 podpac-3.2.0/podpac/datalib/test/test_smap_egi.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)      504 2021-04-14 18:01:37.000000 podpac-3.2.0/podpac/datalib/test/test_soilgrids.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     1778 2021-04-14 18:01:37.000000 podpac-3.2.0/podpac/datalib/test/test_soilscape.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     1293 2021-04-14 18:01:37.000000 podpac-3.2.0/podpac/datalib/test/test_terrain_tiles.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)      848 2021-04-14 18:01:37.000000 podpac-3.2.0/podpac/datalib/test/test_weathercitizen.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)    21178 2022-12-28 12:55:35.000000 podpac-3.2.0/podpac/datalib/weathercitizen.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)    18325 2021-09-09 12:57:17.000000 podpac-3.2.0/podpac/datalib/weathercitizen_sensorburst_pb2.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)      610 2021-04-14 18:01:37.000000 podpac-3.2.0/podpac/interpolators.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)      336 2020-04-23 02:49:54.000000 podpac-3.2.0/podpac/managers.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)      156 2020-04-23 02:49:54.000000 podpac-3.2.0/podpac/style.py
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)      300 2021-03-16 17:05:16.000000 podpac-3.2.0/podpac/utils.py
--rw-r--r--   0 mpu       (1000) mpu       (1000)     1884 2022-12-28 13:29:55.000000 podpac-3.2.0/podpac/version.py
-drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2022-12-28 13:37:31.302906 podpac-3.2.0/podpac.egg-info/
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     2666 2022-12-28 13:37:29.000000 podpac-3.2.0/podpac.egg-info/PKG-INFO
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     4494 2022-12-28 13:37:30.000000 podpac-3.2.0/podpac.egg-info/SOURCES.txt
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)        1 2022-12-28 13:37:29.000000 podpac-3.2.0/podpac.egg-info/dependency_links.txt
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)     1575 2022-12-28 13:37:29.000000 podpac-3.2.0/podpac.egg-info/requires.txt
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)        7 2022-12-28 13:37:29.000000 podpac-3.2.0/podpac.egg-info/top_level.txt
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)       33 2020-04-23 02:49:54.000000 podpac-3.2.0/pyproject.toml
--rwxrwxrwx   0 mpu       (1000) mpu       (1000)      754 2022-12-28 13:37:34.236327 podpac-3.2.0/setup.cfg
--rw-r--r--   0 mpu       (1000) mpu       (1000)     3714 2022-12-28 12:55:35.000000 podpac-3.2.0/setup.py
+drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2023-05-24 15:51:49.261877 podpac-3.2.1/
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)    10316 2019-01-26 02:28:54.000000 podpac-3.2.1/LICENSE
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     2666 2023-05-24 15:51:49.263841 podpac-3.2.1/PKG-INFO
+drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2023-05-24 15:51:45.981276 podpac-3.2.1/podpac/
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)     1568 2020-04-23 02:49:53.000000 podpac-3.2.1/podpac/__init__.py
+drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2023-05-24 15:51:46.118467 podpac-3.2.1/podpac/alglib/
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)      168 2020-04-23 02:49:53.000000 podpac-3.2.1/podpac/alglib/__init__.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)     2008 2021-03-16 17:05:15.000000 podpac-3.2.1/podpac/alglib/climatology.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)      824 2022-12-28 12:55:34.000000 podpac-3.2.1/podpac/algorithm.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)      228 2022-12-28 12:55:34.000000 podpac-3.2.1/podpac/authentication.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)      278 2023-04-27 14:44:06.000000 podpac-3.2.1/podpac/compositor.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     1587 2022-12-28 13:29:54.000000 podpac-3.2.1/podpac/conftest.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)      505 2022-12-28 12:55:34.000000 podpac-3.2.1/podpac/coordinates.py
+drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2023-05-24 15:51:46.315980 podpac-3.2.1/podpac/core/
+-rw-r--r--   0 mpu       (1000) mpu       (1000)      874 2022-12-28 13:29:54.000000 podpac-3.2.1/podpac/core/__init__.py
+drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2023-05-24 15:51:46.540283 podpac-3.2.1/podpac/core/algorithm/
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)        0 2018-03-13 14:02:47.000000 podpac-3.2.1/podpac/core/algorithm/__init__.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     6079 2022-12-28 13:29:54.000000 podpac-3.2.1/podpac/core/algorithm/algorithm.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    12126 2022-12-28 12:55:34.000000 podpac-3.2.1/podpac/core/algorithm/coord_select.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    10228 2022-12-28 12:55:34.000000 podpac-3.2.1/podpac/core/algorithm/generic.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     4443 2022-12-28 13:29:54.000000 podpac-3.2.1/podpac/core/algorithm/reprojection.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    10748 2022-12-28 13:29:54.000000 podpac-3.2.1/podpac/core/algorithm/signal.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    34643 2022-12-28 13:29:54.000000 podpac-3.2.1/podpac/core/algorithm/stats.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     3411 2022-12-28 12:55:34.000000 podpac-3.2.1/podpac/core/algorithm/utility.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     7483 2022-12-28 13:29:54.000000 podpac-3.2.1/podpac/core/authentication.py
+drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2023-05-24 15:51:46.760517 podpac-3.2.1/podpac/core/cache/
+-rw-r--r--   0 mpu       (1000) mpu       (1000)      351 2023-04-27 14:44:06.000000 podpac-3.2.1/podpac/core/cache/__init__.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    10631 2023-04-27 14:44:06.000000 podpac-3.2.1/podpac/core/cache/cache_ctrl.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     3726 2022-12-28 12:55:34.000000 podpac-3.2.1/podpac/core/cache/cache_store.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     5597 2022-12-28 12:55:34.000000 podpac-3.2.1/podpac/core/cache/disk_cache_store.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    11976 2022-12-28 12:55:34.000000 podpac-3.2.1/podpac/core/cache/file_cache_store.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     8237 2022-12-28 13:29:54.000000 podpac-3.2.1/podpac/core/cache/ram_cache_store.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     9032 2022-12-28 12:55:34.000000 podpac-3.2.1/podpac/core/cache/s3_cache_store.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)     2015 2021-03-16 17:05:15.000000 podpac-3.2.1/podpac/core/cache/utils.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)     7817 2021-03-16 17:05:15.000000 podpac-3.2.1/podpac/core/common_test_utils.py
+drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2023-05-24 15:51:46.870291 podpac-3.2.1/podpac/core/compositor/
+-rw-r--r--   0 mpu       (1000) mpu       (1000)      133 2022-12-28 12:55:34.000000 podpac-3.2.1/podpac/core/compositor/__init__.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    10049 2022-12-28 13:29:54.000000 podpac-3.2.1/podpac/core/compositor/compositor.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)     3122 2021-06-02 02:30:11.000000 podpac-3.2.1/podpac/core/compositor/ordered_compositor.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     3770 2023-04-27 14:44:06.000000 podpac-3.2.1/podpac/core/compositor/tile_compositor.py
+drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2023-05-24 15:51:47.204558 podpac-3.2.1/podpac/core/coordinates/
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     1065 2022-12-28 12:55:34.000000 podpac-3.2.1/podpac/core/coordinates/__init__.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    12895 2022-12-28 13:29:54.000000 podpac-3.2.1/podpac/core/coordinates/affine_coordinates.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    12944 2022-12-28 13:29:54.000000 podpac-3.2.1/podpac/core/coordinates/array_coordinates1d.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     3386 2023-05-01 13:05:24.000000 podpac-3.2.1/podpac/core/coordinates/base_coordinates.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)     2975 2021-03-16 17:05:16.000000 podpac-3.2.1/podpac/core/coordinates/cfunctions.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    59801 2023-05-01 13:05:24.000000 podpac-3.2.1/podpac/core/coordinates/coordinates.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    14280 2023-05-01 13:05:24.000000 podpac-3.2.1/podpac/core/coordinates/coordinates1d.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     6943 2022-12-28 12:55:34.000000 podpac-3.2.1/podpac/core/coordinates/group_coordinates.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)     8186 2021-04-14 18:01:37.000000 podpac-3.2.1/podpac/core/coordinates/polar_coordinates.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    24180 2023-05-01 13:05:24.000000 podpac-3.2.1/podpac/core/coordinates/stacked_coordinates.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    18949 2023-05-01 13:05:24.000000 podpac-3.2.1/podpac/core/coordinates/uniform_coordinates1d.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    16775 2023-05-01 13:05:24.000000 podpac-3.2.1/podpac/core/coordinates/utils.py
+drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2023-05-24 15:51:47.579738 podpac-3.2.1/podpac/core/data/
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)        0 2018-03-13 14:02:47.000000 podpac-3.2.1/podpac/core/data/__init__.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     3300 2023-04-27 14:44:06.000000 podpac-3.2.1/podpac/core/data/array_source.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     5969 2023-04-27 14:44:06.000000 podpac-3.2.1/podpac/core/data/csv_source.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     3742 2023-04-27 14:44:06.000000 podpac-3.2.1/podpac/core/data/dataset_source.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    23415 2023-04-27 14:44:06.000000 podpac-3.2.1/podpac/core/data/datasource.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     8765 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/core/data/file_source.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     4330 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/core/data/h5py_source.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    16950 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/core/data/ogc.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     5249 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/core/data/ogr.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     4835 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/core/data/pydap_source.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    12782 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/core/data/rasterio_source.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     4220 2022-12-28 12:55:34.000000 podpac-3.2.1/podpac/core/data/reprojection.py
+drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2023-05-24 15:51:48.008036 podpac-3.2.1/podpac/core/data/test/
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)        0 2018-11-06 18:52:41.000000 podpac-3.2.1/podpac/core/data/test/__init__.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     2409 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/core/data/test/test_array.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    11335 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/core/data/test/test_csv.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     4765 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/core/data/test/test_dataset.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    25785 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/core/data/test/test_datasource.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     9898 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/core/data/test/test_file_source.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)     2920 2020-04-23 02:49:53.000000 podpac-3.2.1/podpac/core/data/test/test_h5py.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     3884 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/core/data/test/test_ogr.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     2950 2022-12-28 13:29:54.000000 podpac-3.2.1/podpac/core/data/test/test_pydap.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     2373 2022-12-28 13:29:54.000000 podpac-3.2.1/podpac/core/data/test/test_rasterio.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     5634 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/core/data/test/test_reprojected_source.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    25113 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/core/data/test/test_wcs.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     2797 2022-12-28 12:55:34.000000 podpac-3.2.1/podpac/core/data/test/test_zarr.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     6989 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/core/data/zarr_source.py
+drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2023-05-24 15:51:48.285372 podpac-3.2.1/podpac/core/interpolation/
+-rw-r--r--   0 mpu       (1000) mpu       (1000)       69 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/core/interpolation/__init__.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    12799 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/core/interpolation/interpolation.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    29770 2023-05-01 13:05:24.000000 podpac-3.2.1/podpac/core/interpolation/interpolation_manager.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)    14366 2021-06-02 02:30:11.000000 podpac-3.2.1/podpac/core/interpolation/interpolator.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    20368 2023-05-24 13:05:25.000000 podpac-3.2.1/podpac/core/interpolation/nearest_neighbor_interpolator.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     2276 2022-12-28 12:55:35.000000 podpac-3.2.1/podpac/core/interpolation/none_interpolator.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)     4214 2021-04-14 18:01:37.000000 podpac-3.2.1/podpac/core/interpolation/rasterio_interpolator.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)     9837 2021-04-14 18:01:37.000000 podpac-3.2.1/podpac/core/interpolation/scipy_interpolator.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    10184 2022-12-28 12:55:35.000000 podpac-3.2.1/podpac/core/interpolation/selector.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     5504 2022-12-28 13:29:54.000000 podpac-3.2.1/podpac/core/interpolation/xarray_interpolator.py
+drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2023-05-24 15:51:48.426894 podpac-3.2.1/podpac/core/managers/
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)        0 2018-11-06 18:52:41.000000 podpac-3.2.1/podpac/core/managers/__init__.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)   103854 2022-12-28 13:29:55.000000 podpac-3.2.1/podpac/core/managers/aws.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)     2272 2021-04-14 18:01:37.000000 podpac-3.2.1/podpac/core/managers/multi_process.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)     2906 2021-03-16 17:05:16.000000 podpac-3.2.1/podpac/core/managers/multi_threading.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    18226 2022-12-28 12:55:35.000000 podpac-3.2.1/podpac/core/managers/parallel.py
+drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2023-05-24 15:51:48.588867 podpac-3.2.1/podpac/core/managers/test/
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)        0 2020-04-21 19:09:56.000000 podpac-3.2.1/podpac/core/managers/test/__init__.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)       64 2020-04-23 02:49:53.000000 podpac-3.2.1/podpac/core/managers/test/test_aws.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)     1642 2021-04-14 18:01:37.000000 podpac-3.2.1/podpac/core/managers/test/test_multiprocess.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)     2818 2020-04-23 02:49:53.000000 podpac-3.2.1/podpac/core/managers/test/test_multithreading.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)     5209 2021-04-14 18:01:37.000000 podpac-3.2.1/podpac/core/managers/test/test_parallel.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    46584 2023-05-02 14:24:13.000000 podpac-3.2.1/podpac/core/node.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)    15492 2021-06-04 18:04:45.000000 podpac-3.2.1/podpac/core/settings.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     6870 2022-12-28 13:29:55.000000 podpac-3.2.1/podpac/core/style.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    26263 2022-12-28 12:55:35.000000 podpac-3.2.1/podpac/core/units.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    20537 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/core/utils.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)      720 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/data.py
+drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2023-05-24 15:51:48.945095 podpac-3.2.1/podpac/datalib/
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)      813 2021-09-09 12:57:17.000000 podpac-3.2.1/podpac/datalib/__init__.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    15156 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/datalib/cosmos_stations.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     3906 2022-12-28 13:29:55.000000 podpac-3.2.1/podpac/datalib/drought_monitor.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    21487 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/datalib/egi.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     4061 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/datalib/gfs.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     7275 2022-12-28 12:55:35.000000 podpac-3.2.1/podpac/datalib/intake_catalog.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    13517 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/datalib/modis_pds.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)     5540 2021-09-09 12:57:17.000000 podpac-3.2.1/podpac/datalib/nasaCMR.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    12177 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/datalib/satutils.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    10444 2022-12-28 13:29:55.000000 podpac-3.2.1/podpac/datalib/smap_egi.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     2732 2022-12-28 13:29:55.000000 podpac-3.2.1/podpac/datalib/soilgrids.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    22144 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/datalib/soilscape.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    15658 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/datalib/terraintiles.py
+drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2023-05-24 15:51:49.243194 podpac-3.2.1/podpac/datalib/test/
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)        0 2021-04-14 18:01:37.000000 podpac-3.2.1/podpac/datalib/test/__init__.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)     1677 2021-04-14 18:01:37.000000 podpac-3.2.1/podpac/datalib/test/coordinates_for_tests.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     1232 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/datalib/test/test_cosmos.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)     2235 2021-06-02 02:30:11.000000 podpac-3.2.1/podpac/datalib/test/test_gfs.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)      504 2021-04-14 18:01:37.000000 podpac-3.2.1/podpac/datalib/test/test_modis.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     1215 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/datalib/test/test_satutils.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)      532 2021-04-14 18:01:37.000000 podpac-3.2.1/podpac/datalib/test/test_smap_egi.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)      504 2021-04-14 18:01:37.000000 podpac-3.2.1/podpac/datalib/test/test_soilgrids.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     1778 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/datalib/test/test_soilscape.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)     1293 2021-04-14 18:01:37.000000 podpac-3.2.1/podpac/datalib/test/test_terrain_tiles.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)      848 2021-04-14 18:01:37.000000 podpac-3.2.1/podpac/datalib/test/test_weathercitizen.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)    21178 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/datalib/weathercitizen.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)    18325 2021-09-09 12:57:17.000000 podpac-3.2.1/podpac/datalib/weathercitizen_sensorburst_pb2.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     8596 2023-05-01 13:23:44.000000 podpac-3.2.1/podpac/example_for_stats.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)      610 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/interpolators.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)      336 2020-04-23 02:49:54.000000 podpac-3.2.1/podpac/managers.py
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)      156 2020-04-23 02:49:54.000000 podpac-3.2.1/podpac/style.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)      300 2023-04-27 14:44:07.000000 podpac-3.2.1/podpac/utils.py
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     1884 2023-05-24 13:06:39.000000 podpac-3.2.1/podpac/version.py
+drwxr-xr-x   0 mpu       (1000) mpu       (1000)        0 2023-05-24 15:51:46.072401 podpac-3.2.1/podpac.egg-info/
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)     2666 2023-05-24 15:51:44.000000 podpac-3.2.1/podpac.egg-info/PKG-INFO
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)     4522 2023-05-24 15:51:45.000000 podpac-3.2.1/podpac.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)        1 2023-05-24 15:51:44.000000 podpac-3.2.1/podpac.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)     1578 2023-05-24 15:51:44.000000 podpac-3.2.1/podpac.egg-info/requires.txt
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)        7 2023-05-24 15:51:44.000000 podpac-3.2.1/podpac.egg-info/top_level.txt
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)       33 2020-04-23 02:49:54.000000 podpac-3.2.1/pyproject.toml
+-rwxrwxrwx   0 mpu       (1000) mpu       (1000)      754 2023-05-24 15:51:49.275309 podpac-3.2.1/setup.cfg
+-rw-r--r--   0 mpu       (1000) mpu       (1000)     3715 2023-05-02 12:59:54.000000 podpac-3.2.1/setup.py
```

### Comparing `podpac-3.2.0/LICENSE` & `podpac-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/PKG-INFO` & `podpac-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podpac
-Version: 3.2.0
+Version: 3.2.1
 Summary: Pipeline for Observational Data Processing, Analysis, and Collaboration
 Home-page: https://podpac.org
 Author: Creare
 License: APACHE 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: GIS
```

### Comparing `podpac-3.2.0/podpac/__init__.py` & `podpac-3.2.1/podpac/__init__.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/alglib/climatology.py` & `podpac-3.2.1/podpac/alglib/climatology.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/algorithm.py` & `podpac-3.2.1/podpac/algorithm.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/conftest.py` & `podpac-3.2.1/podpac/conftest.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/__init__.py` & `podpac-3.2.1/podpac/core/__init__.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/algorithm/algorithm.py` & `podpac-3.2.1/podpac/core/algorithm/algorithm.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/algorithm/coord_select.py` & `podpac-3.2.1/podpac/core/algorithm/coord_select.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/algorithm/generic.py` & `podpac-3.2.1/podpac/core/algorithm/generic.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/algorithm/reprojection.py` & `podpac-3.2.1/podpac/core/algorithm/reprojection.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/algorithm/signal.py` & `podpac-3.2.1/podpac/core/algorithm/signal.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/algorithm/stats.py` & `podpac-3.2.1/podpac/core/algorithm/stats.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/algorithm/utility.py` & `podpac-3.2.1/podpac/core/algorithm/utility.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/authentication.py` & `podpac-3.2.1/podpac/core/authentication.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/cache/cache_ctrl.py` & `podpac-3.2.1/podpac/core/cache/cache_ctrl.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/cache/cache_store.py` & `podpac-3.2.1/podpac/core/cache/cache_store.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/cache/disk_cache_store.py` & `podpac-3.2.1/podpac/core/cache/disk_cache_store.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/cache/file_cache_store.py` & `podpac-3.2.1/podpac/core/cache/file_cache_store.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/cache/ram_cache_store.py` & `podpac-3.2.1/podpac/core/cache/ram_cache_store.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/cache/s3_cache_store.py` & `podpac-3.2.1/podpac/core/cache/s3_cache_store.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/cache/utils.py` & `podpac-3.2.1/podpac/core/cache/utils.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/common_test_utils.py` & `podpac-3.2.1/podpac/core/common_test_utils.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/compositor/compositor.py` & `podpac-3.2.1/podpac/core/compositor/compositor.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/compositor/ordered_compositor.py` & `podpac-3.2.1/podpac/core/compositor/ordered_compositor.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/compositor/tile_compositor.py` & `podpac-3.2.1/podpac/core/compositor/tile_compositor.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/coordinates/__init__.py` & `podpac-3.2.1/podpac/core/coordinates/__init__.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/coordinates/affine_coordinates.py` & `podpac-3.2.1/podpac/core/coordinates/affine_coordinates.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/coordinates/array_coordinates1d.py` & `podpac-3.2.1/podpac/core/coordinates/array_coordinates1d.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/coordinates/base_coordinates.py` & `podpac-3.2.1/podpac/core/coordinates/base_coordinates.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/coordinates/cfunctions.py` & `podpac-3.2.1/podpac/core/coordinates/cfunctions.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/coordinates/coordinates.py` & `podpac-3.2.1/podpac/core/coordinates/coordinates.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/coordinates/coordinates1d.py` & `podpac-3.2.1/podpac/core/coordinates/coordinates1d.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/coordinates/group_coordinates.py` & `podpac-3.2.1/podpac/core/coordinates/group_coordinates.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/coordinates/polar_coordinates.py` & `podpac-3.2.1/podpac/core/coordinates/polar_coordinates.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/coordinates/stacked_coordinates.py` & `podpac-3.2.1/podpac/core/coordinates/stacked_coordinates.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/coordinates/uniform_coordinates1d.py` & `podpac-3.2.1/podpac/core/coordinates/uniform_coordinates1d.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/coordinates/utils.py` & `podpac-3.2.1/podpac/core/coordinates/utils.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/data/array_source.py` & `podpac-3.2.1/podpac/core/data/array_source.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/data/csv_source.py` & `podpac-3.2.1/podpac/core/data/csv_source.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/data/dataset_source.py` & `podpac-3.2.1/podpac/core/data/dataset_source.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/data/datasource.py` & `podpac-3.2.1/podpac/core/data/datasource.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/data/file_source.py` & `podpac-3.2.1/podpac/core/data/file_source.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/data/h5py_source.py` & `podpac-3.2.1/podpac/core/data/h5py_source.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/data/ogc.py` & `podpac-3.2.1/podpac/core/data/ogc.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/data/ogr.py` & `podpac-3.2.1/podpac/core/data/ogr.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/data/pydap_source.py` & `podpac-3.2.1/podpac/core/data/pydap_source.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/data/rasterio_source.py` & `podpac-3.2.1/podpac/core/data/rasterio_source.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/data/reprojection.py` & `podpac-3.2.1/podpac/core/data/reprojection.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/data/test/test_array.py` & `podpac-3.2.1/podpac/core/data/test/test_array.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/data/test/test_csv.py` & `podpac-3.2.1/podpac/core/data/test/test_csv.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/data/test/test_dataset.py` & `podpac-3.2.1/podpac/core/data/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/data/test/test_datasource.py` & `podpac-3.2.1/podpac/core/data/test/test_datasource.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/data/test/test_file_source.py` & `podpac-3.2.1/podpac/core/data/test/test_file_source.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/data/test/test_h5py.py` & `podpac-3.2.1/podpac/core/data/test/test_h5py.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/data/test/test_ogr.py` & `podpac-3.2.1/podpac/core/data/test/test_ogr.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/data/test/test_pydap.py` & `podpac-3.2.1/podpac/core/data/test/test_pydap.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/data/test/test_rasterio.py` & `podpac-3.2.1/podpac/core/data/test/test_rasterio.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/data/test/test_reprojected_source.py` & `podpac-3.2.1/podpac/core/data/test/test_reprojected_source.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/data/test/test_wcs.py` & `podpac-3.2.1/podpac/core/data/test/test_wcs.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/data/test/test_zarr.py` & `podpac-3.2.1/podpac/core/data/test/test_zarr.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/data/zarr_source.py` & `podpac-3.2.1/podpac/core/data/zarr_source.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/interpolation/interpolation.py` & `podpac-3.2.1/podpac/core/interpolation/interpolation.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/interpolation/interpolation_manager.py` & `podpac-3.2.1/podpac/core/interpolation/interpolation_manager.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/interpolation/interpolator.py` & `podpac-3.2.1/podpac/core/interpolation/interpolator.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/interpolation/nearest_neighbor_interpolator.py` & `podpac-3.2.1/podpac/core/interpolation/nearest_neighbor_interpolator.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     """
 
     dims_supported = ["lat", "lon", "alt", "time"]
     methods_supported = ["nearest"]
 
     # defined at instantiation
     method = tl.Unicode(default_value="nearest")
+    ambiguous_rounding = tl.Enum(["-infinity", "+infinity", "unbiased"], default_value="-infinity")
     spatial_tolerance = tl.Float(default_value=np.inf, allow_none=True)
     time_tolerance = tl.Union([tl.Unicode(), tl.Instance(np.timedelta64, allow_none=True)])
     alt_tolerance = tl.Float(default_value=np.inf, allow_none=True)
 
     # spatial_scale only applies when the source is stacked with time or alt. The supplied value will be assigned a distance of "1'"
     spatial_scale = tl.Float(default_value=1, allow_none=True)
     # time_scale only applies when the source is stacked with lat, lon, or alt. The supplied value will be assigned a distance of "1'"
@@ -293,14 +294,25 @@
         return index
 
     def _get_uniform_index(self, dim, source, request, bounds=None):
         tol = self._get_tol(dim, source, request)
 
         index = (request.coordinates - source.start) / source.step
         rindex = np.around(index).astype(int)
+        if self.ambiguous_rounding == "-infinity":
+            # Find all the 0.5 and 1.5's that were rounded to even numbers, and make sure they all round down
+            I = (index % 0.5) == 0
+            rindex[I] = np.floor(index[I])
+        elif self.ambiguous_rounding == "+infinity":
+            # Find all the 0.5 and 1.5's that were rounded to even numbers, and make sure they all round down
+            I = (index % 0.5) == 0
+            rindex[I] = np.ceil(index[I])
+        else: # "unbiased", that's the default np.around behavior, so do nothing
+            pass
+
         stop_ind = int(source.size)
         if self.respect_bounds:
             rindex[(rindex < 0) | (rindex >= stop_ind)] = -1
         else:
             rindex = np.clip(rindex, 0, stop_ind - 1)
         if tol and tol != np.inf:
             if dim == "time":
```

### Comparing `podpac-3.2.0/podpac/core/interpolation/none_interpolator.py` & `podpac-3.2.1/podpac/core/interpolation/none_interpolator.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/interpolation/rasterio_interpolator.py` & `podpac-3.2.1/podpac/core/interpolation/rasterio_interpolator.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/interpolation/scipy_interpolator.py` & `podpac-3.2.1/podpac/core/interpolation/scipy_interpolator.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/interpolation/selector.py` & `podpac-3.2.1/podpac/core/interpolation/selector.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/interpolation/xarray_interpolator.py` & `podpac-3.2.1/podpac/core/interpolation/xarray_interpolator.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/managers/aws.py` & `podpac-3.2.1/podpac/core/managers/aws.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/managers/multi_process.py` & `podpac-3.2.1/podpac/core/managers/multi_process.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/managers/multi_threading.py` & `podpac-3.2.1/podpac/core/managers/multi_threading.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/managers/parallel.py` & `podpac-3.2.1/podpac/core/managers/parallel.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/managers/test/test_multiprocess.py` & `podpac-3.2.1/podpac/core/managers/test/test_multiprocess.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/managers/test/test_multithreading.py` & `podpac-3.2.1/podpac/core/managers/test/test_multithreading.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/managers/test/test_parallel.py` & `podpac-3.2.1/podpac/core/managers/test/test_parallel.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/node.py` & `podpac-3.2.1/podpac/core/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -448,25 +448,22 @@
             Default is None. The time
         alt : float, optional
             Default is None. The altitude location
         crs : str, optional
             Default is None. The CRS of the request.
 
         Returns
+        ---------
         dict
             A dictionary that contains the following for each node:
-            ```
-            {
-                "active": bool,   # If the node is being used or not
-                "value": float,   # The value of the node evaluated at that point
-                "inputs": list,   # List of names of input nodes (based on definition)
-                "name": str,      # node.style.name or self.base_ref if the style name is empty
-                "node_hash": str, # The node's hash
-            }
-            ```
+                * "active": bool,   # If the node is being used or not
+                * "value": float,   # The value of the node evaluated at that point
+                * "inputs": list,   # List of names of input nodes (based on definition)
+                * "name": str,      # node.style.name or self.base_ref if the style name is empty
+                * "node_hash": str, # The node's hash
         """
         return probe_node(self, lat, lon, time, alt, crs)
 
     # -----------------------------------------------------------------------------------------------------------------
     # Serialization
     # -----------------------------------------------------------------------------------------------------------------
```

### Comparing `podpac-3.2.0/podpac/core/settings.py` & `podpac-3.2.1/podpac/core/settings.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/style.py` & `podpac-3.2.1/podpac/core/style.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/units.py` & `podpac-3.2.1/podpac/core/units.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/core/utils.py` & `podpac-3.2.1/podpac/core/utils.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/data.py` & `podpac-3.2.1/podpac/data.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/datalib/__init__.py` & `podpac-3.2.1/podpac/datalib/__init__.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/datalib/cosmos_stations.py` & `podpac-3.2.1/podpac/datalib/cosmos_stations.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/datalib/drought_monitor.py` & `podpac-3.2.1/podpac/datalib/drought_monitor.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/datalib/egi.py` & `podpac-3.2.1/podpac/datalib/egi.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/datalib/gfs.py` & `podpac-3.2.1/podpac/datalib/gfs.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/datalib/intake_catalog.py` & `podpac-3.2.1/podpac/datalib/intake_catalog.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/datalib/modis_pds.py` & `podpac-3.2.1/podpac/datalib/modis_pds.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/datalib/nasaCMR.py` & `podpac-3.2.1/podpac/datalib/nasaCMR.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/datalib/satutils.py` & `podpac-3.2.1/podpac/datalib/satutils.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/datalib/smap_egi.py` & `podpac-3.2.1/podpac/datalib/smap_egi.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/datalib/soilgrids.py` & `podpac-3.2.1/podpac/datalib/soilgrids.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/datalib/soilscape.py` & `podpac-3.2.1/podpac/datalib/soilscape.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/datalib/terraintiles.py` & `podpac-3.2.1/podpac/datalib/terraintiles.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/datalib/test/coordinates_for_tests.py` & `podpac-3.2.1/podpac/datalib/test/coordinates_for_tests.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/datalib/test/test_cosmos.py` & `podpac-3.2.1/podpac/datalib/test/test_cosmos.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/datalib/test/test_gfs.py` & `podpac-3.2.1/podpac/datalib/test/test_gfs.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/datalib/test/test_satutils.py` & `podpac-3.2.1/podpac/datalib/test/test_satutils.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/datalib/test/test_smap_egi.py` & `podpac-3.2.1/podpac/datalib/test/test_smap_egi.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/datalib/test/test_soilscape.py` & `podpac-3.2.1/podpac/datalib/test/test_soilscape.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/datalib/test/test_terrain_tiles.py` & `podpac-3.2.1/podpac/datalib/test/test_terrain_tiles.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/datalib/test/test_weathercitizen.py` & `podpac-3.2.1/podpac/datalib/test/test_weathercitizen.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/datalib/weathercitizen.py` & `podpac-3.2.1/podpac/datalib/weathercitizen.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/datalib/weathercitizen_sensorburst_pb2.py` & `podpac-3.2.1/podpac/datalib/weathercitizen_sensorburst_pb2.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/interpolators.py` & `podpac-3.2.1/podpac/interpolators.py`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/podpac/version.py` & `podpac-3.2.1/podpac/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from collections import OrderedDict
 
 ##############
 ## UPDATE VERSION HERE
 ##############
 MAJOR = 3
 MINOR = 2
-HOTFIX = 0
+HOTFIX = 1
 ##############
 
 
 VERSION_INFO = OrderedDict([("MAJOR", MAJOR), ("MINOR", MINOR), ("HOTFIX", HOTFIX)])
 
 VERSION = (VERSION_INFO["MAJOR"], VERSION_INFO["MINOR"], VERSION_INFO["HOTFIX"])
```

### Comparing `podpac-3.2.0/podpac.egg-info/PKG-INFO` & `podpac-3.2.1/podpac.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podpac
-Version: 3.2.0
+Version: 3.2.1
 Summary: Pipeline for Observational Data Processing, Analysis, and Collaboration
 Home-page: https://podpac.org
 Author: Creare
 License: APACHE 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: GIS
```

### Comparing `podpac-3.2.0/podpac.egg-info/SOURCES.txt` & `podpac-3.2.1/podpac.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 podpac/__init__.py
 podpac/algorithm.py
 podpac/authentication.py
 podpac/compositor.py
 podpac/conftest.py
 podpac/coordinates.py
 podpac/data.py
+podpac/example_for_stats.py
 podpac/interpolators.py
 podpac/managers.py
 podpac/style.py
 podpac/utils.py
 podpac/version.py
 podpac.egg-info/PKG-INFO
 podpac.egg-info/SOURCES.txt
```

### Comparing `podpac-3.2.0/podpac.egg-info/requires.txt` & `podpac-3.2.1/podpac.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 sat-search>=0.2
 sat-stac>=0.3
 numpydoc
 pylint>=1.8.2
 pytest-cov>=2.5.1
 pytest-html>=1.7.0
 pytest-remotedata>=0.3.1
-recommonmark>=0.6
+myst-parser>=1.0.0
 coveralls>=1.3
 six>=1.0
 attrs>=17.4.0
 pre_commit>=1
 sphinx<3.0,>=2.3
 sphinx-rtd-theme>=0.4
 sphinx-autobuild>=0.7
@@ -64,15 +64,15 @@
 h5netcdf
 
 [dev]
 pylint>=1.8.2
 pytest-cov>=2.5.1
 pytest-html>=1.7.0
 pytest-remotedata>=0.3.1
-recommonmark>=0.6
+myst-parser>=1.0.0
 coveralls>=1.3
 six>=1.0
 attrs>=17.4.0
 pre_commit>=1
 sphinx<3.0,>=2.3
 sphinx-rtd-theme>=0.4
 sphinx-autobuild>=0.7
@@ -100,15 +100,15 @@
 sat-search>=0.2
 sat-stac>=0.3
 numpydoc
 pylint>=1.8.2
 pytest-cov>=2.5.1
 pytest-html>=1.7.0
 pytest-remotedata>=0.3.1
-recommonmark>=0.6
+myst-parser>=1.0.0
 coveralls>=1.3
 six>=1.0
 attrs>=17.4.0
 pre_commit>=1
 sphinx<3.0,>=2.3
 sphinx-rtd-theme>=0.4
 sphinx-autobuild>=0.7
```

### Comparing `podpac-3.2.0/setup.cfg` & `podpac-3.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `podpac-3.2.0/setup.py` & `podpac-3.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         "numpydoc"
     ],
     "dev": [
         "pylint>=1.8.2",
         "pytest-cov>=2.5.1",
         "pytest-html>=1.7.0",
         "pytest-remotedata>=0.3.1",
-        "recommonmark>=0.6",
+        "myst-parser>=1.0.0",
         "coveralls>=1.3",
         "six>=1.0",
         "attrs>=17.4.0",
         "pre_commit>=1",
     ],
 }
```

