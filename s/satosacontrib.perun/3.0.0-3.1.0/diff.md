# Comparing `tmp/satosacontrib.perun-3.0.0.tar.gz` & `tmp/satosacontrib.perun-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satosacontrib.perun-3.0.0.tar", last modified: Wed May 10 15:01:44 2023, max compression
+gzip compressed data, was "satosacontrib.perun-3.1.0.tar", last modified: Wed May 24 08:37:42 2023, max compression
```

## Comparing `satosacontrib.perun-3.0.0.tar` & `satosacontrib.perun-3.1.0.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:01:44.492453 satosacontrib.perun-3.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1560 2023-05-09 13:18:33.000000 satosacontrib.perun-3.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      246 2023-05-10 15:01:44.492453 satosacontrib.perun-3.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      971 2023-05-10 14:44:18.000000 satosacontrib.perun-3.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:01:44.368450 satosacontrib.perun-3.0.0/satosacontrib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:18:33.000000 satosacontrib.perun-3.0.0/satosacontrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:01:44.372450 satosacontrib.perun-3.0.0/satosacontrib/perun/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:18:33.000000 satosacontrib.perun-3.0.0/satosacontrib/perun/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:01:44.392451 satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/
--rw-rw-rw-   0 root         (0) root         (0)      588 2023-05-10 14:44:18.000000 satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1677 2023-05-09 13:18:33.000000 satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/attribute_typing_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     5327 2023-05-09 13:18:33.000000 satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/auth_event_logging_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-09 13:18:33.000000 satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/cardinality_single_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     2156 2023-05-10 14:44:18.000000 satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/context_attributes_microservice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:01:44.400451 satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/idm/
--rw-rw-rw-   0 root         (0) root         (0)      387 2023-05-10 10:57:23.000000 satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/idm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5927 2023-05-10 10:57:23.000000 satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/idm/attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    11822 2023-05-10 10:57:23.000000 satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/idm/ensure_member.py
--rw-rw-rw-   0 root         (0) root         (0)    11583 2023-05-10 10:57:23.000000 satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/idm/entitlement.py
--rw-rw-rw-   0 root         (0) root         (0)     4831 2023-05-10 10:57:23.000000 satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/idm/perun_user.py
--rw-rw-rw-   0 root         (0) root         (0)    24791 2023-05-10 10:57:23.000000 satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/idm/sp_authorization.py
--rw-rw-rw-   0 root         (0) root         (0)    11491 2023-05-10 10:57:23.000000 satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/idm/update_user_ext_source.py
--rw-rw-rw-   0 root         (0) root         (0)     3840 2023-05-09 13:18:33.000000 satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/is_eligible_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     2200 2023-05-09 13:18:33.000000 satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/multi_idphint_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     1200 2023-05-09 13:18:33.000000 satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/nameid_attribute_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     3496 2023-05-09 13:18:33.000000 satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/proxystatistics_microservice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:01:44.424452 satosacontrib.perun-3.0.0/satosacontrib/perun/utils/
--rw-rw-rw-   0 root         (0) root         (0)     2042 2023-05-09 13:18:33.000000 satosacontrib.perun-3.0.0/satosacontrib/perun/utils/AuthEventLoggingDbModels.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2023-05-09 13:18:33.000000 satosacontrib.perun-3.0.0/satosacontrib/perun/utils/ConfigStore.py
--rw-rw-rw-   0 root         (0) root         (0)     4435 2023-05-09 13:18:33.000000 satosacontrib.perun-3.0.0/satosacontrib/perun/utils/CurlConnector.py
--rw-rw-rw-   0 root         (0) root         (0)     1391 2023-05-09 13:18:33.000000 satosacontrib.perun-3.0.0/satosacontrib/perun/utils/CurlConnectorInterface.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-05-09 13:18:33.000000 satosacontrib.perun-3.0.0/satosacontrib/perun/utils/PerunConstants.py
--rw-rw-rw-   0 root         (0) root         (0)     6364 2023-05-10 10:57:23.000000 satosacontrib.perun-3.0.0/satosacontrib/perun/utils/Utils.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:18:33.000000 satosacontrib.perun-3.0.0/satosacontrib/perun/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:01:44.372450 satosacontrib.perun-3.0.0/satosacontrib.perun.egg-info/
--rw-r--r--   0 root         (0) root         (0)      246 2023-05-10 15:01:44.000000 satosacontrib.perun-3.0.0/satosacontrib.perun.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1955 2023-05-10 15:01:44.000000 satosacontrib.perun-3.0.0/satosacontrib.perun.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 15:01:44.000000 satosacontrib.perun-3.0.0/satosacontrib.perun.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      179 2023-05-10 15:01:44.000000 satosacontrib.perun-3.0.0/satosacontrib.perun.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-10 15:01:44.000000 satosacontrib.perun-3.0.0/satosacontrib.perun.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-10 15:01:44.492453 satosacontrib.perun-3.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      600 2023-05-10 14:59:19.000000 satosacontrib.perun-3.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:01:44.476453 satosacontrib.perun-3.0.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:18:33.000000 satosacontrib.perun-3.0.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3496 2023-05-10 13:23:50.000000 satosacontrib.perun-3.0.0/tests/test_auth_event_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     3455 2023-05-10 14:44:18.000000 satosacontrib.perun-3.0.0/tests/test_context_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)     7500 2023-05-09 13:18:33.000000 satosacontrib.perun-3.0.0/tests/test_is_eligible_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     2531 2023-05-10 10:57:23.000000 satosacontrib.perun-3.0.0/tests/test_microservice_loader.py
--rw-rw-rw-   0 root         (0) root         (0)     3981 2023-05-10 10:57:23.000000 satosacontrib.perun-3.0.0/tests/test_perun_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    14517 2023-05-10 10:57:23.000000 satosacontrib.perun-3.0.0/tests/test_perun_ensure_member.py
--rw-rw-rw-   0 root         (0) root         (0)     7117 2023-05-10 10:57:23.000000 satosacontrib.perun-3.0.0/tests/test_perun_entitlement.py
--rw-rw-rw-   0 root         (0) root         (0)     5672 2023-05-10 10:57:23.000000 satosacontrib.perun-3.0.0/tests/test_perun_user_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)    36568 2023-05-10 10:57:23.000000 satosacontrib.perun-3.0.0/tests/test_sp_authorization_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     7291 2023-05-10 10:57:23.000000 satosacontrib.perun-3.0.0/tests/test_update_ues.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:37:42.391475 satosacontrib.perun-3.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2023-05-09 13:18:33.000000 satosacontrib.perun-3.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      246 2023-05-24 08:37:42.391475 satosacontrib.perun-3.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-05-24 08:23:21.000000 satosacontrib.perun-3.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:37:41.611456 satosacontrib.perun-3.1.0/satosacontrib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:18:33.000000 satosacontrib.perun-3.1.0/satosacontrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:37:41.611456 satosacontrib.perun-3.1.0/satosacontrib/perun/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:18:33.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:37:41.791460 satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-05-24 08:23:21.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2023-05-09 13:18:33.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/attribute_typing_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     5327 2023-05-09 13:18:33.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/auth_event_logging_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-09 13:18:33.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/cardinality_single_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     2156 2023-05-23 09:13:35.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/context_attributes_microservice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:37:41.987465 satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/idm/
+-rw-rw-rw-   0 root         (0) root         (0)      387 2023-05-10 10:57:23.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/idm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5927 2023-05-10 10:57:23.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/idm/attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    11822 2023-05-10 10:57:23.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/idm/ensure_member.py
+-rw-rw-rw-   0 root         (0) root         (0)    11583 2023-05-10 10:57:23.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/idm/entitlement.py
+-rw-rw-rw-   0 root         (0) root         (0)     4831 2023-05-10 10:57:23.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/idm/perun_user.py
+-rw-rw-rw-   0 root         (0) root         (0)    24791 2023-05-10 10:57:23.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/idm/sp_authorization.py
+-rw-rw-rw-   0 root         (0) root         (0)    11491 2023-05-10 10:57:23.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/idm/update_user_ext_source.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2023-05-24 08:23:21.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/is_banned_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3840 2023-05-09 13:18:33.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/is_eligible_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     2200 2023-05-09 13:18:33.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/multi_idphint_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     1200 2023-05-09 13:18:33.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/nameid_attribute_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3496 2023-05-09 13:18:33.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/proxystatistics_microservice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:37:42.155469 satosacontrib.perun-3.1.0/satosacontrib/perun/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     2042 2023-05-09 13:18:33.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/utils/AuthEventLoggingDbModels.py
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2023-05-09 13:18:33.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/utils/ConfigStore.py
+-rw-rw-rw-   0 root         (0) root         (0)     4435 2023-05-09 13:18:33.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/utils/CurlConnector.py
+-rw-rw-rw-   0 root         (0) root         (0)     1391 2023-05-09 13:18:33.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/utils/CurlConnectorInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-05-09 13:18:33.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/utils/PerunConstants.py
+-rw-rw-rw-   0 root         (0) root         (0)     6364 2023-05-10 10:57:23.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/utils/Utils.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:18:33.000000 satosacontrib.perun-3.1.0/satosacontrib/perun/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:37:41.611456 satosacontrib.perun-3.1.0/satosacontrib.perun.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      246 2023-05-24 08:37:41.000000 satosacontrib.perun-3.1.0/satosacontrib.perun.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2040 2023-05-24 08:37:41.000000 satosacontrib.perun-3.1.0/satosacontrib.perun.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 08:37:41.000000 satosacontrib.perun-3.1.0/satosacontrib.perun.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      192 2023-05-24 08:37:41.000000 satosacontrib.perun-3.1.0/satosacontrib.perun.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-24 08:37:41.000000 satosacontrib.perun-3.1.0/satosacontrib.perun.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-24 08:37:42.391475 satosacontrib.perun-3.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      624 2023-05-24 08:23:21.000000 satosacontrib.perun-3.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:37:42.371474 satosacontrib.perun-3.1.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:18:33.000000 satosacontrib.perun-3.1.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3496 2023-05-10 13:23:50.000000 satosacontrib.perun-3.1.0/tests/test_auth_event_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     3455 2023-05-23 09:13:35.000000 satosacontrib.perun-3.1.0/tests/test_context_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1796 2023-05-24 08:23:21.000000 satosacontrib.perun-3.1.0/tests/test_is_banned.py
+-rw-rw-rw-   0 root         (0) root         (0)     7500 2023-05-09 13:18:33.000000 satosacontrib.perun-3.1.0/tests/test_is_eligible_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     2531 2023-05-10 10:57:23.000000 satosacontrib.perun-3.1.0/tests/test_microservice_loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     3981 2023-05-10 10:57:23.000000 satosacontrib.perun-3.1.0/tests/test_perun_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    14517 2023-05-10 10:57:23.000000 satosacontrib.perun-3.1.0/tests/test_perun_ensure_member.py
+-rw-rw-rw-   0 root         (0) root         (0)     7117 2023-05-10 10:57:23.000000 satosacontrib.perun-3.1.0/tests/test_perun_entitlement.py
+-rw-rw-rw-   0 root         (0) root         (0)     5672 2023-05-10 10:57:23.000000 satosacontrib.perun-3.1.0/tests/test_perun_user_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)    36568 2023-05-10 10:57:23.000000 satosacontrib.perun-3.1.0/tests/test_sp_authorization_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     7291 2023-05-10 10:57:23.000000 satosacontrib.perun-3.1.0/tests/test_update_ues.py
```

### Comparing `satosacontrib.perun-3.0.0/LICENSE` & `satosacontrib.perun-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/README.md` & `satosacontrib.perun-3.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -13,11 +13,15 @@
 - target issuer
 
 The [MetaInfoIssuer](https://github.com/SUNET/swamid-satosa/blob/main/src/swamid_plugins/metainfo/metainfo.py)
 microservice needs to be run beforehand with the following [patch](https://github.com/SUNET/swamid-satosa/compare/main...kofzera:swamid-satosa:add_collector_metadata.patch).
 Another [patch](https://github.com/IdentityPython/SATOSA/compare/master...kofzera:SATOSA:decorate_context_with_metadata.patch) is
 also needed for the satosa package until they are incorporated into the upstream.
 
+### Is banned microservice
+
+The microservice connects to database storing user bans and redirects banned users to configured URL.
+
 ## Perun Microservices
 
 Subpackage of microservices connecting to perun. These have to be allowed (or not denied) for
 a given combination of requester/target_entity in order to run.
```

### Comparing `satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/__init__.py` & `satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from .auth_event_logging_microservice import AuthEventLogging
 from .cardinality_single_microservice import CardinalitySingle
 from .context_attributes_microservice import ContextAttributes
 from .is_eligible_microservice import IsEligible
 from .multi_idphint_microservice import MultiIdpHinting
 from .nameid_attribute_microservice import NameIDAttribute
-
+from .is_banned_microservice import IsBanned
 from .proxystatistics_microservice import ProxyStatistics
 
 
 __all__ = [
     "CardinalitySingle",
     "ContextAttributes",
     "IsEligible",
     "MultiIdpHinting",
     "NameIDAttribute",
     "ProxyStatistics",
     "AuthEventLogging",
+    "IsBanned",
 ]
```

### Comparing `satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/attribute_typing_microservice.py` & `satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/attribute_typing_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/auth_event_logging_microservice.py` & `satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/auth_event_logging_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/cardinality_single_microservice.py` & `satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/cardinality_single_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/context_attributes_microservice.py` & `satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/context_attributes_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/idm/attributes.py` & `satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/idm/attributes.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/idm/ensure_member.py` & `satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/idm/ensure_member.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/idm/entitlement.py` & `satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/idm/entitlement.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/idm/perun_user.py` & `satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/idm/perun_user.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/idm/sp_authorization.py` & `satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/idm/sp_authorization.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/idm/update_user_ext_source.py` & `satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/idm/update_user_ext_source.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/is_eligible_microservice.py` & `satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/is_eligible_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/multi_idphint_microservice.py` & `satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/multi_idphint_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/nameid_attribute_microservice.py` & `satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/nameid_attribute_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/satosacontrib/perun/micro_services/proxystatistics_microservice.py` & `satosacontrib.perun-3.1.0/satosacontrib/perun/micro_services/proxystatistics_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/satosacontrib/perun/utils/AuthEventLoggingDbModels.py` & `satosacontrib.perun-3.1.0/satosacontrib/perun/utils/AuthEventLoggingDbModels.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/satosacontrib/perun/utils/ConfigStore.py` & `satosacontrib.perun-3.1.0/satosacontrib/perun/utils/ConfigStore.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/satosacontrib/perun/utils/CurlConnector.py` & `satosacontrib.perun-3.1.0/satosacontrib/perun/utils/CurlConnector.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/satosacontrib/perun/utils/CurlConnectorInterface.py` & `satosacontrib.perun-3.1.0/satosacontrib/perun/utils/CurlConnectorInterface.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/satosacontrib/perun/utils/Utils.py` & `satosacontrib.perun-3.1.0/satosacontrib/perun/utils/Utils.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/satosacontrib.perun.egg-info/SOURCES.txt` & `satosacontrib.perun-3.1.0/satosacontrib.perun.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 satosacontrib.perun.egg-info/top_level.txt
 satosacontrib/perun/__init__.py
 satosacontrib/perun/micro_services/__init__.py
 satosacontrib/perun/micro_services/attribute_typing_microservice.py
 satosacontrib/perun/micro_services/auth_event_logging_microservice.py
 satosacontrib/perun/micro_services/cardinality_single_microservice.py
 satosacontrib/perun/micro_services/context_attributes_microservice.py
+satosacontrib/perun/micro_services/is_banned_microservice.py
 satosacontrib/perun/micro_services/is_eligible_microservice.py
 satosacontrib/perun/micro_services/multi_idphint_microservice.py
 satosacontrib/perun/micro_services/nameid_attribute_microservice.py
 satosacontrib/perun/micro_services/proxystatistics_microservice.py
 satosacontrib/perun/micro_services/idm/__init__.py
 satosacontrib/perun/micro_services/idm/attributes.py
 satosacontrib/perun/micro_services/idm/ensure_member.py
@@ -31,14 +32,15 @@
 satosacontrib/perun/utils/CurlConnectorInterface.py
 satosacontrib/perun/utils/PerunConstants.py
 satosacontrib/perun/utils/Utils.py
 satosacontrib/perun/utils/__init__.py
 tests/__init__.py
 tests/test_auth_event_logging.py
 tests/test_context_attributes.py
+tests/test_is_banned.py
 tests/test_is_eligible_microservice.py
 tests/test_microservice_loader.py
 tests/test_perun_attributes.py
 tests/test_perun_ensure_member.py
 tests/test_perun_entitlement.py
 tests/test_perun_user_microservice.py
 tests/test_sp_authorization_microservice.py
```

### Comparing `satosacontrib.perun-3.0.0/tests/test_auth_event_logging.py` & `satosacontrib.perun-3.1.0/tests/test_auth_event_logging.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/tests/test_context_attributes.py` & `satosacontrib.perun-3.1.0/tests/test_context_attributes.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/tests/test_is_eligible_microservice.py` & `satosacontrib.perun-3.1.0/tests/test_is_eligible_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/tests/test_microservice_loader.py` & `satosacontrib.perun-3.1.0/tests/test_microservice_loader.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/tests/test_perun_attributes.py` & `satosacontrib.perun-3.1.0/tests/test_perun_attributes.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/tests/test_perun_ensure_member.py` & `satosacontrib.perun-3.1.0/tests/test_perun_ensure_member.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/tests/test_perun_entitlement.py` & `satosacontrib.perun-3.1.0/tests/test_perun_entitlement.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/tests/test_perun_user_microservice.py` & `satosacontrib.perun-3.1.0/tests/test_perun_user_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/tests/test_sp_authorization_microservice.py` & `satosacontrib.perun-3.1.0/tests/test_sp_authorization_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.0.0/tests/test_update_ues.py` & `satosacontrib.perun-3.1.0/tests/test_update_ues.py`

 * *Files identical despite different names*

