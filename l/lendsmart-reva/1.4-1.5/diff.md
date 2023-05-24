# Comparing `tmp/lendsmart_reva-1.4.tar.gz` & `tmp/lendsmart_reva-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lendsmart_reva-1.4.tar", last modified: Thu May 11 12:31:41 2023, max compression
+gzip compressed data, was "lendsmart_reva-1.5.tar", last modified: Wed May 24 11:03:32 2023, max compression
```

## Comparing `lendsmart_reva-1.4.tar` & `lendsmart_reva-1.5.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.884146 lendsmart_reva-1.4/
--rw-rw-r--   0 user      (1000) user      (1000)       36 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     2823 2023-05-11 12:31:41.884146 lendsmart_reva-1.4/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2442 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.872145 lendsmart_reva-1.4/lendsmart_reva.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     2823 2023-05-11 12:31:41.000000 lendsmart_reva-1.4/lendsmart_reva.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1743 2023-05-11 12:31:41.000000 lendsmart_reva-1.4/lendsmart_reva.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-11 12:31:41.000000 lendsmart_reva-1.4/lendsmart_reva.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      448 2023-05-11 12:31:41.000000 lendsmart_reva-1.4/lendsmart_reva.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)      158 2023-05-11 12:31:41.000000 lendsmart_reva-1.4/lendsmart_reva.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        5 2023-05-11 12:31:41.000000 lendsmart_reva-1.4/lendsmart_reva.egg-info/top_level.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.876145 lendsmart_reva-1.4/reva/
--rw-rw-r--   0 user      (1000) user      (1000)       22 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1849 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/autotest.py
--rw-rw-r--   0 user      (1000) user      (1000)     3528 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/cli.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.876145 lendsmart_reva-1.4/reva/conf/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/conf/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      740 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/conf/reva.py
--rw-rw-r--   0 user      (1000) user      (1000)      953 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/document_access_control.py
--rw-rw-r--   0 user      (1000) user      (1000)     1076 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/exception.py
--rw-rw-r--   0 user      (1000) user      (1000)      954 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/info.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.876145 lendsmart_reva-1.4/reva/lib/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.876145 lendsmart_reva-1.4/reva/lib/auto/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/auto/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3988 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/auto/main.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.876145 lendsmart_reva-1.4/reva/lib/base/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/base/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1101 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/base/base.py
--rw-rw-r--   0 user      (1000) user      (1000)      948 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/base/run_query.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.880145 lendsmart_reva-1.4/reva/lib/client/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/client/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      399 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/client/builder.py
--rw-rw-r--   0 user      (1000) user      (1000)     2926 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/client/graphql_client.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.880145 lendsmart_reva-1.4/reva/lib/document_access_control/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/document_access_control/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      728 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/document_access_control/main.py
--rw-rw-r--   0 user      (1000) user      (1000)     1599 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/document_access_control/update.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.880145 lendsmart_reva-1.4/reva/lib/graphql_queries/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/graphql_queries/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      806 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/graphql_queries/document_access_control.py
--rw-rw-r--   0 user      (1000) user      (1000)      551 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/graphql_queries/loan_products.py
--rw-rw-r--   0 user      (1000) user      (1000)      944 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/graphql_queries/roles_and_permissions.py
--rw-rw-r--   0 user      (1000) user      (1000)      590 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/graphql_queries/site_settings.py
--rw-rw-r--   0 user      (1000) user      (1000)      802 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/graphql_queries/workflow.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.880145 lendsmart_reva-1.4/reva/lib/loan_productus/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/loan_productus/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      642 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/loan_productus/main.py
--rw-rw-r--   0 user      (1000) user      (1000)     1482 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/loan_productus/update.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.880145 lendsmart_reva-1.4/reva/lib/roles_and_permissions/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/roles_and_permissions/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      687 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/roles_and_permissions/main.py
--rw-rw-r--   0 user      (1000) user      (1000)     1880 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/roles_and_permissions/update.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.880145 lendsmart_reva-1.4/reva/lib/site_settings/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/site_settings/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      639 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/site_settings/main.py
--rw-rw-r--   0 user      (1000) user      (1000)     1416 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/site_settings/update.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.884146 lendsmart_reva-1.4/reva/lib/utils/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/utils/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      433 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/utils/filter_data_with_id.py
--rw-rw-r--   0 user      (1000) user      (1000)     1607 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/utils/get_json_files.py
--rw-rw-r--   0 user      (1000) user      (1000)     2968 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/utils/get_namespaces.py
--rw-rw-r--   0 user      (1000) user      (1000)     3463 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/utils/get_paths.py
--rw-rw-r--   0 user      (1000) user      (1000)      236 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/utils/list_files.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-11 12:31:41.884146 lendsmart_reva-1.4/reva/lib/workflow/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/workflow/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      608 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/workflow/main.py
--rw-rw-r--   0 user      (1000) user      (1000)     1386 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/lib/workflow/update.py
--rw-rw-r--   0 user      (1000) user      (1000)      878 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/loan_products.py
--rw-rw-r--   0 user      (1000) user      (1000)     1125 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/namespaces.py
--rw-rw-r--   0 user      (1000) user      (1000)      933 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/roles_and_permissions.py
--rw-rw-r--   0 user      (1000) user      (1000)      853 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/site_settings.py
--rw-rw-r--   0 user      (1000) user      (1000)      820 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/reva/workflow.py
--rw-rw-r--   0 user      (1000) user      (1000)       86 2023-05-11 12:31:41.884146 lendsmart_reva-1.4/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2144 2023-05-11 12:01:08.000000 lendsmart_reva-1.4/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.944555 lendsmart_reva-1.5/
+-rw-rw-r--   0 user      (1000) user      (1000)       36 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     2823 2023-05-24 11:03:32.944555 lendsmart_reva-1.5/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2442 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.940555 lendsmart_reva-1.5/lendsmart_reva.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     2823 2023-05-24 11:03:32.000000 lendsmart_reva-1.5/lendsmart_reva.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1743 2023-05-24 11:03:32.000000 lendsmart_reva-1.5/lendsmart_reva.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-24 11:03:32.000000 lendsmart_reva-1.5/lendsmart_reva.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      448 2023-05-24 11:03:32.000000 lendsmart_reva-1.5/lendsmart_reva.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      158 2023-05-24 11:03:32.000000 lendsmart_reva-1.5/lendsmart_reva.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        5 2023-05-24 11:03:32.000000 lendsmart_reva-1.5/lendsmart_reva.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.940555 lendsmart_reva-1.5/reva/
+-rw-rw-r--   0 user      (1000) user      (1000)       22 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1849 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/autotest.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3528 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/cli.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.940555 lendsmart_reva-1.5/reva/conf/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/conf/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      740 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/conf/reva.py
+-rw-rw-r--   0 user      (1000) user      (1000)      953 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/document_access_control.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1076 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/exception.py
+-rw-rw-r--   0 user      (1000) user      (1000)      954 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/info.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.940555 lendsmart_reva-1.5/reva/lib/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.940555 lendsmart_reva-1.5/reva/lib/auto/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/auto/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3988 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/auto/main.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.940555 lendsmart_reva-1.5/reva/lib/base/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/base/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1101 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/base/base.py
+-rw-rw-r--   0 user      (1000) user      (1000)      948 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/base/run_query.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.944555 lendsmart_reva-1.5/reva/lib/client/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/client/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      399 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/client/builder.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2926 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/client/graphql_client.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.944555 lendsmart_reva-1.5/reva/lib/document_access_control/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/document_access_control/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      728 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/document_access_control/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1599 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/document_access_control/update.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.944555 lendsmart_reva-1.5/reva/lib/graphql_queries/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/graphql_queries/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      806 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/graphql_queries/document_access_control.py
+-rw-rw-r--   0 user      (1000) user      (1000)      641 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/graphql_queries/loan_products.py
+-rw-rw-r--   0 user      (1000) user      (1000)      944 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/graphql_queries/roles_and_permissions.py
+-rw-rw-r--   0 user      (1000) user      (1000)      590 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/graphql_queries/site_settings.py
+-rw-rw-r--   0 user      (1000) user      (1000)      802 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/graphql_queries/workflow.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.944555 lendsmart_reva-1.5/reva/lib/loan_productus/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/loan_productus/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      642 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/loan_productus/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1482 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/loan_productus/update.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.944555 lendsmart_reva-1.5/reva/lib/roles_and_permissions/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/roles_and_permissions/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      687 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/roles_and_permissions/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1880 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/roles_and_permissions/update.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.944555 lendsmart_reva-1.5/reva/lib/site_settings/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/site_settings/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      639 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/site_settings/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1416 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/site_settings/update.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.944555 lendsmart_reva-1.5/reva/lib/utils/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/utils/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      433 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/utils/filter_data_with_id.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1607 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/utils/get_json_files.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2968 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/utils/get_namespaces.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3463 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/utils/get_paths.py
+-rw-rw-r--   0 user      (1000) user      (1000)      236 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/utils/list_files.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-24 11:03:32.944555 lendsmart_reva-1.5/reva/lib/workflow/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/workflow/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      608 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/workflow/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1386 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/lib/workflow/update.py
+-rw-rw-r--   0 user      (1000) user      (1000)      878 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/loan_products.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1125 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/namespaces.py
+-rw-rw-r--   0 user      (1000) user      (1000)      933 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/roles_and_permissions.py
+-rw-rw-r--   0 user      (1000) user      (1000)      853 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/site_settings.py
+-rw-rw-r--   0 user      (1000) user      (1000)      820 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/reva/workflow.py
+-rw-rw-r--   0 user      (1000) user      (1000)       86 2023-05-24 11:03:32.944555 lendsmart_reva-1.5/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2144 2023-05-24 10:59:47.000000 lendsmart_reva-1.5/setup.py
```

### Comparing `lendsmart_reva-1.4/PKG-INFO` & `lendsmart_reva-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lendsmart_reva
-Version: 1.4
+Version: 1.5
 Summary: Lendsmart opinionated tool to mirror QA to Prod. Deploy with ease.
 Home-page: https://github.com/lendsmartlabs
 Author: Lendsmart
 Author-email: accounts@lendsmart.ai
 License: MIT
 Keywords: lendsmart reva
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `lendsmart_reva-1.4/README.md` & `lendsmart_reva-1.5/README.md`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/lendsmart_reva.egg-info/PKG-INFO` & `lendsmart_reva-1.5/lendsmart_reva.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lendsmart-reva
-Version: 1.4
+Version: 1.5
 Summary: Lendsmart opinionated tool to mirror QA to Prod. Deploy with ease.
 Home-page: https://github.com/lendsmartlabs
 Author: Lendsmart
 Author-email: accounts@lendsmart.ai
 License: MIT
 Keywords: lendsmart reva
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `lendsmart_reva-1.4/lendsmart_reva.egg-info/SOURCES.txt` & `lendsmart_reva-1.5/lendsmart_reva.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/autotest.py` & `lendsmart_reva-1.5/reva/autotest.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/cli.py` & `lendsmart_reva-1.5/reva/cli.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/conf/reva.py` & `lendsmart_reva-1.5/reva/conf/reva.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/document_access_control.py` & `lendsmart_reva-1.5/reva/document_access_control.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/exception.py` & `lendsmart_reva-1.5/reva/exception.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/info.py` & `lendsmart_reva-1.5/reva/info.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/lib/auto/main.py` & `lendsmart_reva-1.5/reva/lib/auto/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/lib/base/base.py` & `lendsmart_reva-1.5/reva/lib/base/base.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/lib/base/run_query.py` & `lendsmart_reva-1.5/reva/lib/base/run_query.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/lib/client/graphql_client.py` & `lendsmart_reva-1.5/reva/lib/client/graphql_client.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/lib/document_access_control/main.py` & `lendsmart_reva-1.5/reva/lib/document_access_control/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/lib/document_access_control/update.py` & `lendsmart_reva-1.5/reva/lib/document_access_control/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/lib/graphql_queries/document_access_control.py` & `lendsmart_reva-1.5/reva/lib/graphql_queries/document_access_control.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/lib/graphql_queries/roles_and_permissions.py` & `lendsmart_reva-1.5/reva/lib/graphql_queries/roles_and_permissions.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/lib/graphql_queries/site_settings.py` & `lendsmart_reva-1.5/reva/lib/graphql_queries/site_settings.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/lib/graphql_queries/workflow.py` & `lendsmart_reva-1.5/reva/lib/graphql_queries/workflow.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/lib/loan_productus/main.py` & `lendsmart_reva-1.5/reva/lib/loan_productus/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/lib/loan_productus/update.py` & `lendsmart_reva-1.5/reva/lib/loan_productus/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/lib/roles_and_permissions/main.py` & `lendsmart_reva-1.5/reva/lib/roles_and_permissions/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/lib/roles_and_permissions/update.py` & `lendsmart_reva-1.5/reva/lib/roles_and_permissions/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/lib/site_settings/main.py` & `lendsmart_reva-1.5/reva/lib/site_settings/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/lib/site_settings/update.py` & `lendsmart_reva-1.5/reva/lib/site_settings/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/lib/utils/get_json_files.py` & `lendsmart_reva-1.5/reva/lib/utils/get_json_files.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/lib/utils/get_namespaces.py` & `lendsmart_reva-1.5/reva/lib/utils/get_namespaces.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/lib/utils/get_paths.py` & `lendsmart_reva-1.5/reva/lib/utils/get_paths.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/lib/workflow/main.py` & `lendsmart_reva-1.5/reva/lib/workflow/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/lib/workflow/update.py` & `lendsmart_reva-1.5/reva/lib/workflow/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/loan_products.py` & `lendsmart_reva-1.5/reva/loan_products.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/namespaces.py` & `lendsmart_reva-1.5/reva/namespaces.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/roles_and_permissions.py` & `lendsmart_reva-1.5/reva/roles_and_permissions.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/site_settings.py` & `lendsmart_reva-1.5/reva/site_settings.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/reva/workflow.py` & `lendsmart_reva-1.5/reva/workflow.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-1.4/setup.py` & `lendsmart_reva-1.5/setup.py`

 * *Files identical despite different names*

