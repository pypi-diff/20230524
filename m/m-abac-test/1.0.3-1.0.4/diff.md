# Comparing `tmp/m-abac-test-1.0.3.tar.gz` & `tmp/m-abac-test-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m-abac-test-1.0.3.tar", last modified: Fri May 19 09:35:50 2023, max compression
+gzip compressed data, was "m-abac-test-1.0.4.tar", last modified: Wed May 24 07:58:47 2023, max compression
```

## Comparing `m-abac-test-1.0.3.tar` & `m-abac-test-1.0.4.tar`

### file list

```diff
@@ -1,96 +1,97 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.055878 m-abac-test-1.0.3/
--rw-r--r--   0 root         (0) root         (0)     1746 2023-05-19 09:35:50.054878 m-abac-test-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      620 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.005876 m-abac-test-1.0.3/m_abac_test.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1746 2023-05-19 09:35:49.000000 m-abac-test-1.0.3/m_abac_test.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3699 2023-05-19 09:35:49.000000 m-abac-test-1.0.3/m_abac_test.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 09:35:49.000000 m-abac-test-1.0.3/m_abac_test.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-19 09:35:49.000000 m-abac-test-1.0.3/m_abac_test.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-19 09:35:49.000000 m-abac-test-1.0.3/m_abac_test.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:49.996876 m-abac-test-1.0.3/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:49.996876 m-abac-test-1.0.3/mobio/libs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.007876 m-abac-test-1.0.3/mobio/libs/abac/
--rw-r--r--   0 root         (0) root         (0)       70 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.009876 m-abac-test-1.0.3/mobio/libs/abac/adapter/
--rw-r--r--   0 root         (0) root         (0)      267 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/adapter/__init__.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/adapter/adapter.py
--rw-r--r--   0 root         (0) root         (0)    15511 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/adapter/elasticsearch_adapter.py
--rw-r--r--   0 root         (0) root         (0)     8301 2023-05-19 09:33:30.000000 m-abac-test-1.0.3/mobio/libs/abac/call_api.py
--rw-r--r--   0 root         (0) root         (0)    12709 2023-05-19 09:33:30.000000 m-abac-test-1.0.3/mobio/libs/abac/pdp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.012877 m-abac-test-1.0.3/mobio/libs/abac/policy/
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.014876 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      662 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.016877 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/boolean/
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/boolean/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1127 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/boolean/base.py
--rw-r--r--   0 root         (0) root         (0)     1107 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/boolean/check_bool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.023877 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/
--rw-r--r--   0 root         (0) root         (0)      323 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/__init__.py
--rw-r--r--   0 root         (0) root         (0)      629 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/all_in.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/all_not_in.py
--rw-r--r--   0 root         (0) root         (0)      638 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/any_in.py
--rw-r--r--   0 root         (0) root         (0)      664 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/any_not_in.py
--rw-r--r--   0 root         (0) root         (0)     1341 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/base.py
--rw-r--r--   0 root         (0) root         (0)      754 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/is_empty.py
--rw-r--r--   0 root         (0) root         (0)      602 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/is_in.py
--rw-r--r--   0 root         (0) root         (0)      774 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
--rw-r--r--   0 root         (0) root         (0)      728 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/is_not_in.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.030877 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/
--rw-r--r--   0 root         (0) root         (0)      243 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2524 2023-05-19 09:33:30.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/base.py
--rw-r--r--   0 root         (0) root         (0)     1345 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_eq.py
--rw-r--r--   0 root         (0) root         (0)     1367 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_gt.py
--rw-r--r--   0 root         (0) root         (0)     1389 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_gte.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_lt.py
--rw-r--r--   0 root         (0) root         (0)     1380 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_lte.py
--rw-r--r--   0 root         (0) root         (0)     1363 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.035877 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1839 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/base.py
--rw-r--r--   0 root         (0) root         (0)     1004 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/day_eq.py
--rw-r--r--   0 root         (0) root         (0)      975 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/day_gt.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/day_gte.py
--rw-r--r--   0 root         (0) root         (0)      974 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/day_lt.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/day_lte.py
--rw-r--r--   0 root         (0) root         (0)      978 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/day_neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.038877 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/ip_address/
--rw-r--r--   0 root         (0) root         (0)       82 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/ip_address/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/ip_address/base.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.043877 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/
--rw-r--r--   0 root         (0) root         (0)      188 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1450 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/base.py
--rw-r--r--   0 root         (0) root         (0)      853 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/eq.py
--rw-r--r--   0 root         (0) root         (0)      871 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/gt.py
--rw-r--r--   0 root         (0) root         (0)      895 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/gte.py
--rw-r--r--   0 root         (0) root         (0)      863 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/lt.py
--rw-r--r--   0 root         (0) root         (0)      886 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/lte.py
--rw-r--r--   0 root         (0) root         (0)      869 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.045877 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/others/
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/others/__init__.py
--rw-r--r--   0 root         (0) root         (0)      963 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/others/base.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/others/exists.py
--rw-r--r--   0 root         (0) root         (0)      701 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/others/not_exists.py
--rw-r--r--   0 root         (0) root         (0)     2126 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:35:50.053878 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/
--rw-r--r--   0 root         (0) root         (0)      401 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/base.py
--rw-r--r--   0 root         (0) root         (0)     1213 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/contains.py
--rw-r--r--   0 root         (0) root         (0)     1245 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/ends_with.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/equals.py
--rw-r--r--   0 root         (0) root         (0)     1227 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/not_contains.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/not_ends_with.py
--rw-r--r--   0 root         (0) root         (0)     1214 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/not_equals.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/not_starts_with.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/regex_match.py
--rw-r--r--   0 root         (0) root         (0)     1264 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/starts_with.py
--rw-r--r--   0 root         (0) root         (0)     1601 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     6037 2023-05-19 09:33:30.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/policy.py
--rw-r--r--   0 root         (0) root         (0)     5139 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/mobio/libs/abac/policy/utils.py
--rw-r--r--   0 root         (0) root         (0)     3631 2023-05-19 09:33:30.000000 m-abac-test-1.0.3/mobio/libs/abac/result_access.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-15 08:15:49.000000 m-abac-test-1.0.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 09:35:50.055878 m-abac-test-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     9779 2023-05-19 09:35:49.000000 m-abac-test-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.335215 m-abac-test-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-05-24 07:58:47.331215 m-abac-test-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      620 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.279214 m-abac-test-1.0.4/m_abac_test.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-05-24 07:58:46.000000 m-abac-test-1.0.4/m_abac_test.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3725 2023-05-24 07:58:47.000000 m-abac-test-1.0.4/m_abac_test.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:58:46.000000 m-abac-test-1.0.4/m_abac_test.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-24 07:58:46.000000 m-abac-test-1.0.4/m_abac_test.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-24 07:58:46.000000 m-abac-test-1.0.4/m_abac_test.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.269213 m-abac-test-1.0.4/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.269213 m-abac-test-1.0.4/mobio/libs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.282214 m-abac-test-1.0.4/mobio/libs/abac/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.284214 m-abac-test-1.0.4/mobio/libs/abac/adapter/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/adapter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/adapter/adapter.py
+-rw-r--r--   0 root         (0) root         (0)    15511 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/adapter/elasticsearch_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     7837 2023-05-24 07:57:21.000000 m-abac-test-1.0.4/mobio/libs/abac/call_api.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-05-24 07:57:21.000000 m-abac-test-1.0.4/mobio/libs/abac/config.py
+-rw-r--r--   0 root         (0) root         (0)    13319 2023-05-24 07:57:21.000000 m-abac-test-1.0.4/mobio/libs/abac/pdp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.287214 m-abac-test-1.0.4/mobio/libs/abac/policy/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.288214 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      662 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.290214 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/boolean/
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/boolean/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/boolean/base.py
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/boolean/check_bool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.296214 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/
+-rw-r--r--   0 root         (0) root         (0)      323 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      629 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/all_in.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/all_not_in.py
+-rw-r--r--   0 root         (0) root         (0)      638 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/any_in.py
+-rw-r--r--   0 root         (0) root         (0)      664 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/any_not_in.py
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/base.py
+-rw-r--r--   0 root         (0) root         (0)      754 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/is_empty.py
+-rw-r--r--   0 root         (0) root         (0)      602 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/is_in.py
+-rw-r--r--   0 root         (0) root         (0)      774 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
+-rw-r--r--   0 root         (0) root         (0)      728 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/is_not_in.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.302214 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/
+-rw-r--r--   0 root         (0) root         (0)      243 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2023-05-19 09:33:30.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/base.py
+-rw-r--r--   0 root         (0) root         (0)     1345 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_eq.py
+-rw-r--r--   0 root         (0) root         (0)     1367 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_gt.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_gte.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_lt.py
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_lte.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.309214 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/base.py
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/day_eq.py
+-rw-r--r--   0 root         (0) root         (0)      975 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/day_gt.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/day_gte.py
+-rw-r--r--   0 root         (0) root         (0)      974 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/day_lt.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/day_lte.py
+-rw-r--r--   0 root         (0) root         (0)      978 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/day_neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.314214 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/ip_address/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/ip_address/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/ip_address/base.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.319214 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/
+-rw-r--r--   0 root         (0) root         (0)      188 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/base.py
+-rw-r--r--   0 root         (0) root         (0)      853 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/eq.py
+-rw-r--r--   0 root         (0) root         (0)      871 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/gt.py
+-rw-r--r--   0 root         (0) root         (0)      895 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/gte.py
+-rw-r--r--   0 root         (0) root         (0)      863 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/lt.py
+-rw-r--r--   0 root         (0) root         (0)      886 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/lte.py
+-rw-r--r--   0 root         (0) root         (0)      869 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.322215 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/others/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/others/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      963 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/others/base.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/others/exists.py
+-rw-r--r--   0 root         (0) root         (0)      701 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/others/not_exists.py
+-rw-r--r--   0 root         (0) root         (0)     2126 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.330215 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/
+-rw-r--r--   0 root         (0) root         (0)      401 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/base.py
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/contains.py
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/ends_with.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/equals.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/not_contains.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/not_ends_with.py
+-rw-r--r--   0 root         (0) root         (0)     1214 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/not_equals.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/not_starts_with.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/regex_match.py
+-rw-r--r--   0 root         (0) root         (0)     1264 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/starts_with.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     6037 2023-05-19 09:33:30.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/policy.py
+-rw-r--r--   0 root         (0) root         (0)     5139 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3631 2023-05-19 09:33:30.000000 m-abac-test-1.0.4/mobio/libs/abac/result_access.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 07:58:47.335215 m-abac-test-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9779 2023-05-24 07:58:45.000000 m-abac-test-1.0.4/setup.py
```

### Comparing `m-abac-test-1.0.3/PKG-INFO` & `m-abac-test-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abac-test
-Version: 1.0.3
+Version: 1.0.4
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: ### ABAC Engine
```

### Comparing `m-abac-test-1.0.3/README.md` & `m-abac-test-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/m_abac_test.egg-info/PKG-INFO` & `m-abac-test-1.0.4/m_abac_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abac-test
-Version: 1.0.3
+Version: 1.0.4
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: ### ABAC Engine
```

### Comparing `m-abac-test-1.0.3/m_abac_test.egg-info/SOURCES.txt` & `m-abac-test-1.0.4/m_abac_test.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 m_abac_test.egg-info/PKG-INFO
 m_abac_test.egg-info/SOURCES.txt
 m_abac_test.egg-info/dependency_links.txt
 m_abac_test.egg-info/requires.txt
 m_abac_test.egg-info/top_level.txt
 mobio/libs/abac/__init__.py
 mobio/libs/abac/call_api.py
+mobio/libs/abac/config.py
 mobio/libs/abac/pdp.py
 mobio/libs/abac/result_access.py
 mobio/libs/abac/adapter/__init__.py
 mobio/libs/abac/adapter/adapter.py
 mobio/libs/abac/adapter/elasticsearch_adapter.py
 mobio/libs/abac/policy/__init__.py
 mobio/libs/abac/policy/exceptions.py
```

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/adapter/elasticsearch_adapter.py` & `m-abac-test-1.0.4/mobio/libs/abac/adapter/elasticsearch_adapter.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/call_api.py` & `m-abac-test-1.0.4/mobio/libs/abac/call_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,19 @@
-from mobio.libs.caching import LruCache
-import os, requests
-
-
-class StoreCacheType:
-    LOCAL = 1
-    REDIS = 2
-
-class Cache:
-    REDIS_URI = "{}?health_check_interval=30".format(os.environ.get("ADMIN_REDIS_URI", os.environ.get("REDIS_URI")))
-    PREFIX = "m_abac"
-
-lru_cache_redis = LruCache(
-    store_type=StoreCacheType.REDIS,
-    redis_uri=Cache.REDIS_URI,
-    cache_prefix=Cache.PREFIX,
-)
-
-class Mobio:
-    ADMIN_HOST = os.environ.get("ADMIN_HOST")
-    MOBIO_TOKEN = "Basic {}".format(os.environ.get('YEK_REWOP', ''))
+import requests
 
+from .config import lru_cache_redis, Mobio
 
 
 class APIRequest:
     TimeOut = 10
     ADMIN_GET_FULL_INFO_ACCOUNT = "{domain}/adm/api/v2.1/accounts/{account_id}/full-info"
     ADMIN_GET_LIST_ACTION_FOR_MERCHANT = "{domain}/adm/api/v2.1/policies/actions"
     ADMIN_GET_LIST_STATEMENT = "{domain}/adm/api/v2.1/statements"
 
+
 class CallAPI:
 
     @lru_cache_redis.add()
     @staticmethod
     def admin_get_account_info(merchant_id, account_id):
         try:
             url = APIRequest.ADMIN_GET_FULL_INFO_ACCOUNT.format(domain=Mobio.ADMIN_HOST, account_id=account_id)
```

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/pdp.py` & `m-abac-test-1.0.4/mobio/libs/abac/pdp.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from copy import deepcopy
 
 from .call_api import CallAPI
 from .policy import PolicySchema, AccessType
 from .policy.utils import Utils
 from .result_access import ResultAccess
-
+from .config import RedisClient
 
 class PolicyDecisionPoint(object):
     """
         Policy decision point
     """
 
     class AccountType:
@@ -36,29 +36,35 @@
                  merchant_id: str = None, resource: str = None, action: str = None, account_id: str = None,
                  user_info: dict = None, data_before: dict = None, data_after: dict = None, environment: dict = None,
                  account_type=AccountType.NORMAL):
         if not resource:
             raise ValueError("resource required")
         if not action:
             raise ValueError("action required")
+        pass_policy = False
         if not merchant_id or not account_id:
             auth_type, json_token = Utils.get_info_jwt()
             if auth_type == self.AuthorizationType.BEARER:
                 merchant_id = json_token.get("merchant_id")
                 account_id = json_token.get("account_id")
             else:
                 account_type = self.AccountType.SYSTEM
         if account_type == PolicyDecisionPoint.AccountType.NORMAL:
             if not merchant_id:
                 raise ValueError("merchant_id required")
             if not account_id:
                 raise ValueError("account normal account_id required")
             if not user_info:
                 user_info = CallAPI.admin_get_account_info(merchant_id, account_id)
+            if not self.check_merchant_use_abac(merchant_id):
+                pass_policy = True
+        elif account_type == PolicyDecisionPoint.AccountType.SYSTEM:
+            pass_policy = True
 
+        self.pass_policy = pass_policy
         self.account_type = account_type
         self.merchant_id = merchant_id
         self.account_id = account_id
         self.resource = resource
         self.action = action
         self.request_access = {}
         self.result_access = ResultAccess()
@@ -68,27 +74,36 @@
             self.resource: data_before if data_before else {}
         })
         self.data_after = data_after if data_after else {}
         self.data_before = data_before if data_before else {}
         self.access_level = ""
         self.service = ""
 
+    def check_merchant_use_abac(self, merchant_id):
+        use_abac = False
+        data_cache = RedisClient().get_value(RedisClient.KeyCache.MERCHANT_USE_ABAC)
+        if data_cache:
+            data_merchant = str(data_cache.decode("utf-8")).split(";")
+            if merchant_id in data_merchant:
+                use_abac = True
+        return use_abac
+
     def get_policy_statement_for_target(self):
         return CallAPI.admin_get_list_statement(self.merchant_id, self.account_id,
                                                 self.resource, self.action, self.service)
 
     def is_allowed(self):
         """
             Check if authorization request is allowed
 
             :param request: request object
             :return: True if authorized else False
         """
         try:
-            if self.account_type == PolicyDecisionPoint.AccountType.SYSTEM:
+            if self.pass_policy:
                 self.result_access.set_allow_access(True)
                 return self.result_access
             action_info = CallAPI.admin_get_json_action(merchant_id=self.merchant_id)
             if not action_info:
                 raise ValueError("action for merchant_id {} not found".format(self.merchant_id))
             if not action_info.get(self.action):
                 raise ValueError("action {} not found".format(self.action))
```

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/base.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/boolean/base.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/boolean/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/boolean/check_bool.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/boolean/check_bool.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/all_in.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/all_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/all_not_in.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/all_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/any_in.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/any_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/any_not_in.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/any_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/base.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/is_empty.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/is_empty.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/is_in.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/is_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/is_not_empty.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/is_not_empty.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/collection/is_not_in.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/is_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/base.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_eq.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_gt.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_gte.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_lt.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_lte.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/date_time/date_neq.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/base.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/day_eq.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/day_eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/day_gt.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/day_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/day_gte.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/day_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/day_lt.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/day_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/day_lte.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/day_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/day/day_neq.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/day_neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/ip_address/base.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/ip_address/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/base.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/eq.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/gt.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/gte.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/lt.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/lte.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/numeric/neq.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/others/base.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/others/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/others/exists.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/others/exists.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/others/not_exists.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/others/not_exists.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/schema.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/schema.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/base.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/contains.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/ends_with.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/ends_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/equals.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/equals.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/not_contains.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/not_contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/not_ends_with.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/not_ends_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/not_equals.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/not_equals.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/not_starts_with.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/not_starts_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/regex_match.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/regex_match.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/conditions/string/starts_with.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/starts_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/exceptions.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/exceptions.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/policy.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/policy.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/policy/utils.py` & `m-abac-test-1.0.4/mobio/libs/abac/policy/utils.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/mobio/libs/abac/result_access.py` & `m-abac-test-1.0.4/mobio/libs/abac/result_access.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.3/setup.py` & `m-abac-test-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         ]
         # with open(Requirements.requirements_path) as req_file:
         #     for line in req_file.read().splitlines():
         #         if not line.strip().startswith("#"):
         #             requirements.append(line)
         return requirements
 
-version_dev='1.0.3'
+version_dev='1.0.4'
 version_prod='1.0.0'
 
 run_mode='-test'
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
@@ -70,15 +70,15 @@
     # options={"bdist_wheel": {"universal": True}},
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.3',  # Required
+    version='1.0.4',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

