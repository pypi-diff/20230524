# Comparing `tmp/cengal-3.2.0.tar.gz` & `tmp/cengal-3.2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cengal-3.2.0.tar", last modified: Mon May 22 08:06:23 2023, max compression
+gzip compressed data, was "cengal-3.2.0.1.tar", last modified: Tue May 23 21:58:27 2023, max compression
```

## Comparing `cengal-3.2.0.tar` & `cengal-3.2.0.1.tar`

### file list

```diff
@@ -1,1893 +1,1893 @@
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:23.179190 cengal-3.2.0/
--rw-r--r--   0 mb        (1000) mb        (1000)    11358 2022-04-21 11:25:54.000000 cengal-3.2.0/LICENSE.md
--rw-r--r--   0 mb        (1000) mb        (1000)      614 2022-11-01 20:15:42.000000 cengal-3.2.0/NOTICE
--rw-r--r--   0 mb        (1000) mb        (1000)    27214 2023-05-22 08:06:23.169190 cengal-3.2.0/PKG-INFO
--rw-r--r--   0 mb        (1000) mb        (1000)    22105 2023-05-22 07:55:08.000000 cengal-3.2.0/README.md
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.359192 cengal-3.2.0/cengal/
--rw-r--r--   0 mb        (1000) mb        (1000)     8227 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/RequestCache.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2760 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/ServerClock.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.399192 cengal-3.2.0/cengal/base/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/base/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.429192 cengal-3.2.0/cengal/base/classes/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/base/classes/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.429192 cengal-3.2.0/cengal/base/classes/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/base/classes/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.439192 cengal-3.2.0/cengal/base/classes/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/base/classes/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1266 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/base/classes/versions/v_0/classes.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.449192 cengal-3.2.0/cengal/base/classes/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/base/classes/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/base/classes/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.449192 cengal-3.2.0/cengal/base/exceptions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/base/exceptions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.459192 cengal-3.2.0/cengal/base/exceptions/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/base/exceptions/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.479192 cengal-3.2.0/cengal/base/exceptions/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/base/exceptions/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1302 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/base/exceptions/versions/v_0/exceptions.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.489192 cengal-3.2.0/cengal/base/exceptions/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/base/exceptions/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/base/exceptions/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.489192 cengal-3.2.0/cengal/build_tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1209 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/build_tools/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.489192 cengal-3.2.0/cengal/build_tools/current_compiler/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/build_tools/current_compiler/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.489192 cengal-3.2.0/cengal/build_tools/current_compiler/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/build_tools/current_compiler/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.509192 cengal-3.2.0/cengal/build_tools/current_compiler/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/build_tools/current_compiler/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2161 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/build_tools/current_compiler/versions/v_0/current_compiler.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.519192 cengal-3.2.0/cengal/build_tools/current_compiler/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/build_tools/current_compiler/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/build_tools/current_compiler/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.519192 cengal-3.2.0/cengal/build_tools/prepare_cflags/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/build_tools/prepare_cflags/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.519192 cengal-3.2.0/cengal/build_tools/prepare_cflags/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/build_tools/prepare_cflags/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.539192 cengal-3.2.0/cengal/build_tools/prepare_cflags/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/build_tools/prepare_cflags/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    14723 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/build_tools/prepare_cflags/versions/v_0/prepare_cflags.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.539192 cengal-3.2.0/cengal/build_tools/prepare_cflags/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/build_tools/prepare_cflags/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/build_tools/prepare_cflags/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.559192 cengal-3.2.0/cengal/bulk_pip_actions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/bulk_pip_actions/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6286 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/bulk_pip_actions/bulk_install.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6022 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/bulk_pip_actions/install.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1279 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/check_is_in_pycharm.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.559192 cengal-3.2.0/cengal/code_flow_control/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/code_flow_control/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.569192 cengal-3.2.0/cengal/code_flow_control/args_manager/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/code_flow_control/args_manager/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.569192 cengal-3.2.0/cengal/code_flow_control/args_manager/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/code_flow_control/args_manager/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.589192 cengal-3.2.0/cengal/code_flow_control/args_manager/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/code_flow_control/args_manager/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    16576 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/code_flow_control/args_manager/versions/v_0/args_manager.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.609192 cengal-3.2.0/cengal/code_flow_control/args_manager/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/code_flow_control/args_manager/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    17266 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/code_flow_control/args_manager/versions/v_0/tests/_manual_test__args_manager.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/code_flow_control/args_manager/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.619192 cengal-3.2.0/cengal/code_flow_control/call_history_reapplier/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/code_flow_control/call_history_reapplier/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.619192 cengal-3.2.0/cengal/code_flow_control/call_history_reapplier/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/code_flow_control/call_history_reapplier/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.639192 cengal-3.2.0/cengal/code_flow_control/call_history_reapplier/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1244 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/code_flow_control/call_history_reapplier/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2769 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/code_flow_control/call_history_reapplier/versions/v_0/call_history_reapplier.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.659192 cengal-3.2.0/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.659192 cengal-3.2.0/cengal/code_flow_control/chained_flow/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/code_flow_control/chained_flow/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.669192 cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.689192 cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-22 07:55:08.000000 cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    36470 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/v_0/smart_chain.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.709192 cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    32961 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/v_0/tests/example_for__chained_flow.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.719192 cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    35217 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/v_1/chained_flow.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.739192 cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/v_1/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    32961 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/v_1/tests/example_for__chained_flow.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.749192 cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.749192 cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.769192 cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    23327 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/versions/v_0/essence.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.799192 cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2881 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2623 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/quadrangle.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1372 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/quadrangle_test.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3466 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4070 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle_test.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4391 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle_test_old.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.809192 cengal-3.2.0/cengal/code_flow_control/none_or/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/none_or/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.809192 cengal-3.2.0/cengal/code_flow_control/none_or/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/none_or/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.819192 cengal-3.2.0/cengal/code_flow_control/none_or/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/none_or/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1486 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/none_or/versions/v_0/none_or.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.829192 cengal-3.2.0/cengal/code_flow_control/none_or/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/none_or/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/none_or/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.839192 cengal-3.2.0/cengal/code_flow_control/python_bytecode_manipulator/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/python_bytecode_manipulator/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.839192 cengal-3.2.0/cengal/code_flow_control/python_bytecode_manipulator/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/python_bytecode_manipulator/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.849192 cengal-3.2.0/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1249 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    29754 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/python_bytecode_manipulator.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.859192 cengal-3.2.0/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.869192 cengal-3.2.0/cengal/code_flow_control/smart_values/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/smart_values/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.869192 cengal-3.2.0/cengal/code_flow_control/smart_values/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/smart_values/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.869192 cengal-3.2.0/cengal/code_flow_control/smart_values/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/smart_values/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2827 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/smart_values/versions/v_0/result_types.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.889191 cengal-3.2.0/cengal/code_flow_control/smart_values/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/smart_values/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2838 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/smart_values/versions/v_1/smart_values.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.889191 cengal-3.2.0/cengal/code_flow_control/smart_values/versions/v_2/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/smart_values/versions/v_2/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3469 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_flow_control/smart_values/versions/v_2/smart_values.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.889191 cengal-3.2.0/cengal/code_inspection/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_inspection/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.909191 cengal-3.2.0/cengal/code_inspection/auto_line_tracer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_inspection/auto_line_tracer/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.909191 cengal-3.2.0/cengal/code_inspection/auto_line_tracer/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_inspection/auto_line_tracer/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.919191 cengal-3.2.0/cengal/code_inspection/auto_line_tracer/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_inspection/auto_line_tracer/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6170 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_inspection/auto_line_tracer/versions/v_0/auto_line_tracer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.929191 cengal-3.2.0/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.939191 cengal-3.2.0/cengal/code_inspection/line_profiling/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_inspection/line_profiling/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.939191 cengal-3.2.0/cengal/code_inspection/line_profiling/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_inspection/line_profiling/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.949191 cengal-3.2.0/cengal/code_inspection/line_profiling/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_inspection/line_profiling/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2769 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_inspection/line_profiling/versions/v_0/line_profiling.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.949191 cengal-3.2.0/cengal/code_inspection/line_profiling/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_inspection/line_profiling/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_inspection/line_profiling/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.959191 cengal-3.2.0/cengal/code_inspection/line_tracer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_inspection/line_tracer/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.959191 cengal-3.2.0/cengal/code_inspection/line_tracer/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_inspection/line_tracer/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.969191 cengal-3.2.0/cengal/code_inspection/line_tracer/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_inspection/line_tracer/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4304 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_inspection/line_tracer/versions/v_0/line_tracer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.979191 cengal-3.2.0/cengal/code_inspection/line_tracer/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_inspection/line_tracer/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/code_inspection/line_tracer/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.989191 cengal-3.2.0/cengal/cross_version/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/cross_version/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.999191 cengal-3.2.0/cengal/cross_version/console_print/
--rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/cross_version/console_print/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1263 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/cross_version/console_print/python3.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1528 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/cross_version/console_print/universal.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.999191 cengal-3.2.0/cengal/ctypes_tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1209 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.009191 cengal-3.2.0/cengal/ctypes_tools/constants/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/constants/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.009191 cengal-3.2.0/cengal/ctypes_tools/constants/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/constants/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.039191 cengal-3.2.0/cengal/ctypes_tools/constants/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1269 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/constants/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.059191 cengal-3.2.0/cengal/ctypes_tools/constants/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/constants/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/constants/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    13437 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/constants/versions/v_0/win_constants.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.079191 cengal-3.2.0/cengal/ctypes_tools/function_prototypes/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/function_prototypes/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.079191 cengal-3.2.0/cengal/ctypes_tools/function_prototypes/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/function_prototypes/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.079191 cengal-3.2.0/cengal/ctypes_tools/function_prototypes/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1279 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/function_prototypes/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.089191 cengal-3.2.0/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5487 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/function_prototypes/versions/v_0/win_function_prototypes.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.089191 cengal-3.2.0/cengal/ctypes_tools/functions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/functions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.119191 cengal-3.2.0/cengal/ctypes_tools/functions/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/functions/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.139191 cengal-3.2.0/cengal/ctypes_tools/functions/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1295 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/functions/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1316 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/functions/versions/v_0/functions.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.139191 cengal-3.2.0/cengal/ctypes_tools/functions/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/functions/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/functions/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1501 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/functions/versions/v_0/win_functions.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.139191 cengal-3.2.0/cengal/ctypes_tools/libraries/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/libraries/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.169191 cengal-3.2.0/cengal/ctypes_tools/libraries/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/libraries/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.169191 cengal-3.2.0/cengal/ctypes_tools/libraries/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1269 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/libraries/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.189191 cengal-3.2.0/cengal/ctypes_tools/libraries/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/libraries/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/libraries/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1481 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/libraries/versions/v_0/win_libraries.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.189191 cengal-3.2.0/cengal/ctypes_tools/result_api/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/result_api/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.209191 cengal-3.2.0/cengal/ctypes_tools/result_api/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/result_api/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.259191 cengal-3.2.0/cengal/ctypes_tools/result_api/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1335 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/result_api/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1221 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/result_api/versions/v_0/result_api.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1304 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/result_api/versions/v_0/result_api_exceptions.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.259191 cengal-3.2.0/cengal/ctypes_tools/result_api/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/result_api/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/result_api/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2728 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/result_api/versions/v_0/win_result_api.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.259191 cengal-3.2.0/cengal/ctypes_tools/tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/tools/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.259191 cengal-3.2.0/cengal/ctypes_tools/tools/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/tools/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.259191 cengal-3.2.0/cengal/ctypes_tools/tools/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1287 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/tools/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.269191 cengal-3.2.0/cengal/ctypes_tools/tools/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/tools/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/tools/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1596 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/tools/versions/v_0/tools.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1600 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/tools/versions/v_0/win_tools.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.269191 cengal-3.2.0/cengal/ctypes_tools/types/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/types/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.269191 cengal-3.2.0/cengal/ctypes_tools/types/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/types/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.269191 cengal-3.2.0/cengal/ctypes_tools/types/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1265 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/types/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.269191 cengal-3.2.0/cengal/ctypes_tools/types/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/types/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/types/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7772 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/ctypes_tools/types/versions/v_0/win_types.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.269191 cengal-3.2.0/cengal/cython_tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/cython_tools/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1773 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/cython_tools/cythonyser_setup_runner.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.319191 cengal-3.2.0/cengal/data_containers/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.319191 cengal-3.2.0/cengal/data_containers/compound_dict_management/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/compound_dict_management/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.319191 cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.339191 cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.339191 cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2228 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/versions/v_0/manager.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.369191 cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.369191 cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2211 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/versions/v_1/manager.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.389191 cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.389191 cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/
--rw-r--r--   0 mb        (1000) mb        (1000)     1278 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.389191 cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.389191 cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.389191 cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1251 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1541 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/key__hashable__to__value__set.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.389191 cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.389191 cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key_counter/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key_counter/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.389191 cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.389191 cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1597 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/key_counter.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.439191 cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.439191 cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.459191 cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.459191 cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1624 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    24426 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/dynamic_list_of_pieces__cython.pyx
--rw-r--r--   0 mb        (1000) mb        (1000)    28853 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/dynamic_list_of_pieces__python.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.459191 cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.459191 cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1624 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    24390 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/dynamic_list_of_pieces__cython.pyx
--rw-r--r--   0 mb        (1000) mb        (1000)    28796 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/dynamic_list_of_pieces__python.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.459191 cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.459191 cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.459191 cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.499191 cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)    39955 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_0/TagDB.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1259 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5404 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_0/tag_db_interface.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.519191 cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.529191 cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)    41894 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_1/TagDB.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1259 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    13149 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_1/tag_db_interface.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.569191 cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.589191 cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_2/
--rw-r--r--   0 mb        (1000) mb        (1000)     1259 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_2/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     9729 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_2/dynamic_tag_tree.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.589191 cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.599191 cengal-3.2.0/cengal/data_containers/fast_fifo/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/fast_fifo/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.599191 cengal-3.2.0/cengal/data_containers/fast_fifo/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/fast_fifo/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.599191 cengal-3.2.0/cengal/data_containers/fast_fifo/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/fast_fifo/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    12327 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/fast_fifo/versions/v_0/fast_fifo.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.599191 cengal-3.2.0/cengal/data_containers/fast_fifo/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/fast_fifo/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/fast_fifo/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.599191 cengal-3.2.0/cengal/data_containers/fast_fifo/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/fast_fifo/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    12275 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/fast_fifo/versions/v_1/fast_fifo.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.669191 cengal-3.2.0/cengal/data_containers/fast_fifo/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/fast_fifo/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/fast_fifo/versions/v_1/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.679191 cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.679191 cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.679191 cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2033 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/versions/v_0/limitable_dict_with_order.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.679191 cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.689191 cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2464 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/versions/v_1/limitable_dict_with_order.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.699191 cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.699191 cengal-3.2.0/cengal/data_containers/simple_tree/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/simple_tree/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.699191 cengal-3.2.0/cengal/data_containers/simple_tree/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/simple_tree/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.729191 cengal-3.2.0/cengal/data_containers/simple_tree/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/simple_tree/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5000 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/simple_tree/versions/v_0/simple_tree.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.729191 cengal-3.2.0/cengal/data_containers/stack/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/stack/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.729191 cengal-3.2.0/cengal/data_containers/stack/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/stack/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.729191 cengal-3.2.0/cengal/data_containers/stack/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1227 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/stack/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4659 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/stack/versions/v_0/stack.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.749191 cengal-3.2.0/cengal/data_containers/stack/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/stack/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3695 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_containers/stack/versions/v_0/tests/test__stack.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.759191 cengal-3.2.0/cengal/data_generation/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_generation/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.769191 cengal-3.2.0/cengal/data_generation/id_generator/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_generation/id_generator/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.789191 cengal-3.2.0/cengal/data_generation/id_generator/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_generation/id_generator/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.789191 cengal-3.2.0/cengal/data_generation/id_generator/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_generation/id_generator/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2217 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_generation/id_generator/versions/v_0/id_generator.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.799191 cengal-3.2.0/cengal/data_generation/id_generator/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_generation/id_generator/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_generation/id_generator/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.819191 cengal-3.2.0/cengal/data_generation/id_generator/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_generation/id_generator/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3044 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_generation/id_generator/versions/v_1/id_generator.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.859191 cengal-3.2.0/cengal/data_generation/id_generator/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_generation/id_generator/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_generation/id_generator/versions/v_1/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.879191 cengal-3.2.0/cengal/data_manipulation/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.889191 cengal-3.2.0/cengal/data_manipulation/conversion/
--rw-r--r--   0 mb        (1000) mb        (1000)     1209 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.899191 cengal-3.2.0/cengal/data_manipulation/conversion/bit_cast_like/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/bit_cast_like/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.899191 cengal-3.2.0/cengal/data_manipulation/conversion/bit_cast_like/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/bit_cast_like/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.909191 cengal-3.2.0/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2011 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/bit_cast_like.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.919191 cengal-3.2.0/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.919191 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.949191 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.959191 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2475 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/reinterpret_cast.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.989191 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.989191 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/
--rw-r--r--   0 mb        (1000) mb        (1000)     1209 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.989191 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:09.999191 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.019191 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8110 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/manager.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.019191 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.029191 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/
--rw-r--r--   0 mb        (1000) mb        (1000)     1209 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.039191 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.039191 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.059191 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2548 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/copy_wrapper.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.069191 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.069191 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.069191 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.089191 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2564 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/deep_copy_wrapper.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.089191 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.089191 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.099191 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.119191 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.139191 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3538 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/uni_copy_wrapper.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.149191 cengal-3.2.0/cengal/data_manipulation/front_triggerable_variable/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/front_triggerable_variable/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.159191 cengal-3.2.0/cengal/data_manipulation/front_triggerable_variable/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/front_triggerable_variable/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.179190 cengal-3.2.0/cengal/data_manipulation/front_triggerable_variable/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/front_triggerable_variable/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3916 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/front_triggerable_variable/versions/v_0/front_triggerable_variable.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.189190 cengal-3.2.0/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.189190 cengal-3.2.0/cengal/data_manipulation/get_dict_key_with_callable_default/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/get_dict_key_with_callable_default/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.199190 cengal-3.2.0/cengal/data_manipulation/get_dict_key_with_callable_default/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/get_dict_key_with_callable_default/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.219190 cengal-3.2.0/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1256 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1483 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/get_dict_key_with_callable_default.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.259190 cengal-3.2.0/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7544 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/help_tools.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.259190 cengal-3.2.0/cengal/data_manipulation/objects_counter/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/objects_counter/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.269190 cengal-3.2.0/cengal/data_manipulation/objects_counter/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/objects_counter/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.279190 cengal-3.2.0/cengal/data_manipulation/objects_counter/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/objects_counter/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2980 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/objects_counter/versions/v_0/objects_counter.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.289190 cengal-3.2.0/cengal/data_manipulation/objects_counter/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1243 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/objects_counter/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6511 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/objects_counter/versions/v_0/tests/test__objects_counter.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.289190 cengal-3.2.0/cengal/data_manipulation/performant_list_operations/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/performant_list_operations/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.289190 cengal-3.2.0/cengal/data_manipulation/performant_list_operations/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/performant_list_operations/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.309190 cengal-3.2.0/cengal/data_manipulation/performant_list_operations/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1244 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/performant_list_operations/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     9310 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/performant_list_operations/versions/v_0/remove_items_from_list.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.309190 cengal-3.2.0/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.319190 cengal-3.2.0/cengal/data_manipulation/serialization/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/serialization/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.319190 cengal-3.2.0/cengal/data_manipulation/serialization/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/serialization/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.319190 cengal-3.2.0/cengal/data_manipulation/serialization/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/serialization/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    27320 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/serialization/versions/v_0/serialization.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.329190 cengal-3.2.0/cengal/data_manipulation/serialization/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1241 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/serialization/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4070 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/serialization/versions/v_0/tests/test__serialization.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.339190 cengal-3.2.0/cengal/data_manipulation/tree_traversal/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/tree_traversal/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.349190 cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.359190 cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.399190 cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2651 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_0/tests/traverstal_manual_tests.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8191 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_0/tree_traversal.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.419190 cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_1/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.459190 cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_1/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2614 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_1/tests/key_multi_value_traverstal_manual_tests.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2813 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_1/tests/key_value_traverstal_manual_tests.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2746 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_1/tests/traverstal_manual_tests.py
--rw-r--r--   0 mb        (1000) mb        (1000)    24127 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_1/tree_traversal.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5495 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/docten.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.459190 cengal-3.2.0/cengal/entities/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/entities/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.459190 cengal-3.2.0/cengal/entities/bindable_to_type/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/entities/bindable_to_type/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.479190 cengal-3.2.0/cengal/entities/bindable_to_type/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/entities/bindable_to_type/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.479190 cengal-3.2.0/cengal/entities/bindable_to_type/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/entities/bindable_to_type/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4359 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/entities/bindable_to_type/versions/v_0/bindable_to_type.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.479190 cengal-3.2.0/cengal/entities/bindable_to_type/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/entities/bindable_to_type/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/entities/bindable_to_type/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.499190 cengal-3.2.0/cengal/entities/copyable/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/entities/copyable/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.499190 cengal-3.2.0/cengal/entities/copyable/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/entities/copyable/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.509190 cengal-3.2.0/cengal/entities/copyable/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/entities/copyable/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4449 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/entities/copyable/versions/v_0/copyable.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.539190 cengal-3.2.0/cengal/entities/copyable/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/entities/copyable/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/entities/copyable/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.549190 cengal-3.2.0/cengal/file_settings_manager/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_settings_manager/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7335 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_settings_manager/config_manager.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_settings_manager/dir_templates.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.559190 cengal-3.2.0/cengal/file_system/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.569190 cengal-3.2.0/cengal/file_system/app_fs_structure/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/app_fs_structure/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.569190 cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.579190 cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.649190 cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1547 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1288 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_exceptions.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4301 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_base.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8623 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_darwin.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8512 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_linux.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7082 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_win.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3824 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_directory_types.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.659190 cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8150 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/directory_manager.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2528 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/file_manager.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.659190 cengal-3.2.0/cengal/file_system/file_patch/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/file_patch/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.679190 cengal-3.2.0/cengal/file_system/file_patch/brackets/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/file_patch/brackets/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.679190 cengal-3.2.0/cengal/file_system/file_patch/brackets/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/file_patch/brackets/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.689190 cengal-3.2.0/cengal/file_system/file_patch/brackets/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/file_patch/brackets/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2365 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/file_patch/brackets/versions/v_0/brackets.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.709190 cengal-3.2.0/cengal/file_system/file_patch/brackets/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/file_patch/brackets/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/file_patch/brackets/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.709190 cengal-3.2.0/cengal/file_system/file_patch/generic/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/file_patch/generic/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.709190 cengal-3.2.0/cengal/file_system/file_patch/generic/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/file_patch/generic/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.739190 cengal-3.2.0/cengal/file_system/file_patch/generic/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/file_patch/generic/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2227 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/file_patch/generic/versions/v_0/generic.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.749190 cengal-3.2.0/cengal/file_system/file_patch/generic/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/file_patch/generic/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/file_patch/generic/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.759190 cengal-3.2.0/cengal/file_system/file_patch/simple/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/file_patch/simple/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.759190 cengal-3.2.0/cengal/file_system/file_patch/simple/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/file_patch/simple/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.769190 cengal-3.2.0/cengal/file_system/file_patch/simple/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/file_patch/simple/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2310 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/file_patch/simple/versions/v_0/simple.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.779190 cengal-3.2.0/cengal/file_system/file_patch/simple/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/file_patch/simple/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/file_patch/simple/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.779190 cengal-3.2.0/cengal/file_system/path_manager/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/path_manager/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.789190 cengal-3.2.0/cengal/file_system/path_manager/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/path_manager/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.799190 cengal-3.2.0/cengal/file_system/path_manager/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/path_manager/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2580 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/path_manager/versions/v_0/path_manager.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.819190 cengal-3.2.0/cengal/file_system/path_manager/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/path_manager/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/path_manager/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.849190 cengal-3.2.0/cengal/file_system/win_fs/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/win_fs/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3113 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/win_fs/base.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1850 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/win_fs/global_install_uninstall.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1996 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/win_fs/path.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5189 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/win_fs/shutil.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4436 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/file_system/win_fs/shutil_readable.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.859190 cengal-3.2.0/cengal/hardware/
--rw-r--r--   0 mb        (1000) mb        (1000)     1209 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.869190 cengal-3.2.0/cengal/hardware/info/
--rw-r--r--   0 mb        (1000) mb        (1000)     1209 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/info/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.869190 cengal-3.2.0/cengal/hardware/info/cpu/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/info/cpu/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.869190 cengal-3.2.0/cengal/hardware/info/cpu/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/info/cpu/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.899190 cengal-3.2.0/cengal/hardware/info/cpu/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/info/cpu/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2281 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/info/cpu/versions/v_0/cpu.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.909190 cengal-3.2.0/cengal/hardware/info/cpu/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/info/cpu/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/info/cpu/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.919190 cengal-3.2.0/cengal/hardware/info/cpu/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/info/cpu/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8747 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/info/cpu/versions/v_1/cpu.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.939190 cengal-3.2.0/cengal/hardware/info/cpu/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/info/cpu/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/info/cpu/versions/v_1/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.949190 cengal-3.2.0/cengal/hardware/memory/
--rw-r--r--   0 mb        (1000) mb        (1000)     1209 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/memory/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.949190 cengal-3.2.0/cengal/hardware/memory/barriers/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/memory/barriers/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.959190 cengal-3.2.0/cengal/hardware/memory/barriers/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/memory/barriers/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.959190 cengal-3.2.0/cengal/hardware/memory/barriers/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/memory/barriers/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.969190 cengal-3.2.0/cengal/hardware/memory/barriers/versions/v_0/compilable/
--rw-r--r--   0 mb        (1000) mb        (1000)     2021 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/memory/barriers/versions/v_0/compilable/__build_config.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1354 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/memory/barriers/versions/v_0/compilable/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7924 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/memory/barriers/versions/v_0/compilable/barriers__cython.pyx
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.969190 cengal-3.2.0/cengal/hardware/memory/barriers/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/memory/barriers/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/memory/barriers/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.979190 cengal-3.2.0/cengal/hardware/memory/shared_memory/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/memory/shared_memory/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:10.989190 cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.019190 cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1348 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.019190 cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/v_0/compilable/
--rw-r--r--   0 mb        (1000) mb        (1000)     1932 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/v_0/compilable/__build_config.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1359 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/v_0/compilable/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5299 2023-05-22 07:53:53.000000 cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/v_0/compilable/memory_access.c
--rw-r--r--   0 mb        (1000) mb        (1000)     3039 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/v_0/compilable/memory_access.h
--rw-r--r--   0 mb        (1000) mb        (1000)    11807 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/v_0/compilable/memory_access__cython.pyx
--rw-r--r--   0 mb        (1000) mb        (1000)     4229 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/v_0/interfaces.py
--rw-r--r--   0 mb        (1000) mb        (1000)   108882 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/v_0/shared_memory.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.019190 cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8552 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/help_tools.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.039190 cengal-3.2.0/cengal/introspection/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/introspection/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.039190 cengal-3.2.0/cengal/introspection/inspect/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/introspection/inspect/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.039190 cengal-3.2.0/cengal/introspection/inspect/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/introspection/inspect/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.049190 cengal-3.2.0/cengal/introspection/inspect/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/introspection/inspect/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    19833 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/introspection/inspect/versions/v_0/inspect.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.059190 cengal-3.2.0/cengal/introspection/inspect/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/introspection/inspect/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/introspection/inspect/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.069190 cengal-3.2.0/cengal/introspection/third_party/
--rw-r--r--   0 mb        (1000) mb        (1000)     1209 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/introspection/third_party/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.069190 cengal-3.2.0/cengal/introspection/third_party/ctypes/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/introspection/third_party/ctypes/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.069190 cengal-3.2.0/cengal/introspection/third_party/ctypes/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/introspection/third_party/ctypes/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.079190 cengal-3.2.0/cengal/introspection/third_party/ctypes/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/introspection/third_party/ctypes/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5358 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/introspection/third_party/ctypes/versions/v_0/ctypes.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.089190 cengal-3.2.0/cengal/introspection/third_party/ctypes/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/introspection/third_party/ctypes/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/introspection/third_party/ctypes/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.089190 cengal-3.2.0/cengal/io/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.109190 cengal-3.2.0/cengal/io/asock_io/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/asock_io/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.109190 cengal-3.2.0/cengal/io/asock_io/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/asock_io/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.149190 cengal-3.2.0/cengal/io/asock_io/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1280 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/asock_io/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6005 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/asock_io/versions/v_0/base.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.149190 cengal-3.2.0/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1528 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3766 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/recv_buff_size_computer__cython.pyx
--rw-r--r--   0 mb        (1000) mb        (1000)     3191 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/recv_buff_size_computer__python.py
--rw-r--r--   0 mb        (1000) mb        (1000)   113358 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/asock_io/versions/v_0/tcp_app_server.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5056 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/asock_io/versions/v_0/tcp_link.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.199190 cengal-3.2.0/cengal/io/asock_io/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1280 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/asock_io/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    18745 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/asock_io/versions/v_1/abstract.py
--rw-r--r--   0 mb        (1000) mb        (1000)   123888 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/asock_io/versions/v_1/asock_io_core.py
--rw-r--r--   0 mb        (1000) mb        (1000)    15714 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/asock_io/versions/v_1/base.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.209190 cengal-3.2.0/cengal/io/asock_io/versions/v_1/io_loops/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/asock_io/versions/v_1/io_loops/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3921 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/asock_io/versions/v_1/io_loops/epoll_lt.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6408 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/asock_io/versions/v_1/io_loops/select.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.229189 cengal-3.2.0/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1475 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3701 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/recv_buff_size_computer__cython.pyx
--rw-r--r--   0 mb        (1000) mb        (1000)     3129 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/recv_buff_size_computer__python.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4986 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/asock_io/versions/v_1/tcp_link.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.229189 cengal-3.2.0/cengal/io/core/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/core/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.239189 cengal-3.2.0/cengal/io/core/memory_management/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/core/memory_management/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.249189 cengal-3.2.0/cengal/io/core/memory_management/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/core/memory_management/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.289189 cengal-3.2.0/cengal/io/core/memory_management/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/core/memory_management/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3261 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/core/memory_management/versions/v_0/memory_management.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.289189 cengal-3.2.0/cengal/io/core/memory_management/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/core/memory_management/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/core/memory_management/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.289189 cengal-3.2.0/cengal/io/named_connections/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/named_connections/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.289189 cengal-3.2.0/cengal/io/named_connections/named_connections_manager/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/named_connections/named_connections_manager/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.299189 cengal-3.2.0/cengal/io/named_connections/named_connections_manager/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/named_connections/named_connections_manager/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.319189 cengal-3.2.0/cengal/io/named_connections/named_connections_manager/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/named_connections/named_connections_manager/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    10643 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/named_connections/named_connections_manager/versions/v_0/named_connections_manager.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.349189 cengal-3.2.0/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.369189 cengal-3.2.0/cengal/io/named_connections/workers/
--rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/named_connections/workers/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.369189 cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.369189 cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.369189 cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6609 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/asyncio_streams.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.379189 cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.379189 cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams_proxy/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams_proxy/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.409189 cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.409189 cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1243 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/asyncio_streams_proxy.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.419189 cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.429189 cengal-3.2.0/cengal/io/net_io/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/net_io/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.439189 cengal-3.2.0/cengal/io/net_io/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/net_io/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.459189 cengal-3.2.0/cengal/io/net_io/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/net_io/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.459189 cengal-3.2.0/cengal/io/net_io/versions/v_0/crossplatform/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/net_io/versions/v_0/crossplatform/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.539189 cengal-3.2.0/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/abstract.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/linux.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/win32.py
--rw-r--r--   0 mb        (1000) mb        (1000)    11974 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/net_io/versions/v_0/net_io__linux.py
--rw-r--r--   0 mb        (1000) mb        (1000)    14772 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/net_io/versions/v_0/net_io_abstract.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3986 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/net_io/versions/v_0/net_io_method__epoll_lt.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4845 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/net_io/versions/v_0/net_io_method__select.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.549189 cengal-3.2.0/cengal/io/recv_buff_size_computer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/recv_buff_size_computer/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.559189 cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.609189 cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1528 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3766 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/v_0/recv_buff_size_computer__cython.pyx
--rw-r--r--   0 mb        (1000) mb        (1000)     3191 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/v_0/recv_buff_size_computer__python.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.609189 cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.639189 cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1475 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3701 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/v_1/recv_buff_size_computer__cython.pyx
--rw-r--r--   0 mb        (1000) mb        (1000)     3129 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/v_1/recv_buff_size_computer__python.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.639189 cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/v_1/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.639189 cengal-3.2.0/cengal/io/serve_free_ports/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/serve_free_ports/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.639189 cengal-3.2.0/cengal/io/serve_free_ports/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/serve_free_ports/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.649189 cengal-3.2.0/cengal/io/serve_free_ports/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/serve_free_ports/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5138 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/serve_free_ports/versions/v_0/serve_free_ports.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.659189 cengal-3.2.0/cengal/io/serve_free_ports/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/serve_free_ports/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/serve_free_ports/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.659189 cengal-3.2.0/cengal/io/socket/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/socket/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.669189 cengal-3.2.0/cengal/io/socket/constants/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/socket/constants/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.669189 cengal-3.2.0/cengal/io/socket/constants/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/socket/constants/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.679189 cengal-3.2.0/cengal/io/socket/constants/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/socket/constants/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1281 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/socket/constants/versions/v_0/constants.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.689189 cengal-3.2.0/cengal/io/socket/constants/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/socket/constants/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/socket/constants/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.689189 cengal-3.2.0/cengal/io/socket/errors/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/socket/errors/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.699189 cengal-3.2.0/cengal/io/socket/errors/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/socket/errors/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.699189 cengal-3.2.0/cengal/io/socket/errors/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/socket/errors/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2429 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/socket/errors/versions/v_0/errors.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.709189 cengal-3.2.0/cengal/io/socket/errors/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/socket/errors/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/socket/errors/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.719189 cengal-3.2.0/cengal/io/used_ports/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/used_ports/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.729189 cengal-3.2.0/cengal/io/used_ports/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/used_ports/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.769189 cengal-3.2.0/cengal/io/used_ports/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/used_ports/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.769189 cengal-3.2.0/cengal/io/used_ports/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/used_ports/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3132 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/used_ports/versions/v_0/tests/_test__used_ports.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8978 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/io/used_ports/versions/v_0/used_ports.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.779189 cengal-3.2.0/cengal/math/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/math/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.789189 cengal-3.2.0/cengal/math/algebra/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/math/algebra/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.789189 cengal-3.2.0/cengal/math/algebra/fast_algorithms/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/math/algebra/fast_algorithms/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.799189 cengal-3.2.0/cengal/math/algebra/fast_algorithms/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/math/algebra/fast_algorithms/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.799189 cengal-3.2.0/cengal/math/algebra/fast_algorithms/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/math/algebra/fast_algorithms/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1783 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/math/algebra/fast_algorithms/versions/v_0/fast_algorithms.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.809189 cengal-3.2.0/cengal/math/algebra/fast_algorithms/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/math/algebra/fast_algorithms/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/math/algebra/fast_algorithms/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.829189 cengal-3.2.0/cengal/math/geometry/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/math/geometry/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.829189 cengal-3.2.0/cengal/math/geometry/ellipse/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0/cengal/math/geometry/ellipse/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.859189 cengal-3.2.0/cengal/math/geometry/ellipse/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/math/geometry/ellipse/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.879189 cengal-3.2.0/cengal/math/geometry/ellipse/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/math/geometry/ellipse/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4988 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/math/geometry/ellipse/versions/v_0/ellipse.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.919189 cengal-3.2.0/cengal/math/geometry/ellipse/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/math/geometry/ellipse/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/math/geometry/ellipse/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2713 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/math/geometry/ellipse/versions/v_0/tests/informal_tests.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.919189 cengal-3.2.0/cengal/math/geometry/point/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/math/geometry/point/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.919189 cengal-3.2.0/cengal/math/geometry/point/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/math/geometry/point/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.929189 cengal-3.2.0/cengal/math/geometry/point/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1227 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/math/geometry/point/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    16019 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/math/geometry/point/versions/v_0/point.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.959189 cengal-3.2.0/cengal/math/geometry/point/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/math/geometry/point/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/math/geometry/point/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.959189 cengal-3.2.0/cengal/math/geometry/vector/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/math/geometry/vector/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.959189 cengal-3.2.0/cengal/math/geometry/vector/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/math/geometry/vector/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.979189 cengal-3.2.0/cengal/math/geometry/vector/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/math/geometry/vector/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.979189 cengal-3.2.0/cengal/math/geometry/vector/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/math/geometry/vector/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/math/geometry/vector/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    46032 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/math/geometry/vector/versions/v_0/vector.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.989189 cengal-3.2.0/cengal/math/numbers/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/math/numbers/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:11.989189 cengal-3.2.0/cengal/math/numbers/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/math/numbers/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.009189 cengal-3.2.0/cengal/math/numbers/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/math/numbers/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1346 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/math/numbers/versions/v_0/numbers.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.019189 cengal-3.2.0/cengal/math/numbers/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/math/numbers/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/math/numbers/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.089189 cengal-3.2.0/cengal/modules_management/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/modules_management/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1569 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/modules_management/alternative_import.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.099189 cengal-3.2.0/cengal/modules_management/ignore_in_build_mode/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/modules_management/ignore_in_build_mode/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.099189 cengal-3.2.0/cengal/modules_management/ignore_in_build_mode/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/modules_management/ignore_in_build_mode/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.119189 cengal-3.2.0/cengal/modules_management/ignore_in_build_mode/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/modules_management/ignore_in_build_mode/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1511 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/modules_management/ignore_in_build_mode/versions/v_0/ignore_in_build_mode.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.139189 cengal-3.2.0/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2182 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/modules_management/reload_module.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.149189 cengal-3.2.0/cengal/os/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/os/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1348 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/os/help_tools.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.149189 cengal-3.2.0/cengal/parallel_execution/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.169189 cengal-3.2.0/cengal/parallel_execution/asyncio/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.169189 cengal-3.2.0/cengal/parallel_execution/asyncio/atasks/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/atasks/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.179189 cengal-3.2.0/cengal/parallel_execution/asyncio/atasks/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/atasks/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.189189 cengal-3.2.0/cengal/parallel_execution/asyncio/atasks/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/atasks/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1847 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/atasks/versions/v_0/atasks.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.209189 cengal-3.2.0/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.209189 cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.209189 cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.239189 cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1360 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    12104 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_abstract.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2467 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_base.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1989 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_base_internal.py
--rw-r--r--   0 mb        (1000) mb        (1000)    51581 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tcp_efficient_streams.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.299189 cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3772 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/asyncio_streams_client.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6497 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/asyncio_streams_server.py
--rw-r--r--   0 mb        (1000) mb        (1000)    35909 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/udp_efficient_streams.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.299189 cengal-3.2.0/cengal/parallel_execution/asyncio/init_loop/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/init_loop/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.309189 cengal-3.2.0/cengal/parallel_execution/asyncio/init_loop/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/init_loop/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.319189 cengal-3.2.0/cengal/parallel_execution/asyncio/init_loop/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/init_loop/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1392 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/init_loop/versions/v_0/init_loop.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.339189 cengal-3.2.0/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.339189 cengal-3.2.0/cengal/parallel_execution/asyncio/run_in_process_pool/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/run_in_process_pool/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.339189 cengal-3.2.0/cengal/parallel_execution/asyncio/run_in_process_pool/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/run_in_process_pool/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.369189 cengal-3.2.0/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1241 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     9439 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/run_in_process_pool.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.409189 cengal-3.2.0/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.419189 cengal-3.2.0/cengal/parallel_execution/asyncio/run_loop/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/run_loop/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.419189 cengal-3.2.0/cengal/parallel_execution/asyncio/run_loop/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/run_loop/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.439189 cengal-3.2.0/cengal/parallel_execution/asyncio/run_loop/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/run_loop/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3526 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/run_loop/versions/v_0/run_loop.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.469189 cengal-3.2.0/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.489189 cengal-3.2.0/cengal/parallel_execution/asyncio/timed_yield/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/timed_yield/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.489189 cengal-3.2.0/cengal/parallel_execution/asyncio/timed_yield/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/timed_yield/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.519189 cengal-3.2.0/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.519189 cengal-3.2.0/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1641 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/timed_yield.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.549188 cengal-3.2.0/cengal/parallel_execution/coroutines/
--rw-r--r--   0 mb        (1000) mb        (1000)     1300 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.549188 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_scheduler/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_scheduler/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.559188 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_scheduler/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_scheduler/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.569188 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)   126513 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/coro_scheduler.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.609188 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.619188 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/
--rw-r--r--   0 mb        (1000) mb        (1000)     1452 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.619188 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.639188 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.639188 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    11264 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/async_event_bus.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.659188 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.659188 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:12.659188 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.499189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    20727 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/asyncio_loop.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.499189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.499189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/communication/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/communication/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.499189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.499189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6565 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/communication.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.499189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.499189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.499189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.499189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4173 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/cpu_tick_count_per_second.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.499189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.499189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/db/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/db/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.499189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.499189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1224 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    55877 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/db.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.549189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.549189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.549189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.569189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7706 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/event_bus.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.579189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.579189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.589189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.609189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7637 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/fast_aggregator.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.619189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.619189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/instance/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/instance/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.619189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.629189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     9088 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/instance.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.639189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.649189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.649189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.669189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5521 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/kill_coro.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.689189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.689189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.699189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.709189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7536 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/kill_coro_list.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.709189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.719189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.719189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.749189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3907 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/lazy_print.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.799189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.799189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.839189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.859189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    21254 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/lmdb.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.859189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.859189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/log/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/log/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.919189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.999189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    13685 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/log.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.999189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.999189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:19.999189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.069189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1264 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5970 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/bytecode_patcher.py
--rw-r--r--   0 mb        (1000) mb        (1000)    27435 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/loop_yield.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.069189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.069189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.069189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.089189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    22656 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/put_coro.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.119189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.119189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.119189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.119189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6167 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/put_coro_list.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.119189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.119189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.119189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.129189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    25203 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/read_write_locker.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.139189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.149189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.149189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.219189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4955 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/class_info.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3826 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/commands.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1398 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/exceptions.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5315 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/remote_node.py
--rw-r--r--   0 mb        (1000) mb        (1000)    21054 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/remote_nodes.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6043 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/request_class_info.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5876 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/serializers.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.239189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.239189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.299189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.309189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3464 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/run_coro.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.319189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.329189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.339189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.349189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1747 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/shutdown_loop.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.359189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.369189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.369189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.399189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1252 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2896 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/shutdown_on_keyboard_interrupt.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.409189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.419189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.429189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.439189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1651 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/simple_yield.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.449189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.449189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/sleep/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/sleep/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.449189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.469189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2900 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/sleep.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.509189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.519189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.529189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.529189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1724 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/some_printer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.539189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.559189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.569189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.569189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.569189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6824 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/throw_coro.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.569189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.569189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.569189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.569189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7153 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/throw_coro_list.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.569189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.569189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.569189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.569189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    11821 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/timer_coro_runner.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.569189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.569189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.569189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.569189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    11052 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/timer_func_runner.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.569189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.569189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.639189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.659189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    28116 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tkinter.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.659189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.669189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.679189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.699189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    18946 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/wait_coro.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.729189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/
--rw-r--r--   0 mb        (1000) mb        (1000)     1209 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.729189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.739189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.759189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/general.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.809189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.809189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.819189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.829189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1251 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5686 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/service_with_a_direct_request.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.859189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.879189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.889189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/await_coro/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/await_coro/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.889189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.919189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    14141 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/await_coro.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.929189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.939189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.939189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.959189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5185 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/coro_flow_control.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.969189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.999189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/low_latency/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/low_latency/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.999189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:20.999189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.019189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3174 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/ajson.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5181 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/json.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.029189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.029189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.039189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.049189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5978 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/prepare_loop.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.069189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.069189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.089189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.099189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8390 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/run_in_loop.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.109189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.129189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/wait_coro/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/wait_coro/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.139189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.149189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.159189 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7875 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/wait_coro.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.199189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/
--rw-r--r--   0 mb        (1000) mb        (1000)     1209 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.199189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/customtkinter/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/customtkinter/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.199189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.209189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1828 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/customtkinter.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.219189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.229189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/nicegui/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/nicegui/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.249189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/nicegui/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/nicegui/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.249189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    19200 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/nicegui.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.259189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.269189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/pytermgui/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/pytermgui/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.269189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.299189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4690 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/pytermgui.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.309189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.319189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/qt/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/qt/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.329189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/qt/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/qt/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.339189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1224 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    13309 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/qt.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.349189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.349189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvicorn/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvicorn/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.369189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.389189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.419189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5546 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/uvicorn.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.419189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvloop/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvloop/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.419189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvloop/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvloop/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.429189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.439189 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1529 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/uvloop.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.459189 cengal-3.2.0/cengal/parallel_execution/green_threads_tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/green_threads_tools/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3706 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/green_threads_tools/task_management.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.509189 cengal-3.2.0/cengal/parallel_execution/multiprocess/
--rw-r--r--   0 mb        (1000) mb        (1000)     1250 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/multiprocess/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2839 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/multiprocess/multiprocess_testing.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3085 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/multiprocess/multiprocessing_task_pool.py
--rw-r--r--   0 mb        (1000) mb        (1000)    24842 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/multiprocess/multiprocessing_task_runner.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.519189 cengal-3.2.0/cengal/parallel_execution/multithreading/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/multithreading/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7150 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/parallel_execution/multithreading/thread_workers_pool.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.539189 cengal-3.2.0/cengal/performance_test_lib/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/performance_test_lib/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.549189 cengal-3.2.0/cengal/performance_test_lib/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/performance_test_lib/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.569189 cengal-3.2.0/cengal/performance_test_lib/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/performance_test_lib/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8267 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/performance_test_lib/versions/v_0/performance_test_lib.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.569189 cengal-3.2.0/cengal/performance_test_lib/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/performance_test_lib/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2240 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/performance_test_lib/versions/v_0/tests/test__performance_test_lib.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.569189 cengal-3.2.0/cengal/performance_test_lib/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/performance_test_lib/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     9290 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/performance_test_lib/versions/v_1/performance_test_lib.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.579189 cengal-3.2.0/cengal/performance_test_lib/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/performance_test_lib/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2240 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/performance_test_lib/versions/v_1/tests/test__performance_test_lib.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.589189 cengal-3.2.0/cengal/shared_memory/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/shared_memory/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.609189 cengal-3.2.0/cengal/shared_memory/versions/
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.629189 cengal-3.2.0/cengal/shared_memory/versions/1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/shared_memory/versions/1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1501 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/shared_memory/versions/1/mmap.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/shared_memory/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.629189 cengal-3.2.0/cengal/statistics/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/statistics/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.629189 cengal-3.2.0/cengal/statistics/normal_distribution/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/statistics/normal_distribution/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.629189 cengal-3.2.0/cengal/statistics/normal_distribution/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/statistics/normal_distribution/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.639189 cengal-3.2.0/cengal/statistics/normal_distribution/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1241 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/statistics/normal_distribution/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4156 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/statistics/normal_distribution/versions/v_0/normal_distribution.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.649189 cengal-3.2.0/cengal/statistics/normal_distribution/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/statistics/normal_distribution/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/statistics/normal_distribution/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3261 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/system.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.699189 cengal-3.2.0/cengal/testing_lib/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/testing_lib/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3056 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/testing_lib/tests_list_runner.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.709189 cengal-3.2.0/cengal/text_processing/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.729189 cengal-3.2.0/cengal/text_processing/brackets_processing/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/brackets_processing/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.729189 cengal-3.2.0/cengal/text_processing/brackets_processing/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/brackets_processing/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.799189 cengal-3.2.0/cengal/text_processing/brackets_processing/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1289 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/brackets_processing/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2344 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/brackets_processing/versions/v_0/brackets.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6467 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/brackets_processing/versions/v_0/processing.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3779 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/brackets_processing/versions/v_0/standard_brackets.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.809189 cengal-3.2.0/cengal/text_processing/brackets_processing/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/brackets_processing/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/brackets_processing/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.839189 cengal-3.2.0/cengal/text_processing/encoding_detection/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/encoding_detection/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.839189 cengal-3.2.0/cengal/text_processing/encoding_detection/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/encoding_detection/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.859189 cengal-3.2.0/cengal/text_processing/encoding_detection/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/encoding_detection/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2464 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/encoding_detection/versions/v_0/encoding_detection.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.859189 cengal-3.2.0/cengal/text_processing/encoding_detection/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/encoding_detection/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/encoding_detection/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    11968 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/help_tools.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.869189 cengal-3.2.0/cengal/text_processing/optional_formatter/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/optional_formatter/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.869189 cengal-3.2.0/cengal/text_processing/optional_formatter/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/optional_formatter/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.899189 cengal-3.2.0/cengal/text_processing/optional_formatter/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/optional_formatter/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4274 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/optional_formatter/versions/v_0/optional_formatter.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.909189 cengal-3.2.0/cengal/text_processing/optional_formatter/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/optional_formatter/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/optional_formatter/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.909189 cengal-3.2.0/cengal/text_processing/simple_config_file_processor/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/simple_config_file_processor/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.919189 cengal-3.2.0/cengal/text_processing/simple_config_file_processor/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/simple_config_file_processor/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.969189 cengal-3.2.0/cengal/text_processing/simple_config_file_processor/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1250 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/simple_config_file_processor/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/simple_config_file_processor/versions/v_0/simple_config_file_processor.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.989189 cengal-3.2.0/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.989189 cengal-3.2.0/cengal/text_processing/text_patch/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_patch/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.989189 cengal-3.2.0/cengal/text_processing/text_patch/brackets/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_patch/brackets/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:21.999189 cengal-3.2.0/cengal/text_processing/text_patch/brackets/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_patch/brackets/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.009189 cengal-3.2.0/cengal/text_processing/text_patch/brackets/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_patch/brackets/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2009 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_patch/brackets/versions/v_0/brackets.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.029189 cengal-3.2.0/cengal/text_processing/text_patch/brackets/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_patch/brackets/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_patch/brackets/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.039189 cengal-3.2.0/cengal/text_processing/text_patch/simple/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_patch/simple/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.039189 cengal-3.2.0/cengal/text_processing/text_patch/simple/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_patch/simple/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.059189 cengal-3.2.0/cengal/text_processing/text_patch/simple/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_patch/simple/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1829 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_patch/simple/versions/v_0/simple.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.069189 cengal-3.2.0/cengal/text_processing/text_patch/simple/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_patch/simple/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_patch/simple/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.069189 cengal-3.2.0/cengal/text_processing/text_processing/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_processing/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.069189 cengal-3.2.0/cengal/text_processing/text_processing/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_processing/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.079189 cengal-3.2.0/cengal/text_processing/text_processing/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_processing/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6281 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_processing/versions/v_0/processing.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.079189 cengal-3.2.0/cengal/text_processing/text_processing/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_processing/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_processing/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.099189 cengal-3.2.0/cengal/text_processing/text_translator/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_translator/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.099189 cengal-3.2.0/cengal/text_processing/text_translator/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_translator/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.099189 cengal-3.2.0/cengal/text_processing/text_translator/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_translator/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.119189 cengal-3.2.0/cengal/text_processing/text_translator/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_translator/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_translator/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    12695 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/text_translator/versions/v_0/text_translator.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.119189 cengal-3.2.0/cengal/text_processing/utf_bom_processing/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/utf_bom_processing/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.119189 cengal-3.2.0/cengal/text_processing/utf_bom_processing/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/utf_bom_processing/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.139189 cengal-3.2.0/cengal/text_processing/utf_bom_processing/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/utf_bom_processing/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.149190 cengal-3.2.0/cengal/text_processing/utf_bom_processing/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/utf_bom_processing/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/utf_bom_processing/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2993 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/text_processing/utf_bom_processing/versions/v_0/utf_bom_processing.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.159190 cengal-3.2.0/cengal/time_management/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/time_management/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.159190 cengal-3.2.0/cengal/time_management/cpu_clock/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/time_management/cpu_clock/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.159190 cengal-3.2.0/cengal/time_management/cpu_clock/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/time_management/cpu_clock/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.169190 cengal-3.2.0/cengal/time_management/cpu_clock/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/time_management/cpu_clock/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.189190 cengal-3.2.0/cengal/time_management/cpu_clock/versions/v_0/compilable/
--rw-r--r--   0 mb        (1000) mb        (1000)     1356 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/time_management/cpu_clock/versions/v_0/compilable/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1929 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/time_management/cpu_clock/versions/v_0/compilable/__x__build_config.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1639 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/time_management/cpu_clock/versions/v_0/cpu_clock.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.199190 cengal-3.2.0/cengal/time_management/cpu_clock/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/time_management/cpu_clock/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/time_management/cpu_clock/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.199190 cengal-3.2.0/cengal/time_management/cpu_clock_cycles/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/time_management/cpu_clock_cycles/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.229189 cengal-3.2.0/cengal/time_management/cpu_clock_cycles/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/time_management/cpu_clock_cycles/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.229189 cengal-3.2.0/cengal/time_management/cpu_clock_cycles/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/time_management/cpu_clock_cycles/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.239189 cengal-3.2.0/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/
--rw-r--r--   0 mb        (1000) mb        (1000)     1935 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/__build_config.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1411 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1203 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/cpu_clock_cycles.c
--rw-r--r--   0 mb        (1000) mb        (1000)      876 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/cpu_clock_cycles.h
--rw-r--r--   0 mb        (1000) mb        (1000)     1880 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/cpu_clock_cycles__cython.pyx
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.249189 cengal-3.2.0/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.259189 cengal-3.2.0/cengal/time_management/high_precision_sync_sleep/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/high_precision_sync_sleep/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.259189 cengal-3.2.0/cengal/time_management/high_precision_sync_sleep/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/high_precision_sync_sleep/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.259189 cengal-3.2.0/cengal/time_management/high_precision_sync_sleep/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1368 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/high_precision_sync_sleep/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2727 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/high_precision_sync_sleep/versions/v_0/high_precision_sync_sleep__cython.pyx
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.279189 cengal-3.2.0/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.279189 cengal-3.2.0/cengal/time_management/load_best_timer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/load_best_timer/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.289189 cengal-3.2.0/cengal/time_management/load_best_timer/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/load_best_timer/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.299189 cengal-3.2.0/cengal/time_management/load_best_timer/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/load_best_timer/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1445 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/load_best_timer/versions/v_0/load_best_timer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.299189 cengal-3.2.0/cengal/time_management/relative_time/
--rw-r--r--   0 mb        (1000) mb        (1000)     1365 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/relative_time/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.309189 cengal-3.2.0/cengal/time_management/relative_time/approximate_representation/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/relative_time/approximate_representation/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.329190 cengal-3.2.0/cengal/time_management/relative_time/approximate_representation/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/relative_time/approximate_representation/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.329190 cengal-3.2.0/cengal/time_management/relative_time/approximate_representation/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/relative_time/approximate_representation/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8714 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/relative_time/approximate_representation/versions/v_0/approximate_representation.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.329190 cengal-3.2.0/cengal/time_management/relative_time/bysiness_relativedelta/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/relative_time/bysiness_relativedelta/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.329190 cengal-3.2.0/cengal/time_management/relative_time/bysiness_relativedelta/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/relative_time/bysiness_relativedelta/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.359190 cengal-3.2.0/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1244 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1489 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/bysiness_relativedelta.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.359190 cengal-3.2.0/cengal/time_management/relative_time/constants/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/relative_time/constants/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.359190 cengal-3.2.0/cengal/time_management/relative_time/constants/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/relative_time/constants/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.359190 cengal-3.2.0/cengal/time_management/relative_time/constants/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/relative_time/constants/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1418 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/relative_time/constants/versions/v_0/constants.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.359190 cengal-3.2.0/cengal/time_management/relative_time/relativedelta/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/relative_time/relativedelta/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.369190 cengal-3.2.0/cengal/time_management/relative_time/relativedelta/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/relative_time/relativedelta/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.379190 cengal-3.2.0/cengal/time_management/relative_time/relativedelta/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/relative_time/relativedelta/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1859 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/relative_time/relativedelta/versions/v_0/relativedelta.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.379190 cengal-3.2.0/cengal/time_management/relative_time/timedelta/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/relative_time/timedelta/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.379190 cengal-3.2.0/cengal/time_management/relative_time/timedelta/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/relative_time/timedelta/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.399190 cengal-3.2.0/cengal/time_management/relative_time/timedelta/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/relative_time/timedelta/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1632 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/relative_time/timedelta/versions/v_0/timedelta.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.399190 cengal-3.2.0/cengal/time_management/repeat_for_a_time/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/repeat_for_a_time/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.399190 cengal-3.2.0/cengal/time_management/repeat_for_a_time/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/repeat_for_a_time/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.399190 cengal-3.2.0/cengal/time_management/repeat_for_a_time/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1456 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/repeat_for_a_time/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    20785 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/repeat_for_a_time/versions/v_0/repeat_for_a_time__cython.pyx
--rw-r--r--   0 mb        (1000) mb        (1000)    13453 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/repeat_for_a_time/versions/v_0/repeat_for_a_time__python.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.419190 cengal-3.2.0/cengal/time_management/repeat_for_a_time/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/repeat_for_a_time/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/repeat_for_a_time/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    16608 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/repeat_for_a_time/versions/v_0/tests/example_for__repeat_for_a_time.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.429190 cengal-3.2.0/cengal/time_management/sleep_tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/sleep_tools/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.429190 cengal-3.2.0/cengal/time_management/sleep_tools/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/sleep_tools/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.449190 cengal-3.2.0/cengal/time_management/sleep_tools/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/sleep_tools/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4700 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/sleep_tools/versions/v_0/sleep_tools.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.459190 cengal-3.2.0/cengal/time_management/sleep_tools/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/sleep_tools/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/sleep_tools/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.459190 cengal-3.2.0/cengal/time_management/timer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/timer/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.469190 cengal-3.2.0/cengal/time_management/timer/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/timer/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.479189 cengal-3.2.0/cengal/time_management/timer/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1227 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/timer/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.499190 cengal-3.2.0/cengal/time_management/timer/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/timer/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/timer/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4567 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/timer/versions/v_0/timer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.509190 cengal-3.2.0/cengal/time_management/timer/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1227 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/timer/versions/v_1/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.519190 cengal-3.2.0/cengal/time_management/timer/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/timer/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/timer/versions/v_1/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6791 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/timer/versions/v_1/timer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.519190 cengal-3.2.0/cengal/time_management/timer_precision/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/timer_precision/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.529190 cengal-3.2.0/cengal/time_management/timer_precision/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/timer_precision/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.539190 cengal-3.2.0/cengal/time_management/timer_precision/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/timer_precision/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1866 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/timer_precision/versions/v_0/test_timer_precision.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.549190 cengal-3.2.0/cengal/time_management/timer_precision/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/timer_precision/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4327 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/time_management/timer_precision/versions/v_1/timer_precision.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.569190 cengal-3.2.0/cengal/unittest/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/unittest/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.569190 cengal-3.2.0/cengal/unittest/behavior_stabilizer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/unittest/behavior_stabilizer/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.569190 cengal-3.2.0/cengal/unittest/behavior_stabilizer/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/unittest/behavior_stabilizer/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.589190 cengal-3.2.0/cengal/unittest/behavior_stabilizer/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1241 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/unittest/behavior_stabilizer/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2032 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/unittest/behavior_stabilizer/versions/v_0/behavior_stabilizer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.609190 cengal-3.2.0/cengal/unittest/behavior_stabilizer/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/unittest/behavior_stabilizer/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/unittest/behavior_stabilizer/versions/v_0/tests/_test__behavior_stabilizer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.619190 cengal-3.2.0/cengal/unittest/patcher/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/unittest/patcher/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.619190 cengal-3.2.0/cengal/unittest/patcher/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/unittest/patcher/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.639190 cengal-3.2.0/cengal/unittest/patcher/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/unittest/patcher/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3084 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/unittest/patcher/versions/v_0/patcher.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.669190 cengal-3.2.0/cengal/unittest/patcher/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/unittest/patcher/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/unittest/patcher/versions/v_0/tests/_test__patcher.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.719190 cengal-3.2.0/cengal/universal_parser/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/universal_parser/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/universal_parser/help_tools.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1377 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/universal_parser/idioms.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/universal_parser/parser.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8667 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/universal_parser/test.py
--rw-r--r--   0 mb        (1000) mb        (1000)    75709 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/universal_parser/types.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.749190 cengal-3.2.0/cengal/upk_helping_tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/upk_helping_tools/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2299 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/upk_helping_tools/upk_api.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1821 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/upk_helping_tools/upk_constants.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6518 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/upk_helping_tools/upk_utils_api.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.759190 cengal-3.2.0/cengal/user_interface/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.779190 cengal-3.2.0/cengal/user_interface/console/
--rw-r--r--   0 mb        (1000) mb        (1000)     1324 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/console/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3504 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/console/chooser.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1549 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/console/colorama_helpers.py
--rw-r--r--   0 mb        (1000) mb        (1000)    11360 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/console/encoding_changer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.789190 cengal-3.2.0/cengal/user_interface/console/progress_meter/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/console/progress_meter/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.789190 cengal-3.2.0/cengal/user_interface/console/progress_meter/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/console/progress_meter/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.809190 cengal-3.2.0/cengal/user_interface/console/progress_meter/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1364 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/console/progress_meter/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4875 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/console/progress_meter/versions/v_0/progress_meter.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1274 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/console/progress_meter/versions/v_0/progress_meter_python2.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.809190 cengal-3.2.0/cengal/user_interface/gui/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/gui/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.819190 cengal-3.2.0/cengal/user_interface/gui/nt/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/gui/nt/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.819190 cengal-3.2.0/cengal/user_interface/gui/nt/blur_behind/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/gui/nt/blur_behind/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.839190 cengal-3.2.0/cengal/user_interface/gui/nt/blur_behind/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/gui/nt/blur_behind/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.849190 cengal-3.2.0/cengal/user_interface/gui/nt/blur_behind/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/gui/nt/blur_behind/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3161 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/gui/nt/blur_behind/versions/v_0/blur_behind.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.859190 cengal-3.2.0/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.889190 cengal-3.2.0/cengal/user_interface/gui/nt/dpi_awareness/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/gui/nt/dpi_awareness/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.889190 cengal-3.2.0/cengal/user_interface/gui/nt/dpi_awareness/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/gui/nt/dpi_awareness/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.889190 cengal-3.2.0/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3686 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/dpi_awareness.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.899190 cengal-3.2.0/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.909190 cengal-3.2.0/cengal/user_interface/plot/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/plot/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.949190 cengal-3.2.0/cengal/user_interface/plot/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/plot/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.959190 cengal-3.2.0/cengal/user_interface/plot/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/plot/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1877 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/plot/versions/v_0/plot.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:22.989190 cengal-3.2.0/cengal/user_interface/plot/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/plot/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/user_interface/plot/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:23.009190 cengal-3.2.0/cengal/web_tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/web_tools/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:23.019190 cengal-3.2.0/cengal/web_tools/detect_browsers_host_device_type/
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/web_tools/detect_browsers_host_device_type/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:23.029190 cengal-3.2.0/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:23.049190 cengal-3.2.0/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:23.049190 cengal-3.2.0/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4332 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/by_http_user_agent.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:23.099190 cengal-3.2.0/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    12869 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal/web_tools/help_tools.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:08.389192 cengal-3.2.0/cengal.egg-info/
--rw-r--r--   0 mb        (1000) mb        (1000)    27214 2023-05-22 08:06:04.000000 cengal-3.2.0/cengal.egg-info/PKG-INFO
--rw-r--r--   0 mb        (1000) mb        (1000)    86068 2023-05-22 08:06:04.000000 cengal-3.2.0/cengal.egg-info/SOURCES.txt
--rw-r--r--   0 mb        (1000) mb        (1000)        1 2023-05-22 08:06:04.000000 cengal-3.2.0/cengal.egg-info/dependency_links.txt
--rw-r--r--   0 mb        (1000) mb        (1000)      211 2023-05-22 08:06:04.000000 cengal-3.2.0/cengal.egg-info/requires.txt
--rw-r--r--   0 mb        (1000) mb        (1000)       28 2023-05-22 08:06:04.000000 cengal-3.2.0/cengal.egg-info/top_level.txt
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:23.139190 cengal-3.2.0/cengal_setup_scripts/
--rw-r--r--   0 mb        (1000) mb        (1000)     1250 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal_setup_scripts/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2428 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal_setup_scripts/compile_all_cython_modules.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:23.149190 cengal-3.2.0/cengal_setup_scripts/find_and_prepare_cython_modules/
--rw-r--r--   0 mb        (1000) mb        (1000)     1253 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal_setup_scripts/find_and_prepare_cython_modules/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    11688 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal_setup_scripts/find_and_prepare_cython_modules/find_and_prepare_cython_modules.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-22 08:06:23.169190 cengal-3.2.0/cengal_setup_scripts/install_required_packages/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal_setup_scripts/install_required_packages/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    10415 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal_setup_scripts/install_required_packages/install_packages.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1783 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal_setup_scripts/install_required_packages/set_environment_variables.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1500 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal_setup_scripts/setup__dynamic_list_of_pieces.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1497 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal_setup_scripts/setup__recv_buff_size_computer.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1498 2023-05-22 07:55:11.000000 cengal-3.2.0/cengal_setup_scripts/setup__repeat_for_a_time.py
--rw-r--r--   0 mb        (1000) mb        (1000)      167 2023-05-22 07:55:11.000000 cengal-3.2.0/pyproject.toml
--rw-r--r--   0 mb        (1000) mb        (1000)       38 2023-05-22 08:06:23.179190 cengal-3.2.0/setup.cfg
--rw-r--r--   0 mb        (1000) mb        (1000)     9046 2023-05-22 07:55:11.000000 cengal-3.2.0/setup.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:27.107846 cengal-3.2.0.1/
+-rw-r--r--   0 mb        (1000) mb        (1000)    11358 2022-04-21 11:25:54.000000 cengal-3.2.0.1/LICENSE.md
+-rw-r--r--   0 mb        (1000) mb        (1000)      614 2022-11-01 20:15:42.000000 cengal-3.2.0.1/NOTICE
+-rw-r--r--   0 mb        (1000) mb        (1000)    27216 2023-05-23 21:58:27.097846 cengal-3.2.0.1/PKG-INFO
+-rw-r--r--   0 mb        (1000) mb        (1000)    22105 2023-05-22 07:55:08.000000 cengal-3.2.0.1/README.md
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:05.657847 cengal-3.2.0.1/cengal/
+-rw-r--r--   0 mb        (1000) mb        (1000)     8227 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/RequestCache.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2760 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/ServerClock.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:05.717847 cengal-3.2.0.1/cengal/base/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/base/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:05.727847 cengal-3.2.0.1/cengal/base/classes/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/base/classes/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:05.737847 cengal-3.2.0.1/cengal/base/classes/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/base/classes/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:05.787847 cengal-3.2.0.1/cengal/base/classes/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/base/classes/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1266 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/base/classes/versions/v_0/classes.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:05.827847 cengal-3.2.0.1/cengal/base/classes/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/base/classes/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/base/classes/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:05.837847 cengal-3.2.0.1/cengal/base/exceptions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/base/exceptions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:05.847847 cengal-3.2.0.1/cengal/base/exceptions/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/base/exceptions/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:05.867847 cengal-3.2.0.1/cengal/base/exceptions/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/base/exceptions/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1302 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/base/exceptions/versions/v_0/exceptions.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:05.917847 cengal-3.2.0.1/cengal/base/exceptions/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/base/exceptions/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/base/exceptions/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:05.917847 cengal-3.2.0.1/cengal/build_tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1209 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/build_tools/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:05.927847 cengal-3.2.0.1/cengal/build_tools/current_compiler/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/build_tools/current_compiler/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:05.937847 cengal-3.2.0.1/cengal/build_tools/current_compiler/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/build_tools/current_compiler/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:05.967847 cengal-3.2.0.1/cengal/build_tools/current_compiler/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/build_tools/current_compiler/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2161 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/build_tools/current_compiler/versions/v_0/current_compiler.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:05.987847 cengal-3.2.0.1/cengal/build_tools/current_compiler/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/build_tools/current_compiler/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/build_tools/current_compiler/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.017847 cengal-3.2.0.1/cengal/build_tools/prepare_cflags/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/build_tools/prepare_cflags/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.017847 cengal-3.2.0.1/cengal/build_tools/prepare_cflags/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/build_tools/prepare_cflags/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.037847 cengal-3.2.0.1/cengal/build_tools/prepare_cflags/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/build_tools/prepare_cflags/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    14723 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/build_tools/prepare_cflags/versions/v_0/prepare_cflags.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.067847 cengal-3.2.0.1/cengal/build_tools/prepare_cflags/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/build_tools/prepare_cflags/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/build_tools/prepare_cflags/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.097847 cengal-3.2.0.1/cengal/bulk_pip_actions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/bulk_pip_actions/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6286 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/bulk_pip_actions/bulk_install.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6022 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/bulk_pip_actions/install.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1279 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/check_is_in_pycharm.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.097847 cengal-3.2.0.1/cengal/code_flow_control/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/code_flow_control/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.107847 cengal-3.2.0.1/cengal/code_flow_control/args_manager/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/code_flow_control/args_manager/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.127847 cengal-3.2.0.1/cengal/code_flow_control/args_manager/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/code_flow_control/args_manager/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.147847 cengal-3.2.0.1/cengal/code_flow_control/args_manager/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/code_flow_control/args_manager/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    16576 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/code_flow_control/args_manager/versions/v_0/args_manager.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.177847 cengal-3.2.0.1/cengal/code_flow_control/args_manager/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/code_flow_control/args_manager/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    17266 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/code_flow_control/args_manager/versions/v_0/tests/_manual_test__args_manager.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/code_flow_control/args_manager/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.187847 cengal-3.2.0.1/cengal/code_flow_control/call_history_reapplier/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/code_flow_control/call_history_reapplier/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.187847 cengal-3.2.0.1/cengal/code_flow_control/call_history_reapplier/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/code_flow_control/call_history_reapplier/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.217847 cengal-3.2.0.1/cengal/code_flow_control/call_history_reapplier/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1244 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/code_flow_control/call_history_reapplier/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2769 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/code_flow_control/call_history_reapplier/versions/v_0/call_history_reapplier.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.257847 cengal-3.2.0.1/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.327847 cengal-3.2.0.1/cengal/code_flow_control/chained_flow/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/code_flow_control/chained_flow/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.347847 cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.357847 cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-22 07:55:08.000000 cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    36470 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/v_0/smart_chain.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.417847 cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    32961 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/v_0/tests/example_for__chained_flow.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.447847 cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    35217 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/v_1/chained_flow.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.467847 cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/v_1/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    32961 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/v_1/tests/example_for__chained_flow.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.477847 cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.497847 cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.527847 cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    23327 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/versions/v_0/essence.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.627847 cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2881 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2623 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/quadrangle.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1372 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/quadrangle_test.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3466 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4070 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle_test.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4391 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle_test_old.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.637847 cengal-3.2.0.1/cengal/code_flow_control/none_or/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/none_or/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.647847 cengal-3.2.0.1/cengal/code_flow_control/none_or/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/none_or/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.717847 cengal-3.2.0.1/cengal/code_flow_control/none_or/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/none_or/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1486 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/none_or/versions/v_0/none_or.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.727847 cengal-3.2.0.1/cengal/code_flow_control/none_or/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/none_or/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/none_or/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.757847 cengal-3.2.0.1/cengal/code_flow_control/python_bytecode_manipulator/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/python_bytecode_manipulator/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.767847 cengal-3.2.0.1/cengal/code_flow_control/python_bytecode_manipulator/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/python_bytecode_manipulator/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.797847 cengal-3.2.0.1/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1249 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    29754 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/python_bytecode_manipulator.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.847847 cengal-3.2.0.1/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.867847 cengal-3.2.0.1/cengal/code_flow_control/smart_values/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/smart_values/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.887847 cengal-3.2.0.1/cengal/code_flow_control/smart_values/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/smart_values/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.907847 cengal-3.2.0.1/cengal/code_flow_control/smart_values/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/smart_values/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2827 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/smart_values/versions/v_0/result_types.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.917847 cengal-3.2.0.1/cengal/code_flow_control/smart_values/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/smart_values/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2838 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/smart_values/versions/v_1/smart_values.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.937847 cengal-3.2.0.1/cengal/code_flow_control/smart_values/versions/v_2/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/smart_values/versions/v_2/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3469 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_flow_control/smart_values/versions/v_2/smart_values.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.947847 cengal-3.2.0.1/cengal/code_inspection/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_inspection/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.967847 cengal-3.2.0.1/cengal/code_inspection/auto_line_tracer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_inspection/auto_line_tracer/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.967847 cengal-3.2.0.1/cengal/code_inspection/auto_line_tracer/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_inspection/auto_line_tracer/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.977847 cengal-3.2.0.1/cengal/code_inspection/auto_line_tracer/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_inspection/auto_line_tracer/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6170 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_inspection/auto_line_tracer/versions/v_0/auto_line_tracer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.997847 cengal-3.2.0.1/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:06.997847 cengal-3.2.0.1/cengal/code_inspection/line_profiling/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_inspection/line_profiling/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.017847 cengal-3.2.0.1/cengal/code_inspection/line_profiling/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_inspection/line_profiling/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.017847 cengal-3.2.0.1/cengal/code_inspection/line_profiling/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_inspection/line_profiling/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2769 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_inspection/line_profiling/versions/v_0/line_profiling.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.037847 cengal-3.2.0.1/cengal/code_inspection/line_profiling/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_inspection/line_profiling/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_inspection/line_profiling/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.047847 cengal-3.2.0.1/cengal/code_inspection/line_tracer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_inspection/line_tracer/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.047847 cengal-3.2.0.1/cengal/code_inspection/line_tracer/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_inspection/line_tracer/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.067847 cengal-3.2.0.1/cengal/code_inspection/line_tracer/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_inspection/line_tracer/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4304 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_inspection/line_tracer/versions/v_0/line_tracer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.097847 cengal-3.2.0.1/cengal/code_inspection/line_tracer/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_inspection/line_tracer/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/code_inspection/line_tracer/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.097847 cengal-3.2.0.1/cengal/cross_version/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/cross_version/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.097847 cengal-3.2.0.1/cengal/cross_version/console_print/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/cross_version/console_print/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1263 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/cross_version/console_print/python3.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1528 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/cross_version/console_print/universal.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.107847 cengal-3.2.0.1/cengal/ctypes_tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1209 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.117847 cengal-3.2.0.1/cengal/ctypes_tools/constants/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/constants/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.117847 cengal-3.2.0.1/cengal/ctypes_tools/constants/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/constants/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.137847 cengal-3.2.0.1/cengal/ctypes_tools/constants/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1269 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/constants/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.147847 cengal-3.2.0.1/cengal/ctypes_tools/constants/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/constants/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/constants/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    13437 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/constants/versions/v_0/win_constants.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.157847 cengal-3.2.0.1/cengal/ctypes_tools/function_prototypes/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/function_prototypes/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.167847 cengal-3.2.0.1/cengal/ctypes_tools/function_prototypes/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/function_prototypes/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.197847 cengal-3.2.0.1/cengal/ctypes_tools/function_prototypes/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1279 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/function_prototypes/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.217847 cengal-3.2.0.1/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5487 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/function_prototypes/versions/v_0/win_function_prototypes.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.247847 cengal-3.2.0.1/cengal/ctypes_tools/functions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/functions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.247847 cengal-3.2.0.1/cengal/ctypes_tools/functions/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/functions/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.277847 cengal-3.2.0.1/cengal/ctypes_tools/functions/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1295 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/functions/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1316 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/functions/versions/v_0/functions.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.317847 cengal-3.2.0.1/cengal/ctypes_tools/functions/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/functions/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/functions/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1501 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/functions/versions/v_0/win_functions.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.317847 cengal-3.2.0.1/cengal/ctypes_tools/libraries/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/libraries/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.327847 cengal-3.2.0.1/cengal/ctypes_tools/libraries/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/libraries/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.347847 cengal-3.2.0.1/cengal/ctypes_tools/libraries/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1269 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/libraries/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.367847 cengal-3.2.0.1/cengal/ctypes_tools/libraries/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/libraries/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/libraries/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1481 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/libraries/versions/v_0/win_libraries.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.397847 cengal-3.2.0.1/cengal/ctypes_tools/result_api/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/result_api/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.407847 cengal-3.2.0.1/cengal/ctypes_tools/result_api/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/result_api/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.437847 cengal-3.2.0.1/cengal/ctypes_tools/result_api/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1335 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/result_api/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1221 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/result_api/versions/v_0/result_api.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1304 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/result_api/versions/v_0/result_api_exceptions.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.467847 cengal-3.2.0.1/cengal/ctypes_tools/result_api/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/result_api/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/result_api/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2728 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/result_api/versions/v_0/win_result_api.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.467847 cengal-3.2.0.1/cengal/ctypes_tools/tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/tools/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.477847 cengal-3.2.0.1/cengal/ctypes_tools/tools/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/tools/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.567847 cengal-3.2.0.1/cengal/ctypes_tools/tools/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1287 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/tools/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.587847 cengal-3.2.0.1/cengal/ctypes_tools/tools/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/tools/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/tools/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1596 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/tools/versions/v_0/tools.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1600 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/tools/versions/v_0/win_tools.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.597847 cengal-3.2.0.1/cengal/ctypes_tools/types/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/types/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.597847 cengal-3.2.0.1/cengal/ctypes_tools/types/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/types/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.617847 cengal-3.2.0.1/cengal/ctypes_tools/types/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1265 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/types/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.637847 cengal-3.2.0.1/cengal/ctypes_tools/types/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/types/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/types/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7772 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/ctypes_tools/types/versions/v_0/win_types.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.647847 cengal-3.2.0.1/cengal/cython_tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/cython_tools/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1773 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/cython_tools/cythonyser_setup_runner.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.657847 cengal-3.2.0.1/cengal/data_containers/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.667847 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.667847 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.677847 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.697847 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2228 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/versions/v_0/manager.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.717846 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.747847 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2211 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/versions/v_1/manager.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.777847 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.787847 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1278 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.797847 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.807847 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.847847 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1251 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1541 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/key__hashable__to__value__set.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.867847 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.877847 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key_counter/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key_counter/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.917847 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.937847 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1597 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/key_counter.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.957846 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.967846 cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.967846 cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.987846 cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1624 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    24426 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/dynamic_list_of_pieces__cython.pyx
+-rw-r--r--   0 mb        (1000) mb        (1000)    28853 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/dynamic_list_of_pieces__python.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:07.997846 cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.017847 cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1624 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    24390 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/dynamic_list_of_pieces__cython.pyx
+-rw-r--r--   0 mb        (1000) mb        (1000)    28796 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/dynamic_list_of_pieces__python.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.037847 cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.047847 cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.077847 cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.117847 cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)    39955 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_0/TagDB.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1259 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5404 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_0/tag_db_interface.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.127847 cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.147847 cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)    41894 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_1/TagDB.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1259 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    13149 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_1/tag_db_interface.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.147847 cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.167847 cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_2/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1259 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_2/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     9729 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_2/dynamic_tag_tree.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.177847 cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.177847 cengal-3.2.0.1/cengal/data_containers/fast_fifo/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/fast_fifo/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.187847 cengal-3.2.0.1/cengal/data_containers/fast_fifo/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/fast_fifo/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.197847 cengal-3.2.0.1/cengal/data_containers/fast_fifo/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/fast_fifo/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    12327 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/fast_fifo/versions/v_0/fast_fifo.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.217846 cengal-3.2.0.1/cengal/data_containers/fast_fifo/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/fast_fifo/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/fast_fifo/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.237846 cengal-3.2.0.1/cengal/data_containers/fast_fifo/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/fast_fifo/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    12275 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/fast_fifo/versions/v_1/fast_fifo.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.257846 cengal-3.2.0.1/cengal/data_containers/fast_fifo/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/fast_fifo/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/fast_fifo/versions/v_1/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.267846 cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.277846 cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.307847 cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2033 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/versions/v_0/limitable_dict_with_order.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.317847 cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.337847 cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2464 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/versions/v_1/limitable_dict_with_order.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.347847 cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.357847 cengal-3.2.0.1/cengal/data_containers/simple_tree/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/simple_tree/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.367847 cengal-3.2.0.1/cengal/data_containers/simple_tree/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/simple_tree/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.377847 cengal-3.2.0.1/cengal/data_containers/simple_tree/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/simple_tree/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5000 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/simple_tree/versions/v_0/simple_tree.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.387847 cengal-3.2.0.1/cengal/data_containers/stack/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/stack/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.417847 cengal-3.2.0.1/cengal/data_containers/stack/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/stack/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.437847 cengal-3.2.0.1/cengal/data_containers/stack/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1227 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/stack/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4659 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/stack/versions/v_0/stack.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.457846 cengal-3.2.0.1/cengal/data_containers/stack/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/stack/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3695 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_containers/stack/versions/v_0/tests/test__stack.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.467846 cengal-3.2.0.1/cengal/data_generation/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_generation/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.477846 cengal-3.2.0.1/cengal/data_generation/id_generator/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_generation/id_generator/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.497846 cengal-3.2.0.1/cengal/data_generation/id_generator/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_generation/id_generator/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.497846 cengal-3.2.0.1/cengal/data_generation/id_generator/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_generation/id_generator/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2217 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_generation/id_generator/versions/v_0/id_generator.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.517846 cengal-3.2.0.1/cengal/data_generation/id_generator/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_generation/id_generator/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_generation/id_generator/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.537846 cengal-3.2.0.1/cengal/data_generation/id_generator/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_generation/id_generator/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3044 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_generation/id_generator/versions/v_1/id_generator.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.567846 cengal-3.2.0.1/cengal/data_generation/id_generator/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_generation/id_generator/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_generation/id_generator/versions/v_1/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.577847 cengal-3.2.0.1/cengal/data_manipulation/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.607847 cengal-3.2.0.1/cengal/data_manipulation/conversion/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1209 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.617847 cengal-3.2.0.1/cengal/data_manipulation/conversion/bit_cast_like/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/bit_cast_like/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.617847 cengal-3.2.0.1/cengal/data_manipulation/conversion/bit_cast_like/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/bit_cast_like/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.647847 cengal-3.2.0.1/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2011 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/bit_cast_like.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.697847 cengal-3.2.0.1/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.717846 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.727846 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.747846 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2475 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/reinterpret_cast.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.757846 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.767846 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1209 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.767846 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.777846 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.797846 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8110 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/manager.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.807846 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.807846 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1209 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.817846 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.827846 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.847847 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2548 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/copy_wrapper.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.867847 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.867847 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.867847 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.877847 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2564 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/deep_copy_wrapper.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.907847 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.917847 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.917847 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.937847 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.967846 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3538 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/uni_copy_wrapper.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.967846 cengal-3.2.0.1/cengal/data_manipulation/front_triggerable_variable/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/front_triggerable_variable/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.987846 cengal-3.2.0.1/cengal/data_manipulation/front_triggerable_variable/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/front_triggerable_variable/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:08.987846 cengal-3.2.0.1/cengal/data_manipulation/front_triggerable_variable/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/front_triggerable_variable/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3916 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/front_triggerable_variable/versions/v_0/front_triggerable_variable.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.017846 cengal-3.2.0.1/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.027846 cengal-3.2.0.1/cengal/data_manipulation/get_dict_key_with_callable_default/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/get_dict_key_with_callable_default/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.037846 cengal-3.2.0.1/cengal/data_manipulation/get_dict_key_with_callable_default/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/get_dict_key_with_callable_default/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.057846 cengal-3.2.0.1/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1256 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1483 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/get_dict_key_with_callable_default.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.127847 cengal-3.2.0.1/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7544 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/help_tools.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.127847 cengal-3.2.0.1/cengal/data_manipulation/objects_counter/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/objects_counter/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.137847 cengal-3.2.0.1/cengal/data_manipulation/objects_counter/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/objects_counter/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.147847 cengal-3.2.0.1/cengal/data_manipulation/objects_counter/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/objects_counter/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2980 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/objects_counter/versions/v_0/objects_counter.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.167847 cengal-3.2.0.1/cengal/data_manipulation/objects_counter/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1243 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/objects_counter/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6511 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/objects_counter/versions/v_0/tests/test__objects_counter.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.177847 cengal-3.2.0.1/cengal/data_manipulation/performant_list_operations/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/performant_list_operations/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.187847 cengal-3.2.0.1/cengal/data_manipulation/performant_list_operations/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/performant_list_operations/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.247846 cengal-3.2.0.1/cengal/data_manipulation/performant_list_operations/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1244 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/performant_list_operations/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     9310 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/performant_list_operations/versions/v_0/remove_items_from_list.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.287846 cengal-3.2.0.1/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.297846 cengal-3.2.0.1/cengal/data_manipulation/serialization/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/serialization/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.307846 cengal-3.2.0.1/cengal/data_manipulation/serialization/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/serialization/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.317846 cengal-3.2.0.1/cengal/data_manipulation/serialization/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/serialization/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    27320 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/serialization/versions/v_0/serialization.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.337846 cengal-3.2.0.1/cengal/data_manipulation/serialization/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1241 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/serialization/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4070 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/serialization/versions/v_0/tests/test__serialization.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.337846 cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.367847 cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.387847 cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.417847 cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2651 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_0/tests/traverstal_manual_tests.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8191 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_0/tree_traversal.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.417847 cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_1/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.487846 cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_1/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2614 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_1/tests/key_multi_value_traverstal_manual_tests.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2813 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_1/tests/key_value_traverstal_manual_tests.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2746 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_1/tests/traverstal_manual_tests.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    24127 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_1/tree_traversal.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5495 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/docten.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.487846 cengal-3.2.0.1/cengal/entities/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/entities/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.487846 cengal-3.2.0.1/cengal/entities/bindable_to_type/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/entities/bindable_to_type/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.497846 cengal-3.2.0.1/cengal/entities/bindable_to_type/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/entities/bindable_to_type/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.507846 cengal-3.2.0.1/cengal/entities/bindable_to_type/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/entities/bindable_to_type/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4359 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/entities/bindable_to_type/versions/v_0/bindable_to_type.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.517846 cengal-3.2.0.1/cengal/entities/bindable_to_type/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/entities/bindable_to_type/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/entities/bindable_to_type/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.537846 cengal-3.2.0.1/cengal/entities/copyable/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/entities/copyable/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.547846 cengal-3.2.0.1/cengal/entities/copyable/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/entities/copyable/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.557846 cengal-3.2.0.1/cengal/entities/copyable/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/entities/copyable/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4449 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/entities/copyable/versions/v_0/copyable.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.567846 cengal-3.2.0.1/cengal/entities/copyable/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/entities/copyable/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/entities/copyable/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.627846 cengal-3.2.0.1/cengal/file_settings_manager/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_settings_manager/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7335 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_settings_manager/config_manager.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_settings_manager/dir_templates.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.657847 cengal-3.2.0.1/cengal/file_system/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.667847 cengal-3.2.0.1/cengal/file_system/app_fs_structure/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/app_fs_structure/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.667847 cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.677847 cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.767846 cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1547 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1288 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_exceptions.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4301 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_base.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8623 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_darwin.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8512 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_linux.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7082 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_win.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3824 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_directory_types.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.777846 cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8150 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/directory_manager.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2528 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/file_manager.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.817846 cengal-3.2.0.1/cengal/file_system/file_patch/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/file_patch/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.817846 cengal-3.2.0.1/cengal/file_system/file_patch/brackets/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/file_patch/brackets/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.817846 cengal-3.2.0.1/cengal/file_system/file_patch/brackets/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/file_patch/brackets/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.837846 cengal-3.2.0.1/cengal/file_system/file_patch/brackets/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/file_patch/brackets/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2365 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/file_patch/brackets/versions/v_0/brackets.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.847846 cengal-3.2.0.1/cengal/file_system/file_patch/brackets/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/file_patch/brackets/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/file_patch/brackets/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.847846 cengal-3.2.0.1/cengal/file_system/file_patch/generic/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/file_patch/generic/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.857846 cengal-3.2.0.1/cengal/file_system/file_patch/generic/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/file_patch/generic/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.887846 cengal-3.2.0.1/cengal/file_system/file_patch/generic/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/file_patch/generic/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2227 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/file_patch/generic/versions/v_0/generic.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.907847 cengal-3.2.0.1/cengal/file_system/file_patch/generic/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/file_patch/generic/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/file_patch/generic/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.947847 cengal-3.2.0.1/cengal/file_system/file_patch/simple/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/file_patch/simple/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.967846 cengal-3.2.0.1/cengal/file_system/file_patch/simple/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/file_patch/simple/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.967846 cengal-3.2.0.1/cengal/file_system/file_patch/simple/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/file_patch/simple/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2310 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/file_patch/simple/versions/v_0/simple.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.977846 cengal-3.2.0.1/cengal/file_system/file_patch/simple/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/file_patch/simple/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/file_patch/simple/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.987846 cengal-3.2.0.1/cengal/file_system/path_manager/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/path_manager/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:09.987846 cengal-3.2.0.1/cengal/file_system/path_manager/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/path_manager/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.007846 cengal-3.2.0.1/cengal/file_system/path_manager/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/path_manager/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2580 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/path_manager/versions/v_0/path_manager.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.027846 cengal-3.2.0.1/cengal/file_system/path_manager/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/path_manager/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/path_manager/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.077846 cengal-3.2.0.1/cengal/file_system/win_fs/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/win_fs/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3113 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/win_fs/base.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1850 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/win_fs/global_install_uninstall.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1996 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/win_fs/path.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5189 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/win_fs/shutil.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4436 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/file_system/win_fs/shutil_readable.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.087846 cengal-3.2.0.1/cengal/hardware/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1209 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.097846 cengal-3.2.0.1/cengal/hardware/info/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1209 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/info/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.097846 cengal-3.2.0.1/cengal/hardware/info/cpu/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/info/cpu/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.097846 cengal-3.2.0.1/cengal/hardware/info/cpu/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/info/cpu/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.117846 cengal-3.2.0.1/cengal/hardware/info/cpu/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/info/cpu/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2281 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/info/cpu/versions/v_0/cpu.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.147846 cengal-3.2.0.1/cengal/hardware/info/cpu/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/info/cpu/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/info/cpu/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.157846 cengal-3.2.0.1/cengal/hardware/info/cpu/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/info/cpu/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8747 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/info/cpu/versions/v_1/cpu.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.177847 cengal-3.2.0.1/cengal/hardware/info/cpu/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/info/cpu/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/info/cpu/versions/v_1/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.187847 cengal-3.2.0.1/cengal/hardware/memory/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1209 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/memory/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.197847 cengal-3.2.0.1/cengal/hardware/memory/barriers/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/memory/barriers/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.197847 cengal-3.2.0.1/cengal/hardware/memory/barriers/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/memory/barriers/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.207846 cengal-3.2.0.1/cengal/hardware/memory/barriers/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/memory/barriers/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.217846 cengal-3.2.0.1/cengal/hardware/memory/barriers/versions/v_0/compilable/
+-rw-r--r--   0 mb        (1000) mb        (1000)     2021 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/memory/barriers/versions/v_0/compilable/__build_config.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1354 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/memory/barriers/versions/v_0/compilable/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7924 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/memory/barriers/versions/v_0/compilable/barriers__cython.pyx
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.227846 cengal-3.2.0.1/cengal/hardware/memory/barriers/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/memory/barriers/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/memory/barriers/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.227846 cengal-3.2.0.1/cengal/hardware/memory/shared_memory/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/memory/shared_memory/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.227846 cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.267846 cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1348 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.267846 cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/v_0/compilable/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1932 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/v_0/compilable/__build_config.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1359 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/v_0/compilable/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5299 2023-05-22 07:53:53.000000 cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/v_0/compilable/memory_access.c
+-rw-r--r--   0 mb        (1000) mb        (1000)     3039 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/v_0/compilable/memory_access.h
+-rw-r--r--   0 mb        (1000) mb        (1000)    11807 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/v_0/compilable/memory_access__cython.pyx
+-rw-r--r--   0 mb        (1000) mb        (1000)     4229 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/v_0/interfaces.py
+-rw-r--r--   0 mb        (1000) mb        (1000)   108882 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/v_0/shared_memory.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.297846 cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8552 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/help_tools.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.297846 cengal-3.2.0.1/cengal/introspection/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/introspection/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.317846 cengal-3.2.0.1/cengal/introspection/inspect/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/introspection/inspect/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.317846 cengal-3.2.0.1/cengal/introspection/inspect/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/introspection/inspect/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.347846 cengal-3.2.0.1/cengal/introspection/inspect/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/introspection/inspect/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    19833 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/introspection/inspect/versions/v_0/inspect.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.367846 cengal-3.2.0.1/cengal/introspection/inspect/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/introspection/inspect/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/introspection/inspect/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.367846 cengal-3.2.0.1/cengal/introspection/third_party/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1209 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/introspection/third_party/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.377846 cengal-3.2.0.1/cengal/introspection/third_party/ctypes/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/introspection/third_party/ctypes/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.387846 cengal-3.2.0.1/cengal/introspection/third_party/ctypes/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/introspection/third_party/ctypes/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.427847 cengal-3.2.0.1/cengal/introspection/third_party/ctypes/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/introspection/third_party/ctypes/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5358 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/introspection/third_party/ctypes/versions/v_0/ctypes.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.437847 cengal-3.2.0.1/cengal/introspection/third_party/ctypes/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/introspection/third_party/ctypes/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/introspection/third_party/ctypes/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.447847 cengal-3.2.0.1/cengal/io/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.447847 cengal-3.2.0.1/cengal/io/asock_io/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/asock_io/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.467846 cengal-3.2.0.1/cengal/io/asock_io/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/asock_io/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.497846 cengal-3.2.0.1/cengal/io/asock_io/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1280 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/asock_io/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6005 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/asock_io/versions/v_0/base.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.497846 cengal-3.2.0.1/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1528 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3766 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/recv_buff_size_computer__cython.pyx
+-rw-r--r--   0 mb        (1000) mb        (1000)     3191 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/recv_buff_size_computer__python.py
+-rw-r--r--   0 mb        (1000) mb        (1000)   113358 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/asock_io/versions/v_0/tcp_app_server.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5056 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/asock_io/versions/v_0/tcp_link.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.577846 cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1280 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    18745 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/abstract.py
+-rw-r--r--   0 mb        (1000) mb        (1000)   123888 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/asock_io_core.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    15714 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/base.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.597846 cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/io_loops/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/io_loops/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3921 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/io_loops/epoll_lt.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6408 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/io_loops/select.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.597846 cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1475 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3701 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/recv_buff_size_computer__cython.pyx
+-rw-r--r--   0 mb        (1000) mb        (1000)     3129 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/recv_buff_size_computer__python.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4986 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/tcp_link.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.617846 cengal-3.2.0.1/cengal/io/core/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/core/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.667846 cengal-3.2.0.1/cengal/io/core/memory_management/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/core/memory_management/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.667846 cengal-3.2.0.1/cengal/io/core/memory_management/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/core/memory_management/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.687846 cengal-3.2.0.1/cengal/io/core/memory_management/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/core/memory_management/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3261 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/core/memory_management/versions/v_0/memory_management.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.717846 cengal-3.2.0.1/cengal/io/core/memory_management/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/core/memory_management/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/core/memory_management/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.717846 cengal-3.2.0.1/cengal/io/named_connections/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/named_connections/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.717846 cengal-3.2.0.1/cengal/io/named_connections/named_connections_manager/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/named_connections/named_connections_manager/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.727846 cengal-3.2.0.1/cengal/io/named_connections/named_connections_manager/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/named_connections/named_connections_manager/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.777846 cengal-3.2.0.1/cengal/io/named_connections/named_connections_manager/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/named_connections/named_connections_manager/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    10643 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/named_connections/named_connections_manager/versions/v_0/named_connections_manager.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.797846 cengal-3.2.0.1/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.797846 cengal-3.2.0.1/cengal/io/named_connections/workers/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/named_connections/workers/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.807846 cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.807846 cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.827846 cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6609 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/asyncio_streams.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.867846 cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.887846 cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams_proxy/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams_proxy/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.897846 cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.917846 cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1243 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/asyncio_streams_proxy.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.927846 cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.937846 cengal-3.2.0.1/cengal/io/net_io/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/net_io/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.947846 cengal-3.2.0.1/cengal/io/net_io/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/net_io/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.987846 cengal-3.2.0.1/cengal/io/net_io/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/net_io/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:10.997846 cengal-3.2.0.1/cengal/io/net_io/versions/v_0/crossplatform/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/net_io/versions/v_0/crossplatform/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.017846 cengal-3.2.0.1/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/abstract.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/linux.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/win32.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    11974 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/net_io/versions/v_0/net_io__linux.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    14772 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/net_io/versions/v_0/net_io_abstract.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3986 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/net_io/versions/v_0/net_io_method__epoll_lt.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4845 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/net_io/versions/v_0/net_io_method__select.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.017846 cengal-3.2.0.1/cengal/io/recv_buff_size_computer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/recv_buff_size_computer/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.047846 cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.047846 cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1528 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3766 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/v_0/recv_buff_size_computer__cython.pyx
+-rw-r--r--   0 mb        (1000) mb        (1000)     3191 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/v_0/recv_buff_size_computer__python.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.067846 cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.117846 cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1475 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3701 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/v_1/recv_buff_size_computer__cython.pyx
+-rw-r--r--   0 mb        (1000) mb        (1000)     3129 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/v_1/recv_buff_size_computer__python.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.147846 cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/v_1/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.167846 cengal-3.2.0.1/cengal/io/serve_free_ports/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/serve_free_ports/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.167846 cengal-3.2.0.1/cengal/io/serve_free_ports/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/serve_free_ports/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.187846 cengal-3.2.0.1/cengal/io/serve_free_ports/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/serve_free_ports/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5138 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/serve_free_ports/versions/v_0/serve_free_ports.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.217846 cengal-3.2.0.1/cengal/io/serve_free_ports/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/serve_free_ports/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/serve_free_ports/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.227846 cengal-3.2.0.1/cengal/io/socket/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/socket/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.227846 cengal-3.2.0.1/cengal/io/socket/constants/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/socket/constants/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.247846 cengal-3.2.0.1/cengal/io/socket/constants/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/socket/constants/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.267846 cengal-3.2.0.1/cengal/io/socket/constants/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/socket/constants/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1281 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/socket/constants/versions/v_0/constants.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.297846 cengal-3.2.0.1/cengal/io/socket/constants/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/socket/constants/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/socket/constants/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.337846 cengal-3.2.0.1/cengal/io/socket/errors/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/socket/errors/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.347846 cengal-3.2.0.1/cengal/io/socket/errors/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/socket/errors/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.387846 cengal-3.2.0.1/cengal/io/socket/errors/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/socket/errors/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2429 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/socket/errors/versions/v_0/errors.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.397846 cengal-3.2.0.1/cengal/io/socket/errors/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/socket/errors/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/socket/errors/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.397846 cengal-3.2.0.1/cengal/io/used_ports/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/used_ports/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.397846 cengal-3.2.0.1/cengal/io/used_ports/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/used_ports/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.417846 cengal-3.2.0.1/cengal/io/used_ports/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/used_ports/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.447846 cengal-3.2.0.1/cengal/io/used_ports/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/used_ports/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3132 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/used_ports/versions/v_0/tests/_test__used_ports.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8978 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/io/used_ports/versions/v_0/used_ports.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.447846 cengal-3.2.0.1/cengal/math/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/math/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.467846 cengal-3.2.0.1/cengal/math/algebra/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/math/algebra/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.467846 cengal-3.2.0.1/cengal/math/algebra/fast_algorithms/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/math/algebra/fast_algorithms/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.477846 cengal-3.2.0.1/cengal/math/algebra/fast_algorithms/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/math/algebra/fast_algorithms/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.487846 cengal-3.2.0.1/cengal/math/algebra/fast_algorithms/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/math/algebra/fast_algorithms/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1783 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/math/algebra/fast_algorithms/versions/v_0/fast_algorithms.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.517846 cengal-3.2.0.1/cengal/math/algebra/fast_algorithms/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/math/algebra/fast_algorithms/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/math/algebra/fast_algorithms/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.537846 cengal-3.2.0.1/cengal/math/geometry/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/math/geometry/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.547846 cengal-3.2.0.1/cengal/math/geometry/ellipse/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:09.000000 cengal-3.2.0.1/cengal/math/geometry/ellipse/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.557846 cengal-3.2.0.1/cengal/math/geometry/ellipse/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/math/geometry/ellipse/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.577846 cengal-3.2.0.1/cengal/math/geometry/ellipse/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/math/geometry/ellipse/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4988 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/math/geometry/ellipse/versions/v_0/ellipse.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.607846 cengal-3.2.0.1/cengal/math/geometry/ellipse/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/math/geometry/ellipse/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/math/geometry/ellipse/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2713 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/math/geometry/ellipse/versions/v_0/tests/informal_tests.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.617846 cengal-3.2.0.1/cengal/math/geometry/point/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/math/geometry/point/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.627846 cengal-3.2.0.1/cengal/math/geometry/point/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/math/geometry/point/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.647846 cengal-3.2.0.1/cengal/math/geometry/point/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1227 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/math/geometry/point/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    16019 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/math/geometry/point/versions/v_0/point.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.667846 cengal-3.2.0.1/cengal/math/geometry/point/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/math/geometry/point/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/math/geometry/point/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.667846 cengal-3.2.0.1/cengal/math/geometry/vector/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/math/geometry/vector/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.677846 cengal-3.2.0.1/cengal/math/geometry/vector/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/math/geometry/vector/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.717846 cengal-3.2.0.1/cengal/math/geometry/vector/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/math/geometry/vector/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.747846 cengal-3.2.0.1/cengal/math/geometry/vector/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/math/geometry/vector/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/math/geometry/vector/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    46032 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/math/geometry/vector/versions/v_0/vector.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.747846 cengal-3.2.0.1/cengal/math/numbers/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/math/numbers/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.757846 cengal-3.2.0.1/cengal/math/numbers/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/math/numbers/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.797846 cengal-3.2.0.1/cengal/math/numbers/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/math/numbers/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1346 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/math/numbers/versions/v_0/numbers.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.817846 cengal-3.2.0.1/cengal/math/numbers/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/math/numbers/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/math/numbers/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.857846 cengal-3.2.0.1/cengal/modules_management/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/modules_management/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1569 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/modules_management/alternative_import.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.877846 cengal-3.2.0.1/cengal/modules_management/ignore_in_build_mode/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/modules_management/ignore_in_build_mode/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.887846 cengal-3.2.0.1/cengal/modules_management/ignore_in_build_mode/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/modules_management/ignore_in_build_mode/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.917846 cengal-3.2.0.1/cengal/modules_management/ignore_in_build_mode/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/modules_management/ignore_in_build_mode/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1511 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/modules_management/ignore_in_build_mode/versions/v_0/ignore_in_build_mode.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.927846 cengal-3.2.0.1/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2182 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/modules_management/reload_module.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.937846 cengal-3.2.0.1/cengal/os/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/os/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1348 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/os/help_tools.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.967846 cengal-3.2.0.1/cengal/parallel_execution/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.967846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.987846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/atasks/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/atasks/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:11.997846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/atasks/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/atasks/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.027846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/atasks/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/atasks/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1847 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/atasks/versions/v_0/atasks.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.047846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.047846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.057846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.117846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1360 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    12104 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_abstract.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2467 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_base.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1989 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_base_internal.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    51581 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tcp_efficient_streams.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.147846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3772 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/asyncio_streams_client.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6497 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/asyncio_streams_server.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    35909 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/udp_efficient_streams.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.157846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/init_loop/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/init_loop/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.167846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/init_loop/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/init_loop/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.187846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/init_loop/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/init_loop/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1392 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/init_loop/versions/v_0/init_loop.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.197846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.227846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_in_process_pool/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_in_process_pool/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.237846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_in_process_pool/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_in_process_pool/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.247846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1241 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     9439 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/run_in_process_pool.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.267846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.267846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_loop/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_loop/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.277846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_loop/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_loop/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.287846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_loop/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_loop/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3526 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_loop/versions/v_0/run_loop.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.297846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.297846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/timed_yield/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/timed_yield/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.297846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/timed_yield/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/timed_yield/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.327846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.337846 cengal-3.2.0.1/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1641 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/timed_yield.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.337846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-23 18:41:05.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.357846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_scheduler/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_scheduler/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.357846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_scheduler/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_scheduler/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.367846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-23 18:19:54.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)   126513 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/coro_scheduler.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.377846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.377846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-23 18:41:05.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.377846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.387846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.397846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    11264 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/async_event_bus.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.407846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.417846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.427846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.447846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    20727 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/asyncio_loop.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.447846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.457846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/communication/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/communication/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.467846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.477846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6565 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/communication.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.527846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.547846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.547846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.587846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4173 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/cpu_tick_count_per_second.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.627846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.637846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/db/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/db/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.637846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.667846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1224 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    55877 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/db.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.697846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.727846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.727846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.777846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7706 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/event_bus.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.797846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.797846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.807846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.827846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7637 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/fast_aggregator.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.837846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.847846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/instance/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/instance/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.847846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.877846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     9088 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/instance.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.887846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.897846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.907846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.907846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5521 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/kill_coro.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.917846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.937846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.947846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.957846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7536 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/kill_coro_list.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.967846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:12.987846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.007846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.017846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3907 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/lazy_print.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.047846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.057846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.067846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.097846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    21254 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/lmdb.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.117846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.127846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/log/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/log/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.137846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.147846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    13685 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/log.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.157846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.157846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.167846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.187846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1264 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5970 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/bytecode_patcher.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    27435 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/loop_yield.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.197846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.207846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.217846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.217846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    22656 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/put_coro.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.227846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.237846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.257846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.277846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6167 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/put_coro_list.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.287846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.297846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.307846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.327846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    25203 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/read_write_locker.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.357846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.367846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.367846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.447846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4955 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/class_info.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3826 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/commands.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1398 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/exceptions.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5315 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/remote_node.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    21054 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/remote_nodes.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6043 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/request_class_info.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5876 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/serializers.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.447846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.447846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.457846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.477846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3464 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/run_coro.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.507846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.517846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.527846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.557846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1747 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/shutdown_loop.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.587846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.607846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.607846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.627846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1252 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2896 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/shutdown_on_keyboard_interrupt.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.647846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.647846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.657846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.657846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1651 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/simple_yield.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.697846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.717846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/sleep/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/sleep/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.727846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.747846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2900 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/sleep.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.767846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.777846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.787846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.807846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1724 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/some_printer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.827846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.827846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.837846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.857846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.867846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6824 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/throw_coro.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.867846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.887846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.907846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.907846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7153 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/throw_coro_list.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.917846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.917846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:13.947846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:22.707846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    11821 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/timer_coro_runner.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:22.717846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:22.717846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:22.717846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:22.717846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    11052 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/timer_func_runner.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:22.717846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:22.717846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:22.717846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:22.717846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    28116 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tkinter.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:22.717846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:22.717846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:22.717846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:22.847846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    18946 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/wait_coro.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:22.847846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1209 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:22.867846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:22.887846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:22.897846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/general.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:22.927846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:22.937846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:22.947846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:22.997846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1251 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5686 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/service_with_a_direct_request.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.027846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.047846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-23 18:41:05.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.047846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/await_coro/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/await_coro/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.057846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.087846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    14141 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/await_coro.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.127846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.127846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.147846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.147846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5185 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/coro_flow_control.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.177846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.187846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/low_latency/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/low_latency/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.197846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.207846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.257846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3174 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/ajson.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5181 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/json.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.267846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.267846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.287846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.317846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5978 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/prepare_loop.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.347846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.347846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.377846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.407846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8390 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/run_in_loop.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.427846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.437846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/wait_coro/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/wait_coro/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.467846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.507846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.537846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7875 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/wait_coro.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.537846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1209 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.557846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/customtkinter/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/customtkinter/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.577846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.617846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1828 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/customtkinter.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.637846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.637846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/nicegui/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/nicegui/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.637846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/nicegui/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/nicegui/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.677846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    19200 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/nicegui.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.677846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.707846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/pytermgui/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/pytermgui/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.707846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.727846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4690 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/pytermgui.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.747846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.747846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/qt/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/qt/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.777846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/qt/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/qt/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.787846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1224 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    13309 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/qt.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.807846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.807846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvicorn/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvicorn/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.827846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.827846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.867846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5546 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/uvicorn.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.867846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvloop/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvloop/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.867846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvloop/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvloop/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.907846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.967846 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1529 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/uvloop.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:23.977846 cengal-3.2.0.1/cengal/parallel_execution/green_threads_tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/green_threads_tools/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3706 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/green_threads_tools/task_management.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.027846 cengal-3.2.0.1/cengal/parallel_execution/multiprocess/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1250 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/multiprocess/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2839 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/multiprocess/multiprocess_testing.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3085 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/multiprocess/multiprocessing_task_pool.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    24842 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/multiprocess/multiprocessing_task_runner.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.077846 cengal-3.2.0.1/cengal/parallel_execution/multithreading/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/multithreading/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7150 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/parallel_execution/multithreading/thread_workers_pool.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.077846 cengal-3.2.0.1/cengal/performance_test_lib/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/performance_test_lib/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.097846 cengal-3.2.0.1/cengal/performance_test_lib/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/performance_test_lib/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.127846 cengal-3.2.0.1/cengal/performance_test_lib/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/performance_test_lib/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8267 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/performance_test_lib/versions/v_0/performance_test_lib.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.177846 cengal-3.2.0.1/cengal/performance_test_lib/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/performance_test_lib/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2240 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/performance_test_lib/versions/v_0/tests/test__performance_test_lib.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.187846 cengal-3.2.0.1/cengal/performance_test_lib/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/performance_test_lib/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     9290 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/performance_test_lib/versions/v_1/performance_test_lib.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.217846 cengal-3.2.0.1/cengal/performance_test_lib/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/performance_test_lib/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2240 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/performance_test_lib/versions/v_1/tests/test__performance_test_lib.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.217846 cengal-3.2.0.1/cengal/shared_memory/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/shared_memory/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.247846 cengal-3.2.0.1/cengal/shared_memory/versions/
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.277846 cengal-3.2.0.1/cengal/shared_memory/versions/1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/shared_memory/versions/1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1501 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/shared_memory/versions/1/mmap.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/shared_memory/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.307846 cengal-3.2.0.1/cengal/statistics/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/statistics/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.317846 cengal-3.2.0.1/cengal/statistics/normal_distribution/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/statistics/normal_distribution/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.317846 cengal-3.2.0.1/cengal/statistics/normal_distribution/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/statistics/normal_distribution/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.347846 cengal-3.2.0.1/cengal/statistics/normal_distribution/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1241 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/statistics/normal_distribution/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4156 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/statistics/normal_distribution/versions/v_0/normal_distribution.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.367846 cengal-3.2.0.1/cengal/statistics/normal_distribution/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/statistics/normal_distribution/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/statistics/normal_distribution/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3261 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/system.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.367846 cengal-3.2.0.1/cengal/testing_lib/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/testing_lib/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3056 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/testing_lib/tests_list_runner.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.397846 cengal-3.2.0.1/cengal/text_processing/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.407846 cengal-3.2.0.1/cengal/text_processing/brackets_processing/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/brackets_processing/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.427846 cengal-3.2.0.1/cengal/text_processing/brackets_processing/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/brackets_processing/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.497846 cengal-3.2.0.1/cengal/text_processing/brackets_processing/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1289 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/brackets_processing/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2344 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/brackets_processing/versions/v_0/brackets.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6467 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/brackets_processing/versions/v_0/processing.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3779 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/brackets_processing/versions/v_0/standard_brackets.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.537846 cengal-3.2.0.1/cengal/text_processing/brackets_processing/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/brackets_processing/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/brackets_processing/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.557846 cengal-3.2.0.1/cengal/text_processing/encoding_detection/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/encoding_detection/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.587846 cengal-3.2.0.1/cengal/text_processing/encoding_detection/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/encoding_detection/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.607846 cengal-3.2.0.1/cengal/text_processing/encoding_detection/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/encoding_detection/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2464 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/encoding_detection/versions/v_0/encoding_detection.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.657846 cengal-3.2.0.1/cengal/text_processing/encoding_detection/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/encoding_detection/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/encoding_detection/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    11968 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/help_tools.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.667846 cengal-3.2.0.1/cengal/text_processing/optional_formatter/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/optional_formatter/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.677846 cengal-3.2.0.1/cengal/text_processing/optional_formatter/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/optional_formatter/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.697846 cengal-3.2.0.1/cengal/text_processing/optional_formatter/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/optional_formatter/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4274 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/optional_formatter/versions/v_0/optional_formatter.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.727846 cengal-3.2.0.1/cengal/text_processing/optional_formatter/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/optional_formatter/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/optional_formatter/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.727846 cengal-3.2.0.1/cengal/text_processing/simple_config_file_processor/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/simple_config_file_processor/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.747846 cengal-3.2.0.1/cengal/text_processing/simple_config_file_processor/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/simple_config_file_processor/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.757846 cengal-3.2.0.1/cengal/text_processing/simple_config_file_processor/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1250 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/simple_config_file_processor/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/simple_config_file_processor/versions/v_0/simple_config_file_processor.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.807846 cengal-3.2.0.1/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.807846 cengal-3.2.0.1/cengal/text_processing/text_patch/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_patch/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.827846 cengal-3.2.0.1/cengal/text_processing/text_patch/brackets/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_patch/brackets/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.827846 cengal-3.2.0.1/cengal/text_processing/text_patch/brackets/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_patch/brackets/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.857846 cengal-3.2.0.1/cengal/text_processing/text_patch/brackets/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_patch/brackets/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2009 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_patch/brackets/versions/v_0/brackets.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.907846 cengal-3.2.0.1/cengal/text_processing/text_patch/brackets/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_patch/brackets/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_patch/brackets/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.927846 cengal-3.2.0.1/cengal/text_processing/text_patch/simple/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_patch/simple/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.947846 cengal-3.2.0.1/cengal/text_processing/text_patch/simple/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_patch/simple/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:24.967846 cengal-3.2.0.1/cengal/text_processing/text_patch/simple/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_patch/simple/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1829 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_patch/simple/versions/v_0/simple.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.017846 cengal-3.2.0.1/cengal/text_processing/text_patch/simple/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_patch/simple/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_patch/simple/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.017846 cengal-3.2.0.1/cengal/text_processing/text_processing/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_processing/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.037846 cengal-3.2.0.1/cengal/text_processing/text_processing/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_processing/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.047846 cengal-3.2.0.1/cengal/text_processing/text_processing/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_processing/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6281 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_processing/versions/v_0/processing.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.047846 cengal-3.2.0.1/cengal/text_processing/text_processing/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_processing/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_processing/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.057846 cengal-3.2.0.1/cengal/text_processing/text_translator/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_translator/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.077846 cengal-3.2.0.1/cengal/text_processing/text_translator/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_translator/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.087846 cengal-3.2.0.1/cengal/text_processing/text_translator/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_translator/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.117846 cengal-3.2.0.1/cengal/text_processing/text_translator/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_translator/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_translator/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    12695 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/text_translator/versions/v_0/text_translator.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.117846 cengal-3.2.0.1/cengal/text_processing/utf_bom_processing/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/utf_bom_processing/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.127846 cengal-3.2.0.1/cengal/text_processing/utf_bom_processing/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/utf_bom_processing/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.167846 cengal-3.2.0.1/cengal/text_processing/utf_bom_processing/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/utf_bom_processing/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.207846 cengal-3.2.0.1/cengal/text_processing/utf_bom_processing/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/utf_bom_processing/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/utf_bom_processing/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2993 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/text_processing/utf_bom_processing/versions/v_0/utf_bom_processing.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.217846 cengal-3.2.0.1/cengal/time_management/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/time_management/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.217846 cengal-3.2.0.1/cengal/time_management/cpu_clock/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/time_management/cpu_clock/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.227846 cengal-3.2.0.1/cengal/time_management/cpu_clock/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/time_management/cpu_clock/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.257846 cengal-3.2.0.1/cengal/time_management/cpu_clock/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/time_management/cpu_clock/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.277846 cengal-3.2.0.1/cengal/time_management/cpu_clock/versions/v_0/compilable/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1356 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/time_management/cpu_clock/versions/v_0/compilable/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1929 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/time_management/cpu_clock/versions/v_0/compilable/__x__build_config.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1639 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/time_management/cpu_clock/versions/v_0/cpu_clock.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.307846 cengal-3.2.0.1/cengal/time_management/cpu_clock/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/time_management/cpu_clock/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/time_management/cpu_clock/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.317846 cengal-3.2.0.1/cengal/time_management/cpu_clock_cycles/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/time_management/cpu_clock_cycles/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.327846 cengal-3.2.0.1/cengal/time_management/cpu_clock_cycles/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/time_management/cpu_clock_cycles/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.357846 cengal-3.2.0.1/cengal/time_management/cpu_clock_cycles/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/time_management/cpu_clock_cycles/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.387846 cengal-3.2.0.1/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1935 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/__build_config.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1411 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1404 2023-05-23 21:54:33.000000 cengal-3.2.0.1/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/cpu_clock_cycles.c
+-rw-r--r--   0 mb        (1000) mb        (1000)      876 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/cpu_clock_cycles.h
+-rw-r--r--   0 mb        (1000) mb        (1000)     1880 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/cpu_clock_cycles__cython.pyx
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.417846 cengal-3.2.0.1/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:10.000000 cengal-3.2.0.1/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.437846 cengal-3.2.0.1/cengal/time_management/high_precision_sync_sleep/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/high_precision_sync_sleep/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.467846 cengal-3.2.0.1/cengal/time_management/high_precision_sync_sleep/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/high_precision_sync_sleep/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.477846 cengal-3.2.0.1/cengal/time_management/high_precision_sync_sleep/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1368 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/high_precision_sync_sleep/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2727 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/high_precision_sync_sleep/versions/v_0/high_precision_sync_sleep__cython.pyx
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.497846 cengal-3.2.0.1/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.517846 cengal-3.2.0.1/cengal/time_management/load_best_timer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/load_best_timer/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.547846 cengal-3.2.0.1/cengal/time_management/load_best_timer/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/load_best_timer/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.587846 cengal-3.2.0.1/cengal/time_management/load_best_timer/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/load_best_timer/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1445 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/load_best_timer/versions/v_0/load_best_timer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.597846 cengal-3.2.0.1/cengal/time_management/relative_time/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1365 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/relative_time/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.597846 cengal-3.2.0.1/cengal/time_management/relative_time/approximate_representation/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/relative_time/approximate_representation/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.647846 cengal-3.2.0.1/cengal/time_management/relative_time/approximate_representation/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/relative_time/approximate_representation/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.667846 cengal-3.2.0.1/cengal/time_management/relative_time/approximate_representation/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/relative_time/approximate_representation/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8714 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/relative_time/approximate_representation/versions/v_0/approximate_representation.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.667846 cengal-3.2.0.1/cengal/time_management/relative_time/bysiness_relativedelta/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/relative_time/bysiness_relativedelta/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.667846 cengal-3.2.0.1/cengal/time_management/relative_time/bysiness_relativedelta/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/relative_time/bysiness_relativedelta/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.747846 cengal-3.2.0.1/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1244 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1489 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/bysiness_relativedelta.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.747846 cengal-3.2.0.1/cengal/time_management/relative_time/constants/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/relative_time/constants/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.757846 cengal-3.2.0.1/cengal/time_management/relative_time/constants/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/relative_time/constants/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.777846 cengal-3.2.0.1/cengal/time_management/relative_time/constants/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/relative_time/constants/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1418 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/relative_time/constants/versions/v_0/constants.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.837846 cengal-3.2.0.1/cengal/time_management/relative_time/relativedelta/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/relative_time/relativedelta/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.857846 cengal-3.2.0.1/cengal/time_management/relative_time/relativedelta/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/relative_time/relativedelta/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.907846 cengal-3.2.0.1/cengal/time_management/relative_time/relativedelta/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/relative_time/relativedelta/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1859 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/relative_time/relativedelta/versions/v_0/relativedelta.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.917846 cengal-3.2.0.1/cengal/time_management/relative_time/timedelta/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/relative_time/timedelta/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.947846 cengal-3.2.0.1/cengal/time_management/relative_time/timedelta/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/relative_time/timedelta/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.977846 cengal-3.2.0.1/cengal/time_management/relative_time/timedelta/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/relative_time/timedelta/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1632 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/relative_time/timedelta/versions/v_0/timedelta.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.987846 cengal-3.2.0.1/cengal/time_management/repeat_for_a_time/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/repeat_for_a_time/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:25.987846 cengal-3.2.0.1/cengal/time_management/repeat_for_a_time/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/repeat_for_a_time/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.037846 cengal-3.2.0.1/cengal/time_management/repeat_for_a_time/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1456 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/repeat_for_a_time/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    20785 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/repeat_for_a_time/versions/v_0/repeat_for_a_time__cython.pyx
+-rw-r--r--   0 mb        (1000) mb        (1000)    13453 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/repeat_for_a_time/versions/v_0/repeat_for_a_time__python.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.077846 cengal-3.2.0.1/cengal/time_management/repeat_for_a_time/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/repeat_for_a_time/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/repeat_for_a_time/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    16608 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/repeat_for_a_time/versions/v_0/tests/example_for__repeat_for_a_time.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.087846 cengal-3.2.0.1/cengal/time_management/sleep_tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/sleep_tools/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.087846 cengal-3.2.0.1/cengal/time_management/sleep_tools/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/sleep_tools/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.127846 cengal-3.2.0.1/cengal/time_management/sleep_tools/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/sleep_tools/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4700 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/sleep_tools/versions/v_0/sleep_tools.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.137846 cengal-3.2.0.1/cengal/time_management/sleep_tools/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/sleep_tools/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/sleep_tools/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.137846 cengal-3.2.0.1/cengal/time_management/timer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/timer/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.167846 cengal-3.2.0.1/cengal/time_management/timer/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/timer/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.197846 cengal-3.2.0.1/cengal/time_management/timer/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1227 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/timer/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.267846 cengal-3.2.0.1/cengal/time_management/timer/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/timer/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/timer/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4567 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/timer/versions/v_0/timer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.277846 cengal-3.2.0.1/cengal/time_management/timer/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1227 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/timer/versions/v_1/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.297846 cengal-3.2.0.1/cengal/time_management/timer/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/timer/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/timer/versions/v_1/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6791 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/timer/versions/v_1/timer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.297846 cengal-3.2.0.1/cengal/time_management/timer_precision/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/timer_precision/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.337846 cengal-3.2.0.1/cengal/time_management/timer_precision/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/timer_precision/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.347846 cengal-3.2.0.1/cengal/time_management/timer_precision/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/timer_precision/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1866 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/timer_precision/versions/v_0/test_timer_precision.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.367846 cengal-3.2.0.1/cengal/time_management/timer_precision/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/timer_precision/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4327 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/time_management/timer_precision/versions/v_1/timer_precision.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.367846 cengal-3.2.0.1/cengal/unittest/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/unittest/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.377846 cengal-3.2.0.1/cengal/unittest/behavior_stabilizer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/unittest/behavior_stabilizer/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.387846 cengal-3.2.0.1/cengal/unittest/behavior_stabilizer/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/unittest/behavior_stabilizer/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.477846 cengal-3.2.0.1/cengal/unittest/behavior_stabilizer/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1241 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/unittest/behavior_stabilizer/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2032 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/unittest/behavior_stabilizer/versions/v_0/behavior_stabilizer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.507846 cengal-3.2.0.1/cengal/unittest/behavior_stabilizer/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/unittest/behavior_stabilizer/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/unittest/behavior_stabilizer/versions/v_0/tests/_test__behavior_stabilizer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.507846 cengal-3.2.0.1/cengal/unittest/patcher/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/unittest/patcher/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.517846 cengal-3.2.0.1/cengal/unittest/patcher/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/unittest/patcher/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.527846 cengal-3.2.0.1/cengal/unittest/patcher/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/unittest/patcher/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3084 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/unittest/patcher/versions/v_0/patcher.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.557846 cengal-3.2.0.1/cengal/unittest/patcher/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/unittest/patcher/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/unittest/patcher/versions/v_0/tests/_test__patcher.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.607846 cengal-3.2.0.1/cengal/universal_parser/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/universal_parser/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/universal_parser/help_tools.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1377 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/universal_parser/idioms.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/universal_parser/parser.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8667 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/universal_parser/test.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    75709 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/universal_parser/types.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.657846 cengal-3.2.0.1/cengal/upk_helping_tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/upk_helping_tools/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2299 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/upk_helping_tools/upk_api.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1821 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/upk_helping_tools/upk_constants.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6518 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/upk_helping_tools/upk_utils_api.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.657846 cengal-3.2.0.1/cengal/user_interface/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.697846 cengal-3.2.0.1/cengal/user_interface/console/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1324 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/console/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3504 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/console/chooser.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1549 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/console/colorama_helpers.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    11360 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/console/encoding_changer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.697846 cengal-3.2.0.1/cengal/user_interface/console/progress_meter/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/console/progress_meter/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.707846 cengal-3.2.0.1/cengal/user_interface/console/progress_meter/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/console/progress_meter/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.737846 cengal-3.2.0.1/cengal/user_interface/console/progress_meter/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1364 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/console/progress_meter/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4875 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/console/progress_meter/versions/v_0/progress_meter.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1274 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/console/progress_meter/versions/v_0/progress_meter_python2.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.737846 cengal-3.2.0.1/cengal/user_interface/gui/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/gui/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.747846 cengal-3.2.0.1/cengal/user_interface/gui/nt/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/gui/nt/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.757846 cengal-3.2.0.1/cengal/user_interface/gui/nt/blur_behind/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/gui/nt/blur_behind/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.757846 cengal-3.2.0.1/cengal/user_interface/gui/nt/blur_behind/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/gui/nt/blur_behind/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.767846 cengal-3.2.0.1/cengal/user_interface/gui/nt/blur_behind/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/gui/nt/blur_behind/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3161 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/gui/nt/blur_behind/versions/v_0/blur_behind.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.787846 cengal-3.2.0.1/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.787846 cengal-3.2.0.1/cengal/user_interface/gui/nt/dpi_awareness/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/gui/nt/dpi_awareness/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.797846 cengal-3.2.0.1/cengal/user_interface/gui/nt/dpi_awareness/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/gui/nt/dpi_awareness/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.807846 cengal-3.2.0.1/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3686 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/dpi_awareness.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.817846 cengal-3.2.0.1/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.837846 cengal-3.2.0.1/cengal/user_interface/plot/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/plot/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.837846 cengal-3.2.0.1/cengal/user_interface/plot/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/plot/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.877846 cengal-3.2.0.1/cengal/user_interface/plot/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/plot/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1877 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/plot/versions/v_0/plot.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.907846 cengal-3.2.0.1/cengal/user_interface/plot/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/plot/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/user_interface/plot/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.937846 cengal-3.2.0.1/cengal/web_tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/web_tools/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.937846 cengal-3.2.0.1/cengal/web_tools/detect_browsers_host_device_type/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/web_tools/detect_browsers_host_device_type/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.947846 cengal-3.2.0.1/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.957846 cengal-3.2.0.1/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.967846 cengal-3.2.0.1/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4332 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/by_http_user_agent.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:26.977846 cengal-3.2.0.1/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1247 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1205 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    12869 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal/web_tools/help_tools.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:05.717847 cengal-3.2.0.1/cengal.egg-info/
+-rw-r--r--   0 mb        (1000) mb        (1000)    27216 2023-05-23 21:57:59.000000 cengal-3.2.0.1/cengal.egg-info/PKG-INFO
+-rw-r--r--   0 mb        (1000) mb        (1000)    86068 2023-05-23 21:58:00.000000 cengal-3.2.0.1/cengal.egg-info/SOURCES.txt
+-rw-r--r--   0 mb        (1000) mb        (1000)        1 2023-05-23 21:57:59.000000 cengal-3.2.0.1/cengal.egg-info/dependency_links.txt
+-rw-r--r--   0 mb        (1000) mb        (1000)      220 2023-05-23 21:57:59.000000 cengal-3.2.0.1/cengal.egg-info/requires.txt
+-rw-r--r--   0 mb        (1000) mb        (1000)       28 2023-05-23 21:57:59.000000 cengal-3.2.0.1/cengal.egg-info/top_level.txt
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:27.037846 cengal-3.2.0.1/cengal_setup_scripts/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1250 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal_setup_scripts/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2428 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal_setup_scripts/compile_all_cython_modules.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:27.057846 cengal-3.2.0.1/cengal_setup_scripts/find_and_prepare_cython_modules/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1253 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal_setup_scripts/find_and_prepare_cython_modules/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    14243 2023-05-23 21:54:33.000000 cengal-3.2.0.1/cengal_setup_scripts/find_and_prepare_cython_modules/find_and_prepare_cython_modules.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-23 21:58:27.097846 cengal-3.2.0.1/cengal_setup_scripts/install_required_packages/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal_setup_scripts/install_required_packages/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    10424 2023-05-23 21:54:33.000000 cengal-3.2.0.1/cengal_setup_scripts/install_required_packages/install_packages.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1783 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal_setup_scripts/install_required_packages/set_environment_variables.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1500 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal_setup_scripts/setup__dynamic_list_of_pieces.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1497 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal_setup_scripts/setup__recv_buff_size_computer.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1498 2023-05-22 07:55:11.000000 cengal-3.2.0.1/cengal_setup_scripts/setup__repeat_for_a_time.py
+-rw-r--r--   0 mb        (1000) mb        (1000)      176 2023-05-23 21:54:33.000000 cengal-3.2.0.1/pyproject.toml
+-rw-r--r--   0 mb        (1000) mb        (1000)       38 2023-05-23 21:58:27.107846 cengal-3.2.0.1/setup.cfg
+-rw-r--r--   0 mb        (1000) mb        (1000)     9048 2023-05-23 21:55:26.000000 cengal-3.2.0.1/setup.py
```

### Comparing `cengal-3.2.0/LICENSE.md` & `cengal-3.2.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/NOTICE` & `cengal-3.2.0.1/NOTICE`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/PKG-INFO` & `cengal-3.2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cengal
-Version: 3.2.0
+Version: 3.2.0.1
 Summary: General purpose library
 Home-page: https://github.com/FI-Mihej/Cengal
 Author: ButenkoMS
 Author-email: gtalk@butenkoms.space
 License: Apache License, Version 2.0
 Keywords: async loop,coroutine,async Qt,async Tkinter,bytecode manipulation,introspection,text parsing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cengal-3.2.0/README.md` & `cengal-3.2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/RequestCache.py` & `cengal-3.2.0.1/cengal/RequestCache.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ServerClock.py` & `cengal-3.2.0.1/cengal/ServerClock.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/__init__.py` & `cengal-3.2.0.1/cengal/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/base/__init__.py` & `cengal-3.2.0.1/cengal/base/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/base/classes/__init__.py` & `cengal-3.2.0.1/cengal/base/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/base/classes/versions/__init__.py` & `cengal-3.2.0.1/cengal/base/classes/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/base/classes/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/base/classes/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/base/classes/versions/v_0/classes.py` & `cengal-3.2.0.1/cengal/base/classes/versions/v_0/classes.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/base/classes/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/base/classes/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/base/classes/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/base/classes/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/base/exceptions/__init__.py` & `cengal-3.2.0.1/cengal/base/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/base/exceptions/versions/__init__.py` & `cengal-3.2.0.1/cengal/base/exceptions/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/base/exceptions/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/base/exceptions/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/base/exceptions/versions/v_0/exceptions.py` & `cengal-3.2.0.1/cengal/base/exceptions/versions/v_0/exceptions.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/base/exceptions/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/base/exceptions/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/base/exceptions/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/base/exceptions/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/build_tools/__init__.py` & `cengal-3.2.0.1/cengal/build_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/build_tools/current_compiler/__init__.py` & `cengal-3.2.0.1/cengal/build_tools/current_compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/build_tools/current_compiler/versions/__init__.py` & `cengal-3.2.0.1/cengal/build_tools/current_compiler/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/build_tools/current_compiler/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/build_tools/current_compiler/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/build_tools/current_compiler/versions/v_0/current_compiler.py` & `cengal-3.2.0.1/cengal/build_tools/current_compiler/versions/v_0/current_compiler.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/build_tools/current_compiler/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/build_tools/current_compiler/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/build_tools/current_compiler/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/build_tools/current_compiler/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/build_tools/prepare_cflags/__init__.py` & `cengal-3.2.0.1/cengal/build_tools/prepare_cflags/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/build_tools/prepare_cflags/versions/__init__.py` & `cengal-3.2.0.1/cengal/build_tools/prepare_cflags/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/build_tools/prepare_cflags/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/build_tools/prepare_cflags/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/build_tools/prepare_cflags/versions/v_0/prepare_cflags.py` & `cengal-3.2.0.1/cengal/build_tools/prepare_cflags/versions/v_0/prepare_cflags.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/build_tools/prepare_cflags/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/build_tools/prepare_cflags/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/build_tools/prepare_cflags/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/build_tools/prepare_cflags/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/bulk_pip_actions/__init__.py` & `cengal-3.2.0.1/cengal/bulk_pip_actions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/bulk_pip_actions/bulk_install.py` & `cengal-3.2.0.1/cengal/bulk_pip_actions/bulk_install.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/bulk_pip_actions/install.py` & `cengal-3.2.0.1/cengal/bulk_pip_actions/install.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/check_is_in_pycharm.py` & `cengal-3.2.0.1/cengal/check_is_in_pycharm.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/args_manager/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/args_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/args_manager/versions/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/args_manager/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/args_manager/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/args_manager/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/args_manager/versions/v_0/args_manager.py` & `cengal-3.2.0.1/cengal/code_flow_control/args_manager/versions/v_0/args_manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/args_manager/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/args_manager/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/args_manager/versions/v_0/tests/_manual_test__args_manager.py` & `cengal-3.2.0.1/cengal/code_flow_control/args_manager/versions/v_0/tests/_manual_test__args_manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/args_manager/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/code_flow_control/args_manager/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/call_history_reapplier/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/call_history_reapplier/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/call_history_reapplier/versions/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/call_history_reapplier/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/call_history_reapplier/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/call_history_reapplier/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/call_history_reapplier/versions/v_0/call_history_reapplier.py` & `cengal-3.2.0.1/cengal/code_flow_control/call_history_reapplier/versions/v_0/call_history_reapplier.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/chained_flow/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/chained_flow/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/v_0/smart_chain.py` & `cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/v_0/smart_chain.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/v_0/tests/example_for__chained_flow.py` & `cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/v_0/tests/example_for__chained_flow.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/v_1/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/v_1/chained_flow.py` & `cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/v_1/chained_flow.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/v_1/tests/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/chained_flow/versions/v_1/tests/example_for__chained_flow.py` & `cengal-3.2.0.1/cengal/code_flow_control/chained_flow/versions/v_1/tests/example_for__chained_flow.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/versions/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/versions/v_0/essence.py` & `cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/versions/v_0/essence.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/quadrangle.py` & `cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/quadrangle.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/quadrangle_test.py` & `cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/quadrangle_test.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle.py` & `cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle_test.py` & `cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle_test.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle_test_old.py` & `cengal-3.2.0.1/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle_test_old.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/none_or/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/none_or/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/none_or/versions/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/none_or/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/none_or/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/none_or/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/none_or/versions/v_0/none_or.py` & `cengal-3.2.0.1/cengal/code_flow_control/none_or/versions/v_0/none_or.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/none_or/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/none_or/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/none_or/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/code_flow_control/none_or/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/python_bytecode_manipulator/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/python_bytecode_manipulator/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/python_bytecode_manipulator/versions/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/python_bytecode_manipulator/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/python_bytecode_manipulator.py` & `cengal-3.2.0.1/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/python_bytecode_manipulator.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/smart_values/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/smart_values/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/smart_values/versions/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/smart_values/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/smart_values/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/smart_values/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/smart_values/versions/v_0/result_types.py` & `cengal-3.2.0.1/cengal/code_flow_control/smart_values/versions/v_0/result_types.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/smart_values/versions/v_1/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/smart_values/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/smart_values/versions/v_1/smart_values.py` & `cengal-3.2.0.1/cengal/code_flow_control/smart_values/versions/v_1/smart_values.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/smart_values/versions/v_2/__init__.py` & `cengal-3.2.0.1/cengal/code_flow_control/smart_values/versions/v_2/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_flow_control/smart_values/versions/v_2/smart_values.py` & `cengal-3.2.0.1/cengal/code_flow_control/smart_values/versions/v_2/smart_values.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_inspection/__init__.py` & `cengal-3.2.0.1/cengal/code_inspection/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_inspection/auto_line_tracer/__init__.py` & `cengal-3.2.0.1/cengal/code_inspection/auto_line_tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_inspection/auto_line_tracer/versions/__init__.py` & `cengal-3.2.0.1/cengal/code_inspection/auto_line_tracer/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_inspection/auto_line_tracer/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/code_inspection/auto_line_tracer/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_inspection/auto_line_tracer/versions/v_0/auto_line_tracer.py` & `cengal-3.2.0.1/cengal/code_inspection/auto_line_tracer/versions/v_0/auto_line_tracer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_inspection/line_profiling/__init__.py` & `cengal-3.2.0.1/cengal/code_inspection/line_profiling/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_inspection/line_profiling/versions/__init__.py` & `cengal-3.2.0.1/cengal/code_inspection/line_profiling/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_inspection/line_profiling/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/code_inspection/line_profiling/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_inspection/line_profiling/versions/v_0/line_profiling.py` & `cengal-3.2.0.1/cengal/code_inspection/line_profiling/versions/v_0/line_profiling.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_inspection/line_profiling/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/code_inspection/line_profiling/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_inspection/line_profiling/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/code_inspection/line_profiling/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_inspection/line_tracer/__init__.py` & `cengal-3.2.0.1/cengal/code_inspection/line_tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_inspection/line_tracer/versions/__init__.py` & `cengal-3.2.0.1/cengal/code_inspection/line_tracer/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_inspection/line_tracer/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/code_inspection/line_tracer/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_inspection/line_tracer/versions/v_0/line_tracer.py` & `cengal-3.2.0.1/cengal/code_inspection/line_tracer/versions/v_0/line_tracer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_inspection/line_tracer/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/code_inspection/line_tracer/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/code_inspection/line_tracer/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/code_inspection/line_tracer/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/cross_version/__init__.py` & `cengal-3.2.0.1/cengal/cross_version/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/cross_version/console_print/__init__.py` & `cengal-3.2.0.1/cengal/cross_version/console_print/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/cross_version/console_print/python3.py` & `cengal-3.2.0.1/cengal/cross_version/console_print/python3.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/cross_version/console_print/universal.py` & `cengal-3.2.0.1/cengal/cross_version/console_print/universal.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/constants/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/constants/versions/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/constants/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/constants/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/constants/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/constants/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/constants/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/constants/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/ctypes_tools/constants/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/constants/versions/v_0/win_constants.py` & `cengal-3.2.0.1/cengal/ctypes_tools/constants/versions/v_0/win_constants.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/function_prototypes/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/function_prototypes/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/function_prototypes/versions/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/function_prototypes/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/function_prototypes/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/function_prototypes/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/function_prototypes/versions/v_0/win_function_prototypes.py` & `cengal-3.2.0.1/cengal/ctypes_tools/function_prototypes/versions/v_0/win_function_prototypes.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/functions/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/functions/versions/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/functions/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/functions/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/functions/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/functions/versions/v_0/functions.py` & `cengal-3.2.0.1/cengal/ctypes_tools/functions/versions/v_0/functions.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/functions/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/functions/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/functions/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/ctypes_tools/functions/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/functions/versions/v_0/win_functions.py` & `cengal-3.2.0.1/cengal/ctypes_tools/functions/versions/v_0/win_functions.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/libraries/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/libraries/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/libraries/versions/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/libraries/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/libraries/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/libraries/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/libraries/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/libraries/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/libraries/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/ctypes_tools/libraries/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/libraries/versions/v_0/win_libraries.py` & `cengal-3.2.0.1/cengal/ctypes_tools/libraries/versions/v_0/win_libraries.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/result_api/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/result_api/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/result_api/versions/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/result_api/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/result_api/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/result_api/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/result_api/versions/v_0/result_api.py` & `cengal-3.2.0.1/cengal/ctypes_tools/result_api/versions/v_0/result_api.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/result_api/versions/v_0/result_api_exceptions.py` & `cengal-3.2.0.1/cengal/ctypes_tools/result_api/versions/v_0/result_api_exceptions.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/result_api/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/result_api/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/result_api/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/ctypes_tools/result_api/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/result_api/versions/v_0/win_result_api.py` & `cengal-3.2.0.1/cengal/ctypes_tools/result_api/versions/v_0/win_result_api.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/tools/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/tools/versions/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/tools/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/tools/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/tools/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/tools/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/tools/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/tools/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/ctypes_tools/tools/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/tools/versions/v_0/tools.py` & `cengal-3.2.0.1/cengal/ctypes_tools/tools/versions/v_0/tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/tools/versions/v_0/win_tools.py` & `cengal-3.2.0.1/cengal/ctypes_tools/tools/versions/v_0/win_tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/types/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/types/versions/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/types/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/types/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/types/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/types/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/ctypes_tools/types/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/types/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/ctypes_tools/types/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/ctypes_tools/types/versions/v_0/win_types.py` & `cengal-3.2.0.1/cengal/ctypes_tools/types/versions/v_0/win_types.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/cython_tools/__init__.py` & `cengal-3.2.0.1/cengal/cython_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/cython_tools/cythonyser_setup_runner.py` & `cengal-3.2.0.1/cengal/cython_tools/cythonyser_setup_runner.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/compound_dict_management/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/compound_dict_management/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/versions/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/versions/v_0/manager.py` & `cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/versions/v_0/manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/versions/v_1/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/versions/v_1/manager.py` & `cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/versions/v_1/manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/key__hashable__to__value__set.py` & `cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/key__hashable__to__value__set.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key_counter/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key_counter/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/key_counter.py` & `cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/key_counter.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/dynamic_list_of_pieces__cython.pyx` & `cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/dynamic_list_of_pieces__cython.pyx`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/dynamic_list_of_pieces__python.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/dynamic_list_of_pieces__python.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/dynamic_list_of_pieces__cython.pyx` & `cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/dynamic_list_of_pieces__cython.pyx`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/dynamic_list_of_pieces__python.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/dynamic_list_of_pieces__python.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_0/TagDB.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_0/TagDB.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_0/tag_db_interface.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_0/tag_db_interface.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_1/TagDB.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_1/TagDB.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_1/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_1/tag_db_interface.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_1/tag_db_interface.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_2/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_2/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_2/dynamic_tag_tree.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_2/dynamic_tag_tree.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/fast_fifo/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/fast_fifo/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/fast_fifo/versions/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/fast_fifo/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/fast_fifo/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/fast_fifo/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/fast_fifo/versions/v_0/fast_fifo.py` & `cengal-3.2.0.1/cengal/data_containers/fast_fifo/versions/v_0/fast_fifo.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/fast_fifo/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/fast_fifo/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/fast_fifo/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_containers/fast_fifo/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/fast_fifo/versions/v_1/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/fast_fifo/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/fast_fifo/versions/v_1/fast_fifo.py` & `cengal-3.2.0.1/cengal/data_containers/fast_fifo/versions/v_1/fast_fifo.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/fast_fifo/versions/v_1/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/fast_fifo/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/fast_fifo/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_containers/fast_fifo/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/versions/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/versions/v_0/limitable_dict_with_order.py` & `cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/versions/v_0/limitable_dict_with_order.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/versions/v_1/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/versions/v_1/limitable_dict_with_order.py` & `cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/versions/v_1/limitable_dict_with_order.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/simple_tree/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/simple_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/simple_tree/versions/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/simple_tree/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/simple_tree/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/simple_tree/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/simple_tree/versions/v_0/simple_tree.py` & `cengal-3.2.0.1/cengal/data_containers/simple_tree/versions/v_0/simple_tree.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/stack/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/stack/versions/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/stack/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/stack/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/stack/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/stack/versions/v_0/stack.py` & `cengal-3.2.0.1/cengal/data_containers/stack/versions/v_0/stack.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/stack/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_containers/stack/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_containers/stack/versions/v_0/tests/test__stack.py` & `cengal-3.2.0.1/cengal/data_containers/stack/versions/v_0/tests/test__stack.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_generation/__init__.py` & `cengal-3.2.0.1/cengal/data_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_generation/id_generator/__init__.py` & `cengal-3.2.0.1/cengal/data_generation/id_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_generation/id_generator/versions/__init__.py` & `cengal-3.2.0.1/cengal/data_generation/id_generator/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_generation/id_generator/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/data_generation/id_generator/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_generation/id_generator/versions/v_0/id_generator.py` & `cengal-3.2.0.1/cengal/data_generation/id_generator/versions/v_0/id_generator.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_generation/id_generator/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_generation/id_generator/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_generation/id_generator/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_generation/id_generator/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_generation/id_generator/versions/v_1/__init__.py` & `cengal-3.2.0.1/cengal/data_generation/id_generator/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_generation/id_generator/versions/v_1/id_generator.py` & `cengal-3.2.0.1/cengal/data_generation/id_generator/versions/v_1/id_generator.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_generation/id_generator/versions/v_1/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_generation/id_generator/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_generation/id_generator/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_generation/id_generator/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/bit_cast_like/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/bit_cast_like/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/bit_cast_like/versions/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/bit_cast_like/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/bit_cast_like.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/bit_cast_like.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast/versions/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/reinterpret_cast.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/reinterpret_cast.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/manager.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/copy_wrapper.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/copy_wrapper.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/deep_copy_wrapper.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/deep_copy_wrapper.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/uni_copy_wrapper.py` & `cengal-3.2.0.1/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/uni_copy_wrapper.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/front_triggerable_variable/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/front_triggerable_variable/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/front_triggerable_variable/versions/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/front_triggerable_variable/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/front_triggerable_variable/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/front_triggerable_variable/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/front_triggerable_variable/versions/v_0/front_triggerable_variable.py` & `cengal-3.2.0.1/cengal/data_manipulation/front_triggerable_variable/versions/v_0/front_triggerable_variable.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/get_dict_key_with_callable_default/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/get_dict_key_with_callable_default/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/get_dict_key_with_callable_default/versions/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/get_dict_key_with_callable_default/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/get_dict_key_with_callable_default.py` & `cengal-3.2.0.1/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/get_dict_key_with_callable_default.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/help_tools.py` & `cengal-3.2.0.1/cengal/data_manipulation/help_tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/objects_counter/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/objects_counter/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/objects_counter/versions/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/objects_counter/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/objects_counter/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/objects_counter/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/objects_counter/versions/v_0/objects_counter.py` & `cengal-3.2.0.1/cengal/data_manipulation/objects_counter/versions/v_0/objects_counter.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/objects_counter/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/objects_counter/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/objects_counter/versions/v_0/tests/test__objects_counter.py` & `cengal-3.2.0.1/cengal/data_manipulation/objects_counter/versions/v_0/tests/test__objects_counter.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/performant_list_operations/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/performant_list_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/performant_list_operations/versions/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/performant_list_operations/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/performant_list_operations/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/performant_list_operations/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/performant_list_operations/versions/v_0/remove_items_from_list.py` & `cengal-3.2.0.1/cengal/data_manipulation/performant_list_operations/versions/v_0/remove_items_from_list.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/serialization/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/serialization/versions/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/serialization/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/serialization/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/serialization/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/serialization/versions/v_0/serialization.py` & `cengal-3.2.0.1/cengal/data_manipulation/serialization/versions/v_0/serialization.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/serialization/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/serialization/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/serialization/versions/v_0/tests/test__serialization.py` & `cengal-3.2.0.1/cengal/data_manipulation/serialization/versions/v_0/tests/test__serialization.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/tree_traversal/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_0/tests/traverstal_manual_tests.py` & `cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_0/tests/traverstal_manual_tests.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_0/tree_traversal.py` & `cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_0/tree_traversal.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_1/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_1/tests/__init__.py` & `cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_1/tests/key_multi_value_traverstal_manual_tests.py` & `cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_1/tests/key_multi_value_traverstal_manual_tests.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_1/tests/key_value_traverstal_manual_tests.py` & `cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_1/tests/key_value_traverstal_manual_tests.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_1/tests/traverstal_manual_tests.py` & `cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_1/tests/traverstal_manual_tests.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/data_manipulation/tree_traversal/versions/v_1/tree_traversal.py` & `cengal-3.2.0.1/cengal/data_manipulation/tree_traversal/versions/v_1/tree_traversal.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/docten.py` & `cengal-3.2.0.1/cengal/docten.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/entities/__init__.py` & `cengal-3.2.0.1/cengal/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/entities/bindable_to_type/__init__.py` & `cengal-3.2.0.1/cengal/entities/bindable_to_type/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/entities/bindable_to_type/versions/__init__.py` & `cengal-3.2.0.1/cengal/entities/bindable_to_type/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/entities/bindable_to_type/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/entities/bindable_to_type/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/entities/bindable_to_type/versions/v_0/bindable_to_type.py` & `cengal-3.2.0.1/cengal/entities/bindable_to_type/versions/v_0/bindable_to_type.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/entities/bindable_to_type/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/entities/bindable_to_type/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/entities/bindable_to_type/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/entities/bindable_to_type/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/entities/copyable/__init__.py` & `cengal-3.2.0.1/cengal/entities/copyable/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/entities/copyable/versions/__init__.py` & `cengal-3.2.0.1/cengal/entities/copyable/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/entities/copyable/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/entities/copyable/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/entities/copyable/versions/v_0/copyable.py` & `cengal-3.2.0.1/cengal/entities/copyable/versions/v_0/copyable.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/entities/copyable/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/entities/copyable/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/entities/copyable/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/entities/copyable/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_settings_manager/__init__.py` & `cengal-3.2.0.1/cengal/file_settings_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_settings_manager/config_manager.py` & `cengal-3.2.0.1/cengal/file_settings_manager/config_manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_settings_manager/dir_templates.py` & `cengal-3.2.0.1/cengal/file_settings_manager/dir_templates.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/__init__.py` & `cengal-3.2.0.1/cengal/file_system/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/app_fs_structure/__init__.py` & `cengal-3.2.0.1/cengal/file_system/app_fs_structure/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/__init__.py` & `cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/versions/__init__.py` & `cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_exceptions.py` & `cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_exceptions.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_base.py` & `cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_base.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_darwin.py` & `cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_darwin.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_linux.py` & `cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_linux.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_win.py` & `cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_win.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_directory_types.py` & `cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_directory_types.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/directory_manager.py` & `cengal-3.2.0.1/cengal/file_system/directory_manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/file_manager.py` & `cengal-3.2.0.1/cengal/file_system/file_manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/file_patch/__init__.py` & `cengal-3.2.0.1/cengal/file_system/file_patch/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/file_patch/brackets/__init__.py` & `cengal-3.2.0.1/cengal/file_system/file_patch/brackets/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/file_patch/brackets/versions/__init__.py` & `cengal-3.2.0.1/cengal/file_system/file_patch/brackets/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/file_patch/brackets/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/file_system/file_patch/brackets/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/file_patch/brackets/versions/v_0/brackets.py` & `cengal-3.2.0.1/cengal/file_system/file_patch/brackets/versions/v_0/brackets.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/file_patch/brackets/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/file_system/file_patch/brackets/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/file_patch/brackets/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/file_system/file_patch/brackets/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/file_patch/generic/__init__.py` & `cengal-3.2.0.1/cengal/file_system/file_patch/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/file_patch/generic/versions/__init__.py` & `cengal-3.2.0.1/cengal/file_system/file_patch/generic/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/file_patch/generic/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/file_system/file_patch/generic/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/file_patch/generic/versions/v_0/generic.py` & `cengal-3.2.0.1/cengal/file_system/file_patch/generic/versions/v_0/generic.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/file_patch/generic/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/file_system/file_patch/generic/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/file_patch/generic/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/file_system/file_patch/generic/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/file_patch/simple/__init__.py` & `cengal-3.2.0.1/cengal/file_system/file_patch/simple/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/file_patch/simple/versions/__init__.py` & `cengal-3.2.0.1/cengal/file_system/file_patch/simple/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/file_patch/simple/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/file_system/file_patch/simple/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/file_patch/simple/versions/v_0/simple.py` & `cengal-3.2.0.1/cengal/file_system/file_patch/simple/versions/v_0/simple.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/file_patch/simple/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/file_system/file_patch/simple/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/file_patch/simple/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/file_system/file_patch/simple/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/path_manager/__init__.py` & `cengal-3.2.0.1/cengal/file_system/path_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/path_manager/versions/__init__.py` & `cengal-3.2.0.1/cengal/file_system/path_manager/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/path_manager/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/file_system/path_manager/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/path_manager/versions/v_0/path_manager.py` & `cengal-3.2.0.1/cengal/file_system/path_manager/versions/v_0/path_manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/path_manager/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/file_system/path_manager/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/path_manager/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/file_system/path_manager/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/win_fs/__init__.py` & `cengal-3.2.0.1/cengal/file_system/win_fs/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/win_fs/base.py` & `cengal-3.2.0.1/cengal/file_system/win_fs/base.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/win_fs/global_install_uninstall.py` & `cengal-3.2.0.1/cengal/file_system/win_fs/global_install_uninstall.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/win_fs/path.py` & `cengal-3.2.0.1/cengal/file_system/win_fs/path.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/win_fs/shutil.py` & `cengal-3.2.0.1/cengal/file_system/win_fs/shutil.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/file_system/win_fs/shutil_readable.py` & `cengal-3.2.0.1/cengal/file_system/win_fs/shutil_readable.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/__init__.py` & `cengal-3.2.0.1/cengal/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/info/__init__.py` & `cengal-3.2.0.1/cengal/hardware/info/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/info/cpu/__init__.py` & `cengal-3.2.0.1/cengal/hardware/info/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/info/cpu/versions/__init__.py` & `cengal-3.2.0.1/cengal/hardware/info/cpu/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/info/cpu/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/hardware/info/cpu/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/info/cpu/versions/v_0/cpu.py` & `cengal-3.2.0.1/cengal/hardware/info/cpu/versions/v_0/cpu.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/info/cpu/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/hardware/info/cpu/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/info/cpu/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/hardware/info/cpu/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/info/cpu/versions/v_1/__init__.py` & `cengal-3.2.0.1/cengal/hardware/info/cpu/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/info/cpu/versions/v_1/cpu.py` & `cengal-3.2.0.1/cengal/hardware/info/cpu/versions/v_1/cpu.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/info/cpu/versions/v_1/tests/__init__.py` & `cengal-3.2.0.1/cengal/hardware/info/cpu/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/info/cpu/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/hardware/info/cpu/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/memory/__init__.py` & `cengal-3.2.0.1/cengal/hardware/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/memory/barriers/__init__.py` & `cengal-3.2.0.1/cengal/hardware/memory/barriers/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/memory/barriers/versions/__init__.py` & `cengal-3.2.0.1/cengal/hardware/memory/barriers/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/memory/barriers/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/hardware/memory/barriers/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/memory/barriers/versions/v_0/compilable/__build_config.py` & `cengal-3.2.0.1/cengal/hardware/memory/barriers/versions/v_0/compilable/__build_config.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/memory/barriers/versions/v_0/compilable/__init__.py` & `cengal-3.2.0.1/cengal/hardware/memory/barriers/versions/v_0/compilable/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/memory/barriers/versions/v_0/compilable/barriers__cython.pyx` & `cengal-3.2.0.1/cengal/hardware/memory/barriers/versions/v_0/compilable/barriers__cython.pyx`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/memory/barriers/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/hardware/memory/barriers/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/memory/barriers/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/hardware/memory/barriers/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/memory/shared_memory/__init__.py` & `cengal-3.2.0.1/cengal/hardware/memory/shared_memory/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/__init__.py` & `cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/v_0/compilable/__build_config.py` & `cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/v_0/compilable/__build_config.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/v_0/compilable/__init__.py` & `cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/v_0/compilable/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/v_0/compilable/memory_access.c` & `cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/v_0/compilable/memory_access.c`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/v_0/compilable/memory_access.h` & `cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/v_0/compilable/memory_access.h`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/v_0/compilable/memory_access__cython.pyx` & `cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/v_0/compilable/memory_access__cython.pyx`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/v_0/interfaces.py` & `cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/v_0/interfaces.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/v_0/shared_memory.py` & `cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/v_0/shared_memory.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/hardware/memory/shared_memory/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/hardware/memory/shared_memory/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/help_tools.py` & `cengal-3.2.0.1/cengal/help_tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/introspection/__init__.py` & `cengal-3.2.0.1/cengal/introspection/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/introspection/inspect/__init__.py` & `cengal-3.2.0.1/cengal/introspection/inspect/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/introspection/inspect/versions/__init__.py` & `cengal-3.2.0.1/cengal/introspection/inspect/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/introspection/inspect/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/introspection/inspect/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/introspection/inspect/versions/v_0/inspect.py` & `cengal-3.2.0.1/cengal/introspection/inspect/versions/v_0/inspect.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/introspection/inspect/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/introspection/inspect/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/introspection/inspect/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/introspection/inspect/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/introspection/third_party/__init__.py` & `cengal-3.2.0.1/cengal/introspection/third_party/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/introspection/third_party/ctypes/__init__.py` & `cengal-3.2.0.1/cengal/introspection/third_party/ctypes/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/introspection/third_party/ctypes/versions/__init__.py` & `cengal-3.2.0.1/cengal/introspection/third_party/ctypes/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/introspection/third_party/ctypes/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/introspection/third_party/ctypes/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/introspection/third_party/ctypes/versions/v_0/ctypes.py` & `cengal-3.2.0.1/cengal/introspection/third_party/ctypes/versions/v_0/ctypes.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/introspection/third_party/ctypes/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/introspection/third_party/ctypes/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/introspection/third_party/ctypes/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/introspection/third_party/ctypes/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/__init__.py` & `cengal-3.2.0.1/cengal/io/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/asock_io/__init__.py` & `cengal-3.2.0.1/cengal/io/asock_io/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/asock_io/versions/__init__.py` & `cengal-3.2.0.1/cengal/io/asock_io/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/asock_io/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/io/asock_io/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/asock_io/versions/v_0/base.py` & `cengal-3.2.0.1/cengal/io/asock_io/versions/v_0/base.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/__init__.py` & `cengal-3.2.0.1/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/recv_buff_size_computer__cython.pyx` & `cengal-3.2.0.1/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/recv_buff_size_computer__cython.pyx`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/recv_buff_size_computer__python.py` & `cengal-3.2.0.1/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/recv_buff_size_computer__python.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/asock_io/versions/v_0/tcp_app_server.py` & `cengal-3.2.0.1/cengal/io/asock_io/versions/v_0/tcp_app_server.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/asock_io/versions/v_0/tcp_link.py` & `cengal-3.2.0.1/cengal/io/asock_io/versions/v_0/tcp_link.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/asock_io/versions/v_1/__init__.py` & `cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/asock_io/versions/v_1/abstract.py` & `cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/abstract.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/asock_io/versions/v_1/asock_io_core.py` & `cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/asock_io_core.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/asock_io/versions/v_1/base.py` & `cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/base.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/asock_io/versions/v_1/io_loops/__init__.py` & `cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/io_loops/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/asock_io/versions/v_1/io_loops/epoll_lt.py` & `cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/io_loops/epoll_lt.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/asock_io/versions/v_1/io_loops/select.py` & `cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/io_loops/select.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/__init__.py` & `cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/recv_buff_size_computer__cython.pyx` & `cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/recv_buff_size_computer__cython.pyx`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/recv_buff_size_computer__python.py` & `cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/recv_buff_size_computer__python.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/asock_io/versions/v_1/tcp_link.py` & `cengal-3.2.0.1/cengal/io/asock_io/versions/v_1/tcp_link.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/core/__init__.py` & `cengal-3.2.0.1/cengal/io/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/core/memory_management/__init__.py` & `cengal-3.2.0.1/cengal/io/core/memory_management/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/core/memory_management/versions/__init__.py` & `cengal-3.2.0.1/cengal/io/core/memory_management/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/core/memory_management/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/io/core/memory_management/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/core/memory_management/versions/v_0/memory_management.py` & `cengal-3.2.0.1/cengal/io/core/memory_management/versions/v_0/memory_management.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/core/memory_management/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/io/core/memory_management/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/core/memory_management/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/io/core/memory_management/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/named_connections/__init__.py` & `cengal-3.2.0.1/cengal/io/named_connections/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/named_connections/named_connections_manager/__init__.py` & `cengal-3.2.0.1/cengal/io/named_connections/named_connections_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/named_connections/named_connections_manager/versions/__init__.py` & `cengal-3.2.0.1/cengal/io/named_connections/named_connections_manager/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/named_connections/named_connections_manager/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/io/named_connections/named_connections_manager/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/named_connections/named_connections_manager/versions/v_0/named_connections_manager.py` & `cengal-3.2.0.1/cengal/io/named_connections/named_connections_manager/versions/v_0/named_connections_manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/named_connections/workers/__init__.py` & `cengal-3.2.0.1/cengal/io/named_connections/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams/__init__.py` & `cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams/versions/__init__.py` & `cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/asyncio_streams.py` & `cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/asyncio_streams.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams_proxy/__init__.py` & `cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams_proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/__init__.py` & `cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/asyncio_streams_proxy.py` & `cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/asyncio_streams_proxy.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/net_io/__init__.py` & `cengal-3.2.0.1/cengal/io/net_io/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/net_io/versions/__init__.py` & `cengal-3.2.0.1/cengal/io/net_io/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/net_io/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/io/net_io/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/net_io/versions/v_0/crossplatform/__init__.py` & `cengal-3.2.0.1/cengal/io/net_io/versions/v_0/crossplatform/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/__init__.py` & `cengal-3.2.0.1/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/abstract.py` & `cengal-3.2.0.1/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/abstract.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/linux.py` & `cengal-3.2.0.1/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/linux.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/win32.py` & `cengal-3.2.0.1/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/win32.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/net_io/versions/v_0/net_io__linux.py` & `cengal-3.2.0.1/cengal/io/net_io/versions/v_0/net_io__linux.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/net_io/versions/v_0/net_io_abstract.py` & `cengal-3.2.0.1/cengal/io/net_io/versions/v_0/net_io_abstract.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/net_io/versions/v_0/net_io_method__epoll_lt.py` & `cengal-3.2.0.1/cengal/io/net_io/versions/v_0/net_io_method__epoll_lt.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/net_io/versions/v_0/net_io_method__select.py` & `cengal-3.2.0.1/cengal/io/net_io/versions/v_0/net_io_method__select.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/recv_buff_size_computer/__init__.py` & `cengal-3.2.0.1/cengal/io/recv_buff_size_computer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/__init__.py` & `cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/v_0/recv_buff_size_computer__cython.pyx` & `cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/v_0/recv_buff_size_computer__cython.pyx`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/v_0/recv_buff_size_computer__python.py` & `cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/v_0/recv_buff_size_computer__python.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/v_1/__init__.py` & `cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/v_1/recv_buff_size_computer__cython.pyx` & `cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/v_1/recv_buff_size_computer__cython.pyx`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/v_1/recv_buff_size_computer__python.py` & `cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/v_1/recv_buff_size_computer__python.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/v_1/tests/__init__.py` & `cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/recv_buff_size_computer/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/io/recv_buff_size_computer/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/serve_free_ports/__init__.py` & `cengal-3.2.0.1/cengal/io/serve_free_ports/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/serve_free_ports/versions/__init__.py` & `cengal-3.2.0.1/cengal/io/serve_free_ports/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/serve_free_ports/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/io/serve_free_ports/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/serve_free_ports/versions/v_0/serve_free_ports.py` & `cengal-3.2.0.1/cengal/io/serve_free_ports/versions/v_0/serve_free_ports.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/serve_free_ports/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/io/serve_free_ports/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/serve_free_ports/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/io/serve_free_ports/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/socket/__init__.py` & `cengal-3.2.0.1/cengal/io/socket/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/socket/constants/__init__.py` & `cengal-3.2.0.1/cengal/io/socket/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/socket/constants/versions/__init__.py` & `cengal-3.2.0.1/cengal/io/socket/constants/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/socket/constants/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/io/socket/constants/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/socket/constants/versions/v_0/constants.py` & `cengal-3.2.0.1/cengal/io/socket/constants/versions/v_0/constants.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/socket/constants/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/io/socket/constants/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/socket/constants/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/io/socket/constants/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/socket/errors/__init__.py` & `cengal-3.2.0.1/cengal/io/socket/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/socket/errors/versions/__init__.py` & `cengal-3.2.0.1/cengal/io/socket/errors/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/socket/errors/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/io/socket/errors/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/socket/errors/versions/v_0/errors.py` & `cengal-3.2.0.1/cengal/io/socket/errors/versions/v_0/errors.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/socket/errors/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/io/socket/errors/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/socket/errors/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/io/socket/errors/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/used_ports/__init__.py` & `cengal-3.2.0.1/cengal/io/used_ports/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/used_ports/versions/__init__.py` & `cengal-3.2.0.1/cengal/io/used_ports/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/used_ports/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/io/used_ports/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/used_ports/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/io/used_ports/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/used_ports/versions/v_0/tests/_test__used_ports.py` & `cengal-3.2.0.1/cengal/io/used_ports/versions/v_0/tests/_test__used_ports.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/io/used_ports/versions/v_0/used_ports.py` & `cengal-3.2.0.1/cengal/io/used_ports/versions/v_0/used_ports.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/__init__.py` & `cengal-3.2.0.1/cengal/math/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/algebra/__init__.py` & `cengal-3.2.0.1/cengal/math/algebra/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/algebra/fast_algorithms/__init__.py` & `cengal-3.2.0.1/cengal/math/algebra/fast_algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/algebra/fast_algorithms/versions/__init__.py` & `cengal-3.2.0.1/cengal/math/algebra/fast_algorithms/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/algebra/fast_algorithms/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/math/algebra/fast_algorithms/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/algebra/fast_algorithms/versions/v_0/fast_algorithms.py` & `cengal-3.2.0.1/cengal/math/algebra/fast_algorithms/versions/v_0/fast_algorithms.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/algebra/fast_algorithms/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/math/algebra/fast_algorithms/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/algebra/fast_algorithms/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/math/algebra/fast_algorithms/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/geometry/__init__.py` & `cengal-3.2.0.1/cengal/math/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/geometry/ellipse/__init__.py` & `cengal-3.2.0.1/cengal/math/geometry/ellipse/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/geometry/ellipse/versions/__init__.py` & `cengal-3.2.0.1/cengal/math/geometry/ellipse/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/geometry/ellipse/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/math/geometry/ellipse/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/geometry/ellipse/versions/v_0/ellipse.py` & `cengal-3.2.0.1/cengal/math/geometry/ellipse/versions/v_0/ellipse.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/geometry/ellipse/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/math/geometry/ellipse/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/geometry/ellipse/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/math/geometry/ellipse/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/geometry/ellipse/versions/v_0/tests/informal_tests.py` & `cengal-3.2.0.1/cengal/math/geometry/ellipse/versions/v_0/tests/informal_tests.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/geometry/point/__init__.py` & `cengal-3.2.0.1/cengal/math/geometry/point/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/geometry/point/versions/__init__.py` & `cengal-3.2.0.1/cengal/math/geometry/point/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/geometry/point/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/math/geometry/point/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/geometry/point/versions/v_0/point.py` & `cengal-3.2.0.1/cengal/math/geometry/point/versions/v_0/point.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/geometry/point/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/math/geometry/point/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/geometry/point/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/math/geometry/point/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/geometry/vector/__init__.py` & `cengal-3.2.0.1/cengal/math/geometry/vector/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/geometry/vector/versions/__init__.py` & `cengal-3.2.0.1/cengal/math/geometry/vector/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/geometry/vector/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/math/geometry/vector/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/geometry/vector/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/math/geometry/vector/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/geometry/vector/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/math/geometry/vector/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/geometry/vector/versions/v_0/vector.py` & `cengal-3.2.0.1/cengal/math/geometry/vector/versions/v_0/vector.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/numbers/__init__.py` & `cengal-3.2.0.1/cengal/math/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/numbers/versions/__init__.py` & `cengal-3.2.0.1/cengal/math/numbers/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/numbers/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/math/numbers/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/numbers/versions/v_0/numbers.py` & `cengal-3.2.0.1/cengal/math/numbers/versions/v_0/numbers.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/numbers/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/math/numbers/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/math/numbers/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/math/numbers/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/modules_management/__init__.py` & `cengal-3.2.0.1/cengal/modules_management/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/modules_management/alternative_import.py` & `cengal-3.2.0.1/cengal/modules_management/alternative_import.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/modules_management/ignore_in_build_mode/__init__.py` & `cengal-3.2.0.1/cengal/modules_management/ignore_in_build_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/modules_management/ignore_in_build_mode/versions/__init__.py` & `cengal-3.2.0.1/cengal/modules_management/ignore_in_build_mode/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/modules_management/ignore_in_build_mode/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/modules_management/ignore_in_build_mode/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/modules_management/ignore_in_build_mode/versions/v_0/ignore_in_build_mode.py` & `cengal-3.2.0.1/cengal/modules_management/ignore_in_build_mode/versions/v_0/ignore_in_build_mode.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/modules_management/reload_module.py` & `cengal-3.2.0.1/cengal/modules_management/reload_module.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/os/__init__.py` & `cengal-3.2.0.1/cengal/os/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/os/help_tools.py` & `cengal-3.2.0.1/cengal/os/help_tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/atasks/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/atasks/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/atasks/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/atasks/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/atasks/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/atasks/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/atasks/versions/v_0/atasks.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/atasks/versions/v_0/atasks.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_abstract.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_abstract.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_base.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_base.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_base_internal.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_base_internal.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tcp_efficient_streams.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tcp_efficient_streams.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/asyncio_streams_client.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/asyncio_streams_client.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/asyncio_streams_server.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/asyncio_streams_server.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/udp_efficient_streams.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/udp_efficient_streams.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/init_loop/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/init_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/init_loop/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/init_loop/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/init_loop/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/init_loop/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/init_loop/versions/v_0/init_loop.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/init_loop/versions/v_0/init_loop.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/run_in_process_pool/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_in_process_pool/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/run_in_process_pool/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_in_process_pool/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/run_in_process_pool.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/run_in_process_pool.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/run_loop/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/run_loop/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_loop/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/run_loop/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_loop/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/run_loop/versions/v_0/run_loop.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_loop/versions/v_0/run_loop.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/timed_yield/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/timed_yield/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/timed_yield/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/timed_yield/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/timed_yield.py` & `cengal-3.2.0.1/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/timed_yield.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/__init__.py` & `cengal-3.2.0.1/cengal/time_management/cpu_clock/versions/v_0/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 # 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .coro_scheduler import *
-from .coro_standard_services import *
-from .coro_tools import *
+from .cpu_clock import *
 
 """
 Module Docstring
 Docstrings: http://www.python.org/dev/peps/pep-0257/
 """
 
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
```

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_scheduler/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_scheduler/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_scheduler/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/coro_scheduler.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/coro_scheduler.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/__init__.py` & `cengal-3.2.0.1/cengal/time_management/cpu_clock/versions/v_0/cpu_clock.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,23 +11,17 @@
 # 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .put_coro import *
-from .run_coro import *
-from .sleep import *
-from .simple_yield import *
-from .loop_yield import *
-from .timer_func_runner import *
-from .timer_coro_runner import *
-from .communication import *
-from .some_printer import *
+
+__all__ = ['cpu_clock', 'CPU_TICKS_PER_SECOND']
+
 
 """
 Module Docstring
 Docstrings: http://www.python.org/dev/peps/pep-0257/
 """
 
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
@@ -36,7 +30,21 @@
 __license__ = "Apache License, Version 2.0"
 __version__ = "3.2.0"
 __maintainer__ = "ButenkoMS <gtalk@butenkoms.space>"
 __email__ = "gtalk@butenkoms.space"
 # __status__ = "Prototype"
 __status__ = "Development"
 # __status__ = "Production"
+
+
+from cengal.time_management.cpu_clock_cycles import cpu_clock_cycles, set_cycles_per_second, cpu_clock
+from cengal.hardware.info.cpu import cpu_info
+from cengal.time_management.load_best_timer import perf_counter
+
+
+CPU_TICKS_PER_SECOND = cpu_info().hz_advertised[0]
+
+
+if 0 == CPU_TICKS_PER_SECOND:
+    cpu_clock = perf_counter
+else:
+    set_cycles_per_second(CPU_TICKS_PER_SECOND)
```

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/async_event_bus.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/async_event_bus.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/asyncio_loop.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/asyncio_loop.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/communication/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/communication.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/communication.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/cpu_tick_count_per_second.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/cpu_tick_count_per_second.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/db/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/db/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/db.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/db.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/event_bus.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/event_bus.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/fast_aggregator.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/fast_aggregator.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/instance/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/instance.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/instance.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/kill_coro.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/kill_coro.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/kill_coro_list.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/kill_coro_list.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/lazy_print.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/lazy_print.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/lmdb.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/lmdb.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/log/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/log/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/log.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/log.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/bytecode_patcher.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/bytecode_patcher.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/loop_yield.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/loop_yield.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/put_coro.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/put_coro.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/put_coro_list.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/put_coro_list.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/read_write_locker.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/read_write_locker.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/class_info.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/class_info.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/commands.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/commands.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/exceptions.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/exceptions.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/remote_node.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/remote_node.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/remote_nodes.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/remote_nodes.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/request_class_info.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/request_class_info.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/serializers.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/serializers.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/run_coro.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/run_coro.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/shutdown_loop.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/shutdown_loop.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/shutdown_on_keyboard_interrupt.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/shutdown_on_keyboard_interrupt.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/simple_yield.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/simple_yield.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/sleep/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/sleep/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/sleep.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/sleep.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/some_printer.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/some_printer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/throw_coro.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/throw_coro.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/throw_coro_list.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/throw_coro_list.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/timer_coro_runner.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/timer_coro_runner.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/timer_func_runner.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/timer_func_runner.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tkinter.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tkinter.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/wait_coro.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/wait_coro.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/general.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/general.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/service_with_a_direct_request.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/service_with_a_direct_request.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/await_coro/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/await_coro/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .await_coro import *
+from .wait_coro import *
 
 """
 Module Docstring
 Docstrings: http://www.python.org/dev/peps/pep-0257/
 """
 
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
```

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/await_coro.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/await_coro.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/coro_flow_control.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/coro_flow_control.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/low_latency/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/low_latency/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/ajson.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/ajson.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/json.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/json.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/prepare_loop.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/prepare_loop.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/run_in_loop.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/run_in_loop.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/wait_coro/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/wait_coro/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/text_patch/brackets/versions/v_0/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .wait_coro import *
+from .brackets import *
 
 """
 Module Docstring
 Docstrings: http://www.python.org/dev/peps/pep-0257/
 """
 
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
```

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/wait_coro.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/wait_coro.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/customtkinter/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/customtkinter/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/customtkinter.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/customtkinter.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/nicegui/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/nicegui/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/nicegui/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/nicegui/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/nicegui.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/nicegui.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/pytermgui/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/pytermgui/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/pytermgui.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/pytermgui.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/qt/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/qt/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/qt/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/qt.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/qt.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvicorn/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvicorn/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/uvicorn.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/uvicorn.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvloop/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvloop/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvloop/versions/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvloop/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/uvloop.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/uvloop.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/green_threads_tools/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/green_threads_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/green_threads_tools/task_management.py` & `cengal-3.2.0.1/cengal/parallel_execution/green_threads_tools/task_management.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/multiprocess/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/multiprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/multiprocess/multiprocess_testing.py` & `cengal-3.2.0.1/cengal/parallel_execution/multiprocess/multiprocess_testing.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/multiprocess/multiprocessing_task_pool.py` & `cengal-3.2.0.1/cengal/parallel_execution/multiprocess/multiprocessing_task_pool.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/multiprocess/multiprocessing_task_runner.py` & `cengal-3.2.0.1/cengal/parallel_execution/multiprocess/multiprocessing_task_runner.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/multithreading/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/multithreading/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/parallel_execution/multithreading/thread_workers_pool.py` & `cengal-3.2.0.1/cengal/parallel_execution/multithreading/thread_workers_pool.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/performance_test_lib/__init__.py` & `cengal-3.2.0.1/cengal/performance_test_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/performance_test_lib/versions/__init__.py` & `cengal-3.2.0.1/cengal/performance_test_lib/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/performance_test_lib/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/performance_test_lib/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/performance_test_lib/versions/v_0/performance_test_lib.py` & `cengal-3.2.0.1/cengal/performance_test_lib/versions/v_0/performance_test_lib.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/performance_test_lib/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/performance_test_lib/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/performance_test_lib/versions/v_0/tests/test__performance_test_lib.py` & `cengal-3.2.0.1/cengal/performance_test_lib/versions/v_0/tests/test__performance_test_lib.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/performance_test_lib/versions/v_1/__init__.py` & `cengal-3.2.0.1/cengal/performance_test_lib/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/performance_test_lib/versions/v_1/performance_test_lib.py` & `cengal-3.2.0.1/cengal/performance_test_lib/versions/v_1/performance_test_lib.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/performance_test_lib/versions/v_1/tests/__init__.py` & `cengal-3.2.0.1/cengal/performance_test_lib/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/performance_test_lib/versions/v_1/tests/test__performance_test_lib.py` & `cengal-3.2.0.1/cengal/performance_test_lib/versions/v_1/tests/test__performance_test_lib.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/shared_memory/__init__.py` & `cengal-3.2.0.1/cengal/shared_memory/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/shared_memory/versions/1/__init__.py` & `cengal-3.2.0.1/cengal/shared_memory/versions/1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/shared_memory/versions/1/mmap.py` & `cengal-3.2.0.1/cengal/shared_memory/versions/1/mmap.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/shared_memory/versions/__init__.py` & `cengal-3.2.0.1/cengal/shared_memory/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/statistics/__init__.py` & `cengal-3.2.0.1/cengal/statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/statistics/normal_distribution/__init__.py` & `cengal-3.2.0.1/cengal/statistics/normal_distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/statistics/normal_distribution/versions/__init__.py` & `cengal-3.2.0.1/cengal/statistics/normal_distribution/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/statistics/normal_distribution/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/statistics/normal_distribution/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/statistics/normal_distribution/versions/v_0/normal_distribution.py` & `cengal-3.2.0.1/cengal/statistics/normal_distribution/versions/v_0/normal_distribution.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/statistics/normal_distribution/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/statistics/normal_distribution/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/statistics/normal_distribution/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/statistics/normal_distribution/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/system.py` & `cengal-3.2.0.1/cengal/system.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/testing_lib/__init__.py` & `cengal-3.2.0.1/cengal/testing_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/testing_lib/tests_list_runner.py` & `cengal-3.2.0.1/cengal/testing_lib/tests_list_runner.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/brackets_processing/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/brackets_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/brackets_processing/versions/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/brackets_processing/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/brackets_processing/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/brackets_processing/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/brackets_processing/versions/v_0/brackets.py` & `cengal-3.2.0.1/cengal/text_processing/brackets_processing/versions/v_0/brackets.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/brackets_processing/versions/v_0/processing.py` & `cengal-3.2.0.1/cengal/text_processing/brackets_processing/versions/v_0/processing.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/brackets_processing/versions/v_0/standard_brackets.py` & `cengal-3.2.0.1/cengal/text_processing/brackets_processing/versions/v_0/standard_brackets.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/brackets_processing/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/brackets_processing/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/brackets_processing/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/text_processing/brackets_processing/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/encoding_detection/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/encoding_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/encoding_detection/versions/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/encoding_detection/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/encoding_detection/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/encoding_detection/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/encoding_detection/versions/v_0/encoding_detection.py` & `cengal-3.2.0.1/cengal/text_processing/encoding_detection/versions/v_0/encoding_detection.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/encoding_detection/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/encoding_detection/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/encoding_detection/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/text_processing/encoding_detection/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/help_tools.py` & `cengal-3.2.0.1/cengal/text_processing/help_tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/optional_formatter/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/optional_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/optional_formatter/versions/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/optional_formatter/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/optional_formatter/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/optional_formatter/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/optional_formatter/versions/v_0/optional_formatter.py` & `cengal-3.2.0.1/cengal/text_processing/optional_formatter/versions/v_0/optional_formatter.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/optional_formatter/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/optional_formatter/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/optional_formatter/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/text_processing/optional_formatter/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/simple_config_file_processor/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/simple_config_file_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/simple_config_file_processor/versions/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/simple_config_file_processor/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/simple_config_file_processor/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/simple_config_file_processor/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/simple_config_file_processor/versions/v_0/simple_config_file_processor.py` & `cengal-3.2.0.1/cengal/text_processing/simple_config_file_processor/versions/v_0/simple_config_file_processor.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/text_patch/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/text_patch/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/text_patch/brackets/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/text_patch/brackets/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/text_patch/brackets/versions/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/text_patch/brackets/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/text_patch/brackets/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/user_interface/plot/versions/v_0/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .brackets import *
+from .plot import *
 
 """
 Module Docstring
 Docstrings: http://www.python.org/dev/peps/pep-0257/
 """
 
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
```

### Comparing `cengal-3.2.0/cengal/text_processing/text_patch/brackets/versions/v_0/brackets.py` & `cengal-3.2.0.1/cengal/text_processing/text_patch/brackets/versions/v_0/brackets.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/text_patch/brackets/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/text_patch/brackets/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/text_patch/brackets/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/text_processing/text_patch/brackets/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/text_patch/simple/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/text_patch/simple/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/text_patch/simple/versions/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/text_patch/simple/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/text_patch/simple/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/text_patch/simple/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/text_patch/simple/versions/v_0/simple.py` & `cengal-3.2.0.1/cengal/text_processing/text_patch/simple/versions/v_0/simple.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/text_patch/simple/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/text_patch/simple/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/text_patch/simple/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/text_processing/text_patch/simple/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/text_processing/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/text_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/text_processing/versions/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/text_processing/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/text_processing/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/text_processing/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/text_processing/versions/v_0/processing.py` & `cengal-3.2.0.1/cengal/text_processing/text_processing/versions/v_0/processing.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/text_processing/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/text_processing/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/text_processing/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/text_processing/text_processing/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/text_translator/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/text_translator/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/text_translator/versions/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/text_translator/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/text_translator/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/text_translator/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/text_translator/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/text_translator/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/text_translator/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/text_processing/text_translator/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/text_translator/versions/v_0/text_translator.py` & `cengal-3.2.0.1/cengal/text_processing/text_translator/versions/v_0/text_translator.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/utf_bom_processing/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/utf_bom_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/utf_bom_processing/versions/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/utf_bom_processing/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/utf_bom_processing/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/utf_bom_processing/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/utf_bom_processing/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/text_processing/utf_bom_processing/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/utf_bom_processing/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/text_processing/utf_bom_processing/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/text_processing/utf_bom_processing/versions/v_0/utf_bom_processing.py` & `cengal-3.2.0.1/cengal/text_processing/utf_bom_processing/versions/v_0/utf_bom_processing.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/__init__.py` & `cengal-3.2.0.1/cengal/time_management/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/cpu_clock/__init__.py` & `cengal-3.2.0.1/cengal/time_management/cpu_clock/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/cpu_clock/versions/__init__.py` & `cengal-3.2.0.1/cengal/time_management/cpu_clock/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/cpu_clock/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/time_management/relative_time/constants/versions/v_0/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .cpu_clock import *
+from .constants import *
 
 """
 Module Docstring
 Docstrings: http://www.python.org/dev/peps/pep-0257/
 """
 
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
```

### Comparing `cengal-3.2.0/cengal/time_management/cpu_clock/versions/v_0/compilable/__init__.py` & `cengal-3.2.0.1/cengal/time_management/cpu_clock/versions/v_0/compilable/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/cpu_clock/versions/v_0/compilable/__x__build_config.py` & `cengal-3.2.0.1/cengal/time_management/cpu_clock/versions/v_0/compilable/__x__build_config.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/cpu_clock/versions/v_0/cpu_clock.py` & `cengal-3.2.0.1/cengal/unittest/patcher/versions/v_0/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 # 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
-__all__ = ['cpu_clock', 'CPU_TICKS_PER_SECOND']
-
+from .patcher import *
 
 """
 Module Docstring
 Docstrings: http://www.python.org/dev/peps/pep-0257/
 """
 
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
@@ -30,21 +28,7 @@
 __license__ = "Apache License, Version 2.0"
 __version__ = "3.2.0"
 __maintainer__ = "ButenkoMS <gtalk@butenkoms.space>"
 __email__ = "gtalk@butenkoms.space"
 # __status__ = "Prototype"
 __status__ = "Development"
 # __status__ = "Production"
-
-
-from cengal.time_management.cpu_clock_cycles import cpu_clock_cycles, set_cycles_per_second, cpu_clock
-from cengal.hardware.info.cpu import cpu_info
-from cengal.time_management.load_best_timer import perf_counter
-
-
-CPU_TICKS_PER_SECOND = cpu_info().hz_advertised[0]
-
-
-if 0 == CPU_TICKS_PER_SECOND:
-    cpu_clock = perf_counter
-else:
-    set_cycles_per_second(CPU_TICKS_PER_SECOND)
```

### Comparing `cengal-3.2.0/cengal/time_management/cpu_clock/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/time_management/cpu_clock/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/cpu_clock/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/time_management/cpu_clock/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/cpu_clock_cycles/__init__.py` & `cengal-3.2.0.1/cengal/time_management/cpu_clock_cycles/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/cpu_clock_cycles/versions/__init__.py` & `cengal-3.2.0.1/cengal/time_management/cpu_clock_cycles/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/cpu_clock_cycles/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/time_management/cpu_clock_cycles/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/__build_config.py` & `cengal-3.2.0.1/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/__build_config.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/__init__.py` & `cengal-3.2.0.1/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/cpu_clock_cycles.c` & `cengal-3.2.0.1/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/cpu_clock_cycles.h`

 * *Files 21% similar despite different names*

```diff
@@ -9,45 +9,25 @@
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 
+#ifndef RDTSCP_H
+#define RDTSCP_H
+
 #if defined(IS_X86)
 
-extern unsigned long long c_cpu_clock_cycles()
-{
-    long long result;
-    asm volatile(
-        "RDTSCP;"
-        "SHLQ $32,%%rdx;"
-        "ORQ %%rdx,%%rax;"
-        "MOVQ %%rax,%0;"
-        :"=r"(result)
-        :
-        :"rdx","rax", "rcx"
-    );
-    return result;
-}
+unsigned long long c_cpu_clock_cycles();
 
 #elif defined(IS_ARM)
 
-extern u64 c_cpu_clock_cycles()
-{
-    u64 result;
-    asm volatile(
-        "mrs %0, cntvct_el0"
-        : "=r" (result)
-    );
-
-    return result;
-}
+unsigned u64 c_cpu_clock_cycles();
 
 #else
 
-extern unsigned long long c_cpu_clock_cycles()
-{
-    return 0;
-}
+unsigned long long c_cpu_clock_cycles();
+
+#endif
 
-#endif
+#endif
```

### Comparing `cengal-3.2.0/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/cpu_clock_cycles.h` & `cengal-3.2.0.1/cengal/user_interface/console/progress_meter/versions/v_0/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,38 @@
-// Copyright © 2012-2023 ButenkoMS. All rights reserved. Contacts: <gtalk@butenkoms.space>
-// 
-// Licensed under the Apache License, Version 2.0 (the "License");
-// you may not use this file except in compliance with the License.
-// You may obtain a copy of the License at
-// 
-//     http://www.apache.org/licenses/LICENSE-2.0
-// 
-// Unless required by applicable law or agreed to in writing, software
-// distributed under the License is distributed on an "AS IS" BASIS,
-// WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-// See the License for the specific language governing permissions and
-// limitations under the License.
+#!/usr/bin/env python
+# coding=utf-8
 
-
-#ifndef RDTSCP_H
-#define RDTSCP_H
-
-#if defined(IS_X86)
-
-unsigned long long c_cpu_clock_cycles();
-
-#elif defined(IS_ARM)
-
-unsigned u64 c_cpu_clock_cycles();
-
-#else
-
-unsigned long long c_cpu_clock_cycles();
-
-#endif
-
-#endif
+# Copyright © 2012-2023 ButenkoMS. All rights reserved. Contacts: <gtalk@butenkoms.space>
+# 
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+# 
+#     http://www.apache.org/licenses/LICENSE-2.0
+# 
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from cengal.system import PYTHON_VERSION_INT
+if 2 == PYTHON_VERSION_INT[0]:
+    from .progress_meter_python2 import *
+else:
+    from .progress_meter import *
+
+"""
+Module Docstring
+Docstrings: http://www.python.org/dev/peps/pep-0257/
+"""
+
+__author__ = "ButenkoMS <gtalk@butenkoms.space>"
+__copyright__ = "Copyright © 2012-2023 ButenkoMS. All rights reserved. Contacts: <gtalk@butenkoms.space>"
+__credits__ = ["ButenkoMS <gtalk@butenkoms.space>", ]
+__license__ = "Apache License, Version 2.0"
+__version__ = "3.2.0"
+__maintainer__ = "ButenkoMS <gtalk@butenkoms.space>"
+__email__ = "gtalk@butenkoms.space"
+# __status__ = "Prototype"
+__status__ = "Development"
+# __status__ = "Production"
```

### Comparing `cengal-3.2.0/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/cpu_clock_cycles__cython.pyx` & `cengal-3.2.0.1/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/cpu_clock_cycles__cython.pyx`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/high_precision_sync_sleep/__init__.py` & `cengal-3.2.0.1/cengal/time_management/high_precision_sync_sleep/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/high_precision_sync_sleep/versions/__init__.py` & `cengal-3.2.0.1/cengal/time_management/high_precision_sync_sleep/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/high_precision_sync_sleep/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/time_management/high_precision_sync_sleep/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/high_precision_sync_sleep/versions/v_0/high_precision_sync_sleep__cython.pyx` & `cengal-3.2.0.1/cengal/time_management/high_precision_sync_sleep/versions/v_0/high_precision_sync_sleep__cython.pyx`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/load_best_timer/__init__.py` & `cengal-3.2.0.1/cengal/time_management/load_best_timer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/load_best_timer/versions/__init__.py` & `cengal-3.2.0.1/cengal/time_management/load_best_timer/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/load_best_timer/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/time_management/load_best_timer/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/load_best_timer/versions/v_0/load_best_timer.py` & `cengal-3.2.0.1/cengal/time_management/load_best_timer/versions/v_0/load_best_timer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/relative_time/__init__.py` & `cengal-3.2.0.1/cengal/time_management/relative_time/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/relative_time/approximate_representation/__init__.py` & `cengal-3.2.0.1/cengal/time_management/relative_time/approximate_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/relative_time/approximate_representation/versions/__init__.py` & `cengal-3.2.0.1/cengal/time_management/relative_time/approximate_representation/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/relative_time/approximate_representation/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/time_management/relative_time/approximate_representation/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/relative_time/approximate_representation/versions/v_0/approximate_representation.py` & `cengal-3.2.0.1/cengal/time_management/relative_time/approximate_representation/versions/v_0/approximate_representation.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/relative_time/bysiness_relativedelta/__init__.py` & `cengal-3.2.0.1/cengal/time_management/relative_time/bysiness_relativedelta/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/relative_time/bysiness_relativedelta/versions/__init__.py` & `cengal-3.2.0.1/cengal/time_management/relative_time/bysiness_relativedelta/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/bysiness_relativedelta.py` & `cengal-3.2.0.1/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/bysiness_relativedelta.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/relative_time/constants/__init__.py` & `cengal-3.2.0.1/cengal/time_management/relative_time/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/relative_time/constants/versions/__init__.py` & `cengal-3.2.0.1/cengal/time_management/relative_time/constants/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/relative_time/constants/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal_setup_scripts/install_required_packages/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .constants import *
+from .install_packages import *
 
 """
 Module Docstring
 Docstrings: http://www.python.org/dev/peps/pep-0257/
 """
 
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
```

### Comparing `cengal-3.2.0/cengal/time_management/relative_time/constants/versions/v_0/constants.py` & `cengal-3.2.0.1/cengal/time_management/relative_time/constants/versions/v_0/constants.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/relative_time/relativedelta/__init__.py` & `cengal-3.2.0.1/cengal/time_management/relative_time/relativedelta/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/relative_time/relativedelta/versions/__init__.py` & `cengal-3.2.0.1/cengal/time_management/relative_time/relativedelta/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/relative_time/relativedelta/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/time_management/relative_time/relativedelta/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/relative_time/relativedelta/versions/v_0/relativedelta.py` & `cengal-3.2.0.1/cengal/time_management/relative_time/relativedelta/versions/v_0/relativedelta.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/relative_time/timedelta/__init__.py` & `cengal-3.2.0.1/cengal/time_management/relative_time/timedelta/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/relative_time/timedelta/versions/__init__.py` & `cengal-3.2.0.1/cengal/time_management/relative_time/timedelta/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/relative_time/timedelta/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/time_management/relative_time/timedelta/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/relative_time/timedelta/versions/v_0/timedelta.py` & `cengal-3.2.0.1/cengal/time_management/relative_time/timedelta/versions/v_0/timedelta.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/repeat_for_a_time/__init__.py` & `cengal-3.2.0.1/cengal/time_management/repeat_for_a_time/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/repeat_for_a_time/versions/__init__.py` & `cengal-3.2.0.1/cengal/time_management/repeat_for_a_time/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/repeat_for_a_time/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/time_management/repeat_for_a_time/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/repeat_for_a_time/versions/v_0/repeat_for_a_time__cython.pyx` & `cengal-3.2.0.1/cengal/time_management/repeat_for_a_time/versions/v_0/repeat_for_a_time__cython.pyx`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/repeat_for_a_time/versions/v_0/repeat_for_a_time__python.py` & `cengal-3.2.0.1/cengal/time_management/repeat_for_a_time/versions/v_0/repeat_for_a_time__python.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/repeat_for_a_time/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/time_management/repeat_for_a_time/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/repeat_for_a_time/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/time_management/repeat_for_a_time/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/repeat_for_a_time/versions/v_0/tests/example_for__repeat_for_a_time.py` & `cengal-3.2.0.1/cengal/time_management/repeat_for_a_time/versions/v_0/tests/example_for__repeat_for_a_time.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/sleep_tools/__init__.py` & `cengal-3.2.0.1/cengal/time_management/sleep_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/sleep_tools/versions/__init__.py` & `cengal-3.2.0.1/cengal/time_management/sleep_tools/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/sleep_tools/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/time_management/sleep_tools/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/sleep_tools/versions/v_0/sleep_tools.py` & `cengal-3.2.0.1/cengal/time_management/sleep_tools/versions/v_0/sleep_tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/sleep_tools/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/time_management/sleep_tools/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/sleep_tools/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/time_management/sleep_tools/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/timer/__init__.py` & `cengal-3.2.0.1/cengal/time_management/timer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/timer/versions/__init__.py` & `cengal-3.2.0.1/cengal/time_management/timer/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/timer/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/time_management/timer/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/timer/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/time_management/timer/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/timer/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/time_management/timer/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/timer/versions/v_0/timer.py` & `cengal-3.2.0.1/cengal/time_management/timer/versions/v_0/timer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/timer/versions/v_1/__init__.py` & `cengal-3.2.0.1/cengal/time_management/timer/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/timer/versions/v_1/tests/__init__.py` & `cengal-3.2.0.1/cengal/time_management/timer/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/timer/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/time_management/timer/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/timer/versions/v_1/timer.py` & `cengal-3.2.0.1/cengal/time_management/timer/versions/v_1/timer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/timer_precision/__init__.py` & `cengal-3.2.0.1/cengal/time_management/timer_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/timer_precision/versions/__init__.py` & `cengal-3.2.0.1/cengal/time_management/timer_precision/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/timer_precision/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/time_management/timer_precision/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/timer_precision/versions/v_0/test_timer_precision.py` & `cengal-3.2.0.1/cengal/time_management/timer_precision/versions/v_0/test_timer_precision.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/timer_precision/versions/v_1/__init__.py` & `cengal-3.2.0.1/cengal/time_management/timer_precision/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/time_management/timer_precision/versions/v_1/timer_precision.py` & `cengal-3.2.0.1/cengal/time_management/timer_precision/versions/v_1/timer_precision.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/unittest/__init__.py` & `cengal-3.2.0.1/cengal/unittest/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/unittest/behavior_stabilizer/__init__.py` & `cengal-3.2.0.1/cengal/unittest/behavior_stabilizer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/unittest/behavior_stabilizer/versions/__init__.py` & `cengal-3.2.0.1/cengal/unittest/behavior_stabilizer/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/unittest/behavior_stabilizer/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/unittest/behavior_stabilizer/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/unittest/behavior_stabilizer/versions/v_0/behavior_stabilizer.py` & `cengal-3.2.0.1/cengal/unittest/behavior_stabilizer/versions/v_0/behavior_stabilizer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/unittest/behavior_stabilizer/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/unittest/behavior_stabilizer/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/unittest/behavior_stabilizer/versions/v_0/tests/_test__behavior_stabilizer.py` & `cengal-3.2.0.1/cengal/unittest/behavior_stabilizer/versions/v_0/tests/_test__behavior_stabilizer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/unittest/patcher/__init__.py` & `cengal-3.2.0.1/cengal/unittest/patcher/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/unittest/patcher/versions/__init__.py` & `cengal-3.2.0.1/cengal/unittest/patcher/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/unittest/patcher/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/user_interface/console/progress_meter/versions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .patcher import *
+from .v_0 import *
 
 """
 Module Docstring
 Docstrings: http://www.python.org/dev/peps/pep-0257/
 """
 
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
```

### Comparing `cengal-3.2.0/cengal/unittest/patcher/versions/v_0/patcher.py` & `cengal-3.2.0.1/cengal/unittest/patcher/versions/v_0/patcher.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/unittest/patcher/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/unittest/patcher/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/unittest/patcher/versions/v_0/tests/_test__patcher.py` & `cengal-3.2.0.1/cengal/unittest/patcher/versions/v_0/tests/_test__patcher.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/universal_parser/__init__.py` & `cengal-3.2.0.1/cengal/universal_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/universal_parser/help_tools.py` & `cengal-3.2.0.1/cengal/universal_parser/help_tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/universal_parser/idioms.py` & `cengal-3.2.0.1/cengal/universal_parser/idioms.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/universal_parser/parser.py` & `cengal-3.2.0.1/cengal/universal_parser/parser.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/universal_parser/test.py` & `cengal-3.2.0.1/cengal/universal_parser/test.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/universal_parser/types.py` & `cengal-3.2.0.1/cengal/universal_parser/types.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/upk_helping_tools/__init__.py` & `cengal-3.2.0.1/cengal/upk_helping_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/upk_helping_tools/upk_api.py` & `cengal-3.2.0.1/cengal/upk_helping_tools/upk_api.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/upk_helping_tools/upk_constants.py` & `cengal-3.2.0.1/cengal/upk_helping_tools/upk_constants.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/upk_helping_tools/upk_utils_api.py` & `cengal-3.2.0.1/cengal/upk_helping_tools/upk_utils_api.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/__init__.py` & `cengal-3.2.0.1/cengal/user_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/console/__init__.py` & `cengal-3.2.0.1/cengal/user_interface/console/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/console/chooser.py` & `cengal-3.2.0.1/cengal/user_interface/console/chooser.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/console/colorama_helpers.py` & `cengal-3.2.0.1/cengal/user_interface/console/colorama_helpers.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/console/encoding_changer.py` & `cengal-3.2.0.1/cengal/user_interface/console/encoding_changer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/console/progress_meter/__init__.py` & `cengal-3.2.0.1/cengal/user_interface/console/progress_meter/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/console/progress_meter/versions/__init__.py` & `cengal-3.2.0.1/cengal/user_interface/gui/nt/blur_behind/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/console/progress_meter/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal_setup_scripts/find_and_prepare_cython_modules/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,19 +11,15 @@
 # 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from cengal.system import PYTHON_VERSION_INT
-if 2 == PYTHON_VERSION_INT[0]:
-    from .progress_meter_python2 import *
-else:
-    from .progress_meter import *
+from .find_and_prepare_cython_modules import *
 
 """
 Module Docstring
 Docstrings: http://www.python.org/dev/peps/pep-0257/
 """
 
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
```

### Comparing `cengal-3.2.0/cengal/user_interface/console/progress_meter/versions/v_0/progress_meter.py` & `cengal-3.2.0.1/cengal/user_interface/console/progress_meter/versions/v_0/progress_meter.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/console/progress_meter/versions/v_0/progress_meter_python2.py` & `cengal-3.2.0.1/cengal/user_interface/console/progress_meter/versions/v_0/progress_meter_python2.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/gui/__init__.py` & `cengal-3.2.0.1/cengal/user_interface/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/gui/nt/__init__.py` & `cengal-3.2.0.1/cengal/user_interface/gui/nt/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/gui/nt/blur_behind/__init__.py` & `cengal-3.2.0.1/cengal/user_interface/gui/nt/blur_behind/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/gui/nt/blur_behind/versions/__init__.py` & `cengal-3.2.0.1/cengal/user_interface/gui/nt/dpi_awareness/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/gui/nt/blur_behind/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/user_interface/gui/nt/blur_behind/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/gui/nt/blur_behind/versions/v_0/blur_behind.py` & `cengal-3.2.0.1/cengal/user_interface/gui/nt/blur_behind/versions/v_0/blur_behind.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/gui/nt/dpi_awareness/__init__.py` & `cengal-3.2.0.1/cengal/user_interface/gui/nt/dpi_awareness/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/gui/nt/dpi_awareness/versions/__init__.py` & `cengal-3.2.0.1/cengal/user_interface/plot/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/dpi_awareness.py` & `cengal-3.2.0.1/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/dpi_awareness.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/plot/__init__.py` & `cengal-3.2.0.1/cengal/user_interface/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/plot/versions/__init__.py` & `cengal-3.2.0.1/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/plot/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .plot import *
 
 """
 Module Docstring
 Docstrings: http://www.python.org/dev/peps/pep-0257/
 """
 
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
```

### Comparing `cengal-3.2.0/cengal/user_interface/plot/versions/v_0/plot.py` & `cengal-3.2.0.1/cengal/user_interface/plot/versions/v_0/plot.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/plot/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal/user_interface/plot/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/user_interface/plot/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/user_interface/plot/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/web_tools/__init__.py` & `cengal-3.2.0.1/cengal/web_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/web_tools/detect_browsers_host_device_type/__init__.py` & `cengal-3.2.0.1/cengal/web_tools/detect_browsers_host_device_type/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/__init__.py` & `cengal-3.2.0.1/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/__init__.py` & `cengal-3.2.0.1/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .v_0 import *
+from ._test__template_submodule import *
 
 """
 Module Docstring
 Docstrings: http://www.python.org/dev/peps/pep-0257/
 """
 
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
```

### Comparing `cengal-3.2.0/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/__init__.py` & `cengal-3.2.0.1/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/by_http_user_agent.py` & `cengal-3.2.0.1/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/by_http_user_agent.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/__init__.py` & `cengal-3.2.0.1/cengal_setup_scripts/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,24 +11,27 @@
 # 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from ._test__template_submodule import *
 
 """
 Module Docstring
 Docstrings: http://www.python.org/dev/peps/pep-0257/
 """
 
+
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
 __copyright__ = "Copyright © 2012-2023 ButenkoMS. All rights reserved. Contacts: <gtalk@butenkoms.space>"
 __credits__ = ["ButenkoMS <gtalk@butenkoms.space>", ]
 __license__ = "Apache License, Version 2.0"
 __version__ = "3.2.0"
 __maintainer__ = "ButenkoMS <gtalk@butenkoms.space>"
 __email__ = "gtalk@butenkoms.space"
 # __status__ = "Prototype"
 __status__ = "Development"
 # __status__ = "Production"
+
+
+from .install_required_packages import *
```

### Comparing `cengal-3.2.0/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.2.0.1/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal/web_tools/help_tools.py` & `cengal-3.2.0.1/cengal/web_tools/help_tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal.egg-info/PKG-INFO` & `cengal-3.2.0.1/cengal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cengal
-Version: 3.2.0
+Version: 3.2.0.1
 Summary: General purpose library
 Home-page: https://github.com/FI-Mihej/Cengal
 Author: ButenkoMS
 Author-email: gtalk@butenkoms.space
 License: Apache License, Version 2.0
 Keywords: async loop,coroutine,async Qt,async Tkinter,bytecode manipulation,introspection,text parsing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cengal-3.2.0/cengal.egg-info/SOURCES.txt` & `cengal-3.2.0.1/cengal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal_setup_scripts/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_standard_services/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,17 @@
 
 
 """
 Module Docstring
 Docstrings: http://www.python.org/dev/peps/pep-0257/
 """
 
-
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
 __copyright__ = "Copyright © 2012-2023 ButenkoMS. All rights reserved. Contacts: <gtalk@butenkoms.space>"
 __credits__ = ["ButenkoMS <gtalk@butenkoms.space>", ]
 __license__ = "Apache License, Version 2.0"
 __version__ = "3.2.0"
 __maintainer__ = "ButenkoMS <gtalk@butenkoms.space>"
 __email__ = "gtalk@butenkoms.space"
 # __status__ = "Prototype"
 __status__ = "Development"
 # __status__ = "Production"
-
-
-from .install_required_packages import *
```

### Comparing `cengal-3.2.0/cengal_setup_scripts/compile_all_cython_modules.py` & `cengal-3.2.0.1/cengal_setup_scripts/compile_all_cython_modules.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal_setup_scripts/find_and_prepare_cython_modules/__init__.py` & `cengal-3.2.0.1/cengal/parallel_execution/coroutines/coro_tools/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .find_and_prepare_cython_modules import *
 
 """
 Module Docstring
 Docstrings: http://www.python.org/dev/peps/pep-0257/
 """
 
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
```

### Comparing `cengal-3.2.0/cengal_setup_scripts/install_required_packages/__init__.py` & `cengal-3.2.0.1/cengal_setup_scripts/install_required_packages/set_environment_variables.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,24 +11,48 @@
 # 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .install_packages import *
 
 """
 Module Docstring
 Docstrings: http://www.python.org/dev/peps/pep-0257/
 """
 
+
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
 __copyright__ = "Copyright © 2012-2023 ButenkoMS. All rights reserved. Contacts: <gtalk@butenkoms.space>"
 __credits__ = ["ButenkoMS <gtalk@butenkoms.space>", ]
 __license__ = "Apache License, Version 2.0"
 __version__ = "3.2.0"
 __maintainer__ = "ButenkoMS <gtalk@butenkoms.space>"
 __email__ = "gtalk@butenkoms.space"
 # __status__ = "Prototype"
 __status__ = "Development"
 # __status__ = "Production"
+
+
+import os
+import sys
+
+
+
+
+__author__ = 'ButenkoMS <gtalk@butenkoms.space>'
+
+
+def main():
+    if sys.platform == 'linux':
+        dir_of_the_current_file = os.path.dirname(os.path.abspath(__file__))
+        parent_dir = os.path.dirname(dir_of_the_current_file)
+        parent_dir = os.path.dirname(parent_dir)
+        path_to_lib = os.path.join(parent_dir, 'cengal')
+        call_result = os.system('export PYTHONPATH=$PYTHONPATH:{}'.format(path_to_lib))
+        if path_to_lib not in sys.path:
+            sys.path.append(path_to_lib)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `cengal-3.2.0/cengal_setup_scripts/install_required_packages/install_packages.py` & `cengal-3.2.0.1/cengal_setup_scripts/install_required_packages/install_packages.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             'msgpack-pypy',
         ]
 
         self.universal = [
             # 'wheel',
             # 'virtualenv',
 
-            'Cython',
+            'Cython>=0.29.34',
             'python-dateutil',
             # 'holidays',
             # 'bdateutil',  # Used by Cengal. However requires outdated version of python-dateutil==2.2. Leads to conflicts with 'pendulum' and 'pandas'. Must not be installed. Latest dev version will be installed from github in ExternalGitModules.
 
             # 'paver',  # needed for python-lzf module installation process (also for zip-module)
             # 'urllib3',  # already preinstalled in Ubuntu 14.04 x64
             # 'thrift',
```

### Comparing `cengal-3.2.0/cengal_setup_scripts/setup__dynamic_list_of_pieces.py` & `cengal-3.2.0.1/cengal_setup_scripts/setup__dynamic_list_of_pieces.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal_setup_scripts/setup__recv_buff_size_computer.py` & `cengal-3.2.0.1/cengal_setup_scripts/setup__recv_buff_size_computer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/cengal_setup_scripts/setup__repeat_for_a_time.py` & `cengal-3.2.0.1/cengal_setup_scripts/setup__repeat_for_a_time.py`

 * *Files identical despite different names*

### Comparing `cengal-3.2.0/setup.py` & `cengal-3.2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 Docstrings: http://www.python.org/dev/peps/pep-0257/
 """
 
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
 __copyright__ = "Copyright © 2012-2023 ButenkoMS. All rights reserved. Contacts: <gtalk@butenkoms.space>"
 __credits__ = ["ButenkoMS <gtalk@butenkoms.space>", ]
 __license__ = "Apache License, Version 2.0"
-__version__ = "3.2.0"
+__version__ = "3.2.0.1"
 __maintainer__ = "ButenkoMS <gtalk@butenkoms.space>"
 __email__ = "gtalk@butenkoms.space"
 # __status__ = "Prototype"
 __status__ = "Development"
 # __status__ = "Production"
```

