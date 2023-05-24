# Comparing `tmp/validataclass-0.8.1.tar.gz` & `tmp/validataclass-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/validataclass/validataclass/dist/.tmp-8sn8v4ui/validataclass-0.8.1.tar", last modified: Wed Nov 30 12:03:39 2022, max compression
+gzip compressed data, was "/home/runner/work/validataclass/validataclass/dist/.tmp-t7l662o9/validataclass-0.9.0.tar", last modified: Wed May 24 10:22:46 2023, max compression
```

## Comparing `validataclass-0.8.1.tar` & `validataclass-0.9.0.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:03:39.000000 validataclass-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (122)      688 2022-11-30 12:03:29.000000 validataclass-0.8.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:03:39.000000 validataclass-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:03:39.000000 validataclass-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2153 2022-11-30 12:03:29.000000 validataclass-0.8.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2046 2022-11-30 12:03:29.000000 validataclass-0.8.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (122)      170 2022-11-30 12:03:29.000000 validataclass-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)    23195 2022-11-30 12:03:29.000000 validataclass-0.8.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1083 2022-11-30 12:03:29.000000 validataclass-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2410 2022-11-30 12:03:29.000000 validataclass-0.8.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     3326 2022-11-30 12:03:39.000000 validataclass-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1985 2022-11-30 12:03:29.000000 validataclass-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:03:39.000000 validataclass-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (122)    11730 2022-11-30 12:03:29.000000 validataclass-0.8.1/docs/01-introduction.md
--rw-r--r--   0 runner    (1001) docker     (122)     8129 2022-11-30 12:03:29.000000 validataclass-0.8.1/docs/02-error-handling.md
--rw-r--r--   0 runner    (1001) docker     (122)    69727 2022-11-30 12:03:29.000000 validataclass-0.8.1/docs/03-basic-validators.md
--rw-r--r--   0 runner    (1001) docker     (122)    16198 2022-11-30 12:03:29.000000 validataclass-0.8.1/docs/04-lists-and-dicts.md
--rw-r--r--   0 runner    (1001) docker     (122)    48368 2022-11-30 12:03:29.000000 validataclass-0.8.1/docs/05-dataclasses.md
--rw-r--r--   0 runner    (1001) docker     (122)      193 2022-11-30 12:03:29.000000 validataclass-0.8.1/docs/06-build-your-own.md
--rw-r--r--   0 runner    (1001) docker     (122)      951 2022-11-30 12:03:29.000000 validataclass-0.8.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (122)      221 2022-11-30 12:03:29.000000 validataclass-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      215 2022-11-30 12:03:29.000000 validataclass-0.8.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (122)     1486 2022-11-30 12:03:39.000000 validataclass-0.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:03:39.000000 validataclass-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:03:39.000000 validataclass-0.8.1/src/validataclass/
--rw-r--r--   0 runner    (1001) docker     (122)      180 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      176 2022-11-30 12:03:39.000000 validataclass-0.8.1/src/validataclass/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:03:39.000000 validataclass-0.8.1/src/validataclass/dataclasses/
--rw-r--r--   0 runner    (1001) docker     (122)      398 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/dataclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4325 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/dataclasses/defaults.py
--rw-r--r--   0 runner    (1001) docker     (122)    10076 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/dataclasses/validataclass.py
--rw-r--r--   0 runner    (1001) docker     (122)     3796 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/dataclasses/validataclass_field.py
--rw-r--r--   0 runner    (1001) docker     (122)     2106 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/dataclasses/validataclass_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:03:39.000000 validataclass-0.8.1/src/validataclass/exceptions/
--rw-r--r--   0 runner    (1001) docker     (122)     1417 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5731 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/exceptions/common_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3278 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/exceptions/dataclass_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2625 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/exceptions/datetime_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2691 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/exceptions/dict_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      461 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/exceptions/email_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2339 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/exceptions/list_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1144 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/exceptions/meta_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      779 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/exceptions/misc_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2856 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/exceptions/number_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      474 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/exceptions/regex_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2684 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/exceptions/string_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      481 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/exceptions/url_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:03:39.000000 validataclass-0.8.1/src/validataclass/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)     1504 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      827 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/helpers/dataclass_defaults.py
--rw-r--r--   0 runner    (1001) docker     (122)      760 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/helpers/dataclass_mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)      849 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/helpers/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (122)    11042 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/helpers/datetime_range.py
--rw-r--r--   0 runner    (1001) docker     (122)     1998 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/helpers/unset_value.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:03:39.000000 validataclass-0.8.1/src/validataclass/internal/
--rw-r--r--   0 runner    (1001) docker     (122)      180 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3626 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/internal/internet_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:03:39.000000 validataclass-0.8.1/src/validataclass/validators/
--rw-r--r--   0 runner    (1001) docker     (122)     1561 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3000 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/allow_empty_string.py
--rw-r--r--   0 runner    (1001) docker     (122)     7489 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/any_of_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     7532 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/anything_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     2500 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/big_integer_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     2119 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/boolean_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)    11481 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/dataclass_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/date_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)    15185 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/datetime_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     8376 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/decimal_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     7678 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1694 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/discard_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3627 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/email_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     5938 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/enum_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     5621 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/float_to_decimal_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3757 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/float_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     4358 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/integer_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     5025 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/list_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1450 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/none_to_unset_value.py
--rw-r--r--   0 runner    (1001) docker     (122)     2849 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/noneable.py
--rw-r--r--   0 runner    (1001) docker     (122)     3659 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/numeric_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     7442 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/regex_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     4348 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/reject_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     6315 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/string_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3767 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/time_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     7253 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/url_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3827 2022-11-30 12:03:29.000000 validataclass-0.8.1/src/validataclass/validators/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:03:39.000000 validataclass-0.8.1/src/validataclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3326 2022-11-30 12:03:39.000000 validataclass-0.8.1/src/validataclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4788 2022-11-30 12:03:39.000000 validataclass-0.8.1/src/validataclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 12:03:39.000000 validataclass-0.8.1/src/validataclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      120 2022-11-30 12:03:39.000000 validataclass-0.8.1/src/validataclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2022-11-30 12:03:39.000000 validataclass-0.8.1/src/validataclass.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:03:39.000000 validataclass-0.8.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:03:39.000000 validataclass-0.8.1/tests/dataclasses/
--rw-r--r--   0 runner    (1001) docker     (122)     1804 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/dataclasses/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     8644 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/dataclasses/defaults_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     8207 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/dataclasses/validataclass_field_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     4171 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/dataclasses/validataclass_mixin_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    21271 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/dataclasses/validataclass_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:03:39.000000 validataclass-0.8.1/tests/exceptions/
--rw-r--r--   0 runner    (1001) docker     (122)     5468 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/exceptions/common_exceptions_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3233 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/exceptions/dataclass_exceptions_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1330 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/exceptions/dict_exceptions_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1263 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/exceptions/list_exceptions_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:03:39.000000 validataclass-0.8.1/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)     2751 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/helpers/_compatibility_imports_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    26995 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/helpers/datetime_range_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2120 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/helpers/unset_value_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:03:39.000000 validataclass-0.8.1/tests/internal/
--rw-r--r--   0 runner    (1001) docker     (122)     5555 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/internal/internet_helpers_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3228 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2287 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/test_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 12:03:39.000000 validataclass-0.8.1/tests/validators/
--rw-r--r--   0 runner    (1001) docker     (122)     4487 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/allow_empty_string_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    14345 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/any_of_validator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     9038 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/anything_validator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     4081 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/big_integer_validator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2474 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/boolean_validator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    20805 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/dataclass_validator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3273 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/date_validator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    22734 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/datetime_validator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    14893 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/decimal_validator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    22111 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/dict_validator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1809 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/discard_validator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     6780 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/email_validator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    15111 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/enum_validator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    14705 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/float_to_decimal_validator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     6959 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/float_validator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    10721 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/integer_validator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    11613 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/list_validator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1482 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/none_to_unset_value_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     4277 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/noneable_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     9906 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/numeric_validator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    14177 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/regex_validator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     4552 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/reject_validator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    11869 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/string_validator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     6339 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/time_validator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    11978 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/url_validator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1043 2022-11-30 12:03:29.000000 validataclass-0.8.1/tests/validators/validator_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1047 2022-11-30 12:03:29.000000 validataclass-0.8.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:22:46.000000 validataclass-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-24 10:22:36.000000 validataclass-0.9.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:22:46.000000 validataclass-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:22:46.000000 validataclass-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-24 10:22:36.000000 validataclass-0.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-24 10:22:36.000000 validataclass-0.9.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-24 10:22:36.000000 validataclass-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    24313 2023-05-24 10:22:36.000000 validataclass-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-24 10:22:36.000000 validataclass-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-24 10:22:36.000000 validataclass-0.9.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-24 10:22:46.000000 validataclass-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-24 10:22:36.000000 validataclass-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:22:46.000000 validataclass-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-05-24 10:22:36.000000 validataclass-0.9.0/docs/01-introduction.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-05-24 10:22:36.000000 validataclass-0.9.0/docs/02-error-handling.md
+-rw-r--r--   0 runner    (1001) docker     (123)    70006 2023-05-24 10:22:36.000000 validataclass-0.9.0/docs/03-basic-validators.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16198 2023-05-24 10:22:36.000000 validataclass-0.9.0/docs/04-lists-and-dicts.md
+-rw-r--r--   0 runner    (1001) docker     (123)    48272 2023-05-24 10:22:36.000000 validataclass-0.9.0/docs/05-dataclasses.md
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-24 10:22:36.000000 validataclass-0.9.0/docs/06-build-your-own.md
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-24 10:22:36.000000 validataclass-0.9.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-24 10:22:36.000000 validataclass-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-24 10:22:36.000000 validataclass-0.9.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-24 10:22:46.000000 validataclass-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:22:46.000000 validataclass-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:22:46.000000 validataclass-0.9.0/src/validataclass/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 10:22:46.000000 validataclass-0.9.0/src/validataclass/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:22:46.000000 validataclass-0.9.0/src/validataclass/dataclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/dataclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/dataclasses/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/dataclasses/validataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/dataclasses/validataclass_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/dataclasses/validataclass_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:22:46.000000 validataclass-0.9.0/src/validataclass/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/exceptions/common_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/exceptions/dataclass_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/exceptions/datetime_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/exceptions/dict_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/exceptions/email_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/exceptions/list_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/exceptions/meta_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/exceptions/misc_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/exceptions/number_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/exceptions/regex_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/exceptions/string_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/exceptions/url_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:22:46.000000 validataclass-0.9.0/src/validataclass/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/helpers/dataclass_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/helpers/dataclass_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/helpers/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11042 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/helpers/datetime_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/helpers/unset_value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:22:46.000000 validataclass-0.9.0/src/validataclass/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/internal/internet_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:22:46.000000 validataclass-0.9.0/src/validataclass/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/allow_empty_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/any_of_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/anything_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/big_integer_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/boolean_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/dataclass_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/date_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15185 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/datetime_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/decimal_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/discard_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/email_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/enum_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/float_to_decimal_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/float_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/integer_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/list_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/none_to_unset_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/noneable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/numeric_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/regex_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/reject_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/string_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/time_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/url_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-24 10:22:36.000000 validataclass-0.9.0/src/validataclass/validators/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:22:46.000000 validataclass-0.9.0/src/validataclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-24 10:22:46.000000 validataclass-0.9.0/src/validataclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-24 10:22:46.000000 validataclass-0.9.0/src/validataclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 10:22:46.000000 validataclass-0.9.0/src/validataclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-24 10:22:46.000000 validataclass-0.9.0/src/validataclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-24 10:22:46.000000 validataclass-0.9.0/src/validataclass.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:22:46.000000 validataclass-0.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:22:46.000000 validataclass-0.9.0/tests/dataclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/dataclasses/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/dataclasses/defaults_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/dataclasses/validataclass_field_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/dataclasses/validataclass_mixin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21271 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/dataclasses/validataclass_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:22:46.000000 validataclass-0.9.0/tests/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/exceptions/common_exceptions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/exceptions/dataclass_exceptions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/exceptions/dict_exceptions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/exceptions/list_exceptions_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:22:46.000000 validataclass-0.9.0/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/helpers/_compatibility_imports_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26995 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/helpers/datetime_range_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/helpers/unset_value_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:22:46.000000 validataclass-0.9.0/tests/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/internal/internet_helpers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/test_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:22:46.000000 validataclass-0.9.0/tests/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/allow_empty_string_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14345 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/any_of_validator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/anything_validator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/big_integer_validator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/boolean_validator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25245 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/dataclass_validator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/date_validator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22734 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/datetime_validator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14893 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/decimal_validator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/dict_validator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/discard_validator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/email_validator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/enum_validator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14705 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/float_to_decimal_validator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/float_validator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/integer_validator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/list_validator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/none_to_unset_value_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/noneable_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/numeric_validator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14177 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/regex_validator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/reject_validator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11869 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/string_validator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/time_validator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/url_validator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-24 10:22:36.000000 validataclass-0.9.0/tests/validators/validator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-24 10:22:36.000000 validataclass-0.9.0/tox.ini
```

### Comparing `validataclass-0.8.1/.coveragerc` & `validataclass-0.9.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/.github/workflows/release.yml` & `validataclass-0.9.0/.github/workflows/release.yml`

 * *Files 24% similar despite different names*

```diff
@@ -9,50 +9,50 @@
 
 jobs:
   build:
     name: Build package
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
       # We use Python 3.7 here because it's the minimum Python version supported by this library.
       - name: Setup Python 3.7
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: 3.7
 
       - name: Install dependencies
         run: pip install --upgrade pip build
 
       - name: Build package
         run: python -m build
 
       - name: Upload build artifacts
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: dist_packages
           path: dist/
 
   test:
     # This job tests the built package by installing it via pip and running unit tests (without tox).
     name: Test package
     needs: build
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
       - name: Setup Python 3.7
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: 3.7
 
       - name: Download build artifacts
-        uses: actions/download-artifact@v2
+        uses: actions/download-artifact@v3
         with:
           name: dist_packages
           path: dist/
 
       - name: Install test dependencies
         run: pip install pytest pytest-cov
 
@@ -65,23 +65,23 @@
   publish:
     name: Publish package
     needs: test
     runs-on: ubuntu-latest
 
     steps:
       - name: Download build artifacts
-        uses: actions/download-artifact@v2
+        uses: actions/download-artifact@v3
         with:
           name: dist_packages
           path: dist/
 
       - name: Upload package to GitHub release assets
         uses: AButler/upload-release-assets@v2.0
         with:
           files: dist/*
           repo-token: ${{ secrets.GITHUB_TOKEN }}
 
       - name: Publish package to PyPI
-        uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
+        uses: pypa/gh-action-pypi-publish@v1.8.6
         with:
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `validataclass-0.8.1/.github/workflows/tests.yml` & `validataclass-0.9.0/.github/workflows/tests.yml`

 * *Files 12% similar despite different names*

```diff
@@ -19,29 +19,30 @@
       fail-fast: false
       matrix:
         python-version:
           - '3.7'
           - '3.8'
           - '3.9'
           - '3.10'
+          - '3.11'
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
       - name: Setup Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: pip install --upgrade pip tox
 
       - name: Run unit tests with tox
         # Run tox using the version of Python in `PATH`
-        run: tox -e clean,py,flake8,report -- --junit-xml=reports/pytest_${{ matrix.python-version }}.xml
+        run: tox run -e clean,py,flake8,report -- --junit-xml=reports/pytest_${{ matrix.python-version }}.xml
 
       - name: Upload test result artifacts
         uses: actions/upload-artifact@v3
         if: success() || failure()
         with:
           # This will add every pytest_VERSION.xml to the same artifact file
           name: pytest-results
@@ -54,15 +55,15 @@
     # Job depends on test results
     needs: test
 
     # Do not run this job in pull requests from a forked repository (because the test-reporter would fail)
     if: github.event_name != 'pull_request' || github.event.pull_request.head.repo.full_name == github.repository
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
       - name: Download test result artifacts
         uses: actions/download-artifact@v3
         with:
           name: pytest-results
           path: reports/
```

### Comparing `validataclass-0.8.1/CHANGELOG.md` & `validataclass-0.9.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,45 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
+## [0.9.0](https://github.com/binary-butterfly/validataclass/releases/tag/0.9.0) - 2023-05-24
+
+[Full changelog](https://github.com/binary-butterfly/validataclass/compare/0.8.1...0.9.0)
+
+This release adds official support for Python for Workgroups 3.11, as well as some minor changes.
+
+### Added
+
+- `EmailValidator`: Add parameter `to_lowercase`. [#106]
+
+### Changed
+
+- Allow defining `__post_validate__()` with specific context arguments without `**kwargs`. [#105]
+
+### Fixed
+
+- Fix Python 3.11 incompatibilities due to `UnsetValue` not being hashable. [#102]
+- Also fix missing `__hash__` methods in the `Default` classes (for completeness). [#102]
+
+### Testing / CI
+
+- Update GitHub actions to fix deprecation warnings. [#103]
+- Update local test environment for tox 4. [#104]
+
+[#102]: https://github.com/binary-butterfly/validataclass/pull/102
+[#103]: https://github.com/binary-butterfly/validataclass/pull/103
+[#104]: https://github.com/binary-butterfly/validataclass/pull/104
+[#105]: https://github.com/binary-butterfly/validataclass/pull/105
+[#106]: https://github.com/binary-butterfly/validataclass/pull/106
+
+
 ## [0.8.1](https://github.com/binary-butterfly/validataclass/releases/tag/0.8.1) - 2022-11-30
 
 [Full changelog](https://github.com/binary-butterfly/validataclass/compare/0.8.0...0.8.1)
 
 ### Fixed
 
 - `AnyOfValidator` and `EnumValidator`: Fixed wrong default value. Now the validators are really case-insensitive by default.
@@ -31,15 +62,15 @@
 - `EmailValidator` and `RegexValidator`: Add parameter `allow_empty` to allow empty strings (by [@TomasHalgas]). [#89]
 - `EmailValidator`: Add parameter `max_length`. [#97]
 - `DecimalValidator`: Add parameter `rounding` to specify rounding mode (with a new default, see "Changed"). [#99]
 
 ### Changed
 
 - **Breaking change:** `AnyOfValidator` and `EnumValidator` are now **case-sensitive** by default. [#98]
-  - The parameter `case_insensitive` is **replaced** with a new parameter `case_sensitive` which defaults to True.
+  - The parameter `case_insensitive` is **replaced** with a new parameter `case_sensitive` which defaults to False.
   - The old parameter is still supported for compatibility, but is now deprecated and will be removed in a future version.
   - If you have set `case_insensitive=True` before, you can simply remove this parameter now as this is the default now.
 - **Breaking change:** `DecimalValidator` (and all subclasses) now uses `decimal.ROUND_HALF_UP` as default rounding mode. [#99]
   - Until now, the rounding mode of the current decimal context was used, which defaults to `decimal.ROUND_HALF_EVEN`.
   - Use the `rounding` parameter to change this. To restore the old behavior and use the decimal context, set `rounding=None`.
 
 ### Deprecated
```

### Comparing `validataclass-0.8.1/LICENSE` & `validataclass-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/Makefile` & `validataclass-0.9.0/Makefile`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Settings
-# NOTE: The multi-python image is a fork of fkrull/multi-python, which as of now has not been updated for Python 3.10 yet
-DOCKER_MULTI_PYTHON_IMAGE = gnufede/multi-python:focal
+DOCKER_MULTI_PYTHON_IMAGE = acidrain/multi-python:latest
 DOCKER_USER = "$(shell id -u):$(shell id -g)"
 
 # Default target
 .DEFAULT_GOAL := tox
 
 
 # Development environment
@@ -24,30 +23,30 @@
 
 # Test suite
 # ----------
 
 # Run complete tox suite
 .PHONY: tox
 tox:
-	tox
+	tox run
 
 # Run tox in venv (needs to be installed with `make venv` first)
 .PHONY: venv-tox
 venv-tox:
-	. venv/bin/activate && tox
+	. venv/bin/activate && tox run
 
 # Only run pytest
 .PHONY: test
 test:
-	tox -e 'clean,py{310,39,38,37},report'
+	tox run --skip-env flake8
 
 # Only run flake8 linter
 .PHONY: flake8
 flake8:
-	tox -e flake8
+	tox run -e flake8
 
 # Open HTML coverage report in browser
 .PHONY: open-coverage
 open-coverage:
 	$(or $(BROWSER),firefox) ./reports/coverage_html/index.html
 
 # Run complete tox test suite in a multi-python Docker container
@@ -55,18 +54,20 @@
 docker-tox:
 	docker run --rm --tty \
 		--user $(DOCKER_USER) \
 		--mount "type=bind,src=$(shell pwd),target=/code" \
 		--workdir /code \
 		--env HOME=/tmp/home \
 		$(DOCKER_MULTI_PYTHON_IMAGE) \
-		tox --workdir .tox_docker $(TOX_ARGS)
+		tox run --workdir .tox_docker $(TOX_ARGS)
 
 # Run partial tox test suites in Docker
-.PHONY: docker-tox-py310 docker-tox-py39 docker-tox-py38 docker-tox-py37
+.PHONY: docker-tox-py311 docker-tox-py310 docker-tox-py39 docker-tox-py38 docker-tox-py37
+docker-tox-py311: TOX_ARGS="-e clean,py311,py311-report"
+docker-tox-py311: docker-tox
 docker-tox-py310: TOX_ARGS="-e clean,py310,py310-report"
 docker-tox-py310: docker-tox
 docker-tox-py39: TOX_ARGS="-e clean,py39,py39-report"
 docker-tox-py39: docker-tox
 docker-tox-py38: TOX_ARGS="-e clean,py38,py38-report"
 docker-tox-py38: docker-tox
 docker-tox-py37: TOX_ARGS="-e clean,py37,py37-report"
@@ -75,28 +76,28 @@
 # Run all tox test suites, but separately to check code coverage individually
 .PHONY: docker-tox-all
 docker-tox-all:
 	make docker-tox-py37
 	make docker-tox-py38
 	make docker-tox-py39
 	make docker-tox-py310
+	make docker-tox-py311
 
 # Pull the latest image of the multi-python Docker image
 .PHONY: docker-pull
 docker-pull:
 	docker pull $(DOCKER_MULTI_PYTHON_IMAGE)
 
 
 # Cleanup
 # -------
 
 .PHONY: clean
 clean:
-	rm -rf .coverage .pytest_cache reports src/validataclass/_version.py
+	rm -rf .coverage .pytest_cache reports src/validataclass/_version.py .tox .tox_docker .eggs src/*.egg-info venv
 
 .PHONY: clean-dist
 clean-dist:
 	rm -rf dist/
 
 .PHONY: clean-all
 clean-all: clean clean-dist
-	rm -rf .tox .tox_docker .eggs src/*.egg-info venv
```

### Comparing `validataclass-0.8.1/PKG-INFO` & `validataclass-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validataclass
-Version: 0.8.1
+Version: 0.9.0
 Summary: Library for input validation designed for (but not restricted to) JSON-based APIs, neatly integrating with dataclasses.
 Home-page: https://github.com/binary-butterfly/validataclass
 Author: binary butterfly GmbH
 Author-email: lexi.stelter@binary-butterfly.de
 License: MIT
 Project-URL: Documentation, https://github.com/binary-butterfly/validataclass/blob/main/docs/index.md
 Project-URL: Changelog, https://github.com/binary-butterfly/validataclass/blob/main/CHANGELOG.md
@@ -14,14 +14,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
```

### Comparing `validataclass-0.8.1/README.md` & `validataclass-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/docs/01-introduction.md` & `validataclass-0.9.0/docs/01-introduction.md`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/docs/02-error-handling.md` & `validataclass-0.9.0/docs/02-error-handling.md`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/docs/03-basic-validators.md` & `validataclass-0.9.0/docs/03-basic-validators.md`

 * *Files 0% similar despite different names*

```diff
@@ -231,14 +231,16 @@
 Please note that this validator is a bit opinionated and simplified in that it does **not** allow every email address
 that technically is valid according to the RFCs. For example, it does neither allow internationalized email addresses
 (although this might be changed in the future), nor oddities like quoted strings as local part or comments, because most
 mail software does not support those anyway and/or might break with those adresses.
 
 By default, the validator does not accept empty strings as input. To allow them, set the parameter `allow_empty=True`.
 
+To automatically convert the output email address to lowercase, you can set the parameter `to_lowercase=True`.
+
 Also, the default maximum string length is set to 256 characters (which would be a really long, but still valid email
 address), which can be changed using the `max_length` parameter.
 
 **Example:**
 
 ```python
 from validataclass.validators import EmailValidator
@@ -249,14 +251,18 @@
 validator.validate("banana")           # will raise InvalidEmailError(reason='Invalid email address format.')
 validator.validate("")                 # will raise StringTooShortError(min_length=1, max_length=256)
 
 # Allow empty strings as input
 validator = EmailValidator(allow_empty=True)
 validator.validate("foo@example.com")  # will return "foo@example.com"
 validator.validate("")                 # will return "" (empty string)
+
+# Converts email addresses to lowercase
+validator = EmailValidator(to_lowercase=True)
+validator.validate("Foo.Bar@Example.COM")  # will return "foo.bar@example.com")
 ```
 
 
 ### UrlValidators
 
 The `UrlValidator` validates URLs as strings and returns them unmodified.
```

### Comparing `validataclass-0.8.1/docs/04-lists-and-dicts.md` & `validataclass-0.9.0/docs/04-lists-and-dicts.md`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/docs/05-dataclasses.md` & `validataclass-0.9.0/docs/05-dataclasses.md`

 * *Files 1% similar despite different names*

```diff
@@ -789,20 +789,19 @@
 These so called **context arguments** are passed to the `validate()` call as arbitrary keyword arguments. Whether and
 how the validator actually uses these arguments depends on the implementation of the validator. Most validators don't
 do anything with it except for passing it to sub-validators (e.g. the `ListValidator` passes the context arguments to
 the specified item validator).
 
 The `DataclassValidator` supports these context arguments and uses them in two ways: First, it passes them as they are
 to any field validator (which might pass them to other validators as well). Second, it also passes them to the
-`__post_validate__()` method of the dataclass.
+`__post_validate__()` method of the dataclass as long as the method accepts them.
 
-However, for this to work, the method MUST accept arbitrary keyword arguments, i.e. it needs to be declared with a
-`**kwargs` parameter (the parameter name doesn't matter). You can of course declare specific keyword arguments that you
-want to use for post-validation (make sure to define them as optional!), but you still need to accept any other keyword
-argument as well, otherwise the context arguments will not be passed to the method at all.
+You can define the `__post_validate__()` method with specific keyword-only arguments and/or with a `**kwargs` parameter.
+The `DataclassValidator` will make sure to only pass the arguments that the method accepts. Please make sure to use
+**keyword-only** arguments instead of positional arguments. The latter will still work, but emit a warning.
 
 Example:
 
 ```python
 from typing import Optional
 
 from validataclass.dataclasses import validataclass, Default
@@ -810,16 +809,16 @@
 from validataclass.validators import DataclassValidator, BooleanValidator, IntegerValidator
 
 @validataclass
 class ContextSensitiveExampleClass:
     # This field is optional, unless the context says otherwise.
     some_value: Optional[int] = IntegerValidator(), Default(None)
 
-    # Note: Prefix the kwargs parameter with an underscore to avoid "unused parameter" notices.
-    def __post_validate__(self, *, require_some_value: bool = False, **_kwargs):
+    # Note: You can also specify **kwargs here to get all context arguments.
+    def __post_validate__(self, *, require_some_value: bool = False):
         # If require_some_value was set at validation time, ensure that some_value is set!
         if require_some_value and self.some_value is None:
             raise DataclassPostValidationError(field_errors={
                 'some_value': RequiredValueError(reason='Must be set in this context.'),
             })
 
 # Create a validator for this dataclass
```

### Comparing `validataclass-0.8.1/docs/index.md` & `validataclass-0.9.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/setup.cfg` & `validataclass-0.9.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: Utilities
 
 [options]
 package_dir = 
 	= src
```

### Comparing `validataclass-0.8.1/src/validataclass/dataclasses/defaults.py` & `validataclass-0.9.0/src/validataclass/dataclasses/defaults.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,17 @@
         return f'{type(self).__name__}({self.value!r})'
 
     def __eq__(self, other):
         if isinstance(self, type(other)):
             return self.value == other.value
         return NotImplemented
 
+    def __hash__(self):
+        return hash(self.value)
+
     def get_value(self) -> Any:
         return deepcopy(self.value)
 
     def needs_factory(self) -> bool:
         """
         Returns True if a dataclass default_factory is needed for this Default object, for example if the value is a
         mutable object (e.g. a list) that needs to be copied.
@@ -71,14 +74,17 @@
         return f'{type(self).__name__}({self.factory!r})'
 
     def __eq__(self, other):
         if isinstance(self, type(other)):
             return isinstance(other, DefaultFactory) and self.factory == other.factory
         return NotImplemented
 
+    def __hash__(self):
+        return hash(self.factory)
+
     def get_value(self) -> Any:
         return self.factory()
 
     def needs_factory(self) -> bool:
         return True
 
 
@@ -123,14 +129,18 @@
     def __repr__(self):
         return 'NoDefault'
 
     def __eq__(self, other):
         # Nothing is equal to NoDefault except itself
         return type(self) is type(other)
 
+    def __hash__(self):
+        # Use default implementation
+        return object.__hash__(self)
+
     def get_value(self) -> NoReturn:
         raise ValueError('No default value specified!')
 
     # For convenience: Allow NoDefault to be used as `NoDefault()`, returning the sentinel itself.
     def __call__(self):
         return self
```

### Comparing `validataclass-0.8.1/src/validataclass/dataclasses/validataclass.py` & `validataclass-0.9.0/src/validataclass/dataclasses/validataclass.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/dataclasses/validataclass_field.py` & `validataclass-0.9.0/src/validataclass/dataclasses/validataclass_field.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/dataclasses/validataclass_mixin.py` & `validataclass-0.9.0/src/validataclass/dataclasses/validataclass_mixin.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/exceptions/__init__.py` & `validataclass-0.9.0/src/validataclass/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/exceptions/common_exceptions.py` & `validataclass-0.9.0/src/validataclass/exceptions/common_exceptions.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/exceptions/dataclass_exceptions.py` & `validataclass-0.9.0/src/validataclass/exceptions/dataclass_exceptions.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/exceptions/datetime_exceptions.py` & `validataclass-0.9.0/src/validataclass/exceptions/datetime_exceptions.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/exceptions/dict_exceptions.py` & `validataclass-0.9.0/src/validataclass/exceptions/dict_exceptions.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/exceptions/list_exceptions.py` & `validataclass-0.9.0/src/validataclass/exceptions/list_exceptions.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/exceptions/meta_exceptions.py` & `validataclass-0.9.0/src/validataclass/exceptions/meta_exceptions.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/exceptions/misc_exceptions.py` & `validataclass-0.9.0/src/validataclass/exceptions/misc_exceptions.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/exceptions/number_exceptions.py` & `validataclass-0.9.0/src/validataclass/exceptions/number_exceptions.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/exceptions/string_exceptions.py` & `validataclass-0.9.0/src/validataclass/exceptions/string_exceptions.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/helpers/__init__.py` & `validataclass-0.9.0/src/validataclass/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/helpers/dataclass_defaults.py` & `validataclass-0.9.0/src/validataclass/helpers/dataclass_defaults.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/helpers/dataclass_mixins.py` & `validataclass-0.9.0/src/validataclass/helpers/dataclass_mixins.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/helpers/dataclasses.py` & `validataclass-0.9.0/src/validataclass/helpers/dataclasses.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/helpers/datetime_range.py` & `validataclass-0.9.0/src/validataclass/helpers/datetime_range.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/helpers/unset_value.py` & `validataclass-0.9.0/src/validataclass/helpers/unset_value.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 
     def __str__(self):
         return '<UnsetValue>'
 
     def __bool__(self):
         return False
 
-    def __eq__(self, other):
-        return other is self
+    # Don't define __eq__ because the default implementation is fine (identity check), and because we would then have to
+    # implement __hash__ as well, otherwise UnsetValue would be considered mutable by @dataclass.
 
 
 # Create sentinel object and redefine __new__ so that the object cannot be cloned
 UnsetValue = UnsetValueType()
 UnsetValueType.__new__ = lambda cls: UnsetValue
 
 # Type alias OptionalUnset[T] for fields with DefaultUnset (similar to Optional[T] but using UnsetValueType instead of NoneType)
```

### Comparing `validataclass-0.8.1/src/validataclass/internal/internet_helpers.py` & `validataclass-0.9.0/src/validataclass/internal/internet_helpers.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/validators/__init__.py` & `validataclass-0.9.0/src/validataclass/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/validators/allow_empty_string.py` & `validataclass-0.9.0/src/validataclass/validators/allow_empty_string.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/validators/any_of_validator.py` & `validataclass-0.9.0/src/validataclass/validators/any_of_validator.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/validators/anything_validator.py` & `validataclass-0.9.0/src/validataclass/validators/anything_validator.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/validators/big_integer_validator.py` & `validataclass-0.9.0/src/validataclass/validators/big_integer_validator.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/validators/boolean_validator.py` & `validataclass-0.9.0/src/validataclass/validators/boolean_validator.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/validators/dataclass_validator.py` & `validataclass-0.9.0/src/validataclass/validators/dataclass_validator.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 validataclass
 Copyright (c) 2021, binary butterfly GmbH and contributors
 Use of this source code is governed by an MIT-style license that can be found in the LICENSE file.
 """
 
 import dataclasses
 import inspect
+import warnings
 from typing import Any, Dict, Generic, Optional, Type, TypeVar
 
 from validataclass.dataclasses import Default, NoDefault
 from validataclass.exceptions import ValidationError, DataclassValidatorFieldException, DataclassPostValidationError, \
     InvalidValidatorOptionException
 from . import Validator, DictValidator
 
@@ -63,31 +64,28 @@
 
     All fields that do NOT specify a default value (or explicitly use the special value `NoDefault`) are required.
 
     Post-validation checks can be implemented in the dataclass either using the `__post_init__()` special method (which
     is part of regular dataclasses and thus also works without validataclass) or using a `__post_validate__()` method
     (which is called by the DataclassValidator after creating the object). The latter also supports *context-sensitive*
     validation, which means you can pass extra arguments to the `validate()` call that will be passed both to all field
-    validators and to the `__post_validate__()` method (as long as it is defined with a `**kwargs` argument).
+    validators and to the `__post_validate__()` method (as long as it is defined to accept the keyword arguments).
 
     In post-validation you can either raise regular `ValidationError` exceptions, which will be automatically wrapped
     inside a `DataclassPostValidationError` exception, or raise such an exception directly (in which case you can
     also specify errors for individual fields, which provides more precise errors to the user).
 
     Here is an example for such a `__post_validate__()` method that also happens to be context-sensitive:
 
     ```
     @validataclass
     class ExampleDataclass:
         optional_field: str = StringValidator(), Default('')
 
-        # Note: The method MUST accept arbitrary keyword arguments (**kwargs), not just the parameter you defined,
-        # otherwise no context arguments will be passed to it at all. To avoid "unused parameter" notices, you can
-        # prepend the variable name with an underscore.
-        def __post_validate__(self, *, require_optional_field: bool = False, **_kwargs):
+        def __post_validate__(self, *, require_optional_field: bool = False):
             if require_optional_field and not self.optional_field:
                 raise DataclassPostValidationError(field_errors={
                     'value': RequiredValueError(reason='The optional field is required for some reason.'),
                 })
     ```
 
     In this example, the field "optional_field" is usually optional, but there are cases where you need the field to be
@@ -212,14 +210,30 @@
     @staticmethod
     def _post_validate(validated_object: T_Dataclass, **kwargs) -> T_Dataclass:
         """
         Post-validation steps: Calls the `__post_validate__()` method on the dataclass object (if it is defined).
         """
         # Post validation using the custom __post_validate__() method in the dataclass (if defined)
         if hasattr(validated_object, '__post_validate__'):
-            # Only pass context arguments if __post_validate__() accepts them
-            if inspect.getfullargspec(validated_object.__post_validate__).varkw is not None:
-                validated_object.__post_validate__(**kwargs)
+            post_validate_spec = inspect.getfullargspec(validated_object.__post_validate__)
+
+            # Warn about __post_validate__() with positional arguments (ignoring "self")
+            if len(post_validate_spec.args) > 1 or post_validate_spec.varargs:
+                warnings.warn(
+                    f'{validated_object.__class__.__name__}.__post_validate__() is defined with positional arguments. '
+                    'This should still work, but it is recommended to use keyword-only arguments instead.'
+                )
+
+            # If __post_validate__() accepts arbitrary keyword arguments (**kwargs), we can just pass all keyword
+            # arguments to the function. Otherwise we need to filter out all keys that are not accepted as keyword
+            # arguments by the function.
+            if post_validate_spec.varkw is not None:
+                context_kwargs = kwargs
             else:
-                validated_object.__post_validate__()
+                context_kwargs = {
+                    key: value for key, value in kwargs.items()
+                    if key in post_validate_spec.kwonlyargs + post_validate_spec.args
+                }
+
+            validated_object.__post_validate__(**context_kwargs)
 
         return validated_object
```

### Comparing `validataclass-0.8.1/src/validataclass/validators/date_validator.py` & `validataclass-0.9.0/src/validataclass/validators/date_validator.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/validators/datetime_validator.py` & `validataclass-0.9.0/src/validataclass/validators/datetime_validator.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/validators/decimal_validator.py` & `validataclass-0.9.0/src/validataclass/validators/decimal_validator.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/validators/dict_validator.py` & `validataclass-0.9.0/src/validataclass/validators/dict_validator.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/validators/discard_validator.py` & `validataclass-0.9.0/src/validataclass/validators/discard_validator.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/validators/email_validator.py` & `validataclass-0.9.0/src/validataclass/validators/email_validator.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,23 +26,28 @@
     Please note that this validator is a bit opinionated and simplified in that it does *not* allow every email address
     that technically is valid according to the RFCs. For example, it does neither allow internationalized email
     addresses (although this might be changed in the future), nor oddities like quoted strings as local part or comments,
     because most mail software does not support those anyway and/or might break with those addresses.
 
     Set the parameter `allow_empty=True` to allow empty strings as input.
 
+    To automatically convert the output email address to lowercase, you can set the parameter `to_lowercase=True`.
+
     By default, the maximum string length is set to 256 characters. This can be changed with the `max_length` parameter.
 
     Example:
 
     ```
     EmailValidator()
 
     # Accepts also empty strings
     EmailValidator(allow_empty=True)
+
+    # Converts email addresses to lowercase (e.g. "Foo.Bar@Example.COM" -> "foo.bar@example.com")
+    EmailValidator(to_lowercase=True)
     ```
 
     Valid input: email address as `str` (also empty strings if `allow_empty=True`)
     Output: `str`
     """
 
     # Precompiled regular expression
@@ -51,34 +56,41 @@
         @
         (?P<domain> [^@?]+ )
     ''', re.IGNORECASE | re.VERBOSE)
 
     # Whether to accept empty strings
     allow_empty: bool = False
 
+    # Whether to automatically convert strings to lowercase
+    to_lowercase: bool = False
+
     def __init__(
         self,
         *,
         allow_empty: bool = False,
+        to_lowercase: bool = False,
         max_length: int = 256,
     ):
         """
         Create a `EmailValidator`.
 
         Parameters:
-            allow_empty: Boolean, if True, empty strings are accepted as valid email addresses (default: False)
+            allow_empty: Boolean, if True, empty strings are accepted as valid input (default: False)
+            to_lowercase: Boolean, if True, the output will be automatically converted to lowercase (default: False)
             max_length: Integer, maximum length of input string (default: 256)
         """
-        self.allow_empty = allow_empty
-
-        # Allow string with length 0 if `allow_empty=True`
-        min_length = 0 if allow_empty else 1
-
         # Initialize StringValidator with some length requirements
-        super().__init__(min_length=min_length, max_length=max_length)
+        super().__init__(
+            min_length=0 if allow_empty else 1,
+            max_length=max_length,
+        )
+
+        # Save parameters
+        self.allow_empty = allow_empty
+        self.to_lowercase = to_lowercase
 
     def validate(self, input_data: Any, **kwargs) -> str:
         """
         Validate that input is a valid email address string. Returns unmodified string.
         """
         # Validate input data as string
         input_email = super().validate(input_data, **kwargs)
@@ -98,9 +110,13 @@
             raise InvalidEmailError(reason='Local part is too long.')
 
         # Validate domain
         email_domain = regex_match.group('domain')
         if not internet_helpers.validate_domain_name(email_domain, require_tld=True):
             raise InvalidEmailError(reason='Domain not valid.')
 
+        # Convert to lowercase (if enabled)
+        if self.to_lowercase:
+            input_email = input_email.lower()
+
         # Email address is valid :)
         return input_email
```

### Comparing `validataclass-0.8.1/src/validataclass/validators/enum_validator.py` & `validataclass-0.9.0/src/validataclass/validators/enum_validator.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/validators/float_to_decimal_validator.py` & `validataclass-0.9.0/src/validataclass/validators/float_to_decimal_validator.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/validators/float_validator.py` & `validataclass-0.9.0/src/validataclass/validators/float_validator.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/validators/integer_validator.py` & `validataclass-0.9.0/src/validataclass/validators/integer_validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,16 +52,16 @@
     so for example `-1234567` would be valid input!
 
     Valid input: `int` (also `str` if `allow_strings=True`)
     Output: `int`
     """
 
     # Constants (minimum and maximum values for a 32 bit integer)
-    DEFAULT_MIN_VALUE = -2147483648  # -2^32
-    DEFAULT_MAX_VALUE = 2147483647  # 2^32 - 1
+    DEFAULT_MIN_VALUE = -2147483648  # -2^31
+    DEFAULT_MAX_VALUE = 2147483647  # 2^31 - 1
 
     # Value constraints
     min_value: Optional[int] = None
     max_value: Optional[int] = None
 
     # Whether to allow integers as strings
     allow_strings: bool = False
```

### Comparing `validataclass-0.8.1/src/validataclass/validators/list_validator.py` & `validataclass-0.9.0/src/validataclass/validators/list_validator.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/validators/none_to_unset_value.py` & `validataclass-0.9.0/src/validataclass/validators/none_to_unset_value.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/validators/noneable.py` & `validataclass-0.9.0/src/validataclass/validators/noneable.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/validators/numeric_validator.py` & `validataclass-0.9.0/src/validataclass/validators/numeric_validator.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/validators/regex_validator.py` & `validataclass-0.9.0/src/validataclass/validators/regex_validator.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/validators/reject_validator.py` & `validataclass-0.9.0/src/validataclass/validators/reject_validator.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/validators/string_validator.py` & `validataclass-0.9.0/src/validataclass/validators/string_validator.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/validators/time_validator.py` & `validataclass-0.9.0/src/validataclass/validators/time_validator.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/validators/url_validator.py` & `validataclass-0.9.0/src/validataclass/validators/url_validator.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass/validators/validator.py` & `validataclass-0.9.0/src/validataclass/validators/validator.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/src/validataclass.egg-info/PKG-INFO` & `validataclass-0.9.0/src/validataclass.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validataclass
-Version: 0.8.1
+Version: 0.9.0
 Summary: Library for input validation designed for (but not restricted to) JSON-based APIs, neatly integrating with dataclasses.
 Home-page: https://github.com/binary-butterfly/validataclass
 Author: binary butterfly GmbH
 Author-email: lexi.stelter@binary-butterfly.de
 License: MIT
 Project-URL: Documentation, https://github.com/binary-butterfly/validataclass/blob/main/docs/index.md
 Project-URL: Changelog, https://github.com/binary-butterfly/validataclass/blob/main/CHANGELOG.md
@@ -14,14 +14,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
```

### Comparing `validataclass-0.8.1/src/validataclass.egg-info/SOURCES.txt` & `validataclass-0.9.0/src/validataclass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/dataclasses/_helpers.py` & `validataclass-0.9.0/tests/dataclasses/_helpers.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/dataclasses/defaults_test.py` & `validataclass-0.9.0/tests/dataclasses/defaults_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -83,14 +83,20 @@
         ]
     )
     def test_default_non_equality(first, second):
         """ Test non-equality between Default and other objects. """
         assert first != second
         assert second != first
 
+    @staticmethod
+    @pytest.mark.parametrize('value', [None, 0, 42, 'banana'])
+    def test_default_hashable(value):
+        """ Test hashability (__hash__) of Default objects. """
+        assert hash(Default(value)) == hash(value)
+
 
 class DefaultFactoryTest:
     """ Tests for the DefaultFactory class. """
 
     @staticmethod
     def test_default_factory_repr():
         """ Test DefaultFactory __repr__ method. """
@@ -163,14 +169,19 @@
         ]
     )
     def test_default_factory_non_equality(first, second):
         """ Test non-equality between DefaultFactory and other objects. """
         assert first != second
         assert second != first
 
+    @staticmethod
+    def test_default_factory_hashable():
+        """ Test hashability (__hash__) of DefaultFactory objects. """
+        assert hash(DefaultFactory(list)) == hash(list)
+
 
 class DefaultUnsetTest:
     """ Tests for the DefaultUnset sentinel object. """
 
     @staticmethod
     def test_default_unset():
         """ Test the DefaultUnset sentinel object. """
@@ -235,10 +246,15 @@
     @pytest.mark.parametrize('other', [None, Default(None), UnsetValue, DefaultUnset, DefaultFactory(lambda: None)])
     def test_no_default_non_equality(other):
         """ Test non-equality between NoDefault and other objects. """
         assert NoDefault != other
         assert other != NoDefault
 
     @staticmethod
+    def test_no_default_hashable():
+        """ Test that NoDefault is hashable (i.e. implements __hash__). """
+        assert hash(NoDefault) == object.__hash__(NoDefault)
+
+    @staticmethod
     def test_no_default_call():
         """ Test that calling NoDefault returns the sentinel itself. """
         assert NoDefault() is NoDefault
```

### Comparing `validataclass-0.8.1/tests/dataclasses/validataclass_field_test.py` & `validataclass-0.9.0/tests/dataclasses/validataclass_field_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/dataclasses/validataclass_mixin_test.py` & `validataclass-0.9.0/tests/dataclasses/validataclass_mixin_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/dataclasses/validataclass_test.py` & `validataclass-0.9.0/tests/dataclasses/validataclass_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/exceptions/common_exceptions_test.py` & `validataclass-0.9.0/tests/exceptions/common_exceptions_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/exceptions/dataclass_exceptions_test.py` & `validataclass-0.9.0/tests/exceptions/dataclass_exceptions_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/exceptions/dict_exceptions_test.py` & `validataclass-0.9.0/tests/exceptions/dict_exceptions_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/exceptions/list_exceptions_test.py` & `validataclass-0.9.0/tests/exceptions/list_exceptions_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/helpers/_compatibility_imports_test.py` & `validataclass-0.9.0/tests/helpers/_compatibility_imports_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/helpers/datetime_range_test.py` & `validataclass-0.9.0/tests/helpers/datetime_range_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/helpers/unset_value_test.py` & `validataclass-0.9.0/tests/helpers/unset_value_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/internal/internet_helpers_test.py` & `validataclass-0.9.0/tests/internal/internet_helpers_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/test_utils.py` & `validataclass-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/test_utils_test.py` & `validataclass-0.9.0/tests/test_utils_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/validators/allow_empty_string_test.py` & `validataclass-0.9.0/tests/validators/allow_empty_string_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/validators/any_of_validator_test.py` & `validataclass-0.9.0/tests/validators/any_of_validator_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/validators/anything_validator_test.py` & `validataclass-0.9.0/tests/validators/anything_validator_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/validators/big_integer_validator_test.py` & `validataclass-0.9.0/tests/validators/big_integer_validator_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/validators/boolean_validator_test.py` & `validataclass-0.9.0/tests/validators/boolean_validator_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/validators/dataclass_validator_test.py` & `validataclass-0.9.0/tests/validators/dataclass_validator_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -90,21 +90,59 @@
 
     The class has a field "name" that is always required, and a field "value" which usually is optional, but required
     when the context argument "value_required" is set.
     """
     name: str = UnitTestContextValidator()
     value: Optional[int] = (IntegerValidator(), Default(None))
 
-    def __post_validate__(self, *, value_required: bool = False, **_kwargs):
+    def __post_validate__(self, *, value_required: bool = False):
         if value_required and self.value is None:
             raise DataclassPostValidationError(field_errors={
                 'value': RequiredValueError(reason='Value is required in this context.'),
             })
 
 
+@validataclass
+class UnitTestContextSensitiveDataclassWithPosArgs(UnitTestContextSensitiveDataclass):
+    """
+    Dataclass with a __post_validate__() method that takes *positional* arguments. This should work, but emit a warning.
+    """
+
+    # Same as UnitTestContextSensitiveDataclass, but with positional arguments
+    def __post_validate__(self, value_required: bool = False):
+        super().__post_validate__(value_required=value_required)
+
+
+# Regex-escaped warning text emitted when using __post_validate__ of the dataclass above
+POST_VALIDATE_POS_ARGS_WARNING = \
+    r'UnitTestContextSensitiveDataclassWithPosArgs\.__post_validate__\(\) is defined with positional arguments'
+
+
+@validataclass
+class UnitTestContextSensitiveDataclassWithVarKwargs:
+    """
+    Dataclass with a __post_validate__() method that takes fixed *and* variable keyword arguments (`**kwargs`).
+
+    This class only has one validated field "name". Additionally it takes two context parameters "ctx_a" and "ctx_b", as
+    well as arbitrary keyword arguments, which will be written into the attributes "ctx_a", "ctx_b" and "extra_kwargs"
+    respectively.
+    """
+    name: str = UnitTestContextValidator()
+
+    # These are no validated fields, just attributes that are populated by __post_validate__
+    ctx_a = None
+    ctx_b = None
+    extra_kwargs = None
+
+    def __post_validate__(self, *, ctx_a: str = '', ctx_b: str = '', **kwargs):
+        self.ctx_a = ctx_a
+        self.ctx_b = ctx_b
+        self.extra_kwargs = kwargs
+
+
 class DataclassValidatorTest:
     # Tests for DataclassValidator with a simple dataclass
 
     @staticmethod
     def test_dataclass_valid():
         """ Validate a dictionary as a dataclass, using valid data. """
         validator = DataclassValidator(UnitTestDataclass)
@@ -447,14 +485,79 @@
                 'value': {
                     'code': 'required_value',
                     'reason': 'Value is required in this context.',
                 },
             },
         }
 
+    @staticmethod
+    def test_dataclass_with_context_sensitive_post_validate_with_pos_args():
+        """ Validate dataclass with a __post_validate__() method that accepts positional arguments. """
+        validator = DataclassValidator(UnitTestContextSensitiveDataclassWithPosArgs)
+
+        with pytest.warns(UserWarning, match=POST_VALIDATE_POS_ARGS_WARNING):
+            validated_data = validator.validate({'name': 'banana', 'value': 13}, value_required=True, foo=42)
+
+        assert validated_data.name == "banana / {'value_required': True, 'foo': 42}"
+        assert validated_data.value == 13
+
+    @staticmethod
+    def test_dataclass_with_context_sensitive_post_validate_with_pos_args_invalid():
+        """ Validate dataclass with a __post_validate__() method that accepts positional arguments, with invalid input. """
+        validator = DataclassValidator(UnitTestContextSensitiveDataclassWithPosArgs)
+
+        with pytest.raises(DataclassPostValidationError):
+            with pytest.warns(UserWarning, match=POST_VALIDATE_POS_ARGS_WARNING):
+                validator.validate({'name': 'banana'}, value_required=True)
+
+    @staticmethod
+    @pytest.mark.parametrize(
+        'validate_kwargs, expected_ctx_a, expected_ctx_b, expected_extra_kwargs',
+        [
+            # No context arguments
+            ({}, '', '', {}),
+
+            # Only context parameters defined as keyword arguments in __post_validate__ (ctx_a, ctx_b)
+            ({'ctx_a': 'foo'}, 'foo', '', {}),
+            ({'ctx_b': 'bar'}, '', 'bar', {}),
+            ({'ctx_b': 'bar', 'ctx_a': 'foo'}, 'foo', 'bar', {}),
+
+            # Arbitrary context arguments not defined as keyword arguments in __post_validate__
+            (
+                {'some_value': 42},
+                '',
+                '',
+                {'some_value': 42},
+            ),
+            (
+                {'ctx_a': 'foo', 'some_value': 42},
+                'foo',
+                '',
+                {'some_value': 42},
+            ),
+            (
+                {'any_value': 3, 'ctx_a': 'foo', 'some_value': 42, 'ctx_b': 'bar'},
+                'foo',
+                'bar',
+                {'any_value': 3, 'some_value': 42},
+            ),
+        ]
+    )
+    def test_dataclass_with_context_sensitive_post_validate_with_var_kwargs(
+        validate_kwargs, expected_ctx_a, expected_ctx_b, expected_extra_kwargs,
+    ):
+        """ Validate dataclass with a context-sensitive __post_validate__() method that accepts arbitrary keyword arguments. """
+        validator = DataclassValidator(UnitTestContextSensitiveDataclassWithVarKwargs)
+        validated_data = validator.validate({'name': 'unit-test'}, **validate_kwargs)
+
+        assert validated_data.name == f"unit-test / {validate_kwargs}"
+        assert validated_data.ctx_a == expected_ctx_a
+        assert validated_data.ctx_b == expected_ctx_b
+        assert validated_data.extra_kwargs == expected_extra_kwargs
+
     # Test invalid validator options
 
     @staticmethod
     def test_invalid_dataclass_validator_without_dataclass():
         """ Test that a DataclassValidator cannot be created without a dataclass. """
         with pytest.raises(InvalidValidatorOptionException) as exception_info:
             DataclassValidator()
```

### Comparing `validataclass-0.8.1/tests/validators/date_validator_test.py` & `validataclass-0.9.0/tests/validators/date_validator_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/validators/datetime_validator_test.py` & `validataclass-0.9.0/tests/validators/datetime_validator_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/validators/decimal_validator_test.py` & `validataclass-0.9.0/tests/validators/decimal_validator_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/validators/dict_validator_test.py` & `validataclass-0.9.0/tests/validators/dict_validator_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/validators/discard_validator_test.py` & `validataclass-0.9.0/tests/validators/discard_validator_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/validators/email_validator_test.py` & `validataclass-0.9.0/tests/validators/email_validator_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,27 +92,48 @@
             validator.validate('abcde@example.com')
         assert exception_info.value.to_dict() == {
             'code': 'string_too_long',
             'min_length': 1,
             'max_length': 16,
         }
 
+    # Test to_lowercase option
+
+    @staticmethod
+    @pytest.mark.parametrize(
+        'to_lowercase, input_string, expected_output', [
+            # Default behaviour: Keep uppercase letters intact
+            (False, 'foo@example.com', 'foo@example.com'),
+            (False, 'Foo.Bar@Example.COM', 'Foo.Bar@Example.COM'),
+
+            # Set to_lowercase=True
+            (True, 'foo@example.com', 'foo@example.com'),
+            (True, 'Foo.Bar@Example.COM', 'foo.bar@example.com'),
+        ]
+    )
+    def test_email_to_lowercase(to_lowercase, input_string, expected_output):
+        """ Test EmailValidator with the to_lowercase option. """
+        validator = EmailValidator(to_lowercase=to_lowercase)
+        assert validator.validate(input_string) == expected_output
+
     # Tests for regex validation of email address format
 
     @staticmethod
     @pytest.mark.parametrize(
         'input_string', [
             # Regular addresses (with some odd but valid characters)
             'a@example.com',
             '~foo-123+bar{banana}@some.sub.domain.example.com',
             # Addresses with dots at valid positions
             'foo.bar@example.com',
             'a.b.c.d.e@example.com',
             # Very long local part (up to 64 characters are allowed)
-            'fooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooo@example.com'
+            'fooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooo@example.com',
+            # Addresses with uppercase letters (should be left intact by default)
+            'Foo.Bar@Example.COM',
         ]
     )
     def test_email_regex_valid(input_string):
         """ Test EmailValidator regex validation with valid strings. """
         validator = EmailValidator()
         assert validator.validate(input_string) == input_string
 
@@ -125,17 +146,17 @@
             'foo\\bar@example.com',
             'foo bar@example.com',
             # Invalid dot positions
             '.banana@example.com',
             'banana.@example.com',
             'bana..na@example.com',
             # Multiple @ characters
-            'foo@bar@example.com'
+            'foo@bar@example.com',
             # Query part
-            'foobar@example.com?subject=foo'
+            'foobar@example.com?subject=foo',
         ]
     )
     def test_email_regex_invalid(input_string):
         """ Test EmailValidator regex validation with invalid strings. """
         validator = EmailValidator()
         with pytest.raises(InvalidEmailError) as exception_info:
             validator.validate(input_string)
```

### Comparing `validataclass-0.8.1/tests/validators/enum_validator_test.py` & `validataclass-0.9.0/tests/validators/enum_validator_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/validators/float_to_decimal_validator_test.py` & `validataclass-0.9.0/tests/validators/float_to_decimal_validator_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/validators/float_validator_test.py` & `validataclass-0.9.0/tests/validators/float_validator_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/validators/integer_validator_test.py` & `validataclass-0.9.0/tests/validators/integer_validator_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/validators/list_validator_test.py` & `validataclass-0.9.0/tests/validators/list_validator_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/validators/none_to_unset_value_test.py` & `validataclass-0.9.0/tests/validators/none_to_unset_value_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/validators/noneable_test.py` & `validataclass-0.9.0/tests/validators/noneable_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/validators/numeric_validator_test.py` & `validataclass-0.9.0/tests/validators/numeric_validator_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/validators/regex_validator_test.py` & `validataclass-0.9.0/tests/validators/regex_validator_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/validators/reject_validator_test.py` & `validataclass-0.9.0/tests/validators/reject_validator_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/validators/string_validator_test.py` & `validataclass-0.9.0/tests/validators/string_validator_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/validators/time_validator_test.py` & `validataclass-0.9.0/tests/validators/time_validator_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/validators/url_validator_test.py` & `validataclass-0.9.0/tests/validators/url_validator_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tests/validators/validator_test.py` & `validataclass-0.9.0/tests/validators/validator_test.py`

 * *Files identical despite different names*

### Comparing `validataclass-0.8.1/tox.ini` & `validataclass-0.9.0/tox.ini`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [tox]
-envlist = clean,py{310,39,38,37},flake8,report
+minversion = 4.5.1
+envlist = clean,py{311,310,39,38,37},flake8,report
 skip_missing_interpreters = true
 isolated_build = true
 
 [flake8]
 max-line-length = 139
 exclude = _version.py
 ignore =
@@ -21,22 +22,15 @@
 commands = flake8 src/ tests/
 
 [testenv:clean]
 skip_install = true
 deps = {[testenv:report]deps}
 commands = coverage erase
 
-[testenv:report]
+[testenv:report,py{311,310,39,38,37}-report]
 skip_install = true
 deps =
     coverage
     coverage-conditional-plugin
 commands =
     coverage html
     coverage report --fail-under=100
-
-# These environments basically are an alias for "report" that allow to specify the python version used for coverage.
-# tox 4 apparently will have a "labels" option that can be used to define aliases, but that version is not released yet.
-[testenv:py{310,39,38,37}-report]
-skip_install = true
-deps = {[testenv:report]deps}
-commands = {[testenv:report]commands}
```

