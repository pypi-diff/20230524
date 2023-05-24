# Comparing `tmp/xplorts-0.4.tar.gz` & `tmp/xplorts-0.5.tar.gz`

## Comparing `xplorts-0.4.tar` & `xplorts-0.5.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 xplorts-0.4/.gitignore
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 xplorts-0.4/LICENSE
--rw-r--r--   0        0        0     9397 2020-02-02 00:00:00.000000 xplorts-0.4/README.md
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 xplorts-0.4/_NOTES.ipynb
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 xplorts-0.4/pyproject.toml
--rw-r--r--   0        0        0    52377 2020-02-02 00:00:00.000000 xplorts-0.4/data/oph annual bespoke.csv
--rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 xplorts-0.4/data/oph annual by division.csv
--rw-r--r--   0        0        0    20878 2020-02-02 00:00:00.000000 xplorts-0.4/data/oph annual by section.csv
--rw-r--r--   0        0        0    93088 2020-02-02 00:00:00.000000 xplorts-0.4/data/oph quarterly by section.csv
--rw-r--r--   0        0        0  2542592 2020-02-02 00:00:00.000000 xplorts-0.4/data/outputperhourworked.xls
--rw-r--r--   0        0        0  1285776 2020-02-02 00:00:00.000000 xplorts-0.4/docs/html/xplor_lprod oph annual by section.html
--rw-r--r--   0        0        0  1775672 2020-02-02 00:00:00.000000 xplorts-0.4/docs/html/xplor_lprod oph quarterly by section.html
--rw-r--r--   0        0        0    10443 2020-02-02 00:00:00.000000 xplorts-0.4/docs/png/slideselect_date.png
--rw-r--r--   0        0        0    10834 2020-02-02 00:00:00.000000 xplorts-0.4/docs/png/slideselect_industry.png
--rw-r--r--   0        0        0    46598 2020-02-02 00:00:00.000000 xplorts-0.4/docs/png/xplor_lprod_lines_thumbnail_large.png
--rw-r--r--   0        0        0    28431 2020-02-02 00:00:00.000000 xplorts-0.4/docs/png/xplor_lprod_snapcomp_thumbnail_large.png
--rw-r--r--   0        0        0    20261 2020-02-02 00:00:00.000000 xplorts-0.4/docs/png/xplor_lprod_thumbnail.png
--rw-r--r--   0        0        0    37746 2020-02-02 00:00:00.000000 xplorts-0.4/docs/png/xplor_lprod_tscomp_thumbnail_large.png
--rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/__init__.py
--rw-r--r--   0        0        0    32735 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/base.ipynb
--rw-r--r--   0        0        0    16036 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/base.py
--rw-r--r--   0        0        0    12058 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/dutils.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/ghostbokeh.py
--rw-r--r--   0        0        0     6615 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/slideselect.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/dblprod/__init__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/dblprod/__main__.py
--rw-r--r--   0        0        0    19722 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/dblprod/dblprod.py
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/dblprod/prodgrowsnap.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/dblprod/prodgrowts.py
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/dblprod/prodlines.py
--rw-r--r--   0        0        0     8401 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/dblprod/xpdblprod.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/lines/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/lines/__main__.py
--rw-r--r--   0        0        0    13206 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/lines/lines.py
--rw-r--r--   0        0        0     6863 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/lines/xplines.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/scatter/__init__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/scatter/__main__.py
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/scatter/scatter.py
--rw-r--r--   0        0        0     9992 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/scatter/xpscatter.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/snapcomp/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/snapcomp/__main__.py
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/snapcomp/snapcomp.py
--rw-r--r--   0        0        0     7543 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/snapcomp/xpsnapcomp.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/stacks/__init__.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/stacks/__main__.py
--rw-r--r--   0        0        0     9599 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/stacks/bokeh_stacks.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/stacks/stacks.py
--rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/stacks/stacks_util.py
--rw-r--r--   0        0        0     8697 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/stacks/xpstacks.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/tscomp/__init__.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/tscomp/__main__.py
--rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/tscomp/tscomp.py
--rw-r--r--   0        0        0     7899 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/tscomp/xptscomp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/utils/__init__.py
--rw-r--r--   0        0        0     8004 2020-02-02 00:00:00.000000 xplorts-0.4/src/xplorts/utils/ukons_lprod_to_csv.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 xplorts-0.4/tests/conftest.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 xplorts-0.4/tests/test_dblprod.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 xplorts-0.4/tests/test_lines.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 xplorts-0.4/tests/test_scatter.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 xplorts-0.4/tests/test_snapcomp.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 xplorts-0.4/tests/test_stacks.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 xplorts-0.4/tests/test_tscomp.py
--rw-r--r--   0        0        0    15847 2020-02-02 00:00:00.000000 xplorts-0.4/PKG-INFO
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 xplorts-0.5/.gitignore
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 xplorts-0.5/LICENSE
+-rw-r--r--   0        0        0     9304 2020-02-02 00:00:00.000000 xplorts-0.5/README.md
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 xplorts-0.5/_NOTES.ipynb
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 xplorts-0.5/pyproject.toml
+-rw-r--r--   0        0        0    52377 2020-02-02 00:00:00.000000 xplorts-0.5/data/oph annual bespoke.csv
+-rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 xplorts-0.5/data/oph annual by division.csv
+-rw-r--r--   0        0        0    20878 2020-02-02 00:00:00.000000 xplorts-0.5/data/oph annual by section.csv
+-rw-r--r--   0        0        0    93088 2020-02-02 00:00:00.000000 xplorts-0.5/data/oph quarterly by section.csv
+-rw-r--r--   0        0        0  2542592 2020-02-02 00:00:00.000000 xplorts-0.5/data/outputperhourworked.xls
+-rw-r--r--   0        0        0  1285776 2020-02-02 00:00:00.000000 xplorts-0.5/docs/html/xplor_lprod oph annual by section.html
+-rw-r--r--   0        0        0  1775672 2020-02-02 00:00:00.000000 xplorts-0.5/docs/html/xplor_lprod oph quarterly by section.html
+-rw-r--r--   0        0        0    10443 2020-02-02 00:00:00.000000 xplorts-0.5/docs/png/slideselect_date.png
+-rw-r--r--   0        0        0    10834 2020-02-02 00:00:00.000000 xplorts-0.5/docs/png/slideselect_industry.png
+-rw-r--r--   0        0        0    46598 2020-02-02 00:00:00.000000 xplorts-0.5/docs/png/xplor_lprod_lines_thumbnail_large.png
+-rw-r--r--   0        0        0    28431 2020-02-02 00:00:00.000000 xplorts-0.5/docs/png/xplor_lprod_snapcomp_thumbnail_large.png
+-rw-r--r--   0        0        0    20261 2020-02-02 00:00:00.000000 xplorts-0.5/docs/png/xplor_lprod_thumbnail.png
+-rw-r--r--   0        0        0    37746 2020-02-02 00:00:00.000000 xplorts-0.5/docs/png/xplor_lprod_tscomp_thumbnail_large.png
+-rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/__init__.py
+-rw-r--r--   0        0        0    32735 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/base.ipynb
+-rw-r--r--   0        0        0    16036 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/base.py
+-rw-r--r--   0        0        0    12058 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/dutils.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/ghostbokeh.py
+-rw-r--r--   0        0        0     6615 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/slideselect.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/dblprod/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/dblprod/__main__.py
+-rw-r--r--   0        0        0    19722 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/dblprod/dblprod.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/dblprod/prodgrowsnap.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/dblprod/prodgrowts.py
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/dblprod/prodlines.py
+-rw-r--r--   0        0        0     8401 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/dblprod/xpdblprod.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/lines/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/lines/__main__.py
+-rw-r--r--   0        0        0    13206 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/lines/lines.py
+-rw-r--r--   0        0        0     6863 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/lines/xplines.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/scatter/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/scatter/__main__.py
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/scatter/scatter.py
+-rw-r--r--   0        0        0     9992 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/scatter/xpscatter.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/snapcomp/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/snapcomp/__main__.py
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/snapcomp/snapcomp.py
+-rw-r--r--   0        0        0     7543 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/snapcomp/xpsnapcomp.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/stacks/__init__.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/stacks/__main__.py
+-rw-r--r--   0        0        0     9599 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/stacks/bokeh_stacks.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/stacks/stacks.py
+-rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/stacks/stacks_util.py
+-rw-r--r--   0        0        0     8697 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/stacks/xpstacks.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/tscomp/__init__.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/tscomp/__main__.py
+-rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/tscomp/tscomp.py
+-rw-r--r--   0        0        0     7899 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/tscomp/xptscomp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/utils/__init__.py
+-rw-r--r--   0        0        0     8004 2020-02-02 00:00:00.000000 xplorts-0.5/src/xplorts/utils/ukons_lprod_to_csv.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 xplorts-0.5/tests/conftest.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 xplorts-0.5/tests/test_dblprod.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 xplorts-0.5/tests/test_lines.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 xplorts-0.5/tests/test_scatter.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 xplorts-0.5/tests/test_snapcomp.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 xplorts-0.5/tests/test_stacks.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 xplorts-0.5/tests/test_tscomp.py
+-rw-r--r--   0        0        0    15754 2020-02-02 00:00:00.000000 xplorts-0.5/PKG-INFO
```

### Comparing `xplorts-0.4/.gitignore` & `xplorts-0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/LICENSE` & `xplorts-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/README.md` & `xplorts-0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 <!-- This document uses
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/) -->
 
-# ![Thumbnail screenshot of xplorts productivity explorer](docs/png/xplor_lprod_thumbnail.png) Explore time series datasets 
+# Explore time series datasets 
 
 **`xplorts`** ("explore-ts") is a collection of Python tools to make standalone HTML documents containing interactive charts.  It is particularly aimed at showing time series data (hence the "ts") with annual, quarterly or monthly periodicity, such as that published by national statistical institutes by way of national accounts, productivity, or labour markets series. 
 
 Once created, the HTML documents can be used with any web browser.  They do not need an
 active internet connection.
 
 <details>
@@ -93,22 +93,22 @@
 ```
 
 ### Modules
 
 Module | Description
 --- | ---
 base | Miscellaneous helper functions and classes.
+dblprod | Modify a Bokeh Figure by adding charts to show labour productivity levels or growth components.
 ghostbokeh | Define an abstract base class to a build pseudo-subclass of a Bokeh class.
 lines | Modify a Bokeh Figure by adding line charts to show several time series with a split factor.
 scatter | Modify a Bokeh Figure by adding scatter charts to show one or more categorical series with a split factor.
 slideselect | Defines a class combining select and slider widgets, with support for javascript linking to other objects.
 snapcomp | Modify a Bokeh Figure by adding a snapshot growth components chart, with a categorical vertical axis showing levels of a split factor, horizontal stacked bars showing growth components, and markers showing overall growth for each stack of bars.
 stacks | Modify a Bokeh Figure by adding a horizontal or vertical stacked bar chart showing several data series with a split factor.
 tscomp | Modify a Bokeh Figure by adding a time series growth components chart, with a categorical vertical axis showing levels of a split factor, horizontal  stacked bars showing growth components, and a line showing overall growth.  
-dblprod | Modify a Bokeh Figure by adding charts to show labour productivity levels or growth components.
 </details>
 
 <details>
    <summary>
 
 ## Using `xplorts` on the command line
    </summary>
```

### Comparing `xplorts-0.4/_NOTES.ipynb` & `xplorts-0.5/_NOTES.ipynb`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9513888888888888%*

 * *Differences: {"'cells'": "{0: {'id': 'a531217d'}, 1: {'id': '38ef467d'}, 2: {'id': 'bb906b02'}, 3: {'id': "*

 * *            "'27b12926'}, 6: {'id': 'fecb4eed', 'source': ['4. Make test environment and install "*

 * *            "package']}, 7: {'id': '40cebda5'}, 9: {'id': '3cc0d311', 'source': {delete: [5, 4, 3, "*

 * *            "2]}}, insert: [(4, OrderedDict([('cell_type', 'markdown'), ('id', '5bd4bc96'), "*

 * *            "('metadata', OrderedDict()), ('source', ['3. Update pip (Mac only, maybe no longer "*

 * *            "required)']) […]*

```diff
@@ -1,85 +1,114 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "aefb7274",
+            "id": "a531217d",
             "metadata": {},
             "source": [
                 "# Notes on preparing xplorts package\n",
                 "1. Prepare the package"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
-            "id": "30028d3e",
+            "id": "38ef467d",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# (Terminal)\n",
                 "#> cd xplor_time_series\n",
                 "#> conda activate python36_plus_hv2\n",
                 "#> rm dist/*  # clear out old distributions"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "4fe81d54",
+            "id": "bb906b02",
             "metadata": {},
             "source": [
                 "2. Build the package and upload to PyPI or testpypi"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
-            "id": "02452ac6",
+            "id": "27b12926",
             "metadata": {},
             "outputs": [],
             "source": [
                 "#> python3 -m build\n",
                 "#> python3 -m twine upload --repository testpipy dist/*\n",
                 "\n",
                 "## Username:  __token__\n",
                 "## Password:  <paste in token>"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "d36b1af5",
+            "id": "5bd4bc96",
             "metadata": {},
             "source": [
-                "3. Make test environment and install package"
+                "3. Update pip (Mac only, maybe no longer required)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "a667ff1b",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "## If pip is not at least 9.0.3\n",
+                "## If you are running macOS/OS X version 10.12 or older, then you ought to upgrade to the latest pip (9.0.3) \n",
+                "## https://stackoverflow.com/questions/49748063/pip-install-fails-for-every-package-could-not-find-a-version-that-satisfies#49748494\n",
+                "#> curl https://bootstrap.pypa.io/get-pip.py | python\n",
+                "#> pip install --upgrade setuptools"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "fecb4eed",
+            "metadata": {},
+            "source": [
+                "4. Make test environment and install package"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
-            "id": "ec9e8760",
+            "id": "40cebda5",
             "metadata": {},
             "outputs": [],
             "source": [
                 "#> conda env create -n xplorts \"python=3.6\"\n",
                 "#> conda activate xplorts"
             ]
         },
         {
             "cell_type": "code",
+            "execution_count": 8,
+            "id": "b4998559",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "#xplorts> pip install \"bokeh>=2.3.2\" \"numpy>=1.19.2\" \"pandas>=1.1.5\" \"pyyaml>=5.4.1\"\n",
+                "#xplorts> pip install --index-url https://test.pypi.org/simple/ --no-deps xplorts"
+            ]
+        },
+        {
+            "cell_type": "code",
             "execution_count": null,
-            "id": "f2548b2e",
+            "id": "3cc0d311",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# does note work...\n",
-                "#xplorts> pip install \"bokeh>=2.3.2\" \"numpy>=1.19.2\" \"pandas>=1.1.5\" \"yaml>=0.2.5\"\n",
-                "\n",
-                "# jury is out...\n",
-                "#xplorts> pip install \"bokeh>=2.3.2\" \"numpy>=1.19.2\" \"pandas>=1.1.5\" \"pyyaml>=5.4.1\"\n",
-                "#xplorts> pip install yaml  ## Use PyYAML instead? (seems to come with other packages above)"
+                "#xplorts> pip install \"bokeh>=2.3.2\" \"numpy>=1.19.2\" \"pandas>=1.1.5\" \"yaml>=0.2.5\"\n"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
```

### Comparing `xplorts-0.4/pyproject.toml` & `xplorts-0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "xplorts"
-version = "0.4"
+version = "0.5"
 authors = [
   { name="Todd M Bailey", email="tmb@baileywick.plus.com" },
 ]
 description = "Make standalone interactive HTML charts to explore time series datasets"
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `xplorts-0.4/data/oph annual bespoke.csv` & `xplorts-0.5/data/oph annual bespoke.csv`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/data/oph annual by division.csv` & `xplorts-0.5/data/oph annual by division.csv`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/data/oph annual by section.csv` & `xplorts-0.5/data/oph annual by section.csv`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/data/oph quarterly by section.csv` & `xplorts-0.5/data/oph quarterly by section.csv`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/data/outputperhourworked.xls` & `xplorts-0.5/data/outputperhourworked.xls`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/docs/html/xplor_lprod oph annual by section.html` & `xplorts-0.5/docs/html/xplor_lprod oph annual by section.html`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/docs/html/xplor_lprod oph quarterly by section.html` & `xplorts-0.5/docs/html/xplor_lprod oph quarterly by section.html`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/docs/png/slideselect_date.png` & `xplorts-0.5/docs/png/slideselect_date.png`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/docs/png/slideselect_industry.png` & `xplorts-0.5/docs/png/slideselect_industry.png`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/docs/png/xplor_lprod_lines_thumbnail_large.png` & `xplorts-0.5/docs/png/xplor_lprod_lines_thumbnail_large.png`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/docs/png/xplor_lprod_snapcomp_thumbnail_large.png` & `xplorts-0.5/docs/png/xplor_lprod_snapcomp_thumbnail_large.png`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/docs/png/xplor_lprod_thumbnail.png` & `xplorts-0.5/docs/png/xplor_lprod_thumbnail.png`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/docs/png/xplor_lprod_tscomp_thumbnail_large.png` & `xplorts-0.5/docs/png/xplor_lprod_tscomp_thumbnail_large.png`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/__init__.py` & `xplorts-0.5/src/xplorts/__init__.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/base.ipynb` & `xplorts-0.5/src/xplorts/base.ipynb`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/base.py` & `xplorts-0.5/src/xplorts/base.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/dutils.py` & `xplorts-0.5/src/xplorts/dutils.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/ghostbokeh.py` & `xplorts-0.5/src/xplorts/ghostbokeh.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/slideselect.py` & `xplorts-0.5/src/xplorts/slideselect.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/dblprod/__init__.py` & `xplorts-0.5/src/xplorts/dblprod/__init__.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/dblprod/dblprod.py` & `xplorts-0.5/src/xplorts/dblprod/dblprod.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/dblprod/prodgrowsnap.py` & `xplorts-0.5/src/xplorts/dblprod/prodgrowsnap.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/dblprod/prodgrowts.py` & `xplorts-0.5/src/xplorts/dblprod/prodgrowts.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/dblprod/prodlines.py` & `xplorts-0.5/src/xplorts/dblprod/prodlines.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/dblprod/xpdblprod.py` & `xplorts-0.5/src/xplorts/dblprod/xpdblprod.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/lines/lines.py` & `xplorts-0.5/src/xplorts/lines/lines.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/lines/xplines.py` & `xplorts-0.5/src/xplorts/lines/xplines.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/scatter/scatter.py` & `xplorts-0.5/src/xplorts/scatter/scatter.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/scatter/xpscatter.py` & `xplorts-0.5/src/xplorts/scatter/xpscatter.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/snapcomp/__init__.py` & `xplorts-0.5/src/xplorts/snapcomp/__init__.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/snapcomp/snapcomp.py` & `xplorts-0.5/src/xplorts/snapcomp/snapcomp.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/snapcomp/xpsnapcomp.py` & `xplorts-0.5/src/xplorts/snapcomp/xpsnapcomp.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/stacks/bokeh_stacks.py` & `xplorts-0.5/src/xplorts/stacks/bokeh_stacks.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/stacks/stacks.py` & `xplorts-0.5/src/xplorts/stacks/stacks.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/stacks/stacks_util.py` & `xplorts-0.5/src/xplorts/stacks/stacks_util.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/stacks/xpstacks.py` & `xplorts-0.5/src/xplorts/stacks/xpstacks.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/tscomp/__init__.py` & `xplorts-0.5/src/xplorts/tscomp/__init__.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/tscomp/tscomp.py` & `xplorts-0.5/src/xplorts/tscomp/tscomp.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/tscomp/xptscomp.py` & `xplorts-0.5/src/xplorts/tscomp/xptscomp.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/src/xplorts/utils/ukons_lprod_to_csv.py` & `xplorts-0.5/src/xplorts/utils/ukons_lprod_to_csv.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/tests/conftest.py` & `xplorts-0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/tests/test_dblprod.py` & `xplorts-0.5/tests/test_dblprod.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/tests/test_lines.py` & `xplorts-0.5/tests/test_lines.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/tests/test_scatter.py` & `xplorts-0.5/tests/test_scatter.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/tests/test_snapcomp.py` & `xplorts-0.5/tests/test_snapcomp.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/tests/test_stacks.py` & `xplorts-0.5/tests/test_stacks.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/tests/test_tscomp.py` & `xplorts-0.5/tests/test_tscomp.py`

 * *Files identical despite different names*

### Comparing `xplorts-0.4/PKG-INFO` & `xplorts-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xplorts
-Version: 0.4
+Version: 0.5
 Summary: Make standalone interactive HTML charts to explore time series datasets
 Project-URL: Bug Tracker, https://github.com/xplorts/xplorts/issues
 Project-URL: Homepage, https://github.com/xplorts/xplorts
 Author-email: Todd M Bailey <tmb@baileywick.plus.com>
 License: Copyright 2023 Todd Bailey
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
@@ -102,15 +102,15 @@
 Requires-Dist: pyyaml>=5.4.1
 Description-Content-Type: text/markdown
 
 
 <!-- This document uses
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/) -->
 
-# ![Thumbnail screenshot of xplorts productivity explorer](docs/png/xplor_lprod_thumbnail.png) Explore time series datasets 
+# Explore time series datasets 
 
 **`xplorts`** ("explore-ts") is a collection of Python tools to make standalone HTML documents containing interactive charts.  It is particularly aimed at showing time series data (hence the "ts") with annual, quarterly or monthly periodicity, such as that published by national statistical institutes by way of national accounts, productivity, or labour markets series. 
 
 Once created, the HTML documents can be used with any web browser.  They do not need an
 active internet connection.
 
 <details>
@@ -197,22 +197,22 @@
 ```
 
 ### Modules
 
 Module | Description
 --- | ---
 base | Miscellaneous helper functions and classes.
+dblprod | Modify a Bokeh Figure by adding charts to show labour productivity levels or growth components.
 ghostbokeh | Define an abstract base class to a build pseudo-subclass of a Bokeh class.
 lines | Modify a Bokeh Figure by adding line charts to show several time series with a split factor.
 scatter | Modify a Bokeh Figure by adding scatter charts to show one or more categorical series with a split factor.
 slideselect | Defines a class combining select and slider widgets, with support for javascript linking to other objects.
 snapcomp | Modify a Bokeh Figure by adding a snapshot growth components chart, with a categorical vertical axis showing levels of a split factor, horizontal stacked bars showing growth components, and markers showing overall growth for each stack of bars.
 stacks | Modify a Bokeh Figure by adding a horizontal or vertical stacked bar chart showing several data series with a split factor.
 tscomp | Modify a Bokeh Figure by adding a time series growth components chart, with a categorical vertical axis showing levels of a split factor, horizontal  stacked bars showing growth components, and a line showing overall growth.  
-dblprod | Modify a Bokeh Figure by adding charts to show labour productivity levels or growth components.
 </details>
 
 <details>
    <summary>
 
 ## Using `xplorts` on the command line
    </summary>
```

