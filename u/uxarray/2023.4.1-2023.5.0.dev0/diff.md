# Comparing `tmp/uxarray-2023.4.1.tar.gz` & `tmp/uxarray-2023.5.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uxarray-2023.4.1.tar", last modified: Mon Apr 24 21:49:06 2023, max compression
+gzip compressed data, was "uxarray-2023.5.0.dev0.tar", last modified: Wed May 24 20:36:24 2023, max compression
```

## Comparing `uxarray-2023.4.1.tar` & `uxarray-2023.5.0.dev0.tar`

### file list

```diff
@@ -1,142 +1,155 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.904318 uxarray-2023.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.880318 uxarray-2023.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.880318 uxarray-2023.4.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-24 21:48:56.000000 uxarray-2023.4.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-24 21:48:56.000000 uxarray-2023.4.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-24 21:48:56.000000 uxarray-2023.4.1/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-24 21:48:56.000000 uxarray-2023.4.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.880318 uxarray-2023.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-24 21:48:56.000000 uxarray-2023.4.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-24 21:48:56.000000 uxarray-2023.4.1/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-24 21:48:56.000000 uxarray-2023.4.1/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-24 21:48:56.000000 uxarray-2023.4.1/.github/workflows/upstream-dev-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-24 21:48:56.000000 uxarray-2023.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-24 21:48:56.000000 uxarray-2023.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-24 21:48:56.000000 uxarray-2023.4.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-24 21:48:56.000000 uxarray-2023.4.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-24 21:48:56.000000 uxarray-2023.4.1/INSTALLATION.md
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-04-24 21:48:56.000000 uxarray-2023.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-04-24 21:49:06.904318 uxarray-2023.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-04-24 21:48:56.000000 uxarray-2023.4.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-04-24 21:48:56.000000 uxarray-2023.4.1/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.880318 uxarray-2023.4.1/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-24 21:48:56.000000 uxarray-2023.4.1/ci/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 21:48:56.000000 uxarray-2023.4.1/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 21:48:56.000000 uxarray-2023.4.1/ci/upstream-dev-environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.880318 uxarray-2023.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.880318 uxarray-2023.4.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.880318 uxarray-2023.4.1/docs/_static/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.880318 uxarray-2023.4.1/docs/_static/images/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/images/icons/code.svg
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/images/icons/download.svg
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/images/icons/science.svg
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/images/icons/tips.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.884318 uxarray-2023.4.1/docs/_static/images/logos/
--rw-r--r--   0 runner    (1001) docker     (123)   348960 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/images/logos/DOE_vertical.png
--rw-r--r--   0 runner    (1001) docker     (123)    44028 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/images/logos/EarthCube_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   210002 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/images/logos/NSF_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    28358 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/images/logos/PANGEO_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   241224 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/images/logos/uxarray_temp_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/images/nsf.png
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/style.css
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/theme_overrides.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.884318 uxarray-2023.4.1/docs/_static/thumbnails/
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_static/thumbnails/default.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.884318 uxarray-2023.4.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/_templates/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/citation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    30865 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.884318 uxarray-2023.4.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/examples/000-template.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    65555 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/examples/001-read-grid-data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/examples/002-access-grid-info.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13122 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/examples/003-area-calc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/gallery.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.884318 uxarray-2023.4.1/docs/internal_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/internal_api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.884318 uxarray-2023.4.1/docs/user_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/user_api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-04-24 21:48:56.000000 uxarray-2023.4.1/docs/user_api/uxarray_api.md
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-24 21:48:56.000000 uxarray-2023.4.1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 21:48:56.000000 uxarray-2023.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 21:49:06.904318 uxarray-2023.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-24 21:48:56.000000 uxarray-2023.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.884318 uxarray-2023.4.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-24 21:48:56.000000 uxarray-2023.4.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-24 21:48:56.000000 uxarray-2023.4.1/test/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.876318 uxarray-2023.4.1/test/meshfiles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.876318 uxarray-2023.4.1/test/meshfiles/exodus/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.884318 uxarray-2023.4.1/test/meshfiles/exodus/mixed/
--rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-04-24 21:48:56.000000 uxarray-2023.4.1/test/meshfiles/exodus/mixed/mixed.exo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.884318 uxarray-2023.4.1/test/meshfiles/exodus/outCSne8/
--rw-r--r--   0 runner    (1001) docker     (123)    42627 2023-04-24 21:48:56.000000 uxarray-2023.4.1/test/meshfiles/exodus/outCSne8/outCSne8.g
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.876318 uxarray-2023.4.1/test/meshfiles/mpas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.884318 uxarray-2023.4.1/test/meshfiles/mpas/QU/
--rw-r--r--   0 runner    (1001) docker     (123)   178192 2023-04-24 21:48:56.000000 uxarray-2023.4.1/test/meshfiles/mpas/QU/mesh.QU.1920km.151026.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.876318 uxarray-2023.4.1/test/meshfiles/scrip/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.884318 uxarray-2023.4.1/test/meshfiles/scrip/outCSne8/
--rw-r--r--   0 runner    (1001) docker     (123)    48890 2023-04-24 21:48:56.000000 uxarray-2023.4.1/test/meshfiles/scrip/outCSne8/outCSne8.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.884318 uxarray-2023.4.1/test/meshfiles/shp/
--rw-r--r--   0 runner    (1001) docker     (123)   162187 2023-04-24 21:48:56.000000 uxarray-2023.4.1/test/meshfiles/shp/grid_fire.shp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.880318 uxarray-2023.4.1/test/meshfiles/ugrid/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.896318 uxarray-2023.4.1/test/meshfiles/ugrid/fesom/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-24 21:48:56.000000 uxarray-2023.4.1/test/meshfiles/ugrid/fesom/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    46371 2023-04-24 21:48:56.000000 uxarray-2023.4.1/test/meshfiles/ugrid/fesom/a_ice.fesom.1948.nc
--rw-r--r--   0 runner    (1001) docker     (123)  2510328 2023-04-24 21:48:56.000000 uxarray-2023.4.1/test/meshfiles/ugrid/fesom/fesom.mesh.diag.nc
--rw-r--r--   0 runner    (1001) docker     (123)  1203548 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/fesom/salt.fesom.1948.nc
--rw-r--r--   0 runner    (1001) docker     (123)    46383 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/fesom/sst.fesom.1948.nc
--rw-r--r--   0 runner    (1001) docker     (123)  1203552 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/fesom/temp.fesom.1948.nc
--rw-r--r--   0 runner    (1001) docker     (123)    50983 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/fesom/test_scrip_outfile.nc
--rw-r--r--   0 runner    (1001) docker     (123)  2218394 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/fesom/u.fesom.1948.nc
--rw-r--r--   0 runner    (1001) docker     (123)    33799 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/fesom/uice.fesom.1948.nc
--rw-r--r--   0 runner    (1001) docker     (123)  2218394 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/fesom/v.fesom.1948.nc
--rw-r--r--   0 runner    (1001) docker     (123)    33799 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/fesom/vice.fesom.1948.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.900318 uxarray-2023.4.1/test/meshfiles/ugrid/geoflow-small/
--rw-r--r--   0 runner    (1001) docker     (123)  1130591 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/geoflow-small/grid.nc
--rw-r--r--   0 runner    (1001) docker     (123)   971022 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/geoflow-small/v1.nc
--rw-r--r--   0 runner    (1001) docker     (123)   971022 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/geoflow-small/v2.nc
--rw-r--r--   0 runner    (1001) docker     (123)   971022 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/geoflow-small/v3.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.900318 uxarray-2023.4.1/test/meshfiles/ugrid/outCSne30/
--rw-r--r--   0 runner    (1001) docker     (123)   181767 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/outCSne30/outCSne30.ug
--rw-r--r--   0 runner    (1001) docker     (123)    49344 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/outCSne30/outCSne30_var2.nc
--rw-r--r--   0 runner    (1001) docker     (123)    43280 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/outCSne30/outCSne30_vortex.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.904318 uxarray-2023.4.1/test/meshfiles/ugrid/outRLL1deg/
--rw-r--r--   0 runner    (1001) docker     (123)  2076807 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/outRLL1deg/outRLL1deg.ug
--rw-r--r--   0 runner    (1001) docker     (123)   518496 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/outRLL1deg/outRLL1deg_vortex.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.904318 uxarray-2023.4.1/test/meshfiles/ugrid/ov_RLL10deg_CSne4/
--rw-r--r--   0 runner    (1001) docker     (123)    36983 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4.ug
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4_vortex.nc
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/test_exodus.py
--rw-r--r--   0 runner    (1001) docker     (123)    21768 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/test_mpas.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/test_placeholder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/test_scrip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-24 21:48:57.000000 uxarray-2023.4.1/test/test_ugrid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.904318 uxarray-2023.4.1/uxarray/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-24 21:48:57.000000 uxarray-2023.4.1/uxarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12925 2023-04-24 21:48:57.000000 uxarray-2023.4.1/uxarray/_exodus.py
--rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-04-24 21:48:57.000000 uxarray-2023.4.1/uxarray/_mpas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-04-24 21:48:57.000000 uxarray-2023.4.1/uxarray/_scrip.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-24 21:48:57.000000 uxarray-2023.4.1/uxarray/_shapefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-24 21:48:57.000000 uxarray-2023.4.1/uxarray/_ugrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-24 21:48:57.000000 uxarray-2023.4.1/uxarray/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13193 2023-04-24 21:48:57.000000 uxarray-2023.4.1/uxarray/get_quadratureDG.py
--rw-r--r--   0 runner    (1001) docker     (123)    26267 2023-04-24 21:48:57.000000 uxarray-2023.4.1/uxarray/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    21464 2023-04-24 21:48:57.000000 uxarray-2023.4.1/uxarray/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:06.904318 uxarray-2023.4.1/uxarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-04-24 21:49:06.000000 uxarray-2023.4.1/uxarray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-24 21:49:06.000000 uxarray-2023.4.1/uxarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:49:06.000000 uxarray-2023.4.1/uxarray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:49:06.000000 uxarray-2023.4.1/uxarray.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 21:49:06.000000 uxarray-2023.4.1/uxarray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 21:49:06.000000 uxarray-2023.4.1/uxarray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.736801 uxarray-2023.5.0.dev0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.700799 uxarray-2023.5.0.dev0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.700799 uxarray-2023.5.0.dev0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.github/ISSUE_TEMPLATE/release_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.704799 uxarray-2023.5.0.dev0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.github/workflows/upstream-dev-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/INSTALLATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-24 20:36:24.736801 uxarray-2023.5.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.704799 uxarray-2023.5.0.dev0/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/ci/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/ci/upstream-dev-environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.704799 uxarray-2023.5.0.dev0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.704799 uxarray-2023.5.0.dev0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.704799 uxarray-2023.5.0.dev0/docs/_static/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.704799 uxarray-2023.5.0.dev0/docs/_static/images/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/images/icons/code.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/images/icons/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/images/icons/science.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/images/icons/tips.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.704799 uxarray-2023.5.0.dev0/docs/_static/images/logos/
+-rw-r--r--   0 runner    (1001) docker     (123)   348960 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/images/logos/DOE_vertical.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44028 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/images/logos/EarthCube_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   210002 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/images/logos/NSF_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28358 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/images/logos/PANGEO_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   241224 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/images/logos/uxarray_temp_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/images/nsf.png
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/theme_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.708799 uxarray-2023.5.0.dev0/docs/_static/thumbnails/
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_static/thumbnails/default.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.708799 uxarray-2023.5.0.dev0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/_templates/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/citation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30865 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.708799 uxarray-2023.5.0.dev0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/examples/000-template.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    61123 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/examples/001-read-grid-data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/examples/002-access-grid-info.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13122 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/examples/003-area-calc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/gallery.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.708799 uxarray-2023.5.0.dev0/docs/internal_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/internal_api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.708799 uxarray-2023.5.0.dev0/docs/user_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/user_api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8419 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/docs/user_api/uxarray_api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 20:36:24.736801 uxarray-2023.5.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.708799 uxarray-2023.5.0.dev0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.700799 uxarray-2023.5.0.dev0/test/meshfiles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.700799 uxarray-2023.5.0.dev0/test/meshfiles/exodus/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.708799 uxarray-2023.5.0.dev0/test/meshfiles/exodus/mixed/
+-rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/exodus/mixed/mixed.exo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.708799 uxarray-2023.5.0.dev0/test/meshfiles/exodus/outCSne8/
+-rw-r--r--   0 runner    (1001) docker     (123)    42627 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/exodus/outCSne8/outCSne8.g
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.700799 uxarray-2023.5.0.dev0/test/meshfiles/mpas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.708799 uxarray-2023.5.0.dev0/test/meshfiles/mpas/QU/
+-rw-r--r--   0 runner    (1001) docker     (123)   178192 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/mpas/QU/mesh.QU.1920km.151026.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.700799 uxarray-2023.5.0.dev0/test/meshfiles/scrip/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.708799 uxarray-2023.5.0.dev0/test/meshfiles/scrip/outCSne8/
+-rw-r--r--   0 runner    (1001) docker     (123)    48890 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/scrip/outCSne8/outCSne8.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.708799 uxarray-2023.5.0.dev0/test/meshfiles/shp/
+-rw-r--r--   0 runner    (1001) docker     (123)   162187 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/shp/grid_fire.shp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.700799 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.724800 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    46371 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/a_ice.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  2510328 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/fesom.mesh.diag.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  1203548 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/salt.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    46383 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/sst.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  1203552 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/temp.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    50983 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/test_scrip_outfile.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  2218394 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/u.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    33799 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/uice.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  2218394 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/v.fesom.1948.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    33799 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/vice.fesom.1948.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.728800 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/geoflow-small/
+-rw-r--r--   0 runner    (1001) docker     (123)  1130591 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/geoflow-small/grid.nc
+-rw-r--r--   0 runner    (1001) docker     (123)   971022 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/geoflow-small/v1.nc
+-rw-r--r--   0 runner    (1001) docker     (123)   971022 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/geoflow-small/v2.nc
+-rw-r--r--   0 runner    (1001) docker     (123)   971022 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/geoflow-small/v3.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.728800 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/outCSne30/
+-rw-r--r--   0 runner    (1001) docker     (123)   181767 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/outCSne30/outCSne30.ug
+-rw-r--r--   0 runner    (1001) docker     (123)    49344 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/outCSne30/outCSne30_var2.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    43280 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/outCSne30/outCSne30_vortex.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.732801 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/outRLL1deg/
+-rw-r--r--   0 runner    (1001) docker     (123)  2076807 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/outRLL1deg/outRLL1deg.ug
+-rw-r--r--   0 runner    (1001) docker     (123)   518496 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/outRLL1deg/outRLL1deg_vortex.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.732801 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/ov_RLL10deg_CSne4/
+-rw-r--r--   0 runner    (1001) docker     (123)    36983 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4.ug
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4_vortex.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/test_exodus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33115 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/test_mpas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/test_placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/test_scrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/test/test_ugrid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.732801 uxarray-2023.5.0.dev0/uxarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.732801 uxarray-2023.5.0.dev0/uxarray/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/core/dataarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29920 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/core/grid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.736801 uxarray-2023.5.0.dev0/uxarray/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12994 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/io/_exodus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/io/_mpas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/io/_scrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/io/_shapefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/io/_ugrid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.736801 uxarray-2023.5.0.dev0/uxarray/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13193 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/utils/get_quadratureDG.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21470 2023-05-24 20:36:12.000000 uxarray-2023.5.0.dev0/uxarray/utils/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:36:24.732801 uxarray-2023.5.0.dev0/uxarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-24 20:36:24.000000 uxarray-2023.5.0.dev0/uxarray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-24 20:36:24.000000 uxarray-2023.5.0.dev0/uxarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:36:24.000000 uxarray-2023.5.0.dev0/uxarray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:36:24.000000 uxarray-2023.5.0.dev0/uxarray.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 20:36:24.000000 uxarray-2023.5.0.dev0/uxarray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 20:36:24.000000 uxarray-2023.5.0.dev0/uxarray.egg-info/top_level.txt
```

### Comparing `uxarray-2023.4.1/.github/ISSUE_TEMPLATE/bug_report.md` & `uxarray-2023.5.0.dev0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/.github/ISSUE_TEMPLATE/feature_request.md` & `uxarray-2023.5.0.dev0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 assignees: ''
 
 ---
 
 **Describe the feature you'd like added to this project**
 A clear and concise description of what the problem is.
 
-**Link to original NCL functionality, if applicable**
+**Link to original functionality implementation elsewhere, if applicable**
 
 **Links to other examples, if applicable**
 
 **Describe the solution you'd like**
 A clear and concise description of what you want to happen.
 
 **Additional context**
```

### Comparing `uxarray-2023.4.1/.github/workflows/ci.yml` & `uxarray-2023.5.0.dev0/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       run:
         shell: bash -l {0}
 
     strategy:
       fail-fast: false
       matrix:
         os: [ "ubuntu-latest", "macos-latest", "windows-latest"]
-        python-version: [ "3.7", "3.8", "3.9", "3.10"]
+        python-version: [ "3.9", "3.10", "3.11"]
     steps:
       - name: Cancel previous runs
         uses: styfle/cancel-workflow-action@0.11.0
         with:
           access_token: ${{ github.token }}
       - name: checkout
         uses: actions/checkout@v3
@@ -51,14 +51,14 @@
           python -m pytest test
 
       - name: Run Coverage Tests
         run: |
           python -m pytest test -v --cov=./uxarray --cov-report=xml
 
       - name: Upload code coverage to Codecov
-        uses: codecov/codecov-action@v3.1.3
+        uses: codecov/codecov-action@v3.1.4
         with:
           file: ./coverage.xml
           flags: unittests
           env_vars: OS,PYTHON
           name: codecov-umbrella
           fail_ci_if_error: false
```

### Comparing `uxarray-2023.4.1/.github/workflows/pypi.yaml` & `uxarray-2023.5.0.dev0/.github/workflows/pypi.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -44,13 +44,13 @@
           python setup.py sdist bdist_wheel
           python -m pip wheel . -w dist --no-deps
       - name: Test the artifacts
         run: |
           python -m twine check dist/*
 
       - name: Publish package to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.8.5
+        uses: pypa/gh-action-pypi-publish@v1.8.6
         with:
           user: __token__
           password: ${{ secrets.PYPI_UXARRAY }}
           skip_existing: true
           verbose: true
```

### Comparing `uxarray-2023.4.1/.github/workflows/upstream-dev-ci.yml` & `uxarray-2023.5.0.dev0/.github/workflows/upstream-dev-ci.yml`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/.gitignore` & `uxarray-2023.5.0.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/.pre-commit-config.yaml` & `uxarray-2023.5.0.dev0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/LICENSE` & `uxarray-2023.5.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/PKG-INFO` & `uxarray-2023.5.0.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: uxarray
-Version: 2023.4.1
+Version: 2023.5.0.dev0
 Summary: Unstructured grid model reading and recognizing with xarray.
 Home-page: https://github.com/UXARRAY/uxarray
 Maintainer: UXARRAY
 Maintainer-email: 
 Project-URL: Source, https://github.com/UXARRAY/uxarray
 Project-URL: Tracker, https://github.com/UXARRAY/uxarray/issues
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 | CI           | [![GitHub Workflow Status][github-ci-badge]][github-ci-link] [![Code Coverage Status][codecov-badge]][codecov-link]          |
 | :----------- | :--------------------------------------------------------------------------------------------------------------------------: |
 | **Docs**     |                                                                    [![Documentation Status][rtd-badge]][rtd-link]            |
 | **Package**  |                                                         [![Conda][conda-badge]][conda-link] [![PyPI][pypi-badge]][pypi-link] |
```

### Comparing `uxarray-2023.4.1/README.md` & `uxarray-2023.5.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/docs/Makefile` & `uxarray-2023.5.0.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/docs/_static/images/icons/code.svg` & `uxarray-2023.5.0.dev0/docs/_static/images/icons/code.svg`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/docs/_static/images/icons/tips.svg` & `uxarray-2023.5.0.dev0/docs/_static/images/icons/tips.svg`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/docs/_static/images/logos/DOE_vertical.png` & `uxarray-2023.5.0.dev0/docs/_static/images/logos/DOE_vertical.png`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/docs/_static/images/logos/EarthCube_logo.png` & `uxarray-2023.5.0.dev0/docs/_static/images/logos/EarthCube_logo.png`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/docs/_static/images/logos/NSF_logo.png` & `uxarray-2023.5.0.dev0/docs/_static/images/logos/NSF_logo.png`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/docs/_static/images/logos/PANGEO_logo.png` & `uxarray-2023.5.0.dev0/docs/_static/images/logos/PANGEO_logo.png`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/docs/_static/images/logos/uxarray_temp_logo.png` & `uxarray-2023.5.0.dev0/docs/_static/images/logos/uxarray_temp_logo.png`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/docs/_static/images/nsf.png` & `uxarray-2023.5.0.dev0/docs/_static/images/nsf.png`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/docs/_static/thumbnails/default.svg` & `uxarray-2023.5.0.dev0/docs/_static/thumbnails/default.svg`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/docs/conf.py` & `uxarray-2023.5.0.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/docs/contributing.rst` & `uxarray-2023.5.0.dev0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/docs/examples/000-template.ipynb` & `uxarray-2023.5.0.dev0/docs/examples/000-template.ipynb`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/docs/examples/002-access-grid-info.ipynb` & `uxarray-2023.5.0.dev0/docs/examples/002-access-grid-info.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8491446921134421%*

 * *Differences: {"'cells'": "{0: {'metadata': {replace: OrderedDict()}}, 1: {'metadata': {replace: "*

 * *            "OrderedDict()}}, 2: {'metadata': {'jupyter': OrderedDict([('outputs_hidden', "*

 * *            "False)])}}, 3: {'metadata': {'jupyter': OrderedDict([('outputs_hidden', False)])}}, "*

 * *            "4: {'metadata': {replace: OrderedDict()}}, 5: {'metadata': {'jupyter': "*

 * *            "OrderedDict([('outputs_hidden', False)])}}, 6: {'metadata': {replace: "*

 * *            "OrderedDict()}}, 7: {'metadata': {'jupyter': Ordered […]*

```diff
@@ -1,14 +1,12 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "# Accessing Grid Information\n",
                 "\n",
                 "Unstructured grids can be represented in one of many different conventions\n",
                 "(UGRID, SCRIP, EXODUS, etc). These conventions have different definitions\n",
                 "and representations of the attributes and variables used to describe\n",
                 "the unstructured grid topology. Even more, the [UGRID conventions](\n",
@@ -36,44 +34,48 @@
                 "1. Indexing with Original Variable Names\n",
                 "2. Indexing with UXarray Variable Dictionary\n",
                 "3. UXarray's Standardized UGRID Names (Most convenient)"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "## Data\n",
                 "\n",
                 "We will be using two grid files, both of which are in the UGRID convention.\n",
                 "However, the key difference between them is the names used to describe the\n",
                 "attributes and variables.\n",
                 "\n",
                 "Let us first read in the data:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
                 "import uxarray as ux\n",
                 "import xarray as xr"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
                 "# Base data path\n",
                 "base_path = \"../../test/meshfiles/\"\n",
                 "\n",
                 "# Path to Grid files\n",
@@ -86,27 +88,28 @@
                 "\n",
                 "ugrid_01 = ux.Grid(ugrid_01_ds)\n",
                 "ugrid_02 = ux.Grid(ugrid_02_ds)"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "The output of the bottom cell showcases the slight differences\n",
                 "in variable names:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 16,
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\n",
@@ -128,31 +131,32 @@
                 "print(\"\\nAttribute and variable names for each grid:\")\n",
                 "print(\"ugrid_01 variable names:\", ugrid_01_names)\n",
                 "print(\"ugrid_02 variable names:\", ugrid_02_names)"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "## 1. Indexing with Original Variable Names\n",
                 "\n",
                 "The simplest approach is to use the original variable name as an index\n",
                 "into the grid dataset, `Grid.ds`. Since `ugrid_01` and `ugrid_02` have\n",
                 "different names for most of their topology attributes and variables, the\n",
                 "index for accessing them will be different for both grids."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 20,
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
                 "x_1 = ugrid_01.ds['Mesh2_node_x']\n",
                 "y_1 = ugrid_01.ds['Mesh2_node_y']\n",
                 "face_nodes_1 = ugrid_01.ds['Mesh2_face_nodes']\n",
                 "n_face_nodes_1 = ugrid_01.ds['nMaxMesh2_face_nodes']\n",
@@ -161,85 +165,85 @@
                 "y_2 = ugrid_02.ds['mesh_node_y']\n",
                 "face_nodes_2 = ugrid_02.ds['mesh_face_nodes']\n",
                 "n_face_nodes_2 = ugrid_02.ds['nFaceNodes']"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "## 2. Indexing with UXarray Variable Dictionary\n",
                 "\n",
-                "UXarray provides a dictionary, `Grid.ds_var_names`, to map the original\n",
+                "UXarray provides a dictionary, `Grid.grid_var_names`, to map the original\n",
                 "topology attribute and variable names that come from the grid file into\n",
                 "a standardized set of names. In other words, the dictionary uses a\n",
                 "standardized set of UGRID attribute and variable names as keys, and the\n",
                 "original variable names that come from the grid file as values.\n",
                 "\n",
                 "This allows us to use the same index into either dataset. However, this\n",
                 "makes the indexing code much longer than the previous method."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 24,
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
-                "var_names_dict = ugrid_01.ds_var_names\n",
+                "var_names_dict = ugrid_01.grid_var_names\n",
                 "x_1 = ugrid_01.ds[var_names_dict['Mesh2_node_x']]\n",
                 "y_1 = ugrid_01.ds[var_names_dict['Mesh2_node_y']]\n",
                 "face_nodes_1 = ugrid_01.ds[var_names_dict['Mesh2_face_nodes']]\n",
                 "n_face_nodes_1 = ugrid_01.ds[var_names_dict['nMesh2_node']]\n",
                 "\n",
-                "var_names_dict = ugrid_02.ds_var_names\n",
+                "var_names_dict = ugrid_02.grid_var_names\n",
                 "x_2 = ugrid_02.ds[var_names_dict['Mesh2_node_x']]\n",
                 "y_2 = ugrid_02.ds[var_names_dict['Mesh2_node_y']]\n",
                 "face_nodes_2 = ugrid_02.ds[var_names_dict['Mesh2_face_nodes']]\n",
                 "n_face_nodes_2 = ugrid_02.ds[var_names_dict['nMesh2_node']]"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "Please note, for instance, we accessed the actual variable `mesh_node_x`\n",
                 "of `ugrid_02` via indexing the dictionary with the standardized name\n",
                 "`Mesh2_node_x`, likewise in `ugrid_01`."
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "## 3. UXarray's Standardized UGRID Names\n",
                 "The last way of accessing grid topology attributes and variables is to use\n",
                 "the standardized UGRID namings provided by UXarray. This method still\n",
-                "utilizes the dictionary, `ds_var_names`, under the hood to return a\n",
+                "utilizes the dictionary, `grid_var_names`, under the hood to return a\n",
                 "reference to the variable or attribute that is stored withing\n",
                 "`UXarray.Grid.ds`.\n",
                 "\n",
                 "This eliminates the need to remember the original variable names and\n",
-                "needing to index through the `ds_var_names` dictionary. Because of this,\n",
+                "needing to index through the `grid_var_names` dictionary. Because of this,\n",
                 "we find this as the most convenient approach."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 22,
             "metadata": {
-                "collapsed": false
+                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                }
             },
             "outputs": [],
             "source": [
                 "x_1 = ugrid_01.Mesh2_node_x\n",
                 "y_1 = ugrid_01.Mesh2_node_y\n",
                 "face_nodes_1 = ugrid_01.Mesh2_face_nodes\n",
                 "n_face_nodes_1 = ugrid_01.nMesh2_node\n",
@@ -248,40 +252,38 @@
                 "y_2 = ugrid_02.Mesh2_node_y\n",
                 "face_nodes_2 = ugrid_02.Mesh2_face_nodes\n",
                 "n_face_nodes_2 = ugrid_02.nMesh2_node"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
+            "metadata": {},
             "source": [
                 "In conclusion, there are three ways of accessing the grid attributes and\n",
                 "variables. Even though the UXarray developers recommend using the\n",
                 "standardized UGRID names method, users can find each various pros/cons with\n",
                 "each of these access ways."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
-                "version": 2
+                "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython2",
-            "version": "2.7.6"
+            "pygments_lexer": "ipython3",
+            "version": "3.10.10"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 0
+    "nbformat_minor": 4
 }
```

### Comparing `uxarray-2023.4.1/docs/examples/003-area-calc.ipynb` & `uxarray-2023.5.0.dev0/docs/examples/003-area-calc.ipynb`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/docs/index.rst` & `uxarray-2023.5.0.dev0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/docs/installation.rst` & `uxarray-2023.5.0.dev0/docs/installation.rst`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 Required dependencies for installing and testing Uxarray
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The following packages should be installed (in your active conda
 environment)::
 
-    - Python 3.7+
+    - Python 3.9+
     - `pytest <https://docs.pytest.org/en/stable/>`_  (For tests only)
     - `xarray <http://xarray.pydata.org/en/stable/>`_
 
 If you don't have these packages installed, the next section describes
 how to setup a conda environment with them.
 
 Creating a Conda environment
```

### Comparing `uxarray-2023.4.1/docs/make.bat` & `uxarray-2023.5.0.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/docs/user_api/index.rst` & `uxarray-2023.5.0.dev0/docs/user_api/index.rst`

 * *Files 24% similar despite different names*

```diff
@@ -9,38 +9,39 @@
 documentation to see the tentative whole API and let us know if you have any feedback!
 
 Grid Class
 ----------
 .. autosummary::
    :toctree: _autosummary
 
-   grid.Grid
+   uxarray.core.grid.Grid
 
 
 Grid Methods
 ------------
+.. currentmodule:: uxarray.core.grid.Grid
 .. autosummary::
    :toctree: _autosummary
 
-   grid.Grid.calculate_total_face_area
-   grid.Grid.compute_face_areas
-   grid.Grid.encode_as
-   grid.Grid.integrate
-
+   calculate_total_face_area
+   compute_face_areas
+   encode_as
+   integrate
 
 Helper Functions
 ----------------
+.. currentmodule:: uxarray
 .. autosummary::
    :toctree: _autosummary
 
-   helpers.calculate_face_area
-   helpers.calculate_spherical_triangle_jacobian
-   helpers.calculate_spherical_triangle_jacobian_barycentric
-   helpers.get_all_face_area_from_coords
-   helpers.get_gauss_quadratureDG
-   helpers.get_tri_quadratureDG
-   helpers.grid_center_lat_lon
-   helpers.parse_grid_type
-   helpers.node_xyz_to_lonlat_rad
-   helpers.node_lonlat_rad_to_xyz
-   helpers.normalize_in_place
-   helpers.close_face_nodes
+   utils.helpers.calculate_face_area
+   utils.helpers.calculate_spherical_triangle_jacobian
+   utils.helpers.calculate_spherical_triangle_jacobian_barycentric
+   utils.helpers.close_face_nodes
+   utils.helpers.get_all_face_area_from_coords
+   utils.helpers.get_gauss_quadratureDG
+   utils.helpers.get_tri_quadratureDG
+   utils.helpers.grid_center_lat_lon
+   utils.helpers.node_xyz_to_lonlat_rad
+   utils.helpers.node_lonlat_rad_to_xyz
+   utils.helpers.normalize_in_place
+   utils.helpers.parse_grid_type
```

### Comparing `uxarray-2023.4.1/docs/user_api/uxarray_api.md` & `uxarray-2023.5.0.dev0/docs/user_api/uxarray_api.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Core (tier 1) functionality is indicated using regular text/list
 item style. \
 Secondary (tier 2) functionality is indicated using (*) in front.
 
 # class uxarray.Grid
 
-Describes an unstructured grid.
+Describes an unstructured grid via [Dataset
+Accessor](https://docs.xarray.dev/en/stable/internals/extending-xarray.html)
+to a ``xarray.Dataset`` object.
 
 ## uxarray.Grid Attributes
 
 - uxarray.Grid.ds: DataSet\
   DataSet containing uxarray.Grid properties
   `dims={nMesh2_node (total number of nodes),
   nMesh2_face (number of faces),
```

### Comparing `uxarray-2023.4.1/meta.yaml` & `uxarray-2023.5.0.dev0/meta.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% set version = "2023.04.1" %}
+{% set version = "2023.05.0dev" %}
 
 package:
   name: 'uxarray'
   version: {{ version }}
 
 build:
   noarch: python
```

### Comparing `uxarray-2023.4.1/setup.py` & `uxarray-2023.5.0.dev0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,28 +19,28 @@
 
 
 setup(
     name='uxarray',
     version=version(),
     maintainer='UXARRAY',
     maintainer_email='',
-    python_requires='>=3.7',
+    python_requires='>=3.9',
     install_requires=requirements,
     description=
     """Unstructured grid model reading and recognizing with xarray.""",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         'Operating System :: OS Independent',
         'Intended Audience :: Science/Research',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering',
     ],
     include_package_data=True,
     packages=find_packages(exclude=["docs", "test", "docs.*", "test.*"]),
     # namespace_packages=['UXARRAY'],
     url='https://github.com/UXARRAY/uxarray',
     project_urls={
```

### Comparing `uxarray-2023.4.1/test/meshfiles/exodus/mixed/mixed.exo` & `uxarray-2023.5.0.dev0/test/meshfiles/exodus/mixed/mixed.exo`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/exodus/outCSne8/outCSne8.g` & `uxarray-2023.5.0.dev0/test/meshfiles/exodus/outCSne8/outCSne8.g`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/mpas/QU/mesh.QU.1920km.151026.nc` & `uxarray-2023.5.0.dev0/test/meshfiles/mpas/QU/mesh.QU.1920km.151026.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/scrip/outCSne8/outCSne8.nc` & `uxarray-2023.5.0.dev0/test/meshfiles/scrip/outCSne8/outCSne8.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/shp/grid_fire.shp` & `uxarray-2023.5.0.dev0/test/meshfiles/shp/grid_fire.shp`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/ugrid/fesom/README.md` & `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/README.md`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/ugrid/fesom/a_ice.fesom.1948.nc` & `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/a_ice.fesom.1948.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/ugrid/fesom/fesom.mesh.diag.nc` & `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/fesom.mesh.diag.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/ugrid/fesom/salt.fesom.1948.nc` & `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/salt.fesom.1948.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/ugrid/fesom/sst.fesom.1948.nc` & `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/sst.fesom.1948.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/ugrid/fesom/temp.fesom.1948.nc` & `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/temp.fesom.1948.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/ugrid/fesom/test_scrip_outfile.nc` & `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/test_scrip_outfile.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/ugrid/fesom/u.fesom.1948.nc` & `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/u.fesom.1948.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/ugrid/fesom/uice.fesom.1948.nc` & `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/uice.fesom.1948.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/ugrid/fesom/v.fesom.1948.nc` & `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/v.fesom.1948.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/ugrid/fesom/vice.fesom.1948.nc` & `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/fesom/vice.fesom.1948.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/ugrid/geoflow-small/grid.nc` & `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/geoflow-small/grid.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/ugrid/geoflow-small/v1.nc` & `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/geoflow-small/v1.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/ugrid/geoflow-small/v2.nc` & `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/geoflow-small/v2.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/ugrid/geoflow-small/v3.nc` & `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/geoflow-small/v3.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/ugrid/outCSne30/outCSne30.ug` & `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/outCSne30/outCSne30.ug`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/ugrid/outCSne30/outCSne30_var2.nc` & `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/outCSne30/outCSne30_var2.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/ugrid/outCSne30/outCSne30_vortex.nc` & `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/outCSne30/outCSne30_vortex.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/ugrid/outRLL1deg/outRLL1deg.ug` & `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/outRLL1deg/outRLL1deg.ug`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/ugrid/outRLL1deg/outRLL1deg_vortex.nc` & `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/outRLL1deg/outRLL1deg_vortex.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4.ug` & `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4.ug`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4_vortex.nc` & `uxarray-2023.5.0.dev0/test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4_vortex.nc`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/test/test_helpers.py` & `uxarray-2023.5.0.dev0/test/test_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,125 +5,139 @@
 import xarray as xr
 
 from unittest import TestCase
 from pathlib import Path
 
 import uxarray as ux
 
-from uxarray.helpers import _replace_fill_values
-from uxarray.constants import INT_DTYPE, INT_FILL_VALUE
+from uxarray.utils.helpers import _replace_fill_values
+from uxarray.utils.constants import INT_DTYPE, INT_FILL_VALUE
 
 try:
     import constants
 except ImportError:
     from . import constants
 
 # Data files
 current_path = Path(os.path.dirname(os.path.realpath(__file__)))
 
-exodus = current_path / "meshfiles" / "exodus" / "outCSne8" / "outCSne8.g"
-ne8 = current_path / 'meshfiles' / "scrip" / "outCSne8" / 'outCSne8.nc'
+gridfile_exo_CSne8 = current_path / "meshfiles" / "exodus" / "outCSne8" / "outCSne8.g"
+gridfile_scrip_CSne8 = current_path / 'meshfiles' / "scrip" / "outCSne8" / 'outCSne8.nc'
+
 err_tolerance = 1.0e-12
 
 
 class TestIntegrate(TestCase):
 
     def test_face_area_coords(self):
         """Test function for helper function get_all_face_area_from_coords."""
         # Note: currently only testing one face, but this can be used to get area of multiple faces
         x = np.array([0.57735027, 0.57735027, -0.57735027])
         y = np.array([-5.77350269e-01, 5.77350269e-01, 5.77350269e-01])
         z = np.array([-0.57735027, -0.57735027, -0.57735027])
+
         face_nodes = np.array([[0, 1, 2]]).astype(INT_DTYPE)
         face_dimension = np.array([3], dtype=INT_DTYPE)
+
         area = ux.get_all_face_area_from_coords(x,
                                                 y,
                                                 z,
                                                 face_nodes,
                                                 face_dimension,
                                                 3,
                                                 coords_type="cartesian")
+
         nt.assert_almost_equal(area, constants.TRI_AREA, decimal=1)
 
     def test_calculate_face_area(self):
         """Test function for helper function calculate_face_area - only one face."""
         # Note: currently only testing one face, but this can be used to get area of multiple faces
         # Also note, this does not need face_nodes, assumes nodes are in counterclockwise orientation
         x = np.array([0.57735027, 0.57735027, -0.57735027])
         y = np.array([-5.77350269e-01, 5.77350269e-01, 5.77350269e-01])
         z = np.array([-0.57735027, -0.57735027, -0.57735027])
+
         area = ux.calculate_face_area(x, y, z, "gaussian", 5, "cartesian")
+
         nt.assert_almost_equal(area, constants.TRI_AREA, decimal=3)
 
     def test_quadrature(self):
         order = 1
         dG, dW = ux.get_tri_quadratureDG(order)
         G = np.array([[0.33333333, 0.33333333, 0.33333333]])
         W = np.array([1.0])
 
         np.testing.assert_array_almost_equal(G, dG)
         np.testing.assert_array_almost_equal(W, dW)
 
         dG, dW = ux.get_gauss_quadratureDG(order)
+
         G = np.array([[0.5]])
         W = np.array([1.0])
 
         np.testing.assert_array_almost_equal(G, dG)
         np.testing.assert_array_almost_equal(W, dW)
 
 
 class TestGridCenter(TestCase):
 
     def test_grid_center(self):
         """Calculates if the calculated center point of a grid box is the same
         as a given value for the same dataset."""
-        ds_ne8 = xr.open_dataset(ne8)
+        ds_scrip_CSne8 = xr.open_dataset(gridfile_scrip_CSne8)
 
         # select actual center_lat/lon
-        scrip_center_lon = ds_ne8['grid_center_lon']
-        scrip_center_lat = ds_ne8['grid_center_lat']
+        scrip_center_lon = ds_scrip_CSne8['grid_center_lon']
+        scrip_center_lat = ds_scrip_CSne8['grid_center_lat']
 
         # Calculate the center_lat/lon using same dataset's corner_lat/lon
-        calc_center = ux.grid_center_lat_lon(ds_ne8)
+        calc_center = ux.grid_center_lat_lon(ds_scrip_CSne8)
         calc_lat = calc_center[0]
         calc_lon = calc_center[1]
 
         # Test that calculated center_lat/lon is the same as actual center_lat/lon
         np.testing.assert_array_almost_equal(scrip_center_lat, calc_lat)
         np.testing.assert_array_almost_equal(scrip_center_lon, calc_lon)
 
 
 class TestCoordinatesConversion(TestCase):
 
     def test_normalize_in_place(self):
-        [x, y, z] = ux.helpers.normalize_in_place(
+        [x, y, z] = ux.utils.helpers.normalize_in_place(
             [random.random(), random.random(),
              random.random()])
+
         self.assertLessEqual(np.absolute(np.sqrt(x * x + y * y + z * z) - 1),
                              err_tolerance)
 
     def test_node_xyz_to_lonlat_rad(self):
-        [x, y, z] = ux.helpers.normalize_in_place([
+        [x, y, z] = ux.utils.helpers.normalize_in_place([
             random.uniform(-1, 1),
             random.uniform(-1, 1),
             random.uniform(-1, 1)
         ])
-        [lon, lat] = ux.helpers.node_xyz_to_lonlat_rad([x, y, z])
-        [new_x, new_y, new_z] = ux.helpers.node_lonlat_rad_to_xyz([lon, lat])
+
+        [lon, lat] = ux.utils.helpers.node_xyz_to_lonlat_rad([x, y, z])
+        [new_x, new_y,
+         new_z] = ux.utils.helpers.node_lonlat_rad_to_xyz([lon, lat])
+
         self.assertLessEqual(np.absolute(new_x - x), err_tolerance)
         self.assertLessEqual(np.absolute(new_y - y), err_tolerance)
         self.assertLessEqual(np.absolute(new_z - z), err_tolerance)
 
     def test_node_latlon_rad_to_xyz(self):
         [lon, lat] = [
             random.uniform(0, 2 * np.pi),
             random.uniform(-0.5 * np.pi, 0.5 * np.pi)
         ]
-        [x, y, z] = ux.helpers.node_lonlat_rad_to_xyz([lon, lat])
-        [new_lon, new_lat] = ux.helpers.node_xyz_to_lonlat_rad([x, y, z])
+
+        [x, y, z] = ux.utils.helpers.node_lonlat_rad_to_xyz([lon, lat])
+
+        [new_lon, new_lat] = ux.utils.helpers.node_xyz_to_lonlat_rad([x, y, z])
+
         self.assertLessEqual(np.absolute(new_lon - lon), err_tolerance)
         self.assertLessEqual(np.absolute(new_lat - lat), err_tolerance)
 
 
 class TestConstants(TestCase):
     # DTYPE as set in constants.py
     expected_int_dtype = INT_DTYPE
```

### Comparing `uxarray-2023.4.1/test/test_mpas.py` & `uxarray-2023.5.0.dev0/test/test_mpas.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from uxarray._mpas import _replace_padding, _replace_zeros, _to_zero_index
-from uxarray._mpas import _read_mpas, _primal_to_ugrid, _dual_to_ugrid
+from uxarray.io._mpas import _replace_padding, _replace_zeros, _to_zero_index
+from uxarray.io._mpas import _read_mpas
 import uxarray as ux
 import xarray as xr
 from unittest import TestCase
 import numpy as np
 import os
 from pathlib import Path
 
-from uxarray.constants import INT_DTYPE, INT_FILL_VALUE
+from uxarray.utils.constants import INT_DTYPE, INT_FILL_VALUE
 
 current_path = Path(os.path.dirname(os.path.realpath(__file__)))
 
 
 class TestMPAS(TestCase):
     """Test suite for Read MPAS functionality."""
 
@@ -25,16 +25,16 @@
     def test_read_mpas(self):
         """Tests execution of _read_mpas()"""
         mpas_primal_ugrid = _read_mpas(self.mpas_xr_ds, use_dual=False)
         mpas_dual_ugrid = _read_mpas(self.mpas_xr_ds, use_dual=True)
 
     def test_mpas_to_grid(self):
         """Tests creation of Grid object from converted MPAS dataset."""
-        mpas_uxgrid_primal = ux.Grid(self.mpas_xr_ds, use_dual=False)
-        mpas_uxgrid_primal = ux.Grid(self.mpas_xr_ds, use_dual=True)
+        mpas_uxgrid_primal = ux.open_grid(self.mpas_grid_path, use_dual=False)
+        mpas_uxgrid_primal = ux.open_grid(self.mpas_grid_path, use_dual=True)
 
     def test_primal_to_ugrid_conversion(self):
         """Verifies that the Primal-Mesh was converted properly."""
 
         # primal-mesh encoded in the UGRID conventions
         ds = _read_mpas(self.mpas_xr_ds, use_dual=False)
 
@@ -94,16 +94,16 @@
         verticesOnCell = _replace_padding(verticesOnCell, nEdgesOnCell)
         verticesOnCell = _replace_zeros(verticesOnCell)
         verticesOnCell = _to_zero_index(verticesOnCell)
 
         assert np.array_equal(verticesOnCell, gold_output)
 
     def test_set_attrs(self):
-        """Tests the execution of "_set_global_attrs", checking for attributes
-        being correctly stored in "Grid.ds"."""
+        """Tests the execution of ``_set_global_attrs``, checking for
+        attributes being correctly stored in ``Grid._ds``"""
 
         # full set of expected mpas attributes
         expected_attrs = [
             'sphere_radius', 'mesh_spec', 'on_a_sphere', 'mesh_id',
             'is_periodic', 'x_period', 'y_period'
         ]
 
@@ -117,8 +117,8 @@
         ds.attrs['y_period'] = 1.0
 
         # create a grid
         uxgrid = ux.Grid(ds)
 
         # check if all expected attributes are set
         for mpas_attr in expected_attrs:
-            assert mpas_attr in uxgrid.ds.attrs
+            assert mpas_attr in uxgrid._ds.attrs
```

### Comparing `uxarray-2023.4.1/test/test_scrip.py` & `uxarray-2023.5.0.dev0/test/test_scrip.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-from uxarray._scrip import _read_scrip, _encode_scrip
-from uxarray.constants import INT_DTYPE, INT_FILL_VALUE
 import uxarray as ux
 import xarray as xr
 from unittest import TestCase
 import numpy as np
+import numpy.testing as nt
 
 import os
 from pathlib import Path
 
+from uxarray.io._scrip import _read_scrip, _encode_scrip
+from uxarray.utils.constants import INT_DTYPE, INT_FILL_VALUE
+
 current_path = Path(os.path.dirname(os.path.realpath(__file__)))
 
-ne30 = current_path / 'meshfiles' / "ugrid" / "outCSne30" / 'outCSne30.ug'
-ne8 = current_path / 'meshfiles' / "scrip" / "outCSne8" / 'outCSne8.nc'
+gridfile_ne30 = current_path / 'meshfiles' / "ugrid" / "outCSne30" / 'outCSne30.ug'
+gridfile_ne8 = current_path / 'meshfiles' / "scrip" / "outCSne8" / 'outCSne8.nc'
 
-ds_ne30 = xr.open_dataset(ne30, decode_times=False,
+ds_ne30 = xr.open_dataset(gridfile_ne30, decode_times=False,
                           engine='netcdf4')  # mesh2_node_x/y
-ds_ne8 = xr.open_dataset(ne8, decode_times=False,
+ds_ne8 = xr.open_dataset(gridfile_ne8, decode_times=False,
                          engine='netcdf4')  # grid_corner_lat/lon
 
 
 class TestScrip(TestCase):
 
     def test_exception_nonSCRIP(self):
         """Checks that exception is raised if non-SCRIP formatted file is
@@ -47,54 +49,53 @@
 
         # Create UGRID from SCRIP file
         scrip_in_ds = _read_scrip(ds_ne8)
         new_path = current_path / "meshfiles" / "scrip_to_ugrid.ug"
         scrip_in_ds.to_netcdf(str(new_path))  # Save as new file
 
         # Use xarray open_dataset, create a uxarray grid object to then create SCRIP file from new UGRID file
-        xr_obj = xr.open_dataset(str(new_path))
-        ugrid_out = ux.Grid(xr_obj)
+        ugrid_out = ux.open_grid(new_path)
 
         scrip_encode_ds = _encode_scrip(ugrid_out.Mesh2_face_nodes,
                                         ugrid_out.Mesh2_node_x,
                                         ugrid_out.Mesh2_node_y,
                                         ugrid_out.face_areas)
 
         # Test newly created SCRIP is same as original SCRIP
-        np.testing.assert_array_almost_equal(scrip_encode_ds['grid_corner_lat'],
-                                             ds_ne8['grid_corner_lat'])
-        np.testing.assert_array_almost_equal(scrip_encode_ds['grid_corner_lon'],
-                                             ds_ne8['grid_corner_lon'])
+        nt.assert_array_almost_equal(scrip_encode_ds['grid_corner_lat'],
+                                     ds_ne8['grid_corner_lat'])
+        nt.assert_array_almost_equal(scrip_encode_ds['grid_corner_lon'],
+                                     ds_ne8['grid_corner_lon'])
 
         # Tests that calculated center lat/lon values are equivalent to original
-        np.testing.assert_array_almost_equal(scrip_encode_ds['grid_center_lon'],
-                                             ds_ne8['grid_center_lon'])
-        np.testing.assert_array_almost_equal(scrip_encode_ds['grid_center_lat'],
-                                             ds_ne8['grid_center_lat'])
+        nt.assert_array_almost_equal(scrip_encode_ds['grid_center_lon'],
+                                     ds_ne8['grid_center_lon'])
+        nt.assert_array_almost_equal(scrip_encode_ds['grid_center_lat'],
+                                     ds_ne8['grid_center_lat'])
 
         # Tests that calculated face area values are equivalent to original
-        np.testing.assert_array_almost_equal(scrip_encode_ds['grid_area'],
-                                             ds_ne8['grid_area'])
+        nt.assert_array_almost_equal(scrip_encode_ds['grid_area'],
+                                     ds_ne8['grid_area'])
 
         # Tests that calculated grid imask values are equivalent to original
-        np.testing.assert_array_almost_equal(scrip_encode_ds['grid_imask'],
-                                             ds_ne8['grid_imask'])
+        nt.assert_array_almost_equal(scrip_encode_ds['grid_imask'],
+                                     ds_ne8['grid_imask'])
 
         # Test that "mesh" variables are not in new file
         with self.assertRaises(KeyError):
             assert scrip_encode_ds['Mesh2_node_x']
             assert scrip_encode_ds['Mesh2_node_y']
 
     def test_scrip_variable_names(self):
         """Tests that returned dataset from writer function has all required
         SCRIP variables."""
-        xr_ne30 = xr.open_dataset(ne30)
-        ux_ne30 = ux.Grid(xr_ne30)
-        scrip30 = _encode_scrip(ux_ne30.Mesh2_face_nodes, ux_ne30.Mesh2_node_x,
-                                ux_ne30.Mesh2_node_y, ux_ne30.face_areas)
+        uxds_ne30 = ux.open_grid(gridfile_ne30)
+        scrip30 = _encode_scrip(uxds_ne30.Mesh2_face_nodes,
+                                uxds_ne30.Mesh2_node_x, uxds_ne30.Mesh2_node_y,
+                                uxds_ne30.face_areas)
 
         # List of relevant variable names for a scrip file
         var_list = [
             'grid_corner_lat', 'grid_dims', 'grid_imask', 'grid_area',
             'grid_center_lon'
         ]
 
@@ -112,17 +113,14 @@
 
         assert strip_lon.all() == mesh08['Mesh2_node_x'].all()
 
     def test_standardized_dtype_and_fill(self):
         """Test to see if Mesh2_Face_Nodes uses the expected integer datatype
         and expected fill value as set in constants.py."""
 
-        xr_ne30 = xr.open_dataset(ne30)
-        ux_grid_01 = ux.Grid(xr_ne30)
-
-        xr_ne8 = xr.open_dataset(ne8)
-        ux_grid_02 = ux.Grid(xr_ne8)
+        ux_grid_01 = ux.open_grid(gridfile_ne30)
+        ux_grid_02 = ux.open_grid(gridfile_ne8)
 
         grids = [ux_grid_01, ux_grid_02]
         for grid in grids:
             assert grid.Mesh2_face_nodes.dtype == INT_DTYPE
             assert grid.Mesh2_face_nodes._FillValue == INT_FILL_VALUE
```

### Comparing `uxarray-2023.4.1/test/test_ugrid.py` & `uxarray-2023.5.0.dev0/test/test_ugrid.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,89 +1,85 @@
 import os
 import xarray as xr
 
 from unittest import TestCase
 from pathlib import Path
 import warnings
+import numpy.testing as nt
 
 import uxarray as ux
-from uxarray.constants import INT_DTYPE, INT_FILL_VALUE
+from uxarray.utils.constants import INT_DTYPE, INT_FILL_VALUE
 
 try:
     import constants
 except ImportError:
     from . import constants
 
 current_path = Path(os.path.dirname(os.path.realpath(__file__)))
 
+gridfile_ne30 = current_path / "meshfiles" / "ugrid" / "outCSne30" / "outCSne30.ug"
+gridfile_RLL1deg = current_path / "meshfiles" / "ugrid" / "outRLL1deg" / "outRLL1deg.ug"
+gridfile_RLL10deg_ne4 = current_path / "meshfiles" / "ugrid" / "ov_RLL10deg_CSne4" / "ov_RLL10deg_CSne4.ug"
+
+gridfile_exo_ne8 = current_path / "meshfiles" / "exodus" / "outCSne8" / "outCSne8.g"
+
 
 class TestUgrid(TestCase):
 
     def test_read_ugrid(self):
-        """Reads a ugrid file."""
-
-        ug_filename1 = current_path / "meshfiles" / "ugrid" / "outCSne30" / "outCSne30.ug"
-        ug_filename2 = current_path / "meshfiles" / "ugrid" / "outRLL1deg" / "outRLL1deg.ug"
-        ug_filename3 = current_path / "meshfiles" / "ugrid" / "ov_RLL10deg_CSne4" / "ov_RLL10deg_CSne4.ug"
+        """Reads a ugrid file."""\
 
-        xr_grid1 = xr.open_dataset(str(ug_filename1))
-        xr_grid2 = xr.open_dataset(str(ug_filename2))
-        xr_grid3 = xr.open_dataset(str(ug_filename3))
-
-        ux_grid1 = ux.Grid(xr_grid1)
-        ux_grid2 = ux.Grid(xr_grid2)
-        ux_grid3 = ux.Grid(xr_grid3)
-
-        assert (ux_grid1.Mesh2_node_x.size == constants.NNODES_outCSne30)
-        assert (ux_grid2.Mesh2_node_x.size == constants.NNODES_outRLL1deg)
-        assert (
-            ux_grid3.Mesh2_node_x.size == constants.NNODES_ov_RLL10deg_CSne4)
+        uxgrid_ne30 = ux.open_grid(str(gridfile_ne30))
+        uxgrid_RLL1deg = ux.open_grid(str(gridfile_RLL1deg))
+        uxgrid_RLL10deg_ne4 = ux.open_grid(str(gridfile_RLL10deg_ne4))
+
+        nt.assert_equal(uxgrid_ne30.Mesh2_node_x.size,
+                        constants.NNODES_outCSne30)
+        nt.assert_equal(uxgrid_RLL1deg.Mesh2_node_x.size,
+                        constants.NNODES_outRLL1deg)
+        nt.assert_equal(uxgrid_RLL10deg_ne4.Mesh2_node_x.size,
+                        constants.NNODES_ov_RLL10deg_CSne4)
 
     def test_read_ugrid_opendap(self):
         """Read an ugrid model from an OPeNDAP URL."""
 
         try:
             # make sure we can read the ugrid file from the OPeNDAP URL
             url = "http://test.opendap.org:8080/opendap/ugrid/NECOFS_GOM3_FORECAST.nc"
-            xr_grid = xr.open_dataset(url, drop_variables="siglay")
+            uxgrid_url = ux.open_grid(url, drop_variables="siglay")
 
         except OSError:
             # print warning and pass if we can't connect to the OPeNDAP server
             warnings.warn(f'Could not connect to OPeNDAP server: {url}')
             pass
 
         else:
-            ugrid = ux.Grid(xr_grid)
-            assert isinstance(getattr(ugrid, "Mesh2_node_x"), xr.DataArray)
-            assert isinstance(getattr(ugrid, "Mesh2_node_y"), xr.DataArray)
-            assert isinstance(getattr(ugrid, "Mesh2_face_nodes"), xr.DataArray)
+
+            assert isinstance(getattr(uxgrid_url, "Mesh2_node_x"), xr.DataArray)
+            assert isinstance(getattr(uxgrid_url, "Mesh2_node_y"), xr.DataArray)
+            assert isinstance(getattr(uxgrid_url, "Mesh2_face_nodes"),
+                              xr.DataArray)
 
     def test_encode_ugrid(self):
         """Read an Exodus dataset and encode that as a UGRID format."""
 
-        exo2_filename = current_path / "meshfiles" / "exodus" / "outCSne8" / "outCSne8.g"
-        xr_grid = xr.open_dataset(str(exo2_filename))
-        ux_grid = ux.Grid(xr_grid)
+        ux_grid = ux.open_grid(gridfile_exo_ne8)
         ux_grid.encode_as("ugrid")
 
     def test_standardized_dtype_and_fill(self):
         """Test to see if Mesh2_Face_Nodes uses the expected integer datatype
         and expected fill value as set in constants.py."""
 
         ug_filename1 = current_path / "meshfiles" / "ugrid" / "outCSne30" / "outCSne30.ug"
         ug_filename2 = current_path / "meshfiles" / "ugrid" / "outRLL1deg" / "outRLL1deg.ug"
         ug_filename3 = current_path / "meshfiles" / "ugrid" / "ov_RLL10deg_CSne4" / "ov_RLL10deg_CSne4.ug"
 
-        xr_grid1 = xr.open_dataset(str(ug_filename1))
-        xr_grid2 = xr.open_dataset(str(ug_filename2))
-        xr_grid3 = xr.open_dataset(str(ug_filename3))
-
-        ux_grid1 = ux.Grid(xr_grid1)
-        ux_grid2 = ux.Grid(xr_grid2)
-        ux_grid3 = ux.Grid(xr_grid3)
+        ux_grid1 = ux.open_grid(ug_filename1)
+        ux_grid2 = ux.open_grid(ug_filename2)
+        ux_grid3 = ux.open_grid(ug_filename3)
 
         # check for correct dtype and fill value
         grids_with_fill = [ux_grid2]
         for grid in grids_with_fill:
             assert grid.Mesh2_face_nodes.dtype == INT_DTYPE
             assert grid.Mesh2_face_nodes._FillValue == INT_FILL_VALUE
             assert INT_FILL_VALUE in grid.Mesh2_face_nodes.values
@@ -96,12 +92,12 @@
     def test_standardized_dtype_and_fill_dask(self):
         """Test to see if Mesh2_Face_Nodes uses the expected integer datatype
         and expected fill value as set in constants.py.
 
         with dask chunking
         """
         ug_filename = current_path / "meshfiles" / "ugrid" / "outRLL1deg" / "outRLL1deg.ug"
-        xr_grid = xr.open_dataset(str(ug_filename), chunks={'nMesh2_node': 100})
-        ux_grid = ux.Grid(xr_grid)
+        ux_grid = ux.open_grid(ug_filename)
+
         assert ux_grid.Mesh2_face_nodes.dtype == INT_DTYPE
         assert ux_grid.Mesh2_face_nodes._FillValue == INT_FILL_VALUE
         assert INT_FILL_VALUE in ux_grid.Mesh2_face_nodes.values
```

### Comparing `uxarray-2023.4.1/uxarray/_exodus.py` & `uxarray-2023.5.0.dev0/uxarray/io/_exodus.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import xarray as xr
 import numpy as np
 from pathlib import PurePath
 from datetime import datetime
 
-from uxarray.helpers import _replace_fill_values
-from uxarray.constants import INT_DTYPE, INT_FILL_VALUE
+from uxarray.utils.helpers import _replace_fill_values
+from uxarray.utils.constants import INT_DTYPE, INT_FILL_VALUE
 
 
 # Exodus Number is one-based.
-def _read_exodus(ext_ds, ds_var_names):
+def _read_exodus(ext_ds, grid_var_names):
     """Exodus file reader.
 
     Parameters: xarray.Dataset, required
     Returns: ugrid aware xarray.Dataset
     """
 
     # Not loading specific variables.
@@ -107,15 +107,16 @@
             # check if num face nodes is less than max.
             if value.data.shape[1] <= max_face_nodes:
                 conn = np.full((value.data.shape[1], max_face_nodes),
                                0,
                                dtype=conn.dtype)
                 conn = value.data
             else:
-                raise "found face_nodes_dim greater than nMaxMesh2_face_nodes"
+                raise RuntimeError(
+                    "found face_nodes_dim greater than nMaxMesh2_face_nodes")
 
             # find the elem_type as etype for this element
             for k, v in value.attrs.items():
                 if k == "elem_type":
                     # TODO: etype if not used now, remove if it'll never be required
                     etype = v
 
@@ -147,15 +148,15 @@
         ds = ds.set_coords(["Mesh2_node_x", "Mesh2_node_y", "Mesh2_node_z"])
     else:
         ds = ds.set_coords(["Mesh2_node_x", "Mesh2_node_y"])
 
     return ds
 
 
-def _encode_exodus(ds, ds_var_names, outfile=None):
+def _encode_exodus(ds, grid_var_names, outfile=None):
     """Encodes an Exodus file.
 
     Parameters
     ----------
 
     ds : xarray.Dataset, required
         Dataset to be encoded to exodus file.
@@ -207,40 +208,40 @@
     ux_exodus_version = 1.0
     qa_records = [["uxarray"], [ux_exodus_version], [date], [time]]
     exo_ds["qa_records"] = xr.DataArray(data=xr.DataArray(
         np.array(qa_records, dtype='str')),
                                         dims=["four", "num_qa_rec"])
 
     # get orig dimension from Mesh2 attribute topology dimension
-    dim = ds[ds_var_names["Mesh2"]].topology_dimension
+    dim = ds[grid_var_names["Mesh2"]].topology_dimension
 
     c_data = []
     if dim == 2:
         c_data = xr.DataArray([
-            ds[ds_var_names["Mesh2_node_x"]].data.tolist(),
-            ds[ds_var_names["Mesh2_node_y"]].data.tolist()
+            ds[grid_var_names["Mesh2_node_x"]].data.tolist(),
+            ds[grid_var_names["Mesh2_node_y"]].data.tolist()
         ])
     elif dim == 3:
         c_data = xr.DataArray([
-            ds[ds_var_names["Mesh2_node_x"]].data.tolist(),
-            ds[ds_var_names["Mesh2_node_y"]].data.tolist(),
-            ds[ds_var_names["Mesh2_node_z"]].data.tolist()
+            ds[grid_var_names["Mesh2_node_x"]].data.tolist(),
+            ds[grid_var_names["Mesh2_node_y"]].data.tolist(),
+            ds[grid_var_names["Mesh2_node_z"]].data.tolist()
         ])
 
     exo_ds["coord"] = xr.DataArray(data=c_data, dims=["num_dim", "num_nodes"])
 
     # process face nodes, this array holds num faces at corresponding location
     # eg num_el_all_blks = [0, 0, 6, 12] signifies 6 TRI and 12 SHELL elements
-    num_el_all_blks = np.zeros(ds[ds_var_names["nMaxMesh2_face_nodes"]].size,
+    num_el_all_blks = np.zeros(ds[grid_var_names["nMaxMesh2_face_nodes"]].size,
                                "i8")
     # this list stores connectivity without filling
     conn_nofill = []
 
     # store the number of faces in an array
-    for row in ds[ds_var_names["Mesh2_face_nodes"]].astype(INT_DTYPE).data:
+    for row in ds[grid_var_names["Mesh2_face_nodes"]].astype(INT_DTYPE).data:
 
         # find out -1 in each row, this indicates lower than max face nodes
         arr = np.where(row == -1)
         # arr[0].size returns the location of first -1 in the conn list
         # if > 0, arr[0][0] is the num_nodes forming the face
         if arr[0].size > 0:
             # increment the number of faces at the corresponding location
@@ -248,15 +249,15 @@
             # append without -1s eg. [1, 2, 3, -1] to [1, 2, 3]
             # convert to list (for sorting later)
             row = row[:(arr[0][0])].tolist()
             list_node = list(map(int, row))
             conn_nofill.append(list_node)
         elif arr[0].size == 0:
             # increment the number of faces for this "nMaxMesh2_face_nodes" face
-            num_el_all_blks[ds[ds_var_names["nMaxMesh2_face_nodes"]].size -
+            num_el_all_blks[ds[grid_var_names["nMaxMesh2_face_nodes"]].size -
                             1] += 1
             # get integer list nodes
             list_node = list(map(int, row.tolist()))
             conn_nofill.append(list_node)
         else:
             raise RuntimeError(
                 "num nodes in conn array is greater than nMaxMesh2_face_nodes. Abort!"
```

### Comparing `uxarray-2023.4.1/uxarray/_mpas.py` & `uxarray-2023.5.0.dev0/uxarray/io/_mpas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import xarray as xr
 import numpy as np
 import warnings
 
-from uxarray.constants import INT_DTYPE, INT_FILL_VALUE
+from uxarray.utils.constants import INT_DTYPE, INT_FILL_VALUE
 
 
 def _primal_to_ugrid(in_ds, out_ds):
     """Encodes the MPAS Primal-Mesh in the UGRID conventions.
 
     Parameters
     ----------
```

### Comparing `uxarray-2023.4.1/uxarray/_scrip.py` & `uxarray-2023.5.0.dev0/uxarray/io/_scrip.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import xarray as xr
 import numpy as np
 
-from uxarray.helpers import grid_center_lat_lon
+from uxarray.utils.helpers import grid_center_lat_lon, _replace_fill_values
 
-from uxarray.helpers import _replace_fill_values
-from uxarray.constants import INT_DTYPE, INT_FILL_VALUE
+from uxarray.utils.constants import INT_DTYPE, INT_FILL_VALUE
 
 
 def _to_ugrid(in_ds, out_ds):
     """If input dataset (``in_ds``) file is an unstructured SCRIP file,
     function will reassign SCRIP variables to UGRID conventions in output file
     (``out_ds``).
```

### Comparing `uxarray-2023.4.1/uxarray/_ugrid.py` & `uxarray-2023.5.0.dev0/uxarray/io/_ugrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import xarray as xr
 import numpy as np
-from uxarray.helpers import _replace_fill_values
-from uxarray.constants import INT_DTYPE, INT_FILL_VALUE
+from uxarray.utils.helpers import _replace_fill_values
+from uxarray.utils.constants import INT_DTYPE, INT_FILL_VALUE
 
 
 def _read_ugrid(xr_ds, var_names_dict):
     """UGRID file reader.
 
     Parameters: xarray.Dataset, required
     Returns: ugrid aware xarray.Dataset
```

### Comparing `uxarray-2023.4.1/uxarray/get_quadratureDG.py` & `uxarray-2023.5.0.dev0/uxarray/utils/get_quadratureDG.py`

 * *Files identical despite different names*

### Comparing `uxarray-2023.4.1/uxarray/grid.py` & `uxarray-2023.5.0.dev0/uxarray/core/grid.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,124 +1,124 @@
 """uxarray grid module."""
-import os
 import xarray as xr
 import numpy as np
 
 # reader and writer imports
-from ._exodus import _read_exodus, _encode_exodus
-from ._ugrid import _read_ugrid, _encode_ugrid
-from ._shapefile import _read_shpfile
-from ._scrip import _read_scrip, _encode_scrip
-from ._mpas import _read_mpas
-from .helpers import get_all_face_area_from_coords, parse_grid_type, node_xyz_to_lonlat_rad, node_lonlat_rad_to_xyz, close_face_nodes
-from .constants import INT_DTYPE, INT_FILL_VALUE
+from uxarray.io._exodus import _read_exodus, _encode_exodus
+from uxarray.io._mpas import _read_mpas
+from uxarray.io._ugrid import _read_ugrid, _encode_ugrid
+from uxarray.io._shapefile import _read_shpfile
+from uxarray.io._scrip import _read_scrip, _encode_scrip
+from uxarray.utils.helpers import (get_all_face_area_from_coords,
+                                   parse_grid_type, node_xyz_to_lonlat_rad,
+                                   node_lonlat_rad_to_xyz, close_face_nodes)
+from uxarray.utils.constants import INT_DTYPE, INT_FILL_VALUE
 
 
 class Grid:
     """
     Examples
     ----------
 
     Open an exodus file with Uxarray Grid object
 
     >>> xarray_obj = xr.open_dataset("filename.g")
     >>> mesh = ux.Grid(xarray_obj)
 
-    Encode as a `xarray.Dataset` in the UGRID format
+    Encode as the UGRID format
 
     >>> mesh.encode_as("ugrid")
     """
 
-    def __init__(self, dataset, **kwargs):
+    def __init__(self, input_obj, **kwargs):
         """Initialize grid variables, decide if loading happens via file, verts
         or gridspec.
 
         Parameters
         ----------
-        dataset : xarray.Dataset, ndarray, list, tuple, required
-            Input xarray.Dataset or vertex coordinates that form one face.
+        input_obj : xarray.Dataset, ndarray, list, tuple, required
+            Input xarray.Dataset or vertex coordinates that form faces.
 
         Other Parameters
         ----------------
+        gridspec: bool, optional
+            Specifies gridspec
         islatlon : bool, optional
             Specify if the grid is lat/lon based
-        concave: bool, optional
+        isconcave: bool, optional
             Specify if this grid has concave elements (internal checks for this are possible)
-        gridspec: bool, optional
-            Specifies gridspec
-        mesh_type: str, optional
-            Specify the mesh file type, eg. exo, ugrid, shp, mpas, etc
         use_dual: bool, optional
             Specify whether to use the primal (use_dual=False) or dual (use_dual=True) mesh if the file type is mpas
+
         Raises
         ------
             RuntimeError
-                If specified file not found
+                If specified file not found or recognized
         """
+
         # initialize internal variable names
-        self.__init_ds_var_names__()
+        self.__init_grid_var_names__()
 
         # initialize face_area variable
         self._face_areas = None
 
         # TODO: fix when adding/exercising gridspec
 
         # unpack kwargs
         # sets default values for all kwargs to None
         kwargs_list = [
-            'gridspec', 'vertices', 'islatlon', 'concave', 'source_grid',
+            'gridspec', 'vertices', 'islatlon', 'isconcave', 'source_grid',
             'use_dual'
         ]
         for key in kwargs_list:
             setattr(self, key, kwargs.get(key, None))
 
         # check if initializing from verts:
-        if isinstance(dataset, (list, tuple, np.ndarray)):
-            dataset = np.asarray(dataset)
+        if isinstance(input_obj, (list, tuple, np.ndarray)):
+            input_obj = np.asarray(input_obj)
             # grid with multiple faces
-            if dataset.ndim == 3:
-                self.__from_vert__(dataset)
+            if input_obj.ndim == 3:
+                self.__from_vert__(input_obj)
                 self.source_grid = "From vertices"
             # grid with a single face
-            elif dataset.ndim == 2:
-                dataset = np.array([dataset])
-                self.__from_vert__(dataset)
+            elif input_obj.ndim == 2:
+                input_obj = np.array([input_obj])
+                self.__from_vert__(input_obj)
                 self.source_grid = "From vertices"
             else:
                 raise RuntimeError(
-                    f"Invalid Input Dimension: {dataset.ndim}. Expected dimension should be "
+                    f"Invalid Input Dimension: {input_obj.ndim}. Expected dimension should be "
                     f"3: [nMesh2_face, nMesh2_node, Two/Three] or 2 when only "
                     f"one face is passed in.")
+
         # check if initializing from string
         # TODO: re-add gridspec initialization when implemented
-        elif isinstance(dataset, xr.Dataset):
-            self.mesh_type = parse_grid_type(dataset)
-            self.__from_ds__(dataset=dataset)
+        elif isinstance(input_obj, xr.Dataset):
+            self.mesh_type = parse_grid_type(input_obj)
+            self.__from_ds__(dataset=input_obj)
         else:
             raise RuntimeError("Dataset is not a valid input type.")
 
         # initialize convenience attributes
         self.__init_grid_var_attrs__()
 
         # construct connectivity
-        if self.source_grid != "From vertices":
-            if "Mesh2_edge_nodes" not in self.ds:
-                self._build_edge_node_connectivity()
+        self._build_edge_node_connectivity()
 
         # build face dimension, possibly safeguard for large datasets
-        self._build_face_dimension()
+        self._build_nNodes_per_face()
 
-    def __init_ds_var_names__(self):
+    def __init_grid_var_names__(self):
         """Populates a dictionary for storing uxarray's internal representation
         of xarray object.
 
         Note ugrid conventions are flexible with names of variables, see:
         http://ugrid-conventions.github.io/ugrid-conventions/
         """
-        self.ds_var_names = {
+        self.grid_var_names = {
             "Mesh2": "Mesh2",
             "Mesh2_node_x": "Mesh2_node_x",
             "Mesh2_node_y": "Mesh2_node_y",
             "Mesh2_node_z": "Mesh2_node_z",
             "Mesh2_face_nodes": "Mesh2_face_nodes",
             # initialize dims
             "nMesh2_node": "nMesh2_node",
@@ -129,63 +129,64 @@
     def __init_grid_var_attrs__(self) -> None:
         """Initialize attributes for directly accessing UGRID dimensions and
         variables.
 
         Examples
         ----------
         Assuming the mesh node coordinates for longitude are stored with an input
-        name of 'mesh_node_x', we store this variable name in the `ds_var_names`
+        name of 'mesh_node_x', we store this variable name in the `grid_var_names`
         dictionary with the key 'Mesh2_node_x'. In order to access it, we do:
 
-        >>> x = grid.ds[grid.ds_var_names["Mesh2_node_x"]]
+        >>> x = grid._ds[grid.grid_var_names["Mesh2_node_x"]]
 
         With the help of this function, we can directly access it through the
         use of a standardized name based on the UGRID conventions
 
         >>> x = grid.Mesh2_node_x
         """
 
         # Iterate over dict to set access attributes
-        for key, value in self.ds_var_names.items():
+        for key, value in self.grid_var_names.items():
             # Set Attributes for Data Variables
-            if self.ds.data_vars is not None:
-                if value in self.ds.data_vars:
-                    setattr(self, key, self.ds[value])
+            if self._ds.data_vars is not None:
+                if value in self._ds.data_vars:
+                    setattr(self, key, self._ds[value])
 
             # Set Attributes for Coordinates
-            if self.ds.coords is not None:
-                if value in self.ds.coords:
-                    setattr(self, key, self.ds[value])
+            if self._ds.coords is not None:
+                if value in self._ds.coords:
+                    setattr(self, key, self._ds[value])
 
             # Set Attributes for Dimensions
-            if self.ds.dims is not None:
-                if value in self.ds.dims:
-                    setattr(self, key, len(self.ds[value]))
+            if self._ds.dims is not None:
+                if value in self._ds.dims:
+                    setattr(self, key, len(self._ds[value]))
 
     def __from_vert__(self, dataset):
         """Create a grid with faces constructed from vertices specified by the
         given argument.
 
         Parameters
         ----------
         dataset : ndarray, list, tuple, required
             Input vertex coordinates that form our face(s)
         """
-        self.ds = xr.Dataset()
-        self.ds["Mesh2"] = xr.DataArray(
+        self._ds = xr.Dataset()
+        self._ds["Mesh2"] = xr.DataArray(
             attrs={
                 "cf_role": "mesh_topology",
                 "long_name": "Topology data of unstructured mesh",
                 "topology_dimension": -1,
                 "node_coordinates": "Mesh2_node_x Mesh2_node_y Mesh2_node_z",
                 "node_dimension": "nMesh2_node",
                 "face_node_connectivity": "Mesh2_face_nodes",
                 "face_dimension": "nMesh2_face"
             })
-        self.ds.Mesh2.attrs['topology_dimension'] = dataset.ndim
+
+        self._ds.Mesh2.attrs['topology_dimension'] = dataset.ndim
 
         if self.islatlon is not None and self.islatlon is False:
             x_units = 'm'
             y_units = 'm'
             z_units = 'm'
         else:
             x_units = "degrees_east"
@@ -227,64 +228,75 @@
 
             # Update indices accordingly
             for i, idx in enumerate(false_indices):
                 indices[indices == idx] = INT_FILL_VALUE
                 indices[(indices > idx) & (indices != INT_FILL_VALUE)] -= 1
 
         # Create coordinate DataArrays
-        self.ds["Mesh2_node_x"] = xr.DataArray(data=unique_verts[:, 0],
-                                               dims=["nMesh2_node"],
-                                               attrs={"units": x_units})
-        self.ds["Mesh2_node_y"] = xr.DataArray(data=unique_verts[:, 1],
-                                               dims=["nMesh2_node"],
-                                               attrs={"units": y_units})
+        self._ds["Mesh2_node_x"] = xr.DataArray(data=unique_verts[:, 0],
+                                                dims=["nMesh2_node"],
+                                                attrs={"units": x_units})
+        self._ds["Mesh2_node_y"] = xr.DataArray(data=unique_verts[:, 1],
+                                                dims=["nMesh2_node"],
+                                                attrs={"units": y_units})
         if dataset.shape[-1] > 2:
-            self.ds["Mesh2_node_z"] = xr.DataArray(data=unique_verts[:, 2],
-                                                   dims=["nMesh2_node"],
-                                                   attrs={"units": z_units})
+            self._ds["Mesh2_node_z"] = xr.DataArray(data=unique_verts[:, 2],
+                                                    dims=["nMesh2_node"],
+                                                    attrs={"units": z_units})
         else:
-            self.ds["Mesh2_node_z"] = xr.DataArray(data=unique_verts[:, 1] *
-                                                   0.0,
-                                                   dims=["nMesh2_node"],
-                                                   attrs={"units": z_units})
+            self._ds["Mesh2_node_z"] = xr.DataArray(data=unique_verts[:, 1] *
+                                                    0.0,
+                                                    dims=["nMesh2_node"],
+                                                    attrs={"units": z_units})
 
         # Create connectivity array using indices of unique vertices
         connectivity = indices.reshape(dataset.shape[:-1])
-        self.ds["Mesh2_face_nodes"] = xr.DataArray(
+        self._ds["Mesh2_face_nodes"] = xr.DataArray(
             data=xr.DataArray(connectivity).astype(INT_DTYPE),
             dims=["nMesh2_face", "nMaxMesh2_face_nodes"],
             attrs={
                 "cf_role": "face_node_connectivity",
                 "_FillValue": INT_FILL_VALUE,
                 "start_index": 0
             })
 
     # load mesh from a file
     def __from_ds__(self, dataset):
         """Loads a mesh dataset."""
         # call reader as per mesh_type
         if self.mesh_type == "exo":
-            self.ds = _read_exodus(dataset, self.ds_var_names)
+            self._ds = _read_exodus(dataset, self.grid_var_names)
         elif self.mesh_type == "scrip":
-            self.ds = _read_scrip(dataset)
+            self._ds = _read_scrip(dataset)
         elif self.mesh_type == "ugrid":
-            self.ds, self.ds_var_names = _read_ugrid(dataset, self.ds_var_names)
+            self._ds, self.grid_var_names = _read_ugrid(dataset,
+                                                        self.grid_var_names)
         elif self.mesh_type == "shp":
-            self.ds = _read_shpfile(dataset)
+            self._ds = _read_shpfile(dataset)
         elif self.mesh_type == "mpas":
             # select whether to use the dual mesh
             if self.use_dual is not None:
-                self.ds = _read_mpas(dataset, self.use_dual)
+                self._ds = _read_mpas(dataset, self.use_dual)
             else:
-                self.ds = _read_mpas(dataset)
+                self._ds = _read_mpas(dataset)
         else:
             raise RuntimeError("unknown mesh type")
 
         dataset.close()
 
+    def copy(self):
+        """Returns a deep copy of this grid."""
+        return Grid(xr.Dataset(self._ds),
+                    gridspec=self.gridspec,
+                    vertices=self.vertices,
+                    islatlon=self.islatlon,
+                    isconcave=self.isconcave,
+                    source_grid=self.source_grid,
+                    use_dual=self.use_dual)
+
     def encode_as(self, grid_type):
         """Encodes the grid as a new `xarray.Dataset` per grid format supplied
         in the `grid_type` argument.
 
         Parameters
         ----------
         grid_type : str, required
@@ -299,18 +311,18 @@
         Raises
         ------
         RuntimeError
             If provided grid type or file type is unsupported.
         """
 
         if grid_type == "ugrid":
-            out_ds = _encode_ugrid(self.ds)
+            out_ds = _encode_ugrid(self._ds)
 
         elif grid_type == "exodus":
-            out_ds = _encode_exodus(self.ds, self.ds_var_names)
+            out_ds = _encode_exodus(self._ds, self.grid_var_names)
 
         elif grid_type == "scrip":
             out_ds = _encode_scrip(self.Mesh2_face_nodes, self.Mesh2_node_x,
                                    self.Mesh2_node_y, self.face_areas)
         else:
             raise RuntimeError("The grid type not supported: ", grid_type)
 
@@ -354,30 +366,30 @@
 
         Examples
         --------
         Open a uxarray grid file
 
         >>> grid = ux.open_dataset("/home/jain/uxarray/test/meshfiles/ugrid/outCSne30/outCSne30.ug")
 
-        Get area of all faces in the same order as listed in grid.ds.Mesh2_face_nodes
+        Get area of all faces in the same order as listed in grid._ds.Mesh2_face_nodes
 
         >>> grid.face_areas
         array([0.00211174, 0.00211221, 0.00210723, ..., 0.00210723, 0.00211221,
             0.00211174])
         """
         # if self._face_areas is None: # this allows for using the cached result,
         # but is not the expected behavior behavior as we are in need to recompute if this function is called with different quadrature_rule or order
 
         # area of a face call needs the units for coordinate conversion if spherical grid is used
         coords_type = "spherical"
         if not "degree" in self.Mesh2_node_x.units:
             coords_type = "cartesian"
 
         face_nodes = self.Mesh2_face_nodes.data
-        face_dimension = self.Mesh2_face_dimension.data
+        nNodes_per_face = self.nNodes_per_face.data
         dim = self.Mesh2.attrs['topology_dimension']
 
         # initialize z
         z = np.zeros((self.nMesh2_node))
 
         # call func to cal face area of all nodes
         x = self.Mesh2_node_x.data
@@ -391,30 +403,72 @@
         # if not (int etc.), convert to float, this is to avoid numba errors
         x, y, z = (arr.astype(float)
                    if not np.issubdtype(arr[0], np.floating) else arr
                    for arr in (x, y, z))
 
         # call function to get area of all the faces as a np array
         self._face_areas = get_all_face_area_from_coords(
-            x, y, z, face_nodes, face_dimension, dim, quadrature_rule, order,
+            x, y, z, face_nodes, nNodes_per_face, dim, quadrature_rule, order,
             coords_type)
 
         return self._face_areas
 
+    def __eq__(self, other):
+        """Two grids are equal if they have matching grid topology variables,
+        coordinates, and dims all of which are equal.
+
+        Parameters
+        ----------
+        other : uxarray.Grid
+            The second grid object to be compared with `self`
+
+        Returns
+        -------
+        If two grids are equal : bool
+        """
+        if other is not None:
+            # Iterate over dict to set access attributes
+            for key, value in self.grid_var_names.items():
+                # Check if all grid variables are equal
+                if self._ds.data_vars is not None:
+                    if value in self._ds.data_vars:
+                        if not self._ds[value].equals(
+                                other._ds[other.grid_var_names[key]]):
+                            return False
+        else:
+            return False
+
+        return True
+
+    def __ne__(self, other):
+        """Two grids are not equal if they have differing grid topology
+        variables, coordinates, or dims.
+
+        Parameters
+        ----------
+        other : uxarray.Grid
+            The second grid object to be compared with `self`
+
+        Returns
+        -------
+        If two grids are not equal : bool
+        """
+        return not self.__eq__(other)
+
     # use the property keyword for declaration on face_areas property
     @property
     def face_areas(self):
         """Declare face_areas as a property."""
         # if self._face_areas is not None: it allows for using the cached result
         if self._face_areas is None:
             self.compute_face_areas()
         return self._face_areas
 
     def integrate(self, var_ds, quadrature_rule="triangular", order=4):
-        """Integrates over all the faces of the given mesh.
+        """Integrates a xarray.Dataset over all the faces of the given mesh.
 
         Parameters
         ----------
         var_ds : Xarray dataset, required
             Xarray dataset containing values to integrate on this grid
         quadrature_rule : str, optional
             Quadrature rule to use. Defaults to "triangular".
@@ -449,36 +503,49 @@
             )
         var_key = var_key[0]
         face_vals = var_ds[var_key].to_numpy()
         integral = np.dot(face_areas, face_vals)
 
         return integral
 
-    def _build_edge_node_connectivity(self):
+    def _build_edge_node_connectivity(self, repopulate=False):
         """Constructs the UGRID connectivity variable (``Mesh2_edge_nodes``)
-        and stores it within the internal (``Grid.ds``) and through the
+        and stores it within the internal (``Grid._ds``) and through the
         attribute (``Grid.Mesh2_edge_nodes``).
 
         Additionally, the attributes (``inverse_indices``) and
         (``fill_value_mask``) are stored for constructing other
         connectivity variables.
-        """
-        padded_face_nodes = close_face_nodes(self.Mesh2_face_nodes.values,
-                                             self.nMesh2_face,
-                                             self.nMaxMesh2_face_nodes)
-
-        # array of empty edge nodes where each entry is a pair of indices
-        edge_nodes = np.empty((self.nMesh2_face * self.nMaxMesh2_face_nodes, 2),
-                              dtype=INT_DTYPE)
 
-        # first index includes starting node up to non-padded value
-        edge_nodes[:, 0] = padded_face_nodes[:, :-1].ravel()
+        Parameters
+        ----------
+        repopulate : bool, optional
+            Flag used to indicate if we want to overwrite the existed `Mesh2_edge_nodes` and generate a new
+            inverse_indices, default is False
+        """
+
+        # need to derive edge nodes
+        if "Mesh2_edge_nodes" not in self._ds or repopulate:
+            padded_face_nodes = close_face_nodes(self.Mesh2_face_nodes.values,
+                                                 self.nMesh2_face,
+                                                 self.nMaxMesh2_face_nodes)
+
+            # array of empty edge nodes where each entry is a pair of indices
+            edge_nodes = np.empty(
+                (self.nMesh2_face * self.nMaxMesh2_face_nodes, 2),
+                dtype=INT_DTYPE)
+
+            # first index includes starting node up to non-padded value
+            edge_nodes[:, 0] = padded_face_nodes[:, :-1].ravel()
 
-        # second index includes second node up to padded value
-        edge_nodes[:, 1] = padded_face_nodes[:, 1:].ravel()
+            # second index includes second node up to padded value
+            edge_nodes[:, 1] = padded_face_nodes[:, 1:].ravel()
+        else:
+            # If "Mesh2_edge_nodes" already exists, directly return the function call
+            return
 
         # sorted edge nodes
         edge_nodes.sort(axis=1)
 
         # unique edge nodes
         edge_nodes_unique, inverse_indices = np.unique(edge_nodes,
                                                        return_inverse=True,
@@ -504,39 +571,69 @@
                                   side='right')
         # subtract the corresponding indexes from `inverse_indices`
         for i in range(len(inverse_indices)):
             if inverse_indices[i] != INT_FILL_VALUE:
                 inverse_indices[i] -= indexes[i]
 
         # add Mesh2_edge_nodes to internal dataset
-        self.ds['Mesh2_edge_nodes'] = xr.DataArray(
+        self._ds['Mesh2_edge_nodes'] = xr.DataArray(
             edge_nodes_unique,
             dims=["nMesh2_edge", "Two"],
             attrs={
                 "cf_role":
                     "edge_node_connectivity",
+                "_FillValue":
+                    INT_FILL_VALUE,
                 "long_name":
                     "Maps every edge to the two nodes that it connects",
                 "start_index":
                     INT_DTYPE(0),
                 "inverse_indices":
                     inverse_indices,
                 "fill_value_mask":
                     fill_value_mask
             })
 
         # set standardized attributes
-        setattr(self, "Mesh2_edge_nodes", self.ds['Mesh2_edge_nodes'])
+        setattr(self, "Mesh2_edge_nodes", self._ds['Mesh2_edge_nodes'])
         setattr(self, "nMesh2_edge", edge_nodes_unique.shape[0])
 
+    def _build_face_edges_connectivity(self):
+        """Constructs the UGRID connectivity variable (``Mesh2_face_edges``)
+        and stores it within the internal (``Grid._ds``) and through the
+        attribute (``Grid.Mesh2_face_edges``)."""
+        if ("Mesh2_edge_nodes" not in self._ds or
+                "inverse_indices" not in self._ds['Mesh2_edge_nodes'].attrs):
+            self._build_edge_node_connectivity(repopulate=True)
+
+        inverse_indices = self._ds['Mesh2_edge_nodes'].inverse_indices
+        inverse_indices = inverse_indices.reshape(self.nMesh2_face,
+                                                  self.nMaxMesh2_face_nodes)
+
+        self._ds["Mesh2_face_edges"] = xr.DataArray(
+            data=inverse_indices,
+            dims=["nMesh2_face", "nMaxMesh2_face_edges"],
+            attrs={
+                "cf_role":
+                    "face_edges_connectivity",
+                "start_index":
+                    INT_DTYPE(0),
+                "long_name":
+                    "Maps every edge to the two nodes that it connects",
+            })
+
+        # set standardized attributes
+        setattr(self, "nMaxMesh2_face_edges", inverse_indices.shape[1])
+        setattr(self, "Mesh2_face_edges", self._ds["Mesh2_face_edges"])
+
     def _populate_cartesian_xyz_coord(self):
-        """A helper function that populates the xyz attribute in UXarray.ds.
-        This function is called when we need to use the cartesian coordinates
-        for each node to do the calculation but the input data only has the
-        "Mesh2_node_x" and "Mesh2_node_y" in degree.
+        """A helper function that populates the xyz attribute in
+        UXarray.Grid._ds. This function is called when we need to use the
+        cartesian coordinates for each node to do the calculation but the input
+        data only has the "Mesh2_node_x" and "Mesh2_node_y" in degree.
 
         Note
         ----
         In the UXarray, we abide the UGRID convention and make sure the following attributes will always have its
         corresponding units as stated below:
 
         Mesh2_node_x
@@ -550,39 +647,39 @@
         Mesh2_node_cart_y
          unit:  "m"
         Mesh2_node_cart_z
          unit:  "m"
         """
 
         # Check if the cartesian coordinates are already populated
-        if "Mesh2_node_cart_x" in self.ds.keys():
+        if "Mesh2_node_cart_x" in self._ds.keys():
             return
 
-        # check for units and create Mesh2_node_cart_x/y/z set to self.ds
+        # check for units and create Mesh2_node_cart_x/y/z set to self._ds
         nodes_lon_rad = np.deg2rad(self.Mesh2_node_x.values)
         nodes_lat_rad = np.deg2rad(self.Mesh2_node_y.values)
         nodes_rad = np.stack((nodes_lon_rad, nodes_lat_rad), axis=1)
         nodes_cart = np.asarray(
             list(map(node_lonlat_rad_to_xyz, list(nodes_rad))))
 
-        self.ds["Mesh2_node_cart_x"] = xr.DataArray(
+        self._ds["Mesh2_node_cart_x"] = xr.DataArray(
             data=nodes_cart[:, 0],
             dims=["nMesh2_node"],
             attrs={
                 "standard_name": "cartesian x",
                 "units": "m",
             })
-        self.ds["Mesh2_node_cart_y"] = xr.DataArray(
+        self._ds["Mesh2_node_cart_y"] = xr.DataArray(
             data=nodes_cart[:, 1],
             dims=["nMesh2_node"],
             attrs={
                 "standard_name": "cartesian y",
                 "units": "m",
             })
-        self.ds["Mesh2_node_cart_z"] = xr.DataArray(
+        self._ds["Mesh2_node_cart_z"] = xr.DataArray(
             data=nodes_cart[:, 2],
             dims=["nMesh2_node"],
             attrs={
                 "standard_name": "cartesian z",
                 "units": "m",
             })
 
@@ -614,74 +711,75 @@
         Mesh2_node_cart_y
          unit:  "m"
         Mesh2_node_cart_z
          unit:  "m"
         """
 
         # Check if the "Mesh2_node_x" is already in longitude
-        if "degree" in self.ds.Mesh2_node_x.units:
+        if "degree" in self._ds.Mesh2_node_x.units:
             return
 
         # Check if the input Mesh2_node_xyz" are represented in the cartesian format with the unit "m"
-        if ("m" not in self.ds.Mesh2_node_x.units) or ("m" not in self.ds.Mesh2_node_y.units) \
-                or ("m" not in self.ds.Mesh2_node_z.units):
+        if ("m" not in self._ds.Mesh2_node_x.units) or ("m" not in self._ds.Mesh2_node_y.units) \
+                or ("m" not in self._ds.Mesh2_node_z.units):
             raise RuntimeError(
                 "Expected: Mesh2_node_x/y/z should be represented in the cartesian format with the "
                 "unit 'm' when calling this function")
 
         # Put the cartesian coordinates inside the proper data structure
-        self.ds["Mesh2_node_cart_x"] = xr.DataArray(
-            data=self.ds["Mesh2_node_x"].values)
-        self.ds["Mesh2_node_cart_y"] = xr.DataArray(
-            data=self.ds["Mesh2_node_y"].values)
-        self.ds["Mesh2_node_cart_z"] = xr.DataArray(
-            data=self.ds["Mesh2_node_z"].values)
+        self._ds["Mesh2_node_cart_x"] = xr.DataArray(
+            data=self._ds["Mesh2_node_x"].values)
+        self._ds["Mesh2_node_cart_y"] = xr.DataArray(
+            data=self._ds["Mesh2_node_y"].values)
+        self._ds["Mesh2_node_cart_z"] = xr.DataArray(
+            data=self._ds["Mesh2_node_z"].values)
 
         # convert the input cartesian values into the longitude latitude degree
         nodes_cart = np.stack(
-            (self.ds["Mesh2_node_x"].values, self.ds["Mesh2_node_y"].values,
-             self.ds["Mesh2_node_z"].values),
+            (self._ds["Mesh2_node_x"].values, self._ds["Mesh2_node_y"].values,
+             self._ds["Mesh2_node_z"].values),
             axis=1).tolist()
         nodes_rad = list(map(node_xyz_to_lonlat_rad, nodes_cart))
         nodes_degree = np.rad2deg(nodes_rad)
-        self.ds["Mesh2_node_x"] = xr.DataArray(
+        self._ds["Mesh2_node_x"] = xr.DataArray(
             data=nodes_degree[:, 0],
             dims=["nMesh2_node"],
             attrs={
                 "standard_name": "longitude",
                 "long_name": "longitude of mesh nodes",
                 "units": "degrees_east",
             })
-        self.ds["Mesh2_node_y"] = xr.DataArray(
+        self._ds["Mesh2_node_y"] = xr.DataArray(
             data=nodes_degree[:, 1],
             dims=["nMesh2_node"],
             attrs={
                 "standard_name": "lattitude",
                 "long_name": "latitude of mesh nodes",
                 "units": "degrees_north",
             })
 
-    def _build_face_dimension(self):
-        """Constructs ``Mesh2_face_dimension``, which calculates the dimension
-        of each face in ``Mesh2_face_nodes``"""
+    def _build_nNodes_per_face(self):
+        """Constructs ``nNodes_per_face``, which contains the number of non-
+        fill-value nodes for each face in ``Mesh2_face_nodes``"""
 
-        # Triangular Mesh
+        # Triangular Mesh (No Fill Values)
         if not hasattr(self, "nMaxMesh2_face_nodes"):
             nMaxMesh2_face_nodes = self.Mesh2_face_nodes.shape[1]
             setattr(self, "nMaxMesh2_face_nodes", nMaxMesh2_face_nodes)
 
         # padding to shape [nMesh2_face, nMaxMesh2_face_nodes + 1]
         closed = np.ones((self.nMesh2_face, self.nMaxMesh2_face_nodes + 1),
                          dtype=INT_DTYPE) * INT_FILL_VALUE
 
         closed[:, :-1] = self.Mesh2_face_nodes.copy()
 
-        face_dimension = np.argmax(closed == INT_FILL_VALUE, axis=1)
+        nNodes_per_face = np.argmax(closed == INT_FILL_VALUE, axis=1)
 
         # add to internal dataset
-        self.ds["Mesh2_face_dimension"] = xr.DataArray(
-            data=face_dimension,
+        self._ds["nNodes_per_face"] = xr.DataArray(
+            data=nNodes_per_face,
             dims=["nMesh2_face"],
             attrs={"long_name": "number of non-fill value nodes for each face"})
 
         # standardized attribute
-        setattr(self, "Mesh2_face_dimension", self.ds["Mesh2_face_dimension"])
+
+        setattr(self, "nNodes_per_face", self._ds["nNodes_per_face"])
```

### Comparing `uxarray-2023.4.1/uxarray/helpers.py` & `uxarray-2023.5.0.dev0/uxarray/utils/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import xarray as xr
 from pathlib import PurePath
 from .get_quadratureDG import get_gauss_quadratureDG, get_tri_quadratureDG
 from numba import njit, config
 import math
 
-from uxarray.constants import INT_DTYPE, INT_FILL_VALUE
+from uxarray.utils.constants import INT_DTYPE, INT_FILL_VALUE
 
 config.DISABLE_JIT = False
 
 
 def parse_grid_type(dataset):
     """Checks input and contents to determine grid type. Supports detection of
     UGrid, SCRIP, Exodus and shape file.
```

### Comparing `uxarray-2023.4.1/uxarray.egg-info/PKG-INFO` & `uxarray-2023.5.0.dev0/uxarray.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: uxarray
-Version: 2023.4.1
+Version: 2023.5.0.dev0
 Summary: Unstructured grid model reading and recognizing with xarray.
 Home-page: https://github.com/UXARRAY/uxarray
 Maintainer: UXARRAY
 Maintainer-email: 
 Project-URL: Source, https://github.com/UXARRAY/uxarray
 Project-URL: Tracker, https://github.com/UXARRAY/uxarray/issues
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 | CI           | [![GitHub Workflow Status][github-ci-badge]][github-ci-link] [![Code Coverage Status][codecov-badge]][codecov-link]          |
 | :----------- | :--------------------------------------------------------------------------------------------------------------------------: |
 | **Docs**     |                                                                    [![Documentation Status][rtd-badge]][rtd-link]            |
 | **Package**  |                                                         [![Conda][conda-badge]][conda-link] [![PyPI][pypi-badge]][pypi-link] |
```

### Comparing `uxarray-2023.4.1/uxarray.egg-info/SOURCES.txt` & `uxarray-2023.5.0.dev0/uxarray.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 INSTALLATION.md
 LICENSE
 README.md
 build.sh
 meta.yaml
 requirements.txt
 setup.py
+.github/PULL_REQUEST_TEMPLATE.md
 .github/codecov.yml
 .github/dependabot.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
+.github/ISSUE_TEMPLATE/release_request.md
 .github/workflows/ci.yml
 .github/workflows/pre-commit.yml
 .github/workflows/pypi.yaml
 .github/workflows/upstream-dev-ci.yml
 ci/docs.yml
 ci/environment.yml
 ci/upstream-dev-environment.yml
@@ -51,14 +53,16 @@
 docs/examples/002-access-grid-info.ipynb
 docs/examples/003-area-calc.ipynb
 docs/internal_api/index.rst
 docs/user_api/index.rst
 docs/user_api/uxarray_api.md
 test/__init__.py
 test/constants.py
+test/test_api.py
+test/test_dataset.py
 test/test_exodus.py
 test/test_grid.py
 test/test_helpers.py
 test/test_mpas.py
 test/test_placeholder.py
 test/test_scrip.py
 test/test_ugrid.py
@@ -86,22 +90,28 @@
 test/meshfiles/ugrid/outCSne30/outCSne30_var2.nc
 test/meshfiles/ugrid/outCSne30/outCSne30_vortex.nc
 test/meshfiles/ugrid/outRLL1deg/outRLL1deg.ug
 test/meshfiles/ugrid/outRLL1deg/outRLL1deg_vortex.nc
 test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4.ug
 test/meshfiles/ugrid/ov_RLL10deg_CSne4/ov_RLL10deg_CSne4_vortex.nc
 uxarray/__init__.py
-uxarray/_exodus.py
-uxarray/_mpas.py
-uxarray/_scrip.py
-uxarray/_shapefile.py
-uxarray/_ugrid.py
-uxarray/constants.py
-uxarray/get_quadratureDG.py
-uxarray/grid.py
-uxarray/helpers.py
 uxarray.egg-info/PKG-INFO
 uxarray.egg-info/SOURCES.txt
 uxarray.egg-info/dependency_links.txt
 uxarray.egg-info/not-zip-safe
 uxarray.egg-info/requires.txt
-uxarray.egg-info/top_level.txt
+uxarray.egg-info/top_level.txt
+uxarray/core/__init__.py
+uxarray/core/api.py
+uxarray/core/dataarray.py
+uxarray/core/dataset.py
+uxarray/core/grid.py
+uxarray/io/__init__.py
+uxarray/io/_exodus.py
+uxarray/io/_mpas.py
+uxarray/io/_scrip.py
+uxarray/io/_shapefile.py
+uxarray/io/_ugrid.py
+uxarray/utils/__init__.py
+uxarray/utils/constants.py
+uxarray/utils/get_quadratureDG.py
+uxarray/utils/helpers.py
```

