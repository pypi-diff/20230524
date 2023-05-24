# Comparing `tmp/odcs-0.5.0.tar.gz` & `tmp/odcs-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odcs-0.5.0.tar", last modified: Wed Mar  1 02:11:13 2023, max compression
+gzip compressed data, was "dist/odcs-0.6.0.tar", last modified: Fri May 19 17:05:05 2023, max compression
```

## Comparing `odcs-0.5.0.tar` & `odcs-0.6.0.tar`

### file list

```diff
@@ -1,158 +1,156 @@
-drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-03-01 02:11:13.012436 odcs-0.5.0/
--rw-r--r--   0 hlin       (501) wheel        (0)      269 2023-03-01 02:01:26.000000 odcs-0.5.0/MANIFEST.in
--rw-r--r--   0 hlin       (501) wheel        (0)    19824 2023-03-01 02:11:13.011962 odcs-0.5.0/PKG-INFO
--rw-r--r--   0 hlin       (501) wheel        (0)    19359 2023-03-01 02:01:26.000000 odcs-0.5.0/README.md
-drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-03-01 02:11:12.949203 odcs-0.5.0/client/
-drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-03-01 02:11:12.949494 odcs-0.5.0/client/contrib/
--rwxr-xr-x   0 hlin       (501) wheel        (0)    17341 2023-03-01 02:01:26.000000 odcs-0.5.0/client/contrib/odcs
-drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-03-01 02:11:12.949824 odcs-0.5.0/client/odcs/
--rw-r--r--   0 hlin       (501) wheel        (0)       65 2023-03-01 02:01:26.000000 odcs-0.5.0/client/odcs/__init__.py
-drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-03-01 02:11:12.950616 odcs-0.5.0/client/odcs/client/
--rw-r--r--   0 hlin       (501) wheel        (0)      155 2023-03-01 02:01:26.000000 odcs-0.5.0/client/odcs/client/__init__.py
--rw-r--r--   0 hlin       (501) wheel        (0)    25947 2023-03-01 02:01:26.000000 odcs-0.5.0/client/odcs/client/odcs.py
--rw-r--r--   0 hlin       (501) wheel        (0)       50 2023-03-01 02:01:26.000000 odcs-0.5.0/client/requirements.txt
-drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-03-01 02:11:12.951149 odcs-0.5.0/client/tests/
--rw-r--r--   0 hlin       (501) wheel        (0)    23924 2023-03-01 02:01:26.000000 odcs-0.5.0/client/tests/test_client_odcs.py
-drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-03-01 02:11:12.944896 odcs-0.5.0/common/
-drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-03-01 02:11:12.951497 odcs-0.5.0/common/odcs/
--rw-r--r--   0 hlin       (501) wheel        (0)       65 2023-03-01 02:01:26.000000 odcs-0.5.0/common/odcs/__init__.py
-drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-03-01 02:11:12.951981 odcs-0.5.0/common/odcs/common/
--rw-r--r--   0 hlin       (501) wheel        (0)        0 2023-03-01 02:01:26.000000 odcs-0.5.0/common/odcs/common/__init__.py
--rw-r--r--   0 hlin       (501) wheel        (0)     3902 2023-03-01 02:01:26.000000 odcs-0.5.0/common/odcs/common/types.py
-drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-03-01 02:11:12.953785 odcs-0.5.0/docs/
--rw-r--r--   0 hlin       (501) wheel        (0)     1608 2023-03-01 02:01:26.000000 odcs-0.5.0/docs/about.rst
--rw-r--r--   0 hlin       (501) wheel        (0)    14587 2023-03-01 02:01:26.000000 odcs-0.5.0/docs/api.rst
--rw-r--r--   0 hlin       (501) wheel        (0)     3031 2023-03-01 02:01:26.000000 odcs-0.5.0/docs/client.rst
--rw-r--r--   0 hlin       (501) wheel        (0)      641 2023-03-01 02:01:26.000000 odcs-0.5.0/docs/index.rst
--rw-r--r--   0 hlin       (501) wheel        (0)      125 2023-03-01 02:01:26.000000 odcs-0.5.0/docs/module.rst
--rw-r--r--   0 hlin       (501) wheel        (0)     2429 2023-03-01 02:01:26.000000 odcs-0.5.0/docs/pulp.rst
--rw-r--r--   0 hlin       (501) wheel        (0)     8447 2023-03-01 02:01:26.000000 odcs-0.5.0/docs/raw_config.rst
-drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-03-01 02:11:12.956263 odcs-0.5.0/odcs.egg-info/
--rw-r--r--   0 hlin       (501) wheel        (0)    19824 2023-03-01 02:11:12.000000 odcs-0.5.0/odcs.egg-info/PKG-INFO
--rw-r--r--   0 hlin       (501) wheel        (0)     5568 2023-03-01 02:11:12.000000 odcs-0.5.0/odcs.egg-info/SOURCES.txt
--rw-r--r--   0 hlin       (501) wheel        (0)        1 2023-03-01 02:11:12.000000 odcs-0.5.0/odcs.egg-info/dependency_links.txt
--rw-r--r--   0 hlin       (501) wheel        (0)      253 2023-03-01 02:11:12.000000 odcs-0.5.0/odcs.egg-info/entry_points.txt
--rw-r--r--   0 hlin       (501) wheel        (0)        1 2023-03-01 02:03:46.000000 odcs-0.5.0/odcs.egg-info/not-zip-safe
--rw-r--r--   0 hlin       (501) wheel        (0)      706 2023-03-01 02:11:12.000000 odcs-0.5.0/odcs.egg-info/requires.txt
--rw-r--r--   0 hlin       (501) wheel        (0)        5 2023-03-01 02:11:12.000000 odcs-0.5.0/odcs.egg-info/top_level.txt
-drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-03-01 02:11:12.956831 odcs-0.5.0/server/
-drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-03-01 02:11:12.959068 odcs-0.5.0/server/conf/
--rw-r--r--   0 hlin       (501) wheel        (0)       96 2023-03-01 02:01:26.000000 odcs-0.5.0/server/conf/__init__.py
--rw-r--r--   0 hlin       (501) wheel        (0)     8518 2023-03-01 02:01:26.000000 odcs-0.5.0/server/conf/config.py
--rw-r--r--   0 hlin       (501) wheel        (0)      258 2023-03-01 02:01:26.000000 odcs-0.5.0/server/conf/odcs-httpd-krb.conf
--rw-r--r--   0 hlin       (501) wheel        (0)      632 2023-03-01 02:01:26.000000 odcs-0.5.0/server/conf/odcs-httpd-openidc.conf
--rw-r--r--   0 hlin       (501) wheel        (0)     3586 2023-03-01 02:01:26.000000 odcs-0.5.0/server/conf/pungi.conf
--rw-r--r--   0 hlin       (501) wheel        (0)      277 2023-03-01 02:01:26.000000 odcs-0.5.0/server/conf/raw_config_urls.conf
--rw-r--r--   0 hlin       (501) wheel        (0)       77 2023-03-01 02:01:26.000000 odcs-0.5.0/server/conf/raw_config_wrapper.conf
-drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-03-01 02:11:12.959885 odcs-0.5.0/server/contrib/
--rwxr-xr-x   0 hlin       (501) wheel        (0)    12884 2023-03-01 02:01:26.000000 odcs-0.5.0/server/contrib/odcs-promote-compose
--rw-r--r--   0 hlin       (501) wheel        (0)      140 2023-03-01 02:01:26.000000 odcs-0.5.0/server/contrib/odcs.wsgi
--rwxr-xr-x   0 hlin       (501) wheel        (0)    13660 2023-03-01 02:01:26.000000 odcs-0.5.0/server/contrib/odcs_test_deployment
-drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-03-01 02:11:12.960190 odcs-0.5.0/server/odcs/
--rw-r--r--   0 hlin       (501) wheel        (0)       65 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/__init__.py
-drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-03-01 02:11:12.967355 odcs-0.5.0/server/odcs/server/
--rw-r--r--   0 hlin       (501) wheel        (0)     3297 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/__init__.py
--rw-r--r--   0 hlin       (501) wheel        (0)    14727 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/api_utils.py
--rw-r--r--   0 hlin       (501) wheel        (0)    10896 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/auth.py
--rw-r--r--   0 hlin       (501) wheel        (0)    53108 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/backend.py
--rw-r--r--   0 hlin       (501) wheel        (0)     8931 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/cache.py
--rw-r--r--   0 hlin       (501) wheel        (0)    12252 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/celery_tasks.py
--rw-r--r--   0 hlin       (501) wheel        (0)     4706 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/comps.py
--rw-r--r--   0 hlin       (501) wheel        (0)    22061 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/config.py
--rw-r--r--   0 hlin       (501) wheel        (0)     1323 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/errors.py
--rw-r--r--   0 hlin       (501) wheel        (0)     2722 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/events.py
--rw-r--r--   0 hlin       (501) wheel        (0)     3074 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/logger.py
--rw-r--r--   0 hlin       (501) wheel        (0)     4593 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/manage.py
--rw-r--r--   0 hlin       (501) wheel        (0)    12485 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/mbs.py
--rw-r--r--   0 hlin       (501) wheel        (0)     7706 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/mergerepo.py
--rw-r--r--   0 hlin       (501) wheel        (0)     2794 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/messaging.py
--rw-r--r--   0 hlin       (501) wheel        (0)    10344 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/metrics.py
-drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-03-01 02:11:12.968528 odcs-0.5.0/server/odcs/server/migrations/
--rw-r--r--   0 hlin       (501) wheel        (0)       38 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/README
--rw-r--r--   0 hlin       (501) wheel        (0)      770 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/alembic.ini
--rw-r--r--   0 hlin       (501) wheel        (0)     2807 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/env.py
--rw-r--r--   0 hlin       (501) wheel        (0)      412 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/script.py.mako
-drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-03-01 02:11:12.997116 odcs-0.5.0/server/odcs/server/migrations/versions/
--rw-r--r--   0 hlin       (501) wheel        (0)      661 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/0571a5ca58a0_add_index_to_compose_state.py
--rw-r--r--   0 hlin       (501) wheel        (0)      776 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/0d4d8e1cfe29_create_user_model.py
--rw-r--r--   0 hlin       (501) wheel        (0)      461 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/11b350234051_.py
--rw-r--r--   0 hlin       (501) wheel        (0)      917 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/16e08da18b49_add_compose_base_module_stream_version.py
--rw-r--r--   0 hlin       (501) wheel        (0)      711 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/3b92820da295_add_index_to_compose_time_to_expire.py
--rw-r--r--   0 hlin       (501) wheel        (0)      420 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/4514febd31fa_add_builds.py
--rw-r--r--   0 hlin       (501) wheel        (0)      648 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/512890e6864d_add_compose_scratch_modules.py
--rw-r--r--   0 hlin       (501) wheel        (0)     1440 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/566733ac3811_.py
--rw-r--r--   0 hlin       (501) wheel        (0)      872 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/59baece89746_add_compose_base_module_br_name_stream.py
--rw-r--r--   0 hlin       (501) wheel        (0)      480 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/7b143656694f_.py
--rw-r--r--   0 hlin       (501) wheel        (0)      431 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/812f2745248f_.py
--rw-r--r--   0 hlin       (501) wheel        (0)      466 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/82172e6a3154_.py
--rw-r--r--   0 hlin       (501) wheel        (0)      639 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/a855c39e2a0f_store_celery_task_id.py
--rw-r--r--   0 hlin       (501) wheel        (0)      437 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/a8e259e0208c_add_compose_state_reason.py
--rw-r--r--   0 hlin       (501) wheel        (0)      430 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/b00f3b6efaed_.py
--rw-r--r--   0 hlin       (501) wheel        (0)      445 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/b2725d046624_.py
--rw-r--r--   0 hlin       (501) wheel        (0)      421 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/b75ad2afc207_.py
--rw-r--r--   0 hlin       (501) wheel        (0)      423 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/c1b7e84ff39b_.py
--rw-r--r--   0 hlin       (501) wheel        (0)      684 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/c370b90de998_add_index_on_compose_source_type_and_.py
--rw-r--r--   0 hlin       (501) wheel        (0)      471 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/ca08065687c4_.py
--rw-r--r--   0 hlin       (501) wheel        (0)      724 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/cd0781bbdab1_.py
--rw-r--r--   0 hlin       (501) wheel        (0)      648 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/d1da07e15c54_.py
--rw-r--r--   0 hlin       (501) wheel        (0)      818 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/de0a86d7de49_.py
--rw-r--r--   0 hlin       (501) wheel        (0)      651 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/e186faabdafe_.py
--rw-r--r--   0 hlin       (501) wheel        (0)      617 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/e2163db7b15d_.py
--rw-r--r--   0 hlin       (501) wheel        (0)      691 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/f24a36cc8a16_add_index_on_compose_reused_id.py
--rw-r--r--   0 hlin       (501) wheel        (0)      633 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/migrations/versions/f4bc999818d7_add_compose_removed_by.py
--rw-r--r--   0 hlin       (501) wheel        (0)    13271 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/mock_runroot.py
--rw-r--r--   0 hlin       (501) wheel        (0)    20949 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/models.py
--rw-r--r--   0 hlin       (501) wheel        (0)    12560 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/openapi.py
--rw-r--r--   0 hlin       (501) wheel        (0)     2329 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/proxy.py
--rw-r--r--   0 hlin       (501) wheel        (0)    12942 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/pulp.py
--rw-r--r--   0 hlin       (501) wheel        (0)    27376 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/pungi.py
--rw-r--r--   0 hlin       (501) wheel        (0)     3875 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/pungi_compose.py
-drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-03-01 02:11:12.997635 odcs-0.5.0/server/odcs/server/static/
--rw-r--r--   0 hlin       (501) wheel        (0)        0 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/static/.gitkeep
-drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-03-01 02:11:12.998308 odcs-0.5.0/server/odcs/server/templates/
--rw-r--r--   0 hlin       (501) wheel        (0)      535 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/templates/apidoc.html
--rw-r--r--   0 hlin       (501) wheel        (0)     1974 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/templates/index.html
--rw-r--r--   0 hlin       (501) wheel        (0)     6042 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/utils.py
--rw-r--r--   0 hlin       (501) wheel        (0)    37813 2023-03-01 02:01:26.000000 odcs-0.5.0/server/odcs/server/views.py
--rw-r--r--   0 hlin       (501) wheel        (0)      477 2023-03-01 02:01:26.000000 odcs-0.5.0/server/requirements.txt
-drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-03-01 02:11:13.006750 odcs-0.5.0/server/tests/
--rw-r--r--   0 hlin       (501) wheel        (0)     2808 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/Jenkinsfile
--rw-r--r--   0 hlin       (501) wheel        (0)       78 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/__init__.py
-drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-03-01 02:11:13.007125 odcs-0.5.0/server/tests/data/
--rw-r--r--   0 hlin       (501) wheel        (0)      226 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/data/custom_raw_config_wrapper.conf
--rw-r--r--   0 hlin       (501) wheel        (0)     7971 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/mbs.py
-drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-03-01 02:11:13.009141 odcs-0.5.0/server/tests/repo/
--rw-r--r--   0 hlin       (501) wheel        (0)    88568 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/repo/ed-1.14.1-2.module_fd8ca23e.src.rpm
--rw-r--r--   0 hlin       (501) wheel        (0)    80326 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/repo/ed-1.14.1-2.module_fd8ca23e.x86_64.rpm
--rw-r--r--   0 hlin       (501) wheel        (0)    81258 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/repo/ed-debuginfo-1.14.1-2.module_fd8ca23e.x86_64.rpm
--rw-r--r--   0 hlin       (501) wheel        (0)     6878 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/repo/module-build-macros-0.1-1.module_fd8ca23e.noarch.rpm
--rw-r--r--   0 hlin       (501) wheel        (0)     6970 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/repo/module-build-macros-0.1-1.module_fd8ca23e.src.rpm
-drwxr-xr-x   0 hlin       (501) wheel        (0)        0 2023-03-01 02:11:13.011531 odcs-0.5.0/server/tests/repo/repodata/
--rw-r--r--   0 hlin       (501) wheel        (0)     4133 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/repo/repodata/028b753de97c22923bffe2159dcb478cdfa919376e21a68a1aa6ca40fba06f45-primary.sqlite.bz2
--rw-r--r--   0 hlin       (501) wheel        (0)      750 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/repo/repodata/1879db5a1658329be62225ebf1b40cbf8e5d522abd2fdd86157d565c83e1ddc2-modules.yaml.gz
--rw-r--r--   0 hlin       (501) wheel        (0)     1015 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/repo/repodata/2c3a353ba9e47c3e9c8be6c2e25c50fcc11e184a727c645f3f08b66aa1a1654d-other.xml.gz
--rw-r--r--   0 hlin       (501) wheel        (0)     2722 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/repo/repodata/635015f39babdbcdcca3a516576bdcafb57fb77be3b7919cf85363ec558fb8fe-other.sqlite.bz2
--rw-r--r--   0 hlin       (501) wheel        (0)      827 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/repo/repodata/77e6eb5a69d53a9d56f32b3154832d4eff6e2de518c268102d2c6848cffa3e1e-filelists.xml.gz
--rw-r--r--   0 hlin       (501) wheel        (0)     2263 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/repo/repodata/92ec6ea92c2b01e232c69539450c2f6ae0e4b31ccbad0f3a9678a4fc126b9fc0-filelists.sqlite.bz2
--rw-r--r--   0 hlin       (501) wheel        (0)     1884 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/repo/repodata/ca15f74c9060791c17a93315bc8d2df4fd6a5d3e7c8eace70d82d023562a669e-primary.xml.gz
--rw-r--r--   0 hlin       (501) wheel        (0)     3533 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/repo/repodata/repomd.xml
--rw-r--r--   0 hlin       (501) wheel        (0)    18340 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/test_auth.py
--rw-r--r--   0 hlin       (501) wheel        (0)    60109 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/test_backend.py
--rw-r--r--   0 hlin       (501) wheel        (0)     2118 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/test_backend_thread.py
--rw-r--r--   0 hlin       (501) wheel        (0)     8244 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/test_cache.py
--rw-r--r--   0 hlin       (501) wheel        (0)    12703 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/test_celery_tasks.py
--rw-r--r--   0 hlin       (501) wheel        (0)    20302 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/test_composerthread.py
--rw-r--r--   0 hlin       (501) wheel        (0)     5411 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/test_events.py
--rw-r--r--   0 hlin       (501) wheel        (0)     5362 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/test_metrics.py
--rw-r--r--   0 hlin       (501) wheel        (0)     8849 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/test_mock_runroot.py
--rw-r--r--   0 hlin       (501) wheel        (0)    12806 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/test_models.py
--rw-r--r--   0 hlin       (501) wheel        (0)    11052 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/test_pulp.py
--rw-r--r--   0 hlin       (501) wheel        (0)    38544 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/test_pungi.py
--rw-r--r--   0 hlin       (501) wheel        (0)     4667 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/test_pungi_compose.py
--rw-r--r--   0 hlin       (501) wheel        (0)    12068 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/test_remove_expired_composes_thread.py
--rw-r--r--   0 hlin       (501) wheel        (0)     2985 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/test_utils.py
--rw-r--r--   0 hlin       (501) wheel        (0)    86954 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/test_views.py
--rw-r--r--   0 hlin       (501) wheel        (0)     4108 2023-03-01 02:01:26.000000 odcs-0.5.0/server/tests/utils.py
--rw-r--r--   0 hlin       (501) wheel        (0)       38 2023-03-01 02:11:13.012550 odcs-0.5.0/setup.cfg
--rw-r--r--   0 hlin       (501) wheel        (0)     3174 2023-03-01 02:01:26.000000 odcs-0.5.0/setup.py
--rw-r--r--   0 hlin       (501) wheel        (0)       47 2023-03-01 02:01:26.000000 odcs-0.5.0/test-requirements.txt
+drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/
+drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/client/
+drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/client/contrib/
+-rwxrwxr-x   0 hlin      (1000) hlin      (1000)    17671 2023-05-19 17:04:03.000000 odcs-0.6.0/client/contrib/odcs
+drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/client/odcs/
+drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/client/odcs/client/
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      155 2023-05-19 17:04:03.000000 odcs-0.6.0/client/odcs/client/__init__.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    25947 2023-05-19 17:04:03.000000 odcs-0.6.0/client/odcs/client/odcs.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)       65 2023-05-19 17:04:03.000000 odcs-0.6.0/client/odcs/__init__.py
+drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/client/tests/
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    23924 2023-05-19 17:04:03.000000 odcs-0.6.0/client/tests/test_client_odcs.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)       40 2023-05-19 17:04:03.000000 odcs-0.6.0/client/requirements.txt
+drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/common/
+drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/common/odcs/
+drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/common/odcs/common/
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:04:03.000000 odcs-0.6.0/common/odcs/common/__init__.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     3957 2023-05-19 17:04:03.000000 odcs-0.6.0/common/odcs/common/types.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)       65 2023-05-19 17:04:03.000000 odcs-0.6.0/common/odcs/__init__.py
+drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/docs/
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     1608 2023-05-19 17:04:03.000000 odcs-0.6.0/docs/about.rst
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    14670 2023-05-19 17:04:03.000000 odcs-0.6.0/docs/api.rst
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     3031 2023-05-19 17:04:03.000000 odcs-0.6.0/docs/client.rst
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      641 2023-05-19 17:04:03.000000 odcs-0.6.0/docs/index.rst
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      125 2023-05-19 17:04:03.000000 odcs-0.6.0/docs/module.rst
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     2429 2023-05-19 17:04:03.000000 odcs-0.6.0/docs/pulp.rst
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     8447 2023-05-19 17:04:03.000000 odcs-0.6.0/docs/raw_config.rst
+drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/odcs.egg-info/
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    23029 2023-05-19 17:05:05.000000 odcs-0.6.0/odcs.egg-info/PKG-INFO
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     5496 2023-05-19 17:05:05.000000 odcs-0.6.0/odcs.egg-info/SOURCES.txt
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)        1 2023-05-19 17:05:05.000000 odcs-0.6.0/odcs.egg-info/dependency_links.txt
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      254 2023-05-19 17:05:05.000000 odcs-0.6.0/odcs.egg-info/entry_points.txt
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)        1 2023-05-19 17:04:53.000000 odcs-0.6.0/odcs.egg-info/not-zip-safe
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      686 2023-05-19 17:05:05.000000 odcs-0.6.0/odcs.egg-info/requires.txt
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)        5 2023-05-19 17:05:05.000000 odcs-0.6.0/odcs.egg-info/top_level.txt
+drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/
+drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/conf/
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)       96 2023-05-19 17:04:03.000000 odcs-0.6.0/server/conf/__init__.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     8515 2023-05-19 17:04:03.000000 odcs-0.6.0/server/conf/config.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      258 2023-05-19 17:04:03.000000 odcs-0.6.0/server/conf/odcs-httpd-krb.conf
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      632 2023-05-19 17:04:03.000000 odcs-0.6.0/server/conf/odcs-httpd-openidc.conf
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     3586 2023-05-19 17:04:03.000000 odcs-0.6.0/server/conf/pungi.conf
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      277 2023-05-19 17:04:03.000000 odcs-0.6.0/server/conf/raw_config_urls.conf
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)       77 2023-05-19 17:04:03.000000 odcs-0.6.0/server/conf/raw_config_wrapper.conf
+drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/contrib/
+-rwxrwxr-x   0 hlin      (1000) hlin      (1000)    12884 2023-05-19 17:04:03.000000 odcs-0.6.0/server/contrib/odcs-promote-compose
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      140 2023-05-19 17:04:03.000000 odcs-0.6.0/server/contrib/odcs.wsgi
+-rwxrwxr-x   0 hlin      (1000) hlin      (1000)    13660 2023-05-19 17:04:03.000000 odcs-0.6.0/server/contrib/odcs_test_deployment
+drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/odcs/
+drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/odcs/server/
+drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/odcs/server/migrations/
+drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/odcs/server/migrations/versions/
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      661 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/0571a5ca58a0_add_index_to_compose_state.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      776 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/0d4d8e1cfe29_create_user_model.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      461 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/11b350234051_.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      917 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/16e08da18b49_add_compose_base_module_stream_version.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      711 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/3b92820da295_add_index_to_compose_time_to_expire.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      420 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/4514febd31fa_add_builds.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      648 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/512890e6864d_add_compose_scratch_modules.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     1440 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/566733ac3811_.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      872 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/59baece89746_add_compose_base_module_br_name_stream.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      480 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/7b143656694f_.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      431 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/812f2745248f_.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      466 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/82172e6a3154_.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      639 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/a855c39e2a0f_store_celery_task_id.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      437 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/a8e259e0208c_add_compose_state_reason.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      430 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/b00f3b6efaed_.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      445 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/b2725d046624_.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      421 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/b75ad2afc207_.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      423 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/c1b7e84ff39b_.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      684 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/c370b90de998_add_index_on_compose_source_type_and_.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      471 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/ca08065687c4_.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      724 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/cd0781bbdab1_.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      648 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/d1da07e15c54_.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      818 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/de0a86d7de49_.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      651 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/e186faabdafe_.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      617 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/e2163db7b15d_.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      691 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/f24a36cc8a16_add_index_on_compose_reused_id.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      633 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/versions/f4bc999818d7_add_compose_removed_by.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)       38 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/README
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      770 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/alembic.ini
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     2807 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/env.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      412 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/migrations/script.py.mako
+drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/odcs/server/static/
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/static/.gitkeep
+drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/odcs/server/templates/
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      535 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/templates/apidoc.html
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     1974 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/templates/index.html
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     3297 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/__init__.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    14727 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/api_utils.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    10896 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/auth.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    45652 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/backend.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     8931 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/cache.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    13768 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/celery_tasks.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     4706 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/comps.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    21878 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/config.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     1323 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/errors.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     2722 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/events.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     3074 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/logger.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     4593 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/manage.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    12485 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/mbs.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     7706 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/mergerepo.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     2794 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/messaging.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    12080 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/metrics.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    13271 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/mock_runroot.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    20949 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/models.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    12560 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/openapi.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     2329 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/proxy.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    12737 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/pulp.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    27479 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/pungi.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     3875 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/pungi_compose.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     6042 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/utils.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    37813 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/server/views.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)       65 2023-05-19 17:04:03.000000 odcs-0.6.0/server/odcs/__init__.py
+drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/tests/
+drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/tests/data/
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      226 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/data/custom_raw_config_wrapper.conf
+drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/tests/repo/
+drwxrwxr-x   0 hlin      (1000) hlin      (1000)        0 2023-05-19 17:05:05.000000 odcs-0.6.0/server/tests/repo/repodata/
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     4133 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/repodata/028b753de97c22923bffe2159dcb478cdfa919376e21a68a1aa6ca40fba06f45-primary.sqlite.bz2
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      750 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/repodata/1879db5a1658329be62225ebf1b40cbf8e5d522abd2fdd86157d565c83e1ddc2-modules.yaml.gz
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     1015 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/repodata/2c3a353ba9e47c3e9c8be6c2e25c50fcc11e184a727c645f3f08b66aa1a1654d-other.xml.gz
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     2722 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/repodata/635015f39babdbcdcca3a516576bdcafb57fb77be3b7919cf85363ec558fb8fe-other.sqlite.bz2
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      827 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/repodata/77e6eb5a69d53a9d56f32b3154832d4eff6e2de518c268102d2c6848cffa3e1e-filelists.xml.gz
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     2263 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/repodata/92ec6ea92c2b01e232c69539450c2f6ae0e4b31ccbad0f3a9678a4fc126b9fc0-filelists.sqlite.bz2
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     1884 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/repodata/ca15f74c9060791c17a93315bc8d2df4fd6a5d3e7c8eace70d82d023562a669e-primary.xml.gz
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     3533 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/repodata/repomd.xml
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    88568 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/ed-1.14.1-2.module_fd8ca23e.src.rpm
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    80326 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/ed-1.14.1-2.module_fd8ca23e.x86_64.rpm
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    81258 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/ed-debuginfo-1.14.1-2.module_fd8ca23e.x86_64.rpm
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     6878 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/module-build-macros-0.1-1.module_fd8ca23e.noarch.rpm
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     6970 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/repo/module-build-macros-0.1-1.module_fd8ca23e.src.rpm
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     2808 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/Jenkinsfile
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)       78 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/__init__.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     7971 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/mbs.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    18340 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_auth.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    60116 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_backend.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     8244 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_cache.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    12694 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_celery_tasks.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     5411 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_events.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     5362 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_metrics.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     8849 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_mock_runroot.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    12806 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_models.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    11052 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_pulp.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    38575 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_pungi.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     4667 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_pungi_compose.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    12008 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_remove_expired_composes_thread.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     2985 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_utils.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    86954 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/test_views.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     4108 2023-05-19 17:04:03.000000 odcs-0.6.0/server/tests/utils.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      477 2023-05-19 17:04:03.000000 odcs-0.6.0/server/requirements.txt
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)      253 2023-05-19 17:04:03.000000 odcs-0.6.0/MANIFEST.in
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    19349 2023-05-19 17:04:03.000000 odcs-0.6.0/README.md
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)     3226 2023-05-19 17:04:03.000000 odcs-0.6.0/setup.py
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)       47 2023-05-19 17:04:03.000000 odcs-0.6.0/test-requirements.txt
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)    23029 2023-05-19 17:05:05.000000 odcs-0.6.0/PKG-INFO
+-rw-rw-r--   0 hlin      (1000) hlin      (1000)       38 2023-05-19 17:05:05.000000 odcs-0.6.0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `odcs-0.5.0/PKG-INFO` & `odcs-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: odcs
-Version: 0.5.0
-Summary: On Demand Compose Service
-Home-page: https://pagure.io/odcs/
-Author: The Compose Team
-Author-email: odcs-owner@fedoraproject.org
-License: MIT
-Keywords: on demand compose service modularity fedora
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Build Tools
-Description-Content-Type: text/markdown
-Provides-Extra: client
-Provides-Extra: server
-Provides-Extra: all
-
 # On Demand Compose Service - ODCS
 
 ![logo of ODCS](https://pagure.io/odcs/raw/master/f/logo.png)
 
 ## What is ODCS
 
 The main goal of ODCS is to allow generation of temporary composes using the REST API calls. By a compose, we mainly mean RPM repository with packages taken from different sources, but in the future, generation of other output types could be possible too.
@@ -339,15 +323,15 @@
 PULP_SERVER_URL=<URL of the pulp server>
 PULP_USERNAME=<Username for the pulp server>
 PULP_PASSWORD=<Credentials for the pulp server>
 RAW_CONFIG_URLS=<Raw config settings in JSON format>
 
 # ODCS CONFIGURATION
 ODCS_CONFIG_SECTION=DevConfiguration
-ODCS_CONFIG_FILE=/src/server/conf/config.py
+ODCS_CONFIG_DIR=/src/server/conf/
 ODCS_CELERY_BROKER_URL=amqp://guest:guest@rabbitmq:5672/
 ODCS_DB_URL=postgresql+psycopg2://odcs:password@postgres/odcs
 # Directory where the generated composes are stored. This hast to match
 # location where odcs-composes volume is mounted in frontend and backend
 # containers.
 ODCS_TARGET_DIR=/mnt/odcs
 TARGET_DIR_URL=http://localhost:8080
```

### Comparing `odcs-0.5.0/README.md` & `odcs-0.6.0/odcs.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,398 +1,415 @@
-# On Demand Compose Service - ODCS
-
-![logo of ODCS](https://pagure.io/odcs/raw/master/f/logo.png)
-
-## What is ODCS
-
-The main goal of ODCS is to allow generation of temporary composes using the REST API calls. By a compose, we mainly mean RPM repository with packages taken from different sources, but in the future, generation of other output types could be possible too.
-
-ODCS can take RPMs for a compose from multiple sources like Koji tag, module built in Koji or external repository provided by Pulp tool.
-
-## Using ODCS - client library
-
-There is client library written in Python which allows easy access to REST API provided by ODCS server.
-
-### Installing the ODCS client
-
-On Fedora:
-
-```
-$ sudo dnf install odcs-client
-```
-
-If you want to install using `pip`, you can run following:
-
-```
-$ sudo pip install odcs[client]
-```
-
-In case you want your python project to depend on ODCS client library and add it to your `requirements.txt`, you can just use following to depend on ODCS client:
-
-```
-odcs[client]
-```
-
-### ODCS authentication system
-
-ODCS server can be configured to authenticate using OpenIDC, Kerberos or SSL. Eventually it can be set in NoAuth mode to support anonymous access. Depending on the ODCS server configuration, you have to set your authentication method when creating ODCS class instance.
-
-#### Using OpenIDC for authentication
-
-To use OpenIDC, you have to provide the OpenIDC token to ODCS client class constructor. To obtain that OpenIDC token, you can either use `python-openidc-client`, or ask the OpenIDC provider for service token which does not have to be refreshed. Once you have the token, you can create the ODCS instance like this:
-
-```
-from odcs.client.odcs import ODCS, AuthMech
-
-odcs = ODCS("https://odcs.fedoraproject.org",
-            auth_mech=AuthMech.OpenIDC,
-            openidc_token="your_openidc_token")
-```
-
-Getting the `openidc_token` using `python-openidc-client` library can be done like this:
-
-```
-import openidc_client
-staging = False
-
-if staging:
-    id_provider = 'https://id.stg.fedoraproject.org/openidc/'
-else:
-    id_provider = 'https://id.fedoraproject.org/openidc/'
-
-# Get the auth token using the OpenID client.
-oidc = openidc_client.OpenIDCClient(
-    'odcs',
-    id_provider,
-    {'Token': 'Token', 'Authorization': 'Authorization'},
-    'odcs-authorizer',
-    'notsecret',
-)
-
-scopes = [
-    'openid',
-    'https://id.fedoraproject.org/scope/groups',
-    'https://pagure.io/odcs/new-compose',
-    'https://pagure.io/odcs/renew-compose',
-    'https://pagure.io/odcs/delete-compose',
-]
-try:
-    token = oidc.get_token(scopes, new_token=True)
-    token = oidc.report_token_issue()
-except requests.exceptions.HTTPError as e:
-    print(e.response.text)
-    raise
-```
-
-#### Using Kerberos for authentication
-
-To use Kerberos, you have to have valid Kerberos ticket or you need to have the Kerberos keytab file. If you want to use ODCS client library with Kerberos keytab, you have to set the `KRB5_CLIENT_KTNAME` environment variable to full path to the keytab file you want to use. You can for example do it like this:
-
-```
-from odcs.client.odcs import ODCS, AuthMech
-from os import environ
-environ["KRB5_CLIENT_KTNAME"] = "/full/path/to/ketab"
-
-odcs = ODCS("https://odcs.fedoraproject.org",
-            auth_mech=AuthMech.Kerberos)
-```
-
-#### Using SSL for authentication
-
-To use SSL, you have to have SSL client certificate and key files. You then have to choose SSL AuthMech and pass the paths to SSL client certificate and key like this:
-
-```
-from odcs.client.odcs import ODCS, AuthMech
-
-odcs = ODCS("https://odcs.fedoraproject.org",
-            auth_mech=AuthMech.SSL,
-            ssl_cert="/path/to/ssl-crt.pem",
-            ssl_key="/path/to/ssl-key.pem")
-```
-
-### Requesting new compose
-
-The general way how to request new ODCS compose is following:
-
-```
-compose = odcs.new_compose(sources, source_type)
-```
-
-Both `sources` and `source_type` are strings. Depending on `source_type` value, the `sources` have following meaning:
-
-| `source_type` | `source` |
-|---------------|----------|
-| tag           | Name of Koji tag to take RPMs from. |
-| module        | White-space separated NAME:STREAM or NAME:STREAM:VERSION of modules to include in compose. |
-| pulp          | White-space separated list of content-sets or repository ids. Repositories will be included in a compose. |
-| raw_config    | String in `name#commit` hash format. The `name` must match one of the raw config locations defined in ODCS server config as `raw_config_urls`. The `commit` is commit hash defining the version of raw config to use. This config is then used as input config for Pungi. |
-| build         | Source should be omitted in the request. The list of Koji builds included in a compose is defined by `builds` attribute. |
-| pungi_compose | URL to variant repository of external compose generated by the Pungi. For example https://kojipkgs.fedoraproject.org/compose/rawhide/latest-Fedora-Rawhide/compose/Server/. The generated compose will contain the same set of RPMs as the given external compose variant. The packages will be taken from the configured Koji instance. |
-
-There are also additional optional attributes you can pass to `new_compose(...)` method:
-
-- `seconds_to_live` - Number of seconds after which the generated compose should expire and will be removed.
-- `packages` - List of packages which should be included in a compose. This is used only when `source_type` is set to `tag` or `build` to further limit the compose repository.
-If the `packages` is not set, all packages in Koji tag or all packages in a `builds` list will be included in a final compose.
-- `flags` - List of flags to further modify the compose output:
-    - `no_deps` - For `tag` `source_type`, do not resolve dependencies between packages and include only packages listed in the `packages` in the compose. For `module` `source_type`, do not resolve dependencies between modules and include only the requested module in the compose.
-    - `include_unpublished_pulp_repos` - For `pulp` `source_type`, include also unpublished repositories for input content-sets.
-    - `check_deps` - When set, abort the compose when some package has broken dependencies.
-    - `no_reuse` - When set, do not try to reuse old compose.
-    - `ignore_absent_pulp_repos` - For `pulp` `source_type`, ignore any content set that does not exist in Pulp
-    - `use_only_compatible_arch` - For `pulp` `source_type` only. When this flag is set, architecture hardcoded in URL returned from Pulp will be replaced with `$basearch` variable. The repository definition will also define `skip_if_unavailable = 1`. This could be useful when multiple content sets are included in the repofile to completly ignore packages from repositories for incompatible architectures.
-- `sigkeys` - List of signature keys IDs. Only packages signed by one of these keys will be included in a compose. If there is no signed version of a package, compose will fail. It is also possible to pass an empty-string in a list meaning unsigned packages are allowed. For example if you want to prefer packages signed by key with ID `123` and also allow unsigned packages to appear in a compose, you can do it by setting sigkeys to `["123", ""]`.
-- `results` - List of additional results which will be generated as part of a compose. Valid keys are:
-    - `iso` - Generates non-installable ISO files with RPMs from a compose.
-    - `boot.iso` - Generates `images/boot.iso` file which is needed to build base container images from resulting compose.
-- `arches` - List of additional Koji arches to build this compose for. By default, the compose is built only for "x86_64" arch.
-- `multilib_arches` - Subset of `arches` for which the multilib should be enabled. For each architecture in the `multilib_arches` list, ODCS will include also packages from other compatible architectures in a compose. For example when "x86_64" is included `multilib_arches`, ODCS will include also "i686" packages in a compose. The set of packages included in a composes is influenced by `multilib_method` list.
-- `multilib_method` - List defining the method used to determine whether consider package as multilib. Defaults to empty list. The list can have following values:
-    - `iso` - Generates non-installable ISO files with RPMs from a compose.
-    - `runtime` - Packages whose name ends with "-devel" or "-static" suffix will be considered as multilib.
-    - `devel` - Packages that install some shared object file "*.so.*" will be considered as multilib.
-    - `all` - All pakages will be considered as multilib.
-- `builds` - List of NVRs defining the Koji builds to include in a compose. Only valid for `tag` and `build` source types. For `tag` source type, the NVRs will be considered
-for inclusion in a compose on top of Koji tag defined by `source`. For `build` source type, only the Koji builds defined by the NVRs will be considered for inclusion. The `packages` still need to be set to include particular packages from the Koji builds in a compose.
-- `lookaside_repos` - List of URLs pointing to RPM repositories with packages which will be used by internal dependency resolver to resolve dependencies. Packages from these repositories will not appear in the resulting ODCS compose, but they are considered while checking whether the RPM dependencies are satisfied in the resulting compose when `check_deps` ODCS flag.
-- `module_defaults_url` - List with URL to git repository with Module defaults data and the branch name or commit hash. For example ["https://pagure.io/releng/fedora-module-defaults.git", "master"]. This is used only when creating modular compose including non-modular RPMs.
-- `modular_koji_tags` - List of Koji tags in which the modular Koji Content Generator builds are tagged. Such builds will be included in a compose.
-
-The `new_compose` method returns `dict` object describing the compose, for example:
-
-```
-{
-    "arches": "x86_64 ppc64",
-    "flags": [
-        "no_deps"
-    ],
-    "id": 1,
-    "owner": "jkaluza",
-    "packages": "gofer-package",
-    "removed_by": null,
-    "result_repo": "https://odcs.fedoraproject.org/composes/latest-odcs-1-1/compose/Temporary",
-    "result_repofile": "https://odcs.fedoraproject.org/composes/latest-odcs-1-1/compose/Temporary/odcs-1.repo",
-    "results": [
-        "repository"
-    ],
-    "sigkeys": "",
-    "source": "f26",
-    "source_type": 1,
-    "state": 3,
-    "state_name": "wait",
-    "time_done": "2017-10-13T17:03:13Z",
-    "time_removed": "2017-10-14T17:00:00Z",
-    "time_submitted": "2017-10-13T16:59:51Z",
-    "time_to_expire": "2017-10-14T16:59:51Z"
-}
-```
-
-The most useful data there is `result_repofile`, which points to the .repo file with URLs for generated compose. Another very important data there is the `state` and `state_name` field. There are following states of a compose:
-
-| `state` | `state_name` | Description |
-|---------|--------------|-------------|
-| 0       | wait         | Compose is waiting in a queue to be generated |
-| 1       | generating   | Compose is being generated |
-| 2       | done         | Compose is generated - done |
-| 3       | removed      | Compose has expired and is removed |
-| 4       | failed       | Compose generation has failed |
-
-As you can see in our example, compose is in `wait` state and therefore we have to wait until the ODCS generates the compose.
-
-### Waiting until the compose is generated
-
-There are two ways how to wait for the compose generation. The preferred one is listening on Fedora messaging bus for `odcs.state.change` message with `done` or `failed` state and another one is using HTTP polling implemented in `wait_for_compose(...)` method.
-
-If your application does not allow listening on the bus for some reason, you can use `wait_for_compose(...)` method like this:
-
-```
-compose = odcs.new_compose(sources, source_type)
-
-# Blocks until the compose is ready, but maximally for 600 seconds.
-compose = odcs.wait_for_compose(compose["id"], timeout=600)
-
-if compose["state_name"] == "done":
-    print "Compose done, URL with repo file", compose["result_repofile"]
-else:
-    print "Failed to generate compose"
-```
-
-### Checking the state of existing ODCS compose
-
-Once you have the compose ready, you might want to check its state later. This can be done using the `get_compose(...)` method like this:
-
-```
-compose = odcs.get_compose(compose["id"])
-```
-
-### Renewing the compose
-
-If the `time_to_expire` for your compose is getting closer and you know you want to continue using the compose, you can increase the `time_to_expire` using the `renew_compose(...)` method. You can also use this method to regenerate an expired compose in the `removed` state. Such compose will have the same versions of packages as the original compose.
-
-```
-compose = odcs.renew_compose(compose["id"])
-```
-
-## Development
-
-### Code Convention
-
-The code must be well formatted via ``black`` and pass ``flake8`` checking.
-
-Run ``tox -e black,flake8`` to do the check.
-
-### Unit-testing
-
-Install packages required by pip to compile some python packages:
-
-```
-$ sudo dnf install -y gcc swig redhat-rpm-config python-devel openssl-devel openldap-devel \
-    zlib-devel bzip2 bzip2-devel readline-devel sqlite sqlite-devel tk-devel \
-    git python3-cairo-devel cairo-gobject-devel gobject-introspection-devel
-```
-
-A lot of these dependencies come from the module
-[pygobject](https://pygobject.readthedocs.io/en/latest/devguide/dev_environ.html#fedora-dep).
-
-Run the tests:
-
-```
-$ make check
-```
-
-### Testing local composes from plain RPM repositories
-
-You can test ODCS by generating compose from the `./server/tests/repo` repository using following commands:
-
-```
-$ ./create_sqlite_db
-$ ./start_odcs_from_here
-```
-
-Before executing the command `start_odcs_from_here`, a messaging broker supporting AMQP protocol is required to run locally as well in order to run asynchronous tasks to generate composes. Here is an example to run a RabbitMQ broker:
-
-```
-sudo dnf install -y rabbitmq-server
-sudo systemctl start rabbitmq-server
-```
-
-Add the `repo` source type to the server configuration in `./server/odcs/server/config.py`. (This will cause some tests to fail, so it needs to be reverted back after you are done with your changes!)
-
-And in another terminal, submit a request to frontend:
-
-```
-$ ./submit_test_compose repo `pwd`/server/tests/repo ed
-{
-  "id": 1,
-  "owner": "Unknown",
-  "result_repo": null,
-  "source": "/home/hanzz/code/fedora-modularization/odcs/tests/repo",
-  "source_type": 3,
-  "state": 0,
-  "state_name": "wait",
-  "time_done": null,
-  "time_removed": null,
-  "time_submitted": "2017-06-12T14:18:19Z"
-}
-```
-
-You should then see the backend process generating the compose and once it's done, the resulting compose in `./test_composes/latest-Unknown-1/compose/Temporary` directory.
-
-### Using docker-compose for creating a local setup
-
-You can create test setup for ODCS with the docker-compose file. This yaml file creates docker container for the backend and frontend setup of ODCS and run multiple services together. These services are;
-
-* **rabbitmq** (Handles the communication between backend and frontend)
-* **postgres** (Creates the database where the localy generated composes are stored)
-* **backend** (Backend service of ODCS)
-* **frontend** (Frontend service of ODCS that handles the REST API)
-* **static** (Apache service for making storage available)
-* **beat** (Cronjob for backend to check the service status)
-
-In addition to these, there are also three docker volumes (`odcs_odcs-composes`, `odcs_odcs-postgres` and `odcs_rabbitmq`) are created. These are providing persistent storage for the services.
-
-This yaml file requires also an **.env** file that specified some enviroment variables for the configuration of frontend and backend. Such an **.env** file should be in the same path with the **docker-compose.yml** file and here are the necessary variables that need to be specified in this file;
-```
-# Pyhton path
-PYTHONPATH=/src/common:/src/server:/src/client
-
-# POSTGRES
-POSTGRES_USER=odcs
-POSTGRES_PASSWORD=password
-
-# PULP CONFIGURATION
-PULP_SERVER_URL=<URL of the pulp server>
-PULP_USERNAME=<Username for the pulp server>
-PULP_PASSWORD=<Credentials for the pulp server>
-RAW_CONFIG_URLS=<Raw config settings in JSON format>
-
-# ODCS CONFIGURATION
-ODCS_CONFIG_SECTION=DevConfiguration
-ODCS_CONFIG_FILE=/src/server/conf/config.py
-ODCS_CELERY_BROKER_URL=amqp://guest:guest@rabbitmq:5672/
-ODCS_DB_URL=postgresql+psycopg2://odcs:password@postgres/odcs
-# Directory where the generated composes are stored. This hast to match
-# location where odcs-composes volume is mounted in frontend and backend
-# containers.
-ODCS_TARGET_DIR=/mnt/odcs
-TARGET_DIR_URL=http://localhost:8080
-
-# FLASK SETTINGS
-# Force flask to reload application on change of source files.
-FLASK_ENV=development
-```
-
-The services can be start with `sudo docker-compose up` command. If you have face an error or something that does not work correctly please use the following steps;
-
-1. Check whether there is already created docker volume.
-
-
-        $ sudo docker volume ls
-        Emulate Docker CLI using podman. Create /etc/containers/nodocker to quiet msg.
-        DRIVER      VOLUME NAME
-
-
-    If the output is like above, it means there isn't any volume yet and it is sufficient to run `sudo docker-compose up` and then `sudo docker-compose down` command. This creates the volumes and if you run the above command again the output becomes as follows;
-
-
-        $ sudo docker volume ls
-        Emulate Docker CLI using podman. Create /etc/containers/nodocker to quiet msg.
-        DRIVER      VOLUME NAME
-        local       odcs_odcs-composes
-        local       odcs_odcs-postgres
-        local       odcs_odcs-rabbitmq
-
-
-2. After this point we need to set the correct permission to `ocds_odcs-composes` volume. In order to find where is the actual location of the volume type the following
-
-
-        $ sudo docker volume inspect odcs_odcs-composes
-        Emulate Docker CLI using podman. Create /etc/containers/nodocker to quiet msg.
-        [
-            {
-                "Name": "odcs_odcs-composes",
-                "Driver": "local",
-                "Mountpoint": "/var/lib/containers/storage/volumes/odcs_odcs-composes/_data",
-                "CreatedAt": "2021-10-04T13:19:36.478636851+02:00",
-                "Labels": {
-                    "io.podman.compose.project": "odcs"
-                },
-                "Scope": "local",
-                "Options": {}
-            }
+Metadata-Version: 2.1
+Name: odcs
+Version: 0.6.0
+Summary: On Demand Compose Service
+Home-page: https://pagure.io/odcs/
+Author: The Compose Team
+Author-email: odcs-owner@fedoraproject.org
+License: MIT
+Description: # On Demand Compose Service - ODCS
+        
+        ![logo of ODCS](https://pagure.io/odcs/raw/master/f/logo.png)
+        
+        ## What is ODCS
+        
+        The main goal of ODCS is to allow generation of temporary composes using the REST API calls. By a compose, we mainly mean RPM repository with packages taken from different sources, but in the future, generation of other output types could be possible too.
+        
+        ODCS can take RPMs for a compose from multiple sources like Koji tag, module built in Koji or external repository provided by Pulp tool.
+        
+        ## Using ODCS - client library
+        
+        There is client library written in Python which allows easy access to REST API provided by ODCS server.
+        
+        ### Installing the ODCS client
+        
+        On Fedora:
+        
+        ```
+        $ sudo dnf install odcs-client
+        ```
+        
+        If you want to install using `pip`, you can run following:
+        
+        ```
+        $ sudo pip install odcs[client]
+        ```
+        
+        In case you want your python project to depend on ODCS client library and add it to your `requirements.txt`, you can just use following to depend on ODCS client:
+        
+        ```
+        odcs[client]
+        ```
+        
+        ### ODCS authentication system
+        
+        ODCS server can be configured to authenticate using OpenIDC, Kerberos or SSL. Eventually it can be set in NoAuth mode to support anonymous access. Depending on the ODCS server configuration, you have to set your authentication method when creating ODCS class instance.
+        
+        #### Using OpenIDC for authentication
+        
+        To use OpenIDC, you have to provide the OpenIDC token to ODCS client class constructor. To obtain that OpenIDC token, you can either use `python-openidc-client`, or ask the OpenIDC provider for service token which does not have to be refreshed. Once you have the token, you can create the ODCS instance like this:
+        
+        ```
+        from odcs.client.odcs import ODCS, AuthMech
+        
+        odcs = ODCS("https://odcs.fedoraproject.org",
+                    auth_mech=AuthMech.OpenIDC,
+                    openidc_token="your_openidc_token")
+        ```
+        
+        Getting the `openidc_token` using `python-openidc-client` library can be done like this:
+        
+        ```
+        import openidc_client
+        staging = False
+        
+        if staging:
+            id_provider = 'https://id.stg.fedoraproject.org/openidc/'
+        else:
+            id_provider = 'https://id.fedoraproject.org/openidc/'
+        
+        # Get the auth token using the OpenID client.
+        oidc = openidc_client.OpenIDCClient(
+            'odcs',
+            id_provider,
+            {'Token': 'Token', 'Authorization': 'Authorization'},
+            'odcs-authorizer',
+            'notsecret',
+        )
+        
+        scopes = [
+            'openid',
+            'https://id.fedoraproject.org/scope/groups',
+            'https://pagure.io/odcs/new-compose',
+            'https://pagure.io/odcs/renew-compose',
+            'https://pagure.io/odcs/delete-compose',
         ]
-
-    `"Mountpoint": "/var/lib/containers/storage/volumes/odcs_odcs-composes/_data"` shows the exact location of the corresponding volume.
-
-    Add group write permission to the Mountpoint by
-
-
-        $ sudo chmod 775 /var/lib/containers/storage/volumes/odcs_odcs-composes/_data
-
-
-3. In this step it is sufficient to run `sudo docker-compose up` command to start the services properly.
-
-Here are some REST calls for checking the ODCS.
-
-* `$ curl -s http://localhost:5000/api/1/composes/ | jq .` This call shows all the composes in db.
-* `$ odcs --server http://localhost:5000/ create-pulp <Pulp content set>` This call starts a pulp compose that match the given pulp content set
-* `$ odcs --server http://localhost:5000/ create-raw-config --compose-type test my_raw_config master` This call starts a compose with the configuration defined as my_raw_config
+        try:
+            token = oidc.get_token(scopes, new_token=True)
+            token = oidc.report_token_issue()
+        except requests.exceptions.HTTPError as e:
+            print(e.response.text)
+            raise
+        ```
+        
+        #### Using Kerberos for authentication
+        
+        To use Kerberos, you have to have valid Kerberos ticket or you need to have the Kerberos keytab file. If you want to use ODCS client library with Kerberos keytab, you have to set the `KRB5_CLIENT_KTNAME` environment variable to full path to the keytab file you want to use. You can for example do it like this:
+        
+        ```
+        from odcs.client.odcs import ODCS, AuthMech
+        from os import environ
+        environ["KRB5_CLIENT_KTNAME"] = "/full/path/to/ketab"
+        
+        odcs = ODCS("https://odcs.fedoraproject.org",
+                    auth_mech=AuthMech.Kerberos)
+        ```
+        
+        #### Using SSL for authentication
+        
+        To use SSL, you have to have SSL client certificate and key files. You then have to choose SSL AuthMech and pass the paths to SSL client certificate and key like this:
+        
+        ```
+        from odcs.client.odcs import ODCS, AuthMech
+        
+        odcs = ODCS("https://odcs.fedoraproject.org",
+                    auth_mech=AuthMech.SSL,
+                    ssl_cert="/path/to/ssl-crt.pem",
+                    ssl_key="/path/to/ssl-key.pem")
+        ```
+        
+        ### Requesting new compose
+        
+        The general way how to request new ODCS compose is following:
+        
+        ```
+        compose = odcs.new_compose(sources, source_type)
+        ```
+        
+        Both `sources` and `source_type` are strings. Depending on `source_type` value, the `sources` have following meaning:
+        
+        | `source_type` | `source` |
+        |---------------|----------|
+        | tag           | Name of Koji tag to take RPMs from. |
+        | module        | White-space separated NAME:STREAM or NAME:STREAM:VERSION of modules to include in compose. |
+        | pulp          | White-space separated list of content-sets or repository ids. Repositories will be included in a compose. |
+        | raw_config    | String in `name#commit` hash format. The `name` must match one of the raw config locations defined in ODCS server config as `raw_config_urls`. The `commit` is commit hash defining the version of raw config to use. This config is then used as input config for Pungi. |
+        | build         | Source should be omitted in the request. The list of Koji builds included in a compose is defined by `builds` attribute. |
+        | pungi_compose | URL to variant repository of external compose generated by the Pungi. For example https://kojipkgs.fedoraproject.org/compose/rawhide/latest-Fedora-Rawhide/compose/Server/. The generated compose will contain the same set of RPMs as the given external compose variant. The packages will be taken from the configured Koji instance. |
+        
+        There are also additional optional attributes you can pass to `new_compose(...)` method:
+        
+        - `seconds_to_live` - Number of seconds after which the generated compose should expire and will be removed.
+        - `packages` - List of packages which should be included in a compose. This is used only when `source_type` is set to `tag` or `build` to further limit the compose repository.
+        If the `packages` is not set, all packages in Koji tag or all packages in a `builds` list will be included in a final compose.
+        - `flags` - List of flags to further modify the compose output:
+            - `no_deps` - For `tag` `source_type`, do not resolve dependencies between packages and include only packages listed in the `packages` in the compose. For `module` `source_type`, do not resolve dependencies between modules and include only the requested module in the compose.
+            - `include_unpublished_pulp_repos` - For `pulp` `source_type`, include also unpublished repositories for input content-sets.
+            - `check_deps` - When set, abort the compose when some package has broken dependencies.
+            - `no_reuse` - When set, do not try to reuse old compose.
+            - `ignore_absent_pulp_repos` - For `pulp` `source_type`, ignore any content set that does not exist in Pulp
+            - `use_only_compatible_arch` - For `pulp` `source_type` only. When this flag is set, architecture hardcoded in URL returned from Pulp will be replaced with `$basearch` variable. The repository definition will also define `skip_if_unavailable = 1`. This could be useful when multiple content sets are included in the repofile to completly ignore packages from repositories for incompatible architectures.
+        - `sigkeys` - List of signature keys IDs. Only packages signed by one of these keys will be included in a compose. If there is no signed version of a package, compose will fail. It is also possible to pass an empty-string in a list meaning unsigned packages are allowed. For example if you want to prefer packages signed by key with ID `123` and also allow unsigned packages to appear in a compose, you can do it by setting sigkeys to `["123", ""]`.
+        - `results` - List of additional results which will be generated as part of a compose. Valid keys are:
+            - `iso` - Generates non-installable ISO files with RPMs from a compose.
+            - `boot.iso` - Generates `images/boot.iso` file which is needed to build base container images from resulting compose.
+        - `arches` - List of additional Koji arches to build this compose for. By default, the compose is built only for "x86_64" arch.
+        - `multilib_arches` - Subset of `arches` for which the multilib should be enabled. For each architecture in the `multilib_arches` list, ODCS will include also packages from other compatible architectures in a compose. For example when "x86_64" is included `multilib_arches`, ODCS will include also "i686" packages in a compose. The set of packages included in a composes is influenced by `multilib_method` list.
+        - `multilib_method` - List defining the method used to determine whether consider package as multilib. Defaults to empty list. The list can have following values:
+            - `iso` - Generates non-installable ISO files with RPMs from a compose.
+            - `runtime` - Packages whose name ends with "-devel" or "-static" suffix will be considered as multilib.
+            - `devel` - Packages that install some shared object file "*.so.*" will be considered as multilib.
+            - `all` - All pakages will be considered as multilib.
+        - `builds` - List of NVRs defining the Koji builds to include in a compose. Only valid for `tag` and `build` source types. For `tag` source type, the NVRs will be considered
+        for inclusion in a compose on top of Koji tag defined by `source`. For `build` source type, only the Koji builds defined by the NVRs will be considered for inclusion. The `packages` still need to be set to include particular packages from the Koji builds in a compose.
+        - `lookaside_repos` - List of URLs pointing to RPM repositories with packages which will be used by internal dependency resolver to resolve dependencies. Packages from these repositories will not appear in the resulting ODCS compose, but they are considered while checking whether the RPM dependencies are satisfied in the resulting compose when `check_deps` ODCS flag.
+        - `module_defaults_url` - List with URL to git repository with Module defaults data and the branch name or commit hash. For example ["https://pagure.io/releng/fedora-module-defaults.git", "master"]. This is used only when creating modular compose including non-modular RPMs.
+        - `modular_koji_tags` - List of Koji tags in which the modular Koji Content Generator builds are tagged. Such builds will be included in a compose.
+        
+        The `new_compose` method returns `dict` object describing the compose, for example:
+        
+        ```
+        {
+            "arches": "x86_64 ppc64",
+            "flags": [
+                "no_deps"
+            ],
+            "id": 1,
+            "owner": "jkaluza",
+            "packages": "gofer-package",
+            "removed_by": null,
+            "result_repo": "https://odcs.fedoraproject.org/composes/latest-odcs-1-1/compose/Temporary",
+            "result_repofile": "https://odcs.fedoraproject.org/composes/latest-odcs-1-1/compose/Temporary/odcs-1.repo",
+            "results": [
+                "repository"
+            ],
+            "sigkeys": "",
+            "source": "f26",
+            "source_type": 1,
+            "state": 3,
+            "state_name": "wait",
+            "time_done": "2017-10-13T17:03:13Z",
+            "time_removed": "2017-10-14T17:00:00Z",
+            "time_submitted": "2017-10-13T16:59:51Z",
+            "time_to_expire": "2017-10-14T16:59:51Z"
+        }
+        ```
+        
+        The most useful data there is `result_repofile`, which points to the .repo file with URLs for generated compose. Another very important data there is the `state` and `state_name` field. There are following states of a compose:
+        
+        | `state` | `state_name` | Description |
+        |---------|--------------|-------------|
+        | 0       | wait         | Compose is waiting in a queue to be generated |
+        | 1       | generating   | Compose is being generated |
+        | 2       | done         | Compose is generated - done |
+        | 3       | removed      | Compose has expired and is removed |
+        | 4       | failed       | Compose generation has failed |
+        
+        As you can see in our example, compose is in `wait` state and therefore we have to wait until the ODCS generates the compose.
+        
+        ### Waiting until the compose is generated
+        
+        There are two ways how to wait for the compose generation. The preferred one is listening on Fedora messaging bus for `odcs.state.change` message with `done` or `failed` state and another one is using HTTP polling implemented in `wait_for_compose(...)` method.
+        
+        If your application does not allow listening on the bus for some reason, you can use `wait_for_compose(...)` method like this:
+        
+        ```
+        compose = odcs.new_compose(sources, source_type)
+        
+        # Blocks until the compose is ready, but maximally for 600 seconds.
+        compose = odcs.wait_for_compose(compose["id"], timeout=600)
+        
+        if compose["state_name"] == "done":
+            print "Compose done, URL with repo file", compose["result_repofile"]
+        else:
+            print "Failed to generate compose"
+        ```
+        
+        ### Checking the state of existing ODCS compose
+        
+        Once you have the compose ready, you might want to check its state later. This can be done using the `get_compose(...)` method like this:
+        
+        ```
+        compose = odcs.get_compose(compose["id"])
+        ```
+        
+        ### Renewing the compose
+        
+        If the `time_to_expire` for your compose is getting closer and you know you want to continue using the compose, you can increase the `time_to_expire` using the `renew_compose(...)` method. You can also use this method to regenerate an expired compose in the `removed` state. Such compose will have the same versions of packages as the original compose.
+        
+        ```
+        compose = odcs.renew_compose(compose["id"])
+        ```
+        
+        ## Development
+        
+        ### Code Convention
+        
+        The code must be well formatted via ``black`` and pass ``flake8`` checking.
+        
+        Run ``tox -e black,flake8`` to do the check.
+        
+        ### Unit-testing
+        
+        Install packages required by pip to compile some python packages:
+        
+        ```
+        $ sudo dnf install -y gcc swig redhat-rpm-config python-devel openssl-devel openldap-devel \
+            zlib-devel bzip2 bzip2-devel readline-devel sqlite sqlite-devel tk-devel \
+            git python3-cairo-devel cairo-gobject-devel gobject-introspection-devel
+        ```
+        
+        A lot of these dependencies come from the module
+        [pygobject](https://pygobject.readthedocs.io/en/latest/devguide/dev_environ.html#fedora-dep).
+        
+        Run the tests:
+        
+        ```
+        $ make check
+        ```
+        
+        ### Testing local composes from plain RPM repositories
+        
+        You can test ODCS by generating compose from the `./server/tests/repo` repository using following commands:
+        
+        ```
+        $ ./create_sqlite_db
+        $ ./start_odcs_from_here
+        ```
+        
+        Before executing the command `start_odcs_from_here`, a messaging broker supporting AMQP protocol is required to run locally as well in order to run asynchronous tasks to generate composes. Here is an example to run a RabbitMQ broker:
+        
+        ```
+        sudo dnf install -y rabbitmq-server
+        sudo systemctl start rabbitmq-server
+        ```
+        
+        Add the `repo` source type to the server configuration in `./server/odcs/server/config.py`. (This will cause some tests to fail, so it needs to be reverted back after you are done with your changes!)
+        
+        And in another terminal, submit a request to frontend:
+        
+        ```
+        $ ./submit_test_compose repo `pwd`/server/tests/repo ed
+        {
+          "id": 1,
+          "owner": "Unknown",
+          "result_repo": null,
+          "source": "/home/hanzz/code/fedora-modularization/odcs/tests/repo",
+          "source_type": 3,
+          "state": 0,
+          "state_name": "wait",
+          "time_done": null,
+          "time_removed": null,
+          "time_submitted": "2017-06-12T14:18:19Z"
+        }
+        ```
+        
+        You should then see the backend process generating the compose and once it's done, the resulting compose in `./test_composes/latest-Unknown-1/compose/Temporary` directory.
+        
+        ### Using docker-compose for creating a local setup
+        
+        You can create test setup for ODCS with the docker-compose file. This yaml file creates docker container for the backend and frontend setup of ODCS and run multiple services together. These services are;
+        
+        * **rabbitmq** (Handles the communication between backend and frontend)
+        * **postgres** (Creates the database where the localy generated composes are stored)
+        * **backend** (Backend service of ODCS)
+        * **frontend** (Frontend service of ODCS that handles the REST API)
+        * **static** (Apache service for making storage available)
+        * **beat** (Cronjob for backend to check the service status)
+        
+        In addition to these, there are also three docker volumes (`odcs_odcs-composes`, `odcs_odcs-postgres` and `odcs_rabbitmq`) are created. These are providing persistent storage for the services.
+        
+        This yaml file requires also an **.env** file that specified some enviroment variables for the configuration of frontend and backend. Such an **.env** file should be in the same path with the **docker-compose.yml** file and here are the necessary variables that need to be specified in this file;
+        ```
+        # Pyhton path
+        PYTHONPATH=/src/common:/src/server:/src/client
+        
+        # POSTGRES
+        POSTGRES_USER=odcs
+        POSTGRES_PASSWORD=password
+        
+        # PULP CONFIGURATION
+        PULP_SERVER_URL=<URL of the pulp server>
+        PULP_USERNAME=<Username for the pulp server>
+        PULP_PASSWORD=<Credentials for the pulp server>
+        RAW_CONFIG_URLS=<Raw config settings in JSON format>
+        
+        # ODCS CONFIGURATION
+        ODCS_CONFIG_SECTION=DevConfiguration
+        ODCS_CONFIG_DIR=/src/server/conf/
+        ODCS_CELERY_BROKER_URL=amqp://guest:guest@rabbitmq:5672/
+        ODCS_DB_URL=postgresql+psycopg2://odcs:password@postgres/odcs
+        # Directory where the generated composes are stored. This hast to match
+        # location where odcs-composes volume is mounted in frontend and backend
+        # containers.
+        ODCS_TARGET_DIR=/mnt/odcs
+        TARGET_DIR_URL=http://localhost:8080
+        
+        # FLASK SETTINGS
+        # Force flask to reload application on change of source files.
+        FLASK_ENV=development
+        ```
+        
+        The services can be start with `sudo docker-compose up` command. If you have face an error or something that does not work correctly please use the following steps;
+        
+        1. Check whether there is already created docker volume.
+        
+        
+                $ sudo docker volume ls
+                Emulate Docker CLI using podman. Create /etc/containers/nodocker to quiet msg.
+                DRIVER      VOLUME NAME
+        
+        
+            If the output is like above, it means there isn't any volume yet and it is sufficient to run `sudo docker-compose up` and then `sudo docker-compose down` command. This creates the volumes and if you run the above command again the output becomes as follows;
+        
+        
+                $ sudo docker volume ls
+                Emulate Docker CLI using podman. Create /etc/containers/nodocker to quiet msg.
+                DRIVER      VOLUME NAME
+                local       odcs_odcs-composes
+                local       odcs_odcs-postgres
+                local       odcs_odcs-rabbitmq
+        
+        
+        2. After this point we need to set the correct permission to `ocds_odcs-composes` volume. In order to find where is the actual location of the volume type the following
+        
+        
+                $ sudo docker volume inspect odcs_odcs-composes
+                Emulate Docker CLI using podman. Create /etc/containers/nodocker to quiet msg.
+                [
+                    {
+                        "Name": "odcs_odcs-composes",
+                        "Driver": "local",
+                        "Mountpoint": "/var/lib/containers/storage/volumes/odcs_odcs-composes/_data",
+                        "CreatedAt": "2021-10-04T13:19:36.478636851+02:00",
+                        "Labels": {
+                            "io.podman.compose.project": "odcs"
+                        },
+                        "Scope": "local",
+                        "Options": {}
+                    }
+                ]
+        
+            `"Mountpoint": "/var/lib/containers/storage/volumes/odcs_odcs-composes/_data"` shows the exact location of the corresponding volume.
+        
+            Add group write permission to the Mountpoint by
+        
+        
+                $ sudo chmod 775 /var/lib/containers/storage/volumes/odcs_odcs-composes/_data
+        
+        
+        3. In this step it is sufficient to run `sudo docker-compose up` command to start the services properly.
+        
+        Here are some REST calls for checking the ODCS.
+        
+        * `$ curl -s http://localhost:5000/api/1/composes/ | jq .` This call shows all the composes in db.
+        * `$ odcs --server http://localhost:5000/ create-pulp <Pulp content set>` This call starts a pulp compose that match the given pulp content set
+        * `$ odcs --server http://localhost:5000/ create-raw-config --compose-type test my_raw_config master` This call starts a compose with the configuration defined as my_raw_config
+        
+Keywords: on demand compose service modularity fedora
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Build Tools
+Description-Content-Type: text/markdown
+Provides-Extra: client
+Provides-Extra: server
+Provides-Extra: all
```

### Comparing `odcs-0.5.0/client/contrib/odcs` & `odcs-0.6.0/client/contrib/odcs`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,19 @@
     "--scratch-module": dict(
         default=[],
         action="append",
         metavar="scratch_modules",
         help="Scratch modules to be included in the compose with format N:S:V:C",
     ),
     "--label": dict(default=None, help="Label for raw_config compose."),
+    "--no-label": dict(
+        default=False,
+        action="store_true",
+        help="Allow raw_config compose without label.",
+    ),
     "--compose-type": dict(default=None, help="Compose type for raw_config compose."),
     "--build": dict(
         default=[], action="append", help="Builds to be included in the compose."
     ),
 }
 
 
@@ -301,14 +306,15 @@
 create_raw_config_parser.add_argument(
     "raw_config_commit", help="Commit or branch name to get raw_config from."
 )
 _add_arguments(
     create_raw_config_parser,
     "--sigkey",
     "--label",
+    "--no-label",
     "--compose-type",
     "--koji-event",
     "--target-dir",
     "--build",
 )
 
 
@@ -419,14 +425,19 @@
     request_args["flags"] = args.flag
 if getattr(args, "arch", False):
     request_args["arches"] = args.arch
 if getattr(args, "lookaside_repo", False):
     request_args["lookaside_repos"] = args.lookaside_repo
 if getattr(args, "label", False):
     request_args["label"] = args.label
+if getattr(args, "no_label", False):
+    if "flags" in request_args:
+        request_args["flags"].append("no_label")
+    else:
+        request_args["flags"] = ["no_label"]
 if getattr(args, "compose_type", False):
     request_args["compose_type"] = args.compose_type
 if getattr(args, "target_dir", False):
     request_args["target_dir"] = args.target_dir
 
 try:
     args.sigkey = [key.replace("none", "") for key in getattr(args, "sigkey", [])]
```

### Comparing `odcs-0.5.0/client/odcs/client/odcs.py` & `odcs-0.6.0/client/odcs/client/odcs.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/client/tests/test_client_odcs.py` & `odcs-0.6.0/client/tests/test_client_odcs.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/common/odcs/common/types.py` & `odcs-0.6.0/common/odcs/common/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,10 +105,12 @@
     # For "pulp" source_type, ignore any repos do not exist in the remote Pulp
     # instance.
     "ignore_absent_pulp_repos": 32,
     # Do not reuse old composes.
     "no_reuse": 64,
     # Use only compatible architectures
     "use_only_compatible_arch": 128,
+    # Allow compose without label
+    "no_label": 256,
 }
 
 INVERSE_COMPOSE_FLAGS = {v: k for k, v in COMPOSE_FLAGS.items()}
```

### Comparing `odcs-0.5.0/docs/about.rst` & `odcs-0.6.0/docs/about.rst`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/docs/api.rst` & `odcs-0.6.0/docs/api.rst`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     - *no_inheritance* - Only packages/modules directly tagged in the requested Koji tag will be added to the module. Inherited tags will be ignored.
     - *include_unpublished_pulp_repos* - Even unpublished Pulp repositories will be included in the resulting compose.
     - *ignore_absent_pulp_repos* - Ignore non-existing content sets in the source of Pulp compose. The source field on the compose will be updated to match what was actually used in the compose.
     - *check_deps* - Compose will fail if the RPM-level dependencies between packages in the compose are not satisfied.
     - *include_done_modules* - Compose can include also modules which are in the ``done`` state. By default, only modules in ``ready`` state are allowed to be included in a composes.
     - *no_reuse* - Compose will be generated directly instead of trying to reuse old one.
     - *use_only_compatible_arch* - When this flag is set, architecture hardcoded in URL returned from Pulp will be replaced with `$basearch` variable. The repository definition will also define `skip_if_unavailable = 1`. This could be useful when multiple content sets are included in the repofile to completly ignore packages from repositories for incompatible archictures.
+    - *no_label* - Allow compose without label by passing ``--no-label`` to Pungi.
 
 .. _koji_event:
 
 *koji_event* - ``(number or null)``
     The Koji event defining the point in Koji history when the compose was generated. It can be ``null`` if source type does not relate to Koji tag.
 
 .. _label:
```

### Comparing `odcs-0.5.0/docs/client.rst` & `odcs-0.6.0/docs/client.rst`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/docs/index.rst` & `odcs-0.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/docs/pulp.rst` & `odcs-0.6.0/docs/pulp.rst`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/docs/raw_config.rst` & `odcs-0.6.0/docs/raw_config.rst`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/odcs.egg-info/PKG-INFO` & `odcs-0.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,414 +1,415 @@
 Metadata-Version: 2.1
 Name: odcs
-Version: 0.5.0
+Version: 0.6.0
 Summary: On Demand Compose Service
 Home-page: https://pagure.io/odcs/
 Author: The Compose Team
 Author-email: odcs-owner@fedoraproject.org
 License: MIT
+Description: # On Demand Compose Service - ODCS
+        
+        ![logo of ODCS](https://pagure.io/odcs/raw/master/f/logo.png)
+        
+        ## What is ODCS
+        
+        The main goal of ODCS is to allow generation of temporary composes using the REST API calls. By a compose, we mainly mean RPM repository with packages taken from different sources, but in the future, generation of other output types could be possible too.
+        
+        ODCS can take RPMs for a compose from multiple sources like Koji tag, module built in Koji or external repository provided by Pulp tool.
+        
+        ## Using ODCS - client library
+        
+        There is client library written in Python which allows easy access to REST API provided by ODCS server.
+        
+        ### Installing the ODCS client
+        
+        On Fedora:
+        
+        ```
+        $ sudo dnf install odcs-client
+        ```
+        
+        If you want to install using `pip`, you can run following:
+        
+        ```
+        $ sudo pip install odcs[client]
+        ```
+        
+        In case you want your python project to depend on ODCS client library and add it to your `requirements.txt`, you can just use following to depend on ODCS client:
+        
+        ```
+        odcs[client]
+        ```
+        
+        ### ODCS authentication system
+        
+        ODCS server can be configured to authenticate using OpenIDC, Kerberos or SSL. Eventually it can be set in NoAuth mode to support anonymous access. Depending on the ODCS server configuration, you have to set your authentication method when creating ODCS class instance.
+        
+        #### Using OpenIDC for authentication
+        
+        To use OpenIDC, you have to provide the OpenIDC token to ODCS client class constructor. To obtain that OpenIDC token, you can either use `python-openidc-client`, or ask the OpenIDC provider for service token which does not have to be refreshed. Once you have the token, you can create the ODCS instance like this:
+        
+        ```
+        from odcs.client.odcs import ODCS, AuthMech
+        
+        odcs = ODCS("https://odcs.fedoraproject.org",
+                    auth_mech=AuthMech.OpenIDC,
+                    openidc_token="your_openidc_token")
+        ```
+        
+        Getting the `openidc_token` using `python-openidc-client` library can be done like this:
+        
+        ```
+        import openidc_client
+        staging = False
+        
+        if staging:
+            id_provider = 'https://id.stg.fedoraproject.org/openidc/'
+        else:
+            id_provider = 'https://id.fedoraproject.org/openidc/'
+        
+        # Get the auth token using the OpenID client.
+        oidc = openidc_client.OpenIDCClient(
+            'odcs',
+            id_provider,
+            {'Token': 'Token', 'Authorization': 'Authorization'},
+            'odcs-authorizer',
+            'notsecret',
+        )
+        
+        scopes = [
+            'openid',
+            'https://id.fedoraproject.org/scope/groups',
+            'https://pagure.io/odcs/new-compose',
+            'https://pagure.io/odcs/renew-compose',
+            'https://pagure.io/odcs/delete-compose',
+        ]
+        try:
+            token = oidc.get_token(scopes, new_token=True)
+            token = oidc.report_token_issue()
+        except requests.exceptions.HTTPError as e:
+            print(e.response.text)
+            raise
+        ```
+        
+        #### Using Kerberos for authentication
+        
+        To use Kerberos, you have to have valid Kerberos ticket or you need to have the Kerberos keytab file. If you want to use ODCS client library with Kerberos keytab, you have to set the `KRB5_CLIENT_KTNAME` environment variable to full path to the keytab file you want to use. You can for example do it like this:
+        
+        ```
+        from odcs.client.odcs import ODCS, AuthMech
+        from os import environ
+        environ["KRB5_CLIENT_KTNAME"] = "/full/path/to/ketab"
+        
+        odcs = ODCS("https://odcs.fedoraproject.org",
+                    auth_mech=AuthMech.Kerberos)
+        ```
+        
+        #### Using SSL for authentication
+        
+        To use SSL, you have to have SSL client certificate and key files. You then have to choose SSL AuthMech and pass the paths to SSL client certificate and key like this:
+        
+        ```
+        from odcs.client.odcs import ODCS, AuthMech
+        
+        odcs = ODCS("https://odcs.fedoraproject.org",
+                    auth_mech=AuthMech.SSL,
+                    ssl_cert="/path/to/ssl-crt.pem",
+                    ssl_key="/path/to/ssl-key.pem")
+        ```
+        
+        ### Requesting new compose
+        
+        The general way how to request new ODCS compose is following:
+        
+        ```
+        compose = odcs.new_compose(sources, source_type)
+        ```
+        
+        Both `sources` and `source_type` are strings. Depending on `source_type` value, the `sources` have following meaning:
+        
+        | `source_type` | `source` |
+        |---------------|----------|
+        | tag           | Name of Koji tag to take RPMs from. |
+        | module        | White-space separated NAME:STREAM or NAME:STREAM:VERSION of modules to include in compose. |
+        | pulp          | White-space separated list of content-sets or repository ids. Repositories will be included in a compose. |
+        | raw_config    | String in `name#commit` hash format. The `name` must match one of the raw config locations defined in ODCS server config as `raw_config_urls`. The `commit` is commit hash defining the version of raw config to use. This config is then used as input config for Pungi. |
+        | build         | Source should be omitted in the request. The list of Koji builds included in a compose is defined by `builds` attribute. |
+        | pungi_compose | URL to variant repository of external compose generated by the Pungi. For example https://kojipkgs.fedoraproject.org/compose/rawhide/latest-Fedora-Rawhide/compose/Server/. The generated compose will contain the same set of RPMs as the given external compose variant. The packages will be taken from the configured Koji instance. |
+        
+        There are also additional optional attributes you can pass to `new_compose(...)` method:
+        
+        - `seconds_to_live` - Number of seconds after which the generated compose should expire and will be removed.
+        - `packages` - List of packages which should be included in a compose. This is used only when `source_type` is set to `tag` or `build` to further limit the compose repository.
+        If the `packages` is not set, all packages in Koji tag or all packages in a `builds` list will be included in a final compose.
+        - `flags` - List of flags to further modify the compose output:
+            - `no_deps` - For `tag` `source_type`, do not resolve dependencies between packages and include only packages listed in the `packages` in the compose. For `module` `source_type`, do not resolve dependencies between modules and include only the requested module in the compose.
+            - `include_unpublished_pulp_repos` - For `pulp` `source_type`, include also unpublished repositories for input content-sets.
+            - `check_deps` - When set, abort the compose when some package has broken dependencies.
+            - `no_reuse` - When set, do not try to reuse old compose.
+            - `ignore_absent_pulp_repos` - For `pulp` `source_type`, ignore any content set that does not exist in Pulp
+            - `use_only_compatible_arch` - For `pulp` `source_type` only. When this flag is set, architecture hardcoded in URL returned from Pulp will be replaced with `$basearch` variable. The repository definition will also define `skip_if_unavailable = 1`. This could be useful when multiple content sets are included in the repofile to completly ignore packages from repositories for incompatible architectures.
+        - `sigkeys` - List of signature keys IDs. Only packages signed by one of these keys will be included in a compose. If there is no signed version of a package, compose will fail. It is also possible to pass an empty-string in a list meaning unsigned packages are allowed. For example if you want to prefer packages signed by key with ID `123` and also allow unsigned packages to appear in a compose, you can do it by setting sigkeys to `["123", ""]`.
+        - `results` - List of additional results which will be generated as part of a compose. Valid keys are:
+            - `iso` - Generates non-installable ISO files with RPMs from a compose.
+            - `boot.iso` - Generates `images/boot.iso` file which is needed to build base container images from resulting compose.
+        - `arches` - List of additional Koji arches to build this compose for. By default, the compose is built only for "x86_64" arch.
+        - `multilib_arches` - Subset of `arches` for which the multilib should be enabled. For each architecture in the `multilib_arches` list, ODCS will include also packages from other compatible architectures in a compose. For example when "x86_64" is included `multilib_arches`, ODCS will include also "i686" packages in a compose. The set of packages included in a composes is influenced by `multilib_method` list.
+        - `multilib_method` - List defining the method used to determine whether consider package as multilib. Defaults to empty list. The list can have following values:
+            - `iso` - Generates non-installable ISO files with RPMs from a compose.
+            - `runtime` - Packages whose name ends with "-devel" or "-static" suffix will be considered as multilib.
+            - `devel` - Packages that install some shared object file "*.so.*" will be considered as multilib.
+            - `all` - All pakages will be considered as multilib.
+        - `builds` - List of NVRs defining the Koji builds to include in a compose. Only valid for `tag` and `build` source types. For `tag` source type, the NVRs will be considered
+        for inclusion in a compose on top of Koji tag defined by `source`. For `build` source type, only the Koji builds defined by the NVRs will be considered for inclusion. The `packages` still need to be set to include particular packages from the Koji builds in a compose.
+        - `lookaside_repos` - List of URLs pointing to RPM repositories with packages which will be used by internal dependency resolver to resolve dependencies. Packages from these repositories will not appear in the resulting ODCS compose, but they are considered while checking whether the RPM dependencies are satisfied in the resulting compose when `check_deps` ODCS flag.
+        - `module_defaults_url` - List with URL to git repository with Module defaults data and the branch name or commit hash. For example ["https://pagure.io/releng/fedora-module-defaults.git", "master"]. This is used only when creating modular compose including non-modular RPMs.
+        - `modular_koji_tags` - List of Koji tags in which the modular Koji Content Generator builds are tagged. Such builds will be included in a compose.
+        
+        The `new_compose` method returns `dict` object describing the compose, for example:
+        
+        ```
+        {
+            "arches": "x86_64 ppc64",
+            "flags": [
+                "no_deps"
+            ],
+            "id": 1,
+            "owner": "jkaluza",
+            "packages": "gofer-package",
+            "removed_by": null,
+            "result_repo": "https://odcs.fedoraproject.org/composes/latest-odcs-1-1/compose/Temporary",
+            "result_repofile": "https://odcs.fedoraproject.org/composes/latest-odcs-1-1/compose/Temporary/odcs-1.repo",
+            "results": [
+                "repository"
+            ],
+            "sigkeys": "",
+            "source": "f26",
+            "source_type": 1,
+            "state": 3,
+            "state_name": "wait",
+            "time_done": "2017-10-13T17:03:13Z",
+            "time_removed": "2017-10-14T17:00:00Z",
+            "time_submitted": "2017-10-13T16:59:51Z",
+            "time_to_expire": "2017-10-14T16:59:51Z"
+        }
+        ```
+        
+        The most useful data there is `result_repofile`, which points to the .repo file with URLs for generated compose. Another very important data there is the `state` and `state_name` field. There are following states of a compose:
+        
+        | `state` | `state_name` | Description |
+        |---------|--------------|-------------|
+        | 0       | wait         | Compose is waiting in a queue to be generated |
+        | 1       | generating   | Compose is being generated |
+        | 2       | done         | Compose is generated - done |
+        | 3       | removed      | Compose has expired and is removed |
+        | 4       | failed       | Compose generation has failed |
+        
+        As you can see in our example, compose is in `wait` state and therefore we have to wait until the ODCS generates the compose.
+        
+        ### Waiting until the compose is generated
+        
+        There are two ways how to wait for the compose generation. The preferred one is listening on Fedora messaging bus for `odcs.state.change` message with `done` or `failed` state and another one is using HTTP polling implemented in `wait_for_compose(...)` method.
+        
+        If your application does not allow listening on the bus for some reason, you can use `wait_for_compose(...)` method like this:
+        
+        ```
+        compose = odcs.new_compose(sources, source_type)
+        
+        # Blocks until the compose is ready, but maximally for 600 seconds.
+        compose = odcs.wait_for_compose(compose["id"], timeout=600)
+        
+        if compose["state_name"] == "done":
+            print "Compose done, URL with repo file", compose["result_repofile"]
+        else:
+            print "Failed to generate compose"
+        ```
+        
+        ### Checking the state of existing ODCS compose
+        
+        Once you have the compose ready, you might want to check its state later. This can be done using the `get_compose(...)` method like this:
+        
+        ```
+        compose = odcs.get_compose(compose["id"])
+        ```
+        
+        ### Renewing the compose
+        
+        If the `time_to_expire` for your compose is getting closer and you know you want to continue using the compose, you can increase the `time_to_expire` using the `renew_compose(...)` method. You can also use this method to regenerate an expired compose in the `removed` state. Such compose will have the same versions of packages as the original compose.
+        
+        ```
+        compose = odcs.renew_compose(compose["id"])
+        ```
+        
+        ## Development
+        
+        ### Code Convention
+        
+        The code must be well formatted via ``black`` and pass ``flake8`` checking.
+        
+        Run ``tox -e black,flake8`` to do the check.
+        
+        ### Unit-testing
+        
+        Install packages required by pip to compile some python packages:
+        
+        ```
+        $ sudo dnf install -y gcc swig redhat-rpm-config python-devel openssl-devel openldap-devel \
+            zlib-devel bzip2 bzip2-devel readline-devel sqlite sqlite-devel tk-devel \
+            git python3-cairo-devel cairo-gobject-devel gobject-introspection-devel
+        ```
+        
+        A lot of these dependencies come from the module
+        [pygobject](https://pygobject.readthedocs.io/en/latest/devguide/dev_environ.html#fedora-dep).
+        
+        Run the tests:
+        
+        ```
+        $ make check
+        ```
+        
+        ### Testing local composes from plain RPM repositories
+        
+        You can test ODCS by generating compose from the `./server/tests/repo` repository using following commands:
+        
+        ```
+        $ ./create_sqlite_db
+        $ ./start_odcs_from_here
+        ```
+        
+        Before executing the command `start_odcs_from_here`, a messaging broker supporting AMQP protocol is required to run locally as well in order to run asynchronous tasks to generate composes. Here is an example to run a RabbitMQ broker:
+        
+        ```
+        sudo dnf install -y rabbitmq-server
+        sudo systemctl start rabbitmq-server
+        ```
+        
+        Add the `repo` source type to the server configuration in `./server/odcs/server/config.py`. (This will cause some tests to fail, so it needs to be reverted back after you are done with your changes!)
+        
+        And in another terminal, submit a request to frontend:
+        
+        ```
+        $ ./submit_test_compose repo `pwd`/server/tests/repo ed
+        {
+          "id": 1,
+          "owner": "Unknown",
+          "result_repo": null,
+          "source": "/home/hanzz/code/fedora-modularization/odcs/tests/repo",
+          "source_type": 3,
+          "state": 0,
+          "state_name": "wait",
+          "time_done": null,
+          "time_removed": null,
+          "time_submitted": "2017-06-12T14:18:19Z"
+        }
+        ```
+        
+        You should then see the backend process generating the compose and once it's done, the resulting compose in `./test_composes/latest-Unknown-1/compose/Temporary` directory.
+        
+        ### Using docker-compose for creating a local setup
+        
+        You can create test setup for ODCS with the docker-compose file. This yaml file creates docker container for the backend and frontend setup of ODCS and run multiple services together. These services are;
+        
+        * **rabbitmq** (Handles the communication between backend and frontend)
+        * **postgres** (Creates the database where the localy generated composes are stored)
+        * **backend** (Backend service of ODCS)
+        * **frontend** (Frontend service of ODCS that handles the REST API)
+        * **static** (Apache service for making storage available)
+        * **beat** (Cronjob for backend to check the service status)
+        
+        In addition to these, there are also three docker volumes (`odcs_odcs-composes`, `odcs_odcs-postgres` and `odcs_rabbitmq`) are created. These are providing persistent storage for the services.
+        
+        This yaml file requires also an **.env** file that specified some enviroment variables for the configuration of frontend and backend. Such an **.env** file should be in the same path with the **docker-compose.yml** file and here are the necessary variables that need to be specified in this file;
+        ```
+        # Pyhton path
+        PYTHONPATH=/src/common:/src/server:/src/client
+        
+        # POSTGRES
+        POSTGRES_USER=odcs
+        POSTGRES_PASSWORD=password
+        
+        # PULP CONFIGURATION
+        PULP_SERVER_URL=<URL of the pulp server>
+        PULP_USERNAME=<Username for the pulp server>
+        PULP_PASSWORD=<Credentials for the pulp server>
+        RAW_CONFIG_URLS=<Raw config settings in JSON format>
+        
+        # ODCS CONFIGURATION
+        ODCS_CONFIG_SECTION=DevConfiguration
+        ODCS_CONFIG_DIR=/src/server/conf/
+        ODCS_CELERY_BROKER_URL=amqp://guest:guest@rabbitmq:5672/
+        ODCS_DB_URL=postgresql+psycopg2://odcs:password@postgres/odcs
+        # Directory where the generated composes are stored. This hast to match
+        # location where odcs-composes volume is mounted in frontend and backend
+        # containers.
+        ODCS_TARGET_DIR=/mnt/odcs
+        TARGET_DIR_URL=http://localhost:8080
+        
+        # FLASK SETTINGS
+        # Force flask to reload application on change of source files.
+        FLASK_ENV=development
+        ```
+        
+        The services can be start with `sudo docker-compose up` command. If you have face an error or something that does not work correctly please use the following steps;
+        
+        1. Check whether there is already created docker volume.
+        
+        
+                $ sudo docker volume ls
+                Emulate Docker CLI using podman. Create /etc/containers/nodocker to quiet msg.
+                DRIVER      VOLUME NAME
+        
+        
+            If the output is like above, it means there isn't any volume yet and it is sufficient to run `sudo docker-compose up` and then `sudo docker-compose down` command. This creates the volumes and if you run the above command again the output becomes as follows;
+        
+        
+                $ sudo docker volume ls
+                Emulate Docker CLI using podman. Create /etc/containers/nodocker to quiet msg.
+                DRIVER      VOLUME NAME
+                local       odcs_odcs-composes
+                local       odcs_odcs-postgres
+                local       odcs_odcs-rabbitmq
+        
+        
+        2. After this point we need to set the correct permission to `ocds_odcs-composes` volume. In order to find where is the actual location of the volume type the following
+        
+        
+                $ sudo docker volume inspect odcs_odcs-composes
+                Emulate Docker CLI using podman. Create /etc/containers/nodocker to quiet msg.
+                [
+                    {
+                        "Name": "odcs_odcs-composes",
+                        "Driver": "local",
+                        "Mountpoint": "/var/lib/containers/storage/volumes/odcs_odcs-composes/_data",
+                        "CreatedAt": "2021-10-04T13:19:36.478636851+02:00",
+                        "Labels": {
+                            "io.podman.compose.project": "odcs"
+                        },
+                        "Scope": "local",
+                        "Options": {}
+                    }
+                ]
+        
+            `"Mountpoint": "/var/lib/containers/storage/volumes/odcs_odcs-composes/_data"` shows the exact location of the corresponding volume.
+        
+            Add group write permission to the Mountpoint by
+        
+        
+                $ sudo chmod 775 /var/lib/containers/storage/volumes/odcs_odcs-composes/_data
+        
+        
+        3. In this step it is sufficient to run `sudo docker-compose up` command to start the services properly.
+        
+        Here are some REST calls for checking the ODCS.
+        
+        * `$ curl -s http://localhost:5000/api/1/composes/ | jq .` This call shows all the composes in db.
+        * `$ odcs --server http://localhost:5000/ create-pulp <Pulp content set>` This call starts a pulp compose that match the given pulp content set
+        * `$ odcs --server http://localhost:5000/ create-raw-config --compose-type test my_raw_config master` This call starts a compose with the configuration defined as my_raw_config
+        
 Keywords: on demand compose service modularity fedora
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Build Tools
 Description-Content-Type: text/markdown
 Provides-Extra: client
 Provides-Extra: server
 Provides-Extra: all
-
-# On Demand Compose Service - ODCS
-
-![logo of ODCS](https://pagure.io/odcs/raw/master/f/logo.png)
-
-## What is ODCS
-
-The main goal of ODCS is to allow generation of temporary composes using the REST API calls. By a compose, we mainly mean RPM repository with packages taken from different sources, but in the future, generation of other output types could be possible too.
-
-ODCS can take RPMs for a compose from multiple sources like Koji tag, module built in Koji or external repository provided by Pulp tool.
-
-## Using ODCS - client library
-
-There is client library written in Python which allows easy access to REST API provided by ODCS server.
-
-### Installing the ODCS client
-
-On Fedora:
-
-```
-$ sudo dnf install odcs-client
-```
-
-If you want to install using `pip`, you can run following:
-
-```
-$ sudo pip install odcs[client]
-```
-
-In case you want your python project to depend on ODCS client library and add it to your `requirements.txt`, you can just use following to depend on ODCS client:
-
-```
-odcs[client]
-```
-
-### ODCS authentication system
-
-ODCS server can be configured to authenticate using OpenIDC, Kerberos or SSL. Eventually it can be set in NoAuth mode to support anonymous access. Depending on the ODCS server configuration, you have to set your authentication method when creating ODCS class instance.
-
-#### Using OpenIDC for authentication
-
-To use OpenIDC, you have to provide the OpenIDC token to ODCS client class constructor. To obtain that OpenIDC token, you can either use `python-openidc-client`, or ask the OpenIDC provider for service token which does not have to be refreshed. Once you have the token, you can create the ODCS instance like this:
-
-```
-from odcs.client.odcs import ODCS, AuthMech
-
-odcs = ODCS("https://odcs.fedoraproject.org",
-            auth_mech=AuthMech.OpenIDC,
-            openidc_token="your_openidc_token")
-```
-
-Getting the `openidc_token` using `python-openidc-client` library can be done like this:
-
-```
-import openidc_client
-staging = False
-
-if staging:
-    id_provider = 'https://id.stg.fedoraproject.org/openidc/'
-else:
-    id_provider = 'https://id.fedoraproject.org/openidc/'
-
-# Get the auth token using the OpenID client.
-oidc = openidc_client.OpenIDCClient(
-    'odcs',
-    id_provider,
-    {'Token': 'Token', 'Authorization': 'Authorization'},
-    'odcs-authorizer',
-    'notsecret',
-)
-
-scopes = [
-    'openid',
-    'https://id.fedoraproject.org/scope/groups',
-    'https://pagure.io/odcs/new-compose',
-    'https://pagure.io/odcs/renew-compose',
-    'https://pagure.io/odcs/delete-compose',
-]
-try:
-    token = oidc.get_token(scopes, new_token=True)
-    token = oidc.report_token_issue()
-except requests.exceptions.HTTPError as e:
-    print(e.response.text)
-    raise
-```
-
-#### Using Kerberos for authentication
-
-To use Kerberos, you have to have valid Kerberos ticket or you need to have the Kerberos keytab file. If you want to use ODCS client library with Kerberos keytab, you have to set the `KRB5_CLIENT_KTNAME` environment variable to full path to the keytab file you want to use. You can for example do it like this:
-
-```
-from odcs.client.odcs import ODCS, AuthMech
-from os import environ
-environ["KRB5_CLIENT_KTNAME"] = "/full/path/to/ketab"
-
-odcs = ODCS("https://odcs.fedoraproject.org",
-            auth_mech=AuthMech.Kerberos)
-```
-
-#### Using SSL for authentication
-
-To use SSL, you have to have SSL client certificate and key files. You then have to choose SSL AuthMech and pass the paths to SSL client certificate and key like this:
-
-```
-from odcs.client.odcs import ODCS, AuthMech
-
-odcs = ODCS("https://odcs.fedoraproject.org",
-            auth_mech=AuthMech.SSL,
-            ssl_cert="/path/to/ssl-crt.pem",
-            ssl_key="/path/to/ssl-key.pem")
-```
-
-### Requesting new compose
-
-The general way how to request new ODCS compose is following:
-
-```
-compose = odcs.new_compose(sources, source_type)
-```
-
-Both `sources` and `source_type` are strings. Depending on `source_type` value, the `sources` have following meaning:
-
-| `source_type` | `source` |
-|---------------|----------|
-| tag           | Name of Koji tag to take RPMs from. |
-| module        | White-space separated NAME:STREAM or NAME:STREAM:VERSION of modules to include in compose. |
-| pulp          | White-space separated list of content-sets or repository ids. Repositories will be included in a compose. |
-| raw_config    | String in `name#commit` hash format. The `name` must match one of the raw config locations defined in ODCS server config as `raw_config_urls`. The `commit` is commit hash defining the version of raw config to use. This config is then used as input config for Pungi. |
-| build         | Source should be omitted in the request. The list of Koji builds included in a compose is defined by `builds` attribute. |
-| pungi_compose | URL to variant repository of external compose generated by the Pungi. For example https://kojipkgs.fedoraproject.org/compose/rawhide/latest-Fedora-Rawhide/compose/Server/. The generated compose will contain the same set of RPMs as the given external compose variant. The packages will be taken from the configured Koji instance. |
-
-There are also additional optional attributes you can pass to `new_compose(...)` method:
-
-- `seconds_to_live` - Number of seconds after which the generated compose should expire and will be removed.
-- `packages` - List of packages which should be included in a compose. This is used only when `source_type` is set to `tag` or `build` to further limit the compose repository.
-If the `packages` is not set, all packages in Koji tag or all packages in a `builds` list will be included in a final compose.
-- `flags` - List of flags to further modify the compose output:
-    - `no_deps` - For `tag` `source_type`, do not resolve dependencies between packages and include only packages listed in the `packages` in the compose. For `module` `source_type`, do not resolve dependencies between modules and include only the requested module in the compose.
-    - `include_unpublished_pulp_repos` - For `pulp` `source_type`, include also unpublished repositories for input content-sets.
-    - `check_deps` - When set, abort the compose when some package has broken dependencies.
-    - `no_reuse` - When set, do not try to reuse old compose.
-    - `ignore_absent_pulp_repos` - For `pulp` `source_type`, ignore any content set that does not exist in Pulp
-    - `use_only_compatible_arch` - For `pulp` `source_type` only. When this flag is set, architecture hardcoded in URL returned from Pulp will be replaced with `$basearch` variable. The repository definition will also define `skip_if_unavailable = 1`. This could be useful when multiple content sets are included in the repofile to completly ignore packages from repositories for incompatible architectures.
-- `sigkeys` - List of signature keys IDs. Only packages signed by one of these keys will be included in a compose. If there is no signed version of a package, compose will fail. It is also possible to pass an empty-string in a list meaning unsigned packages are allowed. For example if you want to prefer packages signed by key with ID `123` and also allow unsigned packages to appear in a compose, you can do it by setting sigkeys to `["123", ""]`.
-- `results` - List of additional results which will be generated as part of a compose. Valid keys are:
-    - `iso` - Generates non-installable ISO files with RPMs from a compose.
-    - `boot.iso` - Generates `images/boot.iso` file which is needed to build base container images from resulting compose.
-- `arches` - List of additional Koji arches to build this compose for. By default, the compose is built only for "x86_64" arch.
-- `multilib_arches` - Subset of `arches` for which the multilib should be enabled. For each architecture in the `multilib_arches` list, ODCS will include also packages from other compatible architectures in a compose. For example when "x86_64" is included `multilib_arches`, ODCS will include also "i686" packages in a compose. The set of packages included in a composes is influenced by `multilib_method` list.
-- `multilib_method` - List defining the method used to determine whether consider package as multilib. Defaults to empty list. The list can have following values:
-    - `iso` - Generates non-installable ISO files with RPMs from a compose.
-    - `runtime` - Packages whose name ends with "-devel" or "-static" suffix will be considered as multilib.
-    - `devel` - Packages that install some shared object file "*.so.*" will be considered as multilib.
-    - `all` - All pakages will be considered as multilib.
-- `builds` - List of NVRs defining the Koji builds to include in a compose. Only valid for `tag` and `build` source types. For `tag` source type, the NVRs will be considered
-for inclusion in a compose on top of Koji tag defined by `source`. For `build` source type, only the Koji builds defined by the NVRs will be considered for inclusion. The `packages` still need to be set to include particular packages from the Koji builds in a compose.
-- `lookaside_repos` - List of URLs pointing to RPM repositories with packages which will be used by internal dependency resolver to resolve dependencies. Packages from these repositories will not appear in the resulting ODCS compose, but they are considered while checking whether the RPM dependencies are satisfied in the resulting compose when `check_deps` ODCS flag.
-- `module_defaults_url` - List with URL to git repository with Module defaults data and the branch name or commit hash. For example ["https://pagure.io/releng/fedora-module-defaults.git", "master"]. This is used only when creating modular compose including non-modular RPMs.
-- `modular_koji_tags` - List of Koji tags in which the modular Koji Content Generator builds are tagged. Such builds will be included in a compose.
-
-The `new_compose` method returns `dict` object describing the compose, for example:
-
-```
-{
-    "arches": "x86_64 ppc64",
-    "flags": [
-        "no_deps"
-    ],
-    "id": 1,
-    "owner": "jkaluza",
-    "packages": "gofer-package",
-    "removed_by": null,
-    "result_repo": "https://odcs.fedoraproject.org/composes/latest-odcs-1-1/compose/Temporary",
-    "result_repofile": "https://odcs.fedoraproject.org/composes/latest-odcs-1-1/compose/Temporary/odcs-1.repo",
-    "results": [
-        "repository"
-    ],
-    "sigkeys": "",
-    "source": "f26",
-    "source_type": 1,
-    "state": 3,
-    "state_name": "wait",
-    "time_done": "2017-10-13T17:03:13Z",
-    "time_removed": "2017-10-14T17:00:00Z",
-    "time_submitted": "2017-10-13T16:59:51Z",
-    "time_to_expire": "2017-10-14T16:59:51Z"
-}
-```
-
-The most useful data there is `result_repofile`, which points to the .repo file with URLs for generated compose. Another very important data there is the `state` and `state_name` field. There are following states of a compose:
-
-| `state` | `state_name` | Description |
-|---------|--------------|-------------|
-| 0       | wait         | Compose is waiting in a queue to be generated |
-| 1       | generating   | Compose is being generated |
-| 2       | done         | Compose is generated - done |
-| 3       | removed      | Compose has expired and is removed |
-| 4       | failed       | Compose generation has failed |
-
-As you can see in our example, compose is in `wait` state and therefore we have to wait until the ODCS generates the compose.
-
-### Waiting until the compose is generated
-
-There are two ways how to wait for the compose generation. The preferred one is listening on Fedora messaging bus for `odcs.state.change` message with `done` or `failed` state and another one is using HTTP polling implemented in `wait_for_compose(...)` method.
-
-If your application does not allow listening on the bus for some reason, you can use `wait_for_compose(...)` method like this:
-
-```
-compose = odcs.new_compose(sources, source_type)
-
-# Blocks until the compose is ready, but maximally for 600 seconds.
-compose = odcs.wait_for_compose(compose["id"], timeout=600)
-
-if compose["state_name"] == "done":
-    print "Compose done, URL with repo file", compose["result_repofile"]
-else:
-    print "Failed to generate compose"
-```
-
-### Checking the state of existing ODCS compose
-
-Once you have the compose ready, you might want to check its state later. This can be done using the `get_compose(...)` method like this:
-
-```
-compose = odcs.get_compose(compose["id"])
-```
-
-### Renewing the compose
-
-If the `time_to_expire` for your compose is getting closer and you know you want to continue using the compose, you can increase the `time_to_expire` using the `renew_compose(...)` method. You can also use this method to regenerate an expired compose in the `removed` state. Such compose will have the same versions of packages as the original compose.
-
-```
-compose = odcs.renew_compose(compose["id"])
-```
-
-## Development
-
-### Code Convention
-
-The code must be well formatted via ``black`` and pass ``flake8`` checking.
-
-Run ``tox -e black,flake8`` to do the check.
-
-### Unit-testing
-
-Install packages required by pip to compile some python packages:
-
-```
-$ sudo dnf install -y gcc swig redhat-rpm-config python-devel openssl-devel openldap-devel \
-    zlib-devel bzip2 bzip2-devel readline-devel sqlite sqlite-devel tk-devel \
-    git python3-cairo-devel cairo-gobject-devel gobject-introspection-devel
-```
-
-A lot of these dependencies come from the module
-[pygobject](https://pygobject.readthedocs.io/en/latest/devguide/dev_environ.html#fedora-dep).
-
-Run the tests:
-
-```
-$ make check
-```
-
-### Testing local composes from plain RPM repositories
-
-You can test ODCS by generating compose from the `./server/tests/repo` repository using following commands:
-
-```
-$ ./create_sqlite_db
-$ ./start_odcs_from_here
-```
-
-Before executing the command `start_odcs_from_here`, a messaging broker supporting AMQP protocol is required to run locally as well in order to run asynchronous tasks to generate composes. Here is an example to run a RabbitMQ broker:
-
-```
-sudo dnf install -y rabbitmq-server
-sudo systemctl start rabbitmq-server
-```
-
-Add the `repo` source type to the server configuration in `./server/odcs/server/config.py`. (This will cause some tests to fail, so it needs to be reverted back after you are done with your changes!)
-
-And in another terminal, submit a request to frontend:
-
-```
-$ ./submit_test_compose repo `pwd`/server/tests/repo ed
-{
-  "id": 1,
-  "owner": "Unknown",
-  "result_repo": null,
-  "source": "/home/hanzz/code/fedora-modularization/odcs/tests/repo",
-  "source_type": 3,
-  "state": 0,
-  "state_name": "wait",
-  "time_done": null,
-  "time_removed": null,
-  "time_submitted": "2017-06-12T14:18:19Z"
-}
-```
-
-You should then see the backend process generating the compose and once it's done, the resulting compose in `./test_composes/latest-Unknown-1/compose/Temporary` directory.
-
-### Using docker-compose for creating a local setup
-
-You can create test setup for ODCS with the docker-compose file. This yaml file creates docker container for the backend and frontend setup of ODCS and run multiple services together. These services are;
-
-* **rabbitmq** (Handles the communication between backend and frontend)
-* **postgres** (Creates the database where the localy generated composes are stored)
-* **backend** (Backend service of ODCS)
-* **frontend** (Frontend service of ODCS that handles the REST API)
-* **static** (Apache service for making storage available)
-* **beat** (Cronjob for backend to check the service status)
-
-In addition to these, there are also three docker volumes (`odcs_odcs-composes`, `odcs_odcs-postgres` and `odcs_rabbitmq`) are created. These are providing persistent storage for the services.
-
-This yaml file requires also an **.env** file that specified some enviroment variables for the configuration of frontend and backend. Such an **.env** file should be in the same path with the **docker-compose.yml** file and here are the necessary variables that need to be specified in this file;
-```
-# Pyhton path
-PYTHONPATH=/src/common:/src/server:/src/client
-
-# POSTGRES
-POSTGRES_USER=odcs
-POSTGRES_PASSWORD=password
-
-# PULP CONFIGURATION
-PULP_SERVER_URL=<URL of the pulp server>
-PULP_USERNAME=<Username for the pulp server>
-PULP_PASSWORD=<Credentials for the pulp server>
-RAW_CONFIG_URLS=<Raw config settings in JSON format>
-
-# ODCS CONFIGURATION
-ODCS_CONFIG_SECTION=DevConfiguration
-ODCS_CONFIG_FILE=/src/server/conf/config.py
-ODCS_CELERY_BROKER_URL=amqp://guest:guest@rabbitmq:5672/
-ODCS_DB_URL=postgresql+psycopg2://odcs:password@postgres/odcs
-# Directory where the generated composes are stored. This hast to match
-# location where odcs-composes volume is mounted in frontend and backend
-# containers.
-ODCS_TARGET_DIR=/mnt/odcs
-TARGET_DIR_URL=http://localhost:8080
-
-# FLASK SETTINGS
-# Force flask to reload application on change of source files.
-FLASK_ENV=development
-```
-
-The services can be start with `sudo docker-compose up` command. If you have face an error or something that does not work correctly please use the following steps;
-
-1. Check whether there is already created docker volume.
-
-
-        $ sudo docker volume ls
-        Emulate Docker CLI using podman. Create /etc/containers/nodocker to quiet msg.
-        DRIVER      VOLUME NAME
-
-
-    If the output is like above, it means there isn't any volume yet and it is sufficient to run `sudo docker-compose up` and then `sudo docker-compose down` command. This creates the volumes and if you run the above command again the output becomes as follows;
-
-
-        $ sudo docker volume ls
-        Emulate Docker CLI using podman. Create /etc/containers/nodocker to quiet msg.
-        DRIVER      VOLUME NAME
-        local       odcs_odcs-composes
-        local       odcs_odcs-postgres
-        local       odcs_odcs-rabbitmq
-
-
-2. After this point we need to set the correct permission to `ocds_odcs-composes` volume. In order to find where is the actual location of the volume type the following
-
-
-        $ sudo docker volume inspect odcs_odcs-composes
-        Emulate Docker CLI using podman. Create /etc/containers/nodocker to quiet msg.
-        [
-            {
-                "Name": "odcs_odcs-composes",
-                "Driver": "local",
-                "Mountpoint": "/var/lib/containers/storage/volumes/odcs_odcs-composes/_data",
-                "CreatedAt": "2021-10-04T13:19:36.478636851+02:00",
-                "Labels": {
-                    "io.podman.compose.project": "odcs"
-                },
-                "Scope": "local",
-                "Options": {}
-            }
-        ]
-
-    `"Mountpoint": "/var/lib/containers/storage/volumes/odcs_odcs-composes/_data"` shows the exact location of the corresponding volume.
-
-    Add group write permission to the Mountpoint by
-
-
-        $ sudo chmod 775 /var/lib/containers/storage/volumes/odcs_odcs-composes/_data
-
-
-3. In this step it is sufficient to run `sudo docker-compose up` command to start the services properly.
-
-Here are some REST calls for checking the ODCS.
-
-* `$ curl -s http://localhost:5000/api/1/composes/ | jq .` This call shows all the composes in db.
-* `$ odcs --server http://localhost:5000/ create-pulp <Pulp content set>` This call starts a pulp compose that match the given pulp content set
-* `$ odcs --server http://localhost:5000/ create-raw-config --compose-type test my_raw_config master` This call starts a compose with the configuration defined as my_raw_config
```

### Comparing `odcs-0.5.0/odcs.egg-info/SOURCES.txt` & `odcs-0.6.0/odcs.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -97,18 +97,16 @@
 server/odcs/server/templates/apidoc.html
 server/odcs/server/templates/index.html
 server/tests/Jenkinsfile
 server/tests/__init__.py
 server/tests/mbs.py
 server/tests/test_auth.py
 server/tests/test_backend.py
-server/tests/test_backend_thread.py
 server/tests/test_cache.py
 server/tests/test_celery_tasks.py
-server/tests/test_composerthread.py
 server/tests/test_events.py
 server/tests/test_metrics.py
 server/tests/test_mock_runroot.py
 server/tests/test_models.py
 server/tests/test_pulp.py
 server/tests/test_pungi.py
 server/tests/test_pungi_compose.py
```

### Comparing `odcs-0.5.0/server/conf/config.py` & `odcs-0.6.0/server/conf/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -173,18 +173,18 @@
         # Add this option to stop invoking celery built-in periodic task
         # celery.backend_cleanup which is useless and causes issue in odcs.
         "result_expires": None,
     }
 
     if "PULP_SERVER_URL" in environ:
         PULP_SERVER_URL = environ.get("PULP_SERVER_URL")
-    if "PULP_USERNAME" in environ:
-        PULP_USERNAME = environ.get("PULP_USERNAME")
-    if "PULP_PASSWORD" in environ:
-        PULP_PASSWORD = environ.get("PULP_PASSWORD")
+    if "PULP_SSL_KEY" in environ:
+        PULP_SSL_KEY = environ.get("PULP_SSL_KEY")
+    if "PULP_SSL_CERT" in environ:
+        PULP_SSL_CERT = environ.get("PULP_SSL_CERT")
     if "TARGET_DIR_URL" in environ:
         TARGET_DIR_URL = environ.get("TARGET_DIR_URL")
     if "RAW_CONFIG_URLS" in environ:
         RAW_CONFIG_URLS = json.loads(environ.get("RAW_CONFIG_URLS"))
 
 
 class DevConfiguration(BaseConfiguration):
```

### Comparing `odcs-0.5.0/server/conf/odcs-httpd-openidc.conf` & `odcs-0.6.0/server/conf/odcs-httpd-openidc.conf`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/conf/pungi.conf` & `odcs-0.6.0/server/conf/pungi.conf`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/contrib/odcs-promote-compose` & `odcs-0.6.0/server/contrib/odcs-promote-compose`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/contrib/odcs_test_deployment` & `odcs-0.6.0/server/contrib/odcs_test_deployment`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/__init__.py` & `odcs-0.6.0/server/odcs/server/__init__.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/api_utils.py` & `odcs-0.6.0/server/odcs/server/api_utils.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/auth.py` & `odcs-0.6.0/server/odcs/server/auth.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/backend.py` & `odcs-0.6.0/server/odcs/server/backend.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,32 +23,29 @@
 
 import errno
 import itertools
 from textwrap import dedent
 
 import koji
 import os
-import threading
 import shutil
 import productmd.compose
 import productmd.common
-from datetime import datetime, timedelta
 from odcs.server import log, conf, app, db
 from odcs.server.models import Compose, COMPOSE_STATES, COMPOSE_FLAGS
 from odcs.server.pungi import (
     Pungi,
     PungiConfig,
     PungiSourceType,
     PungiLogs,
     RawPungiConfig,
 )
 from odcs.server.pulp import Pulp
 from odcs.server.cache import KojiTagCache
 from odcs.server.pungi_compose import PungiCompose
-from concurrent.futures import ThreadPoolExecutor
 import glob
 import odcs.server.utils
 import odcs.server.mbs
 import defusedxml.ElementTree
 
 import gi
 
@@ -64,98 +61,23 @@
 # }
 LAST_EVENTS_CACHE = {}
 
 # Composes in generating state can be reused only when having this state_reason.
 GENERATING_STATE_REASON = "Compose is generating"
 
 
-class BackendThread(object):
+class RemoveExpiredComposes(object):
     """
-    Base BackendThread class.
-
-    The `BackendThread.do_work(...)` is called repeatedly after `timeout`
-    seconds.
-    """
-
-    def __init__(self, timeout=1):
-        """
-        Creates new BackendThread instance.
-
-        :param int timeout: Timeout in seconds after which do_work is called.
-        """
-        self.thread = None
-        self.exit = False
-        self.exit_cond = threading.Condition()
-        self.timeout = timeout
-
-    def do_work(self):
-        """
-        Reimplement this method in your own BackendThread subclass.
-        This method is called every `timeout` seconds.
-        """
-        raise NotImplementedError("do_work() method not implemented")
-
-    def _run(self):
-        """
-        Main "run" method of a thread. Calls `do_work()` after `self.timeout`
-        seconds. Stops then `stop()` is called.
-        """
-        while not self.exit:
-            try:
-                self.do_work()
-            except Exception:
-                log.exception("Exception in backend thread")
-                try:
-                    db.session.rollback()
-                except Exception:
-                    log.exception("Cannot rollback DB session")
-
-            # If the self.stop has been called from the do_work, break earlier
-            # so we don't wait on exit_cond.
-            if self.exit:
-                break
-
-            self.exit_cond.acquire()
-            self.exit_cond.wait(float(self.timeout))
-            self.exit_cond.release()
-
-    def join(self):
-        """
-        Waits until the thread terminates.
-        """
-        self.thread.join()
-
-    def stop(self):
-        """
-        Stops the thread.
-        """
-        self.exit = True
-        self.exit_cond.acquire()
-        self.exit_cond.notify()
-        self.exit_cond.release()
-
-    def start(self):
-        """
-        Starts the thread.
-        """
-        self.thread = threading.Thread(target=self._run)
-        self.thread.setDaemon(True)
-        self.thread.start()
-
-
-class RemoveExpiredComposesThread(BackendThread):
-    """
-    Thread used to remove old expired composes.
+    Used to remove old expired composes.
     """
 
     def __init__(self):
         """
-        Creates new RemoveExpiredComposesThread instance.
+        Creates new RemoveExpiredComposes instance.
         """
-        super(RemoveExpiredComposesThread, self).__init__(10)
         self._rmtree_errors = {}
 
     def _on_rmtree_error(self, function, path, excinf):
         """
         Helper method passed to `shutil.rmtree` as `onerror` kwarg which stores
         the rmtree errors in the `self._rmtree_errors` dict and allows the rmtree
         to continue removing other files.
@@ -873,16 +795,16 @@
     Generates the "compose" of PULP type - this basically means only
     repo file pointing to data in pulp.
     """
     content_sources = compose.source.split(" ")
 
     pulp = Pulp(
         server_url=conf.pulp_server_url,
-        username=conf.pulp_username,
-        password=conf.pulp_password,
+        ssl_cert=conf.pulp_ssl_cert,
+        ssl_key=conf.pulp_ssl_key,
         compose=compose,
     )
     include_unpublished_repos = (
         compose.flags & COMPOSE_FLAGS["include_unpublished_pulp_repos"]
     )
 
     repos = pulp.get_repos_from_content_sets(content_sources, include_unpublished_repos)
@@ -916,15 +838,15 @@
                 compose.source = " ".join(found_content_sets)
             else:
                 log.error(err)
                 raise ValueError(err)
 
     merged_repos = pulp.merge_repos_by_arch(repos)
     # Get all repos that are used via content sets.
-    used_repo_ids = set(item["id"] for item in merged_repos.values())
+    used_repo_ids = set(item.get("id") for item in merged_repos.values())
     # Add direct repos to the result, as long as the same repo is not already
     # used by a content set.
     for key, repo in direct_repos.items():
         if repo["id"] not in used_repo_ids:
             merged_repos[key] = repo
 
     repofile = ""
@@ -1236,16 +1158,15 @@
             )
             log.error(msg)
             raise RuntimeError(msg)
 
 
 def generate_compose(compose_id, lost_compose=False):
     """
-    Generates the compose defined by its `compose_id`. It is run by
-    ThreadPoolExecutor from the ComposerThread.
+    Generates the compose defined by its `compose_id`.
     """
     compose = None
     with app.app_context():
         try:
             # Get the compose from database.
             compose = Compose.query.filter(Compose.id == compose_id).one()
             log.info("%r: Starting compose generation", compose)
@@ -1287,138 +1208,7 @@
 
         koji_tag_cache = KojiTagCache(compose)
         koji_tag_cache.cleanup_reused(compose)
 
         # Commit the session to ensure that database transaction is closed and
         # does not remain in Idle state acquiring the table lock.
         db.session.commit()
-
-
-class ComposerThread(BackendThread):
-    """
-    Thread used to query the database for composes in "wait" state and
-    generating the composes using Pungi.
-    """
-
-    def __init__(self):
-        """
-        Creates new ComposerThread instance.
-        """
-        super(ComposerThread, self).__init__(1)
-        # ThreadPool to execute composes which calls "pungi" process.
-        self.executor = ThreadPoolExecutor(conf.num_concurrent_pungi)
-        # Threadpool to execute Pulp composes. These composes take just
-        # few seconds and do just single HTTP call to Pulp, so there is
-        # no need to put them into the same queue as Pungi based composes.
-        self.pulp_executor = ThreadPoolExecutor(2)
-
-        # List of composes which are being currently generated by this ODCS
-        # instance.
-        self.currently_generating = []
-
-    def generate_new_compose(self, compose):
-        """
-        Adds the compose to queue of composes to generate, so
-        the ThreadPoolExecutor can start working on it.
-        """
-        compose.transition(COMPOSE_STATES["generating"], "Compose thread started")
-
-        self.currently_generating.append(compose.id)
-        if compose.source_type == PungiSourceType.PULP:
-            self.pulp_executor.submit(generate_compose, compose.id)
-        else:
-            self.executor.submit(generate_compose, compose.id)
-
-    def generate_new_composes(self):
-        """
-        Gets all the composes in "wait" state. Generates them using Pungi
-        by calling `generate_compose(...)` in ThreadPoolExecutor.
-        """
-        composes = Compose.query.filter(Compose.state == COMPOSE_STATES["wait"]).all()
-
-        for compose in composes:
-            log.info("%r: Going to start compose generation.", compose)
-            self.generate_new_compose(compose)
-
-    def fail_lost_generating_composes(self):
-        """
-        Fails the composes in `generating` state in case they are in this
-        state for longer than `2 * conf.pungi_timeout`. Because composes
-        can be generating only for `conf.pungi_timeout` seconds, this is enough
-        time to generate any compose.
-        """
-        common_max_generating_time = 2 * conf.pungi_timeout
-        now = datetime.utcnow()
-        too_old_datetime = now - timedelta(seconds=common_max_generating_time)
-
-        # Get composes which are in 'generating' state for too long.
-        composes = (
-            Compose.query.filter(
-                Compose.state == COMPOSE_STATES["generating"],
-                Compose.time_started < too_old_datetime,
-            )
-            .order_by(Compose.id)
-            .all()
-        )
-
-        for compose in composes:
-            max_generating_time = common_max_generating_time
-            # RawConfig composes can have custom pungi_timeout. Filter them
-            # out here in case they are not `generating` for longer than their
-            # overriden pungi_timeout.
-            if compose.source_type == PungiSourceType.RAW_CONFIG:
-                # Get the pungi_timeout from RawPungiConfig.
-                pungi_cfg = RawPungiConfig(compose)
-                max_generating_time = pungi_cfg.pungi_timeout * 2
-                max_wait_seconds = timedelta(seconds=max_generating_time)
-                if compose.time_started + max_wait_seconds > now:
-                    continue
-
-            compose.transition(
-                COMPOSE_STATES["failed"],
-                "Compose stuck in 'generating' state for longer than %d "
-                "seconds." % max_generating_time,
-            )
-
-    def generate_lost_composes(self):
-        """
-        Gets all the composes in "generating" state and continues with
-        the generation process.
-
-        This method is here to handle situation where the ODCS is restarted
-        in the middle of compose generation.
-        """
-        composes = Compose.query.filter(
-            Compose.state == COMPOSE_STATES["generating"]
-        ).all()
-
-        for compose in composes:
-            if compose.id in self.currently_generating:
-                # We already have a thread working on this compose.
-                continue
-
-            log.info("%r: Going to regenerate lost compose.", compose)
-            self.generate_new_compose(compose)
-
-    def refresh_currently_generating(self):
-        """
-        Checks the status of all composes in self.currently_generating
-        and removes those which have been already done from this list.
-        """
-
-        new_currently_generating_list = []
-        for compose_id in self.currently_generating:
-            compose = Compose.query.filter(Compose.id == compose_id).one()
-            if compose.state != COMPOSE_STATES["generating"]:
-                continue
-
-            new_currently_generating_list.append(compose_id)
-        self.currently_generating = new_currently_generating_list
-
-    def do_work(self):
-        """
-        Gets all the composes in "wait" state. Generates them using Pungi
-        by calling `generate_compose(...)` in ThreadPoolExecutor.
-        """
-        self.generate_lost_composes()
-        self.generate_new_composes()
-        self.refresh_currently_generating()
```

### Comparing `odcs-0.5.0/server/odcs/server/cache.py` & `odcs-0.6.0/server/odcs/server/cache.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/celery_tasks.py` & `odcs-0.6.0/server/odcs/server/celery_tasks.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,25 +28,23 @@
 from celery import Celery
 from urllib.parse import urlparse
 from datetime import datetime, timedelta
 
 from odcs.server import conf, db, log
 from odcs.server.backend import (
     generate_compose as backend_generate_compose,
-    ComposerThread,
-    RemoveExpiredComposesThread,
+    RemoveExpiredComposes,
 )
 from odcs.server.utils import retry
 from odcs.server.models import Compose, COMPOSE_STATES
-from odcs.server.pungi import PungiSourceType
+from odcs.server.pungi import PungiSourceType, RawPungiConfig
 
 
 # Prepare the instances of classes with worker methods.
-composer_thread = ComposerThread()
-remove_expired_compose_thread = RemoveExpiredComposesThread()
+remove_expired_compose = RemoveExpiredComposes()
 
 
 # Create the Celery app.
 if os.environ.get("ODCS_CELERY_BROKER_URL"):
     broker_url = os.environ["ODCS_CELERY_BROKER_URL"]
     conf.celery_broker_url = broker_url
 elif conf.celery_broker_url:
@@ -319,14 +317,55 @@
             COMPOSE_STATES["done"],
             COMPOSE_STATES["failed"],
             COMPOSE_STATES["removed"],
         ):
             compose.transition(reused_compose.state, reused_compose.state_reason)
 
 
+def fail_lost_generating_composes():
+    """
+    Fails the composes in `generating` state in case they are in this
+    state for longer than `2 * conf.pungi_timeout`. Because composes
+    can be generating only for `conf.pungi_timeout` seconds, this is enough
+    time to generate any compose.
+    """
+    common_max_generating_time = 2 * conf.pungi_timeout
+    now = datetime.utcnow()
+    too_old_datetime = now - timedelta(seconds=common_max_generating_time)
+
+    # Get composes which are in 'generating' state for too long.
+    composes = (
+        Compose.query.filter(
+            Compose.state == COMPOSE_STATES["generating"],
+            Compose.time_started < too_old_datetime,
+        )
+        .order_by(Compose.id)
+        .all()
+    )
+
+    for compose in composes:
+        max_generating_time = common_max_generating_time
+        # RawConfig composes can have custom pungi_timeout. Filter them
+        # out here in case they are not `generating` for longer than their
+        # overriden pungi_timeout.
+        if compose.source_type == PungiSourceType.RAW_CONFIG:
+            # Get the pungi_timeout from RawPungiConfig.
+            pungi_cfg = RawPungiConfig(compose)
+            max_generating_time = pungi_cfg.pungi_timeout * 2
+            max_wait_seconds = timedelta(seconds=max_generating_time)
+            if compose.time_started + max_wait_seconds > now:
+                continue
+
+        compose.transition(
+            COMPOSE_STATES["failed"],
+            "Compose stuck in 'generating' state for longer than %d "
+            "seconds." % max_generating_time,
+        )
+
+
 @celery_app.task
 def run_cleanup():
     """
     Runs the cleanup.
     """
 
     @contextlib.contextmanager
@@ -334,14 +373,14 @@
         """Log any exception raised from the block and then ignore it."""
         try:
             yield
         except Exception:
             log.exception(msg)
 
     with log_errors("Error while removing expired composes"):
-        remove_expired_compose_thread.do_work()
+        remove_expired_compose.do_work()
     with log_errors("Error while marking lost generating composes as failed"):
-        composer_thread.fail_lost_generating_composes()
+        fail_lost_generating_composes()
     with log_errors("Error while rescheduling waiting composes"):
         reschedule_waiting_composes()
     with log_errors("Error while cleanup generating composes"):
         cleanup_generating_composes()
```

### Comparing `odcs-0.5.0/server/odcs/server/comps.py` & `odcs-0.6.0/server/odcs/server/comps.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/config.py` & `odcs-0.6.0/server/odcs/server/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,26 +46,24 @@
             "nosetests" in arg
             or "noserunner.py" in arg
             or "py.test" in arg
             or "pytest" in arg
             for arg in sys.argv
         ]
     ):
-        config_dir = os.path.abspath(
-            os.path.join(os.path.dirname(__file__), "..", "..", "conf")
-        )
         config_section = "TestConfiguration"
         sys.stderr.write("WARN: TestConfiguration will be used.\n")
     # DevConfiguration should be used when ODCS_DEVELOPER_ENV is equivalent to true
-    elif "ODCS_DEVELOPER_ENV" in os.environ and os.environ[
-        "ODCS_DEVELOPER_ENV"
-    ].lower() in ("1", "on", "true", "y", "yes"):
-        config_dir = os.path.abspath(
-            os.path.join(os.path.dirname(__file__), "..", "..", "conf")
-        )
+    elif os.environ.get("ODCS_DEVELOPER_ENV", "").lower() in (
+        "1",
+        "on",
+        "true",
+        "y",
+        "yes",
+    ):
         config_section = "DevConfiguration"
         sys.stderr.write("WARN: DevConfiguration will be used.\n")
 
     # Try loading configuration from file
     config_file = os.path.join(config_dir, "config.py")
     try:
         config_module = imp.load_source("odcs_runtime_config", config_file)
@@ -293,23 +291,23 @@
             "type": list,
             "default": [],
             "desc": "Default list of sigkeys. Any package in a compose must "
             "be signed by one of those keys. Can be overriden in a "
             "compose request.",
         },
         "pulp_server_url": {"type": str, "default": "", "desc": "Server URL of Pulp."},
-        "pulp_username": {
+        "pulp_ssl_key": {
             "type": str,
-            "default": "",
-            "desc": "Username to login Pulp.",
+            "default": "/path/to/ssl.key",
+            "desc": "Private key for pulp authentication",
         },
-        "pulp_password": {
+        "pulp_ssl_cert": {
             "type": str,
-            "default": "",
-            "desc": "Password to login Pulp.",
+            "default": "/path/to/ssl.crt",
+            "desc": "Certificate for pulp authentication",
         },
         "koji_config": {"type": str, "default": None, "desc": "Koji config file."},
         "koji_profile": {"type": str, "default": None, "desc": "Koji config profile."},
         "koji_krb_ccache": {
             "type": str,
             "default": None,
             "desc": "Kerberos ccache file to use for Koji auth.",
```

### Comparing `odcs-0.5.0/server/odcs/server/errors.py` & `odcs-0.6.0/server/odcs/server/errors.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/events.py` & `odcs-0.6.0/server/odcs/server/events.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/logger.py` & `odcs-0.6.0/server/odcs/server/logger.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/manage.py` & `odcs-0.6.0/server/odcs/server/manage.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/mbs.py` & `odcs-0.6.0/server/odcs/server/mbs.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/mergerepo.py` & `odcs-0.6.0/server/odcs/server/mergerepo.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/messaging.py` & `odcs-0.6.0/server/odcs/server/messaging.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/metrics.py` & `odcs-0.6.0/server/odcs/server/metrics.py`

 * *Files 13% similar despite different names*

```diff
@@ -255,14 +255,63 @@
 
     def run(self):
         while True:
             self.update_metrics()
             time.sleep(30)
 
 
+class QueueWorkerThread(threading.Thread):
+    """
+    Thread providing and updating following metrics:
+
+    - celery_queue_worker[queue_name] - Number of workers consume tasks from the queue.
+    """
+
+    def __init__(self, registry=None):
+        super(QueueWorkerThread, self).__init__()
+        self.daemon = True
+        self.queue_worker = Gauge(
+            "celery_queue_worker",
+            "Number of workers consume tasks from the queue.",
+            ["queue_name"],
+            registry=registry,
+        )
+
+        # Get all the possible queue names from the config.
+        self.queues = [conf.celery_cleanup_queue]
+        for rules in conf.celery_router_config["routing_rules"].values():
+            self.queues += rules.keys()
+
+        # Get the Celery connetion.
+        self.connection = celery_app.connection_or_acquire()
+        if isinstance(self.connection, FallbackContext):
+            self.connection = self.connection.fallback()
+
+    def update_metrics(self):
+        log.info("[metrics] Getting queue worker number.")
+        try:
+            active_queues = celery_app.control.inspect().active_queues()
+        except Exception:  # pragma: no cover
+            log.exception("[metrics] Error inspect active queues.")
+            return
+
+        # Initialize the queue worker to 0.
+        for queue in self.queues:
+            self.queue_worker.labels(queue).set(0)
+
+        for queues in active_queues.values():
+            for q in queues:
+                self.queue_worker.labels(q["name"]).inc()
+
+    def run(self):
+        while True:
+            self.update_metrics()
+            time.sleep(30)
+
+
 class ComposeCollectorThread(threading.Thread):
     def __init__(self):
         super(ComposeCollectorThread, self).__init__()
         self.daemon = True
 
     def run(self):
         registry.register(ComposesCollector())
@@ -280,7 +329,9 @@
         # by Python when main Python thread is stopped. There is no need to .join()
         # and since they are only updating metrics, they do not have to end up
         # gracefully and can just be "killed" by Python.
         worker_count_thread = WorkerCountThread(registry=registry)
         worker_count_thread.start()
         queue_length_thread = QueueLengthThread(registry=registry)
         queue_length_thread.start()
+        queue_worker_thread = QueueWorkerThread(registry=registry)
+        queue_worker_thread.start()
```

### Comparing `odcs-0.5.0/server/odcs/server/migrations/alembic.ini` & `odcs-0.6.0/server/odcs/server/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/migrations/env.py` & `odcs-0.6.0/server/odcs/server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/migrations/versions/0571a5ca58a0_add_index_to_compose_state.py` & `odcs-0.6.0/server/odcs/server/migrations/versions/0571a5ca58a0_add_index_to_compose_state.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/migrations/versions/0d4d8e1cfe29_create_user_model.py` & `odcs-0.6.0/server/odcs/server/migrations/versions/0d4d8e1cfe29_create_user_model.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/migrations/versions/16e08da18b49_add_compose_base_module_stream_version.py` & `odcs-0.6.0/server/odcs/server/migrations/versions/16e08da18b49_add_compose_base_module_stream_version.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/migrations/versions/3b92820da295_add_index_to_compose_time_to_expire.py` & `odcs-0.6.0/server/odcs/server/migrations/versions/3b92820da295_add_index_to_compose_time_to_expire.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/migrations/versions/512890e6864d_add_compose_scratch_modules.py` & `odcs-0.6.0/server/odcs/server/migrations/versions/512890e6864d_add_compose_scratch_modules.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/migrations/versions/566733ac3811_.py` & `odcs-0.6.0/server/odcs/server/migrations/versions/566733ac3811_.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/migrations/versions/59baece89746_add_compose_base_module_br_name_stream.py` & `odcs-0.6.0/server/odcs/server/migrations/versions/59baece89746_add_compose_base_module_br_name_stream.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/migrations/versions/a855c39e2a0f_store_celery_task_id.py` & `odcs-0.6.0/server/odcs/server/migrations/versions/a855c39e2a0f_store_celery_task_id.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/migrations/versions/c370b90de998_add_index_on_compose_source_type_and_.py` & `odcs-0.6.0/server/odcs/server/migrations/versions/c370b90de998_add_index_on_compose_source_type_and_.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/migrations/versions/cd0781bbdab1_.py` & `odcs-0.6.0/server/odcs/server/migrations/versions/cd0781bbdab1_.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/migrations/versions/d1da07e15c54_.py` & `odcs-0.6.0/server/odcs/server/migrations/versions/d1da07e15c54_.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/migrations/versions/de0a86d7de49_.py` & `odcs-0.6.0/server/odcs/server/migrations/versions/de0a86d7de49_.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/migrations/versions/e186faabdafe_.py` & `odcs-0.6.0/server/odcs/server/migrations/versions/e186faabdafe_.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/migrations/versions/e2163db7b15d_.py` & `odcs-0.6.0/server/odcs/server/migrations/versions/e2163db7b15d_.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/migrations/versions/f24a36cc8a16_add_index_on_compose_reused_id.py` & `odcs-0.6.0/server/odcs/server/migrations/versions/f24a36cc8a16_add_index_on_compose_reused_id.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/migrations/versions/f4bc999818d7_add_compose_removed_by.py` & `odcs-0.6.0/server/odcs/server/migrations/versions/f4bc999818d7_add_compose_removed_by.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/mock_runroot.py` & `odcs-0.6.0/server/odcs/server/mock_runroot.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/models.py` & `odcs-0.6.0/server/odcs/server/models.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/openapi.py` & `odcs-0.6.0/server/odcs/server/openapi.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/proxy.py` & `odcs-0.6.0/server/odcs/server/proxy.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/pulp.py` & `odcs-0.6.0/server/odcs/server/pulp.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,29 +33,29 @@
 from odcs.server.mergerepo import MergeRepo
 from odcs.server.utils import retry
 
 
 class Pulp(object):
     """Interface to Pulp"""
 
-    def __init__(self, server_url, username, password, compose):
-        self.username = username
-        self.password = password
+    def __init__(self, server_url, ssl_cert, ssl_key, compose):
+        self.ssl_cert = ssl_cert
+        self.ssl_key = ssl_key
         self.server_url = server_url
         self.compose = compose
         self.rest_api_root = "{0}/pulp/api/v2/".format(self.server_url.rstrip("/"))
 
     @retry(wait_on=(requests.exceptions.RequestException, ProtocolError))
     def _rest_post(self, endpoint, post_data):
         query_data = json.dumps(post_data)
         try:
             r = requests.post(
                 "{0}{1}".format(self.rest_api_root, endpoint.lstrip("/")),
                 query_data,
-                auth=(self.username, self.password),
+                cert=(self.ssl_cert, self.ssl_key),
                 timeout=conf.net_timeout,
             )
         except requests.exceptions.RequestException as e:
             # also catches ConnectTimeout, ConnectionError
             # change message of the catched exception and re-raise
             msg = "Pulp connection has failed: {}".format(e.args)
             raise requests.exceptions.RequestException(msg)
@@ -64,15 +64,15 @@
         return r.json()
 
     @retry(wait_on=requests.exceptions.RequestException)
     def _rest_get(self, endpoint):
         try:
             r = requests.get(
                 "{0}{1}".format(self.rest_api_root, endpoint),
-                auth=(self.username, self.password),
+                cert=(self.ssl_cert, self.ssl_key),
                 timeout=conf.net_timeout,
             )
         except requests.exceptions.RequestException as e:
             msg = "Pulp connection has failed: {}".format(e.args)
             raise requests.exceptions.RequestException(msg)
 
         r.raise_for_status()
@@ -166,18 +166,14 @@
 
         :param dict raw_repo: the repo info returned from Pulp API endpoint.
         :return: a simple repo info used internally for further handling.
         :rtype: dict
         """
         notes = raw_repo["notes"]
         url = self.server_url.rstrip("/") + "/" + notes["relative_url"]
-        # OSBS cannot verify https during the container image build, so
-        # fallback to http for now.
-        if url.startswith("https://"):
-            url = "http://" + url[len("https://") :]
         return {
             "id": raw_repo["id"],
             "url": url,
             "arches": {notes["arch"]},
             "sigkeys": sorted(notes["signatures"].split(",")),
             "product_versions": notes["product_versions"],
         }
```

### Comparing `odcs-0.5.0/server/odcs/server/pungi.py` & `odcs-0.6.0/server/odcs/server/pungi.py`

 * *Files 1% similar despite different names*

```diff
@@ -508,14 +508,16 @@
         # directly in the configuration.
         if not set(pungi_cmd).intersection(set(compose_type_to_arg.values())):
             # For unknown compose_type, fallback to --test to be safe.
             pungi_cmd.append(compose_type_to_arg.get(compose_type, "--test"))
 
         if compose.label:
             pungi_cmd.append("--label=%s" % str(compose.label))
+        if bool(compose.flags & COMPOSE_FLAGS["no_label"]):
+            pungi_cmd.append("--no-label")
         if compose.parent_pungi_compose_ids:
             for compose_id in compose.parent_pungi_compose_ids.split(" "):
                 pungi_cmd.append("--parent-compose-id=%s" % str(compose_id))
         if compose.respin_of:
             pungi_cmd.append("--respin-of=%s" % str(compose.respin_of))
 
         if self.koji_event:
```

### Comparing `odcs-0.5.0/server/odcs/server/pungi_compose.py` & `odcs-0.6.0/server/odcs/server/pungi_compose.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/templates/apidoc.html` & `odcs-0.6.0/server/odcs/server/templates/apidoc.html`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/templates/index.html` & `odcs-0.6.0/server/odcs/server/templates/index.html`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/utils.py` & `odcs-0.6.0/server/odcs/server/utils.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/odcs/server/views.py` & `odcs-0.6.0/server/odcs/server/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,16 +55,16 @@
     CELERY_AVAILABLE = True
 except ImportError:
     log.exception("Cannot import celery_tasks. The Celery support is turned off.")
     CELERY_AVAILABLE = False
 
 try:
     from . import openapi
-except ImportError as e:
-    log.exception("Can't generate OpenAPI specification because of: %s" % str(e))
+except ImportError:
+    log.warning("Can't generate OpenAPI specification due to missing openapi library")
     openapi = None
 
 
 app.openapispec = openapi.spec if openapi else None
 
 
 def _get_compose_owner():
```

### Comparing `odcs-0.5.0/server/tests/Jenkinsfile` & `odcs-0.6.0/server/tests/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/mbs.py` & `odcs-0.6.0/server/tests/mbs.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/repo/ed-1.14.1-2.module_fd8ca23e.src.rpm` & `odcs-0.6.0/server/tests/repo/ed-1.14.1-2.module_fd8ca23e.src.rpm`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/repo/ed-1.14.1-2.module_fd8ca23e.x86_64.rpm` & `odcs-0.6.0/server/tests/repo/ed-1.14.1-2.module_fd8ca23e.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/repo/ed-debuginfo-1.14.1-2.module_fd8ca23e.x86_64.rpm` & `odcs-0.6.0/server/tests/repo/ed-debuginfo-1.14.1-2.module_fd8ca23e.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/repo/module-build-macros-0.1-1.module_fd8ca23e.noarch.rpm` & `odcs-0.6.0/server/tests/repo/module-build-macros-0.1-1.module_fd8ca23e.noarch.rpm`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/repo/module-build-macros-0.1-1.module_fd8ca23e.src.rpm` & `odcs-0.6.0/server/tests/repo/module-build-macros-0.1-1.module_fd8ca23e.src.rpm`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/repo/repodata/028b753de97c22923bffe2159dcb478cdfa919376e21a68a1aa6ca40fba06f45-primary.sqlite.bz2` & `odcs-0.6.0/server/tests/repo/repodata/028b753de97c22923bffe2159dcb478cdfa919376e21a68a1aa6ca40fba06f45-primary.sqlite.bz2`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/repo/repodata/1879db5a1658329be62225ebf1b40cbf8e5d522abd2fdd86157d565c83e1ddc2-modules.yaml.gz` & `odcs-0.6.0/server/tests/repo/repodata/1879db5a1658329be62225ebf1b40cbf8e5d522abd2fdd86157d565c83e1ddc2-modules.yaml.gz`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/repo/repodata/2c3a353ba9e47c3e9c8be6c2e25c50fcc11e184a727c645f3f08b66aa1a1654d-other.xml.gz` & `odcs-0.6.0/server/tests/repo/repodata/2c3a353ba9e47c3e9c8be6c2e25c50fcc11e184a727c645f3f08b66aa1a1654d-other.xml.gz`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/repo/repodata/635015f39babdbcdcca3a516576bdcafb57fb77be3b7919cf85363ec558fb8fe-other.sqlite.bz2` & `odcs-0.6.0/server/tests/repo/repodata/635015f39babdbcdcca3a516576bdcafb57fb77be3b7919cf85363ec558fb8fe-other.sqlite.bz2`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/repo/repodata/77e6eb5a69d53a9d56f32b3154832d4eff6e2de518c268102d2c6848cffa3e1e-filelists.xml.gz` & `odcs-0.6.0/server/tests/repo/repodata/77e6eb5a69d53a9d56f32b3154832d4eff6e2de518c268102d2c6848cffa3e1e-filelists.xml.gz`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/repo/repodata/92ec6ea92c2b01e232c69539450c2f6ae0e4b31ccbad0f3a9678a4fc126b9fc0-filelists.sqlite.bz2` & `odcs-0.6.0/server/tests/repo/repodata/92ec6ea92c2b01e232c69539450c2f6ae0e4b31ccbad0f3a9678a4fc126b9fc0-filelists.sqlite.bz2`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/repo/repodata/ca15f74c9060791c17a93315bc8d2df4fd6a5d3e7c8eace70d82d023562a669e-primary.xml.gz` & `odcs-0.6.0/server/tests/repo/repodata/ca15f74c9060791c17a93315bc8d2df4fd6a5d3e7c8eace70d82d023562a669e-primary.xml.gz`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/repo/repodata/repomd.xml` & `odcs-0.6.0/server/tests/repo/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/test_auth.py` & `odcs-0.6.0/server/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/test_backend.py` & `odcs-0.6.0/server/tests/test_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -871,39 +871,39 @@
         }
         pulp_rest_post.assert_called_once_with("repositories/search/", expected_query)
 
         expected_repofile = dedent(
             """
             [foo-1]
             name=foo-1
-            baseurl=http://localhost/content/1/x86_64/os
+            baseurl=https://localhost/content/1/x86_64/os
             enabled=1
             gpgcheck=0
 
             [foo-2]
             name=foo-2
-            baseurl=http://localhost/content/2/x86_64/os
+            baseurl=https://localhost/content/2/x86_64/os
             enabled=1
             gpgcheck=0
 
             [foo-3]
             name=foo-3
-            baseurl=http://localhost/content/3/ppc64/os
+            baseurl=https://localhost/content/3/ppc64/os
             enabled=1
             gpgcheck=0
 
             [repo4]
             name=repo4
-            baseurl=http://localhost/content/100/s390/os
+            baseurl=https://localhost/content/100/s390/os
             enabled=1
             gpgcheck=0
 
             [repo5]
             name=repo5
-            baseurl=http://localhost/content/101/x86_64/os
+            baseurl=https://localhost/content/101/x86_64/os
             enabled=1
             gpgcheck=0
             """
         )
         _write_repo_file.assert_called_once_with(c, expected_repofile)
 
         self.assertEqual(c.state, COMPOSE_STATES["done"])
@@ -1081,15 +1081,15 @@
             }
         }
         pulp_rest_post.assert_called_once_with("repositories/search/", expected_query)
         expected_repofile = dedent(
             """
             [foo-1]
             name=foo-1
-            baseurl=http://localhost/content/1/x86_64/os
+            baseurl=https://localhost/content/1/x86_64/os
             enabled=1
             gpgcheck=0
             """
         )
         _write_repo_file.assert_called_once_with(c, expected_repofile)
         write_empty_repo.assert_not_called()
 
@@ -1447,15 +1447,15 @@
             },
         )
 
         expected_repofile = dedent(
             """
             [repo1]
             name=repo1
-            baseurl=http://localhost/content/1/s390/os
+            baseurl=https://localhost/content/1/s390/os
             enabled=1
             gpgcheck=0
             """
         )
         _write_repo_file.assert_called_once_with(c, expected_repofile)
 
         c1 = Compose.query.filter(Compose.id == 1).one()
```

### Comparing `odcs-0.5.0/server/tests/test_cache.py` & `odcs-0.6.0/server/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/test_celery_tasks.py` & `odcs-0.6.0/server/tests/test_celery_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -352,25 +352,25 @@
     def do_nothing(self):
         pass
 
     def raise_error(self):
         raise RuntimeError("It failed")
 
     @patch("odcs.server.celery_tasks.reschedule_waiting_composes")
-    @patch("odcs.server.celery_tasks.composer_thread")
-    @patch("odcs.server.celery_tasks.remove_expired_compose_thread")
+    @patch("odcs.server.celery_tasks.fail_lost_generating_composes")
+    @patch("odcs.server.celery_tasks.remove_expired_compose")
     def test_all_fine(
         self,
-        remove_expired_compose_thread,
-        composer_thread,
+        remove_expired_compose,
+        fail_lost_generating_composes,
         reschedule_waiting_composes,
     ):
         funcs = [
-            remove_expired_compose_thread.do_work,
-            composer_thread.fail_lost_generating_composes,
+            remove_expired_compose.do_work,
+            fail_lost_generating_composes,
             reschedule_waiting_composes,
         ]
         num_funcs = len(funcs)
 
         for i in range(num_funcs):
             # Run cleanup repeatedly, each time setting a different function to fail
             for x, func in enumerate(funcs):
```

### Comparing `odcs-0.5.0/server/tests/test_events.py` & `odcs-0.6.0/server/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/test_metrics.py` & `odcs-0.6.0/server/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/test_mock_runroot.py` & `odcs-0.6.0/server/tests/test_mock_runroot.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/test_models.py` & `odcs-0.6.0/server/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/test_pulp.py` & `odcs-0.6.0/server/tests/test_pulp.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/test_pungi.py` & `odcs-0.6.0/server/tests/test_pungi.py`

 * *Files 0% similar despite different names*

```diff
@@ -440,14 +440,15 @@
         self.compose = MagicMock()
         self.compose.target_dir = conf.target_dir
         self.compose.toplevel_dir = os.path.join(conf.target_dir, "odcs-1")
         self.compose.compose_type = "test"
         self.compose.label = None
         self.compose.pungi_config_dump = None
         self.compose.respin_of = None
+        self.compose.flags = 0
 
         makedirs(self.compose.toplevel_dir)
 
     def tearDown(self):
         super(TestPungi, self).tearDown()
 
         patch.stopall()
```

### Comparing `odcs-0.5.0/server/tests/test_pungi_compose.py` & `odcs-0.6.0/server/tests/test_pungi_compose.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/test_remove_expired_composes_thread.py` & `odcs-0.6.0/server/tests/test_remove_expired_composes_thread.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,43 +20,43 @@
 #
 # Written by Jan Kaluza <jkaluza@redhat.com>
 
 import odcs.server
 from odcs.server import db, conf
 from odcs.server.models import Compose
 from odcs.common.types import COMPOSE_STATES, COMPOSE_RESULTS
-from odcs.server.backend import RemoveExpiredComposesThread
+from odcs.server.backend import RemoveExpiredComposes
 from odcs.server.pungi import PungiSourceType
 from datetime import datetime, timedelta
 
 from .utils import ModelsBaseTest, AnyStringWith
 
 import os
 import mock
 from mock import patch
 
 
-class TestRemoveExpiredComposesThread(ModelsBaseTest):
+class TestRemoveExpiredComposes(ModelsBaseTest):
     maxDiff = None
 
     def setUp(self):
-        super(TestRemoveExpiredComposesThread, self).setUp()
+        super(TestRemoveExpiredComposes, self).setUp()
 
         compose = Compose.create(
             db.session,
             "unknown",
             PungiSourceType.MODULE,
             "testmodule-master",
             COMPOSE_RESULTS["repository"],
             60,
         )
         db.session.add(compose)
         db.session.commit()
 
-        self.thread = RemoveExpiredComposesThread()
+        self.thread = RemoveExpiredComposes()
 
     def test_does_not_remove_a_compose_which_state_is_not_done(self):
         """
         Test that we do not remove a composes on non-done state.
         """
         c = db.session.query(Compose).filter(Compose.id == 1).one()
         c.time_to_expire = datetime.utcnow() - timedelta(seconds=-120)
@@ -164,15 +164,15 @@
                 glob_ret_values[0].append(path)
             else:
                 glob_ret_values[1].append(path)
         glob.side_effect = glob_ret_values
 
     @patch("os.path.isdir")
     @patch("glob.glob")
-    @patch("odcs.server.backend.RemoveExpiredComposesThread._remove_compose_dir")
+    @patch("odcs.server.backend.RemoveExpiredComposes._remove_compose_dir")
     def test_remove_left_composes(self, remove_compose_dir, glob, isdir):
         isdir.return_value = True
         self._mock_glob(glob, ["latest-odcs-96-1", "odcs-96-1-20171005.n.0", "odcs-96"])
         self.thread.do_work()
         self.assertEqual(
             remove_compose_dir.call_args_list,
             [
@@ -180,15 +180,15 @@
                 mock.call(os.path.join(conf.target_dir, "odcs-96-1-20171005.n.0")),
                 mock.call(os.path.join(conf.target_dir, "odcs-96")),
             ],
         )
 
     @patch("os.path.isdir")
     @patch("glob.glob")
-    @patch("odcs.server.backend.RemoveExpiredComposesThread._remove_compose_dir")
+    @patch("odcs.server.backend.RemoveExpiredComposes._remove_compose_dir")
     @patch.object(
         odcs.server.config.Config,
         "extra_target_dirs",
         new={"releng-private": "/tmp/private"},
     )
     def test_remove_left_composes_extra_target_dir(
         self, remove_compose_dir, glob, isdir
@@ -204,46 +204,46 @@
                 mock.call(os.path.join(conf.target_dir, "odcs-*")),
                 mock.call("/tmp/private/odcs-*"),
             ],
         )
 
     @patch("os.path.isdir")
     @patch("glob.glob")
-    @patch("odcs.server.backend.RemoveExpiredComposesThread._remove_compose_dir")
+    @patch("odcs.server.backend.RemoveExpiredComposes._remove_compose_dir")
     def test_remove_left_composes_not_dir(self, remove_compose_dir, glob, isdir):
         isdir.return_value = False
         self._mock_glob(glob, ["latest-odcs-96-1"])
         self.thread.do_work()
         remove_compose_dir.assert_not_called()
 
     @patch("os.path.isdir")
     @patch("glob.glob")
-    @patch("odcs.server.backend.RemoveExpiredComposesThread._remove_compose_dir")
+    @patch("odcs.server.backend.RemoveExpiredComposes._remove_compose_dir")
     def test_remove_left_composes_wrong_dir(self, remove_compose_dir, glob, isdir):
         isdir.return_value = True
         self._mock_glob(glob, ["latest-odcs-", "odcs-", "odcs-abc"])
         self.thread.do_work()
         remove_compose_dir.assert_not_called()
 
     @patch("os.path.isdir")
     @patch("glob.glob")
-    @patch("odcs.server.backend.RemoveExpiredComposesThread._remove_compose_dir")
+    @patch("odcs.server.backend.RemoveExpiredComposes._remove_compose_dir")
     def test_remove_left_composes_valid_compose(self, remove_compose_dir, glob, isdir):
         isdir.return_value = True
         self._mock_glob(glob, ["latest-odcs-1-1", "odcs-1-1-2017.n.0"])
         c = db.session.query(Compose).filter(Compose.id == 1).one()
         c.state = COMPOSE_STATES["done"]
         db.session.add(c)
         db.session.commit()
         self.thread.do_work()
         remove_compose_dir.assert_not_called()
 
     @patch("os.path.isdir")
     @patch("glob.glob")
-    @patch("odcs.server.backend.RemoveExpiredComposesThread._remove_compose_dir")
+    @patch("odcs.server.backend.RemoveExpiredComposes._remove_compose_dir")
     def test_remove_left_composes_expired_compose(
         self, remove_compose_dir, glob, isdir
     ):
         isdir.return_value = True
         self._mock_glob(glob, ["latest-odcs-1-1", "odcs-1-1-2017.n.0"])
         c = db.session.query(Compose).filter(Compose.id == 1).one()
         c.state = COMPOSE_STATES["removed"]
```

### Comparing `odcs-0.5.0/server/tests/test_utils.py` & `odcs-0.6.0/server/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/test_views.py` & `odcs-0.6.0/server/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/server/tests/utils.py` & `odcs-0.6.0/server/tests/utils.py`

 * *Files identical despite different names*

### Comparing `odcs-0.5.0/setup.py` & `odcs-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     long_description = f.read()
 
 setup(
     name="odcs",
     description="On Demand Compose Service",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.5.0",
+    version="0.6.0",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Topic :: Software Development :: Build Tools",
     ],
     keywords="on demand compose service modularity fedora",
     author="The Compose Team",
     # TODO: Not sure which name would be used for mail alias,
@@ -96,12 +96,13 @@
     },
     data_files=[
         (
             get_dir(["etc", "odcs"]),
             [
                 "server/conf/config.py",
                 "server/conf/pungi.conf",
+                "server/conf/raw_config_urls.conf",
                 "server/conf/raw_config_wrapper.conf",
             ],
         ),
     ],
 )
```

