# Comparing `tmp/vmware-cloud-foundation-health-monitoring-1.1.0.tar.gz` & `tmp/vmware-cloud-foundation-health-monitoring-1.1.0.1002.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmware-cloud-foundation-health-monitoring-1.1.0.tar", last modified: Wed May 17 00:05:06 2023, max compression
+gzip compressed data, was "vmware-cloud-foundation-health-monitoring-1.1.0.1002.tar", last modified: Tue May 23 23:07:20 2023, max compression
```

## Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.tar` & `vmware-cloud-foundation-health-monitoring-1.1.0.1002.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 00:05:06.933108 vmware-cloud-foundation-health-monitoring-1.1.0/
--rw-rw-rw-   0        0        0    10974 2023-05-17 00:05:06.933108 vmware-cloud-foundation-health-monitoring-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    10172 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/README.md
--rw-rw-rw-   0        0        0       86 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0     1041 2023-05-17 00:05:06.933108 vmware-cloud-foundation-health-monitoring-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-17 00:05:06.776855 vmware-cloud-foundation-health-monitoring-1.1.0/source/
-drwxrwxrwx   0        0        0        0 2023-05-17 00:05:06.792477 vmware-cloud-foundation-health-monitoring-1.1.0/source/artifacts/
--rw-rw-rw-   0        0        0        0 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/artifacts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 00:05:06.839357 vmware-cloud-foundation-health-monitoring-1.1.0/source/artifacts/vSAN/
--rw-rw-rw-   0        0        0    28694 2023-02-28 20:06:20.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/artifacts/vSAN/Dashboards.zip
--rw-rw-rw-   0        0        0    51491 2023-02-28 03:58:54.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/artifacts/vSAN/Notifications.json
--rw-rw-rw-   0        0        0    16701 2023-02-28 03:10:32.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/artifacts/vSAN/Supermetrics.json
--rw-rw-rw-   0        0        0    10147 2023-05-16 19:30:01.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/artifacts/vSAN/Views.zip
--rw-rw-rw-   0        0        0        0 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/artifacts/vSAN/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 00:05:06.839357 vmware-cloud-foundation-health-monitoring-1.1.0/source/examples/
--rw-rw-rw-   0        0        0        0 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/examples/__init__.py
--rwxrwxrwx   0        0        0       55 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/examples/run_send-data-to-vrops.bat
-drwxrwxrwx   0        0        0        0 2023-05-17 00:05:06.870606 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/
--rw-rw-rw-   0        0        0        0 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/__init__.py
--rw-rw-rw-   0        0        0     3199 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/encrypt-passwords.py
-drwxrwxrwx   0        0        0        0 2023-05-17 00:05:06.870606 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/encrypted_files/
--rw-rw-rw-   0        0        0        0 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/encrypted_files/__init__.py
--rw-rw-rw-   0        0        0     1456 2023-05-16 23:55:35.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/env.json
--rw-rw-rw-   0        0        0    70917 2023-05-16 23:58:10.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/send-data-to-vrops.py
-drwxrwxrwx   0        0        0        0 2023-05-17 00:05:06.901856 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/utils/
--rw-rw-rw-   0        0        0     5862 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/utils/FolderUtility.py
--rw-rw-rw-   0        0        0     4438 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/utils/LogUtility.py
--rw-rw-rw-   0        0        0     3042 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/utils/PSUtility.py
--rw-rw-rw-   0        0        0     7362 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/utils/SosRest.py
--rw-rw-rw-   0        0        0        0 2023-05-16 07:49:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/main/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 00:05:06.933108 vmware-cloud-foundation-health-monitoring-1.1.0/source/vmware_cloud_foundation_health_monitoring.egg-info/
--rw-rw-rw-   0        0        0    10974 2023-05-17 00:05:06.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/vmware_cloud_foundation_health_monitoring.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      915 2023-05-17 00:05:06.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/vmware_cloud_foundation_health_monitoring.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 00:05:06.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/vmware_cloud_foundation_health_monitoring.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-17 00:05:06.000000 vmware-cloud-foundation-health-monitoring-1.1.0/source/vmware_cloud_foundation_health_monitoring.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 23:07:20.040761 vmware-cloud-foundation-health-monitoring-1.1.0.1002/
+-rw-rw-rw-   0        0        0    10980 2023-05-23 23:07:20.056387 vmware-cloud-foundation-health-monitoring-1.1.0.1002/PKG-INFO
+-rw-rw-rw-   0        0        0    10173 2023-05-23 16:56:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/pyproject.toml
+-rw-rw-rw-   0        0        0     1046 2023-05-23 23:07:20.056387 vmware-cloud-foundation-health-monitoring-1.1.0.1002/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-23 23:07:19.993891 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/
+drwxrwxrwx   0        0        0        0 2023-05-23 23:07:20.009512 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/artifacts/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/artifacts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:07:20.009512 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/artifacts/vSAN/
+-rw-rw-rw-   0        0        0    28694 2023-02-28 20:06:20.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/artifacts/vSAN/Dashboards.zip
+-rw-rw-rw-   0        0        0    51491 2023-02-28 03:58:54.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/artifacts/vSAN/Notifications.json
+-rw-rw-rw-   0        0        0    16701 2023-02-28 03:10:32.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/artifacts/vSAN/Supermetrics.json
+-rw-rw-rw-   0        0        0    10147 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/artifacts/vSAN/Views.zip
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/artifacts/vSAN/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:07:20.009512 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/examples/__init__.py
+-rwxrwxrwx   0        0        0       55 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/examples/run_send-data-to-vrops.bat
+drwxrwxrwx   0        0        0        0 2023-05-23 23:07:20.025137 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/__init__.py
+-rw-rw-rw-   0        0        0     3199 2023-05-23 18:12:09.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/encrypt-passwords.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:07:20.025137 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/encrypted_files/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/encrypted_files/__init__.py
+-rw-rw-rw-   0        0        0     1456 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/env.json
+-rw-rw-rw-   0        0        0    70917 2023-05-23 18:12:09.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/send-data-to-vrops.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:07:20.025137 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/utils/
+-rw-rw-rw-   0        0        0     5862 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/utils/FolderUtility.py
+-rw-rw-rw-   0        0        0     4438 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/utils/LogUtility.py
+-rw-rw-rw-   0        0        0     3042 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/utils/PSUtility.py
+-rw-rw-rw-   0        0        0     7362 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/utils/SosRest.py
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:07:20.040761 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/vmware_cloud_foundation_health_monitoring.egg-info/
+-rw-rw-rw-   0        0        0    10980 2023-05-23 23:07:19.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/vmware_cloud_foundation_health_monitoring.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      915 2023-05-23 23:07:19.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/vmware_cloud_foundation_health_monitoring.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 23:07:19.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/vmware_cloud_foundation_health_monitoring.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-23 23:07:19.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/vmware_cloud_foundation_health_monitoring.egg-info/top_level.txt
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0/PKG-INFO` & `vmware-cloud-foundation-health-monitoring-1.1.0.1002/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmware-cloud-foundation-health-monitoring
-Version: 1.1.0
+Version: 1.1.0.1002
 Summary: Python Module for VMware Cloud Foundation Health Monitoring in vRealize Operations
 Home-page: https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
 Author: Bhumitra Nagar
 Author-email: bnagar@vmware.com
 License: BSD-2-Clause
 Project-URL: Bug Tracker, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues
 Project-URL: repository, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
@@ -61,15 +61,15 @@
 ### PowerShell Editions and Versions
 - PowerShell Core 7.2.0 or later
 - Microsoft Windows PowerShell 5.1
 
 
 ### PowerShell Modules
 
-- [PowerShell Module for VMware Cloud Foundation Reporting](https://github.com/vmware/powershell-module-for-vmware-cloud-foundation-reporting) 1.1.0
+- [PowerShell Module for VMware Cloud Foundation Reporting](https://github.com/vmware/powershell-module-for-vmware-cloud-foundation-reporting) 2.0.1
 
 
 
 ## Implementation 
 
 Follow the [Implementation of Health Reporting and Monitoring for VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation/services/vcf-health-reporting-and-monitoring-v1/GUID-AD58BAF1-7DC9-4514-90B7-7E9FA2E9E5FA.html) from [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation)
 
@@ -137,15 +137,15 @@
 ### 1. [Remove FQDN suffix dependency in the name when configuring an NSX-T cloud account in vRealize Operations](https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues/35)
 
 Please make sure that your NSX-T account name is configured as mentioned in this issue. 
 
 ### 2. The vCenter Server name needs to be updated in VMware Cloud Foundation 4.4.x. The filters on the vReaize Operations dashboards depend on the name.
 
 To set the Product Name for the vCenter Server, follow the below steps - 
-1. Log in to the management domain vCenter Server at `https://<management_vcenter_server_fqdn/ui` as `administrator@vsphere.local`.
+1. Log in to the management domain vCenter Server at `https://<management_vcenter_server_fqdn>/ui` as `administrator@vsphere.local`.
 2. In the `VMs and templates` inventory, expand the `management domain vCenter Server` tree and expand the management domain data center.
 3. Select the first `management domain vCenter Server virtual machine` and select `Configure` tab.
 4. In the `Settings` pane select `vApp Options`.
 5. Click the `Edit` button. The `Edit vApp Options` dialog box opens.
 6. If vApp options are disabled, select the `Enable vApp options` check box and click `OK`.
 7. Click the `Details` tab and enter `VMware vCenter Server Appliance` as product name in the `Name` field.
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0/README.md` & `vmware-cloud-foundation-health-monitoring-1.1.0.1002/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 ### PowerShell Editions and Versions
 - PowerShell Core 7.2.0 or later
 - Microsoft Windows PowerShell 5.1
 
 
 ### PowerShell Modules
 
-- [PowerShell Module for VMware Cloud Foundation Reporting](https://github.com/vmware/powershell-module-for-vmware-cloud-foundation-reporting) 1.1.0
+- [PowerShell Module for VMware Cloud Foundation Reporting](https://github.com/vmware/powershell-module-for-vmware-cloud-foundation-reporting) 2.0.1
 
 
 
 ## Implementation 
 
 Follow the [Implementation of Health Reporting and Monitoring for VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation/services/vcf-health-reporting-and-monitoring-v1/GUID-AD58BAF1-7DC9-4514-90B7-7E9FA2E9E5FA.html) from [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation)
 
@@ -121,15 +121,15 @@
 ### 1. [Remove FQDN suffix dependency in the name when configuring an NSX-T cloud account in vRealize Operations](https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues/35)
 
 Please make sure that your NSX-T account name is configured as mentioned in this issue. 
 
 ### 2. The vCenter Server name needs to be updated in VMware Cloud Foundation 4.4.x. The filters on the vReaize Operations dashboards depend on the name.
 
 To set the Product Name for the vCenter Server, follow the below steps - 
-1. Log in to the management domain vCenter Server at `https://<management_vcenter_server_fqdn/ui` as `administrator@vsphere.local`.
+1. Log in to the management domain vCenter Server at `https://<management_vcenter_server_fqdn>/ui` as `administrator@vsphere.local`.
 2. In the `VMs and templates` inventory, expand the `management domain vCenter Server` tree and expand the management domain data center.
 3. Select the first `management domain vCenter Server virtual machine` and select `Configure` tab.
 4. In the `Settings` pane select `vApp Options`.
 5. Click the `Edit` button. The `Edit vApp Options` dialog box opens.
 6. If vApp options are disabled, select the `Enable vApp options` check box and click `OK`.
 7. Click the `Details` tab and enter `VMware vCenter Server Appliance` as product name in the `Name` field.
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0/setup.cfg` & `vmware-cloud-foundation-health-monitoring-1.1.0.1002/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6d77 6172 652d 636c 6f75 642d   = vmware-cloud-
 00000020: 666f 756e 6461 7469 6f6e 2d68 6561 6c74  foundation-healt
 00000030: 682d 6d6f 6e69 746f 7269 6e67 0d0a 7665  h-monitoring..ve
-00000040: 7273 696f 6e20 3d20 312e 312e 300d 0a61  rsion = 1.1.0..a
-00000050: 7574 686f 7220 3d20 4268 756d 6974 7261  uthor = Bhumitra
-00000060: 204e 6167 6172 0d0a 6175 7468 6f72 5f65   Nagar..author_e
-00000070: 6d61 696c 203d 2062 6e61 6761 7240 766d  mail = bnagar@vm
-00000080: 7761 7265 2e63 6f6d 0d0a 6465 7363 7269  ware.com..descri
-00000090: 7074 696f 6e20 3d20 5079 7468 6f6e 204d  ption = Python M
-000000a0: 6f64 756c 6520 666f 7220 564d 7761 7265  odule for VMware
-000000b0: 2043 6c6f 7564 2046 6f75 6e64 6174 696f   Cloud Foundatio
-000000c0: 6e20 4865 616c 7468 204d 6f6e 6974 6f72  n Health Monitor
-000000d0: 696e 6720 696e 2076 5265 616c 697a 6520  ing in vRealize 
-000000e0: 4f70 6572 6174 696f 6e73 0d0a 6c6f 6e67  Operations..long
-000000f0: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
-00000100: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
-00000110: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-00000120: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
-00000130: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a6c  text/markdown..l
-00000140: 6963 656e 7365 203d 2042 5344 2d32 2d43  icense = BSD-2-C
-00000150: 6c61 7573 650d 0a75 726c 203d 2068 7474  lause..url = htt
-00000160: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000170: 766d 7761 7265 2d73 616d 706c 6573 2f76  vmware-samples/v
-00000180: 616c 6964 6174 6564 2d73 6f6c 7574 696f  alidated-solutio
-00000190: 6e73 2d66 6f72 2d63 6c6f 7564 2d66 6f75  ns-for-cloud-fou
-000001a0: 6e64 6174 696f 6e2f 7472 6565 2f6d 6169  ndation/tree/mai
-000001b0: 6e2f 6872 6d0d 0a70 726f 6a65 6374 5f75  n/hrm..project_u
-000001c0: 726c 7320 3d20 0d0a 0942 7567 2054 7261  rls = ...Bug Tra
-000001d0: 636b 6572 203d 2068 7474 7073 3a2f 2f67  cker = https://g
-000001e0: 6974 6875 622e 636f 6d2f 766d 7761 7265  ithub.com/vmware
-000001f0: 2d73 616d 706c 6573 2f76 616c 6964 6174  -samples/validat
-00000200: 6564 2d73 6f6c 7574 696f 6e73 2d66 6f72  ed-solutions-for
-00000210: 2d63 6c6f 7564 2d66 6f75 6e64 6174 696f  -cloud-foundatio
-00000220: 6e2f 6973 7375 6573 0d0a 0972 6570 6f73  n/issues...repos
-00000230: 6974 6f72 7920 3d20 6874 7470 733a 2f2f  itory = https://
-00000240: 6769 7468 7562 2e63 6f6d 2f76 6d77 6172  github.com/vmwar
-00000250: 652d 7361 6d70 6c65 732f 7661 6c69 6461  e-samples/valida
-00000260: 7465 642d 736f 6c75 7469 6f6e 732d 666f  ted-solutions-fo
-00000270: 722d 636c 6f75 642d 666f 756e 6461 7469  r-cloud-foundati
-00000280: 6f6e 2f74 7265 652f 6d61 696e 2f68 726d  on/tree/main/hrm
-00000290: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
-000002a0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-000002b0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000002c0: 6e20 3a3a 2033 0d0a 094c 6963 656e 7365  n :: 3...License
-000002d0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-000002e0: 203a 3a20 4253 4420 4c69 6365 6e73 650d   :: BSD License.
-000002f0: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
-00000300: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
-00000310: 6465 6e74 0d0a 0d0a 5b6f 7074 696f 6e73  dent....[options
-00000320: 5d0d 0a70 6163 6b61 6765 5f64 6972 203d  ]..package_dir =
-00000330: 200d 0a09 3d20 736f 7572 6365 0d0a 7061   ...= source..pa
-00000340: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
-00000350: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
-00000360: 3d20 3e3d 332e 360d 0a69 6e63 6c75 6465  = >=3.6..include
-00000370: 5f70 6163 6b61 6765 5f64 6174 6120 3d20  _package_data = 
-00000380: 5472 7565 0d0a 0d0a 5b6f 7074 696f 6e73  True....[options
-00000390: 2e70 6163 6b61 6765 5f64 6174 615d 0d0a  .package_data]..
-000003a0: 2a20 3d20 2a2e 6a73 6f6e 2c20 2a2e 6261  * = *.json, *.ba
-000003b0: 742c 202a 2e7a 6970 0d0a 0d0a 5b6f 7074  t, *.zip....[opt
-000003c0: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
-000003d0: 6e64 5d0d 0a77 6865 7265 203d 2073 6f75  nd]..where = sou
-000003e0: 7263 650d 0a0d 0a5b 6567 675f 696e 666f  rce....[egg_info
-000003f0: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-00000400: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-00000410: 0a                                       .
+00000040: 7273 696f 6e20 3d20 312e 312e 302e 3130  rsion = 1.1.0.10
+00000050: 3032 0d0a 6175 7468 6f72 203d 2042 6875  02..author = Bhu
+00000060: 6d69 7472 6120 4e61 6761 720d 0a61 7574  mitra Nagar..aut
+00000070: 686f 725f 656d 6169 6c20 3d20 626e 6167  hor_email = bnag
+00000080: 6172 4076 6d77 6172 652e 636f 6d0d 0a64  ar@vmware.com..d
+00000090: 6573 6372 6970 7469 6f6e 203d 2050 7974  escription = Pyt
+000000a0: 686f 6e20 4d6f 6475 6c65 2066 6f72 2056  hon Module for V
+000000b0: 4d77 6172 6520 436c 6f75 6420 466f 756e  Mware Cloud Foun
+000000c0: 6461 7469 6f6e 2048 6561 6c74 6820 4d6f  dation Health Mo
+000000d0: 6e69 746f 7269 6e67 2069 6e20 7652 6561  nitoring in vRea
+000000e0: 6c69 7a65 204f 7065 7261 7469 6f6e 730d  lize Operations.
+000000f0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+00000100: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
+00000110: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
+00000120: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
+00000130: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
+00000140: 776e 0d0a 6c69 6365 6e73 6520 3d20 4253  wn..license = BS
+00000150: 442d 322d 436c 6175 7365 0d0a 7572 6c20  D-2-Clause..url 
+00000160: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+00000170: 2e63 6f6d 2f76 6d77 6172 652d 7361 6d70  .com/vmware-samp
+00000180: 6c65 732f 7661 6c69 6461 7465 642d 736f  les/validated-so
+00000190: 6c75 7469 6f6e 732d 666f 722d 636c 6f75  lutions-for-clou
+000001a0: 642d 666f 756e 6461 7469 6f6e 2f74 7265  d-foundation/tre
+000001b0: 652f 6d61 696e 2f68 726d 0d0a 7072 6f6a  e/main/hrm..proj
+000001c0: 6563 745f 7572 6c73 203d 200d 0a09 4275  ect_urls = ...Bu
+000001d0: 6720 5472 6163 6b65 7220 3d20 6874 7470  g Tracker = http
+000001e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f76  s://github.com/v
+000001f0: 6d77 6172 652d 7361 6d70 6c65 732f 7661  mware-samples/va
+00000200: 6c69 6461 7465 642d 736f 6c75 7469 6f6e  lidated-solution
+00000210: 732d 666f 722d 636c 6f75 642d 666f 756e  s-for-cloud-foun
+00000220: 6461 7469 6f6e 2f69 7373 7565 730d 0a09  dation/issues...
+00000230: 7265 706f 7369 746f 7279 203d 2068 7474  repository = htt
+00000240: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000250: 766d 7761 7265 2d73 616d 706c 6573 2f76  vmware-samples/v
+00000260: 616c 6964 6174 6564 2d73 6f6c 7574 696f  alidated-solutio
+00000270: 6e73 2d66 6f72 2d63 6c6f 7564 2d66 6f75  ns-for-cloud-fou
+00000280: 6e64 6174 696f 6e2f 7472 6565 2f6d 6169  ndation/tree/mai
+00000290: 6e2f 6872 6d0d 0a63 6c61 7373 6966 6965  n/hrm..classifie
+000002a0: 7273 203d 200d 0a09 5072 6f67 7261 6d6d  rs = ...Programm
+000002b0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000002c0: 5079 7468 6f6e 203a 3a20 330d 0a09 4c69  Python :: 3...Li
+000002d0: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+000002e0: 726f 7665 6420 3a3a 2042 5344 204c 6963  roved :: BSD Lic
+000002f0: 656e 7365 0d0a 094f 7065 7261 7469 6e67  ense...Operating
+00000300: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
+00000310: 6465 7065 6e64 656e 740d 0a0d 0a5b 6f70  dependent....[op
+00000320: 7469 6f6e 735d 0d0a 7061 636b 6167 655f  tions]..package_
+00000330: 6469 7220 3d20 0d0a 093d 2073 6f75 7263  dir = ...= sourc
+00000340: 650d 0a70 6163 6b61 6765 7320 3d20 6669  e..packages = fi
+00000350: 6e64 3a0d 0a70 7974 686f 6e5f 7265 7175  nd:..python_requ
+00000360: 6972 6573 203d 203e 3d33 2e36 0d0a 696e  ires = >=3.6..in
+00000370: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
+00000380: 7461 203d 2054 7275 650d 0a0d 0a5b 6f70  ta = True....[op
+00000390: 7469 6f6e 732e 7061 636b 6167 655f 6461  tions.package_da
+000003a0: 7461 5d0d 0a2a 203d 202a 2e6a 736f 6e2c  ta]..* = *.json,
+000003b0: 202a 2e62 6174 2c20 2a2e 7a69 700d 0a0d   *.bat, *.zip...
+000003c0: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
+000003d0: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
+000003e0: 3d20 736f 7572 6365 0d0a 0d0a 5b65 6767  = source....[egg
+000003f0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+00000400: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+00000410: 2030 0d0a 0d0a                            0....
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0/source/artifacts/vSAN/Dashboards.zip` & `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/artifacts/vSAN/Dashboards.zip`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0/source/artifacts/vSAN/Notifications.json` & `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/artifacts/vSAN/Notifications.json`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0/source/artifacts/vSAN/Supermetrics.json` & `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/artifacts/vSAN/Supermetrics.json`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0/source/artifacts/vSAN/Views.zip` & `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/artifacts/vSAN/Views.zip`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0/source/main/encrypt-passwords.py` & `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/encrypt-passwords.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 # OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 # ===================================================================================================================
 # Created by:  Bhumitra Nagar - Senior Member of Technical Staff
 # Authors: Bhumitra Nagar
 # Date:   2023-04-01
-# Version: 1.1.0.1001
+# Version: 1.1.0.1002
 # ===================================================================================================================
 #
 # Description:
 # Script to encrypt passwords for SDDC Manager and vRealize Operations credentials. Passwords are encrypted and saved
 # in an encrypted_pwds file and a key file in encrypted_files directory.
 #
 # Example:
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0/source/main/env.json` & `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/env.json`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0/source/main/send-data-to-vrops.py` & `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/send-data-to-vrops.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 # OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 # ===================================================================================================================
 # Created by:  Bhumitra Nagar - Senior Member of Technical Staff
 # Authors: Bhumitra Nagar, Sowjanya V
 # Date:   2023-05-04
-# Version: 1.1.0.1001
+# Version: 1.1.0.1002
 # ===================================================================================================================
 #
 # Description:
 # The send-data-to-vrops.py script receives the operational health data as JSON from SOS utility and supporting
 # Powershell modules and then sends it to objects in vRealize Operations as custom metrics for use in dashboards
 # to monitor the platform's health.
 #
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0/source/main/utils/FolderUtility.py` & `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/utils/FolderUtility.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0/source/main/utils/LogUtility.py` & `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/utils/LogUtility.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0/source/main/utils/PSUtility.py` & `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/utils/PSUtility.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0/source/main/utils/SosRest.py` & `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/utils/SosRest.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0/source/vmware_cloud_foundation_health_monitoring.egg-info/PKG-INFO` & `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/vmware_cloud_foundation_health_monitoring.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmware-cloud-foundation-health-monitoring
-Version: 1.1.0
+Version: 1.1.0.1002
 Summary: Python Module for VMware Cloud Foundation Health Monitoring in vRealize Operations
 Home-page: https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
 Author: Bhumitra Nagar
 Author-email: bnagar@vmware.com
 License: BSD-2-Clause
 Project-URL: Bug Tracker, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues
 Project-URL: repository, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
@@ -61,15 +61,15 @@
 ### PowerShell Editions and Versions
 - PowerShell Core 7.2.0 or later
 - Microsoft Windows PowerShell 5.1
 
 
 ### PowerShell Modules
 
-- [PowerShell Module for VMware Cloud Foundation Reporting](https://github.com/vmware/powershell-module-for-vmware-cloud-foundation-reporting) 1.1.0
+- [PowerShell Module for VMware Cloud Foundation Reporting](https://github.com/vmware/powershell-module-for-vmware-cloud-foundation-reporting) 2.0.1
 
 
 
 ## Implementation 
 
 Follow the [Implementation of Health Reporting and Monitoring for VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation/services/vcf-health-reporting-and-monitoring-v1/GUID-AD58BAF1-7DC9-4514-90B7-7E9FA2E9E5FA.html) from [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation)
 
@@ -137,15 +137,15 @@
 ### 1. [Remove FQDN suffix dependency in the name when configuring an NSX-T cloud account in vRealize Operations](https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues/35)
 
 Please make sure that your NSX-T account name is configured as mentioned in this issue. 
 
 ### 2. The vCenter Server name needs to be updated in VMware Cloud Foundation 4.4.x. The filters on the vReaize Operations dashboards depend on the name.
 
 To set the Product Name for the vCenter Server, follow the below steps - 
-1. Log in to the management domain vCenter Server at `https://<management_vcenter_server_fqdn/ui` as `administrator@vsphere.local`.
+1. Log in to the management domain vCenter Server at `https://<management_vcenter_server_fqdn>/ui` as `administrator@vsphere.local`.
 2. In the `VMs and templates` inventory, expand the `management domain vCenter Server` tree and expand the management domain data center.
 3. Select the first `management domain vCenter Server virtual machine` and select `Configure` tab.
 4. In the `Settings` pane select `vApp Options`.
 5. Click the `Edit` button. The `Edit vApp Options` dialog box opens.
 6. If vApp options are disabled, select the `Enable vApp options` check box and click `OK`.
 7. Click the `Details` tab and enter `VMware vCenter Server Appliance` as product name in the `Name` field.
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0/source/vmware_cloud_foundation_health_monitoring.egg-info/SOURCES.txt` & `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/vmware_cloud_foundation_health_monitoring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

