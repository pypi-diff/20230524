# Comparing `tmp/alibabacloud_dingtalk-2.0.15.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.15.tar", last modified: Thu May 18 06:04:19 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.16.tar", last modified: Wed May 24 08:33:20 2023, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.15.tar` & `alibabacloud_dingtalk-2.0.16.tar`

### file list

```diff
@@ -1,361 +1,365 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/
--rw-r--r--   0 root         (0) root         (0)    19622 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2309 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1021 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1106 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23314 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169621 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46194 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21260 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23341 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90648 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138912 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   161892 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   317257 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    62246 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   201848 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   569113 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4942 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3871 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   138814 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   331545 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42229 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35138 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   101075 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6044 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10927 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123179 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    85810 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110530 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124904 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   293352 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   387566 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42332 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6576 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10253 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30852 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   220322 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   547684 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7385 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46898 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   391978 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   515455 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152480 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    56301 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45840 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    65285 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   211006 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   267473 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   150160 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   269103 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   195538 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   453174 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   705965 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   116546 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123749 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5096 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     6148 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   312544 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   433417 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   155788 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   302125 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5282 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     5179 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4431 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4668 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9742 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138362 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18903 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5382 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4660 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92926 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137528 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   302532 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   378971 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13884 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18281 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    92472 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   523174 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   756557 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   155140 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   108695 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91118 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   135110 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23076 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   131349 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   159547 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54521 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31076 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40802 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7507 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76720 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137701 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123420 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60347 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    69069 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   260568 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   413706 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    11593 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   174524 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81780 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    93746 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56986 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    83842 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46018 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   361006 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   503423 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26678 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    96217 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   353698 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44880 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    81308 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28559 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65344 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   148231 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16170 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21677 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17519 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18718 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    32237 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110849 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4269 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20486 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66210 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   130783 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8325 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27686 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    29689 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   179772 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   377583 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3772 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   464194 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   687148 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2309 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11880 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2684 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/
+-rw-r--r--   0 root         (0) root         (0)    19687 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23314 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169621 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46194 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21260 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23341 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90648 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138912 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   165948 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   322772 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    62246 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   201848 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   569113 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4942 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3871 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   138814 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   331545 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42229 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35138 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   101075 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10446 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123179 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    85810 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110530 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124904 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   293352 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   387566 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42332 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6576 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10253 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30852 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223914 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   552073 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7385 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46898 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   515455 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152480 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    56301 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45840 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    65285 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   211006 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   267473 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   150160 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   269103 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   195538 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   453174 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   705965 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   116546 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123749 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5096 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   312544 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   433417 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   155788 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   302125 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5282 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     5179 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4431 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4668 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9742 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138362 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18903 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4660 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92926 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137528 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   302532 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   378971 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13884 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18281 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    92472 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   606316 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   855474 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   155140 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   108695 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91118 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   135110 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   131349 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   159547 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54521 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31076 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40802 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76720 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137701 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123420 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60347 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    69069 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   260568 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   413706 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    11593 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   174524 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81780 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    93746 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56986 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    83842 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46018 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   361006 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   503423 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26678 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    96217 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   353698 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44880 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    81308 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28559 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65344 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   148231 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16170 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21677 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17519 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18718 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    32237 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110849 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4269 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20486 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66210 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   130783 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8325 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27686 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    29689 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   179772 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   377583 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   464194 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   687148 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5452 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4490 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12014 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2684 2023-05-24 08:33:20.000000 alibabacloud_dingtalk-2.0.16/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.15/ChangeLog.md` & `alibabacloud_dingtalk-2.0.16/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-05-18 Version: 2.0.15
+- Update AddOfficialAccountFollower.
+
 2023-05-17 Version: 2.0.14
 - Update AddOfficialAccountFollower.
 
 2023-05-16 Version: 2.0.13
 - Update AddOfficialAccountFollower.
 
 2023-05-12 Version: 2.0.12
```

### Comparing `alibabacloud_dingtalk-2.0.15/LICENSE` & `alibabacloud_dingtalk-2.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/PKG-INFO` & `alibabacloud_dingtalk-2.0.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.0.15
+Version: 2.0.16
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.15/README-CN.md` & `alibabacloud_dingtalk-2.0.16/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/README.md` & `alibabacloud_dingtalk-2.0.16/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -429,14 +429,108 @@
         self,
         request: dingtalkattendance__1__0_models.AttendanceBleDevicesRemoveRequest,
     ) -> dingtalkattendance__1__0_models.AttendanceBleDevicesRemoveResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkattendance__1__0_models.AttendanceBleDevicesRemoveHeaders()
         return await self.attendance_ble_devices_remove_with_options_async(request, headers, runtime)
 
+    def batch_boss_check_with_options(
+        self,
+        request: dingtalkattendance__1__0_models.BatchBossCheckRequest,
+        headers: dingtalkattendance__1__0_models.BatchBossCheckHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkattendance__1__0_models.BatchBossCheckResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.op_user_id):
+            query['opUserId'] = request.op_user_id
+        body = {}
+        if not UtilClient.is_unset(request.models):
+            body['models'] = request.models
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='BatchBossCheck',
+            version='attendance_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/attendance/results/batch',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkattendance__1__0_models.BatchBossCheckResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def batch_boss_check_with_options_async(
+        self,
+        request: dingtalkattendance__1__0_models.BatchBossCheckRequest,
+        headers: dingtalkattendance__1__0_models.BatchBossCheckHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkattendance__1__0_models.BatchBossCheckResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.op_user_id):
+            query['opUserId'] = request.op_user_id
+        body = {}
+        if not UtilClient.is_unset(request.models):
+            body['models'] = request.models
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='BatchBossCheck',
+            version='attendance_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/attendance/results/batch',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkattendance__1__0_models.BatchBossCheckResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def batch_boss_check(
+        self,
+        request: dingtalkattendance__1__0_models.BatchBossCheckRequest,
+    ) -> dingtalkattendance__1__0_models.BatchBossCheckResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkattendance__1__0_models.BatchBossCheckHeaders()
+        return self.batch_boss_check_with_options(request, headers, runtime)
+
+    async def batch_boss_check_async(
+        self,
+        request: dingtalkattendance__1__0_models.BatchBossCheckRequest,
+    ) -> dingtalkattendance__1__0_models.BatchBossCheckResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkattendance__1__0_models.BatchBossCheckHeaders()
+        return await self.batch_boss_check_with_options_async(request, headers, runtime)
+
     def check_closing_account_with_options(
         self,
         request: dingtalkattendance__1__0_models.CheckClosingAccountRequest,
         headers: dingtalkattendance__1__0_models.CheckClosingAccountHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkattendance__1__0_models.CheckClosingAccountResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1389,14 +1389,204 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AttendanceBleDevicesRemoveResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class BatchBossCheckHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class BatchBossCheckRequestModels(TeaModel):
+    def __init__(
+        self,
+        absent_min: int = None,
+        plan_id: int = None,
+        remark: str = None,
+        time_result: str = None,
+    ):
+        self.absent_min = absent_min
+        self.plan_id = plan_id
+        self.remark = remark
+        self.time_result = time_result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.absent_min is not None:
+            result['absentMin'] = self.absent_min
+        if self.plan_id is not None:
+            result['planId'] = self.plan_id
+        if self.remark is not None:
+            result['remark'] = self.remark
+        if self.time_result is not None:
+            result['timeResult'] = self.time_result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('absentMin') is not None:
+            self.absent_min = m.get('absentMin')
+        if m.get('planId') is not None:
+            self.plan_id = m.get('planId')
+        if m.get('remark') is not None:
+            self.remark = m.get('remark')
+        if m.get('timeResult') is not None:
+            self.time_result = m.get('timeResult')
+        return self
+
+
+class BatchBossCheckRequest(TeaModel):
+    def __init__(
+        self,
+        models: List[BatchBossCheckRequestModels] = None,
+        op_user_id: str = None,
+    ):
+        self.models = models
+        self.op_user_id = op_user_id
+
+    def validate(self):
+        if self.models:
+            for k in self.models:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['models'] = []
+        if self.models is not None:
+            for k in self.models:
+                result['models'].append(k.to_map() if k else None)
+        if self.op_user_id is not None:
+            result['opUserId'] = self.op_user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.models = []
+        if m.get('models') is not None:
+            for k in m.get('models'):
+                temp_model = BatchBossCheckRequestModels()
+                self.models.append(temp_model.from_map(k))
+        if m.get('opUserId') is not None:
+            self.op_user_id = m.get('opUserId')
+        return self
+
+
+class BatchBossCheckResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class BatchBossCheckResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: BatchBossCheckResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = BatchBossCheckResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CheckClosingAccountHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,27 +136,23 @@
 class GetCheckinRecordByUserResponseBodyResultPageList(TeaModel):
     def __init__(
         self,
         checkin_time: int = None,
         custom_data_list: List[GetCheckinRecordByUserResponseBodyResultPageListCustomDataList] = None,
         detail_place: str = None,
         image_list: List[str] = None,
-        latitude: str = None,
-        longitude: str = None,
         place: str = None,
         remark: str = None,
         user_id: str = None,
         visit_user: str = None,
     ):
         self.checkin_time = checkin_time
         self.custom_data_list = custom_data_list
         self.detail_place = detail_place
         self.image_list = image_list
-        self.latitude = latitude
-        self.longitude = longitude
         self.place = place
         self.remark = remark
         self.user_id = user_id
         self.visit_user = visit_user
 
     def validate(self):
         if self.custom_data_list:
@@ -176,18 +172,14 @@
         if self.custom_data_list is not None:
             for k in self.custom_data_list:
                 result['customDataList'].append(k.to_map() if k else None)
         if self.detail_place is not None:
             result['detailPlace'] = self.detail_place
         if self.image_list is not None:
             result['imageList'] = self.image_list
-        if self.latitude is not None:
-            result['latitude'] = self.latitude
-        if self.longitude is not None:
-            result['longitude'] = self.longitude
         if self.place is not None:
             result['place'] = self.place
         if self.remark is not None:
             result['remark'] = self.remark
         if self.user_id is not None:
             result['userId'] = self.user_id
         if self.visit_user is not None:
@@ -203,18 +195,14 @@
             for k in m.get('customDataList'):
                 temp_model = GetCheckinRecordByUserResponseBodyResultPageListCustomDataList()
                 self.custom_data_list.append(temp_model.from_map(k))
         if m.get('detailPlace') is not None:
             self.detail_place = m.get('detailPlace')
         if m.get('imageList') is not None:
             self.image_list = m.get('imageList')
-        if m.get('latitude') is not None:
-            self.latitude = m.get('latitude')
-        if m.get('longitude') is not None:
-            self.longitude = m.get('longitude')
         if m.get('place') is not None:
             self.place = m.get('place')
         if m.get('remark') is not None:
             self.remark = m.get('remark')
         if m.get('userId') is not None:
             self.user_id = m.get('userId')
         if m.get('visitUser') is not None:
```

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -3999,14 +3999,100 @@
         self,
         request: dingtalkcrm__1__0_models.QueryCrmPersonalCustomerRequest,
     ) -> dingtalkcrm__1__0_models.QueryCrmPersonalCustomerResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkcrm__1__0_models.QueryCrmPersonalCustomerHeaders()
         return await self.query_crm_personal_customer_with_options_async(request, headers, runtime)
 
+    def query_global_info_with_options(
+        self,
+        request: dingtalkcrm__1__0_models.QueryGlobalInfoRequest,
+        headers: dingtalkcrm__1__0_models.QueryGlobalInfoHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkcrm__1__0_models.QueryGlobalInfoResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.user_id):
+            query['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='QueryGlobalInfo',
+            version='crm_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/crm/globalInfos',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkcrm__1__0_models.QueryGlobalInfoResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def query_global_info_with_options_async(
+        self,
+        request: dingtalkcrm__1__0_models.QueryGlobalInfoRequest,
+        headers: dingtalkcrm__1__0_models.QueryGlobalInfoHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkcrm__1__0_models.QueryGlobalInfoResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.user_id):
+            query['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='QueryGlobalInfo',
+            version='crm_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/crm/globalInfos',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkcrm__1__0_models.QueryGlobalInfoResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def query_global_info(
+        self,
+        request: dingtalkcrm__1__0_models.QueryGlobalInfoRequest,
+    ) -> dingtalkcrm__1__0_models.QueryGlobalInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkcrm__1__0_models.QueryGlobalInfoHeaders()
+        return self.query_global_info_with_options(request, headers, runtime)
+
+    async def query_global_info_async(
+        self,
+        request: dingtalkcrm__1__0_models.QueryGlobalInfoRequest,
+    ) -> dingtalkcrm__1__0_models.QueryGlobalInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkcrm__1__0_models.QueryGlobalInfoHeaders()
+        return await self.query_global_info_with_options_async(request, headers, runtime)
+
     def query_official_account_user_basic_info_with_options(
         self,
         request: dingtalkcrm__1__0_models.QueryOfficialAccountUserBasicInfoRequest,
         headers: dingtalkcrm__1__0_models.QueryOfficialAccountUserBasicInfoHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkcrm__1__0_models.QueryOfficialAccountUserBasicInfoResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -13911,14 +13911,174 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = QueryCrmPersonalCustomerResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class QueryGlobalInfoHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class QueryGlobalInfoRequest(TeaModel):
+    def __init__(
+        self,
+        user_id: str = None,
+    ):
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class QueryGlobalInfoResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        oem_enable: bool = None,
+    ):
+        self.oem_enable = oem_enable
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.oem_enable is not None:
+            result['oemEnable'] = self.oem_enable
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('oemEnable') is not None:
+            self.oem_enable = m.get('oemEnable')
+        return self
+
+
+class QueryGlobalInfoResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: QueryGlobalInfoResponseBodyResult = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = QueryGlobalInfoResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        return self
+
+
+class QueryGlobalInfoResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: QueryGlobalInfoResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = QueryGlobalInfoResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class QueryOfficialAccountUserBasicInfoHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -10765,14 +10765,104 @@
         user_id: str,
         request: dingtalkindustry__1__0_models.SaveUserExtendValuesRequest,
     ) -> dingtalkindustry__1__0_models.SaveUserExtendValuesResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkindustry__1__0_models.SaveUserExtendValuesHeaders()
         return await self.save_user_extend_values_with_options_async(user_id, request, headers, runtime)
 
+    def suppl_add_role_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplAddRoleRequest,
+        headers: dingtalkindustry__1__0_models.SupplAddRoleHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplAddRoleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.parent_role_group_id):
+            query['parentRoleGroupId'] = request.parent_role_group_id
+        if not UtilClient.is_unset(request.role_name):
+            query['roleName'] = request.role_name
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplAddRole',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/roles',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplAddRoleResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def suppl_add_role_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplAddRoleRequest,
+        headers: dingtalkindustry__1__0_models.SupplAddRoleHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplAddRoleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.parent_role_group_id):
+            query['parentRoleGroupId'] = request.parent_role_group_id
+        if not UtilClient.is_unset(request.role_name):
+            query['roleName'] = request.role_name
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplAddRole',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/roles',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplAddRoleResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def suppl_add_role(
+        self,
+        request: dingtalkindustry__1__0_models.SupplAddRoleRequest,
+    ) -> dingtalkindustry__1__0_models.SupplAddRoleResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplAddRoleHeaders()
+        return self.suppl_add_role_with_options(request, headers, runtime)
+
+    async def suppl_add_role_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplAddRoleRequest,
+    ) -> dingtalkindustry__1__0_models.SupplAddRoleResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplAddRoleHeaders()
+        return await self.suppl_add_role_with_options_async(request, headers, runtime)
+
     def supply_add_dept_with_options(
         self,
         request: dingtalkindustry__1__0_models.SupplyAddDeptRequest,
         headers: dingtalkindustry__1__0_models.SupplyAddDeptHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkindustry__1__0_models.SupplyAddDeptResponse:
         UtilClient.validate_model(request)
@@ -10877,14 +10967,16 @@
         query = {}
         if not UtilClient.is_unset(request.is_partner_manager):
             query['isPartnerManager'] = request.is_partner_manager
         if not UtilClient.is_unset(request.member_mobile):
             query['memberMobile'] = request.member_mobile
         if not UtilClient.is_unset(request.member_name):
             query['memberName'] = request.member_name
+        if not UtilClient.is_unset(request.member_title):
+            query['memberTitle'] = request.member_title
         if not UtilClient.is_unset(request.member_work_number):
             query['memberWorkNumber'] = request.member_work_number
         if not UtilClient.is_unset(request.supply_dept_id):
             query['supplyDeptId'] = request.supply_dept_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
@@ -10920,14 +11012,16 @@
         query = {}
         if not UtilClient.is_unset(request.is_partner_manager):
             query['isPartnerManager'] = request.is_partner_manager
         if not UtilClient.is_unset(request.member_mobile):
             query['memberMobile'] = request.member_mobile
         if not UtilClient.is_unset(request.member_name):
             query['memberName'] = request.member_name
+        if not UtilClient.is_unset(request.member_title):
+            query['memberTitle'] = request.member_title
         if not UtilClient.is_unset(request.member_work_number):
             query['memberWorkNumber'] = request.member_work_number
         if not UtilClient.is_unset(request.supply_dept_id):
             query['supplyDeptId'] = request.supply_dept_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
@@ -10965,22 +11059,932 @@
         self,
         request: dingtalkindustry__1__0_models.SupplyAddMemberRequest,
     ) -> dingtalkindustry__1__0_models.SupplyAddMemberResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkindustry__1__0_models.SupplyAddMemberHeaders()
         return await self.supply_add_member_with_options_async(request, headers, runtime)
 
+    def supply_add_partner_admins_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyAddPartnerAdminsRequest,
+        headers: dingtalkindustry__1__0_models.SupplyAddPartnerAdminsHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyAddPartnerAdminsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dept_id):
+            query['deptId'] = request.dept_id
+        if not UtilClient.is_unset(request.user_id):
+            query['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyAddPartnerAdmins',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/partnerAdministrators',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyAddPartnerAdminsResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def supply_add_partner_admins_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyAddPartnerAdminsRequest,
+        headers: dingtalkindustry__1__0_models.SupplyAddPartnerAdminsHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyAddPartnerAdminsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dept_id):
+            query['deptId'] = request.dept_id
+        if not UtilClient.is_unset(request.user_id):
+            query['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyAddPartnerAdmins',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/partnerAdministrators',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyAddPartnerAdminsResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def supply_add_partner_admins(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyAddPartnerAdminsRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyAddPartnerAdminsResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyAddPartnerAdminsHeaders()
+        return self.supply_add_partner_admins_with_options(request, headers, runtime)
+
+    async def supply_add_partner_admins_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyAddPartnerAdminsRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyAddPartnerAdminsResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyAddPartnerAdminsHeaders()
+        return await self.supply_add_partner_admins_with_options_async(request, headers, runtime)
+
+    def supply_add_partner_managers_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyAddPartnerManagersRequest,
+        headers: dingtalkindustry__1__0_models.SupplyAddPartnerManagersHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyAddPartnerManagersResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dept_id):
+            query['deptId'] = request.dept_id
+        if not UtilClient.is_unset(request.interface_id):
+            query['interfaceId'] = request.interface_id
+        if not UtilClient.is_unset(request.interface_type):
+            query['interfaceType'] = request.interface_type
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyAddPartnerManagers',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/partnerInterfaces',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyAddPartnerManagersResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def supply_add_partner_managers_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyAddPartnerManagersRequest,
+        headers: dingtalkindustry__1__0_models.SupplyAddPartnerManagersHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyAddPartnerManagersResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dept_id):
+            query['deptId'] = request.dept_id
+        if not UtilClient.is_unset(request.interface_id):
+            query['interfaceId'] = request.interface_id
+        if not UtilClient.is_unset(request.interface_type):
+            query['interfaceType'] = request.interface_type
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyAddPartnerManagers',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/partnerInterfaces',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyAddPartnerManagersResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def supply_add_partner_managers(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyAddPartnerManagersRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyAddPartnerManagersResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyAddPartnerManagersHeaders()
+        return self.supply_add_partner_managers_with_options(request, headers, runtime)
+
+    async def supply_add_partner_managers_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyAddPartnerManagersRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyAddPartnerManagersResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyAddPartnerManagersHeaders()
+        return await self.supply_add_partner_managers_with_options_async(request, headers, runtime)
+
+    def supply_add_partner_type_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyAddPartnerTypeRequest,
+        headers: dingtalkindustry__1__0_models.SupplyAddPartnerTypeHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyAddPartnerTypeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.name):
+            query['name'] = request.name
+        if not UtilClient.is_unset(request.super_id):
+            query['superId'] = request.super_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyAddPartnerType',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/partnerLabels',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyAddPartnerTypeResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def supply_add_partner_type_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyAddPartnerTypeRequest,
+        headers: dingtalkindustry__1__0_models.SupplyAddPartnerTypeHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyAddPartnerTypeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.name):
+            query['name'] = request.name
+        if not UtilClient.is_unset(request.super_id):
+            query['superId'] = request.super_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyAddPartnerType',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/partnerLabels',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyAddPartnerTypeResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def supply_add_partner_type(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyAddPartnerTypeRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyAddPartnerTypeResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyAddPartnerTypeHeaders()
+        return self.supply_add_partner_type_with_options(request, headers, runtime)
+
+    async def supply_add_partner_type_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyAddPartnerTypeRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyAddPartnerTypeResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyAddPartnerTypeHeaders()
+        return await self.supply_add_partner_type_with_options_async(request, headers, runtime)
+
+    def supply_chain_delete_dept_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyChainDeleteDeptRequest,
+        headers: dingtalkindustry__1__0_models.SupplyChainDeleteDeptHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyChainDeleteDeptResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.supply_dept_id):
+            query['supplyDeptId'] = request.supply_dept_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyChainDeleteDept',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/departments',
+            method='DELETE',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyChainDeleteDeptResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def supply_chain_delete_dept_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyChainDeleteDeptRequest,
+        headers: dingtalkindustry__1__0_models.SupplyChainDeleteDeptHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyChainDeleteDeptResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.supply_dept_id):
+            query['supplyDeptId'] = request.supply_dept_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyChainDeleteDept',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/departments',
+            method='DELETE',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyChainDeleteDeptResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def supply_chain_delete_dept(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyChainDeleteDeptRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyChainDeleteDeptResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyChainDeleteDeptHeaders()
+        return self.supply_chain_delete_dept_with_options(request, headers, runtime)
+
+    async def supply_chain_delete_dept_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyChainDeleteDeptRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyChainDeleteDeptResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyChainDeleteDeptHeaders()
+        return await self.supply_chain_delete_dept_with_options_async(request, headers, runtime)
+
+    def supply_chain_query_dept_info_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyChainQueryDeptInfoRequest,
+        headers: dingtalkindustry__1__0_models.SupplyChainQueryDeptInfoHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyChainQueryDeptInfoResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.supply_dept_id):
+            query['supplyDeptId'] = request.supply_dept_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyChainQueryDeptInfo',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/departments',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyChainQueryDeptInfoResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def supply_chain_query_dept_info_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyChainQueryDeptInfoRequest,
+        headers: dingtalkindustry__1__0_models.SupplyChainQueryDeptInfoHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyChainQueryDeptInfoResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.supply_dept_id):
+            query['supplyDeptId'] = request.supply_dept_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyChainQueryDeptInfo',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/departments',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyChainQueryDeptInfoResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def supply_chain_query_dept_info(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyChainQueryDeptInfoRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyChainQueryDeptInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyChainQueryDeptInfoHeaders()
+        return self.supply_chain_query_dept_info_with_options(request, headers, runtime)
+
+    async def supply_chain_query_dept_info_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyChainQueryDeptInfoRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyChainQueryDeptInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyChainQueryDeptInfoHeaders()
+        return await self.supply_chain_query_dept_info_with_options_async(request, headers, runtime)
+
+    def supply_chain_update_dept_info_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyChainUpdateDeptInfoRequest,
+        headers: dingtalkindustry__1__0_models.SupplyChainUpdateDeptInfoHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyChainUpdateDeptInfoResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.name):
+            body['name'] = request.name
+        if not UtilClient.is_unset(request.partner_number):
+            body['partnerNumber'] = request.partner_number
+        if not UtilClient.is_unset(request.partner_type_list):
+            body['partnerTypeList'] = request.partner_type_list
+        if not UtilClient.is_unset(request.super_id):
+            body['superId'] = request.super_id
+        if not UtilClient.is_unset(request.supply_dept_id):
+            body['supplyDeptId'] = request.supply_dept_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='SupplyChainUpdateDeptInfo',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/departments',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyChainUpdateDeptInfoResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def supply_chain_update_dept_info_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyChainUpdateDeptInfoRequest,
+        headers: dingtalkindustry__1__0_models.SupplyChainUpdateDeptInfoHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyChainUpdateDeptInfoResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.name):
+            body['name'] = request.name
+        if not UtilClient.is_unset(request.partner_number):
+            body['partnerNumber'] = request.partner_number
+        if not UtilClient.is_unset(request.partner_type_list):
+            body['partnerTypeList'] = request.partner_type_list
+        if not UtilClient.is_unset(request.super_id):
+            body['superId'] = request.super_id
+        if not UtilClient.is_unset(request.supply_dept_id):
+            body['supplyDeptId'] = request.supply_dept_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='SupplyChainUpdateDeptInfo',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/departments',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyChainUpdateDeptInfoResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def supply_chain_update_dept_info(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyChainUpdateDeptInfoRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyChainUpdateDeptInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyChainUpdateDeptInfoHeaders()
+        return self.supply_chain_update_dept_info_with_options(request, headers, runtime)
+
+    async def supply_chain_update_dept_info_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyChainUpdateDeptInfoRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyChainUpdateDeptInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyChainUpdateDeptInfoHeaders()
+        return await self.supply_chain_update_dept_info_with_options_async(request, headers, runtime)
+
+    def supply_delete_partner_admins_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyDeletePartnerAdminsRequest,
+        headers: dingtalkindustry__1__0_models.SupplyDeletePartnerAdminsHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyDeletePartnerAdminsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dept_id):
+            query['deptId'] = request.dept_id
+        if not UtilClient.is_unset(request.user_id):
+            query['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyDeletePartnerAdmins',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/partnerAdministrators',
+            method='DELETE',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyDeletePartnerAdminsResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def supply_delete_partner_admins_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyDeletePartnerAdminsRequest,
+        headers: dingtalkindustry__1__0_models.SupplyDeletePartnerAdminsHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyDeletePartnerAdminsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dept_id):
+            query['deptId'] = request.dept_id
+        if not UtilClient.is_unset(request.user_id):
+            query['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyDeletePartnerAdmins',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/partnerAdministrators',
+            method='DELETE',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyDeletePartnerAdminsResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def supply_delete_partner_admins(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyDeletePartnerAdminsRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyDeletePartnerAdminsResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyDeletePartnerAdminsHeaders()
+        return self.supply_delete_partner_admins_with_options(request, headers, runtime)
+
+    async def supply_delete_partner_admins_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyDeletePartnerAdminsRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyDeletePartnerAdminsResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyDeletePartnerAdminsHeaders()
+        return await self.supply_delete_partner_admins_with_options_async(request, headers, runtime)
+
+    def supply_delete_partner_managers_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyDeletePartnerManagersRequest,
+        headers: dingtalkindustry__1__0_models.SupplyDeletePartnerManagersHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyDeletePartnerManagersResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dept_id):
+            query['deptId'] = request.dept_id
+        if not UtilClient.is_unset(request.interface_id):
+            query['interfaceId'] = request.interface_id
+        if not UtilClient.is_unset(request.interface_type):
+            query['interfaceType'] = request.interface_type
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyDeletePartnerManagers',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/partnerInterfaces',
+            method='DELETE',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyDeletePartnerManagersResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def supply_delete_partner_managers_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyDeletePartnerManagersRequest,
+        headers: dingtalkindustry__1__0_models.SupplyDeletePartnerManagersHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyDeletePartnerManagersResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dept_id):
+            query['deptId'] = request.dept_id
+        if not UtilClient.is_unset(request.interface_id):
+            query['interfaceId'] = request.interface_id
+        if not UtilClient.is_unset(request.interface_type):
+            query['interfaceType'] = request.interface_type
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyDeletePartnerManagers',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/partnerInterfaces',
+            method='DELETE',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyDeletePartnerManagersResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def supply_delete_partner_managers(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyDeletePartnerManagersRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyDeletePartnerManagersResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyDeletePartnerManagersHeaders()
+        return self.supply_delete_partner_managers_with_options(request, headers, runtime)
+
+    async def supply_delete_partner_managers_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyDeletePartnerManagersRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyDeletePartnerManagersResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyDeletePartnerManagersHeaders()
+        return await self.supply_delete_partner_managers_with_options_async(request, headers, runtime)
+
+    def supply_delete_partner_type_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyDeletePartnerTypeRequest,
+        headers: dingtalkindustry__1__0_models.SupplyDeletePartnerTypeHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyDeletePartnerTypeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.label_id):
+            query['labelId'] = request.label_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyDeletePartnerType',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/partnerLabels',
+            method='DELETE',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyDeletePartnerTypeResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def supply_delete_partner_type_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyDeletePartnerTypeRequest,
+        headers: dingtalkindustry__1__0_models.SupplyDeletePartnerTypeHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyDeletePartnerTypeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.label_id):
+            query['labelId'] = request.label_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyDeletePartnerType',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/partnerLabels',
+            method='DELETE',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyDeletePartnerTypeResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def supply_delete_partner_type(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyDeletePartnerTypeRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyDeletePartnerTypeResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyDeletePartnerTypeHeaders()
+        return self.supply_delete_partner_type_with_options(request, headers, runtime)
+
+    async def supply_delete_partner_type_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyDeletePartnerTypeRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyDeletePartnerTypeResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyDeletePartnerTypeHeaders()
+        return await self.supply_delete_partner_type_with_options_async(request, headers, runtime)
+
+    def supply_delete_role_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyDeleteRoleRequest,
+        headers: dingtalkindustry__1__0_models.SupplyDeleteRoleHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyDeleteRoleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.is_role_group):
+            query['isRoleGroup'] = request.is_role_group
+        if not UtilClient.is_unset(request.role_id):
+            query['roleId'] = request.role_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyDeleteRole',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/roles',
+            method='DELETE',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyDeleteRoleResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def supply_delete_role_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyDeleteRoleRequest,
+        headers: dingtalkindustry__1__0_models.SupplyDeleteRoleHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyDeleteRoleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.is_role_group):
+            query['isRoleGroup'] = request.is_role_group
+        if not UtilClient.is_unset(request.role_id):
+            query['roleId'] = request.role_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyDeleteRole',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/roles',
+            method='DELETE',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyDeleteRoleResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def supply_delete_role(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyDeleteRoleRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyDeleteRoleResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyDeleteRoleHeaders()
+        return self.supply_delete_role_with_options(request, headers, runtime)
+
+    async def supply_delete_role_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyDeleteRoleRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyDeleteRoleResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyDeleteRoleHeaders()
+        return await self.supply_delete_role_with_options_async(request, headers, runtime)
+
     def supply_get_member_with_options(
         self,
         request: dingtalkindustry__1__0_models.SupplyGetMemberRequest,
         headers: dingtalkindustry__1__0_models.SupplyGetMemberHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkindustry__1__0_models.SupplyGetMemberResponse:
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.mobile):
+            query['mobile'] = request.mobile
         if not UtilClient.is_unset(request.union_id):
             query['unionId'] = request.union_id
         if not UtilClient.is_unset(request.user_id):
             query['userId'] = request.user_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
@@ -11010,14 +12014,16 @@
         self,
         request: dingtalkindustry__1__0_models.SupplyGetMemberRequest,
         headers: dingtalkindustry__1__0_models.SupplyGetMemberHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkindustry__1__0_models.SupplyGetMemberResponse:
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.mobile):
+            query['mobile'] = request.mobile
         if not UtilClient.is_unset(request.union_id):
             query['unionId'] = request.union_id
         if not UtilClient.is_unset(request.user_id):
             query['userId'] = request.user_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
@@ -11149,14 +12155,836 @@
         self,
         request: dingtalkindustry__1__0_models.SupplyListDeptMembersRequest,
     ) -> dingtalkindustry__1__0_models.SupplyListDeptMembersResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkindustry__1__0_models.SupplyListDeptMembersHeaders()
         return await self.supply_list_dept_members_with_options_async(request, headers, runtime)
 
+    def supply_list_partner_admins_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyListPartnerAdminsRequest,
+        headers: dingtalkindustry__1__0_models.SupplyListPartnerAdminsHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyListPartnerAdminsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dept_id):
+            query['deptId'] = request.dept_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyListPartnerAdmins',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/partnerAdministrators',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyListPartnerAdminsResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def supply_list_partner_admins_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyListPartnerAdminsRequest,
+        headers: dingtalkindustry__1__0_models.SupplyListPartnerAdminsHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyListPartnerAdminsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dept_id):
+            query['deptId'] = request.dept_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyListPartnerAdmins',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/partnerAdministrators',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyListPartnerAdminsResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def supply_list_partner_admins(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyListPartnerAdminsRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyListPartnerAdminsResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyListPartnerAdminsHeaders()
+        return self.supply_list_partner_admins_with_options(request, headers, runtime)
+
+    async def supply_list_partner_admins_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyListPartnerAdminsRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyListPartnerAdminsResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyListPartnerAdminsHeaders()
+        return await self.supply_list_partner_admins_with_options_async(request, headers, runtime)
+
+    def supply_list_partner_managers_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyListPartnerManagersRequest,
+        headers: dingtalkindustry__1__0_models.SupplyListPartnerManagersHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyListPartnerManagersResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dept_id):
+            query['deptId'] = request.dept_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyListPartnerManagers',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/partnerInterfaces',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyListPartnerManagersResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def supply_list_partner_managers_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyListPartnerManagersRequest,
+        headers: dingtalkindustry__1__0_models.SupplyListPartnerManagersHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyListPartnerManagersResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dept_id):
+            query['deptId'] = request.dept_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyListPartnerManagers',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/partnerInterfaces',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyListPartnerManagersResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def supply_list_partner_managers(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyListPartnerManagersRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyListPartnerManagersResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyListPartnerManagersHeaders()
+        return self.supply_list_partner_managers_with_options(request, headers, runtime)
+
+    async def supply_list_partner_managers_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyListPartnerManagersRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyListPartnerManagersResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyListPartnerManagersHeaders()
+        return await self.supply_list_partner_managers_with_options_async(request, headers, runtime)
+
+    def supply_list_partner_type_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyListPartnerTypeRequest,
+        headers: dingtalkindustry__1__0_models.SupplyListPartnerTypeHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyListPartnerTypeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.label_id):
+            query['labelId'] = request.label_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyListPartnerType',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/partnerLabels/subLabels',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyListPartnerTypeResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def supply_list_partner_type_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyListPartnerTypeRequest,
+        headers: dingtalkindustry__1__0_models.SupplyListPartnerTypeHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyListPartnerTypeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.label_id):
+            query['labelId'] = request.label_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyListPartnerType',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/partnerLabels/subLabels',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyListPartnerTypeResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def supply_list_partner_type(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyListPartnerTypeRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyListPartnerTypeResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyListPartnerTypeHeaders()
+        return self.supply_list_partner_type_with_options(request, headers, runtime)
+
+    async def supply_list_partner_type_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyListPartnerTypeRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyListPartnerTypeResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyListPartnerTypeHeaders()
+        return await self.supply_list_partner_type_with_options_async(request, headers, runtime)
+
+    def supply_list_role_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyListRoleRequest,
+        headers: dingtalkindustry__1__0_models.SupplyListRoleHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyListRoleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.parent_role_id):
+            query['parentRoleId'] = request.parent_role_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyListRole',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/roles',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyListRoleResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def supply_list_role_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyListRoleRequest,
+        headers: dingtalkindustry__1__0_models.SupplyListRoleHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyListRoleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.parent_role_id):
+            query['parentRoleId'] = request.parent_role_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyListRole',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/roles',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyListRoleResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def supply_list_role(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyListRoleRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyListRoleResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyListRoleHeaders()
+        return self.supply_list_role_with_options(request, headers, runtime)
+
+    async def supply_list_role_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyListRoleRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyListRoleResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyListRoleHeaders()
+        return await self.supply_list_role_with_options_async(request, headers, runtime)
+
+    def supply_list_sub_dept_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyListSubDeptRequest,
+        headers: dingtalkindustry__1__0_models.SupplyListSubDeptHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyListSubDeptResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.supply_dept_id):
+            query['supplyDeptId'] = request.supply_dept_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyListSubDept',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/subDepartments',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyListSubDeptResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def supply_list_sub_dept_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyListSubDeptRequest,
+        headers: dingtalkindustry__1__0_models.SupplyListSubDeptHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyListSubDeptResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.supply_dept_id):
+            query['supplyDeptId'] = request.supply_dept_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyListSubDept',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/subDepartments',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyListSubDeptResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def supply_list_sub_dept(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyListSubDeptRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyListSubDeptResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyListSubDeptHeaders()
+        return self.supply_list_sub_dept_with_options(request, headers, runtime)
+
+    async def supply_list_sub_dept_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyListSubDeptRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyListSubDeptResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyListSubDeptHeaders()
+        return await self.supply_list_sub_dept_with_options_async(request, headers, runtime)
+
+    def supply_query_partner_type_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyQueryPartnerTypeRequest,
+        headers: dingtalkindustry__1__0_models.SupplyQueryPartnerTypeHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyQueryPartnerTypeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.label_id):
+            query['labelId'] = request.label_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyQueryPartnerType',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/partnerLabels',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyQueryPartnerTypeResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def supply_query_partner_type_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyQueryPartnerTypeRequest,
+        headers: dingtalkindustry__1__0_models.SupplyQueryPartnerTypeHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyQueryPartnerTypeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.label_id):
+            query['labelId'] = request.label_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyQueryPartnerType',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/partnerLabels',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyQueryPartnerTypeResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def supply_query_partner_type(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyQueryPartnerTypeRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyQueryPartnerTypeResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyQueryPartnerTypeHeaders()
+        return self.supply_query_partner_type_with_options(request, headers, runtime)
+
+    async def supply_query_partner_type_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyQueryPartnerTypeRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyQueryPartnerTypeResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyQueryPartnerTypeHeaders()
+        return await self.supply_query_partner_type_with_options_async(request, headers, runtime)
+
+    def supply_update_member_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyUpdateMemberRequest,
+        headers: dingtalkindustry__1__0_models.SupplyUpdateMemberHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyUpdateMemberResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.is_copy_dept):
+            body['isCopyDept'] = request.is_copy_dept
+        if not UtilClient.is_unset(request.member_title):
+            body['memberTitle'] = request.member_title
+        if not UtilClient.is_unset(request.member_work_number):
+            body['memberWorkNumber'] = request.member_work_number
+        if not UtilClient.is_unset(request.mobile):
+            body['mobile'] = request.mobile
+        if not UtilClient.is_unset(request.new_dept_id):
+            body['newDeptId'] = request.new_dept_id
+        if not UtilClient.is_unset(request.old_dept_id):
+            body['oldDeptId'] = request.old_dept_id
+        if not UtilClient.is_unset(request.role_id_list):
+            body['roleIdList'] = request.role_id_list
+        if not UtilClient.is_unset(request.union_id):
+            body['unionId'] = request.union_id
+        if not UtilClient.is_unset(request.user_id):
+            body['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='SupplyUpdateMember',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/members',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyUpdateMemberResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def supply_update_member_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyUpdateMemberRequest,
+        headers: dingtalkindustry__1__0_models.SupplyUpdateMemberHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyUpdateMemberResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.is_copy_dept):
+            body['isCopyDept'] = request.is_copy_dept
+        if not UtilClient.is_unset(request.member_title):
+            body['memberTitle'] = request.member_title
+        if not UtilClient.is_unset(request.member_work_number):
+            body['memberWorkNumber'] = request.member_work_number
+        if not UtilClient.is_unset(request.mobile):
+            body['mobile'] = request.mobile
+        if not UtilClient.is_unset(request.new_dept_id):
+            body['newDeptId'] = request.new_dept_id
+        if not UtilClient.is_unset(request.old_dept_id):
+            body['oldDeptId'] = request.old_dept_id
+        if not UtilClient.is_unset(request.role_id_list):
+            body['roleIdList'] = request.role_id_list
+        if not UtilClient.is_unset(request.union_id):
+            body['unionId'] = request.union_id
+        if not UtilClient.is_unset(request.user_id):
+            body['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='SupplyUpdateMember',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/members',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyUpdateMemberResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def supply_update_member(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyUpdateMemberRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyUpdateMemberResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyUpdateMemberHeaders()
+        return self.supply_update_member_with_options(request, headers, runtime)
+
+    async def supply_update_member_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyUpdateMemberRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyUpdateMemberResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyUpdateMemberHeaders()
+        return await self.supply_update_member_with_options_async(request, headers, runtime)
+
+    def supply_update_partner_type_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyUpdatePartnerTypeRequest,
+        headers: dingtalkindustry__1__0_models.SupplyUpdatePartnerTypeHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyUpdatePartnerTypeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.label_id):
+            query['labelId'] = request.label_id
+        if not UtilClient.is_unset(request.name):
+            query['name'] = request.name
+        if not UtilClient.is_unset(request.super_id):
+            query['superId'] = request.super_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyUpdatePartnerType',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/partnerLabels',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyUpdatePartnerTypeResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def supply_update_partner_type_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyUpdatePartnerTypeRequest,
+        headers: dingtalkindustry__1__0_models.SupplyUpdatePartnerTypeHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyUpdatePartnerTypeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.label_id):
+            query['labelId'] = request.label_id
+        if not UtilClient.is_unset(request.name):
+            query['name'] = request.name
+        if not UtilClient.is_unset(request.super_id):
+            query['superId'] = request.super_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyUpdatePartnerType',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/partnerLabels',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyUpdatePartnerTypeResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def supply_update_partner_type(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyUpdatePartnerTypeRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyUpdatePartnerTypeResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyUpdatePartnerTypeHeaders()
+        return self.supply_update_partner_type_with_options(request, headers, runtime)
+
+    async def supply_update_partner_type_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyUpdatePartnerTypeRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyUpdatePartnerTypeResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyUpdatePartnerTypeHeaders()
+        return await self.supply_update_partner_type_with_options_async(request, headers, runtime)
+
+    def supply_update_role_with_options(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyUpdateRoleRequest,
+        headers: dingtalkindustry__1__0_models.SupplyUpdateRoleHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyUpdateRoleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.is_role_group):
+            query['isRoleGroup'] = request.is_role_group
+        if not UtilClient.is_unset(request.role_id):
+            query['roleId'] = request.role_id
+        if not UtilClient.is_unset(request.role_name):
+            query['roleName'] = request.role_name
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyUpdateRole',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/roles',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyUpdateRoleResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def supply_update_role_with_options_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyUpdateRoleRequest,
+        headers: dingtalkindustry__1__0_models.SupplyUpdateRoleHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkindustry__1__0_models.SupplyUpdateRoleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.is_role_group):
+            query['isRoleGroup'] = request.is_role_group
+        if not UtilClient.is_unset(request.role_id):
+            query['roleId'] = request.role_id
+        if not UtilClient.is_unset(request.role_name):
+            query['roleName'] = request.role_name
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SupplyUpdateRole',
+            version='industry_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/industry/supplyChains/roles',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkindustry__1__0_models.SupplyUpdateRoleResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def supply_update_role(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyUpdateRoleRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyUpdateRoleResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyUpdateRoleHeaders()
+        return self.supply_update_role_with_options(request, headers, runtime)
+
+    async def supply_update_role_async(
+        self,
+        request: dingtalkindustry__1__0_models.SupplyUpdateRoleRequest,
+    ) -> dingtalkindustry__1__0_models.SupplyUpdateRoleResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkindustry__1__0_models.SupplyUpdateRoleHeaders()
+        return await self.supply_update_role_with_options_async(request, headers, runtime)
+
     def update_user_extend_info_with_options(
         self,
         user_id: str,
         request: dingtalkindustry__1__0_models.UpdateUserExtendInfoRequest,
         headers: dingtalkindustry__1__0_models.UpdateUserExtendInfoHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkindustry__1__0_models.UpdateUserExtendInfoResponse:
```

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -10074,19 +10074,21 @@
 class DigitalStoreRolesResponseBodyContent(TeaModel):
     def __init__(
         self,
         level: int = None,
         role_code: str = None,
         role_id: int = None,
         role_name: str = None,
+        source: str = None,
     ):
         self.level = level
         self.role_code = role_code
         self.role_id = role_id
         self.role_name = role_name
+        self.source = source
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -10097,26 +10099,30 @@
             result['level'] = self.level
         if self.role_code is not None:
             result['roleCode'] = self.role_code
         if self.role_id is not None:
             result['roleId'] = self.role_id
         if self.role_name is not None:
             result['roleName'] = self.role_name
+        if self.source is not None:
+            result['source'] = self.source
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('level') is not None:
             self.level = m.get('level')
         if m.get('roleCode') is not None:
             self.role_code = m.get('roleCode')
         if m.get('roleId') is not None:
             self.role_id = m.get('roleId')
         if m.get('roleName') is not None:
             self.role_name = m.get('roleName')
+        if m.get('source') is not None:
+            self.source = m.get('source')
         return self
 
 
 class DigitalStoreRolesResponseBody(TeaModel):
     def __init__(
         self,
         content: List[DigitalStoreRolesResponseBodyContent] = None,
@@ -22951,14 +22957,151 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = SaveUserExtendValuesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SupplAddRoleHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplAddRoleRequest(TeaModel):
+    def __init__(
+        self,
+        parent_role_group_id: str = None,
+        role_name: str = None,
+    ):
+        self.parent_role_group_id = parent_role_group_id
+        self.role_name = role_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.parent_role_group_id is not None:
+            result['parentRoleGroupId'] = self.parent_role_group_id
+        if self.role_name is not None:
+            result['roleName'] = self.role_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('parentRoleGroupId') is not None:
+            self.parent_role_group_id = m.get('parentRoleGroupId')
+        if m.get('roleName') is not None:
+            self.role_name = m.get('roleName')
+        return self
+
+
+class SupplAddRoleResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: str = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class SupplAddRoleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SupplAddRoleResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SupplAddRoleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class SupplyAddDeptHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -23168,20 +23311,22 @@
 
 class SupplyAddMemberRequest(TeaModel):
     def __init__(
         self,
         is_partner_manager: bool = None,
         member_mobile: str = None,
         member_name: str = None,
+        member_title: str = None,
         member_work_number: str = None,
         supply_dept_id: int = None,
     ):
         self.is_partner_manager = is_partner_manager
         self.member_mobile = member_mobile
         self.member_name = member_name
+        self.member_title = member_title
         self.member_work_number = member_work_number
         self.supply_dept_id = supply_dept_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -23192,28 +23337,32 @@
         result = dict()
         if self.is_partner_manager is not None:
             result['isPartnerManager'] = self.is_partner_manager
         if self.member_mobile is not None:
             result['memberMobile'] = self.member_mobile
         if self.member_name is not None:
             result['memberName'] = self.member_name
+        if self.member_title is not None:
+            result['memberTitle'] = self.member_title
         if self.member_work_number is not None:
             result['memberWorkNumber'] = self.member_work_number
         if self.supply_dept_id is not None:
             result['supplyDeptId'] = self.supply_dept_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('isPartnerManager') is not None:
             self.is_partner_manager = m.get('isPartnerManager')
         if m.get('memberMobile') is not None:
             self.member_mobile = m.get('memberMobile')
         if m.get('memberName') is not None:
             self.member_name = m.get('memberName')
+        if m.get('memberTitle') is not None:
+            self.member_title = m.get('memberTitle')
         if m.get('memberWorkNumber') is not None:
             self.member_work_number = m.get('memberWorkNumber')
         if m.get('supplyDeptId') is not None:
             self.supply_dept_id = m.get('supplyDeptId')
         return self
 
 
@@ -23325,14 +23474,1514 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = SupplyAddMemberResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SupplyAddPartnerAdminsHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplyAddPartnerAdminsRequest(TeaModel):
+    def __init__(
+        self,
+        dept_id: int = None,
+        user_id: str = None,
+    ):
+        self.dept_id = dept_id
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dept_id is not None:
+            result['deptId'] = self.dept_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('deptId') is not None:
+            self.dept_id = m.get('deptId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class SupplyAddPartnerAdminsResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class SupplyAddPartnerAdminsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SupplyAddPartnerAdminsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SupplyAddPartnerAdminsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SupplyAddPartnerManagersHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplyAddPartnerManagersRequest(TeaModel):
+    def __init__(
+        self,
+        dept_id: int = None,
+        interface_id: str = None,
+        interface_type: str = None,
+    ):
+        self.dept_id = dept_id
+        self.interface_id = interface_id
+        self.interface_type = interface_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dept_id is not None:
+            result['deptId'] = self.dept_id
+        if self.interface_id is not None:
+            result['interfaceId'] = self.interface_id
+        if self.interface_type is not None:
+            result['interfaceType'] = self.interface_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('deptId') is not None:
+            self.dept_id = m.get('deptId')
+        if m.get('interfaceId') is not None:
+            self.interface_id = m.get('interfaceId')
+        if m.get('interfaceType') is not None:
+            self.interface_type = m.get('interfaceType')
+        return self
+
+
+class SupplyAddPartnerManagersResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class SupplyAddPartnerManagersResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SupplyAddPartnerManagersResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SupplyAddPartnerManagersResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SupplyAddPartnerTypeHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplyAddPartnerTypeRequest(TeaModel):
+    def __init__(
+        self,
+        name: str = None,
+        super_id: int = None,
+    ):
+        self.name = name
+        self.super_id = super_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.name is not None:
+            result['name'] = self.name
+        if self.super_id is not None:
+            result['superId'] = self.super_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('superId') is not None:
+            self.super_id = m.get('superId')
+        return self
+
+
+class SupplyAddPartnerTypeResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: int = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class SupplyAddPartnerTypeResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SupplyAddPartnerTypeResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SupplyAddPartnerTypeResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SupplyChainDeleteDeptHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplyChainDeleteDeptRequest(TeaModel):
+    def __init__(
+        self,
+        supply_dept_id: int = None,
+    ):
+        self.supply_dept_id = supply_dept_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.supply_dept_id is not None:
+            result['supplyDeptId'] = self.supply_dept_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('supplyDeptId') is not None:
+            self.supply_dept_id = m.get('supplyDeptId')
+        return self
+
+
+class SupplyChainDeleteDeptResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class SupplyChainDeleteDeptResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SupplyChainDeleteDeptResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SupplyChainDeleteDeptResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SupplyChainQueryDeptInfoHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplyChainQueryDeptInfoRequest(TeaModel):
+    def __init__(
+        self,
+        supply_dept_id: int = None,
+    ):
+        self.supply_dept_id = supply_dept_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.supply_dept_id is not None:
+            result['supplyDeptId'] = self.supply_dept_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('supplyDeptId') is not None:
+            self.supply_dept_id = m.get('supplyDeptId')
+        return self
+
+
+class SupplyChainQueryDeptInfoResponseBodyResultPartnerTypeInfoList(TeaModel):
+    def __init__(
+        self,
+        id: int = None,
+        name: str = None,
+        super_id: int = None,
+        super_name: str = None,
+    ):
+        self.id = id
+        self.name = name
+        self.super_id = super_id
+        self.super_name = super_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.id is not None:
+            result['id'] = self.id
+        if self.name is not None:
+            result['name'] = self.name
+        if self.super_id is not None:
+            result['superId'] = self.super_id
+        if self.super_name is not None:
+            result['superName'] = self.super_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('id') is not None:
+            self.id = m.get('id')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('superId') is not None:
+            self.super_id = m.get('superId')
+        if m.get('superName') is not None:
+            self.super_name = m.get('superName')
+        return self
+
+
+class SupplyChainQueryDeptInfoResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        dept_id: int = None,
+        dept_type: str = None,
+        has_sub_dept: bool = None,
+        name: str = None,
+        partner_number: str = None,
+        partner_type_info_list: List[SupplyChainQueryDeptInfoResponseBodyResultPartnerTypeInfoList] = None,
+        super_id: int = None,
+    ):
+        self.dept_id = dept_id
+        self.dept_type = dept_type
+        self.has_sub_dept = has_sub_dept
+        self.name = name
+        self.partner_number = partner_number
+        self.partner_type_info_list = partner_type_info_list
+        self.super_id = super_id
+
+    def validate(self):
+        if self.partner_type_info_list:
+            for k in self.partner_type_info_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dept_id is not None:
+            result['deptId'] = self.dept_id
+        if self.dept_type is not None:
+            result['deptType'] = self.dept_type
+        if self.has_sub_dept is not None:
+            result['hasSubDept'] = self.has_sub_dept
+        if self.name is not None:
+            result['name'] = self.name
+        if self.partner_number is not None:
+            result['partnerNumber'] = self.partner_number
+        result['partnerTypeInfoList'] = []
+        if self.partner_type_info_list is not None:
+            for k in self.partner_type_info_list:
+                result['partnerTypeInfoList'].append(k.to_map() if k else None)
+        if self.super_id is not None:
+            result['superId'] = self.super_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('deptId') is not None:
+            self.dept_id = m.get('deptId')
+        if m.get('deptType') is not None:
+            self.dept_type = m.get('deptType')
+        if m.get('hasSubDept') is not None:
+            self.has_sub_dept = m.get('hasSubDept')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('partnerNumber') is not None:
+            self.partner_number = m.get('partnerNumber')
+        self.partner_type_info_list = []
+        if m.get('partnerTypeInfoList') is not None:
+            for k in m.get('partnerTypeInfoList'):
+                temp_model = SupplyChainQueryDeptInfoResponseBodyResultPartnerTypeInfoList()
+                self.partner_type_info_list.append(temp_model.from_map(k))
+        if m.get('superId') is not None:
+            self.super_id = m.get('superId')
+        return self
+
+
+class SupplyChainQueryDeptInfoResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: SupplyChainQueryDeptInfoResponseBodyResult = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = SupplyChainQueryDeptInfoResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        return self
+
+
+class SupplyChainQueryDeptInfoResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SupplyChainQueryDeptInfoResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SupplyChainQueryDeptInfoResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SupplyChainUpdateDeptInfoHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplyChainUpdateDeptInfoRequest(TeaModel):
+    def __init__(
+        self,
+        name: str = None,
+        partner_number: str = None,
+        partner_type_list: List[int] = None,
+        super_id: int = None,
+        supply_dept_id: int = None,
+    ):
+        self.name = name
+        self.partner_number = partner_number
+        self.partner_type_list = partner_type_list
+        self.super_id = super_id
+        self.supply_dept_id = supply_dept_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.name is not None:
+            result['name'] = self.name
+        if self.partner_number is not None:
+            result['partnerNumber'] = self.partner_number
+        if self.partner_type_list is not None:
+            result['partnerTypeList'] = self.partner_type_list
+        if self.super_id is not None:
+            result['superId'] = self.super_id
+        if self.supply_dept_id is not None:
+            result['supplyDeptId'] = self.supply_dept_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('partnerNumber') is not None:
+            self.partner_number = m.get('partnerNumber')
+        if m.get('partnerTypeList') is not None:
+            self.partner_type_list = m.get('partnerTypeList')
+        if m.get('superId') is not None:
+            self.super_id = m.get('superId')
+        if m.get('supplyDeptId') is not None:
+            self.supply_dept_id = m.get('supplyDeptId')
+        return self
+
+
+class SupplyChainUpdateDeptInfoResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class SupplyChainUpdateDeptInfoResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SupplyChainUpdateDeptInfoResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SupplyChainUpdateDeptInfoResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SupplyDeletePartnerAdminsHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplyDeletePartnerAdminsRequest(TeaModel):
+    def __init__(
+        self,
+        dept_id: int = None,
+        user_id: str = None,
+    ):
+        self.dept_id = dept_id
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dept_id is not None:
+            result['deptId'] = self.dept_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('deptId') is not None:
+            self.dept_id = m.get('deptId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class SupplyDeletePartnerAdminsResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class SupplyDeletePartnerAdminsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SupplyDeletePartnerAdminsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SupplyDeletePartnerAdminsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SupplyDeletePartnerManagersHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplyDeletePartnerManagersRequest(TeaModel):
+    def __init__(
+        self,
+        dept_id: int = None,
+        interface_id: str = None,
+        interface_type: str = None,
+    ):
+        self.dept_id = dept_id
+        self.interface_id = interface_id
+        self.interface_type = interface_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dept_id is not None:
+            result['deptId'] = self.dept_id
+        if self.interface_id is not None:
+            result['interfaceId'] = self.interface_id
+        if self.interface_type is not None:
+            result['interfaceType'] = self.interface_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('deptId') is not None:
+            self.dept_id = m.get('deptId')
+        if m.get('interfaceId') is not None:
+            self.interface_id = m.get('interfaceId')
+        if m.get('interfaceType') is not None:
+            self.interface_type = m.get('interfaceType')
+        return self
+
+
+class SupplyDeletePartnerManagersResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class SupplyDeletePartnerManagersResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SupplyDeletePartnerManagersResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SupplyDeletePartnerManagersResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SupplyDeletePartnerTypeHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplyDeletePartnerTypeRequest(TeaModel):
+    def __init__(
+        self,
+        label_id: int = None,
+    ):
+        self.label_id = label_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.label_id is not None:
+            result['labelId'] = self.label_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('labelId') is not None:
+            self.label_id = m.get('labelId')
+        return self
+
+
+class SupplyDeletePartnerTypeResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class SupplyDeletePartnerTypeResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SupplyDeletePartnerTypeResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SupplyDeletePartnerTypeResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SupplyDeleteRoleHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplyDeleteRoleRequest(TeaModel):
+    def __init__(
+        self,
+        is_role_group: bool = None,
+        role_id: str = None,
+    ):
+        self.is_role_group = is_role_group
+        self.role_id = role_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.is_role_group is not None:
+            result['isRoleGroup'] = self.is_role_group
+        if self.role_id is not None:
+            result['roleId'] = self.role_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('isRoleGroup') is not None:
+            self.is_role_group = m.get('isRoleGroup')
+        if m.get('roleId') is not None:
+            self.role_id = m.get('roleId')
+        return self
+
+
+class SupplyDeleteRoleResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class SupplyDeleteRoleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SupplyDeleteRoleResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SupplyDeleteRoleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class SupplyGetMemberHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -23361,86 +25010,157 @@
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
 class SupplyGetMemberRequest(TeaModel):
     def __init__(
         self,
+        mobile: str = None,
         union_id: str = None,
         user_id: str = None,
     ):
+        self.mobile = mobile
         self.union_id = union_id
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.mobile is not None:
+            result['mobile'] = self.mobile
         if self.union_id is not None:
             result['unionId'] = self.union_id
         if self.user_id is not None:
             result['userId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('mobile') is not None:
+            self.mobile = m.get('mobile')
         if m.get('unionId') is not None:
             self.union_id = m.get('unionId')
         if m.get('userId') is not None:
             self.user_id = m.get('userId')
         return self
 
 
+class SupplyGetMemberResponseBodyResultRoleInfoList(TeaModel):
+    def __init__(
+        self,
+        role_id: str = None,
+        role_name: str = None,
+    ):
+        self.role_id = role_id
+        self.role_name = role_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.role_id is not None:
+            result['roleId'] = self.role_id
+        if self.role_name is not None:
+            result['roleName'] = self.role_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('roleId') is not None:
+            self.role_id = m.get('roleId')
+        if m.get('roleName') is not None:
+            self.role_name = m.get('roleName')
+        return self
+
+
 class SupplyGetMemberResponseBodyResult(TeaModel):
     def __init__(
         self,
+        dept_id_list: List[int] = None,
         ding_member_status: str = None,
         is_active: bool = None,
         member_name: str = None,
+        member_title: str = None,
         member_work_number: str = None,
+        role_info_list: List[SupplyGetMemberResponseBodyResultRoleInfoList] = None,
+        supply_node_list: List[int] = None,
     ):
+        self.dept_id_list = dept_id_list
         self.ding_member_status = ding_member_status
         self.is_active = is_active
         self.member_name = member_name
+        self.member_title = member_title
         self.member_work_number = member_work_number
+        self.role_info_list = role_info_list
+        self.supply_node_list = supply_node_list
 
     def validate(self):
-        pass
+        if self.role_info_list:
+            for k in self.role_info_list:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.dept_id_list is not None:
+            result['deptIdList'] = self.dept_id_list
         if self.ding_member_status is not None:
             result['dingMemberStatus'] = self.ding_member_status
         if self.is_active is not None:
             result['isActive'] = self.is_active
         if self.member_name is not None:
             result['memberName'] = self.member_name
+        if self.member_title is not None:
+            result['memberTitle'] = self.member_title
         if self.member_work_number is not None:
             result['memberWorkNumber'] = self.member_work_number
+        result['roleInfoList'] = []
+        if self.role_info_list is not None:
+            for k in self.role_info_list:
+                result['roleInfoList'].append(k.to_map() if k else None)
+        if self.supply_node_list is not None:
+            result['supplyNodeList'] = self.supply_node_list
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('deptIdList') is not None:
+            self.dept_id_list = m.get('deptIdList')
         if m.get('dingMemberStatus') is not None:
             self.ding_member_status = m.get('dingMemberStatus')
         if m.get('isActive') is not None:
             self.is_active = m.get('isActive')
         if m.get('memberName') is not None:
             self.member_name = m.get('memberName')
+        if m.get('memberTitle') is not None:
+            self.member_title = m.get('memberTitle')
         if m.get('memberWorkNumber') is not None:
             self.member_work_number = m.get('memberWorkNumber')
+        self.role_info_list = []
+        if m.get('roleInfoList') is not None:
+            for k in m.get('roleInfoList'):
+                temp_model = SupplyGetMemberResponseBodyResultRoleInfoList()
+                self.role_info_list.append(temp_model.from_map(k))
+        if m.get('supplyNodeList') is not None:
+            self.supply_node_list = m.get('supplyNodeList')
         return self
 
 
 class SupplyGetMemberResponseBody(TeaModel):
     def __init__(
         self,
         result: SupplyGetMemberResponseBodyResult = None,
@@ -23587,21 +25307,23 @@
 
 class SupplyListDeptMembersResponseBodyList(TeaModel):
     def __init__(
         self,
         ding_member_status: str = None,
         is_active: bool = None,
         member_name: str = None,
+        member_title: str = None,
         member_work_number: str = None,
         union_id: str = None,
         user_id: str = None,
     ):
         self.ding_member_status = ding_member_status
         self.is_active = is_active
         self.member_name = member_name
+        self.member_title = member_title
         self.member_work_number = member_work_number
         self.union_id = union_id
         self.user_id = user_id
 
     def validate(self):
         pass
 
@@ -23613,14 +25335,16 @@
         result = dict()
         if self.ding_member_status is not None:
             result['dingMemberStatus'] = self.ding_member_status
         if self.is_active is not None:
             result['isActive'] = self.is_active
         if self.member_name is not None:
             result['memberName'] = self.member_name
+        if self.member_title is not None:
+            result['memberTitle'] = self.member_title
         if self.member_work_number is not None:
             result['memberWorkNumber'] = self.member_work_number
         if self.union_id is not None:
             result['unionId'] = self.union_id
         if self.user_id is not None:
             result['userId'] = self.user_id
         return result
@@ -23629,14 +25353,16 @@
         m = m or dict()
         if m.get('dingMemberStatus') is not None:
             self.ding_member_status = m.get('dingMemberStatus')
         if m.get('isActive') is not None:
             self.is_active = m.get('isActive')
         if m.get('memberName') is not None:
             self.member_name = m.get('memberName')
+        if m.get('memberTitle') is not None:
+            self.member_title = m.get('memberTitle')
         if m.get('memberWorkNumber') is not None:
             self.member_work_number = m.get('memberWorkNumber')
         if m.get('unionId') is not None:
             self.union_id = m.get('unionId')
         if m.get('userId') is not None:
             self.user_id = m.get('userId')
         return self
@@ -23723,14 +25449,1630 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = SupplyListDeptMembersResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SupplyListPartnerAdminsHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplyListPartnerAdminsRequest(TeaModel):
+    def __init__(
+        self,
+        dept_id: int = None,
+    ):
+        self.dept_id = dept_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dept_id is not None:
+            result['deptId'] = self.dept_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('deptId') is not None:
+            self.dept_id = m.get('deptId')
+        return self
+
+
+class SupplyListPartnerAdminsResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        name: str = None,
+        union_id: str = None,
+        user_id: str = None,
+    ):
+        self.name = name
+        self.union_id = union_id
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.name is not None:
+            result['name'] = self.name
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class SupplyListPartnerAdminsResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: List[SupplyListPartnerAdminsResponseBodyResult] = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            for k in self.result:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['result'] = []
+        if self.result is not None:
+            for k in self.result:
+                result['result'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.result = []
+        if m.get('result') is not None:
+            for k in m.get('result'):
+                temp_model = SupplyListPartnerAdminsResponseBodyResult()
+                self.result.append(temp_model.from_map(k))
+        return self
+
+
+class SupplyListPartnerAdminsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SupplyListPartnerAdminsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SupplyListPartnerAdminsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SupplyListPartnerManagersHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplyListPartnerManagersRequest(TeaModel):
+    def __init__(
+        self,
+        dept_id: int = None,
+    ):
+        self.dept_id = dept_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dept_id is not None:
+            result['deptId'] = self.dept_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('deptId') is not None:
+            self.dept_id = m.get('deptId')
+        return self
+
+
+class SupplyListPartnerManagersResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        dept_id: str = None,
+        dept_name: str = None,
+        interface_type: str = None,
+        user_id: str = None,
+        user_name: str = None,
+    ):
+        self.dept_id = dept_id
+        self.dept_name = dept_name
+        self.interface_type = interface_type
+        self.user_id = user_id
+        self.user_name = user_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dept_id is not None:
+            result['deptId'] = self.dept_id
+        if self.dept_name is not None:
+            result['deptName'] = self.dept_name
+        if self.interface_type is not None:
+            result['interfaceType'] = self.interface_type
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        if self.user_name is not None:
+            result['userName'] = self.user_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('deptId') is not None:
+            self.dept_id = m.get('deptId')
+        if m.get('deptName') is not None:
+            self.dept_name = m.get('deptName')
+        if m.get('interfaceType') is not None:
+            self.interface_type = m.get('interfaceType')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        if m.get('userName') is not None:
+            self.user_name = m.get('userName')
+        return self
+
+
+class SupplyListPartnerManagersResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: List[SupplyListPartnerManagersResponseBodyResult] = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            for k in self.result:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['result'] = []
+        if self.result is not None:
+            for k in self.result:
+                result['result'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.result = []
+        if m.get('result') is not None:
+            for k in m.get('result'):
+                temp_model = SupplyListPartnerManagersResponseBodyResult()
+                self.result.append(temp_model.from_map(k))
+        return self
+
+
+class SupplyListPartnerManagersResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SupplyListPartnerManagersResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SupplyListPartnerManagersResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SupplyListPartnerTypeHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplyListPartnerTypeRequest(TeaModel):
+    def __init__(
+        self,
+        label_id: int = None,
+    ):
+        self.label_id = label_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.label_id is not None:
+            result['labelId'] = self.label_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('labelId') is not None:
+            self.label_id = m.get('labelId')
+        return self
+
+
+class SupplyListPartnerTypeResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        label_id: int = None,
+        name: str = None,
+        super_id: int = None,
+    ):
+        self.label_id = label_id
+        self.name = name
+        self.super_id = super_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.label_id is not None:
+            result['labelId'] = self.label_id
+        if self.name is not None:
+            result['name'] = self.name
+        if self.super_id is not None:
+            result['superId'] = self.super_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('labelId') is not None:
+            self.label_id = m.get('labelId')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('superId') is not None:
+            self.super_id = m.get('superId')
+        return self
+
+
+class SupplyListPartnerTypeResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: List[SupplyListPartnerTypeResponseBodyResult] = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            for k in self.result:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['result'] = []
+        if self.result is not None:
+            for k in self.result:
+                result['result'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.result = []
+        if m.get('result') is not None:
+            for k in m.get('result'):
+                temp_model = SupplyListPartnerTypeResponseBodyResult()
+                self.result.append(temp_model.from_map(k))
+        return self
+
+
+class SupplyListPartnerTypeResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SupplyListPartnerTypeResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SupplyListPartnerTypeResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SupplyListRoleHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplyListRoleRequest(TeaModel):
+    def __init__(
+        self,
+        parent_role_id: str = None,
+    ):
+        self.parent_role_id = parent_role_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.parent_role_id is not None:
+            result['parentRoleId'] = self.parent_role_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('parentRoleId') is not None:
+            self.parent_role_id = m.get('parentRoleId')
+        return self
+
+
+class SupplyListRoleResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        is_role_group: bool = None,
+        role_id: str = None,
+        role_name: str = None,
+    ):
+        self.is_role_group = is_role_group
+        self.role_id = role_id
+        self.role_name = role_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.is_role_group is not None:
+            result['isRoleGroup'] = self.is_role_group
+        if self.role_id is not None:
+            result['roleId'] = self.role_id
+        if self.role_name is not None:
+            result['roleName'] = self.role_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('isRoleGroup') is not None:
+            self.is_role_group = m.get('isRoleGroup')
+        if m.get('roleId') is not None:
+            self.role_id = m.get('roleId')
+        if m.get('roleName') is not None:
+            self.role_name = m.get('roleName')
+        return self
+
+
+class SupplyListRoleResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: List[SupplyListRoleResponseBodyResult] = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            for k in self.result:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['result'] = []
+        if self.result is not None:
+            for k in self.result:
+                result['result'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.result = []
+        if m.get('result') is not None:
+            for k in m.get('result'):
+                temp_model = SupplyListRoleResponseBodyResult()
+                self.result.append(temp_model.from_map(k))
+        return self
+
+
+class SupplyListRoleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SupplyListRoleResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SupplyListRoleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SupplyListSubDeptHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplyListSubDeptRequest(TeaModel):
+    def __init__(
+        self,
+        supply_dept_id: int = None,
+    ):
+        self.supply_dept_id = supply_dept_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.supply_dept_id is not None:
+            result['supplyDeptId'] = self.supply_dept_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('supplyDeptId') is not None:
+            self.supply_dept_id = m.get('supplyDeptId')
+        return self
+
+
+class SupplyListSubDeptResponseBodyResultPartnerTypeInfoList(TeaModel):
+    def __init__(
+        self,
+        id: int = None,
+        name: str = None,
+        super_id: int = None,
+        super_name: str = None,
+    ):
+        self.id = id
+        self.name = name
+        self.super_id = super_id
+        self.super_name = super_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.id is not None:
+            result['id'] = self.id
+        if self.name is not None:
+            result['name'] = self.name
+        if self.super_id is not None:
+            result['superId'] = self.super_id
+        if self.super_name is not None:
+            result['superName'] = self.super_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('id') is not None:
+            self.id = m.get('id')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('superId') is not None:
+            self.super_id = m.get('superId')
+        if m.get('superName') is not None:
+            self.super_name = m.get('superName')
+        return self
+
+
+class SupplyListSubDeptResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        dept_id: int = None,
+        dept_type: str = None,
+        has_sub_dept: bool = None,
+        name: str = None,
+        partner_number: str = None,
+        partner_type_info_list: List[SupplyListSubDeptResponseBodyResultPartnerTypeInfoList] = None,
+        super_id: int = None,
+    ):
+        self.dept_id = dept_id
+        self.dept_type = dept_type
+        self.has_sub_dept = has_sub_dept
+        self.name = name
+        self.partner_number = partner_number
+        self.partner_type_info_list = partner_type_info_list
+        self.super_id = super_id
+
+    def validate(self):
+        if self.partner_type_info_list:
+            for k in self.partner_type_info_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dept_id is not None:
+            result['deptId'] = self.dept_id
+        if self.dept_type is not None:
+            result['deptType'] = self.dept_type
+        if self.has_sub_dept is not None:
+            result['hasSubDept'] = self.has_sub_dept
+        if self.name is not None:
+            result['name'] = self.name
+        if self.partner_number is not None:
+            result['partnerNumber'] = self.partner_number
+        result['partnerTypeInfoList'] = []
+        if self.partner_type_info_list is not None:
+            for k in self.partner_type_info_list:
+                result['partnerTypeInfoList'].append(k.to_map() if k else None)
+        if self.super_id is not None:
+            result['superId'] = self.super_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('deptId') is not None:
+            self.dept_id = m.get('deptId')
+        if m.get('deptType') is not None:
+            self.dept_type = m.get('deptType')
+        if m.get('hasSubDept') is not None:
+            self.has_sub_dept = m.get('hasSubDept')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('partnerNumber') is not None:
+            self.partner_number = m.get('partnerNumber')
+        self.partner_type_info_list = []
+        if m.get('partnerTypeInfoList') is not None:
+            for k in m.get('partnerTypeInfoList'):
+                temp_model = SupplyListSubDeptResponseBodyResultPartnerTypeInfoList()
+                self.partner_type_info_list.append(temp_model.from_map(k))
+        if m.get('superId') is not None:
+            self.super_id = m.get('superId')
+        return self
+
+
+class SupplyListSubDeptResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: List[SupplyListSubDeptResponseBodyResult] = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            for k in self.result:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['result'] = []
+        if self.result is not None:
+            for k in self.result:
+                result['result'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.result = []
+        if m.get('result') is not None:
+            for k in m.get('result'):
+                temp_model = SupplyListSubDeptResponseBodyResult()
+                self.result.append(temp_model.from_map(k))
+        return self
+
+
+class SupplyListSubDeptResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SupplyListSubDeptResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SupplyListSubDeptResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SupplyQueryPartnerTypeHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplyQueryPartnerTypeRequest(TeaModel):
+    def __init__(
+        self,
+        label_id: int = None,
+    ):
+        self.label_id = label_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.label_id is not None:
+            result['labelId'] = self.label_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('labelId') is not None:
+            self.label_id = m.get('labelId')
+        return self
+
+
+class SupplyQueryPartnerTypeResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        label_id: int = None,
+        name: str = None,
+        super_id: int = None,
+    ):
+        self.label_id = label_id
+        self.name = name
+        self.super_id = super_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.label_id is not None:
+            result['labelId'] = self.label_id
+        if self.name is not None:
+            result['name'] = self.name
+        if self.super_id is not None:
+            result['superId'] = self.super_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('labelId') is not None:
+            self.label_id = m.get('labelId')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('superId') is not None:
+            self.super_id = m.get('superId')
+        return self
+
+
+class SupplyQueryPartnerTypeResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: SupplyQueryPartnerTypeResponseBodyResult = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = SupplyQueryPartnerTypeResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        return self
+
+
+class SupplyQueryPartnerTypeResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SupplyQueryPartnerTypeResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SupplyQueryPartnerTypeResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SupplyUpdateMemberHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplyUpdateMemberRequest(TeaModel):
+    def __init__(
+        self,
+        is_copy_dept: bool = None,
+        member_title: str = None,
+        member_work_number: str = None,
+        mobile: str = None,
+        new_dept_id: int = None,
+        old_dept_id: int = None,
+        role_id_list: List[str] = None,
+        union_id: str = None,
+        user_id: str = None,
+    ):
+        self.is_copy_dept = is_copy_dept
+        self.member_title = member_title
+        self.member_work_number = member_work_number
+        self.mobile = mobile
+        self.new_dept_id = new_dept_id
+        self.old_dept_id = old_dept_id
+        self.role_id_list = role_id_list
+        self.union_id = union_id
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.is_copy_dept is not None:
+            result['isCopyDept'] = self.is_copy_dept
+        if self.member_title is not None:
+            result['memberTitle'] = self.member_title
+        if self.member_work_number is not None:
+            result['memberWorkNumber'] = self.member_work_number
+        if self.mobile is not None:
+            result['mobile'] = self.mobile
+        if self.new_dept_id is not None:
+            result['newDeptId'] = self.new_dept_id
+        if self.old_dept_id is not None:
+            result['oldDeptId'] = self.old_dept_id
+        if self.role_id_list is not None:
+            result['roleIdList'] = self.role_id_list
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('isCopyDept') is not None:
+            self.is_copy_dept = m.get('isCopyDept')
+        if m.get('memberTitle') is not None:
+            self.member_title = m.get('memberTitle')
+        if m.get('memberWorkNumber') is not None:
+            self.member_work_number = m.get('memberWorkNumber')
+        if m.get('mobile') is not None:
+            self.mobile = m.get('mobile')
+        if m.get('newDeptId') is not None:
+            self.new_dept_id = m.get('newDeptId')
+        if m.get('oldDeptId') is not None:
+            self.old_dept_id = m.get('oldDeptId')
+        if m.get('roleIdList') is not None:
+            self.role_id_list = m.get('roleIdList')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class SupplyUpdateMemberResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class SupplyUpdateMemberResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SupplyUpdateMemberResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SupplyUpdateMemberResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SupplyUpdatePartnerTypeHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplyUpdatePartnerTypeRequest(TeaModel):
+    def __init__(
+        self,
+        label_id: int = None,
+        name: str = None,
+        super_id: int = None,
+    ):
+        self.label_id = label_id
+        self.name = name
+        self.super_id = super_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.label_id is not None:
+            result['labelId'] = self.label_id
+        if self.name is not None:
+            result['name'] = self.name
+        if self.super_id is not None:
+            result['superId'] = self.super_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('labelId') is not None:
+            self.label_id = m.get('labelId')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('superId') is not None:
+            self.super_id = m.get('superId')
+        return self
+
+
+class SupplyUpdatePartnerTypeResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class SupplyUpdatePartnerTypeResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SupplyUpdatePartnerTypeResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SupplyUpdatePartnerTypeResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SupplyUpdateRoleHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SupplyUpdateRoleRequest(TeaModel):
+    def __init__(
+        self,
+        is_role_group: bool = None,
+        role_id: str = None,
+        role_name: str = None,
+    ):
+        self.is_role_group = is_role_group
+        self.role_id = role_id
+        self.role_name = role_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.is_role_group is not None:
+            result['isRoleGroup'] = self.is_role_group
+        if self.role_id is not None:
+            result['roleId'] = self.role_id
+        if self.role_name is not None:
+            result['roleName'] = self.role_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('isRoleGroup') is not None:
+            self.is_role_group = m.get('isRoleGroup')
+        if m.get('roleId') is not None:
+            self.role_id = m.get('roleId')
+        if m.get('roleName') is not None:
+            self.role_name = m.get('roleName')
+        return self
+
+
+class SupplyUpdateRoleResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class SupplyUpdateRoleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SupplyUpdateRoleResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SupplyUpdateRoleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class UpdateUserExtendInfoHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.0.15
+Version: 2.0.16
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.16/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -264,8 +264,11 @@
 alibabacloud_dingtalk/workflow_1_0/client.py
 alibabacloud_dingtalk/workflow_1_0/models.py
 alibabacloud_dingtalk/workrecord_1_0/__init__.py
 alibabacloud_dingtalk/workrecord_1_0/client.py
 alibabacloud_dingtalk/workrecord_1_0/models.py
 alibabacloud_dingtalk/yida_1_0/__init__.py
 alibabacloud_dingtalk/yida_1_0/client.py
-alibabacloud_dingtalk/yida_1_0/models.py
+alibabacloud_dingtalk/yida_1_0/models.py
+alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+alibabacloud_dingtalk/yun_shu_1_0/client.py
+alibabacloud_dingtalk/yun_shu_1_0/models.py
```

### Comparing `alibabacloud_dingtalk-2.0.15/setup.py` & `alibabacloud_dingtalk-2.0.16/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 18/05/2023
+Created on 24/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

