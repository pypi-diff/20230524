# Comparing `tmp/aliyun-python-sdk-gpdb-1.1.5.tar.gz` & `tmp/aliyun-python-sdk-gpdb-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-gpdb-1.1.5.tar", last modified: Mon Sep 26 08:03:09 2022, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-gpdb-1.1.6.tar", last modified: Wed May 24 02:53:04 2023, max compression
```

## Comparing `aliyun-python-sdk-gpdb-1.1.5.tar` & `aliyun-python-sdk-gpdb-1.1.6.tar`

### file list

```diff
@@ -1,110 +1,113 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/
--rw-r--r--   0 root         (0) root         (0)      575 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1542 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      529 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyun_python_sdk_gpdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1542 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyun_python_sdk_gpdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6245 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyun_python_sdk_gpdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyun_python_sdk_gpdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyun_python_sdk_gpdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyun_python_sdk_gpdb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/
--rw-r--r--   0 root         (0) root         (0)       21 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1628 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/
--rw-r--r--   0 root         (0) root         (0)     1859 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/AddBuDBInstanceRelationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2757 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/AllocateInstancePublicConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1282 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/CheckServiceLinkedRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2717 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/CreateAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     3011 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/CreateDBInstancePlanRequest.py
--rw-r--r--   0 root         (0) root         (0)     6991 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/CreateDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     6730 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/CreateECSDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1642 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/CreateSampleDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1453 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/CreateServiceLinkedRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1817 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DeleteDBInstancePlanRequest.py
--rw-r--r--   0 root         (0) root         (0)     2060 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DeleteDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1857 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DeleteDatabaseRequest.py
--rw-r--r--   0 root         (0) root         (0)     1670 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeAccountsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1815 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeAvailableResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1481 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeBackupPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1662 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBClusterNodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2344 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBClusterPerformanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1885 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1869 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDataBloatRequest.py
--rw-r--r--   0 root         (0) root         (0)     1867 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDataSkewRequest.py
--rw-r--r--   0 root         (0) root         (0)     2456 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDiagnosisSummaryRequest.py
--rw-r--r--   0 root         (0) root         (0)     3072 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceErrorLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     1720 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceIPArrayListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1871 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceIndexUsageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1491 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceNetInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1674 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceOnECSAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2227 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstancePerformanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2623 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstancePlansRequest.py
--rw-r--r--   0 root         (0) root         (0)     2579 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceSQLPatternsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1483 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceSSLRequest.py
--rw-r--r--   0 root         (0) root         (0)     4374 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2963 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDataBackupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2251 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDataShareInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2022 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDataSharePerformanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1495 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisDimensionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2418 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisMonitorPerformanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3104 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1841 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisSQLInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1487 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDownloadRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1630 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeHealthStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2209 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeLogBackupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1851 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeModifyParameterLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     1477 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeParametersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2874 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeRdsVSwitchsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2705 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeRdsVpcsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1435 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1483 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeResourceUsageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1493 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeSQLCollectorPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1660 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeSQLLogByQueryIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     3813 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeSQLLogCountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2032 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeSQLLogFilesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2913 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeSQLLogRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2838 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeSQLLogsOnSliceRequest.py
--rw-r--r--   0 root         (0) root         (0)     4179 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeSQLLogsRequest.py
--rw-r--r--   0 root         (0) root         (0)     4400 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeSQLLogsV2Request.py
--rw-r--r--   0 root         (0) root         (0)     1646 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeSampleDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2541 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeSlowLogRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3990 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeSlowSQLLogsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2235 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeSpecificationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2526 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1666 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeUserEncryptionKeyListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2772 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DownloadDiagnosisRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3187 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1925 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ModifyAccountDescriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2730 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ModifyBackupPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1716 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceConnectionModeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2192 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceConnectionStringRequest.py
--rw-r--r--   0 root         (0) root         (0)     1973 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceDescriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2076 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceMaintainTimeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2313 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceNetworkTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2799 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1899 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceSSLRequest.py
--rw-r--r--   0 root         (0) root         (0)     1917 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ModifyParametersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1728 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ModifySQLCollectorPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2455 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ModifySecurityIpsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1636 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/PauseInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1676 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/RebalanceDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1969 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ReleaseInstancePublicConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1899 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ResetAccountPasswordRequest.py
--rw-r--r--   0 root         (0) root         (0)     1672 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/RestartDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1638 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ResumeInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2014 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/SetDBInstancePlanStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1881 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/SetDataShareInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1905 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/SwitchDBInstanceNetTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2994 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1642 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/UnloadSampleDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2972 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2772 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/UpdateDBInstancePlanRequest.py
--rw-r--r--   0 root         (0) root         (0)     3503 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/UpgradeDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2454 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/UpgradeDBVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2457 2022-09-26 08:03:09.000000 aliyun-python-sdk-gpdb-1.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:53:04.000000 aliyun-python-sdk-gpdb-1.1.6/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-05-24 02:53:04.000000 aliyun-python-sdk-gpdb-1.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:53:04.000000 aliyun-python-sdk-gpdb-1.1.6/aliyun_python_sdk_gpdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyun_python_sdk_gpdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6444 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyun_python_sdk_gpdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyun_python_sdk_gpdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyun_python_sdk_gpdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyun_python_sdk_gpdb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:53:04.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:53:04.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:53:04.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/
+-rw-r--r--   0 root         (0) root         (0)     1859 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/AddBuDBInstanceRelationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2757 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/AllocateInstancePublicConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CheckServiceLinkedRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2717 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CreateAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3011 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CreateDBInstancePlanRequest.py
+-rw-r--r--   0 root         (0) root         (0)     8602 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CreateDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6730 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CreateECSDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CreateSampleDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CreateServiceLinkedRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DeleteDBInstancePlanRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DeleteDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DeleteDatabaseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeAccountsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1815 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeAvailableResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1481 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeBackupPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBClusterNodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBClusterPerformanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDataBloatRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDataSkewRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDiagnosisSummaryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3072 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceErrorLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1720 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceIPArrayListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceIndexUsageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1491 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceNetInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceOnECSAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2227 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstancePerformanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2623 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstancePlansRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2579 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceSQLPatternsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceSSLRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4374 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDataBackupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDataShareInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDataSharePerformanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisDimensionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2418 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisMonitorPerformanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3104 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1841 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisSQLInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDownloadRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1630 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeHealthStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2209 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeLogBackupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeModifyParameterLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1477 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2874 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeRdsVSwitchsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2705 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeRdsVpcsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1435 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeResourceUsageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1493 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLCollectorPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogByQueryIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3813 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogCountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogFilesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2913 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2838 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogsOnSliceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4179 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4400 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogsV2Request.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSampleDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2541 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSlowLogRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3990 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSlowSQLLogsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSpecificationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSupportFeaturesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeUserEncryptionKeyListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1813 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeWaitingSQLInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3106 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeWaitingSQLRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2772 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DownloadDiagnosisRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3187 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyAccountDescriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2730 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyBackupPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceConnectionModeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceConnectionStringRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1973 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceDescriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceMaintainTimeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceNetworkTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceSSLRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1728 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifySQLCollectorPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2646 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifySecurityIpsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/PauseInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/RebalanceDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1969 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ReleaseInstancePublicConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ResetAccountPasswordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/RestartDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ResumeInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/SetDBInstancePlanStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/SetDataShareInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1905 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/SwitchDBInstanceNetTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2994 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/UnloadSampleDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2972 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2772 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/UpdateDBInstancePlanRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3987 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/UpgradeDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2454 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/UpgradeDBVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-24 02:53:04.000000 aliyun-python-sdk-gpdb-1.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-05-24 02:53:03.000000 aliyun-python-sdk-gpdb-1.1.6/setup.py
```

### Comparing `aliyun-python-sdk-gpdb-1.1.5/LICENSE` & `aliyun-python-sdk-gpdb-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/PKG-INFO` & `aliyun-python-sdk-gpdb-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-gpdb
-Version: 1.1.5
+Version: 1.1.6
 Summary: The gpdb module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-gpdb
```

### Comparing `aliyun-python-sdk-gpdb-1.1.5/README.rst` & `aliyun-python-sdk-gpdb-1.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyun_python_sdk_gpdb.egg-info/PKG-INFO` & `aliyun-python-sdk-gpdb-1.1.6/aliyun_python_sdk_gpdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-gpdb
-Version: 1.1.5
+Version: 1.1.6
 Summary: The gpdb module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-gpdb
```

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyun_python_sdk_gpdb.egg-info/SOURCES.txt` & `aliyun-python-sdk-gpdb-1.1.6/aliyun_python_sdk_gpdb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -66,16 +66,19 @@
 aliyunsdkgpdb/request/v20160503/DescribeSQLLogsOnSliceRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeSQLLogsRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeSQLLogsV2Request.py
 aliyunsdkgpdb/request/v20160503/DescribeSampleDataRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeSlowLogRecordsRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeSlowSQLLogsRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeSpecificationRequest.py
+aliyunsdkgpdb/request/v20160503/DescribeSupportFeaturesRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeTagsRequest.py
 aliyunsdkgpdb/request/v20160503/DescribeUserEncryptionKeyListRequest.py
+aliyunsdkgpdb/request/v20160503/DescribeWaitingSQLInfoRequest.py
+aliyunsdkgpdb/request/v20160503/DescribeWaitingSQLRecordsRequest.py
 aliyunsdkgpdb/request/v20160503/DownloadDiagnosisRecordsRequest.py
 aliyunsdkgpdb/request/v20160503/ListTagResourcesRequest.py
 aliyunsdkgpdb/request/v20160503/ModifyAccountDescriptionRequest.py
 aliyunsdkgpdb/request/v20160503/ModifyBackupPolicyRequest.py
 aliyunsdkgpdb/request/v20160503/ModifyDBInstanceConnectionModeRequest.py
 aliyunsdkgpdb/request/v20160503/ModifyDBInstanceConnectionStringRequest.py
 aliyunsdkgpdb/request/v20160503/ModifyDBInstanceDescriptionRequest.py
```

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/endpoint.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/AddBuDBInstanceRelationRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/AddBuDBInstanceRelationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/AllocateInstancePublicConnectionRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/AllocateInstancePublicConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/CheckServiceLinkedRoleRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CheckServiceLinkedRoleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/CreateAccountRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CreateAccountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/CreateDBInstancePlanRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CreateDBInstancePlanRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/CreateDBInstanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CreateECSDBInstanceRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class CreateDBInstanceRequest(RpcRequest):
+class CreateECSDBInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'CreateDBInstance')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'CreateECSDBInstance')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -37,24 +37,24 @@
 	def set_EngineVersion(self, EngineVersion):  # String
 		self.add_query_param('EngineVersion', EngineVersion)
 	def get_DBInstanceCategory(self): # String
 		return self.get_query_params().get('DBInstanceCategory')
 
 	def set_DBInstanceCategory(self, DBInstanceCategory):  # String
 		self.add_query_param('DBInstanceCategory', DBInstanceCategory)
-	def get_StorageType(self): # String
-		return self.get_query_params().get('StorageType')
-
-	def set_StorageType(self, StorageType):  # String
-		self.add_query_param('StorageType', StorageType)
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def get_EncryptionType(self): # String
+		return self.get_query_params().get('EncryptionType')
+
+	def set_EncryptionType(self, EncryptionType):  # String
+		self.add_query_param('EncryptionType', EncryptionType)
 	def get_DBInstanceDescription(self): # String
 		return self.get_query_params().get('DBInstanceDescription')
 
 	def set_DBInstanceDescription(self, DBInstanceDescription):  # String
 		self.add_query_param('DBInstanceDescription', DBInstanceDescription)
 	def get_Tags(self): # RepeatList
 		return self.get_query_params().get('Tag')
@@ -66,24 +66,29 @@
 			if Tag[depth1].get('Key') is not None:
 				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
 	def get_Period(self): # String
 		return self.get_query_params().get('Period')
 
 	def set_Period(self, Period):  # String
 		self.add_query_param('Period', Period)
+	def get_BackupId(self): # String
+		return self.get_query_params().get('BackupId')
+
+	def set_BackupId(self, BackupId):  # String
+		self.add_query_param('BackupId', BackupId)
+	def get_EncryptionKey(self): # String
+		return self.get_query_params().get('EncryptionKey')
+
+	def set_EncryptionKey(self, EncryptionKey):  # String
+		self.add_query_param('EncryptionKey', EncryptionKey)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_DBInstanceClass(self): # String
-		return self.get_query_params().get('DBInstanceClass')
-
-	def set_DBInstanceClass(self, DBInstanceClass):  # String
-		self.add_query_param('DBInstanceClass', DBInstanceClass)
 	def get_SecurityIPList(self): # String
 		return self.get_query_params().get('SecurityIPList')
 
 	def set_SecurityIPList(self, SecurityIPList):  # String
 		self.add_query_param('SecurityIPList', SecurityIPList)
 	def get_VSwitchId(self): # String
 		return self.get_query_params().get('VSwitchId')
@@ -111,54 +116,39 @@
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
 	def get_InstanceSpec(self): # String
 		return self.get_query_params().get('InstanceSpec')
 
 	def set_InstanceSpec(self, InstanceSpec):  # String
 		self.add_query_param('InstanceSpec', InstanceSpec)
-	def get_StorageSize(self): # Long
+	def get_StorageSize(self): # Integer
 		return self.get_query_params().get('StorageSize')
 
-	def set_StorageSize(self, StorageSize):  # Long
+	def set_StorageSize(self, StorageSize):  # Integer
 		self.add_query_param('StorageSize', StorageSize)
 	def get_SegStorageType(self): # String
 		return self.get_query_params().get('SegStorageType')
 
 	def set_SegStorageType(self, SegStorageType):  # String
 		self.add_query_param('SegStorageType', SegStorageType)
-	def get_MasterNodeNum(self): # String
+	def get_MasterNodeNum(self): # Integer
 		return self.get_query_params().get('MasterNodeNum')
 
-	def set_MasterNodeNum(self, MasterNodeNum):  # String
+	def set_MasterNodeNum(self, MasterNodeNum):  # Integer
 		self.add_query_param('MasterNodeNum', MasterNodeNum)
-	def get_SegNodeNum(self): # String
+	def get_SegNodeNum(self): # Integer
 		return self.get_query_params().get('SegNodeNum')
 
-	def set_SegNodeNum(self, SegNodeNum):  # String
+	def set_SegNodeNum(self, SegNodeNum):  # Integer
 		self.add_query_param('SegNodeNum', SegNodeNum)
 	def get_Engine(self): # String
 		return self.get_query_params().get('Engine')
 
 	def set_Engine(self, Engine):  # String
 		self.add_query_param('Engine', Engine)
-	def get_CreateSampleData(self): # Boolean
-		return self.get_query_params().get('CreateSampleData')
-
-	def set_CreateSampleData(self, CreateSampleData):  # Boolean
-		self.add_query_param('CreateSampleData', CreateSampleData)
-	def get_DBInstanceGroupCount(self): # String
-		return self.get_query_params().get('DBInstanceGroupCount')
-
-	def set_DBInstanceGroupCount(self, DBInstanceGroupCount):  # String
-		self.add_query_param('DBInstanceGroupCount', DBInstanceGroupCount)
-	def get_DBInstanceMode(self): # String
-		return self.get_query_params().get('DBInstanceMode')
-
-	def set_DBInstanceMode(self, DBInstanceMode):  # String
-		self.add_query_param('DBInstanceMode', DBInstanceMode)
 	def get_UsedTime(self): # String
 		return self.get_query_params().get('UsedTime')
 
 	def set_UsedTime(self, UsedTime):  # String
 		self.add_query_param('UsedTime', UsedTime)
 	def get_VPCId(self): # String
 		return self.get_query_params().get('VPCId')
@@ -166,7 +156,12 @@
 	def set_VPCId(self, VPCId):  # String
 		self.add_query_param('VPCId', VPCId)
 	def get_PayType(self): # String
 		return self.get_query_params().get('PayType')
 
 	def set_PayType(self, PayType):  # String
 		self.add_query_param('PayType', PayType)
+	def get_SrcDbInstanceName(self): # String
+		return self.get_query_params().get('SrcDbInstanceName')
+
+	def set_SrcDbInstanceName(self, SrcDbInstanceName):  # String
+		self.add_query_param('SrcDbInstanceName', SrcDbInstanceName)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/CreateECSDBInstanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CreateDBInstanceRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkgpdb.endpoint import endpoint_data
 
-class CreateECSDBInstanceRequest(RpcRequest):
+class CreateDBInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'CreateECSDBInstance')
+		RpcRequest.__init__(self, 'gpdb', '2016-05-03', 'CreateDBInstance')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -37,14 +37,19 @@
 	def set_EngineVersion(self, EngineVersion):  # String
 		self.add_query_param('EngineVersion', EngineVersion)
 	def get_DBInstanceCategory(self): # String
 		return self.get_query_params().get('DBInstanceCategory')
 
 	def set_DBInstanceCategory(self, DBInstanceCategory):  # String
 		self.add_query_param('DBInstanceCategory', DBInstanceCategory)
+	def get_StorageType(self): # String
+		return self.get_query_params().get('StorageType')
+
+	def set_StorageType(self, StorageType):  # String
+		self.add_query_param('StorageType', StorageType)
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_EncryptionType(self): # String
 		return self.get_query_params().get('EncryptionType')
@@ -52,43 +57,58 @@
 	def set_EncryptionType(self, EncryptionType):  # String
 		self.add_query_param('EncryptionType', EncryptionType)
 	def get_DBInstanceDescription(self): # String
 		return self.get_query_params().get('DBInstanceDescription')
 
 	def set_DBInstanceDescription(self, DBInstanceDescription):  # String
 		self.add_query_param('DBInstanceDescription', DBInstanceDescription)
+	def get_ServerlessMode(self): # String
+		return self.get_query_params().get('ServerlessMode')
+
+	def set_ServerlessMode(self, ServerlessMode):  # String
+		self.add_query_param('ServerlessMode', ServerlessMode)
 	def get_Tags(self): # RepeatList
 		return self.get_query_params().get('Tag')
 
 	def set_Tags(self, Tag):  # RepeatList
 		for depth1 in range(len(Tag)):
 			if Tag[depth1].get('Value') is not None:
 				self.add_query_param('Tag.' + str(depth1 + 1) + '.Value', Tag[depth1].get('Value'))
 			if Tag[depth1].get('Key') is not None:
 				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
 	def get_Period(self): # String
 		return self.get_query_params().get('Period')
 
 	def set_Period(self, Period):  # String
 		self.add_query_param('Period', Period)
-	def get_BackupId(self): # String
-		return self.get_query_params().get('BackupId')
+	def get_VectorConfigurationStatus(self): # String
+		return self.get_query_params().get('VectorConfigurationStatus')
 
-	def set_BackupId(self, BackupId):  # String
-		self.add_query_param('BackupId', BackupId)
+	def set_VectorConfigurationStatus(self, VectorConfigurationStatus):  # String
+		self.add_query_param('VectorConfigurationStatus', VectorConfigurationStatus)
 	def get_EncryptionKey(self): # String
 		return self.get_query_params().get('EncryptionKey')
 
 	def set_EncryptionKey(self, EncryptionKey):  # String
 		self.add_query_param('EncryptionKey', EncryptionKey)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
+	def get_SegDiskPerformanceLevel(self): # String
+		return self.get_query_params().get('SegDiskPerformanceLevel')
+
+	def set_SegDiskPerformanceLevel(self, SegDiskPerformanceLevel):  # String
+		self.add_query_param('SegDiskPerformanceLevel', SegDiskPerformanceLevel)
+	def get_DBInstanceClass(self): # String
+		return self.get_query_params().get('DBInstanceClass')
+
+	def set_DBInstanceClass(self, DBInstanceClass):  # String
+		self.add_query_param('DBInstanceClass', DBInstanceClass)
 	def get_SecurityIPList(self): # String
 		return self.get_query_params().get('SecurityIPList')
 
 	def set_SecurityIPList(self, SecurityIPList):  # String
 		self.add_query_param('SecurityIPList', SecurityIPList)
 	def get_VSwitchId(self): # String
 		return self.get_query_params().get('VSwitchId')
@@ -116,52 +136,72 @@
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
 	def get_InstanceSpec(self): # String
 		return self.get_query_params().get('InstanceSpec')
 
 	def set_InstanceSpec(self, InstanceSpec):  # String
 		self.add_query_param('InstanceSpec', InstanceSpec)
-	def get_StorageSize(self): # Integer
+	def get_StorageSize(self): # Long
 		return self.get_query_params().get('StorageSize')
 
-	def set_StorageSize(self, StorageSize):  # Integer
+	def set_StorageSize(self, StorageSize):  # Long
 		self.add_query_param('StorageSize', StorageSize)
 	def get_SegStorageType(self): # String
 		return self.get_query_params().get('SegStorageType')
 
 	def set_SegStorageType(self, SegStorageType):  # String
 		self.add_query_param('SegStorageType', SegStorageType)
-	def get_MasterNodeNum(self): # Integer
+	def get_MasterNodeNum(self): # String
 		return self.get_query_params().get('MasterNodeNum')
 
-	def set_MasterNodeNum(self, MasterNodeNum):  # Integer
+	def set_MasterNodeNum(self, MasterNodeNum):  # String
 		self.add_query_param('MasterNodeNum', MasterNodeNum)
-	def get_SegNodeNum(self): # Integer
+	def get_SegNodeNum(self): # String
 		return self.get_query_params().get('SegNodeNum')
 
-	def set_SegNodeNum(self, SegNodeNum):  # Integer
+	def set_SegNodeNum(self, SegNodeNum):  # String
 		self.add_query_param('SegNodeNum', SegNodeNum)
 	def get_Engine(self): # String
 		return self.get_query_params().get('Engine')
 
 	def set_Engine(self, Engine):  # String
 		self.add_query_param('Engine', Engine)
+	def get_CreateSampleData(self): # Boolean
+		return self.get_query_params().get('CreateSampleData')
+
+	def set_CreateSampleData(self, CreateSampleData):  # Boolean
+		self.add_query_param('CreateSampleData', CreateSampleData)
+	def get_DBInstanceGroupCount(self): # String
+		return self.get_query_params().get('DBInstanceGroupCount')
+
+	def set_DBInstanceGroupCount(self, DBInstanceGroupCount):  # String
+		self.add_query_param('DBInstanceGroupCount', DBInstanceGroupCount)
+	def get_DBInstanceMode(self): # String
+		return self.get_query_params().get('DBInstanceMode')
+
+	def set_DBInstanceMode(self, DBInstanceMode):  # String
+		self.add_query_param('DBInstanceMode', DBInstanceMode)
 	def get_UsedTime(self): # String
 		return self.get_query_params().get('UsedTime')
 
 	def set_UsedTime(self, UsedTime):  # String
 		self.add_query_param('UsedTime', UsedTime)
 	def get_VPCId(self): # String
 		return self.get_query_params().get('VPCId')
 
 	def set_VPCId(self, VPCId):  # String
 		self.add_query_param('VPCId', VPCId)
+	def get_ServerlessResource(self): # Integer
+		return self.get_query_params().get('ServerlessResource')
+
+	def set_ServerlessResource(self, ServerlessResource):  # Integer
+		self.add_query_param('ServerlessResource', ServerlessResource)
+	def get_IdleTime(self): # Integer
+		return self.get_query_params().get('IdleTime')
+
+	def set_IdleTime(self, IdleTime):  # Integer
+		self.add_query_param('IdleTime', IdleTime)
 	def get_PayType(self): # String
 		return self.get_query_params().get('PayType')
 
 	def set_PayType(self, PayType):  # String
 		self.add_query_param('PayType', PayType)
-	def get_SrcDbInstanceName(self): # String
-		return self.get_query_params().get('SrcDbInstanceName')
-
-	def set_SrcDbInstanceName(self, SrcDbInstanceName):  # String
-		self.add_query_param('SrcDbInstanceName', SrcDbInstanceName)
```

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/CreateSampleDataRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CreateSampleDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/CreateServiceLinkedRoleRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/CreateServiceLinkedRoleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DeleteDBInstancePlanRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DeleteDBInstancePlanRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DeleteDBInstanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DeleteDBInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DeleteDatabaseRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DeleteDatabaseRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeAccountsRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeAccountsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeAvailableResourcesRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeAvailableResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeBackupPolicyRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeBackupPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBClusterNodeRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBClusterNodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBClusterPerformanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBClusterPerformanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceAttributeRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDataBloatRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDataBloatRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDataSkewRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDataSkewRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDiagnosisSummaryRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceDiagnosisSummaryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceErrorLogRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceErrorLogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceIPArrayListRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceIPArrayListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceIndexUsageRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceIndexUsageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceNetInfoRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceNetInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceOnECSAttributeRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceOnECSAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstancePerformanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstancePerformanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstancePlansRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstancePlansRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceSQLPatternsRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceSQLPatternsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceSSLRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstanceSSLRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDBInstancesRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDBInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDataBackupsRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDataBackupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDataShareInstancesRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDataShareInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDataSharePerformanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDataSharePerformanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisDimensionsRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisDimensionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisMonitorPerformanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisMonitorPerformanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisRecordsRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisSQLInfoRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDiagnosisSQLInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeDownloadRecordsRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeDownloadRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeHealthStatusRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeHealthStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeLogBackupsRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeLogBackupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeModifyParameterLogRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeModifyParameterLogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeParametersRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeParametersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeRdsVSwitchsRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeRdsVSwitchsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeRdsVpcsRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeRdsVpcsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeRegionsRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeResourceUsageRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeResourceUsageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeSQLCollectorPolicyRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLCollectorPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeSQLLogByQueryIdRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogByQueryIdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeSQLLogCountRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogCountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeSQLLogFilesRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeSQLLogRecordsRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeSQLLogsOnSliceRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogsOnSliceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeSQLLogsRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeSQLLogsV2Request.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSQLLogsV2Request.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeSampleDataRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSampleDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeSlowLogRecordsRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSlowLogRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeSlowSQLLogsRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSlowSQLLogsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeSpecificationRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeSpecificationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeTagsRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DescribeUserEncryptionKeyListRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DescribeUserEncryptionKeyListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/DownloadDiagnosisRecordsRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/DownloadDiagnosisRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ListTagResourcesRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ListTagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ModifyAccountDescriptionRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyAccountDescriptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ModifyBackupPolicyRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyBackupPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceConnectionModeRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceConnectionModeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceConnectionStringRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceConnectionStringRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceDescriptionRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceDescriptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceMaintainTimeRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceMaintainTimeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceNetworkTypeRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceNetworkTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceResourceGroupRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceResourceGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceSSLRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyDBInstanceSSLRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ModifyParametersRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifyParametersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ModifySQLCollectorPolicyRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifySQLCollectorPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ModifySecurityIpsRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ModifySecurityIpsRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,19 @@
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_DBInstanceId(self): # String
 		return self.get_query_params().get('DBInstanceId')
 
 	def set_DBInstanceId(self, DBInstanceId):  # String
 		self.add_query_param('DBInstanceId', DBInstanceId)
+	def get_ModifyMode(self): # String
+		return self.get_query_params().get('ModifyMode')
+
+	def set_ModifyMode(self, ModifyMode):  # String
+		self.add_query_param('ModifyMode', ModifyMode)
 	def get_SecurityIPList(self): # String
 		return self.get_query_params().get('SecurityIPList')
 
 	def set_SecurityIPList(self, SecurityIPList):  # String
 		self.add_query_param('SecurityIPList', SecurityIPList)
 	def get_DBInstanceIPArrayAttribute(self): # String
 		return self.get_query_params().get('DBInstanceIPArrayAttribute')
```

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/PauseInstanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/PauseInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/RebalanceDBInstanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/RebalanceDBInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ReleaseInstancePublicConnectionRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ReleaseInstancePublicConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ResetAccountPasswordRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ResetAccountPasswordRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/RestartDBInstanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/RestartDBInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/ResumeInstanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/ResumeInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/SetDBInstancePlanStatusRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/SetDBInstancePlanStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/SetDataShareInstanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/SetDataShareInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/SwitchDBInstanceNetTypeRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/SwitchDBInstanceNetTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/TagResourcesRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/TagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/UnloadSampleDataRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/UnloadSampleDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/UntagResourcesRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/UntagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/UpdateDBInstancePlanRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/UpdateDBInstancePlanRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/UpgradeDBInstanceRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/UpgradeDBInstanceRequest.py`

 * *Files 24% similar despite different names*

```diff
@@ -37,14 +37,19 @@
 	def set_InstanceSpec(self, InstanceSpec):  # String
 		self.add_query_param('InstanceSpec', InstanceSpec)
 	def get_StorageSize(self): # String
 		return self.get_query_params().get('StorageSize')
 
 	def set_StorageSize(self, StorageSize):  # String
 		self.add_query_param('StorageSize', StorageSize)
+	def get_SegStorageType(self): # String
+		return self.get_query_params().get('SegStorageType')
+
+	def set_SegStorageType(self, SegStorageType):  # String
+		self.add_query_param('SegStorageType', SegStorageType)
 	def get_MasterNodeNum(self): # String
 		return self.get_query_params().get('MasterNodeNum')
 
 	def set_MasterNodeNum(self, MasterNodeNum):  # String
 		self.add_query_param('MasterNodeNum', MasterNodeNum)
 	def get_UpgradeType(self): # Long
 		return self.get_query_params().get('UpgradeType')
@@ -72,14 +77,19 @@
 	def set_DBInstanceGroupCount(self, DBInstanceGroupCount):  # String
 		self.add_query_param('DBInstanceGroupCount', DBInstanceGroupCount)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
+	def get_SegDiskPerformanceLevel(self): # String
+		return self.get_query_params().get('SegDiskPerformanceLevel')
+
+	def set_SegDiskPerformanceLevel(self, SegDiskPerformanceLevel):  # String
+		self.add_query_param('SegDiskPerformanceLevel', SegDiskPerformanceLevel)
 	def get_DBInstanceClass(self): # String
 		return self.get_query_params().get('DBInstanceClass')
 
 	def set_DBInstanceClass(self, DBInstanceClass):  # String
 		self.add_query_param('DBInstanceClass', DBInstanceClass)
 	def get_PayType(self): # String
 		return self.get_query_params().get('PayType')
```

### Comparing `aliyun-python-sdk-gpdb-1.1.5/aliyunsdkgpdb/request/v20160503/UpgradeDBVersionRequest.py` & `aliyun-python-sdk-gpdb-1.1.6/aliyunsdkgpdb/request/v20160503/UpgradeDBVersionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-gpdb-1.1.5/setup.py` & `aliyun-python-sdk-gpdb-1.1.6/setup.py`

 * *Files identical despite different names*

