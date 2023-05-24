# Comparing `tmp/irails-1.3.22.tar.gz` & `tmp/irails-1.3.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.3.22.tar", last modified: Mon May 22 15:25:11 2023, max compression
+gzip compressed data, was "irails-1.3.23.tar", last modified: Wed May 24 07:02:01 2023, max compression
```

## Comparing `irails-1.3.22.tar` & `irails-1.3.23.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 15:25:11.052415 irails-1.3.22/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.22/MANIFEST.in
--rw-rw-rw-   0        0        0     4878 2023-05-22 15:25:11.051417 irails-1.3.22/PKG-INFO
--rw-rw-rw-   0        0        0     4096 2023-05-22 07:06:26.000000 irails-1.3.22/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 15:25:10.957289 irails-1.3.22/irails/
--rw-rw-rw-   0        0        0      307 2023-05-22 15:24:45.000000 irails-1.3.22/irails/__init__.py
--rw-rw-rw-   0        0        0     4887 2023-05-21 14:33:24.000000 irails-1.3.22/irails/_i18n.py
--rw-rw-rw-   0        0        0     2878 2023-05-21 08:27:23.000000 irails-1.3.22/irails/_loader.py
--rw-rw-rw-   0        0        0     5253 2023-05-20 14:13:50.000000 irails-1.3.22/irails/_utils.py
--rw-rw-rw-   0        0        0    12042 2023-05-20 06:44:17.000000 irails-1.3.22/irails/auth.py
--rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.22/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-22 15:25:10.966666 irails-1.3.22/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-22 15:25:10.967664 irails-1.3.22/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.22/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10589 2023-05-13 05:03:07.000000 irails-1.3.22/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.22/irails/cbv.py
--rw-rw-rw-   0        0        0     6174 2023-05-19 07:06:13.000000 irails-1.3.22/irails/config.py
--rw-rw-rw-   0        0        0    12478 2023-05-12 05:56:24.000000 irails-1.3.22/irails/controller_utils.py
--rw-rw-rw-   0        0        0    24918 2023-05-19 11:59:51.000000 irails-1.3.22/irails/core.py
--rw-rw-rw-   0        0        0    15980 2023-05-22 15:23:58.000000 irails-1.3.22/irails/database.py
--rw-rw-rw-   0        0        0     1459 2023-05-11 15:27:11.000000 irails-1.3.22/irails/log.py
--rw-rw-rw-   0        0        0     8736 2023-05-21 14:38:31.000000 irails-1.3.22/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.22/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.22/irails/midware_session.py
--rw-rw-rw-   0        0        0     4208 2023-05-16 08:12:27.000000 irails-1.3.22/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-05-22 15:25:10.980629 irails-1.3.22/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.22/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.22/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.22/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.22/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.22/irails/scripts/_migrate.py
--rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.22/irails/scripts/_model.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.22/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1600 2023-05-11 15:45:21.000000 irails-1.3.22/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.22/irails/scripts/_shell.py
--rw-rw-rw-   0        0        0     4930 2023-05-21 14:27:15.000000 irails-1.3.22/irails/scripts/_test.py
--rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.22/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-22 15:25:10.923380 irails-1.3.22/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-22 15:25:10.994143 irails-1.3.22/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.22/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.22/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.22/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.22/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.22/irails/scripts/tpls/app/model.jinja
--rw-rw-rw-   0        0        0     1300 2023-05-20 14:09:55.000000 irails-1.3.22/irails/scripts/tpls/app/service.jinja
--rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.22/irails/scripts/tpls/app/test_controller.jinja
--rw-rw-rw-   0        0        0      893 2023-05-14 14:08:50.000000 irails-1.3.22/irails/scripts/tpls/app/test_service.jinja
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.22/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-22 15:25:10.996140 irails-1.3.22/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.22/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-22 15:25:10.997137 irails-1.3.22/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.22/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 15:25:11.010010 irails-1.3.22/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.22/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.22/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.22/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.22/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.22/irails/scripts/tpls/project/configs/casbin-model.conf
-drwxrwxrwx   0        0        0        0 2023-05-22 15:25:11.022980 irails-1.3.22/irails/scripts/tpls/project/configs/casbin_templates/
--rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.22/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
--rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.22/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
--rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.22/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
--rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.22/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
--rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.22/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
--rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.22/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
--rw-rw-rw-   0        0        0      274 2023-05-18 07:46:03.000000 irails-1.3.22/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
--rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.22/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
--rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.22/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
--rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.22/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.22/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.22/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.22/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.22/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-05-22 15:25:10.928367 irails-1.3.22/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-05-22 15:25:11.026985 irails-1.3.22/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.22/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.22/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.22/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.22/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-22 15:25:11.029789 irails-1.3.22/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.22/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.22/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-22 15:25:11.032161 irails-1.3.22/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-22 15:25:10.931360 irails-1.3.22/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-22 15:25:11.039423 irails-1.3.22/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.22/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-22 15:25:11.044357 irails-1.3.22/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.22/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.22/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.22/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-22 15:25:10.932356 irails-1.3.22/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-22 15:25:11.046940 irails-1.3.22/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.22/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     1052 2023-05-21 13:45:32.000000 irails-1.3.22/irails/unit_test.py
--rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.22/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-22 15:25:10.964669 irails-1.3.22/irails.egg-info/
--rw-rw-rw-   0        0        0     4878 2023-05-22 15:25:10.000000 irails-1.3.22/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3115 2023-05-22 15:25:10.000000 irails-1.3.22/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 15:25:10.000000 irails-1.3.22/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-22 15:25:10.000000 irails-1.3.22/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      360 2023-05-22 15:25:10.000000 irails-1.3.22/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-22 15:25:10.000000 irails-1.3.22/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 15:25:11.052415 irails-1.3.22/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.22/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:02:01.927848 irails-1.3.23/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.23/MANIFEST.in
+-rw-rw-rw-   0        0        0     4878 2023-05-24 07:02:01.926850 irails-1.3.23/PKG-INFO
+-rw-rw-rw-   0        0        0     4096 2023-05-22 07:06:26.000000 irails-1.3.23/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 07:02:01.806564 irails-1.3.23/irails/
+-rw-rw-rw-   0        0        0      307 2023-05-24 07:01:44.000000 irails-1.3.23/irails/__init__.py
+-rw-rw-rw-   0        0        0     4887 2023-05-21 14:33:24.000000 irails-1.3.23/irails/_i18n.py
+-rw-rw-rw-   0        0        0     2878 2023-05-21 08:27:23.000000 irails-1.3.23/irails/_loader.py
+-rw-rw-rw-   0        0        0     5253 2023-05-20 14:13:50.000000 irails-1.3.23/irails/_utils.py
+-rw-rw-rw-   0        0        0    12042 2023-05-20 06:44:17.000000 irails-1.3.23/irails/auth.py
+-rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.23/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:02:01.820527 irails-1.3.23/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-24 07:02:01.821524 irails-1.3.23/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.23/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10589 2023-05-13 05:03:07.000000 irails-1.3.23/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.23/irails/cbv.py
+-rw-rw-rw-   0        0        0     6174 2023-05-19 07:06:13.000000 irails-1.3.23/irails/config.py
+-rw-rw-rw-   0        0        0    12478 2023-05-12 05:56:24.000000 irails-1.3.23/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    24918 2023-05-19 11:59:51.000000 irails-1.3.23/irails/core.py
+-rw-rw-rw-   0        0        0    19789 2023-05-24 06:52:31.000000 irails-1.3.23/irails/database.py
+-rw-rw-rw-   0        0        0     1459 2023-05-11 15:27:11.000000 irails-1.3.23/irails/log.py
+-rw-rw-rw-   0        0        0     8736 2023-05-21 14:38:31.000000 irails-1.3.23/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.23/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.23/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4208 2023-05-16 08:12:27.000000 irails-1.3.23/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:02:01.838066 irails-1.3.23/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.23/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.23/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.23/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.23/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.23/irails/scripts/_migrate.py
+-rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.23/irails/scripts/_model.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.23/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1600 2023-05-11 15:45:21.000000 irails-1.3.23/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.23/irails/scripts/_shell.py
+-rw-rw-rw-   0        0        0     4930 2023-05-21 14:27:15.000000 irails-1.3.23/irails/scripts/_test.py
+-rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.23/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:02:01.760921 irails-1.3.23/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-24 07:02:01.854024 irails-1.3.23/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.23/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.23/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.23/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.23/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.23/irails/scripts/tpls/app/model.jinja
+-rw-rw-rw-   0        0        0     1300 2023-05-20 14:09:55.000000 irails-1.3.23/irails/scripts/tpls/app/service.jinja
+-rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.23/irails/scripts/tpls/app/test_controller.jinja
+-rw-rw-rw-   0        0        0      893 2023-05-14 14:08:50.000000 irails-1.3.23/irails/scripts/tpls/app/test_service.jinja
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.23/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-24 07:02:01.856018 irails-1.3.23/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.23/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-24 07:02:01.859014 irails-1.3.23/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.23/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:02:01.873971 irails-1.3.23/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.23/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.23/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.23/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.23/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.23/irails/scripts/tpls/project/configs/casbin-model.conf
+drwxrwxrwx   0        0        0        0 2023-05-24 07:02:01.889928 irails-1.3.23/irails/scripts/tpls/project/configs/casbin_templates/
+-rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.23/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
+-rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.23/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
+-rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.23/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
+-rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.23/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
+-rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.23/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
+-rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.23/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
+-rw-rw-rw-   0        0        0      274 2023-05-18 07:46:03.000000 irails-1.3.23/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
+-rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.23/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
+-rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.23/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
+-rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.23/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.23/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.23/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.23/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.23/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-05-24 07:02:01.767902 irails-1.3.23/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-05-24 07:02:01.894915 irails-1.3.23/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.23/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.23/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.23/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.23/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:02:01.898917 irails-1.3.23/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.23/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.23/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-24 07:02:01.901915 irails-1.3.23/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-24 07:02:01.770903 irails-1.3.23/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-24 07:02:01.908860 irails-1.3.23/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.23/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-24 07:02:01.920131 irails-1.3.23/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.23/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.23/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.23/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-24 07:02:01.771893 irails-1.3.23/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-24 07:02:01.922858 irails-1.3.23/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.23/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     1585 2023-05-24 07:01:16.000000 irails-1.3.23/irails/unit_test.py
+-rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.23/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-24 07:02:01.818532 irails-1.3.23/irails.egg-info/
+-rw-rw-rw-   0        0        0     4878 2023-05-24 07:02:01.000000 irails-1.3.23/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3115 2023-05-24 07:02:01.000000 irails-1.3.23/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 07:02:01.000000 irails-1.3.23/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-24 07:02:01.000000 irails-1.3.23/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      360 2023-05-24 07:02:01.000000 irails-1.3.23/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-24 07:02:01.000000 irails-1.3.23/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 07:02:01.927848 irails-1.3.23/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.23/setup.py
```

### Comparing `irails-1.3.22/PKG-INFO` & `irails-1.3.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.22
+Version: 1.3.23
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.22/README.md` & `irails-1.3.23/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/_i18n.py` & `irails-1.3.23/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/_loader.py` & `irails-1.3.23/irails/_loader.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/_utils.py` & `irails-1.3.23/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/auth.py` & `irails-1.3.23/irails/auth.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/base_controller.py` & `irails-1.3.23/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.3.23/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.3.23/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/cbv.py` & `irails-1.3.23/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/config.py` & `irails-1.3.23/irails/config.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/controller_utils.py` & `irails-1.3.23/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/core.py` & `irails-1.3.23/irails/core.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/database.py` & `irails-1.3.23/irails/database.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import configparser
 import re,os,sys
-from typing import Any, Dict, List, Type, Union, overload
+from typing import Any, Dict, List, Tuple, Type, Union, overload
 from contextlib import contextmanager
-from sqlalchemy import (DateTime, Integer, 
+from sqlalchemy import (Boolean, DateTime, Integer, 
                         String, Text, 
                         create_engine,
                         Engine,
                         MetaData, 
                         Table, 
                         Column, 
                         ForeignKey, 
@@ -48,42 +48,34 @@
 
  
 DataMap = None
 mapped_base = None
 engine:Engine=None 
 table_prefix=""
 cfg = config.get("database")
+is_deleted_field = 'is_deleted'
+i18n_json_data_field = 'i18n_json_data'
+page_size = 20
 if cfg:
     table_prefix = cfg.get("table_prefix","")
-
+    page_size = int(cfg.get("page_size",20))
+    if page_size<0 :
+        page_size=20
+    is_deleted_field = cfg.get("is_deleted_field",'is_deleted')
+    i18n_json_data_field = cfg.get("i18n_json_data_field",'i18n_json_data')
  
 class Base( DeclarativeBase ):
-    __abstract__ = True
-    update_at = Column(DateTime(timezone=True), server_default=func.now(), onupdate=func.now())
-    create_at = Column(DateTime(timezone=True), server_default=func.now())
-    #i18n_json_data={
-    #       'col1':{
-    #           'en':'bruce',
-    #           'zh':'布鲁斯'
-    #       },
-    #       'col2':{
-    #           'en':'hellow',
-    #           'zh':'你好'
-    #       },
-    #       ....
-    # 
-    # }
-    i18n_json_data = Column(Text,server_default='{}',info={'json':True})
+    __abstract__ = True 
     def __init_subclass__(cls,*args,**kwargs) -> None: 
         for e in EVENTS:
             if hasattr(cls,e):
                 event.listen(cls, e, getattr(cls,e)) 
         set_module_i18n(cls,cls.__module__)
         super().__init_subclass__(*args,**kwargs)
-class Relations():
+class Schemes():
     __all = {}
     @classmethod
     def M2M(self,Tb1:Base,Tb2:Base):
         '''
         set many to many relationship on :Tb1 and :Tb2\n
         :Tb1 will added attribute tb2_tablename(if it's not setted)\n
         :Tb2 will added attribute tb1_tablename(if it's not setted)\n
@@ -96,123 +88,208 @@
         '''
         tb2 = get_plural_name(Tb2.__name__.lower())
         tb1 = get_plural_name(Tb1.__name__.lower())
         tb1_naked_name = get_singularize_name(Tb1.__tablename__.replace(table_prefix,""))
         tb2_naked_name = get_singularize_name(Tb2.__tablename__.replace(table_prefix,""))
         m2m_table_name = f"{table_prefix}{tb1_naked_name}_{tb2_naked_name}"
         m2m_table = Table(m2m_table_name, Base.metadata,
-        Column(f'{tb1_naked_name}_id', Integer, ForeignKey(f'{Tb1.__tablename__}.id'), primary_key=True),
-        Column(f'{tb2_naked_name}_id', Integer, ForeignKey(f'{Tb2.__tablename__}.id'), primary_key=True)
+            Column(f'{tb1_naked_name}_id', Integer, ForeignKey(f'{Tb1.__tablename__}.id'), primary_key=True  ),
+            Column(f'{tb2_naked_name}_id', Integer, ForeignKey(f'{Tb2.__tablename__}.id'), primary_key=True) 
         ) 
-        setattr(Tb1,f"{tb2}",relationship(Tb2.__name__, secondary=m2m_table, back_populates=f"{tb1}"))
-        setattr(Tb2,f"{tb1}",relationship(Tb1.__name__, secondary=m2m_table, back_populates=f"{tb2}"))
+        setattr(Tb1,f"{tb2}",relationship(Tb2.__name__, secondary=m2m_table, back_populates=f"{tb1}",passive_deletes=False  ))
+        setattr(Tb2,f"{tb1}",relationship(Tb1.__name__, secondary=m2m_table, back_populates=f"{tb2}",passive_deletes=False ))
         self.__all[f"M2M{tb1}{tb2}"] = m2m_table
         return m2m_table
     @classmethod
-    def M2O(self,Tb1:Base,Tb2:Base):
+    def M2O(self, ChildTable: Base, ParentTable: Base):
         '''set 
-            :Tb1 belongs to :Tb2
-            and :Tb2 hasmany :Tb1
+        :ChildTable belongs to :ParentTable
+        and :ParentTable hasmany :ChildTable
         '''
-        _tb1s = Tb1.__tablename__
-        _tb2s = Tb2.__tablename__
-        tb1 = get_singularize_name(_tb1s)
-        tb2 = get_singularize_name(_tb2s)
-        
-        if not hasattr(Tb1, f"{tb2}_id"):
-            setattr(Tb1, f"{tb2}_id",Column(Integer, ForeignKey(f'{tb2}.id'))) 
-        if not hasattr(Tb1,f"{tb2}"):
-            setattr(Tb1,f"{tb2}",relationship(f'{tb1}',back_populates=f'{tb2}'))
-        if not hasattr(Tb2,tb1):
-            setattr(Tb2,tb1,relationship(tb1,back_populates=tb2))
-        return Tb1,Tb2
-    pass
+        child_tablename = ChildTable.__tablename__
+        parent_tablename = ParentTable.__tablename__
+        child_tbname = get_singularize_name(child_tablename)
+        parent_tbname = get_singularize_name(parent_tablename)
+
+        setattr(ChildTable, f"{parent_tbname}_id", Column(Integer, ForeignKey(f'{parent_tbname}.id')))
+        setattr(ChildTable, f"{parent_tbname}", relationship(ParentTable.__name__, back_populates=f'{child_tbname}'))
+
+        setattr(ParentTable, child_tbname, relationship(ChildTable.__name__, back_populates=f'{parent_tbname}', cascade='delete,all'))
+        return ChildTable, ParentTable
+
+    @classmethod
+    def SOFT_DELETE(self,*tables):
+        """
+        set a `is_deleted` field on :tables
+        please use irails.service to query ,it will auto add the 'is_deleted' flag
+        """
+        for Tb in tables:
+            setattr(Tb,is_deleted_field,Column(Boolean, default=False))
+    @classmethod
+    def ADD_I18N(self,*tables):
+        #i18n_json_data={
+        #       'col1':{
+        #           'en':'bruce',
+        #           'zh':'布鲁斯'
+        #       },
+        #       'col2':{
+        #           'en':'hellow',
+        #           'zh':'你好'
+        #       },
+        #       ....
+        # 
+        # }
+        for tb in tables:
+            setattr(tb,i18n_json_data_field,Column(Text,server_default='{}',info={'json':True}))
+
+    @classmethod
+    def TIMESTAMPS(self,*tables):
+        '''add timestamp(update_at,create_at) field on :tables'''
+        for tb in tables:
+            tb.update_at = Column(DateTime(timezone=True), server_default=func.now(), onupdate=func.now())
+            tb.create_at = Column(DateTime(timezone=True), server_default=func.now())        
 class InitDbError(Exception):
     pass
 
 
 
  
 class _serviceMeta(type):
     def __new__(cls, name, bases, attrs):
         obj = super().__new__(cls, name, bases, attrs)
         if obj.__name__!="Service":
             set_module_i18n(obj=obj,module_name=attrs['__module__'])
          
         return obj
-
+class ListPager:
+    def __init__(self,query:Query,size:int=None ) -> None: 
+        self.query = query
+        if size:
+            self.page_size = size
+        else:
+            self.page_size = page_size 
+         
+    def count(self)->int:
+        return self.query.count()
+    def page_count(self)->int:
+        import math
+        return math.ceil(self.count()/self.page_size)
+    
+    def page(self,current=1)->Query:
+        return self.query.limit(self.page_size).offset(self.page_size*(current-1))
+    def get(self,current=1)->List[Base]:
+        return self.query.limit(self.page_size).offset(self.page_size*(current-1)).all()
 class Service(metaclass=_serviceMeta):
     __all_generated = {}
      
     _ = _ #the i18n traslation object ,it's will auto redirect the `app_name/locales` dir i18n configure
-    
+    @contextmanager      
+    @staticmethod 
+    def get_session():
+        """Provide a transactional scope around a series of operations."""
+        if not  engine:
+            yield None
+            return
+        if hasattr(Service,"_session"):
+            session = Service._session
+        else:
+            if hasattr(Service,'_session_local'):
+                session_local = getattr(Service,'_session_local')
+            else:
+                session_local =  sessionmaker(bind=engine)
+                setattr(Service,"_session_local", session_local) #cache sessionmaker object
+            session = session_local()
+            setattr(Service,"_session",session)
+         
+        try:
+            yield session
+            session.commit()
+        except Exception as e:
+            session.rollback()
+            raise e
+        # finally:
+        #     session.close()
     @classmethod
     def session(self)->Session:
         if hasattr(self,"_session"):
             return self._session
         if hasattr(self,'_session_local'):
             session_local = getattr(self,'_session_local')
         else:
             session_local =  sessionmaker(bind=engine)
             setattr(self,"_session_local", session_local) #cache sessionmaker object
         session = session_local()
         setattr(self,"_session",session)
         return session
      
-    # @classmethod
-    # def query(self, *entities: _ColumnsClauseArgument[Any], **kwargs: Any)->Query:
-    #     """get query object"""
-    #     session = self.session()   
-    #     return  session.query(*entities,**kwargs)  
+    @classmethod
+    def pager(self,model:Base,*args,**kwargs)->ListPager:
+        """get query object with auto passed is_deleted rows"""
+
+        query = self.query(model,*args,**kwargs)
+        return ListPager(query=query)
      
     @classmethod
     def query(self,model:Base,*args,**kwargs)->Query:
+        '''Get a query object with auto passed is_deleted rows'''
         session = self.session()
+        if hasattr(model,is_deleted_field):
+            if not kwargs:kwargs = {}
+            if not is_deleted_field in kwargs:
+                kwargs[is_deleted_field] = False
         query = session.query(model).filter(*args).filter_by(**kwargs)
         return query
+    
     @classmethod
-    def insert(self,model:Base,**values)->int:
-        '''
-            execute insert :model with :values 
-            :return rowcount
+    def select(self,model:Base,*where,**kwargs)->List[Base]:
+        ''' Auto pass if row has is_deleted field
+            execute select statement with :where condition on :model
+            :return rows of result
         '''
-        stmt = insert(model).values(**values)
+        if hasattr(model,is_deleted_field):
+            if not kwargs:kwargs = {}
+            if not is_deleted_field in kwargs:
+                kwargs[is_deleted_field] = False
+        stmt = select(model).where(*where).filter_by(**kwargs)
         with engine.begin() as conn:
             ret = conn.execute(stmt)
-            conn.commit()
-            return ret.rowcount
+            return ret.fetchall()     
     @classmethod
     def update(self,model:Base,*where,**values)->int:
         '''
             execute update :model with :values on :model by :where
             :return rowcount
         '''
-        stmt = update(model).where(*where).values(**values)
-        with  engine.begin() as conn:
-            return conn.execute(stmt).rowcount
-    @classmethod
-    def select(self,model:Base,*where)->List[Base]:
-        '''
-            execute select statement with :where condition on :model
-            :return rows of result
-        '''
-        stmt = select(model).where(*where)
-        with engine.begin() as conn:
-            ret = conn.execute(stmt)
-            return ret.fetchall()     
-    
+        q = self.query(model,*where) 
+        cnt = 0
+        for r in q:
+            for field in values:
+                setattr(r,field,values[field]) 
+            cnt+=1
+        try:
+            self.session().commit()
+        except Exception as e:
+            self.session().rollback()
+            raise e
+        return cnt
     @classmethod
-    def count(self,model:Base,*args)->int:
-        '''
+    def count(self,model:Base,*args,**kwargs)->int:
+        ''' Auto pass if row has is_deleted field
             :return count by givened :args on :model
         '''
+        if hasattr(model,is_deleted_field):
+                if not kwargs:kwargs = {}
+                if not is_deleted_field in kwargs:
+                    kwargs[is_deleted_field] = False
         if hasattr(model,'id'):
-            return self.session().query(func.count(model.id)).filter(*args).scalar()
+            
+            q = self.query(func.count(model.id),*args,**kwargs)
+            return q.scalar()
         else:
-            return len(self.list( model,*args))
+            return len(self.list( model,*args,**kwargs))
     @classmethod
     def get(self,model:Base,id:int)->Base:
         return self.session().get(model,id)
     @classmethod
     def add(self,model:Union[Type,Base],**kwargs)->Base:
         if isinstance(model,Base):
             m=model
@@ -223,64 +300,74 @@
             session = self.session()
             session.add(m)
             session.commit()
             session.merge(m,load=False)
             return m
         return None
     @classmethod
+    def add_all(self,values:List['Base']):
+        
+        session = self.session()  
+        session.add_all(values)
+        session.commit()
+             
+
+    @classmethod
     def list(self,model:Base,*args, **kwargs)->List[Base]:
+        '''Auto pass is_deleted if model has is_deleted field'''
+        if hasattr(model,is_deleted_field):
+            if not kwargs:kwargs = {}
+            if not is_deleted_field in kwargs:
+                kwargs[is_deleted_field] = False
         session = self.session()  
         query = session.query(model) 
         if args:
             query = query.filter(*args)
         if kwargs:
             query = query.filter_by(**kwargs) 
         return query.all()
     
     
     @classmethod
-    def delete(self,model:Base,*args,**kwargs)->int:
-        query = self.query(model,*args,**kwargs)
+    def delete(self,model:Base,*args,**kwargs)->int:  
+        '''Soft delete if model has is_deleted field Else real delete'''
+        with self.get_session() as session:
+            query = session.query(model).filter(*args).filter_by(**kwargs)
+            rows = query.all()
+            if hasattr(model,is_deleted_field): 
+                for row in rows:
+                    setattr(row,is_deleted_field,True)  
+            else:
+                for row in rows:
+                    session.delete(row)
+            cnt = len(rows)
+            session.commit()
+            return cnt
+    @classmethod
+    def real_delete(self,model:Base,*args,**kwargs):
+        '''Real delete rows in database'''
+        with self.get_session() as session: 
+            query = session.query(model).filter(*args).filter_by(**kwargs)
+            cnt = 0
+            for obj in query:
+                session.delete(obj)
+                cnt += 1
          
-        cnt = query.delete()
-        
-        self.session().commit()
-        return cnt
-    
+            return cnt
+
     @classmethod
     def flush(self,model:Base=None):
         session = self.session()
         if not model:
             return session.commit()
         if not model in session:
             session.merge(model)
         session.commit()
-         
-    @classmethod
-    @contextmanager 
-    def get_session(cls):
-        """Provide a transactional scope around a series of operations."""
-        if not  engine:
-            yield None
-            return
-        if hasattr(cls,'_session_local'):
-            session_local = getattr(cls,'_session_local')
-        else:
-            session_local =  sessionmaker(bind=engine)
-            setattr(cls,"_session_local", session_local) #cache sessionmaker object
-        session = session_local()
-         
-        try:
-            yield session
-            session.commit()
-        except Exception as e:
-            session.rollback()
-            raise e
-        finally:
-            session.close()
+
+    
     @classmethod
     def execute(cls,cmd:Union[str,TextClause],**kwargs):
         if not isinstance(cmd,TextClause):
             cmd = text(str)
         with engine.begin() as conn:
             ret = conn.execute(cmd,**kwargs)
         return ret
@@ -377,15 +464,15 @@
     else:
         command.downgrade(alembic_cfg,"-1")
 def _test_connection():
     #test connect
     try:
         with engine.connect() as conn:
             _log.disabled = False
-            _log.debug(_('database connection successed:') + str(conn))
+            _log.debug(_('database connection successed:')) 
 
     except Exception as e:
         _log.disabled = False
         _log.error(_("database connection failed!"))  
         raise
         exit(1)  
 def init_database(uri: str, debug: bool = False, cfg=None):
```

### Comparing `irails-1.3.22/irails/log.py` & `irails-1.3.23/irails/log.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/midware.py` & `irails-1.3.23/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/midware_casbin.py` & `irails-1.3.23/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/midware_session.py` & `irails-1.3.23/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/mvc_router.py` & `irails-1.3.23/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/_app.py` & `irails-1.3.23/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/_controller.py` & `irails-1.3.23/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/_i18n.py` & `irails-1.3.23/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/_migrate.py` & `irails-1.3.23/irails/scripts/_migrate.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/_model.py` & `irails-1.3.23/irails/scripts/_model.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/_project.py` & `irails-1.3.23/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/_run.py` & `irails-1.3.23/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/_shell.py` & `irails-1.3.23/irails/scripts/_shell.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/_test.py` & `irails-1.3.23/irails/scripts/_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/main.py` & `irails-1.3.23/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/tpls/app/home.css.tpl` & `irails-1.3.23/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/tpls/app/home.tpl` & `irails-1.3.23/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/tpls/app/model.jinja` & `irails-1.3.23/irails/scripts/tpls/app/model.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/tpls/app/service.jinja` & `irails-1.3.23/irails/scripts/tpls/app/service.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/tpls/app/test_service.jinja` & `irails-1.3.23/irails/scripts/tpls/app/test_service.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.3.23/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.3.23/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.3.23/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.3.23/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/tpls/project/public/error_404.html` & `irails-1.3.23/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/tpls/project/public/error_500.html` & `irails-1.3.23/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.3.23/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.3.23/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.3.23/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.3.23/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.3.23/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails/unit_test.py` & `irails-1.3.23/irails/unit_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,43 @@
 
 import unittest
+
+
 from .core import generate_mvc_app
 from ._i18n import set_module_i18n
 
 class _BaseUnitTest(unittest.TestCase):
-    application = generate_mvc_app()
+    
     def __init__(self,*args,**kwargv) -> None:
         super().__init__(*args,**kwargv)
     def __init_subclass__(cls,*args,**kwargs) -> None:  
         set_module_i18n(cls,cls.__module__)
         super().__init_subclass__(*args,**kwargs)    
 class ControllerTest(_BaseUnitTest):
+    
     def __init__(self,*args,**kwargv) -> None:
         super().__init__(*args,**kwargv)
+        if not hasattr(_BaseUnitTest,'application'):
+            _BaseUnitTest.application = generate_mvc_app()
         from fastapi.testclient import TestClient 
         self.client = TestClient(app=self.application)
         
     pass
 
 class ServiceTest(_BaseUnitTest):
     def __init__(self,*args,**kwargv) -> None:
         super().__init__(*args,**kwargv)
-        from irails.database import Service,engine,Session
-        self.service = Service
-        self.engine = engine
-        if not hasattr(ServiceTest,'session'):
-            ServiceTest.session = Session(bind=self.engine)
-        
+        from .config import config
+        from ._loader import _load_apps
+        from irails.database import Service,engine,Session,init_database
+        from irails.database import check_migration
+         
+        # _load_apps()
+        if not hasattr(ServiceTest,'engine'):
+            db_cfg = config.get("database")
+            db_uri = db_cfg.get("uri")
+            alembic_ini = db_cfg.get("alembic_ini")
+            ServiceTest.engine = init_database(db_uri,debug=True,cfg = db_cfg)
+            if ServiceTest.engine:
+                check_migration(engine=ServiceTest.engine,uri= db_uri,alembic_ini= alembic_ini )
+            ServiceTest.service = Service 
     pass
```

### Comparing `irails-1.3.22/irails/view.py` & `irails-1.3.23/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/irails.egg-info/PKG-INFO` & `irails-1.3.23/irails.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.22
+Version: 1.3.23
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.22/irails.egg-info/SOURCES.txt` & `irails-1.3.23/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.3.22/setup.py` & `irails-1.3.23/setup.py`

 * *Files identical despite different names*

