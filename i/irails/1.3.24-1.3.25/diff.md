# Comparing `tmp/irails-1.3.24.tar.gz` & `tmp/irails-1.3.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.3.24.tar", last modified: Wed May 24 10:30:56 2023, max compression
+gzip compressed data, was "irails-1.3.25.tar", last modified: Wed May 24 15:00:12 2023, max compression
```

## Comparing `irails-1.3.24.tar` & `irails-1.3.25.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 10:30:56.261195 irails-1.3.24/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.24/MANIFEST.in
--rw-rw-rw-   0        0        0     4878 2023-05-24 10:30:56.260198 irails-1.3.24/PKG-INFO
--rw-rw-rw-   0        0        0     4096 2023-05-22 07:06:26.000000 irails-1.3.24/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 10:30:56.146613 irails-1.3.24/irails/
--rw-rw-rw-   0        0        0      307 2023-05-24 10:30:45.000000 irails-1.3.24/irails/__init__.py
--rw-rw-rw-   0        0        0     4887 2023-05-21 14:33:24.000000 irails-1.3.24/irails/_i18n.py
--rw-rw-rw-   0        0        0     2878 2023-05-21 08:27:23.000000 irails-1.3.24/irails/_loader.py
--rw-rw-rw-   0        0        0     5253 2023-05-20 14:13:50.000000 irails-1.3.24/irails/_utils.py
--rw-rw-rw-   0        0        0    12042 2023-05-20 06:44:17.000000 irails-1.3.24/irails/auth.py
--rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.24/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-24 10:30:56.154593 irails-1.3.24/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-24 10:30:56.155589 irails-1.3.24/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.24/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10589 2023-05-13 05:03:07.000000 irails-1.3.24/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.24/irails/cbv.py
--rw-rw-rw-   0        0        0     6174 2023-05-19 07:06:13.000000 irails-1.3.24/irails/config.py
--rw-rw-rw-   0        0        0    12478 2023-05-12 05:56:24.000000 irails-1.3.24/irails/controller_utils.py
--rw-rw-rw-   0        0        0    24918 2023-05-19 11:59:51.000000 irails-1.3.24/irails/core.py
--rw-rw-rw-   0        0        0    19577 2023-05-24 10:23:28.000000 irails-1.3.24/irails/database.py
--rw-rw-rw-   0        0        0     1459 2023-05-11 15:27:11.000000 irails-1.3.24/irails/log.py
--rw-rw-rw-   0        0        0     8736 2023-05-21 14:38:31.000000 irails-1.3.24/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.24/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.24/irails/midware_session.py
--rw-rw-rw-   0        0        0     4208 2023-05-16 08:12:27.000000 irails-1.3.24/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-05-24 10:30:56.166446 irails-1.3.24/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.24/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.24/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.24/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.24/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.24/irails/scripts/_migrate.py
--rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.24/irails/scripts/_model.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.24/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1600 2023-05-11 15:45:21.000000 irails-1.3.24/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.24/irails/scripts/_shell.py
--rw-rw-rw-   0        0        0     4930 2023-05-21 14:27:15.000000 irails-1.3.24/irails/scripts/_test.py
--rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.24/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-24 10:30:56.115790 irails-1.3.24/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-24 10:30:56.178416 irails-1.3.24/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.24/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.24/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.24/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.24/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.24/irails/scripts/tpls/app/model.jinja
--rw-rw-rw-   0        0        0     1300 2023-05-20 14:09:55.000000 irails-1.3.24/irails/scripts/tpls/app/service.jinja
--rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.24/irails/scripts/tpls/app/test_controller.jinja
--rw-rw-rw-   0        0        0      893 2023-05-14 14:08:50.000000 irails-1.3.24/irails/scripts/tpls/app/test_service.jinja
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.24/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-24 10:30:56.180411 irails-1.3.24/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.24/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-24 10:30:56.181409 irails-1.3.24/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.24/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 10:30:56.193378 irails-1.3.24/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.24/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.24/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.24/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.24/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.24/irails/scripts/tpls/project/configs/casbin-model.conf
-drwxrwxrwx   0        0        0        0 2023-05-24 10:30:56.223298 irails-1.3.24/irails/scripts/tpls/project/configs/casbin_templates/
--rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.24/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
--rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.24/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
--rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.24/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
--rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.24/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
--rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.24/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
--rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.24/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
--rw-rw-rw-   0        0        0      274 2023-05-18 07:46:03.000000 irails-1.3.24/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
--rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.24/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
--rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.24/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
--rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.24/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.24/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.24/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.24/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.24/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-05-24 10:30:56.118780 irails-1.3.24/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-05-24 10:30:56.234269 irails-1.3.24/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.24/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.24/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.24/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.24/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-24 10:30:56.239256 irails-1.3.24/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.24/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.24/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-24 10:30:56.243245 irails-1.3.24/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-24 10:30:56.121775 irails-1.3.24/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-24 10:30:56.248231 irails-1.3.24/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.24/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-24 10:30:56.256214 irails-1.3.24/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.24/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.24/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.24/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-24 10:30:56.123771 irails-1.3.24/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-24 10:30:56.258204 irails-1.3.24/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.24/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     1585 2023-05-24 07:01:16.000000 irails-1.3.24/irails/unit_test.py
--rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.24/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-24 10:30:56.151599 irails-1.3.24/irails.egg-info/
--rw-rw-rw-   0        0        0     4878 2023-05-24 10:30:55.000000 irails-1.3.24/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3115 2023-05-24 10:30:55.000000 irails-1.3.24/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 10:30:55.000000 irails-1.3.24/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-24 10:30:55.000000 irails-1.3.24/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      360 2023-05-24 10:30:55.000000 irails-1.3.24/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-24 10:30:55.000000 irails-1.3.24/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 10:30:56.261195 irails-1.3.24/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.24/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.897792 irails-1.3.25/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.25/MANIFEST.in
+-rw-rw-rw-   0        0        0     4878 2023-05-24 15:00:12.896807 irails-1.3.25/PKG-INFO
+-rw-rw-rw-   0        0        0     4096 2023-05-22 07:06:26.000000 irails-1.3.25/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.818476 irails-1.3.25/irails/
+-rw-rw-rw-   0        0        0      307 2023-05-24 14:59:48.000000 irails-1.3.25/irails/__init__.py
+-rw-rw-rw-   0        0        0     4887 2023-05-21 14:33:24.000000 irails-1.3.25/irails/_i18n.py
+-rw-rw-rw-   0        0        0     2878 2023-05-21 08:27:23.000000 irails-1.3.25/irails/_loader.py
+-rw-rw-rw-   0        0        0     5253 2023-05-20 14:13:50.000000 irails-1.3.25/irails/_utils.py
+-rw-rw-rw-   0        0        0    12042 2023-05-20 06:44:17.000000 irails-1.3.25/irails/auth.py
+-rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.25/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.826454 irails-1.3.25/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.827452 irails-1.3.25/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.25/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10589 2023-05-13 05:03:07.000000 irails-1.3.25/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.25/irails/cbv.py
+-rw-rw-rw-   0        0        0     6174 2023-05-19 07:06:13.000000 irails-1.3.25/irails/config.py
+-rw-rw-rw-   0        0        0    12478 2023-05-12 05:56:24.000000 irails-1.3.25/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    24918 2023-05-19 11:59:51.000000 irails-1.3.25/irails/core.py
+-rw-rw-rw-   0        0        0    20051 2023-05-24 14:56:19.000000 irails-1.3.25/irails/database.py
+-rw-rw-rw-   0        0        0     1459 2023-05-11 15:27:11.000000 irails-1.3.25/irails/log.py
+-rw-rw-rw-   0        0        0     8736 2023-05-21 14:38:31.000000 irails-1.3.25/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.25/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.25/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4208 2023-05-16 08:12:27.000000 irails-1.3.25/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.839419 irails-1.3.25/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.25/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.25/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.25/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.25/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.25/irails/scripts/_migrate.py
+-rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.25/irails/scripts/_model.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.25/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1600 2023-05-11 15:45:21.000000 irails-1.3.25/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.25/irails/scripts/_shell.py
+-rw-rw-rw-   0        0        0     4930 2023-05-21 14:27:15.000000 irails-1.3.25/irails/scripts/_test.py
+-rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.25/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.786318 irails-1.3.25/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.849403 irails-1.3.25/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.25/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.25/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.25/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.25/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.25/irails/scripts/tpls/app/model.jinja
+-rw-rw-rw-   0        0        0      197 2023-05-24 11:06:24.000000 irails-1.3.25/irails/scripts/tpls/app/service.jinja
+-rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.25/irails/scripts/tpls/app/test_controller.jinja
+-rw-rw-rw-   0        0        0      908 2023-05-24 14:14:47.000000 irails-1.3.25/irails/scripts/tpls/app/test_service.jinja
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.25/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.852385 irails-1.3.25/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.25/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.853383 irails-1.3.25/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.25/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.862359 irails-1.3.25/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.25/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.25/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.25/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.25/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.25/irails/scripts/tpls/project/configs/casbin-model.conf
+drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.875323 irails-1.3.25/irails/scripts/tpls/project/configs/casbin_templates/
+-rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.25/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
+-rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.25/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
+-rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.25/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
+-rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.25/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
+-rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.25/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
+-rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.25/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
+-rw-rw-rw-   0        0        0      274 2023-05-18 07:46:03.000000 irails-1.3.25/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
+-rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.25/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
+-rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.25/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
+-rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.25/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.25/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.25/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.25/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.25/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.789309 irails-1.3.25/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.879312 irails-1.3.25/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.25/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.25/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.25/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.25/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.883323 irails-1.3.25/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.25/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.25/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.886818 irails-1.3.25/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.792149 irails-1.3.25/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.888815 irails-1.3.25/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.25/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.892804 irails-1.3.25/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.25/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.25/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.25/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.793147 irails-1.3.25/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.893802 irails-1.3.25/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.25/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     1585 2023-05-24 07:01:16.000000 irails-1.3.25/irails/unit_test.py
+-rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.25/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.824459 irails-1.3.25/irails.egg-info/
+-rw-rw-rw-   0        0        0     4878 2023-05-24 15:00:12.000000 irails-1.3.25/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3115 2023-05-24 15:00:12.000000 irails-1.3.25/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 15:00:12.000000 irails-1.3.25/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-24 15:00:12.000000 irails-1.3.25/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      367 2023-05-24 15:00:12.000000 irails-1.3.25/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-24 15:00:12.000000 irails-1.3.25/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 15:00:12.897792 irails-1.3.25/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.25/setup.py
```

### Comparing `irails-1.3.24/PKG-INFO` & `irails-1.3.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.24
+Version: 1.3.25
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.24/README.md` & `irails-1.3.25/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/_i18n.py` & `irails-1.3.25/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/_loader.py` & `irails-1.3.25/irails/_loader.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/_utils.py` & `irails-1.3.25/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/auth.py` & `irails-1.3.25/irails/auth.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/base_controller.py` & `irails-1.3.25/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.3.25/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.3.25/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/cbv.py` & `irails-1.3.25/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/config.py` & `irails-1.3.25/irails/config.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/controller_utils.py` & `irails-1.3.25/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/core.py` & `irails-1.3.25/irails/core.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/database.py` & `irails-1.3.25/irails/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
                         ForeignKey, 
                         func,
                         select,join,
                         TableClause,
                         update,insert,delete,
                         event,text,TextClause,Table,
                         inspect)
+import sqlalchemy
 from sqlalchemy.orm import DeclarativeBase,Session,relationship,Query 
 from sqlalchemy.ext.automap import automap_base 
 from sqlalchemy.sql._typing import _ColumnsClauseArgument
 from alembic import command
 from alembic.config import Config 
 from ._utils import camelize_classname,pluralize_collection 
 from .log import _log
@@ -65,16 +66,15 @@
     i18n_json_data_field = cfg.get("i18n_json_data_field",'i18n_json_data')
  
 class Base( DeclarativeBase ):
     __abstract__ = True 
     def __init_subclass__(cls,*args,**kwargs) -> None: 
         super().__init_subclass__(*args,**kwargs)
         for e in EVENTS:
-            if hasattr(cls,e):
-                if callable(getattr(cls,e)):
+            if hasattr(cls,e) and callable(getattr(cls,e)):
                     event.listen(cls, e, getattr(cls,e)) 
         
         metas = inspect(cls)
         for col in metas.columns:
             func_name = f"on_change_{col.name}"
             if hasattr(cls,func_name):
                 func = getattr(cls,func_name)
@@ -109,40 +109,40 @@
             Column(f'{tb2_naked_name}_id', Integer, ForeignKey(f'{Tb2.__tablename__}.id'), primary_key=True) 
         ) 
         setattr(Tb1,f"{tb2}",relationship(Tb2.__name__, secondary=m2m_table, back_populates=f"{tb1}",passive_deletes=False  ))
         setattr(Tb2,f"{tb1}",relationship(Tb1.__name__, secondary=m2m_table, back_populates=f"{tb2}",passive_deletes=False ))
         self.__all[f"M2M{tb1}{tb2}"] = m2m_table
         return m2m_table
     @classmethod
-    def M2O(self, ChildTable: Base, ParentTable: Base):
+    def M2O(self, ChildTable: Base, ParentTable: Base,cascade='delete,all'):
         '''set 
         :ChildTable belongs to :ParentTable
         and :ParentTable hasmany :ChildTable
         '''
         child_tablename = ChildTable.__tablename__
         parent_tablename = ParentTable.__tablename__
         child_tbname = get_singularize_name(child_tablename)
         parent_tbname = get_singularize_name(parent_tablename)
 
         setattr(ChildTable, f"{parent_tbname}_id", Column(Integer, ForeignKey(f'{parent_tbname}.id')))
         setattr(ChildTable, f"{parent_tbname}", relationship(ParentTable.__name__, back_populates=f'{child_tbname}'))
 
-        setattr(ParentTable, child_tbname, relationship(ChildTable.__name__, back_populates=f'{parent_tbname}', cascade='delete,all'))
+        setattr(ParentTable, child_tbname, relationship(ChildTable.__name__, back_populates=f'{parent_tbname}', cascade=cascade))
         return ChildTable, ParentTable
 
     @classmethod
     def SOFT_DELETE(self,*tables):
         """
         set a `is_deleted` field on :tables
         please use irails.service to query ,it will auto add the 'is_deleted' flag
         """
         for Tb in tables:
             setattr(Tb,is_deleted_field,Column(Boolean, default=False))
     @classmethod
-    def ADD_I18N(self,*tables):
+    def I18NABLE(self,*tables):
         #i18n_json_data={
         #       'col1':{
         #           'en':'bruce',
         #           'zh':'布鲁斯'
         #       },
         #       'col2':{
         #           'en':'hellow',
@@ -177,58 +177,70 @@
     def __init__(self,query:Query,size:int=None ) -> None: 
         self.query = query
         if size:
             self.page_size = size
         else:
             self.page_size = page_size 
          
-    def count(self)->int:
+    def count_all(self)->int:
         return self.query.count()
+    
     def page_count(self)->int:
         import math
-        return math.ceil(self.count()/self.page_size)
+        return math.ceil(self.count_all()/self.page_size)
+    
+    def page(self,page_num=1)->Query:
+        return self.query.limit(self.page_size).offset(self.page_size*(page_num-1))
     
-    def page(self,current=1)->Query:
-        return self.query.limit(self.page_size).offset(self.page_size*(current-1))
-    def get(self,current=1)->List[Base]:
-        return self.query.limit(self.page_size).offset(self.page_size*(current-1)).all()
+    def get_rows(self,page_num=1)->List[Base]:
+        return self.query.limit(self.page_size).offset(self.page_size*(page_num-1)).all()
 class Service(metaclass=_serviceMeta):
     __all_generated = {}
-     
+    _session:Session = None
     _ = _ #the i18n traslation object ,it's will auto redirect the `app_name/locales` dir i18n configure
     @contextmanager      
     @staticmethod 
     def get_session():
         """Provide a transactional scope around a series of operations."""
-        if hasattr(Service,'_session'):
-            session = getattr(Service,'_session')
+        if  Service._session:
+            session = Service._session
         else:
             session = Service.session()
         try:
             yield session
             session.commit()
         except Exception as e:
             session.rollback()
             raise e
         # finally:
         #     session.close()
     @classmethod
     def session(self)->Session:
-        if hasattr(Service,"_session"):
+        if  Service._session:
             return Service._session 
         Service._session = Session(bind=engine) 
         return Service._session
      
     @classmethod
     def pager(self,model:Base,*args,**kwargs)->ListPager:
         """get query object with auto passed is_deleted rows"""
 
         query = self.query(model,*args,**kwargs)
         return ListPager(query=query)
-     
+    @classmethod
+    def exists(self,model:Base,field_name:str,value:Any)->bool:
+        session = self.session()
+        kwargs = {field_name:value}
+        try:
+            q = session.query(model).filter_by(**kwargs).one()
+        except sqlalchemy.exc.NoResultFound as e: 
+            return False
+        except sqlalchemy.orm.exc.MultipleResultsFound:
+            return True
+        return not q  is None
     @classmethod
     def query(self,model:Base,*args,**kwargs)->Query:
         '''Get a query object with auto passed is_deleted rows'''
         session = self.session()
         if hasattr(model,is_deleted_field):
             if not kwargs:kwargs = {}
             if not is_deleted_field in kwargs:
@@ -273,20 +285,22 @@
         ''' Auto pass if row has is_deleted field
             :return count by givened :args on :model
         '''
         if hasattr(model,is_deleted_field):
                 if not kwargs:kwargs = {}
                 if not is_deleted_field in kwargs:
                     kwargs[is_deleted_field] = False
+        
         if hasattr(model,'id'):
             
             q = self.query(func.count(model.id),*args,**kwargs)
             return q.scalar()
         else:
             return len(self.list( model,*args,**kwargs))
+        
     @classmethod
     def get(self,model:Base,id:int)->Base:
         return self.session().get(model,id)
     @classmethod
     def add(self,model:Union[Type,Base],**kwargs)->Base:
         if isinstance(model,Base):
             m=model
```

### Comparing `irails-1.3.24/irails/log.py` & `irails-1.3.25/irails/log.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/midware.py` & `irails-1.3.25/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/midware_casbin.py` & `irails-1.3.25/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/midware_session.py` & `irails-1.3.25/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/mvc_router.py` & `irails-1.3.25/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/scripts/_app.py` & `irails-1.3.25/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/scripts/_controller.py` & `irails-1.3.25/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/scripts/_i18n.py` & `irails-1.3.25/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/scripts/_migrate.py` & `irails-1.3.25/irails/scripts/_migrate.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/scripts/_model.py` & `irails-1.3.25/irails/scripts/_model.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/scripts/_project.py` & `irails-1.3.25/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/scripts/_run.py` & `irails-1.3.25/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/scripts/_shell.py` & `irails-1.3.25/irails/scripts/_shell.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/scripts/_test.py` & `irails-1.3.25/irails/scripts/_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/scripts/main.py` & `irails-1.3.25/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/scripts/tpls/app/home.css.tpl` & `irails-1.3.25/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/scripts/tpls/app/home.tpl` & `irails-1.3.25/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/scripts/tpls/app/model.jinja` & `irails-1.3.25/irails/scripts/tpls/app/model.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/scripts/tpls/app/test_service.jinja` & `irails-1.3.25/irails/scripts/tpls/app/test_service.jinja`

 * *Files 6% similar despite different names*

```diff
@@ -17,9 +17,9 @@
             {% endif %}
         {%- if col!='id' %}
         obj.{{col_name}} = "new_value"
         {% endif -%}
         {% endfor -%}
         service.add(obj)
         id = obj.id
-        query_obj = service.get(id)
+        query_obj = service.get({{model_name}},id)
         self.assertEqual(obj,query_obj)
```

### Comparing `irails-1.3.24/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.3.25/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.3.25/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.3.25/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.3.25/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/scripts/tpls/project/public/error_404.html` & `irails-1.3.25/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/scripts/tpls/project/public/error_500.html` & `irails-1.3.25/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.3.25/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.3.25/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.3.25/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.3.25/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.3.25/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/unit_test.py` & `irails-1.3.25/irails/unit_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails/view.py` & `irails-1.3.25/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/irails.egg-info/PKG-INFO` & `irails-1.3.25/irails.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.24
+Version: 1.3.25
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.24/irails.egg-info/SOURCES.txt` & `irails-1.3.25/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.3.24/setup.py` & `irails-1.3.25/setup.py`

 * *Files identical despite different names*

