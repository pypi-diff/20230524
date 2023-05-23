# Comparing `tmp/Fiona-1.9b1.tar.gz` & `tmp/Fiona-1.9b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fiona-1.9b1.tar", last modified: Tue Dec 13 20:29:00 2022, max compression
+gzip compressed data, was "Fiona-1.9b2.tar", last modified: Mon Jan 23 03:04:05 2023, max compression
```

## Comparing `Fiona-1.9b1.tar` & `Fiona-1.9b2.tar`

### file list

```diff
@@ -1,182 +1,194 @@
-drwxrwxr-x   0 seangillies  (1000) seangillies  (1000)        0 2022-12-13 20:29:00.959517 Fiona-1.9b1/
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    37129 2022-12-13 18:37:19.000000 Fiona-1.9b1/CHANGES.txt
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      296 2021-12-28 20:35:56.000000 Fiona-1.9b1/CITATION.txt
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2318 2022-10-22 22:23:14.000000 Fiona-1.9b1/CREDITS.txt
-drwxrwxr-x   0 seangillies  (1000) seangillies  (1000)        0 2022-12-13 20:29:00.947517 Fiona-1.9b1/Fiona.egg-info/
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    52952 2022-12-13 20:29:00.000000 Fiona-1.9b1/Fiona.egg-info/PKG-INFO
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4343 2022-12-13 20:29:00.000000 Fiona-1.9b1/Fiona.egg-info/SOURCES.txt
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)        1 2022-12-13 20:29:00.000000 Fiona-1.9b1/Fiona.egg-info/dependency_links.txt
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      435 2022-12-13 20:29:00.000000 Fiona-1.9b1/Fiona.egg-info/entry_points.txt
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      182 2022-12-13 20:29:00.000000 Fiona-1.9b1/Fiona.egg-info/requires.txt
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)        6 2022-12-13 20:29:00.000000 Fiona-1.9b1/Fiona.egg-info/top_level.txt
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1519 2021-12-28 20:35:56.000000 Fiona-1.9b1/LICENSE.txt
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      428 2022-12-08 21:54:23.000000 Fiona-1.9b1/MANIFEST.in
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    52952 2022-12-13 20:29:00.959517 Fiona-1.9b1/PKG-INFO
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    12458 2022-10-22 22:23:14.000000 Fiona-1.9b1/README.rst
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1113 2021-12-28 20:35:56.000000 Fiona-1.9b1/benchmark.py
-drwxrwxr-x   0 seangillies  (1000) seangillies  (1000)        0 2022-12-13 20:29:00.947517 Fiona-1.9b1/docs/
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)       85 2021-12-28 20:35:56.000000 Fiona-1.9b1/docs/README.rst
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    11031 2022-10-22 22:23:14.000000 Fiona-1.9b1/docs/cli.rst
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1941 2021-12-28 20:35:56.000000 Fiona-1.9b1/docs/encoding.txt
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2351 2021-12-28 20:35:56.000000 Fiona-1.9b1/docs/fiona.fio.rst
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2276 2022-10-22 22:23:14.000000 Fiona-1.9b1/docs/fiona.rst
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      275 2021-12-28 20:35:56.000000 Fiona-1.9b1/docs/index.rst
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    49937 2022-12-09 03:08:29.000000 Fiona-1.9b1/docs/manual.rst
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)       52 2021-12-28 20:35:56.000000 Fiona-1.9b1/docs/modules.rst
-drwxrwxr-x   0 seangillies  (1000) seangillies  (1000)        0 2022-12-13 20:29:00.951516 Fiona-1.9b1/fiona/
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    15548 2022-12-13 18:30:17.000000 Fiona-1.9b1/fiona/__init__.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      733 2021-12-28 20:35:56.000000 Fiona-1.9b1/fiona/_cpl.pxd
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      229 2021-12-28 20:35:56.000000 Fiona-1.9b1/fiona/_csl.pxd
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      382 2022-12-09 20:44:04.000000 Fiona-1.9b1/fiona/_env.pxd
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    15260 2022-12-09 20:38:53.000000 Fiona-1.9b1/fiona/_env.pyx
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      375 2022-10-22 22:23:14.000000 Fiona-1.9b1/fiona/_err.pxd
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     7528 2022-12-09 20:44:04.000000 Fiona-1.9b1/fiona/_err.pyx
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4667 2022-12-09 20:44:12.000000 Fiona-1.9b1/fiona/_geometry.pxd
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    14483 2022-12-09 20:44:12.000000 Fiona-1.9b1/fiona/_geometry.pyx
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1260 2022-10-17 14:44:01.000000 Fiona-1.9b1/fiona/_shim.pxd
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     5416 2022-12-09 20:38:53.000000 Fiona-1.9b1/fiona/_shim.pyx
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1204 2022-12-13 18:21:47.000000 Fiona-1.9b1/fiona/_show_versions.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     5203 2022-12-09 20:38:53.000000 Fiona-1.9b1/fiona/_transform.pyx
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    28133 2022-12-13 18:28:09.000000 Fiona-1.9b1/fiona/collection.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      278 2022-10-22 22:23:14.000000 Fiona-1.9b1/fiona/compat.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      218 2022-10-22 22:23:14.000000 Fiona-1.9b1/fiona/crs.pxd
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    36444 2022-12-09 20:38:53.000000 Fiona-1.9b1/fiona/crs.pyx
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    13483 2022-12-13 18:23:20.000000 Fiona-1.9b1/fiona/drvsupport.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      779 2022-10-22 22:23:14.000000 Fiona-1.9b1/fiona/enums.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    21259 2022-12-09 02:46:11.000000 Fiona-1.9b1/fiona/env.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1810 2022-10-22 22:23:14.000000 Fiona-1.9b1/fiona/errors.py
-drwxrwxr-x   0 seangillies  (1000) seangillies  (1000)        0 2022-12-13 20:29:00.947517 Fiona-1.9b1/fiona/fio/
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      510 2021-12-28 20:35:56.000000 Fiona-1.9b1/fiona/fio/__init__.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     3320 2022-10-22 22:23:14.000000 Fiona-1.9b1/fiona/fio/bounds.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2302 2022-10-22 22:23:14.000000 Fiona-1.9b1/fiona/fio/calc.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     3933 2022-12-13 18:35:28.000000 Fiona-1.9b1/fiona/fio/cat.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     8283 2022-10-22 22:23:14.000000 Fiona-1.9b1/fiona/fio/collect.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1169 2022-10-22 22:23:14.000000 Fiona-1.9b1/fiona/fio/distrib.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     7254 2022-10-22 22:23:14.000000 Fiona-1.9b1/fiona/fio/dump.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1483 2022-12-09 02:46:11.000000 Fiona-1.9b1/fiona/fio/env.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1701 2022-12-13 18:34:06.000000 Fiona-1.9b1/fiona/fio/filter.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4071 2022-10-22 22:23:14.000000 Fiona-1.9b1/fiona/fio/helpers.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2661 2022-12-13 18:33:06.000000 Fiona-1.9b1/fiona/fio/info.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1435 2021-12-28 20:35:56.000000 Fiona-1.9b1/fiona/fio/insp.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     3775 2022-10-22 22:23:14.000000 Fiona-1.9b1/fiona/fio/load.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      400 2021-12-28 20:35:56.000000 Fiona-1.9b1/fiona/fio/ls.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1893 2022-12-13 18:34:47.000000 Fiona-1.9b1/fiona/fio/main.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1143 2021-12-28 20:35:56.000000 Fiona-1.9b1/fiona/fio/options.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      785 2022-12-13 18:32:43.000000 Fiona-1.9b1/fiona/fio/rm.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      438 2022-12-09 20:41:24.000000 Fiona-1.9b1/fiona/gdal.pxd
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    31806 2022-12-09 20:44:12.000000 Fiona-1.9b1/fiona/gdal.pxi
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      981 2022-12-13 18:27:04.000000 Fiona-1.9b1/fiona/inspector.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     5390 2022-12-13 18:32:03.000000 Fiona-1.9b1/fiona/io.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      879 2022-10-22 22:23:14.000000 Fiona-1.9b1/fiona/logutils.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     7054 2022-12-13 18:29:09.000000 Fiona-1.9b1/fiona/meta.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    10771 2022-12-09 20:44:12.000000 Fiona-1.9b1/fiona/model.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    74514 2022-12-11 02:59:19.000000 Fiona-1.9b1/fiona/ogrext.pyx
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4735 2022-10-22 22:23:14.000000 Fiona-1.9b1/fiona/path.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     3633 2022-06-02 19:33:29.000000 Fiona-1.9b1/fiona/rfc3339.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2540 2022-12-09 20:38:53.000000 Fiona-1.9b1/fiona/schema.pyx
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    17885 2022-12-13 18:24:19.000000 Fiona-1.9b1/fiona/session.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4266 2022-12-09 02:46:11.000000 Fiona-1.9b1/fiona/transform.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2559 2022-12-13 18:31:34.000000 Fiona-1.9b1/fiona/vfs.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2108 2022-12-08 21:55:00.000000 Fiona-1.9b1/pyproject.toml
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)       90 2022-12-08 21:54:23.000000 Fiona-1.9b1/requirements.txt
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)       38 2022-12-13 20:29:00.959517 Fiona-1.9b1/setup.cfg
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     7104 2022-12-08 21:54:23.000000 Fiona-1.9b1/setup.py
-drwxrwxr-x   0 seangillies  (1000) seangillies  (1000)        0 2022-12-13 20:29:00.955517 Fiona-1.9b1/tests/
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)       44 2022-12-09 02:46:17.000000 Fiona-1.9b1/tests/__init__.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    19350 2022-12-09 02:46:17.000000 Fiona-1.9b1/tests/conftest.py
-drwxrwxr-x   0 seangillies  (1000) seangillies  (1000)        0 2022-12-13 20:29:00.959517 Fiona-1.9b1/tests/data/
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    12922 2022-06-02 19:33:29.000000 Fiona-1.9b1/tests/data/!test.geojson
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      211 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/data/LICENSE.txt
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    15169 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/data/collection-pp.txt
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     6917 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/data/collection.txt
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)       11 2022-06-02 19:33:29.000000 Fiona-1.9b1/tests/data/coutwildrnp.cpg
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    43233 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/data/coutwildrnp.dbf
--rw-r--r--   0 seangillies  (1000) seangillies  (1000)   253952 2022-03-23 17:00:09.000000 Fiona-1.9b1/tests/data/coutwildrnp.gpkg
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)   302617 2022-03-23 17:00:05.000000 Fiona-1.9b1/tests/data/coutwildrnp.json
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      143 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/data/coutwildrnp.prj
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)   109548 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/data/coutwildrnp.shp
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      636 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/data/coutwildrnp.shx
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)   163840 2022-03-23 17:00:13.000000 Fiona-1.9b1/tests/data/coutwildrnp.tar
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)   154006 2022-07-04 02:33:55.000000 Fiona-1.9b1/tests/data/coutwildrnp.zip
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     7559 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/data/curves_line.csv
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)   422857 2022-12-09 23:16:18.000000 Fiona-1.9b1/tests/data/data.zip
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      822 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/data/example.topojson
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)        6 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/data/gre.cpg
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2834 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/data/gre.dbf
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      143 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/data/gre.prj
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     6972 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/data/gre.shp
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      108 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/data/gre.shx
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    12922 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/data/grenada.geojson
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    32218 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/data/issue627.geojson
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    12910 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/data/sequence-pp.txt
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     6872 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/data/sequence.txt
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2460 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/data/test_gpx.gpx
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      251 2022-12-09 20:44:12.000000 Fiona-1.9b1/tests/data/test_tin.csv
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      147 2022-06-02 19:33:29.000000 Fiona-1.9b1/tests/data/test_tin.dbf
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      272 2022-06-02 19:33:29.000000 Fiona-1.9b1/tests/data/test_tin.shp
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      108 2022-06-02 19:33:29.000000 Fiona-1.9b1/tests/data/test_tin.shx
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      287 2022-06-02 19:33:29.000000 Fiona-1.9b1/tests/data/test_tz.geojson
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     3925 2022-06-10 01:31:19.000000 Fiona-1.9b1/tests/test__env.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2776 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_bigint.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1303 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_binary_field.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2688 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_bounds.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     7192 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_bytescollection.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    38747 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_collection.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2424 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_collection_crs.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     5132 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_collection_legacy.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      666 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_compound_crs.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4901 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_crs.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     5006 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_cursor_interruptions.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      459 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/test_curve_geometries.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1861 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_data_paths.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    30721 2022-12-08 20:48:10.000000 Fiona-1.9b1/tests/test_datetime.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      947 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_driver_options.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      921 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/test_drivers.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    11386 2022-12-09 03:08:29.000000 Fiona-1.9b1/tests/test_drvsupport.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1585 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_encoding.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4858 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_env.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     5356 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_feature.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     3024 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_fio_bounds.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1992 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/test_fio_calc.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4273 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_fio_cat.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2655 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/test_fio_collect.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      564 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/test_fio_distrib.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      980 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_fio_dump.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      852 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_fio_filter.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2868 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/test_fio_info.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     5020 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_fio_load.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1784 2022-06-02 19:33:29.000000 Fiona-1.9b1/tests/test_fio_ls.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1786 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_fio_rm.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4269 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_geojson.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4924 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_geometry.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2495 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_geopackage.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    11104 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_http_session.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1148 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_integration.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2157 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/test_layer.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     3473 2022-12-09 02:46:17.000000 Fiona-1.9b1/tests/test_listing.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1922 2022-06-02 19:33:29.000000 Fiona-1.9b1/tests/test_logutils.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    12379 2022-12-11 02:04:04.000000 Fiona-1.9b1/tests/test_memoryfile.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2107 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_meta.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     7898 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_model.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4069 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_multiconxn.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      935 2022-06-02 19:33:29.000000 Fiona-1.9b1/tests/test_non_counting_layer.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1666 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_open.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      600 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/test_profile.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4523 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_props.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      652 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/test_read_drivers.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     3835 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_remove.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      402 2021-12-28 20:35:56.000000 Fiona-1.9b1/tests/test_revolvingdoor.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1966 2022-06-02 19:33:29.000000 Fiona-1.9b1/tests/test_rfc3339.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1819 2022-12-09 20:44:12.000000 Fiona-1.9b1/tests/test_rfc64_tin.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    13826 2022-12-08 18:27:31.000000 Fiona-1.9b1/tests/test_schema.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     7078 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_schema_geom.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     3335 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_session.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     5354 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_slice.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1566 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_subtypes.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1362 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_topojson.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2704 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_transactions.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4084 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_transform.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     5967 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_unicode.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2446 2022-06-02 19:33:29.000000 Fiona-1.9b1/tests/test_version.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     6326 2022-10-22 22:23:14.000000 Fiona-1.9b1/tests/test_vfs.py
--rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4787 2022-12-11 03:02:37.000000 Fiona-1.9b1/tests/test_write.py
+drwxrwxr-x   0 seangillies  (1000) seangillies  (1000)        0 2023-01-23 03:04:05.654907 Fiona-1.9b2/
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    38002 2023-01-22 18:25:10.000000 Fiona-1.9b2/CHANGES.txt
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      296 2021-12-28 20:35:56.000000 Fiona-1.9b2/CITATION.txt
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2318 2022-10-22 22:23:14.000000 Fiona-1.9b2/CREDITS.txt
+drwxrwxr-x   0 seangillies  (1000) seangillies  (1000)        0 2023-01-23 03:04:05.638907 Fiona-1.9b2/Fiona.egg-info/
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    45941 2023-01-23 03:04:05.000000 Fiona-1.9b2/Fiona.egg-info/PKG-INFO
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4688 2023-01-23 03:04:05.000000 Fiona-1.9b2/Fiona.egg-info/SOURCES.txt
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)        1 2023-01-23 03:04:05.000000 Fiona-1.9b2/Fiona.egg-info/dependency_links.txt
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      435 2023-01-23 03:04:05.000000 Fiona-1.9b2/Fiona.egg-info/entry_points.txt
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      182 2023-01-23 03:04:05.000000 Fiona-1.9b2/Fiona.egg-info/requires.txt
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)        6 2023-01-23 03:04:05.000000 Fiona-1.9b2/Fiona.egg-info/top_level.txt
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1519 2021-12-28 20:35:56.000000 Fiona-1.9b2/LICENSE.txt
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      428 2022-12-13 21:01:24.000000 Fiona-1.9b2/MANIFEST.in
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    45941 2023-01-23 03:04:05.654907 Fiona-1.9b2/PKG-INFO
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4574 2023-01-22 03:05:59.000000 Fiona-1.9b2/README.rst
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1113 2021-12-28 20:35:56.000000 Fiona-1.9b2/benchmark.py
+drwxrwxr-x   0 seangillies  (1000) seangillies  (1000)        0 2023-01-23 03:04:05.638907 Fiona-1.9b2/docs/
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)       85 2021-12-28 20:35:56.000000 Fiona-1.9b2/docs/README.rst
+drwxrwxr-x   0 seangillies  (1000) seangillies  (1000)        0 2023-01-23 03:04:05.630907 Fiona-1.9b2/docs/_build/
+drwxrwxr-x   0 seangillies  (1000) seangillies  (1000)        0 2023-01-23 03:04:05.630907 Fiona-1.9b2/docs/_build/html/
+drwxrwxr-x   0 seangillies  (1000) seangillies  (1000)        0 2023-01-23 03:04:05.638907 Fiona-1.9b2/docs/_build/html/_sources/
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)       85 2021-12-28 20:35:56.000000 Fiona-1.9b2/docs/_build/html/_sources/README.rst.txt
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    11031 2022-10-22 22:23:14.000000 Fiona-1.9b2/docs/_build/html/_sources/cli.rst.txt
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2299 2023-01-22 02:59:24.000000 Fiona-1.9b2/docs/_build/html/_sources/fiona.fio.rst.txt
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2602 2023-01-22 02:59:24.000000 Fiona-1.9b2/docs/_build/html/_sources/fiona.rst.txt
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      301 2023-01-22 02:38:04.000000 Fiona-1.9b2/docs/_build/html/_sources/index.rst.txt
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2758 2023-01-22 02:38:04.000000 Fiona-1.9b2/docs/_build/html/_sources/install.rst.txt
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    49937 2022-12-18 22:48:24.000000 Fiona-1.9b2/docs/_build/html/_sources/manual.rst.txt
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)       52 2021-12-28 20:35:56.000000 Fiona-1.9b2/docs/_build/html/_sources/modules.rst.txt
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    11031 2022-10-22 22:23:14.000000 Fiona-1.9b2/docs/cli.rst
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1941 2021-12-28 20:35:56.000000 Fiona-1.9b2/docs/encoding.txt
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2351 2023-01-22 03:06:38.000000 Fiona-1.9b2/docs/fiona.fio.rst
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2276 2023-01-22 03:06:38.000000 Fiona-1.9b2/docs/fiona.rst
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      301 2023-01-22 03:05:59.000000 Fiona-1.9b2/docs/index.rst
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2758 2023-01-22 03:05:59.000000 Fiona-1.9b2/docs/install.rst
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    50053 2023-01-22 17:31:36.000000 Fiona-1.9b2/docs/manual.rst
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)       52 2021-12-28 20:35:56.000000 Fiona-1.9b2/docs/modules.rst
+drwxrwxr-x   0 seangillies  (1000) seangillies  (1000)        0 2023-01-23 03:04:05.638907 Fiona-1.9b2/fiona/
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    15678 2023-01-23 00:09:23.000000 Fiona-1.9b2/fiona/__init__.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      733 2021-12-28 20:35:56.000000 Fiona-1.9b2/fiona/_cpl.pxd
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      229 2021-12-28 20:35:56.000000 Fiona-1.9b2/fiona/_csl.pxd
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      382 2022-12-13 21:01:24.000000 Fiona-1.9b2/fiona/_env.pxd
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    15260 2022-12-13 21:01:24.000000 Fiona-1.9b2/fiona/_env.pyx
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      375 2022-10-22 22:23:14.000000 Fiona-1.9b2/fiona/_err.pxd
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     7528 2022-12-13 21:01:24.000000 Fiona-1.9b2/fiona/_err.pyx
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4667 2022-12-13 21:01:24.000000 Fiona-1.9b2/fiona/_geometry.pxd
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    14471 2023-01-06 16:28:20.000000 Fiona-1.9b2/fiona/_geometry.pyx
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1260 2022-10-17 14:44:01.000000 Fiona-1.9b2/fiona/_shim.pxd
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     5416 2022-12-09 20:38:53.000000 Fiona-1.9b2/fiona/_shim.pyx
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1204 2022-12-18 22:48:31.000000 Fiona-1.9b2/fiona/_show_versions.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     5203 2022-12-13 21:26:27.000000 Fiona-1.9b2/fiona/_transform.pyx
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    28133 2022-12-18 22:48:31.000000 Fiona-1.9b2/fiona/collection.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      278 2022-12-13 21:29:05.000000 Fiona-1.9b2/fiona/compat.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      218 2022-12-13 21:01:24.000000 Fiona-1.9b2/fiona/crs.pxd
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    36444 2022-12-13 21:01:24.000000 Fiona-1.9b2/fiona/crs.pyx
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    13483 2022-12-18 22:48:31.000000 Fiona-1.9b2/fiona/drvsupport.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      779 2022-12-13 21:01:24.000000 Fiona-1.9b2/fiona/enums.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    21259 2022-12-13 21:01:24.000000 Fiona-1.9b2/fiona/env.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1810 2022-12-13 21:01:24.000000 Fiona-1.9b2/fiona/errors.py
+drwxrwxr-x   0 seangillies  (1000) seangillies  (1000)        0 2023-01-23 03:04:05.638907 Fiona-1.9b2/fiona/fio/
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      510 2021-12-28 20:35:56.000000 Fiona-1.9b2/fiona/fio/__init__.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2873 2023-01-03 16:08:57.000000 Fiona-1.9b2/fiona/fio/bounds.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2105 2023-01-03 16:08:57.000000 Fiona-1.9b2/fiona/fio/calc.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     3773 2023-01-03 16:08:57.000000 Fiona-1.9b2/fiona/fio/cat.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     7760 2023-01-03 16:08:57.000000 Fiona-1.9b2/fiona/fio/collect.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      941 2023-01-03 16:08:57.000000 Fiona-1.9b2/fiona/fio/distrib.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     6771 2023-01-03 16:08:57.000000 Fiona-1.9b2/fiona/fio/dump.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1483 2022-12-13 21:01:24.000000 Fiona-1.9b2/fiona/fio/env.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1488 2023-01-03 16:08:57.000000 Fiona-1.9b2/fiona/fio/filter.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4071 2022-12-13 21:34:58.000000 Fiona-1.9b2/fiona/fio/helpers.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2511 2023-01-03 16:08:57.000000 Fiona-1.9b2/fiona/fio/info.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1212 2023-01-03 16:08:57.000000 Fiona-1.9b2/fiona/fio/insp.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     3699 2023-01-03 16:08:57.000000 Fiona-1.9b2/fiona/fio/load.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      400 2021-12-28 20:35:56.000000 Fiona-1.9b2/fiona/fio/ls.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1893 2022-12-18 22:48:31.000000 Fiona-1.9b2/fiona/fio/main.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1143 2021-12-28 20:35:56.000000 Fiona-1.9b2/fiona/fio/options.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      785 2022-12-18 22:48:31.000000 Fiona-1.9b2/fiona/fio/rm.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      438 2022-12-09 20:41:24.000000 Fiona-1.9b2/fiona/gdal.pxd
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    31806 2022-12-13 21:01:24.000000 Fiona-1.9b2/fiona/gdal.pxi
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      981 2022-12-18 22:48:31.000000 Fiona-1.9b2/fiona/inspector.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     5390 2022-12-18 22:48:31.000000 Fiona-1.9b2/fiona/io.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      879 2022-10-22 22:23:14.000000 Fiona-1.9b2/fiona/logutils.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     7054 2022-12-18 22:48:31.000000 Fiona-1.9b2/fiona/meta.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    10705 2023-01-22 18:26:12.000000 Fiona-1.9b2/fiona/model.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    75155 2023-01-22 16:21:52.000000 Fiona-1.9b2/fiona/ogrext.pyx
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4735 2022-12-13 21:01:24.000000 Fiona-1.9b2/fiona/path.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     3633 2022-06-02 19:33:29.000000 Fiona-1.9b2/fiona/rfc3339.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2540 2022-12-18 22:48:24.000000 Fiona-1.9b2/fiona/schema.pyx
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    17885 2022-12-18 22:48:31.000000 Fiona-1.9b2/fiona/session.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4248 2023-01-06 16:28:20.000000 Fiona-1.9b2/fiona/transform.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2559 2022-12-18 22:48:31.000000 Fiona-1.9b2/fiona/vfs.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2108 2022-12-13 21:01:24.000000 Fiona-1.9b2/pyproject.toml
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)       90 2022-12-13 21:01:24.000000 Fiona-1.9b2/requirements.txt
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)       38 2023-01-23 03:04:05.654907 Fiona-1.9b2/setup.cfg
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     7104 2022-12-18 22:48:24.000000 Fiona-1.9b2/setup.py
+drwxrwxr-x   0 seangillies  (1000) seangillies  (1000)        0 2023-01-23 03:04:05.646907 Fiona-1.9b2/tests/
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)       44 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/__init__.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    19350 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/conftest.py
+drwxrwxr-x   0 seangillies  (1000) seangillies  (1000)        0 2023-01-23 03:04:05.654907 Fiona-1.9b2/tests/data/
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    12922 2022-06-02 19:33:29.000000 Fiona-1.9b2/tests/data/!test.geojson
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      211 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/data/LICENSE.txt
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    15169 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/data/collection-pp.txt
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     6917 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/data/collection.txt
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)       11 2022-06-02 19:33:29.000000 Fiona-1.9b2/tests/data/coutwildrnp.cpg
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    43233 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/data/coutwildrnp.dbf
+-rw-r--r--   0 seangillies  (1000) seangillies  (1000)   253952 2022-03-23 17:00:09.000000 Fiona-1.9b2/tests/data/coutwildrnp.gpkg
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)   302617 2022-03-23 17:00:05.000000 Fiona-1.9b2/tests/data/coutwildrnp.json
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      143 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/data/coutwildrnp.prj
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)   109548 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/data/coutwildrnp.shp
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      636 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/data/coutwildrnp.shx
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)   163840 2022-03-23 17:00:13.000000 Fiona-1.9b2/tests/data/coutwildrnp.tar
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)   154006 2022-12-19 00:01:45.000000 Fiona-1.9b2/tests/data/coutwildrnp.zip
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     7559 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/data/curves_line.csv
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)   422857 2022-12-09 23:16:18.000000 Fiona-1.9b2/tests/data/data.zip
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      822 2022-10-22 22:23:14.000000 Fiona-1.9b2/tests/data/example.topojson
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)        6 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/data/gre.cpg
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2834 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/data/gre.dbf
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      143 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/data/gre.prj
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     6972 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/data/gre.shp
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      108 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/data/gre.shx
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    12922 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/data/grenada.geojson
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    32218 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/data/issue627.geojson
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    12910 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/data/sequence-pp.txt
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     6872 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/data/sequence.txt
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2460 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/data/test_gpx.gpx
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      251 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/data/test_tin.csv
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      147 2022-06-02 19:33:29.000000 Fiona-1.9b2/tests/data/test_tin.dbf
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      272 2022-06-02 19:33:29.000000 Fiona-1.9b2/tests/data/test_tin.shp
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      108 2022-06-02 19:33:29.000000 Fiona-1.9b2/tests/data/test_tin.shx
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      287 2022-06-02 19:33:29.000000 Fiona-1.9b2/tests/data/test_tz.geojson
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     3925 2022-12-18 22:48:24.000000 Fiona-1.9b2/tests/test__env.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2776 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_bigint.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1303 2022-12-13 22:07:47.000000 Fiona-1.9b2/tests/test_binary_field.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2688 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_bounds.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     7192 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_bytescollection.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    38867 2023-01-22 16:21:52.000000 Fiona-1.9b2/tests/test_collection.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2424 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_collection_crs.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     5132 2022-10-22 22:23:14.000000 Fiona-1.9b2/tests/test_collection_legacy.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      666 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_compound_crs.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4901 2022-12-13 22:11:17.000000 Fiona-1.9b2/tests/test_crs.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     5006 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_cursor_interruptions.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      459 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/test_curve_geometries.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1861 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_data_paths.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    30721 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_datetime.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      947 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_driver_options.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      921 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/test_drivers.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    11386 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_drvsupport.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1585 2022-10-22 22:23:14.000000 Fiona-1.9b2/tests/test_encoding.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4858 2022-12-18 22:48:24.000000 Fiona-1.9b2/tests/test_env.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     5243 2023-01-06 16:28:20.000000 Fiona-1.9b2/tests/test_feature.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     3024 2022-10-22 22:23:14.000000 Fiona-1.9b2/tests/test_fio_bounds.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1979 2023-01-03 16:08:57.000000 Fiona-1.9b2/tests/test_fio_calc.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4273 2022-12-18 22:48:24.000000 Fiona-1.9b2/tests/test_fio_cat.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2655 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/test_fio_collect.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      564 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/test_fio_distrib.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      980 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_fio_dump.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      852 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_fio_filter.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2868 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/test_fio_info.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     5020 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_fio_load.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1784 2022-06-02 19:33:29.000000 Fiona-1.9b2/tests/test_fio_ls.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1786 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_fio_rm.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4269 2023-01-22 05:26:48.000000 Fiona-1.9b2/tests/test_geojson.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4869 2023-01-06 16:28:20.000000 Fiona-1.9b2/tests/test_geometry.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2495 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_geopackage.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    11104 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_http_session.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1148 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_integration.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2157 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/test_layer.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     3473 2022-12-18 22:48:24.000000 Fiona-1.9b2/tests/test_listing.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1922 2022-06-02 19:33:29.000000 Fiona-1.9b2/tests/test_logutils.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    12379 2022-12-18 22:48:24.000000 Fiona-1.9b2/tests/test_memoryfile.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2107 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_meta.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     8441 2023-01-22 17:21:24.000000 Fiona-1.9b2/tests/test_model.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4069 2022-12-13 22:13:28.000000 Fiona-1.9b2/tests/test_multiconxn.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      935 2022-06-02 19:33:29.000000 Fiona-1.9b2/tests/test_non_counting_layer.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1666 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_open.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      600 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/test_profile.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4523 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_props.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      652 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/test_read_drivers.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     3835 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_remove.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)      402 2021-12-28 20:35:56.000000 Fiona-1.9b2/tests/test_revolvingdoor.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1966 2022-06-02 19:33:29.000000 Fiona-1.9b2/tests/test_rfc3339.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1819 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_rfc64_tin.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)    13826 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_schema.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     7078 2023-01-05 20:30:02.000000 Fiona-1.9b2/tests/test_schema_geom.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     3335 2022-10-22 22:23:14.000000 Fiona-1.9b2/tests/test_session.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     5354 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_slice.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1566 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_subtypes.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     1362 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_topojson.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2704 2022-12-18 22:48:24.000000 Fiona-1.9b2/tests/test_transactions.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4031 2023-01-06 16:28:20.000000 Fiona-1.9b2/tests/test_transform.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     5967 2022-12-13 22:23:38.000000 Fiona-1.9b2/tests/test_unicode.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     2446 2022-06-02 19:33:29.000000 Fiona-1.9b2/tests/test_version.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     6326 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_vfs.py
+-rw-rw-r--   0 seangillies  (1000) seangillies  (1000)     4787 2022-12-13 21:01:24.000000 Fiona-1.9b2/tests/test_write.py
```

### Comparing `Fiona-1.9b1/CHANGES.txt` & `Fiona-1.9b2/CHANGES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,30 @@
 Changes
 =======
 
 All issue numbers are relative to https://github.com/Toblerity/Fiona/issues.
 
+1.9b2 (2023-01-22)
+------------------
+
+- Add Feature.__geo_interface__ property (#1181).
+- Invalid creation options are filtered and ignored (#1180).
+- The readme doc has been shortened and freshened up, with a modern example for
+  version 1.9.0 (#1174).
+- The Geometry class now provides and looks for __geo_interface__ (#1174).
+- The top level fiona module now exports Feature, Geometry, and Properties
+  (#1174).
+- Functions that take Feature or Geometry objects will continue to take dicts
+  or objects that provide __geo_interface__ (#1177). This reverses the
+  deprecation introduced in 1.9a2.
+- Python ignores SIGPIPE by default. By never catching BrokenPipeError via
+  `except Exception` when, for example, piping the output of rio-shapes to
+  the Unix head program, we avoid getting an unhandled BrokenPipeError message
+  when the interpreter shuts down (#2689).
+
 1.9b1 (2022-12-13)
 ------------------
 
 New features:
 
 * Add listdir and listlayers method to io.MemoryFile (resolving #754).
 * Add support for TIN and triangle geometries (#1163).
```

### Comparing `Fiona-1.9b1/CREDITS.txt` & `Fiona-1.9b2/CREDITS.txt`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/Fiona.egg-info/PKG-INFO` & `Fiona-1.9b2/Fiona.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fiona
-Version: 1.9b1
+Version: 1.9b2
 Summary: Fiona reads and writes spatial data files
 Author: Sean Gillies
 Maintainer: Fiona contributors
 License: BSD 3-Clause
 Project-URL: Documentation, https://fiona.readthedocs.io/
 Project-URL: Repository, https://github.com/Toblerity/Fiona
 Keywords: gis,vector,feature,data
@@ -27,356 +27,150 @@
 Provides-Extra: test
 License-File: LICENSE.txt
 
 =====
 Fiona
 =====
 
-Fiona is GDAL_'s neat and nimble vector API for Python programmers.
-
 .. image:: https://github.com/Toblerity/Fiona/workflows/Linux%20CI/badge.svg?branch=maint-1.9
    :target: https://github.com/Toblerity/Fiona/actions?query=branch%3Amaint-1.9
 
-.. image:: https://ci.appveyor.com/api/projects/status/github/Toblerity/Fiona?svg=true
-   :target: https://ci.appveyor.com/project/sgillies/fiona/branch/maint-1.9
+Fiona streams simple feature data to and from GIS formats like GeoPackage and
+Shapefile.
 
-.. image:: https://coveralls.io/repos/Toblerity/Fiona/badge.svg
-   :target: https://coveralls.io/r/Toblerity/Fiona
+Fiona can read and write real-world data using multi-layered GIS formats,
+zipped and in-memory virtual file systems, from files on your hard drive or in
+cloud storage. This project includes Python modules and a command line
+interface (CLI).
+
+Fiona depends on `GDAL <https://gdal.org>`__ but is different from GDAL's own
+`bindings <https://gdal.org/api/python_bindings.html>`__. Fiona is designed to
+be highly productive and to make it easy to write code which is easy to read.
 
-Fiona is designed to be simple and dependable. It focuses on reading and
-writing data in standard Python IO style and relies upon familiar Python types
-and protocols such as files, dictionaries, mappings, and iterators instead of
-classes specific to OGR. Fiona can read and write real-world data using
-multi-layered GIS formats and zipped virtual file systems and integrates
-readily with other Python GIS packages such as pyproj_, Rtree_, and Shapely_.
+Installation
+============
 
-Fiona is supported only on CPython versions 3.6+.
+Fiona has several `extension modules
+<https://docs.python.org/3/extending/extending.html>`__ which link against
+libgdal. This complicates installation. Binary distributions (wheels)
+containing libgdal and its own dependencies are available from the Python
+Package Index and can be installed using pip.
 
-Why the name "Fiona"? Because Fiona Is OGR's Neat and Nimble API for Python programmers. And a Shrek reference made us laugh.
+.. code-block:: console
 
-For more details, see:
+    pip install fiona
 
-* Fiona `home page <https://github.com/Toblerity/Fiona>`__
-* `Docs and manual <https://fiona.readthedocs.io/>`__
-* `Examples <https://github.com/Toblerity/Fiona/tree/master/examples>`__
-* Main `user discussion group <https://fiona.groups.io/g/main>`__
-* `Developers discussion group <https://fiona.groups.io/g/dev>`__
+These wheels are mainly intended to make installation easy for simple
+applications, not so much for production. They are not tested for compatibility
+with all other binary wheels, conda packages, or QGIS, and omit many of GDAL's
+optional format drivers. If you need, for example, GML support you will need to
+build and install Fiona from a source distribution.
 
-Usage
-=====
+Many users find Anaconda and conda-forge a good way to install Fiona and get
+access to more optional format drivers (like GML).
 
-Collections
------------
+Fiona 1.9 (coming soon) requires Python 3.7 or higher and GDAL 3.2 or higher.
 
-Records are read from and written to ``file``-like `Collection` objects
-returned from the ``fiona.open()`` function.  Records are mappings modeled on
-the GeoJSON format. They don't have any spatial methods of their own, so if you
-want to do anything fancy with them you will probably need Shapely or something
-like it. Here is an example of using Fiona to read some records from one data
-file, change their geometry attributes, and write them to a new data file.
+Python Usage
+============
+
+Features are read from and written to file-like ``Collection`` objects
+returned from the ``fiona.open()`` function. Features are data classes modeled
+on the GeoJSON format. They don't have any spatial methods of their own, so if
+you want to do anything fancy with them you will need Shapely or something like
+it. Here is an example of using Fiona to read some features from one data file,
+change their geometry attributes using Shapely, and write them to a new data
+file.
 
 .. code-block:: python
 
     import fiona
+    from fiona import Feature, Geometry
+    from shapely.geometry import mapping, shape
 
-    # Open a file for reading. We'll call this the "source."
-
-    with fiona.open('tests/data/coutwildrnp.shp') as src:
-
-        # The file we'll write to, the "destination", must be initialized
-        # with a coordinate system, a format driver name, and
-        # a record schema.  We can get initial values from the open
-        # collection's ``meta`` property and then modify them as
-        # desired.
-
-        meta = src.meta
-        meta['schema']['geometry'] = 'Point'
+    # Open a file for reading. We'll call this the source.
+    with fiona.open("tests/data/coutwildrnp.shp") as src:
 
-        # Open an output file, using the same format driver and
-        # coordinate reference system as the source. The ``meta``
-        # mapping fills in the keyword parameters of fiona.open().
-
-        with fiona.open('test_write.shp', 'w', **meta) as dst:
+        # The file we'll write to must be initialized with a coordinate
+        # system, a format driver name, and a record schema. We can get
+        # initial values from the open source's profile property and then
+        # modify them as we need.
+        profile = src.profile
+        profile["schema"]["geometry"] = "Point"
+        profile["driver"] = "GPKG"
+
+        # Open an output file, using the same format driver and coordinate
+        # reference system as the source. The profile mapping fills in the
+        # keyword parameters of fiona.open.
+        with fiona.open("/tmp/example.gpkg", "w", **profile) as dst:
 
             # Process only the records intersecting a box.
             for f in src.filter(bbox=(-107.0, 37.0, -105.0, 39.0)):
 
-                # Get a point on the boundary of the record's
-                # geometry.
-
-                f['geometry'] = {
-                    'type': 'Point',
-                    'coordinates': f['geometry']['coordinates'][0][0]}
-
-                # Write the record out.
-
-                dst.write(f)
-
-    # The destination's contents are flushed to disk and the file is
-    # closed when its ``with`` block ends. This effectively
-    # executes ``dst.flush(); dst.close()``.
-
-Reading Multilayer data
------------------------
-
-Collections can also be made from single layers within multilayer files or
-directories of data. The target layer is specified by name or by its integer
-index within the file or directory. The ``fiona.listlayers()`` function
-provides an index ordered list of layer names.
-
-.. code-block:: python
-
-    for layername in fiona.listlayers('tests/data'):
-        with fiona.open('tests/data', layer=layername) as src:
-            print(layername, len(src))
-
-    # Output:
-    # ('coutwildrnp', 67)
-
-Layer can also be specified by index. In this case, ``layer=0`` and
-``layer='test_uk'`` specify the same layer in the data file or directory.
-
-.. code-block:: python
-
-    for i, layername in enumerate(fiona.listlayers('tests/data')):
-        with fiona.open('tests/data', layer=i) as src:
-            print(i, layername, len(src))
-
-    # Output:
-    # (0, 'coutwildrnp', 67)
-
-Writing Multilayer data
------------------------
-
-Multilayer data can be written as well. Layers must be specified by name when
-writing.
-
-.. code-block:: python
-
-    with open('tests/data/cowildrnp.shp') as src:
-        meta = src.meta
-        f = next(src)
-
-    with fiona.open('/tmp/foo', 'w', layer='bar', **meta) as dst:
-        dst.write(f)
-
-    print(fiona.listlayers('/tmp/foo'))
-
-    with fiona.open('/tmp/foo', layer='bar') as src:
-        print(len(src))
-        f = next(src)
-        print(f['geometry']['type'])
-        print(f['properties'])
-
-        # Output:
-        # ['bar']
-        # 1
-        # Polygon
-        # OrderedDict([('PERIMETER', 1.22107), ('FEATURE2', None), ('NAME', 'Mount Naomi Wilderness'), ('FEATURE1', 'Wilderness'), ('URL', 'http://www.wilderness.net/index.cfm?fuse=NWPS&sec=wildView&wname=Mount%20Naomi'), ('AGBUR', 'FS'), ('AREA', 0.0179264), ('STATE_FIPS', '49'), ('WILDRNP020', 332), ('STATE', 'UT')])
-
-A view of the /tmp/foo directory will confirm the creation of the new files.
-
-.. code-block:: console
-
-    $ ls /tmp/foo
-    bar.cpg bar.dbf bar.prj bar.shp bar.shx
+                # Get the feature's centroid.
+                centroid_shp = shape(f.geometry).centroid
+                new_geom = Geometry.from_dict(centroid_shp)
+
+                # Write the feature out.
+                dst.write(
+                    Feature(geometry=new_geom, properties=f.properties)
+                )
+
+        # The destination's contents are flushed to disk and the file is
+        # closed when its with block ends. This effectively
+        # executes ``dst.flush(); dst.close()``.
 
-Collections from archives and virtual file systems
---------------------------------------------------
-
-Zip and Tar archives can be treated as virtual filesystems and Collections can
-be made from paths and layers within them. In other words, Fiona lets you read
-and write zipped Shapefiles.
-
-.. code-block:: python
-
-    for i, layername in enumerate(fiona.listlayers('zip://tests/data/coutwildrnp.zip')):
-        with fiona.open('zip://tests/data/coutwildrnp.zip', layer=i) as src:
-            print(i, layername, len(src))
-
-    # Output:
-    # (0, 'coutwildrnp', 67)
-
-Fiona can also read from more exotic file systems. For instance, a
-zipped shape file in S3 can be accessed like so:
-
-.. code-block:: python
-
-   with fiona.open('zip+s3://mapbox/rasterio/coutwildrnp.zip') as src:
-       print(len(src))
-
-   # Output:
-   # 67
-
-
-Fiona CLI
+CLI Usage
 =========
 
 Fiona's command line interface, named "fio", is documented at `docs/cli.rst
-<https://github.com/Toblerity/Fiona/blob/master/docs/cli.rst>`__. Its ``fio
-info`` pretty prints information about a data file.
-
-.. code-block:: console
-
-    $ fio info --indent 2 tests/data/coutwildrnp.shp
-    {
-      "count": 67,
-      "crs": "EPSG:4326",
-      "driver": "ESRI Shapefile",
-      "bounds": [
-        -113.56424713134766,
-        37.0689811706543,
-        -104.97087097167969,
-        41.99627685546875
-      ],
-      "schema": {
-        "geometry": "Polygon",
-        "properties": {
-          "PERIMETER": "float:24.15",
-          "FEATURE2": "str:80",
-          "NAME": "str:80",
-          "FEATURE1": "str:80",
-          "URL": "str:101",
-          "AGBUR": "str:80",
-          "AREA": "float:24.15",
-          "STATE_FIPS": "str:80",
-          "WILDRNP020": "int:10",
-          "STATE": "str:80"
-        }
-      }
-    }
-
-Installation
-============
-
-Fiona requires Python 3.6+ and GDAL/OGR 1.8+. To build from
-a source distribution you will need a C compiler and GDAL and Python
-development headers and libraries (libgdal1-dev for Debian/Ubuntu, gdal-dev for
-CentOS/Fedora).
-
-To build from a repository copy, you will also need Cython to build C sources
-from the project's .pyx files. See the project's requirements-dev.txt file for
-guidance.
-
-The `Kyngchaos GDAL frameworks
-<https://www.kyngchaos.com/software/frameworks/#gdal_complete>`__ will satisfy
-the GDAL/OGR dependency for OS X, as will Homebrew's GDAL Formula (``brew install
-gdal``).
-
-Python Requirements
--------------------
-
-Fiona depends on the modules ``cligj`` and ``munch``.
-Pip will fetch these requirements for you, but users installing Fiona from a
-Windows installer must get them separately.
-
-Unix-like systems
------------------
-
-Assuming you're using a virtualenv (if not, skip to the 4th command) and
-GDAL/OGR libraries, headers, and `gdal-config`_ program are installed to well
-known locations on your system via your system's package manager (``brew
-install gdal`` using Homebrew on OS X), installation is this simple.
+<https://github.com/Toblerity/Fiona/blob/master/docs/cli.rst>`__. The CLI has a
+number of different commands. Its ``fio cat`` command streams GeoJSON features
+from any dataset.
 
 .. code-block:: console
 
-  $ mkdir fiona_env
-  $ virtualenv fiona_env
-  $ source fiona_env/bin/activate
-  (fiona_env)$ pip install fiona
-
-If gdal-config is not available or if GDAL/OGR headers and libs aren't
-installed to a well known location, you must set include dirs, library dirs,
-and libraries options via the setup.cfg file or setup command line as shown
-below (using ``git``). You must also specify the version of the GDAL API on the
-command line using the ``--gdalversion`` argument (see example below) or with
-the ``GDAL_VERSION`` environment variable (e.g. ``export GDAL_VERSION=2.1``).
+    $ fio cat --compact tests/data/coutwildrnp.shp | jq -c '.'
+    {"geometry":{"coordinates":[[[-111.73527526855469,41.995094299316406],...]]}}
+    ...
 
-.. code-block:: console
+Documentation
+=============
 
-  (fiona_env)$ git clone git://github.com/Toblerity/Fiona.git
-  (fiona_env)$ cd Fiona
-  (fiona_env)$ python setup.py build_ext -I/path/to/gdal/include -L/path/to/gdal/lib -lgdal install --gdalversion 2.1
+For more details about this project, please see:
 
-Or specify that build options and GDAL API version should be provided by a
-particular gdal-config program.
-
-.. code-block:: console
-
-  (fiona_env)$ GDAL_CONFIG=/path/to/gdal-config pip install fiona
-
-Windows
--------
-
-Binary installers are available at
-https://www.lfd.uci.edu/~gohlke/pythonlibs/#fiona and coming eventually to PyPI.
-
-You can download a binary distribution of GDAL from `here
-<https://www.gisinternals.com/release.php>`_.  You will also need to download
-the compiled libraries and headers (include files).
-
-When building from source on Windows, it is important to know that setup.py
-cannot rely on gdal-config, which is only present on UNIX systems, to discover
-the locations of header files and libraries that Fiona needs to compile its
-C extensions. On Windows, these paths need to be provided by the user.
-You will need to find the include files and the library files for gdal and
-use setup.py as follows. You must also specify the version of the GDAL API on the
-command line using the ``--gdalversion`` argument (see example below) or with
-the ``GDAL_VERSION`` environment variable (e.g. ``set GDAL_VERSION=2.1``).
-
-.. code-block:: console
-
-    $ python setup.py build_ext -I<path to gdal include files> -lgdal_i -L<path to gdal library> install --gdalversion 2.1
-
-Note: The following environment variables needs to be set so that Fiona works correctly:
-
-* The directory containing the GDAL DLL (``gdal304.dll`` or similar) needs to be in your
-  Windows ``PATH`` (e.g. ``C:\gdal\bin``).
-* The gdal-data directory needs to be in your Windows ``PATH`` or the environment variable
-  ``GDAL_DATA`` must be set (e.g. ``C:\gdal\bin\gdal-data``).
-* The environment variable ``PROJ_LIB`` (PROJ < 9.1) | ``PROJ_DATA`` (PROJ 9.1+) must be set to the proj data directory (e.g.
-  ``C:\gdal\bin\proj6\share``)
-
-The `Appveyor CI build <https://ci.appveyor.com/project/sgillies/fiona/history>`__
-uses the GISInternals GDAL binaries to build Fiona. This produces a binary wheel
-for successful builds, which includes GDAL and other dependencies, for users
-wanting to try an unstable development version.
-The `Appveyor configuration file <https://github.com/Toblerity/Fiona/blob/master/appveyor.yml>`__ may be a useful example for
-users building from source on Windows.
-
-Development and testing
-=======================
-
-Building from the source requires Cython. Tests require `pytest <https://pytest.org>`_. If the GDAL/OGR
-libraries, headers, and `gdal-config`_ program are installed to well known
-locations on your system (via your system's package manager), you can do this::
-
-  (fiona_env)$ git clone git://github.com/Toblerity/Fiona.git
-  (fiona_env)$ cd Fiona
-  (fiona_env)$ pip install cython
-  (fiona_env)$ pip install -e .[test]
-  (fiona_env)$ pytest
-
-If you have a non-standard environment, you'll need to specify the include and
-lib dirs and GDAL library on the command line::
-
-  (fiona_env)$ python setup.py build_ext -I/path/to/gdal/include -L/path/to/gdal/lib -lgdal --gdalversion 2 develop
-  (fiona_env)$ pytest
-
-.. _GDAL: https://gdal.org
-.. _pyproj: https://pypi.org/project/pyproj/
-.. _Rtree: https://pypi.org/project/Rtree/
-.. _Shapely: https://pypi.org/project/Shapely/
-.. _gdal-config: https://gdal.org/programs/gdal-config.html
+* Fiona `home page <https://github.com/Toblerity/Fiona>`__
+* `Docs and manual <https://fiona.readthedocs.io/>`__
+* `Examples <https://github.com/Toblerity/Fiona/tree/master/examples>`__
+* Main `user discussion group <https://fiona.groups.io/g/main>`__
+* `Developers discussion group <https://fiona.groups.io/g/dev>`__
 
 Changes
 =======
 
 All issue numbers are relative to https://github.com/Toblerity/Fiona/issues.
 
+1.9b2 (2023-01-22)
+------------------
+
+- Add Feature.__geo_interface__ property (#1181).
+- Invalid creation options are filtered and ignored (#1180).
+- The readme doc has been shortened and freshened up, with a modern example for
+  version 1.9.0 (#1174).
+- The Geometry class now provides and looks for __geo_interface__ (#1174).
+- The top level fiona module now exports Feature, Geometry, and Properties
+  (#1174).
+- Functions that take Feature or Geometry objects will continue to take dicts
+  or objects that provide __geo_interface__ (#1177). This reverses the
+  deprecation introduced in 1.9a2.
+- Python ignores SIGPIPE by default. By never catching BrokenPipeError via
+  `except Exception` when, for example, piping the output of rio-shapes to
+  the Unix head program, we avoid getting an unhandled BrokenPipeError message
+  when the interpreter shuts down (#2689).
+
 1.9b1 (2022-12-13)
 ------------------
 
 New features:
 
 * Add listdir and listlayers method to io.MemoryFile (resolving #754).
 * Add support for TIN and triangle geometries (#1163).
```

### Comparing `Fiona-1.9b1/Fiona.egg-info/SOURCES.txt` & `Fiona-1.9b2/Fiona.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -51,16 +51,25 @@
 Fiona.egg-info/top_level.txt
 docs/README.rst
 docs/cli.rst
 docs/encoding.txt
 docs/fiona.fio.rst
 docs/fiona.rst
 docs/index.rst
+docs/install.rst
 docs/manual.rst
 docs/modules.rst
+docs/_build/html/_sources/README.rst.txt
+docs/_build/html/_sources/cli.rst.txt
+docs/_build/html/_sources/fiona.fio.rst.txt
+docs/_build/html/_sources/fiona.rst.txt
+docs/_build/html/_sources/index.rst.txt
+docs/_build/html/_sources/install.rst.txt
+docs/_build/html/_sources/manual.rst.txt
+docs/_build/html/_sources/modules.rst.txt
 fiona/__init__.py
 fiona/_cpl.pxd
 fiona/_csl.pxd
 fiona/_env.pxd
 fiona/_env.pyx
 fiona/_err.pxd
 fiona/_err.pyx
```

### Comparing `Fiona-1.9b1/LICENSE.txt` & `Fiona-1.9b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/PKG-INFO` & `Fiona-1.9b2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fiona
-Version: 1.9b1
+Version: 1.9b2
 Summary: Fiona reads and writes spatial data files
 Author: Sean Gillies
 Maintainer: Fiona contributors
 License: BSD 3-Clause
 Project-URL: Documentation, https://fiona.readthedocs.io/
 Project-URL: Repository, https://github.com/Toblerity/Fiona
 Keywords: gis,vector,feature,data
@@ -27,356 +27,150 @@
 Provides-Extra: test
 License-File: LICENSE.txt
 
 =====
 Fiona
 =====
 
-Fiona is GDAL_'s neat and nimble vector API for Python programmers.
-
 .. image:: https://github.com/Toblerity/Fiona/workflows/Linux%20CI/badge.svg?branch=maint-1.9
    :target: https://github.com/Toblerity/Fiona/actions?query=branch%3Amaint-1.9
 
-.. image:: https://ci.appveyor.com/api/projects/status/github/Toblerity/Fiona?svg=true
-   :target: https://ci.appveyor.com/project/sgillies/fiona/branch/maint-1.9
+Fiona streams simple feature data to and from GIS formats like GeoPackage and
+Shapefile.
 
-.. image:: https://coveralls.io/repos/Toblerity/Fiona/badge.svg
-   :target: https://coveralls.io/r/Toblerity/Fiona
+Fiona can read and write real-world data using multi-layered GIS formats,
+zipped and in-memory virtual file systems, from files on your hard drive or in
+cloud storage. This project includes Python modules and a command line
+interface (CLI).
+
+Fiona depends on `GDAL <https://gdal.org>`__ but is different from GDAL's own
+`bindings <https://gdal.org/api/python_bindings.html>`__. Fiona is designed to
+be highly productive and to make it easy to write code which is easy to read.
 
-Fiona is designed to be simple and dependable. It focuses on reading and
-writing data in standard Python IO style and relies upon familiar Python types
-and protocols such as files, dictionaries, mappings, and iterators instead of
-classes specific to OGR. Fiona can read and write real-world data using
-multi-layered GIS formats and zipped virtual file systems and integrates
-readily with other Python GIS packages such as pyproj_, Rtree_, and Shapely_.
+Installation
+============
 
-Fiona is supported only on CPython versions 3.6+.
+Fiona has several `extension modules
+<https://docs.python.org/3/extending/extending.html>`__ which link against
+libgdal. This complicates installation. Binary distributions (wheels)
+containing libgdal and its own dependencies are available from the Python
+Package Index and can be installed using pip.
 
-Why the name "Fiona"? Because Fiona Is OGR's Neat and Nimble API for Python programmers. And a Shrek reference made us laugh.
+.. code-block:: console
 
-For more details, see:
+    pip install fiona
 
-* Fiona `home page <https://github.com/Toblerity/Fiona>`__
-* `Docs and manual <https://fiona.readthedocs.io/>`__
-* `Examples <https://github.com/Toblerity/Fiona/tree/master/examples>`__
-* Main `user discussion group <https://fiona.groups.io/g/main>`__
-* `Developers discussion group <https://fiona.groups.io/g/dev>`__
+These wheels are mainly intended to make installation easy for simple
+applications, not so much for production. They are not tested for compatibility
+with all other binary wheels, conda packages, or QGIS, and omit many of GDAL's
+optional format drivers. If you need, for example, GML support you will need to
+build and install Fiona from a source distribution.
 
-Usage
-=====
+Many users find Anaconda and conda-forge a good way to install Fiona and get
+access to more optional format drivers (like GML).
 
-Collections
------------
+Fiona 1.9 (coming soon) requires Python 3.7 or higher and GDAL 3.2 or higher.
 
-Records are read from and written to ``file``-like `Collection` objects
-returned from the ``fiona.open()`` function.  Records are mappings modeled on
-the GeoJSON format. They don't have any spatial methods of their own, so if you
-want to do anything fancy with them you will probably need Shapely or something
-like it. Here is an example of using Fiona to read some records from one data
-file, change their geometry attributes, and write them to a new data file.
+Python Usage
+============
+
+Features are read from and written to file-like ``Collection`` objects
+returned from the ``fiona.open()`` function. Features are data classes modeled
+on the GeoJSON format. They don't have any spatial methods of their own, so if
+you want to do anything fancy with them you will need Shapely or something like
+it. Here is an example of using Fiona to read some features from one data file,
+change their geometry attributes using Shapely, and write them to a new data
+file.
 
 .. code-block:: python
 
     import fiona
+    from fiona import Feature, Geometry
+    from shapely.geometry import mapping, shape
 
-    # Open a file for reading. We'll call this the "source."
-
-    with fiona.open('tests/data/coutwildrnp.shp') as src:
-
-        # The file we'll write to, the "destination", must be initialized
-        # with a coordinate system, a format driver name, and
-        # a record schema.  We can get initial values from the open
-        # collection's ``meta`` property and then modify them as
-        # desired.
-
-        meta = src.meta
-        meta['schema']['geometry'] = 'Point'
+    # Open a file for reading. We'll call this the source.
+    with fiona.open("tests/data/coutwildrnp.shp") as src:
 
-        # Open an output file, using the same format driver and
-        # coordinate reference system as the source. The ``meta``
-        # mapping fills in the keyword parameters of fiona.open().
-
-        with fiona.open('test_write.shp', 'w', **meta) as dst:
+        # The file we'll write to must be initialized with a coordinate
+        # system, a format driver name, and a record schema. We can get
+        # initial values from the open source's profile property and then
+        # modify them as we need.
+        profile = src.profile
+        profile["schema"]["geometry"] = "Point"
+        profile["driver"] = "GPKG"
+
+        # Open an output file, using the same format driver and coordinate
+        # reference system as the source. The profile mapping fills in the
+        # keyword parameters of fiona.open.
+        with fiona.open("/tmp/example.gpkg", "w", **profile) as dst:
 
             # Process only the records intersecting a box.
             for f in src.filter(bbox=(-107.0, 37.0, -105.0, 39.0)):
 
-                # Get a point on the boundary of the record's
-                # geometry.
-
-                f['geometry'] = {
-                    'type': 'Point',
-                    'coordinates': f['geometry']['coordinates'][0][0]}
-
-                # Write the record out.
-
-                dst.write(f)
-
-    # The destination's contents are flushed to disk and the file is
-    # closed when its ``with`` block ends. This effectively
-    # executes ``dst.flush(); dst.close()``.
-
-Reading Multilayer data
------------------------
-
-Collections can also be made from single layers within multilayer files or
-directories of data. The target layer is specified by name or by its integer
-index within the file or directory. The ``fiona.listlayers()`` function
-provides an index ordered list of layer names.
-
-.. code-block:: python
-
-    for layername in fiona.listlayers('tests/data'):
-        with fiona.open('tests/data', layer=layername) as src:
-            print(layername, len(src))
-
-    # Output:
-    # ('coutwildrnp', 67)
-
-Layer can also be specified by index. In this case, ``layer=0`` and
-``layer='test_uk'`` specify the same layer in the data file or directory.
-
-.. code-block:: python
-
-    for i, layername in enumerate(fiona.listlayers('tests/data')):
-        with fiona.open('tests/data', layer=i) as src:
-            print(i, layername, len(src))
-
-    # Output:
-    # (0, 'coutwildrnp', 67)
-
-Writing Multilayer data
------------------------
-
-Multilayer data can be written as well. Layers must be specified by name when
-writing.
-
-.. code-block:: python
-
-    with open('tests/data/cowildrnp.shp') as src:
-        meta = src.meta
-        f = next(src)
-
-    with fiona.open('/tmp/foo', 'w', layer='bar', **meta) as dst:
-        dst.write(f)
-
-    print(fiona.listlayers('/tmp/foo'))
-
-    with fiona.open('/tmp/foo', layer='bar') as src:
-        print(len(src))
-        f = next(src)
-        print(f['geometry']['type'])
-        print(f['properties'])
-
-        # Output:
-        # ['bar']
-        # 1
-        # Polygon
-        # OrderedDict([('PERIMETER', 1.22107), ('FEATURE2', None), ('NAME', 'Mount Naomi Wilderness'), ('FEATURE1', 'Wilderness'), ('URL', 'http://www.wilderness.net/index.cfm?fuse=NWPS&sec=wildView&wname=Mount%20Naomi'), ('AGBUR', 'FS'), ('AREA', 0.0179264), ('STATE_FIPS', '49'), ('WILDRNP020', 332), ('STATE', 'UT')])
-
-A view of the /tmp/foo directory will confirm the creation of the new files.
-
-.. code-block:: console
-
-    $ ls /tmp/foo
-    bar.cpg bar.dbf bar.prj bar.shp bar.shx
+                # Get the feature's centroid.
+                centroid_shp = shape(f.geometry).centroid
+                new_geom = Geometry.from_dict(centroid_shp)
+
+                # Write the feature out.
+                dst.write(
+                    Feature(geometry=new_geom, properties=f.properties)
+                )
+
+        # The destination's contents are flushed to disk and the file is
+        # closed when its with block ends. This effectively
+        # executes ``dst.flush(); dst.close()``.
 
-Collections from archives and virtual file systems
---------------------------------------------------
-
-Zip and Tar archives can be treated as virtual filesystems and Collections can
-be made from paths and layers within them. In other words, Fiona lets you read
-and write zipped Shapefiles.
-
-.. code-block:: python
-
-    for i, layername in enumerate(fiona.listlayers('zip://tests/data/coutwildrnp.zip')):
-        with fiona.open('zip://tests/data/coutwildrnp.zip', layer=i) as src:
-            print(i, layername, len(src))
-
-    # Output:
-    # (0, 'coutwildrnp', 67)
-
-Fiona can also read from more exotic file systems. For instance, a
-zipped shape file in S3 can be accessed like so:
-
-.. code-block:: python
-
-   with fiona.open('zip+s3://mapbox/rasterio/coutwildrnp.zip') as src:
-       print(len(src))
-
-   # Output:
-   # 67
-
-
-Fiona CLI
+CLI Usage
 =========
 
 Fiona's command line interface, named "fio", is documented at `docs/cli.rst
-<https://github.com/Toblerity/Fiona/blob/master/docs/cli.rst>`__. Its ``fio
-info`` pretty prints information about a data file.
-
-.. code-block:: console
-
-    $ fio info --indent 2 tests/data/coutwildrnp.shp
-    {
-      "count": 67,
-      "crs": "EPSG:4326",
-      "driver": "ESRI Shapefile",
-      "bounds": [
-        -113.56424713134766,
-        37.0689811706543,
-        -104.97087097167969,
-        41.99627685546875
-      ],
-      "schema": {
-        "geometry": "Polygon",
-        "properties": {
-          "PERIMETER": "float:24.15",
-          "FEATURE2": "str:80",
-          "NAME": "str:80",
-          "FEATURE1": "str:80",
-          "URL": "str:101",
-          "AGBUR": "str:80",
-          "AREA": "float:24.15",
-          "STATE_FIPS": "str:80",
-          "WILDRNP020": "int:10",
-          "STATE": "str:80"
-        }
-      }
-    }
-
-Installation
-============
-
-Fiona requires Python 3.6+ and GDAL/OGR 1.8+. To build from
-a source distribution you will need a C compiler and GDAL and Python
-development headers and libraries (libgdal1-dev for Debian/Ubuntu, gdal-dev for
-CentOS/Fedora).
-
-To build from a repository copy, you will also need Cython to build C sources
-from the project's .pyx files. See the project's requirements-dev.txt file for
-guidance.
-
-The `Kyngchaos GDAL frameworks
-<https://www.kyngchaos.com/software/frameworks/#gdal_complete>`__ will satisfy
-the GDAL/OGR dependency for OS X, as will Homebrew's GDAL Formula (``brew install
-gdal``).
-
-Python Requirements
--------------------
-
-Fiona depends on the modules ``cligj`` and ``munch``.
-Pip will fetch these requirements for you, but users installing Fiona from a
-Windows installer must get them separately.
-
-Unix-like systems
------------------
-
-Assuming you're using a virtualenv (if not, skip to the 4th command) and
-GDAL/OGR libraries, headers, and `gdal-config`_ program are installed to well
-known locations on your system via your system's package manager (``brew
-install gdal`` using Homebrew on OS X), installation is this simple.
+<https://github.com/Toblerity/Fiona/blob/master/docs/cli.rst>`__. The CLI has a
+number of different commands. Its ``fio cat`` command streams GeoJSON features
+from any dataset.
 
 .. code-block:: console
 
-  $ mkdir fiona_env
-  $ virtualenv fiona_env
-  $ source fiona_env/bin/activate
-  (fiona_env)$ pip install fiona
-
-If gdal-config is not available or if GDAL/OGR headers and libs aren't
-installed to a well known location, you must set include dirs, library dirs,
-and libraries options via the setup.cfg file or setup command line as shown
-below (using ``git``). You must also specify the version of the GDAL API on the
-command line using the ``--gdalversion`` argument (see example below) or with
-the ``GDAL_VERSION`` environment variable (e.g. ``export GDAL_VERSION=2.1``).
+    $ fio cat --compact tests/data/coutwildrnp.shp | jq -c '.'
+    {"geometry":{"coordinates":[[[-111.73527526855469,41.995094299316406],...]]}}
+    ...
 
-.. code-block:: console
+Documentation
+=============
 
-  (fiona_env)$ git clone git://github.com/Toblerity/Fiona.git
-  (fiona_env)$ cd Fiona
-  (fiona_env)$ python setup.py build_ext -I/path/to/gdal/include -L/path/to/gdal/lib -lgdal install --gdalversion 2.1
+For more details about this project, please see:
 
-Or specify that build options and GDAL API version should be provided by a
-particular gdal-config program.
-
-.. code-block:: console
-
-  (fiona_env)$ GDAL_CONFIG=/path/to/gdal-config pip install fiona
-
-Windows
--------
-
-Binary installers are available at
-https://www.lfd.uci.edu/~gohlke/pythonlibs/#fiona and coming eventually to PyPI.
-
-You can download a binary distribution of GDAL from `here
-<https://www.gisinternals.com/release.php>`_.  You will also need to download
-the compiled libraries and headers (include files).
-
-When building from source on Windows, it is important to know that setup.py
-cannot rely on gdal-config, which is only present on UNIX systems, to discover
-the locations of header files and libraries that Fiona needs to compile its
-C extensions. On Windows, these paths need to be provided by the user.
-You will need to find the include files and the library files for gdal and
-use setup.py as follows. You must also specify the version of the GDAL API on the
-command line using the ``--gdalversion`` argument (see example below) or with
-the ``GDAL_VERSION`` environment variable (e.g. ``set GDAL_VERSION=2.1``).
-
-.. code-block:: console
-
-    $ python setup.py build_ext -I<path to gdal include files> -lgdal_i -L<path to gdal library> install --gdalversion 2.1
-
-Note: The following environment variables needs to be set so that Fiona works correctly:
-
-* The directory containing the GDAL DLL (``gdal304.dll`` or similar) needs to be in your
-  Windows ``PATH`` (e.g. ``C:\gdal\bin``).
-* The gdal-data directory needs to be in your Windows ``PATH`` or the environment variable
-  ``GDAL_DATA`` must be set (e.g. ``C:\gdal\bin\gdal-data``).
-* The environment variable ``PROJ_LIB`` (PROJ < 9.1) | ``PROJ_DATA`` (PROJ 9.1+) must be set to the proj data directory (e.g.
-  ``C:\gdal\bin\proj6\share``)
-
-The `Appveyor CI build <https://ci.appveyor.com/project/sgillies/fiona/history>`__
-uses the GISInternals GDAL binaries to build Fiona. This produces a binary wheel
-for successful builds, which includes GDAL and other dependencies, for users
-wanting to try an unstable development version.
-The `Appveyor configuration file <https://github.com/Toblerity/Fiona/blob/master/appveyor.yml>`__ may be a useful example for
-users building from source on Windows.
-
-Development and testing
-=======================
-
-Building from the source requires Cython. Tests require `pytest <https://pytest.org>`_. If the GDAL/OGR
-libraries, headers, and `gdal-config`_ program are installed to well known
-locations on your system (via your system's package manager), you can do this::
-
-  (fiona_env)$ git clone git://github.com/Toblerity/Fiona.git
-  (fiona_env)$ cd Fiona
-  (fiona_env)$ pip install cython
-  (fiona_env)$ pip install -e .[test]
-  (fiona_env)$ pytest
-
-If you have a non-standard environment, you'll need to specify the include and
-lib dirs and GDAL library on the command line::
-
-  (fiona_env)$ python setup.py build_ext -I/path/to/gdal/include -L/path/to/gdal/lib -lgdal --gdalversion 2 develop
-  (fiona_env)$ pytest
-
-.. _GDAL: https://gdal.org
-.. _pyproj: https://pypi.org/project/pyproj/
-.. _Rtree: https://pypi.org/project/Rtree/
-.. _Shapely: https://pypi.org/project/Shapely/
-.. _gdal-config: https://gdal.org/programs/gdal-config.html
+* Fiona `home page <https://github.com/Toblerity/Fiona>`__
+* `Docs and manual <https://fiona.readthedocs.io/>`__
+* `Examples <https://github.com/Toblerity/Fiona/tree/master/examples>`__
+* Main `user discussion group <https://fiona.groups.io/g/main>`__
+* `Developers discussion group <https://fiona.groups.io/g/dev>`__
 
 Changes
 =======
 
 All issue numbers are relative to https://github.com/Toblerity/Fiona/issues.
 
+1.9b2 (2023-01-22)
+------------------
+
+- Add Feature.__geo_interface__ property (#1181).
+- Invalid creation options are filtered and ignored (#1180).
+- The readme doc has been shortened and freshened up, with a modern example for
+  version 1.9.0 (#1174).
+- The Geometry class now provides and looks for __geo_interface__ (#1174).
+- The top level fiona module now exports Feature, Geometry, and Properties
+  (#1174).
+- Functions that take Feature or Geometry objects will continue to take dicts
+  or objects that provide __geo_interface__ (#1177). This reverses the
+  deprecation introduced in 1.9a2.
+- Python ignores SIGPIPE by default. By never catching BrokenPipeError via
+  `except Exception` when, for example, piping the output of rio-shapes to
+  the Unix head program, we avoid getting an unhandled BrokenPipeError message
+  when the interpreter shuts down (#2689).
+
 1.9b1 (2022-12-13)
 ------------------
 
 New features:
 
 * Add listdir and listlayers method to io.MemoryFile (resolving #754).
 * Add support for TIN and triangle geometries (#1163).
```

### Comparing `Fiona-1.9b1/benchmark.py` & `Fiona-1.9b2/benchmark.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/docs/cli.rst` & `Fiona-1.9b2/docs/_build/html/_sources/cli.rst.txt`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/docs/encoding.txt` & `Fiona-1.9b2/docs/encoding.txt`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/docs/fiona.fio.rst` & `Fiona-1.9b2/docs/fiona.fio.rst`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/docs/fiona.rst` & `Fiona-1.9b2/docs/fiona.rst`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/docs/manual.rst` & `Fiona-1.9b2/docs/_build/html/_sources/manual.rst.txt`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/__init__.py` & `Fiona-1.9b2/fiona/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,46 +81,57 @@
     else:
         if "PATH" in os.environ:
             for p in os.environ["PATH"].split(os.pathsep):
                 if glob.glob(os.path.join(p, "gdal*.dll")):
                     os.add_dll_directory(p)
 
 
-from fiona.collection import BytesCollection, Collection
-from fiona.drvsupport import supported_drivers
-from fiona.env import ensure_env_with_credentials, Env
-from fiona.errors import FionaDeprecationWarning
-from fiona._env import driver_count
 from fiona._env import (
     calc_gdal_version_num,
-    get_gdal_version_num,
     get_gdal_release_name,
+    get_gdal_version_num,
     get_gdal_version_tuple,
 )
+from fiona._env import driver_count
+from fiona._show_versions import show_versions
+from fiona.collection import BytesCollection, Collection
+from fiona.drvsupport import supported_drivers
+from fiona.env import ensure_env_with_credentials, Env
+from fiona.errors import FionaDeprecationWarning
 from fiona.io import MemoryFile
+from fiona.model import Feature, Geometry, Properties
 from fiona.ogrext import (
+    FIELD_TYPES_MAP,
     _bounds,
-    _listlayers,
     _listdir,
-    FIELD_TYPES_MAP,
+    _listlayers,
     _remove,
     _remove_layer,
 )
 from fiona.path import ParsedPath, parse_path, vsi_path
 from fiona.vfs import parse_paths as vfs_parse_paths
-from fiona._show_versions import show_versions
 
 # These modules are imported by fiona.ogrext, but are also import here to
 # help tools like cx_Freeze find them automatically
 from fiona import _geometry, _err, rfc3339
 import uuid
 
 
-__all__ = ['bounds', 'listlayers', 'listdir', 'open', 'prop_type', 'prop_width']
-__version__ = "1.9b1"
+__all__ = [
+    "Feature",
+    "Geometry",
+    "Properties",
+    "bounds",
+    "listlayers",
+    "listdir",
+    "open",
+    "prop_type",
+    "prop_width",
+]
+__version__ = "1.9b2"
 __gdal_version__ = get_gdal_release_name()
 
 gdal_version = get_gdal_version_tuple()
 
 log = logging.getLogger(__name__)
 log.addHandler(logging.NullHandler())
```

### Comparing `Fiona-1.9b1/fiona/_cpl.pxd` & `Fiona-1.9b2/fiona/_cpl.pxd`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/_env.pyx` & `Fiona-1.9b2/fiona/_env.pyx`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/_err.pyx` & `Fiona-1.9b2/fiona/_err.pyx`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/_geometry.pxd` & `Fiona-1.9b2/fiona/_geometry.pxd`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/_geometry.pyx` & `Fiona-1.9b2/fiona/_geometry.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import absolute_import
 
 include "gdal.pxi"
 
 import logging
 
 from fiona.errors import UnsupportedGeometryTypeError
-from fiona.model import _guard_model_object, GEOMETRY_TYPES, Geometry, OGRGeometryType
+from fiona.model import decode_object, GEOMETRY_TYPES, Geometry, OGRGeometryType
 from fiona._err cimport exc_wrap_int
 
 
 class NullHandler(logging.Handler):
     def emit(self, record):
         pass
 
@@ -359,12 +359,12 @@
             return self._buildGeometryCollection(geometries)
         else:
             raise UnsupportedGeometryTypeError("Unsupported geometry type %s" % typename)
 
 
 def geometryRT(geom):
     # For testing purposes only, leaks the JSON data
-    geometry = _guard_model_object(geom)
+    geometry = decode_object(geom)
     cdef void *cogr_geometry = OGRGeomBuilder().build(geometry)
     result = GeomBuilder().build(cogr_geometry)
     _deleteOgrGeom(cogr_geometry)
     return result
```

### Comparing `Fiona-1.9b1/fiona/_shim.pxd` & `Fiona-1.9b2/fiona/_shim.pxd`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/_shim.pyx` & `Fiona-1.9b2/fiona/_shim.pyx`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/_show_versions.py` & `Fiona-1.9b2/fiona/_show_versions.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/_transform.pyx` & `Fiona-1.9b2/fiona/_transform.pyx`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/collection.py` & `Fiona-1.9b2/fiona/collection.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/crs.pyx` & `Fiona-1.9b2/fiona/crs.pyx`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/drvsupport.py` & `Fiona-1.9b2/fiona/drvsupport.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/enums.py` & `Fiona-1.9b2/fiona/enums.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/env.py` & `Fiona-1.9b2/fiona/env.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/errors.py` & `Fiona-1.9b2/fiona/errors.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/fio/bounds.py` & `Fiona-1.9b2/fiona/fio/bounds.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """$ fio bounds"""
 
-
 import json
-import logging
 
 import click
 from cligj import precision_opt, use_rs_opt
 
 import fiona
 from fiona.fio.helpers import obj_gen
 from fiona.fio import with_context_env
@@ -34,68 +32,58 @@
 
     To print identifiers for input objects along with their bounds
     as a {id: identifier, bbox: bounds} JSON object, use --with-id.
 
     To print the input objects themselves along with their bounds
     as GeoJSON object, use --with-obj. This has the effect of updating
     input objects with {id: identifier, bbox: bounds}.
+
     """
-    logger = logging.getLogger(__name__)
     stdin = click.get_text_stream('stdin')
+    source = obj_gen(stdin)
 
-    try:
-        source = obj_gen(stdin)
-
-        for i, obj in enumerate(source):
-            obj_id = obj.get('id', 'collection:' + str(i))
-            xs = []
-            ys = []
-            features = obj.get('features') or [obj]
-
-            for j, feat in enumerate(features):
-                feat_id = feat.get('id', 'feature:' + str(i))
-                w, s, e, n = fiona.bounds(feat)
-
-                if precision > 0:
-                    w, s, e, n = (round(v, precision)
-                                  for v in (w, s, e, n))
-                if explode:
-
-                    if with_id:
-                        rec = {
-                            'parent': obj_id,
-                            'id': feat_id,
-                            'bbox': (w, s, e, n)}
-                    elif with_obj:
-                        feat.update(parent=obj_id, bbox=(w, s, e, n))
-                        rec = feat
-                    else:
-                        rec = (w, s, e, n)
-
-                    if use_rs:
-                        click.echo('\x1e', nl=False)
-
-                    click.echo(json.dumps(rec, cls=ObjectEncoder))
-
-                else:
-                    xs.extend([w, e])
-                    ys.extend([s, n])
-
-            if not explode:
-                w, s, e, n = (min(xs), min(ys), max(xs), max(ys))
+    for i, obj in enumerate(source):
+        obj_id = obj.get("id", "collection:" + str(i))
+        xs = []
+        ys = []
+        features = obj.get("features") or [obj]
+
+        for j, feat in enumerate(features):
+            feat_id = feat.get("id", "feature:" + str(i))
+            w, s, e, n = fiona.bounds(feat)
+
+            if precision > 0:
+                w, s, e, n = (round(v, precision) for v in (w, s, e, n))
+            if explode:
 
                 if with_id:
-                    rec = {'id': obj_id, 'bbox': (w, s, e, n)}
+                    rec = {"parent": obj_id, "id": feat_id, "bbox": (w, s, e, n)}
                 elif with_obj:
-                    obj.update(id=obj_id, bbox=(w, s, e, n))
-                    rec = obj
+                    feat.update(parent=obj_id, bbox=(w, s, e, n))
+                    rec = feat
                 else:
                     rec = (w, s, e, n)
 
                 if use_rs:
                     click.echo('\x1e', nl=False)
 
                 click.echo(json.dumps(rec, cls=ObjectEncoder))
 
-    except Exception:
-        logger.exception("Exception caught during processing")
-        raise click.Abort()
+            else:
+                xs.extend([w, e])
+                ys.extend([s, n])
+
+        if not explode:
+            w, s, e, n = (min(xs), min(ys), max(xs), max(ys))
+
+            if with_id:
+                rec = {"id": obj_id, "bbox": (w, s, e, n)}
+            elif with_obj:
+                obj.update(id=obj_id, bbox=(w, s, e, n))
+                rec = obj
+            else:
+                rec = (w, s, e, n)
+
+            if use_rs:
+                click.echo("\x1e", nl=False)
+
+            click.echo(json.dumps(rec, cls=ObjectEncoder))
```

### Comparing `Fiona-1.9b1/fiona/fio/calc.py` & `Fiona-1.9b2/fiona/fio/calc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import division
 import json
-import logging
 
 import click
 from cligj import use_rs_opt
 
 from .helpers import obj_gen, eval_feature_expression
 from fiona.fio import with_context_env
 from fiona.model import ObjectEncoder
@@ -35,31 +34,31 @@
     as the specified property_name. Existing properties will not
     be overwritten by default (an Exception is raised).
 
     Example
 
     \b
     $ fio cat data.shp | fio calc sumAB  "f.properties.A + f.properties.B"
+
     """
-    logger = logging.getLogger(__name__)
     stdin = click.get_text_stream('stdin')
-    try:
-        source = obj_gen(stdin)
-        for i, obj in enumerate(source):
-            features = obj.get('features') or [obj]
-            for j, feat in enumerate(features):
-
-                if not overwrite and property_name in feat['properties']:
-                    raise click.UsageError(
-                        '{0} already exists in properties; '
-                        'rename or use --overwrite'.format(property_name))
-
-                feat['properties'][property_name] = eval_feature_expression(
-                    feat, expression)
-
-                if use_rs:
-                    click.echo('\x1e', nl=False)
-                click.echo(json.dumps(feat, cls=ObjectEncoder))
-
-    except Exception:
-        logger.exception("Exception caught during processing")
-        raise click.Abort()
+    source = obj_gen(stdin)
+
+    for i, obj in enumerate(source):
+        features = obj.get("features") or [obj]
+
+        for j, feat in enumerate(features):
+
+            if not overwrite and property_name in feat["properties"]:
+                raise click.UsageError(
+                    "{0} already exists in properties; "
+                    "rename or use --overwrite".format(property_name)
+                )
+
+            feat["properties"][property_name] = eval_feature_expression(
+                feat, expression
+            )
+
+            if use_rs:
+                click.echo("\x1e", nl=False)
+
+            click.echo(json.dumps(feat, cls=ObjectEncoder))
```

### Comparing `Fiona-1.9b1/fiona/fio/cat.py` & `Fiona-1.9b2/fiona/fio/cat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """fio-cat"""
 
 import json
-import logging
 import warnings
 
 import click
 import cligj
 
 import fiona
 from fiona.transform import transform_geom
@@ -76,16 +75,14 @@
     Concatenate and print the features of input datasets as a sequence of
     GeoJSON features.
 
     When working with a multi-layer dataset the first layer is used by default.
     Use the '--layer' option to select a different layer.
 
     """
-    log = logging.getLogger(__name__)
-
     dump_kwds = {"sort_keys": True}
     if indent:
         dump_kwds["indent"] = indent
     if compact:
         dump_kwds["separators"] = (",", ":")
 
     # Validate file idexes provided in --layer option
@@ -100,19 +97,21 @@
 
     try:
         if bbox:
             try:
                 bbox = tuple(map(float, bbox.split(",")))
             except ValueError:
                 bbox = json.loads(bbox)
+
         for i, path in enumerate(files, 1):
             for lyr in layer[str(i)]:
                 with fiona.open(path, layer=lyr) as src:
                     for i, feat in src.items(bbox=bbox, where=where):
                         geom = feat.geometry
+
                         if dst_crs:
                             geom = transform_geom(
                                 src.crs,
                                 dst_crs,
                                 geom,
                                 antimeridian_cutting=cut_at_antimeridian,
                             )
@@ -122,16 +121,15 @@
 
                         feat = Feature(
                             id=feat.id,
                             properties=feat.properties,
                             geometry=geom,
                             bbox=fiona.bounds(geom),
                         )
+
                         if use_rs:
                             click.echo("\x1e", nl=False)
+
                         click.echo(json.dumps(feat, cls=ObjectEncoder, **dump_kwds))
 
     except AttributeFilterError as e:
         raise click.BadParameter("'where' clause is invalid: " + str(e))
-    except Exception:
-        log.exception("Exception caught during processing")
-        raise click.Abort()
```

### Comparing `Fiona-1.9b1/fiona/fio/collect.py` & `Fiona-1.9b2/fiona/fio/collect.py`

 * *Files 5% similar despite different names*

```diff
@@ -146,110 +146,101 @@
         else:
 
             def feature_text_gen():
                 yield first_line
                 for line in stdin:
                     yield line
 
-    try:
-        source = feature_text_gen()
+    source = feature_text_gen()
 
-        if record_buffered:
-            # Buffer GeoJSON data at the feature level for smaller
-            # memory footprint.
-            indented = bool(indent)
-            rec_indent = "\n" + " " * (2 * (indent or 0))
-
-            collection = {"type": "FeatureCollection", "features": []}
+    if record_buffered:
+        # Buffer GeoJSON data at the feature level for smaller
+        # memory footprint.
+        indented = bool(indent)
+        rec_indent = "\n" + " " * (2 * (indent or 0))
+
+        collection = {"type": "FeatureCollection", "features": []}
+        if with_ld_context:
+            collection["@context"] = helpers.make_ld_context(add_ld_context_item)
+
+        head, tail = json.dumps(collection, cls=ObjectEncoder, **dump_kwds).split("[]")
+
+        sink.write(head)
+        sink.write("[")
+
+        # Try the first record.
+        try:
+            i, first = 0, next(source)
             if with_ld_context:
-                collection["@context"] = helpers.make_ld_context(add_ld_context_item)
-
-            head, tail = json.dumps(collection, cls=ObjectEncoder, **dump_kwds).split(
-                "[]"
-            )
-
-            sink.write(head)
-            sink.write("[")
+                first = helpers.id_record(first)
+            if indented:
+                sink.write(rec_indent)
+            sink.write(first.replace("\n", rec_indent))
+        except StopIteration:
+            pass
+        except Exception as exc:
+            # Ignoring errors is *not* the default.
+            if ignore_errors:
+                logger.error(
+                    "failed to serialize file record %d (%s), " "continuing", i, exc
+                )
+            else:
+                # Log error and close up the GeoJSON, leaving it
+                # more or less valid no matter what happens above.
+                logger.critical(
+                    "failed to serialize file record %d (%s), " "quiting", i, exc
+                )
+                sink.write("]")
+                sink.write(tail)
+                if indented:
+                    sink.write("\n")
+                raise
 
-            # Try the first record.
+        # Because trailing commas aren't valid in JSON arrays
+        # we'll write the item separator before each of the
+        # remaining features.
+        for i, rec in enumerate(source, 1):
             try:
-                i, first = 0, next(source)
                 if with_ld_context:
-                    first = helpers.id_record(first)
+                    rec = helpers.id_record(rec)
                 if indented:
                     sink.write(rec_indent)
-                sink.write(first.replace("\n", rec_indent))
-            except StopIteration:
-                pass
+                sink.write(item_sep)
+                sink.write(rec.replace("\n", rec_indent))
             except Exception as exc:
-                # Ignoring errors is *not* the default.
                 if ignore_errors:
                     logger.error(
-                        "failed to serialize file record %d (%s), " "continuing", i, exc
+                        "failed to serialize file record %d (%s), " "continuing",
+                        i,
+                        exc,
                     )
                 else:
-                    # Log error and close up the GeoJSON, leaving it
-                    # more or less valid no matter what happens above.
                     logger.critical(
-                        "failed to serialize file record %d (%s), " "quiting", i, exc
+                        "failed to serialize file record %d (%s), " "quiting",
+                        i,
+                        exc,
                     )
                     sink.write("]")
                     sink.write(tail)
                     if indented:
                         sink.write("\n")
                     raise
 
-            # Because trailing commas aren't valid in JSON arrays
-            # we'll write the item separator before each of the
-            # remaining features.
-            for i, rec in enumerate(source, 1):
-                try:
-                    if with_ld_context:
-                        rec = helpers.id_record(rec)
-                    if indented:
-                        sink.write(rec_indent)
-                    sink.write(item_sep)
-                    sink.write(rec.replace("\n", rec_indent))
-                except Exception as exc:
-                    if ignore_errors:
-                        logger.error(
-                            "failed to serialize file record %d (%s), " "continuing",
-                            i,
-                            exc,
-                        )
-                    else:
-                        logger.critical(
-                            "failed to serialize file record %d (%s), " "quiting",
-                            i,
-                            exc,
-                        )
-                        sink.write("]")
-                        sink.write(tail)
-                        if indented:
-                            sink.write("\n")
-                        raise
-
-            # Close up the GeoJSON after writing all features.
-            sink.write("]")
-            sink.write(tail)
-            if indented:
-                sink.write("\n")
-
-        else:
-            # Buffer GeoJSON data at the collection level. The default.
-            collection = {"type": "FeatureCollection", "features": []}
-            if with_ld_context:
-                collection["@context"] = helpers.make_ld_context(add_ld_context_item)
-
-            head, tail = json.dumps(collection, cls=ObjectEncoder, **dump_kwds).split(
-                "[]"
-            )
-            sink.write(head)
-            sink.write("[")
-            sink.write(",".join(source))
-            sink.write("]")
-            sink.write(tail)
+        # Close up the GeoJSON after writing all features.
+        sink.write("]")
+        sink.write(tail)
+        if indented:
             sink.write("\n")
 
-    except Exception:
-        logger.exception("Exception caught during processing")
-        raise click.Abort()
+    else:
+        # Buffer GeoJSON data at the collection level. The default.
+        collection = {"type": "FeatureCollection", "features": []}
+        if with_ld_context:
+            collection["@context"] = helpers.make_ld_context(add_ld_context_item)
+
+        head, tail = json.dumps(collection, cls=ObjectEncoder, **dump_kwds).split("[]")
+        sink.write(head)
+        sink.write("[")
+        sink.write(",".join(source))
+        sink.write("]")
+        sink.write(tail)
+        sink.write("\n")
```

### Comparing `Fiona-1.9b1/fiona/fio/distrib.py` & `Fiona-1.9b2/fiona/fio/distrib.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """$ fio distrib"""
 
-
 import json
-import logging
 
 import click
 import cligj
 
 from fiona.fio import helpers, with_context_env
 from fiona.model import ObjectEncoder
 
@@ -17,27 +15,21 @@
 @with_context_env
 def distrib(ctx, use_rs):
     """Distribute features from a collection.
 
     Print the features of GeoJSON objects read from stdin.
 
     """
-    logger = logging.getLogger(__name__)
     stdin = click.get_text_stream('stdin')
+    source = helpers.obj_gen(stdin)
 
-    try:
-        source = helpers.obj_gen(stdin)
-        for i, obj in enumerate(source):
-            obj_id = obj.get('id', 'collection:' + str(i))
-            features = obj.get('features') or [obj]
-            for j, feat in enumerate(features):
-                if obj.get('type') == 'FeatureCollection':
-                    feat['parent'] = obj_id
-                feat_id = feat.get('id', 'feature:' + str(i))
-                feat['id'] = feat_id
-                if use_rs:
-                    click.echo('\x1e', nl=False)
-                click.echo(json.dumps(feat, cls=ObjectEncoder))
-
-    except Exception:
-        logger.exception("Exception caught during processing")
-        raise click.Abort()
+    for i, obj in enumerate(source):
+        obj_id = obj.get("id", "collection:" + str(i))
+        features = obj.get("features") or [obj]
+        for j, feat in enumerate(features):
+            if obj.get("type") == "FeatureCollection":
+                feat["parent"] = obj_id
+            feat_id = feat.get("id", "feature:" + str(i))
+            feat["id"] = feat_id
+            if use_rs:
+                click.echo("\x1e", nl=False)
+            click.echo(json.dumps(feat, cls=ObjectEncoder))
```

### Comparing `Fiona-1.9b1/fiona/fio/dump.py` & `Fiona-1.9b2/fiona/fio/dump.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """fio-dump"""
 
-
 from functools import partial
 import json
 import logging
 
 import click
 import cligj
 
@@ -59,124 +58,122 @@
         open_kwds['layer'] = layer
 
     def transformer(crs, feat):
         tg = partial(transform_geom, crs, 'EPSG:4326',
                      antimeridian_cutting=True, precision=precision)
         return Feature(id=feat.id, properties=feat.properties, geometry=tg(feat.geometry))
 
-    try:
-        with fiona.open(input, **open_kwds) as source:
-            meta = source.meta
-            meta['fields'] = dict(source.schema['properties'].items())
-
-            if record_buffered:
-                # Buffer GeoJSON data at the feature level for smaller
-                # memory footprint.
-                indented = bool(indent)
-                rec_indent = "\n" + " " * (2 * (indent or 0))
-
-                collection = {
-                    'type': 'FeatureCollection',
-                    'fiona:schema': meta['schema'],
-                    'fiona:crs': meta['crs'],
-                    'features': []}
+    with fiona.open(input, **open_kwds) as source:
+        meta = source.meta
+        meta["fields"] = dict(source.schema["properties"].items())
+
+        if record_buffered:
+            # Buffer GeoJSON data at the feature level for smaller
+            # memory footprint.
+            indented = bool(indent)
+            rec_indent = "\n" + " " * (2 * (indent or 0))
+
+            collection = {
+                "type": "FeatureCollection",
+                "fiona:schema": meta["schema"],
+                "fiona:crs": meta["crs"],
+                "features": [],
+            }
+            if with_ld_context:
+                collection["@context"] = helpers.make_ld_context(add_ld_context_item)
+
+            head, tail = json.dumps(collection, **dump_kwds).split("[]")
+
+            sink.write(head)
+            sink.write("[")
+
+            itr = iter(source)
+
+            # Try the first record.
+            try:
+                i, first = 0, next(itr)
+                first = transformer(first)
                 if with_ld_context:
-                    collection['@context'] = helpers.make_ld_context(
-                        add_ld_context_item)
-
-                head, tail = json.dumps(
-                    collection, **dump_kwds).split('[]')
-
-                sink.write(head)
-                sink.write("[")
-
-                itr = iter(source)
+                    first = helpers.id_record(first)
+                if indented:
+                    sink.write(rec_indent)
+                sink.write(
+                    json.dumps(first, cls=ObjectEncoder, **dump_kwds).replace(
+                        "\n", rec_indent
+                    )
+                )
+            except StopIteration:
+                pass
+            except Exception as exc:
+                # Ignoring errors is *not* the default.
+                if ignore_errors:
+                    logger.error(
+                        "failed to serialize file record %d (%s), " "continuing", i, exc
+                    )
+                else:
+                    # Log error and close up the GeoJSON, leaving it
+                    # more or less valid no matter what happens above.
+                    logger.critical(
+                        "failed to serialize file record %d (%s), " "quiting", i, exc
+                    )
+                    sink.write("]")
+                    sink.write(tail)
+                    if indented:
+                        sink.write("\n")
+                    raise
 
-                # Try the first record.
+            # Because trailing commas aren't valid in JSON arrays
+            # we'll write the item separator before each of the
+            # remaining features.
+            for i, rec in enumerate(itr, 1):
+                rec = transformer(rec)
                 try:
-                    i, first = 0, next(itr)
-                    first = transformer(first)
                     if with_ld_context:
-                        first = helpers.id_record(first)
+                        rec = helpers.id_record(rec)
                     if indented:
                         sink.write(rec_indent)
-                    sink.write(json.dumps(
-                        first, cls=ObjectEncoder, **dump_kwds).replace("\n", rec_indent))
-                except StopIteration:
-                    pass
+                    sink.write(item_sep)
+                    sink.write(
+                        json.dumps(rec, cls=ObjectEncoder, **dump_kwds).replace(
+                            "\n", rec_indent
+                        )
+                    )
                 except Exception as exc:
-                    # Ignoring errors is *not* the default.
                     if ignore_errors:
                         logger.error(
                             "failed to serialize file record %d (%s), "
                             "continuing",
                             i, exc)
                     else:
-                        # Log error and close up the GeoJSON, leaving it
-                        # more or less valid no matter what happens above.
                         logger.critical(
                             "failed to serialize file record %d (%s), "
                             "quiting",
                             i, exc)
                         sink.write("]")
                         sink.write(tail)
                         if indented:
                             sink.write("\n")
                         raise
 
-                # Because trailing commas aren't valid in JSON arrays
-                # we'll write the item separator before each of the
-                # remaining features.
-                for i, rec in enumerate(itr, 1):
-                    rec = transformer(rec)
-                    try:
-                        if with_ld_context:
-                            rec = helpers.id_record(rec)
-                        if indented:
-                            sink.write(rec_indent)
-                        sink.write(item_sep)
-                        sink.write(json.dumps(
-                            rec, cls=ObjectEncoder, **dump_kwds).replace("\n", rec_indent))
-                    except Exception as exc:
-                        if ignore_errors:
-                            logger.error(
-                                "failed to serialize file record %d (%s), "
-                                "continuing",
-                                i, exc)
-                        else:
-                            logger.critical(
-                                "failed to serialize file record %d (%s), "
-                                "quiting",
-                                i, exc)
-                            sink.write("]")
-                            sink.write(tail)
-                            if indented:
-                                sink.write("\n")
-                            raise
-
-                # Close up the GeoJSON after writing all features.
-                sink.write("]")
-                sink.write(tail)
-                if indented:
-                    sink.write("\n")
-
+            # Close up the GeoJSON after writing all features.
+            sink.write("]")
+            sink.write(tail)
+            if indented:
+                sink.write("\n")
+
+        else:
+            # Buffer GeoJSON data at the collection level. The default.
+            collection = {
+                "type": "FeatureCollection",
+                "fiona:schema": meta["schema"],
+                "fiona:crs": meta["crs"].to_string(),
+            }
+            if with_ld_context:
+                collection["@context"] = helpers.make_ld_context(add_ld_context_item)
+                collection["features"] = [
+                    helpers.id_record(transformer(rec)) for rec in source
+                ]
             else:
-                # Buffer GeoJSON data at the collection level. The default.
-                collection = {
-                    "type": "FeatureCollection",
-                    "fiona:schema": meta["schema"],
-                    "fiona:crs": meta["crs"].to_string(),
-                }
-                if with_ld_context:
-                    collection['@context'] = helpers.make_ld_context(
-                        add_ld_context_item)
-                    collection['features'] = [
-                        helpers.id_record(transformer(rec))
-                        for rec in source]
-                else:
-                    collection['features'] = [
-                        transformer(source.crs, rec) for rec in source]
-                json.dump(collection, sink, cls=ObjectEncoder, **dump_kwds)
-
-    except Exception:
-        logger.exception("Exception caught during processing")
-        raise click.Abort()
+                collection["features"] = [
+                    transformer(source.crs, rec) for rec in source
+                ]
+            json.dump(collection, sink, cls=ObjectEncoder, **dump_kwds)
```

### Comparing `Fiona-1.9b1/fiona/fio/env.py` & `Fiona-1.9b2/fiona/fio/env.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/fio/filter.py` & `Fiona-1.9b2/fiona/fio/filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 """$ fio filter"""
 
 import json
-import logging
 
 import click
 from cligj import use_rs_opt
 
 from fiona.fio.helpers import obj_gen, eval_feature_expression
 from fiona.fio import with_context_env
 
 
-logger = logging.getLogger(__name__)
-
-
 @click.command()
 @click.argument('filter_expression')
 @use_rs_opt
 @click.pass_context
 @with_context_env
 def filter(ctx, filter_expression, use_rs):
     """
@@ -37,23 +33,18 @@
     \b
         $ fio cat data.shp \\
             | fio filter "f.properties.area > 1000.0" \\
             | fio collect > large_polygons.geojson
 
     """
     stdin = click.get_text_stream('stdin')
+    source = obj_gen(stdin)
 
-    try:
-        source = obj_gen(stdin)
-        for i, obj in enumerate(source):
-            features = obj.get('features') or [obj]
-            for j, feat in enumerate(features):
-                if not eval_feature_expression(feat, filter_expression):
-                    continue
-
-                if use_rs:
-                    click.echo('\x1e', nl=False)
-                click.echo(json.dumps(feat))
-
-    except Exception:
-        logger.exception("Exception caught during processing")
-        raise click.Abort()
+    for i, obj in enumerate(source):
+        features = obj.get("features") or [obj]
+        for j, feat in enumerate(features):
+            if not eval_feature_expression(feat, filter_expression):
+                continue
+
+            if use_rs:
+                click.echo("\x1e", nl=False)
+            click.echo(json.dumps(feat))
```

### Comparing `Fiona-1.9b1/fiona/fio/helpers.py` & `Fiona-1.9b2/fiona/fio/helpers.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/fio/info.py` & `Fiona-1.9b2/fiona/fio/info.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from cligj import indent_opt
 
 import fiona
 import fiona.crs
 from fiona.errors import DriverError
 from fiona.fio import options, with_context_env
 
+logger = logging.getLogger(__name__)
+
 
 @click.command()
 # One or more files.
 @click.argument('input', required=True)
 @click.option('--layer', metavar="INDEX|NAME", callback=options.cb_layer,
               help="Print information about a specific layer.  The first "
                    "layer is used by default.  Layers use zero-based "
@@ -38,40 +40,38 @@
 @with_context_env
 def info(ctx, input, indent, meta_member, layer):
     """
     Print information about a dataset.
 
     When working with a multi-layer dataset the first layer is used by default.
     Use the '--layer' option to select a different layer.
-    """
 
-    logger = logging.getLogger(__name__)
-    try:
-        with fiona.open(input, layer=layer) as src:
-            info = src.meta
-            info.update(name=src.name)
-
-            try:
-                info.update(bounds=src.bounds)
-            except DriverError:
-                info.update(bounds=None)
-                logger.debug("Setting 'bounds' to None - driver was not able to calculate bounds")
-
-            try:
-                info.update(count=len(src))
-            except TypeError:
-                info.update(count=None)
-                logger.debug("Setting 'count' to None/null - layer does not support counting")
-
-            info["crs"] = src.crs.to_string()
-
-            if meta_member:
-                if isinstance(info[meta_member], (list, tuple)):
-                    click.echo(" ".join(map(str, info[meta_member])))
-                else:
-                    click.echo(info[meta_member])
+    """
+    with fiona.open(input, layer=layer) as src:
+        info = src.meta
+        info.update(name=src.name)
+
+        try:
+            info.update(bounds=src.bounds)
+        except DriverError:
+            info.update(bounds=None)
+            logger.debug(
+                "Setting 'bounds' to None - driver was not able to calculate bounds"
+            )
+
+        try:
+            info.update(count=len(src))
+        except TypeError:
+            info.update(count=None)
+            logger.debug(
+                "Setting 'count' to None/null - layer does not support counting"
+            )
+
+        info["crs"] = src.crs.to_string()
+
+        if meta_member:
+            if isinstance(info[meta_member], (list, tuple)):
+                click.echo(" ".join(map(str, info[meta_member])))
             else:
-                click.echo(json.dumps(info, indent=indent))
-
-    except Exception:
-        logger.exception("Exception caught during processing")
-        raise click.Abort()
+                click.echo(info[meta_member])
+        else:
+            click.echo(json.dumps(info, indent=indent))
```

### Comparing `Fiona-1.9b1/fiona/fio/insp.py` & `Fiona-1.9b2/fiona/fio/insp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """$ fio insp"""
 
 
 import code
-import logging
 import sys
 
 import click
 
 import fiona
 from fiona.fio import with_context_env
 
@@ -14,32 +13,29 @@
 @click.command(short_help="Open a dataset and start an interpreter.")
 @click.argument('src_path', required=True)
 @click.option('--ipython', 'interpreter', flag_value='ipython',
               help="Use IPython as interpreter.")
 @click.pass_context
 @with_context_env
 def insp(ctx, src_path, interpreter):
-    """Open a collection within an interactive interpreter.
-    """
-    logger = logging.getLogger(__name__)
-    banner = 'Fiona %s Interactive Inspector (Python %s)\n' \
-             'Type "src.schema", "next(src)", or "help(src)" ' \
-             'for more information.' \
-             % (fiona.__version__, '.'.join(map(str, sys.version_info[:3])))
-
-    try:
-        with fiona.open(src_path) as src:
-            scope = locals()
-            if not interpreter:
-                code.interact(banner, local=scope)
-            elif interpreter == 'ipython':
-                import IPython
-                IPython.InteractiveShell.banner1 = banner
-                IPython.start_ipython(argv=[], user_ns=scope)
-            else:
-                raise click.ClickException(
-                    'Interpreter {} is unsupported or missing '
-                    'dependencies'.format(interpreter))
-
-    except Exception:
-        logger.exception("Exception caught during processing")
-        raise click.Abort()
+    """Open a collection within an interactive interpreter."""
+    banner = (
+        "Fiona %s Interactive Inspector (Python %s)\n"
+        'Type "src.schema", "next(src)", or "help(src)" '
+        "for more information."
+        % (fiona.__version__, ".".join(map(str, sys.version_info[:3])))
+    )
+
+    with fiona.open(src_path) as src:
+        scope = locals()
+        if not interpreter:
+            code.interact(banner, local=scope)
+        elif interpreter == "ipython":
+            import IPython
+
+            IPython.InteractiveShell.banner1 = banner
+            IPython.start_ipython(argv=[], user_ns=scope)
+        else:
+            raise click.ClickException(
+                "Interpreter {} is unsupported or missing "
+                "dependencies".format(interpreter)
+            )
```

### Comparing `Fiona-1.9b1/fiona/fio/load.py` & `Fiona-1.9b2/fiona/fio/load.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """$ fio load"""
 
-
 from functools import partial
-import logging
 
 import click
 import cligj
 
 import fiona
 from fiona.fio import options, with_context_env
 from fiona.model import Feature, Geometry
@@ -76,16 +74,14 @@
 def load(ctx, output, driver, src_crs, dst_crs, features, layer, creation_options):
     """Load features from JSON to a file in another format.
 
     The input is a GeoJSON feature collection or optionally a sequence of
     GeoJSON feature objects.
 
     """
-    logger = logging.getLogger(__name__)
-
     dst_crs = dst_crs or src_crs
 
     if src_crs and dst_crs and src_crs != dst_crs:
         transformer = partial(
             transform_geom, src_crs, dst_crs, antimeridian_cutting=True
         )
     else:
@@ -97,41 +93,43 @@
         """Convert stream of JSON to features.
 
         Yields
         ------
         Feature
 
         """
-        for feat in features:
-            feat["geometry"] = transformer(Geometry.from_dict(**feat["geometry"]))
-            yield Feature.from_dict(**feat)
+        try:
+            for feat in features:
+                feat["geometry"] = transformer(Geometry.from_dict(**feat["geometry"]))
+                yield Feature.from_dict(**feat)
+        except TypeError:
+            raise click.ClickException("Invalid input.")
 
-    try:
-        source = feature_gen()
+    source = feature_gen()
 
-        # Use schema of first feature as a template.
-        # TODO: schema specified on command line?
+    # Use schema of first feature as a template.
+    # TODO: schema specified on command line?
+    try:
         first = next(source)
-        # print(first, first.geometry)
-        schema = {"geometry": first.geometry.type}
-        schema["properties"] = dict(
-            [
-                (k, FIELD_TYPES_MAP_REV.get(type(v)) or "str")
-                for k, v in first.properties.items()
-            ]
-        )
+    except TypeError:
+        raise click.ClickException("Invalid input.")
 
-        with fiona.open(
-            output,
-            "w",
-            driver=driver,
-            crs=dst_crs,
-            schema=schema,
-            layer=layer,
-            **creation_options
-        ) as dst:
-            dst.write(first)
-            dst.writerecords(source)
-
-    except Exception:
-        logger.exception("Exception caught during processing")
-        raise click.Abort()
+    # print(first, first.geometry)
+    schema = {"geometry": first.geometry.type}
+    schema["properties"] = dict(
+        [
+            (k, FIELD_TYPES_MAP_REV.get(type(v)) or "str")
+            for k, v in first.properties.items()
+        ]
+    )
+
+    with fiona.open(
+        output,
+        "w",
+        driver=driver,
+        crs=dst_crs,
+        schema=schema,
+        layer=layer,
+        **creation_options
+    ) as dst:
+        dst.write(first)
+        dst.writerecords(source)
```

### Comparing `Fiona-1.9b1/fiona/fio/main.py` & `Fiona-1.9b2/fiona/fio/main.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/fio/options.py` & `Fiona-1.9b2/fiona/fio/options.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/fio/rm.py` & `Fiona-1.9b2/fiona/fio/rm.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/gdal.pxi` & `Fiona-1.9b2/fiona/gdal.pxi`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/inspector.py` & `Fiona-1.9b2/fiona/inspector.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/io.py` & `Fiona-1.9b2/fiona/io.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/logutils.py` & `Fiona-1.9b2/fiona/logutils.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/meta.py` & `Fiona-1.9b2/fiona/meta.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/model.py` & `Fiona-1.9b2/fiona/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -190,16 +190,16 @@
     def __init__(self, coordinates=None, type=None, geometries=None, **data):
         self._delegate = _Geometry(
             coordinates=coordinates, type=type, geometries=geometries
         )
         super(Geometry, self).__init__(**data)
 
     @classmethod
-    def from_dict(cls, mapping=None, **kwargs):
-        data = dict(mapping or {}, **kwargs)
+    def from_dict(cls, ob=None, **kwargs):
+        data = dict(getattr(ob, "__geo_interface__", ob) or {}, **kwargs)
         return Geometry(
             coordinates=data.pop("coordinates", None),
             type=data.pop("type", None),
             geometries=[
                 Geometry.from_dict(**part)
                 for part in data.pop("geometries", None) or []
             ],
@@ -235,14 +235,18 @@
         Returns
         -------
         list
 
         """
         return self._delegate.geometries
 
+    @property
+    def __geo_interface__(self):
+        return ObjectEncoder().default(self)
+
 
 class _Feature(object):
     def __init__(self, geometry=None, id=None, properties=None):
         self.geometry = geometry
         self.id = id
         self.properties = properties
 
@@ -262,16 +266,16 @@
     def __init__(self, geometry=None, id=None, properties=None, **data):
         if properties is None:
             properties = Properties()
         self._delegate = _Feature(geometry=geometry, id=id, properties=properties)
         super(Feature, self).__init__(**data)
 
     @classmethod
-    def from_dict(cls, mapping=None, **kwargs):
-        data = dict(mapping or {}, **kwargs)
+    def from_dict(cls, ob=None, **kwargs):
+        data = dict(getattr(ob, "__geo_interface__", ob) or {}, **kwargs)
         geom_data = data.pop("geometry", None)
 
         if isinstance(geom_data, Geometry):
             geom = geom_data
         else:
             geom = Geometry.from_dict(**geom_data) if geom_data is not None else None
 
@@ -305,26 +309,26 @@
 
     @property
     def id(self):
         """The feature's id
 
         Returns
         ------
-        obejct
+        object
 
         """
         return self._delegate.id
 
     @property
     def properties(self):
         """The feature's properties
 
         Returns
         -------
-        Object
+        object
 
         """
         return self._delegate.properties
 
     @property
     def type(self):
         """The Feature's type
@@ -332,14 +336,18 @@
         Returns
         -------
         str
 
         """
         return "Feature"
 
+    @property
+    def __geo_interface__(self):
+        return ObjectEncoder().default(self)
+
 
 class Properties(Object):
     """A GeoJSON-like feature's properties"""
 
     def __init__(self, **kwds):
         super(Properties, self).__init__(**kwds)
 
@@ -376,38 +384,28 @@
         A decoded dict.
 
     Returns
     -------
     Feature, Geometry, or dict
 
     """
-    if (obj.get("type", None) == "Feature") or "geometry" in obj:
-        return Feature.from_dict(**obj)
-    elif obj.get("type", None) in list(GEOMETRY_TYPES.values())[:8]:
-        return Geometry.from_dict(**obj)
-    else:
+    if isinstance(obj, Object):
         return obj
+    else:
+        obj = obj.get("__geo_interface__", obj)
+
+        if (obj.get("type", None) == "Feature") or "geometry" in obj:
+            return Feature.from_dict(**obj)
+        elif obj.get("type", None) in list(GEOMETRY_TYPES.values())[:8]:
+            return Geometry.from_dict(**obj)
+        else:
+            return obj
 
 
 def to_dict(val):
     """Converts an object to a dict"""
     try:
         obj = ObjectEncoder().default(val)
     except TypeError:
         return val
     else:
         return obj
-
-
-def _guard_model_object(obj):
-    """Convert dict to Geometry or Feature.
-
-    For use during the 1.9-2.0 transition. Will be removed in 2.0.
-
-    """
-    if not isinstance(obj, Object):
-        warn(
-            "Support for feature and geometry dicts is deprecated. Instances of Feature and Geometry will be required in 2.0.",
-            FionaDeprecationWarning,
-            stacklevel=2,
-        )
-    return decode_object(obj)
```

### Comparing `Fiona-1.9b1/fiona/ogrext.pyx` & `Fiona-1.9b2/fiona/ogrext.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 from fiona._geometry import GEOMETRY_TYPES
 from fiona import compat
 from fiona.compat import strencode
 from fiona.env import Env
 from fiona.errors import (
     DriverError, DriverIOError, SchemaError, CRSError, FionaValueError,
     TransactionError, GeometryTypeValidationError, DatasetDeleteError,
-    AttributeFilterError, FeatureWarning, FionaDeprecationWarning)
-from fiona.model import _guard_model_object, Feature, Geometry, Properties
+    AttributeFilterError, FeatureWarning, FionaDeprecationWarning, UnsupportedGeometryTypeError)
+from fiona.model import decode_object, Feature, Geometry, Properties
 from fiona.path import vsi_path
 from fiona.rfc3339 import parse_date, parse_datetime, parse_time
 from fiona.rfc3339 import FionaDateType, FionaDateTimeType, FionaTimeType
 from fiona.schema import FIELD_TYPES, FIELD_TYPES_MAP, normalize_field_type
 
 from libc.stdlib cimport malloc, free
 from libc.string cimport strcmp
@@ -115,22 +115,24 @@
             name_b = name.encode()
             name_c = name_b
             drv = GDALGetDriverByName(name_c)
             if drv != NULL:
                 drvs = CSLAddString(drvs, name_c)
 
     for k, v in options.items():
-        if v is None:
-            continue
-        k = k.upper().encode('utf-8')
-        if isinstance(v, bool):
-            v = ('ON' if v else 'OFF').encode('utf-8')
-        else:
-            v = str(v).encode('utf-8')
-        open_opts = CSLAddNameValue(open_opts, <const char *>k, <const char *>v)
+
+        if v is not None:
+            kb = k.upper().encode('utf-8')
+
+            if isinstance(v, bool):
+                vb = ('ON' if v else 'OFF').encode('utf-8')
+            else:
+                vb = str(v).encode('utf-8')
+
+            open_opts = CSLAddNameValue(open_opts, <const char *>kb, <const char *>vb)
 
     open_opts = CSLAddNameValue(open_opts, "VALIDATE_OPEN_OPTIONS", "NO")
 
     try:
         cogr_ds = exc_wrap_pointer(
             GDALOpenEx(path_c, flags, <const char *const *>drvs, <const char *const *>open_opts, NULL)
         )
@@ -144,21 +146,34 @@
         CSLDestroy(open_opts)
 
 
 cdef void* gdal_create(void* cogr_driver, const char *path_c, options) except NULL:
     cdef char **creation_opts = NULL
     cdef void *cogr_ds = NULL
 
+    db = <const char *>GDALGetDriverShortName(cogr_driver)
+
+    # To avoid a circular import.
+    from fiona import meta
+
+    option_keys = set(key.upper() for key in options.keys())
+    creation_option_keys = option_keys & set(meta.dataset_creation_options(db.decode("utf-8")))
+
     for k, v in options.items():
-        k = k.upper().encode('utf-8')
-        if isinstance(v, bool):
-            v = ('ON' if v else 'OFF').encode('utf-8')
-        else:
-            v = str(v).encode('utf-8')
-        creation_opts = CSLAddNameValue(creation_opts, <const char *>k, <const char *>v)
+
+        if k.upper() in creation_option_keys:
+
+            kb = k.upper().encode('utf-8')
+
+            if isinstance(v, bool):
+                vb = ('ON' if v else 'OFF').encode('utf-8')
+            else:
+                vb = str(v).encode('utf-8')
+
+            creation_opts = CSLAddNameValue(creation_opts, <const char *>kb, <const char *>vb)
 
     try:
         return exc_wrap_pointer(GDALCreate(cogr_driver, path_c, 0, 0, 0, GDT_Unknown, creation_opts))
     except FionaNullPointerError:
         raise DriverError("Failed to create dataset: {}".format(path_c.decode("utf-8")))
     except CPLE_BaseError as exc:
         raise DriverError(str(exc))
@@ -504,15 +519,15 @@
     if cogr_feature is not NULL:
         OGR_F_Destroy(cogr_feature)
     cogr_feature = NULL
 
 
 def featureRT(feat, collection):
     # For testing purposes only, leaks the JSON data
-    feature = _guard_model_object(feat)
+    feature = decode_object(feat)
     cdef void *cogr_feature = OGRFeatureBuilder().build(feature, collection)
     cdef void *cogr_geometry = OGR_F_GetGeometryRef(cogr_feature)
     if cogr_geometry == NULL:
         raise ValueError("Null geometry")
     result = FeatureBuilder().build(
         cogr_feature,
         encoding='utf-8',
@@ -1127,48 +1142,56 @@
                 log.debug("Deleted pre-existing layer at %s", collection.name)
                 GDALDatasetDeleteLayer(self.cogr_ds, idx)
 
             # Create the named layer in the datasource.
             name_b = collection.name.encode('utf-8')
             name_c = name_b
 
-            for k, v in kwargs.items():
+            # To avoid circular import.
+            from fiona import meta
 
-                if v is None:
-                    continue
+            kwarg_keys = set(key.upper() for key in kwargs.keys())
+            lyr_creation_option_keys = kwarg_keys & set(meta.layer_creation_options(collection.driver))
 
-                # We need to remove encoding from the layer creation
-                # options if we're not creating a shapefile.
-                if k == 'encoding' and "Shapefile" not in collection.driver:
-                    continue
+            for k, v in kwargs.items():
 
-                k = k.upper().encode('utf-8')
+                if v is not None and k.upper() in lyr_creation_option_keys:
+                    kb = k.upper().encode('utf-8')
 
-                if isinstance(v, bool):
-                    v = ('ON' if v else 'OFF').encode('utf-8')
-                else:
-                    v = str(v).encode('utf-8')
-                options = CSLAddNameValue(options, <const char *>k, <const char *>v)
+                    if isinstance(v, bool):
+                        vb = ('ON' if v else 'OFF').encode('utf-8')
+                    else:
+                        vb = str(v).encode('utf-8')
+
+                    options = CSLAddNameValue(options, <const char *>kb, <const char *>vb)
 
             geometry_type = collection.schema.get("geometry", "Unknown")
+
             if not isinstance(geometry_type, str) and geometry_type is not None:
                 geometry_types = set(geometry_type)
+
                 if len(geometry_types) > 1:
                     geometry_type = "Unknown"
                 else:
                     geometry_type = geometry_types.pop()
+
             if geometry_type == "Any" or geometry_type is None:
                 geometry_type = "Unknown"
+
             geometry_code = geometry_type_code(geometry_type)
 
             try:
-                self.cogr_layer = exc_wrap_pointer(
-                    GDALDatasetCreateLayer(
-                        self.cogr_ds, name_c, cogr_srs,
-                        <OGRwkbGeometryType>geometry_code, options))
+                # In GDAL versions > 3.6.0 the following directive may
+                # suffice and we might be able to eliminate the import
+                # of fiona.meta in a future version of Fiona.
+                with Env(GDAL_VALIDATE_CREATION_OPTIONS="NO"):
+                    self.cogr_layer = exc_wrap_pointer(
+                        GDALDatasetCreateLayer(
+                            self.cogr_ds, name_c, cogr_srs,
+                            <OGRwkbGeometryType>geometry_code, options))
 
             except Exception as exc:
                 GDALClose(self.cogr_ds)
                 self.cogr_ds = NULL
                 raise DriverIOError(str(exc))
 
             finally:
@@ -1269,52 +1292,56 @@
         # Mapping of the Python collection schema to normalized field types
         self._schema_normalized_field_types = {k: normalize_field_type(v) for (k, v) in self.collection.schema['properties'].items()}
 
 
         log.debug("Writing started")
 
     def writerecs(self, records, collection):
-        """Writes buffered records to OGR."""
+        """Writes records to collection storage.
+
+        Parameters
+        ----------
+        records : Iterable
+            A stream of feature records.
+        collection : Collection
+            The collection in which feature records are stored.
+
+        Returns
+        -------
+        None
+
+        """
         cdef void *cogr_driver
         cdef void *cogr_feature
         cdef int features_in_transaction = 0
-
         cdef void *cogr_layer = self.cogr_layer
+
         if cogr_layer == NULL:
             raise ValueError("Null layer")
 
-        schema_geom_type = collection.schema['geometry']
-        cogr_driver = GDALGetDatasetDriver(self.cogr_ds)
-        driver_name = OGR_Dr_GetName(cogr_driver).decode("utf-8")
-
         valid_geom_types = collection._valid_geom_types
 
         def validate_geometry_type(record):
             if record["geometry"] is None:
                 return True
             return record["geometry"]["type"].lstrip("3D ") in valid_geom_types
 
         transactions_supported = GDALDatasetTestCapability(self.cogr_ds, ODsCTransactions)
         log.debug("Transaction supported: {}".format(transactions_supported))
+
         if transactions_supported:
             log.debug("Starting transaction (initial)")
             result = GDALDatasetStartTransaction(self.cogr_ds, 0)
             if result == OGRERR_FAILURE:
                 raise TransactionError("Failed to start transaction")
 
         schema_props_keys = set(collection.schema['properties'].keys())
 
         for _rec in records:
-            record = _guard_model_object(_rec)
-
-            # Check for optional elements
-            # if 'properties' not in _rec:
-            #     _rec['properties'] = {}
-            # if 'geometry' not in _rec:
-            #     _rec['geometry'] = None
+            record = decode_object(_rec)
 
             # Validate against collection's schema.
             if set(record.properties.keys()) != schema_props_keys:
                 raise ValueError(
                     "Record does not match collection schema: %r != %r" % (
                         record.properties.keys(),
                         list(schema_props_keys) ))
@@ -1324,32 +1351,41 @@
                     "Record's geometry type does not match "
                     "collection schema's geometry type: %r != %r" % (
                         record.geometry.type,
                         collection.schema['geometry'] ))
 
             cogr_feature = OGRFeatureBuilder().build(record, collection)
             result = OGR_L_CreateFeature(cogr_layer, cogr_feature)
+
             if result != OGRERR_NONE:
                 msg = get_last_error_msg()
-                raise RuntimeError("GDAL Error: {msg} \n \n Failed to write record: "
-                                   "{record}".format(msg=msg, record=record))
+                raise RuntimeError(
+                    "GDAL Error: {msg}. Failed to write record: {record}".format(
+                        msg=msg, record=record
+                    )
+                )
 
             _deleteOgrFeature(cogr_feature)
 
             if transactions_supported:
                 features_in_transaction += 1
+
                 if features_in_transaction == DEFAULT_TRANSACTION_SIZE:
                     log.debug("Committing transaction (intermediate)")
                     result = GDALDatasetCommitTransaction(self.cogr_ds)
+
                     if result == OGRERR_FAILURE:
                         raise TransactionError("Failed to commit transaction")
+
                     log.debug("Starting transaction (intermediate)")
                     result = GDALDatasetStartTransaction(self.cogr_ds, 0)
+
                     if result == OGRERR_FAILURE:
                         raise TransactionError("Failed to start transaction")
+
                     features_in_transaction = 0
 
         if transactions_supported:
             log.debug("Committing transaction (final)")
             result = GDALDatasetCommitTransaction(self.cogr_ds)
             if result == OGRERR_FAILURE:
                 raise TransactionError("Failed to commit transaction")
@@ -1471,15 +1507,15 @@
         if bbox and mask:
             raise ValueError("mask and bbox can not be set together")
 
         if bbox:
             OGR_L_SetSpatialFilterRect(
                 cogr_layer, bbox[0], bbox[1], bbox[2], bbox[3])
         elif mask:
-            mask_geom = _guard_model_object(mask)
+            mask_geom = decode_object(mask)
             cogr_geometry = OGRGeomBuilder().build(mask_geom)
             OGR_L_SetSpatialFilter(cogr_layer, cogr_geometry)
             OGR_G_DestroyGeometry(cogr_geometry)
 
         else:
             OGR_L_SetSpatialFilter(cogr_layer, NULL)
 
@@ -2067,15 +2103,15 @@
         Metadata item
     """
     cdef char* metadata_c = NULL
     cdef void *cogr_driver
 
     if get_gdal_version_tuple() < (2, ):
         return None
-    
+
     if driver is None:
         return None
 
     driver_b = strencode(driver)
     cogr_driver = GDALGetDriverByName(driver_b)
     if cogr_driver == NULL:
         raise FionaValueError("Could not find driver '{}'".format(driver))
```

### Comparing `Fiona-1.9b1/fiona/path.py` & `Fiona-1.9b2/fiona/path.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/rfc3339.py` & `Fiona-1.9b2/fiona/rfc3339.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/schema.pyx` & `Fiona-1.9b2/fiona/schema.pyx`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/session.py` & `Fiona-1.9b2/fiona/session.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/fiona/transform.py` & `Fiona-1.9b2/fiona/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Coordinate and geometry warping and reprojection"""
 
 from warnings import warn
 
 from fiona._transform import _transform, _transform_geom
 from fiona.compat import DICT_TYPES
 from fiona.errors import FionaDeprecationWarning
-from fiona.model import _guard_model_object, Geometry
+from fiona.model import decode_object, Geometry
 
 
 def transform(src_crs, dst_crs, xs, ys):
     """Transform coordinates from one reference system to another.
 
     Parameters
     ----------
@@ -104,21 +104,21 @@
         )
 
     # Function is implemented in the _transform C extension module.
     if isinstance(geom, (Geometry,) + DICT_TYPES):
         return _transform_geom(
             src_crs,
             dst_crs,
-            _guard_model_object(geom),
+            decode_object(geom),
             antimeridian_cutting,
             antimeridian_offset,
             precision,
         )
     else:
         return _transform_geom(
             src_crs,
             dst_crs,
-            (_guard_model_object(g) for g in geom),
+            (decode_object(g) for g in geom),
             antimeridian_cutting,
             antimeridian_offset,
             precision,
         )
```

### Comparing `Fiona-1.9b1/fiona/vfs.py` & `Fiona-1.9b2/fiona/vfs.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/pyproject.toml` & `Fiona-1.9b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/setup.py` & `Fiona-1.9b2/setup.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/conftest.py` & `Fiona-1.9b2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/data/!test.geojson` & `Fiona-1.9b2/tests/data/!test.geojson`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/data/collection-pp.txt` & `Fiona-1.9b2/tests/data/collection-pp.txt`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/data/collection.txt` & `Fiona-1.9b2/tests/data/collection.txt`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/data/coutwildrnp.dbf` & `Fiona-1.9b2/tests/data/coutwildrnp.dbf`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/data/coutwildrnp.gpkg` & `Fiona-1.9b2/tests/data/coutwildrnp.gpkg`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/data/coutwildrnp.json` & `Fiona-1.9b2/tests/data/coutwildrnp.json`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/data/coutwildrnp.shp` & `Fiona-1.9b2/tests/data/coutwildrnp.shp`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/data/coutwildrnp.shx` & `Fiona-1.9b2/tests/data/coutwildrnp.shx`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/data/coutwildrnp.tar` & `Fiona-1.9b2/tests/data/coutwildrnp.tar`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/data/coutwildrnp.zip` & `Fiona-1.9b2/tests/data/coutwildrnp.zip`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/data/curves_line.csv` & `Fiona-1.9b2/tests/data/curves_line.csv`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/data/data.zip` & `Fiona-1.9b2/tests/data/data.zip`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/data/example.topojson` & `Fiona-1.9b2/tests/data/example.topojson`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/data/gre.dbf` & `Fiona-1.9b2/tests/data/gre.dbf`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/data/gre.shp` & `Fiona-1.9b2/tests/data/gre.shp`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/data/grenada.geojson` & `Fiona-1.9b2/tests/data/grenada.geojson`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/data/issue627.geojson` & `Fiona-1.9b2/tests/data/issue627.geojson`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/data/sequence-pp.txt` & `Fiona-1.9b2/tests/data/sequence-pp.txt`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/data/sequence.txt` & `Fiona-1.9b2/tests/data/sequence.txt`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/data/test_gpx.gpx` & `Fiona-1.9b2/tests/data/test_gpx.gpx`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test__env.py` & `Fiona-1.9b2/tests/test__env.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_bigint.py` & `Fiona-1.9b2/tests/test_bigint.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_binary_field.py` & `Fiona-1.9b2/tests/test_binary_field.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_bounds.py` & `Fiona-1.9b2/tests/test_bounds.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_bytescollection.py` & `Fiona-1.9b2/tests/test_bytescollection.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_collection.py` & `Fiona-1.9b2/tests/test_collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Testing collections and workspaces
 
+from collections import OrderedDict
 import datetime
+import logging
 import os
 import random
-import sys
 import re
-from collections import OrderedDict
+import sys
 
 import pytest
 
 import fiona
 from fiona.collection import Collection
 from fiona.drvsupport import supported_drivers, driver_mode_mingdal
 from fiona.env import getenv, GDALVersion
@@ -1043,22 +1044,24 @@
         == "/vsizip/vsicurl/https://raw.githubusercontent.com/Toblerity/Fiona/master/tests/data/coutwildrnp.zip"
     )
     assert len(ds) == 67
 
 
 def test_encoding_option_warning(tmpdir, caplog):
     """There is no ENCODING creation option log warning for GeoJSON"""
-    fiona.Collection(
-        str(tmpdir.join("test.geojson")),
-        "w",
-        driver="GeoJSON",
-        crs="epsg:4326",
-        schema={"geometry": "Point", "properties": {"foo": "int"}},
-    )
-    assert not caplog.text
+    with caplog.at_level(logging.WARNING):
+        fiona.Collection(
+            str(tmpdir.join("test.geojson")),
+            "w",
+            driver="GeoJSON",
+            crs="EPSG:4326",
+            schema={"geometry": "Point", "properties": {"foo": "int"}},
+            encoding="bogus",
+        )
+        assert not caplog.text
 
 
 def test_closed_session_next(gdalenv, path_coutwildrnp_shp):
     """Confirm fix for  issue #687"""
     src = fiona.open(path_coutwildrnp_shp)
     itr = iter(src)
     list(itr)
```

### Comparing `Fiona-1.9b1/tests/test_collection_crs.py` & `Fiona-1.9b2/tests/test_collection_crs.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_collection_legacy.py` & `Fiona-1.9b2/tests/test_collection_legacy.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_compound_crs.py` & `Fiona-1.9b2/tests/test_compound_crs.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_crs.py` & `Fiona-1.9b2/tests/test_crs.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_cursor_interruptions.py` & `Fiona-1.9b2/tests/test_cursor_interruptions.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_data_paths.py` & `Fiona-1.9b2/tests/test_data_paths.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_datetime.py` & `Fiona-1.9b2/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_driver_options.py` & `Fiona-1.9b2/tests/test_driver_options.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_drivers.py` & `Fiona-1.9b2/tests/test_drivers.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_drvsupport.py` & `Fiona-1.9b2/tests/test_drvsupport.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_encoding.py` & `Fiona-1.9b2/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_env.py` & `Fiona-1.9b2/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_feature.py` & `Fiona-1.9b2/tests/test_feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import sys
 import tempfile
 import pytest
 
 import fiona
 from fiona import collection
 from fiona.collection import Collection
-from fiona.errors import FionaDeprecationWarning
 from fiona.model import Feature
 from fiona.ogrext import featureRT
 
 
 class TestPointRoundTrip(object):
     def setup(self):
         self.tempdir = tempfile.mkdtemp()
@@ -32,18 +31,17 @@
 
     def test_geometry(self):
         f = {
             "id": "1",
             "geometry": {"type": "Point", "coordinates": (0.0, 0.0)},
             "properties": {"title": "foo"},
         }
-        with pytest.warns(FionaDeprecationWarning):
-            g = featureRT(f, self.c)
-            assert g.geometry.type == "Point"
-            assert g.geometry.coordinates == (0.0, 0.0)
+        g = featureRT(f, self.c)
+        assert g.geometry.type == "Point"
+        assert g.geometry.coordinates == (0.0, 0.0)
 
     def test_properties(self):
         f = Feature.from_dict(
             **{
                 "id": "1",
                 "geometry": {"type": "Point", "coordinates": (0.0, 0.0)},
                 "properties": {"title": "foo"},
```

### Comparing `Fiona-1.9b1/tests/test_fio_bounds.py` & `Fiona-1.9b2/tests/test_fio_bounds.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_fio_calc.py` & `Fiona-1.9b2/tests/test_fio_calc.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,17 +50,18 @@
     feats = _load(result.output)
     assert len(feats) == 2
     assert feats[0]['properties']['TEST']
     assert not feats[1]['properties']['TEST']
 
 
 def test_existing_property(feature_seq, runner):
-    result = runner.invoke(main_group, ['calc', "AREA", "f.properties.AREA * 2"],
-                           feature_seq)
-    assert result.exit_code == 1
+    result = runner.invoke(
+        main_group, ["calc", "AREA", "f.properties.AREA * 2"], feature_seq
+    )
+    assert result.exit_code == 2
 
     result = runner.invoke(main_group, ['calc', "--overwrite", "AREA", "f.properties.AREA * 2"],
                            feature_seq)
     assert result.exit_code == 0
     feats = _load(result.output)
     assert len(feats) == 2
     for feat in feats:
```

### Comparing `Fiona-1.9b1/tests/test_fio_cat.py` & `Fiona-1.9b2/tests/test_fio_cat.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_fio_collect.py` & `Fiona-1.9b2/tests/test_fio_collect.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_fio_distrib.py` & `Fiona-1.9b2/tests/test_fio_distrib.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_fio_dump.py` & `Fiona-1.9b2/tests/test_fio_dump.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_fio_filter.py` & `Fiona-1.9b2/tests/test_fio_filter.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_fio_info.py` & `Fiona-1.9b2/tests/test_fio_info.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_fio_load.py` & `Fiona-1.9b2/tests/test_fio_load.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_fio_ls.py` & `Fiona-1.9b2/tests/test_fio_ls.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_fio_rm.py` & `Fiona-1.9b2/tests/test_fio_rm.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_geojson.py` & `Fiona-1.9b2/tests/test_geojson.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_geometry.py` & `Fiona-1.9b2/tests/test_geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,18 +67,17 @@
         "type": "GeometryCollection",
         "geometries": [
             {"type": "Point", "coordinates": (0.0, 0.0)},
             {"type": "LineString", "coordinates": [(0.0, 0.0), (1.0, 1.0)]},
         ],
     }
 
-    with pytest.warns(DeprecationWarning):
-        result = geometryRT(geom)
-        assert len(result["geometries"]) == 2
-        assert [g["type"] for g in result["geometries"]] == ["Point", "LineString"]
+    result = geometryRT(geom)
+    assert len(result["geometries"]) == 2
+    assert [g["type"] for g in result["geometries"]] == ["Point", "LineString"]
 
 
 def test_point_wkb():
     # Hex-encoded Point (0 0)
     wkb = "010100000000000000000000000000000000000000"
     geom = geometry_wkb(wkb)
     assert geom["type"] == "Point"
```

### Comparing `Fiona-1.9b1/tests/test_geopackage.py` & `Fiona-1.9b2/tests/test_geopackage.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_http_session.py` & `Fiona-1.9b2/tests/test_http_session.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_integration.py` & `Fiona-1.9b2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_layer.py` & `Fiona-1.9b2/tests/test_layer.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_listing.py` & `Fiona-1.9b2/tests/test_listing.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_logutils.py` & `Fiona-1.9b2/tests/test_logutils.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_memoryfile.py` & `Fiona-1.9b2/tests/test_memoryfile.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_meta.py` & `Fiona-1.9b2/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_model.py` & `Fiona-1.9b2/tests/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,21 @@
     assert Geometry(coordinates=(0, 0), type="Point")._props() == {
         "coordinates": (0, 0),
         "type": "Point",
         "geometries": None,
     }
 
 
+def test_geometry_gi():
+    """Geometry __geo_interface__"""
+    gi = Geometry(coordinates=(0, 0), type="Point").__geo_interface__
+    assert gi["type"] == "Point"
+    assert gi["coordinates"] == (0, 0)
+
+
 def test_feature_no_geometry():
     """Feature has no attribute"""
     feat = Feature()
     assert feat.geometry is None
 
 
 def test_feature_geometry():
@@ -290,7 +297,20 @@
     """Pass through an ordinary dict"""
     assert decode_object(o) == o
 
 
 def test_properties():
     """Property factory works"""
     assert Properties.from_dict(a=1, foo="bar")["a"] == 1
+
+
+def test_feature_gi():
+    """Feature __geo_interface__."""
+    gi = Feature(
+        id="foo",
+        geometry=Geometry(type="Point", coordinates=(0, 0)),
+        properties=Properties(a=1, foo="bar"),
+    )
+
+    assert gi["id"] == "foo"
+    assert gi["geometry"]["type"] == "Point"
+    assert gi["geometry"]["coordinates"] == (0, 0)
```

### Comparing `Fiona-1.9b1/tests/test_multiconxn.py` & `Fiona-1.9b2/tests/test_multiconxn.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_non_counting_layer.py` & `Fiona-1.9b2/tests/test_non_counting_layer.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_open.py` & `Fiona-1.9b2/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_profile.py` & `Fiona-1.9b2/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_props.py` & `Fiona-1.9b2/tests/test_props.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_read_drivers.py` & `Fiona-1.9b2/tests/test_read_drivers.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_remove.py` & `Fiona-1.9b2/tests/test_remove.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_rfc3339.py` & `Fiona-1.9b2/tests/test_rfc3339.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_rfc64_tin.py` & `Fiona-1.9b2/tests/test_rfc64_tin.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_schema.py` & `Fiona-1.9b2/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_schema_geom.py` & `Fiona-1.9b2/tests/test_schema_geom.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_session.py` & `Fiona-1.9b2/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_slice.py` & `Fiona-1.9b2/tests/test_slice.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_subtypes.py` & `Fiona-1.9b2/tests/test_subtypes.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_topojson.py` & `Fiona-1.9b2/tests/test_topojson.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_transactions.py` & `Fiona-1.9b2/tests/test_transactions.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_transform.py` & `Fiona-1.9b2/tests/test_transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,23 +115,22 @@
                     (512381.8870945257, 5866313.311218272),
                     (512371.23869999964, 5866322.282500001),
                     (512364.6014999999, 5866328.260199999),
                 ],
             }
         ],
     }
-    with pytest.warns(FionaDeprecationWarning):
-        geom_transformed = transform.transform_geom(source_crs, dest_src, geom)
-        assert geom_transformed.geometries[0].coordinates[0] == pytest.approx(
-            (9.18427, 52.94630)
-        )
+    geom_transformed = transform.transform_geom(source_crs, dest_src, geom)
+    assert geom_transformed.geometries[0].coordinates[0] == pytest.approx(
+        (9.18427, 52.94630)
+    )
 
 
 def test_transform_geom_precision_deprecation():
-    """Get a deprecation warning in 1.9"""
+    """Get a precision deprecation warning in 1.9."""
     with pytest.warns(FionaDeprecationWarning):
         transform.transform_geom(
             "epsg:4326",
             "epsg:3857",
             Geometry(type="Point", coordinates=(0, 0)),
             precision=2,
         )
```

### Comparing `Fiona-1.9b1/tests/test_unicode.py` & `Fiona-1.9b2/tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_version.py` & `Fiona-1.9b2/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_vfs.py` & `Fiona-1.9b2/tests/test_vfs.py`

 * *Files identical despite different names*

### Comparing `Fiona-1.9b1/tests/test_write.py` & `Fiona-1.9b2/tests/test_write.py`

 * *Files identical despite different names*

