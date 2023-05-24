# Comparing `tmp/cqlpy-0.2.4.tar.gz` & `tmp/cqlpy-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cqlpy-0.2.4.tar", max compression
+gzip compressed data, was "cqlpy-0.2.5.tar", max compression
```

## Comparing `cqlpy-0.2.4.tar` & `cqlpy-0.2.5.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0     1070 2023-05-23 01:02:56.408660 cqlpy-0.2.4/LICENSE
--rw-r--r--   0        0        0        8 2023-05-23 01:02:56.408660 cqlpy-0.2.4/README.md
--rw-r--r--   0        0        0        0 2023-05-23 01:02:56.408660 cqlpy-0.2.4/cqlpy/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 01:02:56.408660 cqlpy-0.2.4/cqlpy/_internal/__init__.py
--rw-r--r--   0        0        0     5073 2023-05-23 01:02:56.408660 cqlpy-0.2.4/cqlpy/_internal/context/context.py
--rw-r--r--   0        0        0      748 2023-05-23 01:02:56.408660 cqlpy-0.2.4/cqlpy/_internal/context/cql_value_set_provider.py
--rw-r--r--   0        0        0   335719 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/context/fhir/r4/map.py
--rw-r--r--   0        0        0    16313 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/context/fhir/r4/model.py
--rw-r--r--   0        0        0      689 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/context/parameter_provider.py
--rw-r--r--   0        0        0     2319 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/context/resource_query.py
--rw-r--r--   0        0        0     1696 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/context/type_factory.py
--rw-r--r--   0        0        0       92 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/exceptions.py
--rw-r--r--   0        0        0      123 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/aggregate/count.py
--rw-r--r--   0        0        0      339 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/arithmetic/max_value.py
--rw-r--r--   0        0        0      320 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/arithmetic/min_value.py
--rw-r--r--   0        0        0      691 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/clinical/any_in_valueset.py
--rw-r--r--   0        0        0     1052 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/clinical/in_valueset.py
--rw-r--r--   0        0        0      120 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/comparison/equal.py
--rw-r--r--   0        0        0      511 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/comparison/equivalent.py
--rw-r--r--   0        0        0      735 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/comparison/greater.py
--rw-r--r--   0        0        0      763 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/comparison/greater_or_equal.py
--rw-r--r--   0        0        0      507 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/comparison/in_list.py
--rw-r--r--   0        0        0      726 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/comparison/less.py
--rw-r--r--   0        0        0      753 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/comparison/less_or_equal.py
--rw-r--r--   0        0        0      741 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/comparison/not_equal.py
--rw-r--r--   0        0        0      671 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/cql_in.py
--rw-r--r--   0        0        0     1165 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/date_time/add.py
--rw-r--r--   0        0        0      541 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/date_time/after.py
--rw-r--r--   0        0        0      558 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/date_time/before.py
--rw-r--r--   0        0        0      588 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/date_time/calculate_age_at.py
--rw-r--r--   0        0        0      157 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/date_time/date_time_precision.py
--rw-r--r--   0        0        0      898 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/date_time/difference_between.py
--rw-r--r--   0        0        0      890 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/date_time/duration_between.py
--rw-r--r--   0        0        0      378 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/date_time/same_or_before.py
--rw-r--r--   0        0        0     1181 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/date_time/subtract.py
--rw-r--r--   0        0        0     3800 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/interval/collapse.py
--rw-r--r--   0        0        0      381 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/interval/end.py
--rw-r--r--   0        0        0     1411 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/interval/in_interval.py
--rw-r--r--   0        0        0     1546 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/interval/included_in.py
--rw-r--r--   0        0        0      587 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/interval/overlaps.py
--rw-r--r--   0        0        0      976 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/interval/start.py
--rw-r--r--   0        0        0      348 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/list/distinct.py
--rw-r--r--   0        0        0      230 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/list/exists.py
--rw-r--r--   0        0        0      324 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/list/first.py
--rw-r--r--   0        0        0      291 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/list/flatten.py
--rw-r--r--   0        0        0     2195 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/list/intersect.py
--rw-r--r--   0        0        0      306 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/list/last.py
--rw-r--r--   0        0        0      404 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/list/singleton_from.py
--rw-r--r--   0        0        0      236 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/list/union.py
--rw-r--r--   0        0        0      409 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/nullological/coalesce.py
--rw-r--r--   0        0        0      212 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/nullological/is_false.py
--rw-r--r--   0        0        0      358 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/nullological/is_null.py
--rw-r--r--   0        0        0      193 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/nullological/is_true.py
--rw-r--r--   0        0        0      254 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/sort/sort_by_column.py
--rw-r--r--   0        0        0      134 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/sort/sort_by_direction.py
--rw-r--r--   0        0        0      173 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/sort/sort_by_expression.py
--rw-r--r--   0        0        0       51 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/sort/tuple_sort.py
--rw-r--r--   0        0        0      166 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/string/ends_with.py
--rw-r--r--   0        0        0      170 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/string/split.py
--rw-r--r--   0        0        0      149 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/to_list.py
--rw-r--r--   0        0        0      162 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/type/to_concept.py
--rw-r--r--   0        0        0      280 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/type/to_datetime.py
--rw-r--r--   0        0        0      509 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/parameter.py
--rw-r--r--   0        0        0     9366 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/scripts/fhir_map_generator.py
--rw-r--r--   0        0        0        0 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/__init__.py
--rw-r--r--   0        0        0     2901 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/any.py
--rw-r--r--   0        0        0      988 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/boolean.py
--rw-r--r--   0        0        0     1700 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/code.py
--rw-r--r--   0        0        0      851 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/code_system.py
--rw-r--r--   0        0        0     2459 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/concept.py
--rw-r--r--   0        0        0     1001 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/date.py
--rw-r--r--   0        0        0     2986 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/datetime.py
--rw-r--r--   0        0        0     1128 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/decimal.py
--rw-r--r--   0        0        0      756 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/integer.py
--rw-r--r--   0        0        0     3674 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/interval.py
--rw-r--r--   0        0        0     1605 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/list.py
--rw-r--r--   0        0        0       81 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/long.py
--rw-r--r--   0        0        0      416 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/null.py
--rw-r--r--   0        0        0      887 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/quantity.py
--rw-r--r--   0        0        0     1053 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/string.py
--rw-r--r--   0        0        0     2003 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/value_set.py
--rw-r--r--   0        0        0      170 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/valueset_provider.py
--rw-r--r--   0        0        0      451 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/context.py
--rw-r--r--   0        0        0     4227 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/operators.py
--rw-r--r--   0        0        0        0 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/providers/__init__.py
--rw-r--r--   0        0        0      216 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/providers/logger.py
--rw-r--r--   0        0        0       15 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/providers/requirements.txt
--rw-r--r--   0        0        0     4871 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/providers/rosetta_valueset_provider.py
--rw-r--r--   0        0        0        0 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/py.typed
--rw-r--r--   0        0        0     1089 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/types.py
--rw-r--r--   0        0        0      636 2023-05-23 01:03:18.340855 cqlpy-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 cqlpy-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-24 13:07:49.980195 cqlpy-0.2.5/LICENSE
+-rw-r--r--   0        0        0        8 2023-05-24 13:07:49.980195 cqlpy-0.2.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/__init__.py
+-rw-r--r--   0        0        0     5073 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/context/context.py
+-rw-r--r--   0        0        0      748 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/context/cql_value_set_provider.py
+-rw-r--r--   0        0        0   342427 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/context/fhir/r4/map.py
+-rw-r--r--   0        0        0    16313 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/context/fhir/r4/model.py
+-rw-r--r--   0        0        0      689 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/context/parameter_provider.py
+-rw-r--r--   0        0        0     2319 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/context/resource_query.py
+-rw-r--r--   0        0        0     1696 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/context/type_factory.py
+-rw-r--r--   0        0        0       92 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/exceptions.py
+-rw-r--r--   0        0        0      123 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/operators/aggregate/count.py
+-rw-r--r--   0        0        0      339 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/operators/arithmetic/max_value.py
+-rw-r--r--   0        0        0      320 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/operators/arithmetic/min_value.py
+-rw-r--r--   0        0        0      691 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/operators/clinical/any_in_valueset.py
+-rw-r--r--   0        0        0     1052 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/operators/clinical/in_valueset.py
+-rw-r--r--   0        0        0      120 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/operators/comparison/equal.py
+-rw-r--r--   0        0        0      511 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/operators/comparison/equivalent.py
+-rw-r--r--   0        0        0      735 2023-05-24 13:07:49.980195 cqlpy-0.2.5/cqlpy/_internal/operators/comparison/greater.py
+-rw-r--r--   0        0        0      763 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/comparison/greater_or_equal.py
+-rw-r--r--   0        0        0      507 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/comparison/in_list.py
+-rw-r--r--   0        0        0      726 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/comparison/less.py
+-rw-r--r--   0        0        0      753 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/comparison/less_or_equal.py
+-rw-r--r--   0        0        0      741 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/comparison/not_equal.py
+-rw-r--r--   0        0        0      671 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/cql_in.py
+-rw-r--r--   0        0        0     1165 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/date_time/add.py
+-rw-r--r--   0        0        0      541 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/date_time/after.py
+-rw-r--r--   0        0        0      558 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/date_time/before.py
+-rw-r--r--   0        0        0      588 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/date_time/calculate_age_at.py
+-rw-r--r--   0        0        0      157 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/date_time/date_time_precision.py
+-rw-r--r--   0        0        0      898 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/date_time/difference_between.py
+-rw-r--r--   0        0        0      890 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/date_time/duration_between.py
+-rw-r--r--   0        0        0      378 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/date_time/same_or_before.py
+-rw-r--r--   0        0        0     1181 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/date_time/subtract.py
+-rw-r--r--   0        0        0     3800 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/interval/collapse.py
+-rw-r--r--   0        0        0      381 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/interval/end.py
+-rw-r--r--   0        0        0     1411 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/interval/in_interval.py
+-rw-r--r--   0        0        0     1546 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/interval/included_in.py
+-rw-r--r--   0        0        0      587 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/interval/overlaps.py
+-rw-r--r--   0        0        0      976 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/interval/start.py
+-rw-r--r--   0        0        0      348 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/list/distinct.py
+-rw-r--r--   0        0        0      230 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/list/exists.py
+-rw-r--r--   0        0        0      324 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/list/first.py
+-rw-r--r--   0        0        0      291 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/list/flatten.py
+-rw-r--r--   0        0        0     2195 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/list/intersect.py
+-rw-r--r--   0        0        0      306 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/list/last.py
+-rw-r--r--   0        0        0      404 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/list/singleton_from.py
+-rw-r--r--   0        0        0      236 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/list/union.py
+-rw-r--r--   0        0        0      409 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/nullological/coalesce.py
+-rw-r--r--   0        0        0      212 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/nullological/is_false.py
+-rw-r--r--   0        0        0      358 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/nullological/is_null.py
+-rw-r--r--   0        0        0      193 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/nullological/is_true.py
+-rw-r--r--   0        0        0      254 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/sort/sort_by_column.py
+-rw-r--r--   0        0        0      134 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/sort/sort_by_direction.py
+-rw-r--r--   0        0        0      173 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/sort/sort_by_expression.py
+-rw-r--r--   0        0        0       51 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/sort/tuple_sort.py
+-rw-r--r--   0        0        0      166 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/string/ends_with.py
+-rw-r--r--   0        0        0      170 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/string/split.py
+-rw-r--r--   0        0        0      149 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/to_list.py
+-rw-r--r--   0        0        0      162 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/type/to_concept.py
+-rw-r--r--   0        0        0      280 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/operators/type/to_datetime.py
+-rw-r--r--   0        0        0      509 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/parameter.py
+-rw-r--r--   0        0        0     9733 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/scripts/fhir_map_generator.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/__init__.py
+-rw-r--r--   0        0        0     2901 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/any.py
+-rw-r--r--   0        0        0      988 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/boolean.py
+-rw-r--r--   0        0        0     1700 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/code.py
+-rw-r--r--   0        0        0      851 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/code_system.py
+-rw-r--r--   0        0        0     2459 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/concept.py
+-rw-r--r--   0        0        0     1001 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/date.py
+-rw-r--r--   0        0        0     2986 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/datetime.py
+-rw-r--r--   0        0        0     1128 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/decimal.py
+-rw-r--r--   0        0        0      756 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/integer.py
+-rw-r--r--   0        0        0     3674 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/interval.py
+-rw-r--r--   0        0        0     1605 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/list.py
+-rw-r--r--   0        0        0       81 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/long.py
+-rw-r--r--   0        0        0      416 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/null.py
+-rw-r--r--   0        0        0      887 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/quantity.py
+-rw-r--r--   0        0        0     1053 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/string.py
+-rw-r--r--   0        0        0     2003 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/types/value_set.py
+-rw-r--r--   0        0        0      170 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/_internal/valueset_provider.py
+-rw-r--r--   0        0        0      451 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/context.py
+-rw-r--r--   0        0        0     4227 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/operators.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/providers/__init__.py
+-rw-r--r--   0        0        0      216 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/providers/logger.py
+-rw-r--r--   0        0        0       15 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/providers/requirements.txt
+-rw-r--r--   0        0        0     4871 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/providers/rosetta_valueset_provider.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/py.typed
+-rw-r--r--   0        0        0     1089 2023-05-24 13:07:49.984196 cqlpy-0.2.5/cqlpy/types.py
+-rw-r--r--   0        0        0      670 2023-05-24 13:08:09.424436 cqlpy-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 cqlpy-0.2.5/PKG-INFO
```

### Comparing `cqlpy-0.2.4/LICENSE` & `cqlpy-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/context/context.py` & `cqlpy-0.2.5/cqlpy/_internal/context/context.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/context/cql_value_set_provider.py` & `cqlpy-0.2.5/cqlpy/_internal/context/cql_value_set_provider.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/context/fhir/r4/map.py` & `cqlpy-0.2.5/cqlpy/_internal/context/fhir/r4/map.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
+        "status": "String",
         "type": "Concept",
         "name": "String",
         "subject": "List<BackboneElement:Reference>",
         "servicePeriod": "Interval<DateTime>",
         "coverage": "List<BackboneElement:Account_Coverage>",
         "owner": "BackboneElement:Reference",
         "description": "String",
@@ -30,14 +31,15 @@
         "modifierExtension": "List<BackboneElement:Extension>",
         "url": "String",
         "identifier": "List<BackboneElement:Identifier>",
         "version": "String",
         "name": "String",
         "title": "String",
         "subtitle": "String",
+        "status": "String",
         "experimental": "Boolean",
         "subject": "Choice:String",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "useContext": "List<BackboneElement:UsageContext>",
@@ -80,14 +82,15 @@
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "BackboneElement:Identifier",
+        "actuality": "String",
         "category": "List<Concept>",
         "event": "Concept",
         "subject": "BackboneElement:Reference",
         "encounter": "BackboneElement:Reference",
         "date": "DateTime",
         "detected": "DateTime",
         "recordedDate": "DateTime",
@@ -111,15 +114,17 @@
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
         "clinicalStatus": "Concept",
         "verificationStatus": "Concept",
+        "type": "String",
         "category": "List<String>",
+        "criticality": "String",
         "code": "Concept",
         "patient": "BackboneElement:Reference",
         "encounter": "BackboneElement:Reference",
         "onset": "Choice:Interval<DateTime>",
         "recordedDate": "DateTime",
         "recorder": "BackboneElement:Reference",
         "asserter": "BackboneElement:Reference",
@@ -133,14 +138,15 @@
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
+        "status": "String",
         "cancelationReason": "Concept",
         "serviceCategory": "List<Concept>",
         "serviceType": "List<Concept>",
         "specialty": "List<Concept>",
         "appointmentType": "Concept",
         "reasonCode": "List<Concept>",
         "reasonReference": "List<BackboneElement:Reference>",
@@ -183,16 +189,18 @@
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "type": "Code",
         "subtype": "List<Code>",
+        "action": "String",
         "period": "Interval<DateTime>",
         "recorded": "String",
+        "outcome": "String",
         "outcomeDesc": "String",
         "purposeOfEvent": "List<Concept>",
         "agent": "List<BackboneElement:AuditEvent_Agent>",
         "source": "BackboneElement:AuditEvent_Source",
         "entity": "List<BackboneElement:AuditEvent_Entity>",
     },
     "Basic": {
@@ -225,15 +233,17 @@
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
+        "productCategory": "String",
         "productCode": "Concept",
+        "status": "String",
         "request": "List<BackboneElement:Reference>",
         "quantity": "Integer",
         "parent": "List<BackboneElement:Reference>",
         "collection": "BackboneElement:BiologicallyDerivedProduct_Collection",
         "processing": "List<BackboneElement:BiologicallyDerivedProduct_Processing>",
         "manipulation": "BackboneElement:BiologicallyDerivedProduct_Manipulation",
         "storage": "List<BackboneElement:BiologicallyDerivedProduct_Storage>",
@@ -258,14 +268,15 @@
     },
     "Bundle": {
         "id": "String",
         "meta": "BackboneElement:Meta",
         "implicitRules": "String",
         "language": "Code",
         "identifier": "BackboneElement:Identifier",
+        "type": "String",
         "timestamp": "String",
         "total": "String",
         "link": "List<BackboneElement:Bundle_Link>",
         "entry": "List<BackboneElement:Bundle_Entry>",
         "signature": "BackboneElement:Signature",
     },
     "CapabilityStatement": {
@@ -277,27 +288,30 @@
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "url": "String",
         "version": "String",
         "name": "String",
         "title": "String",
+        "status": "String",
         "experimental": "Boolean",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "useContext": "List<BackboneElement:UsageContext>",
         "jurisdiction": "List<Concept>",
         "purpose": "String",
         "copyright": "String",
+        "kind": "String",
         "instantiates": "List<String>",
         "imports": "List<String>",
         "software": "BackboneElement:CapabilityStatement_Software",
         "implementation": "BackboneElement:CapabilityStatement_Implementation",
+        "fhirVersion": "String",
         "format": "List<Code>",
         "patchFormat": "List<Code>",
         "implementationGuide": "List<String>",
         "rest": "List<BackboneElement:CapabilityStatement_Rest>",
         "messaging": "List<BackboneElement:CapabilityStatement_Messaging>",
         "document": "List<BackboneElement:CapabilityStatement_Document>",
     },
@@ -340,14 +354,15 @@
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
+        "status": "String",
         "category": "List<Concept>",
         "name": "String",
         "subject": "BackboneElement:Reference",
         "encounter": "BackboneElement:Reference",
         "period": "Interval<DateTime>",
         "participant": "List<BackboneElement:CareTeam_Participant>",
         "reasonCode": "List<Concept>",
@@ -367,14 +382,15 @@
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
         "type": "Concept",
         "orderable": "Boolean",
         "referencedItem": "BackboneElement:Reference",
         "additionalIdentifier": "List<BackboneElement:Identifier>",
         "classification": "List<Concept>",
+        "status": "String",
         "validityPeriod": "Interval<DateTime>",
         "validTo": "DateTime",
         "lastUpdated": "DateTime",
         "additionalCharacteristic": "List<Concept>",
         "additionalClassification": "List<Concept>",
         "relatedEntry": "List<BackboneElement:CatalogEntry_RelatedEntry>",
     },
@@ -386,14 +402,15 @@
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
         "definitionUri": "List<String>",
         "definitionCanonical": "List<String>",
+        "status": "String",
         "partOf": "List<BackboneElement:Reference>",
         "code": "Concept",
         "subject": "BackboneElement:Reference",
         "context": "BackboneElement:Reference",
         "occurrence": "Choice:Interval<DateTime>",
         "performer": "List<BackboneElement:ChargeItem_Performer>",
         "performingOrganization": "BackboneElement:Reference",
@@ -425,14 +442,15 @@
         "url": "String",
         "identifier": "List<BackboneElement:Identifier>",
         "version": "String",
         "title": "String",
         "derivedFromUri": "List<String>",
         "partOf": "List<String>",
         "replaces": "List<String>",
+        "status": "String",
         "experimental": "Boolean",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "useContext": "List<BackboneElement:UsageContext>",
         "jurisdiction": "List<Concept>",
@@ -454,14 +472,15 @@
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
         "status": "Code",
         "type": "Concept",
         "subType": "Concept",
+        "use": "String",
         "patient": "BackboneElement:Reference",
         "billablePeriod": "Interval<DateTime>",
         "created": "DateTime",
         "enterer": "BackboneElement:Reference",
         "insurer": "BackboneElement:Reference",
         "provider": "BackboneElement:Reference",
         "priority": "Concept",
@@ -557,27 +576,30 @@
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "url": "String",
         "identifier": "List<BackboneElement:Identifier>",
         "version": "String",
         "name": "String",
         "title": "String",
+        "status": "String",
         "experimental": "Boolean",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "useContext": "List<BackboneElement:UsageContext>",
         "jurisdiction": "List<Concept>",
         "purpose": "String",
         "copyright": "String",
         "caseSensitive": "Boolean",
         "valueSet": "String",
+        "hierarchyMeaning": "String",
         "compositional": "Boolean",
         "versionNeeded": "Boolean",
+        "content": "String",
         "supplements": "String",
         "count": "String",
         "filter": "List<BackboneElement:CodeSystem_Filter>",
         "property": "List<BackboneElement:CodeSystem_Property>",
         "concept": "List<BackboneElement:CodeSystem_Concept>",
     },
     "Communication": {
@@ -653,34 +675,37 @@
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "url": "String",
         "version": "String",
         "name": "String",
+        "status": "String",
         "experimental": "Boolean",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "useContext": "List<BackboneElement:UsageContext>",
         "purpose": "String",
+        "code": "String",
         "search": "Boolean",
         "resource": "List<BackboneElement:CompartmentDefinition_Resource>",
     },
     "Composition": {
         "id": "String",
         "meta": "BackboneElement:Meta",
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "BackboneElement:Identifier",
+        "status": "String",
         "type": "Concept",
         "category": "List<Concept>",
         "subject": "BackboneElement:Reference",
         "encounter": "BackboneElement:Reference",
         "date": "DateTime",
         "author": "List<BackboneElement:Reference>",
         "title": "String",
@@ -701,14 +726,15 @@
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "url": "String",
         "identifier": "BackboneElement:Identifier",
         "version": "String",
         "name": "String",
         "title": "String",
+        "status": "String",
         "experimental": "Boolean",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "useContext": "List<BackboneElement:UsageContext>",
         "jurisdiction": "List<Concept>",
@@ -751,14 +777,15 @@
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
+        "status": "String",
         "scope": "Concept",
         "category": "List<Concept>",
         "patient": "BackboneElement:Reference",
         "dateTime": "DateTime",
         "performer": "List<BackboneElement:Reference>",
         "organization": "List<BackboneElement:Reference>",
         "source": "Choice:String",
@@ -874,14 +901,15 @@
         "status": "Code",
         "purpose": "List<String>",
         "patient": "BackboneElement:Reference",
         "serviced": "Choice:Interval<DateTime>",
         "created": "DateTime",
         "requestor": "BackboneElement:Reference",
         "request": "BackboneElement:Reference",
+        "outcome": "String",
         "disposition": "String",
         "insurer": "BackboneElement:Reference",
         "insurance": "List<BackboneElement:CoverageEligibilityResponse_Insurance>",
         "preAuthRef": "String",
         "form": "Concept",
         "error": "List<BackboneElement:CoverageEligibilityResponse_Error>",
     },
@@ -893,14 +921,15 @@
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
         "status": "Code",
         "code": "Concept",
+        "severity": "String",
         "patient": "BackboneElement:Reference",
         "identified": "Choice:Interval<DateTime>",
         "author": "BackboneElement:Reference",
         "implicated": "List<BackboneElement:Reference>",
         "evidence": "List<BackboneElement:DetectedIssue_Evidence>",
         "detail": "String",
         "reference": "String",
@@ -914,14 +943,15 @@
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
         "definition": "BackboneElement:Reference",
         "udiCarrier": "List<BackboneElement:Device_UdiCarrier>",
+        "status": "String",
         "statusReason": "List<Concept>",
         "distinctIdentifier": "String",
         "manufacturer": "String",
         "manufactureDate": "DateTime",
         "expirationDate": "DateTime",
         "lotNumber": "String",
         "serialNumber": "String",
@@ -983,14 +1013,17 @@
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
         "type": "Concept",
         "unit": "Concept",
         "source": "BackboneElement:Reference",
         "parent": "BackboneElement:Reference",
+        "operationalStatus": "String",
+        "color": "String",
+        "category": "String",
         "measurementPeriod": "BackboneElement:Timing",
         "calibration": "List<BackboneElement:DeviceMetric_Calibration>",
     },
     "DeviceRequest": {
         "id": "String",
         "meta": "BackboneElement:Meta",
         "implicitRules": "String",
@@ -1030,14 +1063,15 @@
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
         "basedOn": "List<BackboneElement:Reference>",
+        "status": "String",
         "subject": "BackboneElement:Reference",
         "derivedFrom": "List<BackboneElement:Reference>",
         "timing": "Choice:Interval<DateTime>",
         "recordedOn": "DateTime",
         "source": "BackboneElement:Reference",
         "device": "BackboneElement:Reference",
         "reasonCode": "List<Concept>",
@@ -1052,14 +1086,15 @@
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
         "basedOn": "List<BackboneElement:Reference>",
+        "status": "String",
         "category": "List<Concept>",
         "code": "Concept",
         "subject": "BackboneElement:Reference",
         "encounter": "BackboneElement:Reference",
         "effective": "Choice:Interval<DateTime>",
         "issued": "String",
         "performer": "List<BackboneElement:Reference>",
@@ -1079,14 +1114,15 @@
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "masterIdentifier": "BackboneElement:Identifier",
         "identifier": "List<BackboneElement:Identifier>",
+        "status": "String",
         "type": "Concept",
         "subject": "BackboneElement:Reference",
         "created": "DateTime",
         "author": "List<BackboneElement:Reference>",
         "recipient": "List<BackboneElement:Reference>",
         "source": "String",
         "description": "String",
@@ -1100,14 +1136,15 @@
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "masterIdentifier": "BackboneElement:Identifier",
         "identifier": "List<BackboneElement:Identifier>",
+        "status": "String",
         "docStatus": "Code",
         "type": "Concept",
         "category": "List<Concept>",
         "subject": "BackboneElement:Reference",
         "date": "String",
         "author": "List<BackboneElement:Reference>",
         "authenticator": "BackboneElement:Reference",
@@ -1128,14 +1165,15 @@
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "url": "String",
         "identifier": "List<BackboneElement:Identifier>",
         "version": "String",
         "name": "String",
         "title": "String",
+        "status": "String",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "note": "List<BackboneElement:Annotation>",
         "useContext": "List<BackboneElement:UsageContext>",
         "jurisdiction": "List<Concept>",
@@ -1166,14 +1204,15 @@
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
+        "status": "String",
         "statusHistory": "List<BackboneElement:Encounter_StatusHistory>",
         "class": "Code",
         "classHistory": "List<BackboneElement:Encounter_ClassHistory>",
         "type": "List<Concept>",
         "serviceType": "Concept",
         "priority": "Concept",
         "subject": "BackboneElement:Reference",
@@ -1197,14 +1236,15 @@
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
+        "status": "String",
         "connectionType": "Code",
         "name": "String",
         "managingOrganization": "BackboneElement:Reference",
         "contact": "List<BackboneElement:ContactPoint>",
         "period": "Interval<DateTime>",
         "payloadType": "List<Concept>",
         "payloadMimeType": "List<Code>",
@@ -1236,14 +1276,15 @@
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
         "status": "Code",
         "request": "BackboneElement:Reference",
+        "outcome": "String",
         "disposition": "String",
         "created": "DateTime",
         "organization": "BackboneElement:Reference",
         "requestProvider": "BackboneElement:Reference",
     },
     "EpisodeOfCare": {
         "id": "String",
@@ -1251,14 +1292,15 @@
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
+        "status": "String",
         "statusHistory": "List<BackboneElement:EpisodeOfCare_StatusHistory>",
         "type": "List<Concept>",
         "diagnosis": "List<BackboneElement:EpisodeOfCare_Diagnosis>",
         "patient": "BackboneElement:Reference",
         "managingOrganization": "BackboneElement:Reference",
         "period": "Interval<DateTime>",
         "referralRequest": "List<BackboneElement:Reference>",
@@ -1277,14 +1319,15 @@
         "modifierExtension": "List<BackboneElement:Extension>",
         "url": "String",
         "identifier": "List<BackboneElement:Identifier>",
         "version": "String",
         "name": "String",
         "title": "String",
         "subtitle": "String",
+        "status": "String",
         "experimental": "Boolean",
         "subject": "Choice:String",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "useContext": "List<BackboneElement:UsageContext>",
@@ -1315,14 +1358,15 @@
         "url": "String",
         "identifier": "List<BackboneElement:Identifier>",
         "version": "String",
         "name": "String",
         "title": "String",
         "shortTitle": "String",
         "subtitle": "String",
+        "status": "String",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "note": "List<BackboneElement:Annotation>",
         "useContext": "List<BackboneElement:UsageContext>",
         "jurisdiction": "List<Concept>",
@@ -1352,14 +1396,15 @@
         "url": "String",
         "identifier": "List<BackboneElement:Identifier>",
         "version": "String",
         "name": "String",
         "title": "String",
         "shortTitle": "String",
         "subtitle": "String",
+        "status": "String",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "note": "List<BackboneElement:Annotation>",
         "useContext": "List<BackboneElement:UsageContext>",
         "jurisdiction": "List<Concept>",
@@ -1369,14 +1414,15 @@
         "effectivePeriod": "Interval<DateTime>",
         "topic": "List<Concept>",
         "author": "List<BackboneElement:ContactDetail>",
         "editor": "List<BackboneElement:ContactDetail>",
         "reviewer": "List<BackboneElement:ContactDetail>",
         "endorser": "List<BackboneElement:ContactDetail>",
         "relatedArtifact": "List<BackboneElement:RelatedArtifact>",
+        "type": "String",
         "characteristic": "List<BackboneElement:EvidenceVariable_Characteristic>",
     },
     "ExampleScenario": {
         "id": "String",
         "meta": "BackboneElement:Meta",
         "implicitRules": "String",
         "language": "Code",
@@ -1384,14 +1430,15 @@
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "url": "String",
         "identifier": "List<BackboneElement:Identifier>",
         "version": "String",
         "name": "String",
+        "status": "String",
         "experimental": "Boolean",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "useContext": "List<BackboneElement:UsageContext>",
         "jurisdiction": "List<Concept>",
         "copyright": "String",
@@ -1407,14 +1454,15 @@
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
+        "status": "String",
         "type": "Concept",
         "subType": "Concept",
         "use": "Code",
         "patient": "BackboneElement:Reference",
         "billablePeriod": "Interval<DateTime>",
         "created": "DateTime",
         "enterer": "BackboneElement:Reference",
@@ -1461,14 +1509,15 @@
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
         "instantiatesCanonical": "List<String>",
         "instantiatesUri": "List<String>",
+        "status": "String",
         "dataAbsentReason": "Concept",
         "patient": "BackboneElement:Reference",
         "date": "DateTime",
         "name": "String",
         "relationship": "Concept",
         "sex": "Concept",
         "born": "Choice:Interval<DateTime>",
@@ -1486,14 +1535,15 @@
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
+        "status": "String",
         "category": "List<Concept>",
         "code": "Concept",
         "subject": "BackboneElement:Reference",
         "period": "Interval<DateTime>",
         "encounter": "BackboneElement:Reference",
         "author": "BackboneElement:Reference",
     },
@@ -1503,14 +1553,15 @@
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
+        "lifecycleStatus": "String",
         "achievementStatus": "Concept",
         "category": "List<Concept>",
         "priority": "Concept",
         "description": "Concept",
         "subject": "BackboneElement:Reference",
         "start": "Choice:String",
         "target": "List<BackboneElement:Goal_Target>",
@@ -1530,14 +1581,15 @@
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "url": "String",
         "version": "String",
         "name": "String",
+        "status": "String",
         "experimental": "Boolean",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "useContext": "List<BackboneElement:UsageContext>",
         "jurisdiction": "List<Concept>",
@@ -1553,14 +1605,15 @@
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
         "active": "Boolean",
+        "type": "String",
         "actual": "Boolean",
         "code": "Concept",
         "name": "String",
         "quantity": "String",
         "managingEntity": "BackboneElement:Reference",
         "characteristic": "List<BackboneElement:Group_Characteristic>",
         "member": "List<BackboneElement:Group_Member>",
@@ -1573,14 +1626,15 @@
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "requestIdentifier": "BackboneElement:Identifier",
         "identifier": "List<BackboneElement:Identifier>",
         "module": "Choice:String",
+        "status": "String",
         "subject": "BackboneElement:Reference",
         "encounter": "BackboneElement:Reference",
         "occurrenceDateTime": "DateTime",
         "performer": "BackboneElement:Reference",
         "reasonCode": "List<Concept>",
         "reasonReference": "List<BackboneElement:Reference>",
         "note": "List<BackboneElement:Annotation>",
@@ -1629,14 +1683,15 @@
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
+        "status": "String",
         "modality": "List<Code>",
         "subject": "BackboneElement:Reference",
         "encounter": "BackboneElement:Reference",
         "started": "DateTime",
         "basedOn": "List<BackboneElement:Reference>",
         "referrer": "BackboneElement:Reference",
         "interpreter": "List<BackboneElement:Reference>",
@@ -1737,23 +1792,25 @@
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "url": "String",
         "version": "String",
         "name": "String",
         "title": "String",
+        "status": "String",
         "experimental": "Boolean",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "useContext": "List<BackboneElement:UsageContext>",
         "jurisdiction": "List<Concept>",
         "copyright": "String",
         "packageId": "String",
+        "license": "String",
         "fhirVersion": "List<String>",
         "dependsOn": "List<BackboneElement:ImplementationGuide_DependsOn>",
         "global": "List<BackboneElement:ImplementationGuide_Global>",
         "definition": "BackboneElement:ImplementationGuide_Definition",
         "manifest": "BackboneElement:ImplementationGuide_Manifest",
     },
     "InsurancePlan": {
@@ -1762,14 +1819,15 @@
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
+        "status": "String",
         "type": "List<Concept>",
         "name": "String",
         "alias": "List<String>",
         "period": "Interval<DateTime>",
         "ownedBy": "BackboneElement:Reference",
         "administeredBy": "BackboneElement:Reference",
         "coverageArea": "List<BackboneElement:Reference>",
@@ -1785,14 +1843,15 @@
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
+        "status": "String",
         "cancelledReason": "String",
         "type": "Concept",
         "subject": "BackboneElement:Reference",
         "recipient": "BackboneElement:Reference",
         "date": "DateTime",
         "participant": "List<BackboneElement:Invoice_Participant>",
         "issuer": "BackboneElement:Reference",
@@ -1815,14 +1874,15 @@
         "modifierExtension": "List<BackboneElement:Extension>",
         "url": "String",
         "identifier": "List<BackboneElement:Identifier>",
         "version": "String",
         "name": "String",
         "title": "String",
         "subtitle": "String",
+        "status": "String",
         "experimental": "Boolean",
         "type": "Concept",
         "subject": "Choice:String",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
@@ -1863,14 +1923,16 @@
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
+        "status": "String",
+        "mode": "String",
         "title": "String",
         "code": "Concept",
         "subject": "BackboneElement:Reference",
         "encounter": "BackboneElement:Reference",
         "date": "DateTime",
         "source": "BackboneElement:Reference",
         "orderedBy": "Concept",
@@ -1884,18 +1946,20 @@
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
+        "status": "String",
         "operationalStatus": "Code",
         "name": "String",
         "alias": "List<String>",
         "description": "String",
+        "mode": "String",
         "type": "List<Concept>",
         "telecom": "List<BackboneElement:ContactPoint>",
         "address": "BackboneElement:Address",
         "physicalType": "Concept",
         "position": "BackboneElement:Location_Position",
         "managingOrganization": "BackboneElement:Reference",
         "partOf": "BackboneElement:Reference",
@@ -1914,14 +1978,15 @@
         "modifierExtension": "List<BackboneElement:Extension>",
         "url": "String",
         "identifier": "List<BackboneElement:Identifier>",
         "version": "String",
         "name": "String",
         "title": "String",
         "subtitle": "String",
+        "status": "String",
         "experimental": "Boolean",
         "subject": "Choice:String",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "useContext": "List<BackboneElement:UsageContext>",
@@ -1959,14 +2024,16 @@
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
+        "status": "String",
+        "type": "String",
         "measure": "String",
         "subject": "BackboneElement:Reference",
         "date": "DateTime",
         "reporter": "BackboneElement:Reference",
         "period": "Interval<DateTime>",
         "improvementNotation": "Concept",
         "group": "List<BackboneElement:MeasureReport_Group>",
@@ -2389,27 +2456,30 @@
         "modifierExtension": "List<BackboneElement:Extension>",
         "url": "String",
         "identifier": "List<BackboneElement:Identifier>",
         "version": "String",
         "name": "String",
         "title": "String",
         "replaces": "List<String>",
+        "status": "String",
         "experimental": "Boolean",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "useContext": "List<BackboneElement:UsageContext>",
         "jurisdiction": "List<Concept>",
         "purpose": "String",
         "copyright": "String",
         "base": "String",
         "parent": "List<String>",
         "event": "Choice:String",
+        "category": "String",
         "focus": "List<BackboneElement:MessageDefinition_Focus>",
+        "responseRequired": "String",
         "allowedResponse": "List<BackboneElement:MessageDefinition_AllowedResponse>",
         "graph": "List<String>",
     },
     "MessageHeader": {
         "id": "String",
         "meta": "BackboneElement:Meta",
         "implicitRules": "String",
@@ -2436,14 +2506,15 @@
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
+        "type": "String",
         "coordinateSystem": "Integer",
         "patient": "BackboneElement:Reference",
         "specimen": "BackboneElement:Reference",
         "device": "BackboneElement:Reference",
         "performer": "BackboneElement:Reference",
         "quantity": "Decimal",
         "referenceSeq": "BackboneElement:MolecularSequence_ReferenceSeq",
@@ -2461,14 +2532,16 @@
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "name": "String",
+        "status": "String",
+        "kind": "String",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "responsible": "String",
         "type": "Concept",
         "description": "String",
         "useContext": "List<BackboneElement:UsageContext>",
@@ -2511,14 +2584,15 @@
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
         "basedOn": "List<BackboneElement:Reference>",
         "partOf": "List<BackboneElement:Reference>",
+        "status": "String",
         "category": "List<Concept>",
         "code": "Concept",
         "subject": "BackboneElement:Reference",
         "focus": "List<BackboneElement:Reference>",
         "encounter": "BackboneElement:Reference",
         "effective": "Choice:Interval<DateTime>",
         "issued": "String",
@@ -2568,14 +2642,16 @@
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "url": "String",
         "version": "String",
         "name": "String",
         "title": "String",
+        "status": "String",
+        "kind": "String",
         "experimental": "Boolean",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "useContext": "List<BackboneElement:UsageContext>",
         "jurisdiction": "List<Concept>",
@@ -2662,14 +2738,15 @@
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
         "active": "Boolean",
         "name": "List<BackboneElement:HumanName>",
         "telecom": "List<BackboneElement:ContactPoint>",
+        "gender": "String",
         "birthDate": "Date",
         "deceased": "Choice:String",
         "address": "List<BackboneElement:Address>",
         "maritalStatus": "Concept",
         "multipleBirth": "Choice:String",
         "photo": "List<BackboneElement:Attachment>",
         "contact": "List<BackboneElement:Patient_Contact>",
@@ -2712,14 +2789,15 @@
         "identifier": "List<BackboneElement:Identifier>",
         "status": "Code",
         "period": "Interval<DateTime>",
         "created": "DateTime",
         "paymentIssuer": "BackboneElement:Reference",
         "request": "BackboneElement:Reference",
         "requestor": "BackboneElement:Reference",
+        "outcome": "String",
         "disposition": "String",
         "paymentDate": "Date",
         "paymentAmount": "BackboneElement:Money",
         "paymentIdentifier": "BackboneElement:Identifier",
         "detail": "List<BackboneElement:PaymentReconciliation_Detail>",
         "formCode": "Concept",
         "processNote": "List<BackboneElement:PaymentReconciliation_ProcessNote>",
@@ -2732,14 +2810,15 @@
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
         "name": "List<BackboneElement:HumanName>",
         "telecom": "List<BackboneElement:ContactPoint>",
+        "gender": "String",
         "birthDate": "Date",
         "address": "List<BackboneElement:Address>",
         "photo": "BackboneElement:Attachment",
         "managingOrganization": "BackboneElement:Reference",
         "active": "Boolean",
         "link": "List<BackboneElement:Person_Link>",
     },
@@ -2755,14 +2834,15 @@
         "url": "String",
         "identifier": "List<BackboneElement:Identifier>",
         "version": "String",
         "name": "String",
         "title": "String",
         "subtitle": "String",
         "type": "Concept",
+        "status": "String",
         "experimental": "Boolean",
         "subject": "Choice:String",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "useContext": "List<BackboneElement:UsageContext>",
@@ -2793,14 +2873,15 @@
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
         "active": "Boolean",
         "name": "List<BackboneElement:HumanName>",
         "telecom": "List<BackboneElement:ContactPoint>",
         "address": "List<BackboneElement:Address>",
+        "gender": "String",
         "birthDate": "Date",
         "photo": "List<BackboneElement:Attachment>",
         "qualification": "List<BackboneElement:Practitioner_Qualification>",
         "communication": "List<Concept>",
     },
     "PractitionerRole": {
         "id": "String",
@@ -2895,14 +2976,15 @@
         "modifierExtension": "List<BackboneElement:Extension>",
         "url": "String",
         "identifier": "List<BackboneElement:Identifier>",
         "version": "String",
         "name": "String",
         "title": "String",
         "derivedFrom": "List<String>",
+        "status": "String",
         "experimental": "Boolean",
         "subjectType": "List<Code>",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "useContext": "List<BackboneElement:UsageContext>",
@@ -2924,14 +3006,15 @@
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "BackboneElement:Identifier",
         "basedOn": "List<BackboneElement:Reference>",
         "partOf": "List<BackboneElement:Reference>",
         "questionnaire": "String",
+        "status": "String",
         "subject": "BackboneElement:Reference",
         "encounter": "BackboneElement:Reference",
         "authored": "DateTime",
         "author": "BackboneElement:Reference",
         "source": "BackboneElement:Reference",
         "item": "List<BackboneElement:QuestionnaireResponse_Item>",
     },
@@ -2946,14 +3029,15 @@
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
         "active": "Boolean",
         "patient": "BackboneElement:Reference",
         "relationship": "List<Concept>",
         "name": "List<BackboneElement:HumanName>",
         "telecom": "List<BackboneElement:ContactPoint>",
+        "gender": "String",
         "birthDate": "Date",
         "address": "List<BackboneElement:Address>",
         "photo": "List<BackboneElement:Attachment>",
         "period": "Interval<DateTime>",
         "communication": "List<BackboneElement:RelatedPerson_Communication>",
     },
     "RequestGroup": {
@@ -2996,14 +3080,15 @@
         "url": "String",
         "identifier": "List<BackboneElement:Identifier>",
         "version": "String",
         "name": "String",
         "title": "String",
         "shortTitle": "String",
         "subtitle": "String",
+        "status": "String",
         "experimental": "Boolean",
         "subject": "Choice:String",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "comment": "List<String>",
@@ -3039,14 +3124,15 @@
         "url": "String",
         "identifier": "List<BackboneElement:Identifier>",
         "version": "String",
         "name": "String",
         "title": "String",
         "shortTitle": "String",
         "subtitle": "String",
+        "status": "String",
         "experimental": "Boolean",
         "subject": "Choice:String",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "comment": "List<String>",
@@ -3061,14 +3147,16 @@
         "topic": "List<Concept>",
         "author": "List<BackboneElement:ContactDetail>",
         "editor": "List<BackboneElement:ContactDetail>",
         "reviewer": "List<BackboneElement:ContactDetail>",
         "endorser": "List<BackboneElement:ContactDetail>",
         "relatedArtifact": "List<BackboneElement:RelatedArtifact>",
         "library": "List<String>",
+        "type": "String",
+        "variableType": "String",
         "characteristic": "List<BackboneElement:ResearchElementDefinition_Characteristic>",
     },
     "ResearchStudy": {
         "id": "String",
         "meta": "BackboneElement:Meta",
         "implicitRules": "String",
         "language": "Code",
@@ -3076,14 +3164,15 @@
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
         "title": "String",
         "protocol": "List<BackboneElement:Reference>",
         "partOf": "List<BackboneElement:Reference>",
+        "status": "String",
         "primaryPurposeType": "Concept",
         "phase": "Concept",
         "category": "List<Concept>",
         "focus": "List<Concept>",
         "condition": "List<Concept>",
         "contact": "List<BackboneElement:ContactDetail>",
         "relatedArtifact": "List<BackboneElement:RelatedArtifact>",
@@ -3106,14 +3195,15 @@
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
+        "status": "String",
         "period": "Interval<DateTime>",
         "study": "BackboneElement:Reference",
         "individual": "BackboneElement:Reference",
         "assignedArm": "String",
         "actualArm": "String",
         "consent": "BackboneElement:Reference",
     },
@@ -3154,14 +3244,15 @@
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "url": "String",
         "identifier": "List<BackboneElement:Identifier>",
         "version": "String",
         "name": "String",
         "title": "String",
+        "status": "String",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "note": "List<BackboneElement:Annotation>",
         "useContext": "List<BackboneElement:UsageContext>",
         "jurisdiction": "List<Concept>",
@@ -3211,26 +3302,29 @@
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "url": "String",
         "version": "String",
         "name": "String",
         "derivedFrom": "String",
+        "status": "String",
         "experimental": "Boolean",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "useContext": "List<BackboneElement:UsageContext>",
         "jurisdiction": "List<Concept>",
         "purpose": "String",
         "code": "Code",
         "base": "List<Code>",
+        "type": "String",
         "expression": "String",
         "xpath": "String",
+        "xpathUsage": "String",
         "target": "List<Code>",
         "multipleOr": "Boolean",
         "multipleAnd": "Boolean",
         "comparator": "List<String>",
         "modifier": "List<String>",
         "chain": "List<String>",
         "component": "List<BackboneElement:SearchParameter_Component>",
@@ -3289,14 +3383,15 @@
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
         "serviceCategory": "List<Concept>",
         "serviceType": "List<Concept>",
         "specialty": "List<Concept>",
         "appointmentType": "Concept",
         "schedule": "BackboneElement:Reference",
+        "status": "String",
         "start": "String",
         "end": "String",
         "overbooked": "Boolean",
         "comment": "String",
     },
     "Specimen": {
         "id": "String",
@@ -3305,14 +3400,15 @@
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
         "accessionIdentifier": "BackboneElement:Identifier",
+        "status": "String",
         "type": "Concept",
         "subject": "BackboneElement:Reference",
         "receivedTime": "DateTime",
         "parent": "List<BackboneElement:Reference>",
         "request": "List<BackboneElement:Reference>",
         "collection": "BackboneElement:Specimen_Collection",
         "processing": "List<BackboneElement:Specimen_Processing>",
@@ -3346,30 +3442,34 @@
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "url": "String",
         "identifier": "List<BackboneElement:Identifier>",
         "version": "String",
         "name": "String",
         "title": "String",
+        "status": "String",
         "experimental": "Boolean",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "useContext": "List<BackboneElement:UsageContext>",
         "jurisdiction": "List<Concept>",
         "purpose": "String",
         "copyright": "String",
         "keyword": "List<Code>",
+        "fhirVersion": "String",
         "mapping": "List<BackboneElement:StructureDefinition_Mapping>",
+        "kind": "String",
         "abstract": "Boolean",
         "context": "List<BackboneElement:StructureDefinition_Context>",
         "contextInvariant": "List<String>",
         "type": "String",
         "baseDefinition": "String",
+        "derivation": "String",
         "snapshot": "BackboneElement:StructureDefinition_Snapshot",
         "differential": "BackboneElement:StructureDefinition_Differential",
     },
     "StructureMap": {
         "id": "String",
         "meta": "BackboneElement:Meta",
         "implicitRules": "String",
@@ -3379,14 +3479,15 @@
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "url": "String",
         "identifier": "List<BackboneElement:Identifier>",
         "version": "String",
         "name": "String",
         "title": "String",
+        "status": "String",
         "experimental": "Boolean",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "useContext": "List<BackboneElement:UsageContext>",
         "jurisdiction": "List<Concept>",
@@ -3401,14 +3502,15 @@
         "meta": "BackboneElement:Meta",
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "status": "String",
         "contact": "List<BackboneElement:ContactPoint>",
         "end": "String",
         "reason": "String",
         "criteria": "String",
         "error": "String",
         "channel": "BackboneElement:Subscription_Channel",
     },
@@ -3418,14 +3520,15 @@
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
+        "status": "String",
         "category": "List<Concept>",
         "code": "Concept",
         "description": "String",
         "instance": "List<BackboneElement:Substance_Instance>",
         "ingredient": "List<BackboneElement:Substance_Ingredient>",
     },
     "SubstanceNucleicAcid": {
@@ -3539,14 +3642,15 @@
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
         "basedOn": "List<BackboneElement:Reference>",
         "partOf": "List<BackboneElement:Reference>",
+        "status": "String",
         "patient": "BackboneElement:Reference",
         "type": "Concept",
         "suppliedItem": "BackboneElement:SupplyDelivery_SuppliedItem",
         "occurrence": "Choice:Interval<DateTime>",
         "supplier": "BackboneElement:Reference",
         "destination": "BackboneElement:Reference",
         "receiver": "List<BackboneElement:Reference>",
@@ -3557,14 +3661,15 @@
         "implicitRules": "String",
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
+        "status": "String",
         "category": "Concept",
         "priority": "Code",
         "item": "Choice:String",
         "quantity": "Decimal",
         "parameter": "List<BackboneElement:SupplyRequest_Parameter>",
         "occurrence": "Choice:Interval<DateTime>",
         "authoredOn": "DateTime",
@@ -3585,16 +3690,18 @@
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "List<BackboneElement:Identifier>",
         "instantiatesCanonical": "String",
         "instantiatesUri": "String",
         "basedOn": "List<BackboneElement:Reference>",
         "groupIdentifier": "BackboneElement:Identifier",
         "partOf": "List<BackboneElement:Reference>",
+        "status": "String",
         "statusReason": "Concept",
         "businessStatus": "Concept",
+        "intent": "String",
         "priority": "Code",
         "code": "Concept",
         "description": "String",
         "focus": "BackboneElement:Reference",
         "for": "BackboneElement:Reference",
         "encounter": "BackboneElement:Reference",
         "executionPeriod": "Interval<DateTime>",
@@ -3622,14 +3729,15 @@
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "url": "String",
         "version": "String",
         "name": "String",
         "title": "String",
+        "status": "String",
         "experimental": "Boolean",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "useContext": "List<BackboneElement:UsageContext>",
         "jurisdiction": "List<Concept>",
@@ -3637,14 +3745,15 @@
         "copyright": "String",
         "kind": "Code",
         "software": "BackboneElement:TerminologyCapabilities_Software",
         "implementation": "BackboneElement:TerminologyCapabilities_Implementation",
         "lockedDate": "Boolean",
         "codeSystem": "List<BackboneElement:TerminologyCapabilities_CodeSystem>",
         "expansion": "BackboneElement:TerminologyCapabilities_Expansion",
+        "codeSearch": "String",
         "validateCode": "BackboneElement:TerminologyCapabilities_ValidateCode",
         "translation": "BackboneElement:TerminologyCapabilities_Translation",
         "closure": "BackboneElement:TerminologyCapabilities_Closure",
     },
     "TestReport": {
         "id": "String",
         "meta": "BackboneElement:Meta",
@@ -3652,15 +3761,17 @@
         "language": "Code",
         "text": "BackboneElement:Narrative",
         "contained": "List<String>",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "BackboneElement:Identifier",
         "name": "String",
+        "status": "String",
         "testScript": "BackboneElement:Reference",
+        "result": "String",
         "score": "Decimal",
         "tester": "String",
         "issued": "DateTime",
         "participant": "List<BackboneElement:TestReport_Participant>",
         "setup": "BackboneElement:TestReport_Setup",
         "test": "List<BackboneElement:TestReport_Test>",
         "teardown": "BackboneElement:TestReport_Teardown",
@@ -3675,14 +3786,15 @@
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "url": "String",
         "identifier": "BackboneElement:Identifier",
         "version": "String",
         "name": "String",
         "title": "String",
+        "status": "String",
         "experimental": "Boolean",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "useContext": "List<BackboneElement:UsageContext>",
         "jurisdiction": "List<Concept>",
@@ -3708,14 +3820,15 @@
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "url": "String",
         "identifier": "List<BackboneElement:Identifier>",
         "version": "String",
         "name": "String",
         "title": "String",
+        "status": "String",
         "experimental": "Boolean",
         "date": "DateTime",
         "publisher": "String",
         "contact": "List<BackboneElement:ContactDetail>",
         "description": "String",
         "useContext": "List<BackboneElement:UsageContext>",
         "jurisdiction": "List<Concept>",
@@ -3795,14 +3908,16 @@
         "modifierExtension": "List<BackboneElement:Extension>",
         "type": "Code",
         "role": "Concept",
     },
     "Address": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
+        "use": "String",
+        "type": "String",
         "text": "String",
         "line": "List<String>",
         "city": "String",
         "district": "String",
         "state": "String",
         "postalCode": "String",
         "country": "String",
@@ -3824,26 +3939,28 @@
         "instance": "BackboneElement:Reference",
         "causality": "List<BackboneElement:AdverseEvent_Causality>",
     },
     "Age": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "value": "Decimal",
+        "comparator": "String",
         "unit": "String",
         "system": "String",
         "code": "Code",
     },
     "AllergyIntolerance_Reaction": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "substance": "Concept",
         "manifestation": "List<Concept>",
         "description": "String",
         "onset": "DateTime",
+        "severity": "String",
         "exposureRoute": "Concept",
         "note": "List<BackboneElement:Annotation>",
     },
     "Annotation": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "author": "Choice:String",
@@ -3852,14 +3969,16 @@
     },
     "Appointment_Participant": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "type": "List<Concept>",
         "actor": "BackboneElement:Reference",
+        "required": "String",
+        "status": "String",
         "period": "Interval<DateTime>",
     },
     "Attachment": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "contentType": "Code",
         "language": "Code",
@@ -3908,14 +4027,15 @@
         "detail": "List<BackboneElement:AuditEvent_Detail>",
     },
     "AuditEvent_Network": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "address": "String",
+        "type": "String",
     },
     "AuditEvent_Source": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "site": "String",
         "observer": "BackboneElement:Reference",
@@ -3947,14 +4067,15 @@
     },
     "BiologicallyDerivedProduct_Storage": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "description": "String",
         "temperature": "Decimal",
+        "scale": "String",
         "duration": "Interval<DateTime>",
     },
     "Bundle_Entry": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "link": "List<BackboneElement:Bundle_Link>",
@@ -3971,14 +4092,15 @@
         "relation": "String",
         "url": "String",
     },
     "Bundle_Request": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "method": "String",
         "url": "String",
         "ifNoneMatch": "String",
         "ifModifiedSince": "String",
         "ifMatch": "String",
         "ifNoneExist": "String",
     },
     "Bundle_Response": {
@@ -3991,20 +4113,22 @@
         "lastModified": "String",
         "outcome": "String",
     },
     "Bundle_Search": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "mode": "String",
         "score": "Decimal",
     },
     "CapabilityStatement_Document": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "mode": "String",
         "documentation": "String",
         "profile": "String",
     },
     "CapabilityStatement_Endpoint": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
@@ -4019,20 +4143,22 @@
         "url": "String",
         "custodian": "BackboneElement:Reference",
     },
     "CapabilityStatement_Interaction": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "code": "String",
         "documentation": "String",
     },
     "CapabilityStatement_Interaction1": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "code": "String",
         "documentation": "String",
     },
     "CapabilityStatement_Messaging": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "endpoint": "List<BackboneElement:CapabilityStatement_Endpoint>",
@@ -4053,42 +4179,47 @@
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "type": "Code",
         "profile": "String",
         "supportedProfile": "List<String>",
         "documentation": "String",
         "interaction": "List<BackboneElement:CapabilityStatement_Interaction>",
+        "versioning": "String",
         "readHistory": "Boolean",
         "updateCreate": "Boolean",
         "conditionalCreate": "Boolean",
+        "conditionalRead": "String",
         "conditionalUpdate": "Boolean",
+        "conditionalDelete": "String",
         "referencePolicy": "List<String>",
         "searchInclude": "List<String>",
         "searchRevInclude": "List<String>",
         "searchParam": "List<BackboneElement:CapabilityStatement_SearchParam>",
         "operation": "List<BackboneElement:CapabilityStatement_Operation>",
     },
     "CapabilityStatement_Rest": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "mode": "String",
         "documentation": "String",
         "security": "BackboneElement:CapabilityStatement_Security",
         "resource": "List<BackboneElement:CapabilityStatement_Resource>",
         "interaction": "List<BackboneElement:CapabilityStatement_Interaction1>",
         "searchParam": "List<BackboneElement:CapabilityStatement_SearchParam>",
         "operation": "List<BackboneElement:CapabilityStatement_Operation>",
         "compartment": "List<String>",
     },
     "CapabilityStatement_SearchParam": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "name": "String",
         "definition": "String",
+        "type": "String",
         "documentation": "String",
     },
     "CapabilityStatement_Security": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "cors": "Boolean",
@@ -4103,14 +4234,15 @@
         "version": "String",
         "releaseDate": "DateTime",
     },
     "CapabilityStatement_SupportedMessage": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "mode": "String",
         "definition": "String",
     },
     "CarePlan_Activity": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "outcomeCodeableConcept": "List<Concept>",
@@ -4126,14 +4258,15 @@
         "kind": "Code",
         "instantiatesCanonical": "List<String>",
         "instantiatesUri": "List<String>",
         "code": "Concept",
         "reasonCode": "List<Concept>",
         "reasonReference": "List<BackboneElement:Reference>",
         "goal": "List<BackboneElement:Reference>",
+        "status": "String",
         "statusReason": "Concept",
         "doNotPerform": "Boolean",
         "scheduled": "Choice:Interval<DateTime>",
         "location": "BackboneElement:Reference",
         "performer": "List<BackboneElement:Reference>",
         "product": "Choice:String",
         "dailyAmount": "Decimal",
@@ -4149,14 +4282,15 @@
         "onBehalfOf": "BackboneElement:Reference",
         "period": "Interval<DateTime>",
     },
     "CatalogEntry_RelatedEntry": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "relationtype": "String",
         "item": "BackboneElement:Reference",
     },
     "ChargeItemDefinition_Applicability": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "description": "String",
@@ -4281,14 +4415,15 @@
         "identifier": "BackboneElement:Identifier",
     },
     "ClaimResponse_ProcessNote": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "number": "String",
+        "type": "String",
         "text": "String",
         "language": "Concept",
     },
     "ClaimResponse_SubDetail": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
@@ -4497,14 +4632,15 @@
     "CodeSystem_Property": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "code": "Code",
         "uri": "String",
         "description": "String",
+        "type": "String",
     },
     "CodeSystem_Property1": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "code": "Code",
         "value": "Choice:String",
@@ -4544,14 +4680,15 @@
         "param": "List<String>",
         "documentation": "String",
     },
     "Composition_Attester": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "mode": "String",
         "time": "DateTime",
         "party": "BackboneElement:Reference",
     },
     "Composition_Event": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
@@ -4610,22 +4747,24 @@
     },
     "ConceptMap_Target": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "code": "Code",
         "display": "String",
+        "equivalence": "String",
         "comment": "String",
         "dependsOn": "List<BackboneElement:ConceptMap_DependsOn>",
         "product": "List<BackboneElement:ConceptMap_DependsOn>",
     },
     "ConceptMap_Unmapped": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "mode": "String",
         "code": "Code",
         "display": "String",
         "url": "String",
     },
     "Condition_Evidence": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
@@ -4648,27 +4787,29 @@
         "role": "Concept",
         "reference": "BackboneElement:Reference",
     },
     "Consent_Data": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "meaning": "String",
         "reference": "BackboneElement:Reference",
     },
     "Consent_Policy": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "authority": "String",
         "uri": "String",
     },
     "Consent_Provision": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "type": "String",
         "period": "Interval<DateTime>",
         "actor": "List<BackboneElement:Consent_Actor>",
         "action": "List<Concept>",
         "securityLabel": "List<Code>",
         "purpose": "List<Code>",
         "class": "List<Code>",
         "code": "List<Concept>",
@@ -4689,15 +4830,17 @@
         "extension": "List<BackboneElement:Extension>",
         "name": "String",
         "telecom": "List<BackboneElement:ContactPoint>",
     },
     "ContactPoint": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
+        "system": "String",
         "value": "String",
+        "use": "String",
         "rank": "String",
         "period": "Interval<DateTime>",
     },
     "Contract_Action": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
@@ -4866,21 +5009,23 @@
         "recipient": "BackboneElement:Reference",
         "linkId": "List<String>",
         "securityLabelNumber": "List<String>",
     },
     "Contributor": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
+        "type": "String",
         "name": "String",
         "contact": "List<BackboneElement:ContactDetail>",
     },
     "Count": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "value": "Decimal",
+        "comparator": "String",
         "unit": "String",
         "system": "String",
         "code": "Code",
     },
     "CoverageEligibilityRequest_Diagnosis": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
@@ -5013,14 +5158,15 @@
         "value": "Choice:Interval<DateTime>",
     },
     "DataRequirement_Sort": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "path": "String",
+        "direction": "String",
     },
     "DetectedIssue_Evidence": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "code": "List<Concept>",
         "detail": "List<BackboneElement:Reference>",
@@ -5041,14 +5187,15 @@
         "description": "List<Concept>",
     },
     "DeviceDefinition_DeviceName": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "name": "String",
+        "type": "String",
     },
     "DeviceDefinition_Material": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "substance": "Concept",
         "alternate": "Boolean",
@@ -5077,28 +5224,31 @@
         "issuer": "String",
         "jurisdiction": "String",
     },
     "DeviceMetric_Calibration": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "type": "String",
+        "state": "String",
         "time": "String",
     },
     "DeviceRequest_Parameter": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "code": "Concept",
         "value": "Choice:String",
     },
     "Device_DeviceName": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "name": "String",
+        "type": "String",
     },
     "Device_Property": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "type": "Concept",
         "valueQuantity": "List<Decimal>",
@@ -5116,14 +5266,15 @@
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "deviceIdentifier": "String",
         "issuer": "String",
         "jurisdiction": "String",
         "carrierAIDC": "String",
         "carrierHRF": "String",
+        "entryType": "String",
     },
     "Device_Version": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "type": "Concept",
         "component": "BackboneElement:Identifier",
@@ -5136,14 +5287,15 @@
         "comment": "String",
         "link": "BackboneElement:Reference",
     },
     "Distance": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "value": "Decimal",
+        "comparator": "String",
         "unit": "String",
         "system": "String",
         "code": "Code",
     },
     "DocumentManifest_Related": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
@@ -5170,14 +5322,15 @@
         "sourcePatientInfo": "BackboneElement:Reference",
         "related": "List<BackboneElement:Reference>",
     },
     "DocumentReference_RelatesTo": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "code": "String",
         "target": "BackboneElement:Reference",
     },
     "Dosage": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "sequence": "Integer",
@@ -5202,14 +5355,15 @@
         "dose": "Choice:String",
         "rate": "Choice:String",
     },
     "Duration": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "value": "Decimal",
+        "comparator": "String",
         "unit": "String",
         "system": "String",
         "code": "Code",
     },
     "EffectEvidenceSynthesis_Certainty": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
@@ -5247,14 +5401,15 @@
         "to": "Decimal",
     },
     "EffectEvidenceSynthesis_ResultsByExposure": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "description": "String",
+        "exposureState": "String",
         "variantState": "Concept",
         "riskEvidenceSynthesis": "BackboneElement:Reference",
     },
     "EffectEvidenceSynthesis_SampleSize": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
@@ -5310,32 +5465,35 @@
         "min": "String",
         "max": "String",
     },
     "ElementDefinition_Binding": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "strength": "String",
         "description": "String",
         "valueSet": "String",
     },
     "ElementDefinition_Constraint": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "key": "String",
         "requirements": "String",
+        "severity": "String",
         "human": "String",
         "expression": "String",
         "xpath": "String",
         "source": "String",
     },
     "ElementDefinition_Discriminator": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "type": "String",
         "path": "String",
     },
     "ElementDefinition_Example": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "label": "String",
@@ -5353,23 +5511,25 @@
     "ElementDefinition_Slicing": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "discriminator": "List<BackboneElement:ElementDefinition_Discriminator>",
         "description": "String",
         "ordered": "Boolean",
+        "rules": "String",
     },
     "ElementDefinition_Type": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "code": "String",
         "profile": "List<String>",
         "targetProfile": "List<String>",
         "aggregation": "List<String>",
+        "versioning": "String",
     },
     "Encounter_ClassHistory": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "class": "Code",
         "period": "Interval<DateTime>",
@@ -5397,14 +5557,15 @@
         "dischargeDisposition": "Concept",
     },
     "Encounter_Location": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "location": "BackboneElement:Reference",
+        "status": "String",
         "physicalType": "Concept",
         "period": "Interval<DateTime>",
     },
     "Encounter_Participant": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
@@ -5412,46 +5573,50 @@
         "period": "Interval<DateTime>",
         "individual": "BackboneElement:Reference",
     },
     "Encounter_StatusHistory": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "status": "String",
         "period": "Interval<DateTime>",
     },
     "EpisodeOfCare_Diagnosis": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "condition": "BackboneElement:Reference",
         "role": "Concept",
         "rank": "String",
     },
     "EpisodeOfCare_StatusHistory": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "status": "String",
         "period": "Interval<DateTime>",
     },
     "EvidenceVariable_Characteristic": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "description": "String",
         "definition": "Choice:String",
         "usageContext": "List<BackboneElement:UsageContext>",
         "exclude": "Boolean",
         "participantEffective": "Choice:Interval<DateTime>",
         "timeFromStart": "BackboneElement:Duration",
+        "groupMeasure": "String",
     },
     "ExampleScenario_Actor": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "actorId": "String",
+        "type": "String",
         "name": "String",
         "description": "String",
     },
     "ExampleScenario_Alternative": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
@@ -5697,14 +5862,15 @@
         "udi": "List<BackboneElement:Reference>",
     },
     "ExplanationOfBenefit_ProcessNote": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "number": "String",
+        "type": "String",
         "text": "String",
         "language": "Concept",
     },
     "ExplanationOfBenefit_Related": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
@@ -5762,14 +5928,15 @@
         "amount": "BackboneElement:Money",
     },
     "Expression": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "description": "String",
         "name": "String",
+        "language": "String",
         "expression": "String",
         "reference": "String",
     },
     "Extension": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "url": "String",
@@ -5793,15 +5960,17 @@
         "detail": "Choice:String",
         "dueD": "Choice:String",
     },
     "GraphDefinition_Compartment": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "use": "String",
         "code": "Code",
+        "rule": "String",
         "expression": "String",
         "description": "String",
     },
     "GraphDefinition_Link": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
@@ -5861,24 +6030,26 @@
         "modifierExtension": "List<BackboneElement:Extension>",
         "description": "String",
         "during": "Interval<DateTime>",
     },
     "HumanName": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
+        "use": "String",
         "text": "String",
         "family": "String",
         "given": "List<String>",
         "prefix": "List<String>",
         "suffix": "List<String>",
         "period": "Interval<DateTime>",
     },
     "Identifier": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
+        "use": "String",
         "type": "Concept",
         "system": "String",
         "value": "String",
         "period": "Interval<DateTime>",
         "assigner": "BackboneElement:Reference",
     },
     "ImagingStudy_Instance": {
@@ -6016,28 +6187,30 @@
     },
     "ImplementationGuide_Page": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "name": "Choice:String",
         "title": "String",
+        "generation": "String",
         "page": "List<BackboneElement:ImplementationGuide_Page>",
     },
     "ImplementationGuide_Page1": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "name": "String",
         "title": "String",
         "anchor": "List<String>",
     },
     "ImplementationGuide_Parameter": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "code": "String",
         "value": "String",
     },
     "ImplementationGuide_Resource": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "reference": "BackboneElement:Reference",
@@ -6153,22 +6326,24 @@
         "role": "Concept",
         "actor": "BackboneElement:Reference",
     },
     "Invoice_PriceComponent": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "type": "String",
         "code": "Concept",
         "factor": "Decimal",
         "amount": "BackboneElement:Money",
     },
     "Linkage_Item": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "type": "String",
         "resource": "BackboneElement:Reference",
     },
     "List_Entry": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "flag": "Concept",
@@ -6691,14 +6866,15 @@
         "receiver": "BackboneElement:Reference",
     },
     "MessageHeader_Response": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "String",
+        "code": "String",
         "details": "BackboneElement:Reference",
     },
     "MessageHeader_Source": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "name": "String",
@@ -6731,14 +6907,15 @@
         "start": "Integer",
         "end": "Integer",
     },
     "MolecularSequence_Quality": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "type": "String",
         "standardSequence": "Concept",
         "start": "Integer",
         "end": "Integer",
         "score": "Decimal",
         "method": "Concept",
         "truthTP": "Decimal",
         "queryTP": "Decimal",
@@ -6752,24 +6929,27 @@
     },
     "MolecularSequence_ReferenceSeq": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "chromosome": "Concept",
         "genomeBuild": "String",
+        "orientation": "String",
         "referenceSeqId": "Concept",
         "referenceSeqPointer": "BackboneElement:Reference",
         "referenceSeqString": "String",
+        "strand": "String",
         "windowStart": "Integer",
         "windowEnd": "Integer",
     },
     "MolecularSequence_Repository": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "type": "String",
         "": "Choice:String",
         "datasetId": "String",
         "variantsetId": "String",
         "readsetId": "String",
     },
     "MolecularSequence_Roc": {
         "id": "String",
@@ -6810,22 +6990,24 @@
         "value": "Decimal",
         "currency": "Code",
     },
     "NamingSystem_UniqueId": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "type": "String",
         "value": "String",
         "preferred": "Boolean",
         "comment": "String",
         "period": "Interval<DateTime>",
     },
     "Narrative": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
+        "status": "String",
         "div": "String",
     },
     "NutritionOrder_Administration": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "schedule": "BackboneElement:Timing",
@@ -6881,17 +7063,19 @@
         "modifier": "Concept",
         "foodType": "Concept",
     },
     "ObservationDefinition_QualifiedInterval": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "category": "String",
         "range": "Interval<Decimal>",
         "context": "Concept",
         "appliesTo": "List<Concept>",
+        "gender": "String",
         "age": "Interval<Decimal>",
         "gestationalAge": "Interval<Decimal>",
         "condition": "String",
     },
     "ObservationDefinition_QuantitativeDetails": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
@@ -6922,33 +7106,36 @@
         "age": "Interval<Decimal>",
         "text": "String",
     },
     "OperationDefinition_Binding": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "strength": "String",
         "valueSet": "String",
     },
     "OperationDefinition_Overload": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "parameterName": "List<String>",
         "comment": "String",
     },
     "OperationDefinition_Parameter": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "name": "Code",
+        "use": "String",
         "min": "Integer",
         "max": "String",
         "documentation": "String",
         "type": "Code",
         "targetProfile": "List<String>",
+        "searchType": "String",
         "binding": "BackboneElement:OperationDefinition_Binding",
         "referencedFrom": "List<BackboneElement:OperationDefinition_ReferencedFrom>",
         "part": "List<BackboneElement:OperationDefinition_Parameter>",
     },
     "OperationDefinition_ReferencedFrom": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
@@ -6956,14 +7143,16 @@
         "source": "String",
         "sourceId": "String",
     },
     "OperationOutcome_Issue": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "severity": "String",
+        "code": "String",
         "details": "Concept",
         "diagnostics": "String",
         "location": "List<String>",
         "expression": "List<String>",
     },
     "Organization_Contact": {
         "id": "String",
@@ -7005,22 +7194,24 @@
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "relationship": "List<Concept>",
         "name": "BackboneElement:HumanName",
         "telecom": "List<BackboneElement:ContactPoint>",
         "address": "BackboneElement:Address",
+        "gender": "String",
         "organization": "BackboneElement:Reference",
         "period": "Interval<DateTime>",
     },
     "Patient_Link": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "other": "BackboneElement:Reference",
+        "type": "String",
     },
     "PaymentReconciliation_Detail": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "identifier": "BackboneElement:Identifier",
         "predecessor": "BackboneElement:Identifier",
@@ -7033,27 +7224,29 @@
         "payee": "BackboneElement:Reference",
         "amount": "BackboneElement:Money",
     },
     "PaymentReconciliation_ProcessNote": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "type": "String",
         "text": "String",
     },
     "Period": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "start": "DateTime",
         "end": "DateTime",
     },
     "Person_Link": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "target": "BackboneElement:Reference",
+        "assurance": "String",
     },
     "PlanDefinition_Action": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "prefix": "String",
         "title": "String",
@@ -7069,23 +7262,29 @@
         "condition": "List<BackboneElement:PlanDefinition_Condition>",
         "input": "List<BackboneElement:DataRequirement>",
         "output": "List<BackboneElement:DataRequirement>",
         "relatedAction": "List<BackboneElement:PlanDefinition_RelatedAction>",
         "timing": "Choice:Interval<DateTime>",
         "participant": "List<BackboneElement:PlanDefinition_Participant>",
         "type": "Concept",
+        "groupingBehavior": "String",
+        "selectionBehavior": "String",
+        "requiredBehavior": "String",
+        "precheckBehavior": "String",
+        "cardinalityBehavior": "String",
         "definition": "Choice:String",
         "transform": "String",
         "dynamicValue": "List<BackboneElement:PlanDefinition_DynamicValue>",
         "action": "List<BackboneElement:PlanDefinition_Action>",
     },
     "PlanDefinition_Condition": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "kind": "String",
         "expression": "BackboneElement:Expression",
     },
     "PlanDefinition_DynamicValue": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "path": "String",
@@ -7103,21 +7302,23 @@
         "documentation": "List<BackboneElement:RelatedArtifact>",
         "target": "List<BackboneElement:PlanDefinition_Target>",
     },
     "PlanDefinition_Participant": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "type": "String",
         "role": "Concept",
     },
     "PlanDefinition_RelatedAction": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "actionId": "String",
+        "relationship": "String",
         "offset": "Choice:String",
     },
     "PlanDefinition_Target": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "measure": "Concept",
@@ -7207,21 +7408,23 @@
         "who": "BackboneElement:Reference",
         "onBehalfOf": "BackboneElement:Reference",
     },
     "Provenance_Entity": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "role": "String",
         "what": "BackboneElement:Reference",
         "agent": "List<BackboneElement:Provenance_Agent>",
     },
     "Quantity": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "value": "Decimal",
+        "comparator": "String",
         "unit": "String",
         "system": "String",
         "code": "Code",
     },
     "QuestionnaireResponse_Answer": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
@@ -7247,14 +7450,15 @@
         "initialSelected": "Boolean",
     },
     "Questionnaire_EnableWhen": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "question": "String",
+        "operator": "String",
         "answer": "Choice:String",
     },
     "Questionnaire_Initial": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "value": "Choice:String",
@@ -7264,15 +7468,17 @@
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "linkId": "String",
         "definition": "String",
         "code": "List<Code>",
         "prefix": "String",
         "text": "String",
+        "type": "String",
         "enableWhen": "List<BackboneElement:Questionnaire_EnableWhen>",
+        "enableBehavior": "String",
         "required": "Boolean",
         "repeats": "Boolean",
         "readOnly": "Boolean",
         "maxLength": "Integer",
         "answerValueSet": "String",
         "answerOption": "List<BackboneElement:Questionnaire_AnswerOption>",
         "initial": "List<BackboneElement:Questionnaire_Initial>",
@@ -7297,14 +7503,15 @@
         "type": "String",
         "identifier": "BackboneElement:Identifier",
         "display": "String",
     },
     "RelatedArtifact": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
+        "type": "String",
         "label": "String",
         "display": "String",
         "citation": "String",
         "url": "String",
         "document": "BackboneElement:Attachment",
         "resource": "String",
     },
@@ -7361,16 +7568,18 @@
         "definition": "Choice:String",
         "usageContext": "List<BackboneElement:UsageContext>",
         "exclude": "Boolean",
         "unitOfMeasure": "Concept",
         "studyEffectiveDescription": "String",
         "": "Choice:Interval<DateTime>",
         "studyEffectiveTimeFromStart": "BackboneElement:Duration",
+        "studyEffectiveGroupMeasure": "String",
         "participantEffectiveDescription": "String",
         "participantEffectiveTimeFromStart": "BackboneElement:Duration",
+        "participantEffectiveGroupMeasure": "String",
     },
     "ResearchStudy_Arm": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "name": "String",
         "type": "Concept",
@@ -7498,14 +7707,15 @@
     },
     "SpecimenDefinition_TypeTested": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "isDerived": "Boolean",
         "type": "Concept",
+        "preference": "String",
         "container": "BackboneElement:SpecimenDefinition_Container",
         "requirement": "String",
         "retentionTime": "BackboneElement:Duration",
         "rejectionCriterion": "List<Concept>",
         "handling": "List<BackboneElement:SpecimenDefinition_Handling>",
     },
     "Specimen_Collection": {
@@ -7540,14 +7750,15 @@
         "additive": "List<BackboneElement:Reference>",
         "time": "Choice:Interval<DateTime>",
     },
     "StructureDefinition_Context": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "type": "String",
         "expression": "String",
     },
     "StructureDefinition_Differential": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "element": "List<BackboneElement:ElementDefinition>",
@@ -7576,24 +7787,26 @@
     },
     "StructureMap_Group": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "name": "String",
         "extends": "String",
+        "typeMode": "String",
         "documentation": "String",
         "input": "List<BackboneElement:StructureMap_Input>",
         "rule": "List<BackboneElement:StructureMap_Rule>",
     },
     "StructureMap_Input": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "name": "String",
         "type": "String",
+        "mode": "String",
         "documentation": "String",
     },
     "StructureMap_Parameter": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "value": "Choice:String",
@@ -7615,42 +7828,47 @@
         "modifierExtension": "List<BackboneElement:Extension>",
         "context": "String",
         "min": "Integer",
         "max": "String",
         "type": "String",
         "defaultValue": "Choice:Interval<DateTime>",
         "element": "String",
+        "listMode": "String",
         "variable": "String",
         "condition": "String",
         "check": "String",
         "logMessage": "String",
     },
     "StructureMap_Structure": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "url": "String",
+        "mode": "String",
         "alias": "String",
         "documentation": "String",
     },
     "StructureMap_Target": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "context": "String",
+        "contextType": "String",
         "element": "String",
         "variable": "String",
         "listMode": "List<String>",
         "listRuleId": "String",
+        "transform": "String",
         "parameter": "List<BackboneElement:StructureMap_Parameter>",
     },
     "Subscription_Channel": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "type": "String",
         "endpoint": "String",
         "payload": "Code",
         "header": "List<String>",
     },
     "SubstanceAmount": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
@@ -8074,28 +8292,31 @@
         "modifierExtension": "List<BackboneElement:Extension>",
         "operation": "BackboneElement:TestReport_Operation",
     },
     "TestReport_Assert": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "result": "String",
         "message": "String",
         "detail": "String",
     },
     "TestReport_Operation": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "result": "String",
         "message": "String",
         "detail": "String",
     },
     "TestReport_Participant": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
+        "type": "String",
         "uri": "String",
         "display": "String",
     },
     "TestReport_Setup": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
@@ -8137,25 +8358,29 @@
     },
     "TestScript_Assert": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "label": "String",
         "description": "String",
+        "direction": "String",
         "compareToSourceId": "String",
         "compareToSourceExpression": "String",
         "compareToSourcePath": "String",
         "contentType": "Code",
         "expression": "String",
         "headerField": "String",
         "minimumId": "String",
         "navigationLinks": "Boolean",
+        "operator": "String",
         "path": "String",
+        "requestMethod": "String",
         "requestURL": "String",
         "resource": "Code",
+        "response": "String",
         "responseCode": "String",
         "sourceId": "String",
         "validateProfileId": "String",
         "value": "String",
         "warningOnly": "Boolean",
     },
     "TestScript_Capability": {
@@ -8207,14 +8432,15 @@
         "resource": "Code",
         "label": "String",
         "description": "String",
         "accept": "Code",
         "contentType": "Code",
         "destination": "Integer",
         "encodeRequestUrl": "Boolean",
+        "method": "String",
         "origin": "Integer",
         "params": "String",
         "requestHeader": "List<BackboneElement:TestScript_RequestHeader>",
         "requestId": "String",
         "responseId": "String",
         "sourceId": "String",
         "targetId": "String",
@@ -8280,26 +8506,29 @@
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "bounds": "Choice:Interval<DateTime>",
         "count": "String",
         "countMax": "String",
         "duration": "Decimal",
         "durationMax": "Decimal",
+        "durationUnit": "String",
         "frequency": "String",
         "frequencyMax": "String",
         "period": "Decimal",
         "periodMax": "Decimal",
+        "periodUnit": "String",
         "dayOfWeek": "List<Code>",
         "timeOfDay": "List<String>",
         "when": "List<String>",
         "offset": "String",
     },
     "TriggerDefinition": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
+        "type": "String",
         "name": "String",
         "timing": "Choice:String",
         "data": "List<BackboneElement:DataRequirement>",
         "condition": "BackboneElement:Expression",
     },
     "UsageContext": {
         "id": "String",
@@ -8357,14 +8586,15 @@
         "contains": "List<BackboneElement:ValueSet_Contains>",
     },
     "ValueSet_Filter": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "property": "Code",
+        "op": "String",
         "value": "String",
     },
     "ValueSet_Include": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "system": "String",
@@ -8414,14 +8644,15 @@
         "attestationSignature": "BackboneElement:Signature",
     },
     "VisionPrescription_LensSpecification": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "product": "Concept",
+        "eye": "String",
         "sphere": "Decimal",
         "cylinder": "Decimal",
         "axis": "Integer",
         "prism": "List<BackboneElement:VisionPrescription_Prism>",
         "add": "Decimal",
         "power": "Decimal",
         "backCurve": "Decimal",
@@ -8432,9 +8663,10 @@
         "note": "List<BackboneElement:Annotation>",
     },
     "VisionPrescription_Prism": {
         "id": "String",
         "extension": "List<BackboneElement:Extension>",
         "modifierExtension": "List<BackboneElement:Extension>",
         "amount": "Decimal",
+        "base": "String",
     },
 }
```

### Comparing `cqlpy-0.2.4/cqlpy/_internal/context/fhir/r4/model.py` & `cqlpy-0.2.5/cqlpy/_internal/context/fhir/r4/model.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/context/parameter_provider.py` & `cqlpy-0.2.5/cqlpy/_internal/context/parameter_provider.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/context/resource_query.py` & `cqlpy-0.2.5/cqlpy/_internal/context/resource_query.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/context/type_factory.py` & `cqlpy-0.2.5/cqlpy/_internal/context/type_factory.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/operators/clinical/any_in_valueset.py` & `cqlpy-0.2.5/cqlpy/_internal/operators/clinical/any_in_valueset.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/operators/clinical/in_valueset.py` & `cqlpy-0.2.5/cqlpy/_internal/operators/clinical/in_valueset.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/operators/comparison/greater.py` & `cqlpy-0.2.5/cqlpy/_internal/operators/comparison/greater.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/operators/comparison/greater_or_equal.py` & `cqlpy-0.2.5/cqlpy/_internal/operators/comparison/greater_or_equal.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/operators/comparison/less.py` & `cqlpy-0.2.5/cqlpy/_internal/operators/comparison/less.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/operators/comparison/less_or_equal.py` & `cqlpy-0.2.5/cqlpy/_internal/operators/comparison/less_or_equal.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/operators/comparison/not_equal.py` & `cqlpy-0.2.5/cqlpy/_internal/operators/comparison/not_equal.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/operators/cql_in.py` & `cqlpy-0.2.5/cqlpy/_internal/operators/cql_in.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/operators/date_time/add.py` & `cqlpy-0.2.5/cqlpy/_internal/operators/date_time/add.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/operators/date_time/after.py` & `cqlpy-0.2.5/cqlpy/_internal/operators/date_time/after.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/operators/date_time/before.py` & `cqlpy-0.2.5/cqlpy/_internal/operators/date_time/before.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/operators/date_time/calculate_age_at.py` & `cqlpy-0.2.5/cqlpy/_internal/operators/date_time/calculate_age_at.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/operators/date_time/difference_between.py` & `cqlpy-0.2.5/cqlpy/_internal/operators/date_time/difference_between.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/operators/date_time/duration_between.py` & `cqlpy-0.2.5/cqlpy/_internal/operators/date_time/duration_between.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/operators/date_time/subtract.py` & `cqlpy-0.2.5/cqlpy/_internal/operators/date_time/subtract.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/operators/interval/collapse.py` & `cqlpy-0.2.5/cqlpy/_internal/operators/interval/collapse.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/operators/interval/in_interval.py` & `cqlpy-0.2.5/cqlpy/_internal/operators/interval/in_interval.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/operators/interval/included_in.py` & `cqlpy-0.2.5/cqlpy/_internal/operators/interval/included_in.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/operators/interval/overlaps.py` & `cqlpy-0.2.5/cqlpy/_internal/operators/interval/overlaps.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/operators/interval/start.py` & `cqlpy-0.2.5/cqlpy/_internal/operators/interval/start.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/operators/list/intersect.py` & `cqlpy-0.2.5/cqlpy/_internal/operators/list/intersect.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/scripts/fhir_map_generator.py` & `cqlpy-0.2.5/cqlpy/_internal/scripts/fhir_map_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,17 +101,26 @@
         if self.ref is not None:
             return self.ref
         return self.type
 
     @classmethod
     def from_schema(cls, name: str, schema: dict) -> "PropertyDeclaration":
         ref = schema.get("$ref")
-        type = "ref" if ref is not None else schema.get("type")
+        enum = schema.get("enum")
+
+        type = None
+        if enum is not None:
+            type = "enum"
+        elif ref is not None:
+            type = "ref"
+        else:
+            type = schema.get("type")
+
         if type is None:
-            raise ValueError("PropertyDeclaration must have type or ref")
+            raise ValueError("PropertyDeclaration type cannot be determined")
         item_type = None
         if type == "array":
             item_type = _get_property_item_type(schema["items"])
 
         return cls(
             name=name,
             type=type,
@@ -142,15 +151,18 @@
 
 
 def build_resource_declaration(resource: dict) -> dict[str, PropertyDeclaration]:
     choices = extract_choices(resource)
     property_declarations = {
         prop: PropertyDeclaration.from_schema(prop, attributes)
         for prop, attributes in resource["properties"].items()
-        if ("$ref" in attributes or "type" in attributes) and not prop.startswith("_")
+        if any(
+            type_property in attributes for type_property in ["$ref", "type", "enum"]
+        )
+        and not prop.startswith("_")
     }
     choice_declarations = {}
     for name, declaration in property_declarations.items():
         choice = next(
             (choice for choice, values in choices.items() if name in values), None
         )
         if choice is None:
@@ -225,14 +237,16 @@
                         for choice in declaration.choices
                     }
                 )
             )
             if "Interval<DateTime>" in choices:
                 return "Choice:Interval<DateTime>"
             return f"Choice:String"
+        if declaration.type == "enum":
+            return "String"
         if declaration.type == "array":
             return self.map_array_to_cql_type(declaration.item_type)
         if declaration.type == "ref":
             return self.map_ref_to_cql_type(declaration.ref)
 
         return self.map_fhir_to_cql_type(declaration.type)
 
@@ -283,7 +297,8 @@
 
 # %%
 if __name__ == "__main__":
     argument_parser = ArgumentParser()
     argument_parser.add_argument("file_path", type=str)
     args = argument_parser.parse_args()
     print(main(args.file_path))
+    # print(main("C:/Users/jerem/Downloads/fhir.schema.json/fhir.schema.json"))
```

### Comparing `cqlpy-0.2.4/cqlpy/_internal/types/any.py` & `cqlpy-0.2.5/cqlpy/_internal/types/any.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/types/boolean.py` & `cqlpy-0.2.5/cqlpy/_internal/types/boolean.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/types/code.py` & `cqlpy-0.2.5/cqlpy/_internal/types/code.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/types/code_system.py` & `cqlpy-0.2.5/cqlpy/_internal/types/code_system.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/types/concept.py` & `cqlpy-0.2.5/cqlpy/_internal/types/concept.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/types/date.py` & `cqlpy-0.2.5/cqlpy/_internal/types/date.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/types/datetime.py` & `cqlpy-0.2.5/cqlpy/_internal/types/datetime.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/types/decimal.py` & `cqlpy-0.2.5/cqlpy/_internal/types/decimal.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/types/integer.py` & `cqlpy-0.2.5/cqlpy/_internal/types/integer.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/types/interval.py` & `cqlpy-0.2.5/cqlpy/_internal/types/interval.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/types/list.py` & `cqlpy-0.2.5/cqlpy/_internal/types/list.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/types/quantity.py` & `cqlpy-0.2.5/cqlpy/_internal/types/quantity.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/types/string.py` & `cqlpy-0.2.5/cqlpy/_internal/types/string.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/_internal/types/value_set.py` & `cqlpy-0.2.5/cqlpy/_internal/types/value_set.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/operators.py` & `cqlpy-0.2.5/cqlpy/operators.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/providers/rosetta_valueset_provider.py` & `cqlpy-0.2.5/cqlpy/providers/rosetta_valueset_provider.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/cqlpy/types.py` & `cqlpy-0.2.5/cqlpy/types.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.4/pyproject.toml` & `cqlpy-0.2.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,22 +3,22 @@
   "John Wyderko <john@careevolution.com>",
   "Jeremy Fortune <jeremy@careevolution.com>",
 ]
 description = "Tooling to execute CQL-like Python against FHIR resources."
 license = "MIT"
 name = "cqlpy"
 readme = "README.md"
-version = "0.2.4"
+version = "0.2.5"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.1.0"
+black = {extras = ["jupyter"], version = "^23.3.0"}
 mypy = "^1.1.1"
 notebook = "^6.5.3"
 types-python-dateutil = "^2.8.19.11"
 types-requests = "^2.30.0.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
```

### Comparing `cqlpy-0.2.4/PKG-INFO` & `cqlpy-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqlpy
-Version: 0.2.4
+Version: 0.2.5
 Summary: Tooling to execute CQL-like Python against FHIR resources.
 License: MIT
 Author: John Wyderko
 Author-email: john@careevolution.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

