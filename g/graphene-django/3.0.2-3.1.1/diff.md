# Comparing `tmp/graphene-django-3.0.2.tar.gz` & `tmp/graphene-django-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene-django-3.0.2.tar", last modified: Wed May  3 09:17:01 2023, max compression
+gzip compressed data, was "graphene-django-3.1.1.tar", last modified: Wed May 24 13:11:31 2023, max compression
```

## Comparing `graphene-django-3.0.2.tar` & `graphene-django-3.1.1.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.089644 graphene-django-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-03 09:16:57.000000 graphene-django-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-03 09:16:57.000000 graphene-django-3.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-03 09:17:01.089644 graphene-django-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-03 09:16:57.000000 graphene-django-3.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-05-03 09:16:57.000000 graphene-django-3.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.077643 graphene-django-3.0.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.077643 graphene-django-3.0.2/examples/cookbook/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.077643 graphene-django-3.0.2/examples/cookbook/cookbook/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.077643 graphene-django-3.0.2/examples/cookbook/cookbook/ingredients/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.081644 graphene-django-3.0.2/examples/cookbook/cookbook/ingredients/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-03 09:16:57.000000 graphene-django-3.0.2/examples/cookbook/cookbook/ingredients/fixtures/ingredients.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.077643 graphene-django-3.0.2/examples/cookbook-plain/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.077643 graphene-django-3.0.2/examples/cookbook-plain/cookbook/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.077643 graphene-django-3.0.2/examples/cookbook-plain/cookbook/ingredients/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.081644 graphene-django-3.0.2/examples/cookbook-plain/cookbook/ingredients/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-03 09:16:57.000000 graphene-django-3.0.2/examples/cookbook-plain/cookbook/ingredients/fixtures/ingredients.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.081644 graphene-django-3.0.2/graphene_django/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.081644 graphene-django-3.0.2/graphene_django/debug/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/debug/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.081644 graphene-django-3.0.2/graphene_django/debug/exception/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/debug/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/debug/exception/formating.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/debug/exception/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/debug/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.081644 graphene-django-3.0.2/graphene_django/debug/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/debug/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/debug/sql/tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/debug/sql/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.085644 graphene-django-3.0.2/graphene_django/debug/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/debug/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/debug/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/debug/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.085644 graphene-django-3.0.2/graphene_django/filter/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.085644 graphene-django-3.0.2/graphene_django/filter/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/filters/array_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/filters/global_id_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/filters/list_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/filters/range_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/filters/typed_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/filterset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.085644 graphene-django-3.0.2/graphene_django/filter/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/tests/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/tests/test_array_field_contains_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/tests/test_array_field_exact_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/tests/test_array_field_overlap_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/tests/test_enum_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)    37395 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/tests/test_in_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/tests/test_range_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/tests/test_typed_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/filter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.085644 graphene-django-3.0.2/graphene_django/forms/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/forms/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/forms/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/forms/mutation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.085644 graphene-django-3.0.2/graphene_django/forms/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/forms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/forms/tests/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/forms/tests/test_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/forms/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.085644 graphene-django-3.0.2/graphene_django/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.085644 graphene-django-3.0.2/graphene_django/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/management/commands/graphql_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.085644 graphene-django-3.0.2/graphene_django/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/rest_framework/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/rest_framework/mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/rest_framework/serializer_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.085644 graphene-django-3.0.2/graphene_django/rest_framework/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/rest_framework/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/rest_framework/tests/test_field_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/rest_framework/tests/test_multiple_model_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/rest_framework/tests/test_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/rest_framework/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.081644 graphene-django-3.0.2/graphene_django/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.085644 graphene-django-3.0.2/graphene_django/static/graphene_django/
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/static/graphene_django/graphiql.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.081644 graphene-django-3.0.2/graphene_django/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.085644 graphene-django-3.0.2/graphene_django/templates/graphene/
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/templates/graphene/graphiql.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.089644 graphene-django-3.0.2/graphene_django/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.089644 graphene-django-3.0.2/graphene_django/tests/issues/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/issues/test_520.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/mutations.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/schema_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    14942 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20326 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/test_get_queryset.py
--rw-r--r--   0 runner    (1001) docker     (123)    49752 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    17540 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23821 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/urls_inherited.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/tests/urls_pretty.py
--rw-r--r--   0 runner    (1001) docker     (123)    10969 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.089644 graphene-django-3.0.2/graphene_django/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/utils/str_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.089644 graphene-django-3.0.2/graphene_django/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/utils/tests/test_str_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/utils/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-05-03 09:16:57.000000 graphene-django-3.0.2/graphene_django/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:17:01.081644 graphene-django-3.0.2/graphene_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-03 09:17:01.000000 graphene-django-3.0.2/graphene_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-03 09:17:01.000000 graphene-django-3.0.2/graphene_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 09:17:01.000000 graphene-django-3.0.2/graphene_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 09:17:01.000000 graphene-django-3.0.2/graphene_django.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-03 09:17:01.000000 graphene-django-3.0.2/graphene_django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 09:17:01.000000 graphene-django-3.0.2/graphene_django.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-03 09:17:01.089644 graphene-django-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-03 09:16:57.000000 graphene-django-3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.939906 graphene-django-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-24 13:11:28.000000 graphene-django-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-24 13:11:28.000000 graphene-django-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-05-24 13:11:31.939906 graphene-django-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-05-24 13:11:28.000000 graphene-django-3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.923906 graphene-django-3.1.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.923906 graphene-django-3.1.1/examples/cookbook/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.923906 graphene-django-3.1.1/examples/cookbook/cookbook/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.923906 graphene-django-3.1.1/examples/cookbook/cookbook/ingredients/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.923906 graphene-django-3.1.1/examples/cookbook/cookbook/ingredients/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-24 13:11:28.000000 graphene-django-3.1.1/examples/cookbook/cookbook/ingredients/fixtures/ingredients.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.923906 graphene-django-3.1.1/examples/cookbook-plain/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.923906 graphene-django-3.1.1/examples/cookbook-plain/cookbook/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.923906 graphene-django-3.1.1/examples/cookbook-plain/cookbook/ingredients/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.923906 graphene-django-3.1.1/examples/cookbook-plain/cookbook/ingredients/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-24 13:11:28.000000 graphene-django-3.1.1/examples/cookbook-plain/cookbook/ingredients/fixtures/ingredients.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.927906 graphene-django-3.1.1/graphene_django/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.927906 graphene-django-3.1.1/graphene_django/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/debug/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.927906 graphene-django-3.1.1/graphene_django/debug/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/debug/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/debug/exception/formating.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/debug/exception/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/debug/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.927906 graphene-django-3.1.1/graphene_django/debug/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/debug/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/debug/sql/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/debug/sql/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.927906 graphene-django-3.1.1/graphene_django/debug/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/debug/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/debug/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/debug/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.927906 graphene-django-3.1.1/graphene_django/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.927906 graphene-django-3.1.1/graphene_django/filter/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/filters/array_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/filters/global_id_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/filters/list_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/filters/range_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/filters/typed_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/filterset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.931906 graphene-django-3.1.1/graphene_django/filter/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/tests/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/tests/test_array_field_contains_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/tests/test_array_field_exact_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/tests/test_array_field_overlap_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/tests/test_enum_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37395 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/tests/test_in_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/tests/test_range_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/tests/test_typed_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/filter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.931906 graphene-django-3.1.1/graphene_django/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/forms/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/forms/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/forms/mutation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.931906 graphene-django-3.1.1/graphene_django/forms/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/forms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/forms/tests/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/forms/tests/test_djangoinputobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/forms/tests/test_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/forms/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.931906 graphene-django-3.1.1/graphene_django/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.931906 graphene-django-3.1.1/graphene_django/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/management/commands/graphql_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.931906 graphene-django-3.1.1/graphene_django/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/rest_framework/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/rest_framework/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/rest_framework/serializer_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.931906 graphene-django-3.1.1/graphene_django/rest_framework/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/rest_framework/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/rest_framework/tests/test_field_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/rest_framework/tests/test_multiple_model_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/rest_framework/tests/test_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/rest_framework/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.923906 graphene-django-3.1.1/graphene_django/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.931906 graphene-django-3.1.1/graphene_django/static/graphene_django/
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/static/graphene_django/graphiql.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.923906 graphene-django-3.1.1/graphene_django/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.935906 graphene-django-3.1.1/graphene_django/templates/graphene/
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/templates/graphene/graphiql.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.935906 graphene-django-3.1.1/graphene_django/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.935906 graphene-django-3.1.1/graphene_django/tests/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/issues/test_520.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/schema_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14942 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20326 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/test_get_queryset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49750 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17540 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23821 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/urls_inherited.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/tests/urls_pretty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.935906 graphene-django-3.1.1/graphene_django/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/utils/str_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.935906 graphene-django-3.1.1/graphene_django/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/utils/tests/test_str_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/utils/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14752 2023-05-24 13:11:28.000000 graphene-django-3.1.1/graphene_django/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:11:31.927906 graphene-django-3.1.1/graphene_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-05-24 13:11:31.000000 graphene-django-3.1.1/graphene_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-24 13:11:31.000000 graphene-django-3.1.1/graphene_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:11:31.000000 graphene-django-3.1.1/graphene_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:11:31.000000 graphene-django-3.1.1/graphene_django.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-24 13:11:31.000000 graphene-django-3.1.1/graphene_django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-24 13:11:31.000000 graphene-django-3.1.1/graphene_django.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-24 13:11:31.939906 graphene-django-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-24 13:11:28.000000 graphene-django-3.1.1/setup.py
```

### Comparing `graphene-django-3.0.2/LICENSE` & `graphene-django-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/examples/cookbook/cookbook/ingredients/fixtures/ingredients.json` & `graphene-django-3.1.1/examples/cookbook/cookbook/ingredients/fixtures/ingredients.json`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/examples/cookbook-plain/cookbook/ingredients/fixtures/ingredients.json` & `graphene-django-3.1.1/examples/cookbook-plain/cookbook/ingredients/fixtures/ingredients.json`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/compat.py` & `graphene-django-3.1.1/graphene_django/compat.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/converter.py` & `graphene-django-3.1.1/graphene_django/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,20 @@
     named_choices_descriptions = {c[0]: c[2] for c in choices}
 
     class EnumWithDescriptionsType:
         @property
         def description(self):
             return str(named_choices_descriptions[self.name])
 
-    return_type = Enum(name, list(named_choices), type=EnumWithDescriptionsType)
+    return_type = Enum(
+        name,
+        list(named_choices),
+        type=EnumWithDescriptionsType,
+        description="An enumeration.",  # Temporary fix until https://github.com/graphql-python/graphene/pull/1502 is merged
+    )
     return return_type
 
 
 def generate_enum_name(django_model_meta, field):
     if graphene_settings.DJANGO_CHOICE_FIELD_ENUM_CUSTOM_NAME:
         # Try and import custom function
         custom_func = import_string(
```

### Comparing `graphene-django-3.0.2/graphene_django/debug/middleware.py` & `graphene-django-3.1.1/graphene_django/debug/middleware.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/debug/sql/tracking.py` & `graphene-django-3.1.1/graphene_django/debug/sql/tracking.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/debug/sql/types.py` & `graphene-django-3.1.1/graphene_django/debug/sql/types.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/debug/tests/test_query.py` & `graphene-django-3.1.1/graphene_django/debug/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/fields.py` & `graphene-django-3.1.1/graphene_django/fields.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/filter/__init__.py` & `graphene-django-3.1.1/graphene_django/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/filter/fields.py` & `graphene-django-3.1.1/graphene_django/filter/fields.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/filter/filters/__init__.py` & `graphene-django-3.1.1/graphene_django/filter/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/filter/filters/array_filter.py` & `graphene-django-3.1.1/graphene_django/filter/filters/array_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/filter/filters/global_id_filter.py` & `graphene-django-3.1.1/graphene_django/filter/filters/global_id_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/filter/filters/list_filter.py` & `graphene-django-3.1.1/graphene_django/filter/filters/list_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/filter/filters/range_filter.py` & `graphene-django-3.1.1/graphene_django/filter/filters/range_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/filter/filters/typed_filter.py` & `graphene-django-3.1.1/graphene_django/filter/filters/typed_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/filter/filterset.py` & `graphene-django-3.1.1/graphene_django/filter/filterset.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/filter/tests/conftest.py` & `graphene-django-3.1.1/graphene_django/filter/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,14 @@
     we are running unit tests in sqlite which does not have ArrayFields.
     """
 
     class Query(graphene.ObjectType):
         events = DjangoFilterConnectionField(EventType)
 
         def resolve_events(self, info, **kwargs):
-
             events = [
                 Event(name="Live Show", tags=["concert", "music", "rock"]),
                 Event(name="Musical", tags=["movie", "music"]),
                 Event(name="Ballet", tags=["concert", "dance"]),
                 Event(name="Speech", tags=[]),
             ]
```

### Comparing `graphene-django-3.0.2/graphene_django/filter/tests/filters.py` & `graphene-django-3.1.1/graphene_django/filter/tests/filters.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/filter/tests/test_array_field_contains_filter.py` & `graphene-django-3.1.1/graphene_django/filter/tests/test_array_field_contains_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/filter/tests/test_array_field_exact_filter.py` & `graphene-django-3.1.1/graphene_django/filter/tests/test_array_field_exact_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/filter/tests/test_array_field_overlap_filter.py` & `graphene-django-3.1.1/graphene_django/filter/tests/test_array_field_overlap_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/filter/tests/test_enum_filtering.py` & `graphene-django-3.1.1/graphene_django/filter/tests/test_enum_filtering.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/filter/tests/test_fields.py` & `graphene-django-3.1.1/graphene_django/filter/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/filter/tests/test_in_filter.py` & `graphene-django-3.1.1/graphene_django/filter/tests/test_in_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/filter/tests/test_range_filter.py` & `graphene-django-3.1.1/graphene_django/filter/tests/test_range_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/filter/tests/test_typed_filter.py` & `graphene-django-3.1.1/graphene_django/filter/tests/test_typed_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/filter/utils.py` & `graphene-django-3.1.1/graphene_django/filter/utils.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/forms/converter.py` & `graphene-django-3.1.1/graphene_django/forms/converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/forms/forms.py` & `graphene-django-3.1.1/graphene_django/forms/forms.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/forms/mutation.py` & `graphene-django-3.1.1/graphene_django/forms/mutation.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,14 @@
 
     errors = graphene.List(ErrorType)
 
     @classmethod
     def __init_subclass_with_meta__(
         cls, form_class=None, only_fields=(), exclude_fields=(), **options
     ):
-
         if not form_class:
             raise Exception("form_class is required for DjangoFormMutation")
 
         form = form_class()
         input_fields = fields_for_form(form, only_fields, exclude_fields)
         output_fields = fields_for_form(form, only_fields, exclude_fields)
 
@@ -125,15 +124,14 @@
         form_class=None,
         model=None,
         return_field_name=None,
         only_fields=(),
         exclude_fields=(),
         **options,
     ):
-
         if not form_class:
             raise Exception("form_class is required for DjangoModelFormMutation")
 
         if not model:
             model = form_class._meta.model
 
         if not model:
```

### Comparing `graphene-django-3.0.2/graphene_django/forms/tests/test_converter.py` & `graphene-django-3.1.1/graphene_django/forms/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/forms/tests/test_mutation.py` & `graphene-django-3.1.1/graphene_django/forms/tests/test_mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/management/commands/graphql_schema.py` & `graphene-django-3.1.1/graphene_django/management/commands/graphql_schema.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/registry.py` & `graphene-django-3.1.1/graphene_django/registry.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/rest_framework/mutation.py` & `graphene-django-3.1.1/graphene_django/rest_framework/mutation.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,14 @@
         model_operations=("create", "update"),
         only_fields=(),
         exclude_fields=(),
         convert_choices_to_enum=True,
         _meta=None,
         **options
     ):
-
         if not serializer_class:
             raise Exception("serializer_class is required for the SerializerMutation")
 
         if "update" not in model_operations and "create" not in model_operations:
             raise Exception('model_operations must contain "create" and/or "update"')
 
         serializer = serializer_class()
```

### Comparing `graphene-django-3.0.2/graphene_django/rest_framework/serializer_converter.py` & `graphene-django-3.1.1/graphene_django/rest_framework/serializer_converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/rest_framework/tests/test_field_converter.py` & `graphene-django-3.1.1/graphene_django/rest_framework/tests/test_field_converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/rest_framework/tests/test_multiple_model_serializers.py` & `graphene-django-3.1.1/graphene_django/rest_framework/tests/test_multiple_model_serializers.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/rest_framework/tests/test_mutation.py` & `graphene-django-3.1.1/graphene_django/rest_framework/tests/test_mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/settings.py` & `graphene-django-3.1.1/graphene_django/settings.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/static/graphene_django/graphiql.js` & `graphene-django-3.1.1/graphene_django/static/graphene_django/graphiql.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -2,14 +2,15 @@
     document,
 
     GRAPHENE_SETTINGS,
     GraphiQL,
     React,
     ReactDOM,
     graphqlWs,
+    GraphiQLPluginExplorer,
     fetch,
     history,
     location,
 ) {
 
     // Collect the URL parameters
     var parameters = {};
@@ -99,39 +100,60 @@
         parameters.operationName = newOperationName;
         updateURL();
     }
 
     function updateURL() {
         history.replaceState(null, null, locationQuery(parameters));
     }
-    var options = {
-        fetcher: graphQLFetcher,
-        onEditQuery: onEditQuery,
-        onEditVariables: onEditVariables,
-        onEditOperationName: onEditOperationName,
-        isHeadersEditorEnabled: GRAPHENE_SETTINGS.graphiqlHeaderEditorEnabled,
-        shouldPersistHeaders: GRAPHENE_SETTINGS.graphiqlShouldPersistHeaders,
-        query: parameters.query,
-    };
-    if (parameters.variables) {
-        options.variables = parameters.variables;
-    }
-    if (parameters.operation_name) {
-        options.operationName = parameters.operation_name;
+
+    function GraphiQLWithExplorer() {
+        var [query, setQuery] = React.useState(parameters.query);
+
+        function handleQuery(query) {
+            setQuery(query);
+            onEditQuery(query);
+        }
+
+        var explorerPlugin = GraphiQLPluginExplorer.useExplorerPlugin({
+            query: query,
+            onEdit: handleQuery,
+        });
+
+        var options = {
+            fetcher: graphQLFetcher,
+            plugins: [explorerPlugin],
+            defaultEditorToolsVisibility: true,
+            onEditQuery: handleQuery,
+            onEditVariables: onEditVariables,
+            onEditOperationName: onEditOperationName,
+            isHeadersEditorEnabled: GRAPHENE_SETTINGS.graphiqlHeaderEditorEnabled,
+            shouldPersistHeaders: GRAPHENE_SETTINGS.graphiqlShouldPersistHeaders,
+            query: query,
+        };
+        if (parameters.variables) {
+            options.variables = parameters.variables;
+        }
+        if (parameters.operation_name) {
+            options.operationName = parameters.operation_name;
+        }
+
+        return React.createElement(GraphiQL, options);
     }
+
     // Render <GraphiQL /> into the body.
     ReactDOM.render(
-        React.createElement(GraphiQL, options),
+        React.createElement(GraphiQLWithExplorer),
         document.getElementById("editor"),
     );
 })(
     document,
 
     window.GRAPHENE_SETTINGS,
     window.GraphiQL,
     window.React,
     window.ReactDOM,
     window.graphqlWs,
+    window.GraphiQLPluginExplorer,
     window.fetch,
     window.history,
     window.location,
 );
```

### Comparing `graphene-django-3.0.2/graphene_django/templates/graphene/graphiql.html` & `graphene-django-3.1.1/graphene_django/templates/graphene/graphiql.html`

 * *Files 13% similar despite different names*

```diff
@@ -32,14 +32,17 @@
           crossorigin="anonymous"></script>
   <script src="https://cdn.jsdelivr.net/npm/graphiql@{{graphiql_version}}/graphiql.min.js"
           integrity="{{graphiql_sri}}"
           crossorigin="anonymous"></script>
   <script src="https://cdn.jsdelivr.net/npm/graphql-ws@{{subscriptions_transport_ws_version}}/umd/graphql-ws.min.js"
           integrity="{{subscriptions_transport_ws_sri}}"
           crossorigin="anonymous"></script>
+  <script src="https://cdn.jsdelivr.net/npm/@graphiql/plugin-explorer@{{graphiql_plugin_explorer_version}}/dist/graphiql-plugin-explorer.umd.js"
+          integrity="{{graphiql_plugin_explorer_sri}}"
+          crossorigin="anonymous"></script>
 </head>
 <body>
   <div id="editor"></div>
   {% csrf_token %}
   <script type="application/javascript">
     window.GRAPHENE_SETTINGS = {
     {% if subscription_path %}
```

### Comparing `graphene-django-3.0.2/graphene_django/tests/issues/test_520.py` & `graphene-django-3.1.1/graphene_django/tests/issues/test_520.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/tests/models.py` & `graphene-django-3.1.1/graphene_django/tests/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 
 class Reporter(models.Model):
     first_name = models.CharField(max_length=30)
     last_name = models.CharField(max_length=30)
     email = models.EmailField()
     pets = models.ManyToManyField("self")
-    a_choice = models.CharField(max_length=30, choices=CHOICES, blank=True)
+    a_choice = models.IntegerField(choices=CHOICES, null=True, blank=True)
     objects = models.Manager()
     doe_objects = DoeReporterManager()
 
     reporter_type = models.IntegerField(
         "Reporter Type",
         null=True,
         blank=True,
```

### Comparing `graphene-django-3.0.2/graphene_django/tests/schema.py` & `graphene-django-3.1.1/graphene_django/tests/schema.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/tests/schema_view.py` & `graphene-django-3.1.1/graphene_django/tests/schema_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import graphene
 from graphene import ObjectType, Schema
 
 from .mutations import PetFormMutation, PetMutation
 
 
 class QueryRoot(ObjectType):
-
     thrower = graphene.String(required=True)
     request = graphene.String(required=True)
     test = graphene.String(who=graphene.String())
 
     def resolve_thrower(self, info):
         raise Exception("Throws!")
```

### Comparing `graphene-django-3.0.2/graphene_django/tests/test_command.py` & `graphene-django-3.1.1/graphene_django/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/tests/test_converter.py` & `graphene-django-3.1.1/graphene_django/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/tests/test_fields.py` & `graphene-django-3.1.1/graphene_django/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/tests/test_forms.py` & `graphene-django-3.1.1/graphene_django/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/tests/test_get_queryset.py` & `graphene-django-3.1.1/graphene_django/tests/test_get_queryset.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/tests/test_query.py` & `graphene-django-3.1.1/graphene_django/tests/test_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -776,15 +776,14 @@
 
     result = schema.execute(query)
     assert not result.errors
     assert result.data == expected
 
 
 def test_should_query_connectionfields_with_last():
-
     r = Reporter.objects.create(
         first_name="John", last_name="Doe", email="johndoe@example.com", a_choice=1
     )
 
     class ReporterType(DjangoObjectType):
         class Meta:
             model = Reporter
@@ -814,15 +813,14 @@
 
     result = schema.execute(query)
     assert not result.errors
     assert result.data == expected
 
 
 def test_should_query_connectionfields_with_manager():
-
     r = Reporter.objects.create(
         first_name="John", last_name="Doe", email="johndoe@example.com", a_choice=1
     )
 
     r = Reporter.objects.create(
         first_name="John", last_name="NotDoe", email="johndoe@example.com", a_choice=1
     )
```

### Comparing `graphene-django-3.0.2/graphene_django/tests/test_schema.py` & `graphene-django-3.1.1/graphene_django/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/tests/test_types.py` & `graphene-django-3.1.1/graphene_django/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/tests/test_utils.py` & `graphene-django-3.1.1/graphene_django/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/tests/test_views.py` & `graphene-django-3.1.1/graphene_django/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/types.py` & `graphene-django-3.1.1/graphene_django/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,14 +248,15 @@
 
         _meta.model = model
         _meta.registry = registry
         _meta.filter_fields = filter_fields
         _meta.filterset_class = filterset_class
         _meta.fields = django_fields
         _meta.connection = connection
+        _meta.convert_choices_to_enum = convert_choices_to_enum
 
         super().__init_subclass_with_meta__(
             _meta=_meta, interfaces=interfaces, **options
         )
 
         # Validate fields
         validate_fields(cls, model, _meta.fields, fields, exclude)
```

### Comparing `graphene-django-3.0.2/graphene_django/utils/testing.py` & `graphene-django-3.1.1/graphene_django/utils/testing.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/utils/tests/test_testing.py` & `graphene-django-3.1.1/graphene_django/utils/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/utils/utils.py` & `graphene-django-3.1.1/graphene_django/utils/utils.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/graphene_django/views.py` & `graphene-django-3.1.1/graphene_django/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from django.db import connection, transaction
 from django.http import HttpResponse, HttpResponseNotAllowed
 from django.http.response import HttpResponseBadRequest
 from django.shortcuts import render
 from django.utils.decorators import method_decorator
 from django.views.decorators.csrf import ensure_csrf_cookie
 from django.views.generic import View
-from graphql import OperationType, get_operation_ast, parse, validate
+from graphql import OperationType, get_operation_ast, parse
 from graphql.error import GraphQLError
 from graphql.execution import ExecutionResult
 
 from graphene import Schema
 from graphql.execution.middleware import MiddlewareManager
 
 from graphene_django.constants import MUTATION_ERRORS_FLAG
@@ -72,14 +72,17 @@
 
     # The websocket transport library for subscriptions.
     subscriptions_transport_ws_version = "5.12.1"
     subscriptions_transport_ws_sri = (
         "sha256-EZhvg6ANJrBsgLvLAa0uuHNLepLJVCFYS+xlb5U/bqw="
     )
 
+    graphiql_plugin_explorer_version = "0.1.15"
+    graphiql_plugin_explorer_sri = "sha256-3hUuhBXdXlfCj6RTeEkJFtEh/kUG+TCDASFpFPLrzvE="
+
     schema = None
     graphiql = False
     middleware = None
     root_value = None
     pretty = False
     batch = False
     subscription_path = None
@@ -98,25 +101,27 @@
     ):
         if not schema:
             schema = graphene_settings.SCHEMA
 
         if middleware is None:
             middleware = graphene_settings.MIDDLEWARE
 
-        self.schema = self.schema or schema
+        self.schema = schema or self.schema
         if middleware is not None:
             if isinstance(middleware, MiddlewareManager):
                 self.middleware = middleware
             else:
                 self.middleware = list(instantiate_middleware(middleware))
         self.root_value = root_value
-        self.pretty = self.pretty or pretty
-        self.graphiql = self.graphiql or graphiql
-        self.batch = self.batch or batch
-        self.execution_context_class = execution_context_class
+        self.pretty = pretty or self.pretty
+        self.graphiql = graphiql or self.graphiql
+        self.batch = batch or self.batch
+        self.execution_context_class = (
+            execution_context_class or self.execution_context_class
+        )
         if subscription_path is None:
             self.subscription_path = graphene_settings.SUBSCRIPTION_PATH
 
         assert isinstance(
             self.schema, Schema
         ), "A Schema is required to be provided to GraphQLView."
         assert not all((graphiql, batch)), "Use either graphiql or batch processing"
@@ -154,14 +159,16 @@
                     react_sri=self.react_sri,
                     react_dom_sri=self.react_dom_sri,
                     graphiql_version=self.graphiql_version,
                     graphiql_sri=self.graphiql_sri,
                     graphiql_css_sri=self.graphiql_css_sri,
                     subscriptions_transport_ws_version=self.subscriptions_transport_ws_version,
                     subscriptions_transport_ws_sri=self.subscriptions_transport_ws_sri,
+                    graphiql_plugin_explorer_version=self.graphiql_plugin_explorer_version,
+                    graphiql_plugin_explorer_sri=self.graphiql_plugin_explorer_sri,
                     # The SUBSCRIPTION_PATH setting.
                     subscription_path=self.subscription_path,
                     # GraphiQL headers tab,
                     graphiql_header_editor_enabled=graphene_settings.GRAPHIQL_HEADER_EDITOR_ENABLED,
                     graphiql_should_persist_headers=graphene_settings.GRAPHIQL_SHOULD_PERSIST_HEADERS,
                 )
 
@@ -299,19 +306,14 @@
                     HttpResponseNotAllowed(
                         ["POST"],
                         "Can only perform a {} operation from a POST request.".format(
                             operation_ast.operation.value
                         ),
                     )
                 )
-
-        validation_errors = validate(self.schema.graphql_schema, document)
-        if validation_errors:
-            return ExecutionResult(data=None, errors=validation_errors)
-
         try:
             extra_options = {}
             if self.execution_context_class:
                 extra_options["execution_context_class"] = self.execution_context_class
 
             options = {
                 "source": query,
```

### Comparing `graphene-django-3.0.2/graphene_django.egg-info/SOURCES.txt` & `graphene-django-3.1.1/graphene_django.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 MANIFEST.in
 README.md
-README.rst
 setup.cfg
 setup.py
 examples/cookbook-plain/cookbook/ingredients/fixtures/ingredients.json
 examples/cookbook/cookbook/ingredients/fixtures/ingredients.json
 graphene_django/__init__.py
 graphene_django/compat.py
 graphene_django/conftest.py
@@ -57,14 +56,15 @@
 graphene_django/forms/__init__.py
 graphene_django/forms/converter.py
 graphene_django/forms/forms.py
 graphene_django/forms/mutation.py
 graphene_django/forms/types.py
 graphene_django/forms/tests/__init__.py
 graphene_django/forms/tests/test_converter.py
+graphene_django/forms/tests/test_djangoinputobject.py
 graphene_django/forms/tests/test_mutation.py
 graphene_django/management/__init__.py
 graphene_django/management/commands/__init__.py
 graphene_django/management/commands/graphql_schema.py
 graphene_django/rest_framework/__init__.py
 graphene_django/rest_framework/models.py
 graphene_django/rest_framework/mutation.py
```

### Comparing `graphene-django-3.0.2/graphene_django.egg-info/requires.txt` & `graphene-django-3.1.1/graphene_django.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 graphql-core<4,>=3.1.0
 graphql-relay<4,>=3.1.1
 Django>=3.2
 promise>=2.1
 text-unidecode
 
 [dev]
-black==22.8.0
-flake8==5.0.4
-flake8-black==0.3.3
-flake8-bugbear==22.9.11
+black==23.3.0
+flake8==6.0.0
+flake8-black==0.3.6
+flake8-bugbear==23.3.23
 pre-commit
-pytest>=7.1.3
+pytest>=7.3.1
 pytest-cov
 pytest-random-order
 coveralls
 mock
 pytz
 django-filter>=22.1
 pytest-django>=4.5.2
 djangorestframework>=3.6.3
 
 [rest_framework]
 djangorestframework>=3.6.3
 
 [test]
-pytest>=7.1.3
+pytest>=7.3.1
 pytest-cov
 pytest-random-order
 coveralls
 mock
 pytz
 django-filter>=22.1
 pytest-django>=4.5.2
```

### Comparing `graphene-django-3.0.2/setup.cfg` & `graphene-django-3.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `graphene-django-3.0.2/setup.py` & `graphene-django-3.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,51 +10,53 @@
         ast.literal_eval(_version_re.search(f.read().decode("utf-8")).group(1))
     )
 
 rest_framework_require = ["djangorestframework>=3.6.3"]
 
 
 tests_require = [
-    "pytest>=7.1.3",
+    "pytest>=7.3.1",
     "pytest-cov",
     "pytest-random-order",
     "coveralls",
     "mock",
     "pytz",
     "django-filter>=22.1",
     "pytest-django>=4.5.2",
 ] + rest_framework_require
 
 
 dev_requires = [
-    "black==22.8.0",
-    "flake8==5.0.4",
-    "flake8-black==0.3.3",
-    "flake8-bugbear==22.9.11",
+    "black==23.3.0",
+    "flake8==6.0.0",
+    "flake8-black==0.3.6",
+    "flake8-bugbear==23.3.23",
     "pre-commit",
 ] + tests_require
 
 setup(
     name="graphene-django",
     version=version,
     description="Graphene Django integration",
-    long_description=open("README.rst").read(),
+    long_description=open("README.md").read(),
+    long_description_content_type='text/markdown',
     url="https://github.com/graphql-python/graphene-django",
     author="Syrus Akbary",
     author_email="me@syrusakbary.com",
     license="MIT",
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Framework :: Django",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
         "Framework :: Django :: 4.1",
     ],
     keywords="api graphql protocol rest relay graphene",
```

