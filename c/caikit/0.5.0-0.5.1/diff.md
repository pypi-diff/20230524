# Comparing `tmp/caikit-0.5.0.tar.gz` & `tmp/caikit-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "caikit-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `caikit-0.5.0.tar` & `caikit-0.5.1.tar`

### file list

```diff
@@ -1,305 +1,305 @@
--rw-r--r--   0        0        0       60 2023-05-22 21:25:00.861991 caikit-0.5.0/.coveragerc
--rw-r--r--   0        0        0      676 2023-05-22 21:25:00.861991 caikit-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      579 2023-05-22 21:25:00.861991 caikit-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-05-22 21:25:00.861991 caikit-0.5.0/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0        0        0      106 2023-05-22 21:25:00.861991 caikit-0.5.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1272 2023-05-22 21:25:00.861991 caikit-0.5.0/.github/workflows/build-library.yml
--rw-r--r--   0        0        0     1328 2023-05-22 21:25:00.861991 caikit-0.5.0/.github/workflows/lint-code.yml
--rw-r--r--   0        0        0     1136 2023-05-22 21:25:00.861991 caikit-0.5.0/.github/workflows/publish-library.yml
--rw-r--r--   0        0        0      261 2023-05-22 21:25:00.861991 caikit-0.5.0/.gitignore
--rw-r--r--   0        0        0      324 2023-05-22 21:25:00.861991 caikit-0.5.0/.isort.cfg
--rw-r--r--   0        0        0      370 2023-05-22 21:25:00.861991 caikit-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      122 2023-05-22 21:25:00.861991 caikit-0.5.0/.prettierignore
--rw-r--r--   0        0        0       12 2023-05-22 21:25:00.861991 caikit-0.5.0/.prettierrc.yaml
--rw-r--r--   0        0        0    21434 2023-05-22 21:25:00.861991 caikit-0.5.0/.pylintrc
--rw-r--r--   0        0        0       78 2023-05-22 21:25:00.861991 caikit-0.5.0/.whitesource
--rw-r--r--   0        0        0      368 2023-05-22 21:25:00.861991 caikit-0.5.0/CODEOWNERS
--rw-r--r--   0        0        0     7165 2023-05-22 21:25:00.861991 caikit-0.5.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-05-22 21:25:00.861991 caikit-0.5.0/LICENSE
--rw-r--r--   0        0        0     3626 2023-05-22 21:25:00.861991 caikit-0.5.0/README.md
--rw-r--r--   0        0        0      152 2023-05-22 21:25:00.861991 caikit-0.5.0/SECURITY.md
--rw-r--r--   0        0        0    44878 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit-overview.png
--rw-r--r--   0        0        0      427 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/__init__.py
--rw-r--r--   0        0        0      727 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/config/__init__.py
--rw-r--r--   0        0        0     6052 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/config/config.py
--rw-r--r--   0        0        0     6488 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/config/config.yml
--rw-r--r--   0        0        0     1615 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/__init__.py
--rw-r--r--   0        0        0      812 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/augmentors/__init__.py
--rw-r--r--   0        0        0     3506 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/augmentors/base.py
--rw-r--r--   0        0        0     2828 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/augmentors/merged_augmentor.py
--rw-r--r--   0        0        0      355 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/augmentors/schemes/__init__.py
--rw-r--r--   0        0        0     2052 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/augmentors/schemes/always_selection_scheme.py
--rw-r--r--   0        0        0     3164 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/augmentors/schemes/base.py
--rw-r--r--   0        0        0     3264 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
--rw-r--r--   0        0        0     2898 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/augmentors/schemes/random_single_selection_scheme.py
--rw-r--r--   0        0        0     1027 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/__init__.py
--rw-r--r--   0        0        0    35512 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/base.py
--rw-r--r--   0        0        0      750 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     2207 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/data_backends/base.py
--rw-r--r--   0        0        0     4050 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/data_backends/dict_backend.py
--rw-r--r--   0        0        0    14380 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/dataobject.py
--rw-r--r--   0        0        0     4858 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/enums.py
--rw-r--r--   0        0        0     1564 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/producer.py
--rw-r--r--   0        0        0     3914 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/protobufs/__init__.py
--rw-r--r--   0        0        0      577 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/streams/__init__.py
--rw-r--r--   0        0        0     5500 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/streams/converter.py
--rw-r--r--   0        0        0     4788 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/streams/csv_column_formatter.py
--rw-r--r--   0        0        0    40212 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/streams/data_stream.py
--rw-r--r--   0        0        0     3606 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/streams/resolver.py
--rw-r--r--   0        0        0     5245 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/data_model/streams/validator.py
--rw-r--r--   0        0        0    21296 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/model_manager.py
--rw-r--r--   0        0        0      684 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/module_backends/__init__.py
--rw-r--r--   0        0        0     2834 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/module_backends/backend_types.py
--rw-r--r--   0        0        0     4718 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/module_backends/base.py
--rw-r--r--   0        0        0     2802 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/module_backends/local_backend.py
--rw-r--r--   0        0        0     6002 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/module_backends/module_backend_config.py
--rw-r--r--   0        0        0      742 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/modules/__init__.py
--rw-r--r--   0        0        0    30065 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/modules/base.py
--rw-r--r--   0        0        0     6247 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/modules/config.py
--rw-r--r--   0        0        0    10859 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/modules/decorator.py
--rw-r--r--   0        0        0     4151 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/modules/loader.py
--rw-r--r--   0        0        0     6013 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/modules/meta.py
--rw-r--r--   0        0        0    13024 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/modules/saver.py
--rw-r--r--   0        0        0     3895 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/registries.py
--rw-r--r--   0        0        0     5358 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/task.py
--rw-r--r--   0        0        0     1001 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/toolkit/__init__.py
--rw-r--r--   0        0        0     4716 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/toolkit/compatibility.py
--rw-r--r--   0        0        0      637 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/toolkit/errors/__init__.py
--rw-r--r--   0        0        0    21366 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/toolkit/errors/error_handler.py
--rw-r--r--   0        0        0     1400 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/toolkit/errors/validation_error.py
--rw-r--r--   0        0        0     4935 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/toolkit/fileio.py
--rw-r--r--   0        0        0     2292 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/toolkit/isa.py
--rw-r--r--   0        0        0     1648 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/toolkit/logging.py
--rw-r--r--   0        0        0    32206 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/toolkit/quality_evaluation.py
--rw-r--r--   0        0        0     3439 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/toolkit/serializers.py
--rw-r--r--   0        0        0     5979 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/core/toolkit/wip_decorator.py
--rw-r--r--   0        0        0      530 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/interfaces/__init__.py
--rw-r--r--   0        0        0      748 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/interfaces/common/__init__.py
--rw-r--r--   0        0        0     1211 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/interfaces/common/data_model/__init__.py
--rw-r--r--   0        0        0     1431 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/interfaces/common/data_model/producer.py
--rw-r--r--   0        0        0      611 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/interfaces/runtime/__init__.py
--rw-r--r--   0        0        0      763 2023-05-22 21:25:00.865985 caikit-0.5.0/caikit/interfaces/runtime/data_model/__init__.py
--rw-r--r--   0        0        0     1886 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/interfaces/runtime/data_model/training_management.py
--rw-r--r--   0        0        0      577 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/__init__.py
--rw-r--r--   0        0        0     1827 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/dump_services.py
--rw-r--r--   0        0        0    14200 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/grpc_server.py
--rw-r--r--   0        0        0      577 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/interceptors/__init__.py
--rw-r--r--   0        0        0    16502 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
--rw-r--r--   0        0        0      577 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     4659 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/metrics/rpc_meter.py
--rw-r--r--   0        0        0      577 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    17143 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/model_management/batcher.py
--rw-r--r--   0        0        0     2648 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/model_management/loaded_model.py
--rw-r--r--   0        0        0     5802 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/model_management/model_loader.py
--rw-r--r--   0        0        0    12101 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/model_management/model_manager.py
--rw-r--r--   0        0        0     4311 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/model_management/model_sizer.py
--rw-r--r--   0        0        0     1480 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/model_management/training_manager.py
--rw-r--r--   0        0        0      367 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/protobufs/README.md
--rw-r--r--   0        0        0      698 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/protobufs/__init__.py
--rw-r--r--   0        0        0    11375 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/protobufs/model_mesh_pb2.py
--rw-r--r--   0        0        0    12846 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
--rw-r--r--   0        0        0    10107 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/protobufs/model_runtime_pb2.py
--rw-r--r--   0        0        0    10556 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     5535 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/protobufs/process_pb2.py
--rw-r--r--   0        0        0     2569 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/protobufs/process_pb2_grpc.py
--rw-r--r--   0        0        0     8844 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/protobufs/protos/model-mesh.proto
--rw-r--r--   0        0        0     6795 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/protobufs/protos/model-runtime.proto
--rw-r--r--   0        0        0     2479 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/protobufs/protos/process.proto
--rw-r--r--   0        0        0    16699 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_factory.py
--rw-r--r--   0        0        0      109 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     1779 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_generation/compatibility_checker.py
--rw-r--r--   0        0        0     3043 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_generation/core_module_helpers.py
--rw-r--r--   0        0        0     5838 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_generation/create_service.py
--rw-r--r--   0        0        0    13914 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_generation/data_stream_source.py
--rw-r--r--   0        0        0     7155 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_generation/primitives.py
--rw-r--r--   0        0        0    12800 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_generation/rpcs.py
--rw-r--r--   0        0        0      666 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0    10747 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_generation/signature_parsing/docstrings.py
--rw-r--r--   0        0        0     4794 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_generation/signature_parsing/module_signature.py
--rw-r--r--   0        0        0     8225 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_generation/signature_parsing/parsers.py
--rw-r--r--   0        0        0     2571 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/service_generation/type_helpers.py
--rw-r--r--   0        0        0      577 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     9476 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/servicers/global_predict_servicer.py
--rw-r--r--   0        0        0    15326 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/servicers/global_train_servicer.py
--rw-r--r--   0        0        0    10637 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/servicers/model_runtime_servicer.py
--rw-r--r--   0        0        0     5539 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/servicers/model_train_servicer.py
--rw-r--r--   0        0        0     1667 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/servicers/training_management_servicer.py
--rw-r--r--   0        0        0      577 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/types/__init__.py
--rw-r--r--   0        0        0      957 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/types/aborted_exception.py
--rw-r--r--   0        0        0     1558 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/types/caikit_runtime_exception.py
--rw-r--r--   0        0        0      960 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/types/thread_destroyed_exception.py
--rw-r--r--   0        0        0      577 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/utils/__init__.py
--rw-r--r--   0        0        0     6810 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/utils/import_util.py
--rw-r--r--   0        0        0    17892 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/utils/servicer_util.py
--rw-r--r--   0        0        0      577 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     3732 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/work_management/abortable_action.py
--rw-r--r--   0        0        0     2969 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/work_management/call_aborter.py
--rw-r--r--   0        0        0     7596 2023-05-22 21:25:00.869980 caikit-0.5.0/caikit/runtime/work_management/destroyable_thread.py
--rw-r--r--   0        0        0      169 2023-05-22 21:25:00.869980 caikit-0.5.0/code-of-conduct.md
--rw-r--r--   0        0        0       68 2023-05-22 21:25:00.869980 caikit-0.5.0/docs-requirements.txt
--rw-r--r--   0        0        0      634 2023-05-22 21:25:00.869980 caikit-0.5.0/docs/Makefile
--rw-r--r--   0        0        0     1610 2023-05-22 21:25:00.869980 caikit-0.5.0/docs/adrs/010-data-model-definition.md
--rw-r--r--   0        0        0     2352 2023-05-22 21:25:00.869980 caikit-0.5.0/docs/adrs/015-runtime-service-generation.md
--rw-r--r--   0        0        0     2581 2023-05-22 21:25:00.869980 caikit-0.5.0/docs/adrs/018-shared-backends.md
--rw-r--r--   0        0        0     1223 2023-05-22 21:25:00.869980 caikit-0.5.0/docs/adrs/019-loader-stack.md
--rw-r--r--   0        0        0      404 2023-05-22 21:25:00.869980 caikit-0.5.0/docs/adrs/README.md
--rw-r--r--   0        0        0     2423 2023-05-22 21:25:00.869980 caikit-0.5.0/docs/architecture_club/04-25-23.md
--rw-r--r--   0        0        0      342 2023-05-22 21:25:00.869980 caikit-0.5.0/docs/architecture_club/README.md
--rw-r--r--   0        0        0     2660 2023-05-22 21:25:00.869980 caikit-0.5.0/docs/conf.py
--rw-r--r--   0        0        0      225 2023-05-22 21:25:00.869980 caikit-0.5.0/docs/index.rst
--rw-r--r--   0        0        0      800 2023-05-22 21:25:00.869980 caikit-0.5.0/docs/make.bat
--rw-r--r--   0        0        0      837 2023-05-22 21:25:00.869980 caikit-0.5.0/examples/start_runtime_with_sample_lib.py
--rw-r--r--   0        0        0     6095 2023-05-22 21:25:00.869980 caikit-0.5.0/examples/text-sentiment/README.md
--rw-r--r--   0        0        0     1425 2023-05-22 21:25:00.869980 caikit-0.5.0/examples/text-sentiment/client.py
--rw-r--r--   0        0        0      673 2023-05-22 21:25:00.869980 caikit-0.5.0/examples/text-sentiment/models/text_sentiment/config.yml
--rw-r--r--   0        0        0       72 2023-05-22 21:25:00.869980 caikit-0.5.0/examples/text-sentiment/requirements.txt
--rw-r--r--   0        0        0      961 2023-05-22 21:25:00.873974 caikit-0.5.0/examples/text-sentiment/start_runtime.py
--rw-r--r--   0        0        0      816 2023-05-22 21:25:00.873974 caikit-0.5.0/examples/text-sentiment/text_sentiment/__init__.py
--rw-r--r--   0        0        0      742 2023-05-22 21:25:00.873974 caikit-0.5.0/examples/text-sentiment/text_sentiment/config.yml
--rw-r--r--   0        0        0      661 2023-05-22 21:25:00.873974 caikit-0.5.0/examples/text-sentiment/text_sentiment/data_model/__init__.py
--rw-r--r--   0        0        0     1422 2023-05-22 21:25:00.873974 caikit-0.5.0/examples/text-sentiment/text_sentiment/data_model/classification.py
--rw-r--r--   0        0        0      645 2023-05-22 21:25:00.873974 caikit-0.5.0/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
--rw-r--r--   0        0        0     3067 2023-05-22 21:25:00.873974 caikit-0.5.0/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py
--rw-r--r--   0        0        0     1179 2023-05-22 21:25:04.013929 caikit-0.5.0/pyproject.toml
--rwxr-xr-x   0        0        0      639 2023-05-22 21:25:00.873974 caikit-0.5.0/scripts/check_deps.sh
--rwxr-xr-x   0        0        0      720 2023-05-22 21:25:00.873974 caikit-0.5.0/scripts/fmt.sh
--rw-r--r--   0        0        0       33 2023-05-22 21:25:00.873974 caikit-0.5.0/setup_requirements.txt
--rw-r--r--   0        0        0     1006 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0     3439 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/base.py
--rw-r--r--   0        0        0        0 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/config/__init__.py
--rw-r--r--   0        0        0     5358 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/config/test_configs.py
--rw-r--r--   0        0        0     8956 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/__init__.py
--rw-r--r--   0        0        0     2853 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/augmentors/test_augmentor_base.py
--rw-r--r--   0        0        0     9114 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/augmentors/test_merged_augmentors.py
--rw-r--r--   0        0        0        0 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/data_model/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     5033 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/data_model/data_backends/test_dict_backend.py
--rw-r--r--   0        0        0     3306 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/data_model/streams/test_converter.py
--rw-r--r--   0        0        0     3314 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/data_model/streams/test_csv_column_formatter.py
--rw-r--r--   0        0        0    26459 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/data_model/streams/test_data_stream.py
--rw-r--r--   0        0        0     3498 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/data_model/streams/test_resolver.py
--rw-r--r--   0        0        0     2908 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/data_model/streams/test_validator.py
--rw-r--r--   0        0        0    16232 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/data_model/test_base.py
--rw-r--r--   0        0        0    19538 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/data_model/test_dataobject.py
--rw-r--r--   0        0        0     5083 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/data_model/test_enums.py
--rw-r--r--   0        0        0     1104 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/data_model/test_producer.py
--rw-r--r--   0        0        0     4357 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/helpers.py
--rw-r--r--   0        0        0        0 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/module_backends/__init__.py
--rw-r--r--   0        0        0     2320 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/module_backends/test_backend_types.py
--rw-r--r--   0        0        0     6922 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/module_backends/test_module_backend_config.py
--rw-r--r--   0        0        0        0 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/modules/__init__.py
--rw-r--r--   0        0        0    12293 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/modules/test_module.py
--rw-r--r--   0        0        0     6274 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/modules/test_module_metadata.py
--rw-r--r--   0        0        0      521 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/test_imports.py
--rw-r--r--   0        0        0    21421 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/test_model_manager.py
--rw-r--r--   0        0        0     1038 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/test_no_write_permissions.py
--rw-r--r--   0        0        0     2460 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/test_task.py
--rw-r--r--   0        0        0     7967 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/toolkit/test_compatibility.py
--rw-r--r--   0        0        0    18396 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/toolkit/test_error_handler.py
--rw-r--r--   0        0        0     4997 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/toolkit/test_fileio.py
--rw-r--r--   0        0        0    25851 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/toolkit/test_quality_evaluation.py
--rw-r--r--   0        0        0     2634 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/toolkit/test_serializers.py
--rw-r--r--   0        0        0     7824 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/core/toolkit/test_wip_decorator.py
--rw-r--r--   0        0        0     6782 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/data_model_helpers.py
--rw-r--r--   0        0        0       39 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      647 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/config/config.yml
--rw-r--r--   0        0        0       27 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/bad_file.json
--rw-r--r--   0        0        0      154 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/control_chars.jsonl
--rw-r--r--   0        0        0      106 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample.csv
--rw-r--r--   0        0        0       66 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample.json
--rw-r--r--   0        0        0      233 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample.jsonl
--rw-r--r--   0        0        0     1322 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample.txt
--rw-r--r--   0        0        0       11 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
--rw-r--r--   0        0        0       11 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
--rw-r--r--   0        0        0       11 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
--rw-r--r--   0        0        0       27 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
--rw-r--r--   0        0        0       27 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
--rw-r--r--   0        0        0       63 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
--rw-r--r--   0        0        0      147 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
--rw-r--r--   0        0        0      218 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
--rw-r--r--   0        0        0       87 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
--rw-r--r--   0        0        0       52 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
--rw-r--r--   0        0        0       56 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
--rw-r--r--   0        0        0       55 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
--rw-r--r--   0        0        0      125 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/data_stream_inputs/sample_w_header.csv
--rw-r--r--   0        0        0      222 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/dummy_dataset.json
--rw-r--r--   0        0        0     1016 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/dummy_module.zip
--rw-r--r--   0        0        0      675 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/dummy_module/config.yml
--rw-r--r--   0        0        0      299 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/dummy_module/data.json
--rw-r--r--   0        0        0       14 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/dummy_module/data.pkl
--rw-r--r--   0        0        0      191 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/dummy_module_backend/config.yml
--rw-r--r--   0        0        0      179 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/dummy_module_foo/config.yml
--rw-r--r--   0        0        0      506 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/dummy_module_no_nesting.zip
--rw-r--r--   0        0        0      570 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/dummy_module_singleton/config.yml
--rw-r--r--   0        0        0      299 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/dummy_module_singleton/data.json
--rw-r--r--   0        0        0       14 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/dummy_module_singleton/data.pkl
--rw-r--r--   0        0        0      230 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/dummy_resource/config.yml
--rw-r--r--   0        0        0     3034 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/fixtures.py
--rw-r--r--   0        0        0      918 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/invalid.zip
--rw-r--r--   0        0        0     2551 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/linux.txt
--rw-r--r--   0        0        0       10 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/models/bad_archive.zip
--rw-r--r--   0        0        0      376 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/models/bad_model.zip
--rw-r--r--   0        0        0      360 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/models/bar/config.yml
--rw-r--r--   0        0        0      364 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/models/foo/config.yml
--rw-r--r--   0        0        0      422 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/models/foo_archive.zip
--rw-r--r--   0        0        0     2142 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/primitive_party.proto
--rw-r--r--   0        0        0      145 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/protobufs/__init__.py
--rw-r--r--   0        0        0     2080 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/protobufs/caikit_runtime_pb2.py
--rw-r--r--   0        0        0     2447 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     2217 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
--rw-r--r--   0        0        0     2602 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
--rw-r--r--   0        0        0     5995 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/protobufs/primitive_party_pb2.py
--rw-r--r--   0        0        0      416 2023-05-22 21:25:00.873974 caikit-0.5.0/tests/fixtures/protos/caikit_runtime.proto
--rw-r--r--   0        0        0      437 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/protos/caikit_runtime_train.proto
--rw-r--r--   0        0        0       24 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      294 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/__init__.py
--rw-r--r--   0        0        0      410 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/config.yml
--rw-r--r--   0        0        0      157 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/data_model/__init__.py
--rw-r--r--   0        0        0     1257 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/data_model/sample.py
--rw-r--r--   0        0        0      156 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/modules/__init__.py
--rw-r--r--   0        0        0       89 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/modules/other_task/__init__.py
--rw-r--r--   0        0        0     1882 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/modules/other_task/other_implementation.py
--rw-r--r--   0        0        0      250 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/modules/sample_task/__init__.py
--rw-r--r--   0        0        0     1720 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/modules/sample_task/composite_module.py
--rw-r--r--   0        0        0      651 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/modules/sample_task/inner_module.py
--rw-r--r--   0        0        0     2463 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py
--rw-r--r--   0        0        0     1312 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py
--rw-r--r--   0        0        0     2720 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py
--rw-r--r--   0        0        0      364 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/fixtures/sample_module/config.yml
--rw-r--r--   0        0        0        0 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/__init__.py
--rw-r--r--   0        0        0      756 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/generated/__init__.py
--rw-r--r--   0        0        0      577 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     3845 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/metrics/test_rpc_meter.py
--rw-r--r--   0        0        0      577 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    14141 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/model_management/test_batcher.py
--rw-r--r--   0        0        0    10266 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/model_management/test_model_loader.py
--rw-r--r--   0        0        0    17911 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/model_management/test_model_manager.py
--rw-r--r--   0        0        0     5303 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/model_management/test_model_sizer.py
--rw-r--r--   0        0        0     2254 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/model_management/test_training_manager.py
--rw-r--r--   0        0        0        0 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0      577 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0     5398 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/service_generation/signature_parsing/test_docstrings.py
--rw-r--r--   0        0        0     8706 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/service_generation/signature_parsing/test_parsers.py
--rw-r--r--   0        0        0     3349 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/service_generation/test_create_service.py
--rw-r--r--   0        0        0    18431 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/service_generation/test_data_stream_source.py
--rw-r--r--   0        0        0     4065 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/service_generation/test_primitives.py
--rw-r--r--   0        0        0     1721 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/service_generation/test_rpcs.py
--rw-r--r--   0        0        0     1376 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/service_generation/test_type_helpers.py
--rw-r--r--   0        0        0      577 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     7859 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/servicers/test_global_predict_servicer_impl.py
--rw-r--r--   0        0        0    15481 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/servicers/test_global_train_servicer_impl.py
--rw-r--r--   0        0        0     3640 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/servicers/test_model_runtime_servicer_impl.py
--rw-r--r--   0        0        0     7372 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/servicers/test_model_train_servicer_impl.py
--rw-r--r--   0        0        0     4204 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/servicers/test_training_management_servicer.py
--rw-r--r--   0        0        0    30156 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/test_grpc_server.py
--rw-r--r--   0        0        0    11106 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/test_service_factory.py
--rw-r--r--   0        0        0      577 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/utils/__init__.py
--rw-r--r--   0        0        0     4899 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/utils/test_import_util.py
--rw-r--r--   0        0        0    26269 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/utils/test_servicer_util.py
--rw-r--r--   0        0        0      577 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     2758 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/work_management/test_abortable_action.py
--rw-r--r--   0        0        0     1868 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/work_management/test_call_aborter.py
--rw-r--r--   0        0        0     3355 2023-05-22 21:25:00.877969 caikit-0.5.0/tests/runtime/work_management/test_destroyable_thread.py
--rw-r--r--   0        0        0     2115 2023-05-22 21:25:00.877969 caikit-0.5.0/tox.ini
--rw-r--r--   0        0        0     4768 1970-01-01 00:00:00.000000 caikit-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-05-23 22:27:54.481803 caikit-0.5.1/.coveragerc
+-rw-r--r--   0        0        0      676 2023-05-23 22:27:54.481803 caikit-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      579 2023-05-23 22:27:54.481803 caikit-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-05-23 22:27:54.481803 caikit-0.5.1/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0        0        0      106 2023-05-23 22:27:54.481803 caikit-0.5.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1452 2023-05-23 22:27:54.481803 caikit-0.5.1/.github/workflows/build-library.yml
+-rw-r--r--   0        0        0     1328 2023-05-23 22:27:54.481803 caikit-0.5.1/.github/workflows/lint-code.yml
+-rw-r--r--   0        0        0     1136 2023-05-23 22:27:54.481803 caikit-0.5.1/.github/workflows/publish-library.yml
+-rw-r--r--   0        0        0      261 2023-05-23 22:27:54.481803 caikit-0.5.1/.gitignore
+-rw-r--r--   0        0        0      324 2023-05-23 22:27:54.481803 caikit-0.5.1/.isort.cfg
+-rw-r--r--   0        0        0      370 2023-05-23 22:27:54.481803 caikit-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      122 2023-05-23 22:27:54.481803 caikit-0.5.1/.prettierignore
+-rw-r--r--   0        0        0       12 2023-05-23 22:27:54.481803 caikit-0.5.1/.prettierrc.yaml
+-rw-r--r--   0        0        0    21434 2023-05-23 22:27:54.481803 caikit-0.5.1/.pylintrc
+-rw-r--r--   0        0        0       78 2023-05-23 22:27:54.481803 caikit-0.5.1/.whitesource
+-rw-r--r--   0        0        0      368 2023-05-23 22:27:54.481803 caikit-0.5.1/CODEOWNERS
+-rw-r--r--   0        0        0     7165 2023-05-23 22:27:54.481803 caikit-0.5.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-05-23 22:27:54.481803 caikit-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3626 2023-05-23 22:27:54.481803 caikit-0.5.1/README.md
+-rw-r--r--   0        0        0      152 2023-05-23 22:27:54.481803 caikit-0.5.1/SECURITY.md
+-rw-r--r--   0        0        0    44878 2023-05-23 22:27:54.481803 caikit-0.5.1/caikit-overview.png
+-rw-r--r--   0        0        0      427 2023-05-23 22:27:54.481803 caikit-0.5.1/caikit/__init__.py
+-rw-r--r--   0        0        0      727 2023-05-23 22:27:54.481803 caikit-0.5.1/caikit/config/__init__.py
+-rw-r--r--   0        0        0     6052 2023-05-23 22:27:54.481803 caikit-0.5.1/caikit/config/config.py
+-rw-r--r--   0        0        0     6488 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/config/config.yml
+-rw-r--r--   0        0        0     1642 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/__init__.py
+-rw-r--r--   0        0        0      812 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/augmentors/__init__.py
+-rw-r--r--   0        0        0     3506 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/augmentors/base.py
+-rw-r--r--   0        0        0     2828 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/augmentors/merged_augmentor.py
+-rw-r--r--   0        0        0      355 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/augmentors/schemes/__init__.py
+-rw-r--r--   0        0        0     2052 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/augmentors/schemes/always_selection_scheme.py
+-rw-r--r--   0        0        0     3164 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/augmentors/schemes/base.py
+-rw-r--r--   0        0        0     3264 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
+-rw-r--r--   0        0        0     2898 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/augmentors/schemes/random_single_selection_scheme.py
+-rw-r--r--   0        0        0     1027 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/data_model/__init__.py
+-rw-r--r--   0        0        0    35636 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/data_model/base.py
+-rw-r--r--   0        0        0      750 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     2207 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/data_model/data_backends/base.py
+-rw-r--r--   0        0        0     4050 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/data_model/data_backends/dict_backend.py
+-rw-r--r--   0        0        0    14380 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/data_model/dataobject.py
+-rw-r--r--   0        0        0     4858 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/data_model/enums.py
+-rw-r--r--   0        0        0     1564 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/data_model/producer.py
+-rw-r--r--   0        0        0     3914 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/data_model/protobufs/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/data_model/streams/__init__.py
+-rw-r--r--   0        0        0     5500 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/data_model/streams/converter.py
+-rw-r--r--   0        0        0     4788 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/data_model/streams/csv_column_formatter.py
+-rw-r--r--   0        0        0    40212 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/data_model/streams/data_stream.py
+-rw-r--r--   0        0        0     3606 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/data_model/streams/resolver.py
+-rw-r--r--   0        0        0     5245 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/data_model/streams/validator.py
+-rw-r--r--   0        0        0    21296 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/model_manager.py
+-rw-r--r--   0        0        0      684 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     2834 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/module_backends/backend_types.py
+-rw-r--r--   0        0        0     4718 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/module_backends/base.py
+-rw-r--r--   0        0        0     2802 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/module_backends/local_backend.py
+-rw-r--r--   0        0        0     6002 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/module_backends/module_backend_config.py
+-rw-r--r--   0        0        0      742 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/modules/__init__.py
+-rw-r--r--   0        0        0    30065 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/modules/base.py
+-rw-r--r--   0        0        0     6247 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/modules/config.py
+-rw-r--r--   0        0        0    10859 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/modules/decorator.py
+-rw-r--r--   0        0        0     4151 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/modules/loader.py
+-rw-r--r--   0        0        0     6013 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/modules/meta.py
+-rw-r--r--   0        0        0    13024 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/modules/saver.py
+-rw-r--r--   0        0        0     3895 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/registries.py
+-rw-r--r--   0        0        0     5358 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/task.py
+-rw-r--r--   0        0        0     1001 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/toolkit/__init__.py
+-rw-r--r--   0        0        0     4716 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/toolkit/compatibility.py
+-rw-r--r--   0        0        0      637 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/toolkit/errors/__init__.py
+-rw-r--r--   0        0        0    21366 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/toolkit/errors/error_handler.py
+-rw-r--r--   0        0        0     1400 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/toolkit/errors/validation_error.py
+-rw-r--r--   0        0        0     4935 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/toolkit/fileio.py
+-rw-r--r--   0        0        0     2292 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/toolkit/isa.py
+-rw-r--r--   0        0        0     1648 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/toolkit/logging.py
+-rw-r--r--   0        0        0    32206 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/toolkit/quality_evaluation.py
+-rw-r--r--   0        0        0     3439 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/toolkit/serializers.py
+-rw-r--r--   0        0        0     5979 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/core/toolkit/wip_decorator.py
+-rw-r--r--   0        0        0      530 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/interfaces/__init__.py
+-rw-r--r--   0        0        0      748 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/interfaces/common/__init__.py
+-rw-r--r--   0        0        0     1211 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/interfaces/common/data_model/__init__.py
+-rw-r--r--   0        0        0     1431 2023-05-23 22:27:54.485803 caikit-0.5.1/caikit/interfaces/common/data_model/producer.py
+-rw-r--r--   0        0        0      611 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/interfaces/runtime/__init__.py
+-rw-r--r--   0        0        0      763 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/interfaces/runtime/data_model/__init__.py
+-rw-r--r--   0        0        0     1886 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/interfaces/runtime/data_model/training_management.py
+-rw-r--r--   0        0        0      577 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/__init__.py
+-rw-r--r--   0        0        0     1827 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/dump_services.py
+-rw-r--r--   0        0        0    14200 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/grpc_server.py
+-rw-r--r--   0        0        0      577 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/interceptors/__init__.py
+-rw-r--r--   0        0        0    16502 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
+-rw-r--r--   0        0        0      577 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     4659 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/metrics/rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    17143 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/model_management/batcher.py
+-rw-r--r--   0        0        0     2648 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/model_management/loaded_model.py
+-rw-r--r--   0        0        0     5802 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/model_management/model_loader.py
+-rw-r--r--   0        0        0    12101 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/model_management/model_manager.py
+-rw-r--r--   0        0        0     4311 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/model_management/model_sizer.py
+-rw-r--r--   0        0        0     1480 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/model_management/training_manager.py
+-rw-r--r--   0        0        0      367 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/protobufs/README.md
+-rw-r--r--   0        0        0      698 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/protobufs/__init__.py
+-rw-r--r--   0        0        0    11375 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/protobufs/model_mesh_pb2.py
+-rw-r--r--   0        0        0    12846 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
+-rw-r--r--   0        0        0    10107 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/protobufs/model_runtime_pb2.py
+-rw-r--r--   0        0        0    10556 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     5535 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/protobufs/process_pb2.py
+-rw-r--r--   0        0        0     2569 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/protobufs/process_pb2_grpc.py
+-rw-r--r--   0        0        0     8844 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/protobufs/protos/model-mesh.proto
+-rw-r--r--   0        0        0     6795 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/protobufs/protos/model-runtime.proto
+-rw-r--r--   0        0        0     2479 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/protobufs/protos/process.proto
+-rw-r--r--   0        0        0    16699 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/service_factory.py
+-rw-r--r--   0        0        0      109 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     1779 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/service_generation/compatibility_checker.py
+-rw-r--r--   0        0        0     3043 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/service_generation/core_module_helpers.py
+-rw-r--r--   0        0        0     5838 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/service_generation/create_service.py
+-rw-r--r--   0        0        0    13914 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/service_generation/data_stream_source.py
+-rw-r--r--   0        0        0     7155 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/service_generation/primitives.py
+-rw-r--r--   0        0        0    12800 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/service_generation/rpcs.py
+-rw-r--r--   0        0        0      666 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/service_generation/signature_parsing/__init__.py
+-rw-r--r--   0        0        0    10747 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/service_generation/signature_parsing/docstrings.py
+-rw-r--r--   0        0        0     4794 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/service_generation/signature_parsing/module_signature.py
+-rw-r--r--   0        0        0     8225 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/service_generation/signature_parsing/parsers.py
+-rw-r--r--   0        0        0     2571 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/service_generation/type_helpers.py
+-rw-r--r--   0        0        0      577 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     9476 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/servicers/global_predict_servicer.py
+-rw-r--r--   0        0        0    15326 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/servicers/global_train_servicer.py
+-rw-r--r--   0        0        0    10637 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/servicers/model_runtime_servicer.py
+-rw-r--r--   0        0        0     5539 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/servicers/model_train_servicer.py
+-rw-r--r--   0        0        0     1667 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/servicers/training_management_servicer.py
+-rw-r--r--   0        0        0      577 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/types/__init__.py
+-rw-r--r--   0        0        0      957 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/types/aborted_exception.py
+-rw-r--r--   0        0        0     1558 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/types/caikit_runtime_exception.py
+-rw-r--r--   0        0        0      960 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/types/thread_destroyed_exception.py
+-rw-r--r--   0        0        0      577 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     6810 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/utils/import_util.py
+-rw-r--r--   0        0        0    17892 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/utils/servicer_util.py
+-rw-r--r--   0        0        0      577 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     3732 2023-05-23 22:27:54.489803 caikit-0.5.1/caikit/runtime/work_management/abortable_action.py
+-rw-r--r--   0        0        0     2969 2023-05-23 22:27:54.493803 caikit-0.5.1/caikit/runtime/work_management/call_aborter.py
+-rw-r--r--   0        0        0     7596 2023-05-23 22:27:54.493803 caikit-0.5.1/caikit/runtime/work_management/destroyable_thread.py
+-rw-r--r--   0        0        0      169 2023-05-23 22:27:54.493803 caikit-0.5.1/code-of-conduct.md
+-rw-r--r--   0        0        0       68 2023-05-23 22:27:54.493803 caikit-0.5.1/docs-requirements.txt
+-rw-r--r--   0        0        0      634 2023-05-23 22:27:54.493803 caikit-0.5.1/docs/Makefile
+-rw-r--r--   0        0        0     1610 2023-05-23 22:27:54.493803 caikit-0.5.1/docs/adrs/010-data-model-definition.md
+-rw-r--r--   0        0        0     2352 2023-05-23 22:27:54.493803 caikit-0.5.1/docs/adrs/015-runtime-service-generation.md
+-rw-r--r--   0        0        0     2581 2023-05-23 22:27:54.493803 caikit-0.5.1/docs/adrs/018-shared-backends.md
+-rw-r--r--   0        0        0     1223 2023-05-23 22:27:54.493803 caikit-0.5.1/docs/adrs/019-loader-stack.md
+-rw-r--r--   0        0        0      404 2023-05-23 22:27:54.493803 caikit-0.5.1/docs/adrs/README.md
+-rw-r--r--   0        0        0     2423 2023-05-23 22:27:54.493803 caikit-0.5.1/docs/architecture_club/04-25-23.md
+-rw-r--r--   0        0        0      342 2023-05-23 22:27:54.493803 caikit-0.5.1/docs/architecture_club/README.md
+-rw-r--r--   0        0        0     2660 2023-05-23 22:27:54.493803 caikit-0.5.1/docs/conf.py
+-rw-r--r--   0        0        0      225 2023-05-23 22:27:54.493803 caikit-0.5.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-05-23 22:27:54.493803 caikit-0.5.1/docs/make.bat
+-rw-r--r--   0        0        0      837 2023-05-23 22:27:54.493803 caikit-0.5.1/examples/start_runtime_with_sample_lib.py
+-rw-r--r--   0        0        0     6095 2023-05-23 22:27:54.493803 caikit-0.5.1/examples/text-sentiment/README.md
+-rw-r--r--   0        0        0     1425 2023-05-23 22:27:54.493803 caikit-0.5.1/examples/text-sentiment/client.py
+-rw-r--r--   0        0        0      673 2023-05-23 22:27:54.493803 caikit-0.5.1/examples/text-sentiment/models/text_sentiment/config.yml
+-rw-r--r--   0        0        0       72 2023-05-23 22:27:54.493803 caikit-0.5.1/examples/text-sentiment/requirements.txt
+-rw-r--r--   0        0        0      961 2023-05-23 22:27:54.493803 caikit-0.5.1/examples/text-sentiment/start_runtime.py
+-rw-r--r--   0        0        0      816 2023-05-23 22:27:54.493803 caikit-0.5.1/examples/text-sentiment/text_sentiment/__init__.py
+-rw-r--r--   0        0        0      742 2023-05-23 22:27:54.493803 caikit-0.5.1/examples/text-sentiment/text_sentiment/config.yml
+-rw-r--r--   0        0        0      661 2023-05-23 22:27:54.493803 caikit-0.5.1/examples/text-sentiment/text_sentiment/data_model/__init__.py
+-rw-r--r--   0        0        0     1422 2023-05-23 22:27:54.493803 caikit-0.5.1/examples/text-sentiment/text_sentiment/data_model/classification.py
+-rw-r--r--   0        0        0      645 2023-05-23 22:27:54.493803 caikit-0.5.1/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
+-rw-r--r--   0        0        0     3067 2023-05-23 22:27:54.493803 caikit-0.5.1/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py
+-rw-r--r--   0        0        0     1179 2023-05-23 22:27:57.965917 caikit-0.5.1/pyproject.toml
+-rwxr-xr-x   0        0        0      639 2023-05-23 22:27:54.493803 caikit-0.5.1/scripts/check_deps.sh
+-rwxr-xr-x   0        0        0      720 2023-05-23 22:27:54.493803 caikit-0.5.1/scripts/fmt.sh
+-rw-r--r--   0        0        0       33 2023-05-23 22:27:54.493803 caikit-0.5.1/setup_requirements.txt
+-rw-r--r--   0        0        0     1006 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/__init__.py
+-rw-r--r--   0        0        0     3439 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/base.py
+-rw-r--r--   0        0        0        0 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/config/__init__.py
+-rw-r--r--   0        0        0     5358 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/config/test_configs.py
+-rw-r--r--   0        0        0     8956 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/__init__.py
+-rw-r--r--   0        0        0     2853 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/augmentors/test_augmentor_base.py
+-rw-r--r--   0        0        0     9114 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/augmentors/test_merged_augmentors.py
+-rw-r--r--   0        0        0        0 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/data_model/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     5033 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/data_model/data_backends/test_dict_backend.py
+-rw-r--r--   0        0        0     3306 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/data_model/streams/test_converter.py
+-rw-r--r--   0        0        0     3314 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/data_model/streams/test_csv_column_formatter.py
+-rw-r--r--   0        0        0    26459 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/data_model/streams/test_data_stream.py
+-rw-r--r--   0        0        0     3498 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/data_model/streams/test_resolver.py
+-rw-r--r--   0        0        0     2908 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/data_model/streams/test_validator.py
+-rw-r--r--   0        0        0    16232 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/data_model/test_base.py
+-rw-r--r--   0        0        0    20408 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/data_model/test_dataobject.py
+-rw-r--r--   0        0        0     5083 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/data_model/test_enums.py
+-rw-r--r--   0        0        0     1104 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/data_model/test_producer.py
+-rw-r--r--   0        0        0     4357 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/helpers.py
+-rw-r--r--   0        0        0        0 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     2320 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/module_backends/test_backend_types.py
+-rw-r--r--   0        0        0     6922 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/module_backends/test_module_backend_config.py
+-rw-r--r--   0        0        0        0 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/modules/__init__.py
+-rw-r--r--   0        0        0    12293 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/modules/test_module.py
+-rw-r--r--   0        0        0     6274 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/modules/test_module_metadata.py
+-rw-r--r--   0        0        0      521 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/test_imports.py
+-rw-r--r--   0        0        0    21421 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/test_model_manager.py
+-rw-r--r--   0        0        0     1038 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/test_no_write_permissions.py
+-rw-r--r--   0        0        0     2460 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/test_task.py
+-rw-r--r--   0        0        0     7967 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/toolkit/test_compatibility.py
+-rw-r--r--   0        0        0    18396 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/toolkit/test_error_handler.py
+-rw-r--r--   0        0        0     4997 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/toolkit/test_fileio.py
+-rw-r--r--   0        0        0    25851 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/toolkit/test_quality_evaluation.py
+-rw-r--r--   0        0        0     2634 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/toolkit/test_serializers.py
+-rw-r--r--   0        0        0     7824 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/core/toolkit/test_wip_decorator.py
+-rw-r--r--   0        0        0     6782 2023-05-23 22:27:54.493803 caikit-0.5.1/tests/data_model_helpers.py
+-rw-r--r--   0        0        0       39 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      647 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/config/config.yml
+-rw-r--r--   0        0        0       27 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/data_stream_inputs/bad_file.json
+-rw-r--r--   0        0        0      154 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/data_stream_inputs/control_chars.jsonl
+-rw-r--r--   0        0        0      106 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/data_stream_inputs/sample.csv
+-rw-r--r--   0        0        0       66 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/data_stream_inputs/sample.json
+-rw-r--r--   0        0        0      233 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/data_stream_inputs/sample.jsonl
+-rw-r--r--   0        0        0     1322 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/data_stream_inputs/sample.txt
+-rw-r--r--   0        0        0       11 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
+-rw-r--r--   0        0        0       11 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
+-rw-r--r--   0        0        0       11 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
+-rw-r--r--   0        0        0       27 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
+-rw-r--r--   0        0        0       27 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
+-rw-r--r--   0        0        0       63 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
+-rw-r--r--   0        0        0      147 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
+-rw-r--r--   0        0        0      218 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
+-rw-r--r--   0        0        0       87 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
+-rw-r--r--   0        0        0       52 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
+-rw-r--r--   0        0        0       56 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
+-rw-r--r--   0        0        0       55 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
+-rw-r--r--   0        0        0      125 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/data_stream_inputs/sample_w_header.csv
+-rw-r--r--   0        0        0      222 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/dummy_dataset.json
+-rw-r--r--   0        0        0     1016 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/dummy_module.zip
+-rw-r--r--   0        0        0      675 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/dummy_module/config.yml
+-rw-r--r--   0        0        0      299 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/dummy_module/data.json
+-rw-r--r--   0        0        0       14 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/dummy_module/data.pkl
+-rw-r--r--   0        0        0      191 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/dummy_module_backend/config.yml
+-rw-r--r--   0        0        0      179 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/dummy_module_foo/config.yml
+-rw-r--r--   0        0        0      506 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/dummy_module_no_nesting.zip
+-rw-r--r--   0        0        0      570 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/dummy_module_singleton/config.yml
+-rw-r--r--   0        0        0      299 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/dummy_module_singleton/data.json
+-rw-r--r--   0        0        0       14 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/dummy_module_singleton/data.pkl
+-rw-r--r--   0        0        0      230 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/dummy_resource/config.yml
+-rw-r--r--   0        0        0     3034 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/fixtures.py
+-rw-r--r--   0        0        0      918 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/invalid.zip
+-rw-r--r--   0        0        0     2551 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/linux.txt
+-rw-r--r--   0        0        0       10 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/models/bad_archive.zip
+-rw-r--r--   0        0        0      376 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/models/bad_model.zip
+-rw-r--r--   0        0        0      360 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/models/bar/config.yml
+-rw-r--r--   0        0        0      364 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/models/foo/config.yml
+-rw-r--r--   0        0        0      422 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/models/foo_archive.zip
+-rw-r--r--   0        0        0     2142 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/primitive_party.proto
+-rw-r--r--   0        0        0      145 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/protobufs/__init__.py
+-rw-r--r--   0        0        0     2080 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/protobufs/caikit_runtime_pb2.py
+-rw-r--r--   0        0        0     2447 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     2217 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
+-rw-r--r--   0        0        0     2602 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
+-rw-r--r--   0        0        0     5995 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/protobufs/primitive_party_pb2.py
+-rw-r--r--   0        0        0      416 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/protos/caikit_runtime.proto
+-rw-r--r--   0        0        0      437 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/protos/caikit_runtime_train.proto
+-rw-r--r--   0        0        0       24 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      294 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/sample_lib/__init__.py
+-rw-r--r--   0        0        0      410 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/sample_lib/config.yml
+-rw-r--r--   0        0        0      157 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/sample_lib/data_model/__init__.py
+-rw-r--r--   0        0        0     1257 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/sample_lib/data_model/sample.py
+-rw-r--r--   0        0        0      156 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/sample_lib/modules/__init__.py
+-rw-r--r--   0        0        0       89 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/sample_lib/modules/other_task/__init__.py
+-rw-r--r--   0        0        0     1882 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/sample_lib/modules/other_task/other_implementation.py
+-rw-r--r--   0        0        0      250 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/sample_lib/modules/sample_task/__init__.py
+-rw-r--r--   0        0        0     1720 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/sample_lib/modules/sample_task/composite_module.py
+-rw-r--r--   0        0        0      651 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/sample_lib/modules/sample_task/inner_module.py
+-rw-r--r--   0        0        0     2463 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py
+-rw-r--r--   0        0        0     1312 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py
+-rw-r--r--   0        0        0     2720 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0      364 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/fixtures/sample_module/config.yml
+-rw-r--r--   0        0        0        0 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/runtime/__init__.py
+-rw-r--r--   0        0        0      756 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/runtime/generated/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     3845 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/runtime/metrics/test_rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    14141 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/runtime/model_management/test_batcher.py
+-rw-r--r--   0        0        0    10266 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/runtime/model_management/test_model_loader.py
+-rw-r--r--   0        0        0    17911 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/runtime/model_management/test_model_manager.py
+-rw-r--r--   0        0        0     5303 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/runtime/model_management/test_model_sizer.py
+-rw-r--r--   0        0        0     2254 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/runtime/model_management/test_training_manager.py
+-rw-r--r--   0        0        0        0 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/runtime/service_generation/signature_parsing/__init__.py
+-rw-r--r--   0        0        0     5398 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/runtime/service_generation/signature_parsing/test_docstrings.py
+-rw-r--r--   0        0        0     8706 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/runtime/service_generation/signature_parsing/test_parsers.py
+-rw-r--r--   0        0        0     3349 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/runtime/service_generation/test_create_service.py
+-rw-r--r--   0        0        0    18431 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/runtime/service_generation/test_data_stream_source.py
+-rw-r--r--   0        0        0     4065 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/runtime/service_generation/test_primitives.py
+-rw-r--r--   0        0        0     1721 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/runtime/service_generation/test_rpcs.py
+-rw-r--r--   0        0        0     1376 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/runtime/service_generation/test_type_helpers.py
+-rw-r--r--   0        0        0      577 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     7859 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/runtime/servicers/test_global_predict_servicer_impl.py
+-rw-r--r--   0        0        0    15481 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/runtime/servicers/test_global_train_servicer_impl.py
+-rw-r--r--   0        0        0     3640 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/runtime/servicers/test_model_runtime_servicer_impl.py
+-rw-r--r--   0        0        0     7372 2023-05-23 22:27:54.497803 caikit-0.5.1/tests/runtime/servicers/test_model_train_servicer_impl.py
+-rw-r--r--   0        0        0     4204 2023-05-23 22:27:54.501803 caikit-0.5.1/tests/runtime/servicers/test_training_management_servicer.py
+-rw-r--r--   0        0        0    30156 2023-05-23 22:27:54.501803 caikit-0.5.1/tests/runtime/test_grpc_server.py
+-rw-r--r--   0        0        0    11106 2023-05-23 22:27:54.501803 caikit-0.5.1/tests/runtime/test_service_factory.py
+-rw-r--r--   0        0        0      577 2023-05-23 22:27:54.501803 caikit-0.5.1/tests/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     4899 2023-05-23 22:27:54.501803 caikit-0.5.1/tests/runtime/utils/test_import_util.py
+-rw-r--r--   0        0        0    26269 2023-05-23 22:27:54.501803 caikit-0.5.1/tests/runtime/utils/test_servicer_util.py
+-rw-r--r--   0        0        0      577 2023-05-23 22:27:54.501803 caikit-0.5.1/tests/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     2758 2023-05-23 22:27:54.501803 caikit-0.5.1/tests/runtime/work_management/test_abortable_action.py
+-rw-r--r--   0        0        0     1868 2023-05-23 22:27:54.501803 caikit-0.5.1/tests/runtime/work_management/test_call_aborter.py
+-rw-r--r--   0        0        0     3355 2023-05-23 22:27:54.501803 caikit-0.5.1/tests/runtime/work_management/test_destroyable_thread.py
+-rw-r--r--   0        0        0     2115 2023-05-23 22:27:54.501803 caikit-0.5.1/tox.ini
+-rw-r--r--   0        0        0     4768 1970-01-01 00:00:00.000000 caikit-0.5.1/PKG-INFO
```

### Comparing `caikit-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/.github/ISSUE_TEMPLATE/user_story.md` & `caikit-0.5.1/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/.github/workflows/build-library.yml` & `caikit-0.5.1/.github/workflows/build-library.yml`

 * *Files 13% similar despite different names*

```diff
@@ -21,22 +21,30 @@
     branches: [ "main" ]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.8', '3.9', '3.10' , '3.11']
+        python-version:
+          - setup: '3.8'
+            tox: 'py38'
+          - setup: '3.9'
+            tox: 'py39'
+          - setup: '3.10'
+            tox: 'py310'
+          - setup: '3.11'
+            tox: 'py311'
 
     steps:
       - uses: actions/checkout@v3
-      - name: Set up Python ${{ matrix.python-version }}
+      - name: Set up Python ${{ matrix.python-version.setup }}
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python-version }}
+          python-version: ${{ matrix.python-version.setup }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install -r setup_requirements.txt
       - name: Build and test with tox
-        run: tox -e ${{ matrix.python-version }}
-    
+        run: tox -e ${{ matrix.python-version.tox }}
+
```

### Comparing `caikit-0.5.0/.github/workflows/lint-code.yml` & `caikit-0.5.1/.github/workflows/lint-code.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/.github/workflows/publish-library.yml` & `caikit-0.5.1/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/.pylintrc` & `caikit-0.5.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/CONTRIBUTING.md` & `caikit-0.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/LICENSE` & `caikit-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/README.md` & `caikit-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit-overview.png` & `caikit-0.5.1/caikit-overview.png`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/config/__init__.py` & `caikit-0.5.1/caikit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/config/config.py` & `caikit-0.5.1/caikit/config/config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/config/config.yml` & `caikit-0.5.1/caikit/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/__init__.py` & `caikit-0.5.1/caikit/core/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 _warnings.filterwarnings("ignore")
 
 # Local
 from .data_model import DataObjectBase, dataobject
 from .model_manager import *
 from .module_backends import *
 from .module_backends.module_backend_config import configure as backend_configure
-from .modules import ModuleBase, ModuleConfig, module
+from .modules import ModuleBase, ModuleConfig, ModuleLoader, ModuleSaver, module
 from .task import TaskBase, task
 from .toolkit import *
 
 # Configure the global model wrangling functions
 MODEL_MANAGER = ModelManager()
 extract = MODEL_MANAGER.extract
 load = MODEL_MANAGER.load
```

### Comparing `caikit-0.5.0/caikit/core/augmentors/__init__.py` & `caikit-0.5.1/caikit/core/augmentors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/augmentors/base.py` & `caikit-0.5.1/caikit/core/augmentors/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/augmentors/merged_augmentor.py` & `caikit-0.5.1/caikit/core/augmentors/merged_augmentor.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/augmentors/schemes/always_selection_scheme.py` & `caikit-0.5.1/caikit/core/augmentors/schemes/always_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/augmentors/schemes/base.py` & `caikit-0.5.1/caikit/core/augmentors/schemes/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/augmentors/schemes/random_multi_selection_scheme.py` & `caikit-0.5.1/caikit/core/augmentors/schemes/random_multi_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/augmentors/schemes/random_single_selection_scheme.py` & `caikit-0.5.1/caikit/core/augmentors/schemes/random_single_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/data_model/__init__.py` & `caikit-0.5.1/caikit/core/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/data_model/base.py` & `caikit-0.5.1/caikit/core/data_model/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -593,16 +593,17 @@
                         "protobufs `{}` does not have field `{}`".format(
                             proto.DESCRIPTOR.name, field
                         )
                     ),
                 )
 
             if field in cls._fields_primitive or field in cls._fields_enum:
-                kwargs[field] = proto_attr
-
+                # special case for oneofs
+                if field not in cls._fields_to_oneof or proto.HasField(field):
+                    kwargs[field] = proto_attr
             elif (
                 field in cls._fields_primitive_repeated
                 or field in cls._fields_enum_repeated
             ):
                 kwargs[field] = list(proto_attr)
 
             elif field in cls._fields_map:
```

### Comparing `caikit-0.5.0/caikit/core/data_model/data_backends/__init__.py` & `caikit-0.5.1/caikit/core/data_model/data_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/data_model/data_backends/base.py` & `caikit-0.5.1/caikit/core/data_model/data_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/data_model/data_backends/dict_backend.py` & `caikit-0.5.1/caikit/core/data_model/data_backends/dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/data_model/dataobject.py` & `caikit-0.5.1/caikit/core/data_model/dataobject.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/data_model/enums.py` & `caikit-0.5.1/caikit/core/data_model/enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/data_model/producer.py` & `caikit-0.5.1/caikit/core/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/data_model/protobufs/__init__.py` & `caikit-0.5.1/caikit/core/data_model/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/data_model/streams/__init__.py` & `caikit-0.5.1/caikit/core/data_model/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/data_model/streams/converter.py` & `caikit-0.5.1/caikit/core/data_model/streams/converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/data_model/streams/csv_column_formatter.py` & `caikit-0.5.1/caikit/core/data_model/streams/csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/data_model/streams/data_stream.py` & `caikit-0.5.1/caikit/core/data_model/streams/data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/data_model/streams/resolver.py` & `caikit-0.5.1/caikit/core/data_model/streams/resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/data_model/streams/validator.py` & `caikit-0.5.1/caikit/core/data_model/streams/validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/model_manager.py` & `caikit-0.5.1/caikit/core/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/module_backends/__init__.py` & `caikit-0.5.1/caikit/core/module_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/module_backends/backend_types.py` & `caikit-0.5.1/caikit/core/module_backends/backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/module_backends/base.py` & `caikit-0.5.1/caikit/core/module_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/module_backends/local_backend.py` & `caikit-0.5.1/caikit/core/module_backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/module_backends/module_backend_config.py` & `caikit-0.5.1/caikit/core/module_backends/module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/modules/__init__.py` & `caikit-0.5.1/caikit/core/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/modules/base.py` & `caikit-0.5.1/caikit/core/modules/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/modules/config.py` & `caikit-0.5.1/caikit/core/modules/config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/modules/decorator.py` & `caikit-0.5.1/caikit/core/modules/decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/modules/loader.py` & `caikit-0.5.1/caikit/core/modules/loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/modules/meta.py` & `caikit-0.5.1/caikit/core/modules/meta.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/modules/saver.py` & `caikit-0.5.1/caikit/core/modules/saver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/registries.py` & `caikit-0.5.1/caikit/core/registries.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/task.py` & `caikit-0.5.1/caikit/core/task.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/toolkit/__init__.py` & `caikit-0.5.1/caikit/core/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/toolkit/compatibility.py` & `caikit-0.5.1/caikit/core/toolkit/compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/toolkit/errors/__init__.py` & `caikit-0.5.1/caikit/core/toolkit/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/toolkit/errors/error_handler.py` & `caikit-0.5.1/caikit/core/toolkit/errors/error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/toolkit/errors/validation_error.py` & `caikit-0.5.1/caikit/core/toolkit/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/toolkit/fileio.py` & `caikit-0.5.1/caikit/core/toolkit/fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/toolkit/isa.py` & `caikit-0.5.1/caikit/core/toolkit/isa.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/toolkit/logging.py` & `caikit-0.5.1/caikit/core/toolkit/logging.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/toolkit/quality_evaluation.py` & `caikit-0.5.1/caikit/core/toolkit/quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/toolkit/serializers.py` & `caikit-0.5.1/caikit/core/toolkit/serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/core/toolkit/wip_decorator.py` & `caikit-0.5.1/caikit/core/toolkit/wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/interfaces/__init__.py` & `caikit-0.5.1/caikit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/interfaces/common/__init__.py` & `caikit-0.5.1/caikit/interfaces/common/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/interfaces/common/data_model/__init__.py` & `caikit-0.5.1/caikit/interfaces/common/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/interfaces/common/data_model/producer.py` & `caikit-0.5.1/caikit/interfaces/common/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/interfaces/runtime/__init__.py` & `caikit-0.5.1/caikit/interfaces/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/interfaces/runtime/data_model/__init__.py` & `caikit-0.5.1/caikit/interfaces/runtime/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/interfaces/runtime/data_model/training_management.py` & `caikit-0.5.1/caikit/interfaces/runtime/data_model/training_management.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/__init__.py` & `caikit-0.5.1/caikit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/dump_services.py` & `caikit-0.5.1/caikit/runtime/dump_services.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/grpc_server.py` & `caikit-0.5.1/caikit/runtime/grpc_server.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/interceptors/__init__.py` & `caikit-0.5.1/caikit/runtime/interceptors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py` & `caikit-0.5.1/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/metrics/__init__.py` & `caikit-0.5.1/caikit/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/metrics/rpc_meter.py` & `caikit-0.5.1/caikit/runtime/metrics/rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/model_management/__init__.py` & `caikit-0.5.1/caikit/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/model_management/batcher.py` & `caikit-0.5.1/caikit/runtime/model_management/batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/model_management/loaded_model.py` & `caikit-0.5.1/caikit/runtime/model_management/loaded_model.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/model_management/model_loader.py` & `caikit-0.5.1/caikit/runtime/model_management/model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/model_management/model_manager.py` & `caikit-0.5.1/caikit/runtime/model_management/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/model_management/model_sizer.py` & `caikit-0.5.1/caikit/runtime/model_management/model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/model_management/training_manager.py` & `caikit-0.5.1/caikit/runtime/model_management/training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/protobufs/__init__.py` & `caikit-0.5.1/caikit/runtime/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/protobufs/model_mesh_pb2.py` & `caikit-0.5.1/caikit/runtime/protobufs/model_mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/protobufs/model_mesh_pb2_grpc.py` & `caikit-0.5.1/caikit/runtime/protobufs/model_mesh_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/protobufs/model_runtime_pb2.py` & `caikit-0.5.1/caikit/runtime/protobufs/model_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/protobufs/model_runtime_pb2_grpc.py` & `caikit-0.5.1/caikit/runtime/protobufs/model_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/protobufs/process_pb2.py` & `caikit-0.5.1/caikit/runtime/protobufs/process_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/protobufs/process_pb2_grpc.py` & `caikit-0.5.1/caikit/runtime/protobufs/process_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/protobufs/protos/model-mesh.proto` & `caikit-0.5.1/caikit/runtime/protobufs/protos/model-mesh.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/protobufs/protos/model-runtime.proto` & `caikit-0.5.1/caikit/runtime/protobufs/protos/model-runtime.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/protobufs/protos/process.proto` & `caikit-0.5.1/caikit/runtime/protobufs/protos/process.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/service_factory.py` & `caikit-0.5.1/caikit/runtime/service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/service_generation/compatibility_checker.py` & `caikit-0.5.1/caikit/runtime/service_generation/compatibility_checker.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/service_generation/core_module_helpers.py` & `caikit-0.5.1/caikit/runtime/service_generation/core_module_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/service_generation/create_service.py` & `caikit-0.5.1/caikit/runtime/service_generation/create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/service_generation/data_stream_source.py` & `caikit-0.5.1/caikit/runtime/service_generation/data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/service_generation/primitives.py` & `caikit-0.5.1/caikit/runtime/service_generation/primitives.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/service_generation/rpcs.py` & `caikit-0.5.1/caikit/runtime/service_generation/rpcs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.5.1/caikit/runtime/service_generation/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/service_generation/signature_parsing/docstrings.py` & `caikit-0.5.1/caikit/runtime/service_generation/signature_parsing/docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/service_generation/signature_parsing/module_signature.py` & `caikit-0.5.1/caikit/runtime/service_generation/signature_parsing/module_signature.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/service_generation/signature_parsing/parsers.py` & `caikit-0.5.1/caikit/runtime/service_generation/signature_parsing/parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/service_generation/type_helpers.py` & `caikit-0.5.1/caikit/runtime/service_generation/type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/servicers/__init__.py` & `caikit-0.5.1/caikit/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/servicers/global_predict_servicer.py` & `caikit-0.5.1/caikit/runtime/servicers/global_predict_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/servicers/global_train_servicer.py` & `caikit-0.5.1/caikit/runtime/servicers/global_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/servicers/model_runtime_servicer.py` & `caikit-0.5.1/caikit/runtime/servicers/model_runtime_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/servicers/model_train_servicer.py` & `caikit-0.5.1/caikit/runtime/servicers/model_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/servicers/training_management_servicer.py` & `caikit-0.5.1/caikit/runtime/servicers/training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/types/__init__.py` & `caikit-0.5.1/caikit/runtime/types/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/types/aborted_exception.py` & `caikit-0.5.1/caikit/runtime/types/aborted_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/types/caikit_runtime_exception.py` & `caikit-0.5.1/caikit/runtime/types/caikit_runtime_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/types/thread_destroyed_exception.py` & `caikit-0.5.1/caikit/runtime/types/thread_destroyed_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/utils/__init__.py` & `caikit-0.5.1/caikit/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/utils/import_util.py` & `caikit-0.5.1/caikit/runtime/utils/import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/utils/servicer_util.py` & `caikit-0.5.1/caikit/runtime/utils/servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/work_management/__init__.py` & `caikit-0.5.1/caikit/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/work_management/abortable_action.py` & `caikit-0.5.1/caikit/runtime/work_management/abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/work_management/call_aborter.py` & `caikit-0.5.1/caikit/runtime/work_management/call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/caikit/runtime/work_management/destroyable_thread.py` & `caikit-0.5.1/caikit/runtime/work_management/destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/docs/Makefile` & `caikit-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/docs/adrs/010-data-model-definition.md` & `caikit-0.5.1/docs/adrs/010-data-model-definition.md`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/docs/adrs/015-runtime-service-generation.md` & `caikit-0.5.1/docs/adrs/015-runtime-service-generation.md`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/docs/adrs/018-shared-backends.md` & `caikit-0.5.1/docs/adrs/018-shared-backends.md`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/docs/adrs/019-loader-stack.md` & `caikit-0.5.1/docs/adrs/019-loader-stack.md`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/docs/architecture_club/04-25-23.md` & `caikit-0.5.1/docs/architecture_club/04-25-23.md`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/docs/conf.py` & `caikit-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/docs/make.bat` & `caikit-0.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/examples/start_runtime_with_sample_lib.py` & `caikit-0.5.1/examples/start_runtime_with_sample_lib.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/examples/text-sentiment/README.md` & `caikit-0.5.1/examples/text-sentiment/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/examples/text-sentiment/client.py` & `caikit-0.5.1/examples/text-sentiment/client.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/examples/text-sentiment/models/text_sentiment/config.yml` & `caikit-0.5.1/examples/text-sentiment/models/text_sentiment/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/examples/text-sentiment/start_runtime.py` & `caikit-0.5.1/examples/text-sentiment/start_runtime.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/examples/text-sentiment/text_sentiment/__init__.py` & `caikit-0.5.1/examples/text-sentiment/text_sentiment/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/examples/text-sentiment/text_sentiment/config.yml` & `caikit-0.5.1/examples/text-sentiment/text_sentiment/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/examples/text-sentiment/text_sentiment/data_model/__init__.py` & `caikit-0.5.1/examples/text-sentiment/text_sentiment/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/examples/text-sentiment/text_sentiment/data_model/classification.py` & `caikit-0.5.1/examples/text-sentiment/text_sentiment/data_model/classification.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/examples/text-sentiment/text_sentiment/runtime_model/__init__.py` & `caikit-0.5.1/examples/text-sentiment/text_sentiment/runtime_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py` & `caikit-0.5.1/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/pyproject.toml` & `caikit-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "caikit"
 # Not the actual current version: overwritten by CI
-version = "0.5.0"
+version = "0.5.1"
 description = "AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework"
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = "~=3.8"
 classifiers=[
     "License :: OSI Approved :: Apache Software License"
 ]
```

### Comparing `caikit-0.5.0/scripts/check_deps.sh` & `caikit-0.5.1/scripts/check_deps.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/scripts/fmt.sh` & `caikit-0.5.1/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/__init__.py` & `caikit-0.5.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/base.py` & `caikit-0.5.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/config/test_configs.py` & `caikit-0.5.1/tests/config/test_configs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/conftest.py` & `caikit-0.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/augmentors/test_augmentor_base.py` & `caikit-0.5.1/tests/core/augmentors/test_augmentor_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/augmentors/test_merged_augmentors.py` & `caikit-0.5.1/tests/core/augmentors/test_merged_augmentors.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/data_model/data_backends/test_dict_backend.py` & `caikit-0.5.1/tests/core/data_model/data_backends/test_dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/data_model/streams/test_converter.py` & `caikit-0.5.1/tests/core/data_model/streams/test_converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/data_model/streams/test_csv_column_formatter.py` & `caikit-0.5.1/tests/core/data_model/streams/test_csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/data_model/streams/test_data_stream.py` & `caikit-0.5.1/tests/core/data_model/streams/test_data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/data_model/streams/test_resolver.py` & `caikit-0.5.1/tests/core/data_model/streams/test_resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/data_model/streams/test_validator.py` & `caikit-0.5.1/tests/core/data_model/streams/test_validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/data_model/test_base.py` & `caikit-0.5.1/tests/core/data_model/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/data_model/test_dataobject.py` & `caikit-0.5.1/tests/core/data_model/test_dataobject.py`

 * *Files 3% similar despite different names*

```diff
@@ -455,14 +455,42 @@
     # unless set explicitly
     foo2 = Foo(foo_bool2=True)
     assert foo2.which_oneof("foo") == "foo_bool2"
     assert foo2.foo_bool1 == None
     assert foo2.foo_bool2
 
 
+def test_dataobject_primitive_oneof_round_trips():
+    @dataobject
+    class Foo(DataObjectBase):
+        foo: Union[
+            Annotated[int, FieldNumber(10), OneofField("foo_int")],
+            Annotated[float, FieldNumber(20), OneofField("foo_float")],
+        ]
+
+    # proto round trip
+    foo1 = Foo(foo_int=2)
+    assert foo1.which_oneof("foo") == "foo_int"
+    proto_repr_foo = foo1.to_proto()
+    assert Foo.from_proto(proto=proto_repr_foo).to_proto() == proto_repr_foo
+
+    foo2 = Foo(foo=2)
+    assert foo2.which_oneof("foo") == "foo_int"
+    proto_repr_foo = foo2.to_proto()
+    assert Foo.from_proto(proto=proto_repr_foo).to_proto() == proto_repr_foo
+
+    # json round trip
+    json_repr_foo = foo1.to_json()
+    assert json.loads(json_repr_foo) == {
+        "foo_int": 2,
+        "foo_float": None,
+    }
+    assert Foo.from_json(json_repr_foo) == foo1
+
+
 def test_dataobject_round_trip_json():
     """Make sure that a dataobject class can serialize to/from json"""
 
     @dataobject
     class BazObj(DataObjectBase):
         foo: str
         bar: int
```

### Comparing `caikit-0.5.0/tests/core/data_model/test_enums.py` & `caikit-0.5.1/tests/core/data_model/test_enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/data_model/test_producer.py` & `caikit-0.5.1/tests/core/data_model/test_producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/helpers.py` & `caikit-0.5.1/tests/core/helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/module_backends/test_backend_types.py` & `caikit-0.5.1/tests/core/module_backends/test_backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/module_backends/test_module_backend_config.py` & `caikit-0.5.1/tests/core/module_backends/test_module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/modules/test_module.py` & `caikit-0.5.1/tests/core/modules/test_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/modules/test_module_metadata.py` & `caikit-0.5.1/tests/core/modules/test_module_metadata.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/test_imports.py` & `caikit-0.5.1/tests/core/test_imports.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/test_model_manager.py` & `caikit-0.5.1/tests/core/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/test_no_write_permissions.py` & `caikit-0.5.1/tests/core/test_no_write_permissions.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/test_task.py` & `caikit-0.5.1/tests/core/test_task.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/toolkit/test_compatibility.py` & `caikit-0.5.1/tests/core/toolkit/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/toolkit/test_error_handler.py` & `caikit-0.5.1/tests/core/toolkit/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/toolkit/test_fileio.py` & `caikit-0.5.1/tests/core/toolkit/test_fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/toolkit/test_quality_evaluation.py` & `caikit-0.5.1/tests/core/toolkit/test_quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/toolkit/test_serializers.py` & `caikit-0.5.1/tests/core/toolkit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/core/toolkit/test_wip_decorator.py` & `caikit-0.5.1/tests/core/toolkit/test_wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/data_model_helpers.py` & `caikit-0.5.1/tests/data_model_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/fixtures/config/config.yml` & `caikit-0.5.1/tests/fixtures/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/fixtures/data_stream_inputs/sample.txt` & `caikit-0.5.1/tests/fixtures/data_stream_inputs/sample.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/fixtures/dummy_module.zip` & `caikit-0.5.1/tests/fixtures/dummy_module.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/fixtures/dummy_module/config.yml` & `caikit-0.5.1/tests/fixtures/dummy_module/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/fixtures/dummy_module_singleton/config.yml` & `caikit-0.5.1/tests/fixtures/dummy_module_singleton/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/fixtures/fixtures.py` & `caikit-0.5.1/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/fixtures/invalid.zip` & `caikit-0.5.1/tests/fixtures/invalid.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/fixtures/linux.txt` & `caikit-0.5.1/tests/fixtures/linux.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/fixtures/primitive_party.proto` & `caikit-0.5.1/tests/fixtures/primitive_party.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/fixtures/protobufs/caikit_runtime_pb2.py` & `caikit-0.5.1/tests/fixtures/protobufs/caikit_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py` & `caikit-0.5.1/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/fixtures/protobufs/caikit_runtime_train_pb2.py` & `caikit-0.5.1/tests/fixtures/protobufs/caikit_runtime_train_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py` & `caikit-0.5.1/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/fixtures/protobufs/primitive_party_pb2.py` & `caikit-0.5.1/tests/fixtures/protobufs/primitive_party_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/fixtures/sample_lib/data_model/sample.py` & `caikit-0.5.1/tests/fixtures/sample_lib/data_model/sample.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/fixtures/sample_lib/modules/other_task/other_implementation.py` & `caikit-0.5.1/tests/fixtures/sample_lib/modules/other_task/other_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/fixtures/sample_lib/modules/sample_task/composite_module.py` & `caikit-0.5.1/tests/fixtures/sample_lib/modules/sample_task/composite_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/fixtures/sample_lib/modules/sample_task/inner_module.py` & `caikit-0.5.1/tests/fixtures/sample_lib/modules/sample_task/inner_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py` & `caikit-0.5.1/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py` & `caikit-0.5.1/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py` & `caikit-0.5.1/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/generated/__init__.py` & `caikit-0.5.1/tests/runtime/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/metrics/__init__.py` & `caikit-0.5.1/tests/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/metrics/test_rpc_meter.py` & `caikit-0.5.1/tests/runtime/metrics/test_rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/model_management/__init__.py` & `caikit-0.5.1/tests/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/model_management/test_batcher.py` & `caikit-0.5.1/tests/runtime/model_management/test_batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/model_management/test_model_loader.py` & `caikit-0.5.1/tests/runtime/model_management/test_model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/model_management/test_model_manager.py` & `caikit-0.5.1/tests/runtime/model_management/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/model_management/test_model_sizer.py` & `caikit-0.5.1/tests/runtime/model_management/test_model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/model_management/test_training_manager.py` & `caikit-0.5.1/tests/runtime/model_management/test_training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.5.1/tests/runtime/service_generation/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/service_generation/signature_parsing/test_docstrings.py` & `caikit-0.5.1/tests/runtime/service_generation/signature_parsing/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/service_generation/signature_parsing/test_parsers.py` & `caikit-0.5.1/tests/runtime/service_generation/signature_parsing/test_parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/service_generation/test_create_service.py` & `caikit-0.5.1/tests/runtime/service_generation/test_create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/service_generation/test_data_stream_source.py` & `caikit-0.5.1/tests/runtime/service_generation/test_data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/service_generation/test_primitives.py` & `caikit-0.5.1/tests/runtime/service_generation/test_primitives.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/service_generation/test_rpcs.py` & `caikit-0.5.1/tests/runtime/service_generation/test_rpcs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/service_generation/test_type_helpers.py` & `caikit-0.5.1/tests/runtime/service_generation/test_type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/servicers/__init__.py` & `caikit-0.5.1/tests/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/servicers/test_global_predict_servicer_impl.py` & `caikit-0.5.1/tests/runtime/servicers/test_global_predict_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/servicers/test_global_train_servicer_impl.py` & `caikit-0.5.1/tests/runtime/servicers/test_global_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/servicers/test_model_runtime_servicer_impl.py` & `caikit-0.5.1/tests/runtime/servicers/test_model_runtime_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/servicers/test_model_train_servicer_impl.py` & `caikit-0.5.1/tests/runtime/servicers/test_model_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/servicers/test_training_management_servicer.py` & `caikit-0.5.1/tests/runtime/servicers/test_training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/test_grpc_server.py` & `caikit-0.5.1/tests/runtime/test_grpc_server.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/test_service_factory.py` & `caikit-0.5.1/tests/runtime/test_service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/utils/__init__.py` & `caikit-0.5.1/tests/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/utils/test_import_util.py` & `caikit-0.5.1/tests/runtime/utils/test_import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/utils/test_servicer_util.py` & `caikit-0.5.1/tests/runtime/utils/test_servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/work_management/__init__.py` & `caikit-0.5.1/tests/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/work_management/test_abortable_action.py` & `caikit-0.5.1/tests/runtime/work_management/test_abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/work_management/test_call_aborter.py` & `caikit-0.5.1/tests/runtime/work_management/test_call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tests/runtime/work_management/test_destroyable_thread.py` & `caikit-0.5.1/tests/runtime/work_management/test_destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/tox.ini` & `caikit-0.5.1/tox.ini`

 * *Files identical despite different names*

### Comparing `caikit-0.5.0/PKG-INFO` & `caikit-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caikit
-Version: 0.5.0
+Version: 0.5.1
 Summary: AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: alchemy-config>=1.1.1,<2.0.0
 Requires-Dist: alchemy-logging>=1.0.4,<2.0.0
 Requires-Dist: anytree>=2.7.0,<3.0
```

