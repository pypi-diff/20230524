# Comparing `tmp/pyglove-0.3.1.dev20230522.tar.gz` & `tmp/pyglove-0.3.1.dev20230523.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyglove-0.3.1.dev20230522.tar", last modified: Mon May 22 08:07:03 2023, max compression
+gzip compressed data, was "pyglove-0.3.1.dev20230523.tar", last modified: Tue May 23 08:06:37 2023, max compression
```

## Comparing `pyglove-0.3.1.dev20230522.tar` & `pyglove-0.3.1.dev20230523.tar`

### file list

```diff
@@ -1,194 +1,194 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.056222 pyglove-0.3.1.dev20230522/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-22 08:07:03.056222 pyglove-0.3.1.dev20230522/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-22 08:06:58.000000 pyglove-0.3.1.dev20230522/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.024222 pyglove-0.3.1.dev20230522/pyglove/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.024222 pyglove-0.3.1.dev20230522/pyglove/core/
--rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.028222 pyglove-0.3.1.dev20230522/pyglove/core/detouring/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/detouring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/detouring/class_detour.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/detouring/class_detour_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.032222 pyglove-0.3.1.dev20230522/pyglove/core/geno/
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64370 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/deduping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/deduping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/dna_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/dna_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/random_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/space.py
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/space_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/sweeping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/sweeping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.036222 pyglove-0.3.1.dev20230522/pyglove/core/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/derived.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/derived_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22812 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/dynamic_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/dynamic_evaluation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/evolvable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/evolvable_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/iter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/object_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/object_template_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/logging_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.044222 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/codegen_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/common_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/common_traits_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/docstr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/docstr_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/formatting_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/hierarchical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/thread_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/thread_local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/value_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/value_location_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.044222 pyglove-0.3.1.dev20230522/pyglove/core/patching/
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/patching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/patching/object_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/patching/object_factory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/patching/pattern_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/patching/pattern_based_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/patching/rule_based.py
--rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/patching/rule_based_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.048222 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72533 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/boilerplate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22447 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/class_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/class_wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/compounding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/compounding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/contextual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/contextual_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    33112 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    58261 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/dict_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/diff_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/flags_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23864 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/functor.py
--rw-r--r--   0 runner    (1001) docker     (123)    28989 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/functor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    27492 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    52333 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/list_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    34428 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    80848 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/origin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/pure_symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/symbolize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/symbolize_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.048222 pyglove-0.3.1.dev20230522/pyglove/core/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/tuning/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/tuning/backend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/tuning/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/tuning/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/tuning/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/tuning/protocols_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/tuning/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/tuning/sample_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.052222 pyglove-0.3.1.dev20230522/pyglove/core/typing/
--rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/annotation_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/annotation_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/callable_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/callable_ext_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/callable_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/callable_signature_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    49538 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/class_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/class_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/class_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/class_schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/custom_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/key_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/key_specs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/pytype_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/type_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/typed_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/typed_missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    79366 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/value_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)   103891 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/value_specs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.052222 pyglove-0.3.1.dev20230522/pyglove/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.052222 pyglove-0.3.1.dev20230522/pyglove/ext/early_stopping/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/early_stopping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/early_stopping/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/early_stopping/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/early_stopping/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/early_stopping/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.052222 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/hill_climb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/hill_climb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/mutators.py
--rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/mutators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/neat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/neat_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/nsga2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/recombinators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/recombinators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/regularized_evolution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/selectors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/where.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/where_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.052222 pyglove-0.3.1.dev20230522/pyglove/ext/mutfun/
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/mutfun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/mutfun/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/mutfun/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/mutfun/basic_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/mutfun/basic_ops_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.056222 pyglove-0.3.1.dev20230522/pyglove/ext/scalars/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/scalars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/scalars/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/scalars/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/scalars/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/scalars/maths_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/scalars/randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/scalars/randoms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/scalars/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/scalars/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.024222 pyglove-0.3.1.dev20230522/pyglove.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-22 08:07:02.000000 pyglove-0.3.1.dev20230522/pyglove.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-22 08:07:02.000000 pyglove-0.3.1.dev20230522/pyglove.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:07:02.000000 pyglove-0.3.1.dev20230522/pyglove.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-22 08:07:02.000000 pyglove-0.3.1.dev20230522/pyglove.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 08:07:02.000000 pyglove-0.3.1.dev20230522/pyglove.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 08:07:03.056222 pyglove-0.3.1.dev20230522/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.194134 pyglove-0.3.1.dev20230523/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-23 08:06:37.194134 pyglove-0.3.1.dev20230523/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-23 08:06:35.000000 pyglove-0.3.1.dev20230523/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.170134 pyglove-0.3.1.dev20230523/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.170134 pyglove-0.3.1.dev20230523/pyglove/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.170134 pyglove-0.3.1.dev20230523/pyglove/core/detouring/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/detouring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/detouring/class_detour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/detouring/class_detour_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.174134 pyglove-0.3.1.dev20230523/pyglove/core/geno/
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64370 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/deduping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/deduping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/dna_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/dna_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/space_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/sweeping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/sweeping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.174134 pyglove-0.3.1.dev20230523/pyglove/core/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/derived.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/derived_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22812 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/dynamic_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/dynamic_evaluation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/evolvable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/evolvable_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/iter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/object_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/object_template_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/logging_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.178134 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/codegen_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/common_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/common_traits_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/docstr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/docstr_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/formatting_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/hierarchical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/thread_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/thread_local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/value_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/value_location_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.178134 pyglove-0.3.1.dev20230523/pyglove/core/patching/
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/patching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/patching/object_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/patching/object_factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/patching/pattern_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/patching/pattern_based_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/patching/rule_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/patching/rule_based_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.182134 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75319 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/boilerplate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22447 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/class_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/class_wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/compounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/compounding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/contextual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/contextual_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33066 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58215 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/dict_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/diff_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/flags_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23879 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/functor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28989 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/functor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27446 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52472 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/list_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34428 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81342 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/origin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/pure_symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/symbolize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/symbolize_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.186134 pyglove-0.3.1.dev20230523/pyglove/core/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/tuning/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/tuning/backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/tuning/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/tuning/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/tuning/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/tuning/protocols_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/tuning/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/tuning/sample_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.186134 pyglove-0.3.1.dev20230523/pyglove/core/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/annotation_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/annotation_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/callable_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/callable_ext_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/callable_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/callable_signature_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49538 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/class_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/class_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/class_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/class_schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/custom_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/key_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/key_specs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/pytype_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/type_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/typed_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/typed_missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79366 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/value_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103891 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/value_specs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.186134 pyglove-0.3.1.dev20230523/pyglove/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.190134 pyglove-0.3.1.dev20230523/pyglove/ext/early_stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/early_stopping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/early_stopping/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/early_stopping/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/early_stopping/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/early_stopping/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.190134 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/hill_climb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/hill_climb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/mutators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/mutators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/neat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/neat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/nsga2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/recombinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/recombinators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/regularized_evolution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/selectors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/where_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.190134 pyglove-0.3.1.dev20230523/pyglove/ext/mutfun/
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/mutfun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/mutfun/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/mutfun/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/mutfun/basic_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/mutfun/basic_ops_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.194134 pyglove-0.3.1.dev20230523/pyglove/ext/scalars/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/scalars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/scalars/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/scalars/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/scalars/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/scalars/maths_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/scalars/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/scalars/randoms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/scalars/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/scalars/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.170134 pyglove-0.3.1.dev20230523/pyglove.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-23 08:06:37.000000 pyglove-0.3.1.dev20230523/pyglove.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-23 08:06:37.000000 pyglove-0.3.1.dev20230523/pyglove.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:06:37.000000 pyglove-0.3.1.dev20230523/pyglove.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 08:06:37.000000 pyglove-0.3.1.dev20230523/pyglove.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 08:06:37.000000 pyglove-0.3.1.dev20230523/pyglove.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 08:06:37.194134 pyglove-0.3.1.dev20230523/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/setup.py
```

### Comparing `pyglove-0.3.1.dev20230522/LICENSE` & `pyglove-0.3.1.dev20230523/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/PKG-INFO` & `pyglove-0.3.1.dev20230523/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.3.1.dev20230522
+Version: 0.3.1.dev20230523
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.3.1.dev20230522/README.md` & `pyglove-0.3.1.dev20230523/README.md`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/__init__.py` & `pyglove-0.3.1.dev20230523/pyglove/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/__init__.py` & `pyglove-0.3.1.dev20230523/pyglove/core/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,17 +79,14 @@
 List = symbolic.List
 list = List   # pylint: disable=redefined-builtin
 
 Object = symbolic.Object
 ClassWrapper = symbolic.ClassWrapper
 Functor = symbolic.Functor
 
-# Contextual value marker.
-Contextual = symbolic.Contextual
-
 # Decorator for declaring symbolic. members for `pg.Object`.
 members = symbolic.members
 
 #
 # Methods for making symbolic types.
 #
 
@@ -113,14 +110,15 @@
 
 # Function for making compound class.
 compound_class = symbolic.compound_class
 
 # Method for declaring a boilerplated class from a symbolic instance.
 boilerplate_class = symbolic.boilerplate_class
 
+
 #
 # Context manager for swapping wrapped class with their wrappers.
 #
 
 apply_wrappers = symbolic.apply_wrappers
 
 
@@ -160,14 +158,21 @@
 
 # Auxiliary classes:
 Origin = symbolic.Origin
 FieldUpdate = symbolic.FieldUpdate
 Insertion = symbolic.Insertion
 WritePermissionError = symbolic.WritePermissionError
 
+# Contextual value marker.
+ContextualValue = symbolic.ContextualValue
+ContextualGetter = symbolic.ContextualGetter
+
+# Decorator for making contextual getters.
+contextual_getter = symbolic.contextual_getter
+
 
 #
 # Symbols from 'typing.py'
 #
 
 # NOTE(daiyip): we introduce 'typing' as an alias for 'schema' sub-module, since
 # it may be easier to comprehend when users use pytype.
```

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/detouring/__init__.py` & `pyglove-0.3.1.dev20230523/pyglove/core/detouring/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/detouring/class_detour.py` & `pyglove-0.3.1.dev20230523/pyglove/core/detouring/class_detour.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/detouring/class_detour_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/detouring/class_detour_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/geno/__init__.py` & `pyglove-0.3.1.dev20230523/pyglove/core/geno/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/geno/base.py` & `pyglove-0.3.1.dev20230523/pyglove/core/geno/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/geno/base_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/geno/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/geno/categorical.py` & `pyglove-0.3.1.dev20230523/pyglove/core/geno/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/geno/categorical_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/geno/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/geno/custom.py` & `pyglove-0.3.1.dev20230523/pyglove/core/geno/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/geno/custom_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/geno/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/geno/deduping.py` & `pyglove-0.3.1.dev20230523/pyglove/core/geno/deduping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/geno/deduping_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/geno/deduping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/geno/dna_generator.py` & `pyglove-0.3.1.dev20230523/pyglove/core/geno/dna_generator.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/geno/dna_generator_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/geno/dna_generator_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/geno/numerical.py` & `pyglove-0.3.1.dev20230523/pyglove/core/geno/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/geno/numerical_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/geno/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/geno/random.py` & `pyglove-0.3.1.dev20230523/pyglove/core/geno/random.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/geno/random_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/geno/random_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/geno/space.py` & `pyglove-0.3.1.dev20230523/pyglove/core/geno/space.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/geno/space_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/geno/space_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/geno/sweeping.py` & `pyglove-0.3.1.dev20230523/pyglove/core/geno/sweeping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/geno/sweeping_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/geno/sweeping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/hyper/__init__.py` & `pyglove-0.3.1.dev20230523/pyglove/core/hyper/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/hyper/base.py` & `pyglove-0.3.1.dev20230523/pyglove/core/hyper/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/hyper/categorical.py` & `pyglove-0.3.1.dev20230523/pyglove/core/hyper/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/hyper/categorical_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/hyper/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/hyper/custom.py` & `pyglove-0.3.1.dev20230523/pyglove/core/hyper/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/hyper/custom_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/hyper/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/hyper/derived.py` & `pyglove-0.3.1.dev20230523/pyglove/core/hyper/derived.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/hyper/derived_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/hyper/derived_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/hyper/dynamic_evaluation.py` & `pyglove-0.3.1.dev20230523/pyglove/core/hyper/dynamic_evaluation.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/hyper/dynamic_evaluation_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/hyper/dynamic_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/hyper/evolvable.py` & `pyglove-0.3.1.dev20230523/pyglove/core/hyper/evolvable.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/hyper/evolvable_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/hyper/evolvable_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/hyper/iter.py` & `pyglove-0.3.1.dev20230523/pyglove/core/hyper/iter.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/hyper/iter_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/hyper/iter_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/hyper/numerical.py` & `pyglove-0.3.1.dev20230523/pyglove/core/hyper/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/hyper/numerical_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/hyper/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/hyper/object_template.py` & `pyglove-0.3.1.dev20230523/pyglove/core/hyper/object_template.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/hyper/object_template_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/hyper/object_template_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/logging.py` & `pyglove-0.3.1.dev20230523/pyglove/core/logging.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/logging_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/logging_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/__init__.py` & `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/codegen.py` & `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/codegen.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/codegen_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/codegen_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/common_traits.py` & `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/common_traits.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/common_traits_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/common_traits_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/docstr_utils.py` & `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/docstr_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/docstr_utils_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/docstr_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/formatting.py` & `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/formatting.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/formatting_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/formatting_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/hierarchical.py` & `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/hierarchical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/hierarchical_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/hierarchical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/missing.py` & `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/missing_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/thread_local.py` & `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/thread_local.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/thread_local_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/thread_local_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/value_location.py` & `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/value_location.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/value_location_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/value_location_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/patching/__init__.py` & `pyglove-0.3.1.dev20230523/pyglove/core/patching/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/patching/object_factory.py` & `pyglove-0.3.1.dev20230523/pyglove/core/patching/object_factory.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/patching/object_factory_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/patching/object_factory_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/patching/pattern_based.py` & `pyglove-0.3.1.dev20230523/pyglove/core/patching/pattern_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/patching/pattern_based_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/patching/pattern_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/patching/rule_based.py` & `pyglove-0.3.1.dev20230523/pyglove/core/patching/rule_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/patching/rule_based_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/patching/rule_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/__init__.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,19 @@
 
 from pyglove.core.symbolic.flags import notify_on_change
 from pyglove.core.symbolic.flags import is_change_notification_enabled
 
 from pyglove.core.symbolic.flags import auto_call_functors
 from pyglove.core.symbolic.flags import should_call_functors_during_init
 
+# Marker for contextual values.
+from pyglove.core.symbolic.base import ContextualValue
+from pyglove.core.symbolic.contextual import ContextualGetter
+from pyglove.core.symbolic.contextual import contextual_getter
+
 # Symbolic types and their definition helpers.
 from pyglove.core.symbolic.base import Symbolic
 from pyglove.core.symbolic.list import List
 from pyglove.core.symbolic.dict import Dict
 
 from pyglove.core.symbolic.object import ObjectMeta
 from pyglove.core.symbolic.object import Object
@@ -105,17 +110,14 @@
 from pyglove.core.symbolic.base import from_json
 from pyglove.core.symbolic.base import from_json_str
 from pyglove.core.symbolic.base import to_json
 from pyglove.core.symbolic.base import to_json_str
 from pyglove.core.symbolic.base import load
 from pyglove.core.symbolic.base import save
 
-# Marker for contextual values.
-from pyglove.core.symbolic.contextual import Contextual
-
 # Interfaces for pure symbolic objects.
 from pyglove.core.symbolic.pure_symbolic import PureSymbolic
 from pyglove.core.symbolic.pure_symbolic import NonDeterministic
 
 # Symbolic helper classes.
 from pyglove.core.symbolic.base import FieldUpdate
 from pyglove.core.symbolic.base import DescendantQueryOption
```

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/base.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 import sys
 import typing
 from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, Type, Union
 
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import flags
-from pyglove.core.symbolic.contextual import Contextual
 from pyglove.core.symbolic.origin import Origin
 from pyglove.core.symbolic.pure_symbolic import NonDeterministic
 from pyglove.core.symbolic.pure_symbolic import PureSymbolic
 
 
 class WritePermissionError(Exception):
   """Exception raisen when write access to object fields is not allowed."""
@@ -110,14 +109,100 @@
   # Returning only the immediate matched descendants.
   IMMEDIATE = 1
 
   # Returning only the leaf matched descendants.
   LEAF = 2
 
 
+class ContextualValue(
+    pg_typing.CustomTyping,
+    object_utils.JSONConvertible,
+    object_utils.Formattable,
+):
+  """Base class for contextual value markers.
+
+  Contextual value markers allows a symbolic attribute to be late bound
+  based on the entire symbolic tree where current symbolic value is part of.
+  As a result, users could access the late bound values directly through
+  symbolic attributes.
+
+  For example::
+
+    class A(pg.Object):
+      x: int
+      y: int = pg.ContextualValue()
+
+    # Not okay: `x` is not contextual and is not specified.
+    A()
+
+    # Okay: both `x` and `y` are specified.
+    A(x=1, y=2)
+
+    # Okay: `y` is contextual, hence optional.
+    a = A(x=1)
+
+    # Raises: `y` is neither specified during __init__
+    # nor provided from the context.
+    a.y
+
+    d = pg.Dict(y=2, z=pg.Dict(a=a))
+
+    # `a.y` now refers to `d.a` since `d` is in its symbolic parent chain,
+    # aka. context.
+    assert a.y == 2
+  """
+
+  def get(self, name: str, context: 'Symbolic') -> Any:
+    """Try get the contextual value for a symbolic attribute from a parent.
+
+    Args:
+      name: The name of the request symbolic attribute.
+      context: A symbolic parent which represents the current context.
+
+    Returns:
+      The value for the requested symbolic attribute from the current context.
+        If ``pg.MISSING_VALUE``, it means that current symbolic parent cannot
+          provide a contextual value for the attribute, so the current context
+          is moved upward, until it reaches to the root of the symbolic tree.
+        If a ``pg.ContextualValue`` object, it will use the new contextual
+          marker returned to resolve its value from its symbolic parent chains.
+    """
+    return self.value_from(name, context)
+
+  def value_from(self, name: str, context: 'Symbolic') -> Any:
+    """Try get the contextual value for a symbolic attribute from a parent."""
+    return getattr(context, name, pg_typing.MISSING_VALUE)
+
+  def custom_apply(self, *args, **kwargs: Any) -> Tuple[bool, Any]:
+    # This is to make a ``ContextualValue`` object assignable
+    # to any symbolic attribute.
+    return (False, self)
+
+  def format(
+      self,
+      compact: bool = False,
+      verbose: bool = True,
+      root_indent: int = 0,
+      **kwargs: Any,
+  ) -> str:
+    del compact, verbose, root_indent, kwargs
+    return 'ContextualValue()'
+
+  def to_json(self, **kwargs: Any) -> Dict[str, Any]:
+    return self.to_json_dict({})
+
+  def __eq__(self, other: Any) -> bool:
+    # NOTE(daiyip): We do strict type match here since subclasses might
+    # have their own __eq__ logic.
+    return type(other) is ContextualValue  # pylint: disable=unidiomatic-typecheck
+
+  def __ne__(self, other: Any) -> bool:
+    return not self.__eq__(other)
+
+
 class Symbolic(object_utils.JSONConvertible,
                object_utils.MaybePartial,
                object_utils.Formattable):
   """Base for all symbolic types.
 
   Symbolic types are types that provide interfaces for symbolic programming,
   based on which symbolic objects can be created. In PyGlove, there are three
@@ -396,76 +481,77 @@
           self._error_message(
               f'{self.__class__!r} object has no symbolic attribute {key!r}.'))
     return self._sym_getattr(key)
 
   def sym_contextual_hasattr(
       self,
       key: Union[str, int],
-      getter: Optional[Contextual] = None,
+      getter: Optional[ContextualValue] = None,
       start: Union[
           'Symbolic', object_utils.MissingValue
       ] = pg_typing.MISSING_VALUE,
   ) -> bool:
     """Returns True if an attribute exists from current object's context.
 
     Args:
       key: Key of symbolic attribute.
-      getter: An optional ``Contextual`` object as the value retriever.
+      getter: An optional ``ContextualValue`` object as the value retriever.
       start: An object from current object to the root of the composition as the
         starting point of context lookup (upward). If ``pg.MISSING_VALUE``, it
         will start with current node.
 
     Returns:
       True if the attribute exists. Otherwise False.
     """
+    getter = getter or ContextualValue()
     v = self.sym_contextual_getattr(
         key, default=(pg_typing.MISSING_VALUE,), getter=getter, start=start
     )
     return v != (pg_typing.MISSING_VALUE,)
 
   def sym_contextual_getattr(
       self,
       key: Union[str, int],
       default: Any = object_utils.MISSING_VALUE,
-      getter: Optional[Contextual] = None,
+      getter: Optional[ContextualValue] = None,
       start: Union[
           'Symbolic', object_utils.MissingValue
       ] = pg_typing.MISSING_VALUE,
   ) -> Any:
     """Gets a key from current object's context (symbolic parent chain).
 
     Args:
       key: Key of symbolic attribute.
       default: Default value if attribute does not exist. If absent,
         `AttributeError` will be thrown.
-      getter: An optional ``Contextual`` object as the value retriever.
+      getter: An optional ``ContextualValue`` object as the value retriever.
       start: An object from current object to the root of the composition as the
         starting point of context lookup (upward). If ``pg.MISSING_VALUE``, it
         will start with current node.
 
     Returns:
       Value of symbolic attribute if found, otherwise the default value
       if it's specified.
 
     Raises:
       AttributeError if `key` does not exist along the parent chain and
         default value is not ``pg.MISSING_VALUE``.
     """
-    getter = getter or Contextual()
+    getter = getter or ContextualValue()
     if start == pg_typing.MISSING_VALUE:
       current = self
     else:
       current = typing.cast(Symbolic, start)
 
     while current is not None:
-      v = getter.value_from(key, current)
-      # NOTE(daiyip): when the contextual value from the parent returns
-      # another contextual object, we should follow the new return value's
+      v = getter.get(key, current)
+      # NOTE(daiyip): when the ContextualValue value from the parent returns
+      # another ContextualValue object, we should follow the new return value's
       # instruction instead of the original one.
-      if isinstance(v, Contextual):
+      if isinstance(v, ContextualValue):
         getter = v
       elif v != object_utils.MISSING_VALUE:
         return v
       current = current.sym_parent
 
     if default != object_utils.MISSING_VALUE:
       return default
```

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/boilerplate.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/boilerplate.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/boilerplate_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/boilerplate_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/class_wrapper.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/class_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/class_wrapper_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/class_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/compounding.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/compounding.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/compounding_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/compounding_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/contextual_test.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/scalars/randoms_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,63 @@
-# Copyright 2023 The PyGlove Authors
+# Copyright 2022 The PyGlove Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Tests for pyglove.symbolic.Contextual."""
+"""Tests for random scalars."""
 
-import dataclasses
 import unittest
+from pyglove.ext.scalars import randoms as scalars
 
-from pyglove.core import typing as pg_typing
-from pyglove.core.symbolic.contextual import Contextual
 
+class RandomScalarsTest(unittest.TestCase):
+  """Random scalars tests."""
 
-class ContextualTest(unittest.TestCase):
-  """Tests for `pg.symbolic.Contextual`."""
-
-  def test_str(self):
-    self.assertEqual(str(Contextual()), 'CONTEXTUAL')
-    self.assertEqual(str(Contextual(lambda k, p: 1)), 'CONTEXTUAL')
-
-  def test_repr(self):
-    self.assertEqual(repr(Contextual()), 'CONTEXTUAL')
-    self.assertEqual(repr(Contextual(lambda k, p: 1)), 'CONTEXTUAL')
-
-  def test_eq(self):
-    self.assertEqual(Contextual(), Contextual())
-    getter = lambda k, p: 1
-    self.assertEqual(Contextual(getter), Contextual(getter))
-
-    self.assertNotEqual(Contextual(), 1)
-    self.assertNotEqual(Contextual(getter), Contextual())
-
-  def test_value_from(self):
-    @dataclasses.dataclass
-    class A:
-      x: int = 1
-      y: int = 2
-
-    self.assertEqual(Contextual().value_from('x', A()), 1)
-    self.assertEqual(Contextual(lambda k, p: p.y).value_from('x', A()), 2)
-
-  def test_custom_typing(self):
-    v = Contextual()
-    self.assertIs(pg_typing.Int().apply(v), v)
-    self.assertIs(pg_typing.Str().apply(v), v)
+  def test_uniform(self):
+    sv = scalars.Uniform(seed=1)
+    self.assertEqual(sv(0), 0.13436424411240122)
+    self.assertEqual(sv(0), 0.8474337369372327)
+
+    sv = scalars.Uniform(1, 10, seed=1)
+    self.assertEqual(sv(0), 3)
+    self.assertEqual(sv(0), 10)
+
+    with self.assertRaisesRegex(
+        ValueError,
+        '`low` must be less or equal than `high`.'):
+      scalars.Uniform(10, 1, seed=1)
+
+  def test_triangular(self):
+    sv = scalars.Triangular(0.0, 1.0, 0.9, seed=1)
+    self.assertEqual(sv(0), 0.34774677525630787)
+    self.assertEqual(sv(0), 0.8733214547023962)
+
+    sv = scalars.Triangular(10, 20, seed=1)
+    self.assertEqual(sv(0), 12)
+    self.assertEqual(sv(0), 17)
+
+  def test_gaussian(self):
+    sv = scalars.Gaussian(1.0, 0.2, seed=1)
+    self.assertEqual(sv(0), 1.2576369506310927)
+    self.assertEqual(sv(0), 1.2898891217399542)
+
+  def test_normal(self):
+    sv = scalars.Normal(1.0, 0.2, seed=1)
+    self.assertEqual(sv(0), 1.1214911715287412)
+    self.assertEqual(sv(0), 0.997154910897843)
+
+  def test_log_normal(self):
+    sv = scalars.LogNormal(1.0, 0.2, seed=1)
+    self.assertEqual(sv(0), 3.0694278358084994)
+    self.assertEqual(sv(0), 2.710559065635824)
 
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/dict.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 import typing
 from typing import Any, Callable, Iterable, Iterator, List, Optional, Sequence, Set, Tuple, Union
 
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
-from pyglove.core.symbolic import contextual
 from pyglove.core.symbolic import flags
 
 
 class Dict(dict, base.Symbolic, pg_typing.CustomTyping):
   """Symbolic dict.
 
   ``pg.Dict`` implements a dict type whose instances are symbolically
@@ -575,15 +574,15 @@
     """On change event of Dict."""
     if self._onchange_callback:
       self._onchange_callback(field_updates)
 
   def __getitem__(self, key: str) -> Any:
     """Get item in this Dict."""
     v = super().__getitem__(key)
-    if isinstance(v, contextual.Contextual):
+    if isinstance(v, base.ContextualValue):
       start = self.sym_parent
       # NOTE(daiyip): The parent of `pg.Object`'s attribute dict points to
       # the `pg.Object` instance once it's set up. Here we let the ancester
       # traversal to bypass `pg.Object` to avoid double entry, which causes
       # dead loop.
       if self._as_object_attributes_container and self.sym_parent:
         start = start.sym_parent
```

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/dict_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/dict_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 import unittest
 
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
 from pyglove.core.symbolic import flags
 from pyglove.core.symbolic import object as pg_object
-from pyglove.core.symbolic.contextual import Contextual
 from pyglove.core.symbolic.dict import Dict
 from pyglove.core.symbolic.list import List
 from pyglove.core.symbolic.pure_symbolic import NonDeterministic
 from pyglove.core.symbolic.pure_symbolic import PureSymbolic
 
 
 MISSING_VALUE = object_utils.MISSING_VALUE
@@ -1349,15 +1348,15 @@
     self.assertFalse(sd.is_sealed)
     self.assertFalse(sd.a.is_sealed)
     sd.seal()
     self.assertTrue(sd.is_sealed)
     self.assertTrue(sd.a.is_sealed)
 
   def test_contextual(self):
-    sd = Dict(x=Contextual())
+    sd = Dict(x=base.ContextualValue())
     with self.assertRaisesRegex(
         AttributeError, '`x` is not found under its context'
     ):
       _ = sd.x
 
     p = Dict(x=Dict(p='foo'), y=Dict(z=sd))
     self.assertEqual(sd.x, Dict(p='foo'))
```

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/diff.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/diff.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/diff_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/diff_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/flags.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/flags.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/flags_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/flags_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/functor.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/functor.py`

 * *Files 0% similar despite different names*

```diff
@@ -471,18 +471,20 @@
         able to load existing serialized JSON values.
 
   Returns:
     A function that converts a regular function into a symbolic function.
   """
   if inspect.isfunction(args):
     assert returns is None
-    assert base_class is None
     return functor_class(
         typing.cast(Callable[..., Any], args),
-        add_to_registry=True, **kwargs)
+        base_class=base_class,
+        add_to_registry=True,
+        **kwargs,
+    )
   return lambda fn: functor_class(  # pylint: disable=g-long-lambda  # pytype: disable=wrong-arg-types
       fn, args, returns,
       base_class=base_class,
       add_to_registry=True,
       **kwargs)
```

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/functor_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/functor_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/list.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/list.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import dataclasses
 import math
 import typing
 from typing import Any, Callable, Dict, Iterable, Iterator, Optional, Tuple, Union
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
-from pyglove.core.symbolic import contextual
 from pyglove.core.symbolic import flags
 
 
 class List(list, base.Symbolic, pg_typing.CustomTyping):
   """Symbolic list.
 
   ``pg.List`` implements a list type whose instances are symbolically
@@ -460,15 +459,15 @@
 
     if self._onchange_callback is not None:
       self._onchange_callback(field_updates)
 
   def __getitem__(self, index) -> Any:
     """Gets the item at a given position."""
     v = super().__getitem__(index)
-    if isinstance(v, contextual.Contextual):
+    if isinstance(v, base.ContextualValue):
       v = self.sym_contextual_getattr(index, getter=v, start=self.sym_parent)
     return v
 
   def __setitem__(self, index, value: Any) -> None:
     """Set item in this List."""
     if base.treats_as_sealed(self):
       raise base.WritePermissionError(
```

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/list_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/list_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 import inspect
 import io
 import unittest
 
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
+from pyglove.core.symbolic import contextual
 from pyglove.core.symbolic import flags
 from pyglove.core.symbolic import object as pg_object
-from pyglove.core.symbolic.contextual import Contextual
 from pyglove.core.symbolic.dict import Dict
 from pyglove.core.symbolic.list import Insertion
 from pyglove.core.symbolic.list import List
 from pyglove.core.symbolic.pure_symbolic import NonDeterministic
 from pyglove.core.symbolic.pure_symbolic import PureSymbolic
 
 
@@ -1152,15 +1152,20 @@
     sl.seal()
     self.assertTrue(sl.is_sealed)
     self.assertTrue(sl[0].is_sealed)
 
   def test_contextual(self):
     # Test contextual access for schemaless list.
     # Okay: sl[1] is contextual.
-    sl = List([0, Contextual(lambda i, x: x.a)])
+    @contextual.contextual_getter
+    def redirectd_value(k, p, key):
+      del k
+      return getattr(p, key)
+
+    sl = List([0, redirectd_value(key='a')])  # pylint: disable=no-value-for-parameter
 
     self.assertEqual(sl[0], 0)
     with self.assertRaisesRegex(
         AttributeError, '`1` is not found under its context'
     ):
       _ = sl[1]
```

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/object.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/object.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/object_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/object_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 import tempfile
 import typing
 import unittest
 
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
+from pyglove.core.symbolic import contextual
 from pyglove.core.symbolic import flags
 from pyglove.core.symbolic.base import query as pg_query
 from pyglove.core.symbolic.base import traverse as pg_traverse
-from pyglove.core.symbolic.contextual import Contextual
 from pyglove.core.symbolic.dict import Dict
 from pyglove.core.symbolic.functor import functor as pg_functor
 from pyglove.core.symbolic.list import List
 from pyglove.core.symbolic.object import members as pg_members
 from pyglove.core.symbolic.object import Object
 from pyglove.core.symbolic.origin import Origin
 from pyglove.core.symbolic.pure_symbolic import NonDeterministic
@@ -716,38 +716,43 @@
         AttributeError, 'has no symbolic attribute \'y\''):
       _ = b.sym_getattr('y')
 
   def test_sym_contextual_hasattr(self):
     class A(Object):
       x: int
       y: int = 1
-      z: int = Contextual()
+      z: int = base.ContextualValue()
 
     a = A(0)
     _ = Dict(p=Dict(a=a, b=3), z=2)
     self.assertTrue(a.sym_contextual_hasattr('x'))
     self.assertTrue(a.sym_contextual_hasattr('y'))
     self.assertTrue(a.sym_contextual_hasattr('z'))
 
     # Custom start.
     self.assertFalse(a.sym_contextual_hasattr('x', start=a.sym_parent))
     self.assertFalse(a.sym_contextual_hasattr('y', start=a.sym_parent))
     self.assertTrue(a.sym_contextual_hasattr('z', start=a.sym_parent))
 
     # Custom getter.
-    getter = Contextual(lambda k, p: getattr(p, 'b'))
+    @contextual.contextual_getter
+    def redirected_value(k, p, key):
+      del k
+      return getattr(p, key)
+
+    getter = redirected_value(key='b')  # pylint: disable=no-value-for-parameter
     self.assertTrue(a.sym_contextual_hasattr('x', getter, start=a.sym_parent))
     self.assertTrue(a.sym_contextual_hasattr('y', getter, start=a.sym_parent))
     self.assertTrue(a.sym_contextual_hasattr('z', getter, start=a.sym_parent))
 
   def test_sym_contextual_getattr(self):
     class A(Object):
       x: int
       y: int = 1
-      z: int = Contextual()
+      z: int = base.ContextualValue()
 
     a = A(0)
 
     with self.assertRaises(AttributeError):
       _ = a.z
 
     _ = Dict(p=Dict(a=a, b=3), z=2)
@@ -767,15 +772,20 @@
         AttributeError, '`y` is not found under its context'
     ):
       a.sym_contextual_getattr('y', start=a.sym_parent)
 
     self.assertEqual(a.sym_contextual_getattr('z', start=a.sym_parent), 2)
 
     # Custom getter.
-    getter = Contextual(lambda k, p: getattr(p, 'b'))
+    @contextual.contextual_getter
+    def redirected_value(k, p, key):
+      del k
+      return getattr(p, key)
+
+    getter = redirected_value(key='b')  # pylint: disable=no-value-for-parameter
     self.assertEqual(
         a.sym_contextual_getattr('x', getter=getter, start=a.sym_parent), 3
     )
     self.assertEqual(
         a.sym_contextual_getattr('y', getter=getter, start=a.sym_parent), 3
     )
     self.assertEqual(
@@ -1850,15 +1860,15 @@
       @pg_members([], init_arg_list=['*y'])
       class E(B):  # pylint: disable=unused-variable
         pass
 
   def test_contextual(self):
     class A(Object):
       x: int
-      y: str = Contextual()
+      y: str = base.ContextualValue()
 
     # Okay: `A.y` is contextual.
     a = A(1)
 
     # Not okay: `A.y` is not yet available in its context.
     with self.assertRaisesRegex(
         AttributeError, '`y` is not found under its context'
@@ -1872,32 +1882,33 @@
     a.sym_setparent(None)
     with self.assertRaisesRegex(
         AttributeError, '`y` is not found under its context'
     ):
       _ = a.y
 
     # Test parent contextual value with custom getter.
-    sd = Dict(
-        a='bar',
-        b=Dict(
-            x=a,
-            y=Contextual(lambda k, p: getattr(p, 'a'))))
+    @contextual.contextual_getter
+    def redirected_value(k, p, key):
+      del k
+      return getattr(p, key)
+
+    sd = Dict(a='bar', b=Dict(x=a, y=redirected_value(key='a')))  # pylint: disable=no-value-for-parameter
 
     # a.y is redirected to sd.a.
     self.assertEqual(a.y, 'bar')
 
+    @contextual.contextual_getter
+    def immediate_attr(k, p):
+      return p.sym_getattr(k)
+
     class B(Object):
-      x: int = Contextual(lambda k, p: p.sym_getattr(k))
+      x: int = immediate_attr()  # pylint: disable=no-value-for-parameter
 
     b = B()
-    sd = Dict(
-        a='bar',
-        b=Dict(
-            b=b,
-            x=Contextual(lambda k, p: getattr(p, 'a'))))
+    sd = Dict(a='bar', b=Dict(b=b, x=redirected_value(key='a')))  # pylint: disable=no-value-for-parameter
 
     # a.y is redirected to sd.a.
     self.assertEqual(b.x, 'bar')
 
 
 class RebindTest(unittest.TestCase):
   """Dedicated tests for `pg.Dict.rebind`."""
```

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/origin.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/origin.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/origin_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/origin_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/pure_symbolic.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/pure_symbolic.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/schema_utils.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/schema_utils_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/symbolize.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/symbolize.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/symbolize_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/symbolize_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/tuning/__init__.py` & `pyglove-0.3.1.dev20230523/pyglove/core/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/tuning/backend.py` & `pyglove-0.3.1.dev20230523/pyglove/core/tuning/backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/tuning/backend_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/tuning/backend_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/tuning/early_stopping.py` & `pyglove-0.3.1.dev20230523/pyglove/core/tuning/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/tuning/local_backend.py` & `pyglove-0.3.1.dev20230523/pyglove/core/tuning/local_backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/tuning/protocols.py` & `pyglove-0.3.1.dev20230523/pyglove/core/tuning/protocols.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/tuning/protocols_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/tuning/protocols_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/tuning/sample.py` & `pyglove-0.3.1.dev20230523/pyglove/core/tuning/sample.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/tuning/sample_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/tuning/sample_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/typing/__init__.py` & `pyglove-0.3.1.dev20230523/pyglove/core/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/typing/annotation_conversion.py` & `pyglove-0.3.1.dev20230523/pyglove/core/typing/annotation_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/typing/annotation_conversion_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/typing/annotation_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/typing/callable_ext.py` & `pyglove-0.3.1.dev20230523/pyglove/core/typing/callable_ext.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/typing/callable_ext_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/typing/callable_ext_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/typing/callable_signature.py` & `pyglove-0.3.1.dev20230523/pyglove/core/typing/callable_signature.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/typing/callable_signature_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/typing/callable_signature_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/typing/class_schema.py` & `pyglove-0.3.1.dev20230523/pyglove/core/typing/class_schema.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/typing/class_schema_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/typing/class_schema_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/typing/class_schema_utils.py` & `pyglove-0.3.1.dev20230523/pyglove/core/typing/class_schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/typing/class_schema_utils_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/typing/class_schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/typing/custom_typing.py` & `pyglove-0.3.1.dev20230523/pyglove/core/typing/custom_typing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/typing/key_specs.py` & `pyglove-0.3.1.dev20230523/pyglove/core/typing/key_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/typing/key_specs_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/typing/key_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/typing/pytype_support.py` & `pyglove-0.3.1.dev20230523/pyglove/core/typing/pytype_support.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/typing/type_conversion.py` & `pyglove-0.3.1.dev20230523/pyglove/core/typing/type_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/typing/type_conversion_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/typing/type_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/typing/typed_missing.py` & `pyglove-0.3.1.dev20230523/pyglove/core/typing/typed_missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/typing/typed_missing_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/typing/typed_missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/typing/value_specs.py` & `pyglove-0.3.1.dev20230523/pyglove/core/typing/value_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/core/typing/value_specs_test.py` & `pyglove-0.3.1.dev20230523/pyglove/core/typing/value_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/__init__.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/early_stopping/__init__.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/early_stopping/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/early_stopping/base.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/early_stopping/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/early_stopping/base_test.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/early_stopping/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/early_stopping/step_wise.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/early_stopping/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/early_stopping/step_wise_test.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/early_stopping/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/__init__.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/base.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/base_test.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/hill_climb.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/hill_climb.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/hill_climb_test.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/hill_climb_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/mutators.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/mutators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/mutators_test.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/mutators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/neat.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/neat.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/neat_test.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/neat_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/nsga2.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/nsga2.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/nsga2_test.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/nsga2_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/recombinators.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/recombinators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/recombinators_test.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/recombinators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/regularized_evolution.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/regularized_evolution_test.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/regularized_evolution_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/selectors.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/selectors.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/selectors_test.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/selectors_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/where.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/where.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/where_test.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/where_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/mutfun/__init__.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/mutfun/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/mutfun/base.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/mutfun/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/mutfun/base_test.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/mutfun/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/mutfun/basic_ops.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/mutfun/basic_ops.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/mutfun/basic_ops_test.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/mutfun/basic_ops_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/scalars/__init__.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/scalars/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/scalars/base.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/scalars/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/scalars/base_test.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/scalars/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/scalars/maths.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/scalars/maths.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/scalars/maths_test.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/scalars/maths_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/scalars/randoms.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/scalars/randoms.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/scalars/step_wise.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/scalars/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove/ext/scalars/step_wise_test.py` & `pyglove-0.3.1.dev20230523/pyglove/ext/scalars/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/pyglove.egg-info/PKG-INFO` & `pyglove-0.3.1.dev20230523/pyglove.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.3.1.dev20230522
+Version: 0.3.1.dev20230523
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.3.1.dev20230522/pyglove.egg-info/SOURCES.txt` & `pyglove-0.3.1.dev20230523/pyglove.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230522/setup.py` & `pyglove-0.3.1.dev20230523/setup.py`

 * *Files identical despite different names*

