# Comparing `tmp/plurk.py-0.0.1.tar.gz` & `tmp/plurk.py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plurk.py-0.0.1.tar", last modified: Sat May 13 06:41:21 2023, max compression
+gzip compressed data, was "plurk.py-0.0.2.tar", last modified: Wed May 24 16:40:26 2023, max compression
```

## Comparing `plurk.py-0.0.1.tar` & `plurk.py-0.0.2.tar`

### file list

```diff
@@ -1,75 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:41:21.915946 plurk.py-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-13 06:41:08.000000 plurk.py-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-13 06:41:21.915946 plurk.py-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-13 06:41:08.000000 plurk.py-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-13 06:41:08.000000 plurk.py-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-13 06:41:21.919946 plurk.py-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-13 06:41:09.000000 plurk.py-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:41:21.903946 plurk.py-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:41:21.903946 plurk.py-0.0.1/src/plurk/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:41:21.907946 plurk.py-0.0.1/src/plurk/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/apis/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/apis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/apis/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/apis/cliques.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/apis/emoticons.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/apis/friends_fans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/apis/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/apis/plurk_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/apis/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/apis/realtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/apis/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)    14716 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/apis/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/apis/user_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/apis/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:41:21.911946 plurk.py-0.0.1/src/plurk/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/enums/abuse_category.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/enums/alert_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/enums/avatar_size.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/enums/channel_data_entry_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/enums/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/enums/language.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/enums/privacy.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/enums/qualifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/enums/relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:41:21.915946 plurk.py-0.0.1/src/plurk/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/models/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/models/general_resps.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/models/karma_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/models/plurk.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/models/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/models/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/models/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/models/user_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/models/user_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-13 06:41:09.000000 plurk.py-0.0.1/src/plurk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:41:21.907946 plurk.py-0.0.1/src/plurk.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-13 06:41:21.000000 plurk.py-0.0.1/src/plurk.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-13 06:41:21.000000 plurk.py-0.0.1/src/plurk.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 06:41:21.000000 plurk.py-0.0.1/src/plurk.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-13 06:41:21.000000 plurk.py-0.0.1/src/plurk.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-13 06:41:21.000000 plurk.py-0.0.1/src/plurk.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 06:41:21.000000 plurk.py-0.0.1/src/plurk.py.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 06:41:21.915946 plurk.py-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-13 06:41:09.000000 plurk.py-0.0.1/tests/test_apis_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-13 06:41:09.000000 plurk.py-0.0.1/tests/test_apis_cliques.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-13 06:41:09.000000 plurk.py-0.0.1/tests/test_apis_emoticons.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-05-13 06:41:09.000000 plurk.py-0.0.1/tests/test_apis_friends_fans.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-13 06:41:09.000000 plurk.py-0.0.1/tests/test_apis_plurk_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-13 06:41:09.000000 plurk.py-0.0.1/tests/test_apis_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-13 06:41:09.000000 plurk.py-0.0.1/tests/test_apis_realtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-13 06:41:09.000000 plurk.py-0.0.1/tests/test_apis_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-05-13 06:41:09.000000 plurk.py-0.0.1/tests/test_apis_timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-13 06:41:09.000000 plurk.py-0.0.1/tests/test_apis_user_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-13 06:41:09.000000 plurk.py-0.0.1/tests/test_apis_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-13 06:41:09.000000 plurk.py-0.0.1/tests/test_oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:40:26.639647 plurk.py-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-24 16:40:15.000000 plurk.py-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-24 16:40:26.639647 plurk.py-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-24 16:40:15.000000 plurk.py-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-24 16:40:15.000000 plurk.py-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-24 16:40:26.639647 plurk.py-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-24 16:40:15.000000 plurk.py-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:40:26.627647 plurk.py-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:40:26.627647 plurk.py-0.0.2/src/plurk/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:40:26.631646 plurk.py-0.0.2/src/plurk/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/apis/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/apis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/apis/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/apis/cliques.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/apis/emoticons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/apis/friends_fans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/apis/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/apis/plurk_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/apis/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/apis/realtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/apis/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14460 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/apis/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/apis/user_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/apis/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:40:26.635646 plurk.py-0.0.2/src/plurk/async_apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/async_apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/async_apis/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/async_apis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/async_apis/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/async_apis/cliques.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/async_apis/emoticons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/async_apis/friends_fans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/async_apis/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/async_apis/plurk_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/async_apis/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/async_apis/realtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/async_apis/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/async_apis/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/async_apis/user_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/async_apis/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/async_oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:40:26.635646 plurk.py-0.0.2/src/plurk/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/clients/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/clients/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/clients/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:40:26.635646 plurk.py-0.0.2/src/plurk/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/enums/abuse_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/enums/alert_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/enums/avatar_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/enums/channel_data_entry_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/enums/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/enums/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/enums/privacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/enums/qualifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/enums/relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:40:26.635646 plurk.py-0.0.2/src/plurk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/models/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/models/general_resps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/models/karma_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/models/plurk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/models/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/models/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/models/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/models/user_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/models/user_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-24 16:40:15.000000 plurk.py-0.0.2/src/plurk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:40:26.631646 plurk.py-0.0.2/src/plurk.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-24 16:40:26.000000 plurk.py-0.0.2/src/plurk.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-24 16:40:26.000000 plurk.py-0.0.2/src/plurk.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:40:26.000000 plurk.py-0.0.2/src/plurk.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-24 16:40:26.000000 plurk.py-0.0.2/src/plurk.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 16:40:26.000000 plurk.py-0.0.2/src/plurk.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:40:26.000000 plurk.py-0.0.2/src/plurk.py.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:40:26.639647 plurk.py-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-24 16:40:15.000000 plurk.py-0.0.2/tests/test_apis_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-24 16:40:15.000000 plurk.py-0.0.2/tests/test_apis_cliques.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-24 16:40:15.000000 plurk.py-0.0.2/tests/test_apis_emoticons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-24 16:40:15.000000 plurk.py-0.0.2/tests/test_apis_friends_fans.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-24 16:40:15.000000 plurk.py-0.0.2/tests/test_apis_plurk_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-24 16:40:15.000000 plurk.py-0.0.2/tests/test_apis_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-24 16:40:15.000000 plurk.py-0.0.2/tests/test_apis_realtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-24 16:40:15.000000 plurk.py-0.0.2/tests/test_apis_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-05-24 16:40:15.000000 plurk.py-0.0.2/tests/test_apis_timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-24 16:40:15.000000 plurk.py-0.0.2/tests/test_apis_user_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-24 16:40:15.000000 plurk.py-0.0.2/tests/test_apis_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-24 16:40:15.000000 plurk.py-0.0.2/tests/test_async_apis_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-24 16:40:15.000000 plurk.py-0.0.2/tests/test_async_apis_cliques.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-24 16:40:15.000000 plurk.py-0.0.2/tests/test_async_apis_emoticons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-05-24 16:40:15.000000 plurk.py-0.0.2/tests/test_async_apis_friends_fans.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-24 16:40:15.000000 plurk.py-0.0.2/tests/test_async_apis_plurk_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-24 16:40:15.000000 plurk.py-0.0.2/tests/test_async_apis_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-24 16:40:15.000000 plurk.py-0.0.2/tests/test_async_apis_realtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-24 16:40:15.000000 plurk.py-0.0.2/tests/test_async_apis_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-05-24 16:40:15.000000 plurk.py-0.0.2/tests/test_async_apis_timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-24 16:40:15.000000 plurk.py-0.0.2/tests/test_async_apis_user_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-24 16:40:15.000000 plurk.py-0.0.2/tests/test_async_apis_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-24 16:40:15.000000 plurk.py-0.0.2/tests/test_async_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-24 16:40:15.000000 plurk.py-0.0.2/tests/test_oauth.py
```

### Comparing `plurk.py-0.0.1/LICENSE` & `plurk.py-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/PKG-INFO` & `plurk.py-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: plurk.py
-Version: 0.0.1
-Summary: An unofficial Plurk API 2.0 SDK for Python 3.8+.
-Home-page: https://github.com/shc261392/plurk.py
-Author: James Chien
-Author-email: shc261392@gmail.com
-Keywords: plurk,oauth
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: docs
-License-File: LICENSE
-
 # plurk.py
 An unofficial library of interacting with Plurk API 2.0 for Python 3.8+.
 
 ![main](https://github.com/shc261392/plurk.py/actions/workflows/ci.yml/badge.svg?branch=main)
 
 ## Features
 
@@ -34,15 +15,15 @@
 - Python 3.8+
 
 Testing dependencies requires Python 3.8+. The package might still works for Python 3.7 though it is not recommended.
 
 ## Installation
 
 ```shell
-$ pip3 install git+https://github.com/shc261392/plurk.py
+$ pip3 install plurk.py
 ```
 
 ## Quickstart
 
 See the example below for how to use **plurk.py**.
 
 Replace the value of `APP_KEY` and `APP_SECRET` with your Plurk app's key and secret.
@@ -69,14 +50,16 @@
 
     # Access Plurk API
     user_data = client.users.me()
     print('Display name: ', user_data.display_name)
     print('Plurks created: ', user_data.plurks_count)
 ```
 
+For async example, check [here](https://github.com/shc261392/plurk.py/blob/main/examples/async_get_plurks.py).
+
 ## Development
 
 ```shell
 $ git clone git@github.com:shc261392/plurk.py.git
 $ cd plurk.py
 $ make test
 $ make install
```

### Comparing `plurk.py-0.0.1/setup.cfg` & `plurk.py-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = plurk.py
-version = 0.0.1
+version = 0.0.2
 author = James Chien
 author_email = shc261392@gmail.com
 description = An unofficial Plurk API 2.0 SDK for Python 3.8+.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = plurk, oauth
 url = https://github.com/shc261392/plurk.py
@@ -53,28 +53,30 @@
 	line-too-long,
 	missing-module-docstring,
 	missing-class-docstring,
 	missing-function-docstring,
 	too-few-public-methods,
 	too-many-public-methods,
 	too-many-arguments,
+	duplicate-code,
 
 [flake8]
 max-line-length = 120
 max-complexity = 10
 exclude = .git,__pycache__,__init__.py,.mypy_cache,.pytest_cache,venv,.venv
 
 [tox:tox]
 envlist = 
 	py37, py38, py39,py310, flake8, pylint, bandit
 
 [testenv]
 deps = 
 	coverage
 	pytest
+	pytest-asyncio
 	pytest-mock
 	pytest-httpx
 	pydantic_factories
 	-r {tox_root}/requirements.txt
 commands = 
 	coverage run -p -m pytest tests
```

### Comparing `plurk.py-0.0.1/src/plurk/apis/__init__.py` & `plurk.py-0.0.2/src/plurk/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/apis/alerts.py` & `plurk.py-0.0.2/src/plurk/apis/alerts.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/apis/blocks.py` & `plurk.py-0.0.2/src/plurk/apis/blocks.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/apis/cliques.py` & `plurk.py-0.0.2/src/plurk/apis/cliques.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/apis/emoticons.py` & `plurk.py-0.0.2/src/plurk/apis/emoticons.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/apis/friends_fans.py` & `plurk.py-0.0.2/src/plurk/apis/friends_fans.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/apis/helper.py` & `plurk.py-0.0.2/src/plurk/apis/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from plurk.models import ChannelResp
 
 
 class Helper(BaseApi):
     """The class represents the collection of helper methods build on
     existing Plurk APIs. It does not represent an API endpoint directly.
     """
+
     def subscribe_to_user_channel(self):
         """Returns a generator that yields plurks posted to the user channel.
 
         The method uses the `/APP/Realtime/getUserChannel` endpoint to get the current users channel
         and yield received results.
 
         The generator will yield results indefinitely in a `while True:` loop.
```

### Comparing `plurk.py-0.0.1/src/plurk/apis/plurk_search.py` & `plurk.py-0.0.2/src/plurk/apis/plurk_search.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/apis/profile.py` & `plurk.py-0.0.2/src/plurk/apis/profile.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/apis/realtime.py` & `plurk.py-0.0.2/src/plurk/apis/realtime.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/apis/responses.py` & `plurk.py-0.0.2/src/plurk/apis/responses.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/apis/timeline.py` & `plurk.py-0.0.2/src/plurk/apis/timeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,22 +33,22 @@
             replurkers_detail=replurkers_detail,
         )
         resp = self.client.http_client.get(endpoint, params=params)
         validate_resp(resp)
         return GetPlurkResp(**resp.json())
 
     def get_plurks(
-                self,
-                offset: Optional[Union[str, datetime]] = None,
-                limit: int = 20,
-                filter: Optional[Filter] = None,  # pylint: disable=redefined-builtin
-                favorers_detail=False,
-                limited_detail=False,
-                replurkers_detail=False,
-            ):
+        self,
+        offset: Optional[Union[str, datetime]] = None,
+        limit: int = 20,
+        filter: Optional[Filter] = None,  # pylint: disable=redefined-builtin
+        favorers_detail=False,
+        limited_detail=False,
+        replurkers_detail=False,
+    ):
         """Return plurks on timeline.
 
         Args:
             offset: return plurks older than offset, formatted as `YYYY-mm-DDTHH:MM:SS`. The function can also
                 accept a datetime object and convert it automatically to the format for the API.
             limit: how many plurks should be returned. Default: `20`.
             filter: can be `my`, `responded`, `private`, `favorite`, `replurked` or `mentioned`; `mentioned` is only
@@ -72,22 +72,22 @@
             replurkers_detail=replurkers_detail,
         )
         resp = self.client.http_client.get(endpoint, params=params)
         validate_resp(resp)
         return GetPlurksResp(**resp.json())
 
     def get_unread_plurks(
-                self,
-                offset: Optional[Union[str, datetime]] = None,
-                limit: int = 20,
-                filter: Optional[Filter] = None,  # pylint: disable=redefined-builtin
-                favorers_detail=False,
-                limited_detail=False,
-                replurkers_detail=False,
-            ):
+        self,
+        offset: Optional[Union[str, datetime]] = None,
+        limit: int = 20,
+        filter: Optional[Filter] = None,  # pylint: disable=redefined-builtin
+        favorers_detail=False,
+        limited_detail=False,
+        replurkers_detail=False,
+    ):
         """Return unread plurks on timeline.
 
         Args:
             offset: return plurks older than offset, formatted as `YYYY-mm-DDTHH:MM:SS`. The function can also
                 accept a datetime object and convert it automatically to the format for the API.
             limit: how many plurks should be returned. Default: `20`.
             filter: can be `my`, `responded`, `private`, `favorite`, `replurked` or `mentioned`; `mentioned` is only
@@ -111,23 +111,23 @@
             replurkers_detail=replurkers_detail,
         )
         resp = self.client.http_client.get(endpoint, params=params)
         validate_resp(resp)
         return GetPlurksResp(**resp.json())
 
     def get_public_plurks(
-                self,
-                user_id: Union[int, str],
-                offset: Optional[Union[str, datetime]] = None,
-                limit: int = 20,
-                filter: Optional[Filter] = None,  # pylint: disable=redefined-builtin
-                favorers_detail=False,
-                limited_detail=False,
-                replurkers_detail=False,
-            ):
+        self,
+        user_id: Union[int, str],
+        offset: Optional[Union[str, datetime]] = None,
+        limit: int = 20,
+        filter: Optional[Filter] = None,  # pylint: disable=redefined-builtin
+        favorers_detail=False,
+        limited_detail=False,
+        replurkers_detail=False,
+    ):
         """Return public plurks of a specific user on timeline.
 
         Args:
             user_id: the user_id of the public plurks owner to get, can be the unique user_id (int) or nick_name (str)
             offset: return plurks older than offset, formatted as `YYYY-mm-DDTHH:MM:SS`. The function can also
                 accept a datetime object and convert it automatically to the format for the API.
             limit: how many plurks should be returned. Default: `20`.
@@ -153,21 +153,21 @@
             replurkers_detail=replurkers_detail,
         )
         resp = self.client.http_client.get(endpoint, params=params)
         validate_resp(resp)
         return GetPlurksResp(**resp.json())
 
     def plurk_add(
-                self,
-                content: str,
-                qualifier: Qualifier = Qualifier.EMPTY,
-                limited_to: Optional[List[int]] = None,
-                no_comments: Optional[int] = None,
-                lang: Optional[Language] = None,
-            ):
+        self,
+        content: str,
+        qualifier: Qualifier = Qualifier.EMPTY,
+        limited_to: Optional[List[int]] = None,
+        no_comments: Optional[int] = None,
+        lang: Optional[Language] = None,
+    ):
         """Add a new plurk.
 
         Args:
             content: the content of the plurk.
             qualifier: the qualifier of the plurk.
             limited_to: a list of user_id. if provided, the plurk will be limited to the list of users.
             no_comments: set to 1 to disable all responses, set to 2 to restrict responses to friend-only.
```

### Comparing `plurk.py-0.0.1/src/plurk/apis/user_search.py` & `plurk.py-0.0.2/src/plurk/apis/user_search.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/apis/users.py` & `plurk.py-0.0.2/src/plurk/apis/users.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/client.py` & `plurk.py-0.0.2/src/plurk/clients/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,17 @@
-from abc import abstractmethod
 from typing import Dict, TypeVar
 
 from authlib.integrations.httpx_client import OAuth1Client
 
 from plurk import apis, oauth
+from plurk.clients.base import BaseClient
 from plurk.exceptions import validate_resp
 
-T = TypeVar('T')
-
 
-class BaseClient():
-    """Base class for clients
-    """
-    @property
-    @abstractmethod
-    def http_client_class(self):
-        pass
-
-    def __init__(self, app_key: str, app_secret: str, base_url='https://www.plurk.com'):
-        self.http_client = None
-        self.app_key = app_key
-        self.app_secret = app_secret
-        self.base_url = base_url
-        self.token = None
-        self.token_secret = None
+T = TypeVar('T')
 
 
 class Client(BaseClient):
     """Synchronous client for Plurk API
     """
     @property
     def http_client_class(self):
```

### Comparing `plurk.py-0.0.1/src/plurk/enums/language.py` & `plurk.py-0.0.2/src/plurk/enums/language.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/enums/qualifier.py` & `plurk.py-0.0.2/src/plurk/enums/qualifier.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/exceptions.py` & `plurk.py-0.0.2/src/plurk/exceptions.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/models/__init__.py` & `plurk.py-0.0.2/src/plurk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/models/alert.py` & `plurk.py-0.0.2/src/plurk/models/alert.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/models/base.py` & `plurk.py-0.0.2/src/plurk/models/base.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/models/general_resps.py` & `plurk.py-0.0.2/src/plurk/models/general_resps.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/models/karma_stats.py` & `plurk.py-0.0.2/src/plurk/models/karma_stats.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/models/plurk.py` & `plurk.py-0.0.2/src/plurk/models/plurk.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/models/profile.py` & `plurk.py-0.0.2/src/plurk/models/profile.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/models/response.py` & `plurk.py-0.0.2/src/plurk/models/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     """The response id.
     """
     lang: Language
     last_edited: Optional[datetime]
     plurk_id: int
     posted: datetime
     qualifier: Qualifier
-    qualifier_translated: str
+    qualifier_translated: Optional[str]
     user_id: int
     with_random_emos: Optional[bool]
 
     _parse_last_edited = parse_time_validator('last_edited')
     _parse_posted = parse_time_validator('posted')
```

### Comparing `plurk.py-0.0.1/src/plurk/models/timeline.py` & `plurk.py-0.0.2/src/plurk/models/timeline.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/models/user_channel.py` & `plurk.py-0.0.2/src/plurk/models/user_channel.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/models/user_data.py` & `plurk.py-0.0.2/src/plurk/models/user_data.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk/oauth.py` & `plurk.py-0.0.2/src/plurk/oauth.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 
 def get_auth_url(client: OAuth1Client, authenticate_url: str, request_token: Dict[str, str]):
     return client.create_authorization_url(authenticate_url, request_token['oauth_token'])
 
 
 def fetch_access_token(
-            client_id: str, client_secret: str, access_token_url: str,
-            request_token: Dict[str, str], oauth_verifier: str,
-        ):
+    client_id: str, client_secret: str, access_token_url: str,
+    request_token: Dict[str, str], oauth_verifier: str,
+):
     with OAuth1Client(
         client_id,
         client_secret,
         token=request_token['oauth_token'],
         token_secret=request_token['oauth_token_secret']
     ) as client:
         token = client.fetch_access_token(access_token_url, oauth_verifier)
```

### Comparing `plurk.py-0.0.1/src/plurk/utils.py` & `plurk.py-0.0.2/src/plurk/utils.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/src/plurk.py.egg-info/PKG-INFO` & `plurk.py-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plurk.py
-Version: 0.0.1
+Version: 0.0.2
 Summary: An unofficial Plurk API 2.0 SDK for Python 3.8+.
 Home-page: https://github.com/shc261392/plurk.py
 Author: James Chien
 Author-email: shc261392@gmail.com
 Keywords: plurk,oauth
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -34,15 +34,15 @@
 - Python 3.8+
 
 Testing dependencies requires Python 3.8+. The package might still works for Python 3.7 though it is not recommended.
 
 ## Installation
 
 ```shell
-$ pip3 install git+https://github.com/shc261392/plurk.py
+$ pip3 install plurk.py
 ```
 
 ## Quickstart
 
 See the example below for how to use **plurk.py**.
 
 Replace the value of `APP_KEY` and `APP_SECRET` with your Plurk app's key and secret.
@@ -69,14 +69,16 @@
 
     # Access Plurk API
     user_data = client.users.me()
     print('Display name: ', user_data.display_name)
     print('Plurks created: ', user_data.plurks_count)
 ```
 
+For async example, check [here](https://github.com/shc261392/plurk.py/blob/main/examples/async_get_plurks.py).
+
 ## Development
 
 ```shell
 $ git clone git@github.com:shc261392/plurk.py.git
 $ cd plurk.py
 $ make test
 $ make install
```

### Comparing `plurk.py-0.0.1/tests/test_apis_blocks.py` & `plurk.py-0.0.2/tests/test_apis_blocks.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/tests/test_apis_cliques.py` & `plurk.py-0.0.2/tests/test_apis_cliques.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/tests/test_apis_friends_fans.py` & `plurk.py-0.0.2/tests/test_apis_friends_fans.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         status_code=200,
         json=resp_json,
     )
     with Client(*FAKE_APP_CREDENTIALS) as client:
         resp = client.friends_fans.get_fans_by_offset(FAKE_USER_ID)
     assert isinstance(resp, List)
     assert [i.dict_original() for i in resp] == resp_json
-    
+
 
 def test_get_following_by_offset(httpx_mock: HTTPXMock, public_user_data_list_fixture: List[PublicUserData]):
     resp_json = [i.dict_original() for i in public_user_data_list_fixture]
     httpx_mock.add_response(
         status_code=200,
         json=resp_json,
     )
```

### Comparing `plurk.py-0.0.1/tests/test_apis_plurk_search.py` & `plurk.py-0.0.2/tests/test_apis_plurk_search.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/tests/test_apis_profile.py` & `plurk.py-0.0.2/tests/test_apis_profile.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/tests/test_apis_realtime.py` & `plurk.py-0.0.2/tests/test_apis_realtime.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/tests/test_apis_responses.py` & `plurk.py-0.0.2/tests/test_apis_responses.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/tests/test_apis_timeline.py` & `plurk.py-0.0.2/tests/test_apis_timeline.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/tests/test_apis_user_search.py` & `plurk.py-0.0.2/tests/test_apis_user_search.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/tests/test_apis_users.py` & `plurk.py-0.0.2/tests/test_apis_users.py`

 * *Files identical despite different names*

### Comparing `plurk.py-0.0.1/tests/test_oauth.py` & `plurk.py-0.0.2/tests/test_oauth.py`

 * *Files identical despite different names*

