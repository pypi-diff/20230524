# Comparing `tmp/momento-1.4.0.tar.gz` & `tmp/momento-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momento-1.4.0.tar", max compression
+gzip compressed data, was "momento-1.5.0.tar", max compression
```

## Comparing `momento-1.4.0.tar` & `momento-1.5.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0    11357 2023-05-19 21:35:52.949685 momento-1.4.0/LICENSE
--rw-r--r--   0        0        0     5668 2023-05-19 21:35:52.953686 momento-1.4.0/README.md
--rw-r--r--   0        0        0     3685 2023-05-19 21:36:12.342445 momento-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      619 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/__init__.py
--rw-r--r--   0        0        0       86 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/auth/__init__.py
--rw-r--r--   0        0        0     2868 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/auth/credential_provider.py
--rw-r--r--   0        0        0     2003 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/auth/momento_endpoint_resolver.py
--rw-r--r--   0        0        0    43744 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/cache_client.py
--rw-r--r--   0        0        0    44407 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/cache_client_async.py
--rw-r--r--   0        0        0      176 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/config/__init__.py
--rw-r--r--   0        0        0     3250 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/config/configuration.py
--rw-r--r--   0        0        0     4290 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/config/configurations.py
--rw-r--r--   0        0        0        0 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/config/transport/__init__.py
--rw-r--r--   0        0        0      314 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/config/transport/grpc_configuration.py
--rw-r--r--   0        0        0     2358 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/config/transport/transport_strategy.py
--rw-r--r--   0        0        0     1503 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/errors/__init__.py
--rw-r--r--   0        0        0     3991 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/errors/error_converter.py
--rw-r--r--   0        0        0     2329 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/errors/error_details.py
--rw-r--r--   0        0        0     8799 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/errors/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/internal/__init__.py
--rw-r--r--   0        0        0      360 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/internal/_utilities/__init__.py
--rw-r--r--   0        0        0     4710 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/internal/_utilities/_data_validation.py
--rw-r--r--   0        0        0        0 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/internal/aio/__init__.py
--rw-r--r--   0        0        0     4377 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/internal/aio/_add_header_client_interceptor.py
--rw-r--r--   0        0        0     1856 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/internal/aio/_retry_interceptor.py
--rw-r--r--   0        0        0     6120 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/internal/aio/_scs_control_client.py
--rw-r--r--   0        0        0    48528 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/internal/aio/_scs_data_client.py
--rw-r--r--   0        0        0     3163 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/internal/aio/_scs_grpc_manager.py
--rw-r--r--   0        0        0      123 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/internal/aio/_utilities.py
--rw-r--r--   0        0        0        0 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/internal/synchronous/__init__.py
--rw-r--r--   0        0        0     3714 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/internal/synchronous/_add_header_client_interceptor.py
--rw-r--r--   0        0        0     1829 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/internal/synchronous/_retry_interceptor.py
--rw-r--r--   0        0        0     6026 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/internal/synchronous/_scs_control_client.py
--rw-r--r--   0        0        0    48148 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/internal/synchronous/_scs_data_client.py
--rw-r--r--   0        0        0     2393 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/internal/synchronous/_scs_grpc_manager.py
--rw-r--r--   0        0        0      159 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/internal/synchronous/_utilities.py
--rw-r--r--   0        0        0     2790 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/logs.py
--rw-r--r--   0        0        0        0 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/py.typed
--rw-r--r--   0        0        0      154 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/requests/__init__.py
--rw-r--r--   0        0        0     3800 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/requests/collection_ttl.py
--rw-r--r--   0        0        0       91 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/requests/sort_order.py
--rw-r--r--   0        0        0     6841 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/responses/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/responses/control/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/responses/control/cache/__init__.py
--rw-r--r--   0        0        0     1758 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/responses/control/cache/create.py
--rw-r--r--   0        0        0     1405 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/responses/control/cache/delete.py
--rw-r--r--   0        0        0      849 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/responses/control/cache/flush.py
--rw-r--r--   0        0        0     2311 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/responses/control/cache/list.py
--rw-r--r--   0        0        0        0 2023-05-19 21:35:52.953686 momento-1.4.0/src/momento/responses/control/signing_key/__init__.py
--rw-r--r--   0        0        0     1764 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/control/signing_key/create.py
--rw-r--r--   0        0        0     2479 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/control/signing_key/list.py
--rw-r--r--   0        0        0      979 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/control/signing_key/revoke.py
--rw-r--r--   0        0        0        0 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/dictionary/__init__.py
--rw-r--r--   0        0        0     2047 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/dictionary/fetch.py
--rw-r--r--   0        0        0     1678 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/dictionary/get_field.py
--rw-r--r--   0        0        0     3320 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/dictionary/get_fields.py
--rw-r--r--   0        0        0     1050 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/dictionary/increment.py
--rw-r--r--   0        0        0      945 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/dictionary/remove_field.py
--rw-r--r--   0        0        0      953 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/dictionary/remove_fields.py
--rw-r--r--   0        0        0      921 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/dictionary/set_field.py
--rw-r--r--   0        0        0      929 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/dictionary/set_fields.py
--rw-r--r--   0        0        0        0 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/list/__init__.py
--rw-r--r--   0        0        0     1052 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/list/concatenate_back.py
--rw-r--r--   0        0        0     1060 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/list/concatenate_front.py
--rw-r--r--   0        0        0     1402 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/list/fetch.py
--rw-r--r--   0        0        0     1070 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/list/length.py
--rw-r--r--   0        0        0     1189 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/list/pop_back.py
--rw-r--r--   0        0        0     1199 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/list/pop_front.py
--rw-r--r--   0        0        0      977 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/list/push_back.py
--rw-r--r--   0        0        0      985 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/list/push_front.py
--rw-r--r--   0        0        0      874 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/list/remove_value.py
--rw-r--r--   0        0        0        0 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/scalar/__init__.py
--rw-r--r--   0        0        0      823 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/scalar/delete.py
--rw-r--r--   0        0        0     1155 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/scalar/get.py
--rw-r--r--   0        0        0     1141 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/scalar/increment.py
--rw-r--r--   0        0        0      799 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/scalar/set.py
--rw-r--r--   0        0        0     1056 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/scalar/set_if_not_exists.py
--rw-r--r--   0        0        0        0 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/set/__init__.py
--rw-r--r--   0        0        0      870 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/set/add_element.py
--rw-r--r--   0        0        0      880 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/set/add_elements.py
--rw-r--r--   0        0        0     1452 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/set/fetch.py
--rw-r--r--   0        0        0      896 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/set/remove_element.py
--rw-r--r--   0        0        0      906 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/set/remove_elements.py
--rw-r--r--   0        0        0        0 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/sorted_set/__init__.py
--rw-r--r--   0        0        0     1616 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/sorted_set/fetch.py
--rw-r--r--   0        0        0     1205 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/sorted_set/get_rank.py
--rw-r--r--   0        0        0     1581 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/sorted_set/get_score.py
--rw-r--r--   0        0        0     2323 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/sorted_set/get_scores.py
--rw-r--r--   0        0        0     1046 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/sorted_set/increment.py
--rw-r--r--   0        0        0      944 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/sorted_set/put_element.py
--rw-r--r--   0        0        0      952 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/sorted_set/put_elements.py
--rw-r--r--   0        0        0      971 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/sorted_set/remove_element.py
--rw-r--r--   0        0        0      979 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/data/sorted_set/remove_elements.py
--rw-r--r--   0        0        0     1460 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/mixins.py
--rw-r--r--   0        0        0     4724 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/responses/response.py
--rw-r--r--   0        0        0      423 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/retry/__init__.py
--rw-r--r--   0        0        0     2900 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/retry/default_eligibility_strategy.py
--rw-r--r--   0        0        0      216 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/retry/eligibility_strategy.py
--rw-r--r--   0        0        0     2181 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/retry/fixed_count_retry_strategy.py
--rw-r--r--   0        0        0      251 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/retry/retry_strategy.py
--rw-r--r--   0        0        0      291 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/retry/retryable_props.py
--rw-r--r--   0        0        0     1722 2023-05-19 21:35:52.957686 momento-1.4.0/src/momento/typing.py
--rw-r--r--   0        0        0     7118 1970-01-01 00:00:00.000000 momento-1.4.0/setup.py
--rw-r--r--   0        0        0     6901 1970-01-01 00:00:00.000000 momento-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-24 00:18:16.696815 momento-1.5.0/LICENSE
+-rw-r--r--   0        0        0     5668 2023-05-24 00:18:16.696815 momento-1.5.0/README.md
+-rw-r--r--   0        0        0     3685 2023-05-24 00:18:35.041112 momento-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      619 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/__init__.py
+-rw-r--r--   0        0        0       86 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/auth/__init__.py
+-rw-r--r--   0        0        0     2868 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/auth/credential_provider.py
+-rw-r--r--   0        0        0     2003 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/auth/momento_endpoint_resolver.py
+-rw-r--r--   0        0        0    43756 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/cache_client.py
+-rw-r--r--   0        0        0    44407 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/cache_client_async.py
+-rw-r--r--   0        0        0      176 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/config/__init__.py
+-rw-r--r--   0        0        0     3250 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/config/configuration.py
+-rw-r--r--   0        0        0     4290 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/config/configurations.py
+-rw-r--r--   0        0        0        0 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/config/transport/__init__.py
+-rw-r--r--   0        0        0      314 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/config/transport/grpc_configuration.py
+-rw-r--r--   0        0        0     2358 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/config/transport/transport_strategy.py
+-rw-r--r--   0        0        0     1503 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/errors/__init__.py
+-rw-r--r--   0        0        0     3991 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/errors/error_converter.py
+-rw-r--r--   0        0        0     2329 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/errors/error_details.py
+-rw-r--r--   0        0        0     8799 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/errors/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/internal/__init__.py
+-rw-r--r--   0        0        0      360 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/internal/_utilities/__init__.py
+-rw-r--r--   0        0        0     4735 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/internal/_utilities/_data_validation.py
+-rw-r--r--   0        0        0        0 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/internal/aio/__init__.py
+-rw-r--r--   0        0        0     4377 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/internal/aio/_add_header_client_interceptor.py
+-rw-r--r--   0        0        0     1856 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/internal/aio/_retry_interceptor.py
+-rw-r--r--   0        0        0     5794 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/internal/aio/_scs_control_client.py
+-rw-r--r--   0        0        0    47746 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/internal/aio/_scs_data_client.py
+-rw-r--r--   0        0        0     3239 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/internal/aio/_scs_grpc_manager.py
+-rw-r--r--   0        0        0      123 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/internal/aio/_utilities.py
+-rw-r--r--   0        0        0        0 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/internal/synchronous/__init__.py
+-rw-r--r--   0        0        0     3714 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/internal/synchronous/_add_header_client_interceptor.py
+-rw-r--r--   0        0        0     1829 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/internal/synchronous/_retry_interceptor.py
+-rw-r--r--   0        0        0     5700 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/internal/synchronous/_scs_control_client.py
+-rw-r--r--   0        0        0    47366 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/internal/synchronous/_scs_data_client.py
+-rw-r--r--   0        0        0     2469 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/internal/synchronous/_scs_grpc_manager.py
+-rw-r--r--   0        0        0      159 2023-05-24 00:18:16.696815 momento-1.5.0/src/momento/internal/synchronous/_utilities.py
+-rw-r--r--   0        0        0     2790 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/logs.py
+-rw-r--r--   0        0        0        0 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/py.typed
+-rw-r--r--   0        0        0      154 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/requests/__init__.py
+-rw-r--r--   0        0        0     3800 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/requests/collection_ttl.py
+-rw-r--r--   0        0        0       91 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/requests/sort_order.py
+-rw-r--r--   0        0        0     6841 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/control/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/control/cache/__init__.py
+-rw-r--r--   0        0        0     1758 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/control/cache/create.py
+-rw-r--r--   0        0        0     1405 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/control/cache/delete.py
+-rw-r--r--   0        0        0      849 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/control/cache/flush.py
+-rw-r--r--   0        0        0     2275 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/control/cache/list.py
+-rw-r--r--   0        0        0        0 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/control/signing_key/__init__.py
+-rw-r--r--   0        0        0     1764 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/control/signing_key/create.py
+-rw-r--r--   0        0        0     2479 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/control/signing_key/list.py
+-rw-r--r--   0        0        0      979 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/control/signing_key/revoke.py
+-rw-r--r--   0        0        0        0 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/dictionary/__init__.py
+-rw-r--r--   0        0        0     2047 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/dictionary/fetch.py
+-rw-r--r--   0        0        0     1678 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/dictionary/get_field.py
+-rw-r--r--   0        0        0     3320 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/dictionary/get_fields.py
+-rw-r--r--   0        0        0     1050 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/dictionary/increment.py
+-rw-r--r--   0        0        0      945 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/dictionary/remove_field.py
+-rw-r--r--   0        0        0      953 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/dictionary/remove_fields.py
+-rw-r--r--   0        0        0      921 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/dictionary/set_field.py
+-rw-r--r--   0        0        0      929 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/dictionary/set_fields.py
+-rw-r--r--   0        0        0        0 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/list/__init__.py
+-rw-r--r--   0        0        0     1052 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/list/concatenate_back.py
+-rw-r--r--   0        0        0     1060 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/list/concatenate_front.py
+-rw-r--r--   0        0        0     1402 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/list/fetch.py
+-rw-r--r--   0        0        0     1070 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/list/length.py
+-rw-r--r--   0        0        0     1189 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/list/pop_back.py
+-rw-r--r--   0        0        0     1199 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/list/pop_front.py
+-rw-r--r--   0        0        0      977 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/list/push_back.py
+-rw-r--r--   0        0        0      985 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/list/push_front.py
+-rw-r--r--   0        0        0      874 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/list/remove_value.py
+-rw-r--r--   0        0        0        0 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/scalar/__init__.py
+-rw-r--r--   0        0        0      823 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/scalar/delete.py
+-rw-r--r--   0        0        0     1155 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/scalar/get.py
+-rw-r--r--   0        0        0     1141 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/scalar/increment.py
+-rw-r--r--   0        0        0      799 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/scalar/set.py
+-rw-r--r--   0        0        0     1056 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/scalar/set_if_not_exists.py
+-rw-r--r--   0        0        0        0 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/set/__init__.py
+-rw-r--r--   0        0        0      870 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/set/add_element.py
+-rw-r--r--   0        0        0      880 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/set/add_elements.py
+-rw-r--r--   0        0        0     1452 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/set/fetch.py
+-rw-r--r--   0        0        0      896 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/set/remove_element.py
+-rw-r--r--   0        0        0      906 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/set/remove_elements.py
+-rw-r--r--   0        0        0        0 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/sorted_set/__init__.py
+-rw-r--r--   0        0        0     1616 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/sorted_set/fetch.py
+-rw-r--r--   0        0        0     1205 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/sorted_set/get_rank.py
+-rw-r--r--   0        0        0     1581 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/sorted_set/get_score.py
+-rw-r--r--   0        0        0     2323 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/sorted_set/get_scores.py
+-rw-r--r--   0        0        0     1046 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/sorted_set/increment.py
+-rw-r--r--   0        0        0      944 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/sorted_set/put_element.py
+-rw-r--r--   0        0        0      952 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/sorted_set/put_elements.py
+-rw-r--r--   0        0        0      971 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/sorted_set/remove_element.py
+-rw-r--r--   0        0        0      979 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/data/sorted_set/remove_elements.py
+-rw-r--r--   0        0        0     1460 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/mixins.py
+-rw-r--r--   0        0        0     4724 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/responses/response.py
+-rw-r--r--   0        0        0      423 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/retry/__init__.py
+-rw-r--r--   0        0        0     2900 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/retry/default_eligibility_strategy.py
+-rw-r--r--   0        0        0      216 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/retry/eligibility_strategy.py
+-rw-r--r--   0        0        0     2181 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/retry/fixed_count_retry_strategy.py
+-rw-r--r--   0        0        0      251 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/retry/retry_strategy.py
+-rw-r--r--   0        0        0      291 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/retry/retryable_props.py
+-rw-r--r--   0        0        0     1722 2023-05-24 00:18:16.700815 momento-1.5.0/src/momento/typing.py
+-rw-r--r--   0        0        0     7118 1970-01-01 00:00:00.000000 momento-1.5.0/setup.py
+-rw-r--r--   0        0        0     6901 1970-01-01 00:00:00.000000 momento-1.5.0/PKG-INFO
```

### Comparing `momento-1.4.0/LICENSE` & `momento-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/README.md` & `momento-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/pyproject.toml` & `momento-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "momento"
-version = "1.4.0"
+version = "1.5.0"
 
 authors = ["Momento <hello@momentohq.com>"]
 description = "SDK for Momento"
 
 license = "Apache-2.0"
 
 documentation = "https://docs.momentohq.com/"
@@ -26,15 +26,15 @@
 ]
 
 exclude = ["src/momento/internal/codegen.py"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
-momento-wire-types = "^0.60"
+momento-wire-types = "^0.64"
 grpcio = "^1.46.0"
 # note if you bump this presigned url test need be updated
 pyjwt = "^2.4.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.1.3"
 pytest-asyncio = "^0.19.0"
```

### Comparing `momento-1.4.0/src/momento/__init__.py` & `momento-1.5.0/src/momento/__init__.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/auth/credential_provider.py` & `momento-1.5.0/src/momento/auth/credential_provider.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/auth/momento_endpoint_resolver.py` & `momento-1.5.0/src/momento/auth/momento_endpoint_resolver.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/cache_client.py` & `momento-1.5.0/src/momento/cache_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,37 +199,37 @@
     def create_cache(self, cache_name: str) -> CreateCacheResponse:
         """Creates a cache if it doesn't exist.
 
         Args:
             cache_name (str): Name of the cache to be created.
 
         Returns:
-            CreateCacheResponse: The result of a Cache Create operation.
+            CreateCacheResponse: The result of a Create Cache operation.
         """
         return self._control_client.create_cache(cache_name)
 
     def delete_cache(self, cache_name: str) -> DeleteCacheResponse:
         """Deletes a cache and all of the items within it.
 
         Args:
             cache_name (str): Name of the cache to be deleted.
 
         Returns:
-            DeleteCacheResponse: The result of a Delete operation.
+            DeleteCacheResponse: The result of a Delete Cache operation.
         """
         return self._control_client.delete_cache(cache_name)
 
     def flush_cache(self, cache_name: str) -> CacheFlushResponse:
         """Flushes a cache and empties it of all its items.
 
         Args:
             cache_name (str): Name of the cache to be flushed.
 
         Returns:
-            CacheFlushResponse: The result of a flush operation.
+            CacheFlushResponse: The result of a Flush Cache operation.
         """
         return self._control_client.flush(cache_name)
 
     def list_caches(self) -> ListCachesResponse:
         """Lists all caches.
 
         Returns:
```

### Comparing `momento-1.4.0/src/momento/cache_client_async.py` & `momento-1.5.0/src/momento/cache_client_async.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/config/configuration.py` & `momento-1.5.0/src/momento/config/configuration.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/config/configurations.py` & `momento-1.5.0/src/momento/config/configurations.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/config/transport/transport_strategy.py` & `momento-1.5.0/src/momento/config/transport/transport_strategy.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/errors/__init__.py` & `momento-1.5.0/src/momento/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/errors/error_converter.py` & `momento-1.5.0/src/momento/errors/error_converter.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/errors/error_details.py` & `momento-1.5.0/src/momento/errors/error_details.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/errors/exceptions.py` & `momento-1.5.0/src/momento/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/internal/_utilities/_data_validation.py` & `momento-1.5.0/src/momento/internal/_utilities/_data_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,22 +111,24 @@
 
 def _gen_sorted_set_values_as_bytes(
     fields: TSortedSetValues, error_message: str = DEFAULT_DICTIONARY_FIELDS_CONVERSION_ERROR
 ) -> Iterable[bytes]:
     yield from _gen_iterable_as_bytes(fields, error_message)
 
 
-def _validate_timedelta_ttl(ttl: Optional[timedelta], field_name: str) -> None:
+def _validate_timedelta_ttl(ttl: timedelta, field_name: str) -> None:
     if not isinstance(ttl, timedelta):
         raise InvalidArgumentException(f"{field_name} must be a timedelta.")
     if ttl.total_seconds() <= 0:
         raise InvalidArgumentException(f"{field_name} must be a positive amount of time.")
 
 
 def _validate_ttl(ttl: Optional[timedelta]) -> None:
+    if ttl is None:
+        return
     _validate_timedelta_ttl(ttl=ttl, field_name="TTL")
 
 
 def _validate_request_timeout(request_timeout: Optional[timedelta]) -> None:
     if request_timeout is None:
         return
     _validate_timedelta_ttl(ttl=request_timeout, field_name="Request timeout")
```

### Comparing `momento-1.4.0/src/momento/internal/aio/_add_header_client_interceptor.py` & `momento-1.5.0/src/momento/internal/aio/_add_header_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/internal/aio/_retry_interceptor.py` & `momento-1.5.0/src/momento/internal/aio/_retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/internal/aio/_scs_control_client.py` & `momento-1.5.0/src/momento/internal/aio/_scs_control_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,12 @@
 from datetime import timedelta
 
 import grpc
-from momento_wire_types.controlclient_pb2 import (
-    _CreateCacheRequest,
-    _CreateSigningKeyRequest,
-    _DeleteCacheRequest,
-    _FlushCacheRequest,
-    _ListCachesRequest,
-    _ListSigningKeysRequest,
-    _RevokeSigningKeyRequest,
-)
-from momento_wire_types.controlclient_pb2_grpc import ScsControlStub
+from momento_wire_types import controlclient_pb2 as ctrl_pb
+from momento_wire_types import controlclient_pb2_grpc as ctrl_grpc
 
 from momento import logs
 from momento.auth import CredentialProvider
 from momento.config import Configuration
 from momento.errors import convert_error
 from momento.internal._utilities import _validate_cache_name, _validate_ttl
 from momento.internal.aio._scs_grpc_manager import _ControlGrpcManager
@@ -52,92 +44,85 @@
     def endpoint(self) -> str:
         return self._endpoint
 
     async def create_cache(self, cache_name: str) -> CreateCacheResponse:
         try:
             self._logger.info(f"Creating cache with name: {cache_name}")
             _validate_cache_name(cache_name)
-            request = _CreateCacheRequest()
-            request.cache_name = cache_name
+            request = ctrl_pb._CreateCacheRequest(cache_name=cache_name)
             await self._build_stub().CreateCache(request, timeout=_DEADLINE_SECONDS)
         except Exception as e:
             self._logger.debug("Failed to create cache: %s with exception: %s", cache_name, e)
             if isinstance(e, grpc.RpcError) and e.code() == grpc.StatusCode.ALREADY_EXISTS:
                 return CreateCache.CacheAlreadyExists()
             return CreateCache.Error(convert_error(e))
         return CreateCache.Success()
 
     async def delete_cache(self, cache_name: str) -> DeleteCacheResponse:
         try:
             self._logger.info(f"Deleting cache with name: {cache_name}")
             _validate_cache_name(cache_name)
-            request = _DeleteCacheRequest()
-            request.cache_name = cache_name
+            request = ctrl_pb._DeleteCacheRequest(cache_name=cache_name)
             await self._build_stub().DeleteCache(request, timeout=_DEADLINE_SECONDS)
         except Exception as e:
             self._logger.debug("Failed to delete cache: %s with exception: %s", cache_name, e)
             return DeleteCache.Error(convert_error(e))
         return DeleteCache.Success()
 
     async def list_caches(self) -> ListCachesResponse:
         try:
-            list_caches_request = _ListCachesRequest()
-            list_caches_request.next_token = ""
+            list_caches_request = ctrl_pb._ListCachesRequest(next_token="")
             response = await self._build_stub().ListCaches(list_caches_request, timeout=_DEADLINE_SECONDS)
             return ListCaches.Success.from_grpc_response(response)
         except Exception as e:
             return ListCaches.Error(convert_error(e))
 
     async def flush(self, cache_name: str) -> CacheFlushResponse:
         try:
             _validate_cache_name(cache_name)
-            request = _FlushCacheRequest()
-            request.cache_name = cache_name
+            request = ctrl_pb._FlushCacheRequest(cache_name=cache_name)
             await self._build_stub().FlushCache(request, timeout=_DEADLINE_SECONDS)
             return CacheFlush.Success()
         except Exception as e:
             return CacheFlush.Error(convert_error(e))
 
     async def create_signing_key(self, ttl: timedelta, endpoint: str) -> CreateSigningKeyResponse:
         try:
             self._logger.info(f"Creating signing key with ttl={ttl!r} and endpoint={endpoint!r}")
             _validate_ttl(ttl)
             ttl_minutes = round(ttl.total_seconds() / 60)
             self._logger.info(f"Creating signing key with ttl (in minutes): {ttl_minutes}")
-            create_signing_key_request = _CreateSigningKeyRequest()
-            create_signing_key_request.ttl_minutes = ttl_minutes
+            create_signing_key_request = ctrl_pb._CreateSigningKeyRequest(ttl_minutes=ttl_minutes)
             response = await self._build_stub().CreateSigningKey(create_signing_key_request, timeout=_DEADLINE_SECONDS)
             return CreateSigningKey.Success.from_grpc_response(response, endpoint)
         except Exception as e:
             self._logger.warning(f"Failed to create signing key with exception: {e}")
             return CreateSigningKey.Error(convert_error(e))
 
     async def revoke_signing_key(self, key_id: str) -> RevokeSigningKeyResponse:
         try:
             self._logger.info(f"Revoking signing key with key_id {key_id}")
-            request = _RevokeSigningKeyRequest()
-            request.key_id = key_id
+            request = ctrl_pb._RevokeSigningKeyRequest(key_id=key_id)
             await self._build_stub().RevokeSigningKey(request, timeout=_DEADLINE_SECONDS)
             return RevokeSigningKey.Success()
         except Exception as e:
             self._logger.warning(f"Failed to revoke signing key with key_id {key_id} exception: {e}")
             return RevokeSigningKey.Error(convert_error(e))
 
     async def list_signing_keys(self, endpoint: str) -> ListSigningKeysResponse:
         try:
             self._logger.info("List signing keys")
-            list_signing_keys_request = _ListSigningKeysRequest()
-            list_signing_keys_request.next_token = ""
+            list_signing_keys_request = ctrl_pb._ListSigningKeysRequest(next_token="")
             response = await self._build_stub().ListSigningKeys(list_signing_keys_request, timeout=_DEADLINE_SECONDS)
             return ListSigningKeys.Success.from_grpc_response(
                 response,
                 endpoint,
             )
         except Exception as e:
             self._logger.warning(f"Failed to list signing keys with exception: {e}")
             return ListSigningKeys.Error(convert_error(e))
 
-    def _build_stub(self) -> ScsControlStub:
+    def _build_stub(self) -> ctrl_grpc.ScsControlStub:
         return self._grpc_manager.async_stub()
 
     async def close(self) -> None:
         await self._grpc_manager.close()
```

### Comparing `momento-1.4.0/src/momento/internal/aio/_scs_data_client.py` & `momento-1.5.0/src/momento/internal/synchronous/_scs_data_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,14 @@
 from __future__ import annotations
 
 from datetime import timedelta
-from typing import Optional
+from typing import Any, Optional
 
-from momento_wire_types.cacheclient_pb2 import (
-    Hit,
-    Miss,
-    _DeleteRequest,
-    _DictionaryDeleteRequest,
-    _DictionaryFetchRequest,
-    _DictionaryFieldValuePair,
-    _DictionaryGetRequest,
-    _DictionaryIncrementRequest,
-    _DictionarySetRequest,
-    _GetRequest,
-    _IncrementRequest,
-    _ListConcatenateBackRequest,
-    _ListConcatenateFrontRequest,
-    _ListFetchRequest,
-    _ListLengthRequest,
-    _ListPopBackRequest,
-    _ListPopFrontRequest,
-    _ListPushBackRequest,
-    _ListPushFrontRequest,
-    _ListRemoveRequest,
-    _SetDifferenceRequest,
-    _SetFetchRequest,
-    _SetIfNotExistsRequest,
-    _SetRequest,
-    _SetUnionRequest,
-    _SortedSetElement,
-    _SortedSetFetchRequest,
-    _SortedSetGetRankRequest,
-    _SortedSetGetScoreRequest,
-    _SortedSetIncrementRequest,
-    _SortedSetPutRequest,
-    _SortedSetRemoveRequest,
-    _Unbounded,
-)
-from momento_wire_types.cacheclient_pb2_grpc import ScsStub
+from momento_wire_types import cacheclient_pb2 as cache_pb
+from momento_wire_types import cacheclient_pb2_grpc as cache_grpc
 
 from momento import logs
 from momento.auth import CredentialProvider
 from momento.config import Configuration
 from momento.errors import UnknownException, convert_error
 from momento.internal._utilities import (
     _as_bytes,
@@ -58,16 +24,16 @@
 )
 from momento.internal._utilities._data_validation import (
     _gen_sorted_set_elements_as_bytes,
     _gen_sorted_set_values_as_bytes,
     _validate_sorted_set_name,
     _validate_sorted_set_score,
 )
-from momento.internal.aio._scs_grpc_manager import _DataGrpcManager
-from momento.internal.aio._utilities import make_metadata
+from momento.internal.synchronous._scs_grpc_manager import _DataGrpcManager
+from momento.internal.synchronous._utilities import make_metadata
 from momento.requests import CollectionTtl, SortOrder
 from momento.responses import (
     CacheDelete,
     CacheDeleteResponse,
     CacheDictionaryFetch,
     CacheDictionaryFetchResponse,
     CacheDictionaryGetField,
@@ -194,81 +160,79 @@
         _validate_ttl(default_ttl)
         self._default_ttl = default_ttl
 
     @property
     def endpoint(self) -> str:
         return self._endpoint
 
-    async def increment(
+    def increment(
         self, cache_name: TCacheName, key: TScalarKey, amount: int = 1, ttl: Optional[timedelta] = None
     ) -> CacheIncrementResponse:
         try:
             self._log_issuing_request("Increment", {"key": str(key), "amount": str(amount)})
             _validate_cache_name(cache_name)
-            item_ttl = self._default_ttl if ttl is None else ttl
-            _validate_ttl(item_ttl)
+            _validate_ttl(ttl)
 
-            request = _IncrementRequest()
-            request.cache_key = _as_bytes(key, "Unsupported type for key: ")
-            request.amount = amount
-            request.ttl_milliseconds = int(item_ttl.total_seconds() * 1000)
+            request = cache_pb._IncrementRequest(
+                cache_key=_as_bytes(key, "Unsupported type for key: "),
+                amount=amount,
+                ttl_milliseconds=self._ttl_or_default_milliseconds(ttl),
+            )
 
-            response = await self._build_stub().Increment(
+            response = self._build_stub().Increment(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("Increment", {"key": str(key), "amount": str(amount)})
             return CacheIncrement.Success(response.value)
         except Exception as e:
             self._log_request_error("increment", e)
             return CacheIncrement.Error(convert_error(e))
 
-    async def set(
+    def set(
         self,
         cache_name: str,
         key: TScalarKey,
         value: TScalarValue,
         ttl: Optional[timedelta],
     ) -> CacheSetResponse:
         try:
             self._log_issuing_request("Set", {"key": str(key)})
             _validate_cache_name(cache_name)
-            item_ttl = self._default_ttl if ttl is None else ttl
-            _validate_ttl(item_ttl)
-            request = _SetRequest()
-            request.cache_key = _as_bytes(key, "Unsupported type for key: ")
-            request.cache_body = _as_bytes(value, "Unsupported type for value: ")
-            request.ttl_milliseconds = int(item_ttl.total_seconds() * 1000)
-
-            await self._build_stub().Set(
-                request, metadata=make_metadata(cache_name), timeout=self._default_deadline_seconds
+            _validate_ttl(ttl)
+            request = cache_pb._SetRequest(
+                cache_key=_as_bytes(key, "Unsupported type for key: "),
+                cache_body=_as_bytes(value, "Unsupported type for value: "),
+                ttl_milliseconds=self._ttl_or_default_milliseconds(ttl),
             )
 
+            self._build_stub().Set(request, metadata=make_metadata(cache_name), timeout=self._default_deadline_seconds)
+
             self._log_received_response("Set", {"key": str(key)})
             return CacheSet.Success()
         except Exception as e:
             self._log_request_error("set", e)
             return CacheSet.Error(convert_error(e))
 
-    async def set_if_not_exists(
+    def set_if_not_exists(
         self, cache_name: TCacheName, key: TScalarKey, value: TScalarValue, ttl: Optional[timedelta]
     ) -> CacheSetIfNotExistsResponse:
         try:
             self._log_issuing_request("SetIfNotExists", {"key": str(key)})
 
             _validate_cache_name(cache_name)
-            item_ttl = self._default_ttl if ttl is None else ttl
-            _validate_ttl(item_ttl)
-            request = _SetIfNotExistsRequest()
-            request.cache_key = _as_bytes(key, "Unsupported type for key: ")
-            request.cache_body = _as_bytes(value, "Unsupported type for value: ")
-            request.ttl_milliseconds = int(item_ttl.total_seconds() * 1000)
+            _validate_ttl(ttl)
+            request = cache_pb._SetIfNotExistsRequest(
+                cache_key=_as_bytes(key, "Unsupported type for key: "),
+                cache_body=_as_bytes(value, "Unsupported type for value: "),
+                ttl_milliseconds=self._ttl_or_default_milliseconds(ttl),
+            )
 
-            response = await self._build_stub().SetIfNotExists(
+            response = self._build_stub().SetIfNotExists(
                 request, metadata=make_metadata(cache_name), timeout=self._default_deadline_seconds
             )
 
             self._log_received_response("SetIfNotExists", {"key": str(key)})
 
             result = response.WhichOneof("result")
             if result == "stored":
@@ -277,107 +241,106 @@
                 return CacheSetIfNotExists.NotStored()
             else:
                 raise UnknownException("SetIfNotExists responded with an unknown result")
         except Exception as e:
             self._log_request_error("set_if_not_exists", e)
             return CacheSetIfNotExists.Error(convert_error(e))
 
-    async def get(self, cache_name: str, key: TScalarKey) -> CacheGetResponse:
+    def get(self, cache_name: str, key: TScalarKey) -> CacheGetResponse:
         try:
             self._log_issuing_request("Get", {"key": str(key)})
 
             _validate_cache_name(cache_name)
-            request = _GetRequest()
-            request.cache_key = _as_bytes(key, "Unsupported type for key: ")
+            request = cache_pb._GetRequest(cache_key=_as_bytes(key, "Unsupported type for key: "))
 
-            response = await self._build_stub().Get(
+            response = self._build_stub().Get(
                 request, metadata=make_metadata(cache_name), timeout=self._default_deadline_seconds
             )
 
             self._log_received_response("Get", {"key": str(key)})
 
-            if response.result == Hit:
+            if response.result == cache_pb.Hit:
                 return CacheGet.Hit(response.cache_body)
-            elif response.result == Miss:
+            elif response.result == cache_pb.Miss:
                 return CacheGet.Miss()
             else:
                 raise UnknownException("Get responded with an unknown result")
         except Exception as e:
             self._log_request_error("set_if_not_exists", e)
             return CacheGet.Error(convert_error(e))
 
-    async def delete(self, cache_name: str, key: TScalarKey) -> CacheDeleteResponse:
+    def delete(self, cache_name: str, key: TScalarKey) -> CacheDeleteResponse:
         try:
             self._log_issuing_request("Delete", {"key": str(key)})
             _validate_cache_name(cache_name)
-            request = _DeleteRequest()
-            request.cache_key = _as_bytes(key, "Unsupported type for key: ")
+            request = cache_pb._DeleteRequest(cache_key=_as_bytes(key, "Unsupported type for key: "))
 
-            await self._build_stub().Delete(
+            self._build_stub().Delete(
                 request, metadata=make_metadata(cache_name), timeout=self._default_deadline_seconds
             )
 
             self._log_received_response("Delete", {"key": str(key)})
             return CacheDelete.Success()
         except Exception as e:
             self._log_request_error("set", e)
             return CacheDelete.Error(convert_error(e))
 
     # DICTIONARY COLLECTION METHODS
-    async def dictionary_get_fields(
+    def dictionary_get_fields(
         self,
         cache_name: TCacheName,
         dictionary_name: TDictionaryName,
         fields: TDictionaryFields,
     ) -> CacheDictionaryGetFieldsResponse:
         try:
             self._log_issuing_request("DictionaryGet", {"dictionary_name": dictionary_name})
             _validate_cache_name(cache_name)
             _validate_dictionary_name(dictionary_name)
 
-            request = _DictionaryGetRequest()
-            request.dictionary_name = _as_bytes(dictionary_name, self.__UNSUPPORTED_DICTIONARY_NAME_TYPE_MSG)
             bytes_fields = list(_gen_dictionary_fields_as_bytes(fields, self.__UNSUPPORTED_DICTIONARY_FIELDS_TYPE_MSG))
+            request = cache_pb._DictionaryGetRequest(
+                dictionary_name=_as_bytes(dictionary_name, self.__UNSUPPORTED_DICTIONARY_NAME_TYPE_MSG),
+                fields=bytes_fields,
+            )
 
-            request.fields.extend(bytes_fields)
-
-            response = await self._build_stub().DictionaryGet(
+            response = self._build_stub().DictionaryGet(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("DictionaryGet", {"dictionary_name": dictionary_name})
 
             type = response.WhichOneof("dictionary")
             if type == "found":
                 get_responses: list[CacheDictionaryGetFieldResponse] = []
                 for field, get_response in zip(bytes_fields, response.found.items):
-                    if get_response.result == Miss:
+                    if get_response.result == cache_pb.Miss:
                         get_responses.append(CacheDictionaryGetField.Miss())
                     else:
                         get_responses.append(CacheDictionaryGetField.Hit(get_response.cache_body, field))
                 return CacheDictionaryGetFields.Hit(get_responses)
             elif type == "missing":
                 return CacheDictionaryGetFields.Miss()
             else:
                 raise UnknownException("Unknown dictionary field")
         except Exception as e:
             self._log_request_error("dictionary_get_fields", e)
             return CacheDictionaryGetFields.Error(convert_error(e))
 
-    async def dictionary_fetch(
+    def dictionary_fetch(
         self, cache_name: TCacheName, dictionary_name: TDictionaryName
     ) -> CacheDictionaryFetchResponse:
         try:
             self._log_issuing_request("DictionaryFetch", {"dictionary_name": dictionary_name})
             _validate_cache_name(cache_name)
             _validate_dictionary_name(dictionary_name)
-            request = _DictionaryFetchRequest()
-            request.dictionary_name = _as_bytes(dictionary_name, self.__UNSUPPORTED_DICTIONARY_NAME_TYPE_MSG)
-            response = await self._build_stub().DictionaryFetch(
+            request = cache_pb._DictionaryFetchRequest(
+                dictionary_name=_as_bytes(dictionary_name, self.__UNSUPPORTED_DICTIONARY_NAME_TYPE_MSG)
+            )
+            response = self._build_stub().DictionaryFetch(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("DictionaryFetch", {"dictionary_name": dictionary_name})
 
             type = response.WhichOneof("dictionary")
@@ -387,179 +350,178 @@
                 return CacheDictionaryFetch.Hit({item.field: item.value for item in response.found.items})
             else:
                 raise UnknownException("Unknown dictionary field")
         except Exception as e:
             self._log_request_error("dictionary_fetch", e)
             return CacheDictionaryFetch.Error(convert_error(e))
 
-    async def dictionary_increment(
+    def dictionary_increment(
         self,
         cache_name: TCacheName,
         dictionary_name: TDictionaryName,
         field: TDictionaryField,
         amount: int = 1,
         ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
     ) -> CacheDictionaryIncrementResponse:
         try:
             self._log_issuing_request("DictionaryIncrement", {"dictionary_name": dictionary_name})
             _validate_cache_name(cache_name)
             _validate_dictionary_name(dictionary_name)
 
-            request = _DictionaryIncrementRequest()
-            request.dictionary_name = _as_bytes(dictionary_name, self.__UNSUPPORTED_DICTIONARY_NAME_TYPE_MSG)
-            request.field = _as_bytes(field, self.__UNSUPPORTED_DICTIONARY_FIELD_TYPE_MSG)
-            request.amount = amount
-            request.ttl_milliseconds = self._collection_ttl_or_default_milliseconds(ttl)
-            request.refresh_ttl = ttl.refresh_ttl
+            request = cache_pb._DictionaryIncrementRequest(
+                dictionary_name=_as_bytes(dictionary_name, self.__UNSUPPORTED_DICTIONARY_NAME_TYPE_MSG),
+                field=_as_bytes(field, self.__UNSUPPORTED_DICTIONARY_FIELD_TYPE_MSG),
+                amount=amount,
+                **self._prepare_collection_ttl_for_request(ttl),
+            )
 
-            response = await self._build_stub().DictionaryIncrement(
+            response = self._build_stub().DictionaryIncrement(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("DictionaryIncrement", {"dictionary_name": dictionary_name})
             return CacheDictionaryIncrement.Success(response.value)
         except Exception as e:
             self._log_request_error("dictionary_increment", e)
             return CacheDictionaryIncrement.Error(convert_error(e))
 
-    async def dictionary_remove_fields(
+    def dictionary_remove_fields(
         self,
         cache_name: TCacheName,
         dictionary_name: TDictionaryName,
         fields: TDictionaryFields,
     ) -> CacheDictionaryRemoveFieldsResponse:
         try:
             self._log_issuing_request("DictionaryDelete", {"dictionary_name": dictionary_name})
             _validate_cache_name(cache_name)
             _validate_dictionary_name(dictionary_name)
 
-            request = _DictionaryDeleteRequest()
-            request.dictionary_name = _as_bytes(dictionary_name, self.__UNSUPPORTED_DICTIONARY_NAME_TYPE_MSG)
-            request.some.fields.extend(
-                _gen_dictionary_fields_as_bytes(fields, self.__UNSUPPORTED_DICTIONARY_FIELDS_TYPE_MSG)
+            request = cache_pb._DictionaryDeleteRequest(
+                dictionary_name=_as_bytes(dictionary_name, self.__UNSUPPORTED_DICTIONARY_NAME_TYPE_MSG),
+                some=cache_pb._DictionaryDeleteRequest.Some(
+                    fields=_gen_dictionary_fields_as_bytes(fields, self.__UNSUPPORTED_DICTIONARY_FIELDS_TYPE_MSG)
+                ),
             )
 
-            await self._build_stub().DictionaryDelete(
+            self._build_stub().DictionaryDelete(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("DictionaryDelete", {"dictionary_name": dictionary_name})
             return CacheDictionaryRemoveFields.Success()
         except Exception as e:
             self._log_request_error("dictionary_remove_fields", e)
             return CacheDictionaryRemoveFields.Error(convert_error(e))
 
-    async def dictionary_set_fields(
+    def dictionary_set_fields(
         self,
         cache_name: TCacheName,
         dictionary_name: TDictionaryName,
         items: TDictionaryItems,
         ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
     ) -> CacheDictionarySetFieldsResponse:
         try:
             self._log_issuing_request("DictionarySet", {"dictionary_name": dictionary_name})
             _validate_cache_name(cache_name)
             _validate_dictionary_name(dictionary_name)
 
-            request = _DictionarySetRequest()
-            request.dictionary_name = _as_bytes(dictionary_name, self.__UNSUPPORTED_DICTIONARY_NAME_TYPE_MSG)
-            for field, value in _gen_dictionary_items_as_bytes(items, self.__UNSUPPORTED_DICTIONARY_ITEMS_TYPE_MSG):
-                field_value_pair = _DictionaryFieldValuePair()
-                field_value_pair.field = field
-                field_value_pair.value = value
-                request.items.append(field_value_pair)
-            request.ttl_milliseconds = self._collection_ttl_or_default_milliseconds(ttl)
-            request.refresh_ttl = ttl.refresh_ttl
+            request = cache_pb._DictionarySetRequest(
+                dictionary_name=_as_bytes(dictionary_name, self.__UNSUPPORTED_DICTIONARY_NAME_TYPE_MSG),
+                items=[
+                    cache_pb._DictionaryFieldValuePair(field=field, value=value)
+                    for field, value in _gen_dictionary_items_as_bytes(
+                        items, self.__UNSUPPORTED_DICTIONARY_ITEMS_TYPE_MSG
+                    )
+                ],
+                **self._prepare_collection_ttl_for_request(ttl),
+            )
 
-            await self._build_stub().DictionarySet(
+            self._build_stub().DictionarySet(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("DictionarySet", {"dictionary_name": dictionary_name})
             return CacheDictionarySetFields.Success()
         except Exception as e:
             self._log_request_error("dictionary_set_fields", e)
             return CacheDictionarySetFields.Error(convert_error(e))
 
     # LIST COLLECTION METHODS
-    async def list_concatenate_back(
+    def list_concatenate_back(
         self,
         cache_name: TCacheName,
         list_name: TListName,
         values: TListValuesInput,
         ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
         truncate_front_to_size: Optional[int] = None,
     ) -> CacheListConcatenateBackResponse:
         try:
             self._log_issuing_request("ListConcatenateBack", {})
             _validate_cache_name(cache_name)
             _validate_list_name(list_name)
 
-            request = _ListConcatenateBackRequest()
-            request.list_name = _as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG)
-            request.values.extend(_gen_list_as_bytes(values, self.__UNSUPPORTED_LIST_VALUES_TYPE_MSG))
-            request.ttl_milliseconds = self._collection_ttl_or_default_milliseconds(ttl)
-            request.refresh_ttl = ttl.refresh_ttl
-            if truncate_front_to_size is not None:
-                request.truncate_front_to_size = truncate_front_to_size
+            request = cache_pb._ListConcatenateBackRequest(
+                list_name=_as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG),
+                values=_gen_list_as_bytes(values, self.__UNSUPPORTED_LIST_VALUES_TYPE_MSG),
+                truncate_front_to_size=truncate_front_to_size,
+                **self._prepare_collection_ttl_for_request(ttl),
+            )
 
-            response = await self._build_stub().ListConcatenateBack(
+            response = self._build_stub().ListConcatenateBack(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("ListConcatenateBack", {"list_name": str(request.list_name)})
             return CacheListConcatenateBack.Success(response.list_length)
         except Exception as e:
             self._log_request_error("list_concatenate_back", e)
             return CacheListConcatenateBack.Error(convert_error(e))
 
-    async def list_concatenate_front(
+    def list_concatenate_front(
         self,
         cache_name: TCacheName,
         list_name: TListName,
         values: TListValuesInput,
         ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
         truncate_back_to_size: Optional[int] = None,
     ) -> CacheListConcatenateFrontResponse:
         try:
             self._log_issuing_request("ListConcatenateFront", {})
             _validate_cache_name(cache_name)
             _validate_list_name(list_name)
 
-            request = _ListConcatenateFrontRequest()
-            request.list_name = _as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG)
-            request.values.extend(_gen_list_as_bytes(values, self.__UNSUPPORTED_LIST_VALUES_TYPE_MSG))
-            request.ttl_milliseconds = self._collection_ttl_or_default_milliseconds(ttl)
-            request.refresh_ttl = ttl.refresh_ttl
-            if truncate_back_to_size is not None:
-                request.truncate_back_to_size = truncate_back_to_size
+            request = cache_pb._ListConcatenateFrontRequest(
+                list_name=_as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG),
+                values=_gen_list_as_bytes(values, self.__UNSUPPORTED_LIST_VALUES_TYPE_MSG),
+                truncate_back_to_size=truncate_back_to_size,
+                **self._prepare_collection_ttl_for_request(ttl),
+            )
 
-            response = await self._build_stub().ListConcatenateFront(
+            response = self._build_stub().ListConcatenateFront(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("ListConcatenateFront", {"list_name": str(request.list_name)})
             return CacheListConcatenateFront.Success(response.list_length)
         except Exception as e:
             self._log_request_error("list_concatenate_front", e)
             return CacheListConcatenateFront.Error(convert_error(e))
 
-    async def list_fetch(self, cache_name: TCacheName, list_name: TListName) -> CacheListFetchResponse:
+    def list_fetch(self, cache_name: TCacheName, list_name: TListName) -> CacheListFetchResponse:
         try:
             self._log_issuing_request("ListFetch", {"list_name": str(list_name)})
             _validate_cache_name(cache_name)
             _validate_list_name(list_name)
-            request = _ListFetchRequest()
-            request.list_name = _as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG)
-            response = await self._build_stub().ListFetch(
+            request = cache_pb._ListFetchRequest(list_name=_as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG))
+            response = self._build_stub().ListFetch(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("ListFetch", {"list_name": str(request.list_name)})
 
             type = response.WhichOneof("list")
@@ -569,22 +531,21 @@
                 return CacheListFetch.Hit(list(response.found.values))
             else:
                 raise UnknownException("Unknown list field")
         except Exception as e:
             self._log_request_error("list_fetch", e)
             return CacheListFetch.Error(convert_error(e))
 
-    async def list_length(self, cache_name: TCacheName, list_name: TListName) -> CacheListLengthResponse:
+    def list_length(self, cache_name: TCacheName, list_name: TListName) -> CacheListLengthResponse:
         try:
             self._log_issuing_request("ListLength", {"list_name": str(list_name)})
             _validate_cache_name(cache_name)
             _validate_list_name(list_name)
-            request = _ListLengthRequest()
-            request.list_name = _as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG)
-            response = await self._build_stub().ListLength(
+            request = cache_pb._ListLengthRequest(list_name=_as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG))
+            response = self._build_stub().ListLength(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("ListLength", {"list_name": str(request.list_name)})
 
             type = response.WhichOneof("list")
@@ -594,22 +555,23 @@
                 return CacheListLength.Hit(response.found.length)
             else:
                 raise UnknownException("Unknown list field")
         except Exception as e:
             self._log_request_error("list_length", e)
             return CacheListLength.Error(convert_error(e))
 
-    async def list_pop_back(self, cache_name: TCacheName, list_name: TListName) -> CacheListPopBackResponse:
+    def list_pop_back(self, cache_name: TCacheName, list_name: TListName) -> CacheListPopBackResponse:
         try:
             self._log_issuing_request("ListPopBack", {"list_name": str(list_name)})
             _validate_cache_name(cache_name)
             _validate_list_name(list_name)
-            request = _ListPopBackRequest()
-            request.list_name = _as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG)
-            response = await self._build_stub().ListPopBack(
+            request = cache_pb._ListPopBackRequest(
+                list_name=_as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG)
+            )
+            response = self._build_stub().ListPopBack(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("ListPopBack", {"list_name": str(request.list_name)})
 
             type = response.WhichOneof("list")
@@ -619,22 +581,23 @@
                 return CacheListPopBack.Hit(response.found.back)
             else:
                 raise UnknownException("Unknown list field")
         except Exception as e:
             self._log_request_error("list_pop_back", e)
             return CacheListPopBack.Error(convert_error(e))
 
-    async def list_pop_front(self, cache_name: TCacheName, list_name: TListName) -> CacheListPopFrontResponse:
+    def list_pop_front(self, cache_name: TCacheName, list_name: TListName) -> CacheListPopFrontResponse:
         try:
             self._log_issuing_request("ListPopFront", {"list_name": str(list_name)})
             _validate_cache_name(cache_name)
             _validate_list_name(list_name)
-            request = _ListPopFrontRequest()
-            request.list_name = _as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG)
-            response = await self._build_stub().ListPopFront(
+            request = cache_pb._ListPopFrontRequest(
+                list_name=_as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG)
+            )
+            response = self._build_stub().ListPopFront(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("ListPopFront", {"list_name": str(request.list_name)})
 
             type = response.WhichOneof("list")
@@ -644,147 +607,145 @@
                 return CacheListPopFront.Hit(response.found.front)
             else:
                 raise UnknownException("Unknown list field")
         except Exception as e:
             self._log_request_error("list_pop_front", e)
             return CacheListPopFront.Error(convert_error(e))
 
-    async def list_push_back(
+    def list_push_back(
         self,
         cache_name: TCacheName,
         list_name: TListName,
         value: TListValue,
         ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
         truncate_front_to_size: Optional[int] = None,
     ) -> CacheListPushBackResponse:
         try:
             self._log_issuing_request("ListPushBack", {})
             _validate_cache_name(cache_name)
             _validate_list_name(list_name)
 
-            request = _ListPushBackRequest()
-            request.list_name = _as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG)
-            request.value = _as_bytes(value, self.__UNSUPPORTED_LIST_VALUE_TYPE_MSG)
-            request.ttl_milliseconds = self._collection_ttl_or_default_milliseconds(ttl)
-            request.refresh_ttl = ttl.refresh_ttl
-            if truncate_front_to_size is not None:
-                request.truncate_front_to_size = truncate_front_to_size
+            request = cache_pb._ListPushBackRequest(
+                list_name=_as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG),
+                value=_as_bytes(value, self.__UNSUPPORTED_LIST_VALUE_TYPE_MSG),
+                truncate_front_to_size=truncate_front_to_size,
+                **self._prepare_collection_ttl_for_request(ttl),
+            )
 
-            response = await self._build_stub().ListPushBack(
+            response = self._build_stub().ListPushBack(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("ListPushBack", {"list_name": str(request.list_name)})
             return CacheListPushBack.Success(response.list_length)
         except Exception as e:
             self._log_request_error("list_push_back", e)
             return CacheListPushBack.Error(convert_error(e))
 
-    async def list_push_front(
+    def list_push_front(
         self,
         cache_name: TCacheName,
         list_name: TListName,
         value: TListValue,
         ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
         truncate_back_to_size: Optional[int] = None,
     ) -> CacheListPushFrontResponse:
         try:
             self._log_issuing_request("ListPushFront", {})
             _validate_cache_name(cache_name)
             _validate_list_name(list_name)
 
-            request = _ListPushFrontRequest()
-            request.list_name = _as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG)
-            request.value = _as_bytes(value, self.__UNSUPPORTED_LIST_VALUE_TYPE_MSG)
-            request.ttl_milliseconds = self._collection_ttl_or_default_milliseconds(ttl)
-            request.refresh_ttl = ttl.refresh_ttl
-            if truncate_back_to_size is not None:
-                request.truncate_back_to_size = truncate_back_to_size
+            request = cache_pb._ListPushFrontRequest(
+                list_name=_as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG),
+                value=_as_bytes(value, self.__UNSUPPORTED_LIST_VALUE_TYPE_MSG),
+                truncate_back_to_size=truncate_back_to_size,
+                **self._prepare_collection_ttl_for_request(ttl),
+            )
 
-            response = await self._build_stub().ListPushFront(
+            response = self._build_stub().ListPushFront(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("ListPushFront", {"list_name": str(request.list_name)})
             return CacheListPushFront.Success(response.list_length)
         except Exception as e:
             self._log_request_error("list_push_front", e)
             return CacheListPushFront.Error(convert_error(e))
 
-    async def list_remove_value(
+    def list_remove_value(
         self,
         cache_name: TCacheName,
         list_name: TListName,
         value: TListValue,
     ) -> CacheListRemoveValueResponse:
         try:
             self._log_issuing_request("ListRemoveValue", {})
             _validate_cache_name(cache_name)
             _validate_list_name(list_name)
 
-            request = _ListRemoveRequest()
-            request.list_name = _as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG)
-            request.all_elements_with_value = _as_bytes(value, self.__UNSUPPORTED_LIST_VALUE_TYPE_MSG)
+            request = cache_pb._ListRemoveRequest(
+                list_name=_as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG),
+                all_elements_with_value=_as_bytes(value, self.__UNSUPPORTED_LIST_VALUE_TYPE_MSG),
+            )
 
-            await self._build_stub().ListRemove(
+            self._build_stub().ListRemove(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("ListRemoveValue", {"list_name": str(request.list_name)})
             return CacheListRemoveValue.Success()
         except Exception as e:
             self._log_request_error("list_remove_value", e)
             return CacheListRemoveValue.Error(convert_error(e))
 
     # SET COLLECTION METHODS
-    async def set_add_elements(
+    def set_add_elements(
         self,
         cache_name: TCacheName,
         set_name: TSetName,
         elements: TSetElementsInput,
         ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
     ) -> CacheSetAddElementsResponse:
         try:
             self._log_issuing_request("SetAddElements", {})
             _validate_cache_name(cache_name)
             _validate_set_name(set_name)
 
-            request = _SetUnionRequest()
-            request.set_name = _as_bytes(set_name, self.__UNSUPPORTED_SET_NAME_TYPE_MSG)
-            request.elements.extend(_gen_set_input_as_bytes(elements, self.__UNSUPPORTED_SET_ELEMENTS_TYPE_MSG))
-            request.ttl_milliseconds = self._collection_ttl_or_default_milliseconds(ttl)
-            request.refresh_ttl = ttl.refresh_ttl
+            request = cache_pb._SetUnionRequest(
+                set_name=_as_bytes(set_name, self.__UNSUPPORTED_SET_NAME_TYPE_MSG),
+                elements=_gen_set_input_as_bytes(elements, self.__UNSUPPORTED_SET_ELEMENTS_TYPE_MSG),
+                **self._prepare_collection_ttl_for_request(ttl),
+            )
 
-            await self._build_stub().SetUnion(
+            self._build_stub().SetUnion(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("SetAddElements", {"set_name": str(request.set_name)})
             return CacheSetAddElements.Success()
         except Exception as e:
             self._log_request_error("set_remove_elements", e)
             return CacheSetAddElements.Error(convert_error(e))
 
-    async def set_fetch(
+    def set_fetch(
         self,
         cache_name: TCacheName,
         set_name: TSetName,
     ) -> CacheSetFetchResponse:
         try:
             self._log_issuing_request("SetFetch", {"set_name": str(set_name)})
             _validate_cache_name(cache_name)
             _validate_set_name(set_name)
 
-            request = _SetFetchRequest()
-            request.set_name = _as_bytes(set_name, "Unsupported type for set_name: ")
-            response = await self._build_stub().SetFetch(
+            request = cache_pb._SetFetchRequest(set_name=_as_bytes(set_name, "Unsupported type for set_name: "))
+            response = self._build_stub().SetFetch(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("SetFetch", {"set_name": str(request.set_name)})
 
             type = response.WhichOneof("set")
@@ -794,121 +755,120 @@
                 return CacheSetFetch.Hit(set(response.found.elements))
             else:
                 raise UnknownException(f"Unknown set field in response: {type}")
         except Exception as e:
             self._log_request_error("set_fetch", e)
             return CacheSetFetch.Error(convert_error(e))
 
-    async def set_remove_elements(
+    def set_remove_elements(
         self, cache_name: TCacheName, set_name: TSetName, elements: TSetElementsInput
     ) -> CacheSetRemoveElementsResponse:
         try:
             self._log_issuing_request("SetRemoveElements", {})
             _validate_cache_name(cache_name)
             _validate_set_name(set_name)
 
-            request = _SetDifferenceRequest()
-            request.set_name = _as_bytes(set_name, self.__UNSUPPORTED_SET_NAME_TYPE_MSG)
-            request.subtrahend.set.elements.extend(
-                _gen_set_input_as_bytes(elements, self.__UNSUPPORTED_SET_ELEMENTS_TYPE_MSG)
+            request = cache_pb._SetDifferenceRequest(
+                set_name=_as_bytes(set_name, self.__UNSUPPORTED_SET_NAME_TYPE_MSG),
+                subtrahend=cache_pb._SetDifferenceRequest._Subtrahend(
+                    set=cache_pb._SetDifferenceRequest._Subtrahend._Set(
+                        elements=_gen_set_input_as_bytes(elements, self.__UNSUPPORTED_SET_ELEMENTS_TYPE_MSG)
+                    )
+                ),
             )
 
-            await self._build_stub().SetDifference(
+            self._build_stub().SetDifference(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("SetRemoveElements", {"set_name": str(request.set_name)})
             return CacheSetRemoveElements.Success()
         except Exception as e:
             self._log_request_error("set_remove_elements", e)
             return CacheSetRemoveElements.Error(convert_error(e))
 
-    async def sorted_set_put_elements(
+    def sorted_set_put_elements(
         self,
         cache_name: TCacheName,
         sorted_set_name: TSetName,
         elements: TSortedSetElements,
         ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
     ) -> CacheSortedSetPutElementsResponse:
         try:
             self._log_issuing_request("SortedSetPutElements", {})
             _validate_cache_name(cache_name)
             _validate_sorted_set_name(sorted_set_name)
 
-            request = _SortedSetPutRequest()
-            request.set_name = _as_bytes(sorted_set_name, self.__UNSUPPORTED_SORTED_SET_NAME_TYPE_MSG)
+            request = cache_pb._SortedSetPutRequest(
+                set_name=_as_bytes(sorted_set_name, self.__UNSUPPORTED_SORTED_SET_NAME_TYPE_MSG),
+                **self._prepare_collection_ttl_for_request(ttl),
+            )
             for value, score in _gen_sorted_set_elements_as_bytes(
                 elements, self.__UNSUPPORTED_SORTED_SET_ELEMENTS_TYPE_MSG
             ):
                 _validate_sorted_set_score(score)
-                element = _SortedSetElement()
-                element.value = value
-                element.score = score
-                request.elements.append(element)
-            request.ttl_milliseconds = self._collection_ttl_or_default_milliseconds(ttl)
-            request.refresh_ttl = ttl.refresh_ttl
+                request.elements.append(cache_pb._SortedSetElement(value=value, score=score))
 
-            await self._build_stub().SortedSetPut(
+            self._build_stub().SortedSetPut(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("SortedSetPutElements", {"sorted_set_name": str(request.set_name)})
             return CacheSortedSetPutElements.Success()
         except Exception as e:
             self._log_request_error("sorted_set_put_elements", e)
             return CacheSortedSetPutElements.Error(convert_error(e))
 
-    async def sorted_set_fetch_by_score(
+    def sorted_set_fetch_by_score(
         self,
         cache_name: TCacheName,
         sorted_set_name: TSortedSetName,
         min_score: Optional[float],
         max_score: Optional[float],
         sort_order: SortOrder,
         offset: Optional[int],
         count: Optional[int],
     ) -> CacheSortedSetFetchResponse:
         try:
             self._log_issuing_request("SortedSetFetch", {"sorted_set_name": str(sorted_set_name)})
             _validate_cache_name(cache_name)
             _validate_sorted_set_name(sorted_set_name)
 
-            request = _SortedSetFetchRequest()
-            request.set_name = _as_bytes(sorted_set_name, "Unsupported type for set_name: ")
-            request.with_scores = True
+            request = cache_pb._SortedSetFetchRequest(
+                set_name=_as_bytes(sorted_set_name, "Unsupported type for set_name: "), with_scores=True
+            )
 
             if min_score is not None:
-                request.by_score.min_score = min_score
+                request.by_score.min_score = cache_pb._SortedSetFetchRequest._ByScore._Score(score=min_score)
             else:
-                request.by_score.unbounded_min.CopyFrom(_Unbounded())
+                request.by_score.unbounded_min.CopyFrom(cache_pb._Unbounded())
 
             if max_score is not None:
-                request.by_score.max_score = max_score
+                request.by_score.max_score = cache_pb._SortedSetFetchRequest._ByScore._Score(score=max_score)
             else:
-                request.by_score.unbounded_max.CopyFrom(_Unbounded())
+                request.by_score.unbounded_max.CopyFrom(cache_pb._Unbounded())
 
             if offset is not None:
                 request.by_score.offset = offset
             else:
                 request.by_score.offset = 0
 
             if count is not None:
                 request.by_score.count = count
             else:
                 request.by_score.count = -1
 
-            # ascending = 0, descending = 1
             if sort_order == SortOrder.ASCENDING:
-                request.order = 0
+                request.order = cache_pb._SortedSetFetchRequest.ASCENDING
             else:
-                request.order = 1
+                request.order = cache_pb._SortedSetFetchRequest.DESCENDING
 
-            response = await self._build_stub().SortedSetFetch(
+            response = self._build_stub().SortedSetFetch(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("SortedSetFetch", {"sorted_set_name": str(request.set_name)})
 
             type = response.WhichOneof("sorted_set")
@@ -920,48 +880,47 @@
                 )
             else:
                 raise UnknownException(f"Unknown set field in response: {type}")
         except Exception as e:
             self._log_request_error("sorted_set_fetch", e)
             return CacheSortedSetFetch.Error(convert_error(e))
 
-    async def sorted_set_fetch_by_rank(
+    def sorted_set_fetch_by_rank(
         self,
         cache_name: TCacheName,
         sorted_set_name: TSortedSetName,
         start_rank: Optional[int],
         end_rank: Optional[int],
         sort_order: SortOrder,
     ) -> CacheSortedSetFetchResponse:
         try:
             self._log_issuing_request("SortedSetFetch", {"sorted_set_name": str(sorted_set_name)})
             _validate_cache_name(cache_name)
             _validate_sorted_set_name(sorted_set_name)
 
-            request = _SortedSetFetchRequest()
-            request.set_name = _as_bytes(sorted_set_name, "Unsupported type for set_name: ")
-            request.with_scores = True
+            request = cache_pb._SortedSetFetchRequest(
+                set_name=_as_bytes(sorted_set_name, "Unsupported type for set_name: "), with_scores=True
+            )
 
             if start_rank is not None:
                 request.by_index.inclusive_start_index = start_rank
             else:
-                request.by_index.unbounded_start.CopyFrom(_Unbounded())
+                request.by_index.unbounded_start.CopyFrom(cache_pb._Unbounded())
 
             if end_rank is not None:
                 request.by_index.exclusive_end_index = end_rank
             else:
-                request.by_index.unbounded_end.CopyFrom(_Unbounded())
+                request.by_index.unbounded_end.CopyFrom(cache_pb._Unbounded())
 
-            # ascending = 0, descending = 1
             if sort_order == SortOrder.ASCENDING:
-                request.order = 0
+                request.order = cache_pb._SortedSetFetchRequest.ASCENDING
             else:
-                request.order = 1
+                request.order = cache_pb._SortedSetFetchRequest.DESCENDING
 
-            response = await self._build_stub().SortedSetFetch(
+            response = self._build_stub().SortedSetFetch(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("SortedSetFetch", {"sorted_set_name": str(request.set_name)})
 
             type = response.WhichOneof("sorted_set")
@@ -973,142 +932,142 @@
                 )
             else:
                 raise UnknownException(f"Unknown set field in response: {type}")
         except Exception as e:
             self._log_request_error("sorted_set_fetch", e)
             return CacheSortedSetFetch.Error(convert_error(e))
 
-    async def sorted_set_get_scores(
+    def sorted_set_get_scores(
         self, cache_name: TCacheName, sorted_set_name: TSortedSetName, values: TSortedSetValues
     ) -> CacheSortedSetGetScoresResponse:
         try:
             self._log_issuing_request("SortedSetGetScores", {"sorted_set_name": str(sorted_set_name)})
             _validate_cache_name(cache_name)
             _validate_sorted_set_name(sorted_set_name)
 
-            request = _SortedSetGetScoreRequest()
-            request.set_name = _as_bytes(sorted_set_name, "Unsupported type for sorted_set_name: ")
-
             bytes_values = list(_gen_sorted_set_values_as_bytes(values, self.__UNSUPPORTED_SORTED_SET_VALUES_TYPE_MSG))
-            request.values.extend(bytes_values)
+            request = cache_pb._SortedSetGetScoreRequest(
+                set_name=_as_bytes(sorted_set_name, "Unsupported type for sorted_set_name: "), values=bytes_values
+            )
 
-            response = await self._build_stub().SortedSetGetScore(
+            response = self._build_stub().SortedSetGetScore(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("SortedSetGetScores", {"sorted_set_name": str(request.set_name)})
 
             type = response.WhichOneof("sorted_set")
             if type == "found":
                 get_responses: list[CacheSortedSetGetScoreResponse] = []
                 for value, get_response in zip(bytes_values, response.found.elements):
-                    if get_response.result == Miss:
+                    if get_response.result == cache_pb.Miss:
                         get_responses.append(CacheSortedSetGetScore.Miss(value))
                     else:
                         get_responses.append(CacheSortedSetGetScore.Hit(value, get_response.score))
                 return CacheSortedSetGetScores.Hit(get_responses)
             elif type == "missing":
                 return CacheSortedSetGetScores.Miss()
             else:
                 raise UnknownException(f"Unknown field in response: {type}")
         except Exception as e:
             self._log_request_error("sorted_set_get_scores", e)
             return CacheSortedSetGetScores.Error(convert_error(e))
 
-    async def sorted_set_get_rank(
+    def sorted_set_get_rank(
         self,
         cache_name: TCacheName,
         sorted_set_name: TSortedSetName,
         value: TSortedSetValue,
         sort_order: SortOrder,
     ) -> CacheSortedSetGetRankResponse:
         try:
             self._log_issuing_request("SortedSetGetRank", {"sorted_set_name": str(sorted_set_name)})
             _validate_cache_name(cache_name)
             _validate_sorted_set_name(sorted_set_name)
 
-            request = _SortedSetGetRankRequest()
-            request.set_name = _as_bytes(sorted_set_name, "Unsupported type for sorted_set_name: ")
-            request.value = _as_bytes(value, self.__UNSUPPORTED_SORTED_SET_VALUE_TYPE_MSG)
+            request = cache_pb._SortedSetGetRankRequest(
+                set_name=_as_bytes(sorted_set_name, "Unsupported type for sorted_set_name: "),
+                value=_as_bytes(value, self.__UNSUPPORTED_SORTED_SET_VALUE_TYPE_MSG),
+            )
 
-            # ascending = 0, descending = 1
             if sort_order == SortOrder.ASCENDING:
-                request.order = 0
+                request.order = cache_pb._SortedSetGetRankRequest.ASCENDING
             else:
-                request.order = 1
+                request.order = cache_pb._SortedSetGetRankRequest.DESCENDING
 
-            response = await self._build_stub().SortedSetGetRank(
+            response = self._build_stub().SortedSetGetRank(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("SortedSetGetRank", {"sorted_set_name": str(request.set_name)})
 
-            if response.element_rank.result == Hit:
+            if response.element_rank.result == cache_pb.Hit:
                 return CacheSortedSetGetRank.Hit(response.element_rank.rank)
-            if response.element_rank.result == Miss:
+            if response.element_rank.result == cache_pb.Miss:
                 return CacheSortedSetGetRank.Miss()
             else:
                 raise UnknownException(f"Unknown field in response: {type}")
         except Exception as e:
             self._log_request_error("sorted_set_get_rank", e)
             return CacheSortedSetGetRank.Error(convert_error(e))
 
-    async def sorted_set_remove_elements(
+    def sorted_set_remove_elements(
         self,
         cache_name: TCacheName,
         sorted_set_name: TSortedSetName,
         values: TSortedSetValues,
     ) -> CacheSortedSetRemoveElementsResponse:
         try:
             self._log_issuing_request("SortedSetRemoveElements", {"sorted_set_name": str(sorted_set_name)})
             _validate_cache_name(cache_name)
             _validate_sorted_set_name(sorted_set_name)
 
-            request = _SortedSetRemoveRequest()
-            request.set_name = _as_bytes(sorted_set_name, "Unsupported type for sorted_set_name: ")
-            request.some.values.extend(
-                _gen_sorted_set_values_as_bytes(values, self.__UNSUPPORTED_SORTED_SET_VALUES_TYPE_MSG)
+            request = cache_pb._SortedSetRemoveRequest(
+                set_name=_as_bytes(sorted_set_name, "Unsupported type for sorted_set_name: "),
+                some=cache_pb._SortedSetRemoveRequest._Some(
+                    values=_gen_sorted_set_values_as_bytes(values, self.__UNSUPPORTED_SORTED_SET_VALUES_TYPE_MSG)
+                ),
             )
 
-            await self._build_stub().SortedSetRemove(
+            self._build_stub().SortedSetRemove(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("SortedSetRemoveElements", {"sorted_set_name": str(request.set_name)})
 
             return CacheSortedSetRemoveElements.Success()
         except Exception as e:
             self._log_request_error("sorted_set_remove_elements", e)
             return CacheSortedSetRemoveElements.Error(convert_error(e))
 
-    async def sorted_set_increment(
+    def sorted_set_increment(
         self,
         cache_name: TCacheName,
         sorted_set_name: TSortedSetName,
         value: TSortedSetValue,
         score: TSortedSetScore,
         ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
     ) -> CacheSortedSetIncrementResponse:
         try:
             self._log_issuing_request("SortedSetIncrement", {"sorted_set_name": str(sorted_set_name)})
             _validate_cache_name(cache_name)
             _validate_sorted_set_name(sorted_set_name)
             _validate_sorted_set_score(score)
 
-            request = _SortedSetIncrementRequest()
-            request.set_name = _as_bytes(sorted_set_name, "Unsupported type for sorted_set_name: ")
-            request.value = _as_bytes(value)
-            request.amount = score
-            request.ttl_milliseconds = self._collection_ttl_or_default_milliseconds(ttl)
-            request.refresh_ttl = ttl.refresh_ttl
+            request = cache_pb._SortedSetIncrementRequest(
+                set_name=_as_bytes(sorted_set_name, "Unsupported type for sorted_set_name: "),
+                value=_as_bytes(value),
+                amount=score,
+                **self._prepare_collection_ttl_for_request(ttl),
+            )
 
-            response = await self._build_stub().SortedSetIncrement(
+            response = self._build_stub().SortedSetIncrement(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("SortedSetIncrement", {"sorted_set_name": str(request.set_name)})
 
             return CacheSortedSetIncrement.Success(response.score)
@@ -1121,22 +1080,36 @@
 
     def _log_issuing_request(self, request_type: str, request_args: dict[str, str]) -> None:
         self._logger.log(logs.TRACE, f"Issuing a {request_type} request with {request_args}")
 
     def _log_request_error(self, request_type: str, e: Exception) -> None:
         self._logger.warning(f"{request_type} failed with exception: {e}")
 
-    def _collection_ttl_or_default_milliseconds(self, collection_ttl: CollectionTtl) -> int:
-        return self._ttl_or_default_milliseconds(collection_ttl.ttl)
+    def _prepare_collection_ttl_for_request(self, collection_ttl: CollectionTtl) -> dict[str, Any]:  # type: ignore
+        """Converts a CollectionTtl object into a dictionary that can be used as kwargs for a request.
+
+        The TTL is converted to milliseconds, with a default of the client default TTL.
+        The refresh TTL is left as is.
+
+        Args:
+            collection_ttl (CollectionTtl): The CollectionTtl object to convert.
+
+        Returns:
+            dict[str, Any]: The dictionary that can be used as kwargs for a request.
+        """
+        return {
+            "ttl_milliseconds": self._ttl_or_default_milliseconds(collection_ttl.ttl),
+            "refresh_ttl": collection_ttl.refresh_ttl,
+        }
 
     def _ttl_or_default_milliseconds(self, ttl: Optional[timedelta]) -> int:
         which_ttl = self._default_ttl
         if ttl is not None:
             which_ttl = ttl
 
         return int(which_ttl.total_seconds() * 1000)
 
-    def _build_stub(self) -> ScsStub:
-        return self._grpc_manager.async_stub()
+    def _build_stub(self) -> cache_grpc.ScsStub:
+        return self._grpc_manager.stub()
 
-    async def close(self) -> None:
-        await self._grpc_manager.close()
+    def close(self) -> None:
+        self._grpc_manager.close()
```

### Comparing `momento-1.4.0/src/momento/internal/aio/_scs_grpc_manager.py` & `momento-1.5.0/src/momento/internal/aio/_scs_grpc_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import grpc
-import momento_wire_types.cacheclient_pb2_grpc as cache_client
-import momento_wire_types.controlclient_pb2_grpc as control_client
 import pkg_resources
+from momento_wire_types import cacheclient_pb2_grpc as cache_client
+from momento_wire_types import controlclient_pb2_grpc as control_client
 
 from momento.auth import CredentialProvider
 from momento.config import Configuration
 from momento.retry import RetryStrategy
 
 from ._add_header_client_interceptor import AddHeaderClientInterceptor, Header
 from ._retry_interceptor import RetryInterceptor
@@ -25,15 +25,15 @@
             interceptors=_interceptors(credential_provider.auth_token, configuration.get_retry_strategy()),
         )
 
     async def close(self) -> None:
         await self._secure_channel.close()
 
     def async_stub(self) -> control_client.ScsControlStub:
-        return control_client.ScsControlStub(self._secure_channel)
+        return control_client.ScsControlStub(self._secure_channel)  # type: ignore[no-untyped-call]
 
 
 class _DataGrpcManager:
     """Internal gRPC data mananger."""
 
     version = pkg_resources.get_distribution("momento").version
 
@@ -58,15 +58,15 @@
             ],
         )
 
     async def close(self) -> None:
         await self._secure_channel.close()
 
     def async_stub(self) -> cache_client.ScsStub:
-        return cache_client.ScsStub(self._secure_channel)
+        return cache_client.ScsStub(self._secure_channel)  # type: ignore[no-untyped-call]
 
 
 def _interceptors(auth_token: str, retry_strategy: RetryStrategy) -> list[grpc.aio.ClientInterceptor]:
     headers = [
         Header("authorization", auth_token),
         Header("agent", f"python:{_ControlGrpcManager.version}"),
     ]
```

### Comparing `momento-1.4.0/src/momento/internal/synchronous/_add_header_client_interceptor.py` & `momento-1.5.0/src/momento/internal/synchronous/_add_header_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/internal/synchronous/_retry_interceptor.py` & `momento-1.5.0/src/momento/internal/synchronous/_retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/internal/synchronous/_scs_control_client.py` & `momento-1.5.0/src/momento/internal/synchronous/_scs_control_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,12 @@
 from datetime import timedelta
 
 import grpc
-from momento_wire_types.controlclient_pb2 import (
-    _CreateCacheRequest,
-    _CreateSigningKeyRequest,
-    _DeleteCacheRequest,
-    _FlushCacheRequest,
-    _ListCachesRequest,
-    _ListSigningKeysRequest,
-    _RevokeSigningKeyRequest,
-)
-from momento_wire_types.controlclient_pb2_grpc import ScsControlStub
+from momento_wire_types import controlclient_pb2 as ctrl_pb
+from momento_wire_types import controlclient_pb2_grpc as ctrl_grpc
 
 from momento import logs
 from momento.auth import CredentialProvider
 from momento.config import Configuration
 from momento.errors import convert_error
 from momento.internal._utilities import _validate_cache_name, _validate_ttl
 from momento.internal.synchronous._scs_grpc_manager import _ControlGrpcManager
@@ -52,92 +44,85 @@
     def endpoint(self) -> str:
         return self._endpoint
 
     def create_cache(self, cache_name: str) -> CreateCacheResponse:
         try:
             self._logger.info(f"Creating cache with name: {cache_name}")
             _validate_cache_name(cache_name)
-            request = _CreateCacheRequest()
-            request.cache_name = cache_name
+            request = ctrl_pb._CreateCacheRequest(cache_name=cache_name)
             self._build_stub().CreateCache(request, timeout=_DEADLINE_SECONDS)
         except Exception as e:
             self._logger.debug("Failed to create cache: %s with exception: %s", cache_name, e)
             if isinstance(e, grpc.RpcError) and e.code() == grpc.StatusCode.ALREADY_EXISTS:
                 return CreateCache.CacheAlreadyExists()
             return CreateCache.Error(convert_error(e))
         return CreateCache.Success()
 
     def delete_cache(self, cache_name: str) -> DeleteCacheResponse:
         try:
             self._logger.info(f"Deleting cache with name: {cache_name}")
             _validate_cache_name(cache_name)
-            request = _DeleteCacheRequest()
-            request.cache_name = cache_name
+            request = ctrl_pb._DeleteCacheRequest(cache_name=cache_name)
             self._build_stub().DeleteCache(request, timeout=_DEADLINE_SECONDS)
         except Exception as e:
             self._logger.debug("Failed to delete cache: %s with exception: %s", cache_name, e)
             return DeleteCache.Error(convert_error(e))
         return DeleteCache.Success()
 
     def list_caches(self) -> ListCachesResponse:
         try:
-            list_caches_request = _ListCachesRequest()
-            list_caches_request.next_token = ""
+            list_caches_request = ctrl_pb._ListCachesRequest(next_token="")
             response = self._build_stub().ListCaches(list_caches_request, timeout=_DEADLINE_SECONDS)
             return ListCaches.Success.from_grpc_response(response)
         except Exception as e:
             return ListCaches.Error(convert_error(e))
 
     def flush(self, cache_name: str) -> CacheFlushResponse:
         try:
             _validate_cache_name(cache_name)
-            request = _FlushCacheRequest()
-            request.cache_name = cache_name
+            request = ctrl_pb._FlushCacheRequest(cache_name=cache_name)
             self._build_stub().FlushCache(request, timeout=_DEADLINE_SECONDS)
             return CacheFlush.Success()
         except Exception as e:
             return CacheFlush.Error(convert_error(e))
 
     def create_signing_key(self, ttl: timedelta, endpoint: str) -> CreateSigningKeyResponse:
         try:
             self._logger.info(f"Creating signing key with ttl={ttl!r} and endpoint={endpoint!r}")
             _validate_ttl(ttl)
             ttl_minutes = round(ttl.total_seconds() / 60)
             self._logger.info(f"Creating signing key with ttl (in minutes): {ttl_minutes}")
-            create_signing_key_request = _CreateSigningKeyRequest()
-            create_signing_key_request.ttl_minutes = ttl_minutes
+            create_signing_key_request = ctrl_pb._CreateSigningKeyRequest(ttl_minutes=ttl_minutes)
             response = self._build_stub().CreateSigningKey(create_signing_key_request, timeout=_DEADLINE_SECONDS)
             return CreateSigningKey.Success.from_grpc_response(response, endpoint)
         except Exception as e:
             self._logger.warning(f"Failed to create signing key with exception: {e}")
             return CreateSigningKey.Error(convert_error(e))
 
     def revoke_signing_key(self, key_id: str) -> RevokeSigningKeyResponse:
         try:
             self._logger.info(f"Revoking signing key with key_id {key_id}")
-            request = _RevokeSigningKeyRequest()
-            request.key_id = key_id
+            request = ctrl_pb._RevokeSigningKeyRequest(key_id=key_id)
             self._build_stub().RevokeSigningKey(request, timeout=_DEADLINE_SECONDS)
             return RevokeSigningKey.Success()
         except Exception as e:
             self._logger.warning(f"Failed to revoke signing key with key_id {key_id} exception: {e}")
             return RevokeSigningKey.Error(convert_error(e))
 
     def list_signing_keys(self, endpoint: str) -> ListSigningKeysResponse:
         try:
             self._logger.info("List signing keys")
-            list_signing_keys_request = _ListSigningKeysRequest()
-            list_signing_keys_request.next_token = ""
+            list_signing_keys_request = ctrl_pb._ListSigningKeysRequest(next_token="")
             response = self._build_stub().ListSigningKeys(list_signing_keys_request, timeout=_DEADLINE_SECONDS)
             return ListSigningKeys.Success.from_grpc_response(
                 response,
                 endpoint,
             )
         except Exception as e:
             self._logger.warning(f"Failed to list signing keys with exception: {e}")
             return ListSigningKeys.Error(convert_error(e))
 
-    def _build_stub(self) -> ScsControlStub:
+    def _build_stub(self) -> ctrl_grpc.ScsControlStub:
         return self._grpc_manager.stub()
 
     def close(self) -> None:
         self._grpc_manager.close()
```

### Comparing `momento-1.4.0/src/momento/internal/synchronous/_scs_data_client.py` & `momento-1.5.0/src/momento/internal/aio/_scs_data_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,14 @@
 from __future__ import annotations
 
 from datetime import timedelta
-from typing import Optional
+from typing import Any, Optional
 
-from momento_wire_types.cacheclient_pb2 import (
-    Hit,
-    Miss,
-    _DeleteRequest,
-    _DictionaryDeleteRequest,
-    _DictionaryFetchRequest,
-    _DictionaryFieldValuePair,
-    _DictionaryGetRequest,
-    _DictionaryIncrementRequest,
-    _DictionarySetRequest,
-    _GetRequest,
-    _IncrementRequest,
-    _ListConcatenateBackRequest,
-    _ListConcatenateFrontRequest,
-    _ListFetchRequest,
-    _ListLengthRequest,
-    _ListPopBackRequest,
-    _ListPopFrontRequest,
-    _ListPushBackRequest,
-    _ListPushFrontRequest,
-    _ListRemoveRequest,
-    _SetDifferenceRequest,
-    _SetFetchRequest,
-    _SetIfNotExistsRequest,
-    _SetRequest,
-    _SetUnionRequest,
-    _SortedSetElement,
-    _SortedSetFetchRequest,
-    _SortedSetGetRankRequest,
-    _SortedSetGetScoreRequest,
-    _SortedSetIncrementRequest,
-    _SortedSetPutRequest,
-    _SortedSetRemoveRequest,
-    _Unbounded,
-)
-from momento_wire_types.cacheclient_pb2_grpc import ScsStub
+from momento_wire_types import cacheclient_pb2 as cache_pb
+from momento_wire_types import cacheclient_pb2_grpc as cache_grpc
 
 from momento import logs
 from momento.auth import CredentialProvider
 from momento.config import Configuration
 from momento.errors import UnknownException, convert_error
 from momento.internal._utilities import (
     _as_bytes,
@@ -58,16 +24,16 @@
 )
 from momento.internal._utilities._data_validation import (
     _gen_sorted_set_elements_as_bytes,
     _gen_sorted_set_values_as_bytes,
     _validate_sorted_set_name,
     _validate_sorted_set_score,
 )
-from momento.internal.synchronous._scs_grpc_manager import _DataGrpcManager
-from momento.internal.synchronous._utilities import make_metadata
+from momento.internal.aio._scs_grpc_manager import _DataGrpcManager
+from momento.internal.aio._utilities import make_metadata
 from momento.requests import CollectionTtl, SortOrder
 from momento.responses import (
     CacheDelete,
     CacheDeleteResponse,
     CacheDictionaryFetch,
     CacheDictionaryFetchResponse,
     CacheDictionaryGetField,
@@ -194,79 +160,81 @@
         _validate_ttl(default_ttl)
         self._default_ttl = default_ttl
 
     @property
     def endpoint(self) -> str:
         return self._endpoint
 
-    def increment(
+    async def increment(
         self, cache_name: TCacheName, key: TScalarKey, amount: int = 1, ttl: Optional[timedelta] = None
     ) -> CacheIncrementResponse:
         try:
             self._log_issuing_request("Increment", {"key": str(key), "amount": str(amount)})
             _validate_cache_name(cache_name)
-            item_ttl = self._default_ttl if ttl is None else ttl
-            _validate_ttl(item_ttl)
+            _validate_ttl(ttl)
 
-            request = _IncrementRequest()
-            request.cache_key = _as_bytes(key, "Unsupported type for key: ")
-            request.amount = amount
-            request.ttl_milliseconds = int(item_ttl.total_seconds() * 1000)
+            request = cache_pb._IncrementRequest(
+                cache_key=_as_bytes(key, "Unsupported type for key: "),
+                amount=amount,
+                ttl_milliseconds=self._ttl_or_default_milliseconds(ttl),
+            )
 
-            response = self._build_stub().Increment(
+            response = await self._build_stub().Increment(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("Increment", {"key": str(key), "amount": str(amount)})
             return CacheIncrement.Success(response.value)
         except Exception as e:
             self._log_request_error("increment", e)
             return CacheIncrement.Error(convert_error(e))
 
-    def set(
+    async def set(
         self,
         cache_name: str,
         key: TScalarKey,
         value: TScalarValue,
         ttl: Optional[timedelta],
     ) -> CacheSetResponse:
         try:
             self._log_issuing_request("Set", {"key": str(key)})
             _validate_cache_name(cache_name)
-            item_ttl = self._default_ttl if ttl is None else ttl
-            _validate_ttl(item_ttl)
-            request = _SetRequest()
-            request.cache_key = _as_bytes(key, "Unsupported type for key: ")
-            request.cache_body = _as_bytes(value, "Unsupported type for value: ")
-            request.ttl_milliseconds = int(item_ttl.total_seconds() * 1000)
+            _validate_ttl(ttl)
+            request = cache_pb._SetRequest(
+                cache_key=_as_bytes(key, "Unsupported type for key: "),
+                cache_body=_as_bytes(value, "Unsupported type for value: "),
+                ttl_milliseconds=self._ttl_or_default_milliseconds(ttl),
+            )
 
-            self._build_stub().Set(request, metadata=make_metadata(cache_name), timeout=self._default_deadline_seconds)
+            await self._build_stub().Set(
+                request, metadata=make_metadata(cache_name), timeout=self._default_deadline_seconds
+            )
 
             self._log_received_response("Set", {"key": str(key)})
             return CacheSet.Success()
         except Exception as e:
             self._log_request_error("set", e)
             return CacheSet.Error(convert_error(e))
 
-    def set_if_not_exists(
+    async def set_if_not_exists(
         self, cache_name: TCacheName, key: TScalarKey, value: TScalarValue, ttl: Optional[timedelta]
     ) -> CacheSetIfNotExistsResponse:
         try:
             self._log_issuing_request("SetIfNotExists", {"key": str(key)})
 
             _validate_cache_name(cache_name)
-            item_ttl = self._default_ttl if ttl is None else ttl
-            _validate_ttl(item_ttl)
-            request = _SetIfNotExistsRequest()
-            request.cache_key = _as_bytes(key, "Unsupported type for key: ")
-            request.cache_body = _as_bytes(value, "Unsupported type for value: ")
-            request.ttl_milliseconds = int(item_ttl.total_seconds() * 1000)
+            _validate_ttl(ttl)
+            request = cache_pb._SetIfNotExistsRequest(
+                cache_key=_as_bytes(key, "Unsupported type for key: "),
+                cache_body=_as_bytes(value, "Unsupported type for value: "),
+                ttl_milliseconds=self._ttl_or_default_milliseconds(ttl),
+            )
 
-            response = self._build_stub().SetIfNotExists(
+            response = await self._build_stub().SetIfNotExists(
                 request, metadata=make_metadata(cache_name), timeout=self._default_deadline_seconds
             )
 
             self._log_received_response("SetIfNotExists", {"key": str(key)})
 
             result = response.WhichOneof("result")
             if result == "stored":
@@ -275,107 +243,106 @@
                 return CacheSetIfNotExists.NotStored()
             else:
                 raise UnknownException("SetIfNotExists responded with an unknown result")
         except Exception as e:
             self._log_request_error("set_if_not_exists", e)
             return CacheSetIfNotExists.Error(convert_error(e))
 
-    def get(self, cache_name: str, key: TScalarKey) -> CacheGetResponse:
+    async def get(self, cache_name: str, key: TScalarKey) -> CacheGetResponse:
         try:
             self._log_issuing_request("Get", {"key": str(key)})
 
             _validate_cache_name(cache_name)
-            request = _GetRequest()
-            request.cache_key = _as_bytes(key, "Unsupported type for key: ")
+            request = cache_pb._GetRequest(cache_key=_as_bytes(key, "Unsupported type for key: "))
 
-            response = self._build_stub().Get(
+            response = await self._build_stub().Get(
                 request, metadata=make_metadata(cache_name), timeout=self._default_deadline_seconds
             )
 
             self._log_received_response("Get", {"key": str(key)})
 
-            if response.result == Hit:
+            if response.result == cache_pb.Hit:
                 return CacheGet.Hit(response.cache_body)
-            elif response.result == Miss:
+            elif response.result == cache_pb.Miss:
                 return CacheGet.Miss()
             else:
                 raise UnknownException("Get responded with an unknown result")
         except Exception as e:
             self._log_request_error("set_if_not_exists", e)
             return CacheGet.Error(convert_error(e))
 
-    def delete(self, cache_name: str, key: TScalarKey) -> CacheDeleteResponse:
+    async def delete(self, cache_name: str, key: TScalarKey) -> CacheDeleteResponse:
         try:
             self._log_issuing_request("Delete", {"key": str(key)})
             _validate_cache_name(cache_name)
-            request = _DeleteRequest()
-            request.cache_key = _as_bytes(key, "Unsupported type for key: ")
+            request = cache_pb._DeleteRequest(cache_key=_as_bytes(key, "Unsupported type for key: "))
 
-            self._build_stub().Delete(
+            await self._build_stub().Delete(
                 request, metadata=make_metadata(cache_name), timeout=self._default_deadline_seconds
             )
 
             self._log_received_response("Delete", {"key": str(key)})
             return CacheDelete.Success()
         except Exception as e:
             self._log_request_error("set", e)
             return CacheDelete.Error(convert_error(e))
 
     # DICTIONARY COLLECTION METHODS
-    def dictionary_get_fields(
+    async def dictionary_get_fields(
         self,
         cache_name: TCacheName,
         dictionary_name: TDictionaryName,
         fields: TDictionaryFields,
     ) -> CacheDictionaryGetFieldsResponse:
         try:
             self._log_issuing_request("DictionaryGet", {"dictionary_name": dictionary_name})
             _validate_cache_name(cache_name)
             _validate_dictionary_name(dictionary_name)
 
-            request = _DictionaryGetRequest()
-            request.dictionary_name = _as_bytes(dictionary_name, self.__UNSUPPORTED_DICTIONARY_NAME_TYPE_MSG)
             bytes_fields = list(_gen_dictionary_fields_as_bytes(fields, self.__UNSUPPORTED_DICTIONARY_FIELDS_TYPE_MSG))
+            request = cache_pb._DictionaryGetRequest(
+                dictionary_name=_as_bytes(dictionary_name, self.__UNSUPPORTED_DICTIONARY_NAME_TYPE_MSG),
+                fields=bytes_fields,
+            )
 
-            request.fields.extend(bytes_fields)
-
-            response = self._build_stub().DictionaryGet(
+            response = await self._build_stub().DictionaryGet(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("DictionaryGet", {"dictionary_name": dictionary_name})
 
             type = response.WhichOneof("dictionary")
             if type == "found":
                 get_responses: list[CacheDictionaryGetFieldResponse] = []
                 for field, get_response in zip(bytes_fields, response.found.items):
-                    if get_response.result == Miss:
+                    if get_response.result == cache_pb.Miss:
                         get_responses.append(CacheDictionaryGetField.Miss())
                     else:
                         get_responses.append(CacheDictionaryGetField.Hit(get_response.cache_body, field))
                 return CacheDictionaryGetFields.Hit(get_responses)
             elif type == "missing":
                 return CacheDictionaryGetFields.Miss()
             else:
                 raise UnknownException("Unknown dictionary field")
         except Exception as e:
             self._log_request_error("dictionary_get_fields", e)
             return CacheDictionaryGetFields.Error(convert_error(e))
 
-    def dictionary_fetch(
+    async def dictionary_fetch(
         self, cache_name: TCacheName, dictionary_name: TDictionaryName
     ) -> CacheDictionaryFetchResponse:
         try:
             self._log_issuing_request("DictionaryFetch", {"dictionary_name": dictionary_name})
             _validate_cache_name(cache_name)
             _validate_dictionary_name(dictionary_name)
-            request = _DictionaryFetchRequest()
-            request.dictionary_name = _as_bytes(dictionary_name, self.__UNSUPPORTED_DICTIONARY_NAME_TYPE_MSG)
-            response = self._build_stub().DictionaryFetch(
+            request = cache_pb._DictionaryFetchRequest(
+                dictionary_name=_as_bytes(dictionary_name, self.__UNSUPPORTED_DICTIONARY_NAME_TYPE_MSG)
+            )
+            response = await self._build_stub().DictionaryFetch(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("DictionaryFetch", {"dictionary_name": dictionary_name})
 
             type = response.WhichOneof("dictionary")
@@ -385,179 +352,178 @@
                 return CacheDictionaryFetch.Hit({item.field: item.value for item in response.found.items})
             else:
                 raise UnknownException("Unknown dictionary field")
         except Exception as e:
             self._log_request_error("dictionary_fetch", e)
             return CacheDictionaryFetch.Error(convert_error(e))
 
-    def dictionary_increment(
+    async def dictionary_increment(
         self,
         cache_name: TCacheName,
         dictionary_name: TDictionaryName,
         field: TDictionaryField,
         amount: int = 1,
         ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
     ) -> CacheDictionaryIncrementResponse:
         try:
             self._log_issuing_request("DictionaryIncrement", {"dictionary_name": dictionary_name})
             _validate_cache_name(cache_name)
             _validate_dictionary_name(dictionary_name)
 
-            request = _DictionaryIncrementRequest()
-            request.dictionary_name = _as_bytes(dictionary_name, self.__UNSUPPORTED_DICTIONARY_NAME_TYPE_MSG)
-            request.field = _as_bytes(field, self.__UNSUPPORTED_DICTIONARY_FIELD_TYPE_MSG)
-            request.amount = amount
-            request.ttl_milliseconds = self._collection_ttl_or_default_milliseconds(ttl)
-            request.refresh_ttl = ttl.refresh_ttl
+            request = cache_pb._DictionaryIncrementRequest(
+                dictionary_name=_as_bytes(dictionary_name, self.__UNSUPPORTED_DICTIONARY_NAME_TYPE_MSG),
+                field=_as_bytes(field, self.__UNSUPPORTED_DICTIONARY_FIELD_TYPE_MSG),
+                amount=amount,
+                **self._prepare_collection_ttl_for_request(ttl),
+            )
 
-            response = self._build_stub().DictionaryIncrement(
+            response = await self._build_stub().DictionaryIncrement(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("DictionaryIncrement", {"dictionary_name": dictionary_name})
             return CacheDictionaryIncrement.Success(response.value)
         except Exception as e:
             self._log_request_error("dictionary_increment", e)
             return CacheDictionaryIncrement.Error(convert_error(e))
 
-    def dictionary_remove_fields(
+    async def dictionary_remove_fields(
         self,
         cache_name: TCacheName,
         dictionary_name: TDictionaryName,
         fields: TDictionaryFields,
     ) -> CacheDictionaryRemoveFieldsResponse:
         try:
             self._log_issuing_request("DictionaryDelete", {"dictionary_name": dictionary_name})
             _validate_cache_name(cache_name)
             _validate_dictionary_name(dictionary_name)
 
-            request = _DictionaryDeleteRequest()
-            request.dictionary_name = _as_bytes(dictionary_name, self.__UNSUPPORTED_DICTIONARY_NAME_TYPE_MSG)
-            request.some.fields.extend(
-                _gen_dictionary_fields_as_bytes(fields, self.__UNSUPPORTED_DICTIONARY_FIELDS_TYPE_MSG)
+            request = cache_pb._DictionaryDeleteRequest(
+                dictionary_name=_as_bytes(dictionary_name, self.__UNSUPPORTED_DICTIONARY_NAME_TYPE_MSG),
+                some=cache_pb._DictionaryDeleteRequest.Some(
+                    fields=_gen_dictionary_fields_as_bytes(fields, self.__UNSUPPORTED_DICTIONARY_FIELDS_TYPE_MSG)
+                ),
             )
 
-            self._build_stub().DictionaryDelete(
+            await self._build_stub().DictionaryDelete(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("DictionaryDelete", {"dictionary_name": dictionary_name})
             return CacheDictionaryRemoveFields.Success()
         except Exception as e:
             self._log_request_error("dictionary_remove_fields", e)
             return CacheDictionaryRemoveFields.Error(convert_error(e))
 
-    def dictionary_set_fields(
+    async def dictionary_set_fields(
         self,
         cache_name: TCacheName,
         dictionary_name: TDictionaryName,
         items: TDictionaryItems,
         ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
     ) -> CacheDictionarySetFieldsResponse:
         try:
             self._log_issuing_request("DictionarySet", {"dictionary_name": dictionary_name})
             _validate_cache_name(cache_name)
             _validate_dictionary_name(dictionary_name)
 
-            request = _DictionarySetRequest()
-            request.dictionary_name = _as_bytes(dictionary_name, self.__UNSUPPORTED_DICTIONARY_NAME_TYPE_MSG)
-            for field, value in _gen_dictionary_items_as_bytes(items, self.__UNSUPPORTED_DICTIONARY_ITEMS_TYPE_MSG):
-                field_value_pair = _DictionaryFieldValuePair()
-                field_value_pair.field = field
-                field_value_pair.value = value
-                request.items.append(field_value_pair)
-            request.ttl_milliseconds = self._collection_ttl_or_default_milliseconds(ttl)
-            request.refresh_ttl = ttl.refresh_ttl
+            request = cache_pb._DictionarySetRequest(
+                dictionary_name=_as_bytes(dictionary_name, self.__UNSUPPORTED_DICTIONARY_NAME_TYPE_MSG),
+                items=[
+                    cache_pb._DictionaryFieldValuePair(field=field, value=value)
+                    for field, value in _gen_dictionary_items_as_bytes(
+                        items, self.__UNSUPPORTED_DICTIONARY_ITEMS_TYPE_MSG
+                    )
+                ],
+                **self._prepare_collection_ttl_for_request(ttl),
+            )
 
-            self._build_stub().DictionarySet(
+            await self._build_stub().DictionarySet(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("DictionarySet", {"dictionary_name": dictionary_name})
             return CacheDictionarySetFields.Success()
         except Exception as e:
             self._log_request_error("dictionary_set_fields", e)
             return CacheDictionarySetFields.Error(convert_error(e))
 
     # LIST COLLECTION METHODS
-    def list_concatenate_back(
+    async def list_concatenate_back(
         self,
         cache_name: TCacheName,
         list_name: TListName,
         values: TListValuesInput,
         ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
         truncate_front_to_size: Optional[int] = None,
     ) -> CacheListConcatenateBackResponse:
         try:
             self._log_issuing_request("ListConcatenateBack", {})
             _validate_cache_name(cache_name)
             _validate_list_name(list_name)
 
-            request = _ListConcatenateBackRequest()
-            request.list_name = _as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG)
-            request.values.extend(_gen_list_as_bytes(values, self.__UNSUPPORTED_LIST_VALUES_TYPE_MSG))
-            request.ttl_milliseconds = self._collection_ttl_or_default_milliseconds(ttl)
-            request.refresh_ttl = ttl.refresh_ttl
-            if truncate_front_to_size is not None:
-                request.truncate_front_to_size = truncate_front_to_size
+            request = cache_pb._ListConcatenateBackRequest(
+                list_name=_as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG),
+                values=_gen_list_as_bytes(values, self.__UNSUPPORTED_LIST_VALUES_TYPE_MSG),
+                truncate_front_to_size=truncate_front_to_size,
+                **self._prepare_collection_ttl_for_request(ttl),
+            )
 
-            response = self._build_stub().ListConcatenateBack(
+            response = await self._build_stub().ListConcatenateBack(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("ListConcatenateBack", {"list_name": str(request.list_name)})
             return CacheListConcatenateBack.Success(response.list_length)
         except Exception as e:
             self._log_request_error("list_concatenate_back", e)
             return CacheListConcatenateBack.Error(convert_error(e))
 
-    def list_concatenate_front(
+    async def list_concatenate_front(
         self,
         cache_name: TCacheName,
         list_name: TListName,
         values: TListValuesInput,
         ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
         truncate_back_to_size: Optional[int] = None,
     ) -> CacheListConcatenateFrontResponse:
         try:
             self._log_issuing_request("ListConcatenateFront", {})
             _validate_cache_name(cache_name)
             _validate_list_name(list_name)
 
-            request = _ListConcatenateFrontRequest()
-            request.list_name = _as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG)
-            request.values.extend(_gen_list_as_bytes(values, self.__UNSUPPORTED_LIST_VALUES_TYPE_MSG))
-            request.ttl_milliseconds = self._collection_ttl_or_default_milliseconds(ttl)
-            request.refresh_ttl = ttl.refresh_ttl
-            if truncate_back_to_size is not None:
-                request.truncate_back_to_size = truncate_back_to_size
+            request = cache_pb._ListConcatenateFrontRequest(
+                list_name=_as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG),
+                values=_gen_list_as_bytes(values, self.__UNSUPPORTED_LIST_VALUES_TYPE_MSG),
+                truncate_back_to_size=truncate_back_to_size,
+                **self._prepare_collection_ttl_for_request(ttl),
+            )
 
-            response = self._build_stub().ListConcatenateFront(
+            response = await self._build_stub().ListConcatenateFront(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("ListConcatenateFront", {"list_name": str(request.list_name)})
             return CacheListConcatenateFront.Success(response.list_length)
         except Exception as e:
             self._log_request_error("list_concatenate_front", e)
             return CacheListConcatenateFront.Error(convert_error(e))
 
-    def list_fetch(self, cache_name: TCacheName, list_name: TListName) -> CacheListFetchResponse:
+    async def list_fetch(self, cache_name: TCacheName, list_name: TListName) -> CacheListFetchResponse:
         try:
             self._log_issuing_request("ListFetch", {"list_name": str(list_name)})
             _validate_cache_name(cache_name)
             _validate_list_name(list_name)
-            request = _ListFetchRequest()
-            request.list_name = _as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG)
-            response = self._build_stub().ListFetch(
+            request = cache_pb._ListFetchRequest(list_name=_as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG))
+            response = await self._build_stub().ListFetch(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("ListFetch", {"list_name": str(request.list_name)})
 
             type = response.WhichOneof("list")
@@ -567,22 +533,21 @@
                 return CacheListFetch.Hit(list(response.found.values))
             else:
                 raise UnknownException("Unknown list field")
         except Exception as e:
             self._log_request_error("list_fetch", e)
             return CacheListFetch.Error(convert_error(e))
 
-    def list_length(self, cache_name: TCacheName, list_name: TListName) -> CacheListLengthResponse:
+    async def list_length(self, cache_name: TCacheName, list_name: TListName) -> CacheListLengthResponse:
         try:
             self._log_issuing_request("ListLength", {"list_name": str(list_name)})
             _validate_cache_name(cache_name)
             _validate_list_name(list_name)
-            request = _ListLengthRequest()
-            request.list_name = _as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG)
-            response = self._build_stub().ListLength(
+            request = cache_pb._ListLengthRequest(list_name=_as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG))
+            response = await self._build_stub().ListLength(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("ListLength", {"list_name": str(request.list_name)})
 
             type = response.WhichOneof("list")
@@ -592,22 +557,23 @@
                 return CacheListLength.Hit(response.found.length)
             else:
                 raise UnknownException("Unknown list field")
         except Exception as e:
             self._log_request_error("list_length", e)
             return CacheListLength.Error(convert_error(e))
 
-    def list_pop_back(self, cache_name: TCacheName, list_name: TListName) -> CacheListPopBackResponse:
+    async def list_pop_back(self, cache_name: TCacheName, list_name: TListName) -> CacheListPopBackResponse:
         try:
             self._log_issuing_request("ListPopBack", {"list_name": str(list_name)})
             _validate_cache_name(cache_name)
             _validate_list_name(list_name)
-            request = _ListPopBackRequest()
-            request.list_name = _as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG)
-            response = self._build_stub().ListPopBack(
+            request = cache_pb._ListPopBackRequest(
+                list_name=_as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG)
+            )
+            response = await self._build_stub().ListPopBack(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("ListPopBack", {"list_name": str(request.list_name)})
 
             type = response.WhichOneof("list")
@@ -617,22 +583,23 @@
                 return CacheListPopBack.Hit(response.found.back)
             else:
                 raise UnknownException("Unknown list field")
         except Exception as e:
             self._log_request_error("list_pop_back", e)
             return CacheListPopBack.Error(convert_error(e))
 
-    def list_pop_front(self, cache_name: TCacheName, list_name: TListName) -> CacheListPopFrontResponse:
+    async def list_pop_front(self, cache_name: TCacheName, list_name: TListName) -> CacheListPopFrontResponse:
         try:
             self._log_issuing_request("ListPopFront", {"list_name": str(list_name)})
             _validate_cache_name(cache_name)
             _validate_list_name(list_name)
-            request = _ListPopFrontRequest()
-            request.list_name = _as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG)
-            response = self._build_stub().ListPopFront(
+            request = cache_pb._ListPopFrontRequest(
+                list_name=_as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG)
+            )
+            response = await self._build_stub().ListPopFront(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("ListPopFront", {"list_name": str(request.list_name)})
 
             type = response.WhichOneof("list")
@@ -642,147 +609,145 @@
                 return CacheListPopFront.Hit(response.found.front)
             else:
                 raise UnknownException("Unknown list field")
         except Exception as e:
             self._log_request_error("list_pop_front", e)
             return CacheListPopFront.Error(convert_error(e))
 
-    def list_push_back(
+    async def list_push_back(
         self,
         cache_name: TCacheName,
         list_name: TListName,
         value: TListValue,
         ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
         truncate_front_to_size: Optional[int] = None,
     ) -> CacheListPushBackResponse:
         try:
             self._log_issuing_request("ListPushBack", {})
             _validate_cache_name(cache_name)
             _validate_list_name(list_name)
 
-            request = _ListPushBackRequest()
-            request.list_name = _as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG)
-            request.value = _as_bytes(value, self.__UNSUPPORTED_LIST_VALUE_TYPE_MSG)
-            request.ttl_milliseconds = self._collection_ttl_or_default_milliseconds(ttl)
-            request.refresh_ttl = ttl.refresh_ttl
-            if truncate_front_to_size is not None:
-                request.truncate_front_to_size = truncate_front_to_size
+            request = cache_pb._ListPushBackRequest(
+                list_name=_as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG),
+                value=_as_bytes(value, self.__UNSUPPORTED_LIST_VALUE_TYPE_MSG),
+                truncate_front_to_size=truncate_front_to_size,
+                **self._prepare_collection_ttl_for_request(ttl),
+            )
 
-            response = self._build_stub().ListPushBack(
+            response = await self._build_stub().ListPushBack(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("ListPushBack", {"list_name": str(request.list_name)})
             return CacheListPushBack.Success(response.list_length)
         except Exception as e:
             self._log_request_error("list_push_back", e)
             return CacheListPushBack.Error(convert_error(e))
 
-    def list_push_front(
+    async def list_push_front(
         self,
         cache_name: TCacheName,
         list_name: TListName,
         value: TListValue,
         ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
         truncate_back_to_size: Optional[int] = None,
     ) -> CacheListPushFrontResponse:
         try:
             self._log_issuing_request("ListPushFront", {})
             _validate_cache_name(cache_name)
             _validate_list_name(list_name)
 
-            request = _ListPushFrontRequest()
-            request.list_name = _as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG)
-            request.value = _as_bytes(value, self.__UNSUPPORTED_LIST_VALUE_TYPE_MSG)
-            request.ttl_milliseconds = self._collection_ttl_or_default_milliseconds(ttl)
-            request.refresh_ttl = ttl.refresh_ttl
-            if truncate_back_to_size is not None:
-                request.truncate_back_to_size = truncate_back_to_size
+            request = cache_pb._ListPushFrontRequest(
+                list_name=_as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG),
+                value=_as_bytes(value, self.__UNSUPPORTED_LIST_VALUE_TYPE_MSG),
+                truncate_back_to_size=truncate_back_to_size,
+                **self._prepare_collection_ttl_for_request(ttl),
+            )
 
-            response = self._build_stub().ListPushFront(
+            response = await self._build_stub().ListPushFront(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("ListPushFront", {"list_name": str(request.list_name)})
             return CacheListPushFront.Success(response.list_length)
         except Exception as e:
             self._log_request_error("list_push_front", e)
             return CacheListPushFront.Error(convert_error(e))
 
-    def list_remove_value(
+    async def list_remove_value(
         self,
         cache_name: TCacheName,
         list_name: TListName,
         value: TListValue,
     ) -> CacheListRemoveValueResponse:
         try:
             self._log_issuing_request("ListRemoveValue", {})
             _validate_cache_name(cache_name)
             _validate_list_name(list_name)
 
-            request = _ListRemoveRequest()
-            request.list_name = _as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG)
-            request.all_elements_with_value = _as_bytes(value, self.__UNSUPPORTED_LIST_VALUE_TYPE_MSG)
+            request = cache_pb._ListRemoveRequest(
+                list_name=_as_bytes(list_name, self.__UNSUPPORTED_LIST_NAME_TYPE_MSG),
+                all_elements_with_value=_as_bytes(value, self.__UNSUPPORTED_LIST_VALUE_TYPE_MSG),
+            )
 
-            self._build_stub().ListRemove(
+            await self._build_stub().ListRemove(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("ListRemoveValue", {"list_name": str(request.list_name)})
             return CacheListRemoveValue.Success()
         except Exception as e:
             self._log_request_error("list_remove_value", e)
             return CacheListRemoveValue.Error(convert_error(e))
 
     # SET COLLECTION METHODS
-    def set_add_elements(
+    async def set_add_elements(
         self,
         cache_name: TCacheName,
         set_name: TSetName,
         elements: TSetElementsInput,
         ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
     ) -> CacheSetAddElementsResponse:
         try:
             self._log_issuing_request("SetAddElements", {})
             _validate_cache_name(cache_name)
             _validate_set_name(set_name)
 
-            request = _SetUnionRequest()
-            request.set_name = _as_bytes(set_name, self.__UNSUPPORTED_SET_NAME_TYPE_MSG)
-            request.elements.extend(_gen_set_input_as_bytes(elements, self.__UNSUPPORTED_SET_ELEMENTS_TYPE_MSG))
-            request.ttl_milliseconds = self._collection_ttl_or_default_milliseconds(ttl)
-            request.refresh_ttl = ttl.refresh_ttl
+            request = cache_pb._SetUnionRequest(
+                set_name=_as_bytes(set_name, self.__UNSUPPORTED_SET_NAME_TYPE_MSG),
+                elements=_gen_set_input_as_bytes(elements, self.__UNSUPPORTED_SET_ELEMENTS_TYPE_MSG),
+                **self._prepare_collection_ttl_for_request(ttl),
+            )
 
-            self._build_stub().SetUnion(
+            await self._build_stub().SetUnion(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("SetAddElements", {"set_name": str(request.set_name)})
             return CacheSetAddElements.Success()
         except Exception as e:
             self._log_request_error("set_remove_elements", e)
             return CacheSetAddElements.Error(convert_error(e))
 
-    def set_fetch(
+    async def set_fetch(
         self,
         cache_name: TCacheName,
         set_name: TSetName,
     ) -> CacheSetFetchResponse:
         try:
             self._log_issuing_request("SetFetch", {"set_name": str(set_name)})
             _validate_cache_name(cache_name)
             _validate_set_name(set_name)
 
-            request = _SetFetchRequest()
-            request.set_name = _as_bytes(set_name, "Unsupported type for set_name: ")
-            response = self._build_stub().SetFetch(
+            request = cache_pb._SetFetchRequest(set_name=_as_bytes(set_name, "Unsupported type for set_name: "))
+            response = await self._build_stub().SetFetch(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("SetFetch", {"set_name": str(request.set_name)})
 
             type = response.WhichOneof("set")
@@ -792,121 +757,120 @@
                 return CacheSetFetch.Hit(set(response.found.elements))
             else:
                 raise UnknownException(f"Unknown set field in response: {type}")
         except Exception as e:
             self._log_request_error("set_fetch", e)
             return CacheSetFetch.Error(convert_error(e))
 
-    def set_remove_elements(
+    async def set_remove_elements(
         self, cache_name: TCacheName, set_name: TSetName, elements: TSetElementsInput
     ) -> CacheSetRemoveElementsResponse:
         try:
             self._log_issuing_request("SetRemoveElements", {})
             _validate_cache_name(cache_name)
             _validate_set_name(set_name)
 
-            request = _SetDifferenceRequest()
-            request.set_name = _as_bytes(set_name, self.__UNSUPPORTED_SET_NAME_TYPE_MSG)
-            request.subtrahend.set.elements.extend(
-                _gen_set_input_as_bytes(elements, self.__UNSUPPORTED_SET_ELEMENTS_TYPE_MSG)
+            request = cache_pb._SetDifferenceRequest(
+                set_name=_as_bytes(set_name, self.__UNSUPPORTED_SET_NAME_TYPE_MSG),
+                subtrahend=cache_pb._SetDifferenceRequest._Subtrahend(
+                    set=cache_pb._SetDifferenceRequest._Subtrahend._Set(
+                        elements=_gen_set_input_as_bytes(elements, self.__UNSUPPORTED_SET_ELEMENTS_TYPE_MSG)
+                    )
+                ),
             )
 
-            self._build_stub().SetDifference(
+            await self._build_stub().SetDifference(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("SetRemoveElements", {"set_name": str(request.set_name)})
             return CacheSetRemoveElements.Success()
         except Exception as e:
             self._log_request_error("set_remove_elements", e)
             return CacheSetRemoveElements.Error(convert_error(e))
 
-    def sorted_set_put_elements(
+    async def sorted_set_put_elements(
         self,
         cache_name: TCacheName,
         sorted_set_name: TSetName,
         elements: TSortedSetElements,
         ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
     ) -> CacheSortedSetPutElementsResponse:
         try:
             self._log_issuing_request("SortedSetPutElements", {})
             _validate_cache_name(cache_name)
             _validate_sorted_set_name(sorted_set_name)
 
-            request = _SortedSetPutRequest()
-            request.set_name = _as_bytes(sorted_set_name, self.__UNSUPPORTED_SORTED_SET_NAME_TYPE_MSG)
+            request = cache_pb._SortedSetPutRequest(
+                set_name=_as_bytes(sorted_set_name, self.__UNSUPPORTED_SORTED_SET_NAME_TYPE_MSG),
+                **self._prepare_collection_ttl_for_request(ttl),
+            )
             for value, score in _gen_sorted_set_elements_as_bytes(
                 elements, self.__UNSUPPORTED_SORTED_SET_ELEMENTS_TYPE_MSG
             ):
                 _validate_sorted_set_score(score)
-                element = _SortedSetElement()
-                element.value = value
-                element.score = score
-                request.elements.append(element)
-            request.ttl_milliseconds = self._collection_ttl_or_default_milliseconds(ttl)
-            request.refresh_ttl = ttl.refresh_ttl
+                request.elements.append(cache_pb._SortedSetElement(value=value, score=score))
 
-            self._build_stub().SortedSetPut(
+            await self._build_stub().SortedSetPut(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("SortedSetPutElements", {"sorted_set_name": str(request.set_name)})
             return CacheSortedSetPutElements.Success()
         except Exception as e:
             self._log_request_error("sorted_set_put_elements", e)
             return CacheSortedSetPutElements.Error(convert_error(e))
 
-    def sorted_set_fetch_by_score(
+    async def sorted_set_fetch_by_score(
         self,
         cache_name: TCacheName,
         sorted_set_name: TSortedSetName,
         min_score: Optional[float],
         max_score: Optional[float],
         sort_order: SortOrder,
         offset: Optional[int],
         count: Optional[int],
     ) -> CacheSortedSetFetchResponse:
         try:
             self._log_issuing_request("SortedSetFetch", {"sorted_set_name": str(sorted_set_name)})
             _validate_cache_name(cache_name)
             _validate_sorted_set_name(sorted_set_name)
 
-            request = _SortedSetFetchRequest()
-            request.set_name = _as_bytes(sorted_set_name, "Unsupported type for set_name: ")
-            request.with_scores = True
+            request = cache_pb._SortedSetFetchRequest(
+                set_name=_as_bytes(sorted_set_name, "Unsupported type for set_name: "), with_scores=True
+            )
 
             if min_score is not None:
-                request.by_score.min_score = min_score
+                request.by_score.min_score = cache_pb._SortedSetFetchRequest._ByScore._Score(score=min_score)
             else:
-                request.by_score.unbounded_min.CopyFrom(_Unbounded())
+                request.by_score.unbounded_min.CopyFrom(cache_pb._Unbounded())
 
             if max_score is not None:
-                request.by_score.max_score = max_score
+                request.by_score.max_score = cache_pb._SortedSetFetchRequest._ByScore._Score(score=max_score)
             else:
-                request.by_score.unbounded_max.CopyFrom(_Unbounded())
+                request.by_score.unbounded_max.CopyFrom(cache_pb._Unbounded())
 
             if offset is not None:
                 request.by_score.offset = offset
             else:
                 request.by_score.offset = 0
 
             if count is not None:
                 request.by_score.count = count
             else:
                 request.by_score.count = -1
 
-            # ascending = 0, descending = 1
             if sort_order == SortOrder.ASCENDING:
-                request.order = 0
+                request.order = cache_pb._SortedSetFetchRequest.ASCENDING
             else:
-                request.order = 1
+                request.order = cache_pb._SortedSetFetchRequest.DESCENDING
 
-            response = self._build_stub().SortedSetFetch(
+            response = await self._build_stub().SortedSetFetch(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("SortedSetFetch", {"sorted_set_name": str(request.set_name)})
 
             type = response.WhichOneof("sorted_set")
@@ -918,48 +882,47 @@
                 )
             else:
                 raise UnknownException(f"Unknown set field in response: {type}")
         except Exception as e:
             self._log_request_error("sorted_set_fetch", e)
             return CacheSortedSetFetch.Error(convert_error(e))
 
-    def sorted_set_fetch_by_rank(
+    async def sorted_set_fetch_by_rank(
         self,
         cache_name: TCacheName,
         sorted_set_name: TSortedSetName,
         start_rank: Optional[int],
         end_rank: Optional[int],
         sort_order: SortOrder,
     ) -> CacheSortedSetFetchResponse:
         try:
             self._log_issuing_request("SortedSetFetch", {"sorted_set_name": str(sorted_set_name)})
             _validate_cache_name(cache_name)
             _validate_sorted_set_name(sorted_set_name)
 
-            request = _SortedSetFetchRequest()
-            request.set_name = _as_bytes(sorted_set_name, "Unsupported type for set_name: ")
-            request.with_scores = True
+            request = cache_pb._SortedSetFetchRequest(
+                set_name=_as_bytes(sorted_set_name, "Unsupported type for set_name: "), with_scores=True
+            )
 
             if start_rank is not None:
                 request.by_index.inclusive_start_index = start_rank
             else:
-                request.by_index.unbounded_start.CopyFrom(_Unbounded())
+                request.by_index.unbounded_start.CopyFrom(cache_pb._Unbounded())
 
             if end_rank is not None:
                 request.by_index.exclusive_end_index = end_rank
             else:
-                request.by_index.unbounded_end.CopyFrom(_Unbounded())
+                request.by_index.unbounded_end.CopyFrom(cache_pb._Unbounded())
 
-            # ascending = 0, descending = 1
             if sort_order == SortOrder.ASCENDING:
-                request.order = 0
+                request.order = cache_pb._SortedSetFetchRequest.ASCENDING
             else:
-                request.order = 1
+                request.order = cache_pb._SortedSetFetchRequest.DESCENDING
 
-            response = self._build_stub().SortedSetFetch(
+            response = await self._build_stub().SortedSetFetch(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("SortedSetFetch", {"sorted_set_name": str(request.set_name)})
 
             type = response.WhichOneof("sorted_set")
@@ -971,142 +934,142 @@
                 )
             else:
                 raise UnknownException(f"Unknown set field in response: {type}")
         except Exception as e:
             self._log_request_error("sorted_set_fetch", e)
             return CacheSortedSetFetch.Error(convert_error(e))
 
-    def sorted_set_get_scores(
+    async def sorted_set_get_scores(
         self, cache_name: TCacheName, sorted_set_name: TSortedSetName, values: TSortedSetValues
     ) -> CacheSortedSetGetScoresResponse:
         try:
             self._log_issuing_request("SortedSetGetScores", {"sorted_set_name": str(sorted_set_name)})
             _validate_cache_name(cache_name)
             _validate_sorted_set_name(sorted_set_name)
 
-            request = _SortedSetGetScoreRequest()
-            request.set_name = _as_bytes(sorted_set_name, "Unsupported type for sorted_set_name: ")
-
             bytes_values = list(_gen_sorted_set_values_as_bytes(values, self.__UNSUPPORTED_SORTED_SET_VALUES_TYPE_MSG))
-            request.values.extend(bytes_values)
+            request = cache_pb._SortedSetGetScoreRequest(
+                set_name=_as_bytes(sorted_set_name, "Unsupported type for sorted_set_name: "), values=bytes_values
+            )
 
-            response = self._build_stub().SortedSetGetScore(
+            response = await self._build_stub().SortedSetGetScore(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("SortedSetGetScores", {"sorted_set_name": str(request.set_name)})
 
             type = response.WhichOneof("sorted_set")
             if type == "found":
                 get_responses: list[CacheSortedSetGetScoreResponse] = []
                 for value, get_response in zip(bytes_values, response.found.elements):
-                    if get_response.result == Miss:
+                    if get_response.result == cache_pb.Miss:
                         get_responses.append(CacheSortedSetGetScore.Miss(value))
                     else:
                         get_responses.append(CacheSortedSetGetScore.Hit(value, get_response.score))
                 return CacheSortedSetGetScores.Hit(get_responses)
             elif type == "missing":
                 return CacheSortedSetGetScores.Miss()
             else:
                 raise UnknownException(f"Unknown field in response: {type}")
         except Exception as e:
             self._log_request_error("sorted_set_get_scores", e)
             return CacheSortedSetGetScores.Error(convert_error(e))
 
-    def sorted_set_get_rank(
+    async def sorted_set_get_rank(
         self,
         cache_name: TCacheName,
         sorted_set_name: TSortedSetName,
         value: TSortedSetValue,
         sort_order: SortOrder,
     ) -> CacheSortedSetGetRankResponse:
         try:
             self._log_issuing_request("SortedSetGetRank", {"sorted_set_name": str(sorted_set_name)})
             _validate_cache_name(cache_name)
             _validate_sorted_set_name(sorted_set_name)
 
-            request = _SortedSetGetRankRequest()
-            request.set_name = _as_bytes(sorted_set_name, "Unsupported type for sorted_set_name: ")
-            request.value = _as_bytes(value, self.__UNSUPPORTED_SORTED_SET_VALUE_TYPE_MSG)
+            request = cache_pb._SortedSetGetRankRequest(
+                set_name=_as_bytes(sorted_set_name, "Unsupported type for sorted_set_name: "),
+                value=_as_bytes(value, self.__UNSUPPORTED_SORTED_SET_VALUE_TYPE_MSG),
+            )
 
-            # ascending = 0, descending = 1
             if sort_order == SortOrder.ASCENDING:
-                request.order = 0
+                request.order = cache_pb._SortedSetGetRankRequest.ASCENDING
             else:
-                request.order = 1
+                request.order = cache_pb._SortedSetGetRankRequest.DESCENDING
 
-            response = self._build_stub().SortedSetGetRank(
+            response = await self._build_stub().SortedSetGetRank(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("SortedSetGetRank", {"sorted_set_name": str(request.set_name)})
 
-            if response.element_rank.result == Hit:
+            if response.element_rank.result == cache_pb.Hit:
                 return CacheSortedSetGetRank.Hit(response.element_rank.rank)
-            if response.element_rank.result == Miss:
+            if response.element_rank.result == cache_pb.Miss:
                 return CacheSortedSetGetRank.Miss()
             else:
                 raise UnknownException(f"Unknown field in response: {type}")
         except Exception as e:
             self._log_request_error("sorted_set_get_rank", e)
             return CacheSortedSetGetRank.Error(convert_error(e))
 
-    def sorted_set_remove_elements(
+    async def sorted_set_remove_elements(
         self,
         cache_name: TCacheName,
         sorted_set_name: TSortedSetName,
         values: TSortedSetValues,
     ) -> CacheSortedSetRemoveElementsResponse:
         try:
             self._log_issuing_request("SortedSetRemoveElements", {"sorted_set_name": str(sorted_set_name)})
             _validate_cache_name(cache_name)
             _validate_sorted_set_name(sorted_set_name)
 
-            request = _SortedSetRemoveRequest()
-            request.set_name = _as_bytes(sorted_set_name, "Unsupported type for sorted_set_name: ")
-            request.some.values.extend(
-                _gen_sorted_set_values_as_bytes(values, self.__UNSUPPORTED_SORTED_SET_VALUES_TYPE_MSG)
+            request = cache_pb._SortedSetRemoveRequest(
+                set_name=_as_bytes(sorted_set_name, "Unsupported type for sorted_set_name: "),
+                some=cache_pb._SortedSetRemoveRequest._Some(
+                    values=_gen_sorted_set_values_as_bytes(values, self.__UNSUPPORTED_SORTED_SET_VALUES_TYPE_MSG)
+                ),
             )
 
-            self._build_stub().SortedSetRemove(
+            await self._build_stub().SortedSetRemove(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("SortedSetRemoveElements", {"sorted_set_name": str(request.set_name)})
 
             return CacheSortedSetRemoveElements.Success()
         except Exception as e:
             self._log_request_error("sorted_set_remove_elements", e)
             return CacheSortedSetRemoveElements.Error(convert_error(e))
 
-    def sorted_set_increment(
+    async def sorted_set_increment(
         self,
         cache_name: TCacheName,
         sorted_set_name: TSortedSetName,
         value: TSortedSetValue,
         score: TSortedSetScore,
         ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
     ) -> CacheSortedSetIncrementResponse:
         try:
             self._log_issuing_request("SortedSetIncrement", {"sorted_set_name": str(sorted_set_name)})
             _validate_cache_name(cache_name)
             _validate_sorted_set_name(sorted_set_name)
             _validate_sorted_set_score(score)
 
-            request = _SortedSetIncrementRequest()
-            request.set_name = _as_bytes(sorted_set_name, "Unsupported type for sorted_set_name: ")
-            request.value = _as_bytes(value)
-            request.amount = score
-            request.ttl_milliseconds = self._collection_ttl_or_default_milliseconds(ttl)
-            request.refresh_ttl = ttl.refresh_ttl
+            request = cache_pb._SortedSetIncrementRequest(
+                set_name=_as_bytes(sorted_set_name, "Unsupported type for sorted_set_name: "),
+                value=_as_bytes(value),
+                amount=score,
+                **self._prepare_collection_ttl_for_request(ttl),
+            )
 
-            response = self._build_stub().SortedSetIncrement(
+            response = await self._build_stub().SortedSetIncrement(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("SortedSetIncrement", {"sorted_set_name": str(request.set_name)})
 
             return CacheSortedSetIncrement.Success(response.score)
@@ -1119,22 +1082,36 @@
 
     def _log_issuing_request(self, request_type: str, request_args: dict[str, str]) -> None:
         self._logger.log(logs.TRACE, f"Issuing a {request_type} request with {request_args}")
 
     def _log_request_error(self, request_type: str, e: Exception) -> None:
         self._logger.warning(f"{request_type} failed with exception: {e}")
 
-    def _collection_ttl_or_default_milliseconds(self, collection_ttl: CollectionTtl) -> int:
-        return self._ttl_or_default_milliseconds(collection_ttl.ttl)
+    def _prepare_collection_ttl_for_request(self, collection_ttl: CollectionTtl) -> dict[str, Any]:  # type: ignore
+        """Converts a CollectionTtl object into a dictionary that can be used as kwargs for a request.
+
+        The TTL is converted to milliseconds, with a default of the client default TTL.
+        The refresh TTL is left as is.
+
+        Args:
+            collection_ttl (CollectionTtl): The CollectionTtl object to convert.
+
+        Returns:
+            dict[str, Any]: The dictionary that can be used as kwargs for a request.
+        """
+        return {
+            "ttl_milliseconds": self._ttl_or_default_milliseconds(collection_ttl.ttl),
+            "refresh_ttl": collection_ttl.refresh_ttl,
+        }
 
     def _ttl_or_default_milliseconds(self, ttl: Optional[timedelta]) -> int:
         which_ttl = self._default_ttl
         if ttl is not None:
             which_ttl = ttl
 
         return int(which_ttl.total_seconds() * 1000)
 
-    def _build_stub(self) -> ScsStub:
-        return self._grpc_manager.stub()
+    def _build_stub(self) -> cache_grpc.ScsStub:
+        return self._grpc_manager.async_stub()
 
-    def close(self) -> None:
-        self._grpc_manager.close()
+    async def close(self) -> None:
+        await self._grpc_manager.close()
```

### Comparing `momento-1.4.0/src/momento/internal/synchronous/_scs_grpc_manager.py` & `momento-1.5.0/src/momento/internal/synchronous/_scs_grpc_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import grpc
-import momento_wire_types.cacheclient_pb2_grpc as cache_client
-import momento_wire_types.controlclient_pb2_grpc as control_client
 import pkg_resources
+from momento_wire_types import cacheclient_pb2_grpc as cache_client
+from momento_wire_types import controlclient_pb2_grpc as control_client
 
 from momento.auth import CredentialProvider
 from momento.config import Configuration
 from momento.internal.synchronous._add_header_client_interceptor import (
     AddHeaderClientInterceptor,
     Header,
 )
@@ -23,15 +23,15 @@
     def __init__(self, configuration: Configuration, credential_provider: CredentialProvider):
         self._secure_channel = grpc.secure_channel(
             target=credential_provider.control_endpoint, credentials=grpc.ssl_channel_credentials()
         )
         intercept_channel = grpc.intercept_channel(
             self._secure_channel, *_interceptors(credential_provider.auth_token, configuration.get_retry_strategy())
         )
-        self._stub = control_client.ScsControlStub(intercept_channel)
+        self._stub = control_client.ScsControlStub(intercept_channel)  # type: ignore[no-untyped-call]
 
     def close(self) -> None:
         self._secure_channel.close()
 
     def stub(self) -> control_client.ScsControlStub:
         return self._stub
 
@@ -45,15 +45,15 @@
         self._secure_channel = grpc.secure_channel(
             target=credential_provider.cache_endpoint,
             credentials=grpc.ssl_channel_credentials(),
         )
         intercept_channel = grpc.intercept_channel(
             self._secure_channel, *_interceptors(credential_provider.auth_token, configuration.get_retry_strategy())
         )
-        self._stub = cache_client.ScsStub(intercept_channel)
+        self._stub = cache_client.ScsStub(intercept_channel)  # type: ignore[no-untyped-call]
 
     def close(self) -> None:
         self._secure_channel.close()
 
     def stub(self) -> cache_client.ScsStub:
         return self._stub
```

### Comparing `momento-1.4.0/src/momento/logs.py` & `momento-1.5.0/src/momento/logs.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/requests/collection_ttl.py` & `momento-1.5.0/src/momento/requests/collection_ttl.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/__init__.py` & `momento-1.5.0/src/momento/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/control/cache/create.py` & `momento-1.5.0/src/momento/responses/control/cache/create.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/control/cache/delete.py` & `momento-1.5.0/src/momento/responses/control/cache/delete.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/control/cache/flush.py` & `momento-1.5.0/src/momento/responses/control/cache/flush.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/control/cache/list.py` & `momento-1.5.0/src/momento/responses/control/cache/list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from abc import ABC
 from dataclasses import dataclass
 from typing import List
 
-from momento_wire_types.controlclient_pb2 import _ListCachesResponse
+from momento_wire_types import controlclient_pb2 as ctrl_pb
 
 from momento.responses.response import ControlResponse
 
 from ...mixins import ErrorResponseMixin
 
 
 class ListCachesResponse(ControlResponse):
@@ -56,15 +56,15 @@
     class Success(ListCachesResponse):
         """Indicates the request was successful."""
 
         caches: List[CacheInfo]
         """The list of caches available to the user."""
 
         @staticmethod
-        def from_grpc_response(grpc_list_cache_response: _ListCachesResponse) -> ListCaches.Success:  # type: ignore[misc] # noqa: E501
+        def from_grpc_response(grpc_list_cache_response: ctrl_pb._ListCachesResponse) -> ListCaches.Success:
             """Initializes ListCacheResponse to handle list cache response.
 
             Args:
                 grpc_list_cache_response: Protobuf based response returned by Scs.
             """
             caches = [CacheInfo(cache.cache_name) for cache in grpc_list_cache_response.cache]  # type: ignore[misc]
             return ListCaches.Success(caches=caches)
```

### Comparing `momento-1.4.0/src/momento/responses/control/signing_key/create.py` & `momento-1.5.0/src/momento/responses/control/signing_key/create.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/control/signing_key/list.py` & `momento-1.5.0/src/momento/responses/control/signing_key/list.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/control/signing_key/revoke.py` & `momento-1.5.0/src/momento/responses/control/signing_key/revoke.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/dictionary/fetch.py` & `momento-1.5.0/src/momento/responses/data/dictionary/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/dictionary/get_field.py` & `momento-1.5.0/src/momento/responses/data/dictionary/get_field.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/dictionary/get_fields.py` & `momento-1.5.0/src/momento/responses/data/dictionary/get_fields.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/dictionary/increment.py` & `momento-1.5.0/src/momento/responses/data/dictionary/increment.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/dictionary/remove_field.py` & `momento-1.5.0/src/momento/responses/data/dictionary/remove_field.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/dictionary/remove_fields.py` & `momento-1.5.0/src/momento/responses/data/dictionary/remove_fields.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/dictionary/set_field.py` & `momento-1.5.0/src/momento/responses/data/dictionary/set_field.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/dictionary/set_fields.py` & `momento-1.5.0/src/momento/responses/data/dictionary/set_fields.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/list/concatenate_back.py` & `momento-1.5.0/src/momento/responses/data/list/concatenate_back.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/list/concatenate_front.py` & `momento-1.5.0/src/momento/responses/data/list/concatenate_front.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/list/fetch.py` & `momento-1.5.0/src/momento/responses/data/list/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/list/length.py` & `momento-1.5.0/src/momento/responses/data/list/length.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/list/pop_back.py` & `momento-1.5.0/src/momento/responses/data/list/pop_back.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/list/pop_front.py` & `momento-1.5.0/src/momento/responses/data/list/pop_front.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/list/push_back.py` & `momento-1.5.0/src/momento/responses/data/list/push_back.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/list/push_front.py` & `momento-1.5.0/src/momento/responses/data/list/push_front.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/list/remove_value.py` & `momento-1.5.0/src/momento/responses/data/list/remove_value.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/scalar/delete.py` & `momento-1.5.0/src/momento/responses/data/scalar/delete.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/scalar/get.py` & `momento-1.5.0/src/momento/responses/data/scalar/get.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/scalar/increment.py` & `momento-1.5.0/src/momento/responses/data/scalar/increment.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/scalar/set.py` & `momento-1.5.0/src/momento/responses/data/scalar/set.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/scalar/set_if_not_exists.py` & `momento-1.5.0/src/momento/responses/data/scalar/set_if_not_exists.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/set/add_element.py` & `momento-1.5.0/src/momento/responses/data/set/add_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/set/add_elements.py` & `momento-1.5.0/src/momento/responses/data/set/add_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/set/fetch.py` & `momento-1.5.0/src/momento/responses/data/set/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/set/remove_element.py` & `momento-1.5.0/src/momento/responses/data/set/remove_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/set/remove_elements.py` & `momento-1.5.0/src/momento/responses/data/set/remove_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/sorted_set/fetch.py` & `momento-1.5.0/src/momento/responses/data/sorted_set/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/sorted_set/get_rank.py` & `momento-1.5.0/src/momento/responses/data/sorted_set/get_rank.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/sorted_set/get_score.py` & `momento-1.5.0/src/momento/responses/data/sorted_set/get_score.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/sorted_set/get_scores.py` & `momento-1.5.0/src/momento/responses/data/sorted_set/get_scores.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/sorted_set/increment.py` & `momento-1.5.0/src/momento/responses/data/sorted_set/increment.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/sorted_set/put_element.py` & `momento-1.5.0/src/momento/responses/data/sorted_set/put_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/sorted_set/put_elements.py` & `momento-1.5.0/src/momento/responses/data/sorted_set/put_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/sorted_set/remove_element.py` & `momento-1.5.0/src/momento/responses/data/sorted_set/remove_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/data/sorted_set/remove_elements.py` & `momento-1.5.0/src/momento/responses/data/sorted_set/remove_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/mixins.py` & `momento-1.5.0/src/momento/responses/mixins.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/responses/response.py` & `momento-1.5.0/src/momento/responses/response.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/retry/default_eligibility_strategy.py` & `momento-1.5.0/src/momento/retry/default_eligibility_strategy.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/retry/fixed_count_retry_strategy.py` & `momento-1.5.0/src/momento/retry/fixed_count_retry_strategy.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/src/momento/typing.py` & `momento-1.5.0/src/momento/typing.py`

 * *Files identical despite different names*

### Comparing `momento-1.4.0/setup.py` & `momento-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,20 +28,20 @@
  'momento.retry']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['grpcio>=1.46.0,<2.0.0',
- 'momento-wire-types>=0.60,<0.61',
+ 'momento-wire-types>=0.64,<0.65',
  'pyjwt>=2.4.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'momento',
-    'version': '1.4.0',
+    'version': '1.5.0',
     'description': 'SDK for Momento',
     'long_description': '<img src="https://docs.momentohq.com/img/logo.svg" alt="logo" width="400"/>\n\n[![project status](https://momentohq.github.io/standards-and-practices/badges/project-status-official.svg)](https://github.com/momentohq/standards-and-practices/blob/main/docs/momento-on-github.md)\n[![project stability](https://momentohq.github.io/standards-and-practices/badges/project-stability-stable.svg)](https://github.com/momentohq/standards-and-practices/blob/main/docs/momento-on-github.md) \n\n# Momento Python Client Library\n\n\nPython client SDK for Momento Serverless Cache: a fast, simple, pay-as-you-go caching solution without\nany of the operational overhead required by traditional caching solutions!\n\n\n\n## Getting Started :running:\n\n### Requirements\n\n- [Python 3.7](https://www.python.org/downloads/) or above is required\n- A Momento Auth Token is required, you can generate one using the [Momento CLI](https://github.com/momentohq/momento-cli)\n\n### Examples\n\nReady to dive right in? Just check out the [examples](https://github.com/momentohq/client-sdk-python/tree/main/examples) directory for complete, working examples of\nhow to use the SDK.\n\n### Installation\n\nThe [Momento SDK is available on PyPi](https://pypi.org/project/momento/). To install via pip:\n\n```bash\npip install momento\n```\n\n### Usage\n\nThe examples below require an environment variable named MOMENTO_AUTH_TOKEN which must\nbe set to a valid [Momento authentication token](https://docs.momentohq.com/docs/getting-started#obtain-an-auth-token).\n\nPython 3.10 introduced the `match` statement, which allows for [structural pattern matching on objects](https://peps.python.org/pep-0636/#adding-a-ui-matching-objects).\nIf you are running python 3.10 or greater, here is a quickstart you can use in your own project:\n\n```python\nfrom datetime import timedelta\n\nfrom momento import CacheClient, Configurations, CredentialProvider\nfrom momento.responses import CacheGet, CacheSet, CreateCache\n\nif __name__ == "__main__":\n    cache_name = "default-cache"\n    with CacheClient(\n        configuration=Configurations.Laptop.v1(),\n        credential_provider=CredentialProvider.from_environment_variable("MOMENTO_AUTH_TOKEN"),\n        default_ttl=timedelta(seconds=60),\n    ) as cache_client:\n        create_cache_response = cache_client.create_cache(cache_name)\n        match create_cache_response:\n            case CreateCache.CacheAlreadyExists():\n                print(f"Cache with name: {cache_name} already exists.")\n            case CreateCache.Error() as error:\n                raise error.inner_exception\n\n        print("Setting Key: foo to Value: FOO")\n        set_response = cache_client.set(cache_name, "foo", "FOO")\n        match set_response:\n            case CacheSet.Error() as error:\n                raise error.inner_exception\n\n        print("Getting Key: foo")\n        get_response = cache_client.get(cache_name, "foo")\n        match get_response:\n            case CacheGet.Hit() as hit:\n                print(f"Look up resulted in a hit: {hit}")\n                print(f"Looked up Value: {hit.value_string!r}")\n            case CacheGet.Miss():\n                print("Look up resulted in a: miss. This is unexpected.")\n            case CacheGet.Error() as error:\n                raise error.inner_exception\n\n```\n\nThe above code uses [structural pattern matching](https://peps.python.org/pep-0636/), a feature introduced in Python 3.10.\nUsing a Python version less than 3.10? No problem. Here is the same example compatible across all versions of Python:\n\n```python\nfrom datetime import timedelta\nfrom momento import CacheClient, Configurations, CredentialProvider\nfrom momento.responses import CacheGet, CacheSet, CreateCache\n\nif __name__ == "__main__":\n    cache_name = \'default-cache\'\n    with CacheClient(configuration=Configurations.Laptop.v1(),\n                     credential_provider=CredentialProvider.from_environment_variable(\'MOMENTO_AUTH_TOKEN\'),\n                     default_ttl=timedelta(seconds=60)\n                     ) as cache_client:\n        create_cache_response = cache_client.create_cache(cache_name)\n        if isinstance(create_cache_response, CreateCache.CacheAlreadyExists):\n            print(f"Cache with name: {cache_name} already exists.")\n        elif isinstance(create_cache_response, CreateCache.Error):\n            raise create_cache_response.inner_exception\n\n        print("Setting Key: foo to Value: FOO")\n        set_response = cache_client.set(cache_name, \'foo\', \'FOO\')\n        if isinstance(set_response, CacheSet.Error):\n            raise set_response.inner_exception\n\n        print("Getting Key: foo")\n        get_response = cache_client.get(cache_name, \'foo\')\n        if isinstance(get_response, CacheGet.Hit):\n            print(f"Look up resulted in a hit: {get_response.value_string}")\n            print(f"Looked up Value: {get_response.value_string}")\n        elif isinstance(get_response, CacheGet.Miss):\n            print("Look up resulted in a: miss. This is unexpected.")\n        elif isinstance(get_response, CacheGet.Error):\n            raise get_response.inner_exception\n```\n\n### Logging\n\nTo avoid cluttering DEBUG logging with per-method logs the Momento SDK adds a TRACE logging level. This will only happen\nif the TRACE level does not already exist.\n\nTo enable TRACE level logging you can call logging.basicConfig() before making any log statements:\n\n```python\nimport logging\n\nlogging.basicConfig(level=\'TRACE\')\n```\n\n### Error Handling\n\nComing Soon!\n\n### Tuning\n\nComing Soon!\n\n----------------------------------------------------------------------------------------\nFor more info, visit our website at [https://gomomento.com](https://gomomento.com)!\n',
     'author': 'Momento',
     'author_email': 'hello@momentohq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gomomento.com',
```

### Comparing `momento-1.4.0/PKG-INFO` & `momento-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momento
-Version: 1.4.0
+Version: 1.5.0
 Summary: SDK for Momento
 Home-page: https://gomomento.com
 License: Apache-2.0
 Keywords: Momento,caching,key-value store,serverless
 Author: Momento
 Author-email: hello@momentohq.com
 Requires-Python: >=3.7,<4.0
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Typing :: Typed
 Requires-Dist: grpcio (>=1.46.0,<2.0.0)
-Requires-Dist: momento-wire-types (>=0.60,<0.61)
+Requires-Dist: momento-wire-types (>=0.64,<0.65)
 Requires-Dist: pyjwt (>=2.4.0,<3.0.0)
 Project-URL: Documentation, https://docs.momentohq.com/
 Project-URL: Repository, https://github.com/momentohq/client-sdk-python
 Description-Content-Type: text/markdown
 
 <img src="https://docs.momentohq.com/img/logo.svg" alt="logo" width="400"/>
```

