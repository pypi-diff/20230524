# Comparing `tmp/PyVBMC-1.0.0.tar.gz` & `tmp/PyVBMC-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyVBMC-1.0.0.tar", last modified: Thu Mar 16 12:49:10 2023, max compression
+gzip compressed data, was "PyVBMC-1.0.1.tar", last modified: Wed May 24 08:36:28 2023, max compression
```

## Comparing `PyVBMC-1.0.0.tar` & `PyVBMC-1.0.1.tar`

### file list

```diff
@@ -1,228 +1,228 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.592330 PyVBMC-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-16 12:48:54.000000 PyVBMC-1.0.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-16 12:48:54.000000 PyVBMC-1.0.0/.coveragerc-html.css
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-16 12:48:54.000000 PyVBMC-1.0.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.480329 PyVBMC-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.500329 PyVBMC-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-16 12:48:54.000000 PyVBMC-1.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-03-16 12:48:54.000000 PyVBMC-1.0.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-03-16 12:48:54.000000 PyVBMC-1.0.0/.github/workflows/merge-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-16 12:48:54.000000 PyVBMC-1.0.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-16 12:48:54.000000 PyVBMC-1.0.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-03-16 12:48:54.000000 PyVBMC-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-16 12:48:54.000000 PyVBMC-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-03-16 12:48:54.000000 PyVBMC-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-16 12:48:54.000000 PyVBMC-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16385 2023-03-16 12:49:10.592330 PyVBMC-1.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.500329 PyVBMC-1.0.0/PyVBMC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16385 2023-03-16 12:49:10.000000 PyVBMC-1.0.0/PyVBMC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-03-16 12:49:10.000000 PyVBMC-1.0.0/PyVBMC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 12:49:10.000000 PyVBMC-1.0.0/PyVBMC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-16 12:49:10.000000 PyVBMC-1.0.0/PyVBMC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-16 12:49:10.000000 PyVBMC-1.0.0/PyVBMC.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14389 2023-03-16 12:48:54.000000 PyVBMC-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.544330 PyVBMC-1.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    95868 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/examples/pyvbmc_example_1_basic_usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123) 29799799 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/examples/pyvbmc_example_2_inputs_outputs.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18763 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/examples/pyvbmc_example_3_diagnostics_and_saving.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   177797 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/examples/pyvbmc_example_4_validation.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   316414 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/examples/pyvbmc_example_5_prior_distributions.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   168238 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/examples/pyvbmc_example_6_noisy_likelihoods.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.548329 PyVBMC-1.0.0/examples/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/examples/scripts/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/examples/scripts/pyvbmc_example_1_full_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/examples/scripts/pyvbmc_example_2_full_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/examples/scripts/pyvbmc_example_3_full_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/examples/scripts/pyvbmc_example_4_full_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/examples/scripts/pyvbmc_example_5_full_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/examples/scripts/pyvbmc_example_6_full_code.py
--rw-r--r--   0 runner    (1001) docker     (123)   545101 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.552329 PyVBMC-1.0.0/pyvbmc/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.556330 PyVBMC-1.0.0/pyvbmc/acquisition_functions/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/acquisition_functions/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/acquisition_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/acquisition_functions/abstract_acq_fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/acquisition_functions/acq_fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9603 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/acquisition_functions/acq_fcn_imiqr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/acquisition_functions/acq_fcn_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/acquisition_functions/acq_fcn_noisy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/acquisition_functions/acq_fcn_vanilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/acquisition_functions/acq_fcn_viqr.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/acquisition_functions/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.556330 PyVBMC-1.0.0/pyvbmc/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/decorators/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/decorators/handle_0D_1D_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.556330 PyVBMC-1.0.0/pyvbmc/entropy/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/entropy/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/entropy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/entropy/entlb_vbmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/entropy/entmc_vbmc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.560330 PyVBMC-1.0.0/pyvbmc/formatting/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/formatting/formatting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.560330 PyVBMC-1.0.0/pyvbmc/function_logger/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/function_logger/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/function_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16189 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/function_logger/function_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.560330 PyVBMC-1.0.0/pyvbmc/parameter_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/parameter_transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/parameter_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17512 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/parameter_transformer/parameter_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.564329 PyVBMC-1.0.0/pyvbmc/priors/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/priors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/priors/convert_to_prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/priors/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/priors/product.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/priors/scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/priors/smooth_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/priors/spline_trapezoidal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/priors/tile_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/priors/trapezoidal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/priors/uniform_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/priors/user_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.564329 PyVBMC-1.0.0/pyvbmc/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/stats/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/stats/get_hpd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/stats/kde_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/stats/kl_div_mvn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.564329 PyVBMC-1.0.0/pyvbmc/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/_check_grad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/_compare_matlab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.568329 PyVBMC-1.0.0/pyvbmc/testing/acquisition_functions/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/acquisition_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/acquisition_functions/test_abstract_acquisition_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/acquisition_functions/test_acq_fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/acquisition_functions/test_acq_fcn_imiqr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/acquisition_functions/test_acq_fcn_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/acquisition_functions/test_acq_fcn_noisy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/acquisition_functions/test_acq_fcn_vanilla.py
--rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/acquisition_functions/test_acq_fcn_viqr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.568329 PyVBMC-1.0.0/pyvbmc/testing/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/decorators/test_handle_0D_1D_input_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.568329 PyVBMC-1.0.0/pyvbmc/testing/entropy/
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/entropy/entropy-test.mat
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/entropy/test_entlb_vbmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/entropy/test_entmc_vbmc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.568329 PyVBMC-1.0.0/pyvbmc/testing/function_logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/function_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/function_logger/test_function_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.568329 PyVBMC-1.0.0/pyvbmc/testing/parameter_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/parameter_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26815 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/parameter_transformer/test_parameter_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.572330 PyVBMC-1.0.0/pyvbmc/testing/priors/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/priors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/priors/test_convert_to_prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/priors/test_priors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/priors/test_product_prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/priors/test_scipy_prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/priors/test_smooth_box_prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/priors/test_spline_trapezoid_prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/priors/test_tile_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/priors/test_trapezoid_prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/priors/test_uniform_box_prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/priors/test_user_function_prior.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.572330 PyVBMC-1.0.0/pyvbmc/testing/stats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/stats/test_get_hpd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/stats/test_kde1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/stats/test_kldiv_mvn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.572330 PyVBMC-1.0.0/pyvbmc/testing/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/testing/test_check_grad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.572330 PyVBMC-1.0.0/pyvbmc/testing/timer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/timer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/timer/test_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.576330 PyVBMC-1.0.0/pyvbmc/testing/variational_posterior/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/variational_posterior/X.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/variational_posterior/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/variational_posterior/bnd_lb.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/variational_posterior/bnd_ub.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/variational_posterior/mu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/variational_posterior/test_moments_no_orig_flag_2_MATLAB.mat
--rw-r--r--   0 runner    (1001) docker     (123)    24759 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/variational_posterior/test_variational_posterior.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/variational_posterior/test_vp_save_and_load.py
--rw-r--r--   0 runner    (1001) docker     (123)   209285 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/variational_posterior/test_vp_save_static.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/variational_posterior/vp-test.mat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.580330 PyVBMC-1.0.0/pyvbmc/testing/vbmc/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/X.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.584329 PyVBMC-1.0.0/pyvbmc/testing/vbmc/compare_MATLAB/
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/compare_MATLAB/activesample_proposalpdf.m
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/compare_MATLAB/activesample_proposalpdf.mat
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/compare_MATLAB/fess.m
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/compare_MATLAB/fess.mat
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/compare_MATLAB/log_isbasefun.m
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/compare_MATLAB/log_isbasefun.mat
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/dF.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/dG_gp_log_joint.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/hyp.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/mu.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_active_importance_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_gaussian_process_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_iteration_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_minimize_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    12766 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_variational_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    26199 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_vbmc_active_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_vbmc_determine_best_vp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_vbmc_finalboost.py
--rw-r--r--   0 runner    (1001) docker     (123)    35797 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_vbmc_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_vbmc_loop_termination.py
--rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_vbmc_optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_vbmc_save_and_load.py
--rw-r--r--   0 runner    (1001) docker     (123)  1265762 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_vbmc_save_static.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/vbmc/y.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.584329 PyVBMC-1.0.0/pyvbmc/testing/whitening/
--rw-r--r--   0 runner    (1001) docker     (123)    10560 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/whitening/test_rotoscaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/whitening/test_warp_gp_and_vp_gp_X.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/whitening/test_warp_gp_and_vp_gp_hyps.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/whitening/test_warp_gp_and_vp_gp_hyps_new.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/whitening/test_warp_gp_and_vp_gp_y.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/whitening/test_warp_gp_and_vp_vp_K.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/whitening/test_warp_gp_and_vp_vp_lambda.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/whitening/test_warp_gp_and_vp_vp_mu.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/whitening/test_warp_gp_and_vp_vp_sigma.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/whitening/test_warp_gp_and_vp_vp_w.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/whitening/test_warp_input_R_mat.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/whitening/test_warp_input_rands.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/whitening/test_warp_input_scale.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/testing/whitening/vp_initialized_MATLAB.mat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.588330 PyVBMC-1.0.0/pyvbmc/timer/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/timer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/timer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/timer/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.588330 PyVBMC-1.0.0/pyvbmc/variational_posterior/
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/variational_posterior/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/variational_posterior/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50594 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/variational_posterior/variational_posterior.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.588330 PyVBMC-1.0.0/pyvbmc/vbmc/
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/vbmc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/vbmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17357 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/vbmc/active_importance_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    32403 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/vbmc/active_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/vbmc/create_vbmc_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)    27532 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/vbmc/gaussian_process_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/vbmc/iteration_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/vbmc/minimize_adam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.592330 PyVBMC-1.0.0/pyvbmc/vbmc/option_configs/
--rw-r--r--   0 runner    (1001) docker     (123)    14089 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/vbmc/option_configs/advanced_vbmc_options.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/vbmc/option_configs/basic_vbmc_options.ini
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/vbmc/option_configs/test_options.ini
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/vbmc/option_configs/test_options2.ini
--rw-r--r--   0 runner    (1001) docker     (123)    11576 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/vbmc/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    52699 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/vbmc/variational_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)   100181 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/vbmc/vbmc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:49:10.592330 PyVBMC-1.0.0/pyvbmc/whitening/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/whitening/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/whitening/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13121 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/pyvbmc/whitening/whitening.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 12:49:10.592330 PyVBMC-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-16 12:48:55.000000 PyVBMC-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.186777 PyVBMC-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/.coveragerc-html.css
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.130777 PyVBMC-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.134776 PyVBMC-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/.github/workflows/merge-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17181 2023-05-24 08:36:28.186777 PyVBMC-1.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.134776 PyVBMC-1.0.1/PyVBMC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17181 2023-05-24 08:36:27.000000 PyVBMC-1.0.1/PyVBMC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-24 08:36:28.000000 PyVBMC-1.0.1/PyVBMC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 08:36:27.000000 PyVBMC-1.0.1/PyVBMC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-24 08:36:27.000000 PyVBMC-1.0.1/PyVBMC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 08:36:27.000000 PyVBMC-1.0.1/PyVBMC.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15185 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.166777 PyVBMC-1.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    95868 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/examples/pyvbmc_example_1_basic_usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123) 29799799 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/examples/pyvbmc_example_2_inputs_outputs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18763 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/examples/pyvbmc_example_3_diagnostics_and_saving.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   177797 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/examples/pyvbmc_example_4_validation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   316414 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/examples/pyvbmc_example_5_prior_distributions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   168238 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/examples/pyvbmc_example_6_noisy_likelihoods.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.166777 PyVBMC-1.0.1/examples/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/examples/scripts/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/examples/scripts/pyvbmc_example_1_full_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/examples/scripts/pyvbmc_example_2_full_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/examples/scripts/pyvbmc_example_3_full_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/examples/scripts/pyvbmc_example_4_full_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/examples/scripts/pyvbmc_example_5_full_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/examples/scripts/pyvbmc_example_6_full_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)   545101 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.166777 PyVBMC-1.0.1/pyvbmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.166777 PyVBMC-1.0.1/pyvbmc/acquisition_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/acquisition_functions/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/acquisition_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/acquisition_functions/abstract_acq_fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/acquisition_functions/acq_fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9603 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/acquisition_functions/acq_fcn_imiqr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/acquisition_functions/acq_fcn_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/acquisition_functions/acq_fcn_noisy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/acquisition_functions/acq_fcn_vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/acquisition_functions/acq_fcn_viqr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/acquisition_functions/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.166777 PyVBMC-1.0.1/pyvbmc/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/decorators/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/decorators/handle_0D_1D_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.170777 PyVBMC-1.0.1/pyvbmc/entropy/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/entropy/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/entropy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/entropy/entlb_vbmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/entropy/entmc_vbmc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.170777 PyVBMC-1.0.1/pyvbmc/formatting/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/formatting/formatting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.170777 PyVBMC-1.0.1/pyvbmc/function_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/function_logger/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/function_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16183 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/function_logger/function_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.170777 PyVBMC-1.0.1/pyvbmc/parameter_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/parameter_transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/parameter_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17512 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/parameter_transformer/parameter_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.170777 PyVBMC-1.0.1/pyvbmc/priors/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/priors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/priors/convert_to_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/priors/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/priors/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/priors/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/priors/smooth_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/priors/spline_trapezoidal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/priors/tile_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/priors/trapezoidal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/priors/uniform_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/priors/user_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.170777 PyVBMC-1.0.1/pyvbmc/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/stats/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/stats/get_hpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/stats/kde_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/stats/kl_div_mvn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.170777 PyVBMC-1.0.1/pyvbmc/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/_check_grad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/_compare_matlab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.174777 PyVBMC-1.0.1/pyvbmc/testing/acquisition_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/acquisition_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/acquisition_functions/test_abstract_acquisition_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/acquisition_functions/test_acq_fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/acquisition_functions/test_acq_fcn_imiqr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/acquisition_functions/test_acq_fcn_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/acquisition_functions/test_acq_fcn_noisy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/acquisition_functions/test_acq_fcn_vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/acquisition_functions/test_acq_fcn_viqr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.174777 PyVBMC-1.0.1/pyvbmc/testing/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/decorators/test_handle_0D_1D_input_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.174777 PyVBMC-1.0.1/pyvbmc/testing/entropy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/entropy/entropy-test.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/entropy/test_entlb_vbmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/entropy/test_entmc_vbmc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.174777 PyVBMC-1.0.1/pyvbmc/testing/function_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/function_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/function_logger/test_function_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.174777 PyVBMC-1.0.1/pyvbmc/testing/parameter_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/parameter_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26815 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/parameter_transformer/test_parameter_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.174777 PyVBMC-1.0.1/pyvbmc/testing/priors/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/priors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/priors/test_convert_to_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/priors/test_priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/priors/test_product_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/priors/test_scipy_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/priors/test_smooth_box_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/priors/test_spline_trapezoid_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/priors/test_tile_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/priors/test_trapezoid_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/priors/test_uniform_box_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/priors/test_user_function_prior.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.174777 PyVBMC-1.0.1/pyvbmc/testing/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/stats/test_get_hpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/stats/test_kde1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/stats/test_kldiv_mvn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.174777 PyVBMC-1.0.1/pyvbmc/testing/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/testing/test_check_grad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.174777 PyVBMC-1.0.1/pyvbmc/testing/timer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/timer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/timer/test_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.178777 PyVBMC-1.0.1/pyvbmc/testing/variational_posterior/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/variational_posterior/X.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/variational_posterior/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/variational_posterior/bnd_lb.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/variational_posterior/bnd_ub.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/variational_posterior/mu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/variational_posterior/test_moments_no_orig_flag_2_MATLAB.mat
+-rw-r--r--   0 runner    (1001) docker     (123)    24759 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/variational_posterior/test_variational_posterior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/variational_posterior/test_vp_save_and_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)   209285 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/variational_posterior/test_vp_save_static.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/variational_posterior/vp-test.mat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.182777 PyVBMC-1.0.1/pyvbmc/testing/vbmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/X.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.182777 PyVBMC-1.0.1/pyvbmc/testing/vbmc/compare_MATLAB/
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/compare_MATLAB/activesample_proposalpdf.m
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/compare_MATLAB/activesample_proposalpdf.mat
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/compare_MATLAB/fess.m
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/compare_MATLAB/fess.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/compare_MATLAB/log_isbasefun.m
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/compare_MATLAB/log_isbasefun.mat
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/dF.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/dG_gp_log_joint.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/hyp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/mu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_active_importance_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_gaussian_process_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_iteration_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_minimize_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12766 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_variational_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26199 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_vbmc_active_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_vbmc_determine_best_vp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_vbmc_finalboost.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35797 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_vbmc_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_vbmc_loop_termination.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_vbmc_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_vbmc_save_and_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1265762 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_vbmc_save_static.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/vbmc/y.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.182777 PyVBMC-1.0.1/pyvbmc/testing/whitening/
+-rw-r--r--   0 runner    (1001) docker     (123)    10560 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/whitening/test_rotoscaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/whitening/test_warp_gp_and_vp_gp_X.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/whitening/test_warp_gp_and_vp_gp_hyps.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/whitening/test_warp_gp_and_vp_gp_hyps_new.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/whitening/test_warp_gp_and_vp_gp_y.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/whitening/test_warp_gp_and_vp_vp_K.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/whitening/test_warp_gp_and_vp_vp_lambda.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/whitening/test_warp_gp_and_vp_vp_mu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/whitening/test_warp_gp_and_vp_vp_sigma.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/whitening/test_warp_gp_and_vp_vp_w.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/whitening/test_warp_input_R_mat.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/whitening/test_warp_input_rands.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/whitening/test_warp_input_scale.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/testing/whitening/vp_initialized_MATLAB.mat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.182777 PyVBMC-1.0.1/pyvbmc/timer/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/timer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/timer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/timer/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.186777 PyVBMC-1.0.1/pyvbmc/variational_posterior/
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/variational_posterior/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/variational_posterior/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50594 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/variational_posterior/variational_posterior.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.186777 PyVBMC-1.0.1/pyvbmc/vbmc/
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/vbmc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/vbmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17357 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/vbmc/active_importance_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32466 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/vbmc/active_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/vbmc/create_vbmc_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27532 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/vbmc/gaussian_process_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/vbmc/iteration_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/vbmc/minimize_adam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.186777 PyVBMC-1.0.1/pyvbmc/vbmc/option_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)    13895 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/vbmc/option_configs/advanced_vbmc_options.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/vbmc/option_configs/basic_vbmc_options.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/vbmc/option_configs/test_options.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/vbmc/option_configs/test_options2.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    11576 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/vbmc/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52699 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/vbmc/variational_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100005 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/vbmc/vbmc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:36:28.186777 PyVBMC-1.0.1/pyvbmc/whitening/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/whitening/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/whitening/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13121 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/pyvbmc/whitening/whitening.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 08:36:28.186777 PyVBMC-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-24 08:36:13.000000 PyVBMC-1.0.1/setup.py
```

### Comparing `PyVBMC-1.0.0/.github/workflows/docs.yml` & `PyVBMC-1.0.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/.github/workflows/merge-tests.yml` & `PyVBMC-1.0.1/.github/workflows/merge-tests.yml`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/.github/workflows/release.yml` & `PyVBMC-1.0.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/.github/workflows/tests.yml` & `PyVBMC-1.0.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/.gitignore` & `PyVBMC-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/.pre-commit-config.yaml` & `PyVBMC-1.0.1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.1.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
         exclude: ^docs/
       - id: end-of-file-fixer
         exclude_types: [json, binary]
         exclude: ^docs/
   - repo: https://github.com/PyCQA/isort
-    rev: "5.10.1"
+    rev: "5.12.0"
     hooks:
       - id: isort
         additional_dependencies: [toml]
         exclude: docs/tutorials
   - repo: https://github.com/psf/black
-    rev: "22.3.0"
+    rev: "23.3.0"
     hooks:
       - id: black-jupyter
   - repo: https://github.com/hadialqattan/pycln
-    rev: "v1.2.5"
+    rev: "v2.1.3"
     hooks:
       - id: pycln
```

### Comparing `PyVBMC-1.0.0/LICENSE` & `PyVBMC-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/PKG-INFO` & `PyVBMC-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyVBMC
-Version: 1.0.0
+Version: 1.0.1
 Summary: Variational Bayesian Monte Carlo in Python.
 License: BSD 3-Clause License
         
         Copyright (c) 2021, PyVBMC Developers and their Assignees
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -115,15 +115,15 @@
 ```python
 from pyvbmc import VBMC
 # ... define your model/target density here
 vbmc = VBMC(target, x0, LB, UB, PLB, PUB)
 vp, results = vbmc.optimize()
 ```
 with input arguments:
-- `target`: the target (unnormalized) log density — often an unnormalized log posterior. `target` is a callable that should take as input a parameter vector and return the log density at the point;
+- `target`: the target (unnormalized) log density — often an unnormalized log posterior. `target` is a callable that should take as input a parameter vector and return the log density at the point. The returned log density must return a *finite* real value, i.e. non `NaN` or `-inf`. See the [VBMC FAQ](https://github.com/acerbilab/vbmc/wiki#how-do-i-prevent-vbmc-from-evaluating-certain-inputs-or-regions-of-input-space) for more details;
 - `x0`: an array representing the starting point of the inference in parameter space;
 - `LB` and `UB`: arrays of hard lower (resp. upper) bounds constraining the parameters (possibly `-/+np.inf` for unbounded parameters);
 - `PLB` and `PUB`: arrays of plausible lower (resp. upper) bounds: that is, a box that ideally brackets a high posterior density region of the target.
 
 The outputs are:
 - `vp`: a `VariationalPosterior` object which approximates the true target density;
 - `results`: a `dict` containing additional information. Important keys are:
@@ -170,37 +170,47 @@
 If you have trouble doing something with PyVBMC, spot bugs or strange behavior, or you simply have some questions, please feel free to:
 - Post in the lab's [Discussions forum](https://github.com/orgs/acerbilab/discussions) with questions or comments about PyVBMC, your problems & applications;
 - [Open an issue](https://github.com/acerbilab/pyvbmc/issues/new) on GitHub;
 - Contact the project lead at <luigi.acerbi@helsinki.fi>, putting 'PyVBMC' in the subject of the email.
 
 ## References and citation
 
-1. Acerbi, L. (2018). Variational Bayesian Monte Carlo. In *Advances in Neural Information Processing Systems 31*: 8222-8232. ([paper + supplement on arXiv](https://arxiv.org/abs/1810.05558), [NeurIPS Proceedings](https://papers.nips.cc/paper/8043-variational-bayesian-monte-carlo))
-2. Acerbi, L. (2020). Variational Bayesian Monte Carlo with Noisy Likelihoods. In *Advances in Neural Information Processing Systems 33*: 8211-8222 ([paper + supplement on arXiv](https://arxiv.org/abs/2006.08655), [NeurIPS Proceedings](https://papers.nips.cc/paper/2020/hash/5d40954183d62a82257835477ccad3d2-Abstract.html)).
+1. Huggins, B., Li, C., Tobaben, M., Aarnos, M., & Acerbi, L. (2023). *PyVBMC: Efficient Bayesian inference in Python*. arXiv. https://arxiv.org/abs/2303.09519
+2. Acerbi, L. (2018). Variational Bayesian Monte Carlo. In *Advances in Neural Information Processing Systems 31*: 8222-8232. ([paper + supplement on arXiv](https://arxiv.org/abs/1810.05558), [NeurIPS Proceedings](https://papers.nips.cc/paper/8043-variational-bayesian-monte-carlo))
+3. Acerbi, L. (2020). Variational Bayesian Monte Carlo with Noisy Likelihoods. In *Advances in Neural Information Processing Systems 33*: 8211-8222 ([paper + supplement on arXiv](https://arxiv.org/abs/2006.08655), [NeurIPS Proceedings](https://papers.nips.cc/paper/2020/hash/5d40954183d62a82257835477ccad3d2-Abstract.html)).
 
-Please cite both references if you use PyVBMC in your work (the 2018 paper introduced the framework, and the 2020 paper includes a number of major improvements, including but not limited to support for noisy likelihoods). You can cite PyVBMC in your work with something along the lines of
+Please cite all three references if you use PyVBMC in your work (the 2018 paper introduced the framework, and the 2020 paper includes a number of major improvements, including but not limited to support for noisy likelihoods). You can cite PyVBMC in your work with something along the lines of
 
-> We estimated approximate posterior distibutions and approximate lower bounds to the model evidence of our models using Variational Bayesian Monte Carlo (PyVBMC; Acerbi, 2018, 2020). PyVBMC combines variational inference and active-sampling Bayesian quadrature to perform approximate Bayesian inference in a sample-efficient manner.
+> We estimated approximate posterior distibutions and approximate lower bounds to the model evidence of our models using Variational Bayesian Monte Carlo (PyVBMC; Acerbi, 2018, 2020) via the PyVBMC software (Huggins et al., 2023). PyVBMC combines variational inference and active-sampling Bayesian quadrature to perform approximate Bayesian inference in a sample-efficient manner.
 
 Besides formal citations, you can demonstrate your appreciation for PyVBMC in the following ways:
 
 - *Star :star:* the VBMC repository on GitHub;
 - [Subscribe](http://eepurl.com/idcvc9) to the lab's newsletter for news and updates (new features, bug fixes, new releases, etc.);
 - [Follow Luigi Acerbi on Twitter](https://twitter.com/AcerbiLuigi) for updates about VBMC/PyVBMC and other projects;
 - Tell us about your model-fitting problem and your experience with PyVBMC (positive or negative) in the lab's [Discussions forum](https://github.com/orgs/acerbilab/discussions).
 
 You may also want to check out [Bayesian Adaptive Direct Search in Python (PyBADS)](https://github.com/acerbilab/pybads), our companion method for fast Bayesian optimization.
 
 ### Additional references
 
-3. Acerbi, L. (2019). An Exploration of Acquisition and Mean Functions in Variational Bayesian Monte Carlo. In *Proc. Machine Learning Research* 96: 1-10. 1st Symposium on Advances in Approximate Bayesian Inference, Montréal, Canada. ([paper in PMLR](http://proceedings.mlr.press/v96/acerbi19a.html))
+4. Acerbi, L. (2019). An Exploration of Acquisition and Mean Functions in Variational Bayesian Monte Carlo. In *Proc. Machine Learning Research* 96: 1-10. 1st Symposium on Advances in Approximate Bayesian Inference, Montréal, Canada. ([paper in PMLR](http://proceedings.mlr.press/v96/acerbi19a.html))
 
 ### BibTeX
 
 ```BibTeX
+@article{huggins2023pyvbmc,
+  title = {PyVBMC: Efficient Bayesian inference in Python},
+  author = {Huggins, Bobby and Li, Chengkun and Tobaben, Marlon and Aarnos, Mikko J. and Acerbi, Luigi},
+  publisher = {preprint},
+  journal = {{arXiv}},
+  url = {https://arxiv.org/abs/2303.09519},
+  doi = {10.48550/ARXIV.2303.09519},
+  year = {2023},
+}
 @article{acerbi2018variational,
   title={{V}ariational {B}ayesian {M}onte {C}arlo},
   author={Acerbi, Luigi},
   journal={Advances in Neural Information Processing Systems},
   volume={31},
   pages={8222--8232},
   year={2018}
```

### Comparing `PyVBMC-1.0.0/PyVBMC.egg-info/PKG-INFO` & `PyVBMC-1.0.1/PyVBMC.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyVBMC
-Version: 1.0.0
+Version: 1.0.1
 Summary: Variational Bayesian Monte Carlo in Python.
 License: BSD 3-Clause License
         
         Copyright (c) 2021, PyVBMC Developers and their Assignees
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -115,15 +115,15 @@
 ```python
 from pyvbmc import VBMC
 # ... define your model/target density here
 vbmc = VBMC(target, x0, LB, UB, PLB, PUB)
 vp, results = vbmc.optimize()
 ```
 with input arguments:
-- `target`: the target (unnormalized) log density — often an unnormalized log posterior. `target` is a callable that should take as input a parameter vector and return the log density at the point;
+- `target`: the target (unnormalized) log density — often an unnormalized log posterior. `target` is a callable that should take as input a parameter vector and return the log density at the point. The returned log density must return a *finite* real value, i.e. non `NaN` or `-inf`. See the [VBMC FAQ](https://github.com/acerbilab/vbmc/wiki#how-do-i-prevent-vbmc-from-evaluating-certain-inputs-or-regions-of-input-space) for more details;
 - `x0`: an array representing the starting point of the inference in parameter space;
 - `LB` and `UB`: arrays of hard lower (resp. upper) bounds constraining the parameters (possibly `-/+np.inf` for unbounded parameters);
 - `PLB` and `PUB`: arrays of plausible lower (resp. upper) bounds: that is, a box that ideally brackets a high posterior density region of the target.
 
 The outputs are:
 - `vp`: a `VariationalPosterior` object which approximates the true target density;
 - `results`: a `dict` containing additional information. Important keys are:
@@ -170,37 +170,47 @@
 If you have trouble doing something with PyVBMC, spot bugs or strange behavior, or you simply have some questions, please feel free to:
 - Post in the lab's [Discussions forum](https://github.com/orgs/acerbilab/discussions) with questions or comments about PyVBMC, your problems & applications;
 - [Open an issue](https://github.com/acerbilab/pyvbmc/issues/new) on GitHub;
 - Contact the project lead at <luigi.acerbi@helsinki.fi>, putting 'PyVBMC' in the subject of the email.
 
 ## References and citation
 
-1. Acerbi, L. (2018). Variational Bayesian Monte Carlo. In *Advances in Neural Information Processing Systems 31*: 8222-8232. ([paper + supplement on arXiv](https://arxiv.org/abs/1810.05558), [NeurIPS Proceedings](https://papers.nips.cc/paper/8043-variational-bayesian-monte-carlo))
-2. Acerbi, L. (2020). Variational Bayesian Monte Carlo with Noisy Likelihoods. In *Advances in Neural Information Processing Systems 33*: 8211-8222 ([paper + supplement on arXiv](https://arxiv.org/abs/2006.08655), [NeurIPS Proceedings](https://papers.nips.cc/paper/2020/hash/5d40954183d62a82257835477ccad3d2-Abstract.html)).
+1. Huggins, B., Li, C., Tobaben, M., Aarnos, M., & Acerbi, L. (2023). *PyVBMC: Efficient Bayesian inference in Python*. arXiv. https://arxiv.org/abs/2303.09519
+2. Acerbi, L. (2018). Variational Bayesian Monte Carlo. In *Advances in Neural Information Processing Systems 31*: 8222-8232. ([paper + supplement on arXiv](https://arxiv.org/abs/1810.05558), [NeurIPS Proceedings](https://papers.nips.cc/paper/8043-variational-bayesian-monte-carlo))
+3. Acerbi, L. (2020). Variational Bayesian Monte Carlo with Noisy Likelihoods. In *Advances in Neural Information Processing Systems 33*: 8211-8222 ([paper + supplement on arXiv](https://arxiv.org/abs/2006.08655), [NeurIPS Proceedings](https://papers.nips.cc/paper/2020/hash/5d40954183d62a82257835477ccad3d2-Abstract.html)).
 
-Please cite both references if you use PyVBMC in your work (the 2018 paper introduced the framework, and the 2020 paper includes a number of major improvements, including but not limited to support for noisy likelihoods). You can cite PyVBMC in your work with something along the lines of
+Please cite all three references if you use PyVBMC in your work (the 2018 paper introduced the framework, and the 2020 paper includes a number of major improvements, including but not limited to support for noisy likelihoods). You can cite PyVBMC in your work with something along the lines of
 
-> We estimated approximate posterior distibutions and approximate lower bounds to the model evidence of our models using Variational Bayesian Monte Carlo (PyVBMC; Acerbi, 2018, 2020). PyVBMC combines variational inference and active-sampling Bayesian quadrature to perform approximate Bayesian inference in a sample-efficient manner.
+> We estimated approximate posterior distibutions and approximate lower bounds to the model evidence of our models using Variational Bayesian Monte Carlo (PyVBMC; Acerbi, 2018, 2020) via the PyVBMC software (Huggins et al., 2023). PyVBMC combines variational inference and active-sampling Bayesian quadrature to perform approximate Bayesian inference in a sample-efficient manner.
 
 Besides formal citations, you can demonstrate your appreciation for PyVBMC in the following ways:
 
 - *Star :star:* the VBMC repository on GitHub;
 - [Subscribe](http://eepurl.com/idcvc9) to the lab's newsletter for news and updates (new features, bug fixes, new releases, etc.);
 - [Follow Luigi Acerbi on Twitter](https://twitter.com/AcerbiLuigi) for updates about VBMC/PyVBMC and other projects;
 - Tell us about your model-fitting problem and your experience with PyVBMC (positive or negative) in the lab's [Discussions forum](https://github.com/orgs/acerbilab/discussions).
 
 You may also want to check out [Bayesian Adaptive Direct Search in Python (PyBADS)](https://github.com/acerbilab/pybads), our companion method for fast Bayesian optimization.
 
 ### Additional references
 
-3. Acerbi, L. (2019). An Exploration of Acquisition and Mean Functions in Variational Bayesian Monte Carlo. In *Proc. Machine Learning Research* 96: 1-10. 1st Symposium on Advances in Approximate Bayesian Inference, Montréal, Canada. ([paper in PMLR](http://proceedings.mlr.press/v96/acerbi19a.html))
+4. Acerbi, L. (2019). An Exploration of Acquisition and Mean Functions in Variational Bayesian Monte Carlo. In *Proc. Machine Learning Research* 96: 1-10. 1st Symposium on Advances in Approximate Bayesian Inference, Montréal, Canada. ([paper in PMLR](http://proceedings.mlr.press/v96/acerbi19a.html))
 
 ### BibTeX
 
 ```BibTeX
+@article{huggins2023pyvbmc,
+  title = {PyVBMC: Efficient Bayesian inference in Python},
+  author = {Huggins, Bobby and Li, Chengkun and Tobaben, Marlon and Aarnos, Mikko J. and Acerbi, Luigi},
+  publisher = {preprint},
+  journal = {{arXiv}},
+  url = {https://arxiv.org/abs/2303.09519},
+  doi = {10.48550/ARXIV.2303.09519},
+  year = {2023},
+}
 @article{acerbi2018variational,
   title={{V}ariational {B}ayesian {M}onte {C}arlo},
   author={Acerbi, Luigi},
   journal={Advances in Neural Information Processing Systems},
   volume={31},
   pages={8222--8232},
   year={2018}
```

### Comparing `PyVBMC-1.0.0/PyVBMC.egg-info/SOURCES.txt` & `PyVBMC-1.0.1/PyVBMC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/README.md` & `PyVBMC-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 ```python
 from pyvbmc import VBMC
 # ... define your model/target density here
 vbmc = VBMC(target, x0, LB, UB, PLB, PUB)
 vp, results = vbmc.optimize()
 ```
 with input arguments:
-- `target`: the target (unnormalized) log density — often an unnormalized log posterior. `target` is a callable that should take as input a parameter vector and return the log density at the point;
+- `target`: the target (unnormalized) log density — often an unnormalized log posterior. `target` is a callable that should take as input a parameter vector and return the log density at the point. The returned log density must return a *finite* real value, i.e. non `NaN` or `-inf`. See the [VBMC FAQ](https://github.com/acerbilab/vbmc/wiki#how-do-i-prevent-vbmc-from-evaluating-certain-inputs-or-regions-of-input-space) for more details;
 - `x0`: an array representing the starting point of the inference in parameter space;
 - `LB` and `UB`: arrays of hard lower (resp. upper) bounds constraining the parameters (possibly `-/+np.inf` for unbounded parameters);
 - `PLB` and `PUB`: arrays of plausible lower (resp. upper) bounds: that is, a box that ideally brackets a high posterior density region of the target.
 
 The outputs are:
 - `vp`: a `VariationalPosterior` object which approximates the true target density;
 - `results`: a `dict` containing additional information. Important keys are:
@@ -131,37 +131,47 @@
 If you have trouble doing something with PyVBMC, spot bugs or strange behavior, or you simply have some questions, please feel free to:
 - Post in the lab's [Discussions forum](https://github.com/orgs/acerbilab/discussions) with questions or comments about PyVBMC, your problems & applications;
 - [Open an issue](https://github.com/acerbilab/pyvbmc/issues/new) on GitHub;
 - Contact the project lead at <luigi.acerbi@helsinki.fi>, putting 'PyVBMC' in the subject of the email.
 
 ## References and citation
 
-1. Acerbi, L. (2018). Variational Bayesian Monte Carlo. In *Advances in Neural Information Processing Systems 31*: 8222-8232. ([paper + supplement on arXiv](https://arxiv.org/abs/1810.05558), [NeurIPS Proceedings](https://papers.nips.cc/paper/8043-variational-bayesian-monte-carlo))
-2. Acerbi, L. (2020). Variational Bayesian Monte Carlo with Noisy Likelihoods. In *Advances in Neural Information Processing Systems 33*: 8211-8222 ([paper + supplement on arXiv](https://arxiv.org/abs/2006.08655), [NeurIPS Proceedings](https://papers.nips.cc/paper/2020/hash/5d40954183d62a82257835477ccad3d2-Abstract.html)).
+1. Huggins, B., Li, C., Tobaben, M., Aarnos, M., & Acerbi, L. (2023). *PyVBMC: Efficient Bayesian inference in Python*. arXiv. https://arxiv.org/abs/2303.09519
+2. Acerbi, L. (2018). Variational Bayesian Monte Carlo. In *Advances in Neural Information Processing Systems 31*: 8222-8232. ([paper + supplement on arXiv](https://arxiv.org/abs/1810.05558), [NeurIPS Proceedings](https://papers.nips.cc/paper/8043-variational-bayesian-monte-carlo))
+3. Acerbi, L. (2020). Variational Bayesian Monte Carlo with Noisy Likelihoods. In *Advances in Neural Information Processing Systems 33*: 8211-8222 ([paper + supplement on arXiv](https://arxiv.org/abs/2006.08655), [NeurIPS Proceedings](https://papers.nips.cc/paper/2020/hash/5d40954183d62a82257835477ccad3d2-Abstract.html)).
 
-Please cite both references if you use PyVBMC in your work (the 2018 paper introduced the framework, and the 2020 paper includes a number of major improvements, including but not limited to support for noisy likelihoods). You can cite PyVBMC in your work with something along the lines of
+Please cite all three references if you use PyVBMC in your work (the 2018 paper introduced the framework, and the 2020 paper includes a number of major improvements, including but not limited to support for noisy likelihoods). You can cite PyVBMC in your work with something along the lines of
 
-> We estimated approximate posterior distibutions and approximate lower bounds to the model evidence of our models using Variational Bayesian Monte Carlo (PyVBMC; Acerbi, 2018, 2020). PyVBMC combines variational inference and active-sampling Bayesian quadrature to perform approximate Bayesian inference in a sample-efficient manner.
+> We estimated approximate posterior distibutions and approximate lower bounds to the model evidence of our models using Variational Bayesian Monte Carlo (PyVBMC; Acerbi, 2018, 2020) via the PyVBMC software (Huggins et al., 2023). PyVBMC combines variational inference and active-sampling Bayesian quadrature to perform approximate Bayesian inference in a sample-efficient manner.
 
 Besides formal citations, you can demonstrate your appreciation for PyVBMC in the following ways:
 
 - *Star :star:* the VBMC repository on GitHub;
 - [Subscribe](http://eepurl.com/idcvc9) to the lab's newsletter for news and updates (new features, bug fixes, new releases, etc.);
 - [Follow Luigi Acerbi on Twitter](https://twitter.com/AcerbiLuigi) for updates about VBMC/PyVBMC and other projects;
 - Tell us about your model-fitting problem and your experience with PyVBMC (positive or negative) in the lab's [Discussions forum](https://github.com/orgs/acerbilab/discussions).
 
 You may also want to check out [Bayesian Adaptive Direct Search in Python (PyBADS)](https://github.com/acerbilab/pybads), our companion method for fast Bayesian optimization.
 
 ### Additional references
 
-3. Acerbi, L. (2019). An Exploration of Acquisition and Mean Functions in Variational Bayesian Monte Carlo. In *Proc. Machine Learning Research* 96: 1-10. 1st Symposium on Advances in Approximate Bayesian Inference, Montréal, Canada. ([paper in PMLR](http://proceedings.mlr.press/v96/acerbi19a.html))
+4. Acerbi, L. (2019). An Exploration of Acquisition and Mean Functions in Variational Bayesian Monte Carlo. In *Proc. Machine Learning Research* 96: 1-10. 1st Symposium on Advances in Approximate Bayesian Inference, Montréal, Canada. ([paper in PMLR](http://proceedings.mlr.press/v96/acerbi19a.html))
 
 ### BibTeX
 
 ```BibTeX
+@article{huggins2023pyvbmc,
+  title = {PyVBMC: Efficient Bayesian inference in Python},
+  author = {Huggins, Bobby and Li, Chengkun and Tobaben, Marlon and Aarnos, Mikko J. and Acerbi, Luigi},
+  publisher = {preprint},
+  journal = {{arXiv}},
+  url = {https://arxiv.org/abs/2303.09519},
+  doi = {10.48550/ARXIV.2303.09519},
+  year = {2023},
+}
 @article{acerbi2018variational,
   title={{V}ariational {B}ayesian {M}onte {C}arlo},
   author={Acerbi, Luigi},
   journal={Advances in Neural Information Processing Systems},
   volume={31},
   pages={8222--8232},
   year={2018}
```

### Comparing `PyVBMC-1.0.0/examples/pyvbmc_example_1_basic_usage.ipynb` & `PyVBMC-1.0.1/examples/pyvbmc_example_1_basic_usage.ipynb`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/examples/pyvbmc_example_2_inputs_outputs.ipynb` & `PyVBMC-1.0.1/examples/pyvbmc_example_2_inputs_outputs.ipynb`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/examples/pyvbmc_example_3_diagnostics_and_saving.ipynb` & `PyVBMC-1.0.1/examples/pyvbmc_example_3_diagnostics_and_saving.ipynb`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/examples/pyvbmc_example_4_validation.ipynb` & `PyVBMC-1.0.1/examples/pyvbmc_example_4_validation.ipynb`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/examples/pyvbmc_example_5_prior_distributions.ipynb` & `PyVBMC-1.0.1/examples/pyvbmc_example_5_prior_distributions.ipynb`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/examples/pyvbmc_example_6_noisy_likelihoods.ipynb` & `PyVBMC-1.0.1/examples/pyvbmc_example_6_noisy_likelihoods.ipynb`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/examples/scripts/Makefile` & `PyVBMC-1.0.1/examples/scripts/Makefile`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/examples/scripts/pyvbmc_example_1_full_code.py` & `PyVBMC-1.0.1/examples/scripts/pyvbmc_example_1_full_code.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/examples/scripts/pyvbmc_example_2_full_code.py` & `PyVBMC-1.0.1/examples/scripts/pyvbmc_example_2_full_code.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/examples/scripts/pyvbmc_example_3_full_code.py` & `PyVBMC-1.0.1/examples/scripts/pyvbmc_example_3_full_code.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/examples/scripts/pyvbmc_example_4_full_code.py` & `PyVBMC-1.0.1/examples/scripts/pyvbmc_example_4_full_code.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/examples/scripts/pyvbmc_example_5_full_code.py` & `PyVBMC-1.0.1/examples/scripts/pyvbmc_example_5_full_code.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/examples/scripts/pyvbmc_example_6_full_code.py` & `PyVBMC-1.0.1/examples/scripts/pyvbmc_example_6_full_code.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/logo.svg` & `PyVBMC-1.0.1/logo.svg`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pylintrc` & `PyVBMC-1.0.1/pylintrc`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyproject.toml` & `PyVBMC-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/__main__.py` & `PyVBMC-1.0.1/pyvbmc/__main__.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/acquisition_functions/README.md` & `PyVBMC-1.0.1/pyvbmc/acquisition_functions/README.md`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/acquisition_functions/abstract_acq_fcn.py` & `PyVBMC-1.0.1/pyvbmc/acquisition_functions/abstract_acq_fcn.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/acquisition_functions/acq_fcn.py` & `PyVBMC-1.0.1/pyvbmc/acquisition_functions/acq_fcn.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/acquisition_functions/acq_fcn_imiqr.py` & `PyVBMC-1.0.1/pyvbmc/acquisition_functions/acq_fcn_imiqr.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/acquisition_functions/acq_fcn_log.py` & `PyVBMC-1.0.1/pyvbmc/acquisition_functions/acq_fcn_log.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/acquisition_functions/acq_fcn_noisy.py` & `PyVBMC-1.0.1/pyvbmc/acquisition_functions/acq_fcn_noisy.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/acquisition_functions/acq_fcn_vanilla.py` & `PyVBMC-1.0.1/pyvbmc/acquisition_functions/acq_fcn_vanilla.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/acquisition_functions/acq_fcn_viqr.py` & `PyVBMC-1.0.1/pyvbmc/acquisition_functions/acq_fcn_viqr.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/acquisition_functions/utilities.py` & `PyVBMC-1.0.1/pyvbmc/acquisition_functions/utilities.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/decorators/README.md` & `PyVBMC-1.0.1/pyvbmc/decorators/README.md`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/decorators/handle_0D_1D_input.py` & `PyVBMC-1.0.1/pyvbmc/decorators/handle_0D_1D_input.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/entropy/entlb_vbmc.py` & `PyVBMC-1.0.1/pyvbmc/entropy/entlb_vbmc.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/entropy/entmc_vbmc.py` & `PyVBMC-1.0.1/pyvbmc/entropy/entmc_vbmc.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/formatting/formatting.py` & `PyVBMC-1.0.1/pyvbmc/formatting/formatting.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/function_logger/function_logger.py` & `PyVBMC-1.0.1/pyvbmc/function_logger/function_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         timer.stop_timer("fun_time")
 
         # if f_val is an array with only one element, extract that element
         if not np.isscalar(f_val_orig) and np.size(f_val_orig) == 1:
             f_val_orig = np.array(f_val_orig).flat[0]
 
         # Check function value
-        if np.any(
+        if (
             not np.isscalar(f_val_orig)
             or not np.isfinite(f_val_orig)
             or not np.isreal(f_val_orig)
         ):
             error_message = """FunctionLogger:InvalidFuncValue:
             The returned function value must be a finite real-valued scalar
             (returned value {})"""
```

### Comparing `PyVBMC-1.0.0/pyvbmc/parameter_transformer/parameter_transformer.py` & `PyVBMC-1.0.1/pyvbmc/parameter_transformer/parameter_transformer.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/priors/convert_to_prior.py` & `PyVBMC-1.0.1/pyvbmc/priors/convert_to_prior.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/priors/prior.py` & `PyVBMC-1.0.1/pyvbmc/priors/prior.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/priors/product.py` & `PyVBMC-1.0.1/pyvbmc/priors/product.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/priors/scipy.py` & `PyVBMC-1.0.1/pyvbmc/priors/scipy.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/priors/smooth_box.py` & `PyVBMC-1.0.1/pyvbmc/priors/smooth_box.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/priors/spline_trapezoidal.py` & `PyVBMC-1.0.1/pyvbmc/priors/spline_trapezoidal.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/priors/tile_inputs.py` & `PyVBMC-1.0.1/pyvbmc/priors/tile_inputs.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/priors/trapezoidal.py` & `PyVBMC-1.0.1/pyvbmc/priors/trapezoidal.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/priors/uniform_box.py` & `PyVBMC-1.0.1/pyvbmc/priors/uniform_box.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/priors/user_function.py` & `PyVBMC-1.0.1/pyvbmc/priors/user_function.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/stats/README.md` & `PyVBMC-1.0.1/pyvbmc/stats/README.md`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/stats/get_hpd.py` & `PyVBMC-1.0.1/pyvbmc/stats/get_hpd.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/stats/kde_1d.py` & `PyVBMC-1.0.1/pyvbmc/stats/kde_1d.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/stats/kl_div_mvn.py` & `PyVBMC-1.0.1/pyvbmc/stats/kl_div_mvn.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/_check_grad.py` & `PyVBMC-1.0.1/pyvbmc/testing/_check_grad.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/_compare_matlab.py` & `PyVBMC-1.0.1/pyvbmc/testing/_compare_matlab.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/acquisition_functions/test_abstract_acquisition_function.py` & `PyVBMC-1.0.1/pyvbmc/testing/acquisition_functions/test_abstract_acquisition_function.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/acquisition_functions/test_acq_fcn.py` & `PyVBMC-1.0.1/pyvbmc/testing/acquisition_functions/test_acq_fcn.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/acquisition_functions/test_acq_fcn_imiqr.py` & `PyVBMC-1.0.1/pyvbmc/testing/acquisition_functions/test_acq_fcn_imiqr.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/acquisition_functions/test_acq_fcn_log.py` & `PyVBMC-1.0.1/pyvbmc/testing/acquisition_functions/test_acq_fcn_log.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/acquisition_functions/test_acq_fcn_noisy.py` & `PyVBMC-1.0.1/pyvbmc/testing/acquisition_functions/test_acq_fcn_noisy.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/acquisition_functions/test_acq_fcn_vanilla.py` & `PyVBMC-1.0.1/pyvbmc/testing/acquisition_functions/test_acq_fcn_vanilla.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/acquisition_functions/test_acq_fcn_viqr.py` & `PyVBMC-1.0.1/pyvbmc/testing/acquisition_functions/test_acq_fcn_viqr.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/decorators/test_handle_0D_1D_input_decorator.py` & `PyVBMC-1.0.1/pyvbmc/testing/decorators/test_handle_0D_1D_input_decorator.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/entropy/entropy-test.mat` & `PyVBMC-1.0.1/pyvbmc/testing/entropy/entropy-test.mat`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/entropy/test_entlb_vbmc.py` & `PyVBMC-1.0.1/pyvbmc/testing/entropy/test_entlb_vbmc.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/entropy/test_entmc_vbmc.py` & `PyVBMC-1.0.1/pyvbmc/testing/entropy/test_entmc_vbmc.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/function_logger/test_function_logger.py` & `PyVBMC-1.0.1/pyvbmc/testing/function_logger/test_function_logger.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/parameter_transformer/test_parameter_transformer.py` & `PyVBMC-1.0.1/pyvbmc/testing/parameter_transformer/test_parameter_transformer.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/priors/test_convert_to_prior.py` & `PyVBMC-1.0.1/pyvbmc/testing/priors/test_convert_to_prior.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/priors/test_priors.py` & `PyVBMC-1.0.1/pyvbmc/testing/priors/test_priors.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/priors/test_product_prior.py` & `PyVBMC-1.0.1/pyvbmc/testing/priors/test_product_prior.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/priors/test_scipy_prior.py` & `PyVBMC-1.0.1/pyvbmc/testing/priors/test_scipy_prior.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/priors/test_smooth_box_prior.py` & `PyVBMC-1.0.1/pyvbmc/testing/priors/test_smooth_box_prior.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/priors/test_spline_trapezoid_prior.py` & `PyVBMC-1.0.1/pyvbmc/testing/priors/test_spline_trapezoid_prior.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/priors/test_tile_inputs.py` & `PyVBMC-1.0.1/pyvbmc/testing/priors/test_tile_inputs.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/priors/test_trapezoid_prior.py` & `PyVBMC-1.0.1/pyvbmc/testing/priors/test_trapezoid_prior.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/priors/test_uniform_box_prior.py` & `PyVBMC-1.0.1/pyvbmc/testing/priors/test_uniform_box_prior.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/priors/test_user_function_prior.py` & `PyVBMC-1.0.1/pyvbmc/testing/priors/test_user_function_prior.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/stats/test_get_hpd.py` & `PyVBMC-1.0.1/pyvbmc/testing/stats/test_get_hpd.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/stats/test_kde1d.py` & `PyVBMC-1.0.1/pyvbmc/testing/stats/test_kde1d.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/stats/test_kldiv_mvn.py` & `PyVBMC-1.0.1/pyvbmc/testing/stats/test_kldiv_mvn.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/timer/test_timer.py` & `PyVBMC-1.0.1/pyvbmc/testing/timer/test_timer.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/variational_posterior/test_variational_posterior.py` & `PyVBMC-1.0.1/pyvbmc/testing/variational_posterior/test_variational_posterior.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/variational_posterior/test_vp_save_and_load.py` & `PyVBMC-1.0.1/pyvbmc/testing/variational_posterior/test_vp_save_and_load.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/variational_posterior/test_vp_save_static.pkl` & `PyVBMC-1.0.1/pyvbmc/testing/variational_posterior/test_vp_save_static.pkl`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/variational_posterior/vp-test.mat` & `PyVBMC-1.0.1/pyvbmc/testing/variational_posterior/vp-test.mat`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/vbmc/compare_MATLAB/activesample_proposalpdf.m` & `PyVBMC-1.0.1/pyvbmc/testing/vbmc/compare_MATLAB/activesample_proposalpdf.m`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/vbmc/compare_MATLAB/fess.m` & `PyVBMC-1.0.1/pyvbmc/testing/vbmc/compare_MATLAB/fess.m`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/vbmc/compare_MATLAB/log_isbasefun.m` & `PyVBMC-1.0.1/pyvbmc/testing/vbmc/compare_MATLAB/log_isbasefun.m`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/vbmc/hyp.txt` & `PyVBMC-1.0.1/pyvbmc/testing/vbmc/hyp.txt`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_active_importance_sampling.py` & `PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_active_importance_sampling.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_gaussian_process_train.py` & `PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_gaussian_process_train.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_iteration_history.py` & `PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_iteration_history.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_minimize_adam.py` & `PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_minimize_adam.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_options.py` & `PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_options.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_variational_optimization.py` & `PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_variational_optimization.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_vbmc_active_sample.py` & `PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_vbmc_active_sample.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_vbmc_determine_best_vp.py` & `PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_vbmc_determine_best_vp.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_vbmc_finalboost.py` & `PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_vbmc_finalboost.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_vbmc_init.py` & `PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_vbmc_init.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_vbmc_loop_termination.py` & `PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_vbmc_loop_termination.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_vbmc_optimize.py` & `PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_vbmc_optimize.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_vbmc_save_and_load.py` & `PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_vbmc_save_and_load.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/vbmc/test_vbmc_save_static.pkl` & `PyVBMC-1.0.1/pyvbmc/testing/vbmc/test_vbmc_save_static.pkl`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/whitening/test_rotoscaling.py` & `PyVBMC-1.0.1/pyvbmc/testing/whitening/test_rotoscaling.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/whitening/test_warp_gp_and_vp_gp_X.txt` & `PyVBMC-1.0.1/pyvbmc/testing/whitening/test_warp_gp_and_vp_gp_X.txt`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/whitening/test_warp_gp_and_vp_gp_y.txt` & `PyVBMC-1.0.1/pyvbmc/testing/whitening/test_warp_gp_and_vp_gp_y.txt`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/whitening/test_warp_gp_and_vp_vp_mu.txt` & `PyVBMC-1.0.1/pyvbmc/testing/whitening/test_warp_gp_and_vp_vp_mu.txt`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/whitening/test_warp_gp_and_vp_vp_sigma.txt` & `PyVBMC-1.0.1/pyvbmc/testing/whitening/test_warp_gp_and_vp_vp_sigma.txt`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/whitening/test_warp_input_rands.txt` & `PyVBMC-1.0.1/pyvbmc/testing/whitening/test_warp_input_rands.txt`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/testing/whitening/vp_initialized_MATLAB.mat` & `PyVBMC-1.0.1/pyvbmc/testing/whitening/vp_initialized_MATLAB.mat`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/timer/timer.py` & `PyVBMC-1.0.1/pyvbmc/timer/timer.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/variational_posterior/README.md` & `PyVBMC-1.0.1/pyvbmc/variational_posterior/README.md`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/variational_posterior/variational_posterior.py` & `PyVBMC-1.0.1/pyvbmc/variational_posterior/variational_posterior.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/vbmc/README.md` & `PyVBMC-1.0.1/pyvbmc/vbmc/README.md`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/vbmc/active_importance_sampling.py` & `PyVBMC-1.0.1/pyvbmc/vbmc/active_importance_sampling.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/vbmc/active_sample.py` & `PyVBMC-1.0.1/pyvbmc/vbmc/active_sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import math
 
 import cma
 import gpyreg as gpr
 import numpy as np
 
 from pyvbmc.acquisition_functions import AbstractAcqFcn
+from pyvbmc.acquisition_functions.utilities import string_to_acq
 from pyvbmc.function_logger import FunctionLogger
 from pyvbmc.stats import get_hpd
 from pyvbmc.timer import main_timer as timer
 from pyvbmc.variational_posterior import VariationalPosterior
 from pyvbmc.vbmc.active_importance_sampling import active_importance_sampling
 from pyvbmc.vbmc.gaussian_process_train import reupdate_gp, train_gp
 from pyvbmc.vbmc.iteration_history import IterationHistory
@@ -267,15 +268,14 @@
             Ns_gp = np.size(gp.posteriors)
             sn2new = np.zeros((gp.X.shape[0], Ns_gp))
 
             cov_N = gp.covariance.hyperparameter_count(gp.D)
             noise_N = gp.noise.hyperparameter_count()
 
             for s in range(Ns_gp):
-
                 hyp_noise = gp.posteriors[s].hyp[cov_N : cov_N + noise_N]
                 if hasattr(function_logger, "S"):
                     s2 = (
                         function_logger.S[function_logger.X_flag] ** 2
                     ) * function_logger.n_evals[function_logger.X_flag]
                 else:
                     s2 = None
@@ -376,15 +376,14 @@
 
                 if acq_eval.acq_info.get("log_flag"):
                     tol_fun = 1e-2
                 else:
                     tol_fun = max(1e-12, abs(f_val_old * 1e-3))
 
                 if options["search_optimizer"] == "cmaes":
-
                     if options["search_cmaes_vp_init"]:
                         _, Sigma = vp.moments(orig_flag=False, cov_flag=True)
                     else:
                         X_hpd = get_hpd(gp.X, gp.y, options["hpd_frac"])[0]
                         Sigma = np.cov(X_hpd, rowvar=False, bias=True)
 
                     insigma = np.sqrt(np.diag(Sigma))
```

### Comparing `PyVBMC-1.0.0/pyvbmc/vbmc/create_vbmc_animation.py` & `PyVBMC-1.0.1/pyvbmc/vbmc/create_vbmc_animation.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/vbmc/gaussian_process_train.py` & `PyVBMC-1.0.1/pyvbmc/vbmc/gaussian_process_train.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/vbmc/iteration_history.py` & `PyVBMC-1.0.1/pyvbmc/vbmc/iteration_history.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/vbmc/minimize_adam.py` & `PyVBMC-1.0.1/pyvbmc/vbmc/minimize_adam.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/vbmc/option_configs/advanced_vbmc_options.ini` & `PyVBMC-1.0.1/pyvbmc/vbmc/option_configs/advanced_vbmc_options.ini`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 uncertainty_handling = []
 # Array with indices of integer variables
 integer_vars = []
 # Base observation noise magnitude (standard deviation)
 noise_size = []
 # Max number of consecutive repeated measurements for noisy inputs
 max_repeated_observations = 0
-# Multiplicative discount True acquisition fcn to repeat measurement at the same location
-repeated_acq_discount = 1
 # Number of initial target fcn evals
 fun_eval_start = np.maximum(D, 10)
 # Base step size for stochastic gradient descent
 sgd_step_size = 0.005
 # Skip active sampling the first iteration after warmup
 skip_active_sampling_after_warmup = False
 # Use ranking criterion to pick best non-converged solution
@@ -29,16 +27,14 @@
 diagnostics = False
 # Output function
 output_fcn = []
 # Fraction of allowed exceptions when computing iteration stability
 tol_stable_excpt_frac = 0.2
 # Evaluated fcn values at X0
 f_vals = []
-# Use Optimization Toolbox (if empty determine at runtime)
-optim_toolbox = []
 # Weighted proposal fcn for uncertainty search
 proposal_fcn = None
 # Automatic nonlinear rescaling of variables
 nonlinear_scaling = True
 # Search acquisition fcn(s), from pyvbmc.acquisition_functions. If length is greater than 1, a function is randomly selected for each new point.
 search_acq_fcn = [AcqFcnLog()]
 # Samples for fast acquisition fcn eval per new point
```

### Comparing `PyVBMC-1.0.0/pyvbmc/vbmc/option_configs/basic_vbmc_options.ini` & `PyVBMC-1.0.1/pyvbmc/vbmc/option_configs/basic_vbmc_options.ini`

 * *Files 12% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 max_iter = 50*(2+D)
 # Max number of target fcn evals
 max_fun_evals = 50*(2+D)
 # Number of target fcn evals per iteration
 fun_evals_per_iter = 5
 # Required stable fcn evals for termination
 tol_stable_count = 60
-# Max number of target fcn evals on retry (0 = no retry)
-retry_max_fun_evals = 0
 # Number of variational components to refine posterior at termination
 min_final_components = 50
 # Target log joint function returns noise estimate (SD) as second output
 specify_target_noise = False
 # Name of file to write logs to (if None, no log file will be written)
 log_file_name = None
 # Logging level for log file, one of ("iter", "notify", "final", or "off"), or a level from logging module (e.g. logging.DEBUG)
```

### Comparing `PyVBMC-1.0.0/pyvbmc/vbmc/options.py` & `PyVBMC-1.0.1/pyvbmc/vbmc/options.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/vbmc/variational_optimization.py` & `PyVBMC-1.0.1/pyvbmc/vbmc/variational_optimization.py`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/vbmc/vbmc.py` & `PyVBMC-1.0.1/pyvbmc/vbmc/vbmc.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     ----------
     log_density : callable
         A given target log-posterior or log-likelihood. If ``log_prior`` is
         ``None``, ``log_density`` accepts input ``x`` and returns the value of
         the target log-joint, that is, the unnormalized log-posterior density
         at ``x``. If ``log_prior`` is not ``None``, ``log_density`` should
         return the unnormalized log-likelihood. In either case, if
-        ``options["specifytargetnoise"]`` is true, ``log_density`` should
+        ``options["specify_target_noise"]`` is true, ``log_density`` should
         return a tuple where the first element is the noisy log-density, and
         the second is an estimate of the standard deviation of the noise.
     x0 : np.ndarray, optional
         Starting point for the inference. Ideally ``x0`` is a point in the
         proximity of the mode of the posterior. Default is ``None``.
     lower_bounds, upper_bounds : np.ndarray, optional
         ``lower_bounds`` (`LB`) and ``upper_bounds`` (`UB`) define a set
@@ -107,19 +107,14 @@
     ------
     ValueError
         When neither `x0` or (`plausible_lower_bounds` and
         `plausible_upper_bounds`) are specified.
     ValueError
         When various checks for the bounds (LB, UB, PLB, PUB) of VBMC fail.
 
-    Notes
-    -----
-    The current version of ``VBMC`` only supports noiseless evaluations of the
-    log posterior [1]_. Noisy evaluations as in [2]_ are not implemented yet.
-
     References
     ----------
     .. [1] Acerbi, L. (2018). "Variational Bayesian Monte Carlo". In Advances
        in Neural Information Processing Systems 31 (NeurIPS 2018), pp. 8213-8223.
     .. [2] Acerbi, L. (2020). "Variational Bayesian Monte Carlo with Noisy
        Likelihoods". In Advances in Neural Information Processing Systems 33
        (NeurIPS 2020).
```

### Comparing `PyVBMC-1.0.0/pyvbmc/whitening/README.md` & `PyVBMC-1.0.1/pyvbmc/whitening/README.md`

 * *Files identical despite different names*

### Comparing `PyVBMC-1.0.0/pyvbmc/whitening/whitening.py` & `PyVBMC-1.0.1/pyvbmc/whitening/whitening.py`

 * *Files identical despite different names*

