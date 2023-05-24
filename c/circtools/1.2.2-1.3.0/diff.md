# Comparing `tmp/circtools-1.2.2.tar.gz` & `tmp/circtools-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/circtools-1.2.2.tar", last modified: Wed Feb 15 18:14:33 2023, max compression
+gzip compressed data, was "dist/circtools-1.3.0.tar", last modified: Tue May 23 23:59:09 2023, max compression
```

## Comparing `circtools-1.2.2.tar` & `circtools-1.3.0.tar`

### file list

```diff
@@ -1,66 +1,239 @@
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-02-15 18:14:33.000000 circtools-1.2.2/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    35147 2018-04-13 15:26:28.000000 circtools-1.2.2/LICENSE
--rw-rw-r--   0 tjakobi   (1000) tjakobi   (1000)      112 2017-02-26 23:34:59.000000 circtools-1.2.2/MANIFEST.in
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     9336 2023-02-15 18:14:33.000000 circtools-1.2.2/PKG-INFO
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     8361 2018-09-20 20:27:56.000000 circtools-1.2.2/README.rst
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-02-15 18:14:33.000000 circtools-1.2.2/circtools/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)       35 2017-07-03 12:19:07.000000 circtools-1.2.2/circtools/__init__.py
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-02-15 18:14:33.000000 circtools-1.2.2/circtools/circ_module/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2017-04-19 12:18:16.000000 circtools-1.2.2/circtools/circ_module/__init__.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3183 2018-06-21 15:38:20.000000 circtools-1.2.2/circtools/circ_module/circ_template.py
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-02-15 18:14:33.000000 circtools-1.2.2/circtools/circtest/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2018-06-21 15:38:20.000000 circtools-1.2.2/circtools/circtest/__init__.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     6198 2018-06-21 15:38:20.000000 circtools-1.2.2/circtools/circtest/circtest.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    49102 2023-02-15 18:06:21.000000 circtools-1.2.2/circtools/circtools.py
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-02-15 18:14:33.000000 circtools-1.2.2/circtools/enrichment/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2017-04-18 15:25:07.000000 circtools-1.2.2/circtools/enrichment/__init__.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    56943 2021-06-17 00:37:35.000000 circtools-1.2.2/circtools/enrichment/enrichment_check.py
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-02-15 18:14:33.000000 circtools-1.2.2/circtools/exon_usage/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2018-06-21 15:38:20.000000 circtools-1.2.2/circtools/exon_usage/__init__.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     5889 2018-09-20 20:27:56.000000 circtools-1.2.2/circtools/exon_usage/exon_usage.py
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-02-15 18:14:33.000000 circtools-1.2.2/circtools/mirna/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2017-04-18 15:25:07.000000 circtools-1.2.2/circtools/mirna/__init__.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     1197 2017-11-24 09:23:27.000000 circtools-1.2.2/circtools/mirna/mirna.py
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-02-15 18:14:33.000000 circtools-1.2.2/circtools/primex/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2018-06-21 15:38:20.000000 circtools-1.2.2/circtools/primex/__init__.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    27052 2020-01-15 10:25:18.000000 circtools-1.2.2/circtools/primex/primex.py
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-02-15 18:14:33.000000 circtools-1.2.2/circtools/quickcheck/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2018-06-21 15:38:20.000000 circtools-1.2.2/circtools/quickcheck/__init__.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     5392 2018-09-20 20:27:56.000000 circtools-1.2.2/circtools/quickcheck/quickcheck.py
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-02-15 18:14:33.000000 circtools-1.2.2/circtools/sirna/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2019-11-18 09:29:11.000000 circtools-1.2.2/circtools/sirna/__init__.py
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    40131 2019-11-18 09:29:11.000000 circtools-1.2.2/circtools/sirna/sirna.py
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-02-15 18:14:33.000000 circtools-1.2.2/circtools.egg-info/
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     9336 2023-02-15 18:14:33.000000 circtools-1.2.2/circtools.egg-info/PKG-INFO
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1704 2023-02-15 18:14:33.000000 circtools-1.2.2/circtools.egg-info/SOURCES.txt
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        1 2023-02-15 18:14:33.000000 circtools-1.2.2/circtools.egg-info/dependency_links.txt
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        1 2017-06-26 12:29:28.000000 circtools-1.2.2/circtools.egg-info/not-zip-safe
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      140 2023-02-15 18:14:33.000000 circtools-1.2.2/circtools.egg-info/requires.txt
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)       10 2023-02-15 18:14:33.000000 circtools-1.2.2/circtools.egg-info/top_level.txt
-drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-02-15 18:14:33.000000 circtools-1.2.2/scripts/
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)      724 2017-07-03 12:19:07.000000 circtools-1.2.2/scripts/circtools
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     6910 2019-05-31 11:20:12.000000 circtools-1.2.2/scripts/circtools_circtest_wrapper.R
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     1236 2018-06-21 15:38:20.000000 circtools-1.2.2/scripts/circtools_detect_write_skip_tracks.pl
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    22665 2018-10-19 15:54:16.000000 circtools-1.2.2/scripts/circtools_enrich_visualization.R
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    21557 2019-11-18 09:28:42.000000 circtools-1.2.2/scripts/circtools_exon_wrapper.R
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     5214 2018-09-20 20:27:56.000000 circtools-1.2.2/scripts/circtools_generate_flanking_introns.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     1595 2020-08-04 10:08:25.000000 circtools-1.2.2/scripts/circtools_generate_intron_gtf.sh
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     1019 2019-10-24 19:24:35.000000 circtools-1.2.2/scripts/circtools_merge_enrich_results.sh
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     8487 2018-11-30 11:28:45.000000 circtools-1.2.2/scripts/circtools_primex_formatter.R
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     5071 2019-10-24 19:24:35.000000 circtools-1.2.2/scripts/circtools_primex_wrapper.R
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    15186 2018-12-14 16:28:09.000000 circtools-1.2.2/scripts/circtools_quickcheck_wrapper.R
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    12125 2018-10-11 12:47:39.000000 circtools-1.2.2/scripts/circtools_reconstruct_visualization.R
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     4311 2019-01-24 13:10:12.000000 circtools-1.2.2/scripts/circtools_reconstruct_write_gtf.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    11032 2019-11-18 09:29:11.000000 circtools-1.2.2/scripts/circtools_sirna_formatter.R
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     8503 2018-06-21 15:38:20.000000 circtools-1.2.2/scripts/create_igv_script.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     6585 2018-06-21 15:38:20.000000 circtools-1.2.2/scripts/create_igv_script_from_gene_names.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     6870 2018-06-21 15:38:20.000000 circtools-1.2.2/scripts/create_igv_script_from_position_list.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    11321 2019-01-25 17:14:36.000000 circtools-1.2.2/scripts/detect_new_exons_from_fuchs_data.py
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     2144 2018-06-21 15:38:20.000000 circtools-1.2.2/scripts/get_introns_from_ensembl.pl
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)      813 2019-08-30 09:51:08.000000 circtools-1.2.2/scripts/get_significant_enriched_circles.sh
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     2233 2022-04-12 23:02:18.000000 circtools-1.2.2/scripts/install_R_dependencies.R
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     1066 2020-08-17 10:33:07.000000 circtools-1.2.2/scripts/install_add_to_bashrc.sh
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)      922 2019-11-18 11:12:20.000000 circtools-1.2.2/scripts/install_create_r_environ.sh
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     1913 2022-08-24 16:05:39.000000 circtools-1.2.2/scripts/install_external.sh
--rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)       38 2023-02-15 18:14:33.000000 circtools-1.2.2/setup.cfg
--rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     7299 2023-02-15 18:06:10.000000 circtools-1.2.2/setup.py
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    35147 2022-06-17 23:38:57.000000 circtools-1.3.0/LICENSE
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      196 2023-03-10 01:23:32.000000 circtools-1.3.0/MANIFEST.in
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     9770 2023-05-23 23:59:09.000000 circtools-1.3.0/PKG-INFO
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     8830 2023-03-14 18:30:52.000000 circtools-1.3.0/README.rst
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2023-03-10 00:17:31.000000 circtools-1.3.0/circtools/__init__.py
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/circ_module/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/circ_module/__init__.py
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3183 2022-07-29 21:01:07.000000 circtools-1.3.0/circtools/circ_module/circ_template.py
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/circtest/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/circtest/__init__.py
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     6214 2023-03-21 00:23:22.000000 circtools-1.3.0/circtools/circtest/circtest.py
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    49652 2023-05-23 21:41:07.000000 circtools-1.3.0/circtools/circtools.py
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/circtest/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)       28 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/contrib/circtest/.Rbuildignore
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      569 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/contrib/circtest/.gitignore
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      478 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/DESCRIPTION
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      151 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/NAMESPACE
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/circtest/R/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2500 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/R/Circ.filter.R
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     6106 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/R/Circ.linePlot.R
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     7248 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/R/Circ.ratioplot.R
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     5286 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/R/Circ.test.R
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     4428 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/R/HostGeneCount.R
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     4296 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/R/documentData.R
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1696 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/R/summarySE.R
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     6938 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/README.md
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/circtest/data/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3611 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/data/Circ.rda
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3031 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/data/Coordinates.rda
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     4386 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/data/Linear.rda
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/circtest/man/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1972 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/man/Circ.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1442 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/man/Circ.filter.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1925 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/man/Circ.lineplot.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1813 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/man/Circ.ratioplot.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1427 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/man/Circ.test.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      549 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/man/Coordinates.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      903 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/man/HostGeneCount.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1958 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/man/Linear.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      717 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/man/read_one_scanBam.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      762 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/man/read_scanBam.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      266 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/circtest/man/summarySE.Rd
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      112 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/.Rbuildignore
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1387 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/CONDUCT.md
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      846 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/DESCRIPTION
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    34904 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/LICENSE
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      410 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/NAMESPACE
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)       19 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/NEWS.md
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/R/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      143 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/R/data.R
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     8497 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/R/design.R
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3590 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/R/plotting.R
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3535 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/R/select.R
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1888 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/R/settings.R
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2708 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/R/transform.R
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      442 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/R/utils.R
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1596 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/README.Rmd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3215 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/README.md
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)       43 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/_pkgdown.yml
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/docs/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    38348 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/LICENSE.html
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/docs/articles/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    26375 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/articles/Usage.html
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/docs/articles/Usage_files/
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/docs/articles/Usage_files/figure-html/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)   160986 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/articles/Usage_files/figure-html/unnamed-chunk-10-1.png
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)   119338 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/articles/Usage_files/figure-html/unnamed-chunk-7-1.png
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3572 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/articles/index.html
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3492 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/authors.html
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     9664 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/index.html
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2798 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/jquery.sticky-kit.min.js
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      810 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/link.svg
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/docs/news/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3803 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/news/index.html
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2828 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/pkgdown.css
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1085 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/pkgdown.js
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     4619 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/addSeq.html
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     7074 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/bcl6exons.html
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     9876 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/design.html
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     5976 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/diagnose.html
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     4262 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/extractExonPairs.html
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     7328 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/index.html
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     4606 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/p3Settings.html
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3684 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/p3Version.html
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     4088 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/plotSegments.html
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    11416 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/primerSize.html
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    11461 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/primerTm.html
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     4391 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/primersToList.html
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    10879 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/productSize.html
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3819 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/reexports.html
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     4797 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/runPrimer3.html
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     4613 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/selectPairs.html
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     5918 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/seqSettings.html
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     4439 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/docs/reference/toGRanges.html
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/inst/
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      373 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/dangle.dh
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      548 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/dangle.ds
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      994 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/dangle_i.dh
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1017 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/dangle_i.ds
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1856 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/loops_i.dh
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      699 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/loops_i.ds
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2667 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/stack_i.dh
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2592 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/stack_i.ds
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2751 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/stackmm_i_mm.dh
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2643 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/stackmm_i_mm.ds
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      815 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tetraloop_i.dh
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      873 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tetraloop_i.ds
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      194 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/triloop_i.dh
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      160 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/triloop_i.ds
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2486 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack2_i.dh
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2720 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack2_i.ds
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2135 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack_i.dh
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2463 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack_i.ds
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2135 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack_tm_inf_i.dh
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2494 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/interpretations/tstack_tm_inf_i.ds
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      441 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/loops.dh
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      692 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/loops.ds
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1057 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/stack.dh
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1056 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/stack.ds
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1144 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/stackmm.dh
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1109 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/stackmm.ds
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      913 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/tetraloop.dh
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      824 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/tetraloop.ds
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      192 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/triloop.dh
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      128 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/triloop.ds
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      890 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/tstack.dh
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      950 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/tstack2.dh
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1184 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/tstack2.ds
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1152 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_config/tstack_tm_inf.ds
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)   312896 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_core_Darwin_64
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)   239308 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_core_Linux_32
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)   994360 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_core_Linux_64
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3331 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/inst/primer3/primer3_v1_1_4_default_settings.txt
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/man/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      600 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/addSeq.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      350 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/bcl6exons.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1163 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/design.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      662 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/diagnose.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      345 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/extractExonPairs.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      503 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/p3Settings.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      207 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/p3Version.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      298 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/plotSegments.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      605 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/primerSize.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      638 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/primerTm.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      435 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/primersToList.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      492 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/productSize.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      397 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/reexports.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      582 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/runPrimer3.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      528 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/selectPairs.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1163 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/seqSettings.Rd
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      404 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/man/toGRanges.Rd
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/contrib/primex/vignettes/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     6488 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/contrib/primex/vignettes/Usage.Rmd
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/detect/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    20587 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/detect/Circ_nonCirc_Exon_Match.py
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     7245 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/detect/CombineCounts.py
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     5230 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/detect/IntervalTree.py
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/detect/__init__.py
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     8673 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/detect/circAnnotate.py
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     5913 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/detect/circFilter.py
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    39917 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/detect/detect.py
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    11374 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/detect/findcircRNA.py
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     5745 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/detect/fix2chimera.py
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    13103 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/detect/genecount.py
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/enrichment/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/enrichment/__init__.py
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    56944 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/enrichment/enrichment_check.py
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/exon_usage/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/exon_usage/__init__.py
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     5907 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/exon_usage/exon_usage.py
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/primex/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/primex/__init__.py
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    27288 2023-03-21 01:10:49.000000 circtools-1.3.0/circtools/primex/primex.py
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/quickcheck/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/quickcheck/__init__.py
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     5440 2023-03-21 00:50:01.000000 circtools-1.3.0/circtools/quickcheck/quickcheck.py
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/reconstruct/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/reconstruct/__init__.py
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     7926 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/reconstruct/detect_skipped_exons.py
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     6747 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/reconstruct/detect_splicing_variants.py
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     5077 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/reconstruct/extract_reads.py
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    17026 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/reconstruct/get_coverage_profile.py
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     6805 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/reconstruct/get_mate_information.py
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     4147 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/reconstruct/get_readnames_from_DCC.py
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    27401 2023-03-21 20:18:54.000000 circtools-1.3.0/circtools/reconstruct/guided_denovo_circle_structure_parallel.py
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     3771 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/reconstruct/permutate_motifs.py
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2622 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/reconstruct/proportion_of_fully_covered_circRNAs.py
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    18178 2023-03-21 18:20:04.000000 circtools-1.3.0/circtools/reconstruct/reconstruct.py
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2732 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/reconstruct/replace_ids_with_names.py
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     8423 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/reconstruct/write_fasta_for_fimo.py
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/scripts/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2023-03-10 00:17:31.000000 circtools-1.3.0/circtools/scripts/__init__.py
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      983 2023-03-10 01:50:40.000000 circtools-1.3.0/circtools/scripts/bash_runner.py
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     6910 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/scripts/circtools_circtest_wrapper.R
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    22665 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/scripts/circtools_enrich_visualization.R
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    21557 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/scripts/circtools_exon_wrapper.R
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     5214 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/scripts/circtools_generate_flanking_introns.py
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     1595 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/scripts/circtools_generate_intron_gtf.sh
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     1019 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/scripts/circtools_merge_enrich_results.sh
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     8398 2023-03-20 04:04:13.000000 circtools-1.3.0/circtools/scripts/circtools_primex_formatter.R
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     5071 2023-03-06 20:37:07.000000 circtools-1.3.0/circtools/scripts/circtools_primex_wrapper.R
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    15182 2023-03-20 03:02:00.000000 circtools-1.3.0/circtools/scripts/circtools_quickcheck_wrapper.R
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     1488 2023-03-21 18:36:38.000000 circtools-1.3.0/circtools/scripts/circtools_reconstruct_coverage_graph.R
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     8495 2023-03-21 18:36:39.000000 circtools-1.3.0/circtools/scripts/circtools_reconstruct_summarized_coverage_profiles.R
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     2225 2023-03-21 18:13:25.000000 circtools-1.3.0/circtools/scripts/circtools_reconstruct_summary_graphs.R
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    12125 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/scripts/circtools_reconstruct_visualization.R
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    10905 2023-03-06 20:38:19.000000 circtools-1.3.0/circtools/scripts/circtools_sirna_formatter.R
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     8784 2023-03-10 00:30:08.000000 circtools-1.3.0/circtools/scripts/create_igv_script.py
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     6813 2023-03-10 00:32:59.000000 circtools-1.3.0/circtools/scripts/create_igv_script_from_gene_names.py
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     7098 2023-03-10 00:32:59.000000 circtools-1.3.0/circtools/scripts/create_igv_script_from_position_list.py
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)    11775 2023-03-10 00:33:48.000000 circtools-1.3.0/circtools/scripts/detect_new_exons_from_fuchs_data.py
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     3722 2023-03-21 18:15:46.000000 circtools-1.3.0/circtools/scripts/install_R_dependencies.R
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     1066 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/scripts/install_add_to_bashrc.sh
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)      922 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/scripts/install_create_r_environ.sh
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     1451 2023-03-14 19:06:55.000000 circtools-1.3.0/circtools/scripts/install_external.sh
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2907 2023-03-21 18:22:31.000000 circtools-1.3.0/circtools/scripts/r_runner.py
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)     1203 2023-03-19 02:39:54.000000 circtools-1.3.0/circtools/scripts/wonderdump
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools/sirna/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        0 2022-06-17 23:38:57.000000 circtools-1.3.0/circtools/sirna/__init__.py
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)    40141 2023-03-06 20:38:18.000000 circtools-1.3.0/circtools/sirna/sirna.py
+drwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)        0 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools.egg-info/
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     9770 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools.egg-info/PKG-INFO
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     9826 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools.egg-info/SOURCES.txt
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        1 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools.egg-info/dependency_links.txt
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     1552 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools.egg-info/entry_points.txt
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)        1 2022-08-03 17:38:24.000000 circtools-1.3.0/circtools.egg-info/not-zip-safe
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)      150 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools.egg-info/requires.txt
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)       10 2023-05-23 23:59:09.000000 circtools-1.3.0/circtools.egg-info/top_level.txt
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)       94 2023-03-10 18:13:54.000000 circtools-1.3.0/pyproject.toml
+-rw-r--r--   0 tjakobi   (1000) tjakobi   (1000)     2830 2023-05-23 23:59:09.000000 circtools-1.3.0/setup.cfg
+-rwxr-xr-x   0 tjakobi   (1000) tjakobi   (1000)       69 2023-02-13 23:45:49.000000 circtools-1.3.0/setup.py
```

### Comparing `circtools-1.2.2/LICENSE` & `circtools-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circtools-1.2.2/PKG-INFO` & `circtools-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: circtools
-Version: 1.2.2
+Version: 1.3.0
 Summary: circtools - a circular RNA toolbox
-Home-page: https://github.com/dieterich-lab/circtools
+Home-page: https://github.com/jakobilab/circtools
 Author: Tobias Jakobi
-Author-email: Tobias.Jakobi@med.Uni-Heidelberg.DE
+Author-email: tjakobi@arizona.edu
 License: GNU General Public License (GPL)
-Project-URL: Bug Reports, https://github.com/dieterich-lab/circtools/issues
-Project-URL: Dieterich Lab, https://dieterichlab.org
-Project-URL: Source, https://github.com/dieterich-lab/circtools
-Project-URL: Documentation, http://docs.circ.tools
-Keywords: circular RNA bioinformatics
+Project-URL: Bug Reports, https://github.com/jakobilab/circtools/issues
+Project-URL: Jakobi Lab, https://jakobilab.org
+Project-URL: Source, https://github.com/jakobilab/circtools
+Project-URL: Documentation, https://docs.circ.tools
+Keywords: circRNA,circular RNA bioinformatics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >3.5
-License-File: LICENSE
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
 
 **circtools**
 ======================================================================
 
 **a one-stop software solution for circular RNA research**
 
-.. figure:: https://raw.githubusercontent.com/dieterich-lab/circtools/master/docs/img/circtools_200px.png
+.. figure:: https://raw.githubusercontent.com/jakobilab/circtools/master/docs/img/circtools_200px.png
    :alt: circtools
 
-|docs| |build| |zenodo| |downloads| |pypi|
+|docs| |build| |docker| |zenodo| |downloads| |pypi|
 
 Introduction
 -------------
 
 Circular RNAs (circRNAs) originate through back-splicing events from linear primary transcripts, are resistant to exonucleases, typically not polyadenylated, and have been shown to be highly specific for cell type and developmental stage. Although few circular RNA molecules have been shown to exhibit miRNA sponge function, for the vast majority of circRNAs however, their function is yet to be determined.
 
 The prediction of circular RNAs is a multi-stage bioinformatics process starting with raw sequencing data and usually ending with a list of potential circRNA candidates which, depending on tissue and condition may contain hundreds to thousands of potential circRNAs. While there already exist a number of tools for the prediction process (e.g. `DCC <https://github.com/dieterich-lab/DCC>`__ and `CircTest <https://github.com/dieterich-lab/CircTest>`__), publicly available downstream analysis tools are rare.
@@ -42,63 +42,70 @@
 a quick check of circRNA mapping results, RBP enrichment screenings, circRNA primer design, statistical testing, and an exon usage module.
 
 
 
 Documentation
 -------------
 
-Click `here <http://docs.circ.tools/>`__ to access the complete documentation on Read the Docs.
+Click `here <https://docs.circ.tools/>`__ to access the complete documentation on Read the Docs.
 
 Installation
 ------------
 
-The ``circtools`` package is written in Python3 (>=3.4), two modules, namely ``detect`` and ``reconstruct`` also require a working Python 2 installation (>=2.7). It requires only a small number of external dependencies, namely standard bioinformatics tools:
+The ``circtools`` package is written in Python 3 (supporting Python 3.7 - 3.10). It requires only a small number of external dependencies, namely standard bioinformatics tools:
 
 -  `bedtools (>= 2.27.1) <https://bedtools.readthedocs.io/en/latest/content/installation.html>`__
    [RBP enrichment module, installed automatically]
--  `R (>= 3.3) <https://www.digitalocean.com/community/tutorials/how-to-install-r-on-ubuntu-16-04-2>`__
+-  `R (>= 4.0) <https://www.digitalocean.com/community/tutorials/how-to-install-r-on-ubuntu-22-04>`__
    [Data visualization and data processing]
 
-Installation is managed through ``python3 setup.py install``. No sudo
-access is required if the installation is executed with ``--user`` which
-will install the package in a user-writeable folder. The binaries should
-be installed to ``/home/$user/.local/bin/`` in case of Debian-based
-systems.
-
-``circtools`` was developed and tested on Debian Jessie but should also
-run with any distribution.
-
-The installation requires running python on the command line:
-
-::
-
-    git clone https://github.com/dieterich-lab/circtools.git
-    cd circtools
-    python3 setup.py install --verbose --user
-
-The installation procedure will automatically install two dependencies:
-`DCC <https://github.com/dieterich-lab/DCC>`__ and
-`FUCHS <https://github.com/dieterich-lab/FUCHS>`__. The primer-design
-module as well as the exon analysis and circRNA testing module require a
-working installation of `R <https://cran.r-project.org/>`__ with
+Installation is managed through ``pip3 install circtools`` or ``python3 setup.py
+install`` when installed from the cloned GitHub repository. No sudo access is
+required if the installation is executed with ``--user`` which will install the
+package in a user-writeable folder. The binaries should be installed
+to ``/home/$user/.local/bin/`` in case of Debian-based systems.
+
+``circtools`` was developed and tested on Debian Buster, but should also
+run with any other distribution.
+
+The installation can be performed directly from Pypi:
+
+.. code-block:: console
+
+    # install circtools
+    pip install numpy # required for HTSeq, a dependency of circtools
+    pip install circtools
+
+    # install R packages for circtools
+    circtools_install_R_dependencies
+
+Additionally, this repository offers the latest development version:
+
+.. code-block:: console
+
+    pip install numpy # required for HTSeq, a dependency of circtools
+    pip install git+https://github.com/jakobilab/circtools.git
+
+The primer-design module as well as the exon analysis and circRNA testing module
+require a working installation of `R <https://cran.r-project.org/>`__ with
 `BioConductor <https://www.bioconductor.org/install/>`__. All R packages
-required are automatically installed during the setup. Please see the
+required can be automatically installed during the setup. Please see the
 `"Installing circtools" <http://docs.circ.tools/en/latest/Installation.html>`__
 chapter of the main circtools documentation for more detailed installation instructions.
 
 Modules
 -------
 
 Circtools currently offers seven modules:
 
 detect `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Detect.html>`__
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The ``detect`` command is an interface to
-`DCC <https://github.com/dieterich-lab/DCC>`__, also developed at the
+`DCC <https://github.com/dieterich-lab/DCC>`__, developed at the
 Dieterich Lab. The module allows to detect circRNAs from RNA sequencing
 data. The module is the foundation of all other steps for the circtools
 work flow. All parameters supplied to circtools will be directly passed
 to DCC.
 
 quickcheck `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Quickcheck.html>`__
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
@@ -154,23 +161,29 @@
 
 primer `(detailed documentation) <https://circtools.readthedocs.io/en/latest/primer.html>`__
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The ``primer`` command is used to design and visualize primers required
 for follow up wet lab experiments to verify circRNA candidates.
 
+
 .. |docs| image:: https://readthedocs.org/projects/circtools/badge/?version=latest
     :alt: Documentation Status
     :scale: 100%
     :target: https://circtools.readthedocs.io/en/latest/?badge=latest
 
-.. |build| image:: https://travis-ci.org/dieterich-lab/circtools.svg?branch=master
-    :alt: Build Status
+.. |build| image:: https://github.com/jakobilab/circtools/actions/workflows/run_circtools_detect.yml/badge.svg?branch=master
+    :alt: CI Status
+    :scale: 100%
+    :target: https://github.com/jakobilab/circtools/actions/workflows/run_circtools_detect.yml
+
+.. |docker| image:: https://github.com/jakobilab/circtools/actions/workflows/build_docker.yml/badge.svg?branch=master
+    :alt: Docker Build
     :scale: 100%
-    :target: https://travis-ci.org/dieterich-lab/circtools
+    :target: https://github.com/jakobilab/circtools/actions/workflows/build_docker.yml
 
 .. |zenodo| image:: https://zenodo.org/badge/83248654.svg
     :alt: Zenodo DOI link
     :scale: 100%
     :target: https://zenodo.org/badge/latestdoi/83248654
 
 .. |downloads| image:: https://pepy.tech/badge/circtools
```

### Comparing `circtools-1.2.2/README.rst` & `circtools-1.3.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 **circtools**
 ======================================================================
 
 **a one-stop software solution for circular RNA research**
 
-.. figure:: https://raw.githubusercontent.com/dieterich-lab/circtools/master/docs/img/circtools_200px.png
+.. figure:: https://raw.githubusercontent.com/jakobilab/circtools/master/docs/img/circtools_200px.png
    :alt: circtools
 
-|docs| |build| |zenodo| |downloads| |pypi|
+|docs| |build| |docker| |zenodo| |downloads| |pypi|
 
 Introduction
 -------------
 
 Circular RNAs (circRNAs) originate through back-splicing events from linear primary transcripts, are resistant to exonucleases, typically not polyadenylated, and have been shown to be highly specific for cell type and developmental stage. Although few circular RNA molecules have been shown to exhibit miRNA sponge function, for the vast majority of circRNAs however, their function is yet to be determined.
 
 The prediction of circular RNAs is a multi-stage bioinformatics process starting with raw sequencing data and usually ending with a list of potential circRNA candidates which, depending on tissue and condition may contain hundreds to thousands of potential circRNAs. While there already exist a number of tools for the prediction process (e.g. `DCC <https://github.com/dieterich-lab/DCC>`__ and `CircTest <https://github.com/dieterich-lab/CircTest>`__), publicly available downstream analysis tools are rare.
@@ -19,63 +19,70 @@
 a quick check of circRNA mapping results, RBP enrichment screenings, circRNA primer design, statistical testing, and an exon usage module.
 
 
 
 Documentation
 -------------
 
-Click `here <http://docs.circ.tools/>`__ to access the complete documentation on Read the Docs.
+Click `here <https://docs.circ.tools/>`__ to access the complete documentation on Read the Docs.
 
 Installation
 ------------
 
-The ``circtools`` package is written in Python3 (>=3.4), two modules, namely ``detect`` and ``reconstruct`` also require a working Python 2 installation (>=2.7). It requires only a small number of external dependencies, namely standard bioinformatics tools:
+The ``circtools`` package is written in Python 3 (supporting Python 3.7 - 3.10). It requires only a small number of external dependencies, namely standard bioinformatics tools:
 
 -  `bedtools (>= 2.27.1) <https://bedtools.readthedocs.io/en/latest/content/installation.html>`__
    [RBP enrichment module, installed automatically]
--  `R (>= 3.3) <https://www.digitalocean.com/community/tutorials/how-to-install-r-on-ubuntu-16-04-2>`__
+-  `R (>= 4.0) <https://www.digitalocean.com/community/tutorials/how-to-install-r-on-ubuntu-22-04>`__
    [Data visualization and data processing]
 
-Installation is managed through ``python3 setup.py install``. No sudo
-access is required if the installation is executed with ``--user`` which
-will install the package in a user-writeable folder. The binaries should
-be installed to ``/home/$user/.local/bin/`` in case of Debian-based
-systems.
-
-``circtools`` was developed and tested on Debian Jessie but should also
-run with any distribution.
-
-The installation requires running python on the command line:
-
-::
-
-    git clone https://github.com/dieterich-lab/circtools.git
-    cd circtools
-    python3 setup.py install --verbose --user
-
-The installation procedure will automatically install two dependencies:
-`DCC <https://github.com/dieterich-lab/DCC>`__ and
-`FUCHS <https://github.com/dieterich-lab/FUCHS>`__. The primer-design
-module as well as the exon analysis and circRNA testing module require a
-working installation of `R <https://cran.r-project.org/>`__ with
+Installation is managed through ``pip3 install circtools`` or ``python3 setup.py
+install`` when installed from the cloned GitHub repository. No sudo access is
+required if the installation is executed with ``--user`` which will install the
+package in a user-writeable folder. The binaries should be installed
+to ``/home/$user/.local/bin/`` in case of Debian-based systems.
+
+``circtools`` was developed and tested on Debian Buster, but should also
+run with any other distribution.
+
+The installation can be performed directly from Pypi:
+
+.. code-block:: console
+
+    # install circtools
+    pip install numpy # required for HTSeq, a dependency of circtools
+    pip install circtools
+
+    # install R packages for circtools
+    circtools_install_R_dependencies
+
+Additionally, this repository offers the latest development version:
+
+.. code-block:: console
+
+    pip install numpy # required for HTSeq, a dependency of circtools
+    pip install git+https://github.com/jakobilab/circtools.git
+
+The primer-design module as well as the exon analysis and circRNA testing module
+require a working installation of `R <https://cran.r-project.org/>`__ with
 `BioConductor <https://www.bioconductor.org/install/>`__. All R packages
-required are automatically installed during the setup. Please see the
+required can be automatically installed during the setup. Please see the
 `"Installing circtools" <http://docs.circ.tools/en/latest/Installation.html>`__
 chapter of the main circtools documentation for more detailed installation instructions.
 
 Modules
 -------
 
 Circtools currently offers seven modules:
 
 detect `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Detect.html>`__
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The ``detect`` command is an interface to
-`DCC <https://github.com/dieterich-lab/DCC>`__, also developed at the
+`DCC <https://github.com/dieterich-lab/DCC>`__, developed at the
 Dieterich Lab. The module allows to detect circRNAs from RNA sequencing
 data. The module is the foundation of all other steps for the circtools
 work flow. All parameters supplied to circtools will be directly passed
 to DCC.
 
 quickcheck `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Quickcheck.html>`__
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
@@ -131,23 +138,29 @@
 
 primer `(detailed documentation) <https://circtools.readthedocs.io/en/latest/primer.html>`__
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The ``primer`` command is used to design and visualize primers required
 for follow up wet lab experiments to verify circRNA candidates.
 
+
 .. |docs| image:: https://readthedocs.org/projects/circtools/badge/?version=latest
     :alt: Documentation Status
     :scale: 100%
     :target: https://circtools.readthedocs.io/en/latest/?badge=latest
 
-.. |build| image:: https://travis-ci.org/dieterich-lab/circtools.svg?branch=master
-    :alt: Build Status
+.. |build| image:: https://github.com/jakobilab/circtools/actions/workflows/run_circtools_detect.yml/badge.svg?branch=master
+    :alt: CI Status
+    :scale: 100%
+    :target: https://github.com/jakobilab/circtools/actions/workflows/run_circtools_detect.yml
+
+.. |docker| image:: https://github.com/jakobilab/circtools/actions/workflows/build_docker.yml/badge.svg?branch=master
+    :alt: Docker Build
     :scale: 100%
-    :target: https://travis-ci.org/dieterich-lab/circtools
+    :target: https://github.com/jakobilab/circtools/actions/workflows/build_docker.yml
 
 .. |zenodo| image:: https://zenodo.org/badge/83248654.svg
     :alt: Zenodo DOI link
     :scale: 100%
     :target: https://zenodo.org/badge/latestdoi/83248654
 
 .. |downloads| image:: https://pepy.tech/badge/circtools
```

### Comparing `circtools-1.2.2/circtools/circ_module/circ_template.py` & `circtools-1.3.0/circtools/circ_module/circ_template.py`

 * *Files identical despite different names*

### Comparing `circtools-1.2.2/circtools/circtest/circtest.py` & `circtools-1.3.0/circtools/circtest/circtest.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,25 +46,25 @@
         # let's first check if the output directory exists
         if not (os.access(self.cli_params.output_directory, os.W_OK)):
             self.log_entry("Output directory %s not writable." % self.cli_params.output_directory)
             # exit with -1 error if we can't use it
             exit(-1)
 
         # check DCC directory
-        if not (os.path.exists(self.cli_params.DCC_dir)):
+        if not (os.path.exists(self.cli_params.detect_dir)):
             self.log_entry("DCC/detect data directory %s does not exist (or is not accessible)."
-                           % self.cli_params.DCC_dir)
+                           % self.cli_params.detect_dir)
             # exit with -1 error if we can't use it
             exit(-1)
 
         # check DCC files (only existence, not the content)
         self.check_input_files([
-            self.cli_params.DCC_dir + "CircRNACount",
-            self.cli_params.DCC_dir + "LinearCount",
-            self.cli_params.DCC_dir + "CircCoordinates"
+            self.cli_params.detect_dir + "CircRNACount",
+            self.cli_params.detect_dir + "LinearCount",
+            self.cli_params.detect_dir + "CircCoordinates"
         ])
 
         # check sample names
         if len(self.cli_params.condition_list.split(",")) < 2:
             self.log_entry("Error: Length of parameter list specified via -c is < 2.")
 
         # check columns
@@ -128,19 +128,19 @@
         r_version = m.group(0)
 
         self.log_entry("Using R version %s [%s]" % (r_version, r_location))
 
         # ------------------------------------ need to call the correct R script here -----------------------
 
         # need to define path top R wrapper
-        primer_script = 'circtools_circtest_wrapper.R'
+        primer_script = 'circtools_circtest_wrapper'
 
         # Variable number of args in a list
         args = [
-            self.cli_params.DCC_dir,
+            self.cli_params.detect_dir,
             self.cli_params.num_replicates,
             self.cli_params.condition_list,
             self.cli_params.condition_columns,
             self.cli_params.output_directory + "/" + self.cli_params.output_name,
             self.cli_params.max_fdr,
             self.cli_params.max_plots,
             self.cli_params.filter_sample,
```

### Comparing `circtools-1.2.2/circtools/circtools.py` & `circtools-1.3.0/circtools/circtools.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import argparse
 import os.path
 import sys
 
 # global settings
-version = "1.2.2"
+version = "1.3.0"
 program_name = "circtools"
 
 
 # samtools/git like parsing from http://chase-seibert.github.io/blog/2014/03/21/python-multilevel-argparse.html
 
 
 def main():
@@ -42,25 +42,25 @@
 class CircTools(object):
 
     def __init__(self):
         parser = argparse.ArgumentParser(
             description="circtools: a modular, python-based framework for circRNA-related tools that unifies "
                         "several functions in single command line driven software.",
             usage="""circtools [-V] <command> [<args>]
-            
+
             Available commands:
 
-               enrich:       circular RNA RBP enrichment scan
+               detect:       circular RNA detection
+               quickcheck:   circular RNA sequencing library quick checks
+               circtest:     circular RNA statistical testing
                primex:       circular RNA primer design tool
                sirna:        circular RNA sirna design tool
-               detect:       circular RNA detection with DCC
-               reconstruct:  circular RNA reconstruction with FUCHS
-               circtest:     circular RNA statistical testing
+               reconstruct:  circular RNA reconstruction
+               enrich:       circular RNA RBP enrichment scan
                exon:         circular RNA alternative exon analysis
-               quickcheck:   circular RNA sequencing library quick checks               
             """)
         parser.add_argument("command", help="Command to run")
 
         parser.add_argument("-V",
                             "--version",
                             action="version",
                             version=version
@@ -84,15 +84,15 @@
 
         # REQUIRED ARGUMENTS
         group = parser.add_argument_group("Required options")
 
         group.add_argument("-c",
                            "--circ-file",
                            dest="circ_rna_input",
-                           help="Path to the CircCoordinates file generated by DCC",
+                           help="Path to the CircCoordinates file generated by circtools detect",
                            required=True
                            )
 
         group.add_argument("-b",
                            "--bed-input",
                            dest="bed_input",
                            help="One or more BED files containing features to overlap",
@@ -210,17 +210,17 @@
         parser = argparse.ArgumentParser(
             description="circular RNA primer design")
         # NOT prefixing the argument with -- means it"s not optional
 
         group = parser.add_argument_group("Input")
 
         group.add_argument("-d",
-                           "--dcc-file",
-                           dest="dcc_file",
-                           help="CircCoordinates file from DCC / detect module",
+                           "--detect-dir",
+                           dest="detect_dir",
+                           help="CircCoordinates file from circtools detect module",
                            required=True
                            )
 
         group.add_argument("-g",
                            "--gtf-file",
                            dest="gtf_file",
                            help="GTF file of genome annotation e.g. ENSEMBL",
@@ -336,23 +336,23 @@
         import primex.primex
         primex_instance = primex.primex.Primex(args, program_name, version)
         primex_instance.run_module()
 
     @staticmethod
     def sirna():
         parser = argparse.ArgumentParser(
-            description="circular RNA sirna design")
+            description="circular RNA siRNA design")
         # NOT prefixing the argument with -- means it"s not optional
 
         group = parser.add_argument_group("Input")
 
         group.add_argument("-d",
-                           "--dcc-file",
-                           dest="dcc_file",
-                           help="CircCoordinates file from DCC / detect module",
+                           "--detect-file",
+                           dest="detect_file",
+                           help="CircCoordinates file from circtools detect module",
                            required=True
                            )
 
         group.add_argument("-g",
                            "--gtf-file",
                            dest="gtf_file",
                            help="GTF file of genome annotation e.g. ENSEMBL",
@@ -525,27 +525,27 @@
     def detect():
         parser = argparse.ArgumentParser(
             description="circular RNA detection",
             fromfile_prefix_chars="@",
         )
 
         parser.add_argument("--version", action="version", version=version)
-        parser.add_argument("Command", choices=['detect'])
+
         parser.add_argument("Input", metavar="Input", nargs="+",
                             help="Input of the Chimeric.out.junction file from STAR. Alternatively, a sample sheet "
                                  "specifying where your chimeric.out.junction files are, each sample per line, "
                                  "provide with @ prefix (e.g. @samplesheet)")
         parser.add_argument("-k", "--keep-temp", dest="temp", action="store_true", default=False,
                             help="Temporary files will not be deleted [default: False]")
         parser.add_argument("-T", "--threads", dest="cpu_threads", type=int, default=2,
                             help="Number of CPU threads used for computation [default: 2]")
         parser.add_argument("-O", "--output", dest="out_dir", default="./",
-                            help="DCC output directory [default: .]")
-        parser.add_argument("-t", "--temp", dest="tmp_dir", default="_tmp_DCC/",
-                            help="DCC temporary directory [default: _tmp_DCC/]")
+                            help="Output directory [default: .]")
+        parser.add_argument("-t", "--temp", dest="tmp_dir", default="_tmp_circtools/",
+                            help="Temporary directory [default: _tmp_circtools/]")
 
         group = parser.add_argument_group("Find circRNA Options", "Options to find circRNAs from STAR output")
         group.add_argument("-D", "--detect", action="store_true", dest="detect", default=False,
                            help="Enable circRNA detection from Chimeric.out.junction files [default: False]")
         group.add_argument("-ss", action="store_true", dest="secondstrand", default=False,
                            help="Must be enabled for stranded libraries, aka 'fr-secondstrand' [default: False]")
         group.add_argument("-N", "--nonstrand", action="store_false", dest="strand", default=True,
@@ -591,55 +591,61 @@
 
         group = parser.add_argument_group("Host gene count Options", "Options to count host gene expression")
         group.add_argument("-G", "--gene", action="store_true", dest="gene", default=False,
                            help="If specified, the program will count host gene expression given circRNA coordinates "
                                 "[default: False]")
         group.add_argument("-C", "--circ", dest="circ",
                            help="User specified circRNA coordinates, any tab delimited file with first three "
-                                "columns as circRNA coordinates: chr\tstart\tend, which DCC will use to count "
+                                "columns as circRNA coordinates: chr\tstart\tend, which circtools will use to count "
                                 "host gene expression")
         group.add_argument("-B", "--bam", dest="bam", nargs="+",
                            help="A file specifying the mapped BAM files from which host gene expression is computed; "
                                 "must have the same order as input chimeric junction files")
         group.add_argument("-A", "--refseq", dest="refseq",
                            help="Reference sequence FASTA file")
 
         parser.add_argument_group(group)
 
-        import DCC
-        DCC.main(parser)
+        args = parser.parse_args(sys.argv[2:])
+
+        # make sure we can load the sub module
+        sys.path.append(os.path.join(os.path.dirname(__file__)))
+
+        import detect.detect
+        detect_instance = detect.detect.Detect(args, program_name, version)
+        detect_instance.run_module()
 
     @staticmethod
     def circtest():
         parser = argparse.ArgumentParser(
             description="circular RNA statistical testing - Interface to https://github.com/dieterich-lab/CircTest")
         # NOT prefixing the argument with -- means it"s not optional
 
         ######################################################
 
         group = parser.add_argument_group("Required")
         group.add_argument("-d",
-                           "--DCC",
-                           dest="DCC_dir",
-                           help="Path to the detect/DCC data directory",
+                           "--detect",
+                           dest="detect_dir",
+                           help="Path to the circtools detect data directory",
                            required=True
                            )
 
         group.add_argument("-l",
                            "--condition-list",
                            dest="condition_list",
                            help="Comma-separated list of conditions which should be compared"
                                 "E.g. \"RNaseR +\",\"RNaseR -\"",
                            required=True
                            )
 
         group.add_argument("-c",
                            "--condition-columns",
                            dest="condition_columns",
-                           help="Comma-separated list of 1-based column numbers in the detect/DCC output"
+                           help="Comma-separated list of 1-based column numbers in the circtools detect output"
                                 " which should be compared; e.g. 10,11,12,13,14,15",
                            required=True
                            )
 
         group.add_argument("-g",
                            "--grouping",
                            dest="grouping",
@@ -775,17 +781,17 @@
             description="circular RNA sequencing library quality assessment")
         # NOT prefixing the argument with -- means it"s not optional
 
         ######################################################
 
         group = parser.add_argument_group("Required")
         group.add_argument("-d",
-                           "--DCC",
-                           dest="DCC_dir",
-                           help="Path to the detect/DCC data directory",
+                           "--detect",
+                           dest="detect_dir",
+                           help="Path to the circtools detect data directory",
                            required=True
                            )
 
         group.add_argument("-s",
                            "--star",
                            dest="star_dir",
                            help="Path to the base STAR data directory containing sub-folders with per-sample mappings",
@@ -835,47 +841,47 @@
                            )
 
         group.add_argument("-C",
                            "--cleanup",
                            dest="cleanup",
                            help="String to be removed from each sample name "
                                 "[Default: \"_STARmapping.*Chimeric.out.junction\"]",
-                           default="_STARmapping.*Chimeric.out.junction"
+                           default="*Chimeric.out.junction"
                            )
 
         group.add_argument("-S",
                            "--starfolder",
                            dest="starfolder",
                            help="Suffix string of the STAR folders"
-                                "[Default: \"_STARmapping\"]",
-                           default="_STARmapping"
+                                "[Default: \"\"]",
+                           default=""
                            )
 
         group.add_argument("-L",
                            "--remove-last",
                            dest="remove_suffix_chars",
-                           help="Remove last N characters from each column name of the DCC input data "
+                           help="Remove last N characters from each column name of the circtools detect input data "
                                 "[Default: 0]",
                            type=int,
                            default=0
                            )
 
         group.add_argument("-F",
                            "--remove-first",
                            dest="remove_prefix_chars",
-                           help="Remove first N characters from each column name of the DCC input data "
+                           help="Remove first N characters from each column name of the circtools detect input data "
                                 "[Default: 0]",
                            type=int,
                            default=0
                            )
 
         group.add_argument("-R",
                            "--remove-columns",
                            dest="remove_columns",
-                           help="Comma-separated list of columns in the DCC data files to not includes in the check",
+                           help="Comma-separated list of columns in the circtools detect data files to not includes in the check",
                            default="0"
                            )
         ######################################################
 
         args = parser.parse_args(sys.argv[2:])
 
         # start the primer module
@@ -893,32 +899,32 @@
             description="circular RNA exon usage analysis")
         # NOT prefixing the argument with -- means it"s not optional
 
         ######################################################
 
         group = parser.add_argument_group("Required")
         group.add_argument("-d",
-                           "--DCC",
-                           dest="DCC_dir",
-                           help="Path to the detect/DCC data directory",
+                           "--detect",
+                           dest="detect_dir",
+                           help="Path to the circtools detect data directory",
                            required=True
                            )
 
         group.add_argument("-l",
                            "--condition-list",
                            dest="condition_list",
                            help="Comma-separated list of conditions which should be compared"
                                 "E.g. \"RNaseR +\",\"RNaseR -\"",
                            required=True
                            )
 
         group.add_argument("-c",
                            "--condition-columns",
                            dest="condition_columns",
-                           help="Comma-separated list of 1-based column numbers in the detect/DCC output"
+                           help="Comma-separated list of 1-based column numbers in the circtools detect output"
                                 " which should be compared; e.g. 10,11,12,13,14,15",
                            required=True
                            )
 
         group.add_argument("-g",
                            "--grouping",
                            dest="grouping",
@@ -1010,23 +1016,23 @@
         exon_instance = exon_usage.exon_usage.ExonUsage(args, program_name, version)
         exon_instance.run_module()
 
     @staticmethod
     def reconstruct():
         parser = argparse.ArgumentParser(
             description="circular RNA reconstruction")
-        # NOT prefixing the argument with -- means it"s not optional
+        # NOT prefixing the argument with -- means it's not optional
 
         # input
         parser.add_argument('-C', '--circIDs', dest='circlefile', default='none',
                             help='Tab-separated file chr:start_end(tab)read1,read2,read3.')
-        parser.add_argument('-D', '--DCC', dest='CircRNACount', default='none',
+        parser.add_argument('-D', '--detect', dest='CircRNACount', default='none',
                             help='If you mapped with STAR and are using step1 you need to provide a list'
-                                 ' of circle ids (CircRNACount or CircCoordinates from DCC)'
-                                 'You must supply either -C or -DCC')
+                                 ' of circle ids (CircRNACount or CircCoordinates from circtools detect)'
+                                 'You must supply either -C or -D')
         parser.add_argument('-J', '--chimericJunctions', dest='chimeric_junction', default='none',
                             help='If you mapped with STAR and are using step1 you need to provide the paired end Chimeric.junction.out file here')
         parser.add_argument('-F', '--mate1', dest='mate1', default='none',
                             help='If you mapped with STAR and are using step1 you need to provide the mate1.Chimeric.junction.out file here (optional if ends were mapped separately)')
         parser.add_argument('-R', '--mate2', dest='mate2', default='none',
                             help='If you mapped with STAR and are using step1 you need to provide the mate2.Chimeric.junction.out file here (optional if ends were mapped separately)')
         parser.add_argument('-B', '--bamfile', dest='bamfile', required=True,
@@ -1058,12 +1064,19 @@
                             help='Comma separated list of steps that should be skipped (e.g. step3,step4,step6)')
         parser.add_argument('-T', '--tmp', dest='tmp_folder', default='/tmp/',
                             help='Folder to store temporary files generated by pybedtools.')
 
         parser.add_argument('-P', '--cpus', dest='num_cpus', default=4, type=int,
                             help='Number of CPUs used.')
 
-        import FUCHS
-        FUCHS.main(parser)
+        args = parser.parse_args(sys.argv[2:])
+
+        # make sure we can load the sub module
+        sys.path.append(os.path.join(os.path.dirname(__file__)))
+
+        import reconstruct.reconstruct
+        reconstruct_instance = reconstruct.reconstruct.Reconstruct(args, program_name, version)
+        reconstruct_instance.run_module()
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `circtools-1.2.2/circtools/enrichment/enrichment_check.py` & `circtools-1.3.0/circtools/enrichment/enrichment_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -745,15 +745,15 @@
                                                                        ) - circ_count
                     # key has the form: chromosome_start_stop[strand]
                     key = bed_feature[0] + "_" + \
                           str(bed_feature[1]) + "_" + \
                           str(bed_feature[2]) + "_" + \
                           bed_feature[5]
 
-                    # in feature mode, we extend the ey by count and feature length
+                    # in feature mode, we extend the key by count and feature length
                     if self.virtual_inclusion_file_path != "all":
                         key += "_" + str(bed_feature[4])
 
             else:
 
                 # we have to create the nested dictionaries if not already existing
                 if gene_name not in count_table:
```

### Comparing `circtools-1.2.2/circtools/exon_usage/exon_usage.py` & `circtools-1.3.0/circtools/exon_usage/exon_usage.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,25 +46,25 @@
             exit(-1)
 
         # let's first check if the temporary directory exists
         if not os.path.exists(self.cli_params.output_directory):
             os.makedirs(self.cli_params.output_directory)
 
         # check DCC directory
-        if not (os.path.exists(self.cli_params.DCC_dir)):
+        if not (os.path.exists(self.cli_params.detect_dir)):
             self.log_entry("DCC/detect data directory %s does not exist (or is not accessible)."
-                           % self.cli_params.DCC_dir)
+                           % self.cli_params.detect_dir)
             # exit with -1 error if we can't use it
             exit(-1)
 
         # check DCC files (only existence, not the content)
         self.check_input_files([
-                                self.cli_params.DCC_dir+"CircRNACount",
-                                self.cli_params.DCC_dir+"LinearCount",
-                                self.cli_params.DCC_dir+"CircCoordinates"
+                                self.cli_params.detect_dir+"CircRNACount",
+                                self.cli_params.detect_dir+"LinearCount",
+                                self.cli_params.detect_dir+"CircCoordinates"
                                 ])
 
         # check Ballgown directory
         if self.cli_params.ballgown_data and not (os.path.exists(self.cli_params.ballgown_data)):
             self.log_entry("Ballgown data directory %s does not exist (or is not accessible)."
                            % self.cli_params.ballgown_data)
             # exit with -1 error if we can't use it
@@ -124,15 +124,15 @@
         # ------------------------------------ need to call the correct R script here -----------------------
 
         # need to define path top R wrapper
         exon_script = 'circtools_exon_wrapper.R'
 
         # Variable number of args in a list
         args = [
-                self.cli_params.DCC_dir,
+                self.cli_params.detect_dir,
                 self.cli_params.replicates,
                 self.cli_params.condition_list,
                 self.cli_params.condition_columns,
                 self.cli_params.grouping,
                 self.cli_params.output_directory+"/"+self.cli_params.output_prefix,
                 self.cli_params.ballgown_data,
                 self.cli_params.gtf_file,
```

### Comparing `circtools-1.2.2/circtools/mirna/mirna.py` & `circtools-1.3.0/circtools/scripts/circtools_merge_enrich_results.sh`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,25 @@
-#! /usr/bin/env python3
+#!/bin/bash
 
-# Copyright (C) 2017 Tobias Jakobi
+# Copyright (C) 2018 Tobias Jakobi
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either self.version 3 of the License, or
-# (at your option) any later self.version.
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-import circ_module.circ_template
 
+# check if we have 2 arguments
+if [ ! $# == 4 ]; then
+  echo "Usage: $0 [Input path to enrich results] [Number of iterations (for regex)] [target dir e.g. /tmp/] [file name]"
+  exit
+fi
 
-class MirnaModule(circ_module.circ_template.CircTemplate):
-    def __init__(self, argparse_arguments, program_name, version):
-
-        # get the user supplied options
-        self.cli_params = argparse_arguments
-        self.program_name = program_name
-        self.version = version
-
-    def run_module(self):
-        return
-
-    def module_name(self):
-        """"Return a string representing the name of the module."""
-        return self.program_name
+awk -v OFS='\t' -F '\t' '{print FILENAME,$0}' $1/*.csv |  sed "s/_${2}_.*.csv//g" | sed "s~$1~~" | sed "s~/~~" | grep -v circRNA_host_gene > $3/$4
```

### Comparing `circtools-1.2.2/circtools/primex/primex.py` & `circtools-1.3.0/circtools/primex/primex.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         self.cli_params = argparse_arguments
         self.program_name = program_name
         self.version = version
         self.command = 'Rscript'
         self.temp_dir = self.cli_params.global_temp_dir
         self.gtf_file = self.cli_params.gtf_file
         self.fasta_file = self.cli_params.fasta_file
-        self.dcc_file = self.cli_params.dcc_file
+        self.detect_dir = self.cli_params.detect_dir
         self.output_dir = self.cli_params.output_dir
         self.organism = self.cli_params.organism
         self.gene_list = self.cli_params.gene_list
         self.id_list = self.cli_params.id_list
         self.product_range = self.cli_params.product_size
         self.junction = self.cli_params.junction
         self.no_blast = self.cli_params.blast
@@ -219,15 +219,15 @@
 
                     data_store.write("\t".join([name, str(record.seq), "", "\n"]))
                     exon_cache[name] = {1: str(record.seq), 2: ""}
 
         else:
             exons = self.read_annotation_file(self.gtf_file, entity="exon")
 
-            with open(self.dcc_file) as fp:
+            with open(self.detect_dir) as fp:
 
                 for line in fp:
 
                     # make sure we remove the header
                     if line.startswith('Chr\t'):
                         continue
 
@@ -342,15 +342,15 @@
                         data_store.write("\t".join([name, exon1, exon2, "\n"]))
 
         if not exon_cache:
             print("Could not find any circRNAs matching your criteria, exiting.")
             exit(-1)
 
         # need to define path top R wrapper
-        primer_script = 'circtools_primex_wrapper.R'
+        primer_script = 'circtools_primex_wrapper'
 
         # ------------------------------------ run script and check output -----------------------
 
         script_result = os.popen(primer_script + " " +
                                  exon_storage_tmp + " " +
                                  str(self.product_range[0]) + "," + str(self.product_range[1]) + " " +
                                  self.junction + " " + str(self.num_pairs)).read()
@@ -464,15 +464,15 @@
             # update line
             primex_data_with_blast_results += line + "\t" + left_result + "\t" + right_result + "\n"
 
         with open(blast_storage_tmp, 'w') as data_store:
             data_store.write(primex_data_with_blast_results)
 
         # need to define path top R wrapper
-        primer_script = 'circtools_primex_formatter.R'
+        primer_script = 'circtools_primex_formatter'
 
         # ------------------------------------ run script and check output -----------------------
 
         primex_data_formatted = os.popen(primer_script + " " +
                                          blast_storage_tmp + " "
                                          + "\"" + self.experiment_title + "\""
                                          ).read()
@@ -520,31 +520,39 @@
 
                 product_size = entry[14]
 
                 gdd = GenomeDiagram.Diagram('circRNA primer diagram')
                 gdt_features = gdd.new_track(1, greytrack=True, name="", )
                 gds_features = gdt_features.new_set()
 
-                feature = SeqFeature(FeatureLocation(0, exon1_length), strand=+1)
+                feature = SeqFeature(FeatureLocation(0, exon1_length))
+                feature.location.strand = +1
                 gds_features.add_feature(feature, name="Exon 1", label=False, color="#ff6877", label_size=22)
 
-                feature = SeqFeature(FeatureLocation(circrna_length - exon2_length, circrna_length), strand=+1)
+                feature = SeqFeature(FeatureLocation(circrna_length - exon2_length, circrna_length))
+                feature.location.strand = +1
+
                 gds_features.add_feature(feature, name="Exon 2", label=False, color=exon2_colour, label_size=22)
 
-                feature = SeqFeature(FeatureLocation(forward_primer_start, circrna_length), strand=-1)
+                feature = SeqFeature(FeatureLocation(forward_primer_start, circrna_length))
+                feature.location.strand = -1
+
                 gds_features.add_feature(feature, name="Product", label=False, color="#6881ff")
 
-                feature = SeqFeature(FeatureLocation(0, reverse_primer_start), strand=-1)
+                feature = SeqFeature(FeatureLocation(0, reverse_primer_start))
+                feature.location.strand = -1
+
                 gds_features.add_feature(feature, name="Product: " + product_size + "bp", label=False, color="#6881ff",
                                          label_size=22, label_position="middle")
 
                 if self.junction == "f":
 
-                    feature = SeqFeature(FeatureLocation(reverse_primer_start - reverse_primer_length, reverse_primer_start),
-                                         strand=-1)
+                    feature = SeqFeature(FeatureLocation(reverse_primer_start - reverse_primer_length, reverse_primer_start))
+                    feature.location.strand = -1
+
                     gds_features.add_feature(feature, name="Reverse", label=False, sigil="BIGARROW", color="#75ff68",
                                              arrowshaft_height=0.3, arrowhead_length=0.1, label_size=22)
 
                     # the primer spans the BSJ, therefore we have to draw it in two pieces:
                     # piece 1: primer start to circRNA end
                     # piece 2: remaining primer portion beginning from 0
 
@@ -560,15 +568,17 @@
                                              arrowshaft_height=0.3, arrowhead_length=0.1, label_size=22)
                 elif self.junction == "r":
                     # the primer spans the BSJ, therefore we have to draw it in two pieces:
                     # piece 1: primer start of circRNA to circRNA end
                     # piece 2: remaining primer portion beginning from 0
 
                     # piece 1:
-                    feature = SeqFeature(FeatureLocation(circrna_length - reverse_primer_start, circrna_length), strand=-1)
+                    feature = SeqFeature(FeatureLocation(circrna_length - reverse_primer_start, circrna_length))
+                    feature.location.strand = -1
+
                     gds_features.add_feature(feature, name="Reverse", label=False, sigil="BIGARROW", color="#75ff68",
                                              arrowshaft_height=0.3, arrowhead_length=0.1, label_size=22)
 
                     # piece 2:
                     feature = SeqFeature(
                         FeatureLocation(0, reverse_primer_start), strand=-1)
                     gds_features.add_feature(feature, name="Reverse", label=False, sigil="BIGARROW", color="#75ff68",
@@ -576,16 +586,17 @@
 
                     feature = SeqFeature(
                         FeatureLocation(forward_primer_start, forward_primer_start + forward_primer_length))
                     gds_features.add_feature(feature, name="Forward", label=False, sigil="BIGARROW", color="#75ff68",
                                              arrowshaft_height=0.3, arrowhead_length=0.1, label_size=22)
                 else:
                     feature = SeqFeature(
-                        FeatureLocation(reverse_primer_start - reverse_primer_length, reverse_primer_start),
-                        strand=-1)
+                        FeatureLocation(reverse_primer_start - reverse_primer_length, reverse_primer_start))
+                    feature.location.strand = -1
+
                     gds_features.add_feature(feature, name="Reverse", label=False, sigil="BIGARROW", color="#75ff68",
                                              arrowshaft_height=0.3, arrowhead_length=0.1, label_size=22)
 
                     feature = SeqFeature(
                         FeatureLocation(forward_primer_start, forward_primer_start + forward_primer_length))
                     gds_features.add_feature(feature, name="Forward", label=False, sigil="BIGARROW", color="#75ff68",
                                              arrowshaft_height=0.3, arrowhead_length=0.1, label_size=22)
@@ -596,15 +607,17 @@
                 if circular_rna_id in flanking_exon_cache:
                     for exon in flanking_exon_cache[circular_rna_id]:
                         exon_start, exon_stop = exon.split('_')
 
                         exon_start = int(exon_start) - int(entry[2])
                         exon_stop = int(exon_stop) - int(entry[2])
 
-                        feature = SeqFeature(FeatureLocation(exon_start, exon_stop), strand=+1)
+                        feature = SeqFeature(FeatureLocation(exon_start, exon_stop))
+                        feature.location.strand = +1
+
                         gds_features.add_feature(feature, name="Exon", label=False, color="grey", label_size=22)
 
                 gdd.draw(format='circular', pagesize=(600, 600), circle_core=0.6, track_size=0.3, tracklines=0, x=0.00,
                          y=0.00, start=0, end=circrna_length-1)
 
                 gdd.write(self.output_dir + "/" + circular_rna_id_isoform + ".svg", "svg")
```

### Comparing `circtools-1.2.2/circtools/quickcheck/quickcheck.py` & `circtools-1.3.0/circtools/quickcheck/quickcheck.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,26 +45,26 @@
 
         # let's first check if the output directory exists
         if not (os.access(self.cli_params.output_directory, os.W_OK)):
             self.log_entry("Output directory %s not writable." % self.cli_params.output_directory)
             # exit with -1 error if we can't use it
             exit(-1)
 
-        # check DCC directory
-        if not (os.path.exists(self.cli_params.DCC_dir)):
-            self.log_entry("DCC/detect data directory %s does not exist (or is not accessible)."
-                           % self.cli_params.DCC_dir)
+        # check circtools detect directory
+        if not (os.path.exists(self.cli_params.detect_dir)):
+            self.log_entry("circtools detect data directory %s does not exist (or is not accessible)."
+                           % self.cli_params.detect_dir)
             # exit with -1 error if we can't use it
             exit(-1)
 
-        # check DCC files (only existence, not the content)
+        # check circtools detect files (only existence, not the content)
         self.check_input_files([
-                                self.cli_params.DCC_dir+"CircRNACount",
-                                self.cli_params.DCC_dir+"LinearCount",
-                                self.cli_params.DCC_dir+"CircCoordinates"
+                                self.cli_params.detect_dir+"CircRNACount",
+                                self.cli_params.detect_dir+"LinearCount",
+                                self.cli_params.detect_dir+"CircCoordinates"
                                 ])
 
         # check STAR directory
         if not (os.path.exists(self.cli_params.star_dir)):
             self.log_entry("STAR data directory %s does not exist (or is not accessible)."
                            % self.cli_params.star_dir)
             # exit with -1 error if we can't use it
@@ -105,22 +105,22 @@
         r_version = m.group(0)
 
         self.log_entry("Using R version %s [%s]" % (r_version, r_location))
 
         # ------------------------------------ need to call the correct R script here -----------------------
 
         # need to define path top R wrapper
-        quickcheck_script = 'circtools_quickcheck_wrapper.R'
+        quickcheck_script = 'circtools_quickcheck_wrapper'
 
         if self.cli_params.starfolder == "":
             self.cli_params.starfolder = 0
 
         # Variable number of args in a list
         args = [
-                self.cli_params.DCC_dir,
+                self.cli_params.detect_dir,
                 self.cli_params.star_dir,
                 self.cli_params.output_directory + "/" + self.cli_params.output_name,
                 self.cli_params.condition_list,
                 self.cli_params.grouping,
                 self.cli_params.colour,
                 self.cli_params.cleanup,
                 self.cli_params.starfolder,
```

### Comparing `circtools-1.2.2/circtools/sirna/sirna.py` & `circtools-1.3.0/circtools/sirna/sirna.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.homo_sapiens_blast_db = "GPIPE/9606/current/rna"
         self.mus_musculus_blast_db = "GPIPE/10090/current/rna"
         self.rattus_norvegicus_blast_db = "GPIPE/10116/current/rna"
         self.sus_scrofa_blast_db = "GPIPE/9823/current/rna"
 
         self.other_blast_db = "nt"
         
-        self.dcc_file = self.cli_params.dcc_file
+        self.detect_dir = self.cli_params.detect_dir
 
         self.fasta_file = self.cli_params.fasta_file
         self.gtf_file = self.cli_params.gtf_file
         
         self.gene_list = self.cli_params.gene_list
         self.id_list = self.cli_params.id_list
         self.input_circRNA = self.cli_params.sequence_file
@@ -181,16 +181,16 @@
                 seq = str(record.seq)
                 bsj = seq[-31:] + seq[0:31]
                 self.exon_cache[name] = {1: str(record.seq), 2: "", 3: bsj}
                 
         else:
             exons = self.read_annotation_file(self.gtf_file, entity="exon")
 
-            dcc_file = self.dcc_file
-            with open(dcc_file) as fp:
+            detect_dir = self.detect_dir
+            with open(detect_dir) as fp:
 
                 for line in fp:
 
                     # make sure we remove the header
                     if line.startswith('Chr\t'):
                         continue
```

### Comparing `circtools-1.2.2/circtools.egg-info/PKG-INFO` & `circtools-1.3.0/circtools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: circtools
-Version: 1.2.2
+Version: 1.3.0
 Summary: circtools - a circular RNA toolbox
-Home-page: https://github.com/dieterich-lab/circtools
+Home-page: https://github.com/jakobilab/circtools
 Author: Tobias Jakobi
-Author-email: Tobias.Jakobi@med.Uni-Heidelberg.DE
+Author-email: tjakobi@arizona.edu
 License: GNU General Public License (GPL)
-Project-URL: Bug Reports, https://github.com/dieterich-lab/circtools/issues
-Project-URL: Dieterich Lab, https://dieterichlab.org
-Project-URL: Source, https://github.com/dieterich-lab/circtools
-Project-URL: Documentation, http://docs.circ.tools
-Keywords: circular RNA bioinformatics
+Project-URL: Bug Reports, https://github.com/jakobilab/circtools/issues
+Project-URL: Jakobi Lab, https://jakobilab.org
+Project-URL: Source, https://github.com/jakobilab/circtools
+Project-URL: Documentation, https://docs.circ.tools
+Keywords: circRNA,circular RNA bioinformatics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >3.5
-License-File: LICENSE
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
 
 **circtools**
 ======================================================================
 
 **a one-stop software solution for circular RNA research**
 
-.. figure:: https://raw.githubusercontent.com/dieterich-lab/circtools/master/docs/img/circtools_200px.png
+.. figure:: https://raw.githubusercontent.com/jakobilab/circtools/master/docs/img/circtools_200px.png
    :alt: circtools
 
-|docs| |build| |zenodo| |downloads| |pypi|
+|docs| |build| |docker| |zenodo| |downloads| |pypi|
 
 Introduction
 -------------
 
 Circular RNAs (circRNAs) originate through back-splicing events from linear primary transcripts, are resistant to exonucleases, typically not polyadenylated, and have been shown to be highly specific for cell type and developmental stage. Although few circular RNA molecules have been shown to exhibit miRNA sponge function, for the vast majority of circRNAs however, their function is yet to be determined.
 
 The prediction of circular RNAs is a multi-stage bioinformatics process starting with raw sequencing data and usually ending with a list of potential circRNA candidates which, depending on tissue and condition may contain hundreds to thousands of potential circRNAs. While there already exist a number of tools for the prediction process (e.g. `DCC <https://github.com/dieterich-lab/DCC>`__ and `CircTest <https://github.com/dieterich-lab/CircTest>`__), publicly available downstream analysis tools are rare.
@@ -42,63 +42,70 @@
 a quick check of circRNA mapping results, RBP enrichment screenings, circRNA primer design, statistical testing, and an exon usage module.
 
 
 
 Documentation
 -------------
 
-Click `here <http://docs.circ.tools/>`__ to access the complete documentation on Read the Docs.
+Click `here <https://docs.circ.tools/>`__ to access the complete documentation on Read the Docs.
 
 Installation
 ------------
 
-The ``circtools`` package is written in Python3 (>=3.4), two modules, namely ``detect`` and ``reconstruct`` also require a working Python 2 installation (>=2.7). It requires only a small number of external dependencies, namely standard bioinformatics tools:
+The ``circtools`` package is written in Python 3 (supporting Python 3.7 - 3.10). It requires only a small number of external dependencies, namely standard bioinformatics tools:
 
 -  `bedtools (>= 2.27.1) <https://bedtools.readthedocs.io/en/latest/content/installation.html>`__
    [RBP enrichment module, installed automatically]
--  `R (>= 3.3) <https://www.digitalocean.com/community/tutorials/how-to-install-r-on-ubuntu-16-04-2>`__
+-  `R (>= 4.0) <https://www.digitalocean.com/community/tutorials/how-to-install-r-on-ubuntu-22-04>`__
    [Data visualization and data processing]
 
-Installation is managed through ``python3 setup.py install``. No sudo
-access is required if the installation is executed with ``--user`` which
-will install the package in a user-writeable folder. The binaries should
-be installed to ``/home/$user/.local/bin/`` in case of Debian-based
-systems.
-
-``circtools`` was developed and tested on Debian Jessie but should also
-run with any distribution.
-
-The installation requires running python on the command line:
-
-::
-
-    git clone https://github.com/dieterich-lab/circtools.git
-    cd circtools
-    python3 setup.py install --verbose --user
-
-The installation procedure will automatically install two dependencies:
-`DCC <https://github.com/dieterich-lab/DCC>`__ and
-`FUCHS <https://github.com/dieterich-lab/FUCHS>`__. The primer-design
-module as well as the exon analysis and circRNA testing module require a
-working installation of `R <https://cran.r-project.org/>`__ with
+Installation is managed through ``pip3 install circtools`` or ``python3 setup.py
+install`` when installed from the cloned GitHub repository. No sudo access is
+required if the installation is executed with ``--user`` which will install the
+package in a user-writeable folder. The binaries should be installed
+to ``/home/$user/.local/bin/`` in case of Debian-based systems.
+
+``circtools`` was developed and tested on Debian Buster, but should also
+run with any other distribution.
+
+The installation can be performed directly from Pypi:
+
+.. code-block:: console
+
+    # install circtools
+    pip install numpy # required for HTSeq, a dependency of circtools
+    pip install circtools
+
+    # install R packages for circtools
+    circtools_install_R_dependencies
+
+Additionally, this repository offers the latest development version:
+
+.. code-block:: console
+
+    pip install numpy # required for HTSeq, a dependency of circtools
+    pip install git+https://github.com/jakobilab/circtools.git
+
+The primer-design module as well as the exon analysis and circRNA testing module
+require a working installation of `R <https://cran.r-project.org/>`__ with
 `BioConductor <https://www.bioconductor.org/install/>`__. All R packages
-required are automatically installed during the setup. Please see the
+required can be automatically installed during the setup. Please see the
 `"Installing circtools" <http://docs.circ.tools/en/latest/Installation.html>`__
 chapter of the main circtools documentation for more detailed installation instructions.
 
 Modules
 -------
 
 Circtools currently offers seven modules:
 
 detect `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Detect.html>`__
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The ``detect`` command is an interface to
-`DCC <https://github.com/dieterich-lab/DCC>`__, also developed at the
+`DCC <https://github.com/dieterich-lab/DCC>`__, developed at the
 Dieterich Lab. The module allows to detect circRNAs from RNA sequencing
 data. The module is the foundation of all other steps for the circtools
 work flow. All parameters supplied to circtools will be directly passed
 to DCC.
 
 quickcheck `(detailed documentation) <https://circtools.readthedocs.io/en/latest/Quickcheck.html>`__
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
@@ -154,23 +161,29 @@
 
 primer `(detailed documentation) <https://circtools.readthedocs.io/en/latest/primer.html>`__
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The ``primer`` command is used to design and visualize primers required
 for follow up wet lab experiments to verify circRNA candidates.
 
+
 .. |docs| image:: https://readthedocs.org/projects/circtools/badge/?version=latest
     :alt: Documentation Status
     :scale: 100%
     :target: https://circtools.readthedocs.io/en/latest/?badge=latest
 
-.. |build| image:: https://travis-ci.org/dieterich-lab/circtools.svg?branch=master
-    :alt: Build Status
+.. |build| image:: https://github.com/jakobilab/circtools/actions/workflows/run_circtools_detect.yml/badge.svg?branch=master
+    :alt: CI Status
+    :scale: 100%
+    :target: https://github.com/jakobilab/circtools/actions/workflows/run_circtools_detect.yml
+
+.. |docker| image:: https://github.com/jakobilab/circtools/actions/workflows/build_docker.yml/badge.svg?branch=master
+    :alt: Docker Build
     :scale: 100%
-    :target: https://travis-ci.org/dieterich-lab/circtools
+    :target: https://github.com/jakobilab/circtools/actions/workflows/build_docker.yml
 
 .. |zenodo| image:: https://zenodo.org/badge/83248654.svg
     :alt: Zenodo DOI link
     :scale: 100%
     :target: https://zenodo.org/badge/latestdoi/83248654
 
 .. |downloads| image:: https://pepy.tech/badge/circtools
```

### Comparing `circtools-1.2.2/scripts/circtools_circtest_wrapper.R` & `circtools-1.3.0/circtools/scripts/circtools_circtest_wrapper.R`

 * *Files identical despite different names*

### Comparing `circtools-1.2.2/scripts/circtools_enrich_visualization.R` & `circtools-1.3.0/circtools/scripts/circtools_enrich_visualization.R`

 * *Files identical despite different names*

### Comparing `circtools-1.2.2/scripts/circtools_exon_wrapper.R` & `circtools-1.3.0/circtools/scripts/circtools_exon_wrapper.R`

 * *Files identical despite different names*

### Comparing `circtools-1.2.2/scripts/circtools_generate_flanking_introns.py` & `circtools-1.3.0/circtools/scripts/circtools_generate_flanking_introns.py`

 * *Files identical despite different names*

### Comparing `circtools-1.2.2/scripts/circtools_generate_intron_gtf.sh` & `circtools-1.3.0/circtools/scripts/circtools_generate_intron_gtf.sh`

 * *Files identical despite different names*

### Comparing `circtools-1.2.2/scripts/circtools_merge_enrich_results.sh` & `circtools-1.3.0/circtools/scripts/bash_runner.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,32 @@
-#!/bin/bash
+#!/usr/bin/env python3
 
-# Copyright (C) 2018 Tobias Jakobi
+# Copyright (C) 2023 Tobias Jakobi
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+# runner idea from https://stackoverflow.com/a/73649412/1900920
 
-# check if we have 2 arguments
-if [ ! $# == 4 ]; then
-  echo "Usage: $0 [Input path to enrich results] [Number of iterations (for regex)] [target dir e.g. /tmp/] [file name]"
-  exit
-fi
+import subprocess
+import circtools as _
+
+base_path = _.__path__[0]
+
+
+def _run(bash_script):
+    return subprocess.call(bash_script, shell=True)
+
+
+def wonderdump():
+    return _run("/" + base_path + "/scripts/wonderdump")
 
-awk -v OFS='\t' -F '\t' '{print FILENAME,$0}' $1/*.csv |  sed "s/_${2}_.*.csv//g" | sed "s~$1~~" | sed "s~/~~" | grep -v circRNA_host_gene > $3/$4
```

### Comparing `circtools-1.2.2/scripts/circtools_primex_formatter.R` & `circtools-1.3.0/circtools/scripts/circtools_primex_formatter.R`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env Rscript
 
 # suppress loading messages
 suppressMessages(library(formattable))
 suppressMessages(library(kableExtra))
 suppressMessages(library(dplyr))
 suppressMessages(library(RColorBrewer))
-suppressMessages(library(colortools))
+# suppressMessages(library(colortools))
 
 # switch to red warning color if more blast hits are found
 high_count_number = 0
 
 args <- commandArgs(trailingOnly = TRUE)
 
 experiment_name <- args[2]
@@ -79,18 +79,14 @@
         from <- default_value - bottom_val
         to <- default_value + bottom_val
     }
 
     return(as.character(cut(column,seq( from, to, length.out= length(palette)+1 ), labels=palette, include.lowest = T)))
 }
 
-generate_complementary_column <- function (input){
-    return (complementary(input)[2])
-}
-
 # read data file name from args
 data_file_name <- args[1]
 
 # read whole file into data table
 data_table <- read.csv(data_file_name, header = FALSE, sep = "\t")
 data_table$circid <- paste(data_table$V1,data_table$V2,data_table$V3,data_table$V4,data_table$V5,data_table$V6,sep="_")
```

### Comparing `circtools-1.2.2/scripts/circtools_primex_wrapper.R` & `circtools-1.3.0/circtools/scripts/circtools_primex_wrapper.R`

 * *Files identical despite different names*

### Comparing `circtools-1.2.2/scripts/circtools_quickcheck_wrapper.R` & `circtools-1.3.0/circtools/scripts/circtools_quickcheck_wrapper.R`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
 # summing up counts per column (i.e. library)
 circ_counts_summed <- apply(CircRNACount[, - c(1 : 3)], 2, sum)
 linear_counts_summed <- apply(LinearCount[, - c(1 : 3)], 2, sum)
 
 num_samples <- ncol(LinearCount[, - c(1 : 3)])
 
-message(paste("Found ", num_samples, " data columns in provided DCC data", sep=""))
+message(paste("Found ", num_samples, " data columns in provided data", sep=""))
 
 message(paste(group_length, " different groups provided", sep=""))
 
 if (length(arg_grouping) < num_samples) {
   message("Assuming (1,2),(1,2),(1,2),... sample grouping")
   dummy_list <- rep(arg_grouping, (num_samples/group_length))
   colors <- unlist(lapply(seq(1, num_samples), function(x) {
```

### Comparing `circtools-1.2.2/scripts/circtools_reconstruct_visualization.R` & `circtools-1.3.0/circtools/scripts/circtools_reconstruct_visualization.R`

 * *Files identical despite different names*

### Comparing `circtools-1.2.2/scripts/circtools_sirna_formatter.R` & `circtools-1.3.0/circtools/scripts/circtools_sirna_formatter.R`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 # suppress loading messages
 suppressMessages(library(formattable))
 suppressMessages(library(kableExtra))
 suppressMessages(library(dplyr))
 suppressMessages(library(magrittr))
 suppressMessages(library(RColorBrewer))
-suppressMessages(library(colortools))
 
 # switch to red warning color if more blast hits are found
 high_count_number = 0
 
 args <- commandArgs(trailingOnly = TRUE)
 experiment_name <- args[4]
 #experiment_name <- "testing"
@@ -110,18 +109,14 @@
   color_column = c()
   for(val in column){
     color_column <- append(color_column, "#ffffff")
   }
   return(as.character(color_column))
 }
 
-generate_complementary_column <- function (input){
-  return (complementary(input)[2])
-}
-
 # read data file name from args
 
 #args <- commandArgs(trailingOnly = TRUE)
 csv <- args[1]
 blast_r <- args[2]
 output_dir <- args[3]
 experiment_title <- args[4]
```

### Comparing `circtools-1.2.2/scripts/create_igv_script.py` & `circtools-1.3.0/circtools/scripts/create_igv_script.py`

 * *Files 5% similar despite different names*

```diff
@@ -168,87 +168,89 @@
                     entries_list[host_gene]['location'][location][cell][rbp] = 1
 
     return entries_list
 
 
 # main script starts here
 
-parser = argparse.ArgumentParser(description='Create an auto-executing IGV script')
+def main():
 
-group = parser.add_argument_group("Input")
+    parser = argparse.ArgumentParser(description='Create an auto-executing IGV script')
 
-group.add_argument("-e",
-                   "--enrichment-file",
-                   dest="enrichment_file",
-                   help="An enrichment module output file",
-                   required=True
-                   )
-
-group.add_argument("-b",
-                   "--bam-files",
-                   dest="bam_files",
-                   nargs='*',
-                   help="List of one or more BAM files with read mapping data",
-                   required=True
-                   )
-
-group.add_argument("-a",
-                   "--alternative-exon-dirs",
-                   dest="alt_exon_dirs",
-                   nargs='*',
-                   help="List of one or more directories containing the result files "
-                        "of the exon module",
-                   required=True
-                   )
-
-group.add_argument("-f",
-                   "--fuchs-files",
-                   dest="fuchs_files",
-                   nargs='*',
-                   help="List of one or more BED files containing results of "
-                        "FUCHS / reconstruct module",
-                   required=True
-                   )
-
-group.add_argument("-c",
-                   "--clip-peaks",
-                   dest="peak_directory",
-                   help="Directory of the CLIP peal bed files",
-                   required=True
-                   )
-
-group.add_argument("-g",
-                   "--genome",
-                   dest="genome_build",
-                   help="Which genome build to use as reference [Default: hg38]",
-                   choices=("hg38", "hg19", "mm9", "mm10"),
-                   default="hg38"
-                   )
-
-group.add_argument("-s",
-                   "--samples",
-                   dest="sample_list",
-                   nargs='*',
-                   help="List of one or more sample/conditions",
-                   required=True
-                   )
-
-group.add_argument("-m",
-                   "--max-number",
-                   dest="max_genes",
-                   help="Maximum number of genes to show [Default: 5]",
-                   type=int,
-                   default=5
-                   )
-
-group = parser.add_argument_group("Output")
-
-group.add_argument("-o",
-                   "--output-directory",
-                   dest="output_directory",
-                   help="Directory for snapshots created by IGV [Default: ./]",
-                   default="./"
-                   )
+    group = parser.add_argument_group("Input")
 
-args = parser.parse_args()
+    group.add_argument("-e",
+                       "--enrichment-file",
+                       dest="enrichment_file",
+                       help="An enrichment module output file",
+                       required=True
+                       )
+
+    group.add_argument("-b",
+                       "--bam-files",
+                       dest="bam_files",
+                       nargs='*',
+                       help="List of one or more BAM files with read mapping data",
+                       required=True
+                       )
+
+    group.add_argument("-a",
+                       "--alternative-exon-dirs",
+                       dest="alt_exon_dirs",
+                       nargs='*',
+                       help="List of one or more directories containing the result files "
+                            "of the exon module",
+                       required=True
+                       )
+
+    group.add_argument("-f",
+                       "--fuchs-files",
+                       dest="fuchs_files",
+                       nargs='*',
+                       help="List of one or more BED files containing results of "
+                            "FUCHS / reconstruct module",
+                       required=True
+                       )
+
+    group.add_argument("-c",
+                       "--clip-peaks",
+                       dest="peak_directory",
+                       help="Directory of the CLIP peal bed files",
+                       required=True
+                       )
+
+    group.add_argument("-g",
+                       "--genome",
+                       dest="genome_build",
+                       help="Which genome build to use as reference [Default: hg38]",
+                       choices=("hg38", "hg19", "mm9", "mm10"),
+                       default="hg38"
+                       )
+
+    group.add_argument("-s",
+                       "--samples",
+                       dest="sample_list",
+                       nargs='*',
+                       help="List of one or more sample/conditions",
+                       required=True
+                       )
+
+    group.add_argument("-m",
+                       "--max-number",
+                       dest="max_genes",
+                       help="Maximum number of genes to show [Default: 5]",
+                       type=int,
+                       default=5
+                       )
+
+    group = parser.add_argument_group("Output")
+
+    group.add_argument("-o",
+                       "--output-directory",
+                       dest="output_directory",
+                       help="Directory for snapshots created by IGV [Default: ./]",
+                       default="./"
+                       )
 
-build_tracks(args)
+    args = parser.parse_args()
+
+    build_tracks(args)
```

### Comparing `circtools-1.2.2/scripts/create_igv_script_from_gene_names.py` & `circtools-1.3.0/circtools/scripts/create_igv_script_from_gene_names.py`

 * *Files 10% similar despite different names*

```diff
@@ -128,73 +128,74 @@
                 if location not in entries_list[host_gene]['location']:
                     entries_list[host_gene]['location'][location] = 1
 
     return entries_list
 
 
 # main script starts here
+def main():
 
-parser = argparse.ArgumentParser(description='Create an auto-executing IGV script')
+    parser = argparse.ArgumentParser(description='Create an auto-executing IGV script')
 
-group = parser.add_argument_group("Input")
+    group = parser.add_argument_group("Input")
 
-group.add_argument("-i",
-                   "--input-file",
-                   dest="input_file",
-                   help="A CSV/BED file from DCC / CircTest",
-                   required=True
-                   )
-
-group.add_argument("-b",
-                   "--bam-files",
-                   dest="bam_files",
-                   nargs='*',
-                   help="List of one or more BAM files with read mapping data",
-                   required=True
-                   )
-
-group.add_argument("-a",
-                   "--alternative-exon-dirs",
-                   dest="alt_exon_dirs",
-                   nargs='*',
-                   help="List of one or more directories containing the result files "
-                        "of the exon module",
-                   required=True
-                   )
-
-group.add_argument("-f",
-                   "--fuchs-files",
-                   dest="fuchs_files",
-                   nargs='*',
-                   help="List of one or more BED files containing results of "
-                        "FUCHS / reconstruct module",
-                   required=True
-                   )
-
-group.add_argument("-g",
-                   "--genome",
-                   dest="genome_build",
-                   help="Which genome build to use as reference [Default: hg38]",
-                   choices=("hg38", "hg19", "mm9", "mm10"),
-                   default="hg38"
-                   )
-
-group.add_argument("-m",
-                   "--max-number",
-                   dest="max_genes",
-                   help="Maximum number of genes to show [Default: 5]",
-                   type=int,
-                   default=5
-                   )
-
-group = parser.add_argument_group("Output")
-
-group.add_argument("-o",
-                   "--output-directory",
-                   dest="output_directory",
-                   help="Directory for snapshots created by IGV [Default: ./]",
-                   default="./"
-                   )
+    group.add_argument("-i",
+                       "--input-file",
+                       dest="input_file",
+                       help="A CSV/BED file from DCC / CircTest",
+                       required=True
+                       )
+
+    group.add_argument("-b",
+                       "--bam-files",
+                       dest="bam_files",
+                       nargs='*',
+                       help="List of one or more BAM files with read mapping data",
+                       required=True
+                       )
+
+    group.add_argument("-a",
+                       "--alternative-exon-dirs",
+                       dest="alt_exon_dirs",
+                       nargs='*',
+                       help="List of one or more directories containing the result files "
+                            "of the exon module",
+                       required=True
+                       )
+
+    group.add_argument("-f",
+                       "--fuchs-files",
+                       dest="fuchs_files",
+                       nargs='*',
+                       help="List of one or more BED files containing results of "
+                            "FUCHS / reconstruct module",
+                       required=True
+                       )
+
+    group.add_argument("-g",
+                       "--genome",
+                       dest="genome_build",
+                       help="Which genome build to use as reference [Default: hg38]",
+                       choices=("hg38", "hg19", "mm9", "mm10"),
+                       default="hg38"
+                       )
+
+    group.add_argument("-m",
+                       "--max-number",
+                       dest="max_genes",
+                       help="Maximum number of genes to show [Default: 5]",
+                       type=int,
+                       default=5
+                       )
+
+    group = parser.add_argument_group("Output")
+
+    group.add_argument("-o",
+                       "--output-directory",
+                       dest="output_directory",
+                       help="Directory for snapshots created by IGV [Default: ./]",
+                       default="./"
+                       )
 
-args = parser.parse_args()
+    args = parser.parse_args()
 
-build_tracks(args)
+    build_tracks(args)
```

### Comparing `circtools-1.2.2/scripts/create_igv_script_from_position_list.py` & `circtools-1.3.0/circtools/scripts/create_igv_script_from_position_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,73 +131,74 @@
                 if location not in entries_list[host_gene]['location']:
                     entries_list[host_gene]['location'][location] = 1
 
     return entries_list
 
 
 # main script starts here
+def main():
 
-parser = argparse.ArgumentParser(description='Create an auto-executing IGV script')
+    parser = argparse.ArgumentParser(description='Create an auto-executing IGV script')
 
-group = parser.add_argument_group("Input")
+    group = parser.add_argument_group("Input")
 
-group.add_argument("-i",
-                   "--input-file",
-                   dest="input_file",
-                   help="A CSV/BED file from DCC / CircTest",
-                   required=True
-                   )
-
-group.add_argument("-b",
-                   "--bam-files",
-                   dest="bam_files",
-                   nargs='*',
-                   help="List of one or more BAM files with read mapping data",
-                   required=True
-                   )
-
-group.add_argument("-a",
-                   "--alternative-exon-dirs",
-                   dest="alt_exon_dirs",
-                   nargs='*',
-                   help="List of one or more directories containing the result files "
-                        "of the exon module",
-                   required=True
-                   )
-
-group.add_argument("-f",
-                   "--fuchs-files",
-                   dest="fuchs_files",
-                   nargs='*',
-                   help="List of one or more BED files containing results of "
-                        "FUCHS / reconstruct module",
-                   required=True
-                   )
-
-group.add_argument("-g",
-                   "--genome",
-                   dest="genome_build",
-                   help="Which genome build to use as reference [Default: hg38]",
-                   choices=("hg38", "hg19", "mm9", "mm10"),
-                   default="hg38"
-                   )
-
-group.add_argument("-m",
-                   "--max-number",
-                   dest="max_genes",
-                   help="Maximum number of genes to show [Default: 5]",
-                   type=int,
-                   default=5
-                   )
-
-group = parser.add_argument_group("Output")
-
-group.add_argument("-o",
-                   "--output-directory",
-                   dest="output_directory",
-                   help="Directory for snapshots created by IGV [Default: ./]",
-                   default="./"
-                   )
+    group.add_argument("-i",
+                       "--input-file",
+                       dest="input_file",
+                       help="A CSV/BED file from DCC / CircTest",
+                       required=True
+                       )
+
+    group.add_argument("-b",
+                       "--bam-files",
+                       dest="bam_files",
+                       nargs='*',
+                       help="List of one or more BAM files with read mapping data",
+                       required=True
+                       )
+
+    group.add_argument("-a",
+                       "--alternative-exon-dirs",
+                       dest="alt_exon_dirs",
+                       nargs='*',
+                       help="List of one or more directories containing the result files "
+                            "of the exon module",
+                       required=True
+                       )
+
+    group.add_argument("-f",
+                       "--fuchs-files",
+                       dest="fuchs_files",
+                       nargs='*',
+                       help="List of one or more BED files containing results of "
+                            "FUCHS / reconstruct module",
+                       required=True
+                       )
+
+    group.add_argument("-g",
+                       "--genome",
+                       dest="genome_build",
+                       help="Which genome build to use as reference [Default: hg38]",
+                       choices=("hg38", "hg19", "mm9", "mm10"),
+                       default="hg38"
+                       )
+
+    group.add_argument("-m",
+                       "--max-number",
+                       dest="max_genes",
+                       help="Maximum number of genes to show [Default: 5]",
+                       type=int,
+                       default=5
+                       )
+
+    group = parser.add_argument_group("Output")
+
+    group.add_argument("-o",
+                       "--output-directory",
+                       dest="output_directory",
+                       help="Directory for snapshots created by IGV [Default: ./]",
+                       default="./"
+                       )
 
-args = parser.parse_args()
+    args = parser.parse_args()
 
-build_tracks(args)
+    build_tracks(args)
```

### Comparing `circtools-1.2.2/scripts/detect_new_exons_from_fuchs_data.py` & `circtools-1.3.0/circtools/scripts/detect_new_exons_from_fuchs_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -204,155 +204,154 @@
               file=output_file
               )
         counter += 1
 
 # main script starts here
 
 
-parser = argparse.ArgumentParser(description='Output newly identified exons compare to reference annotation')
+def main():
 
-group = parser.add_argument_group("Input")
+    parser = argparse.ArgumentParser(description='Output newly identified exons compare to reference annotation')
 
-group.add_argument("-a",
-                   "--annotation",
-                   dest="base_exon_file",
-                   help="Base annotation in GTF format (ENSEMBL)",
-                   required=True
-                   )
-
-group.add_argument("-g",
-                   "--group-assignment",
-                   dest="assignment",
-                   help="Assignment of BED files to sample groups",
-                   required=True,
-                   nargs='+',
-                   type=int
-                   )
-
-group.add_argument("-f",
-                   "--bed-files",
-                   dest="bed_files",
-                   help="Space-separated list of BED files to scan",
-                   required=True,
-                   nargs='+',
-                   )
-
-group.add_argument("-t",
-                   "--threshold",
-                   dest="threshold",
-                   help="Minimal number of samples that have to agree on a novel exon [default: 2]",
-                   type=int,
-                   default=2
-                   )
-
-group.add_argument("-c",
-                   "--coverage",
-                   dest="min_coverage",
-                   help="Minimal coverage of exons [default: 1.0 == 100]",
-                   type=float,
-                   default=1.0
-                   )
-
-group.add_argument("-w",
-                   "--wobble",
-                   dest="wobble",
-                   help="Specify the amount of wobble bases to identify novel exons",
-                   type=int,
-                   default=10
-                   )
-
-group.add_argument("-m",
-                   "--max-length",
-                   dest="max_length",
-                   help="Maximum length (in BP) of novel exons [Default: 2000]",
-                   type=int,
-                   default=2000
-                   )
-
-group.add_argument("-B",
-                   "--bed-type",
-                   dest="bed_type",
-                   help="Which BED file type: bed6 or bed12 [Default: bed6]",
-                   choices=("bed6", "bed12"),
-                   default="bed12"
-                   )
-
-args = parser.parse_args()
-
-check_input_files(args.bed_files)
-
-if len(args.bed_files) != len(args.assignment):
-    print("Differing counts for BED files and group assignment, exiting.")
-    exit(-1)
-
-if args.threshold > len(args.bed_files):
-    print("Threshold > number of provided sources files.")
-    exit(-1)
-
-global_dict = {}
-
-assignment_dict = {}
-
-final_dict = {}
-
-gtf_input = parse_gtf_file(args.base_exon_file)
-
-num_files = len(args.bed_files)
-
-sample_num = len(set(args.assignment))
-
-file_dict = {}
-
-for file in range(0, num_files):
-
-    if args.assignment[file] not in global_dict:
-        global_dict[args.assignment[file]] = {}
-
-    file_dict[args.bed_files[file]] = args.assignment[file]
-
-    if args.assignment[file] not in assignment_dict:
-        assignment_dict[args.assignment[file]] = 1
-    else:
-        assignment_dict[args.assignment[file]] += 1
-
-    if args.bed_type == "bed6":
-
-        global_dict[args.assignment[file]] = parse_bed_6_file(args.bed_files[file],
-                                                              gtf_input,
-                                                              global_dict[args.assignment[file]],
-                                                              args.wobble
-                                                              )
-    else:
-        global_dict[args.assignment[file]] = parse_bed_12_file(args.bed_files[file],
-                                                               gtf_input,
-                                                               global_dict[args.assignment[file]],
-                                                               args.min_coverage,
-                                                               args.wobble
-                                                               )
-# remove non-stringent exons
-for sample in global_dict:
-    final_dict[sample] = {}
-    for key in global_dict[sample]:
-        if global_dict[sample][key] >= args.threshold:
-            final_dict[sample][key] = global_dict[sample][key]
-
-
-reference_annotation = pybedtools.BedTool(args.base_exon_file)
-
-for sample in final_dict:
-
-    file = ""
-    for key in final_dict[sample]:
-        entry = key.split('\t')
-
-        sep = "\t"
+    group = parser.add_argument_group("Input")
 
-        if int(entry[2]) - int(entry[1]) <= args.max_length:
-            file += (sep.join([entry[0], "circtools", "exon", entry[1], entry[2], ".", ".", ".", "."]) + "\n")
-
-    sample_bed = pybedtools.BedTool(file, from_string=True)
-    return_bed = sample_bed.intersect(reference_annotation, v=True)
-
-    print_gtf(return_bed, open("sample_"+str(sample)+".gtf", "w"))
+    group.add_argument("-a",
+                       "--annotation",
+                       dest="base_exon_file",
+                       help="Base annotation in GTF format (ENSEMBL)",
+                       required=True
+                       )
+
+    group.add_argument("-g",
+                       "--group-assignment",
+                       dest="assignment",
+                       help="Assignment of BED files to sample groups",
+                       required=True,
+                       nargs='+',
+                       type=int
+                       )
+
+    group.add_argument("-f",
+                       "--bed-files",
+                       dest="bed_files",
+                       help="Space-separated list of BED files to scan",
+                       required=True,
+                       nargs='+',
+                       )
+
+    group.add_argument("-t",
+                       "--threshold",
+                       dest="threshold",
+                       help="Minimal number of samples that have to agree on a novel exon [default: 2]",
+                       type=int,
+                       default=2
+                       )
+
+    group.add_argument("-c",
+                       "--coverage",
+                       dest="min_coverage",
+                       help="Minimal coverage of exons [default: 1.0 == 100]",
+                       type=float,
+                       default=1.0
+                       )
+
+    group.add_argument("-w",
+                       "--wobble",
+                       dest="wobble",
+                       help="Specify the amount of wobble bases to identify novel exons",
+                       type=int,
+                       default=10
+                       )
+
+    group.add_argument("-m",
+                       "--max-length",
+                       dest="max_length",
+                       help="Maximum length (in BP) of novel exons [Default: 2000]",
+                       type=int,
+                       default=2000
+                       )
+
+    group.add_argument("-B",
+                       "--bed-type",
+                       dest="bed_type",
+                       help="Which BED file type: bed6 or bed12 [Default: bed6]",
+                       choices=("bed6", "bed12"),
+                       default="bed12"
+                       )
+
+    args = parser.parse_args()
+
+    check_input_files(args.bed_files)
+
+    if len(args.bed_files) != len(args.assignment):
+        print("Differing counts for BED files and group assignment, exiting.")
+        exit(-1)
+
+    if args.threshold > len(args.bed_files):
+        print("Threshold > number of provided sources files.")
+        exit(-1)
+
+    global_dict = {}
+
+    assignment_dict = {}
+
+    final_dict = {}
+
+    gtf_input = parse_gtf_file(args.base_exon_file)
+
+    num_files = len(args.bed_files)
+
+    sample_num = len(set(args.assignment))
+
+    file_dict = {}
+
+    for file in range(0, num_files):
+
+        if args.assignment[file] not in global_dict:
+            global_dict[args.assignment[file]] = {}
+
+        file_dict[args.bed_files[file]] = args.assignment[file]
+
+        if args.assignment[file] not in assignment_dict:
+            assignment_dict[args.assignment[file]] = 1
+        else:
+            assignment_dict[args.assignment[file]] += 1
+
+        if args.bed_type == "bed6":
+
+            global_dict[args.assignment[file]] = parse_bed_6_file(args.bed_files[file],
+                                                                  gtf_input,
+                                                                  global_dict[args.assignment[file]],
+                                                                  args.wobble
+                                                                  )
+        else:
+            global_dict[args.assignment[file]] = parse_bed_12_file(args.bed_files[file],
+                                                                   gtf_input,
+                                                                   global_dict[args.assignment[file]],
+                                                                   args.min_coverage,
+                                                                   args.wobble
+                                                                   )
+    # remove non-stringent exons
+    for sample in global_dict:
+        final_dict[sample] = {}
+        for key in global_dict[sample]:
+            if global_dict[sample][key] >= args.threshold:
+                final_dict[sample][key] = global_dict[sample][key]
+
+
+    reference_annotation = pybedtools.BedTool(args.base_exon_file)
+
+    for sample in final_dict:
+
+        file = ""
+        for key in final_dict[sample]:
+            entry = key.split('\t')
+
+            sep = "\t"
 
+            if int(entry[2]) - int(entry[1]) <= args.max_length:
+                file += (sep.join([entry[0], "circtools", "exon", entry[1], entry[2], ".", ".", ".", "."]) + "\n")
 
+        sample_bed = pybedtools.BedTool(file, from_string=True)
+        return_bed = sample_bed.intersect(reference_annotation, v=True)
 
+        print_gtf(return_bed, open("sample_"+str(sample)+".gtf", "w"))
```

### Comparing `circtools-1.2.2/scripts/install_add_to_bashrc.sh` & `circtools-1.3.0/circtools/scripts/install_add_to_bashrc.sh`

 * *Files identical despite different names*

### Comparing `circtools-1.2.2/scripts/install_create_r_environ.sh` & `circtools-1.3.0/circtools/scripts/install_create_r_environ.sh`

 * *Files identical despite different names*

### Comparing `circtools-1.2.2/scripts/install_external.sh` & `circtools-1.3.0/circtools/scripts/install_external.sh`

 * *Files 20% similar despite different names*

```diff
@@ -12,51 +12,31 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 function install_bedtools {
-    cd /tmp/
 
     if [[ "$OSTYPE" == "linux-gnu" ]]; then
-        wget https://github.com/arq5x/bedtools2/releases/download/v2.29.2/bedtools-2.29.2.tar.gz
+        wget https://github.com/arq5x/bedtools2/releases/download/v2.30.0/bedtools.static.binary -O /usr/bin/bedtools
     elif [[ "$OSTYPE" == "darwin"* ]]; then
-        curl -O https://github.com/arq5x/bedtools2/releases/download/v2.29.2/bedtools-2.29.2.tar.gz
+        curl -O https://github.com/arq5x/bedtools2/releases/download/v2.30.0/bedtools.static.binary -o /usr/bin/bedtools
     else
-        echo "Sorry, this OS type not supported. Please contact circtools@dieterichlab.org for help."
+        echo "Sorry, this OS type not supported. Please contact tjakobi@arizona.edu for help."
     fi
-
-    tar -zxvf bedtools-2.27.1.tar.gz
-    cd bedtools2
-    make
-    mkdir -p  $HOME/.local/bin/
-    cp -av bin/* $HOME/.local/bin/
-    # mkdir -p  $HOME/.local/share/bedtools/
-    # cp genomes -av $HOME/.local/share/bedtools/
-    rm /tmp/bedtools2 -rf
 }
 
-
-# install dependencies for R first
-Rscript scripts/install_R_dependencies.R
-
 BEDTOOLS=`which bedtools`
 
 if [ $BEDTOOLS ]; then
 
     # get current version of bedtools
     VERSION=`bedtools --version | cut -f 2 -d '.'`
 
     # we want to have >= 27 in order to work correctly
     if [ "$VERSION" -lt "27"  ]; then
         install_bedtools
     fi
 else
      install_bedtools
 fi
-
-# install DCC
-pip install -U git+https://github.com/dieterich-lab/DCC.git
-
-# install FUCHS
-pip install -U git+https://github.com/dieterich-lab/FUCHS.git
```

