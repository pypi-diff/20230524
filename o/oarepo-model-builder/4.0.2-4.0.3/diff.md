# Comparing `tmp/oarepo-model-builder-4.0.2.tar.gz` & `tmp/oarepo-model-builder-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-4.0.2.tar", last modified: Mon May 22 17:28:15 2023, max compression
+gzip compressed data, was "oarepo-model-builder-4.0.3.tar", last modified: Wed May 24 12:00:59 2023, max compression
```

## Comparing `oarepo-model-builder-4.0.2.tar` & `oarepo-model-builder-4.0.3.tar`

### file list

```diff
@@ -1,230 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:15.947023 oarepo-model-builder-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-22 17:28:15.947023 oarepo-model-builder-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:15.923022 oarepo-model-builder-4.0.2/oarepo_model_builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:15.923022 oarepo-model-builder-4.0.2/oarepo_model_builder/builders/
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/builders/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/builders/json_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/builders/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/builders/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/builders/model_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/builders/pyproject_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/builders/python.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/builders/python_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/builders/setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/builders/setup_py.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:15.923022 oarepo-model-builder-4.0.2/oarepo_model_builder/builders/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/builders/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/builders/templates/setup.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/builders/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:15.927023 oarepo-model-builder-4.0.2/oarepo_model_builder/builtin_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/builtin_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/builtin_models/invenio.json
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:15.927023 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:15.927023 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/facets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:15.927023 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/marshmallow/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/marshmallow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/marshmallow/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/marshmallow/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/marshmallow/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/marshmallow/object.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/marshmallow/ui_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/marshmallow/ui_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/marshmallow/ui_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:15.931023 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/blueprints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/marshmallow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/model_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/record_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/ui_marshmallow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:15.931023 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/containers/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/containers/array.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/containers/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/containers/nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/containers/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/primitive_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/generate_doc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:15.935023 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_api_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_app_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_ext_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record_jsonschemas_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record_marshmallow.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record_metadata_alembic_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record_metadata_models_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record_pid_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record_resource_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record_resource_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record_search_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record_service_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record_ui_marshmallow.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record_ui_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_script_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:15.939023 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/api_views.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/app_views.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/config.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/ext.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/imports.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/invenio_record_facets.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/invenio_record_search_options.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/marshmallow.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/permissions.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/pid_provider.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/proxies.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/record.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/record_dumper.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/record_metadata.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/resource.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/resource_config.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/service.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/service_config.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/ui_serializer.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/version.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:15.939023 oarepo-model-builder-4.0.2/oarepo_model_builder/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/merger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:15.939023 oarepo-model-builder-4.0.2/oarepo_model_builder/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/outputs/cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/outputs/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/outputs/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/outputs/json_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/outputs/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/outputs/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/outputs/python.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/outputs/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/outputs/toml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/outputs/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:15.939023 oarepo-model-builder-4.0.2/oarepo_model_builder/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/profiles/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/profiles/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:15.939023 oarepo-model-builder-4.0.2/oarepo_model_builder/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/settings/opensearch.json
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/settings/python.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:15.939023 oarepo-model-builder-4.0.2/oarepo_model_builder/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:15.943023 oarepo-model-builder-4.0.2/oarepo_model_builder/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/utils/absolute_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/utils/camelcase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:15.943023 oarepo-model-builder-4.0.2/oarepo_model_builder/utils/cst/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/utils/cst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/utils/cst/call.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/utils/cst/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/utils/cst/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/utils/cst/indented_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/utils/cst/mergers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/utils/cst/simple_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/utils/deepmerge.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/utils/facet_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/utils/import_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/utils/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/utils/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/utils/python_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/utils/verbose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:15.943023 oarepo-model-builder-4.0.2/oarepo_model_builder/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/validation/extensibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/validation/model_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/oarepo_model_builder/validation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:15.923022 oarepo-model-builder-4.0.2/oarepo_model_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-22 17:28:15.000000 oarepo-model-builder-4.0.2/oarepo_model_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-05-22 17:28:15.000000 oarepo-model-builder-4.0.2/oarepo_model_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:28:15.000000 oarepo-model-builder-4.0.2/oarepo_model_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-05-22 17:28:15.000000 oarepo-model-builder-4.0.2/oarepo_model_builder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-22 17:28:15.000000 oarepo-model-builder-4.0.2/oarepo_model_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-22 17:28:15.000000 oarepo-model-builder-4.0.2/oarepo_model_builder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-05-22 17:28:15.951023 oarepo-model-builder-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:15.947023 oarepo-model-builder-4.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/faker_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/multilang.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_builder_from_entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_cfg_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_datatype_prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_datatype_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_empty_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)   396304 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_extend.py
--rw-r--r--   0 runner    (1001) docker     (123)    26948 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_facets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_fulltext_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_jsonchema_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_mapping_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_marshmallow_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15815 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_marshmallow_ui_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    23597 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_model_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_overwrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_pid_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_plugin_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_python_mergers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_sample_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_schema_props.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_search_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16438 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_simple_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_template_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_type_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-22 17:27:32.000000 oarepo-model-builder-4.0.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:59.345605 oarepo-model-builder-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-24 12:00:59.345605 oarepo-model-builder-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:59.293605 oarepo-model-builder-4.0.3/oarepo_model_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:59.297605 oarepo-model-builder-4.0.3/oarepo_model_builder/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/builders/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/builders/json_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/builders/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/builders/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/builders/model_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/builders/pyproject_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/builders/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/builders/python_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/builders/setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/builders/setup_py.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:59.297605 oarepo-model-builder-4.0.3/oarepo_model_builder/builders/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/builders/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/builders/templates/setup.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/builders/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:59.301605 oarepo-model-builder-4.0.3/oarepo_model_builder/builtin_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/builtin_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/builtin_models/invenio.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:59.301605 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:59.301605 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:59.301605 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/facets/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/facets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/facets/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/facets/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/facets/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/facets/object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:59.305605 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/marshmallow/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/marshmallow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/marshmallow/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/marshmallow/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/marshmallow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/marshmallow/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/marshmallow/ui_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/marshmallow/ui_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/marshmallow/ui_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:59.309605 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/model_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/record_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/search_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/ui_marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:59.309605 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/containers/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/containers/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/containers/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/containers/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/primitive_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/generate_doc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:59.317605 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_api_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_app_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_ext_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_jsonschemas_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_metadata_alembic_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_metadata_models_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_pid_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_resource_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_resource_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_search_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_search_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_service_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_ui_marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_ui_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_script_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:59.321605 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/api_views.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/app_views.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/config.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/ext.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/imports.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/invenio_record_facets.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/invenio_record_search_options.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/marshmallow.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/permissions.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/pid_provider.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/proxies.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/record.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/record_dumper.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/record_metadata.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/resource.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/resource_config.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/service.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/service_config.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/ui_serializer.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/version.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:59.321605 oarepo-model-builder-4.0.3/oarepo_model_builder/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/merger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:59.329605 oarepo-model-builder-4.0.3/oarepo_model_builder/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/outputs/cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/outputs/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/outputs/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/outputs/json_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/outputs/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/outputs/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/outputs/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/outputs/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/outputs/toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/outputs/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:59.329605 oarepo-model-builder-4.0.3/oarepo_model_builder/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/profiles/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/profiles/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:59.329605 oarepo-model-builder-4.0.3/oarepo_model_builder/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/settings/opensearch.json
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/settings/python.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:59.329605 oarepo-model-builder-4.0.3/oarepo_model_builder/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:59.333605 oarepo-model-builder-4.0.3/oarepo_model_builder/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/utils/absolute_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/utils/camelcase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:59.333605 oarepo-model-builder-4.0.3/oarepo_model_builder/utils/cst/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/utils/cst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/utils/cst/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/utils/cst/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/utils/cst/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/utils/cst/indented_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/utils/cst/mergers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/utils/cst/simple_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/utils/deepmerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/utils/facet_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/utils/import_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/utils/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/utils/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/utils/python_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/utils/verbose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:59.333605 oarepo-model-builder-4.0.3/oarepo_model_builder/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/validation/extensibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/validation/model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/oarepo_model_builder/validation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:59.297605 oarepo-model-builder-4.0.3/oarepo_model_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-24 12:00:59.000000 oarepo-model-builder-4.0.3/oarepo_model_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9802 2023-05-24 12:00:59.000000 oarepo-model-builder-4.0.3/oarepo_model_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:00:59.000000 oarepo-model-builder-4.0.3/oarepo_model_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-24 12:00:59.000000 oarepo-model-builder-4.0.3/oarepo_model_builder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-24 12:00:59.000000 oarepo-model-builder-4.0.3/oarepo_model_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-24 12:00:59.000000 oarepo-model-builder-4.0.3/oarepo_model_builder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-05-24 12:00:59.345605 oarepo-model-builder-4.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:00:59.345605 oarepo-model-builder-4.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/faker_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/multilang.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_builder_from_entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_cfg_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12992 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_datatype_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_datatype_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_empty_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)   396304 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28951 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_fulltext_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_jsonchema_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_mapping_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_marshmallow_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15815 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_marshmallow_ui_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23543 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_model_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_overwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_pid_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_plugin_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_python_mergers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_sample_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_schema_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_search_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16544 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_simple_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_template_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_type_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-24 11:59:53.000000 oarepo-model-builder-4.0.3/tests/utils.py
```

### Comparing `oarepo-model-builder-4.0.2/LICENSE` & `oarepo-model-builder-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/PKG-INFO` & `oarepo-model-builder-4.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder
-Version: 4.0.2
+Version: 4.0.3
 Summary: A utility library that generates OARepo required data model files from a JSON specification file
 Description-Content-Type: text/markdown
 Provides-Extra: devs
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo model builder
```

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/builder.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/builder.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/builders/__init__.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/builders/extend.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/builders/extend.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/builders/json_base.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/builders/json_base.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/builders/jsonschema.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/builders/jsonschema.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/builders/mapping.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/builders/mapping.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/builders/model_saver.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/builders/model_saver.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/builders/python.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/builders/python.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/builders/python_structure.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/builders/python_structure.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/builders/setup_cfg.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/builders/setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/builders/utils.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/builders/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/builtin_models/invenio.json` & `oarepo-model-builder-4.0.3/oarepo_model_builder/builtin_models/invenio.json`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/cli.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/__init__.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,16 @@
 from .primitive_types import NumberDataType  # noqa , just for export
 from .primitive_types import (
     BooleanDataType,
     DoubleDataType,
     FloatDataType,
     IntegerDataType,
 )
-from .strings import (  # noqa , just for export; noqa
+from .strings import StringDataType  # noqa , just for export
+from .strings import (  # noqa
     FulltextDataType,
     FulltextKeywordDataType,
     KeywordDataType,
     StringDataType,
     URLDataType,
     UUIDDataType,
 )
```

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/__init__.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 from .enum import EnumComponent
-from .facets import RegularFacetsComponent
+
+from .facets import (
+    ArrayFacetsComponent,
+    NestedFacetsComponent,
+    ObjectFacetsComponent,
+    RegularFacetsComponent,
+)
+
 from .marshmallow import (
     ArrayMarshmallowComponent,
     ObjectMarshmallowComponent,
     RegularMarshmallowComponent,
     UIArrayMarshmallowComponent,
     UIMarshmallowComponent,
     UIObjectMarshmallowComponent,
@@ -22,23 +29,24 @@
     ProxyModelComponent,
     RecordDumperModelComponent,
     RecordMetadataModelComponent,
     RecordModelComponent,
     ResourceModelComponent,
     SampleModelComponent,
     SavedModelComponent,
+    SearchOptionsModelComponent,
     ServiceModelComponent,
     UIMarshmallowModelComponent,
     UIModelComponent,
 )
 from .sample import ArraySampleComponent, RegularSampleComponent
 from .ui import ObjectUIComponent, RegularUIComponent
 
 DEFAULT_COMPONENTS = [
-    RegularFacetsComponent,
+    SearchOptionsModelComponent,
     ArraySampleComponent,
     RegularSampleComponent,
     RegularMarshmallowComponent,
     ObjectMarshmallowComponent,
     RegularUIComponent,
     ObjectUIComponent,
     ArrayMarshmallowComponent,
@@ -62,8 +70,13 @@
     SavedModelComponent,
     ServiceModelComponent,
     UIMarshmallowModelComponent,
     UIModelComponent,
     DefaultsModelComponent,
     ProxyModelComponent,
     PluginsModelComponent,
+    ObjectFacetsComponent,
+    NestedFacetsComponent,
+    RegularFacetsComponent,
+    ArrayFacetsComponent,
+
 ]
```

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/enum.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/enum.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/marshmallow/__init__.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/marshmallow/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/marshmallow/array.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/marshmallow/array.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import List
 
+
 from oarepo_model_builder.datatypes.containers.array import ArrayDataType
 from oarepo_model_builder.datatypes.datatypes import DataType, Section, datatypes
 
 from .field import RegularMarshmallowComponent, RegularMarshmallowComponentMixin
 from .graph import MarshmallowField
```

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/marshmallow/field.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/marshmallow/field.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/marshmallow/graph.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/marshmallow/graph.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/marshmallow/object.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/marshmallow/object.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/marshmallow/ui_array.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/marshmallow/ui_array.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/marshmallow/ui_field.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/marshmallow/ui_field.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/marshmallow/ui_object.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/marshmallow/ui_object.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/__init__.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 from .plugins import PluginsModelComponent
 from .proxy import ProxyModelComponent
 from .record import RecordModelComponent
 from .record_dumper import RecordDumperModelComponent
 from .record_metadata import RecordMetadataModelComponent
 from .resource import ResourceModelComponent
 from .sample import SampleModelComponent
+from .search_options import SearchOptionsModelComponent
 from .service import ServiceModelComponent
 from .ui import UIModelComponent
 from .ui_marshmallow import UIMarshmallowModelComponent
 
 __all__ = [
     "AppModelComponent",
     "BlueprintsModelComponent",
     "FacetsModelComponent",
+    "SearchOptionsModelComponent",
     "JSONSchemaModelComponent",
     "MappingModelComponent",
     "MarshmallowModelComponent",
     "PIDModelComponent",
     "PermissionsModelComponent",
     "RecordDumperModelComponent",
     "RecordMetadataModelComponent",
```

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/app.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/app.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/blueprints.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/blueprints.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/defaults.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/defaults.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/facets.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/record_metadata.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,115 +1,83 @@
 import marshmallow as ma
 
-from oarepo_model_builder.datatypes import ModelDataType
-from oarepo_model_builder.utils.python_name import (
-    convert_config_to_qualified_name,
-    parent_module,
-)
+from oarepo_model_builder.datatypes import DataTypeComponent, ModelDataType
+from oarepo_model_builder.utils.python_name import parent_module
 from oarepo_model_builder.validation.utils import ImportSchema
 
-from ..facets import RegularFacetsComponent
-from .service import ServiceModelComponent
+from .defaults import DefaultsModelComponent
+from .record import RecordModelComponent
 from .utils import set_default
 
 
-class FacetsSchema(ma.Schema):
+class RecordMetadataClassSchema(ma.Schema):
     class Meta:
         unknown = ma.RAISE
 
-    generate = ma.fields.Bool(metadata={"doc": "Set true (default) to generate facets"})
-
-    extra_code = ma.fields.String(
-        attribute="extra-code",
-        data_key="extra-code",
-        metadata={"doc": "Extra code that will be copied to facet's file"},
+    alias = ma.fields.Str(
+        metadata={"doc": "Alias under which the metadata is registered in setup.cfg"}
     )
+    generate = ma.fields.Bool(metadata={"doc": "True to generate the metadata class"})
     module = ma.fields.String(
-        metadata={"doc": "Module where the facets will be placed"}
-    )
-    imports = ma.fields.List(
-        ma.fields.Nested(ImportSchema), metadata={"doc": "List of python imports"}
-    )
-
-
-class SearchOptionsSchema(ma.Schema):
-    class Meta:
-        unknown = ma.RAISE
-
-    generate = ma.fields.Bool(
-        metadata={"doc": "Set true (default) to generate search options"}
-    )
-
-    extra_code = ma.fields.String(
-        attribute="extra-code",
-        data_key="extra-code",
-        metadata={"doc": "Extra code to be pasted to search options module"},
+        metadata={"doc": "Module where the metadata class resides"}
     )
-    module = ma.fields.String(
-        metadata={"doc": "Module where the facets will be placed"}
-    )
-    class_ = ma.fields.String(
+    class_ = ma.fields.Str(
         attribute="class",
         data_key="class",
-        metadata={"doc": "Qualified name of search options class"},
+        metadata={"doc": "Qualified name of the class"},
     )
-    base_classes = ma.fields.String(
+    base_classes = ma.fields.List(
+        ma.fields.Str(),
         attribute="base-classes",
         data_key="base-classes",
-        metadata={"doc": "List of base classes"},
+        metadata={"doc": "A list of base classes"},
     )
-    skip = ma.fields.Boolean()
+    extra_code = ma.fields.Str(
+        attribute="extra-code",
+        data_key="extra-code",
+        metadata={"doc": "Extra code to be put below the record"},
+    )
+    table = ma.fields.Str(
+        attribute="table",
+        data_key="table",
+        metadata={"doc": "Name of the database table"},
+    )
+    alembic = ma.fields.Str(metadata={"doc": "module where alembic files are stored"})
     imports = ma.fields.List(
         ma.fields.Nested(ImportSchema), metadata={"doc": "List of python imports"}
     )
+    skip = ma.fields.Boolean()
 
 
-class FacetsSchema(ma.Schema):
-    class Meta:
-        unknown = ma.RAISE
-
-
-class FacetsModelComponent(RegularFacetsComponent):
+class RecordMetadataModelComponent(DataTypeComponent):
     eligible_datatypes = [ModelDataType]
-    depends_on = [ServiceModelComponent]
+    depends_on = [DefaultsModelComponent, RecordModelComponent]
 
     class ModelSchema(ma.Schema):
-        class Meta:
-            unknown = ma.RAISE
-
-    searchable = ma.fields.Bool()
-    facets = ma.fields.Nested(
-        FacetsSchema, metadata={"doc": "Definition of facet generator options"}
-    )
-    search_options = ma.fields.Nested(
-        SearchOptionsSchema,
-        attribute="search-options",
-        data_key="search-options",
-        metadata={"doc": "Definition of search options"},
-    )
+        record_metadata = ma.fields.Nested(
+            RecordMetadataClassSchema,
+            attribute="record-metadata",
+            data_key="record-metadata",
+            metadata={"doc": "Record metadata settings"},
+        )
 
     def before_model_prepare(self, datatype, **kwargs):
-        service_module = parent_module(datatype.definition["service"]["module"])
+        records_module = parent_module(datatype.definition["record"]["module"])
         prefix = datatype.definition["module"]["prefix"]
+        alias = datatype.definition["module"]["alias"]
 
-        facets = set_default(datatype, "facets", {})
-        facets.setdefault("module", f"{service_module}.facets")
-        facets.setdefault("generate", True)
-        facets.setdefault("extra-code", "")
-        facets.setdefault("imports", [])
-
-        search_options = set_default(datatype, "search-options", {})
-        search_module = search_options.setdefault("module", f"{service_module}.search")
-        search_options.setdefault("class", f"{search_module}.{prefix}SearchOptions")
-        search_options.setdefault("base-classes", ["InvenioSearchOptions"])
-        search_options.setdefault("generate", True)
-        search_options.setdefault("extra-code", "")
-        search_options.setdefault(
+        metadata = set_default(datatype, "record-metadata", {})
+        metadata.setdefault("generate", True)
+        metadata_module = metadata.setdefault("module", f"{records_module}.models")
+        metadata.setdefault("class", f"{metadata_module}.{prefix}Metadata")
+        metadata.setdefault("base-classes", ["db.Model", "RecordMetadataBase"])
+        metadata.setdefault("extra-code", "")
+        metadata.setdefault(
             "imports",
             [
-                {
-                    "import": "invenio_records_resources.services.SearchOptions",
-                    "alias": "InvenioSearchOptions",
-                }
+                {"import": "invenio_records.models.RecordMetadataBase"},
+                {"import": "invenio_db.db"},
             ],
         )
-        convert_config_to_qualified_name(search_options)
+        metadata.setdefault("table", f"{prefix.lower()}_metadata")
+        metadata.setdefault("alembic", f"{records_module}.alembic")
+        metadata.setdefault("alias", alias)
```

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/jsonschema.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/jsonschema.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/mapping.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/mapping.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/marshmallow.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/marshmallow.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/model_saver.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/model_saver.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/permissions.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/permissions.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/pid.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/pid.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/plugins.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/plugins.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/proxy.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/proxy.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/record.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/record.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/record_dumper.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/record_dumper.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/resource.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/sample.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/sample.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/service.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/service.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/ui.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/ui_marshmallow.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/ui_marshmallow.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/model/utils.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/model/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/sample.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/sample.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/components/ui.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/components/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/containers/array.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/containers/array.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,14 +13,17 @@
         }
     }
     marshmallow = {
         "field-class": "ma_fields.List",
     }
     json_schema = {"type": "array"}
 
+    facets = {"facet_class": "TermsFacet"}
+
+
     class ModelSchema(DataType.ModelSchema):
         items = fields.Nested(FieldSchema)
         uniqueItems = fields.Boolean(required=False)
         minItems = fields.Integer(required=False)
         maxItems = fields.Integer(required=False)
 
     def prepare(self, context):
```

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/containers/object.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/containers/object.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/datatypes.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/datatypes.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/dates.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/dates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 from .datatypes import DataType
 
 
 class BaseDateDataType(DataType):
-    marshmallow = {"field-class": "ma_fields.String"}  # NOSONAR
+
+    marshmallow = {"field-class": "ma_fields.String"}
+
+    facets = {
+        "facet_class": "DateTimeFacet",
+        "imports": [{"import": "oarepo_runtime.facets.date.DateTimeFacet"}],
+    }
+
 
 
 class DateDataType(BaseDateDataType):
     model_type = "date"
     ui = {
         "marshmallow": {
             "field-class": "l10n.LocalizedDate",
```

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/model.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/model.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/datatypes/primitive_types.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/datatypes/primitive_types.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 from marshmallow import fields
 
 from .datatypes import DataType
 
 
 class NumberDataType(DataType):
-    pass
+    facets = {
+        "facet_class": "TermsFacet",
+        "imports": [
+            {"import": "invenio_records_resources.services.records.facets.TermsFacet"}
+        ],
+    }
+
 
 
 class IntegerDataType(NumberDataType):
     model_type = "integer"
 
     ui = {
         "marshmallow": {
@@ -78,7 +84,14 @@
             "field-class": "ma_fields.Boolean",
         }
     }
     marshmallow = {
         "field-class": "ma_fields.Boolean",
     }
     json_schema = {"type": "boolean"}
+    facets = {
+        "facet_class": "TermsFacet",
+        "imports": [
+            {"import": "invenio_records_resources.services.records.facets.TermsFacet"}
+        ],
+    }
+
```

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/entrypoints.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/entrypoints.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/fs.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/fs.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/generate_doc.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/generate_doc.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/__init__.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_base.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_base.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_ext_setup_cfg.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_ext_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record_jsonschemas_setup_cfg.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_jsonschemas_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record_marshmallow.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_marshmallow.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record_metadata_alembic_setup_cfg.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_metadata_alembic_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record_metadata_models_setup_cfg.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_metadata_models_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record_resource_setup_cfg.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_resource_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record_search_setup_cfg.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_search_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_record_service_config.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_record_service_config.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/invenio_script_sample_data.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/invenio_script_sample_data.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/api_views.py.jinja2` & `oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/api_views.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/app_views.py.jinja2` & `oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/app_views.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/config.py.jinja2` & `oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/config.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/ext.py.jinja2` & `oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/ext.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/marshmallow.py.jinja2` & `oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/marshmallow.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/permissions.py.jinja2` & `oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/permissions.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/record.py.jinja2` & `oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/record.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/resource_config.py.jinja2` & `oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/resource_config.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/invenio/templates/service_config.py.jinja2` & `oarepo-model-builder-4.0.3/oarepo_model_builder/invenio/templates/service_config.py.jinja2`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 {{ vars.service_config.imports|generate_import }}
 {{ link_imports|generate_import }}
 {{ vars.record.class|generate_import }}
 {{ vars.permissions.class|generate_import }}
 {{ vars.marshmallow.class|generate_import }}
+{{ vars.search_options.class|generate_import }}
 
 
 class {{ vars.service_config|class_header }}:
     """{{ vars.record.class|base_name }} service config."""
     PERMISSIONS_PRESETS = [{% for p in vars.permissions.presets %}"{{ p }}"{{ ", " if not loop.last else "" }} {% endfor %}]
 
     url_prefix = "{{ vars.resource_config.base_url }}"
     {% if not vars.permissions.skip %}
     base_permission_policy_cls = {{ vars.permissions.class|base_name }}
     {% endif %}
     {% if not vars.marshmallow.skip %}
     schema = {{ vars.marshmallow.class|base_name }}
     {% endif %}
+    search = {{ vars.search_options.class|base_name }}
     {% if not vars.record.skip %}
     record_cls = {{ vars.record.class|base_name }}
     {% endif %}
     {% if not vars.service_config.skip %}
     service_id = "{{ vars.service_config.service_id }}"
     {% endif %}
```

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/loaders/__init__.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/merger.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/merger.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/outputs/cfg.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/outputs/cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/outputs/diff.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/outputs/diff.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/outputs/json.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/outputs/json.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/outputs/json_stack.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/outputs/json_stack.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/outputs/python.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/outputs/python.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/outputs/text.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/outputs/text.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/outputs/toml.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/outputs/toml.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/outputs/yaml.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/outputs/yaml.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/profiles/record.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/profiles/record.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/schema.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/templates/__init__.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/utils/cst/call.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/utils/cst/call.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/utils/cst/collections.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/utils/cst/collections.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/utils/cst/common.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/utils/cst/common.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/utils/cst/indented_nodes.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/utils/cst/indented_nodes.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/utils/cst/mergers.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/utils/cst/mergers.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/utils/cst/simple_nodes.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/utils/cst/simple_nodes.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/utils/deepmerge.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/utils/deepmerge.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/utils/facet_helpers.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/utils/facet_helpers.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/utils/jinja.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/utils/jinja.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/utils/properties.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/utils/properties.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/utils/python_name.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/utils/python_name.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/utils/verbose.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/utils/verbose.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/validation/__init__.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/validation/extensibility.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/validation/extensibility.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/validation/model_validation.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/validation/model_validation.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder/validation/utils.py` & `oarepo-model-builder-4.0.3/oarepo_model_builder/validation/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder.egg-info/PKG-INFO` & `oarepo-model-builder-4.0.3/oarepo_model_builder.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder
-Version: 4.0.2
+Version: 4.0.3
 Summary: A utility library that generates OARepo required data model files from a JSON specification file
 Description-Content-Type: text/markdown
 Provides-Extra: devs
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo model builder
```

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder.egg-info/SOURCES.txt` & `oarepo-model-builder-4.0.3/oarepo_model_builder.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -38,17 +38,21 @@
 oarepo_model_builder/datatypes/datatypes.py
 oarepo_model_builder/datatypes/dates.py
 oarepo_model_builder/datatypes/model.py
 oarepo_model_builder/datatypes/primitive_types.py
 oarepo_model_builder/datatypes/strings.py
 oarepo_model_builder/datatypes/components/__init__.py
 oarepo_model_builder/datatypes/components/enum.py
-oarepo_model_builder/datatypes/components/facets.py
 oarepo_model_builder/datatypes/components/sample.py
 oarepo_model_builder/datatypes/components/ui.py
+oarepo_model_builder/datatypes/components/facets/__init__.py
+oarepo_model_builder/datatypes/components/facets/array.py
+oarepo_model_builder/datatypes/components/facets/field.py
+oarepo_model_builder/datatypes/components/facets/nested.py
+oarepo_model_builder/datatypes/components/facets/object.py
 oarepo_model_builder/datatypes/components/marshmallow/__init__.py
 oarepo_model_builder/datatypes/components/marshmallow/array.py
 oarepo_model_builder/datatypes/components/marshmallow/field.py
 oarepo_model_builder/datatypes/components/marshmallow/graph.py
 oarepo_model_builder/datatypes/components/marshmallow/object.py
 oarepo_model_builder/datatypes/components/marshmallow/ui_array.py
 oarepo_model_builder/datatypes/components/marshmallow/ui_field.py
@@ -67,14 +71,15 @@
 oarepo_model_builder/datatypes/components/model/plugins.py
 oarepo_model_builder/datatypes/components/model/proxy.py
 oarepo_model_builder/datatypes/components/model/record.py
 oarepo_model_builder/datatypes/components/model/record_dumper.py
 oarepo_model_builder/datatypes/components/model/record_metadata.py
 oarepo_model_builder/datatypes/components/model/resource.py
 oarepo_model_builder/datatypes/components/model/sample.py
+oarepo_model_builder/datatypes/components/model/search_options.py
 oarepo_model_builder/datatypes/components/model/service.py
 oarepo_model_builder/datatypes/components/model/ui.py
 oarepo_model_builder/datatypes/components/model/ui_marshmallow.py
 oarepo_model_builder/datatypes/components/model/utils.py
 oarepo_model_builder/datatypes/containers/__init__.py
 oarepo_model_builder/datatypes/containers/array.py
 oarepo_model_builder/datatypes/containers/flatten.py
@@ -97,14 +102,15 @@
 oarepo_model_builder/invenio/invenio_record_metadata_models_setup_cfg.py
 oarepo_model_builder/invenio/invenio_record_permissions.py
 oarepo_model_builder/invenio/invenio_record_pid_provider.py
 oarepo_model_builder/invenio/invenio_record_resource.py
 oarepo_model_builder/invenio/invenio_record_resource_config.py
 oarepo_model_builder/invenio/invenio_record_resource_setup_cfg.py
 oarepo_model_builder/invenio/invenio_record_search.py
+oarepo_model_builder/invenio/invenio_record_search_options.py
 oarepo_model_builder/invenio/invenio_record_search_setup_cfg.py
 oarepo_model_builder/invenio/invenio_record_service.py
 oarepo_model_builder/invenio/invenio_record_service_config.py
 oarepo_model_builder/invenio/invenio_record_ui_marshmallow.py
 oarepo_model_builder/invenio/invenio_record_ui_serializer.py
 oarepo_model_builder/invenio/invenio_script_sample_data.py
 oarepo_model_builder/invenio/invenio_version.py
```

### Comparing `oarepo-model-builder-4.0.2/oarepo_model_builder.egg-info/entry_points.txt` & `oarepo-model-builder-4.0.3/oarepo_model_builder.egg-info/entry_points.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,16 @@
 0100-python_structure = oarepo_model_builder.builders.python_structure:PythonStructureBuilder
 0105-invenio_record_pid_provider = oarepo_model_builder.invenio.invenio_record_pid_provider:InvenioRecordPIDProviderBuilder
 0110-invenio_record = oarepo_model_builder.invenio.invenio_record:InvenioRecordBuilder
 0120-invenio_record_metadata = oarepo_model_builder.invenio.invenio_record_metadata:InvenioRecordMetadataBuilder
 0130-invenio_record_marshmallow = oarepo_model_builder.invenio.invenio_record_marshmallow:InvenioRecordMarshmallowBuilder
 0140-invenio_record_ui_marshmallow = oarepo_model_builder.invenio.invenio_record_ui_marshmallow:InvenioRecordUIMarshmallowBuilder
 0200-invenio_record_permissions = oarepo_model_builder.invenio.invenio_record_permissions:InvenioRecordPermissionsBuilder
-0300-invenio_record_search_options = oarepo_model_builder.invenio.invenio_record_search:InvenioRecordSearchOptionsBuilder
+0300-invenio_record_search_facets = oarepo_model_builder.invenio.invenio_record_search:InvenioRecordSearchFacetsBuilder
+0305-invenio_record_search_options = oarepo_model_builder.invenio.invenio_record_search_options:InvenioRecordSearchOptionsBuilder
 0310-invenio_record_service_config = oarepo_model_builder.invenio.invenio_record_service_config:InvenioRecordServiceConfigBuilder
 0320-invenio_record_service = oarepo_model_builder.invenio.invenio_record_service:InvenioRecordServiceBuilder
 0340-invenio_record_dumper = oarepo_model_builder.invenio.invenio_record_dumper:InvenioRecordDumperBuilder
 0400-invenio_record_resource_config = oarepo_model_builder.invenio.invenio_record_resource_config:InvenioRecordResourceConfigBuilder
 0410-invenio_record_resource = oarepo_model_builder.invenio.invenio_record_resource:InvenioRecordResourceBuilder
 0420-invenio_api_views = oarepo_model_builder.invenio.invenio_api_views:InvenioAPIViewsBuilder
 0421-invenio_app_views = oarepo_model_builder.invenio.invenio_app_views:InvenioAPPViewsBuilder
```

### Comparing `oarepo-model-builder-4.0.2/setup.cfg` & `oarepo-model-builder-4.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder
-version = 4.0.2
+version = 4.0.3
 description = A utility library that generates OARepo required data model files from a JSON specification file
 authors = Miroslav Bauer <bauer@cesnet.cz>, Miroslav Simek <simeki@vscht.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
@@ -101,15 +101,17 @@
 	0100-python_structure  = oarepo_model_builder.builders.python_structure:PythonStructureBuilder
 	0105-invenio_record_pid_provider = oarepo_model_builder.invenio.invenio_record_pid_provider:InvenioRecordPIDProviderBuilder
 	0110-invenio_record  = oarepo_model_builder.invenio.invenio_record:InvenioRecordBuilder
 	0120-invenio_record_metadata  = oarepo_model_builder.invenio.invenio_record_metadata:InvenioRecordMetadataBuilder
 	0130-invenio_record_marshmallow  = oarepo_model_builder.invenio.invenio_record_marshmallow:InvenioRecordMarshmallowBuilder
 	0140-invenio_record_ui_marshmallow  = oarepo_model_builder.invenio.invenio_record_ui_marshmallow:InvenioRecordUIMarshmallowBuilder
 	0200-invenio_record_permissions  = oarepo_model_builder.invenio.invenio_record_permissions:InvenioRecordPermissionsBuilder
-	0300-invenio_record_search_options  = oarepo_model_builder.invenio.invenio_record_search:InvenioRecordSearchOptionsBuilder
+	0300-invenio_record_search_facets  = oarepo_model_builder.invenio.invenio_record_search:InvenioRecordSearchFacetsBuilder
+	0305-invenio_record_search_options  = oarepo_model_builder.invenio.invenio_record_search_options:InvenioRecordSearchOptionsBuilder
+	
 	0310-invenio_record_service_config  = oarepo_model_builder.invenio.invenio_record_service_config:InvenioRecordServiceConfigBuilder
 	0320-invenio_record_service  = oarepo_model_builder.invenio.invenio_record_service:InvenioRecordServiceBuilder
 	0340-invenio_record_dumper  = oarepo_model_builder.invenio.invenio_record_dumper:InvenioRecordDumperBuilder
 	0400-invenio_record_resource_config  = oarepo_model_builder.invenio.invenio_record_resource_config:InvenioRecordResourceConfigBuilder
 	0410-invenio_record_resource  = oarepo_model_builder.invenio.invenio_record_resource:InvenioRecordResourceBuilder
 	0420-invenio_api_views  = oarepo_model_builder.invenio.invenio_api_views:InvenioAPIViewsBuilder
 	0421-invenio_app_views  = oarepo_model_builder.invenio.invenio_app_views:InvenioAPPViewsBuilder
```

### Comparing `oarepo-model-builder-4.0.2/tests/multilang.py` & `oarepo-model-builder-4.0.3/tests/multilang.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/tests/test_builder_from_entrypoints.py` & `oarepo-model-builder-4.0.3/tests/test_builder_from_entrypoints.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/tests/test_cfg_builders.py` & `oarepo-model-builder-4.0.3/tests/test_cfg_builders.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/tests/test_datatype_prepare.py` & `oarepo-model-builder-4.0.3/tests/test_datatype_prepare.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,14 @@
             "generate": True,
             "imports": [],
             "module": "my.test.ext",
         },
         "facets": {
             "extra-code": "",
             "generate": True,
-            "imports": [],
             "module": "my.test.services.records.facets",
         },
         "json-schema-settings": {
             "alias": "my_test_record",
             "file": "my/test/records/jsonschemas/test-1.0.0.json",
             "generate": True,
             "module": "my.test.records.jsonschemas",
```

### Comparing `oarepo-model-builder-4.0.2/tests/test_datatype_validator.py` & `oarepo-model-builder-4.0.3/tests/test_datatype_validator.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/tests/test_dependencies.py` & `oarepo-model-builder-4.0.3/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/tests/test_empty_metadata.py` & `oarepo-model-builder-4.0.3/tests/test_empty_metadata.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/tests/test_extend.py` & `oarepo-model-builder-4.0.3/tests/test_extend.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/tests/test_facets.py` & `oarepo-model-builder-4.0.3/tests/test_facets.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,109 +2,119 @@
 import re
 
 from oarepo_model_builder.entrypoints import create_builder_from_entrypoints, load_model
 from oarepo_model_builder.fs import InMemoryFileSystem
 
 DUMMY_YAML = "test.yaml"
 
-import pytest
-
-pytestmark = pytest.mark.skip()  # skip the tests for now ...
-
 
 def test_include_invenio():
     schema = load_model(
-        DUMMY_YAML,
+        "test.yaml",
         model_content={
-            "model": {
+            "record": {
                 "use": "invenio",
+                "module" : {"qualified": "test"},
                 "properties": {
                     "jej": {
                         "type": "nested",
                         "properties": {
                             "c": {
                                 "type": "keyword",
-                                "facets": {
-                                    "field": 'TermsFacet(field="cosi")'  # NOSONAR
-                                },
+                                "facets": {"path": "cosi"},
                             }
                         },
                     },
-                    "a": "fulltext+keyword",  # NOSONAR
+                    "a": "fulltext+keyword",
                     "b": {
                         "type": "keyword",
-                        "facets": {"field": 'TermsFacet(field="cosi")'},
+                        "facets": {
+                            "path": "cosi",
+                            "imports": [
+                                {
+                                    "import": "invenio_records_resources.services.records.facets.TermsFacet2"
+                                }
+                            ],
+                        },
                     },
                     "c": "fulltext",
                 },
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
-        os.path.join("test", "services", "records", "facets.py")  # NOSONAR
+        os.path.join("test", "services", "records", "facets.py")
     ).read()
+    print(data)
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
 \"""Facet definitions.\"""
 
 from invenio_search.engine import dsl
 from flask_babelex import lazy_gettext as _
 
+
 from invenio_records_resources.services.records.facets import TermsFacet
+from invenio_records_resources.services.records.facets import TermsFacet2
+
 from oarepo_runtime.facets.date import DateTimeFacet
 from oarepo_runtime.facets.nested_facet import NestedLabeledFacet
 
 
 
-jej_c = NestedLabeledFacet(path ="jej", nested_facet = TermsFacet(field="cosi"))
+_schema = TermsFacet(field="$schema", label=_("$schema.label") )
 
 
 
 a_keyword = TermsFacet(field="a.keyword", label=_("a/keyword.label") )
 
 
 
-b = TermsFacet(field="cosi")
+b = TermsFacet(field="b.cosi", label =_("b.label"))
+
+
+
+created = DateTimeFacet(field="created", label=_("created.label") )
 
 
 
 _id = TermsFacet(field="id", label=_("id.label") )
 
 
 
-created = DateTimeFacet(field="created", label=_("created.label") )
+jej_c = NestedLabeledFacet(path ="jej", nested_facet = TermsFacet(field="jej.c.cosi", label =_("jej/c.label")))
 
 
 
 updated = DateTimeFacet(field="updated", label=_("updated.label") )
 
 
 
-_schema = TermsFacet(field="$schema", label=_("$schema.label") )
-
 
     """,
     )
 
 
 def test_nested():
     schema = load_model(
         DUMMY_YAML,
         model_content={
-            "model": {
+            "record": {
                 "use": "invenio",
+                "module": {"qualified": "test"},
                 "properties": {
                     "b": {
                         "type": "nested",
                         "properties": {
                             "c": {
                                 "type": "keyword",
                             },
@@ -116,20 +126,21 @@
                         },
                     }
                 },
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "services", "records", "facets.py")
     ).read()
     print(data)
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
@@ -140,131 +151,137 @@
 from invenio_search.engine import dsl
 from flask_babelex import lazy_gettext as _
 
 from invenio_records_resources.services.records.facets import TermsFacet
 from oarepo_runtime.facets.date import DateTimeFacet
 from oarepo_runtime.facets.nested_facet import NestedLabeledFacet
 
-
+_schema = TermsFacet(field="$schema", label=_("$schema.label") )
 
 b_c = NestedLabeledFacet(path ="b", nested_facet = TermsFacet(field="b.c", label=_("b/c.label") ))
 
 
 
 b_d_keyword = NestedLabeledFacet(path ="b", nested_facet = TermsFacet(field="b.d.keyword", label=_("b/d/keyword.label") ))
 
 
 
 b_f_g = NestedLabeledFacet(path ="b", nested_facet = NestedLabeledFacet(path ="b.f", nested_facet = TermsFacet(field="b.f.g", label=_("b/f/g.label") )))
 
-
+created = DateTimeFacet(field="created", label=_("created.label") )
 
 _id = TermsFacet(field="id", label=_("id.label") )
 
 
 
-created = DateTimeFacet(field="created", label=_("created.label") )
+
 
 
 
 updated = DateTimeFacet(field="updated", label=_("updated.label") )
 
 
 
-_schema = TermsFacet(field="$schema", label=_("$schema.label") )
+
 
 """,
     )
 
 
 def test_object():
     schema = load_model(
         DUMMY_YAML,
         model_content={
-            "model": {
+            "record": {
                 "use": "invenio",
+                "module": {"qualified": "test"},
                 "properties": {
                     "b": {
                         "type": "object",
                         "properties": {
                             "c": {
                                 "type": "keyword",
                             },
                             "d": {"type": "fulltext+keyword"},
                             "f": {
                                 "type": "object",
-                                "properties": {"g": {"type": "keyword"}},
+                                "properties": {
+                                    "g": {"type": "keyword", "facets": {"path": "cosi"}}
+                                },
                             },
                             "e": "fulltext",
                         },
                     }
                 },
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "services", "records", "facets.py")
     ).read()
+    print(data)
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
         \"""Facet definitions.\"""
 
 from invenio_search.engine import dsl
 from flask_babelex import lazy_gettext as _
 
 from invenio_records_resources.services.records.facets import TermsFacet
 from oarepo_runtime.facets.date import DateTimeFacet
 
-
+_schema = TermsFacet(field="$schema", label=_("$schema.label") )
 
 b_c = TermsFacet(field="b.c", label=_("b/c.label") )
 
 
 
 b_d_keyword = TermsFacet(field="b.d.keyword", label=_("b/d/keyword.label") )
 
 
 
-b_f_g = TermsFacet(field="b.f.g", label=_("b/f/g.label") )
-
+b_f_g = TermsFacet(field="b.f.g.cosi", label=_("b/f/g.label") )
 
+created = DateTimeFacet(field="created", label=_("created.label") )
 
 _id = TermsFacet(field="id", label=_("id.label") )
 
 
 
-created = DateTimeFacet(field="created", label=_("created.label") )
+
 
 
 
 updated = DateTimeFacet(field="updated", label=_("updated.label") )
 
 
 
-_schema = TermsFacet(field="$schema", label=_("$schema.label") )
+
 """,
     )
 
 
 def test_nest_obj():
     schema = load_model(
         DUMMY_YAML,
         model_content={
-            "model": {
+            "record": {
                 "use": "invenio",
+                "module": {"qualified": "test"},
                 "properties": {
                     "b_nes": {
                         "type": "nested",
                         "properties": {
                             "c": {
                                 "type": "keyword",
                             },
@@ -289,20 +306,21 @@
                         },
                     },
                 },
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "services", "records", "facets.py")
     ).read()
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
@@ -313,14 +331,15 @@
 from flask_babelex import lazy_gettext as _
 
 from invenio_records_resources.services.records.facets import TermsFacet
 from oarepo_runtime.facets.date import DateTimeFacet
 from oarepo_runtime.facets.nested_facet import NestedLabeledFacet
 
 
+_schema = TermsFacet(field="$schema", label=_("$schema.label") )
 
 b_nes_c = NestedLabeledFacet(path ="b_nes", nested_facet = TermsFacet(field="b_nes.c", label=_("b_nes/c.label") ))
 
 
 
 b_nes_d_keyword = NestedLabeledFacet(path ="b_nes", nested_facet = TermsFacet(field="b_nes.d.keyword", label=_("b_nes/d/keyword.label") ))
 
@@ -338,52 +357,54 @@
 
 
 
 b_obj_f_g = NestedLabeledFacet(path ="b_obj.f", nested_facet = TermsFacet(field="b_obj.f.g", label=_("b_obj/f/g.label") ))
 
 
 
-_id = TermsFacet(field="id", label=_("id.label") )
 
 
 
-created = DateTimeFacet(field="created", label=_("created.label") )
 
+created = DateTimeFacet(field="created", label=_("created.label") )
 
+_id = TermsFacet(field="id", label=_("id.label") )
 
 updated = DateTimeFacet(field="updated", label=_("updated.label") )
 
 
 
-_schema = TermsFacet(field="$schema", label=_("$schema.label") )
+
 """,
     )
 
 
 def test_array():
     schema = load_model(
         DUMMY_YAML,
         model_content={
-            "model": {
+            "record": {
                 "use": "invenio",
+                "module": {"qualified": "test"},
                 "properties": {
                     "a[]": "keyword",
                     "b[]": "fulltext",
                     "c[]": "fulltext+keyword",
                 },
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
     data = builder.filesystem.open(
         os.path.join("test", "services", "records", "facets.py")
     ).read()
     print(data)
 
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
@@ -393,47 +414,48 @@
 
 from invenio_search.engine import dsl
 from flask_babelex import lazy_gettext as _
 
 from invenio_records_resources.services.records.facets import TermsFacet
 from oarepo_runtime.facets.date import DateTimeFacet
 
-
+_schema = TermsFacet(field="$schema", label=_("$schema.label") )
 
 a = TermsFacet(field="a", label=_("a.label") )
 
 
 
 c_keyword = TermsFacet(field="c.keyword", label=_("c/keyword.label") )
 
 
 
-_id = TermsFacet(field="id", label=_("id.label") )
 
 
 
-created = DateTimeFacet(field="created", label=_("created.label") )
 
+created = DateTimeFacet(field="created", label=_("created.label") )
 
+_id = TermsFacet(field="id", label=_("id.label") )
 
 updated = DateTimeFacet(field="updated", label=_("updated.label") )
 
 
 
-_schema = TermsFacet(field="$schema", label=_("$schema.label") )
+
 """,
     )
 
 
 def test_array_object():
     schema = load_model(
         DUMMY_YAML,
         model_content={
-            "model": {
+            "record": {
                 "use": "invenio",
+                "module": {"qualified": "test"},
                 "properties": {
                     "arr": {
                         "type": "array",
                         "items": {
                             "type": "object",
                             "properties": {
                                 "a": {
@@ -458,20 +480,21 @@
                         },
                     },
                 },
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "services", "records", "facets.py")
     ).read()
     print(data)
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
@@ -482,63 +505,58 @@
 from invenio_search.engine import dsl
 from flask_babelex import lazy_gettext as _
 
 from invenio_records_resources.services.records.facets import TermsFacet
 from oarepo_runtime.facets.date import DateTimeFacet
 from oarepo_runtime.facets.nested_facet import NestedLabeledFacet
 
-
+_schema = TermsFacet(field="$schema", label=_("$schema.label") )
 
 arr_a_c = TermsFacet(field="arr.a.c", label=_("arr/a/c.label") )
 
 
 
-test = TermsFacet(field="test", label=_("test.label") )
-
-
-
-test2_g = NestedLabeledFacet(path ="test2", nested_facet = TermsFacet(field="test2.g", label=_("test2/g.label") ))
-
-
+created = DateTimeFacet(field="created", label=_("created.label") )
 
 _id = TermsFacet(field="id", label=_("id.label") )
 
+test = TermsFacet(field="test", label=_("test.label") )
 
 
-created = DateTimeFacet(field="created", label=_("created.label") )
-
 
+test2_g = NestedLabeledFacet(path ="test2", nested_facet = TermsFacet(field="test2.g", label=_("test2/g.label") ))
 
 updated = DateTimeFacet(field="updated", label=_("updated.label") )
 
 
 
-_schema = TermsFacet(field="$schema", label=_("$schema.label") )
+
 """,
     )
 
 
 def test_array_nested():
     schema = load_model(
         DUMMY_YAML,
         model_content={
-            "model": {
+            "record": {
                 "use": "invenio",
+                "module": {"qualified": "test"},
                 "properties": {
                     "obj": {
                         "type": "object",
                         "properties": {
                             "arr": {
                                 "type": "array",
                                 "items": {
                                     "type": "nested",
                                     "properties": {
                                         "d": {
                                             "type": "fulltext+keyword",
-                                            # "facets": {"key": "test"},
+                                            "facets": {"key": "test"},
                                         },
                                         "e": {
                                             "type": "object",
                                             "properties": {"f": "keyword"},
                                         },
                                     },
                                 },
@@ -546,75 +564,74 @@
                         },
                     },
                 },
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "services", "records", "facets.py")
     ).read()
+    print(data)
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
         \"""Facet definitions.\"""
 
 from invenio_search.engine import dsl
 from flask_babelex import lazy_gettext as _
 
 from invenio_records_resources.services.records.facets import TermsFacet
 from oarepo_runtime.facets.date import DateTimeFacet
 from oarepo_runtime.facets.nested_facet import NestedLabeledFacet
 
+_schema = TermsFacet(field="$schema", label=_("$schema.label") )
 
 
-obj_arr_d_keyword = NestedLabeledFacet(path ="obj.arr", nested_facet = TermsFacet(field="obj.arr.d.keyword", label=_("obj/arr/d/keyword.label") ))
-
-
-
-obj_arr_e_f = NestedLabeledFacet(path ="obj.arr", nested_facet = TermsFacet(field="obj.arr.e.f", label=_("obj/arr/e/f.label") ))
-
 
+created = DateTimeFacet(field="created", label=_("created.label") )
 
 _id = TermsFacet(field="id", label=_("id.label") )
 
+test = NestedLabeledFacet(path ="obj.arr", nested_facet = TermsFacet(field="obj.arr.d.keyword", label=_("obj/arr/d/keyword.label") ))
 
 
-created = DateTimeFacet(field="created", label=_("created.label") )
-
 
+obj_arr_e_f = NestedLabeledFacet(path ="obj.arr", nested_facet = TermsFacet(field="obj.arr.e.f", label=_("obj/arr/e/f.label") ))
 
 updated = DateTimeFacet(field="updated", label=_("updated.label") )
 
 
 
-_schema = TermsFacet(field="$schema", label=_("$schema.label") )
+
 """,
     )
 
 
 def test_not_searchable():
     schema = load_model(
         DUMMY_YAML,
         model_content={
-            "model": {
+            "record": {
                 "use": "invenio",
+                "module": {"qualified": "test"},
                 "properties": {
                     "a": {"type": "fulltext+keyword", "facets": {"searchable": False}},
                     "b": {
                         "type": "keyword",
-                        "facets": {"field": 'TermsFacet(field="cosi")'},
+                        "facets": {"path": "cosi"},
                     },
                     "arr": {
                         "type": "array",
                         "items": {
                             "type": "nested",
                             "properties": {
                                 "d": {
@@ -631,77 +648,80 @@
                         },
                     },
                 },
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "services", "records", "facets.py")
     ).read()
-
+    print(data)
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
 \"""Facet definitions.\"""
 
 from invenio_search.engine import dsl
 from flask_babelex import lazy_gettext as _
 
 from invenio_records_resources.services.records.facets import TermsFacet
 from oarepo_runtime.facets.date import DateTimeFacet
 from oarepo_runtime.facets.nested_facet import NestedLabeledFacet
 
 
+_schema = TermsFacet(field="$schema", label=_("$schema.label") )
+
+
 
-b = TermsFacet(field="cosi")
 
 
 
 arr_e_f = NestedLabeledFacet(path ="arr", nested_facet = TermsFacet(field="arr.e.f", label=_("arr/e/f.label") ))
 
+b = TermsFacet(field="b.cosi", label =_("b.label") )
 
 
-_id = TermsFacet(field="id", label=_("id.label") )
-
 
 
 created = DateTimeFacet(field="created", label=_("created.label") )
 
+_id = TermsFacet(field="id", label=_("id.label") )
 
 
 updated = DateTimeFacet(field="updated", label=_("updated.label") )
 
 
 
-_schema = TermsFacet(field="$schema", label=_("$schema.label") )
 
     """,
     )
 
 
 def test_top_facets():
     schema = load_model(
         DUMMY_YAML,
         model_content={
-            "model": {
+            "record": {
                 "use": "invenio",
+                "module": {"qualified": "test"},
                 "searchable": False,
                 "properties": {
                     "a": {"type": "fulltext+keyword", "facets": {"searchable": True}},
                     "b": {
                         "type": "keyword",
-                        "facets": {"field": 'TermsFacet(field="cosi")'},
+                        "facets": {"field": "cosi"},
                     },
                     "c": "keyword",
                     "arr": {
                         "type": "array",
                         "facets": {"searchable": True},
                         "items": {
                             "type": "nested",
@@ -718,231 +738,242 @@
                     },
                     "lst[]": "keyword",
                 },
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "services", "records", "facets.py")
     ).read()
-
+    print(data)
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
 \"""Facet definitions.\"""
 
 from invenio_search.engine import dsl
 from flask_babelex import lazy_gettext as _
 
 from invenio_records_resources.services.records.facets import TermsFacet
 from oarepo_runtime.facets.date import DateTimeFacet
 from oarepo_runtime.facets.nested_facet import NestedLabeledFacet
 
 
-
-a_keyword = TermsFacet(field="a.keyword", label=_("a/keyword.label") )
-
+_schema = TermsFacet(field="$schema", label=_("$schema.label") )
 
 
-b = TermsFacet(field="cosi")
+a_keyword = TermsFacet(field="a.keyword", label=_("a/keyword.label") )
 
 
 
 arr_d = NestedLabeledFacet(path ="arr", nested_facet = TermsFacet(field="arr.d", label=_("arr/d.label") ))
 
 
 
 arr_e_f = NestedLabeledFacet(path ="arr", nested_facet = TermsFacet(field="arr.e.f", label=_("arr/e/f.label") ))
 
+created = DateTimeFacet(field="created", label=_("created.label") )
 
 
 _id = TermsFacet(field="id", label=_("id.label") )
 
 
 
-created = DateTimeFacet(field="created", label=_("created.label") )
 
 
 
 updated = DateTimeFacet(field="updated", label=_("updated.label") )
 
 
 
-_schema = TermsFacet(field="$schema", label=_("$schema.label") )
 
     """,
     )
 
 
 def test_searchable_true():
     schema = load_model(
         DUMMY_YAML,
         model_content={
-            "model": {
+            "record": {
                 "use": "invenio",
+                "module": {"qualified": "test"},
                 "properties": {
                     "a": {"type": "fulltext+keyword", "facets": {"searchable": False}},
                     "b": {
                         "type": "keyword",
-                        "facets": {"field": 'TermsFacet(field="cosi")'},
+                        "facets": {"path": "cosi"},
                     },
                     "c": "fulltext",
                     "f": {
                         "type": "object",
                         "facets": {"searchable": False},
                         "properties": {"g": {"type": "keyword"}},
                     },
                 },
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
     data = builder.filesystem.open(
         os.path.join("test", "services", "records", "facets.py")
     ).read()
-
+    print(data)
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
 \"""Facet definitions.\"""
 
 from invenio_search.engine import dsl
 from flask_babelex import lazy_gettext as _
 
 from invenio_records_resources.services.records.facets import TermsFacet
 from oarepo_runtime.facets.date import DateTimeFacet
 
 
+_schema = TermsFacet(field="$schema", label=_("$schema.label") )
 
-b = TermsFacet(field="cosi")
-
-
-
-_id = TermsFacet(field="id", label=_("id.label") )
-
+b = TermsFacet(field="b.cosi", label =_("b.label"))
 
 
 created = DateTimeFacet(field="created", label=_("created.label") )
 
+_id = TermsFacet(field="id", label=_("id.label") )
 
 
 updated = DateTimeFacet(field="updated", label=_("updated.label") )
 
 
 
-_schema = TermsFacet(field="$schema", label=_("$schema.label") )
 
     """,
     )
 
 
 def test_enum():
     schema = load_model(
         DUMMY_YAML,
         model_content={
-            "model": {
+            "record": {
                 "use": "invenio",
+                "module": {"qualified": "test"},
                 "properties": {
-                    "a": {"type": "keyword", "enum": ["a", "b"]},
+                    "a": {
+                        "type": "keyword",
+                        "enum": ["a", "b"],
+                        "facets": {
+                            "facet-class": "EnumTermsFacet",
+                            "imports": [
+                                {"import": "oarepo_runtime.facets.enum.EnumTermsFacet"}
+                            ],
+                        },
+                    },
                     "b": {
                         "type": "keyword",
                     },
                 },
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "services", "records", "facets.py")
     ).read()
+    print(data)
 
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
 \"""Facet definitions.\"""
 
 from invenio_search.engine import dsl
 from flask_babelex import lazy_gettext as _
 
 from invenio_records_resources.services.records.facets import TermsFacet
 from oarepo_runtime.facets.date import DateTimeFacet
 from oarepo_runtime.facets.enum import EnumTermsFacet
 
+_schema = TermsFacet(field="$schema", label=_("$schema.label") )
+
 
 a = EnumTermsFacet(field="a", label=_("a.label") )
 
 
 
 b = TermsFacet(field="b", label=_("b.label") )
 
 
-_id = TermsFacet(field="id", label=_("id.label") )
 
 
 
 created = DateTimeFacet(field="created", label=_("created.label") )
 
+_id = TermsFacet(field="id", label=_("id.label") )
 
 
 updated = DateTimeFacet(field="updated", label=_("updated.label") )
 
 
 
-_schema = TermsFacet(field="$schema", label=_("$schema.label") )
 
     """,
     )
 
 
 def test_customizations_args_class():
     schema = load_model(
         DUMMY_YAML,
         model_content={
-            "model": {
+            "record": {
                 "use": "invenio",
+                "module": {"qualified": "test"},
                 "properties": {
                     "a": {
                         "type": "keyword",
                         "facets": {
                             "facet-class": "MyFacetClass",
                             "args": ["blah=123"],
                             "imports": [{"import": "blah.MyFacetClass"}],
                         },
                     },
                 },
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "services", "records", "facets.py")
     ).read()
     print(data)
 
     assert re.sub(r"\s", "", data) == re.sub(
@@ -954,62 +985,67 @@
 from invenio_search.engine import dsl
 from flask_babelex import lazy_gettext as _
 
 from blah import MyFacetClass
 from invenio_records_resources.services.records.facets import TermsFacet
 from oarepo_runtime.facets.date import DateTimeFacet
 
+_schema = TermsFacet(field="$schema", label=_("$schema.label") )
+
 
 a = MyFacetClass(field="a", label=_("a.label"), blah=123 )
 
 
+created = DateTimeFacet(field="created", label=_("created.label") )
+
+
 _id = TermsFacet(field="id", label=_("id.label") )
 
 
 
-created = DateTimeFacet(field="created", label=_("created.label") )
 
 
 
 updated = DateTimeFacet(field="updated", label=_("updated.label") )
 
 
 
-_schema = TermsFacet(field="$schema", label=_("$schema.label") )
 
     """,
     )
 
 
 def test_customizations_field():
     schema = load_model(
         DUMMY_YAML,
         model_content={
-            "model": {
+            "record": {
                 "use": "invenio",
+                "module": {"qualified": "test"},
                 "properties": {
                     "a": {
                         "type": "keyword",
                         "facets": {
                             "facet-class": "MyFacetClass",
-                            "args": ["blah=123"],
+                            "args": ["blah=123", 'alzp="jej"'],
                             "path": "aaa",
                             "imports": [{"import": "blah.MyFacetClass"}],
                         },
                     },
                 },
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "services", "records", "facets.py")
     ).read()
     print(data)
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
@@ -1023,26 +1059,28 @@
 from blah import MyFacetClass
 
 from invenio_records_resources.services.records.facets import TermsFacet
 
 from oarepo_runtime.facets.date import DateTimeFacet
 
 
-a = MyFacetClass(field="a.aaa", label=_("a.label"), blah=123 )
+_schema = TermsFacet(field="$schema", label=_("$schema.label") )
+
+
+a = MyFacetClass(field="a.aaa", label=_("a.label"), blah=123, alzp="jej" )
 
 
-_id = TermsFacet(field="id", label=_("id.label") )
 
 
 
 created = DateTimeFacet(field="created", label=_("created.label") )
 
+_id = TermsFacet(field="id", label=_("id.label") )
 
 
 updated = DateTimeFacet(field="updated", label=_("updated.label") )
 
 
 
-_schema = TermsFacet(field="$schema", label=_("$schema.label") )
 
     """,
     )
```

### Comparing `oarepo-model-builder-4.0.2/tests/test_fulltext_keyword.py` & `oarepo-model-builder-4.0.3/tests/test_fulltext_keyword.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/tests/test_jsonchema_builder.py` & `oarepo-model-builder-4.0.3/tests/test_jsonchema_builder.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/tests/test_loading.py` & `oarepo-model-builder-4.0.3/tests/test_loading.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/tests/test_mapping_builder.py` & `oarepo-model-builder-4.0.3/tests/test_mapping_builder.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/tests/test_marshmallow_builder.py` & `oarepo-model-builder-4.0.3/tests/test_marshmallow_builder.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/tests/test_marshmallow_ui_builder.py` & `oarepo-model-builder-4.0.3/tests/test_marshmallow_ui_builder.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/tests/test_merge.py` & `oarepo-model-builder-4.0.3/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/tests/test_model_saver.py` & `oarepo-model-builder-4.0.3/tests/test_model_saver.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
             "generate": True,
             "imports": [],
             "module": "test.ext",
         },
         "facets": {
             "extra-code": "",
             "generate": True,
-            "imports": [],
             "module": "test.services.records.facets",
         },
         "json-schema-settings": {
             "alias": "test",
             "file": "test/records/jsonschemas/test-1.0.0.json",
             "generate": True,
             "module": "test.records.jsonschemas",
@@ -400,15 +399,14 @@
             "generate": True,
             "imports": [],
             "module": "test.ext",
         },
         "facets": {
             "extra-code": "",
             "generate": True,
-            "imports": [],
             "module": "test.services.records.facets",
         },
         "json-schema-settings": {
             "alias": "test",
             "file": "test/records/jsonschemas/test-1.0.0.json",
             "generate": True,
             "module": "test.records.jsonschemas",
```

### Comparing `oarepo-model-builder-4.0.2/tests/test_overwrite.py` & `oarepo-model-builder-4.0.3/tests/test_overwrite.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/tests/test_pid_provider.py` & `oarepo-model-builder-4.0.3/tests/test_pid_provider.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/tests/test_plugin_configuration.py` & `oarepo-model-builder-4.0.3/tests/test_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/tests/test_python_mergers.py` & `oarepo-model-builder-4.0.3/tests/test_python_mergers.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/tests/test_raw.py` & `oarepo-model-builder-4.0.3/tests/test_raw.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,14 @@
         }
     }
 
     data = builder.filesystem.read(
         os.path.join("test", "records", "jsonschemas", "test-1.0.0.json")
     )
     data = json.loads(data)
-    print(data)
     assert data == {
         "properties": {
             "a": {"type": "object"},
             "id": {"type": "string"},
             "created": {"type": "string", "format": "date-time"},
             "updated": {"type": "string", "format": "date-time"},
             "$schema": {"type": "string"},
```

### Comparing `oarepo-model-builder-4.0.2/tests/test_sample_builder.py` & `oarepo-model-builder-4.0.3/tests/test_sample_builder.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/tests/test_schema_props.py` & `oarepo-model-builder-4.0.3/tests/test_schema_props.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/tests/test_search_options.py` & `oarepo-model-builder-4.0.3/tests/test_search_options.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,125 +1,123 @@
 import os
 import re
 
-import pytest
-
 from oarepo_model_builder.entrypoints import create_builder_from_entrypoints, load_model
 from oarepo_model_builder.fs import InMemoryFileSystem
 
-pytestmark = pytest.mark.skip()  # skip the tests for now ...
-
-
 DUMMY_YAML = "test.yaml"
 
 
-def test_sort():
-    schema = load_model(
-        DUMMY_YAML,
-        model_content={
-            "record": {
-                "use": "invenio",
-                "properties": {
-                    "a": {
-                        "type": "fulltext+keyword",
-                        "sortable": {"key": "a_test"},
-                    },
-                    "b": {
-                        "type": "keyword",
-                        "facets": {"field": 'TermsFacet(field="cosi")'},
-                        "sortable": {"key": "b_test", "order": "desc"},
-                    },
-                },
-            },
-        },
-        isort=False,
-        black=False,
-    )
-
-    filesystem = InMemoryFileSystem()
-    builder = create_builder_from_entrypoints(filesystem=filesystem)
-    builder.build(schema, "")
-
-    data = builder.filesystem.open(
-        os.path.join("test", "services", "records", "search.py")
-    ).read()
-    assert re.sub(r"\s", "", data) == re.sub(
-        r"\s",
-        "",
-        """
-from invenio_records_resources.services import SearchOptions as InvenioSearchOptions
-from flask_babelex import lazy_gettext as _
-from . import facets
-
-class TestSearchOptions(InvenioSearchOptions):
-    \"""TestRecord search options.\"""
-
-    facets = {
-    'a_keyword': facets.a_keyword,
-    'b': facets.b,
-    '_id': facets._id,
-    'created': facets.created,
-    'updated': facets.updated,
-    '_schema': facets._schema,
-    }
-    sort_options = {
-        **InvenioSearchOptions.sort_options,
-    'a_test': {'fields': ['a']},
-    'b_test': {'fields': ['-b']},
-    }
-    """,
-    )
+# def test_sort():
+#     schema = load_model(
+#         DUMMY_YAML,
+#         "test",
+#         model_content={
+#             "record": {
+#                 "use": "invenio",
+#                 "properties": {
+#                     "a": {
+#                         "type": "fulltext+keyword",
+#                         "sortable": {"key": "a_test"},
+#                     },
+#                     "b": {
+#                         "type": "keyword",
+#                         "facets": {"field": 'TermsFacet(field="cosi")'},
+#                         "sortable": {"key": "b_test", "order": "desc"},
+#                     },
+#                 },
+#             },
+#         },
+#         isort=False,
+#         black=False,
+#     )
+#
+#     filesystem = InMemoryFileSystem()
+#     builder = create_builder_from_entrypoints(filesystem=filesystem)
+#     builder.build(schema, "")
+#
+#     data = builder.filesystem.open(
+#         os.path.join("test", "services", "records", "search.py")
+#     ).read()
+#     assert re.sub(r"\s", "", data) == re.sub(
+#         r"\s",
+#         "",
+#         """
+# from invenio_records_resources.services import SearchOptions as InvenioSearchOptions
+# from flask_babelex import lazy_gettext as _
+# from . import facets
+#
+# class TestSearchOptions(InvenioSearchOptions):
+#     \"""TestRecord search options.\"""
+#
+#     facets = {
+#     'a_keyword': facets.a_keyword,
+#     'b': facets.b,
+#     '_id': facets._id,
+#     'created': facets.created,
+#     'updated': facets.updated,
+#     '_schema': facets._schema,
+#     }
+#     sort_options = {
+#         **InvenioSearchOptions.sort_options,
+#     'a_test': {'fields': ['a']},
+#     'b_test': {'fields': ['-b']},
+#     }
+#     """,
+#     )
 
 
 def test_search_class():
     schema = load_model(
         DUMMY_YAML,
         model_content={
             "record": {
                 "use": "invenio",
+                "module": {"qualified": "test"},
                 "properties": {
                     "a": {"type": "fulltext+keyword"},
                     "b": {
                         "type": "keyword",
-                        "facets": {"field": 'TermsFacet(field="cosi")'},
+                        "facets": {"field": "cosi"},
                     },
                 },
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "services", "records", "search.py")
     ).read()
-    print(data)
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
 from invenio_records_resources.services import SearchOptions as InvenioSearchOptions
 from flask_babelex import lazy_gettext as _
 from . import facets
 
 
 class TestSearchOptions(InvenioSearchOptions):
     \"""TestRecord search options.\"""
 
     facets = {
+        '_schema': facets._schema,
       'a_keyword': facets.a_keyword,
       'b': facets.b,
-      '_id': facets._id,
       'created': facets.created,
+      '_id': facets._id,
       'updated': facets.updated,
-      '_schema': facets._schema,
+      
     }
     sort_options = {
         **InvenioSearchOptions.sort_options,
     }
     """,
     )
```

### Comparing `oarepo-model-builder-4.0.2/tests/test_shortcuts.py` & `oarepo-model-builder-4.0.3/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/tests/test_simple_builders.py` & `oarepo-model-builder-4.0.3/tests/test_simple_builders.py`

 * *Files 2% similar despite different names*

```diff
@@ -372,31 +372,34 @@
 
 def test_service_config():
     data = build_python_model(
         {"properties": {"a": {"type": "keyword"}}},
         [InvenioRecordServiceConfigBuilder],
         os.path.join("test", "services", "records", "config.py"),
     )
-
+    print(data)
     assert strip_whitespaces(data) == strip_whitespaces(
         '''
 from invenio_records_resources.services import RecordServiceConfig as InvenioRecordServiceConfig
 from oarepo_runtime.config.service import PermissionsPresetsConfigMixin
 from invenio_records_resources.services import RecordLink
 from invenio_records_resources.services import pagination_links
 from test.records.api import TestRecord
 from test.services.records.permissions import TestPermissionPolicy
 from test.services.records.schema import TestSchema
+from test.services.records.search import TestSearchOptions
+
 
 class TestServiceConfig(PermissionsPresetsConfigMixin, InvenioRecordServiceConfig):
     """TestRecord service config."""
     PERMISSIONS_PRESETS = ["everyone"]
     url_prefix = "/test/"
     base_permission_policy_cls = TestPermissionPolicy
     schema = TestSchema
+    search = TestSearchOptions
     record_cls = TestRecord
     service_id = "test"
     components = [ *PermissionsPresetsConfigMixin.components, *InvenioRecordServiceConfig.components]
     model = "test"
     
     @property
     def links_item(self):
```

### Comparing `oarepo-model-builder-4.0.2/tests/test_type_shortcuts.py` & `oarepo-model-builder-4.0.3/tests/test_type_shortcuts.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/tests/test_validation.py` & `oarepo-model-builder-4.0.3/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.2/tests/utils.py` & `oarepo-model-builder-4.0.3/tests/utils.py`

 * *Files identical despite different names*

