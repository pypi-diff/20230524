# Comparing `tmp/RecordFlux-0.9.0.tar.gz` & `tmp/RecordFlux-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RecordFlux-0.9.0.tar", last modified: Fri Jan  6 14:17:01 2023, max compression
+gzip compressed data, was "RecordFlux-0.9.1.tar", last modified: Tue Mar 28 13:41:25 2023, max compression
```

## Comparing `RecordFlux-0.9.0.tar` & `RecordFlux-0.9.1.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-06 14:17:01.289000 RecordFlux-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11632 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-01-06 14:17:01.289000 RecordFlux-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-06 14:17:01.289000 RecordFlux-0.9.0/RecordFlux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1797 2023-01-06 14:17:01.000000 RecordFlux-0.9.0/RecordFlux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)      724 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-06 14:17:01.273000 RecordFlux-0.9.0/bin/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      125 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/bin/rflx
--rw-r--r--   0 runner    (1001) docker     (122)     3074 2023-01-06 14:16:53.000000 RecordFlux-0.9.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-06 14:17:01.277001 RecordFlux-0.9.0/rflx/
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    66904 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/ada.py
--rw-r--r--   0 runner    (1001) docker     (122)    14948 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     2041 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/const.py
--rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-06 14:17:01.277001 RecordFlux-0.9.0/rflx/converter/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/converter/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    10910 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/converter/iana.py
--rw-r--r--   0 runner    (1001) docker     (122)     6106 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/error.py
--rw-r--r--   0 runner    (1001) docker     (122)   115814 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/expression.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-06 14:17:01.281000 RecordFlux-0.9.0/rflx/generator/
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16584 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/generator/allocator.py
--rw-r--r--   0 runner    (1001) docker     (122)    41781 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/generator/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     2529 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/generator/const.py
--rw-r--r--   0 runner    (1001) docker     (122)    59234 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/generator/generator.py
--rw-r--r--   0 runner    (1001) docker     (122)   131569 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/generator/message.py
--rw-r--r--   0 runner    (1001) docker     (122)    50203 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/generator/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)    82993 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/generator/serializer.py
--rw-r--r--   0 runner    (1001) docker     (122)   212039 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/generator/session.py
--rw-r--r--   0 runner    (1001) docker     (122)     4928 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/graph.py
--rw-r--r--   0 runner    (1001) docker     (122)     4104 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/identifier.py
--rw-r--r--   0 runner    (1001) docker     (122)     8451 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-06 14:17:01.281000 RecordFlux-0.9.0/rflx/model/
--rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1203 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/model/basic_declaration.py
--rw-r--r--   0 runner    (1001) docker     (122)     8293 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/model/declaration.py
--rw-r--r--   0 runner    (1001) docker     (122)   109707 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/model/message.py
--rw-r--r--   0 runner    (1001) docker     (122)     7644 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/model/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1325 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/model/package.py
--rw-r--r--   0 runner    (1001) docker     (122)    33763 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/model/session.py
--rw-r--r--   0 runner    (1001) docker     (122)     9940 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/model/statement.py
--rw-r--r--   0 runner    (1001) docker     (122)    22357 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/model/type_.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-06 14:17:01.285000 RecordFlux-0.9.0/rflx/pyrflx/
--rw-r--r--   0 runner    (1001) docker     (122)      500 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/pyrflx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/pyrflx/bitstring.py
--rw-r--r--   0 runner    (1001) docker     (122)      244 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/pyrflx/error.py
--rw-r--r--   0 runner    (1001) docker     (122)     1449 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/pyrflx/package.py
--rw-r--r--   0 runner    (1001) docker     (122)     2904 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/pyrflx/pyrflx.py
--rw-r--r--   0 runner    (1001) docker     (122)    55108 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/pyrflx/typevalue.py
--rw-r--r--   0 runner    (1001) docker     (122)      654 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/pyrflx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-06 14:17:01.285000 RecordFlux-0.9.0/rflx/specification/
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/specification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/specification/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/specification/const.py
--rw-r--r--   0 runner    (1001) docker     (122)    73605 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/specification/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     8124 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/specification/style.py
--rw-r--r--   0 runner    (1001) docker     (122)    10692 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/tac.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-06 14:17:01.289000 RecordFlux-0.9.0/rflx/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/templates/license_header
--rw-r--r--   0 runner    (1001) docker     (122)     2152 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/templates/rflx_arithmetic.adb
--rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/templates/rflx_arithmetic.ads
--rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/templates/rflx_builtin_types-conversions.ads
--rw-r--r--   0 runner    (1001) docker     (122)      465 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/templates/rflx_builtin_types.ads
--rw-r--r--   0 runner    (1001) docker     (122)    15196 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/templates/rflx_generic_types-generic_operations.adb
--rw-r--r--   0 runner    (1001) docker     (122)     3241 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/templates/rflx_generic_types-generic_operations.ads
--rw-r--r--   0 runner    (1001) docker     (122)      788 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/templates/rflx_generic_types-generic_operators.ads
--rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/templates/rflx_generic_types.ads
--rw-r--r--   0 runner    (1001) docker     (122)     3183 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/templates/rflx_message_sequence.adb
--rw-r--r--   0 runner    (1001) docker     (122)    10754 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/templates/rflx_message_sequence.ads
--rw-r--r--   0 runner    (1001) docker     (122)     4164 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/templates/rflx_scalar_sequence.adb
--rw-r--r--   0 runner    (1001) docker     (122)     9047 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/templates/rflx_scalar_sequence.ads
--rw-r--r--   0 runner    (1001) docker     (122)      270 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/templates/rflx_types-operations.ads
--rw-r--r--   0 runner    (1001) docker     (122)      201 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/templates/rflx_types-operators.ads
--rw-r--r--   0 runner    (1001) docker     (122)      362 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/templates/rflx_types.ads
--rw-r--r--   0 runner    (1001) docker     (122)    12753 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/typing_.py
--rw-r--r--   0 runner    (1001) docker     (122)    18274 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/rflx/validator.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-06 14:17:01.289000 RecordFlux-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2379 2023-01-06 14:16:49.000000 RecordFlux-0.9.0/setup.py
+drwxr-xr-x   0 devel     (1001) devel     (1002)        0 2023-03-28 13:41:25.985789 RecordFlux-0.9.1/
+-rw-r--r--   0 devel     (1001) devel     (1002)    11895 2023-03-28 13:39:44.000000 RecordFlux-0.9.1/CHANGELOG.md
+-rw-r--r--   0 devel     (1001) devel     (1002)    34520 2023-01-18 17:05:22.000000 RecordFlux-0.9.1/LICENSE
+-rw-r--r--   0 devel     (1001) devel     (1002)     2902 2023-03-28 13:41:25.985789 RecordFlux-0.9.1/PKG-INFO
+-rw-r--r--   0 devel     (1001) devel     (1002)     1691 2023-03-28 08:47:28.000000 RecordFlux-0.9.1/README.md
+drwxr-xr-x   0 devel     (1001) devel     (1002)        0 2023-03-28 13:41:25.985789 RecordFlux-0.9.1/RecordFlux.egg-info/
+-rw-r--r--   0 devel     (1001) devel     (1002)     1824 2023-03-28 13:41:25.000000 RecordFlux-0.9.1/RecordFlux.egg-info/SOURCES.txt
+-rw-r--r--   0 devel     (1001) devel     (1002)      721 2023-03-13 16:02:33.000000 RecordFlux-0.9.1/SECURITY.md
+drwxr-xr-x   0 devel     (1001) devel     (1002)        0 2023-03-28 13:41:25.959123 RecordFlux-0.9.1/bin/
+-rw-r--r--   0 devel     (1001) devel     (1002)        0 2023-03-22 17:30:31.000000 RecordFlux-0.9.1/bin/__init__.py
+-rwxr-xr-x   0 devel     (1001) devel     (1002)      125 2023-01-18 17:05:22.000000 RecordFlux-0.9.1/bin/rflx
+-rw-r--r--   0 devel     (1001) devel     (1002)     3094 2023-03-28 13:41:16.000000 RecordFlux-0.9.1/pyproject.toml
+drwxr-xr-x   0 devel     (1001) devel     (1002)        0 2023-03-28 13:41:25.965789 RecordFlux-0.9.1/rflx/
+-rw-r--r--   0 devel     (1001) devel     (1002)       97 2023-03-22 17:30:31.000000 RecordFlux-0.9.1/rflx/__init__.py
+-rw-r--r--   0 devel     (1001) devel     (1002)    66904 2023-03-28 13:39:20.000000 RecordFlux-0.9.1/rflx/ada.py
+-rw-r--r--   0 devel     (1001) devel     (1002)    14923 2023-03-28 13:39:20.000000 RecordFlux-0.9.1/rflx/cli.py
+-rw-r--r--   0 devel     (1001) devel     (1002)     2041 2023-03-22 17:30:31.000000 RecordFlux-0.9.1/rflx/common.py
+-rw-r--r--   0 devel     (1001) devel     (1002)      204 2023-03-22 17:30:31.000000 RecordFlux-0.9.1/rflx/const.py
+-rw-r--r--   0 devel     (1001) devel     (1002)     2131 2023-03-22 17:30:31.000000 RecordFlux-0.9.1/rflx/contract.py
+drwxr-xr-x   0 devel     (1001) devel     (1002)        0 2023-03-28 13:41:25.969123 RecordFlux-0.9.1/rflx/converter/
+-rw-r--r--   0 devel     (1001) devel     (1002)        0 2023-03-22 17:30:31.000000 RecordFlux-0.9.1/rflx/converter/__init__.py
+-rwxr-xr-x   0 devel     (1001) devel     (1002)    10910 2023-03-22 17:30:31.000000 RecordFlux-0.9.1/rflx/converter/iana.py
+-rw-r--r--   0 devel     (1001) devel     (1002)     6048 2023-03-27 15:16:04.000000 RecordFlux-0.9.1/rflx/error.py
+-rw-r--r--   0 devel     (1001) devel     (1002)   120204 2023-03-28 13:39:20.000000 RecordFlux-0.9.1/rflx/expression.py
+drwxr-xr-x   0 devel     (1001) devel     (1002)        0 2023-03-28 13:41:25.972456 RecordFlux-0.9.1/rflx/generator/
+-rw-r--r--   0 devel     (1001) devel     (1002)      109 2023-03-22 17:30:31.000000 RecordFlux-0.9.1/rflx/generator/__init__.py
+-rw-r--r--   0 devel     (1001) devel     (1002)    16584 2023-03-28 13:39:20.000000 RecordFlux-0.9.1/rflx/generator/allocator.py
+-rw-r--r--   0 devel     (1001) devel     (1002)    41737 2023-03-28 13:39:20.000000 RecordFlux-0.9.1/rflx/generator/common.py
+-rw-r--r--   0 devel     (1001) devel     (1002)     2507 2023-03-22 17:30:31.000000 RecordFlux-0.9.1/rflx/generator/const.py
+-rw-r--r--   0 devel     (1001) devel     (1002)    59190 2023-03-28 13:39:20.000000 RecordFlux-0.9.1/rflx/generator/generator.py
+-rw-r--r--   0 devel     (1001) devel     (1002)   131239 2023-03-22 17:30:31.000000 RecordFlux-0.9.1/rflx/generator/message.py
+-rw-r--r--   0 devel     (1001) devel     (1002)    50137 2023-03-22 17:30:31.000000 RecordFlux-0.9.1/rflx/generator/parser.py
+-rw-r--r--   0 devel     (1001) devel     (1002)    82949 2023-03-22 17:30:31.000000 RecordFlux-0.9.1/rflx/generator/serializer.py
+-rw-r--r--   0 devel     (1001) devel     (1002)   212440 2023-03-28 13:39:20.000000 RecordFlux-0.9.1/rflx/generator/session.py
+-rw-r--r--   0 devel     (1001) devel     (1002)     4928 2023-03-22 17:30:31.000000 RecordFlux-0.9.1/rflx/graph.py
+-rw-r--r--   0 devel     (1001) devel     (1002)     4234 2023-03-27 15:16:04.000000 RecordFlux-0.9.1/rflx/identifier.py
+-rw-r--r--   0 devel     (1001) devel     (1002)     8451 2023-03-22 17:30:31.000000 RecordFlux-0.9.1/rflx/integration.py
+drwxr-xr-x   0 devel     (1001) devel     (1002)        0 2023-03-28 13:41:25.979123 RecordFlux-0.9.1/rflx/model/
+-rw-r--r--   0 devel     (1001) devel     (1002)     1241 2023-03-22 17:30:31.000000 RecordFlux-0.9.1/rflx/model/__init__.py
+-rw-r--r--   0 devel     (1001) devel     (1002)     1203 2023-03-22 17:30:31.000000 RecordFlux-0.9.1/rflx/model/basic_declaration.py
+-rw-r--r--   0 devel     (1001) devel     (1002)     8293 2023-03-22 17:30:31.000000 RecordFlux-0.9.1/rflx/model/declaration.py
+-rw-r--r--   0 devel     (1001) devel     (1002)   109685 2023-03-28 13:39:20.000000 RecordFlux-0.9.1/rflx/model/message.py
+-rw-r--r--   0 devel     (1001) devel     (1002)     7644 2023-03-22 17:30:31.000000 RecordFlux-0.9.1/rflx/model/model.py
+-rw-r--r--   0 devel     (1001) devel     (1002)     1325 2023-03-22 17:30:31.000000 RecordFlux-0.9.1/rflx/model/package.py
+-rw-r--r--   0 devel     (1001) devel     (1002)    33891 2023-03-28 13:39:20.000000 RecordFlux-0.9.1/rflx/model/session.py
+-rw-r--r--   0 devel     (1001) devel     (1002)    35306 2023-03-27 17:18:17.000000 RecordFlux-0.9.1/rflx/model/session.py.orig
+-rw-r--r--   0 devel     (1001) devel     (1002)    14068 2023-03-27 15:16:04.000000 RecordFlux-0.9.1/rflx/model/statement.py
+-rw-r--r--   0 devel     (1001) devel     (1002)    22313 2023-03-28 13:39:20.000000 RecordFlux-0.9.1/rflx/model/type_.py
+-rw-r--r--   0 devel     (1001) devel     (1002)        0 2023-01-18 17:05:22.000000 RecordFlux-0.9.1/rflx/py.typed
+drwxr-xr-x   0 devel     (1001) devel     (1002)        0 2023-03-28 13:41:25.979123 RecordFlux-0.9.1/rflx/pyrflx/
+-rw-r--r--   0 devel     (1001) devel     (1002)      500 2023-03-22 17:30:31.000000 RecordFlux-0.9.1/rflx/pyrflx/__init__.py
+-rw-r--r--   0 devel     (1001) devel     (1002)     2283 2023-03-28 13:39:20.000000 RecordFlux-0.9.1/rflx/pyrflx/bitstring.py
+-rw-r--r--   0 devel     (1001) devel     (1002)      244 2023-03-22 17:30:31.000000 RecordFlux-0.9.1/rflx/pyrflx/error.py
+-rw-r--r--   0 devel     (1001) devel     (1002)     1449 2023-03-28 13:39:20.000000 RecordFlux-0.9.1/rflx/pyrflx/package.py
+-rw-r--r--   0 devel     (1001) devel     (1002)     2904 2023-03-28 13:39:20.000000 RecordFlux-0.9.1/rflx/pyrflx/pyrflx.py
+-rw-r--r--   0 devel     (1001) devel     (1002)    55086 2023-03-28 13:39:20.000000 RecordFlux-0.9.1/rflx/pyrflx/typevalue.py
+-rw-r--r--   0 devel     (1001) devel     (1002)      654 2023-03-22 17:30:31.000000 RecordFlux-0.9.1/rflx/pyrflx/utils.py
+drwxr-xr-x   0 devel     (1001) devel     (1002)        0 2023-03-28 13:41:25.982456 RecordFlux-0.9.1/rflx/specification/
+-rw-r--r--   0 devel     (1001) devel     (1002)       51 2023-03-22 17:30:31.000000 RecordFlux-0.9.1/rflx/specification/__init__.py
+-rw-r--r--   0 devel     (1001) devel     (1002)     2418 2023-03-28 13:39:20.000000 RecordFlux-0.9.1/rflx/specification/cache.py
+-rw-r--r--   0 devel     (1001) devel     (1002)     1095 2023-03-22 17:30:31.000000 RecordFlux-0.9.1/rflx/specification/const.py
+-rw-r--r--   0 devel     (1001) devel     (1002)    73583 2023-03-28 13:39:20.000000 RecordFlux-0.9.1/rflx/specification/parser.py
+-rw-r--r--   0 devel     (1001) devel     (1002)     8124 2023-03-28 13:39:20.000000 RecordFlux-0.9.1/rflx/specification/style.py
+-rw-r--r--   0 devel     (1001) devel     (1002)    46579 2023-03-28 13:39:20.000000 RecordFlux-0.9.1/rflx/tac.py
+drwxr-xr-x   0 devel     (1001) devel     (1002)        0 2023-03-28 13:41:25.985789 RecordFlux-0.9.1/rflx/templates/
+-rw-r--r--   0 devel     (1001) devel     (1002)      198 2023-03-13 16:02:33.000000 RecordFlux-0.9.1/rflx/templates/license_header
+-rw-r--r--   0 devel     (1001) devel     (1002)     2152 2023-03-13 16:02:33.000000 RecordFlux-0.9.1/rflx/templates/rflx_arithmetic.adb
+-rw-r--r--   0 devel     (1001) devel     (1002)     4024 2023-03-13 16:02:33.000000 RecordFlux-0.9.1/rflx/templates/rflx_arithmetic.ads
+-rw-r--r--   0 devel     (1001) devel     (1002)     1568 2023-03-13 16:02:33.000000 RecordFlux-0.9.1/rflx/templates/rflx_builtin_types-conversions.ads
+-rw-r--r--   0 devel     (1001) devel     (1002)      465 2023-03-13 16:02:33.000000 RecordFlux-0.9.1/rflx/templates/rflx_builtin_types.ads
+-rw-r--r--   0 devel     (1001) devel     (1002)    15196 2023-03-13 16:02:33.000000 RecordFlux-0.9.1/rflx/templates/rflx_generic_types-generic_operations.adb
+-rw-r--r--   0 devel     (1001) devel     (1002)     3241 2023-03-13 16:02:33.000000 RecordFlux-0.9.1/rflx/templates/rflx_generic_types-generic_operations.ads
+-rw-r--r--   0 devel     (1001) devel     (1002)      788 2023-03-13 16:02:33.000000 RecordFlux-0.9.1/rflx/templates/rflx_generic_types-generic_operators.ads
+-rw-r--r--   0 devel     (1001) devel     (1002)     3302 2023-03-13 16:02:33.000000 RecordFlux-0.9.1/rflx/templates/rflx_generic_types.ads
+-rw-r--r--   0 devel     (1001) devel     (1002)     3183 2023-03-13 16:02:33.000000 RecordFlux-0.9.1/rflx/templates/rflx_message_sequence.adb
+-rw-r--r--   0 devel     (1001) devel     (1002)    10732 2023-03-13 16:02:33.000000 RecordFlux-0.9.1/rflx/templates/rflx_message_sequence.ads
+-rw-r--r--   0 devel     (1001) devel     (1002)     4164 2023-03-13 16:02:33.000000 RecordFlux-0.9.1/rflx/templates/rflx_scalar_sequence.adb
+-rw-r--r--   0 devel     (1001) devel     (1002)     9025 2023-03-13 16:02:33.000000 RecordFlux-0.9.1/rflx/templates/rflx_scalar_sequence.ads
+-rw-r--r--   0 devel     (1001) devel     (1002)      270 2023-03-13 16:02:33.000000 RecordFlux-0.9.1/rflx/templates/rflx_types-operations.ads
+-rw-r--r--   0 devel     (1001) devel     (1002)      201 2023-03-13 16:02:33.000000 RecordFlux-0.9.1/rflx/templates/rflx_types-operators.ads
+-rw-r--r--   0 devel     (1001) devel     (1002)      362 2023-03-13 16:02:33.000000 RecordFlux-0.9.1/rflx/templates/rflx_types.ads
+-rw-r--r--   0 devel     (1001) devel     (1002)    12753 2023-03-28 13:39:20.000000 RecordFlux-0.9.1/rflx/typing_.py
+-rw-r--r--   0 devel     (1001) devel     (1002)    18274 2023-03-28 13:39:20.000000 RecordFlux-0.9.1/rflx/validator.py
+-rw-r--r--   0 devel     (1001) devel     (1002)       38 2023-03-28 13:41:25.985789 RecordFlux-0.9.1/setup.cfg
+-rw-r--r--   0 devel     (1001) devel     (1002)     2375 2023-03-27 15:16:04.000000 RecordFlux-0.9.1/setup.py
```

### Comparing `RecordFlux-0.9.0/CHANGELOG.md` & `RecordFlux-0.9.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.9.1] - 2023-03-28
+
+### Fixed
+
+- Missing with clause in session package for indirectly used enumeration types (#1298)
+- Compilation error for message field access in state transition (#1299)
+- Warning about that `with RFLX.RFLX_Types` is unreferenced or might be moved to body of session package
+
 ## [0.9.0] - 2023-01-06
 
 ### Added
 
 - Support for Python 3.11
 
 ### Removed
@@ -339,19 +347,19 @@
 - PyDotPlus (used for generation of graphs)
 - Z3 (used for verification of message specifications)
 
 ## [0.2.0] - 2019-09-16
 
 ## [0.1.0] - 2019-05-14
 
-[unreleased]: https://github.com/Componolit/RecordFlux/compare/v0.9.0...HEAD
-[0.9.0]: https://github.com/Componolit/RecordFlux/compare/v0.8.0...v0.9.0
-[0.8.0]: https://github.com/Componolit/RecordFlux/compare/v0.7.1...v0.8.0
-[0.7.1]: https://github.com/Componolit/RecordFlux/compare/v0.7.0...v0.7.1
-[0.7.0]: https://github.com/Componolit/RecordFlux/compare/v0.6.0...v0.7.0
-[0.6.0]: https://github.com/Componolit/RecordFlux/compare/v0.5.0...v0.6.0
-[0.5.0]: https://github.com/Componolit/RecordFlux/compare/v0.4.1...v0.5.0
-[0.4.1]: https://github.com/Componolit/RecordFlux/compare/v0.4.0...v0.4.1
-[0.4.0]: https://github.com/Componolit/RecordFlux/compare/v0.3.0...v0.4.0
-[0.3.0]: https://github.com/Componolit/RecordFlux/compare/v0.2.0...v0.3.0
-[0.2.0]: https://github.com/Componolit/RecordFlux/compare/v0.1.0...v0.2.0
-[0.1.0]: https://github.com/Componolit/RecordFlux/compare/29a292a794af58d29ee0d499e74f3d86b73309fa...v0.1.0
+[0.9.1]: https://github.com/AdaCore/RecordFlux/compare/v0.9.0...v0.9.1
+[0.9.0]: https://github.com/AdaCore/RecordFlux/compare/v0.8.0...v0.9.0
+[0.8.0]: https://github.com/AdaCore/RecordFlux/compare/v0.7.1...v0.8.0
+[0.7.1]: https://github.com/AdaCore/RecordFlux/compare/v0.7.0...v0.7.1
+[0.7.0]: https://github.com/AdaCore/RecordFlux/compare/v0.6.0...v0.7.0
+[0.6.0]: https://github.com/AdaCore/RecordFlux/compare/v0.5.0...v0.6.0
+[0.5.0]: https://github.com/AdaCore/RecordFlux/compare/v0.4.1...v0.5.0
+[0.4.1]: https://github.com/AdaCore/RecordFlux/compare/v0.4.0...v0.4.1
+[0.4.0]: https://github.com/AdaCore/RecordFlux/compare/v0.3.0...v0.4.0
+[0.3.0]: https://github.com/AdaCore/RecordFlux/compare/v0.2.0...v0.3.0
+[0.2.0]: https://github.com/AdaCore/RecordFlux/compare/v0.1.0...v0.2.0
+[0.1.0]: https://github.com/AdaCore/RecordFlux/compare/29a292a794af58d29ee0d499e74f3d86b73309fa...v0.1.0
```

### Comparing `RecordFlux-0.9.0/LICENSE` & `RecordFlux-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/PKG-INFO` & `RecordFlux-0.9.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: RecordFlux
-Version: 0.9.0
+Version: 0.9.1
 Summary: A toolset for the formal specification and generation of verifiable binary parsers, message generators and protocol state machines.
-Home-page: https://github.com/Componolit/RecordFlux
+Home-page: https://github.com/AdaCore/RecordFlux
 Author: Tobias Reiher
-Author-email: reiher@componolit.com
+Author-email: reiher@adacore.com
 License: AGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Ada
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -23,28 +23,28 @@
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: devel
 License-File: LICENSE
 
-# [![RecordFlux](https://raw.githubusercontent.com/Componolit/RecordFlux/main/doc/img/logo.svg)](https://github.com/Componolit/RecordFlux/)
+# [RecordFlux](https://github.com/AdaCore/RecordFlux/)
 
 [![PyPI](https://img.shields.io/pypi/v/RecordFlux?color=blue)](https://pypi.org/project/RecordFlux/)
 [![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue.svg)](https://python.org/)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
-[![Tests](https://github.com/Componolit/RecordFlux/workflows/tests/badge.svg)](https://github.com/Componolit/RecordFlux/actions)
+[![Tests](https://github.com/AdaCore/RecordFlux/workflows/tests/badge.svg)](https://github.com/AdaCore/RecordFlux/actions)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/5052/badge)](https://bestpractices.coreinfrastructure.org/projects/5052)
 
 RecordFlux is a toolset for the formal specification and generation of verifiable binary parsers, message generators and protocol state machines.
 
-See the [documentation](https://componolit.github.io/RecordFlux/) for more information.
+See the [documentation](https://adacore.github.io/RecordFlux/) for more information.
 
 ## Contribution and Feedback
 
-Contributions and feedback to RecordFlux are very welcome. To discuss a bug or an enhancement, [open a ticket on GitHub](https://github.com/Componolit/RecordFlux/issues/new/choose) and select the appropriate issue template. Please give sufficient information about your issue, the software version you are using and your environment such that the developers can understand and (if necessary) reproduce the problem. If none of the provided issue templates fit your needs, feel free to open [a blank issue](https://github.com/Componolit/RecordFlux/issues/new).
+Contributions and feedback to RecordFlux are very welcome. To discuss a bug or an enhancement, [open a ticket on GitHub](https://github.com/AdaCore/RecordFlux/issues/new/choose) and select the appropriate issue template. Please give sufficient information about your issue, the software version you are using and your environment such that the developers can understand and (if necessary) reproduce the problem. If none of the provided issue templates fit your needs, feel free to open [a blank issue](https://github.com/AdaCore/RecordFlux/issues/new).
 
-See the [development guide](https://componolit.github.io/RecordFlux/development_guide/) on how to contribute to RecordFlux.
+See the [development guide](https://adacore.github.io/RecordFlux/development_guide/) on how to contribute to RecordFlux.
 
 ## Licence
 
 This software is licensed under the `AGPL-3.0`. See the `LICENSE` file for the full license text.
```

### Comparing `RecordFlux-0.9.0/README.md` & `RecordFlux-0.9.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# [![RecordFlux](https://raw.githubusercontent.com/Componolit/RecordFlux/main/doc/img/logo.svg)](https://github.com/Componolit/RecordFlux/)
+# [RecordFlux](https://github.com/AdaCore/RecordFlux/)
 
 [![PyPI](https://img.shields.io/pypi/v/RecordFlux?color=blue)](https://pypi.org/project/RecordFlux/)
 [![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue.svg)](https://python.org/)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
-[![Tests](https://github.com/Componolit/RecordFlux/workflows/tests/badge.svg)](https://github.com/Componolit/RecordFlux/actions)
+[![Tests](https://github.com/AdaCore/RecordFlux/workflows/tests/badge.svg)](https://github.com/AdaCore/RecordFlux/actions)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/5052/badge)](https://bestpractices.coreinfrastructure.org/projects/5052)
 
 RecordFlux is a toolset for the formal specification and generation of verifiable binary parsers, message generators and protocol state machines.
 
-See the [documentation](https://componolit.github.io/RecordFlux/) for more information.
+See the [documentation](https://adacore.github.io/RecordFlux/) for more information.
 
 ## Contribution and Feedback
 
-Contributions and feedback to RecordFlux are very welcome. To discuss a bug or an enhancement, [open a ticket on GitHub](https://github.com/Componolit/RecordFlux/issues/new/choose) and select the appropriate issue template. Please give sufficient information about your issue, the software version you are using and your environment such that the developers can understand and (if necessary) reproduce the problem. If none of the provided issue templates fit your needs, feel free to open [a blank issue](https://github.com/Componolit/RecordFlux/issues/new).
+Contributions and feedback to RecordFlux are very welcome. To discuss a bug or an enhancement, [open a ticket on GitHub](https://github.com/AdaCore/RecordFlux/issues/new/choose) and select the appropriate issue template. Please give sufficient information about your issue, the software version you are using and your environment such that the developers can understand and (if necessary) reproduce the problem. If none of the provided issue templates fit your needs, feel free to open [a blank issue](https://github.com/AdaCore/RecordFlux/issues/new).
 
-See the [development guide](https://componolit.github.io/RecordFlux/development_guide/) on how to contribute to RecordFlux.
+See the [development guide](https://adacore.github.io/RecordFlux/development_guide/) on how to contribute to RecordFlux.
 
 ## Licence
 
 This software is licensed under the `AGPL-3.0`. See the `LICENSE` file for the full license text.
```

### Comparing `RecordFlux-0.9.0/RecordFlux.egg-info/SOURCES.txt` & `RecordFlux-0.9.1/RecordFlux.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 rflx/model/__init__.py
 rflx/model/basic_declaration.py
 rflx/model/declaration.py
 rflx/model/message.py
 rflx/model/model.py
 rflx/model/package.py
 rflx/model/session.py
+rflx/model/session.py.orig
 rflx/model/statement.py
 rflx/model/type_.py
 rflx/pyrflx/__init__.py
 rflx/pyrflx/bitstring.py
 rflx/pyrflx/error.py
 rflx/pyrflx/package.py
 rflx/pyrflx/pyrflx.py
```

### Comparing `RecordFlux-0.9.0/SECURITY.md` & `RecordFlux-0.9.1/SECURITY.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Security Policy
 
 ## Reporting a Vulnerability
 
-Open an issue on GitHub using [the vulnerability template](https://github.com/Componolit/RecordFlux/issues/new?labels=vulnerability&template=vulnerability.md). In addition to the `vulnerability` tag (which should be added automatically) also add tags for the versions that you know are affected.
+Open an issue on GitHub using [the vulnerability template](https://github.com/AdaCore/RecordFlux/issues/new?labels=vulnerability&template=vulnerability.md). In addition to the `vulnerability` tag (which should be added automatically) also add tags for the versions that you know are affected.
 
 We will get back to you within a working day to discuss the next steps.
 
 ## Confidential Reporting
 
 If you would like to report a security vulnerability confidentially, please send an email to [product-security@adacore.com](mailto:product-security@adacore.com).
```

### Comparing `RecordFlux-0.9.0/pyproject.toml` & `RecordFlux-0.9.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     'pydotplus',
     'pytest',
     'z3',
 ]
 
 [tool.pylint.master]
 jobs = 0
-load-plugins = 'python_style.pylint_checker'
+load-plugins = 'devutils.pylint_checker'
 
 [tool.pylint.messages_control]
 enable = [
     'useless-suppression'
 ]
 disable = [
     'duplicate-code',  # ISSUE: PyCQA/pylint#4118
@@ -109,14 +109,15 @@
 [[tool.mypy.overrides]]
 module = [
     'astroid',
     'langkit.*',
     'pylint.*',
     'ruamel',
     'setuptools.*',
+    'setuptools_scm.*',
     'wheel.*',
 ]
 ignore_missing_imports = true
 
 [tool.pydocstyle]
 ignore = [
     'D100',
```

### Comparing `RecordFlux-0.9.0/rflx/ada.py` & `RecordFlux-0.9.1/rflx/ada.py`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/cli.py` & `RecordFlux-0.9.1/rflx/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,15 +276,15 @@
 Command: {' '.join(argv)}
 
 {traceback.format_exc()}
 ----------------------------------------------------------------------------
 
 A bug was detected. Please report this issue on GitHub:
 
-https://github.com/Componolit/RecordFlux/issues/new?labels=bug
+https://github.com/AdaCore/RecordFlux/issues/new?labels=bug
 
 Include the complete content of the bug box shown above and all input files
 in the report."""
 
     return 0
 
 
@@ -304,15 +304,15 @@
 
 
 def check(args: argparse.Namespace) -> None:
     parse(args.files, args.no_verification, args.workers)
 
 
 def generate(args: argparse.Namespace) -> None:
-    # https://github.com/Componolit/Workarounds/issues/28
+    # Eng/RecordFlux/Workarounds#28
     args.prefix = args.prefix if args.prefix != " " else ""
 
     if args.prefix and "" in args.prefix.split("."):
         fail(f'invalid prefix: "{args.prefix}"', Subsystem.CLI)
 
     if not args.output_directory.is_dir():
         fail(f'directory not found: "{args.output_directory}"', Subsystem.CLI)
```

### Comparing `RecordFlux-0.9.0/rflx/common.py` & `RecordFlux-0.9.1/rflx/common.py`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/contract.py` & `RecordFlux-0.9.1/rflx/contract.py`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/converter/iana.py` & `RecordFlux-0.9.1/rflx/converter/iana.py`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/error.py` & `RecordFlux-0.9.1/rflx/error.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-from abc import abstractmethod
 from collections import deque
 from collections.abc import Sequence
 from enum import Enum, auto
 from pathlib import Path
 from threading import local
 from typing import NoReturn, Optional, TypeVar, Union
 
@@ -111,18 +110,24 @@
         def severity(self) -> Severity:
             return self._severity
 
         @property
         def location(self) -> Optional[Location]:
             return self._location
 
-    @abstractmethod
-    def __init__(self) -> None:
+    def __init__(
+        self,
+        entries: Optional[
+            Union[Sequence[tuple[str, Subsystem, Severity, Optional[Location]]], BaseError]
+        ] = None,
+    ) -> None:
         super().__init__()
         self._messages: deque[BaseError.Entry] = deque()
+        if entries:
+            self.extend(entries)
 
     def __repr__(self) -> str:
         return verbose_repr(self, ["errors"])
 
     def __str__(self) -> str:
         def locn(entry: BaseError.Entry) -> str:
             if entry.location:
@@ -175,28 +180,22 @@
             print(self)
             self._messages = deque()
 
 
 class RecordFluxError(BaseError):
     """Error indicating an issue in an input or a known limitation."""
 
-    def __init__(self) -> None:  # pylint: disable = useless-super-delegation
-        super().__init__()
-
 
 class FatalError(BaseError):
     """
     Error indicating a bug.
 
     This exception should never be caught outside of RecordFlux.
     """
 
-    def __init__(self) -> None:  # pylint: disable = useless-super-delegation
-        super().__init__()
-
 
 def fail(
     message: str,
     subsystem: Subsystem,
     severity: Severity = Severity.ERROR,
     location: Optional[Location] = None,
 ) -> NoReturn:
```

### Comparing `RecordFlux-0.9.0/rflx/expression.py` & `RecordFlux-0.9.1/rflx/expression.py`

 * *Files 4% similar despite different names*

```diff
@@ -361,15 +361,22 @@
         z3expr = self.expr.z3expr()
         if not isinstance(z3expr, z3.BoolRef):
             raise Z3TypeError("negating non-boolean term")
         return z3.Not(z3expr)
 
     def to_tac(self, target: StrID, variable_id: Generator[ID, None, None]) -> list[tac.Stmt]:
         inner_stmts, inner_expr = _to_tac_basic_bool(self.expr, variable_id)
-        return [*inner_stmts, tac.Assign(target, tac.Not(inner_expr))]
+        return [
+            *inner_stmts,
+            tac.Assign(
+                target,
+                tac.Not(inner_expr, origin=self),
+                origin=self,
+            ),
+        ]
 
 
 class BinExpr(Expr):
     def __init__(
         self,
         left: Expr,
         right: Expr,
@@ -637,36 +644,47 @@
     @property
     @abstractmethod
     def symbol(self) -> str:
         raise NotImplementedError
 
     def to_tac(self, target: StrID, variable_id: Generator[ID, None, None]) -> list[tac.Stmt]:
         if len(self.terms) == 0:
-            return [tac.Assign(target, tac.BoolVal(True))]
+            return [tac.Assign(target, tac.BoolVal(True), origin=self)]
 
         if len(self.terms) == 1:
             first_stmts, first_expr = _to_tac_basic_bool(self.terms[0], variable_id)
-            return [*first_stmts, tac.Assign(target, first_expr)]
+            return [
+                *first_stmts,
+                tac.Assign(target, first_expr, origin=self),
+            ]
 
         if len(self.terms) == 2:
             left_stmts, left_expr = _to_tac_basic_bool(self.terms[0], variable_id)
             right_stmts, right_expr = _to_tac_basic_bool(self.terms[1], variable_id)
             return [
                 *left_stmts,
                 *right_stmts,
-                tac.Assign(target, getattr(tac, self.__class__.__name__)(left_expr, right_expr)),
+                tac.Assign(
+                    target,
+                    getattr(tac, self.__class__.__name__)(left_expr, right_expr, origin=self),
+                    origin=self,
+                ),
             ]
 
         right_id = next(variable_id)
         left_stmts, left_expr = _to_tac_basic_bool(self.terms[0], variable_id)
         return [
             *(self.__class__(*self.terms[1:]).to_tac(right_id, variable_id)),
             *left_stmts,
             tac.Assign(
-                target, getattr(tac, self.__class__.__name__)(left_expr, tac.BoolVar(right_id))
+                target,
+                getattr(tac, self.__class__.__name__)(
+                    left_expr, tac.BoolVar(right_id), origin=self
+                ),
+                origin=self,
             ),
         ]
 
 
 class And(BoolAssExpr):
     def __neg__(self) -> Expr:
         raise NotImplementedError
@@ -866,15 +884,21 @@
     def ada_expr(self) -> ada.Expr:
         return ada.Number(self.value, self.base)
 
     def z3expr(self) -> z3.ArithRef:
         return z3.IntVal(self.value)
 
     def to_tac(self, target: StrID, variable_id: Generator[ID, None, None]) -> list[tac.Stmt]:
-        return [tac.Assign(target, tac.IntVal(self.value))]
+        return [
+            tac.Assign(
+                target,
+                tac.IntVal(self.value, origin=self),
+                origin=self,
+            )
+        ]
 
 
 class MathAssExpr(AssExpr):
     def __init__(self, *terms: Expr, location: Optional[Location] = None) -> None:
         super().__init__(*terms, location=location)
         common_type = rty.common_type([t.type_ for t in terms])
         self.type_ = common_type if common_type != rty.Undefined() else rty.UndefinedInteger()
@@ -883,36 +907,54 @@
         error = RecordFluxError()
         for t in self.terms:
             error += t.check_type_instance(rty.AnyInteger)
         return error
 
     def to_tac(self, target: StrID, variable_id: Generator[ID, None, None]) -> list[tac.Stmt]:
         if len(self.terms) == 0:
-            return [tac.Assign(target, tac.IntVal(0))]
+            return [
+                tac.Assign(
+                    target,
+                    tac.IntVal(0, origin=self),
+                    origin=self,
+                )
+            ]
 
         if len(self.terms) == 1:
             first_stmts, first_expr = _to_tac_basic_int(self.terms[0], variable_id)
-            return [*first_stmts, tac.Assign(target, first_expr)]
+            return [
+                *first_stmts,
+                tac.Assign(target, first_expr, origin=self),
+            ]
 
         if len(self.terms) == 2:
             left_stmts, left_expr = _to_tac_basic_int(self.terms[0], variable_id)
             right_stmts, right_expr = _to_tac_basic_int(self.terms[1], variable_id)
             return [
                 *left_stmts,
                 *right_stmts,
-                tac.Assign(target, getattr(tac, self.__class__.__name__)(left_expr, right_expr)),
+                tac.Assign(
+                    target,
+                    getattr(tac, self.__class__.__name__)(left_expr, right_expr, origin=self),
+                ),
             ]
 
         right_id = next(variable_id)
         left_stmts, left_expr = _to_tac_basic_int(self.terms[0], variable_id)
+        right_origin = self.__class__(*self.terms[1:], location=self.terms[1].location)
         return [
-            *(self.__class__(*self.terms[1:]).to_tac(right_id, variable_id)),
+            *(right_origin.to_tac(right_id, variable_id)),
             *left_stmts,
             tac.Assign(
-                target, getattr(tac, self.__class__.__name__)(left_expr, tac.IntVar(right_id))
+                target,
+                getattr(tac, self.__class__.__name__)(
+                    left_expr,
+                    tac.IntVar(right_id, origin=right_origin),
+                    origin=self,
+                ),
             ),
         ]
 
 
 class Add(MathAssExpr):
     def _update_str(self) -> None:
         if not self.terms:
@@ -1015,15 +1057,19 @@
 
     def to_tac(self, target: StrID, variable_id: Generator[ID, None, None]) -> list[tac.Stmt]:
         left_stmts, left_expr = _to_tac_basic_int(self.left, variable_id)
         right_stmts, right_expr = _to_tac_basic_int(self.right, variable_id)
         return [
             *left_stmts,
             *right_stmts,
-            tac.Assign(target, getattr(tac, self.__class__.__name__)(left_expr, right_expr)),
+            tac.Assign(
+                target,
+                getattr(tac, self.__class__.__name__)(left_expr, right_expr, origin=self),
+                origin=self,
+            ),
         ]
 
 
 class Sub(MathBinExpr):
     @property
     def precedence(self) -> Precedence:
         return Precedence.BINARY_ADDING_OPERATOR
@@ -1240,19 +1286,25 @@
             return z3.BoolVal(True)
         if self.identifier == ID("False"):
             return z3.BoolVal(False)
         return z3.Int(self.name)
 
     def to_tac(self, target: StrID, variable_id: Generator[ID, None, None]) -> list[tac.Stmt]:
         if self.identifier == ID("True"):
-            return [tac.Assign(target, tac.BoolVal(True))]
+            return [tac.Assign(target, tac.BoolVal(True), origin=self)]
         if self.identifier == ID("False"):
-            return [tac.Assign(target, tac.BoolVal(False))]
+            return [tac.Assign(target, tac.BoolVal(False), origin=self)]
         assert self.type_ != rty.BOOLEAN
-        return [tac.Assign(target, tac.IntVar(self.name))]
+        return [
+            tac.Assign(
+                target,
+                tac.IntVar(self.name, origin=self),
+                origin=self,
+            )
+        ]
 
     def copy(
         self,
         identifier: Optional[StrID] = None,
         type_: Optional[rty.Type] = None,
         location: Optional[Location] = None,
     ) -> Literal:
@@ -1312,24 +1364,37 @@
         if self.type_ == rty.BOOLEAN:
             return z3.Bool(self.name)
         if self.negative:
             return -z3.Int(self.name)
         return z3.Int(self.name)
 
     def to_tac(self, target: StrID, variable_id: Generator[ID, None, None]) -> list[tac.Stmt]:
-        assert not isinstance(self.type_, rty.Undefined)
         if self.type_ == rty.BOOLEAN:
-            return [tac.Assign(target, tac.BoolVar(self.name))]
-        if isinstance(self.type_, rty.Integer):
-            return [tac.Assign(target, tac.IntVar(self.name, self.negative))]
-        if isinstance(self.type_, rty.Message):
-            return [tac.Assign(target, tac.MsgVar(self.name))]
-        if isinstance(self.type_, rty.Sequence):
-            return [tac.Assign(target, tac.SeqVar(self.name))]
-        assert False
+            return [
+                tac.Assign(
+                    target,
+                    tac.BoolVar(self.name, origin=self),
+                    origin=self,
+                )
+            ]
+        if isinstance(self.type_, (rty.Integer, rty.Enumeration)):
+            return [
+                tac.Assign(
+                    target,
+                    tac.IntVar(self.name, self.negative, origin=self),
+                    origin=self,
+                )
+            ]
+        return [
+            tac.Assign(
+                target,
+                tac.ObjVar(self.name, origin=self),
+                origin=self,
+            )
+        ]
 
     def copy(
         self,
         identifier: Optional[StrID] = None,
         negative: Optional[bool] = None,
         immutable: Optional[bool] = None,
         type_: Optional[rty.Type] = None,
@@ -1401,56 +1466,77 @@
         if not isinstance(self.prefix, (Variable, Literal, Selected)):
             raise Z3TypeError("illegal prefix of attribute")
         if self.negative:
             return -z3.Int(self.representation)
         return z3.Int(self.representation)
 
     def to_tac(self, target: StrID, variable_id: Generator[ID, None, None]) -> list[tac.Stmt]:
-        assert not isinstance(self.type_, rty.Undefined)
-        assert isinstance(self.prefix, (Variable, Literal, Selected))
-        if self.type_ == rty.BOOLEAN:
-            return [tac.Assign(target, tac.BoolVar(self.representation))]
-        return [tac.Assign(target, tac.IntVar(self.representation, self.negative))]
+        prefix_stmts, prefix_expr = _to_tac_basic_expr(self.prefix, variable_id)
+        assert isinstance(prefix_expr, tac.Var)
+        return [
+            *prefix_stmts,
+            tac.Assign(
+                target,
+                self._to_tac(prefix_expr.identifier),
+                origin=self,
+            ),
+        ]
+
+    @abstractmethod
+    def _to_tac(self, prefix: ID) -> tac.Expr:
+        raise NotImplementedError
 
 
 class Size(Attribute):
     def __init__(self, prefix: Union[StrID, Expr], negative: bool = False) -> None:
         super().__init__(prefix, negative)
         self.type_ = rty.UniversalInteger()
 
     def _check_type_subexpr(self) -> RecordFluxError:
         return self.prefix.check_type_instance(rty.Any)
 
+    def _to_tac(self, prefix: ID) -> tac.Expr:
+        return tac.Size(prefix)
+
 
 class Length(Attribute):
     def __init__(self, prefix: Union[StrID, Expr], negative: bool = False) -> None:
         super().__init__(prefix, negative)
         self.type_ = rty.UniversalInteger()
 
     def _check_type_subexpr(self) -> RecordFluxError:
         return self.prefix.check_type_instance(rty.Any)
 
+    def _to_tac(self, prefix: ID) -> tac.Expr:
+        return tac.Length(prefix)
+
 
 class First(Attribute):
     def __init__(self, prefix: Union[StrID, Expr], negative: bool = False) -> None:
         super().__init__(prefix, negative)
         self.type_ = rty.UniversalInteger()
 
     def _check_type_subexpr(self) -> RecordFluxError:
         return self.prefix.check_type_instance(rty.Any)
 
+    def _to_tac(self, prefix: ID) -> tac.Expr:
+        return tac.First(prefix)
+
 
 class Last(Attribute):
     def __init__(self, prefix: Union[StrID, Expr], negative: bool = False) -> None:
         super().__init__(prefix, negative)
         self.type_ = rty.UniversalInteger()
 
     def _check_type_subexpr(self) -> RecordFluxError:
         return self.prefix.check_type_instance(rty.Any)
 
+    def _to_tac(self, prefix: ID) -> tac.Expr:
+        return tac.Last(prefix)
+
 
 class ValidChecksum(Attribute):
     def __init__(self, prefix: Union[StrID, Expr], negative: bool = False) -> None:
         super().__init__(prefix, negative)
         self.type_ = rty.BOOLEAN
 
     def _check_type_subexpr(self) -> RecordFluxError:
@@ -1459,23 +1545,29 @@
     def z3expr(self) -> z3.BoolRef:
         return z3.Bool(self.representation)
 
     @property
     def representation(self) -> str:
         return f"{self.prefix}'Valid_Checksum"
 
+    def _to_tac(self, prefix: ID) -> tac.Expr:
+        return tac.ValidChecksum(prefix)
+
 
 class Valid(Attribute):
     def __init__(self, prefix: Union[StrID, Expr], negative: bool = False) -> None:
         super().__init__(prefix, negative)
         self.type_ = rty.BOOLEAN
 
     def _check_type_subexpr(self) -> RecordFluxError:
         return self.prefix.check_type_instance((rty.Sequence, rty.Message))
 
+    def _to_tac(self, prefix: ID) -> tac.Expr:
+        return tac.Valid(prefix)
+
 
 class Present(Attribute):
     def __init__(self, prefix: Union[StrID, Expr], negative: bool = False) -> None:
         super().__init__(prefix, negative)
         self.type_ = rty.BOOLEAN
 
     def _check_type_subexpr(self) -> RecordFluxError:
@@ -1491,27 +1583,33 @@
                         Severity.ERROR,
                         self.location,
                     )
                 ]
             )
         return error
 
+    def _to_tac(self, prefix: ID) -> tac.Expr:
+        return tac.Present(prefix)
+
 
 class HasData(Attribute):
     def __init__(self, prefix: Union[StrID, Expr], negative: bool = False) -> None:
         super().__init__(prefix, negative)
         self.type_ = rty.BOOLEAN
 
     @property
     def symbol(self) -> str:
         return "Has_Data"
 
     def _check_type_subexpr(self) -> RecordFluxError:
         return self.prefix.check_type_instance(rty.Message)
 
+    def _to_tac(self, prefix: ID) -> tac.Expr:
+        return tac.HasData(prefix)
+
 
 class Head(Attribute):
     def __init__(
         self, prefix: Union[StrID, Expr], negative: bool = False, type_: rty.Type = rty.Undefined()
     ):
         super().__init__(prefix, negative)
         self.type_ = type_
@@ -1532,30 +1630,39 @@
                         Severity.ERROR,
                         self.prefix.location,
                     )
                 ],
             )
         return error
 
+    def _to_tac(self, prefix: ID) -> tac.Expr:
+        return tac.Head(prefix)
+
 
 class Opaque(Attribute):
     def __init__(self, prefix: Union[StrID, Expr], negative: bool = False) -> None:
         super().__init__(prefix, negative)
         self.type_ = rty.OPAQUE
 
     def _check_type_subexpr(self) -> RecordFluxError:
         return self.prefix.check_type_instance((rty.Sequence, rty.Message))
 
+    def _to_tac(self, prefix: ID) -> tac.Expr:
+        return tac.Opaque(prefix)
+
 
 class Constrained(Attribute):
     """Only used by code generator and therefore provides minimum functionality."""
 
     def _check_type_subexpr(self) -> RecordFluxError:
         raise NotImplementedError
 
+    def _to_tac(self, prefix: ID) -> tac.Expr:
+        raise NotImplementedError
+
 
 class Val(Attribute):
     """Only used by code generator and therefore provides minimum functionality."""
 
     def __init__(
         self, prefix: Union[StrID, Expr], expression: Expr, negative: bool = False
     ) -> None:
@@ -1594,14 +1701,17 @@
         )
         assert isinstance(result, ada.Expr)
         return result
 
     def z3expr(self) -> z3.ExprRef:
         raise NotImplementedError
 
+    def _to_tac(self, prefix: ID) -> tac.Expr:
+        raise NotImplementedError
+
 
 @invariant(lambda self: len(self.elements) > 0)
 class Indexed(Name):
     """Only used by code generator and therefore provides minimum functionality."""
 
     def __init__(self, prefix: Expr, *elements: Expr, negative: bool = False) -> None:
         self.prefix = prefix
@@ -1714,28 +1824,48 @@
         if self.negative:
             return -z3.Int(self.representation)
         return z3.Int(self.representation)
 
     def to_tac(self, target: StrID, variable_id: Generator[ID, None, None]) -> list[tac.Stmt]:
         assert not isinstance(self.type_, rty.Undefined)
         stmts, msg = _to_tac_basic_expr(self.prefix, variable_id)
-        assert isinstance(msg, tac.MsgVar)
+        assert isinstance(msg, tac.ObjVar)
         if self.type_ == rty.BOOLEAN:
             return [
                 *stmts,
-                tac.Assign(target, tac.BoolFieldAccess(msg.identifier, self.selector)),
+                tac.Assign(
+                    target,
+                    tac.BoolFieldAccess(msg.identifier, self.selector, origin=self),
+                    origin=self,
+                ),
             ]
         if isinstance(self.type_, rty.Integer):
             return [
                 *stmts,
                 tac.Assign(
-                    target, tac.IntFieldAccess(msg.identifier, self.selector, self.negative)
+                    target,
+                    tac.IntFieldAccess(
+                        msg.identifier,
+                        self.selector,
+                        self.negative,
+                        origin=self,
+                    ),
+                    origin=self,
+                ),
+            ]
+        if isinstance(self.type_, (rty.Enumeration, rty.Sequence)):
+            return [
+                *stmts,
+                tac.Assign(
+                    target,
+                    tac.ObjFieldAccess(msg.identifier, self.selector, origin=self),
+                    origin=self,
                 ),
             ]
-        assert False
+        assert False, self.type_
 
     def copy(
         self,
         prefix: Optional[Expr] = None,
         selector: Optional[StrID] = None,
         negative: Optional[bool] = None,
         immutable: Optional[bool] = None,
@@ -1834,21 +1964,47 @@
             a_stmts, a_expr = _to_tac_basic_expr(a, variable_id)
             arguments_stmts.extend(a_stmts)
             arguments_exprs.append(a_expr)
 
         if self.type_ is rty.BOOLEAN:
             return [
                 *arguments_stmts,
-                tac.Assign(target, tac.BoolCall(self.identifier, *arguments_exprs)),
+                tac.Assign(
+                    target,
+                    tac.BoolCall(
+                        self.identifier,
+                        *arguments_exprs,
+                        origin=self,
+                    ),
+                    origin=self,
+                ),
+            ]
+
+        if isinstance(self.type_, rty.AnyInteger):
+            return [
+                *arguments_stmts,
+                tac.Assign(
+                    target,
+                    tac.IntCall(
+                        self.identifier,
+                        *arguments_exprs,
+                        origin=self,
+                    ),
+                    origin=self,
+                ),
             ]
 
-        assert isinstance(self.type_, rty.AnyInteger)
+        assert isinstance(self.type_, (rty.Enumeration, rty.Structure, rty.Message))
         return [
             *arguments_stmts,
-            tac.Assign(target, tac.IntCall(self.identifier, *arguments_exprs)),
+            tac.Assign(
+                target,
+                tac.ObjCall(self.identifier, *arguments_exprs, origin=self),
+                origin=self,
+            ),
         ]
 
     def variables(self) -> list[Variable]:
         result = [Variable(self.identifier, location=self.location)]
         for t in self.args:
             result.extend(t.variables())
         return result
@@ -1983,15 +2139,28 @@
     def ada_expr(self) -> ada.Expr:
         return ada.Aggregate(*[e.ada_expr() for e in self.elements])
 
     def z3expr(self) -> z3.ExprRef:
         return z3.BoolVal(False)
 
     def to_tac(self, target: StrID, variable_id: Generator[ID, None, None]) -> list[tac.Stmt]:
-        raise NotImplementedError
+        elements = []
+        stmts = []
+        for e in self.elements:
+            e_stmts, e_expr = _to_tac_basic_expr(e, variable_id)
+            elements.append(e_expr)
+            stmts.extend(e_stmts)
+        return [
+            *stmts,
+            tac.Assign(
+                target,
+                tac.Agg(*elements, origin=self),
+                origin=self,
+            ),
+        ]
 
 
 class String(Aggregate):
     def __init__(self, data: str, location: Optional[Location] = None) -> None:
         super().__init__(*[Number(ord(d)) for d in data], location=location)
         self.data = data
 
@@ -2099,16 +2268,20 @@
 
     def to_tac(self, target: StrID, variable_id: Generator[ID, None, None]) -> list[tac.Stmt]:
         left_stmts, left_expr = _to_tac_basic_int(self.left, variable_id)
         right_stmts, right_expr = _to_tac_basic_int(self.right, variable_id)
         return [
             *left_stmts,
             *right_stmts,
-            # pylint: disable-next = abstract-class-instantiated
-            tac.Assign(target, getattr(tac, self.__class__.__name__)(left_expr, right_expr)),
+            tac.Assign(
+                target,
+                # pylint: disable-next = abstract-class-instantiated
+                getattr(tac, self.__class__.__name__)(left_expr, right_expr, origin=self),
+                origin=self,
+            ),
         ]
 
 
 class Less(Relation):
     def __neg__(self) -> Expr:
         return GreaterEqual(self.left, self.right)
 
@@ -2433,26 +2606,44 @@
         if then_expression.type_ is rty.BOOLEAN and self.else_expression.type_ is rty.BOOLEAN:
             then_bool_stmts, then_bool_expr = _to_tac_basic_bool(then_expression, variable_id)
             else_bool_stmts, else_bool_expr = _to_tac_basic_bool(self.else_expression, variable_id)
             return [
                 *condition_stmts,
                 *then_bool_stmts,
                 *else_bool_stmts,
-                tac.Assign(target, tac.BoolIfExpr(condition_expr, then_bool_expr, else_bool_expr)),
+                tac.Assign(
+                    target,
+                    tac.BoolIfExpr(
+                        condition_expr,
+                        then_bool_expr,
+                        else_bool_expr,
+                        origin=self,
+                    ),
+                    origin=self,
+                ),
             ]
 
         assert isinstance(then_expression.type_, rty.AnyInteger)
         assert isinstance(self.else_expression.type_, rty.AnyInteger)
         then_int_stmts, then_int_expr = _to_tac_basic_int(then_expression, variable_id)
         else_int_stmts, else_int_expr = _to_tac_basic_int(self.else_expression, variable_id)
         return [
             *condition_stmts,
             *then_int_stmts,
             *else_int_stmts,
-            tac.Assign(target, tac.IntIfExpr(condition_expr, then_int_expr, else_int_expr)),
+            tac.Assign(
+                target,
+                tac.IntIfExpr(
+                    condition_expr,
+                    then_int_expr,
+                    else_int_expr,
+                    origin=self,
+                ),
+                origin=self,
+            ),
         ]
 
 
 class QuantifiedExpr(Expr):
     def __init__(
         self,
         parameter_identifier: StrID,
@@ -2732,15 +2923,23 @@
     def ada_expr(self) -> ada.Expr:
         return ada.Conversion(self.identifier, self.argument.ada_expr())
 
     def z3expr(self) -> z3.ExprRef:
         raise NotImplementedError
 
     def to_tac(self, target: StrID, variable_id: Generator[ID, None, None]) -> list[tac.Stmt]:
-        raise NotImplementedError
+        argument_stmts, argument_expr = _to_tac_basic_expr(self.argument, variable_id)
+        return [
+            *argument_stmts,
+            tac.Assign(
+                target,
+                tac.Conversion(self.identifier, argument_expr, origin=self),
+                origin=self,
+            ),
+        ]
 
     def variables(self) -> list[Variable]:
         return self.argument.variables()
 
 
 class QualifiedExpr(Expr):
     """Only used by code generator and therefore provides minimum functionality."""
@@ -2858,15 +3057,33 @@
     def ada_expr(self) -> ada.Expr:
         raise NotImplementedError
 
     def z3expr(self) -> z3.ExprRef:
         raise NotImplementedError
 
     def to_tac(self, target: StrID, variable_id: Generator[ID, None, None]) -> list[tac.Stmt]:
-        raise NotImplementedError
+        sequence_stmts, sequence_expr = _to_tac_basic_expr(self.sequence, variable_id)
+        selector_stmts, selector_expr = _to_tac_basic_expr(self.selector, variable_id)
+        condition_stmts, condition_expr = _to_tac_basic_bool(self.condition, variable_id)
+        return [
+            *sequence_stmts,
+            tac.Assign(
+                target,
+                tac.Comprehension(
+                    self.iterator,
+                    sequence_expr,
+                    selector_stmts,
+                    selector_expr,
+                    condition_stmts,
+                    condition_expr,
+                    origin=self,
+                ),
+                origin=self,
+            ),
+        ]
 
     def variables(self) -> list[Variable]:
         return [
             v
             for v in self.sequence.variables()
             + self.selector.variables()
             + self.condition.variables()
@@ -2891,24 +3108,41 @@
             ", ".join([f"{k} => {self.field_values[k]}" for k in self.field_values])
             if self.field_values
             else "null message"
         )
         self._str = intern(f"{self.identifier}'({field_values})")
 
     def _check_type_subexpr(self) -> RecordFluxError:
-        if not isinstance(self.type_, rty.Message):
-            error = RecordFluxError()
+        error = RecordFluxError()
 
+        if not isinstance(self.type_, rty.Message):
             for d in self.field_values.values():
                 error += d.check_type_instance(rty.Any)
 
             return error
 
+        return self._check_for_invalid_fields() + self._check_for_missing_fields()
+
+    def _field_combinations(self) -> set[tuple[str, ...]]:
+        assert isinstance(self.type_, rty.Message)
+
+        return set(self.type_.field_combinations)
+
+    def _matching_field_combinations(self, field_position: int) -> set[tuple[str, ...]]:
+        field = list(self.field_values)[field_position]
+        return {
+            c
+            for c in self._field_combinations()
+            if len(c) > field_position and c[field_position] == str(field)
+        }
+
+    def _check_for_invalid_fields(self) -> RecordFluxError:
+        assert isinstance(self.type_, rty.Message)
+
         error = RecordFluxError()
-        field_combinations = set(self.type_.field_combinations)
 
         for i, (field, expr) in enumerate(self.field_values.items()):
             if field not in self.type_.types:
                 error.extend(
                     [
                         (
                             f'invalid field "{field}" for {self.type_}',
@@ -2928,44 +3162,50 @@
                     r.field == field and expr.type_.is_compatible(r.sdu)
                     for r in self.type_.refinements
                 ):
                     error += expr.check_type(field_type)
             else:
                 error += expr.check_type(field_type)
 
-            field_combinations = {
-                c for c in field_combinations if len(c) > i and c[i] == str(field)
-            }
-
-            if not field_combinations:
+            if not self._matching_field_combinations(i):
                 error.extend(
                     [
                         (
                             f'invalid position for field "{field}" of {self.type_}',
                             Subsystem.MODEL,
                             Severity.ERROR,
                             field.location,
                         )
                     ],
                 )
                 break
 
-        if field_combinations and all(len(c) > len(self.field_values) for c in field_combinations):
+        return error
+
+    def _check_for_missing_fields(self) -> RecordFluxError:
+        error = RecordFluxError()
+
+        if self._field_combinations() and all(
+            len(c) > len(self.field_values) for c in self._field_combinations()
+        ):
             error.extend(
                 [
                     (
                         f"missing fields for {self.type_}",
                         Subsystem.MODEL,
                         Severity.ERROR,
                         self.location,
                     ),
                     (
                         "possible next fields: "
                         + ", ".join(
-                            unique(c[len(self.field_values)] for c in sorted(field_combinations))
+                            unique(
+                                c[len(self.field_values)]
+                                for c in sorted(self._field_combinations())
+                            )
                         ),
                         Subsystem.MODEL,
                         Severity.INFO,
                         self.location,
                     ),
                 ],
             )
@@ -2978,29 +3218,29 @@
     def findall(self, match: Callable[[Expr], bool]) -> Sequence[Expr]:
         return [
             *([self] if match(self) else []),
             *[e for v in self.field_values.values() for e in v.findall(match)],
         ]
 
     def simplified(self) -> Expr:
-        return MessageAggregate(
+        return self.__class__(
             self.identifier,
             {k: self.field_values[k].simplified() for k in self.field_values},
             self.type_,
             self.location,
         )
 
     def substituted(
         self,
         func: Optional[Callable[[Expr], Expr]] = None,
         mapping: Optional[Mapping[Name, Expr]] = None,
     ) -> Expr:
         func = substitution(mapping or {}, func)
         expr = func(self)
-        if isinstance(expr, MessageAggregate):
+        if isinstance(expr, self.__class__):
             return expr.__class__(
                 expr.identifier,
                 {k: expr.field_values[k].substituted(func) for k in expr.field_values},
                 type_=expr.type_,
                 location=expr.location,
             )
         return expr
@@ -3012,156 +3252,65 @@
     def ada_expr(self) -> ada.Expr:
         raise NotImplementedError
 
     def z3expr(self) -> z3.ExprRef:
         raise NotImplementedError
 
     def to_tac(self, target: StrID, variable_id: Generator[ID, None, None]) -> list[tac.Stmt]:
-        raise NotImplementedError
+        field_values = {}
+        stmts = []
+        for i, e in self.field_values.items():
+            e_stmts, e_expr = _to_tac_basic_expr(e, variable_id)
+            field_values[i] = e_expr
+            stmts.extend(e_stmts)
+        return [
+            *stmts,
+            tac.Assign(
+                target,
+                self._tac_expr(self.identifier, field_values, self),
+                origin=self,
+            ),
+        ]
 
     def variables(self) -> list[Variable]:
         result = []
         for v in self.field_values.values():
             result.extend(v.variables())
         return result
 
+    @property
+    def _tac_expr(self) -> Callable[[ID, dict[ID, tac.BasicExpr], tac.Origin], tac.Expr]:
+        return tac.MsgAgg
 
-class DeltaMessageAggregate(Expr):
-    """For internal use only."""
 
-    def __init__(
-        self,
-        identifier: StrID,
-        field_values: Mapping[StrID, Expr],
-        type_: rty.Type = rty.Undefined(),
-        location: Optional[Location] = None,
-    ) -> None:
-        super().__init__(type_, location)
-        self.identifier = ID(identifier)
-        self.field_values = {ID(k): v for k, v in field_values.items()}
+class DeltaMessageAggregate(MessageAggregate):
+    """For internal use only."""
 
     def _update_str(self) -> None:
         field_values = (
             ", ".join([f"{k} => {self.field_values[k]}" for k in self.field_values])
             if self.field_values
             else "null message"
         )
         self._str = intern(f"{self.identifier} with delta {field_values}")
 
-    def _check_type_subexpr(self) -> RecordFluxError:
-        error = RecordFluxError()
-
-        if not isinstance(self.type_, rty.Message):
-            for d in self.field_values.values():
-                error += d.check_type_instance(rty.Any)
-
-            return error
-
-        field_combinations = set(self.type_.field_combinations)
-        fields: tuple[str, ...] = ()
-
-        for i, (field, expr) in enumerate(self.field_values.items()):
-            if field not in self.type_.fields:
-                error.extend(
-                    [
-                        (
-                            f'invalid field "{field}" for {self.type_}',
-                            Subsystem.MODEL,
-                            Severity.ERROR,
-                            field.location,
-                        ),
-                        *_similar_field_names(field, self.type_.fields, field.location),
-                    ]
-                )
-                continue
-
-            field_type = self.type_.types[field]
-
-            if field_type == rty.OPAQUE:
-                if not any(
-                    r.field == field and expr.type_.is_compatible(r.sdu)
-                    for r in self.type_.refinements
-                ):
-                    error += expr.check_type(field_type)
-            else:
-                error += expr.check_type(field_type)
-
-            fields = (*fields, str(field))
-            field_combinations = {
-                c
-                for c in field_combinations
-                if any(fields == c[i : len(fields) + i] for i in range(len(c) - len(fields) + 1))
-            }
-
-            if not field_combinations:
-                error.extend(
-                    [
-                        (
-                            f'invalid position for field "{field}" of {self.type_}',
-                            Subsystem.MODEL,
-                            Severity.ERROR,
-                            field.location,
-                        )
-                    ],
-                )
-                break
-
-        return error
-
-    def __neg__(self) -> Expr:
-        raise NotImplementedError
-
-    def findall(self, match: Callable[[Expr], bool]) -> Sequence[Expr]:
-        return [
-            *([self] if match(self) else []),
-            *[e for v in self.field_values.values() for e in v.findall(match)],
-        ]
-
-    def simplified(self) -> Expr:
-        return DeltaMessageAggregate(
-            self.identifier,
-            {k: self.field_values[k].simplified() for k in self.field_values},
-            self.type_,
-            self.location,
-        )
-
-    def substituted(
-        self,
-        func: Optional[Callable[[Expr], Expr]] = None,
-        mapping: Optional[Mapping[Name, Expr]] = None,
-    ) -> Expr:
-        func = substitution(mapping or {}, func)
-        expr = func(self)
-        if isinstance(expr, DeltaMessageAggregate):
-            return expr.__class__(
-                expr.identifier,
-                {k: expr.field_values[k].substituted(func) for k in expr.field_values},
-                type_=expr.type_,
-                location=expr.location,
-            )
-        return expr
-
     @property
-    def precedence(self) -> Precedence:
-        raise NotImplementedError
-
-    def ada_expr(self) -> ada.Expr:
-        raise NotImplementedError
+    def _tac_expr(self) -> Callable[[ID, dict[ID, tac.BasicExpr], tac.Origin], tac.Expr]:
+        return tac.DeltaMsgAgg
 
-    def z3expr(self) -> z3.ExprRef:
-        raise NotImplementedError
-
-    def to_tac(self, target: StrID, variable_id: Generator[ID, None, None]) -> list[tac.Stmt]:
-        raise NotImplementedError
+    def _matching_field_combinations(self, field_position: int) -> set[tuple[str, ...]]:
+        fields = tuple(str(f) for i, f in enumerate(self.field_values) if i <= field_position)
+        return {
+            c
+            for c in self._field_combinations()
+            if any(fields == c[i : len(fields) + i] for i in range(len(c) - len(fields) + 1))
+        }
 
-    def variables(self) -> list[Variable]:
-        result = []
-        for v in self.field_values.values():
-            result.extend(v.variables())
-        return result
+    def _check_for_missing_fields(self) -> RecordFluxError:
+        return RecordFluxError()
 
 
 def substitution(
     mapping: Mapping[Name, Expr], func: Optional[Callable[[Expr], Expr]] = None
 ) -> Callable[[Expr], Expr]:
     if func:
         return func
@@ -3470,15 +3619,37 @@
         ]
         return ada.CaseExpr(self.expr.ada_expr(), choices)
 
     def z3expr(self) -> z3.ExprRef:
         raise NotImplementedError
 
     def to_tac(self, target: StrID, variable_id: Generator[ID, None, None]) -> list[tac.Stmt]:
-        raise NotImplementedError
+        expression_stmts, expression_expr = _to_tac_basic_expr(self.expr, variable_id)
+        choices = []
+        for choice, expr in self.choices:
+            e_stmts, e_expr = _to_tac_basic_expr(expr, variable_id)
+            choices.append(
+                (
+                    [tac.EnumLit(c) if isinstance(c, ID) else tac.IntVal(int(c)) for c in choice],
+                    e_stmts,
+                    e_expr,
+                )
+            )
+        return [
+            *expression_stmts,
+            tac.Assign(
+                target,
+                tac.CaseExpr(
+                    expression_expr,
+                    choices,
+                    origin=self,
+                ),
+                origin=self,
+            ),
+        ]
 
     def variables(self) -> list[Variable]:
         simplified = self.simplified()
         assert isinstance(simplified, CaseExpr)
         return list(
             unique(
                 [
@@ -3506,54 +3677,51 @@
                 Severity.INFO,
                 location,
             )
         ]
     return []
 
 
-def var_id_gen() -> Generator[ID, None, None]:
-    i = 0
-    while True:
-        yield ID(f"T_{i}")
-        i += 1
-
-
 def _to_tac_basic_int(
     expression: Expr, variable_id: Generator[ID, None, None]
 ) -> tuple[list[tac.Stmt], tac.BasicIntExpr]:
+    assert isinstance(expression.type_, (rty.AnyInteger, rty.Enumeration))
+
     result_id = next(variable_id)
     result_stmts = expression.to_tac(result_id, variable_id)
     if (
         len(result_stmts) == 1
         and isinstance(result_stmts[0], tac.Assign)
         and isinstance(result_stmts[0].expression, tac.BasicExpr)
     ):
         assert isinstance(result_stmts[0].expression, tac.BasicIntExpr)
         result_expr = result_stmts[0].expression
         result_stmts = []
     else:
-        result_expr = tac.IntVar(result_id)
+        result_expr = tac.IntVar(result_id, origin=expression)
     return (result_stmts, result_expr)
 
 
 def _to_tac_basic_bool(
     expression: Expr, variable_id: Generator[ID, None, None]
 ) -> tuple[list[tac.Stmt], tac.BasicBoolExpr]:
+    assert expression.type_ == rty.BOOLEAN
+
     result_id = next(variable_id)
     result_stmts = expression.to_tac(result_id, variable_id)
     if (
         len(result_stmts) == 1
         and isinstance(result_stmts[0], tac.Assign)
         and isinstance(result_stmts[0].expression, tac.BasicExpr)
     ):
         assert isinstance(result_stmts[0].expression, tac.BasicBoolExpr)
         result_expr = result_stmts[0].expression
         result_stmts = []
     else:
-        result_expr = tac.BoolVar(result_id)
+        result_expr = tac.BoolVar(result_id, origin=expression)
     return (result_stmts, result_expr)
 
 
 def _to_tac_basic_expr(
     expression: Expr, variable_id: Generator[ID, None, None]
 ) -> tuple[list[tac.Stmt], tac.BasicExpr]:
     result_id = next(variable_id)
@@ -3565,12 +3733,14 @@
     ):
         result_expr = result_stmts[0].expression
         result_stmts = []
     else:
         assign = result_stmts[-1]
         assert isinstance(assign, tac.Assign)
         if isinstance(assign.expression, tac.BoolExpr):
-            result_expr = tac.BoolVar(result_id)
+            result_expr = tac.BoolVar(result_id, origin=expression)
+        elif isinstance(assign.expression, tac.IntExpr):
+            result_expr = tac.IntVar(result_id, origin=expression)
         else:
-            assert isinstance(assign.expression, tac.IntExpr)
-            result_expr = tac.IntVar(result_id)
+            assert isinstance(assign.expression, tac.Expr)
+            result_expr = tac.ObjVar(result_id, origin=expression)
     return (result_stmts, result_expr)
```

### Comparing `RecordFlux-0.9.0/rflx/generator/allocator.py` & `RecordFlux-0.9.1/rflx/generator/allocator.py`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/generator/common.py` & `RecordFlux-0.9.1/rflx/generator/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,15 +296,15 @@
             expr.Literal(t.package * l): type_conversion(
                 expr.Call("To_Base_Integer", [expr.Variable(prefix * t.package * l)])
             )
             for t in message.types.values()
             if isinstance(t, model.Enumeration) and t != model.BOOLEAN
             for l in t.literals.keys()
         },
-        # https://github.com/Componolit/RecordFlux/issues/276
+        # Eng/RecordFlux/RecordFlux#276
         **{expr.ValidChecksum(f): expr.TRUE for f in message.checksums},
     }
 
 
 def message_structure_invariant(
     message: model.Message, prefix: str, link: Optional[model.Link] = None, embedded: bool = False
 ) -> Expr:
@@ -755,15 +755,15 @@
     field: model.Field, reset_written_last: bool = False
 ) -> list[Statement]:
     return [
         CallStatement(
             "Reset_Dependent_Fields",
             [Variable("Ctx"), Variable(field.affixed_name)],
         ),
-        # https://github.com/Componolit/RecordFlux/issues/868
+        # Eng/RecordFlux/RecordFlux#868
         PragmaStatement(
             "Warnings",
             [
                 Variable("Off"),
                 String("attribute Update is an obsolescent feature"),
             ],
         ),
```

### Comparing `RecordFlux-0.9.0/rflx/generator/const.py` & `RecordFlux-0.9.1/rflx/generator/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,10 +64,10 @@
 TYPES_LOW_ORDER_FIRST = TYPES * "Low_Order_First"
 TYPES_OPERATIONS = TYPES_OPERATIONS_PACKAGE
 
 UNREACHABLE = ada.Call(TYPES * "Unreachable")
 
 CONFIGURATION_PRAGMAS = [
     ada.Pragma("Style_Checks", [ada.String("N3aAbCdefhiIklnOprStux")]),
-    # https://github.com/Componolit/RecordFlux/issues/508
+    # Eng/RecordFlux/RecordFlux#508
     ada.Pragma("Warnings", [ada.Variable("Off"), ada.String("redundant conversion")]),
 ]
```

### Comparing `RecordFlux-0.9.0/rflx/generator/generator.py` & `RecordFlux-0.9.1/rflx/generator/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
             create_file(
                 directory / filename,
                 self._license_header()
                 + "\n".join(
                     [
                         l.format(prefix=prefix)
                         for l in template_file.split("\n")
-                        if "/Workarounds/" not in l
+                        if "/Workarounds#" not in l
                     ]
                 ),
             )
 
         if self._debug == common.Debug.EXTERNAL:
             debug_package_id = self._prefix * ID("RFLX_Debug")
             create_file(
@@ -228,15 +228,15 @@
                 unit = self._create_unit(t.package, terminating=False)
                 units[t.package] = unit
 
             if isinstance(t, (Scalar, Composite)):
                 units.update(self._create_type(t, t.package, units))
 
             elif isinstance(t, Message):
-                # https://github.com/Componolit/RecordFlux/issues/276
+                # Eng/RecordFlux/RecordFlux#276
                 for c in t.checksums:
                     if not self._ignore_unsupported_checksum:
                         fail(
                             "unsupported checksum (consider --ignore-unsupported-checksum option)",
                             Subsystem.GENERATOR,
                             location=c.location,
                         )
@@ -725,15 +725,15 @@
     def _create_sequence(self, sequence_type: Sequence) -> dict[ID, Unit]:
         context, package = common.create_sequence_instantiation(sequence_type, self._prefix)
         return {
             package.identifier: self._create_instantiation_unit(
                 [
                     Pragma("SPARK_Mode"),
                     *context,
-                    # https://github.com/Componolit/Workarounds/issues/33
+                    # Eng/RecordFlux/Workarounds#33
                     # A compiler error about a non-visible declaration of RFLX_Types inside the
                     # generic sequence package is prevented by adding a with-clause for this
                     # package.
                     Pragma(
                         "Warnings",
                         [Variable("Off"), String('unit "*RFLX_Types" is not referenced')],
                     ),
```

### Comparing `RecordFlux-0.9.0/rflx/generator/message.py` & `RecordFlux-0.9.1/rflx/generator/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,25 +308,25 @@
         ],
     )
 
     return UnitPart(
         [],
         [],
         [
-            # https://github.com/Componolit/Workarounds/issues/36
+            # Eng/RecordFlux/Workarounds#36
             # An access constant type cannot be used here, because the "implicit conversion
             # between access types with different designated types is not yet supported".
             Pragma(
                 "Warnings",
                 [
                     Variable("Off"),
                     String('"Buffer" is not modified, could be of access constant type'),
                 ],
             ),
-            # https://github.com/Componolit/Workarounds/issues/47
+            # Eng/RecordFlux/Workarounds#47
             Pragma(
                 "Warnings",
                 [Variable("Off"), String("postcondition does not mention function result")],
             ),
             ExpressionFunctionDeclaration(
                 specification,
                 common.context_predicate(message, composite_fields, prefix),
@@ -686,15 +686,15 @@
 
 def create_initialized_function(prefix: str, message: Message) -> UnitPart:
     specification = FunctionSpecification("Initialized", "Boolean", [Parameter(["Ctx"], "Context")])
     first_field = message.fields[0]
 
     return UnitPart(
         [
-            # https://github.com/Componolit/Workarounds/issues/47
+            # Eng/RecordFlux/Workarounds#47
             Pragma(
                 "Warnings",
                 [Variable("Off"), String("postcondition does not mention function result")],
             ),
             SubprogramDeclaration(specification, [Postcondition(TRUE)]),
             Pragma(
                 "Warnings",
@@ -1079,15 +1079,15 @@
             ExpressionFunctionDeclaration(
                 FunctionSpecification(
                     "Always_Valid",
                     "Boolean",
                     [Parameter(["Buffer"], const.TYPES_BYTES)],
                 ),
                 TRUE,
-                # https://github.com/Componolit/Workarounds/issues/48
+                # Eng/RecordFlux/Workarounds#48
                 # Ghost entities are not allowed as formal generic parameters.
                 # aspects=[Ghost()],
             ),
             Pragma(
                 "Warnings",
                 [Variable("On"), String('unused variable "*"')],
             ),
@@ -1181,15 +1181,15 @@
                     "Boolean",
                     [
                         Parameter(["Context_Buffer_Length"], const.TYPES_LENGTH),
                         Parameter(["Offset"], const.TYPES_LENGTH),
                     ],
                 ),
                 TRUE,
-                # https://github.com/Componolit/Workarounds/issues/48
+                # Eng/RecordFlux/Workarounds#48
                 # Ghost entities are not allowed as formal generic parameters.
                 # aspects=[Ghost()],
             ),
             Pragma(
                 "Warnings",
                 [Variable("On"), String('unused variable "*"')],
             ),
@@ -1297,15 +1297,15 @@
                                 Last("Ctx.Buffer"),
                             ),
                             Variable("Length"),
                             Length("Ctx.Buffer"),
                             Variable("Offset"),
                         ],
                     ),
-                    # https://github.com/Componolit/Workarounds/issues/39
+                    # Eng/RecordFlux/Workarounds#39
                     # Improve the check message in case of a wrong instantiation of "Write".
                     PragmaStatement(
                         "Assert",
                         [
                             LessEqual(
                                 Variable("Length"),
                                 Length(
@@ -1355,15 +1355,15 @@
             Parameter(["Fld" if scalar_fields else "Unused_Fld"], "Field"),
             Parameter(["Val" if scalar_fields else "Unused_Val"], const.TYPES_BASE_INT),
         ],
     )
 
     return UnitPart(
         [
-            # https://github.com/Componolit/Workarounds/issues/47
+            # Eng/RecordFlux/Workarounds#47
             Pragma(
                 "Warnings",
                 [Variable("Off"), String("postcondition does not mention function result")],
             ),
             SubprogramDeclaration(
                 specification,
                 [Postcondition(TRUE)],
@@ -1441,15 +1441,15 @@
         "Path_Condition",
         "Boolean",
         [Parameter(["Ctx"], "Context"), Parameter(["Fld"], "Field")],
     )
 
     return UnitPart(
         [
-            # https://github.com/Componolit/Workarounds/issues/47
+            # Eng/RecordFlux/Workarounds#47
             Pragma(
                 "Warnings",
                 [Variable("Off"), String("postcondition does not mention function result")],
             ),
             SubprogramDeclaration(
                 specification,
                 [
@@ -1617,15 +1617,15 @@
         "Field_First",
         const.TYPES_BIT_INDEX,
         [Parameter(["Ctx"], "Context"), Parameter(["Fld"], "Field")],
     )
 
     return UnitPart(
         [
-            # https://github.com/Componolit/Workarounds/issues/47
+            # Eng/RecordFlux/Workarounds#47
             Pragma(
                 "Warnings",
                 [Variable("Off"), String("postcondition does not mention function result")],
             ),
             SubprogramDeclaration(
                 specification,
                 [
@@ -1759,15 +1759,15 @@
                             [
                                 expr.Variable("Ctx"),
                                 expr.Variable(field.affixed_name, immutable=True),
                             ],
                         )
                     ],
                 ),
-                # https://github.com/Componolit/RecordFlux/issues/276
+                # Eng/RecordFlux/RecordFlux#276
                 **{expr.ValidChecksum(f): expr.TRUE for f in message.checksums},
             }
         )
         if isinstance(message.field_types[field], Scalar):
             c = c.substituted(
                 lambda x: expr.Variable("Val") if x == expr.Variable(field.name) else x
             )
@@ -1799,15 +1799,15 @@
         ),
     ]
 
     specification = FunctionSpecification("Field_Condition", "Boolean", parameters)
 
     return UnitPart(
         [
-            # https://github.com/Componolit/Workarounds/issues/47
+            # Eng/RecordFlux/Workarounds#47
             Pragma(
                 "Warnings",
                 [Variable("Off"), String("postcondition does not mention function result")],
             ),
             SubprogramDeclaration(
                 specification,
                 [
@@ -1863,15 +1863,15 @@
         "Predecessor",
         "Virtual_Field",
         [Parameter(["Ctx"], "Context"), Parameter(["Fld"], "Virtual_Field")],
     )
 
     return UnitPart(
         [
-            # https://github.com/Componolit/Workarounds/issues/47
+            # Eng/RecordFlux/Workarounds#47
             Pragma(
                 "Warnings",
                 [Variable("Off"), String("postcondition does not mention function result")],
             ),
             SubprogramDeclaration(specification, [Postcondition(TRUE)]),
             Pragma(
                 "Warnings",
@@ -1907,15 +1907,15 @@
         "Virtual_Field",
         [Parameter(["Ctx"], "Context"), Parameter(["Fld"], "Field")],
     )
 
     return UnitPart(
         [],
         [
-            # https://github.com/Componolit/Workarounds/issues/31
+            # Eng/RecordFlux/Workarounds#31
             Pragma("Warnings", [Variable("Off"), String("precondition is always False")]),
             ExpressionFunctionDeclaration(
                 specification,
                 Case(
                     Variable("Fld"),
                     [
                         (
@@ -2038,15 +2038,15 @@
         "Valid_Predecessor",
         "Boolean",
         [Parameter(["Ctx"], "Context"), Parameter(["Fld"], "Virtual_Field")],
     )
 
     return UnitPart(
         [
-            # https://github.com/Componolit/Workarounds/issues/47
+            # Eng/RecordFlux/Workarounds#47
             Pragma(
                 "Warnings",
                 [Variable("Off"), String("postcondition does not mention function result")],
             ),
             SubprogramDeclaration(specification, [Postcondition(TRUE)]),
             Pragma(
                 "Warnings",
@@ -3187,15 +3187,15 @@
     ]
     conditions = [
         condition
         for path in message.paths(FINAL)
         for link in path
         for condition in [
             link.condition.substituted(
-                # https://github.com/Componolit/RecordFlux/issues/276
+                # Eng/RecordFlux/RecordFlux#276
                 mapping={expr.ValidChecksum(f): expr.TRUE for f in message.checksums},
             )
             .substituted(_struct_substitution(message))
             .substituted(common.substitution(message, prefix))
             .simplified()
             .ada_expr()
         ]
```

### Comparing `RecordFlux-0.9.0/rflx/generator/parser.py` & `RecordFlux-0.9.1/rflx/generator/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,15 +345,15 @@
             )
             if scalar_fields and composite_fields
             else set_context_cursor_scalar()
             if scalar_fields and not composite_fields
             else set_context_cursor_composite_field("Fld"),
             *(
                 [
-                    # https://github.com/Componolit/RecordFlux/issues/664
+                    # Eng/RecordFlux/RecordFlux#664
                     # The provability of the context predicate is increased by splitting the
                     # assignment into multiple statements.
                     Assignment(
                         Indexed(
                             Variable("Ctx.Cursors"),
                             Call(
                                 "Successor",
@@ -759,15 +759,15 @@
     def create_incomplete_message_function() -> UnitPart:
         specification = FunctionSpecification(
             "Incomplete_Message", "Boolean", [Parameter(["Ctx"], "Context")]
         )
 
         return UnitPart(
             [
-                # https://github.com/Componolit/Workarounds/issues/47
+                # Eng/RecordFlux/Workarounds#47
                 Pragma(
                     "Warnings",
                     [Variable("Off"), String("postcondition does not mention function result")],
                 ),
                 SubprogramDeclaration(specification, [Postcondition(TRUE)]),
                 Pragma(
                     "Warnings",
@@ -806,15 +806,15 @@
             return Call(
                 "To_Actual",
                 [Selected(Indexed(Variable("Ctx.Cursors"), Variable(field.affixed_name)), "Value")],
             )
 
         return UnitPart(
             [
-                # https://github.com/Componolit/Workarounds/issues/31
+                # Eng/RecordFlux/Workarounds#31
                 Pragma("Warnings", [Variable("Off"), String("precondition is always False")]),
                 *[
                     SubprogramDeclaration(
                         specification(f, t),
                         [
                             Precondition(
                                 Call(
```

### Comparing `RecordFlux-0.9.0/rflx/generator/serializer.py` & `RecordFlux-0.9.1/rflx/generator/serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
                 Parameter(["Fld"], "Field"),
                 Parameter(["Length"], const.TYPES_LENGTH),
             ],
         )
 
         return UnitPart(
             [
-                # https://github.com/Componolit/Workarounds/issues/47
+                # Eng/RecordFlux/Workarounds#47
                 Pragma(
                     "Warnings",
                     [Variable("Off"), String("postcondition does not mention function result")],
                 ),
                 SubprogramDeclaration(
                     specification,
                     [
@@ -1868,15 +1868,15 @@
                 ),
                 Size(const.TYPES_BYTE),
             )
         )
         return [
             # Improve provability of context predicate
             PragmaStatement("Assert", [Equal(Mod(last, Size(const.TYPES_BYTE)), Number(0))]),
-            # https://github.com/Componolit/RecordFlux/issues/868
+            # Eng/RecordFlux/RecordFlux#868
             PragmaStatement(
                 "Warnings",
                 [
                     Variable("Off"),
                     String("attribute Update is an obsolescent feature"),
                 ],
             ),
```

### Comparing `RecordFlux-0.9.0/rflx/generator/session.py` & `RecordFlux-0.9.1/rflx/generator/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,18 +211,15 @@
 
     def _create_context(self) -> tuple[list[ContextItem], list[ContextItem]]:
         declaration_context: list[ContextItem] = []
 
         if self._allocator.required:
             declaration_context.append(WithClause(self._prefix * self._allocator.unit_identifier))
 
-        if any(
-            t.parent not in [INTERNAL_PACKAGE, BUILTINS_PACKAGE]
-            for t in [*self._session_context.used_types, *self._session_context.used_types_body]
-        ):
+        if any(t.parent == const.TYPES for t in self._session_context.used_types):
             declaration_context.append(WithClause(self._prefix * const.TYPES_PACKAGE))
 
         body_context: list[ContextItem] = [
             *(
                 [
                     WithClause(self._prefix * ID("RFLX_Debug"))
                     if self._debug == common.Debug.EXTERNAL
@@ -258,14 +255,22 @@
                     ]
                 )
 
         body_context.extend(
             [WithClause(self._prefix * p) for p in self._session_context.referenced_packages_body],
         )
 
+        if any(
+            t.parent == const.TYPES
+            for t in (
+                set(self._session_context.used_types_body) - set(self._session_context.used_types)
+            )
+        ):
+            body_context.append(WithClause(self._prefix * const.TYPES_PACKAGE))
+
         for type_identifier in self._session_context.used_types_body:
             if type_identifier.parent in [INTERNAL_PACKAGE, BUILTINS_PACKAGE]:
                 continue
             if type_identifier in self._session_context.used_types:
                 continue
             if type_identifier in [
                 const.TYPES_LENGTH,
@@ -2119,21 +2124,21 @@
         target_type: rty.Type,
         expression: expr.Expr,
         exception_handler: ExceptionHandler,
         is_global: Callable[[ID], bool],
         state: ID,
         alloc_id: Optional[Location],
     ) -> Sequence[Statement]:
-        if isinstance(expression, expr.MessageAggregate):
-            return self._assign_to_message_aggregate(
+        if isinstance(expression, expr.DeltaMessageAggregate):
+            return self._assign_to_delta_message_aggregate(
                 target, expression, exception_handler, is_global, state
             )
 
-        if isinstance(expression, expr.DeltaMessageAggregate):
-            return self._assign_to_delta_message_aggregate(
+        if isinstance(expression, expr.MessageAggregate):
+            return self._assign_to_message_aggregate(
                 target, expression, exception_handler, is_global, state
             )
 
         if isinstance(target_type, rty.Message):
             for v in expression.findall(
                 lambda x: isinstance(x, expr.Variable) and x.identifier == target
             ):
@@ -2266,15 +2271,15 @@
                     ],
                     f'access to invalid field "{selector}" of' f' "{message_context}"',
                     exception_handler,
                 )
             ]
 
         if isinstance(selected.type_, rty.Sequence):
-            # https://github.com/Componolit/RecordFlux/issues/577
+            # Eng/RecordFlux/RecordFlux#577
             # The relevant buffer part has to be copied from the message context into a
             # sequence context. With the current implementation the sequence needs to
             # be parsed after copying. It must be ensured that the sequence is not
             # accidentally parsed beyond the original end of the sequence in the message
             # (i.e. misinterpreting trailing bytes in the new buffer as sequence elements).
             fail(
                 "copying of sequence not yet supported",
@@ -2982,15 +2987,15 @@
                         ),
                         -expr.Number(2),
                     ),
                 )
                 type_identifier = self._ada_type(a.prefix.type_.identifier)
                 local_declarations.extend(
                     [
-                        # https://github.com/Componolit/RecordFlux/issues/917
+                        # Eng/RecordFlux/RecordFlux#917
                         # The use of intermediate buffers should be removed.
                         ObjectDeclaration(
                             [argument_name],
                             Slice(
                                 Variable(const.TYPES_BYTES),
                                 First(const.TYPES_INDEX),
                                 Add(
@@ -3056,15 +3061,15 @@
                         -expr.Number(2),
                     ),
                 )
                 type_identifier = self._ada_type(a.prefix.type_.identifier)
                 message_context = context_id(a.prefix.identifier, is_global)
                 local_declarations.extend(
                     [
-                        # https://github.com/Componolit/RecordFlux/issues/917
+                        # Eng/RecordFlux/RecordFlux#917
                         # The use of intermediate buffers should be removed.
                         ObjectDeclaration(
                             [argument_name],
                             Slice(
                                 Variable(const.TYPES_BYTES),
                                 First(const.TYPES_INDEX),
                                 Add(
@@ -3514,34 +3519,40 @@
             # pylint: disable = too-many-branches, too-many-return-statements
             if isinstance(expression, (expr.Relation, expr.MathBinExpr)):
                 for e in [expression.left, expression.right]:
                     if isinstance(e.type_, rty.Integer) or (
                         isinstance(e.type_, rty.Enumeration) and not e.type_.always_valid
                     ):
                         self._session_context.used_types_body.append(e.type_.identifier)
+                        self._session_context.referenced_types_body.append(e.type_.identifier)
 
             if isinstance(expression, expr.MathAssExpr):
                 for e in expression.terms:
                     if isinstance(e.type_, (rty.Integer, rty.Enumeration)):
                         self._session_context.used_types_body.append(e.type_.identifier)
 
             if isinstance(expression, expr.And):
                 return expr.AndThen(*expression.terms)
 
             if isinstance(expression, expr.Or):
                 return expr.OrElse(*expression.terms)
 
             if isinstance(expression, expr.Selected):
                 if isinstance(expression.prefix, expr.Variable):
-                    assert isinstance(expression.prefix.type_, rty.Message)
+                    assert isinstance(expression.prefix.type_, (rty.Message, rty.Structure))
                     if expression.selector in expression.prefix.type_.parameter_types:
                         return expr.Selected(
                             expr.Variable(context_id(expression.prefix.identifier, is_global)),
                             expression.selector,
                         )
+                    if isinstance(expression.prefix.type_, rty.Structure):
+                        return expr.Selected(
+                            expr.Variable(expression.prefix.identifier),
+                            expression.selector,
+                        )
                     return expr.Call(
                         expression.prefix.type_.identifier * f"Get_{expression.selector}",
                         [expr.Variable(context_id(expression.prefix.identifier, is_global))],
                     )
 
                 assert False
 
@@ -4530,15 +4541,15 @@
         sequence_identifier: ID,
         sequence_type: ID,
         statements: Callable[[ExceptionHandler], Sequence[Statement]],
         exception_handler: ExceptionHandler,
         is_global: Callable[[ID], bool],
         alloc_id: Optional[Location],
     ) -> IfStatement:
-        # https://github.com/Componolit/RecordFlux/issues/577
+        # Eng/RecordFlux/RecordFlux#577
         sequence_context = context_id(sequence_identifier, is_global)
         take_buffer = self._take_buffer(copy_id(sequence_identifier), sequence_type, is_global)
         free_buffer = self._free_buffer(copy_id(sequence_identifier), alloc_id)
 
         return self._if_valid_sequence(
             sequence_type,
             sequence_context,
@@ -4583,15 +4594,15 @@
         sequence_type: ID,
         statements: Callable[[ExceptionHandler], Sequence[Statement]],
         target_buffer_is_smaller: bool,
         exception_handler: ExceptionHandler,
         is_global: Callable[[ID], bool],
         alloc_id: Optional[Location],
     ) -> Declare:
-        # https://github.com/Componolit/RecordFlux/issues/577
+        # Eng/RecordFlux/RecordFlux#577
         take_buffer = self._take_buffer(sequence_identifier, sequence_type, is_global)
         free_buffer = self._free_buffer(sequence_identifier, alloc_id)
         local_exception_handler = exception_handler.copy(free_buffer)
         return Declare(
             self._declare_context_buffer(sequence_identifier, sequence_type, is_global),
             [
                 *self._allocate_buffer(sequence_identifier, alloc_id),
@@ -5051,15 +5062,15 @@
     @staticmethod
     def _take_buffer(
         identifier: ID, type_: ID, is_global: Callable[[ID], bool], buf: Optional[ID] = None
     ) -> Sequence[Statement]:
         context = context_id(identifier, is_global)
         buf = buf or buffer_id(identifier)
         return [
-            # https://github.com/Componolit/Workarounds/issues/32
+            # Eng/RecordFlux/Workarounds#32
             PragmaStatement(
                 "Warnings",
                 [
                     Variable("Off"),
                     String(
                         f'"{context.ada_str}" is set by "Take_Buffer" but not used after the call'
                     ),
@@ -5084,15 +5095,15 @@
         ]
 
     @staticmethod
     def _update_context(
         sequence_context: ID, element_context: ID, sequence_type: ID
     ) -> Sequence[Statement]:
         return [
-            # https://github.com/Componolit/Workarounds/issues/32
+            # Eng/RecordFlux/Workarounds#32
             PragmaStatement(
                 "Warnings",
                 [
                     Variable("Off"),
                     String(
                         f'"{element_context.ada_str}" is set by "Update" '
                         f"but not used after the call"
```

### Comparing `RecordFlux-0.9.0/rflx/graph.py` & `RecordFlux-0.9.1/rflx/graph.py`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/identifier.py` & `RecordFlux-0.9.1/rflx/identifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import re
-from collections.abc import Sequence
+from collections.abc import Generator, Sequence
 from typing import Optional, TypeVar, Union
 
 from rflx.error import Location, RecordFluxError, Severity, Subsystem, fatal_fail
 
 Self = TypeVar("Self", bound="ID")
 
 
@@ -116,7 +116,14 @@
 
     @property
     def ada_str(self) -> str:
         return ".".join(self.parts)
 
 
 StrID = Union[str, ID]
+
+
+def id_generator() -> Generator[ID, None, None]:
+    i = 0
+    while True:
+        yield ID(f"T_{i}")
+        i += 1
```

### Comparing `RecordFlux-0.9.0/rflx/integration.py` & `RecordFlux-0.9.1/rflx/integration.py`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/model/__init__.py` & `RecordFlux-0.9.1/rflx/model/__init__.py`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/model/basic_declaration.py` & `RecordFlux-0.9.1/rflx/model/basic_declaration.py`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/model/declaration.py` & `RecordFlux-0.9.1/rflx/model/declaration.py`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/model/message.py` & `RecordFlux-0.9.1/rflx/model/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -792,15 +792,15 @@
                         f'structure of "{self.identifier}" contains cycle',
                         Subsystem.MODEL,
                         Severity.ERROR,
                         self.location,
                     )
                 ],
             )
-            # https://github.com/Componolit/RecordFlux/issues/256
+            # Eng/RecordFlux/RecordFlux#256
             return None
         return tuple(f for f in result if f not in [INITIAL, FINAL])
 
     def _compute_definite_predecessors(self, final: Field) -> tuple[Field, ...]:
         return tuple(
             f
             for f in self.fields
```

### Comparing `RecordFlux-0.9.0/rflx/model/model.py` & `RecordFlux-0.9.1/rflx/model/model.py`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/model/package.py` & `RecordFlux-0.9.1/rflx/model/package.py`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/model/session.py` & `RecordFlux-0.9.1/rflx/model/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,14 +292,17 @@
                 assert isinstance(message_decl.type_, rty.Structure)
                 self.declarations[name] = message_decl
 
                 for action in self._actions:
                     if isinstance(action, stmt.Assignment):
                         substituted(action.expression, message_decl.type_)
 
+                for transition in self._transitions:
+                    substituted(transition.condition, message_decl.type_)
+
 
 class AbstractSession(BasicDeclaration):
     # pylint: disable=too-many-arguments, too-many-instance-attributes
     @abstractmethod
     def __init__(
         self,
         identifier: StrID,
```

### Comparing `RecordFlux-0.9.0/rflx/model/type_.py` & `RecordFlux-0.9.1/rflx/model/type_.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
                         Subsystem.MODEL,
                         Severity.ERROR,
                         self.location,
                     )
                 ],
             )
 
-        # https://github.com/Componolit/RecordFlux/issues/1077
+        # Eng/RecordFlux/RecordFlux#1077
         # size of integers is limited to 63bits
 
         if int(size_num) > const.MAX_SCALAR_SIZE:
             self.error.extend(
                 [
                     (
                         f'size of "{self.name}" exceeds limit (2**{const.MAX_SCALAR_SIZE})',
@@ -350,15 +350,15 @@
                             Subsystem.MODEL,
                             Severity.ERROR,
                             self.location,
                         )
                     ],
                 )
 
-        # https://github.com/Componolit/RecordFlux/issues/1077
+        # Eng/RecordFlux/RecordFlux#1077
         # size of integers is limited to 63bits
 
         if int(size_num) > const.MAX_SCALAR_SIZE:
             self.error.extend(
                 [
                     (
                         f'size of "{self.name}" exceeds limit (2**{const.MAX_SCALAR_SIZE})',
```

### Comparing `RecordFlux-0.9.0/rflx/pyrflx/bitstring.py` & `RecordFlux-0.9.1/rflx/pyrflx/bitstring.py`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/pyrflx/package.py` & `RecordFlux-0.9.1/rflx/pyrflx/package.py`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/pyrflx/pyrflx.py` & `RecordFlux-0.9.1/rflx/pyrflx/pyrflx.py`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/pyrflx/typevalue.py` & `RecordFlux-0.9.1/rflx/pyrflx/typevalue.py`

 * *Files 0% similar despite different names*

```diff
@@ -1342,15 +1342,15 @@
                 self._simplified_mapping[self._message_last_name] = (
                     Number(message_size - 1) if message_size else last
                 )
                 self._simplified_mapping[self._message_size_name] = (
                     Number(message_size) if message_size else last + Number(1)
                 )
 
-        # https://github.com/Componolit/RecordFlux/issues/422
+        # Eng/RecordFlux/RecordFlux#422
         self._simplified_mapping.update({ValidChecksum(f): TRUE for f in self._checksums})
 
     def _simplified(self, expr: Expr, max_iterations: int = 16) -> Expr:
         if expr in {TRUE, FALSE}:
             return expr
 
         def subst(expression: Expr) -> Expr:
```

### Comparing `RecordFlux-0.9.0/rflx/pyrflx/utils.py` & `RecordFlux-0.9.1/rflx/pyrflx/utils.py`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/specification/cache.py` & `RecordFlux-0.9.1/rflx/specification/cache.py`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/specification/const.py` & `RecordFlux-0.9.1/rflx/specification/const.py`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/specification/parser.py` & `RecordFlux-0.9.1/rflx/specification/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1709,15 +1709,15 @@
                         Subsystem.PARSER,
                         Severity.ERROR,
                         node_location(package.f_identifier, name),
                     )
                 ],
             )
     for t in package.f_declarations:
-        # https://github.com/Componolit/RecordFlux/issues/1208
+        # Eng/RecordFlux/RecordFlux#1208
         if isinstance(t, lang.TypeDecl) and model.is_builtin_type(
             create_id(error, t.f_identifier, name).name
         ):
             error.extend(
                 [
                     (
                         f'illegal redefinition of built-in type "{t.f_identifier.text}"',
```

### Comparing `RecordFlux-0.9.0/rflx/specification/style.py` & `RecordFlux-0.9.1/rflx/specification/style.py`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/templates/rflx_arithmetic.adb` & `RecordFlux-0.9.1/rflx/templates/rflx_arithmetic.adb`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/templates/rflx_arithmetic.ads` & `RecordFlux-0.9.1/rflx/templates/rflx_arithmetic.ads`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/templates/rflx_builtin_types-conversions.ads` & `RecordFlux-0.9.1/rflx/templates/rflx_builtin_types-conversions.ads`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/templates/rflx_generic_types-generic_operations.adb` & `RecordFlux-0.9.1/rflx/templates/rflx_generic_types-generic_operations.adb`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/templates/rflx_generic_types-generic_operations.ads` & `RecordFlux-0.9.1/rflx/templates/rflx_generic_types-generic_operations.ads`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/templates/rflx_generic_types-generic_operators.ads` & `RecordFlux-0.9.1/rflx/templates/rflx_generic_types-generic_operators.ads`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/templates/rflx_generic_types.ads` & `RecordFlux-0.9.1/rflx/templates/rflx_generic_types.ads`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/templates/rflx_message_sequence.adb` & `RecordFlux-0.9.1/rflx/templates/rflx_message_sequence.adb`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/templates/rflx_message_sequence.ads` & `RecordFlux-0.9.1/rflx/templates/rflx_message_sequence.ads`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
      Pre =>
        (Has_Buffer (Ctx)
         and then Valid (Ctx)
         and then Data'Length = Byte_Size (Ctx));
 
 private
 
-   -- https://github.com/Componolit/Workarounds/issues/24
+   -- Eng/RecordFlux/Workarounds#24
    pragma Warnings (Off, "use clause for package * has no effect");
 
    use {prefix}RFLX_Types;
 
    pragma Warnings (On, "use clause for package * has no effect");
 
    type Context_State is (S_Valid, S_Invalid);
```

### Comparing `RecordFlux-0.9.0/rflx/templates/rflx_scalar_sequence.adb` & `RecordFlux-0.9.1/rflx/templates/rflx_scalar_sequence.adb`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/templates/rflx_scalar_sequence.ads` & `RecordFlux-0.9.1/rflx/templates/rflx_scalar_sequence.ads`

 * *Files 2% similar despite different names*

```diff
@@ -176,15 +176,15 @@
      Pre =>
        (Has_Buffer (Ctx)
         and then Valid (Ctx)
         and then Data'Length = Byte_Size (Ctx));
 
 private
 
-   -- https://github.com/Componolit/Workarounds/issues/24
+   -- Eng/RecordFlux/Workarounds#24
    pragma Warnings (Off, "use clause for package * has no effect");
 
    use {prefix}RFLX_Types;
 
    pragma Warnings (On, "use clause for package * has no effect");
 
    type Context_State is (S_Valid, S_Invalid);
```

### Comparing `RecordFlux-0.9.0/rflx/typing_.py` & `RecordFlux-0.9.1/rflx/typing_.py`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/rflx/validator.py` & `RecordFlux-0.9.1/rflx/validator.py`

 * *Files identical despite different names*

### Comparing `RecordFlux-0.9.0/setup.py` & `RecordFlux-0.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     description=(
         "A toolset for the formal specification and generation of verifiable binary parsers, "
         "message generators and protocol state machines."
     ),
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Tobias Reiher",
-    author_email="reiher@componolit.com",
-    url="https://github.com/Componolit/RecordFlux",
+    author_email="reiher@adacore.com",
+    url="https://github.com/AdaCore/RecordFlux",
     license="AGPL-3.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Ada",
@@ -57,14 +57,14 @@
             "furo == 2022.4.7",
             "hypothesis >=6.14, <6.24",
             "pyicontract-lint >=2.1.2, <2.2",
             "pytest-timeout >=2, <3",
             "scapy ==2.4.5",
             "setuptools_scm >=6.2, <8",
             "sphinx >=4.5, <5",
-            "sphinx-copybutton >=0.5, <0.6",
+            "sphinx-rtd-theme >= 1.1.1, <1.2",
             "tqdm >=4.61.1, <4.63",
             "types-pkg_resources >=0.1.3, <0.2",
         ]
     },
     scripts=["bin/rflx"],
 )
```

