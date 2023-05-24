# Comparing `tmp/pulumi_vsphere-4.5.0a1684391558.tar.gz` & `tmp/pulumi_vsphere-4.5.0a1684947541.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_vsphere-4.5.0a1684391558.tar", last modified: Thu May 18 06:40:05 2023, max compression
+gzip compressed data, was "pulumi_vsphere-4.5.0a1684947541.tar", last modified: Wed May 24 17:04:07 2023, max compression
```

## Comparing `pulumi_vsphere-4.5.0a1684391558.tar` & `pulumi_vsphere-4.5.0a1684947541.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:05.151285 pulumi_vsphere-4.5.0a1684391558/
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-18 06:40:05.151285 pulumi_vsphere-4.5.0a1684391558/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:05.147285 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/
--rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    81397 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)   231990 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/compute_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    11620 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/compute_cluster_host_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    22943 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/compute_cluster_vm_affinity_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    16038 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/compute_cluster_vm_anti_affinity_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/compute_cluster_vm_dependency_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/compute_cluster_vm_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    21803 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/compute_cluster_vm_host_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:05.147285 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    15087 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/content_library.py
--rw-r--r--   0 runner    (1001) docker     (123)    15640 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/content_library_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    15935 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    89388 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/datastore_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    16257 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/datastore_cluster_vm_anti_affinity_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)   129818 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/distributed_port_group.py
--rw-r--r--   0 runner    (1001) docker     (123)   257355 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/distributed_virtual_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/dpm_host_override.py
--rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/drs_vm_override.py
--rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/entity_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21472 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    20105 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_compute_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_compute_cluster_host_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_content_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_content_library_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_datastore_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_distributed_virtual_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_host.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_host_pci_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_host_thumbprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_license.py
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    31941 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_ovf_vm_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_resource_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_tag_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_vapp_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    54162 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_vmfs_disks.py
--rw-r--r--   0 runner    (1001) docker     (123)    58963 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/ha_vm_override.py
--rw-r--r--   0 runner    (1001) docker     (123)    43166 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/host.py
--rw-r--r--   0 runner    (1001) docker     (123)    56784 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/host_port_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    60596 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/host_virtual_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/license.py
--rw-r--r--   0 runner    (1001) docker     (123)    46325 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/nas_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    81214 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    54091 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/resource_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    20828 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/storage_drs_vm_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    13982 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/tag_category.py
--rw-r--r--   0 runner    (1001) docker     (123)    48255 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/vapp_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    29555 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/vapp_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    22447 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/virtual_disk.py
--rw-r--r--   0 runner    (1001) docker     (123)   245191 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)    23926 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/virtual_machine_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)    20958 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/vm_storage_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    32719 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/vmfs_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    27602 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/vnic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:05.147285 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-18 06:40:05.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-18 06:40:05.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:40:05.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:40:05.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-18 06:40:05.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-18 06:40:05.000000 pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 06:40:05.151285 pulumi_vsphere-4.5.0a1684391558/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-18 06:40:04.000000 pulumi_vsphere-4.5.0a1684391558/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:04:07.945200 pulumi_vsphere-4.5.0a1684947541/
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-05-24 17:04:07.945200 pulumi_vsphere-4.5.0a1684947541/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:04:07.941200 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/
+-rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87225 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)   237133 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/compute_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/compute_cluster_host_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24459 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/compute_cluster_vm_affinity_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17554 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/compute_cluster_vm_anti_affinity_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21613 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/compute_cluster_vm_dependency_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13459 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/compute_cluster_vm_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24422 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/compute_cluster_vm_host_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:04:07.941200 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15087 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/content_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15640 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/content_library_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91913 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/datastore_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16842 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/datastore_cluster_vm_anti_affinity_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134499 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/distributed_port_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)   263381 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/distributed_virtual_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15371 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/dpm_host_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16657 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/drs_vm_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/entity_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23387 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25630 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_compute_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_compute_cluster_host_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_content_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_content_library_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_datastore_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_distributed_virtual_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_host_pci_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_host_thumbprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32193 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_ovf_vm_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_resource_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_tag_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_vapp_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55448 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_vmfs_disks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58963 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/ha_vm_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45915 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56784 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/host_port_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61643 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/host_virtual_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48202 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/nas_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87056 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    54091 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/resource_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20828 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/storage_drs_vm_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15120 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/tag_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48255 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/vapp_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29555 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/vapp_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28150 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/virtual_disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)   270022 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23926 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/virtual_machine_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21418 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/vm_storage_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34596 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/vmfs_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28500 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/vnic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:04:07.941200 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 17:04:07.945200 pulumi_vsphere-4.5.0a1684947541/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-05-24 17:04:07.000000 pulumi_vsphere-4.5.0a1684947541/setup.py
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/PKG-INFO` & `pulumi_vsphere-4.5.0a1684947541/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi_vsphere
-Version: 4.5.0a1684391558
+Version: 4.5.0a1684947541
 Summary: A Pulumi package for creating vsphere resources
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-vsphere
 Keywords: pulumi vsphere
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-vsphere/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-vsphere/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fvsphere.svg)](https://www.npmjs.com/package/@pulumi/vsphere)
 [![Python version](https://badge.fury.io/py/pulumi-vsphere.svg)](https://pypi.org/project/pulumi-vsphere)
 [![NuGet version](https://badge.fury.io/nu/pulumi.vsphere.svg)](https://badge.fury.io/nu/pulumi.vsphere)
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/README.md` & `pulumi_vsphere-4.5.0a1684947541/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/__init__.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/_inputs.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/_inputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,42 @@
 class ComputeClusterVsanDiskGroupArgs:
     def __init__(__self__, *,
                  cache: Optional[pulumi.Input[str]] = None,
                  storages: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] cache: The canonical name of the disk to use for vSAN cache.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] storages: An array of disk canonical names for vSAN storage.
+               
+               > **NOTE:** You must disable vSphere HA before you enable vSAN on the cluster.
+               You can enable or re-enable vSphere HA after vSAN is configured.
+               
+               ```python
+               import pulumi
+               import pulumi_vsphere as vsphere
+               
+               compute_cluster = vsphere.ComputeCluster("computeCluster",
+                   datacenter_id=data["vsphere_datacenter"]["datacenter"]["id"],
+                   host_system_ids=[[__item["id"] for __item in data["vsphere_host"]["host"]]],
+                   drs_enabled=True,
+                   drs_automation_level="fullyAutomated",
+                   ha_enabled=False,
+                   vsan_enabled=True,
+                   vsan_dedup_enabled=True,
+                   vsan_compression_enabled=True,
+                   vsan_performance_enabled=True,
+                   vsan_verbose_mode_enabled=True,
+                   vsan_network_diagnostic_mode_enabled=True,
+                   vsan_unmap_enabled=True,
+                   vsan_dit_encryption_enabled=True,
+                   vsan_dit_rekey_interval=1800,
+                   vsan_disk_groups=[vsphere.ComputeClusterVsanDiskGroupArgs(
+                       cache=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                       storages=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                   )])
+               ```
         """
         if cache is not None:
             pulumi.set(__self__, "cache", cache)
         if storages is not None:
             pulumi.set(__self__, "storages", storages)
 
     @property
@@ -62,14 +90,42 @@
         pulumi.set(self, "cache", value)
 
     @property
     @pulumi.getter
     def storages(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         An array of disk canonical names for vSAN storage.
+
+        > **NOTE:** You must disable vSphere HA before you enable vSAN on the cluster.
+        You can enable or re-enable vSphere HA after vSAN is configured.
+
+        ```python
+        import pulumi
+        import pulumi_vsphere as vsphere
+
+        compute_cluster = vsphere.ComputeCluster("computeCluster",
+            datacenter_id=data["vsphere_datacenter"]["datacenter"]["id"],
+            host_system_ids=[[__item["id"] for __item in data["vsphere_host"]["host"]]],
+            drs_enabled=True,
+            drs_automation_level="fullyAutomated",
+            ha_enabled=False,
+            vsan_enabled=True,
+            vsan_dedup_enabled=True,
+            vsan_compression_enabled=True,
+            vsan_performance_enabled=True,
+            vsan_verbose_mode_enabled=True,
+            vsan_network_diagnostic_mode_enabled=True,
+            vsan_unmap_enabled=True,
+            vsan_dit_encryption_enabled=True,
+            vsan_dit_rekey_interval=1800,
+            vsan_disk_groups=[vsphere.ComputeClusterVsanDiskGroupArgs(
+                cache=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                storages=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+            )])
+        ```
         """
         return pulumi.get(self, "storages")
 
     @storages.setter
     def storages(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "storages", value)
 
@@ -539,16 +595,22 @@
                  datastore_id: Optional[pulumi.Input[str]] = None,
                  device_address: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[int]] = None,
                  path: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[bool] client_device: Indicates whether the device should be backed by remote client device. Conflicts with `datastore_id` and `path`.
         :param pulumi.Input[str] datastore_id: The managed object reference ID of the datastore in which to place the virtual machine. The virtual machine configuration files is placed here, along with any virtual disks that are created where a datastore is not explicitly specified. See the section on virtual machine migration for more information on modifying this value.
+               
+               > **NOTE:** Datastores cannot be assigned to individual disks when `datastore_cluster_id` is used.
         :param pulumi.Input[int] key: The ID of the device within the virtual machine.
         :param pulumi.Input[str] path: When using `attach`, this parameter controls the path of a virtual disk to attach externally. Otherwise, it is a computed attribute that contains the virtual disk filename.
+               
+               > **NOTE:** Either `client_device` (for a remote backed CD-ROM) or `datastore_id` and `path` (for a datastore ISO backed CD-ROM) are required to .
+               
+               > **NOTE:** Some CD-ROM drive types are not supported by this resource, such as pass-through devices. If these drives are present in a cloned template, or added outside of the provider, the desired state will be corrected to the defined device, or removed if no `cdrom` block is present.
         """
         if client_device is not None:
             pulumi.set(__self__, "client_device", client_device)
         if datastore_id is not None:
             pulumi.set(__self__, "datastore_id", datastore_id)
         if device_address is not None:
             pulumi.set(__self__, "device_address", device_address)
@@ -570,14 +632,16 @@
         pulumi.set(self, "client_device", value)
 
     @property
     @pulumi.getter(name="datastoreId")
     def datastore_id(self) -> Optional[pulumi.Input[str]]:
         """
         The managed object reference ID of the datastore in which to place the virtual machine. The virtual machine configuration files is placed here, along with any virtual disks that are created where a datastore is not explicitly specified. See the section on virtual machine migration for more information on modifying this value.
+
+        > **NOTE:** Datastores cannot be assigned to individual disks when `datastore_cluster_id` is used.
         """
         return pulumi.get(self, "datastore_id")
 
     @datastore_id.setter
     def datastore_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "datastore_id", value)
 
@@ -603,14 +667,18 @@
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def path(self) -> Optional[pulumi.Input[str]]:
         """
         When using `attach`, this parameter controls the path of a virtual disk to attach externally. Otherwise, it is a computed attribute that contains the virtual disk filename.
+
+        > **NOTE:** Either `client_device` (for a remote backed CD-ROM) or `datastore_id` and `path` (for a datastore ISO backed CD-ROM) are required to .
+
+        > **NOTE:** Some CD-ROM drive types are not supported by this resource, such as pass-through devices. If these drives are present in a cloned template, or added outside of the provider, the desired state will be corrected to the defined device, or removed if no `cdrom` block is present.
         """
         return pulumi.get(self, "path")
 
     @path.setter
     def path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "path", value)
 
@@ -1131,28 +1199,39 @@
                  size: Optional[pulumi.Input[int]] = None,
                  storage_policy_id: Optional[pulumi.Input[str]] = None,
                  thin_provisioned: Optional[pulumi.Input[bool]] = None,
                  unit_number: Optional[pulumi.Input[int]] = None,
                  uuid: Optional[pulumi.Input[str]] = None,
                  write_through: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[str] label: A label for the virtual disk. Forces a new disk, if changed.
         :param pulumi.Input[bool] attach: Attach an external disk instead of creating a new one. Implies and conflicts with `keep_on_remove`. If set, you cannot set `size`, `eagerly_scrub`, or `thin_provisioned`. Must set `path` if used.
+               
+               > **NOTE:** External disks cannot be attached when `datastore_cluster_id` is used.
         :param pulumi.Input[str] controller_type: The type of storage controller to attach the  disk to. Can be `scsi`, `sata`, or `ide`. You must have the appropriate number of controllers enabled for the selected type. Default `scsi`.
         :param pulumi.Input[str] datastore_id: The managed object reference ID of the datastore in which to place the virtual machine. The virtual machine configuration files is placed here, along with any virtual disks that are created where a datastore is not explicitly specified. See the section on virtual machine migration for more information on modifying this value.
+               
+               > **NOTE:** Datastores cannot be assigned to individual disks when `datastore_cluster_id` is used.
         :param pulumi.Input[str] disk_mode: The mode of this this virtual disk for purposes of writes and snapshots. One of `append`, `independent_nonpersistent`, `independent_persistent`, `nonpersistent`, `persistent`, or `undoable`. Default: `persistent`. For more information on these option, please refer to the [product documentation][vmware-docs-disk-mode].
+               
+               [vmware-docs-disk-mode]: https://vdc-download.vmware.com/vmwb-repository/dcr-public/da47f910-60ac-438b-8b9b-6122f4d14524/16b7274a-bf8b-4b4c-a05e-746f2aa93c8c/doc/vim.vm.device.VirtualDiskOption.DiskMode.html
         :param pulumi.Input[str] disk_sharing: The sharing mode of this virtual disk. One of `sharingMultiWriter` or `sharingNone`. Default: `sharingNone`.
+               
+               > **NOTE:** Disk sharing is only available on vSphere 6.0 and later.
         :param pulumi.Input[bool] eagerly_scrub: If set to `true`, the disk space is zeroed out when the virtual machine is created. This will delay the creation of the virtual disk. Cannot be set to `true` when `thin_provisioned` is `true`.  See the section on picking a disk type for more information.  Default: `false`.
         :param pulumi.Input[int] io_limit: The upper limit of IOPS that this disk can use. The default is no limit.
         :param pulumi.Input[int] io_reservation: The I/O reservation (guarantee) for the virtual disk has, in IOPS.  The default is no reservation.
         :param pulumi.Input[int] io_share_count: The share count for the virtual disk when the share level is `custom`.
         :param pulumi.Input[str] io_share_level: The share allocation level for the virtual disk. One of `low`, `normal`, `high`, or `custom`. Default: `normal`.
         :param pulumi.Input[bool] keep_on_remove: Keep this disk when removing the device or destroying the virtual machine. Default: `false`.
         :param pulumi.Input[int] key: The ID of the device within the virtual machine.
         :param pulumi.Input[str] path: When using `attach`, this parameter controls the path of a virtual disk to attach externally. Otherwise, it is a computed attribute that contains the virtual disk filename.
+               
+               > **NOTE:** Either `client_device` (for a remote backed CD-ROM) or `datastore_id` and `path` (for a datastore ISO backed CD-ROM) are required to .
+               
+               > **NOTE:** Some CD-ROM drive types are not supported by this resource, such as pass-through devices. If these drives are present in a cloned template, or added outside of the provider, the desired state will be corrected to the defined device, or removed if no `cdrom` block is present.
         :param pulumi.Input[int] size: The size of the disk, in GB. Must be a whole number.
         :param pulumi.Input[str] storage_policy_id: The ID of the storage policy to assign to the home directory of a virtual machine.
         :param pulumi.Input[bool] thin_provisioned: If `true`, the disk is thin provisioned, with space for the file being allocated on an as-needed basis. Cannot be set to `true` when `eagerly_scrub` is `true`. See the section on selecting a disk type for more information. Default: `true`.
         :param pulumi.Input[int] unit_number: The disk number on the storage bus. The maximum value for this setting is the value of the controller count times the controller capacity (15 for SCSI, 30 for SATA, and 2 for IDE). Duplicate unit numbers are not allowed. Default `0`, for which one disk must be set to.
         :param pulumi.Input[str] uuid: The UUID of the virtual disk VMDK file. This is used to track the virtual disk on the virtual machine.
         :param pulumi.Input[bool] write_through: If `true`, writes for this disk are sent directly to the filesystem immediately instead of being buffered. Default: `false`.
         """
@@ -1197,28 +1276,27 @@
             pulumi.set(__self__, "uuid", uuid)
         if write_through is not None:
             pulumi.set(__self__, "write_through", write_through)
 
     @property
     @pulumi.getter
     def label(self) -> pulumi.Input[str]:
-        """
-        A label for the virtual disk. Forces a new disk, if changed.
-        """
         return pulumi.get(self, "label")
 
     @label.setter
     def label(self, value: pulumi.Input[str]):
         pulumi.set(self, "label", value)
 
     @property
     @pulumi.getter
     def attach(self) -> Optional[pulumi.Input[bool]]:
         """
         Attach an external disk instead of creating a new one. Implies and conflicts with `keep_on_remove`. If set, you cannot set `size`, `eagerly_scrub`, or `thin_provisioned`. Must set `path` if used.
+
+        > **NOTE:** External disks cannot be attached when `datastore_cluster_id` is used.
         """
         return pulumi.get(self, "attach")
 
     @attach.setter
     def attach(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "attach", value)
 
@@ -1235,14 +1313,16 @@
         pulumi.set(self, "controller_type", value)
 
     @property
     @pulumi.getter(name="datastoreId")
     def datastore_id(self) -> Optional[pulumi.Input[str]]:
         """
         The managed object reference ID of the datastore in which to place the virtual machine. The virtual machine configuration files is placed here, along with any virtual disks that are created where a datastore is not explicitly specified. See the section on virtual machine migration for more information on modifying this value.
+
+        > **NOTE:** Datastores cannot be assigned to individual disks when `datastore_cluster_id` is used.
         """
         return pulumi.get(self, "datastore_id")
 
     @datastore_id.setter
     def datastore_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "datastore_id", value)
 
@@ -1256,26 +1336,30 @@
         pulumi.set(self, "device_address", value)
 
     @property
     @pulumi.getter(name="diskMode")
     def disk_mode(self) -> Optional[pulumi.Input[str]]:
         """
         The mode of this this virtual disk for purposes of writes and snapshots. One of `append`, `independent_nonpersistent`, `independent_persistent`, `nonpersistent`, `persistent`, or `undoable`. Default: `persistent`. For more information on these option, please refer to the [product documentation][vmware-docs-disk-mode].
+
+        [vmware-docs-disk-mode]: https://vdc-download.vmware.com/vmwb-repository/dcr-public/da47f910-60ac-438b-8b9b-6122f4d14524/16b7274a-bf8b-4b4c-a05e-746f2aa93c8c/doc/vim.vm.device.VirtualDiskOption.DiskMode.html
         """
         return pulumi.get(self, "disk_mode")
 
     @disk_mode.setter
     def disk_mode(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "disk_mode", value)
 
     @property
     @pulumi.getter(name="diskSharing")
     def disk_sharing(self) -> Optional[pulumi.Input[str]]:
         """
         The sharing mode of this virtual disk. One of `sharingMultiWriter` or `sharingNone`. Default: `sharingNone`.
+
+        > **NOTE:** Disk sharing is only available on vSphere 6.0 and later.
         """
         return pulumi.get(self, "disk_sharing")
 
     @disk_sharing.setter
     def disk_sharing(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "disk_sharing", value)
 
@@ -1364,14 +1448,18 @@
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def path(self) -> Optional[pulumi.Input[str]]:
         """
         When using `attach`, this parameter controls the path of a virtual disk to attach externally. Otherwise, it is a computed attribute that contains the virtual disk filename.
+
+        > **NOTE:** Either `client_device` (for a remote backed CD-ROM) or `datastore_id` and `path` (for a datastore ISO backed CD-ROM) are required to .
+
+        > **NOTE:** Some CD-ROM drive types are not supported by this resource, such as pass-through devices. If these drives are present in a cloned template, or added outside of the provider, the desired state will be corrected to the defined device, or removed if no `cdrom` block is present.
         """
         return pulumi.get(self, "path")
 
     @path.setter
     def path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "path", value)
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/_utilities.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/compute_cluster.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/compute_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,17 @@
                  vsan_verbose_mode_enabled: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a ComputeCluster resource.
         :param pulumi.Input[str] datacenter_id: The managed object ID of
                the datacenter to create the cluster in. Forces a new resource if changed.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: A map of custom attribute ids to attribute
                value strings to set for the datastore cluster.
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+               and require vCenter Server.
         :param pulumi.Input[str] dpm_automation_level: The automation level for host power
                operations in this cluster. Can be one of `manual` or `automated`. Default:
                `manual`.
         :param pulumi.Input[bool] dpm_enabled: Enable DPM support for DRS in this cluster.
                Requires `drs_enabled` to be `true` in order to be effective.
                Default: `false`.
         :param pulumi.Input[int] dpm_threshold: A value between `1` and `5` indicating the
@@ -101,14 +104,16 @@
                options for DRS and DPM.
         :param pulumi.Input[str] drs_automation_level: The default automation level for all
                virtual machines in this cluster. Can be one of `manual`,
                `partiallyAutomated`, or `fullyAutomated`. Default: `manual`.
         :param pulumi.Input[bool] drs_enable_predictive_drs: When `true`, enables DRS to use data
                from [vRealize Operations Manager][ref-vsphere-vrops] to make proactive DRS
                recommendations. <sup>\\*</sup>
+               
+               [ref-vsphere-vrops]: https://docs.vmware.com/en/vRealize-Operations-Manager/index.html
         :param pulumi.Input[bool] drs_enable_vm_overrides: Allow individual DRS overrides to be
                set for virtual machines in the cluster. Default: `true`.
         :param pulumi.Input[bool] drs_enabled: Enable DRS for this cluster. Default: `false`.
         :param pulumi.Input[int] drs_migration_threshold: A value between `1` and `5` indicating
                the threshold of imbalance tolerated between hosts. A lower setting will
                tolerate more imbalance while a higher setting will tolerate less. Default:
                `3`.
@@ -122,14 +127,21 @@
                host folder located at `/dc1/host/foo/bar`, with the final inventory path
                being `/dc1/host/foo/bar/datastore-cluster-test`.
         :param pulumi.Input[bool] force_evacuate_on_destroy: When destroying the resource, setting this to
                `true` will auto-remove any hosts that are currently a member of the cluster,
                as if they were removed by taking their entry out of `host_system_ids` (see
                below. This is an advanced
                option and should only be used for testing. Default: `false`.
+               
+               > **NOTE:** Do not set `force_evacuate_on_destroy` in production operation as
+               there are many pitfalls to its use when working with complex cluster
+               configurations. Depending on the virtual machines currently on the cluster, and
+               your DRS and HA settings, the full host evacuation may fail. Instead,
+               incrementally remove hosts from your configuration by adjusting the contents of
+               the `host_system_ids` attribute.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ha_admission_control_failover_host_system_ids: Defines the
                managed object IDs of hosts to use as dedicated failover
                hosts. These hosts are kept as available as possible - admission control will
                block access to the host, and DRS will ignore the host when making
                recommendations.
         :param pulumi.Input[int] ha_admission_control_host_failure_tolerance: The maximum number
                of failed hosts that admission control tolerates when making decisions on
@@ -439,14 +451,17 @@
 
     @property
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         A map of custom attribute ids to attribute
         value strings to set for the datastore cluster.
+
+        > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+        and require vCenter Server.
         """
         return pulumi.get(self, "custom_attributes")
 
     @custom_attributes.setter
     def custom_attributes(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "custom_attributes", value)
 
@@ -523,14 +538,16 @@
     @property
     @pulumi.getter(name="drsEnablePredictiveDrs")
     def drs_enable_predictive_drs(self) -> Optional[pulumi.Input[bool]]:
         """
         When `true`, enables DRS to use data
         from [vRealize Operations Manager][ref-vsphere-vrops] to make proactive DRS
         recommendations. <sup>\\*</sup>
+
+        [ref-vsphere-vrops]: https://docs.vmware.com/en/vRealize-Operations-Manager/index.html
         """
         return pulumi.get(self, "drs_enable_predictive_drs")
 
     @drs_enable_predictive_drs.setter
     def drs_enable_predictive_drs(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "drs_enable_predictive_drs", value)
 
@@ -610,14 +627,21 @@
     def force_evacuate_on_destroy(self) -> Optional[pulumi.Input[bool]]:
         """
         When destroying the resource, setting this to
         `true` will auto-remove any hosts that are currently a member of the cluster,
         as if they were removed by taking their entry out of `host_system_ids` (see
         below. This is an advanced
         option and should only be used for testing. Default: `false`.
+
+        > **NOTE:** Do not set `force_evacuate_on_destroy` in production operation as
+        there are many pitfalls to its use when working with complex cluster
+        configurations. Depending on the virtual machines currently on the cluster, and
+        your DRS and HA settings, the full host evacuation may fail. Instead,
+        incrementally remove hosts from your configuration by adjusting the contents of
+        the `host_system_ids` attribute.
         """
         return pulumi.get(self, "force_evacuate_on_destroy")
 
     @force_evacuate_on_destroy.setter
     def force_evacuate_on_destroy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "force_evacuate_on_destroy", value)
 
@@ -1419,14 +1443,17 @@
                  vsan_remote_datastore_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  vsan_unmap_enabled: Optional[pulumi.Input[bool]] = None,
                  vsan_verbose_mode_enabled: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering ComputeCluster resources.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: A map of custom attribute ids to attribute
                value strings to set for the datastore cluster.
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+               and require vCenter Server.
         :param pulumi.Input[str] datacenter_id: The managed object ID of
                the datacenter to create the cluster in. Forces a new resource if changed.
         :param pulumi.Input[str] dpm_automation_level: The automation level for host power
                operations in this cluster. Can be one of `manual` or `automated`. Default:
                `manual`.
         :param pulumi.Input[bool] dpm_enabled: Enable DPM support for DRS in this cluster.
                Requires `drs_enabled` to be `true` in order to be effective.
@@ -1439,14 +1466,16 @@
                options for DRS and DPM.
         :param pulumi.Input[str] drs_automation_level: The default automation level for all
                virtual machines in this cluster. Can be one of `manual`,
                `partiallyAutomated`, or `fullyAutomated`. Default: `manual`.
         :param pulumi.Input[bool] drs_enable_predictive_drs: When `true`, enables DRS to use data
                from [vRealize Operations Manager][ref-vsphere-vrops] to make proactive DRS
                recommendations. <sup>\\*</sup>
+               
+               [ref-vsphere-vrops]: https://docs.vmware.com/en/vRealize-Operations-Manager/index.html
         :param pulumi.Input[bool] drs_enable_vm_overrides: Allow individual DRS overrides to be
                set for virtual machines in the cluster. Default: `true`.
         :param pulumi.Input[bool] drs_enabled: Enable DRS for this cluster. Default: `false`.
         :param pulumi.Input[int] drs_migration_threshold: A value between `1` and `5` indicating
                the threshold of imbalance tolerated between hosts. A lower setting will
                tolerate more imbalance while a higher setting will tolerate less. Default:
                `3`.
@@ -1460,14 +1489,21 @@
                host folder located at `/dc1/host/foo/bar`, with the final inventory path
                being `/dc1/host/foo/bar/datastore-cluster-test`.
         :param pulumi.Input[bool] force_evacuate_on_destroy: When destroying the resource, setting this to
                `true` will auto-remove any hosts that are currently a member of the cluster,
                as if they were removed by taking their entry out of `host_system_ids` (see
                below. This is an advanced
                option and should only be used for testing. Default: `false`.
+               
+               > **NOTE:** Do not set `force_evacuate_on_destroy` in production operation as
+               there are many pitfalls to its use when working with complex cluster
+               configurations. Depending on the virtual machines currently on the cluster, and
+               your DRS and HA settings, the full host evacuation may fail. Instead,
+               incrementally remove hosts from your configuration by adjusting the contents of
+               the `host_system_ids` attribute.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ha_admission_control_failover_host_system_ids: Defines the
                managed object IDs of hosts to use as dedicated failover
                hosts. These hosts are kept as available as possible - admission control will
                block access to the host, and DRS will ignore the host when making
                recommendations.
         :param pulumi.Input[int] ha_admission_control_host_failure_tolerance: The maximum number
                of failed hosts that admission control tolerates when making decisions on
@@ -1772,14 +1808,17 @@
 
     @property
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         A map of custom attribute ids to attribute
         value strings to set for the datastore cluster.
+
+        > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+        and require vCenter Server.
         """
         return pulumi.get(self, "custom_attributes")
 
     @custom_attributes.setter
     def custom_attributes(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "custom_attributes", value)
 
@@ -1869,14 +1908,16 @@
     @property
     @pulumi.getter(name="drsEnablePredictiveDrs")
     def drs_enable_predictive_drs(self) -> Optional[pulumi.Input[bool]]:
         """
         When `true`, enables DRS to use data
         from [vRealize Operations Manager][ref-vsphere-vrops] to make proactive DRS
         recommendations. <sup>\\*</sup>
+
+        [ref-vsphere-vrops]: https://docs.vmware.com/en/vRealize-Operations-Manager/index.html
         """
         return pulumi.get(self, "drs_enable_predictive_drs")
 
     @drs_enable_predictive_drs.setter
     def drs_enable_predictive_drs(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "drs_enable_predictive_drs", value)
 
@@ -1956,14 +1997,21 @@
     def force_evacuate_on_destroy(self) -> Optional[pulumi.Input[bool]]:
         """
         When destroying the resource, setting this to
         `true` will auto-remove any hosts that are currently a member of the cluster,
         as if they were removed by taking their entry out of `host_system_ids` (see
         below. This is an advanced
         option and should only be used for testing. Default: `false`.
+
+        > **NOTE:** Do not set `force_evacuate_on_destroy` in production operation as
+        there are many pitfalls to its use when working with complex cluster
+        configurations. Depending on the virtual machines currently on the cluster, and
+        your DRS and HA settings, the full host evacuation may fail. Instead,
+        incrementally remove hosts from your configuration by adjusting the contents of
+        the `host_system_ids` attribute.
         """
         return pulumi.get(self, "force_evacuate_on_destroy")
 
     @force_evacuate_on_destroy.setter
     def force_evacuate_on_destroy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "force_evacuate_on_destroy", value)
 
@@ -2785,14 +2833,17 @@
                  __props__=None):
         """
         Create a ComputeCluster resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: A map of custom attribute ids to attribute
                value strings to set for the datastore cluster.
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+               and require vCenter Server.
         :param pulumi.Input[str] datacenter_id: The managed object ID of
                the datacenter to create the cluster in. Forces a new resource if changed.
         :param pulumi.Input[str] dpm_automation_level: The automation level for host power
                operations in this cluster. Can be one of `manual` or `automated`. Default:
                `manual`.
         :param pulumi.Input[bool] dpm_enabled: Enable DPM support for DRS in this cluster.
                Requires `drs_enabled` to be `true` in order to be effective.
@@ -2805,14 +2856,16 @@
                options for DRS and DPM.
         :param pulumi.Input[str] drs_automation_level: The default automation level for all
                virtual machines in this cluster. Can be one of `manual`,
                `partiallyAutomated`, or `fullyAutomated`. Default: `manual`.
         :param pulumi.Input[bool] drs_enable_predictive_drs: When `true`, enables DRS to use data
                from [vRealize Operations Manager][ref-vsphere-vrops] to make proactive DRS
                recommendations. <sup>\\*</sup>
+               
+               [ref-vsphere-vrops]: https://docs.vmware.com/en/vRealize-Operations-Manager/index.html
         :param pulumi.Input[bool] drs_enable_vm_overrides: Allow individual DRS overrides to be
                set for virtual machines in the cluster. Default: `true`.
         :param pulumi.Input[bool] drs_enabled: Enable DRS for this cluster. Default: `false`.
         :param pulumi.Input[int] drs_migration_threshold: A value between `1` and `5` indicating
                the threshold of imbalance tolerated between hosts. A lower setting will
                tolerate more imbalance while a higher setting will tolerate less. Default:
                `3`.
@@ -2826,14 +2879,21 @@
                host folder located at `/dc1/host/foo/bar`, with the final inventory path
                being `/dc1/host/foo/bar/datastore-cluster-test`.
         :param pulumi.Input[bool] force_evacuate_on_destroy: When destroying the resource, setting this to
                `true` will auto-remove any hosts that are currently a member of the cluster,
                as if they were removed by taking their entry out of `host_system_ids` (see
                below. This is an advanced
                option and should only be used for testing. Default: `false`.
+               
+               > **NOTE:** Do not set `force_evacuate_on_destroy` in production operation as
+               there are many pitfalls to its use when working with complex cluster
+               configurations. Depending on the virtual machines currently on the cluster, and
+               your DRS and HA settings, the full host evacuation may fail. Instead,
+               incrementally remove hosts from your configuration by adjusting the contents of
+               the `host_system_ids` attribute.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ha_admission_control_failover_host_system_ids: Defines the
                managed object IDs of hosts to use as dedicated failover
                hosts. These hosts are kept as available as possible - admission control will
                block access to the host, and DRS will ignore the host when making
                recommendations.
         :param pulumi.Input[int] ha_admission_control_host_failure_tolerance: The maximum number
                of failed hosts that admission control tolerates when making decisions on
@@ -3244,14 +3304,17 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: A map of custom attribute ids to attribute
                value strings to set for the datastore cluster.
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+               and require vCenter Server.
         :param pulumi.Input[str] datacenter_id: The managed object ID of
                the datacenter to create the cluster in. Forces a new resource if changed.
         :param pulumi.Input[str] dpm_automation_level: The automation level for host power
                operations in this cluster. Can be one of `manual` or `automated`. Default:
                `manual`.
         :param pulumi.Input[bool] dpm_enabled: Enable DPM support for DRS in this cluster.
                Requires `drs_enabled` to be `true` in order to be effective.
@@ -3264,14 +3327,16 @@
                options for DRS and DPM.
         :param pulumi.Input[str] drs_automation_level: The default automation level for all
                virtual machines in this cluster. Can be one of `manual`,
                `partiallyAutomated`, or `fullyAutomated`. Default: `manual`.
         :param pulumi.Input[bool] drs_enable_predictive_drs: When `true`, enables DRS to use data
                from [vRealize Operations Manager][ref-vsphere-vrops] to make proactive DRS
                recommendations. <sup>\\*</sup>
+               
+               [ref-vsphere-vrops]: https://docs.vmware.com/en/vRealize-Operations-Manager/index.html
         :param pulumi.Input[bool] drs_enable_vm_overrides: Allow individual DRS overrides to be
                set for virtual machines in the cluster. Default: `true`.
         :param pulumi.Input[bool] drs_enabled: Enable DRS for this cluster. Default: `false`.
         :param pulumi.Input[int] drs_migration_threshold: A value between `1` and `5` indicating
                the threshold of imbalance tolerated between hosts. A lower setting will
                tolerate more imbalance while a higher setting will tolerate less. Default:
                `3`.
@@ -3285,14 +3350,21 @@
                host folder located at `/dc1/host/foo/bar`, with the final inventory path
                being `/dc1/host/foo/bar/datastore-cluster-test`.
         :param pulumi.Input[bool] force_evacuate_on_destroy: When destroying the resource, setting this to
                `true` will auto-remove any hosts that are currently a member of the cluster,
                as if they were removed by taking their entry out of `host_system_ids` (see
                below. This is an advanced
                option and should only be used for testing. Default: `false`.
+               
+               > **NOTE:** Do not set `force_evacuate_on_destroy` in production operation as
+               there are many pitfalls to its use when working with complex cluster
+               configurations. Depending on the virtual machines currently on the cluster, and
+               your DRS and HA settings, the full host evacuation may fail. Instead,
+               incrementally remove hosts from your configuration by adjusting the contents of
+               the `host_system_ids` attribute.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ha_admission_control_failover_host_system_ids: Defines the
                managed object IDs of hosts to use as dedicated failover
                hosts. These hosts are kept as available as possible - admission control will
                block access to the host, and DRS will ignore the host when making
                recommendations.
         :param pulumi.Input[int] ha_admission_control_host_failure_tolerance: The maximum number
                of failed hosts that admission control tolerates when making decisions on
@@ -3536,14 +3608,17 @@
 
     @property
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
         A map of custom attribute ids to attribute
         value strings to set for the datastore cluster.
+
+        > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+        and require vCenter Server.
         """
         return pulumi.get(self, "custom_attributes")
 
     @property
     @pulumi.getter(name="datacenterId")
     def datacenter_id(self) -> pulumi.Output[str]:
         """
@@ -3605,14 +3680,16 @@
     @property
     @pulumi.getter(name="drsEnablePredictiveDrs")
     def drs_enable_predictive_drs(self) -> pulumi.Output[Optional[bool]]:
         """
         When `true`, enables DRS to use data
         from [vRealize Operations Manager][ref-vsphere-vrops] to make proactive DRS
         recommendations. <sup>\\*</sup>
+
+        [ref-vsphere-vrops]: https://docs.vmware.com/en/vRealize-Operations-Manager/index.html
         """
         return pulumi.get(self, "drs_enable_predictive_drs")
 
     @property
     @pulumi.getter(name="drsEnableVmOverrides")
     def drs_enable_vm_overrides(self) -> pulumi.Output[Optional[bool]]:
         """
@@ -3668,14 +3745,21 @@
     def force_evacuate_on_destroy(self) -> pulumi.Output[Optional[bool]]:
         """
         When destroying the resource, setting this to
         `true` will auto-remove any hosts that are currently a member of the cluster,
         as if they were removed by taking their entry out of `host_system_ids` (see
         below. This is an advanced
         option and should only be used for testing. Default: `false`.
+
+        > **NOTE:** Do not set `force_evacuate_on_destroy` in production operation as
+        there are many pitfalls to its use when working with complex cluster
+        configurations. Depending on the virtual machines currently on the cluster, and
+        your DRS and HA settings, the full host evacuation may fail. Instead,
+        incrementally remove hosts from your configuration by adjusting the contents of
+        the `host_system_ids` attribute.
         """
         return pulumi.get(self, "force_evacuate_on_destroy")
 
     @property
     @pulumi.getter(name="haAdmissionControlFailoverHostSystemIds")
     def ha_admission_control_failover_host_system_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/compute_cluster_vm_affinity_rule.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/compute_cluster_vm_affinity_rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,18 @@
                ID of the cluster to put the group in.  Forces a new
                resource if changed.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machine_ids: The UUIDs of the virtual machines to run
                on the same host together.
         :param pulumi.Input[bool] enabled: Enable this rule in the cluster. Default: `true`.
         :param pulumi.Input[bool] mandatory: When this value is `true`, prevents any virtual
                machine operations that may violate this rule. Default: `false`.
+               
+               > **NOTE:** The namespace for rule names on this resource (defined by the
+               `name` argument) is shared with all rules in the cluster - consider
+               this when naming your rules.
         :param pulumi.Input[str] name: The name of the rule. This must be unique in the cluster.
         """
         pulumi.set(__self__, "compute_cluster_id", compute_cluster_id)
         pulumi.set(__self__, "virtual_machine_ids", virtual_machine_ids)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if mandatory is not None:
@@ -81,14 +85,18 @@
 
     @property
     @pulumi.getter
     def mandatory(self) -> Optional[pulumi.Input[bool]]:
         """
         When this value is `true`, prevents any virtual
         machine operations that may violate this rule. Default: `false`.
+
+        > **NOTE:** The namespace for rule names on this resource (defined by the
+        `name` argument) is shared with all rules in the cluster - consider
+        this when naming your rules.
         """
         return pulumi.get(self, "mandatory")
 
     @mandatory.setter
     def mandatory(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "mandatory", value)
 
@@ -117,14 +125,18 @@
         Input properties used for looking up and filtering ComputeClusterVmAffinityRule resources.
         :param pulumi.Input[str] compute_cluster_id: The managed object reference
                ID of the cluster to put the group in.  Forces a new
                resource if changed.
         :param pulumi.Input[bool] enabled: Enable this rule in the cluster. Default: `true`.
         :param pulumi.Input[bool] mandatory: When this value is `true`, prevents any virtual
                machine operations that may violate this rule. Default: `false`.
+               
+               > **NOTE:** The namespace for rule names on this resource (defined by the
+               `name` argument) is shared with all rules in the cluster - consider
+               this when naming your rules.
         :param pulumi.Input[str] name: The name of the rule. This must be unique in the cluster.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machine_ids: The UUIDs of the virtual machines to run
                on the same host together.
         """
         if compute_cluster_id is not None:
             pulumi.set(__self__, "compute_cluster_id", compute_cluster_id)
         if enabled is not None:
@@ -164,14 +176,18 @@
 
     @property
     @pulumi.getter
     def mandatory(self) -> Optional[pulumi.Input[bool]]:
         """
         When this value is `true`, prevents any virtual
         machine operations that may violate this rule. Default: `false`.
+
+        > **NOTE:** The namespace for rule names on this resource (defined by the
+        `name` argument) is shared with all rules in the cluster - consider
+        this when naming your rules.
         """
         return pulumi.get(self, "mandatory")
 
     @mandatory.setter
     def mandatory(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "mandatory", value)
 
@@ -302,14 +318,18 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] compute_cluster_id: The managed object reference
                ID of the cluster to put the group in.  Forces a new
                resource if changed.
         :param pulumi.Input[bool] enabled: Enable this rule in the cluster. Default: `true`.
         :param pulumi.Input[bool] mandatory: When this value is `true`, prevents any virtual
                machine operations that may violate this rule. Default: `false`.
+               
+               > **NOTE:** The namespace for rule names on this resource (defined by the
+               `name` argument) is shared with all rules in the cluster - consider
+               this when naming your rules.
         :param pulumi.Input[str] name: The name of the rule. This must be unique in the cluster.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machine_ids: The UUIDs of the virtual machines to run
                on the same host together.
         """
         ...
     @overload
     def __init__(__self__,
@@ -464,14 +484,18 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] compute_cluster_id: The managed object reference
                ID of the cluster to put the group in.  Forces a new
                resource if changed.
         :param pulumi.Input[bool] enabled: Enable this rule in the cluster. Default: `true`.
         :param pulumi.Input[bool] mandatory: When this value is `true`, prevents any virtual
                machine operations that may violate this rule. Default: `false`.
+               
+               > **NOTE:** The namespace for rule names on this resource (defined by the
+               `name` argument) is shared with all rules in the cluster - consider
+               this when naming your rules.
         :param pulumi.Input[str] name: The name of the rule. This must be unique in the cluster.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machine_ids: The UUIDs of the virtual machines to run
                on the same host together.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ComputeClusterVmAffinityRuleState.__new__(_ComputeClusterVmAffinityRuleState)
@@ -503,14 +527,18 @@
 
     @property
     @pulumi.getter
     def mandatory(self) -> pulumi.Output[Optional[bool]]:
         """
         When this value is `true`, prevents any virtual
         machine operations that may violate this rule. Default: `false`.
+
+        > **NOTE:** The namespace for rule names on this resource (defined by the
+        `name` argument) is shared with all rules in the cluster - consider
+        this when naming your rules.
         """
         return pulumi.get(self, "mandatory")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/compute_cluster_vm_anti_affinity_rule.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/compute_cluster_vm_anti_affinity_rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,18 @@
                ID of the cluster to put the group in.  Forces a new
                resource if changed.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machine_ids: The UUIDs of the virtual machines to run
                on hosts different from each other.
         :param pulumi.Input[bool] enabled: Enable this rule in the cluster. Default: `true`.
         :param pulumi.Input[bool] mandatory: When this value is `true`, prevents any virtual
                machine operations that may violate this rule. Default: `false`.
+               
+               > **NOTE:** The namespace for rule names on this resource (defined by the
+               `name` argument) is shared with all rules in the cluster - consider
+               this when naming your rules.
         :param pulumi.Input[str] name: The name of the rule. This must be unique in the cluster.
         """
         pulumi.set(__self__, "compute_cluster_id", compute_cluster_id)
         pulumi.set(__self__, "virtual_machine_ids", virtual_machine_ids)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if mandatory is not None:
@@ -81,14 +85,18 @@
 
     @property
     @pulumi.getter
     def mandatory(self) -> Optional[pulumi.Input[bool]]:
         """
         When this value is `true`, prevents any virtual
         machine operations that may violate this rule. Default: `false`.
+
+        > **NOTE:** The namespace for rule names on this resource (defined by the
+        `name` argument) is shared with all rules in the cluster - consider
+        this when naming your rules.
         """
         return pulumi.get(self, "mandatory")
 
     @mandatory.setter
     def mandatory(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "mandatory", value)
 
@@ -117,14 +125,18 @@
         Input properties used for looking up and filtering ComputeClusterVmAntiAffinityRule resources.
         :param pulumi.Input[str] compute_cluster_id: The managed object reference
                ID of the cluster to put the group in.  Forces a new
                resource if changed.
         :param pulumi.Input[bool] enabled: Enable this rule in the cluster. Default: `true`.
         :param pulumi.Input[bool] mandatory: When this value is `true`, prevents any virtual
                machine operations that may violate this rule. Default: `false`.
+               
+               > **NOTE:** The namespace for rule names on this resource (defined by the
+               `name` argument) is shared with all rules in the cluster - consider
+               this when naming your rules.
         :param pulumi.Input[str] name: The name of the rule. This must be unique in the cluster.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machine_ids: The UUIDs of the virtual machines to run
                on hosts different from each other.
         """
         if compute_cluster_id is not None:
             pulumi.set(__self__, "compute_cluster_id", compute_cluster_id)
         if enabled is not None:
@@ -164,14 +176,18 @@
 
     @property
     @pulumi.getter
     def mandatory(self) -> Optional[pulumi.Input[bool]]:
         """
         When this value is `true`, prevents any virtual
         machine operations that may violate this rule. Default: `false`.
+
+        > **NOTE:** The namespace for rule names on this resource (defined by the
+        `name` argument) is shared with all rules in the cluster - consider
+        this when naming your rules.
         """
         return pulumi.get(self, "mandatory")
 
     @mandatory.setter
     def mandatory(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "mandatory", value)
 
@@ -218,14 +234,18 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] compute_cluster_id: The managed object reference
                ID of the cluster to put the group in.  Forces a new
                resource if changed.
         :param pulumi.Input[bool] enabled: Enable this rule in the cluster. Default: `true`.
         :param pulumi.Input[bool] mandatory: When this value is `true`, prevents any virtual
                machine operations that may violate this rule. Default: `false`.
+               
+               > **NOTE:** The namespace for rule names on this resource (defined by the
+               `name` argument) is shared with all rules in the cluster - consider
+               this when naming your rules.
         :param pulumi.Input[str] name: The name of the rule. This must be unique in the cluster.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machine_ids: The UUIDs of the virtual machines to run
                on hosts different from each other.
         """
         ...
     @overload
     def __init__(__self__,
@@ -296,14 +316,18 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] compute_cluster_id: The managed object reference
                ID of the cluster to put the group in.  Forces a new
                resource if changed.
         :param pulumi.Input[bool] enabled: Enable this rule in the cluster. Default: `true`.
         :param pulumi.Input[bool] mandatory: When this value is `true`, prevents any virtual
                machine operations that may violate this rule. Default: `false`.
+               
+               > **NOTE:** The namespace for rule names on this resource (defined by the
+               `name` argument) is shared with all rules in the cluster - consider
+               this when naming your rules.
         :param pulumi.Input[str] name: The name of the rule. This must be unique in the cluster.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machine_ids: The UUIDs of the virtual machines to run
                on hosts different from each other.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ComputeClusterVmAntiAffinityRuleState.__new__(_ComputeClusterVmAntiAffinityRuleState)
@@ -335,14 +359,18 @@
 
     @property
     @pulumi.getter
     def mandatory(self) -> pulumi.Output[Optional[bool]]:
         """
         When this value is `true`, prevents any virtual
         machine operations that may violate this rule. Default: `false`.
+
+        > **NOTE:** The namespace for rule names on this resource (defined by the
+        `name` argument) is shared with all rules in the cluster - consider
+        this when naming your rules.
         """
         return pulumi.get(self, "mandatory")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/compute_cluster_vm_dependency_rule.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/compute_cluster_vm_dependency_rule.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,18 @@
         :param pulumi.Input[str] vm_group_name: The name of the VM group that is the subject of
                this rule. The VMs defined in this group will not be started until the VMs in
                the group specified by
                `dependency_vm_group_name` are started.
         :param pulumi.Input[bool] enabled: Enable this rule in the cluster. Default: `true`.
         :param pulumi.Input[bool] mandatory: When this value is `true`, prevents any virtual
                machine operations that may violate this rule. Default: `false`.
+               
+               > **NOTE:** The namespace for rule names on this resource (defined by the
+               `name` argument) is shared with all rules in the cluster - consider
+               this when naming your rules.
         :param pulumi.Input[str] name: The name of the rule. This must be unique in the
                cluster.
         """
         pulumi.set(__self__, "compute_cluster_id", compute_cluster_id)
         pulumi.set(__self__, "dependency_vm_group_name", dependency_vm_group_name)
         pulumi.set(__self__, "vm_group_name", vm_group_name)
         if enabled is not None:
@@ -107,14 +111,18 @@
 
     @property
     @pulumi.getter
     def mandatory(self) -> Optional[pulumi.Input[bool]]:
         """
         When this value is `true`, prevents any virtual
         machine operations that may violate this rule. Default: `false`.
+
+        > **NOTE:** The namespace for rule names on this resource (defined by the
+        `name` argument) is shared with all rules in the cluster - consider
+        this when naming your rules.
         """
         return pulumi.get(self, "mandatory")
 
     @mandatory.setter
     def mandatory(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "mandatory", value)
 
@@ -149,14 +157,18 @@
         :param pulumi.Input[str] dependency_vm_group_name: The name of the VM group that this
                rule depends on. The VMs defined in the group specified by
                `vm_group_name` will not be started until the VMs in this
                group are started.
         :param pulumi.Input[bool] enabled: Enable this rule in the cluster. Default: `true`.
         :param pulumi.Input[bool] mandatory: When this value is `true`, prevents any virtual
                machine operations that may violate this rule. Default: `false`.
+               
+               > **NOTE:** The namespace for rule names on this resource (defined by the
+               `name` argument) is shared with all rules in the cluster - consider
+               this when naming your rules.
         :param pulumi.Input[str] name: The name of the rule. This must be unique in the
                cluster.
         :param pulumi.Input[str] vm_group_name: The name of the VM group that is the subject of
                this rule. The VMs defined in this group will not be started until the VMs in
                the group specified by
                `dependency_vm_group_name` are started.
         """
@@ -216,14 +228,18 @@
 
     @property
     @pulumi.getter
     def mandatory(self) -> Optional[pulumi.Input[bool]]:
         """
         When this value is `true`, prevents any virtual
         machine operations that may violate this rule. Default: `false`.
+
+        > **NOTE:** The namespace for rule names on this resource (defined by the
+        `name` argument) is shared with all rules in the cluster - consider
+        this when naming your rules.
         """
         return pulumi.get(self, "mandatory")
 
     @mandatory.setter
     def mandatory(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "mandatory", value)
 
@@ -278,14 +294,18 @@
         :param pulumi.Input[str] dependency_vm_group_name: The name of the VM group that this
                rule depends on. The VMs defined in the group specified by
                `vm_group_name` will not be started until the VMs in this
                group are started.
         :param pulumi.Input[bool] enabled: Enable this rule in the cluster. Default: `true`.
         :param pulumi.Input[bool] mandatory: When this value is `true`, prevents any virtual
                machine operations that may violate this rule. Default: `false`.
+               
+               > **NOTE:** The namespace for rule names on this resource (defined by the
+               `name` argument) is shared with all rules in the cluster - consider
+               this when naming your rules.
         :param pulumi.Input[str] name: The name of the rule. This must be unique in the
                cluster.
         :param pulumi.Input[str] vm_group_name: The name of the VM group that is the subject of
                this rule. The VMs defined in this group will not be started until the VMs in
                the group specified by
                `dependency_vm_group_name` are started.
         """
@@ -368,14 +388,18 @@
         :param pulumi.Input[str] dependency_vm_group_name: The name of the VM group that this
                rule depends on. The VMs defined in the group specified by
                `vm_group_name` will not be started until the VMs in this
                group are started.
         :param pulumi.Input[bool] enabled: Enable this rule in the cluster. Default: `true`.
         :param pulumi.Input[bool] mandatory: When this value is `true`, prevents any virtual
                machine operations that may violate this rule. Default: `false`.
+               
+               > **NOTE:** The namespace for rule names on this resource (defined by the
+               `name` argument) is shared with all rules in the cluster - consider
+               this when naming your rules.
         :param pulumi.Input[str] name: The name of the rule. This must be unique in the
                cluster.
         :param pulumi.Input[str] vm_group_name: The name of the VM group that is the subject of
                this rule. The VMs defined in this group will not be started until the VMs in
                the group specified by
                `dependency_vm_group_name` are started.
         """
@@ -422,14 +446,18 @@
 
     @property
     @pulumi.getter
     def mandatory(self) -> pulumi.Output[Optional[bool]]:
         """
         When this value is `true`, prevents any virtual
         machine operations that may violate this rule. Default: `false`.
+
+        > **NOTE:** The namespace for rule names on this resource (defined by the
+        `name` argument) is shared with all rules in the cluster - consider
+        this when naming your rules.
         """
         return pulumi.get(self, "mandatory")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/compute_cluster_vm_group.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/compute_cluster_vm_group.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,19 @@
         :param pulumi.Input[str] compute_cluster_id: The managed object reference
                ID of the cluster to put the group in.  Forces a new
                resource if changed.
         :param pulumi.Input[str] name: The name of the VM group. This must be unique in the
                cluster. Forces a new resource if changed.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machine_ids: The UUIDs of the virtual machines in this
                group.
+               
+               > **NOTE:** The namespace for cluster names on this resource (defined by the
+               `name` argument) is shared with the
+               `ComputeClusterHostGroup`
+               resource. Make sure your names are unique across both resources.
         """
         pulumi.set(__self__, "compute_cluster_id", compute_cluster_id)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if virtual_machine_ids is not None:
             pulumi.set(__self__, "virtual_machine_ids", virtual_machine_ids)
 
@@ -62,14 +67,19 @@
 
     @property
     @pulumi.getter(name="virtualMachineIds")
     def virtual_machine_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The UUIDs of the virtual machines in this
         group.
+
+        > **NOTE:** The namespace for cluster names on this resource (defined by the
+        `name` argument) is shared with the
+        `ComputeClusterHostGroup`
+        resource. Make sure your names are unique across both resources.
         """
         return pulumi.get(self, "virtual_machine_ids")
 
     @virtual_machine_ids.setter
     def virtual_machine_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "virtual_machine_ids", value)
 
@@ -85,14 +95,19 @@
         :param pulumi.Input[str] compute_cluster_id: The managed object reference
                ID of the cluster to put the group in.  Forces a new
                resource if changed.
         :param pulumi.Input[str] name: The name of the VM group. This must be unique in the
                cluster. Forces a new resource if changed.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machine_ids: The UUIDs of the virtual machines in this
                group.
+               
+               > **NOTE:** The namespace for cluster names on this resource (defined by the
+               `name` argument) is shared with the
+               `ComputeClusterHostGroup`
+               resource. Make sure your names are unique across both resources.
         """
         if compute_cluster_id is not None:
             pulumi.set(__self__, "compute_cluster_id", compute_cluster_id)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if virtual_machine_ids is not None:
             pulumi.set(__self__, "virtual_machine_ids", virtual_machine_ids)
@@ -126,14 +141,19 @@
 
     @property
     @pulumi.getter(name="virtualMachineIds")
     def virtual_machine_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The UUIDs of the virtual machines in this
         group.
+
+        > **NOTE:** The namespace for cluster names on this resource (defined by the
+        `name` argument) is shared with the
+        `ComputeClusterHostGroup`
+        resource. Make sure your names are unique across both resources.
         """
         return pulumi.get(self, "virtual_machine_ids")
 
     @virtual_machine_ids.setter
     def virtual_machine_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "virtual_machine_ids", value)
 
@@ -154,14 +174,19 @@
         :param pulumi.Input[str] compute_cluster_id: The managed object reference
                ID of the cluster to put the group in.  Forces a new
                resource if changed.
         :param pulumi.Input[str] name: The name of the VM group. This must be unique in the
                cluster. Forces a new resource if changed.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machine_ids: The UUIDs of the virtual machines in this
                group.
+               
+               > **NOTE:** The namespace for cluster names on this resource (defined by the
+               `name` argument) is shared with the
+               `ComputeClusterHostGroup`
+               resource. Make sure your names are unique across both resources.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ComputeClusterVmGroupArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -222,14 +247,19 @@
         :param pulumi.Input[str] compute_cluster_id: The managed object reference
                ID of the cluster to put the group in.  Forces a new
                resource if changed.
         :param pulumi.Input[str] name: The name of the VM group. This must be unique in the
                cluster. Forces a new resource if changed.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machine_ids: The UUIDs of the virtual machines in this
                group.
+               
+               > **NOTE:** The namespace for cluster names on this resource (defined by the
+               `name` argument) is shared with the
+               `ComputeClusterHostGroup`
+               resource. Make sure your names are unique across both resources.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ComputeClusterVmGroupState.__new__(_ComputeClusterVmGroupState)
 
         __props__.__dict__["compute_cluster_id"] = compute_cluster_id
         __props__.__dict__["name"] = name
@@ -257,10 +287,15 @@
 
     @property
     @pulumi.getter(name="virtualMachineIds")
     def virtual_machine_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         The UUIDs of the virtual machines in this
         group.
+
+        > **NOTE:** The namespace for cluster names on this resource (defined by the
+        `name` argument) is shared with the
+        `ComputeClusterHostGroup`
+        resource. Make sure your names are unique across both resources.
         """
         return pulumi.get(self, "virtual_machine_ids")
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/compute_cluster_vm_host_rule.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/compute_cluster_vm_host_rule.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,14 +33,22 @@
                hosts defined in this host group.
         :param pulumi.Input[str] anti_affinity_host_group_name: When this field is used, the
                virtual machines defined in `vm_group_name` will _not_ be
                run on the hosts defined in this host group.
         :param pulumi.Input[bool] enabled: Enable this rule in the cluster. Default: `true`.
         :param pulumi.Input[bool] mandatory: When this value is `true`, prevents any virtual
                machine operations that may violate this rule. Default: `false`.
+               
+               > **NOTE:** One of `affinity_host_group_name` or
+               `anti_affinity_host_group_name` must be
+               defined, but not both.
+               
+               > **NOTE:** The namespace for rule names on this resource (defined by the
+               `name` argument) is shared with all rules in the cluster - consider
+               this when naming your rules.
         :param pulumi.Input[str] name: The name of the rule. This must be unique in the
                cluster.
         """
         pulumi.set(__self__, "compute_cluster_id", compute_cluster_id)
         pulumi.set(__self__, "vm_group_name", vm_group_name)
         if affinity_host_group_name is not None:
             pulumi.set(__self__, "affinity_host_group_name", affinity_host_group_name)
@@ -122,14 +130,22 @@
 
     @property
     @pulumi.getter
     def mandatory(self) -> Optional[pulumi.Input[bool]]:
         """
         When this value is `true`, prevents any virtual
         machine operations that may violate this rule. Default: `false`.
+
+        > **NOTE:** One of `affinity_host_group_name` or
+        `anti_affinity_host_group_name` must be
+        defined, but not both.
+
+        > **NOTE:** The namespace for rule names on this resource (defined by the
+        `name` argument) is shared with all rules in the cluster - consider
+        this when naming your rules.
         """
         return pulumi.get(self, "mandatory")
 
     @mandatory.setter
     def mandatory(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "mandatory", value)
 
@@ -167,14 +183,22 @@
                run on the hosts defined in this host group.
         :param pulumi.Input[str] compute_cluster_id: The managed object reference
                ID of the cluster to put the group in.  Forces a new
                resource if changed.
         :param pulumi.Input[bool] enabled: Enable this rule in the cluster. Default: `true`.
         :param pulumi.Input[bool] mandatory: When this value is `true`, prevents any virtual
                machine operations that may violate this rule. Default: `false`.
+               
+               > **NOTE:** One of `affinity_host_group_name` or
+               `anti_affinity_host_group_name` must be
+               defined, but not both.
+               
+               > **NOTE:** The namespace for rule names on this resource (defined by the
+               `name` argument) is shared with all rules in the cluster - consider
+               this when naming your rules.
         :param pulumi.Input[str] name: The name of the rule. This must be unique in the
                cluster.
         :param pulumi.Input[str] vm_group_name: The name of the virtual machine group to use
                with this rule.
         """
         if affinity_host_group_name is not None:
             pulumi.set(__self__, "affinity_host_group_name", affinity_host_group_name)
@@ -247,14 +271,22 @@
 
     @property
     @pulumi.getter
     def mandatory(self) -> Optional[pulumi.Input[bool]]:
         """
         When this value is `true`, prevents any virtual
         machine operations that may violate this rule. Default: `false`.
+
+        > **NOTE:** One of `affinity_host_group_name` or
+        `anti_affinity_host_group_name` must be
+        defined, but not both.
+
+        > **NOTE:** The namespace for rule names on this resource (defined by the
+        `name` argument) is shared with all rules in the cluster - consider
+        this when naming your rules.
         """
         return pulumi.get(self, "mandatory")
 
     @mandatory.setter
     def mandatory(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "mandatory", value)
 
@@ -310,14 +342,22 @@
                run on the hosts defined in this host group.
         :param pulumi.Input[str] compute_cluster_id: The managed object reference
                ID of the cluster to put the group in.  Forces a new
                resource if changed.
         :param pulumi.Input[bool] enabled: Enable this rule in the cluster. Default: `true`.
         :param pulumi.Input[bool] mandatory: When this value is `true`, prevents any virtual
                machine operations that may violate this rule. Default: `false`.
+               
+               > **NOTE:** One of `affinity_host_group_name` or
+               `anti_affinity_host_group_name` must be
+               defined, but not both.
+               
+               > **NOTE:** The namespace for rule names on this resource (defined by the
+               `name` argument) is shared with all rules in the cluster - consider
+               this when naming your rules.
         :param pulumi.Input[str] name: The name of the rule. This must be unique in the
                cluster.
         :param pulumi.Input[str] vm_group_name: The name of the virtual machine group to use
                with this rule.
         """
         ...
     @overload
@@ -401,14 +441,22 @@
                run on the hosts defined in this host group.
         :param pulumi.Input[str] compute_cluster_id: The managed object reference
                ID of the cluster to put the group in.  Forces a new
                resource if changed.
         :param pulumi.Input[bool] enabled: Enable this rule in the cluster. Default: `true`.
         :param pulumi.Input[bool] mandatory: When this value is `true`, prevents any virtual
                machine operations that may violate this rule. Default: `false`.
+               
+               > **NOTE:** One of `affinity_host_group_name` or
+               `anti_affinity_host_group_name` must be
+               defined, but not both.
+               
+               > **NOTE:** The namespace for rule names on this resource (defined by the
+               `name` argument) is shared with all rules in the cluster - consider
+               this when naming your rules.
         :param pulumi.Input[str] name: The name of the rule. This must be unique in the
                cluster.
         :param pulumi.Input[str] vm_group_name: The name of the virtual machine group to use
                with this rule.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
@@ -463,14 +511,22 @@
 
     @property
     @pulumi.getter
     def mandatory(self) -> pulumi.Output[Optional[bool]]:
         """
         When this value is `true`, prevents any virtual
         machine operations that may violate this rule. Default: `false`.
+
+        > **NOTE:** One of `affinity_host_group_name` or
+        `anti_affinity_host_group_name` must be
+        defined, but not both.
+
+        > **NOTE:** The namespace for rule names on this resource (defined by the
+        `name` argument) is shared with all rules in the cluster - consider
+        this when naming your rules.
         """
         return pulumi.get(self, "mandatory")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/config/vars.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/content_library.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/content_library.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/content_library_item.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/content_library_item.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/custom_attribute.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/datacenter.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/datacenter.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,19 +20,27 @@
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a Datacenter resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to value 
                strings to set for datacenter resource. See
                [here][docs-setting-custom-attributes] for a reference on how to set values
                for custom attributes.
+               
+               [docs-setting-custom-attributes]: /docs/providers/vsphere/r/custom_attribute.html#using-custom-attributes-in-a-supported-resource
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+               and require vCenter.
         :param pulumi.Input[str] folder: The folder where the datacenter should be created.
                Forces a new resource if changed.
         :param pulumi.Input[str] name: The name of the datacenter. This name needs to be unique
                within the folder. Forces a new resource if changed.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource.
+               
+               > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+               requires vCenter 6.0 or higher.
         """
         if custom_attributes is not None:
             pulumi.set(__self__, "custom_attributes", custom_attributes)
         if folder is not None:
             pulumi.set(__self__, "folder", folder)
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -43,14 +51,19 @@
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Map of custom attribute ids to value 
         strings to set for datacenter resource. See
         [here][docs-setting-custom-attributes] for a reference on how to set values
         for custom attributes.
+
+        [docs-setting-custom-attributes]: /docs/providers/vsphere/r/custom_attribute.html#using-custom-attributes-in-a-supported-resource
+
+        > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+        and require vCenter.
         """
         return pulumi.get(self, "custom_attributes")
 
     @custom_attributes.setter
     def custom_attributes(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "custom_attributes", value)
 
@@ -81,14 +94,17 @@
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The IDs of any tags to attach to this resource.
+
+        > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+        requires vCenter 6.0 or higher.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -103,20 +119,28 @@
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering Datacenter resources.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to value 
                strings to set for datacenter resource. See
                [here][docs-setting-custom-attributes] for a reference on how to set values
                for custom attributes.
+               
+               [docs-setting-custom-attributes]: /docs/providers/vsphere/r/custom_attribute.html#using-custom-attributes-in-a-supported-resource
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+               and require vCenter.
         :param pulumi.Input[str] folder: The folder where the datacenter should be created.
                Forces a new resource if changed.
         :param pulumi.Input[str] moid: Managed object ID of this datacenter.
         :param pulumi.Input[str] name: The name of the datacenter. This name needs to be unique
                within the folder. Forces a new resource if changed.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource.
+               
+               > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+               requires vCenter 6.0 or higher.
         """
         if custom_attributes is not None:
             pulumi.set(__self__, "custom_attributes", custom_attributes)
         if folder is not None:
             pulumi.set(__self__, "folder", folder)
         if moid is not None:
             pulumi.set(__self__, "moid", moid)
@@ -129,14 +153,19 @@
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Map of custom attribute ids to value 
         strings to set for datacenter resource. See
         [here][docs-setting-custom-attributes] for a reference on how to set values
         for custom attributes.
+
+        [docs-setting-custom-attributes]: /docs/providers/vsphere/r/custom_attribute.html#using-custom-attributes-in-a-supported-resource
+
+        > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+        and require vCenter.
         """
         return pulumi.get(self, "custom_attributes")
 
     @custom_attributes.setter
     def custom_attributes(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "custom_attributes", value)
 
@@ -179,14 +208,17 @@
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The IDs of any tags to attach to this resource.
+
+        > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+        requires vCenter 6.0 or higher.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -225,19 +257,27 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to value 
                strings to set for datacenter resource. See
                [here][docs-setting-custom-attributes] for a reference on how to set values
                for custom attributes.
+               
+               [docs-setting-custom-attributes]: /docs/providers/vsphere/r/custom_attribute.html#using-custom-attributes-in-a-supported-resource
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+               and require vCenter.
         :param pulumi.Input[str] folder: The folder where the datacenter should be created.
                Forces a new resource if changed.
         :param pulumi.Input[str] name: The name of the datacenter. This name needs to be unique
                within the folder. Forces a new resource if changed.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource.
+               
+               > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+               requires vCenter 6.0 or higher.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[DatacenterArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -318,20 +358,28 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to value 
                strings to set for datacenter resource. See
                [here][docs-setting-custom-attributes] for a reference on how to set values
                for custom attributes.
+               
+               [docs-setting-custom-attributes]: /docs/providers/vsphere/r/custom_attribute.html#using-custom-attributes-in-a-supported-resource
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+               and require vCenter.
         :param pulumi.Input[str] folder: The folder where the datacenter should be created.
                Forces a new resource if changed.
         :param pulumi.Input[str] moid: Managed object ID of this datacenter.
         :param pulumi.Input[str] name: The name of the datacenter. This name needs to be unique
                within the folder. Forces a new resource if changed.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource.
+               
+               > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+               requires vCenter 6.0 or higher.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _DatacenterState.__new__(_DatacenterState)
 
         __props__.__dict__["custom_attributes"] = custom_attributes
         __props__.__dict__["folder"] = folder
@@ -344,14 +392,19 @@
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
         Map of custom attribute ids to value 
         strings to set for datacenter resource. See
         [here][docs-setting-custom-attributes] for a reference on how to set values
         for custom attributes.
+
+        [docs-setting-custom-attributes]: /docs/providers/vsphere/r/custom_attribute.html#using-custom-attributes-in-a-supported-resource
+
+        > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+        and require vCenter.
         """
         return pulumi.get(self, "custom_attributes")
 
     @property
     @pulumi.getter
     def folder(self) -> pulumi.Output[Optional[str]]:
         """
@@ -378,10 +431,13 @@
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def tags(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         The IDs of any tags to attach to this resource.
+
+        > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+        requires vCenter 6.0 or higher.
         """
         return pulumi.get(self, "tags")
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/datastore_cluster.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/datastore_cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,19 @@
         :param pulumi.Input[str] datacenter_id: The managed object ID of
                the datacenter to create the datastore cluster in. Forces a new resource if
                changed.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: A map of custom attribute ids to attribute
                value strings to set for the datastore cluster. See
                [here][docs-setting-custom-attributes] for a reference on how to set values
                for custom attributes.
+               
+               [docs-setting-custom-attributes]: /docs/providers/vsphere/r/custom_attribute.html#using-custom-attributes-in-a-supported-resource
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+               and require vCenter.
         :param pulumi.Input[str] folder: The relative path to a folder to put this datastore
                cluster in.  This is a path relative to the datacenter you are deploying the
                datastore to.  Example: for the `dc1` datacenter, and a provided `folder` of
                `foo/bar`, The provider will place a datastore cluster named
                `datastore-cluster-test` in a datastore folder located at
                `/dc1/datastore/foo/bar`, with the final inventory path being
                `/dc1/datastore/foo/bar/datastore-cluster-test`.
@@ -111,14 +116,16 @@
                automation settings when correcting disk space imbalances.
         :param pulumi.Input[int] sdrs_space_utilization_threshold: Runtime thresholds govern 
                when Storage DRS performs or recommends migrations
                (based on the selected automation level). Default: `80` percent.
         :param pulumi.Input[str] sdrs_vm_evacuation_automation_level: Overrides the default
                automation settings when generating recommendations for datastore evacuation.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource.
+               
+               > **NOTE:** Tagging support requires vCenter 6.0 or higher.
         """
         pulumi.set(__self__, "datacenter_id", datacenter_id)
         if custom_attributes is not None:
             pulumi.set(__self__, "custom_attributes", custom_attributes)
         if folder is not None:
             pulumi.set(__self__, "folder", folder)
         if name is not None:
@@ -184,14 +191,19 @@
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         A map of custom attribute ids to attribute
         value strings to set for the datastore cluster. See
         [here][docs-setting-custom-attributes] for a reference on how to set values
         for custom attributes.
+
+        [docs-setting-custom-attributes]: /docs/providers/vsphere/r/custom_attribute.html#using-custom-attributes-in-a-supported-resource
+
+        > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+        and require vCenter.
         """
         return pulumi.get(self, "custom_attributes")
 
     @custom_attributes.setter
     def custom_attributes(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "custom_attributes", value)
 
@@ -504,14 +516,16 @@
         pulumi.set(self, "sdrs_vm_evacuation_automation_level", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The IDs of any tags to attach to this resource.
+
+        > **NOTE:** Tagging support requires vCenter 6.0 or higher.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -546,14 +560,19 @@
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering DatastoreCluster resources.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: A map of custom attribute ids to attribute
                value strings to set for the datastore cluster. See
                [here][docs-setting-custom-attributes] for a reference on how to set values
                for custom attributes.
+               
+               [docs-setting-custom-attributes]: /docs/providers/vsphere/r/custom_attribute.html#using-custom-attributes-in-a-supported-resource
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+               and require vCenter.
         :param pulumi.Input[str] datacenter_id: The managed object ID of
                the datacenter to create the datastore cluster in. Forces a new resource if
                changed.
         :param pulumi.Input[str] folder: The relative path to a folder to put this datastore
                cluster in.  This is a path relative to the datacenter you are deploying the
                datastore to.  Example: for the `dc1` datacenter, and a provided `folder` of
                `foo/bar`, The provider will place a datastore cluster named
@@ -616,14 +635,16 @@
                automation settings when correcting disk space imbalances.
         :param pulumi.Input[int] sdrs_space_utilization_threshold: Runtime thresholds govern 
                when Storage DRS performs or recommends migrations
                (based on the selected automation level). Default: `80` percent.
         :param pulumi.Input[str] sdrs_vm_evacuation_automation_level: Overrides the default
                automation settings when generating recommendations for datastore evacuation.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource.
+               
+               > **NOTE:** Tagging support requires vCenter 6.0 or higher.
         """
         if custom_attributes is not None:
             pulumi.set(__self__, "custom_attributes", custom_attributes)
         if datacenter_id is not None:
             pulumi.set(__self__, "datacenter_id", datacenter_id)
         if folder is not None:
             pulumi.set(__self__, "folder", folder)
@@ -676,14 +697,19 @@
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         A map of custom attribute ids to attribute
         value strings to set for the datastore cluster. See
         [here][docs-setting-custom-attributes] for a reference on how to set values
         for custom attributes.
+
+        [docs-setting-custom-attributes]: /docs/providers/vsphere/r/custom_attribute.html#using-custom-attributes-in-a-supported-resource
+
+        > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+        and require vCenter.
         """
         return pulumi.get(self, "custom_attributes")
 
     @custom_attributes.setter
     def custom_attributes(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "custom_attributes", value)
 
@@ -1010,14 +1036,16 @@
         pulumi.set(self, "sdrs_vm_evacuation_automation_level", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The IDs of any tags to attach to this resource.
+
+        > **NOTE:** Tagging support requires vCenter 6.0 or higher.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -1057,14 +1085,19 @@
         Create a DatastoreCluster resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: A map of custom attribute ids to attribute
                value strings to set for the datastore cluster. See
                [here][docs-setting-custom-attributes] for a reference on how to set values
                for custom attributes.
+               
+               [docs-setting-custom-attributes]: /docs/providers/vsphere/r/custom_attribute.html#using-custom-attributes-in-a-supported-resource
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+               and require vCenter.
         :param pulumi.Input[str] datacenter_id: The managed object ID of
                the datacenter to create the datastore cluster in. Forces a new resource if
                changed.
         :param pulumi.Input[str] folder: The relative path to a folder to put this datastore
                cluster in.  This is a path relative to the datacenter you are deploying the
                datastore to.  Example: for the `dc1` datacenter, and a provided `folder` of
                `foo/bar`, The provider will place a datastore cluster named
@@ -1127,14 +1160,16 @@
                automation settings when correcting disk space imbalances.
         :param pulumi.Input[int] sdrs_space_utilization_threshold: Runtime thresholds govern 
                when Storage DRS performs or recommends migrations
                (based on the selected automation level). Default: `80` percent.
         :param pulumi.Input[str] sdrs_vm_evacuation_automation_level: Overrides the default
                automation settings when generating recommendations for datastore evacuation.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource.
+               
+               > **NOTE:** Tagging support requires vCenter 6.0 or higher.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: DatastoreClusterArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -1258,14 +1293,19 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: A map of custom attribute ids to attribute
                value strings to set for the datastore cluster. See
                [here][docs-setting-custom-attributes] for a reference on how to set values
                for custom attributes.
+               
+               [docs-setting-custom-attributes]: /docs/providers/vsphere/r/custom_attribute.html#using-custom-attributes-in-a-supported-resource
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+               and require vCenter.
         :param pulumi.Input[str] datacenter_id: The managed object ID of
                the datacenter to create the datastore cluster in. Forces a new resource if
                changed.
         :param pulumi.Input[str] folder: The relative path to a folder to put this datastore
                cluster in.  This is a path relative to the datacenter you are deploying the
                datastore to.  Example: for the `dc1` datacenter, and a provided `folder` of
                `foo/bar`, The provider will place a datastore cluster named
@@ -1328,14 +1368,16 @@
                automation settings when correcting disk space imbalances.
         :param pulumi.Input[int] sdrs_space_utilization_threshold: Runtime thresholds govern 
                when Storage DRS performs or recommends migrations
                (based on the selected automation level). Default: `80` percent.
         :param pulumi.Input[str] sdrs_vm_evacuation_automation_level: Overrides the default
                automation settings when generating recommendations for datastore evacuation.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource.
+               
+               > **NOTE:** Tagging support requires vCenter 6.0 or higher.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _DatastoreClusterState.__new__(_DatastoreClusterState)
 
         __props__.__dict__["custom_attributes"] = custom_attributes
         __props__.__dict__["datacenter_id"] = datacenter_id
@@ -1368,14 +1410,19 @@
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
         A map of custom attribute ids to attribute
         value strings to set for the datastore cluster. See
         [here][docs-setting-custom-attributes] for a reference on how to set values
         for custom attributes.
+
+        [docs-setting-custom-attributes]: /docs/providers/vsphere/r/custom_attribute.html#using-custom-attributes-in-a-supported-resource
+
+        > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+        and require vCenter.
         """
         return pulumi.get(self, "custom_attributes")
 
     @property
     @pulumi.getter(name="datacenterId")
     def datacenter_id(self) -> pulumi.Output[str]:
         """
@@ -1606,10 +1653,12 @@
         return pulumi.get(self, "sdrs_vm_evacuation_automation_level")
 
     @property
     @pulumi.getter
     def tags(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         The IDs of any tags to attach to this resource.
+
+        > **NOTE:** Tagging support requires vCenter 6.0 or higher.
         """
         return pulumi.get(self, "tags")
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/datastore_cluster_vm_anti_affinity_rule.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/datastore_cluster_vm_anti_affinity_rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,16 @@
         """
         The set of arguments for constructing a DatastoreClusterVmAntiAffinityRule resource.
         :param pulumi.Input[str] datastore_cluster_id: The managed object reference
                ID of the datastore cluster to put the group in.  Forces
                a new resource if changed.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machine_ids: The UUIDs of the virtual machines to run
                on different datastores from each other.
+               
+               > **NOTE:** The minimum length of `virtual_machine_ids` is 2.
         :param pulumi.Input[bool] enabled: Enable this rule in the cluster. Default: `true`.
         :param pulumi.Input[bool] mandatory: When this value is `true`, prevents any virtual
                machine operations that may violate this rule. Default: `false`.
         :param pulumi.Input[str] name: The name of the rule. This must be unique in the cluster.
         """
         pulumi.set(__self__, "datastore_cluster_id", datastore_cluster_id)
         pulumi.set(__self__, "virtual_machine_ids", virtual_machine_ids)
@@ -56,14 +58,16 @@
 
     @property
     @pulumi.getter(name="virtualMachineIds")
     def virtual_machine_ids(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
         The UUIDs of the virtual machines to run
         on different datastores from each other.
+
+        > **NOTE:** The minimum length of `virtual_machine_ids` is 2.
         """
         return pulumi.get(self, "virtual_machine_ids")
 
     @virtual_machine_ids.setter
     def virtual_machine_ids(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "virtual_machine_ids", value)
 
@@ -120,14 +124,16 @@
                a new resource if changed.
         :param pulumi.Input[bool] enabled: Enable this rule in the cluster. Default: `true`.
         :param pulumi.Input[bool] mandatory: When this value is `true`, prevents any virtual
                machine operations that may violate this rule. Default: `false`.
         :param pulumi.Input[str] name: The name of the rule. This must be unique in the cluster.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machine_ids: The UUIDs of the virtual machines to run
                on different datastores from each other.
+               
+               > **NOTE:** The minimum length of `virtual_machine_ids` is 2.
         """
         if datastore_cluster_id is not None:
             pulumi.set(__self__, "datastore_cluster_id", datastore_cluster_id)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if mandatory is not None:
             pulumi.set(__self__, "mandatory", mandatory)
@@ -189,14 +195,16 @@
 
     @property
     @pulumi.getter(name="virtualMachineIds")
     def virtual_machine_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The UUIDs of the virtual machines to run
         on different datastores from each other.
+
+        > **NOTE:** The minimum length of `virtual_machine_ids` is 2.
         """
         return pulumi.get(self, "virtual_machine_ids")
 
     @virtual_machine_ids.setter
     def virtual_machine_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "virtual_machine_ids", value)
 
@@ -221,14 +229,16 @@
                a new resource if changed.
         :param pulumi.Input[bool] enabled: Enable this rule in the cluster. Default: `true`.
         :param pulumi.Input[bool] mandatory: When this value is `true`, prevents any virtual
                machine operations that may violate this rule. Default: `false`.
         :param pulumi.Input[str] name: The name of the rule. This must be unique in the cluster.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machine_ids: The UUIDs of the virtual machines to run
                on different datastores from each other.
+               
+               > **NOTE:** The minimum length of `virtual_machine_ids` is 2.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: DatastoreClusterVmAntiAffinityRuleArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -299,14 +309,16 @@
                a new resource if changed.
         :param pulumi.Input[bool] enabled: Enable this rule in the cluster. Default: `true`.
         :param pulumi.Input[bool] mandatory: When this value is `true`, prevents any virtual
                machine operations that may violate this rule. Default: `false`.
         :param pulumi.Input[str] name: The name of the rule. This must be unique in the cluster.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] virtual_machine_ids: The UUIDs of the virtual machines to run
                on different datastores from each other.
+               
+               > **NOTE:** The minimum length of `virtual_machine_ids` is 2.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _DatastoreClusterVmAntiAffinityRuleState.__new__(_DatastoreClusterVmAntiAffinityRuleState)
 
         __props__.__dict__["datastore_cluster_id"] = datastore_cluster_id
         __props__.__dict__["enabled"] = enabled
@@ -352,10 +364,12 @@
 
     @property
     @pulumi.getter(name="virtualMachineIds")
     def virtual_machine_ids(self) -> pulumi.Output[Sequence[str]]:
         """
         The UUIDs of the virtual machines to run
         on different datastores from each other.
+
+        > **NOTE:** The minimum length of `virtual_machine_ids` is 2.
         """
         return pulumi.get(self, "virtual_machine_ids")
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/distributed_port_group.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/distributed_port_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,20 +69,27 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] active_uplinks: List of active uplinks used for load balancing, matching the names of the uplinks assigned in the DVS.
         :param pulumi.Input[bool] allow_forged_transmits: Controls whether or not the virtual network adapter is allowed to send network traffic with a different MAC address than
                that of its own.
         :param pulumi.Input[bool] allow_mac_changes: Controls whether or not the Media Access Control (MAC) address can be changed.
         :param pulumi.Input[bool] allow_promiscuous: Enable promiscuous mode on the network. This flag indicates whether or not all traffic is seen on a given port.
         :param pulumi.Input[bool] auto_expand: Allows the port group to create additional ports
                past the limit specified in `number_of_ports` if necessary. Default: `true`.
+               
+               > **NOTE:** Using `auto_expand` with a statically defined `number_of_ports`
+               may lead to errors when the port count grows past the amount specified.  If you
+               specify `number_of_ports`, you may wish to set `auto_expand` to `false`.
         :param pulumi.Input[bool] block_all_ports: Indicates whether to block all ports by default.
         :param pulumi.Input[bool] block_override_allowed: Allow the port shutdown
                policy to be overridden on an individual port.
         :param pulumi.Input[bool] check_beacon: Enable beacon probing on the ports this policy applies to.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to attribute
                value string to set for port group.
+               
+               > **NOTE:** Custom attributes are not supported on direct ESXi host
+               connections and require vCenter Server.
         :param pulumi.Input[str] description: An optional description for the port group.
         :param pulumi.Input[bool] directpath_gen2_allowed: Allow VMDirectPath Gen2 on the ports this policy applies to.
         :param pulumi.Input[int] egress_shaping_average_bandwidth: The average egress bandwidth in bits per second if egress shaping is enabled on the port.
         :param pulumi.Input[int] egress_shaping_burst_size: The maximum egress burst size allowed in bytes if egress shaping is enabled on the port.
         :param pulumi.Input[bool] egress_shaping_enabled: True if the traffic shaper is enabled for egress traffic on the port.
         :param pulumi.Input[int] egress_shaping_peak_bandwidth: The peak egress bandwidth during bursts in bits per second if egress traffic shaping is enabled on the port.
         :param pulumi.Input[bool] failback: If true, the teaming policy will re-activate failed interfaces higher in precedence when they come back up.
@@ -108,14 +115,16 @@
         :param pulumi.Input[int] number_of_ports: The number of ports available on this port
                group. Cannot be decreased below the amount of used ports on the port group.
         :param pulumi.Input[bool] port_config_reset_at_disconnect: Reset a port's settings to the
                settings defined on this port group policy when the port disconnects.
         :param pulumi.Input[str] port_name_format: An optional formatting policy for naming of
                the ports in this port group. See the `portNameFormat` attribute listed
                [here][ext-vsphere-portname-format] for details on the format syntax.
+               
+               [ext-vsphere-portname-format]: https://vdc-download.vmware.com/vmwb-repository/dcr-public/b50dcbbf-051d-4204-a3e7-e1b618c1e384/538cf2ec-b34f-4bae-a332-3820ef9e7773/vim.dvs.DistributedVirtualPortgroup.ConfigInfo.html#portNameFormat
         :param pulumi.Input[int] port_private_secondary_vlan_id: The secondary VLAN ID for this port.
         :param pulumi.Input[bool] security_policy_override_allowed: Allow the 
                [security policy settings][sec-policy-settings] defined in this port group
                policy to be overridden on an individual port.
         :param pulumi.Input[bool] shaping_override_allowed: Allow the
                [traffic shaping options][traffic-shaping-settings] on this port group policy
                to be overridden on an individual port.
@@ -294,14 +303,18 @@
 
     @property
     @pulumi.getter(name="autoExpand")
     def auto_expand(self) -> Optional[pulumi.Input[bool]]:
         """
         Allows the port group to create additional ports
         past the limit specified in `number_of_ports` if necessary. Default: `true`.
+
+        > **NOTE:** Using `auto_expand` with a statically defined `number_of_ports`
+        may lead to errors when the port count grows past the amount specified.  If you
+        specify `number_of_ports`, you may wish to set `auto_expand` to `false`.
         """
         return pulumi.get(self, "auto_expand")
 
     @auto_expand.setter
     def auto_expand(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "auto_expand", value)
 
@@ -344,14 +357,17 @@
 
     @property
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Map of custom attribute ids to attribute
         value string to set for port group.
+
+        > **NOTE:** Custom attributes are not supported on direct ESXi host
+        connections and require vCenter Server.
         """
         return pulumi.get(self, "custom_attributes")
 
     @custom_attributes.setter
     def custom_attributes(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "custom_attributes", value)
 
@@ -630,14 +646,16 @@
     @property
     @pulumi.getter(name="portNameFormat")
     def port_name_format(self) -> Optional[pulumi.Input[str]]:
         """
         An optional formatting policy for naming of
         the ports in this port group. See the `portNameFormat` attribute listed
         [here][ext-vsphere-portname-format] for details on the format syntax.
+
+        [ext-vsphere-portname-format]: https://vdc-download.vmware.com/vmwb-repository/dcr-public/b50dcbbf-051d-4204-a3e7-e1b618c1e384/538cf2ec-b34f-4bae-a332-3820ef9e7773/vim.dvs.DistributedVirtualPortgroup.ConfigInfo.html#portNameFormat
         """
         return pulumi.get(self, "port_name_format")
 
     @port_name_format.setter
     def port_name_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "port_name_format", value)
 
@@ -866,22 +884,29 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] active_uplinks: List of active uplinks used for load balancing, matching the names of the uplinks assigned in the DVS.
         :param pulumi.Input[bool] allow_forged_transmits: Controls whether or not the virtual network adapter is allowed to send network traffic with a different MAC address than
                that of its own.
         :param pulumi.Input[bool] allow_mac_changes: Controls whether or not the Media Access Control (MAC) address can be changed.
         :param pulumi.Input[bool] allow_promiscuous: Enable promiscuous mode on the network. This flag indicates whether or not all traffic is seen on a given port.
         :param pulumi.Input[bool] auto_expand: Allows the port group to create additional ports
                past the limit specified in `number_of_ports` if necessary. Default: `true`.
+               
+               > **NOTE:** Using `auto_expand` with a statically defined `number_of_ports`
+               may lead to errors when the port count grows past the amount specified.  If you
+               specify `number_of_ports`, you may wish to set `auto_expand` to `false`.
         :param pulumi.Input[bool] block_all_ports: Indicates whether to block all ports by default.
         :param pulumi.Input[bool] block_override_allowed: Allow the port shutdown
                policy to be overridden on an individual port.
         :param pulumi.Input[bool] check_beacon: Enable beacon probing on the ports this policy applies to.
         :param pulumi.Input[str] config_version: The current version of the port group configuration,
                incremented by subsequent updates to the port group.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to attribute
                value string to set for port group.
+               
+               > **NOTE:** Custom attributes are not supported on direct ESXi host
+               connections and require vCenter Server.
         :param pulumi.Input[str] description: An optional description for the port group.
         :param pulumi.Input[bool] directpath_gen2_allowed: Allow VMDirectPath Gen2 on the ports this policy applies to.
         :param pulumi.Input[str] distributed_virtual_switch_uuid: The ID of the VDS to add the
                port group to. Forces a new resource if changed.
         :param pulumi.Input[int] egress_shaping_average_bandwidth: The average egress bandwidth in bits per second if egress shaping is enabled on the port.
         :param pulumi.Input[int] egress_shaping_burst_size: The maximum egress burst size allowed in bytes if egress shaping is enabled on the port.
         :param pulumi.Input[bool] egress_shaping_enabled: True if the traffic shaper is enabled for egress traffic on the port.
@@ -910,14 +935,16 @@
         :param pulumi.Input[int] number_of_ports: The number of ports available on this port
                group. Cannot be decreased below the amount of used ports on the port group.
         :param pulumi.Input[bool] port_config_reset_at_disconnect: Reset a port's settings to the
                settings defined on this port group policy when the port disconnects.
         :param pulumi.Input[str] port_name_format: An optional formatting policy for naming of
                the ports in this port group. See the `portNameFormat` attribute listed
                [here][ext-vsphere-portname-format] for details on the format syntax.
+               
+               [ext-vsphere-portname-format]: https://vdc-download.vmware.com/vmwb-repository/dcr-public/b50dcbbf-051d-4204-a3e7-e1b618c1e384/538cf2ec-b34f-4bae-a332-3820ef9e7773/vim.dvs.DistributedVirtualPortgroup.ConfigInfo.html#portNameFormat
         :param pulumi.Input[int] port_private_secondary_vlan_id: The secondary VLAN ID for this port.
         :param pulumi.Input[bool] security_policy_override_allowed: Allow the 
                [security policy settings][sec-policy-settings] defined in this port group
                policy to be overridden on an individual port.
         :param pulumi.Input[bool] shaping_override_allowed: Allow the
                [traffic shaping options][traffic-shaping-settings] on this port group policy
                to be overridden on an individual port.
@@ -1088,14 +1115,18 @@
 
     @property
     @pulumi.getter(name="autoExpand")
     def auto_expand(self) -> Optional[pulumi.Input[bool]]:
         """
         Allows the port group to create additional ports
         past the limit specified in `number_of_ports` if necessary. Default: `true`.
+
+        > **NOTE:** Using `auto_expand` with a statically defined `number_of_ports`
+        may lead to errors when the port count grows past the amount specified.  If you
+        specify `number_of_ports`, you may wish to set `auto_expand` to `false`.
         """
         return pulumi.get(self, "auto_expand")
 
     @auto_expand.setter
     def auto_expand(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "auto_expand", value)
 
@@ -1151,14 +1182,17 @@
 
     @property
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Map of custom attribute ids to attribute
         value string to set for port group.
+
+        > **NOTE:** Custom attributes are not supported on direct ESXi host
+        connections and require vCenter Server.
         """
         return pulumi.get(self, "custom_attributes")
 
     @custom_attributes.setter
     def custom_attributes(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "custom_attributes", value)
 
@@ -1462,14 +1496,16 @@
     @property
     @pulumi.getter(name="portNameFormat")
     def port_name_format(self) -> Optional[pulumi.Input[str]]:
         """
         An optional formatting policy for naming of
         the ports in this port group. See the `portNameFormat` attribute listed
         [here][ext-vsphere-portname-format] for details on the format syntax.
+
+        [ext-vsphere-portname-format]: https://vdc-download.vmware.com/vmwb-repository/dcr-public/b50dcbbf-051d-4204-a3e7-e1b618c1e384/538cf2ec-b34f-4bae-a332-3820ef9e7773/vim.dvs.DistributedVirtualPortgroup.ConfigInfo.html#portNameFormat
         """
         return pulumi.get(self, "port_name_format")
 
     @port_name_format.setter
     def port_name_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "port_name_format", value)
 
@@ -1701,20 +1737,27 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] active_uplinks: List of active uplinks used for load balancing, matching the names of the uplinks assigned in the DVS.
         :param pulumi.Input[bool] allow_forged_transmits: Controls whether or not the virtual network adapter is allowed to send network traffic with a different MAC address than
                that of its own.
         :param pulumi.Input[bool] allow_mac_changes: Controls whether or not the Media Access Control (MAC) address can be changed.
         :param pulumi.Input[bool] allow_promiscuous: Enable promiscuous mode on the network. This flag indicates whether or not all traffic is seen on a given port.
         :param pulumi.Input[bool] auto_expand: Allows the port group to create additional ports
                past the limit specified in `number_of_ports` if necessary. Default: `true`.
+               
+               > **NOTE:** Using `auto_expand` with a statically defined `number_of_ports`
+               may lead to errors when the port count grows past the amount specified.  If you
+               specify `number_of_ports`, you may wish to set `auto_expand` to `false`.
         :param pulumi.Input[bool] block_all_ports: Indicates whether to block all ports by default.
         :param pulumi.Input[bool] block_override_allowed: Allow the port shutdown
                policy to be overridden on an individual port.
         :param pulumi.Input[bool] check_beacon: Enable beacon probing on the ports this policy applies to.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to attribute
                value string to set for port group.
+               
+               > **NOTE:** Custom attributes are not supported on direct ESXi host
+               connections and require vCenter Server.
         :param pulumi.Input[str] description: An optional description for the port group.
         :param pulumi.Input[bool] directpath_gen2_allowed: Allow VMDirectPath Gen2 on the ports this policy applies to.
         :param pulumi.Input[str] distributed_virtual_switch_uuid: The ID of the VDS to add the
                port group to. Forces a new resource if changed.
         :param pulumi.Input[int] egress_shaping_average_bandwidth: The average egress bandwidth in bits per second if egress shaping is enabled on the port.
         :param pulumi.Input[int] egress_shaping_burst_size: The maximum egress burst size allowed in bytes if egress shaping is enabled on the port.
         :param pulumi.Input[bool] egress_shaping_enabled: True if the traffic shaper is enabled for egress traffic on the port.
@@ -1742,14 +1785,16 @@
         :param pulumi.Input[int] number_of_ports: The number of ports available on this port
                group. Cannot be decreased below the amount of used ports on the port group.
         :param pulumi.Input[bool] port_config_reset_at_disconnect: Reset a port's settings to the
                settings defined on this port group policy when the port disconnects.
         :param pulumi.Input[str] port_name_format: An optional formatting policy for naming of
                the ports in this port group. See the `portNameFormat` attribute listed
                [here][ext-vsphere-portname-format] for details on the format syntax.
+               
+               [ext-vsphere-portname-format]: https://vdc-download.vmware.com/vmwb-repository/dcr-public/b50dcbbf-051d-4204-a3e7-e1b618c1e384/538cf2ec-b34f-4bae-a332-3820ef9e7773/vim.dvs.DistributedVirtualPortgroup.ConfigInfo.html#portNameFormat
         :param pulumi.Input[int] port_private_secondary_vlan_id: The secondary VLAN ID for this port.
         :param pulumi.Input[bool] security_policy_override_allowed: Allow the 
                [security policy settings][sec-policy-settings] defined in this port group
                policy to be overridden on an individual port.
         :param pulumi.Input[bool] shaping_override_allowed: Allow the
                [traffic shaping options][traffic-shaping-settings] on this port group policy
                to be overridden on an individual port.
@@ -1968,22 +2013,29 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] active_uplinks: List of active uplinks used for load balancing, matching the names of the uplinks assigned in the DVS.
         :param pulumi.Input[bool] allow_forged_transmits: Controls whether or not the virtual network adapter is allowed to send network traffic with a different MAC address than
                that of its own.
         :param pulumi.Input[bool] allow_mac_changes: Controls whether or not the Media Access Control (MAC) address can be changed.
         :param pulumi.Input[bool] allow_promiscuous: Enable promiscuous mode on the network. This flag indicates whether or not all traffic is seen on a given port.
         :param pulumi.Input[bool] auto_expand: Allows the port group to create additional ports
                past the limit specified in `number_of_ports` if necessary. Default: `true`.
+               
+               > **NOTE:** Using `auto_expand` with a statically defined `number_of_ports`
+               may lead to errors when the port count grows past the amount specified.  If you
+               specify `number_of_ports`, you may wish to set `auto_expand` to `false`.
         :param pulumi.Input[bool] block_all_ports: Indicates whether to block all ports by default.
         :param pulumi.Input[bool] block_override_allowed: Allow the port shutdown
                policy to be overridden on an individual port.
         :param pulumi.Input[bool] check_beacon: Enable beacon probing on the ports this policy applies to.
         :param pulumi.Input[str] config_version: The current version of the port group configuration,
                incremented by subsequent updates to the port group.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to attribute
                value string to set for port group.
+               
+               > **NOTE:** Custom attributes are not supported on direct ESXi host
+               connections and require vCenter Server.
         :param pulumi.Input[str] description: An optional description for the port group.
         :param pulumi.Input[bool] directpath_gen2_allowed: Allow VMDirectPath Gen2 on the ports this policy applies to.
         :param pulumi.Input[str] distributed_virtual_switch_uuid: The ID of the VDS to add the
                port group to. Forces a new resource if changed.
         :param pulumi.Input[int] egress_shaping_average_bandwidth: The average egress bandwidth in bits per second if egress shaping is enabled on the port.
         :param pulumi.Input[int] egress_shaping_burst_size: The maximum egress burst size allowed in bytes if egress shaping is enabled on the port.
         :param pulumi.Input[bool] egress_shaping_enabled: True if the traffic shaper is enabled for egress traffic on the port.
@@ -2012,14 +2064,16 @@
         :param pulumi.Input[int] number_of_ports: The number of ports available on this port
                group. Cannot be decreased below the amount of used ports on the port group.
         :param pulumi.Input[bool] port_config_reset_at_disconnect: Reset a port's settings to the
                settings defined on this port group policy when the port disconnects.
         :param pulumi.Input[str] port_name_format: An optional formatting policy for naming of
                the ports in this port group. See the `portNameFormat` attribute listed
                [here][ext-vsphere-portname-format] for details on the format syntax.
+               
+               [ext-vsphere-portname-format]: https://vdc-download.vmware.com/vmwb-repository/dcr-public/b50dcbbf-051d-4204-a3e7-e1b618c1e384/538cf2ec-b34f-4bae-a332-3820ef9e7773/vim.dvs.DistributedVirtualPortgroup.ConfigInfo.html#portNameFormat
         :param pulumi.Input[int] port_private_secondary_vlan_id: The secondary VLAN ID for this port.
         :param pulumi.Input[bool] security_policy_override_allowed: Allow the 
                [security policy settings][sec-policy-settings] defined in this port group
                policy to be overridden on an individual port.
         :param pulumi.Input[bool] shaping_override_allowed: Allow the
                [traffic shaping options][traffic-shaping-settings] on this port group policy
                to be overridden on an individual port.
@@ -2131,14 +2185,18 @@
 
     @property
     @pulumi.getter(name="autoExpand")
     def auto_expand(self) -> pulumi.Output[Optional[bool]]:
         """
         Allows the port group to create additional ports
         past the limit specified in `number_of_ports` if necessary. Default: `true`.
+
+        > **NOTE:** Using `auto_expand` with a statically defined `number_of_ports`
+        may lead to errors when the port count grows past the amount specified.  If you
+        specify `number_of_ports`, you may wish to set `auto_expand` to `false`.
         """
         return pulumi.get(self, "auto_expand")
 
     @property
     @pulumi.getter(name="blockAllPorts")
     def block_all_ports(self) -> pulumi.Output[bool]:
         """
@@ -2174,14 +2232,17 @@
 
     @property
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
         Map of custom attribute ids to attribute
         value string to set for port group.
+
+        > **NOTE:** Custom attributes are not supported on direct ESXi host
+        connections and require vCenter Server.
         """
         return pulumi.get(self, "custom_attributes")
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
@@ -2385,14 +2446,16 @@
     @property
     @pulumi.getter(name="portNameFormat")
     def port_name_format(self) -> pulumi.Output[Optional[str]]:
         """
         An optional formatting policy for naming of
         the ports in this port group. See the `portNameFormat` attribute listed
         [here][ext-vsphere-portname-format] for details on the format syntax.
+
+        [ext-vsphere-portname-format]: https://vdc-download.vmware.com/vmwb-repository/dcr-public/b50dcbbf-051d-4204-a3e7-e1b618c1e384/538cf2ec-b34f-4bae-a332-3820ef9e7773/vim.dvs.DistributedVirtualPortgroup.ConfigInfo.html#portNameFormat
         """
         return pulumi.get(self, "port_name_format")
 
     @property
     @pulumi.getter(name="portPrivateSecondaryVlanId")
     def port_private_secondary_vlan_id(self) -> pulumi.Output[int]:
         """
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/distributed_virtual_switch.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/distributed_virtual_switch.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,20 +130,26 @@
         :param pulumi.Input[int] backupnfc_share_count: The amount of shares to allocate to the backupNfc traffic class for a custom share level.
         :param pulumi.Input[str] backupnfc_share_level: The allocation level for the backupNfc traffic class. Can be one of high, low, normal, or custom.
         :param pulumi.Input[bool] block_all_ports: Shuts down all ports in the port groups that
                this policy applies to, effectively blocking all network access to connected
                virtual devices.
         :param pulumi.Input[bool] check_beacon: Enables beacon probing as an additional measure
                to detect NIC failure.
+               
+               > **NOTE:** VMware recommends using a minimum of 3 NICs when using beacon
+               probing.
         :param pulumi.Input[str] contact_detail: The detailed contact information for the person
                who is responsible for the VDS.
         :param pulumi.Input[str] contact_name: The name of the person who is responsible for the
                VDS.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to attribute
                value strings to set for VDS.
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi host connections
+               and requires vCenter Server.
         :param pulumi.Input[str] description: A detailed description for the VDS.
         :param pulumi.Input[bool] directpath_gen2_allowed: Allow VMDirectPath Gen2 for the ports
                for which this policy applies to.
         :param pulumi.Input[int] egress_shaping_average_bandwidth: The average bandwidth in bits
                per second if egress traffic shaping is enabled on the port.
         :param pulumi.Input[int] egress_shaping_burst_size: The maximum burst size allowed in
                bytes if egress traffic shaping is enabled on the port.
@@ -236,14 +242,16 @@
         :param pulumi.Input[Sequence[pulumi.Input['DistributedVirtualSwitchPvlanMappingArgs']]] pvlan_mappings: Use the `pvlan_mapping` block to declare a
                private VLAN mapping. The options are:
         :param pulumi.Input[Sequence[pulumi.Input[str]]] standby_uplinks: A list of standby uplinks to be used in
                failover. These uplinks need to match the definitions in the
                `uplinks` VDS argument. See
                here for more details.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource.
+               
+               > **NOTE:** Tagging support requires vCenter Server 6.0 or higher.
         :param pulumi.Input[str] teaming_policy: The uplink teaming policy. Can be one of
                `loadbalance_ip`, `loadbalance_srcmac`, `loadbalance_srcid`,
                `failover_explicit`, or `loadbalance_loadbased`.
         :param pulumi.Input[bool] tx_uplink: Forward all traffic transmitted by ports for which
                this policy applies to its VDS uplinks.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] uplinks: A list of strings that uniquely identifies the names
                of the uplinks on the VDS across hosts. The number of items in this list
@@ -262,14 +270,30 @@
         :param pulumi.Input[int] virtualmachine_share_count: The amount of shares to allocate to the virtualMachine traffic class for a custom share level.
         :param pulumi.Input[str] virtualmachine_share_level: The allocation level for the virtualMachine traffic class. Can be one of high, low, normal, or custom.
         :param pulumi.Input[int] vlan_id: The VLAN ID for single VLAN mode. 0 denotes no VLAN.
         :param pulumi.Input[Sequence[pulumi.Input['DistributedVirtualSwitchVlanRangeArgs']]] vlan_ranges: Used to denote VLAN trunking. Use the `min_vlan`
                and `max_vlan` sub-arguments to define the tagged VLAN range. Multiple
                `vlan_range` definitions are allowed, but they must not overlap. Example
                below:
+               
+               ```python
+               import pulumi
+               import pulumi_vsphere as vsphere
+               
+               vds = vsphere.DistributedVirtualSwitch("vds", vlan_ranges=[
+                   vsphere.DistributedVirtualSwitchVlanRangeArgs(
+                       max_vlan=199,
+                       min_vlan=100,
+                   ),
+                   vsphere.DistributedVirtualSwitchVlanRangeArgs(
+                       max_vlan=399,
+                       min_vlan=300,
+                   ),
+               ])
+               ```
         :param pulumi.Input[int] vmotion_maximum_mbit: The maximum allowed usage for the vmotion traffic class, in Mbits/sec.
         :param pulumi.Input[int] vmotion_reservation_mbit: The amount of guaranteed bandwidth for the vmotion traffic class, in Mbits/sec.
         :param pulumi.Input[int] vmotion_share_count: The amount of shares to allocate to the vmotion traffic class for a custom share level.
         :param pulumi.Input[str] vmotion_share_level: The allocation level for the vmotion traffic class. Can be one of high, low, normal, or custom.
         :param pulumi.Input[int] vsan_maximum_mbit: The maximum allowed usage for the vsan traffic class, in Mbits/sec.
         :param pulumi.Input[int] vsan_reservation_mbit: The amount of guaranteed bandwidth for the vsan traffic class, in Mbits/sec.
         :param pulumi.Input[int] vsan_share_count: The amount of shares to allocate to the vsan traffic class for a custom share level.
@@ -595,14 +619,17 @@
 
     @property
     @pulumi.getter(name="checkBeacon")
     def check_beacon(self) -> Optional[pulumi.Input[bool]]:
         """
         Enables beacon probing as an additional measure
         to detect NIC failure.
+
+        > **NOTE:** VMware recommends using a minimum of 3 NICs when using beacon
+        probing.
         """
         return pulumi.get(self, "check_beacon")
 
     @check_beacon.setter
     def check_beacon(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "check_beacon", value)
 
@@ -634,14 +661,17 @@
 
     @property
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Map of custom attribute ids to attribute
         value strings to set for VDS.
+
+        > **NOTE:** Custom attributes are unsupported on direct ESXi host connections
+        and requires vCenter Server.
         """
         return pulumi.get(self, "custom_attributes")
 
     @custom_attributes.setter
     def custom_attributes(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "custom_attributes", value)
 
@@ -1372,14 +1402,16 @@
         pulumi.set(self, "standby_uplinks", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The IDs of any tags to attach to this resource.
+
+        > **NOTE:** Tagging support requires vCenter Server 6.0 or higher.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -1552,14 +1584,30 @@
     @pulumi.getter(name="vlanRanges")
     def vlan_ranges(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['DistributedVirtualSwitchVlanRangeArgs']]]]:
         """
         Used to denote VLAN trunking. Use the `min_vlan`
         and `max_vlan` sub-arguments to define the tagged VLAN range. Multiple
         `vlan_range` definitions are allowed, but they must not overlap. Example
         below:
+
+        ```python
+        import pulumi
+        import pulumi_vsphere as vsphere
+
+        vds = vsphere.DistributedVirtualSwitch("vds", vlan_ranges=[
+            vsphere.DistributedVirtualSwitchVlanRangeArgs(
+                max_vlan=199,
+                min_vlan=100,
+            ),
+            vsphere.DistributedVirtualSwitchVlanRangeArgs(
+                max_vlan=399,
+                min_vlan=300,
+            ),
+        ])
+        ```
         """
         return pulumi.get(self, "vlan_ranges")
 
     @vlan_ranges.setter
     def vlan_ranges(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['DistributedVirtualSwitchVlanRangeArgs']]]]):
         pulumi.set(self, "vlan_ranges", value)
 
@@ -1776,22 +1824,28 @@
         :param pulumi.Input[int] backupnfc_share_count: The amount of shares to allocate to the backupNfc traffic class for a custom share level.
         :param pulumi.Input[str] backupnfc_share_level: The allocation level for the backupNfc traffic class. Can be one of high, low, normal, or custom.
         :param pulumi.Input[bool] block_all_ports: Shuts down all ports in the port groups that
                this policy applies to, effectively blocking all network access to connected
                virtual devices.
         :param pulumi.Input[bool] check_beacon: Enables beacon probing as an additional measure
                to detect NIC failure.
+               
+               > **NOTE:** VMware recommends using a minimum of 3 NICs when using beacon
+               probing.
         :param pulumi.Input[str] config_version: The current version of the VDS configuration, incremented
                by subsequent updates to the VDS.
         :param pulumi.Input[str] contact_detail: The detailed contact information for the person
                who is responsible for the VDS.
         :param pulumi.Input[str] contact_name: The name of the person who is responsible for the
                VDS.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to attribute
                value strings to set for VDS.
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi host connections
+               and requires vCenter Server.
         :param pulumi.Input[str] datacenter_id: The ID of the datacenter where the VDS will be
                created. Forces a new resource if changed.
         :param pulumi.Input[str] description: A detailed description for the VDS.
         :param pulumi.Input[bool] directpath_gen2_allowed: Allow VMDirectPath Gen2 for the ports
                for which this policy applies to.
         :param pulumi.Input[int] egress_shaping_average_bandwidth: The average bandwidth in bits
                per second if egress traffic shaping is enabled on the port.
@@ -1886,14 +1940,16 @@
         :param pulumi.Input[Sequence[pulumi.Input['DistributedVirtualSwitchPvlanMappingArgs']]] pvlan_mappings: Use the `pvlan_mapping` block to declare a
                private VLAN mapping. The options are:
         :param pulumi.Input[Sequence[pulumi.Input[str]]] standby_uplinks: A list of standby uplinks to be used in
                failover. These uplinks need to match the definitions in the
                `uplinks` VDS argument. See
                here for more details.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource.
+               
+               > **NOTE:** Tagging support requires vCenter Server 6.0 or higher.
         :param pulumi.Input[str] teaming_policy: The uplink teaming policy. Can be one of
                `loadbalance_ip`, `loadbalance_srcmac`, `loadbalance_srcid`,
                `failover_explicit`, or `loadbalance_loadbased`.
         :param pulumi.Input[bool] tx_uplink: Forward all traffic transmitted by ports for which
                this policy applies to its VDS uplinks.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] uplinks: A list of strings that uniquely identifies the names
                of the uplinks on the VDS across hosts. The number of items in this list
@@ -1912,14 +1968,30 @@
         :param pulumi.Input[int] virtualmachine_share_count: The amount of shares to allocate to the virtualMachine traffic class for a custom share level.
         :param pulumi.Input[str] virtualmachine_share_level: The allocation level for the virtualMachine traffic class. Can be one of high, low, normal, or custom.
         :param pulumi.Input[int] vlan_id: The VLAN ID for single VLAN mode. 0 denotes no VLAN.
         :param pulumi.Input[Sequence[pulumi.Input['DistributedVirtualSwitchVlanRangeArgs']]] vlan_ranges: Used to denote VLAN trunking. Use the `min_vlan`
                and `max_vlan` sub-arguments to define the tagged VLAN range. Multiple
                `vlan_range` definitions are allowed, but they must not overlap. Example
                below:
+               
+               ```python
+               import pulumi
+               import pulumi_vsphere as vsphere
+               
+               vds = vsphere.DistributedVirtualSwitch("vds", vlan_ranges=[
+                   vsphere.DistributedVirtualSwitchVlanRangeArgs(
+                       max_vlan=199,
+                       min_vlan=100,
+                   ),
+                   vsphere.DistributedVirtualSwitchVlanRangeArgs(
+                       max_vlan=399,
+                       min_vlan=300,
+                   ),
+               ])
+               ```
         :param pulumi.Input[int] vmotion_maximum_mbit: The maximum allowed usage for the vmotion traffic class, in Mbits/sec.
         :param pulumi.Input[int] vmotion_reservation_mbit: The amount of guaranteed bandwidth for the vmotion traffic class, in Mbits/sec.
         :param pulumi.Input[int] vmotion_share_count: The amount of shares to allocate to the vmotion traffic class for a custom share level.
         :param pulumi.Input[str] vmotion_share_level: The allocation level for the vmotion traffic class. Can be one of high, low, normal, or custom.
         :param pulumi.Input[int] vsan_maximum_mbit: The maximum allowed usage for the vsan traffic class, in Mbits/sec.
         :param pulumi.Input[int] vsan_reservation_mbit: The amount of guaranteed bandwidth for the vsan traffic class, in Mbits/sec.
         :param pulumi.Input[int] vsan_share_count: The amount of shares to allocate to the vsan traffic class for a custom share level.
@@ -2235,14 +2307,17 @@
 
     @property
     @pulumi.getter(name="checkBeacon")
     def check_beacon(self) -> Optional[pulumi.Input[bool]]:
         """
         Enables beacon probing as an additional measure
         to detect NIC failure.
+
+        > **NOTE:** VMware recommends using a minimum of 3 NICs when using beacon
+        probing.
         """
         return pulumi.get(self, "check_beacon")
 
     @check_beacon.setter
     def check_beacon(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "check_beacon", value)
 
@@ -2287,14 +2362,17 @@
 
     @property
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Map of custom attribute ids to attribute
         value strings to set for VDS.
+
+        > **NOTE:** Custom attributes are unsupported on direct ESXi host connections
+        and requires vCenter Server.
         """
         return pulumi.get(self, "custom_attributes")
 
     @custom_attributes.setter
     def custom_attributes(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "custom_attributes", value)
 
@@ -3038,14 +3116,16 @@
         pulumi.set(self, "standby_uplinks", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The IDs of any tags to attach to this resource.
+
+        > **NOTE:** Tagging support requires vCenter Server 6.0 or higher.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -3218,14 +3298,30 @@
     @pulumi.getter(name="vlanRanges")
     def vlan_ranges(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['DistributedVirtualSwitchVlanRangeArgs']]]]:
         """
         Used to denote VLAN trunking. Use the `min_vlan`
         and `max_vlan` sub-arguments to define the tagged VLAN range. Multiple
         `vlan_range` definitions are allowed, but they must not overlap. Example
         below:
+
+        ```python
+        import pulumi
+        import pulumi_vsphere as vsphere
+
+        vds = vsphere.DistributedVirtualSwitch("vds", vlan_ranges=[
+            vsphere.DistributedVirtualSwitchVlanRangeArgs(
+                max_vlan=199,
+                min_vlan=100,
+            ),
+            vsphere.DistributedVirtualSwitchVlanRangeArgs(
+                max_vlan=399,
+                min_vlan=300,
+            ),
+        ])
+        ```
         """
         return pulumi.get(self, "vlan_ranges")
 
     @vlan_ranges.setter
     def vlan_ranges(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['DistributedVirtualSwitchVlanRangeArgs']]]]):
         pulumi.set(self, "vlan_ranges", value)
 
@@ -3446,20 +3542,26 @@
         :param pulumi.Input[int] backupnfc_share_count: The amount of shares to allocate to the backupNfc traffic class for a custom share level.
         :param pulumi.Input[str] backupnfc_share_level: The allocation level for the backupNfc traffic class. Can be one of high, low, normal, or custom.
         :param pulumi.Input[bool] block_all_ports: Shuts down all ports in the port groups that
                this policy applies to, effectively blocking all network access to connected
                virtual devices.
         :param pulumi.Input[bool] check_beacon: Enables beacon probing as an additional measure
                to detect NIC failure.
+               
+               > **NOTE:** VMware recommends using a minimum of 3 NICs when using beacon
+               probing.
         :param pulumi.Input[str] contact_detail: The detailed contact information for the person
                who is responsible for the VDS.
         :param pulumi.Input[str] contact_name: The name of the person who is responsible for the
                VDS.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to attribute
                value strings to set for VDS.
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi host connections
+               and requires vCenter Server.
         :param pulumi.Input[str] datacenter_id: The ID of the datacenter where the VDS will be
                created. Forces a new resource if changed.
         :param pulumi.Input[str] description: A detailed description for the VDS.
         :param pulumi.Input[bool] directpath_gen2_allowed: Allow VMDirectPath Gen2 for the ports
                for which this policy applies to.
         :param pulumi.Input[int] egress_shaping_average_bandwidth: The average bandwidth in bits
                per second if egress traffic shaping is enabled on the port.
@@ -3554,14 +3656,16 @@
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DistributedVirtualSwitchPvlanMappingArgs']]]] pvlan_mappings: Use the `pvlan_mapping` block to declare a
                private VLAN mapping. The options are:
         :param pulumi.Input[Sequence[pulumi.Input[str]]] standby_uplinks: A list of standby uplinks to be used in
                failover. These uplinks need to match the definitions in the
                `uplinks` VDS argument. See
                here for more details.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource.
+               
+               > **NOTE:** Tagging support requires vCenter Server 6.0 or higher.
         :param pulumi.Input[str] teaming_policy: The uplink teaming policy. Can be one of
                `loadbalance_ip`, `loadbalance_srcmac`, `loadbalance_srcid`,
                `failover_explicit`, or `loadbalance_loadbased`.
         :param pulumi.Input[bool] tx_uplink: Forward all traffic transmitted by ports for which
                this policy applies to its VDS uplinks.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] uplinks: A list of strings that uniquely identifies the names
                of the uplinks on the VDS across hosts. The number of items in this list
@@ -3580,14 +3684,30 @@
         :param pulumi.Input[int] virtualmachine_share_count: The amount of shares to allocate to the virtualMachine traffic class for a custom share level.
         :param pulumi.Input[str] virtualmachine_share_level: The allocation level for the virtualMachine traffic class. Can be one of high, low, normal, or custom.
         :param pulumi.Input[int] vlan_id: The VLAN ID for single VLAN mode. 0 denotes no VLAN.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DistributedVirtualSwitchVlanRangeArgs']]]] vlan_ranges: Used to denote VLAN trunking. Use the `min_vlan`
                and `max_vlan` sub-arguments to define the tagged VLAN range. Multiple
                `vlan_range` definitions are allowed, but they must not overlap. Example
                below:
+               
+               ```python
+               import pulumi
+               import pulumi_vsphere as vsphere
+               
+               vds = vsphere.DistributedVirtualSwitch("vds", vlan_ranges=[
+                   vsphere.DistributedVirtualSwitchVlanRangeArgs(
+                       max_vlan=199,
+                       min_vlan=100,
+                   ),
+                   vsphere.DistributedVirtualSwitchVlanRangeArgs(
+                       max_vlan=399,
+                       min_vlan=300,
+                   ),
+               ])
+               ```
         :param pulumi.Input[int] vmotion_maximum_mbit: The maximum allowed usage for the vmotion traffic class, in Mbits/sec.
         :param pulumi.Input[int] vmotion_reservation_mbit: The amount of guaranteed bandwidth for the vmotion traffic class, in Mbits/sec.
         :param pulumi.Input[int] vmotion_share_count: The amount of shares to allocate to the vmotion traffic class for a custom share level.
         :param pulumi.Input[str] vmotion_share_level: The allocation level for the vmotion traffic class. Can be one of high, low, normal, or custom.
         :param pulumi.Input[int] vsan_maximum_mbit: The maximum allowed usage for the vsan traffic class, in Mbits/sec.
         :param pulumi.Input[int] vsan_reservation_mbit: The amount of guaranteed bandwidth for the vsan traffic class, in Mbits/sec.
         :param pulumi.Input[int] vsan_share_count: The amount of shares to allocate to the vsan traffic class for a custom share level.
@@ -3944,22 +4064,28 @@
         :param pulumi.Input[int] backupnfc_share_count: The amount of shares to allocate to the backupNfc traffic class for a custom share level.
         :param pulumi.Input[str] backupnfc_share_level: The allocation level for the backupNfc traffic class. Can be one of high, low, normal, or custom.
         :param pulumi.Input[bool] block_all_ports: Shuts down all ports in the port groups that
                this policy applies to, effectively blocking all network access to connected
                virtual devices.
         :param pulumi.Input[bool] check_beacon: Enables beacon probing as an additional measure
                to detect NIC failure.
+               
+               > **NOTE:** VMware recommends using a minimum of 3 NICs when using beacon
+               probing.
         :param pulumi.Input[str] config_version: The current version of the VDS configuration, incremented
                by subsequent updates to the VDS.
         :param pulumi.Input[str] contact_detail: The detailed contact information for the person
                who is responsible for the VDS.
         :param pulumi.Input[str] contact_name: The name of the person who is responsible for the
                VDS.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to attribute
                value strings to set for VDS.
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi host connections
+               and requires vCenter Server.
         :param pulumi.Input[str] datacenter_id: The ID of the datacenter where the VDS will be
                created. Forces a new resource if changed.
         :param pulumi.Input[str] description: A detailed description for the VDS.
         :param pulumi.Input[bool] directpath_gen2_allowed: Allow VMDirectPath Gen2 for the ports
                for which this policy applies to.
         :param pulumi.Input[int] egress_shaping_average_bandwidth: The average bandwidth in bits
                per second if egress traffic shaping is enabled on the port.
@@ -4054,14 +4180,16 @@
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DistributedVirtualSwitchPvlanMappingArgs']]]] pvlan_mappings: Use the `pvlan_mapping` block to declare a
                private VLAN mapping. The options are:
         :param pulumi.Input[Sequence[pulumi.Input[str]]] standby_uplinks: A list of standby uplinks to be used in
                failover. These uplinks need to match the definitions in the
                `uplinks` VDS argument. See
                here for more details.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource.
+               
+               > **NOTE:** Tagging support requires vCenter Server 6.0 or higher.
         :param pulumi.Input[str] teaming_policy: The uplink teaming policy. Can be one of
                `loadbalance_ip`, `loadbalance_srcmac`, `loadbalance_srcid`,
                `failover_explicit`, or `loadbalance_loadbased`.
         :param pulumi.Input[bool] tx_uplink: Forward all traffic transmitted by ports for which
                this policy applies to its VDS uplinks.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] uplinks: A list of strings that uniquely identifies the names
                of the uplinks on the VDS across hosts. The number of items in this list
@@ -4080,14 +4208,30 @@
         :param pulumi.Input[int] virtualmachine_share_count: The amount of shares to allocate to the virtualMachine traffic class for a custom share level.
         :param pulumi.Input[str] virtualmachine_share_level: The allocation level for the virtualMachine traffic class. Can be one of high, low, normal, or custom.
         :param pulumi.Input[int] vlan_id: The VLAN ID for single VLAN mode. 0 denotes no VLAN.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DistributedVirtualSwitchVlanRangeArgs']]]] vlan_ranges: Used to denote VLAN trunking. Use the `min_vlan`
                and `max_vlan` sub-arguments to define the tagged VLAN range. Multiple
                `vlan_range` definitions are allowed, but they must not overlap. Example
                below:
+               
+               ```python
+               import pulumi
+               import pulumi_vsphere as vsphere
+               
+               vds = vsphere.DistributedVirtualSwitch("vds", vlan_ranges=[
+                   vsphere.DistributedVirtualSwitchVlanRangeArgs(
+                       max_vlan=199,
+                       min_vlan=100,
+                   ),
+                   vsphere.DistributedVirtualSwitchVlanRangeArgs(
+                       max_vlan=399,
+                       min_vlan=300,
+                   ),
+               ])
+               ```
         :param pulumi.Input[int] vmotion_maximum_mbit: The maximum allowed usage for the vmotion traffic class, in Mbits/sec.
         :param pulumi.Input[int] vmotion_reservation_mbit: The amount of guaranteed bandwidth for the vmotion traffic class, in Mbits/sec.
         :param pulumi.Input[int] vmotion_share_count: The amount of shares to allocate to the vmotion traffic class for a custom share level.
         :param pulumi.Input[str] vmotion_share_level: The allocation level for the vmotion traffic class. Can be one of high, low, normal, or custom.
         :param pulumi.Input[int] vsan_maximum_mbit: The maximum allowed usage for the vsan traffic class, in Mbits/sec.
         :param pulumi.Input[int] vsan_reservation_mbit: The amount of guaranteed bandwidth for the vsan traffic class, in Mbits/sec.
         :param pulumi.Input[int] vsan_share_count: The amount of shares to allocate to the vsan traffic class for a custom share level.
@@ -4277,14 +4421,17 @@
 
     @property
     @pulumi.getter(name="checkBeacon")
     def check_beacon(self) -> pulumi.Output[bool]:
         """
         Enables beacon probing as an additional measure
         to detect NIC failure.
+
+        > **NOTE:** VMware recommends using a minimum of 3 NICs when using beacon
+        probing.
         """
         return pulumi.get(self, "check_beacon")
 
     @property
     @pulumi.getter(name="configVersion")
     def config_version(self) -> pulumi.Output[str]:
         """
@@ -4313,14 +4460,17 @@
 
     @property
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
         Map of custom attribute ids to attribute
         value strings to set for VDS.
+
+        > **NOTE:** Custom attributes are unsupported on direct ESXi host connections
+        and requires vCenter Server.
         """
         return pulumi.get(self, "custom_attributes")
 
     @property
     @pulumi.getter(name="datacenterId")
     def datacenter_id(self) -> pulumi.Output[str]:
         """
@@ -4828,14 +4978,16 @@
         return pulumi.get(self, "standby_uplinks")
 
     @property
     @pulumi.getter
     def tags(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         The IDs of any tags to attach to this resource.
+
+        > **NOTE:** Tagging support requires vCenter Server 6.0 or higher.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="teamingPolicy")
     def teaming_policy(self) -> pulumi.Output[str]:
         """
@@ -4952,14 +5104,30 @@
     @pulumi.getter(name="vlanRanges")
     def vlan_ranges(self) -> pulumi.Output[Sequence['outputs.DistributedVirtualSwitchVlanRange']]:
         """
         Used to denote VLAN trunking. Use the `min_vlan`
         and `max_vlan` sub-arguments to define the tagged VLAN range. Multiple
         `vlan_range` definitions are allowed, but they must not overlap. Example
         below:
+
+        ```python
+        import pulumi
+        import pulumi_vsphere as vsphere
+
+        vds = vsphere.DistributedVirtualSwitch("vds", vlan_ranges=[
+            vsphere.DistributedVirtualSwitchVlanRangeArgs(
+                max_vlan=199,
+                min_vlan=100,
+            ),
+            vsphere.DistributedVirtualSwitchVlanRangeArgs(
+                max_vlan=399,
+                min_vlan=300,
+            ),
+        ])
+        ```
         """
         return pulumi.get(self, "vlan_ranges")
 
     @property
     @pulumi.getter(name="vmotionMaximumMbit")
     def vmotion_maximum_mbit(self) -> pulumi.Output[int]:
         """
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/dpm_host_override.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/dpm_host_override.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,18 @@
         :param pulumi.Input[str] compute_cluster_id: The managed object reference
                ID of the cluster to put the override in.  Forces a new
                resource if changed.
         :param pulumi.Input[str] host_system_id: The managed object ID of the host.
         :param pulumi.Input[str] dpm_automation_level: The automation level for host power
                operations on this host. Can be one of `manual` or `automated`. Default:
                `manual`.
+               
+               > **NOTE:** Using this resource _always_ implies an override, even if one of
+               `dpm_enabled` or `dpm_automation_level` is omitted. Take note of the defaults
+               for both options.
         :param pulumi.Input[bool] dpm_enabled: Enable DPM support for this host. Default:
                `false`.
         """
         pulumi.set(__self__, "compute_cluster_id", compute_cluster_id)
         pulumi.set(__self__, "host_system_id", host_system_id)
         if dpm_automation_level is not None:
             pulumi.set(__self__, "dpm_automation_level", dpm_automation_level)
@@ -66,14 +70,18 @@
     @property
     @pulumi.getter(name="dpmAutomationLevel")
     def dpm_automation_level(self) -> Optional[pulumi.Input[str]]:
         """
         The automation level for host power
         operations on this host. Can be one of `manual` or `automated`. Default:
         `manual`.
+
+        > **NOTE:** Using this resource _always_ implies an override, even if one of
+        `dpm_enabled` or `dpm_automation_level` is omitted. Take note of the defaults
+        for both options.
         """
         return pulumi.get(self, "dpm_automation_level")
 
     @dpm_automation_level.setter
     def dpm_automation_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "dpm_automation_level", value)
 
@@ -102,14 +110,18 @@
         Input properties used for looking up and filtering DpmHostOverride resources.
         :param pulumi.Input[str] compute_cluster_id: The managed object reference
                ID of the cluster to put the override in.  Forces a new
                resource if changed.
         :param pulumi.Input[str] dpm_automation_level: The automation level for host power
                operations on this host. Can be one of `manual` or `automated`. Default:
                `manual`.
+               
+               > **NOTE:** Using this resource _always_ implies an override, even if one of
+               `dpm_enabled` or `dpm_automation_level` is omitted. Take note of the defaults
+               for both options.
         :param pulumi.Input[bool] dpm_enabled: Enable DPM support for this host. Default:
                `false`.
         :param pulumi.Input[str] host_system_id: The managed object ID of the host.
         """
         if compute_cluster_id is not None:
             pulumi.set(__self__, "compute_cluster_id", compute_cluster_id)
         if dpm_automation_level is not None:
@@ -136,14 +148,18 @@
     @property
     @pulumi.getter(name="dpmAutomationLevel")
     def dpm_automation_level(self) -> Optional[pulumi.Input[str]]:
         """
         The automation level for host power
         operations on this host. Can be one of `manual` or `automated`. Default:
         `manual`.
+
+        > **NOTE:** Using this resource _always_ implies an override, even if one of
+        `dpm_enabled` or `dpm_automation_level` is omitted. Take note of the defaults
+        for both options.
         """
         return pulumi.get(self, "dpm_automation_level")
 
     @dpm_automation_level.setter
     def dpm_automation_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "dpm_automation_level", value)
 
@@ -189,14 +205,18 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] compute_cluster_id: The managed object reference
                ID of the cluster to put the override in.  Forces a new
                resource if changed.
         :param pulumi.Input[str] dpm_automation_level: The automation level for host power
                operations on this host. Can be one of `manual` or `automated`. Default:
                `manual`.
+               
+               > **NOTE:** Using this resource _always_ implies an override, even if one of
+               `dpm_enabled` or `dpm_automation_level` is omitted. Take note of the defaults
+               for both options.
         :param pulumi.Input[bool] dpm_enabled: Enable DPM support for this host. Default:
                `false`.
         :param pulumi.Input[str] host_system_id: The managed object ID of the host.
         """
         ...
     @overload
     def __init__(__self__,
@@ -264,14 +284,18 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] compute_cluster_id: The managed object reference
                ID of the cluster to put the override in.  Forces a new
                resource if changed.
         :param pulumi.Input[str] dpm_automation_level: The automation level for host power
                operations on this host. Can be one of `manual` or `automated`. Default:
                `manual`.
+               
+               > **NOTE:** Using this resource _always_ implies an override, even if one of
+               `dpm_enabled` or `dpm_automation_level` is omitted. Take note of the defaults
+               for both options.
         :param pulumi.Input[bool] dpm_enabled: Enable DPM support for this host. Default:
                `false`.
         :param pulumi.Input[str] host_system_id: The managed object ID of the host.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _DpmHostOverrideState.__new__(_DpmHostOverrideState)
@@ -295,14 +319,18 @@
     @property
     @pulumi.getter(name="dpmAutomationLevel")
     def dpm_automation_level(self) -> pulumi.Output[Optional[str]]:
         """
         The automation level for host power
         operations on this host. Can be one of `manual` or `automated`. Default:
         `manual`.
+
+        > **NOTE:** Using this resource _always_ implies an override, even if one of
+        `dpm_enabled` or `dpm_automation_level` is omitted. Take note of the defaults
+        for both options.
         """
         return pulumi.get(self, "dpm_automation_level")
 
     @property
     @pulumi.getter(name="dpmEnabled")
     def dpm_enabled(self) -> pulumi.Output[Optional[bool]]:
         """
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/drs_vm_override.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/drs_vm_override.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,18 @@
                ID of the cluster to put the override in.  Forces a new
                resource if changed.
         :param pulumi.Input[str] virtual_machine_id: The UUID of the virtual machine to create
                the override for.  Forces a new resource if changed.
         :param pulumi.Input[str] drs_automation_level: Overrides the automation level for this virtual
                machine in the cluster. Can be one of `manual`, `partiallyAutomated`, or
                `fullyAutomated`. Default: `manual`.
+               
+               > **NOTE:** Using this resource _always_ implies an override, even if one of
+               `drs_enabled` or `drs_automation_level` is omitted. Take note of the defaults
+               for both options.
         :param pulumi.Input[bool] drs_enabled: Overrides the default DRS setting for this virtual
                machine. Can be either `true` or `false`. Default: `false`.
         """
         pulumi.set(__self__, "compute_cluster_id", compute_cluster_id)
         pulumi.set(__self__, "virtual_machine_id", virtual_machine_id)
         if drs_automation_level is not None:
             pulumi.set(__self__, "drs_automation_level", drs_automation_level)
@@ -68,14 +72,18 @@
     @property
     @pulumi.getter(name="drsAutomationLevel")
     def drs_automation_level(self) -> Optional[pulumi.Input[str]]:
         """
         Overrides the automation level for this virtual
         machine in the cluster. Can be one of `manual`, `partiallyAutomated`, or
         `fullyAutomated`. Default: `manual`.
+
+        > **NOTE:** Using this resource _always_ implies an override, even if one of
+        `drs_enabled` or `drs_automation_level` is omitted. Take note of the defaults
+        for both options.
         """
         return pulumi.get(self, "drs_automation_level")
 
     @drs_automation_level.setter
     def drs_automation_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "drs_automation_level", value)
 
@@ -104,14 +112,18 @@
         Input properties used for looking up and filtering DrsVmOverride resources.
         :param pulumi.Input[str] compute_cluster_id: The managed object reference
                ID of the cluster to put the override in.  Forces a new
                resource if changed.
         :param pulumi.Input[str] drs_automation_level: Overrides the automation level for this virtual
                machine in the cluster. Can be one of `manual`, `partiallyAutomated`, or
                `fullyAutomated`. Default: `manual`.
+               
+               > **NOTE:** Using this resource _always_ implies an override, even if one of
+               `drs_enabled` or `drs_automation_level` is omitted. Take note of the defaults
+               for both options.
         :param pulumi.Input[bool] drs_enabled: Overrides the default DRS setting for this virtual
                machine. Can be either `true` or `false`. Default: `false`.
         :param pulumi.Input[str] virtual_machine_id: The UUID of the virtual machine to create
                the override for.  Forces a new resource if changed.
         """
         if compute_cluster_id is not None:
             pulumi.set(__self__, "compute_cluster_id", compute_cluster_id)
@@ -139,14 +151,18 @@
     @property
     @pulumi.getter(name="drsAutomationLevel")
     def drs_automation_level(self) -> Optional[pulumi.Input[str]]:
         """
         Overrides the automation level for this virtual
         machine in the cluster. Can be one of `manual`, `partiallyAutomated`, or
         `fullyAutomated`. Default: `manual`.
+
+        > **NOTE:** Using this resource _always_ implies an override, even if one of
+        `drs_enabled` or `drs_automation_level` is omitted. Take note of the defaults
+        for both options.
         """
         return pulumi.get(self, "drs_automation_level")
 
     @drs_automation_level.setter
     def drs_automation_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "drs_automation_level", value)
 
@@ -193,14 +209,18 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] compute_cluster_id: The managed object reference
                ID of the cluster to put the override in.  Forces a new
                resource if changed.
         :param pulumi.Input[str] drs_automation_level: Overrides the automation level for this virtual
                machine in the cluster. Can be one of `manual`, `partiallyAutomated`, or
                `fullyAutomated`. Default: `manual`.
+               
+               > **NOTE:** Using this resource _always_ implies an override, even if one of
+               `drs_enabled` or `drs_automation_level` is omitted. Take note of the defaults
+               for both options.
         :param pulumi.Input[bool] drs_enabled: Overrides the default DRS setting for this virtual
                machine. Can be either `true` or `false`. Default: `false`.
         :param pulumi.Input[str] virtual_machine_id: The UUID of the virtual machine to create
                the override for.  Forces a new resource if changed.
         """
         ...
     @overload
@@ -269,14 +289,18 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] compute_cluster_id: The managed object reference
                ID of the cluster to put the override in.  Forces a new
                resource if changed.
         :param pulumi.Input[str] drs_automation_level: Overrides the automation level for this virtual
                machine in the cluster. Can be one of `manual`, `partiallyAutomated`, or
                `fullyAutomated`. Default: `manual`.
+               
+               > **NOTE:** Using this resource _always_ implies an override, even if one of
+               `drs_enabled` or `drs_automation_level` is omitted. Take note of the defaults
+               for both options.
         :param pulumi.Input[bool] drs_enabled: Overrides the default DRS setting for this virtual
                machine. Can be either `true` or `false`. Default: `false`.
         :param pulumi.Input[str] virtual_machine_id: The UUID of the virtual machine to create
                the override for.  Forces a new resource if changed.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
@@ -301,14 +325,18 @@
     @property
     @pulumi.getter(name="drsAutomationLevel")
     def drs_automation_level(self) -> pulumi.Output[Optional[str]]:
         """
         Overrides the automation level for this virtual
         machine in the cluster. Can be one of `manual`, `partiallyAutomated`, or
         `fullyAutomated`. Default: `manual`.
+
+        > **NOTE:** Using this resource _always_ implies an override, even if one of
+        `drs_enabled` or `drs_automation_level` is omitted. Take note of the defaults
+        for both options.
         """
         return pulumi.get(self, "drs_automation_level")
 
     @property
     @pulumi.getter(name="drsEnabled")
     def drs_enabled(self) -> pulumi.Output[Optional[bool]]:
         """
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/entity_permissions.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/entity_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/file.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/file.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,18 @@
         The set of arguments for constructing a File resource.
         :param pulumi.Input[str] datastore: The name of the datastore to which to upload the
                file.
         :param pulumi.Input[str] destination_file: The path to where the file should be uploaded
                or copied to on the destination `datastore` in vSphere.
         :param pulumi.Input[bool] create_directories: Create directories in `destination_file`
                path parameter on first apply if any are missing for copy operation.
+               
+               > **NOTE:** Any directory created as part of the `create_directories` argument
+               will not be deleted when the resource is destroyed. New directories are not
+               created if the `destination_file` path is changed in subsequent applies.
         :param pulumi.Input[str] datacenter: The name of a datacenter to which the file will be
                uploaded.
         :param pulumi.Input[str] source_datacenter: The name of a datacenter from which the file
                will be copied. Forces a new resource if changed.
         :param pulumi.Input[str] source_datastore: The name of the datastore from which file will
                be copied. Forces a new resource if changed.
         """
@@ -85,14 +89,18 @@
 
     @property
     @pulumi.getter(name="createDirectories")
     def create_directories(self) -> Optional[pulumi.Input[bool]]:
         """
         Create directories in `destination_file`
         path parameter on first apply if any are missing for copy operation.
+
+        > **NOTE:** Any directory created as part of the `create_directories` argument
+        will not be deleted when the resource is destroyed. New directories are not
+        created if the `destination_file` path is changed in subsequent applies.
         """
         return pulumi.get(self, "create_directories")
 
     @create_directories.setter
     def create_directories(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "create_directories", value)
 
@@ -146,14 +154,18 @@
                  source_datacenter: Optional[pulumi.Input[str]] = None,
                  source_datastore: Optional[pulumi.Input[str]] = None,
                  source_file: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering File resources.
         :param pulumi.Input[bool] create_directories: Create directories in `destination_file`
                path parameter on first apply if any are missing for copy operation.
+               
+               > **NOTE:** Any directory created as part of the `create_directories` argument
+               will not be deleted when the resource is destroyed. New directories are not
+               created if the `destination_file` path is changed in subsequent applies.
         :param pulumi.Input[str] datacenter: The name of a datacenter to which the file will be
                uploaded.
         :param pulumi.Input[str] datastore: The name of the datastore to which to upload the
                file.
         :param pulumi.Input[str] destination_file: The path to where the file should be uploaded
                or copied to on the destination `datastore` in vSphere.
         :param pulumi.Input[str] source_datacenter: The name of a datacenter from which the file
@@ -178,14 +190,18 @@
 
     @property
     @pulumi.getter(name="createDirectories")
     def create_directories(self) -> Optional[pulumi.Input[bool]]:
         """
         Create directories in `destination_file`
         path parameter on first apply if any are missing for copy operation.
+
+        > **NOTE:** Any directory created as part of the `create_directories` argument
+        will not be deleted when the resource is destroyed. New directories are not
+        created if the `destination_file` path is changed in subsequent applies.
         """
         return pulumi.get(self, "create_directories")
 
     @create_directories.setter
     def create_directories(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "create_directories", value)
 
@@ -308,14 +324,18 @@
             source_file="/my/src/path/custom_ubuntu.vmdk")
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] create_directories: Create directories in `destination_file`
                path parameter on first apply if any are missing for copy operation.
+               
+               > **NOTE:** Any directory created as part of the `create_directories` argument
+               will not be deleted when the resource is destroyed. New directories are not
+               created if the `destination_file` path is changed in subsequent applies.
         :param pulumi.Input[str] datacenter: The name of a datacenter to which the file will be
                uploaded.
         :param pulumi.Input[str] datastore: The name of the datastore to which to upload the
                file.
         :param pulumi.Input[str] destination_file: The path to where the file should be uploaded
                or copied to on the destination `datastore` in vSphere.
         :param pulumi.Input[str] source_datacenter: The name of a datacenter from which the file
@@ -426,14 +446,18 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] create_directories: Create directories in `destination_file`
                path parameter on first apply if any are missing for copy operation.
+               
+               > **NOTE:** Any directory created as part of the `create_directories` argument
+               will not be deleted when the resource is destroyed. New directories are not
+               created if the `destination_file` path is changed in subsequent applies.
         :param pulumi.Input[str] datacenter: The name of a datacenter to which the file will be
                uploaded.
         :param pulumi.Input[str] datastore: The name of the datastore to which to upload the
                file.
         :param pulumi.Input[str] destination_file: The path to where the file should be uploaded
                or copied to on the destination `datastore` in vSphere.
         :param pulumi.Input[str] source_datacenter: The name of a datacenter from which the file
@@ -456,14 +480,18 @@
 
     @property
     @pulumi.getter(name="createDirectories")
     def create_directories(self) -> pulumi.Output[Optional[bool]]:
         """
         Create directories in `destination_file`
         path parameter on first apply if any are missing for copy operation.
+
+        > **NOTE:** Any directory created as part of the `create_directories` argument
+        will not be deleted when the resource is destroyed. New directories are not
+        created if the `destination_file` path is changed in subsequent applies.
         """
         return pulumi.get(self, "create_directories")
 
     @property
     @pulumi.getter
     def datacenter(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/folder.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/folder.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,25 +23,38 @@
         The set of arguments for constructing a Folder resource.
         :param pulumi.Input[str] path: The path of the folder to be created. This is relative to
                the root of the type of folder you are creating, and the supplied datacenter.
                For example, given a default datacenter of `default-dc`, a folder of type
                `vm` (denoting a virtual machine folder), and a supplied folder of
                `test-folder`, the resulting path would be
                `/default-dc/vm/test-folder`.
+               
+               > **NOTE:** `path` can be modified - the resulting behavior is dependent on
+               what section of `path` you are modifying. If you are modifying the parent (so
+               any part before the last `/`), your folder will be moved to that new parent. If
+               modifying the name (the part after the last `/`), your folder will be renamed.
         :param pulumi.Input[str] type: The type of folder to create. Allowed options are
                `datacenter` for datacenter folders, `host` for host and cluster folders,
                `vm` for virtual machine folders, `datastore` for datastore folders, and
                `network` for network folders. Forces a new resource if changed.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to attribute 
                value strings to set for folder. See [here][docs-setting-custom-attributes]
                for a reference on how to set values for custom attributes.
+               
+               [docs-setting-custom-attributes]: /docs/providers/vsphere/r/custom_attribute.html#using-custom-attributes-in-a-supported-resource
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+               and require vCenter.
         :param pulumi.Input[str] datacenter_id: The ID of the datacenter the folder will be created in.
                Required for all folder types except for datacenter folders. Forces a new
                resource if changed.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource.
+               
+               > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+               requires vCenter 6.0 or higher.
         """
         pulumi.set(__self__, "path", path)
         pulumi.set(__self__, "type", type)
         if custom_attributes is not None:
             pulumi.set(__self__, "custom_attributes", custom_attributes)
         if datacenter_id is not None:
             pulumi.set(__self__, "datacenter_id", datacenter_id)
@@ -54,14 +67,19 @@
         """
         The path of the folder to be created. This is relative to
         the root of the type of folder you are creating, and the supplied datacenter.
         For example, given a default datacenter of `default-dc`, a folder of type
         `vm` (denoting a virtual machine folder), and a supplied folder of
         `test-folder`, the resulting path would be
         `/default-dc/vm/test-folder`.
+
+        > **NOTE:** `path` can be modified - the resulting behavior is dependent on
+        what section of `path` you are modifying. If you are modifying the parent (so
+        any part before the last `/`), your folder will be moved to that new parent. If
+        modifying the name (the part after the last `/`), your folder will be renamed.
         """
         return pulumi.get(self, "path")
 
     @path.setter
     def path(self, value: pulumi.Input[str]):
         pulumi.set(self, "path", value)
 
@@ -83,14 +101,19 @@
     @property
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Map of custom attribute ids to attribute 
         value strings to set for folder. See [here][docs-setting-custom-attributes]
         for a reference on how to set values for custom attributes.
+
+        [docs-setting-custom-attributes]: /docs/providers/vsphere/r/custom_attribute.html#using-custom-attributes-in-a-supported-resource
+
+        > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+        and require vCenter.
         """
         return pulumi.get(self, "custom_attributes")
 
     @custom_attributes.setter
     def custom_attributes(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "custom_attributes", value)
 
@@ -109,14 +132,17 @@
         pulumi.set(self, "datacenter_id", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The IDs of any tags to attach to this resource.
+
+        > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+        requires vCenter 6.0 or higher.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -130,24 +156,37 @@
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  type: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Folder resources.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to attribute 
                value strings to set for folder. See [here][docs-setting-custom-attributes]
                for a reference on how to set values for custom attributes.
+               
+               [docs-setting-custom-attributes]: /docs/providers/vsphere/r/custom_attribute.html#using-custom-attributes-in-a-supported-resource
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+               and require vCenter.
         :param pulumi.Input[str] datacenter_id: The ID of the datacenter the folder will be created in.
                Required for all folder types except for datacenter folders. Forces a new
                resource if changed.
         :param pulumi.Input[str] path: The path of the folder to be created. This is relative to
                the root of the type of folder you are creating, and the supplied datacenter.
                For example, given a default datacenter of `default-dc`, a folder of type
                `vm` (denoting a virtual machine folder), and a supplied folder of
                `test-folder`, the resulting path would be
                `/default-dc/vm/test-folder`.
+               
+               > **NOTE:** `path` can be modified - the resulting behavior is dependent on
+               what section of `path` you are modifying. If you are modifying the parent (so
+               any part before the last `/`), your folder will be moved to that new parent. If
+               modifying the name (the part after the last `/`), your folder will be renamed.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource.
+               
+               > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+               requires vCenter 6.0 or higher.
         :param pulumi.Input[str] type: The type of folder to create. Allowed options are
                `datacenter` for datacenter folders, `host` for host and cluster folders,
                `vm` for virtual machine folders, `datastore` for datastore folders, and
                `network` for network folders. Forces a new resource if changed.
         """
         if custom_attributes is not None:
             pulumi.set(__self__, "custom_attributes", custom_attributes)
@@ -163,14 +202,19 @@
     @property
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Map of custom attribute ids to attribute 
         value strings to set for folder. See [here][docs-setting-custom-attributes]
         for a reference on how to set values for custom attributes.
+
+        [docs-setting-custom-attributes]: /docs/providers/vsphere/r/custom_attribute.html#using-custom-attributes-in-a-supported-resource
+
+        > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+        and require vCenter.
         """
         return pulumi.get(self, "custom_attributes")
 
     @custom_attributes.setter
     def custom_attributes(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "custom_attributes", value)
 
@@ -194,26 +238,34 @@
         """
         The path of the folder to be created. This is relative to
         the root of the type of folder you are creating, and the supplied datacenter.
         For example, given a default datacenter of `default-dc`, a folder of type
         `vm` (denoting a virtual machine folder), and a supplied folder of
         `test-folder`, the resulting path would be
         `/default-dc/vm/test-folder`.
+
+        > **NOTE:** `path` can be modified - the resulting behavior is dependent on
+        what section of `path` you are modifying. If you are modifying the parent (so
+        any part before the last `/`), your folder will be moved to that new parent. If
+        modifying the name (the part after the last `/`), your folder will be renamed.
         """
         return pulumi.get(self, "path")
 
     @path.setter
     def path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "path", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The IDs of any tags to attach to this resource.
+
+        > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+        requires vCenter 6.0 or higher.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -247,24 +299,37 @@
         """
         Create a Folder resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to attribute 
                value strings to set for folder. See [here][docs-setting-custom-attributes]
                for a reference on how to set values for custom attributes.
+               
+               [docs-setting-custom-attributes]: /docs/providers/vsphere/r/custom_attribute.html#using-custom-attributes-in-a-supported-resource
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+               and require vCenter.
         :param pulumi.Input[str] datacenter_id: The ID of the datacenter the folder will be created in.
                Required for all folder types except for datacenter folders. Forces a new
                resource if changed.
         :param pulumi.Input[str] path: The path of the folder to be created. This is relative to
                the root of the type of folder you are creating, and the supplied datacenter.
                For example, given a default datacenter of `default-dc`, a folder of type
                `vm` (denoting a virtual machine folder), and a supplied folder of
                `test-folder`, the resulting path would be
                `/default-dc/vm/test-folder`.
+               
+               > **NOTE:** `path` can be modified - the resulting behavior is dependent on
+               what section of `path` you are modifying. If you are modifying the parent (so
+               any part before the last `/`), your folder will be moved to that new parent. If
+               modifying the name (the part after the last `/`), your folder will be renamed.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource.
+               
+               > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+               requires vCenter 6.0 or higher.
         :param pulumi.Input[str] type: The type of folder to create. Allowed options are
                `datacenter` for datacenter folders, `host` for host and cluster folders,
                `vm` for virtual machine folders, `datastore` for datastore folders, and
                `network` for network folders. Forces a new resource if changed.
         """
         ...
     @overload
@@ -333,24 +398,37 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to attribute 
                value strings to set for folder. See [here][docs-setting-custom-attributes]
                for a reference on how to set values for custom attributes.
+               
+               [docs-setting-custom-attributes]: /docs/providers/vsphere/r/custom_attribute.html#using-custom-attributes-in-a-supported-resource
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+               and require vCenter.
         :param pulumi.Input[str] datacenter_id: The ID of the datacenter the folder will be created in.
                Required for all folder types except for datacenter folders. Forces a new
                resource if changed.
         :param pulumi.Input[str] path: The path of the folder to be created. This is relative to
                the root of the type of folder you are creating, and the supplied datacenter.
                For example, given a default datacenter of `default-dc`, a folder of type
                `vm` (denoting a virtual machine folder), and a supplied folder of
                `test-folder`, the resulting path would be
                `/default-dc/vm/test-folder`.
+               
+               > **NOTE:** `path` can be modified - the resulting behavior is dependent on
+               what section of `path` you are modifying. If you are modifying the parent (so
+               any part before the last `/`), your folder will be moved to that new parent. If
+               modifying the name (the part after the last `/`), your folder will be renamed.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource.
+               
+               > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+               requires vCenter 6.0 or higher.
         :param pulumi.Input[str] type: The type of folder to create. Allowed options are
                `datacenter` for datacenter folders, `host` for host and cluster folders,
                `vm` for virtual machine folders, `datastore` for datastore folders, and
                `network` for network folders. Forces a new resource if changed.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
@@ -366,14 +444,19 @@
     @property
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
         Map of custom attribute ids to attribute 
         value strings to set for folder. See [here][docs-setting-custom-attributes]
         for a reference on how to set values for custom attributes.
+
+        [docs-setting-custom-attributes]: /docs/providers/vsphere/r/custom_attribute.html#using-custom-attributes-in-a-supported-resource
+
+        > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+        and require vCenter.
         """
         return pulumi.get(self, "custom_attributes")
 
     @property
     @pulumi.getter(name="datacenterId")
     def datacenter_id(self) -> pulumi.Output[Optional[str]]:
         """
@@ -389,22 +472,30 @@
         """
         The path of the folder to be created. This is relative to
         the root of the type of folder you are creating, and the supplied datacenter.
         For example, given a default datacenter of `default-dc`, a folder of type
         `vm` (denoting a virtual machine folder), and a supplied folder of
         `test-folder`, the resulting path would be
         `/default-dc/vm/test-folder`.
+
+        > **NOTE:** `path` can be modified - the resulting behavior is dependent on
+        what section of `path` you are modifying. If you are modifying the parent (so
+        any part before the last `/`), your folder will be moved to that new parent. If
+        modifying the name (the part after the last `/`), your folder will be renamed.
         """
         return pulumi.get(self, "path")
 
     @property
     @pulumi.getter
     def tags(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         The IDs of any tags to attach to this resource.
+
+        > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+        requires vCenter 6.0 or higher.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_compute_cluster.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_compute_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_compute_cluster_host_group.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_compute_cluster_host_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,28 +85,30 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_vsphere as vsphere
 
-    datacenter = vsphere.get_datacenter(name=var["vsphere_datacenter"])
-    cluster = vsphere.get_compute_cluster(name=var["vsphere_cluster"],
+    datacenter = vsphere.get_datacenter(name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+    cluster = vsphere.get_compute_cluster(name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         datacenter_id=datacenter.id)
     host_group1 = vsphere.get_compute_cluster_host_group(name="host_group1",
         compute_cluster_id=cluster.id)
     host_rule1 = vsphere.ComputeClusterVmHostRule("hostRule1",
         compute_cluster_id=cluster.id,
         vm_group_name="vm_group1",
         affinity_host_group_name=host_group1.name)
     ```
 
 
     :param str compute_cluster_id: The [managed object reference ID][docs-about-morefs]
            of the compute cluster for the host group.
+           
+           [docs-about-morefs]: /docs/providers/vsphere/index.html#use-of-managed-object-references-by-the-vsphere-provider
     :param str name: The name of the host group.
     """
     __args__ = dict()
     __args__['computeClusterId'] = compute_cluster_id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('vsphere:index/getComputeClusterHostGroup:getComputeClusterHostGroup', __args__, opts=opts, typ=GetComputeClusterHostGroupResult).value
@@ -129,24 +131,26 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_vsphere as vsphere
 
-    datacenter = vsphere.get_datacenter(name=var["vsphere_datacenter"])
-    cluster = vsphere.get_compute_cluster(name=var["vsphere_cluster"],
+    datacenter = vsphere.get_datacenter(name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+    cluster = vsphere.get_compute_cluster(name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
         datacenter_id=datacenter.id)
     host_group1 = vsphere.get_compute_cluster_host_group(name="host_group1",
         compute_cluster_id=cluster.id)
     host_rule1 = vsphere.ComputeClusterVmHostRule("hostRule1",
         compute_cluster_id=cluster.id,
         vm_group_name="vm_group1",
         affinity_host_group_name=host_group1.name)
     ```
 
 
     :param str compute_cluster_id: The [managed object reference ID][docs-about-morefs]
            of the compute cluster for the host group.
+           
+           [docs-about-morefs]: /docs/providers/vsphere/index.html#use-of-managed-object-references-by-the-vsphere-provider
     :param str name: The name of the host group.
     """
     ...
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_content_library.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_content_library.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_content_library_item.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_content_library_item.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_custom_attribute.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_datacenter.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_datacenter.py`

 * *Files 11% similar despite different names*

```diff
@@ -69,14 +69,19 @@
 
     datacenter = vsphere.get_datacenter(name="dc-01")
     ```
 
 
     :param str name: The name of the datacenter. This can be a name or path.
            Can be omitted if there is only one datacenter in the inventory.
+           
+           > **NOTE:** When used with an ESXi host, this data source _always_ returns the
+           host's "default" datacenter, which is a special datacenter name unrelated to the
+           datacenters that exist in the vSphere inventory when managed by a vCenter Server
+           instance. Hence, the `name` attribute is completely ignored.
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('vsphere:index/getDatacenter:getDatacenter', __args__, opts=opts, typ=GetDatacenterResult).value
 
     return AwaitableGetDatacenterResult(
@@ -101,9 +106,14 @@
 
     datacenter = vsphere.get_datacenter(name="dc-01")
     ```
 
 
     :param str name: The name of the datacenter. This can be a name or path.
            Can be omitted if there is only one datacenter in the inventory.
+           
+           > **NOTE:** When used with an ESXi host, this data source _always_ returns the
+           host's "default" datacenter, which is a special datacenter name unrelated to the
+           datacenters that exist in the vSphere inventory when managed by a vCenter Server
+           instance. Hence, the `name` attribute is completely ignored.
     """
     ...
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_datastore.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_datastore.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             name=self.name)
 
 
 def get_datastore(datacenter_id: Optional[str] = None,
                   name: Optional[str] = None,
                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDatastoreResult:
     """
-    The _get_datastore_ data source can be used to discover the ID of a
+    The `get_datastore` data source can be used to discover the ID of a
     vSphere datastore object. This can then be used with resources or data sources
     that require a datastore. For example, to create virtual machines in using the
     `VirtualMachine` resource.
 
     ## Example Usage
 
     ```python
@@ -102,15 +102,15 @@
 
 
 @_utilities.lift_output_func(get_datastore)
 def get_datastore_output(datacenter_id: Optional[pulumi.Input[Optional[str]]] = None,
                          name: Optional[pulumi.Input[str]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatastoreResult]:
     """
-    The _get_datastore_ data source can be used to discover the ID of a
+    The `get_datastore` data source can be used to discover the ID of a
     vSphere datastore object. This can then be used with resources or data sources
     that require a datastore. For example, to create virtual machines in using the
     `VirtualMachine` resource.
 
     ## Example Usage
 
     ```python
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_datastore_cluster.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_datastore_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_distributed_virtual_switch.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_distributed_virtual_switch.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_dynamic.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_dynamic.py`

 * *Files 25% similar despite different names*

```diff
@@ -74,29 +74,29 @@
 def get_dynamic(filters: Optional[Sequence[str]] = None,
                 name_regex: Optional[str] = None,
                 type: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDynamicResult:
     """
     [docs-about-morefs]: /docs/providers/vsphere/index.html#use-of-managed-object-references-by-the-vsphere-provider
 
-    The _get_dynamic_ data source can be used to get the [managed object reference ID][docs-about-morefs]
+    The `get_dynamic` data source can be used to get the [managed object reference ID][docs-about-morefs]
     of any tagged managed object in vCenter Server by providing a list of tag IDs
     and an optional regular expression to filter objects by name.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_vsphere as vsphere
 
     category = vsphere.get_tag_category(name="SomeCategory")
     tag1 = vsphere.get_tag(name="FirstTag",
-        category_id=data["vsphere_tag_category"]["cat"]["id"])
+        category_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
     tag2 = vsphere.get_tag(name="SecondTag",
-        category_id=data["vsphere_tag_category"]["cat"]["id"])
+        category_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
     dyn = vsphere.get_dynamic(filters=[
             tag1.id,
             tag1.id,
         ],
         name_regex="ubuntu",
         type="Datacenter")
     ```
@@ -128,29 +128,29 @@
 def get_dynamic_output(filters: Optional[pulumi.Input[Sequence[str]]] = None,
                        name_regex: Optional[pulumi.Input[Optional[str]]] = None,
                        type: Optional[pulumi.Input[Optional[str]]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDynamicResult]:
     """
     [docs-about-morefs]: /docs/providers/vsphere/index.html#use-of-managed-object-references-by-the-vsphere-provider
 
-    The _get_dynamic_ data source can be used to get the [managed object reference ID][docs-about-morefs]
+    The `get_dynamic` data source can be used to get the [managed object reference ID][docs-about-morefs]
     of any tagged managed object in vCenter Server by providing a list of tag IDs
     and an optional regular expression to filter objects by name.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_vsphere as vsphere
 
     category = vsphere.get_tag_category(name="SomeCategory")
     tag1 = vsphere.get_tag(name="FirstTag",
-        category_id=data["vsphere_tag_category"]["cat"]["id"])
+        category_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
     tag2 = vsphere.get_tag(name="SecondTag",
-        category_id=data["vsphere_tag_category"]["cat"]["id"])
+        category_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
     dyn = vsphere.get_dynamic(filters=[
             tag1.id,
             tag1.id,
         ],
         name_regex="ubuntu",
         type="Datacenter")
     ```
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_folder.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_host.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_host.py`

 * *Files 10% similar despite different names*

```diff
@@ -95,14 +95,17 @@
     ```
 
 
     :param str datacenter_id: The managed object reference ID
            of a vSphere datacenter object.
     :param str name: The name of the ESXI host. This can be a name or path.
            Can be omitted if there is only one host in your inventory.
+           
+           > **NOTE:** When used against an ESXi host directly, this data source _always_
+           returns the ESXi host's object ID, regardless of what is entered into `name`.
     """
     __args__ = dict()
     __args__['datacenterId'] = datacenter_id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('vsphere:index/getHost:getHost', __args__, opts=opts, typ=GetHostResult).value
 
@@ -134,9 +137,12 @@
     ```
 
 
     :param str datacenter_id: The managed object reference ID
            of a vSphere datacenter object.
     :param str name: The name of the ESXI host. This can be a name or path.
            Can be omitted if there is only one host in your inventory.
+           
+           > **NOTE:** When used against an ESXi host directly, this data source _always_
+           returns the ESXi host's object ID, regardless of what is entered into `name`.
     """
     ...
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_host_pci_device.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_host_pci_device.py`

 * *Files 8% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
 def get_host_pci_device(class_id: Optional[str] = None,
                         host_id: Optional[str] = None,
                         name_regex: Optional[str] = None,
                         vendor_id: Optional[str] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetHostPciDeviceResult:
     """
-    The _get_host_pci_device_ data source can be used to discover the device ID
+    The `get_host_pci_device` data source can be used to discover the device ID
     of a vSphere host's PCI device. This can then be used with
     `VirtualMachine`'s `pci_device_id`.
 
     ## Example Usage
     ### With Vendor ID And Class ID
 
     ```python
@@ -116,14 +116,18 @@
         class_id="123",
         vendor_id="456")
     ```
     ### With Name Regular Expression
 
 
     :param str class_id: The hexadecimal PCI device class ID
+           
+           [docs-about-morefs]: /docs/providers/vsphere/index.html#use-of-managed-object-references-by-the-vsphere-provider
+           
+           > **NOTE:** `name_regex`, `vendor_id`, and `class_id` can all be used together.
     :param str host_id: The [managed object reference ID][docs-about-morefs] of a host.
     :param str name_regex: A regular expression that will be used to match the
            host PCI device name.
     :param str vendor_id: The hexadecimal PCI device vendor ID.
     """
     __args__ = dict()
     __args__['classId'] = class_id
@@ -145,15 +149,15 @@
 @_utilities.lift_output_func(get_host_pci_device)
 def get_host_pci_device_output(class_id: Optional[pulumi.Input[Optional[str]]] = None,
                                host_id: Optional[pulumi.Input[str]] = None,
                                name_regex: Optional[pulumi.Input[Optional[str]]] = None,
                                vendor_id: Optional[pulumi.Input[Optional[str]]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetHostPciDeviceResult]:
     """
-    The _get_host_pci_device_ data source can be used to discover the device ID
+    The `get_host_pci_device` data source can be used to discover the device ID
     of a vSphere host's PCI device. This can then be used with
     `VirtualMachine`'s `pci_device_id`.
 
     ## Example Usage
     ### With Vendor ID And Class ID
 
     ```python
@@ -167,13 +171,17 @@
         class_id="123",
         vendor_id="456")
     ```
     ### With Name Regular Expression
 
 
     :param str class_id: The hexadecimal PCI device class ID
+           
+           [docs-about-morefs]: /docs/providers/vsphere/index.html#use-of-managed-object-references-by-the-vsphere-provider
+           
+           > **NOTE:** `name_regex`, `vendor_id`, and `class_id` can all be used together.
     :param str host_id: The [managed object reference ID][docs-about-morefs] of a host.
     :param str name_regex: A regular expression that will be used to match the
            host PCI device name.
     :param str vendor_id: The hexadecimal PCI device vendor ID.
     """
     ...
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_host_thumbprint.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_host_thumbprint.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_license.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_license.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_network.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_network.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
 
 def get_network(datacenter_id: Optional[str] = None,
                 distributed_virtual_switch_uuid: Optional[str] = None,
                 name: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetNetworkResult:
     """
-    The _get_network_ data source can be used to discover the ID of a network
+    The `get_network` data source can be used to discover the ID of a network
     in vSphere. This can be any network that can be used as the backing for a
     network interface for `VirtualMachine` or any other vSphere resource
     that requires a network. This includes standard (host-based) port groups,
     distributed port groups, or opaque networks such as those managed by NSX.
 
     ## Example Usage
 
@@ -136,15 +136,15 @@
 
 @_utilities.lift_output_func(get_network)
 def get_network_output(datacenter_id: Optional[pulumi.Input[Optional[str]]] = None,
                        distributed_virtual_switch_uuid: Optional[pulumi.Input[Optional[str]]] = None,
                        name: Optional[pulumi.Input[str]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNetworkResult]:
     """
-    The _get_network_ data source can be used to discover the ID of a network
+    The `get_network` data source can be used to discover the ID of a network
     in vSphere. This can be any network that can be used as the backing for a
     network interface for `VirtualMachine` or any other vSphere resource
     that requires a network. This includes standard (host-based) port groups,
     distributed port groups, or opaque networks such as those managed by NSX.
 
     ## Example Usage
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_ovf_vm_template.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_ovf_vm_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,15 +377,15 @@
                         local_ovf_path: Optional[str] = None,
                         name: Optional[str] = None,
                         ovf_network_map: Optional[Mapping[str, str]] = None,
                         remote_ovf_url: Optional[str] = None,
                         resource_pool_id: Optional[str] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetOvfVmTemplateResult:
     """
-    The _get_ovf_vm_template_ data source can be used to submit an OVF to
+    The `get_ovf_vm_template` data source can be used to submit an OVF to
     vSphere and extract its hardware settings in a form that can be then used as
     inputs for a `VirtualMachine` resource.
 
     ## Remote OVF/OVA Source
 
     data "vsphere_ovf_vm_template" "ovfRemote" {
       name              = "Nested-ESXi-7.0-Terraform-Deploy-1"
@@ -491,14 +491,17 @@
     :param str local_ovf_path: The absolute path to the OVF/OVA file on the
            local system. When deploying from an OVF, ensure all necessary files such as
            the `.vmdk` files are present in the same directory as the OVF.
     :param str name: Name of the virtual machine to create.
     :param Mapping[str, str] ovf_network_map: The mapping of name of network identifiers
            from the OVF descriptor to network UUID in the environment.
     :param str remote_ovf_url: URL of the remote OVF/OVA file to be deployed.
+           
+           > **NOTE:** Either `local_ovf_path` or `remote_ovf_url` is required, both can
+           not be empty.
     :param str resource_pool_id: The ID of a resource pool in which to place
            the virtual machine.
     """
     __args__ = dict()
     __args__['allowUnverifiedSslCert'] = allow_unverified_ssl_cert
     __args__['datastoreId'] = datastore_id
     __args__['deploymentOption'] = deployment_option
@@ -564,15 +567,15 @@
                                local_ovf_path: Optional[pulumi.Input[Optional[str]]] = None,
                                name: Optional[pulumi.Input[str]] = None,
                                ovf_network_map: Optional[pulumi.Input[Optional[Mapping[str, str]]]] = None,
                                remote_ovf_url: Optional[pulumi.Input[Optional[str]]] = None,
                                resource_pool_id: Optional[pulumi.Input[str]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOvfVmTemplateResult]:
     """
-    The _get_ovf_vm_template_ data source can be used to submit an OVF to
+    The `get_ovf_vm_template` data source can be used to submit an OVF to
     vSphere and extract its hardware settings in a form that can be then used as
     inputs for a `VirtualMachine` resource.
 
     ## Remote OVF/OVA Source
 
     data "vsphere_ovf_vm_template" "ovfRemote" {
       name              = "Nested-ESXi-7.0-Terraform-Deploy-1"
@@ -678,11 +681,14 @@
     :param str local_ovf_path: The absolute path to the OVF/OVA file on the
            local system. When deploying from an OVF, ensure all necessary files such as
            the `.vmdk` files are present in the same directory as the OVF.
     :param str name: Name of the virtual machine to create.
     :param Mapping[str, str] ovf_network_map: The mapping of name of network identifiers
            from the OVF descriptor to network UUID in the environment.
     :param str remote_ovf_url: URL of the remote OVF/OVA file to be deployed.
+           
+           > **NOTE:** Either `local_ovf_path` or `remote_ovf_url` is required, both can
+           not be empty.
     :param str resource_pool_id: The ID of a resource pool in which to place
            the virtual machine.
     """
     ...
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_policy.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_policy.py`

 * *Files 15% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             id=self.id,
             name=self.name)
 
 
 def get_policy(name: Optional[str] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPolicyResult:
     """
-    The _get_policy_ data source can be used to discover the UUID of a
+    The `get_policy` data source can be used to discover the UUID of a
     storage policy. This can then be used with other resources or data sources that
     use a storage policy.
 
     > **NOTE:** Storage policies are not supported on direct ESXi hosts and
     requires vCenter Server.
 
     ## Example Usage
@@ -86,15 +86,15 @@
         name=__ret__.name)
 
 
 @_utilities.lift_output_func(get_policy)
 def get_policy_output(name: Optional[pulumi.Input[str]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPolicyResult]:
     """
-    The _get_policy_ data source can be used to discover the UUID of a
+    The `get_policy` data source can be used to discover the UUID of a
     storage policy. This can then be used with other resources or data sources that
     use a storage policy.
 
     > **NOTE:** Storage policies are not supported on direct ESXi hosts and
     requires vCenter Server.
 
     ## Example Usage
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_resource_pool.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_resource_pool.py`

 * *Files 15% similar despite different names*

```diff
@@ -92,27 +92,31 @@
     _root resource pool_ and can be looked up by specifying the path.
 
     ```python
     import pulumi
     import pulumi_vsphere as vsphere
 
     pool = vsphere.get_resource_pool(name="esxi-01.example.com/Resources",
-        datacenter_id=data["vsphere_datacenter"]["datacenter"]["id"])
+        datacenter_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
     ```
 
     For more information on the root resource pool, see [Managing Resource Pools][vmware-docs-resource-pools] in the vSphere documentation.
 
     [vmware-docs-resource-pools]: https://docs.vmware.com/en/VMware-vSphere/7.0/com.vmware.vsphere.resmgmt.doc/GUID-60077B40-66FF-4625-934A-641703ED7601.html
 
 
     :param str datacenter_id: The managed object reference ID
            of the datacenter in which the resource pool is located. This can be omitted
            if the search path used in `name` is an absolute path. For default
            datacenters, use the id attribute from an empty `Datacenter` data
            source.
+           
+           > **Note:** When using ESXi without a vCenter Server instance, you do not
+           need to specify either attribute to use this data source. An empty declaration
+           will load the ESXi host's root resource pool.
     :param str name: The name of the resource pool. This can be a name or
            path. This is required when using vCenter.
     """
     __args__ = dict()
     __args__['datacenterId'] = datacenter_id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -155,24 +159,28 @@
     _root resource pool_ and can be looked up by specifying the path.
 
     ```python
     import pulumi
     import pulumi_vsphere as vsphere
 
     pool = vsphere.get_resource_pool(name="esxi-01.example.com/Resources",
-        datacenter_id=data["vsphere_datacenter"]["datacenter"]["id"])
+        datacenter_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
     ```
 
     For more information on the root resource pool, see [Managing Resource Pools][vmware-docs-resource-pools] in the vSphere documentation.
 
     [vmware-docs-resource-pools]: https://docs.vmware.com/en/VMware-vSphere/7.0/com.vmware.vsphere.resmgmt.doc/GUID-60077B40-66FF-4625-934A-641703ED7601.html
 
 
     :param str datacenter_id: The managed object reference ID
            of the datacenter in which the resource pool is located. This can be omitted
            if the search path used in `name` is an absolute path. For default
            datacenters, use the id attribute from an empty `Datacenter` data
            source.
+           
+           > **Note:** When using ESXi without a vCenter Server instance, you do not
+           need to specify either attribute to use this data source. An empty declaration
+           will load the ESXi host's root resource pool.
     :param str name: The name of the resource pool. This can be a name or
            path. This is required when using vCenter.
     """
     ...
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_role.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_tag.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_tag_category.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_tag_category.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_vapp_container.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_vapp_container.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_virtual_machine.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_virtual_machine.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ]
 
 @pulumi.output_type
 class GetVirtualMachineResult:
     """
     A collection of values returned by getVirtualMachine.
     """
-    def __init__(__self__, alternate_guest_name=None, annotation=None, boot_delay=None, boot_retry_delay=None, boot_retry_enabled=None, change_version=None, cpu_hot_add_enabled=None, cpu_hot_remove_enabled=None, cpu_limit=None, cpu_performance_counters_enabled=None, cpu_reservation=None, cpu_share_count=None, cpu_share_level=None, datacenter_id=None, default_ip_address=None, disks=None, efi_secure_boot_enabled=None, enable_disk_uuid=None, enable_logging=None, ept_rvi_mode=None, extra_config=None, extra_config_reboot_required=None, firmware=None, guest_id=None, guest_ip_addresses=None, hardware_version=None, hv_mode=None, id=None, ide_controller_scan_count=None, latency_sensitivity=None, memory=None, memory_hot_add_enabled=None, memory_limit=None, memory_reservation=None, memory_share_count=None, memory_share_level=None, name=None, nested_hv_enabled=None, network_interface_types=None, network_interfaces=None, num_cores_per_socket=None, num_cpus=None, replace_trigger=None, run_tools_scripts_after_power_on=None, run_tools_scripts_after_resume=None, run_tools_scripts_before_guest_reboot=None, run_tools_scripts_before_guest_shutdown=None, run_tools_scripts_before_guest_standby=None, sata_controller_scan_count=None, scsi_bus_sharing=None, scsi_controller_scan_count=None, scsi_type=None, storage_policy_id=None, swap_placement_policy=None, sync_time_with_host=None, sync_time_with_host_periodically=None, tools_upgrade_policy=None, uuid=None, vapp=None, vapp_transports=None, vbs_enabled=None, vvtd_enabled=None):
+    def __init__(__self__, alternate_guest_name=None, annotation=None, boot_delay=None, boot_retry_delay=None, boot_retry_enabled=None, change_version=None, cpu_hot_add_enabled=None, cpu_hot_remove_enabled=None, cpu_limit=None, cpu_performance_counters_enabled=None, cpu_reservation=None, cpu_share_count=None, cpu_share_level=None, datacenter_id=None, default_ip_address=None, disks=None, efi_secure_boot_enabled=None, enable_disk_uuid=None, enable_logging=None, ept_rvi_mode=None, extra_config=None, extra_config_reboot_required=None, firmware=None, guest_id=None, guest_ip_addresses=None, hardware_version=None, hv_mode=None, id=None, ide_controller_scan_count=None, latency_sensitivity=None, memory=None, memory_hot_add_enabled=None, memory_limit=None, memory_reservation=None, memory_share_count=None, memory_share_level=None, moid=None, name=None, nested_hv_enabled=None, network_interface_types=None, network_interfaces=None, num_cores_per_socket=None, num_cpus=None, replace_trigger=None, run_tools_scripts_after_power_on=None, run_tools_scripts_after_resume=None, run_tools_scripts_before_guest_reboot=None, run_tools_scripts_before_guest_shutdown=None, run_tools_scripts_before_guest_standby=None, sata_controller_scan_count=None, scsi_bus_sharing=None, scsi_controller_scan_count=None, scsi_type=None, storage_policy_id=None, swap_placement_policy=None, sync_time_with_host=None, sync_time_with_host_periodically=None, tools_upgrade_policy=None, uuid=None, vapp=None, vapp_transports=None, vbs_enabled=None, vvtd_enabled=None):
         if alternate_guest_name and not isinstance(alternate_guest_name, str):
             raise TypeError("Expected argument 'alternate_guest_name' to be a str")
         pulumi.set(__self__, "alternate_guest_name", alternate_guest_name)
         if annotation and not isinstance(annotation, str):
             raise TypeError("Expected argument 'annotation' to be a str")
         pulumi.set(__self__, "annotation", annotation)
         if boot_delay and not isinstance(boot_delay, int):
@@ -128,14 +128,17 @@
         pulumi.set(__self__, "memory_reservation", memory_reservation)
         if memory_share_count and not isinstance(memory_share_count, int):
             raise TypeError("Expected argument 'memory_share_count' to be a int")
         pulumi.set(__self__, "memory_share_count", memory_share_count)
         if memory_share_level and not isinstance(memory_share_level, str):
             raise TypeError("Expected argument 'memory_share_level' to be a str")
         pulumi.set(__self__, "memory_share_level", memory_share_level)
+        if moid and not isinstance(moid, str):
+            raise TypeError("Expected argument 'moid' to be a str")
+        pulumi.set(__self__, "moid", moid)
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
         if nested_hv_enabled and not isinstance(nested_hv_enabled, bool):
             raise TypeError("Expected argument 'nested_hv_enabled' to be a bool")
         pulumi.set(__self__, "nested_hv_enabled", nested_hv_enabled)
         if network_interface_types and not isinstance(network_interface_types, list):
@@ -431,14 +434,19 @@
     @property
     @pulumi.getter(name="memoryShareLevel")
     def memory_share_level(self) -> Optional[str]:
         return pulumi.get(self, "memory_share_level")
 
     @property
     @pulumi.getter
+    def moid(self) -> str:
+        return pulumi.get(self, "moid")
+
+    @property
+    @pulumi.getter
     def name(self) -> Optional[str]:
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="nestedHvEnabled")
     def nested_hv_enabled(self) -> Optional[bool]:
         return pulumi.get(self, "nested_hv_enabled")
@@ -635,14 +643,15 @@
             latency_sensitivity=self.latency_sensitivity,
             memory=self.memory,
             memory_hot_add_enabled=self.memory_hot_add_enabled,
             memory_limit=self.memory_limit,
             memory_reservation=self.memory_reservation,
             memory_share_count=self.memory_share_count,
             memory_share_level=self.memory_share_level,
+            moid=self.moid,
             name=self.name,
             nested_hv_enabled=self.nested_hv_enabled,
             network_interface_types=self.network_interface_types,
             network_interfaces=self.network_interfaces,
             num_cores_per_socket=self.num_cores_per_socket,
             num_cpus=self.num_cpus,
             replace_trigger=self.replace_trigger,
@@ -694,14 +703,15 @@
                         latency_sensitivity: Optional[str] = None,
                         memory: Optional[int] = None,
                         memory_hot_add_enabled: Optional[bool] = None,
                         memory_limit: Optional[int] = None,
                         memory_reservation: Optional[int] = None,
                         memory_share_count: Optional[int] = None,
                         memory_share_level: Optional[str] = None,
+                        moid: Optional[str] = None,
                         name: Optional[str] = None,
                         nested_hv_enabled: Optional[bool] = None,
                         num_cores_per_socket: Optional[int] = None,
                         num_cpus: Optional[int] = None,
                         replace_trigger: Optional[str] = None,
                         run_tools_scripts_after_power_on: Optional[bool] = None,
                         run_tools_scripts_after_resume: Optional[bool] = None,
@@ -771,14 +781,20 @@
            the full path relative to the datacenter. This is required if a UUID lookup
            is not performed.
     :param int num_cores_per_socket: The number of cores per socket for this virtual machine.
     :param int num_cpus: The total number of virtual processor cores assigned to this
            virtual machine.
     :param int scsi_controller_scan_count: The number of SCSI controllers to
            scan for disk attributes and controller types on. Default: `1`.
+           
+           > **NOTE:** For best results, ensure that all the disks on any templates you
+           use with this data source reside on the primary controller, and leave this
+           value at the default. See the `VirtualMachine`
+           resource documentation for the significance of this setting, specifically the
+           additional requirements and notes for cloning section.
     :param str uuid: Specify this field for a UUID lookup, `name` and `datacenter_id`
            are not required if this is specified.
     """
     __args__ = dict()
     __args__['alternateGuestName'] = alternate_guest_name
     __args__['annotation'] = annotation
     __args__['bootDelay'] = boot_delay
@@ -806,14 +822,15 @@
     __args__['latencySensitivity'] = latency_sensitivity
     __args__['memory'] = memory
     __args__['memoryHotAddEnabled'] = memory_hot_add_enabled
     __args__['memoryLimit'] = memory_limit
     __args__['memoryReservation'] = memory_reservation
     __args__['memoryShareCount'] = memory_share_count
     __args__['memoryShareLevel'] = memory_share_level
+    __args__['moid'] = moid
     __args__['name'] = name
     __args__['nestedHvEnabled'] = nested_hv_enabled
     __args__['numCoresPerSocket'] = num_cores_per_socket
     __args__['numCpus'] = num_cpus
     __args__['replaceTrigger'] = replace_trigger
     __args__['runToolsScriptsAfterPowerOn'] = run_tools_scripts_after_power_on
     __args__['runToolsScriptsAfterResume'] = run_tools_scripts_after_resume
@@ -867,14 +884,15 @@
         latency_sensitivity=__ret__.latency_sensitivity,
         memory=__ret__.memory,
         memory_hot_add_enabled=__ret__.memory_hot_add_enabled,
         memory_limit=__ret__.memory_limit,
         memory_reservation=__ret__.memory_reservation,
         memory_share_count=__ret__.memory_share_count,
         memory_share_level=__ret__.memory_share_level,
+        moid=__ret__.moid,
         name=__ret__.name,
         nested_hv_enabled=__ret__.nested_hv_enabled,
         network_interface_types=__ret__.network_interface_types,
         network_interfaces=__ret__.network_interfaces,
         num_cores_per_socket=__ret__.num_cores_per_socket,
         num_cpus=__ret__.num_cpus,
         replace_trigger=__ret__.replace_trigger,
@@ -927,14 +945,15 @@
                                latency_sensitivity: Optional[pulumi.Input[Optional[str]]] = None,
                                memory: Optional[pulumi.Input[Optional[int]]] = None,
                                memory_hot_add_enabled: Optional[pulumi.Input[Optional[bool]]] = None,
                                memory_limit: Optional[pulumi.Input[Optional[int]]] = None,
                                memory_reservation: Optional[pulumi.Input[Optional[int]]] = None,
                                memory_share_count: Optional[pulumi.Input[Optional[int]]] = None,
                                memory_share_level: Optional[pulumi.Input[Optional[str]]] = None,
+                               moid: Optional[pulumi.Input[Optional[str]]] = None,
                                name: Optional[pulumi.Input[Optional[str]]] = None,
                                nested_hv_enabled: Optional[pulumi.Input[Optional[bool]]] = None,
                                num_cores_per_socket: Optional[pulumi.Input[Optional[int]]] = None,
                                num_cpus: Optional[pulumi.Input[Optional[int]]] = None,
                                replace_trigger: Optional[pulumi.Input[Optional[str]]] = None,
                                run_tools_scripts_after_power_on: Optional[pulumi.Input[Optional[bool]]] = None,
                                run_tools_scripts_after_resume: Optional[pulumi.Input[Optional[bool]]] = None,
@@ -1004,11 +1023,17 @@
            the full path relative to the datacenter. This is required if a UUID lookup
            is not performed.
     :param int num_cores_per_socket: The number of cores per socket for this virtual machine.
     :param int num_cpus: The total number of virtual processor cores assigned to this
            virtual machine.
     :param int scsi_controller_scan_count: The number of SCSI controllers to
            scan for disk attributes and controller types on. Default: `1`.
+           
+           > **NOTE:** For best results, ensure that all the disks on any templates you
+           use with this data source reside on the primary controller, and leave this
+           value at the default. See the `VirtualMachine`
+           resource documentation for the significance of this setting, specifically the
+           additional requirements and notes for cloning section.
     :param str uuid: Specify this field for a UUID lookup, `name` and `datacenter_id`
            are not required if this is specified.
     """
     ...
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/get_vmfs_disks.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/get_vmfs_disks.py`

 * *Files 10% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
 
 def get_vmfs_disks(filter: Optional[str] = None,
                    host_system_id: Optional[str] = None,
                    rescan: Optional[bool] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVmfsDisksResult:
     """
-    The _get_vmfs_disks_ data source can be used to discover the storage
+    The `get_vmfs_disks` data source can be used to discover the storage
     devices available on an ESXi host. This data source can be combined with the
     `VmfsDatastore` resource to create VMFS
     datastores based off a set of discovered disks.
 
     ## Example Usage
 
     ```python
@@ -107,14 +107,18 @@
         rescan=True,
         filter="mpx.vmhba1:C0:T[12]:L0")
     ```
 
 
     :param str filter: A regular expression to filter the disks against. Only
            disks with canonical names that match will be included.
+           
+           > **NOTE:** Using a `filter` is recommended if there is any chance the host
+           will have any specific storage devices added to it that may affect the order of
+           the output `disks` attribute below, which is lexicographically sorted.
     :param str host_system_id: The managed object ID of
            the host to look for disks on.
     :param bool rescan: Whether or not to rescan storage adapters before
            searching for disks. This may lengthen the time it takes to perform the
            search. Default: `false`.
     """
     __args__ = dict()
@@ -134,15 +138,15 @@
 
 @_utilities.lift_output_func(get_vmfs_disks)
 def get_vmfs_disks_output(filter: Optional[pulumi.Input[Optional[str]]] = None,
                           host_system_id: Optional[pulumi.Input[str]] = None,
                           rescan: Optional[pulumi.Input[Optional[bool]]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVmfsDisksResult]:
     """
-    The _get_vmfs_disks_ data source can be used to discover the storage
+    The `get_vmfs_disks` data source can be used to discover the storage
     devices available on an ESXi host. This data source can be combined with the
     `VmfsDatastore` resource to create VMFS
     datastores based off a set of discovered disks.
 
     ## Example Usage
 
     ```python
@@ -156,14 +160,18 @@
         rescan=True,
         filter="mpx.vmhba1:C0:T[12]:L0")
     ```
 
 
     :param str filter: A regular expression to filter the disks against. Only
            disks with canonical names that match will be included.
+           
+           > **NOTE:** Using a `filter` is recommended if there is any chance the host
+           will have any specific storage devices added to it that may affect the order of
+           the output `disks` attribute below, which is lexicographically sorted.
     :param str host_system_id: The managed object ID of
            the host to look for disks on.
     :param bool rescan: Whether or not to rescan storage adapters before
            searching for disks. This may lengthen the time it takes to perform the
            search. Default: `false`.
     """
     ...
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/ha_vm_override.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/ha_vm_override.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/host.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/host.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,42 +33,50 @@
         :param pulumi.Input[str] hostname: FQDN or IP address of the host to be added.
         :param pulumi.Input[str] password: Password that will be used by vSphere to authenticate
                to the host.
         :param pulumi.Input[str] username: Username that will be used by vSphere to authenticate
                to the host.
         :param pulumi.Input[str] cluster: The ID of the Compute Cluster this host should
                be added to. This should not be set if `datacenter` is set. Conflicts with:
-               `cluster`.
+               `cluster_managed`.
         :param pulumi.Input[bool] cluster_managed: Can be set to `true` if compute cluster
                membership will be managed through the `compute_cluster` resource rather
                than the`host` resource. Conflicts with: `cluster`.
         :param pulumi.Input[bool] connected: If set to false then the host will be disconnected.
                Default is `false`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: A map of custom attribute IDs and string
                values to apply to the resource. Please refer to the
                `vsphere_custom_attributes` resource for more information on applying
                tags to resources.
+               
+               > **NOTE:** Custom attributes are not supported on direct ESXi host
+               connections and require vCenter Server.
+               
+               [docs-host-thumbprint-data-source]: /docs/providers/vsphere/d/host_thumbprint.html
         :param pulumi.Input[str] datacenter: The ID of the datacenter this host should
                be added to. This should not be set if `cluster` is set.
         :param pulumi.Input[bool] force: If set to `true` then it will force the host to be added,
                even if the host is already connected to a different vCenter Server instance.
                Default is `false`.
         :param pulumi.Input[str] license: The license key that will be applied to the host.
                The license key is expected to be present in vSphere.
         :param pulumi.Input[str] lockdown: Set the lockdown state of the host. Valid options are
                `disabled`, `normal`, and `strict`. Default is `disabled`.
         :param pulumi.Input[bool] maintenance: Set the management state of the host.
                Default is `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource. Please
                refer to the `Tag` resource for more information on applying
                tags to resources.
+               
+               > **NOTE:** Tagging support is not supported on direct ESXi host
+               connections and require vCenter Server.
         :param pulumi.Input[str] thumbprint: Host's certificate SHA-1 thumbprint. If not set the
                CA that signed the host's certificate should be trusted. If the CA is not
                trusted and no thumbprint is set then the operation will fail. See data source
-               [_get_host_thumbprint_][docs-host-thumbprint-data-source].
+               [`get_host_thumbprint`][docs-host-thumbprint-data-source].
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "password", password)
         pulumi.set(__self__, "username", username)
         if cluster is not None:
             pulumi.set(__self__, "cluster", cluster)
         if cluster_managed is not None:
@@ -132,15 +140,15 @@
 
     @property
     @pulumi.getter
     def cluster(self) -> Optional[pulumi.Input[str]]:
         """
         The ID of the Compute Cluster this host should
         be added to. This should not be set if `datacenter` is set. Conflicts with:
-        `cluster`.
+        `cluster_managed`.
         """
         return pulumi.get(self, "cluster")
 
     @cluster.setter
     def cluster(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cluster", value)
 
@@ -175,14 +183,19 @@
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         A map of custom attribute IDs and string
         values to apply to the resource. Please refer to the
         `vsphere_custom_attributes` resource for more information on applying
         tags to resources.
+
+        > **NOTE:** Custom attributes are not supported on direct ESXi host
+        connections and require vCenter Server.
+
+        [docs-host-thumbprint-data-source]: /docs/providers/vsphere/d/host_thumbprint.html
         """
         return pulumi.get(self, "custom_attributes")
 
     @custom_attributes.setter
     def custom_attributes(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "custom_attributes", value)
 
@@ -255,29 +268,32 @@
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The IDs of any tags to attach to this resource. Please
         refer to the `Tag` resource for more information on applying
         tags to resources.
+
+        > **NOTE:** Tagging support is not supported on direct ESXi host
+        connections and require vCenter Server.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
     @pulumi.getter
     def thumbprint(self) -> Optional[pulumi.Input[str]]:
         """
         Host's certificate SHA-1 thumbprint. If not set the
         CA that signed the host's certificate should be trusted. If the CA is not
         trusted and no thumbprint is set then the operation will fail. See data source
-        [_get_host_thumbprint_][docs-host-thumbprint-data-source].
+        [`get_host_thumbprint`][docs-host-thumbprint-data-source].
         """
         return pulumi.get(self, "thumbprint")
 
     @thumbprint.setter
     def thumbprint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "thumbprint", value)
 
@@ -299,24 +315,29 @@
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  thumbprint: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Host resources.
         :param pulumi.Input[str] cluster: The ID of the Compute Cluster this host should
                be added to. This should not be set if `datacenter` is set. Conflicts with:
-               `cluster`.
+               `cluster_managed`.
         :param pulumi.Input[bool] cluster_managed: Can be set to `true` if compute cluster
                membership will be managed through the `compute_cluster` resource rather
                than the`host` resource. Conflicts with: `cluster`.
         :param pulumi.Input[bool] connected: If set to false then the host will be disconnected.
                Default is `false`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: A map of custom attribute IDs and string
                values to apply to the resource. Please refer to the
                `vsphere_custom_attributes` resource for more information on applying
                tags to resources.
+               
+               > **NOTE:** Custom attributes are not supported on direct ESXi host
+               connections and require vCenter Server.
+               
+               [docs-host-thumbprint-data-source]: /docs/providers/vsphere/d/host_thumbprint.html
         :param pulumi.Input[str] datacenter: The ID of the datacenter this host should
                be added to. This should not be set if `cluster` is set.
         :param pulumi.Input[bool] force: If set to `true` then it will force the host to be added,
                even if the host is already connected to a different vCenter Server instance.
                Default is `false`.
         :param pulumi.Input[str] hostname: FQDN or IP address of the host to be added.
         :param pulumi.Input[str] license: The license key that will be applied to the host.
@@ -326,18 +347,21 @@
         :param pulumi.Input[bool] maintenance: Set the management state of the host.
                Default is `false`.
         :param pulumi.Input[str] password: Password that will be used by vSphere to authenticate
                to the host.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource. Please
                refer to the `Tag` resource for more information on applying
                tags to resources.
+               
+               > **NOTE:** Tagging support is not supported on direct ESXi host
+               connections and require vCenter Server.
         :param pulumi.Input[str] thumbprint: Host's certificate SHA-1 thumbprint. If not set the
                CA that signed the host's certificate should be trusted. If the CA is not
                trusted and no thumbprint is set then the operation will fail. See data source
-               [_get_host_thumbprint_][docs-host-thumbprint-data-source].
+               [`get_host_thumbprint`][docs-host-thumbprint-data-source].
         :param pulumi.Input[str] username: Username that will be used by vSphere to authenticate
                to the host.
         """
         if cluster is not None:
             pulumi.set(__self__, "cluster", cluster)
         if cluster_managed is not None:
             pulumi.set(__self__, "cluster_managed", cluster_managed)
@@ -368,15 +392,15 @@
 
     @property
     @pulumi.getter
     def cluster(self) -> Optional[pulumi.Input[str]]:
         """
         The ID of the Compute Cluster this host should
         be added to. This should not be set if `datacenter` is set. Conflicts with:
-        `cluster`.
+        `cluster_managed`.
         """
         return pulumi.get(self, "cluster")
 
     @cluster.setter
     def cluster(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cluster", value)
 
@@ -411,14 +435,19 @@
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         A map of custom attribute IDs and string
         values to apply to the resource. Please refer to the
         `vsphere_custom_attributes` resource for more information on applying
         tags to resources.
+
+        > **NOTE:** Custom attributes are not supported on direct ESXi host
+        connections and require vCenter Server.
+
+        [docs-host-thumbprint-data-source]: /docs/providers/vsphere/d/host_thumbprint.html
         """
         return pulumi.get(self, "custom_attributes")
 
     @custom_attributes.setter
     def custom_attributes(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "custom_attributes", value)
 
@@ -516,29 +545,32 @@
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The IDs of any tags to attach to this resource. Please
         refer to the `Tag` resource for more information on applying
         tags to resources.
+
+        > **NOTE:** Tagging support is not supported on direct ESXi host
+        connections and require vCenter Server.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
     @pulumi.getter
     def thumbprint(self) -> Optional[pulumi.Input[str]]:
         """
         Host's certificate SHA-1 thumbprint. If not set the
         CA that signed the host's certificate should be trusted. If the CA is not
         trusted and no thumbprint is set then the operation will fail. See data source
-        [_get_host_thumbprint_][docs-host-thumbprint-data-source].
+        [`get_host_thumbprint`][docs-host-thumbprint-data-source].
         """
         return pulumi.get(self, "thumbprint")
 
     @thumbprint.setter
     def thumbprint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "thumbprint", value)
 
@@ -630,24 +662,29 @@
 
         The above would import the host with ID `host-123`.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cluster: The ID of the Compute Cluster this host should
                be added to. This should not be set if `datacenter` is set. Conflicts with:
-               `cluster`.
+               `cluster_managed`.
         :param pulumi.Input[bool] cluster_managed: Can be set to `true` if compute cluster
                membership will be managed through the `compute_cluster` resource rather
                than the`host` resource. Conflicts with: `cluster`.
         :param pulumi.Input[bool] connected: If set to false then the host will be disconnected.
                Default is `false`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: A map of custom attribute IDs and string
                values to apply to the resource. Please refer to the
                `vsphere_custom_attributes` resource for more information on applying
                tags to resources.
+               
+               > **NOTE:** Custom attributes are not supported on direct ESXi host
+               connections and require vCenter Server.
+               
+               [docs-host-thumbprint-data-source]: /docs/providers/vsphere/d/host_thumbprint.html
         :param pulumi.Input[str] datacenter: The ID of the datacenter this host should
                be added to. This should not be set if `cluster` is set.
         :param pulumi.Input[bool] force: If set to `true` then it will force the host to be added,
                even if the host is already connected to a different vCenter Server instance.
                Default is `false`.
         :param pulumi.Input[str] hostname: FQDN or IP address of the host to be added.
         :param pulumi.Input[str] license: The license key that will be applied to the host.
@@ -657,18 +694,21 @@
         :param pulumi.Input[bool] maintenance: Set the management state of the host.
                Default is `false`.
         :param pulumi.Input[str] password: Password that will be used by vSphere to authenticate
                to the host.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource. Please
                refer to the `Tag` resource for more information on applying
                tags to resources.
+               
+               > **NOTE:** Tagging support is not supported on direct ESXi host
+               connections and require vCenter Server.
         :param pulumi.Input[str] thumbprint: Host's certificate SHA-1 thumbprint. If not set the
                CA that signed the host's certificate should be trusted. If the CA is not
                trusted and no thumbprint is set then the operation will fail. See data source
-               [_get_host_thumbprint_][docs-host-thumbprint-data-source].
+               [`get_host_thumbprint`][docs-host-thumbprint-data-source].
         :param pulumi.Input[str] username: Username that will be used by vSphere to authenticate
                to the host.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -817,24 +857,29 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cluster: The ID of the Compute Cluster this host should
                be added to. This should not be set if `datacenter` is set. Conflicts with:
-               `cluster`.
+               `cluster_managed`.
         :param pulumi.Input[bool] cluster_managed: Can be set to `true` if compute cluster
                membership will be managed through the `compute_cluster` resource rather
                than the`host` resource. Conflicts with: `cluster`.
         :param pulumi.Input[bool] connected: If set to false then the host will be disconnected.
                Default is `false`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: A map of custom attribute IDs and string
                values to apply to the resource. Please refer to the
                `vsphere_custom_attributes` resource for more information on applying
                tags to resources.
+               
+               > **NOTE:** Custom attributes are not supported on direct ESXi host
+               connections and require vCenter Server.
+               
+               [docs-host-thumbprint-data-source]: /docs/providers/vsphere/d/host_thumbprint.html
         :param pulumi.Input[str] datacenter: The ID of the datacenter this host should
                be added to. This should not be set if `cluster` is set.
         :param pulumi.Input[bool] force: If set to `true` then it will force the host to be added,
                even if the host is already connected to a different vCenter Server instance.
                Default is `false`.
         :param pulumi.Input[str] hostname: FQDN or IP address of the host to be added.
         :param pulumi.Input[str] license: The license key that will be applied to the host.
@@ -844,18 +889,21 @@
         :param pulumi.Input[bool] maintenance: Set the management state of the host.
                Default is `false`.
         :param pulumi.Input[str] password: Password that will be used by vSphere to authenticate
                to the host.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource. Please
                refer to the `Tag` resource for more information on applying
                tags to resources.
+               
+               > **NOTE:** Tagging support is not supported on direct ESXi host
+               connections and require vCenter Server.
         :param pulumi.Input[str] thumbprint: Host's certificate SHA-1 thumbprint. If not set the
                CA that signed the host's certificate should be trusted. If the CA is not
                trusted and no thumbprint is set then the operation will fail. See data source
-               [_get_host_thumbprint_][docs-host-thumbprint-data-source].
+               [`get_host_thumbprint`][docs-host-thumbprint-data-source].
         :param pulumi.Input[str] username: Username that will be used by vSphere to authenticate
                to the host.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _HostState.__new__(_HostState)
 
@@ -877,15 +925,15 @@
 
     @property
     @pulumi.getter
     def cluster(self) -> pulumi.Output[Optional[str]]:
         """
         The ID of the Compute Cluster this host should
         be added to. This should not be set if `datacenter` is set. Conflicts with:
-        `cluster`.
+        `cluster_managed`.
         """
         return pulumi.get(self, "cluster")
 
     @property
     @pulumi.getter(name="clusterManaged")
     def cluster_managed(self) -> pulumi.Output[Optional[bool]]:
         """
@@ -908,14 +956,19 @@
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
         A map of custom attribute IDs and string
         values to apply to the resource. Please refer to the
         `vsphere_custom_attributes` resource for more information on applying
         tags to resources.
+
+        > **NOTE:** Custom attributes are not supported on direct ESXi host
+        connections and require vCenter Server.
+
+        [docs-host-thumbprint-data-source]: /docs/providers/vsphere/d/host_thumbprint.html
         """
         return pulumi.get(self, "custom_attributes")
 
     @property
     @pulumi.getter
     def datacenter(self) -> pulumi.Output[Optional[str]]:
         """
@@ -981,25 +1034,28 @@
     @property
     @pulumi.getter
     def tags(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         The IDs of any tags to attach to this resource. Please
         refer to the `Tag` resource for more information on applying
         tags to resources.
+
+        > **NOTE:** Tagging support is not supported on direct ESXi host
+        connections and require vCenter Server.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def thumbprint(self) -> pulumi.Output[Optional[str]]:
         """
         Host's certificate SHA-1 thumbprint. If not set the
         CA that signed the host's certificate should be trusted. If the CA is not
         trusted and no thumbprint is set then the operation will fail. See data source
-        [_get_host_thumbprint_][docs-host-thumbprint-data-source].
+        [`get_host_thumbprint`][docs-host-thumbprint-data-source].
         """
         return pulumi.get(self, "thumbprint")
 
     @property
     @pulumi.getter
     def username(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/host_port_group.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/host_port_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/host_virtual_switch.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/host_virtual_switch.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,17 @@
         :param pulumi.Input[str] name: The name of the virtual switch. Forces a new resource if
                changed.
         :param pulumi.Input[bool] notify_switches: If set to `true`, the teaming policy will
                notify the broadcast network of a NIC failover, triggering cache updates.
                Default: `true`.
         :param pulumi.Input[int] number_of_ports: The number of ports to create with this
                virtual switch. Default: `128`.
+               
+               > **NOTE:** Changing the port count requires a reboot of the host. This provider
+               will not restart the host for you.
         :param pulumi.Input[int] shaping_average_bandwidth: The average bandwidth in bits per
                second if traffic shaping is enabled. Default: `0`
         :param pulumi.Input[int] shaping_burst_size: The maximum burst size allowed in bytes if
                shaping is enabled. Default: `0`
         :param pulumi.Input[bool] shaping_enabled: Set to `true` to enable the traffic shaper for
                ports managed by this virtual switch. Default: `false`.
         :param pulumi.Input[int] shaping_peak_bandwidth: The peak bandwidth during bursts in
@@ -317,14 +320,17 @@
 
     @property
     @pulumi.getter(name="numberOfPorts")
     def number_of_ports(self) -> Optional[pulumi.Input[int]]:
         """
         The number of ports to create with this
         virtual switch. Default: `128`.
+
+        > **NOTE:** Changing the port count requires a reboot of the host. This provider
+        will not restart the host for you.
         """
         return pulumi.get(self, "number_of_ports")
 
     @number_of_ports.setter
     def number_of_ports(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "number_of_ports", value)
 
@@ -466,14 +472,17 @@
                changed.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_adapters: The network interfaces to bind to the bridge.
         :param pulumi.Input[bool] notify_switches: If set to `true`, the teaming policy will
                notify the broadcast network of a NIC failover, triggering cache updates.
                Default: `true`.
         :param pulumi.Input[int] number_of_ports: The number of ports to create with this
                virtual switch. Default: `128`.
+               
+               > **NOTE:** Changing the port count requires a reboot of the host. This provider
+               will not restart the host for you.
         :param pulumi.Input[int] shaping_average_bandwidth: The average bandwidth in bits per
                second if traffic shaping is enabled. Default: `0`
         :param pulumi.Input[int] shaping_burst_size: The maximum burst size allowed in bytes if
                shaping is enabled. Default: `0`
         :param pulumi.Input[bool] shaping_enabled: Set to `true` to enable the traffic shaper for
                ports managed by this virtual switch. Default: `false`.
         :param pulumi.Input[int] shaping_peak_bandwidth: The peak bandwidth during bursts in
@@ -717,14 +726,17 @@
 
     @property
     @pulumi.getter(name="numberOfPorts")
     def number_of_ports(self) -> Optional[pulumi.Input[int]]:
         """
         The number of ports to create with this
         virtual switch. Default: `128`.
+
+        > **NOTE:** Changing the port count requires a reboot of the host. This provider
+        will not restart the host for you.
         """
         return pulumi.get(self, "number_of_ports")
 
     @number_of_ports.setter
     def number_of_ports(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "number_of_ports", value)
 
@@ -871,14 +883,17 @@
                changed.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_adapters: The network interfaces to bind to the bridge.
         :param pulumi.Input[bool] notify_switches: If set to `true`, the teaming policy will
                notify the broadcast network of a NIC failover, triggering cache updates.
                Default: `true`.
         :param pulumi.Input[int] number_of_ports: The number of ports to create with this
                virtual switch. Default: `128`.
+               
+               > **NOTE:** Changing the port count requires a reboot of the host. This provider
+               will not restart the host for you.
         :param pulumi.Input[int] shaping_average_bandwidth: The average bandwidth in bits per
                second if traffic shaping is enabled. Default: `0`
         :param pulumi.Input[int] shaping_burst_size: The maximum burst size allowed in bytes if
                shaping is enabled. Default: `0`
         :param pulumi.Input[bool] shaping_enabled: Set to `true` to enable the traffic shaper for
                ports managed by this virtual switch. Default: `false`.
         :param pulumi.Input[int] shaping_peak_bandwidth: The peak bandwidth during bursts in
@@ -1039,14 +1054,17 @@
                changed.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_adapters: The network interfaces to bind to the bridge.
         :param pulumi.Input[bool] notify_switches: If set to `true`, the teaming policy will
                notify the broadcast network of a NIC failover, triggering cache updates.
                Default: `true`.
         :param pulumi.Input[int] number_of_ports: The number of ports to create with this
                virtual switch. Default: `128`.
+               
+               > **NOTE:** Changing the port count requires a reboot of the host. This provider
+               will not restart the host for you.
         :param pulumi.Input[int] shaping_average_bandwidth: The average bandwidth in bits per
                second if traffic shaping is enabled. Default: `0`
         :param pulumi.Input[int] shaping_burst_size: The maximum burst size allowed in bytes if
                shaping is enabled. Default: `0`
         :param pulumi.Input[bool] shaping_enabled: Set to `true` to enable the traffic shaper for
                ports managed by this virtual switch. Default: `false`.
         :param pulumi.Input[int] shaping_peak_bandwidth: The peak bandwidth during bursts in
@@ -1218,14 +1236,17 @@
 
     @property
     @pulumi.getter(name="numberOfPorts")
     def number_of_ports(self) -> pulumi.Output[Optional[int]]:
         """
         The number of ports to create with this
         virtual switch. Default: `128`.
+
+        > **NOTE:** Changing the port count requires a reboot of the host. This provider
+        will not restart the host for you.
         """
         return pulumi.get(self, "number_of_ports")
 
     @property
     @pulumi.getter(name="shapingAverageBandwidth")
     def shaping_average_bandwidth(self) -> pulumi.Output[Optional[int]]:
         """
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/license.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/license.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/nas_datastore.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/nas_datastore.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,17 @@
                resource if changed.
         :param pulumi.Input[str] access_mode: Access mode for the mount point. Can be one of
                `readOnly` or `readWrite`. Note that `readWrite` does not necessarily mean
                that the datastore will be read-write depending on the permissions of the
                actual share. Default: `readWrite`. Forces a new resource if changed.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to attribute 
                value strings to set on datasource resource.
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+               and require vCenter.
         :param pulumi.Input[str] datastore_cluster_id: The managed object
                ID of a datastore cluster to put this datastore in.
                Conflicts with `folder`.
         :param pulumi.Input[str] folder: The relative path to a folder to put this datastore in.
                This is a path relative to the datacenter you are deploying the datastore to.
                Example: for the `dc1` datacenter, and a provided `folder` of `foo/bar`,
                The provider will place a datastore named `test` in a datastore folder
@@ -51,15 +54,18 @@
                `/dc1/datastore/foo/bar/test`. Conflicts with
                `datastore_cluster_id`.
         :param pulumi.Input[str] name: The name of the datastore. Forces a new resource if
                changed.
         :param pulumi.Input[str] security_type: The security type to use when using NFS v4.1.
                Can be one of `AUTH_SYS`, `SEC_KRB5`, or `SEC_KRB5I`. Forces a new resource
                if changed.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource. 
+               
+               > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+               requires vCenter 6.0 or higher.
         :param pulumi.Input[str] type: The type of NAS volume. Can be one of `NFS` (to denote
                v3) or `NFS41` (to denote NFS v4.1). Default: `NFS`. Forces a new resource if
                changed.
         """
         pulumi.set(__self__, "host_system_ids", host_system_ids)
         pulumi.set(__self__, "remote_hosts", remote_hosts)
         pulumi.set(__self__, "remote_path", remote_path)
@@ -137,14 +143,17 @@
 
     @property
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Map of custom attribute ids to attribute 
         value strings to set on datasource resource.
+
+        > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+        and require vCenter.
         """
         return pulumi.get(self, "custom_attributes")
 
     @custom_attributes.setter
     def custom_attributes(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "custom_attributes", value)
 
@@ -207,15 +216,18 @@
     def security_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "security_type", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The IDs of any tags to attach to this resource.
+        The IDs of any tags to attach to this resource. 
+
+        > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+        requires vCenter 6.0 or higher.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -263,14 +275,17 @@
                that the datastore will be read-write depending on the permissions of the
                actual share. Default: `readWrite`. Forces a new resource if changed.
         :param pulumi.Input[bool] accessible: The connectivity status of the datastore. If this is `false`,
                some other computed attributes may be out of date.
         :param pulumi.Input[int] capacity: Maximum capacity of the datastore, in megabytes.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to attribute 
                value strings to set on datasource resource.
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+               and require vCenter.
         :param pulumi.Input[str] datastore_cluster_id: The managed object
                ID of a datastore cluster to put this datastore in.
                Conflicts with `folder`.
         :param pulumi.Input[str] folder: The relative path to a folder to put this datastore in.
                This is a path relative to the datacenter you are deploying the datastore to.
                Example: for the `dc1` datacenter, and a provided `folder` of `foo/bar`,
                The provider will place a datastore named `test` in a datastore folder
@@ -291,15 +306,18 @@
                server or servers. Only one element should be present for NFS v3 but multiple
                can be present for NFS v4.1. Forces a new resource if changed.
         :param pulumi.Input[str] remote_path: The remote path of the mount point. Forces a new
                resource if changed.
         :param pulumi.Input[str] security_type: The security type to use when using NFS v4.1.
                Can be one of `AUTH_SYS`, `SEC_KRB5`, or `SEC_KRB5I`. Forces a new resource
                if changed.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource. 
+               
+               > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+               requires vCenter 6.0 or higher.
         :param pulumi.Input[str] type: The type of NAS volume. Can be one of `NFS` (to denote
                v3) or `NFS41` (to denote NFS v4.1). Default: `NFS`. Forces a new resource if
                changed.
         :param pulumi.Input[int] uncommitted_space: Total additional storage space, in megabytes,
                potentially used by all virtual machines on this datastore.
         :param pulumi.Input[str] url: The unique locator for the datastore.
         """
@@ -384,14 +402,17 @@
 
     @property
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Map of custom attribute ids to attribute 
         value strings to set on datasource resource.
+
+        > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+        and require vCenter.
         """
         return pulumi.get(self, "custom_attributes")
 
     @custom_attributes.setter
     def custom_attributes(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "custom_attributes", value)
 
@@ -544,15 +565,18 @@
     def security_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "security_type", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The IDs of any tags to attach to this resource.
+        The IDs of any tags to attach to this resource. 
+
+        > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+        requires vCenter 6.0 or higher.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -619,14 +643,17 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_mode: Access mode for the mount point. Can be one of
                `readOnly` or `readWrite`. Note that `readWrite` does not necessarily mean
                that the datastore will be read-write depending on the permissions of the
                actual share. Default: `readWrite`. Forces a new resource if changed.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to attribute 
                value strings to set on datasource resource.
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+               and require vCenter.
         :param pulumi.Input[str] datastore_cluster_id: The managed object
                ID of a datastore cluster to put this datastore in.
                Conflicts with `folder`.
         :param pulumi.Input[str] folder: The relative path to a folder to put this datastore in.
                This is a path relative to the datacenter you are deploying the datastore to.
                Example: for the `dc1` datacenter, and a provided `folder` of `foo/bar`,
                The provider will place a datastore named `test` in a datastore folder
@@ -641,15 +668,18 @@
                server or servers. Only one element should be present for NFS v3 but multiple
                can be present for NFS v4.1. Forces a new resource if changed.
         :param pulumi.Input[str] remote_path: The remote path of the mount point. Forces a new
                resource if changed.
         :param pulumi.Input[str] security_type: The security type to use when using NFS v4.1.
                Can be one of `AUTH_SYS`, `SEC_KRB5`, or `SEC_KRB5I`. Forces a new resource
                if changed.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource. 
+               
+               > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+               requires vCenter 6.0 or higher.
         :param pulumi.Input[str] type: The type of NAS volume. Can be one of `NFS` (to denote
                v3) or `NFS41` (to denote NFS v4.1). Default: `NFS`. Forces a new resource if
                changed.
         """
         ...
     @overload
     def __init__(__self__,
@@ -759,14 +789,17 @@
                that the datastore will be read-write depending on the permissions of the
                actual share. Default: `readWrite`. Forces a new resource if changed.
         :param pulumi.Input[bool] accessible: The connectivity status of the datastore. If this is `false`,
                some other computed attributes may be out of date.
         :param pulumi.Input[int] capacity: Maximum capacity of the datastore, in megabytes.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to attribute 
                value strings to set on datasource resource.
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+               and require vCenter.
         :param pulumi.Input[str] datastore_cluster_id: The managed object
                ID of a datastore cluster to put this datastore in.
                Conflicts with `folder`.
         :param pulumi.Input[str] folder: The relative path to a folder to put this datastore in.
                This is a path relative to the datacenter you are deploying the datastore to.
                Example: for the `dc1` datacenter, and a provided `folder` of `foo/bar`,
                The provider will place a datastore named `test` in a datastore folder
@@ -787,15 +820,18 @@
                server or servers. Only one element should be present for NFS v3 but multiple
                can be present for NFS v4.1. Forces a new resource if changed.
         :param pulumi.Input[str] remote_path: The remote path of the mount point. Forces a new
                resource if changed.
         :param pulumi.Input[str] security_type: The security type to use when using NFS v4.1.
                Can be one of `AUTH_SYS`, `SEC_KRB5`, or `SEC_KRB5I`. Forces a new resource
                if changed.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource. 
+               
+               > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+               requires vCenter 6.0 or higher.
         :param pulumi.Input[str] type: The type of NAS volume. Can be one of `NFS` (to denote
                v3) or `NFS41` (to denote NFS v4.1). Default: `NFS`. Forces a new resource if
                changed.
         :param pulumi.Input[int] uncommitted_space: Total additional storage space, in megabytes,
                potentially used by all virtual machines on this datastore.
         :param pulumi.Input[str] url: The unique locator for the datastore.
         """
@@ -854,14 +890,17 @@
 
     @property
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
         Map of custom attribute ids to attribute 
         value strings to set on datasource resource.
+
+        > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+        and require vCenter.
         """
         return pulumi.get(self, "custom_attributes")
 
     @property
     @pulumi.getter(name="datastoreClusterId")
     def datastore_cluster_id(self) -> pulumi.Output[Optional[str]]:
         """
@@ -966,15 +1005,18 @@
         """
         return pulumi.get(self, "security_type")
 
     @property
     @pulumi.getter
     def tags(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        The IDs of any tags to attach to this resource.
+        The IDs of any tags to attach to this resource. 
+
+        > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+        requires vCenter 6.0 or higher.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/outputs.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/outputs.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,42 @@
 class ComputeClusterVsanDiskGroup(dict):
     def __init__(__self__, *,
                  cache: Optional[str] = None,
                  storages: Optional[Sequence[str]] = None):
         """
         :param str cache: The canonical name of the disk to use for vSAN cache.
         :param Sequence[str] storages: An array of disk canonical names for vSAN storage.
+               
+               > **NOTE:** You must disable vSphere HA before you enable vSAN on the cluster.
+               You can enable or re-enable vSphere HA after vSAN is configured.
+               
+               ```python
+               import pulumi
+               import pulumi_vsphere as vsphere
+               
+               compute_cluster = vsphere.ComputeCluster("computeCluster",
+                   datacenter_id=data["vsphere_datacenter"]["datacenter"]["id"],
+                   host_system_ids=[[__item["id"] for __item in data["vsphere_host"]["host"]]],
+                   drs_enabled=True,
+                   drs_automation_level="fullyAutomated",
+                   ha_enabled=False,
+                   vsan_enabled=True,
+                   vsan_dedup_enabled=True,
+                   vsan_compression_enabled=True,
+                   vsan_performance_enabled=True,
+                   vsan_verbose_mode_enabled=True,
+                   vsan_network_diagnostic_mode_enabled=True,
+                   vsan_unmap_enabled=True,
+                   vsan_dit_encryption_enabled=True,
+                   vsan_dit_rekey_interval=1800,
+                   vsan_disk_groups=[vsphere.ComputeClusterVsanDiskGroupArgs(
+                       cache=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                       storages=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                   )])
+               ```
         """
         if cache is not None:
             pulumi.set(__self__, "cache", cache)
         if storages is not None:
             pulumi.set(__self__, "storages", storages)
 
     @property
@@ -61,14 +89,42 @@
         return pulumi.get(self, "cache")
 
     @property
     @pulumi.getter
     def storages(self) -> Optional[Sequence[str]]:
         """
         An array of disk canonical names for vSAN storage.
+
+        > **NOTE:** You must disable vSphere HA before you enable vSAN on the cluster.
+        You can enable or re-enable vSphere HA after vSAN is configured.
+
+        ```python
+        import pulumi
+        import pulumi_vsphere as vsphere
+
+        compute_cluster = vsphere.ComputeCluster("computeCluster",
+            datacenter_id=data["vsphere_datacenter"]["datacenter"]["id"],
+            host_system_ids=[[__item["id"] for __item in data["vsphere_host"]["host"]]],
+            drs_enabled=True,
+            drs_automation_level="fullyAutomated",
+            ha_enabled=False,
+            vsan_enabled=True,
+            vsan_dedup_enabled=True,
+            vsan_compression_enabled=True,
+            vsan_performance_enabled=True,
+            vsan_verbose_mode_enabled=True,
+            vsan_network_diagnostic_mode_enabled=True,
+            vsan_unmap_enabled=True,
+            vsan_dit_encryption_enabled=True,
+            vsan_dit_rekey_interval=1800,
+            vsan_disk_groups=[vsphere.ComputeClusterVsanDiskGroupArgs(
+                cache=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+                storages=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+            )])
+        ```
         """
         return pulumi.get(self, "storages")
 
 
 @pulumi.output_type
 class ContentLibraryPublication(dict):
     @staticmethod
@@ -603,16 +659,22 @@
                  datastore_id: Optional[str] = None,
                  device_address: Optional[str] = None,
                  key: Optional[int] = None,
                  path: Optional[str] = None):
         """
         :param bool client_device: Indicates whether the device should be backed by remote client device. Conflicts with `datastore_id` and `path`.
         :param str datastore_id: The managed object reference ID of the datastore in which to place the virtual machine. The virtual machine configuration files is placed here, along with any virtual disks that are created where a datastore is not explicitly specified. See the section on virtual machine migration for more information on modifying this value.
+               
+               > **NOTE:** Datastores cannot be assigned to individual disks when `datastore_cluster_id` is used.
         :param int key: The ID of the device within the virtual machine.
         :param str path: When using `attach`, this parameter controls the path of a virtual disk to attach externally. Otherwise, it is a computed attribute that contains the virtual disk filename.
+               
+               > **NOTE:** Either `client_device` (for a remote backed CD-ROM) or `datastore_id` and `path` (for a datastore ISO backed CD-ROM) are required to .
+               
+               > **NOTE:** Some CD-ROM drive types are not supported by this resource, such as pass-through devices. If these drives are present in a cloned template, or added outside of the provider, the desired state will be corrected to the defined device, or removed if no `cdrom` block is present.
         """
         if client_device is not None:
             pulumi.set(__self__, "client_device", client_device)
         if datastore_id is not None:
             pulumi.set(__self__, "datastore_id", datastore_id)
         if device_address is not None:
             pulumi.set(__self__, "device_address", device_address)
@@ -630,14 +692,16 @@
         return pulumi.get(self, "client_device")
 
     @property
     @pulumi.getter(name="datastoreId")
     def datastore_id(self) -> Optional[str]:
         """
         The managed object reference ID of the datastore in which to place the virtual machine. The virtual machine configuration files is placed here, along with any virtual disks that are created where a datastore is not explicitly specified. See the section on virtual machine migration for more information on modifying this value.
+
+        > **NOTE:** Datastores cannot be assigned to individual disks when `datastore_cluster_id` is used.
         """
         return pulumi.get(self, "datastore_id")
 
     @property
     @pulumi.getter(name="deviceAddress")
     def device_address(self) -> Optional[str]:
         return pulumi.get(self, "device_address")
@@ -651,14 +715,18 @@
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def path(self) -> Optional[str]:
         """
         When using `attach`, this parameter controls the path of a virtual disk to attach externally. Otherwise, it is a computed attribute that contains the virtual disk filename.
+
+        > **NOTE:** Either `client_device` (for a remote backed CD-ROM) or `datastore_id` and `path` (for a datastore ISO backed CD-ROM) are required to .
+
+        > **NOTE:** Some CD-ROM drive types are not supported by this resource, such as pass-through devices. If these drives are present in a cloned template, or added outside of the provider, the desired state will be corrected to the defined device, or removed if no `cdrom` block is present.
         """
         return pulumi.get(self, "path")
 
 
 @pulumi.output_type
 class VirtualMachineClone(dict):
     @staticmethod
@@ -1207,28 +1275,39 @@
                  size: Optional[int] = None,
                  storage_policy_id: Optional[str] = None,
                  thin_provisioned: Optional[bool] = None,
                  unit_number: Optional[int] = None,
                  uuid: Optional[str] = None,
                  write_through: Optional[bool] = None):
         """
-        :param str label: A label for the virtual disk. Forces a new disk, if changed.
         :param bool attach: Attach an external disk instead of creating a new one. Implies and conflicts with `keep_on_remove`. If set, you cannot set `size`, `eagerly_scrub`, or `thin_provisioned`. Must set `path` if used.
+               
+               > **NOTE:** External disks cannot be attached when `datastore_cluster_id` is used.
         :param str controller_type: The type of storage controller to attach the  disk to. Can be `scsi`, `sata`, or `ide`. You must have the appropriate number of controllers enabled for the selected type. Default `scsi`.
         :param str datastore_id: The managed object reference ID of the datastore in which to place the virtual machine. The virtual machine configuration files is placed here, along with any virtual disks that are created where a datastore is not explicitly specified. See the section on virtual machine migration for more information on modifying this value.
+               
+               > **NOTE:** Datastores cannot be assigned to individual disks when `datastore_cluster_id` is used.
         :param str disk_mode: The mode of this this virtual disk for purposes of writes and snapshots. One of `append`, `independent_nonpersistent`, `independent_persistent`, `nonpersistent`, `persistent`, or `undoable`. Default: `persistent`. For more information on these option, please refer to the [product documentation][vmware-docs-disk-mode].
+               
+               [vmware-docs-disk-mode]: https://vdc-download.vmware.com/vmwb-repository/dcr-public/da47f910-60ac-438b-8b9b-6122f4d14524/16b7274a-bf8b-4b4c-a05e-746f2aa93c8c/doc/vim.vm.device.VirtualDiskOption.DiskMode.html
         :param str disk_sharing: The sharing mode of this virtual disk. One of `sharingMultiWriter` or `sharingNone`. Default: `sharingNone`.
+               
+               > **NOTE:** Disk sharing is only available on vSphere 6.0 and later.
         :param bool eagerly_scrub: If set to `true`, the disk space is zeroed out when the virtual machine is created. This will delay the creation of the virtual disk. Cannot be set to `true` when `thin_provisioned` is `true`.  See the section on picking a disk type for more information.  Default: `false`.
         :param int io_limit: The upper limit of IOPS that this disk can use. The default is no limit.
         :param int io_reservation: The I/O reservation (guarantee) for the virtual disk has, in IOPS.  The default is no reservation.
         :param int io_share_count: The share count for the virtual disk when the share level is `custom`.
         :param str io_share_level: The share allocation level for the virtual disk. One of `low`, `normal`, `high`, or `custom`. Default: `normal`.
         :param bool keep_on_remove: Keep this disk when removing the device or destroying the virtual machine. Default: `false`.
         :param int key: The ID of the device within the virtual machine.
         :param str path: When using `attach`, this parameter controls the path of a virtual disk to attach externally. Otherwise, it is a computed attribute that contains the virtual disk filename.
+               
+               > **NOTE:** Either `client_device` (for a remote backed CD-ROM) or `datastore_id` and `path` (for a datastore ISO backed CD-ROM) are required to .
+               
+               > **NOTE:** Some CD-ROM drive types are not supported by this resource, such as pass-through devices. If these drives are present in a cloned template, or added outside of the provider, the desired state will be corrected to the defined device, or removed if no `cdrom` block is present.
         :param int size: The size of the disk, in GB. Must be a whole number.
         :param str storage_policy_id: The ID of the storage policy to assign to the home directory of a virtual machine.
         :param bool thin_provisioned: If `true`, the disk is thin provisioned, with space for the file being allocated on an as-needed basis. Cannot be set to `true` when `eagerly_scrub` is `true`. See the section on selecting a disk type for more information. Default: `true`.
         :param int unit_number: The disk number on the storage bus. The maximum value for this setting is the value of the controller count times the controller capacity (15 for SCSI, 30 for SATA, and 2 for IDE). Duplicate unit numbers are not allowed. Default `0`, for which one disk must be set to.
         :param str uuid: The UUID of the virtual disk VMDK file. This is used to track the virtual disk on the virtual machine.
         :param bool write_through: If `true`, writes for this disk are sent directly to the filesystem immediately instead of being buffered. Default: `false`.
         """
@@ -1273,24 +1352,23 @@
             pulumi.set(__self__, "uuid", uuid)
         if write_through is not None:
             pulumi.set(__self__, "write_through", write_through)
 
     @property
     @pulumi.getter
     def label(self) -> str:
-        """
-        A label for the virtual disk. Forces a new disk, if changed.
-        """
         return pulumi.get(self, "label")
 
     @property
     @pulumi.getter
     def attach(self) -> Optional[bool]:
         """
         Attach an external disk instead of creating a new one. Implies and conflicts with `keep_on_remove`. If set, you cannot set `size`, `eagerly_scrub`, or `thin_provisioned`. Must set `path` if used.
+
+        > **NOTE:** External disks cannot be attached when `datastore_cluster_id` is used.
         """
         return pulumi.get(self, "attach")
 
     @property
     @pulumi.getter(name="controllerType")
     def controller_type(self) -> Optional[str]:
         """
@@ -1299,35 +1377,41 @@
         return pulumi.get(self, "controller_type")
 
     @property
     @pulumi.getter(name="datastoreId")
     def datastore_id(self) -> Optional[str]:
         """
         The managed object reference ID of the datastore in which to place the virtual machine. The virtual machine configuration files is placed here, along with any virtual disks that are created where a datastore is not explicitly specified. See the section on virtual machine migration for more information on modifying this value.
+
+        > **NOTE:** Datastores cannot be assigned to individual disks when `datastore_cluster_id` is used.
         """
         return pulumi.get(self, "datastore_id")
 
     @property
     @pulumi.getter(name="deviceAddress")
     def device_address(self) -> Optional[str]:
         return pulumi.get(self, "device_address")
 
     @property
     @pulumi.getter(name="diskMode")
     def disk_mode(self) -> Optional[str]:
         """
         The mode of this this virtual disk for purposes of writes and snapshots. One of `append`, `independent_nonpersistent`, `independent_persistent`, `nonpersistent`, `persistent`, or `undoable`. Default: `persistent`. For more information on these option, please refer to the [product documentation][vmware-docs-disk-mode].
+
+        [vmware-docs-disk-mode]: https://vdc-download.vmware.com/vmwb-repository/dcr-public/da47f910-60ac-438b-8b9b-6122f4d14524/16b7274a-bf8b-4b4c-a05e-746f2aa93c8c/doc/vim.vm.device.VirtualDiskOption.DiskMode.html
         """
         return pulumi.get(self, "disk_mode")
 
     @property
     @pulumi.getter(name="diskSharing")
     def disk_sharing(self) -> Optional[str]:
         """
         The sharing mode of this virtual disk. One of `sharingMultiWriter` or `sharingNone`. Default: `sharingNone`.
+
+        > **NOTE:** Disk sharing is only available on vSphere 6.0 and later.
         """
         return pulumi.get(self, "disk_sharing")
 
     @property
     @pulumi.getter(name="eagerlyScrub")
     def eagerly_scrub(self) -> Optional[bool]:
         """
@@ -1384,14 +1468,18 @@
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def path(self) -> Optional[str]:
         """
         When using `attach`, this parameter controls the path of a virtual disk to attach externally. Otherwise, it is a computed attribute that contains the virtual disk filename.
+
+        > **NOTE:** Either `client_device` (for a remote backed CD-ROM) or `datastore_id` and `path` (for a datastore ISO backed CD-ROM) are required to .
+
+        > **NOTE:** Some CD-ROM drive types are not supported by this resource, such as pass-through devices. If these drives are present in a cloned template, or added outside of the provider, the desired state will be corrected to the defined device, or removed if no `cdrom` block is present.
         """
         return pulumi.get(self, "path")
 
     @property
     @pulumi.getter
     def size(self) -> Optional[int]:
         """
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/provider.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/resource_pool.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/resource_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/role.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/storage_drs_vm_override.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/storage_drs_vm_override.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/tag.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/tag_category.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/tag_category.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,17 @@
                valid to be assigned to. For a full list, click
                here.
         :param pulumi.Input[str] cardinality: The number of tags that can be assigned from this
                category to a single object at once. Can be one of `SINGLE` (object can only
                be assigned one tag in this category), to `MULTIPLE` (object can be assigned
                multiple tags in this category). Forces a new resource if changed.
         :param pulumi.Input[str] description: A description for the category.
+               
+               > **NOTE:** You can add associable types to a category, but you cannot remove
+               them. Attempting to do so will result in an error.
         :param pulumi.Input[str] name: The name of the category.
         """
         pulumi.set(__self__, "associable_types", associable_types)
         pulumi.set(__self__, "cardinality", cardinality)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if name is not None:
@@ -67,14 +70,17 @@
         pulumi.set(self, "cardinality", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
         A description for the category.
+
+        > **NOTE:** You can add associable types to a category, but you cannot remove
+        them. Attempting to do so will result in an error.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
@@ -104,14 +110,17 @@
                valid to be assigned to. For a full list, click
                here.
         :param pulumi.Input[str] cardinality: The number of tags that can be assigned from this
                category to a single object at once. Can be one of `SINGLE` (object can only
                be assigned one tag in this category), to `MULTIPLE` (object can be assigned
                multiple tags in this category). Forces a new resource if changed.
         :param pulumi.Input[str] description: A description for the category.
+               
+               > **NOTE:** You can add associable types to a category, but you cannot remove
+               them. Attempting to do so will result in an error.
         :param pulumi.Input[str] name: The name of the category.
         """
         if associable_types is not None:
             pulumi.set(__self__, "associable_types", associable_types)
         if cardinality is not None:
             pulumi.set(__self__, "cardinality", cardinality)
         if description is not None:
@@ -149,14 +158,17 @@
         pulumi.set(self, "cardinality", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
         A description for the category.
+
+        > **NOTE:** You can add associable types to a category, but you cannot remove
+        them. Attempting to do so will result in an error.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
@@ -191,14 +203,17 @@
                valid to be assigned to. For a full list, click
                here.
         :param pulumi.Input[str] cardinality: The number of tags that can be assigned from this
                category to a single object at once. Can be one of `SINGLE` (object can only
                be assigned one tag in this category), to `MULTIPLE` (object can be assigned
                multiple tags in this category). Forces a new resource if changed.
         :param pulumi.Input[str] description: A description for the category.
+               
+               > **NOTE:** You can add associable types to a category, but you cannot remove
+               them. Attempting to do so will result in an error.
         :param pulumi.Input[str] name: The name of the category.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: TagCategoryArgs,
@@ -266,14 +281,17 @@
                valid to be assigned to. For a full list, click
                here.
         :param pulumi.Input[str] cardinality: The number of tags that can be assigned from this
                category to a single object at once. Can be one of `SINGLE` (object can only
                be assigned one tag in this category), to `MULTIPLE` (object can be assigned
                multiple tags in this category). Forces a new resource if changed.
         :param pulumi.Input[str] description: A description for the category.
+               
+               > **NOTE:** You can add associable types to a category, but you cannot remove
+               them. Attempting to do so will result in an error.
         :param pulumi.Input[str] name: The name of the category.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _TagCategoryState.__new__(_TagCategoryState)
 
         __props__.__dict__["associable_types"] = associable_types
@@ -304,14 +322,17 @@
         return pulumi.get(self, "cardinality")
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
         A description for the category.
+
+        > **NOTE:** You can add associable types to a category, but you cannot remove
+        them. Attempting to do so will result in an error.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/vapp_container.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/vapp_container.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/vapp_entity.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/vapp_entity.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/virtual_disk.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/virtual_disk.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,24 +26,37 @@
         :param pulumi.Input[str] datastore: The name of the datastore in which to create the
                disk.
         :param pulumi.Input[int] size: Size of the disk (in GB).
         :param pulumi.Input[str] vmdk_path: The path, including filename, of the virtual disk to
                be created.  This needs to end in `.vmdk`.
         :param pulumi.Input[str] adapter_type: The adapter type for this virtual disk. Can be
                one of `ide`, `lsiLogic`, or `busLogic`.  Default: `lsiLogic`.
+               
+               > **NOTE:** `adapter_type` is **deprecated**: it does not dictate the type of
+               controller that the virtual disk will be attached to on the virtual machine.
+               Please see the `scsi_type` parameter
+               in the `VirtualMachine` resource for information on how to control
+               disk controller types. This parameter will be removed in future versions of the
+               vSphere provider.
         :param pulumi.Input[bool] create_directories: Tells the resource to create any
                directories that are a part of the `vmdk_path` parameter if they are missing.
                Default: `false`.
+               
+               > **NOTE:** Any directory created as part of the operation when
+               `create_directories` is enabled will not be deleted when the resource is
+               destroyed.
         :param pulumi.Input[str] datacenter: The name of the datacenter in which to create the
                disk. Can be omitted when when ESXi or if there is only one datacenter in
                your infrastructure.
         :param pulumi.Input[str] type: The type of disk to create. Can be one of
                `eagerZeroedThick`, `lazy`, or `thin`. Default: `eagerZeroedThick`. For
                information on what each kind of disk provisioning policy means, click
                [here][docs-vmware-vm-disk-provisioning].
+               
+               [docs-vmware-vm-disk-provisioning]: https://docs.vmware.com/en/VMware-vSphere/7.0/com.vmware.vsphere.vm_admin.doc/GUID-4C0F4D73-82F2-4B81-8AA7-1DD752A8A5AC.html
         """
         pulumi.set(__self__, "datastore", datastore)
         pulumi.set(__self__, "size", size)
         pulumi.set(__self__, "vmdk_path", vmdk_path)
         if adapter_type is not None:
             warnings.warn("""this attribute has no effect on controller types - please use scsi_type in vsphere_virtual_machine instead""", DeprecationWarning)
             pulumi.log.warn("""adapter_type is deprecated: this attribute has no effect on controller types - please use scsi_type in vsphere_virtual_machine instead""")
@@ -96,28 +109,39 @@
 
     @property
     @pulumi.getter(name="adapterType")
     def adapter_type(self) -> Optional[pulumi.Input[str]]:
         """
         The adapter type for this virtual disk. Can be
         one of `ide`, `lsiLogic`, or `busLogic`.  Default: `lsiLogic`.
+
+        > **NOTE:** `adapter_type` is **deprecated**: it does not dictate the type of
+        controller that the virtual disk will be attached to on the virtual machine.
+        Please see the `scsi_type` parameter
+        in the `VirtualMachine` resource for information on how to control
+        disk controller types. This parameter will be removed in future versions of the
+        vSphere provider.
         """
         return pulumi.get(self, "adapter_type")
 
     @adapter_type.setter
     def adapter_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "adapter_type", value)
 
     @property
     @pulumi.getter(name="createDirectories")
     def create_directories(self) -> Optional[pulumi.Input[bool]]:
         """
         Tells the resource to create any
         directories that are a part of the `vmdk_path` parameter if they are missing.
         Default: `false`.
+
+        > **NOTE:** Any directory created as part of the operation when
+        `create_directories` is enabled will not be deleted when the resource is
+        destroyed.
         """
         return pulumi.get(self, "create_directories")
 
     @create_directories.setter
     def create_directories(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "create_directories", value)
 
@@ -139,14 +163,16 @@
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
         The type of disk to create. Can be one of
         `eagerZeroedThick`, `lazy`, or `thin`. Default: `eagerZeroedThick`. For
         information on what each kind of disk provisioning policy means, click
         [here][docs-vmware-vm-disk-provisioning].
+
+        [docs-vmware-vm-disk-provisioning]: https://docs.vmware.com/en/VMware-vSphere/7.0/com.vmware.vsphere.vm_admin.doc/GUID-4C0F4D73-82F2-4B81-8AA7-1DD752A8A5AC.html
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -161,27 +187,40 @@
                  size: Optional[pulumi.Input[int]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  vmdk_path: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering VirtualDisk resources.
         :param pulumi.Input[str] adapter_type: The adapter type for this virtual disk. Can be
                one of `ide`, `lsiLogic`, or `busLogic`.  Default: `lsiLogic`.
+               
+               > **NOTE:** `adapter_type` is **deprecated**: it does not dictate the type of
+               controller that the virtual disk will be attached to on the virtual machine.
+               Please see the `scsi_type` parameter
+               in the `VirtualMachine` resource for information on how to control
+               disk controller types. This parameter will be removed in future versions of the
+               vSphere provider.
         :param pulumi.Input[bool] create_directories: Tells the resource to create any
                directories that are a part of the `vmdk_path` parameter if they are missing.
                Default: `false`.
+               
+               > **NOTE:** Any directory created as part of the operation when
+               `create_directories` is enabled will not be deleted when the resource is
+               destroyed.
         :param pulumi.Input[str] datacenter: The name of the datacenter in which to create the
                disk. Can be omitted when when ESXi or if there is only one datacenter in
                your infrastructure.
         :param pulumi.Input[str] datastore: The name of the datastore in which to create the
                disk.
         :param pulumi.Input[int] size: Size of the disk (in GB).
         :param pulumi.Input[str] type: The type of disk to create. Can be one of
                `eagerZeroedThick`, `lazy`, or `thin`. Default: `eagerZeroedThick`. For
                information on what each kind of disk provisioning policy means, click
                [here][docs-vmware-vm-disk-provisioning].
+               
+               [docs-vmware-vm-disk-provisioning]: https://docs.vmware.com/en/VMware-vSphere/7.0/com.vmware.vsphere.vm_admin.doc/GUID-4C0F4D73-82F2-4B81-8AA7-1DD752A8A5AC.html
         :param pulumi.Input[str] vmdk_path: The path, including filename, of the virtual disk to
                be created.  This needs to end in `.vmdk`.
         """
         if adapter_type is not None:
             warnings.warn("""this attribute has no effect on controller types - please use scsi_type in vsphere_virtual_machine instead""", DeprecationWarning)
             pulumi.log.warn("""adapter_type is deprecated: this attribute has no effect on controller types - please use scsi_type in vsphere_virtual_machine instead""")
         if adapter_type is not None:
@@ -201,28 +240,39 @@
 
     @property
     @pulumi.getter(name="adapterType")
     def adapter_type(self) -> Optional[pulumi.Input[str]]:
         """
         The adapter type for this virtual disk. Can be
         one of `ide`, `lsiLogic`, or `busLogic`.  Default: `lsiLogic`.
+
+        > **NOTE:** `adapter_type` is **deprecated**: it does not dictate the type of
+        controller that the virtual disk will be attached to on the virtual machine.
+        Please see the `scsi_type` parameter
+        in the `VirtualMachine` resource for information on how to control
+        disk controller types. This parameter will be removed in future versions of the
+        vSphere provider.
         """
         return pulumi.get(self, "adapter_type")
 
     @adapter_type.setter
     def adapter_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "adapter_type", value)
 
     @property
     @pulumi.getter(name="createDirectories")
     def create_directories(self) -> Optional[pulumi.Input[bool]]:
         """
         Tells the resource to create any
         directories that are a part of the `vmdk_path` parameter if they are missing.
         Default: `false`.
+
+        > **NOTE:** Any directory created as part of the operation when
+        `create_directories` is enabled will not be deleted when the resource is
+        destroyed.
         """
         return pulumi.get(self, "create_directories")
 
     @create_directories.setter
     def create_directories(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "create_directories", value)
 
@@ -269,14 +319,16 @@
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
         The type of disk to create. Can be one of
         `eagerZeroedThick`, `lazy`, or `thin`. Default: `eagerZeroedThick`. For
         information on what each kind of disk provisioning policy means, click
         [here][docs-vmware-vm-disk-provisioning].
+
+        [docs-vmware-vm-disk-provisioning]: https://docs.vmware.com/en/VMware-vSphere/7.0/com.vmware.vsphere.vm_admin.doc/GUID-4C0F4D73-82F2-4B81-8AA7-1DD752A8A5AC.html
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -309,27 +361,40 @@
                  __props__=None):
         """
         Create a VirtualDisk resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] adapter_type: The adapter type for this virtual disk. Can be
                one of `ide`, `lsiLogic`, or `busLogic`.  Default: `lsiLogic`.
+               
+               > **NOTE:** `adapter_type` is **deprecated**: it does not dictate the type of
+               controller that the virtual disk will be attached to on the virtual machine.
+               Please see the `scsi_type` parameter
+               in the `VirtualMachine` resource for information on how to control
+               disk controller types. This parameter will be removed in future versions of the
+               vSphere provider.
         :param pulumi.Input[bool] create_directories: Tells the resource to create any
                directories that are a part of the `vmdk_path` parameter if they are missing.
                Default: `false`.
+               
+               > **NOTE:** Any directory created as part of the operation when
+               `create_directories` is enabled will not be deleted when the resource is
+               destroyed.
         :param pulumi.Input[str] datacenter: The name of the datacenter in which to create the
                disk. Can be omitted when when ESXi or if there is only one datacenter in
                your infrastructure.
         :param pulumi.Input[str] datastore: The name of the datastore in which to create the
                disk.
         :param pulumi.Input[int] size: Size of the disk (in GB).
         :param pulumi.Input[str] type: The type of disk to create. Can be one of
                `eagerZeroedThick`, `lazy`, or `thin`. Default: `eagerZeroedThick`. For
                information on what each kind of disk provisioning policy means, click
                [here][docs-vmware-vm-disk-provisioning].
+               
+               [docs-vmware-vm-disk-provisioning]: https://docs.vmware.com/en/VMware-vSphere/7.0/com.vmware.vsphere.vm_admin.doc/GUID-4C0F4D73-82F2-4B81-8AA7-1DD752A8A5AC.html
         :param pulumi.Input[str] vmdk_path: The path, including filename, of the virtual disk to
                be created.  This needs to end in `.vmdk`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -406,27 +471,40 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] adapter_type: The adapter type for this virtual disk. Can be
                one of `ide`, `lsiLogic`, or `busLogic`.  Default: `lsiLogic`.
+               
+               > **NOTE:** `adapter_type` is **deprecated**: it does not dictate the type of
+               controller that the virtual disk will be attached to on the virtual machine.
+               Please see the `scsi_type` parameter
+               in the `VirtualMachine` resource for information on how to control
+               disk controller types. This parameter will be removed in future versions of the
+               vSphere provider.
         :param pulumi.Input[bool] create_directories: Tells the resource to create any
                directories that are a part of the `vmdk_path` parameter if they are missing.
                Default: `false`.
+               
+               > **NOTE:** Any directory created as part of the operation when
+               `create_directories` is enabled will not be deleted when the resource is
+               destroyed.
         :param pulumi.Input[str] datacenter: The name of the datacenter in which to create the
                disk. Can be omitted when when ESXi or if there is only one datacenter in
                your infrastructure.
         :param pulumi.Input[str] datastore: The name of the datastore in which to create the
                disk.
         :param pulumi.Input[int] size: Size of the disk (in GB).
         :param pulumi.Input[str] type: The type of disk to create. Can be one of
                `eagerZeroedThick`, `lazy`, or `thin`. Default: `eagerZeroedThick`. For
                information on what each kind of disk provisioning policy means, click
                [here][docs-vmware-vm-disk-provisioning].
+               
+               [docs-vmware-vm-disk-provisioning]: https://docs.vmware.com/en/VMware-vSphere/7.0/com.vmware.vsphere.vm_admin.doc/GUID-4C0F4D73-82F2-4B81-8AA7-1DD752A8A5AC.html
         :param pulumi.Input[str] vmdk_path: The path, including filename, of the virtual disk to
                be created.  This needs to end in `.vmdk`.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _VirtualDiskState.__new__(_VirtualDiskState)
 
@@ -441,24 +519,35 @@
 
     @property
     @pulumi.getter(name="adapterType")
     def adapter_type(self) -> pulumi.Output[Optional[str]]:
         """
         The adapter type for this virtual disk. Can be
         one of `ide`, `lsiLogic`, or `busLogic`.  Default: `lsiLogic`.
+
+        > **NOTE:** `adapter_type` is **deprecated**: it does not dictate the type of
+        controller that the virtual disk will be attached to on the virtual machine.
+        Please see the `scsi_type` parameter
+        in the `VirtualMachine` resource for information on how to control
+        disk controller types. This parameter will be removed in future versions of the
+        vSphere provider.
         """
         return pulumi.get(self, "adapter_type")
 
     @property
     @pulumi.getter(name="createDirectories")
     def create_directories(self) -> pulumi.Output[Optional[bool]]:
         """
         Tells the resource to create any
         directories that are a part of the `vmdk_path` parameter if they are missing.
         Default: `false`.
+
+        > **NOTE:** Any directory created as part of the operation when
+        `create_directories` is enabled will not be deleted when the resource is
+        destroyed.
         """
         return pulumi.get(self, "create_directories")
 
     @property
     @pulumi.getter
     def datacenter(self) -> pulumi.Output[Optional[str]]:
         """
@@ -489,14 +578,16 @@
     @pulumi.getter
     def type(self) -> pulumi.Output[Optional[str]]:
         """
         The type of disk to create. Can be one of
         `eagerZeroedThick`, `lazy`, or `thin`. Default: `eagerZeroedThick`. For
         information on what each kind of disk provisioning policy means, click
         [here][docs-vmware-vm-disk-provisioning].
+
+        [docs-vmware-vm-disk-provisioning]: https://docs.vmware.com/en/VMware-vSphere/7.0/com.vmware.vsphere.vm_admin.doc/GUID-4C0F4D73-82F2-4B81-8AA7-1DD752A8A5AC.html
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter(name="vmdkPath")
     def vmdk_path(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/virtual_machine.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/virtual_machine.py`

 * *Files 12% similar despite different names*

```diff
@@ -89,14 +89,16 @@
                  vvtd_enabled: Optional[pulumi.Input[bool]] = None,
                  wait_for_guest_ip_timeout: Optional[pulumi.Input[int]] = None,
                  wait_for_guest_net_routable: Optional[pulumi.Input[bool]] = None,
                  wait_for_guest_net_timeout: Optional[pulumi.Input[int]] = None):
         """
         The set of arguments for constructing a VirtualMachine resource.
         :param pulumi.Input[str] resource_pool_id: The managed object reference ID of the resource pool in which to place the virtual machine. See the Virtual Machine Migration section for more information on modifying this value.
+               
+               > **NOTE:** All clusters and standalone hosts have a default root resource pool. This resource argument does not directly accept the cluster or standalone host resource. For more information, see the section on specifying the Root Resource Pool in the `ResourcePool` data source documentation on using the root resource pool.
         :param pulumi.Input[str] alternate_guest_name: The guest name for the operating system when `guest_id` is `otherGuest` or `otherGuest64`.
         :param pulumi.Input[str] annotation: A user-provided description of the virtual machine.
         :param pulumi.Input[int] boot_delay: The number of milliseconds to wait before starting the boot sequence. The default is no delay.
         :param pulumi.Input[int] boot_retry_delay: The number of milliseconds to wait before retrying the boot sequence. This option is only valid if `boot_retry_enabled` is `true`. Default: `10000` (10 seconds).
         :param pulumi.Input[bool] boot_retry_enabled: If set to `true`, a virtual machine that fails to boot will try again after the delay defined in `boot_retry_delay`. Default: `false`.
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineCdromArgs']]] cdroms: A specification for a CD-ROM device on the virtual machine. See CD-ROM options for more information.
         :param pulumi.Input['VirtualMachineCloneArgs'] clone: When specified, the virtual machine will be created as a clone of a specified template. Optional customization options can be submitted for the resource. See creating a virtual machine from a template for more information.
@@ -104,50 +106,82 @@
         :param pulumi.Input[bool] cpu_hot_remove_enabled: Allow CPUs to be removed to the virtual machine while it is powered on.
         :param pulumi.Input[int] cpu_limit: The maximum amount of CPU (in MHz) that the virtual machine can consume, regardless of available resources. The default is no limit.
         :param pulumi.Input[bool] cpu_performance_counters_enabled: Enable CPU performance counters on the virtual machine. Default: `false`.
         :param pulumi.Input[int] cpu_reservation: The amount of CPU (in MHz) that the virtual machine is guaranteed. The default is no reservation.
         :param pulumi.Input[int] cpu_share_count: The number of CPU shares allocated to the virtual machine when the `cpu_share_level` is `custom`.
         :param pulumi.Input[str] cpu_share_level: The allocation level for the virtual machine CPU resources. One of `high`, `low`, `normal`, or `custom`. Default: `custom`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to attribute value strings to set for virtual machine. Please refer to the `vsphere_custom_attributes` resource for more information on setting custom attributes.
+               
+               > **NOTE:** Custom attributes requires vCenter Server and is not supported on direct ESXi host connections.
         :param pulumi.Input[str] datacenter_id: The datacenter ID. Required only when deploying an OVF/OVA template.
         :param pulumi.Input[str] datastore_cluster_id: The managed object reference ID of the datastore cluster in which to place the virtual machine. This setting applies to entire virtual machine and implies that you wish to use vSphere Storage DRS with the virtual machine. See the section on virtual machine migration for more information on modifying this value.
+               
+               > **NOTE:** One of `datastore_id` or `datastore_cluster_id` must be specified.
+               
+               > **NOTE:** Use of `datastore_cluster_id` requires vSphere Storage DRS to be enabled on the specified datastore cluster.
+               
+               > **NOTE:** The `datastore_cluster_id` setting applies to the entire virtual machine resource. You cannot assign individual individual disks to datastore clusters. In addition, you cannot use the `attach` setting to attach external disks on virtual machines that are assigned to datastore clusters.
         :param pulumi.Input[str] datastore_id: The managed object reference ID of the datastore in which to place the virtual machine. The virtual machine configuration files is placed here, along with any virtual disks that are created where a datastore is not explicitly specified. See the section on virtual machine migration for more information on modifying this value.
+               
+               > **NOTE:** Datastores cannot be assigned to individual disks when `datastore_cluster_id` is used.
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineDiskArgs']]] disks: A specification for a virtual disk device on the virtual machine. See disk options for more information.
         :param pulumi.Input[bool] efi_secure_boot_enabled: Use this option to enable EFI secure boot when the `firmware` type is set to is `efi`. Default: `false`.
+               
+               > **NOTE:** EFI secure boot is only available on vSphere 6.5 and later.
         :param pulumi.Input[bool] enable_disk_uuid: Expose the UUIDs of attached virtual disks to the virtual machine, allowing access to them in the guest. Default: `false`.
         :param pulumi.Input[bool] enable_logging: Enable logging of virtual machine events to a log file stored in the virtual machine directory. Default: `false`.
         :param pulumi.Input[str] ept_rvi_mode: The EPT/RVI (hardware memory virtualization) setting for the virtual machine. One of `automatic`, `on`, or `off`. Default: `automatic`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] extra_config: Extra configuration data for the virtual machine. Can be used to supply advanced parameters not normally in configuration, such as instance metadata and userdata.
+               
+               > **NOTE:** Do not use `extra_config` when working with a template imported from OVF/OVA as your settings may be ignored. Use the `vapp` block `properties` section as described in Using vApp Properties for OVF/OVA Configuration.
         :param pulumi.Input[bool] extra_config_reboot_required: Allow the virtual machine to be rebooted when a change to `extra_config` occurs. Default: `true`.
         :param pulumi.Input[str] firmware: The firmware for the virtual machine. One of `bios` or `efi`.
         :param pulumi.Input[str] folder: The path to the virtual machine folder in which to place the virtual machine, relative to the datacenter path (`/<datacenter-name>/vm`).  For example, `/dc-01/vm/foo`
         :param pulumi.Input[bool] force_power_off: If a guest shutdown failed or times out while updating or destroying (see `shutdown_wait_timeout`), force the power-off of the virtual machine. Default: `true`.
         :param pulumi.Input[str] guest_id: The guest ID for the operating system type. For a full list of possible values, see [here][vmware-docs-guest-ids]. Default: `otherGuest64`.
+               
+               [vmware-docs-guest-ids]: https://vdc-download.vmware.com/vmwb-repository/dcr-public/b50dcbbf-051d-4204-a3e7-e1b618c1e384/538cf2ec-b34f-4bae-a332-3820ef9e7773/vim.vm.GuestOsDescriptor.GuestOsIdentifier.html
         :param pulumi.Input[int] hardware_version: The hardware version number. Valid range is from 4 to 19. The hardware version cannot be downgraded. See [virtual machine hardware compatibility][virtual-machine-hardware-compatibility] for more information.
+               
+               [virtual-machine-hardware-compatibility]: https://kb.vmware.com/s/article/2007240
         :param pulumi.Input[str] host_system_id: The managed object reference ID of a host on which to place the virtual machine. See the section on virtual machine migration for more information on modifying this value. When using a vSphere cluster, if a `host_system_id` is not supplied, vSphere will select a host in the cluster to place the virtual machine, according to any defaults or vSphere DRS placement policies.
         :param pulumi.Input[str] hv_mode: The hardware virtualization (non-nested) setting for the virtual machine. One of `hvAuto`, `hvOn`, or `hvOff`. Default: `hvAuto`.
         :param pulumi.Input[int] ide_controller_count: The number of IDE controllers that the virtual machine. This directly affects the number of disks you can add to the virtual machine and the maximum disk unit number. Note that lowering this value does not remove controllers. Default: `2`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ignored_guest_ips: List of IP addresses and CIDR networks to ignore while waiting for an available IP address using either of the waiters. Any IP addresses in this list will be ignored so that the waiter will continue to wait for a valid IP address. Default: `[]`.
         :param pulumi.Input[str] latency_sensitivity: Controls the scheduling delay of the virtual machine. Use a higher sensitivity for applications that require lower latency, such as VOIP, media player applications, or applications that require frequent access to mouse or keyboard devices. One of `low`, `normal`, `medium`, or `high`.
+               
+               > **NOTE:** On higher sensitivities, you may need to adjust the `memory_reservation` to the full amount of memory provisioned for the virtual machine.
         :param pulumi.Input[int] memory: The memory size to assign to the virtual machine, in MB. Default: `1024` (1 GB).
         :param pulumi.Input[bool] memory_hot_add_enabled: Allow memory to be added to the virtual machine while it is powered on.
+               
+               > **NOTE:** CPU and memory hot add options are not available on all guest operating systems. Please refer to the [VMware Guest OS Compatibility Guide][vmware-docs-compat-guide] to which settings are allow for your guest operating system. In addition, at least one `pulumi up` must be run before you are able to use CPU and memory hot add.
+               
+               [vmware-docs-compat-guide]: http://partnerweb.vmware.com/comp_guide2/pdf/VMware_GOS_Compatibility_Guide.pdf
+               
+               > **NOTE:** For Linux 64-bit guest operating systems with less than or equal to 3GB, the virtual machine must powered off to add memory beyond 3GB. Subsequent hot add of memory does not require the virtual machine to be powered-off to apply the plan. Please refer to [VMware KB 2008405][vmware-kb-2008405].
+               
+               [vmware-kb-2008405]: https://kb.vmware.com/s/article/2008405
         :param pulumi.Input[int] memory_limit: The maximum amount of memory (in MB) that th virtual machine can consume, regardless of available resources. The default is no limit.
         :param pulumi.Input[int] memory_reservation: The amount of memory (in MB) that the virtual machine is guaranteed. The default is no reservation.
         :param pulumi.Input[int] memory_share_count: The number of memory shares allocated to the virtual machine when the `memory_share_level` is `custom`.
         :param pulumi.Input[str] memory_share_level: The allocation level for the virtual machine memory resources. One of `high`, `low`, `normal`, or `custom`. Default: `custom`.
         :param pulumi.Input[int] migrate_wait_timeout: The amount of time, in minutes, to wait for a virtual machine migration to complete before failing. Default: `10` minutes. See the section on virtual machine migration for more information.
         :param pulumi.Input[str] name: The name of the virtual machine.
         :param pulumi.Input[bool] nested_hv_enabled: Enable nested hardware virtualization on the virtual machine, facilitating nested virtualization in the guest operating system. Default: `false`.
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineNetworkInterfaceArgs']]] network_interfaces: A specification for a virtual NIC on the virtual machine. See network interface options for more information.
         :param pulumi.Input[int] num_cores_per_socket: The number of cores per socket in the virtual machine. The number of vCPUs on the virtual machine will be `num_cpus` divided by `num_cores_per_socket`. If specified, the value supplied to `num_cpus` must be evenly divisible by this value. Default: `1`.
         :param pulumi.Input[int] num_cpus: The total number of virtual processor cores to assign to the virtual machine. Default: `1`.
         :param pulumi.Input['VirtualMachineOvfDeployArgs'] ovf_deploy: When specified, the virtual machine will be deployed from the provided OVF/OVA template. See creating a virtual machine from an OVF/OVA template for more information.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] pci_device_ids: List of host PCI device IDs in which to create PCI passthroughs.
+               
+               > **NOTE:** Cloning requires vCenter Server and is not supported on direct ESXi host connections.
         :param pulumi.Input[int] poweron_timeout: The amount of time, in seconds, that we will be trying to power on a VM
         :param pulumi.Input[str] replace_trigger: Triggers replacement of resource whenever it changes.
+               
+               For example, `replace_trigger = sha256(format("%s-%s",data.template_file.cloud_init_metadata.rendered,data.template_file.cloud_init_userdata.rendered))` will fingerprint the changes in cloud-init metadata and userdata templates. This will enable a replacement of the resource whenever the dependant template renders a new configuration. (Forces a replacement.)
         :param pulumi.Input[bool] run_tools_scripts_after_power_on: Enable post-power-on scripts to run when VMware Tools is installed. Default: `true`.
         :param pulumi.Input[bool] run_tools_scripts_after_resume: Enable ost-resume scripts to run when VMware Tools is installed. Default: `true`.
         :param pulumi.Input[bool] run_tools_scripts_before_guest_reboot: Enable pre-reboot scripts to run when VMware Tools is installed. Default: `false`.
         :param pulumi.Input[bool] run_tools_scripts_before_guest_shutdown: Enable pre-shutdown scripts to run when VMware Tools is installed. Default: `true`.
         :param pulumi.Input[bool] run_tools_scripts_before_guest_standby: Enable pre-standby scripts to run when VMware Tools is installed. Default: `true`.
         :param pulumi.Input[int] sata_controller_count: The number of SATA controllers that Terraform manages on this virtual machine. This directly affects the amount of disks
                you can add to the virtual machine and the maximum disk unit number. Note that lowering this value does not remove
@@ -159,14 +193,16 @@
         :param pulumi.Input[str] scsi_type: The SCSI controller type for the virtual machine. One of `lsilogic` (LSI Logic Parallel), `lsilogic-sas` (LSI Logic SAS) or `pvscsi` (VMware Paravirtual). Default: `pvscsi`.
         :param pulumi.Input[int] shutdown_wait_timeout: The amount of time, in minutes, to wait for a graceful guest shutdown when making necessary updates to the virtual machine. If `force_power_off` is set to `true`, the virtual machine will be forced to power-off after the timeout, otherwise an error is returned. Default: `3` minutes.
         :param pulumi.Input[str] storage_policy_id: The ID of the storage policy to assign to the home directory of a virtual machine.
         :param pulumi.Input[str] swap_placement_policy: The swap file placement policy for the virtual machine. One of `inherit`, `hostLocal`, or `vmDirectory`. Default: `inherit`.
         :param pulumi.Input[bool] sync_time_with_host: Enable the guest operating system to synchronization its clock with the host when the virtual machine is powered on or resumed. Requires vSphere 7.0 Update 1 and later. Requires VMware Tools to be installed. Default: `false`.
         :param pulumi.Input[bool] sync_time_with_host_periodically: Enable the guest operating system to periodically synchronize its clock with the host. Requires vSphere 7.0 Update 1 and later. On previous versions, setting `sync_time_with_host` is will enable periodic synchronization. Requires VMware Tools to be installed. Default: `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource. Please refer to the `Tag` resource for more information on applying tags to virtual machine resources.
+               
+               > **NOTE:** Tagging support is unsupported on direct ESXi host connections and requires vCenter Server instance.
         :param pulumi.Input[str] tools_upgrade_policy: Enable automatic upgrade of the VMware Tools version when the virtual machine is rebooted. If necessary, VMware Tools is upgraded to the latest version supported by the host on which the virtual machine is running. Requires VMware Tools to be installed. One of `manual` or `upgradeAtPowerCycle`. Default: `manual`.
         :param pulumi.Input['VirtualMachineVappArgs'] vapp: Used for vApp configurations. The only sub-key available is `properties`, which is a key/value map of properties for virtual machines imported from and OVF/OVA. See Using vApp Properties for OVF/OVA Configuration for more information.
         :param pulumi.Input[bool] vbs_enabled: Enable Virtualization Based Security. Requires `firmware` to be `efi`. In addition, `vvtd_enabled`, `nested_hv_enabled`, and `efi_secure_boot_enabled` must all have a value of `true`. Supported on vSphere 6.7 and later. Default: `false`.
         :param pulumi.Input[bool] vvtd_enabled: Enable Intel Virtualization Technology for Directed I/O for the virtual machine (_I/O MMU_ in the vSphere Client). Supported on vSphere 6.7 and later. Default: `false`.
         :param pulumi.Input[int] wait_for_guest_ip_timeout: The amount of time, in minutes, to wait for an available guest IP address on the virtual machine. This should only be used if the version VMware Tools does not allow the `wait_for_guest_net_timeout` waiter to be used. A value less than `1` disables the waiter. Default: `0`.
         :param pulumi.Input[bool] wait_for_guest_net_routable: Controls whether or not the guest network waiter waits for a routable address. When `false`, the waiter does not wait for a default gateway, nor are IP addresses checked against any discovered default gateways as part of its success criteria. This property is ignored if the `wait_for_guest_ip_timeout` waiter is used. Default: `true`.
         :param pulumi.Input[int] wait_for_guest_net_timeout: The amount of time, in minutes, to wait for an available guest IP address on the virtual machine. Older versions of VMware Tools do not populate this property. In those cases, this waiter can be disabled and the `wait_for_guest_ip_timeout` waiter can be used instead. A value less than `1` disables the waiter. Default: `5` minutes.
@@ -320,14 +356,16 @@
             pulumi.set(__self__, "wait_for_guest_net_timeout", wait_for_guest_net_timeout)
 
     @property
     @pulumi.getter(name="resourcePoolId")
     def resource_pool_id(self) -> pulumi.Input[str]:
         """
         The managed object reference ID of the resource pool in which to place the virtual machine. See the Virtual Machine Migration section for more information on modifying this value.
+
+        > **NOTE:** All clusters and standalone hosts have a default root resource pool. This resource argument does not directly accept the cluster or standalone host resource. For more information, see the section on specifying the Root Resource Pool in the `ResourcePool` data source documentation on using the root resource pool.
         """
         return pulumi.get(self, "resource_pool_id")
 
     @resource_pool_id.setter
     def resource_pool_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "resource_pool_id", value)
 
@@ -500,14 +538,16 @@
         pulumi.set(self, "cpu_share_level", value)
 
     @property
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Map of custom attribute ids to attribute value strings to set for virtual machine. Please refer to the `vsphere_custom_attributes` resource for more information on setting custom attributes.
+
+        > **NOTE:** Custom attributes requires vCenter Server and is not supported on direct ESXi host connections.
         """
         return pulumi.get(self, "custom_attributes")
 
     @custom_attributes.setter
     def custom_attributes(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "custom_attributes", value)
 
@@ -524,26 +564,34 @@
         pulumi.set(self, "datacenter_id", value)
 
     @property
     @pulumi.getter(name="datastoreClusterId")
     def datastore_cluster_id(self) -> Optional[pulumi.Input[str]]:
         """
         The managed object reference ID of the datastore cluster in which to place the virtual machine. This setting applies to entire virtual machine and implies that you wish to use vSphere Storage DRS with the virtual machine. See the section on virtual machine migration for more information on modifying this value.
+
+        > **NOTE:** One of `datastore_id` or `datastore_cluster_id` must be specified.
+
+        > **NOTE:** Use of `datastore_cluster_id` requires vSphere Storage DRS to be enabled on the specified datastore cluster.
+
+        > **NOTE:** The `datastore_cluster_id` setting applies to the entire virtual machine resource. You cannot assign individual individual disks to datastore clusters. In addition, you cannot use the `attach` setting to attach external disks on virtual machines that are assigned to datastore clusters.
         """
         return pulumi.get(self, "datastore_cluster_id")
 
     @datastore_cluster_id.setter
     def datastore_cluster_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "datastore_cluster_id", value)
 
     @property
     @pulumi.getter(name="datastoreId")
     def datastore_id(self) -> Optional[pulumi.Input[str]]:
         """
         The managed object reference ID of the datastore in which to place the virtual machine. The virtual machine configuration files is placed here, along with any virtual disks that are created where a datastore is not explicitly specified. See the section on virtual machine migration for more information on modifying this value.
+
+        > **NOTE:** Datastores cannot be assigned to individual disks when `datastore_cluster_id` is used.
         """
         return pulumi.get(self, "datastore_id")
 
     @datastore_id.setter
     def datastore_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "datastore_id", value)
 
@@ -560,14 +608,16 @@
         pulumi.set(self, "disks", value)
 
     @property
     @pulumi.getter(name="efiSecureBootEnabled")
     def efi_secure_boot_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
         Use this option to enable EFI secure boot when the `firmware` type is set to is `efi`. Default: `false`.
+
+        > **NOTE:** EFI secure boot is only available on vSphere 6.5 and later.
         """
         return pulumi.get(self, "efi_secure_boot_enabled")
 
     @efi_secure_boot_enabled.setter
     def efi_secure_boot_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "efi_secure_boot_enabled", value)
 
@@ -608,14 +658,16 @@
         pulumi.set(self, "ept_rvi_mode", value)
 
     @property
     @pulumi.getter(name="extraConfig")
     def extra_config(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Extra configuration data for the virtual machine. Can be used to supply advanced parameters not normally in configuration, such as instance metadata and userdata.
+
+        > **NOTE:** Do not use `extra_config` when working with a template imported from OVF/OVA as your settings may be ignored. Use the `vapp` block `properties` section as described in Using vApp Properties for OVF/OVA Configuration.
         """
         return pulumi.get(self, "extra_config")
 
     @extra_config.setter
     def extra_config(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "extra_config", value)
 
@@ -668,26 +720,30 @@
         pulumi.set(self, "force_power_off", value)
 
     @property
     @pulumi.getter(name="guestId")
     def guest_id(self) -> Optional[pulumi.Input[str]]:
         """
         The guest ID for the operating system type. For a full list of possible values, see [here][vmware-docs-guest-ids]. Default: `otherGuest64`.
+
+        [vmware-docs-guest-ids]: https://vdc-download.vmware.com/vmwb-repository/dcr-public/b50dcbbf-051d-4204-a3e7-e1b618c1e384/538cf2ec-b34f-4bae-a332-3820ef9e7773/vim.vm.GuestOsDescriptor.GuestOsIdentifier.html
         """
         return pulumi.get(self, "guest_id")
 
     @guest_id.setter
     def guest_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "guest_id", value)
 
     @property
     @pulumi.getter(name="hardwareVersion")
     def hardware_version(self) -> Optional[pulumi.Input[int]]:
         """
         The hardware version number. Valid range is from 4 to 19. The hardware version cannot be downgraded. See [virtual machine hardware compatibility][virtual-machine-hardware-compatibility] for more information.
+
+        [virtual-machine-hardware-compatibility]: https://kb.vmware.com/s/article/2007240
         """
         return pulumi.get(self, "hardware_version")
 
     @hardware_version.setter
     def hardware_version(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "hardware_version", value)
 
@@ -740,14 +796,16 @@
         pulumi.set(self, "ignored_guest_ips", value)
 
     @property
     @pulumi.getter(name="latencySensitivity")
     def latency_sensitivity(self) -> Optional[pulumi.Input[str]]:
         """
         Controls the scheduling delay of the virtual machine. Use a higher sensitivity for applications that require lower latency, such as VOIP, media player applications, or applications that require frequent access to mouse or keyboard devices. One of `low`, `normal`, `medium`, or `high`.
+
+        > **NOTE:** On higher sensitivities, you may need to adjust the `memory_reservation` to the full amount of memory provisioned for the virtual machine.
         """
         return pulumi.get(self, "latency_sensitivity")
 
     @latency_sensitivity.setter
     def latency_sensitivity(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "latency_sensitivity", value)
 
@@ -764,14 +822,22 @@
         pulumi.set(self, "memory", value)
 
     @property
     @pulumi.getter(name="memoryHotAddEnabled")
     def memory_hot_add_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
         Allow memory to be added to the virtual machine while it is powered on.
+
+        > **NOTE:** CPU and memory hot add options are not available on all guest operating systems. Please refer to the [VMware Guest OS Compatibility Guide][vmware-docs-compat-guide] to which settings are allow for your guest operating system. In addition, at least one `pulumi up` must be run before you are able to use CPU and memory hot add.
+
+        [vmware-docs-compat-guide]: http://partnerweb.vmware.com/comp_guide2/pdf/VMware_GOS_Compatibility_Guide.pdf
+
+        > **NOTE:** For Linux 64-bit guest operating systems with less than or equal to 3GB, the virtual machine must powered off to add memory beyond 3GB. Subsequent hot add of memory does not require the virtual machine to be powered-off to apply the plan. Please refer to [VMware KB 2008405][vmware-kb-2008405].
+
+        [vmware-kb-2008405]: https://kb.vmware.com/s/article/2008405
         """
         return pulumi.get(self, "memory_hot_add_enabled")
 
     @memory_hot_add_enabled.setter
     def memory_hot_add_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "memory_hot_add_enabled", value)
 
@@ -908,14 +974,16 @@
         pulumi.set(self, "ovf_deploy", value)
 
     @property
     @pulumi.getter(name="pciDeviceIds")
     def pci_device_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         List of host PCI device IDs in which to create PCI passthroughs.
+
+        > **NOTE:** Cloning requires vCenter Server and is not supported on direct ESXi host connections.
         """
         return pulumi.get(self, "pci_device_ids")
 
     @pci_device_ids.setter
     def pci_device_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "pci_device_ids", value)
 
@@ -932,14 +1000,16 @@
         pulumi.set(self, "poweron_timeout", value)
 
     @property
     @pulumi.getter(name="replaceTrigger")
     def replace_trigger(self) -> Optional[pulumi.Input[str]]:
         """
         Triggers replacement of resource whenever it changes.
+
+        For example, `replace_trigger = sha256(format("%s-%s",data.template_file.cloud_init_metadata.rendered,data.template_file.cloud_init_userdata.rendered))` will fingerprint the changes in cloud-init metadata and userdata templates. This will enable a replacement of the resource whenever the dependant template renders a new configuration. (Forces a replacement.)
         """
         return pulumi.get(self, "replace_trigger")
 
     @replace_trigger.setter
     def replace_trigger(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "replace_trigger", value)
 
@@ -1116,14 +1186,16 @@
         pulumi.set(self, "sync_time_with_host_periodically", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The IDs of any tags to attach to this resource. Please refer to the `Tag` resource for more information on applying tags to virtual machine resources.
+
+        > **NOTE:** Tagging support is unsupported on direct ESXi host connections and requires vCenter Server instance.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -1314,57 +1386,91 @@
         :param pulumi.Input[bool] cpu_hot_remove_enabled: Allow CPUs to be removed to the virtual machine while it is powered on.
         :param pulumi.Input[int] cpu_limit: The maximum amount of CPU (in MHz) that the virtual machine can consume, regardless of available resources. The default is no limit.
         :param pulumi.Input[bool] cpu_performance_counters_enabled: Enable CPU performance counters on the virtual machine. Default: `false`.
         :param pulumi.Input[int] cpu_reservation: The amount of CPU (in MHz) that the virtual machine is guaranteed. The default is no reservation.
         :param pulumi.Input[int] cpu_share_count: The number of CPU shares allocated to the virtual machine when the `cpu_share_level` is `custom`.
         :param pulumi.Input[str] cpu_share_level: The allocation level for the virtual machine CPU resources. One of `high`, `low`, `normal`, or `custom`. Default: `custom`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to attribute value strings to set for virtual machine. Please refer to the `vsphere_custom_attributes` resource for more information on setting custom attributes.
+               
+               > **NOTE:** Custom attributes requires vCenter Server and is not supported on direct ESXi host connections.
         :param pulumi.Input[str] datacenter_id: The datacenter ID. Required only when deploying an OVF/OVA template.
         :param pulumi.Input[str] datastore_cluster_id: The managed object reference ID of the datastore cluster in which to place the virtual machine. This setting applies to entire virtual machine and implies that you wish to use vSphere Storage DRS with the virtual machine. See the section on virtual machine migration for more information on modifying this value.
+               
+               > **NOTE:** One of `datastore_id` or `datastore_cluster_id` must be specified.
+               
+               > **NOTE:** Use of `datastore_cluster_id` requires vSphere Storage DRS to be enabled on the specified datastore cluster.
+               
+               > **NOTE:** The `datastore_cluster_id` setting applies to the entire virtual machine resource. You cannot assign individual individual disks to datastore clusters. In addition, you cannot use the `attach` setting to attach external disks on virtual machines that are assigned to datastore clusters.
         :param pulumi.Input[str] datastore_id: The managed object reference ID of the datastore in which to place the virtual machine. The virtual machine configuration files is placed here, along with any virtual disks that are created where a datastore is not explicitly specified. See the section on virtual machine migration for more information on modifying this value.
+               
+               > **NOTE:** Datastores cannot be assigned to individual disks when `datastore_cluster_id` is used.
         :param pulumi.Input[str] default_ip_address: The IP address selected by the provider to be used with any provisioners configured on this resource. When possible, this is the first IPv4 address that is reachable through the default gateway configured on the machine, then the first reachable IPv6 address, and then the first general discovered address if neither exists. If  VMware Tools is not running on the virtual machine, or if the virtual machine is powered off, this value will be blank.
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineDiskArgs']]] disks: A specification for a virtual disk device on the virtual machine. See disk options for more information.
         :param pulumi.Input[bool] efi_secure_boot_enabled: Use this option to enable EFI secure boot when the `firmware` type is set to is `efi`. Default: `false`.
+               
+               > **NOTE:** EFI secure boot is only available on vSphere 6.5 and later.
         :param pulumi.Input[bool] enable_disk_uuid: Expose the UUIDs of attached virtual disks to the virtual machine, allowing access to them in the guest. Default: `false`.
         :param pulumi.Input[bool] enable_logging: Enable logging of virtual machine events to a log file stored in the virtual machine directory. Default: `false`.
         :param pulumi.Input[str] ept_rvi_mode: The EPT/RVI (hardware memory virtualization) setting for the virtual machine. One of `automatic`, `on`, or `off`. Default: `automatic`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] extra_config: Extra configuration data for the virtual machine. Can be used to supply advanced parameters not normally in configuration, such as instance metadata and userdata.
+               
+               > **NOTE:** Do not use `extra_config` when working with a template imported from OVF/OVA as your settings may be ignored. Use the `vapp` block `properties` section as described in Using vApp Properties for OVF/OVA Configuration.
         :param pulumi.Input[bool] extra_config_reboot_required: Allow the virtual machine to be rebooted when a change to `extra_config` occurs. Default: `true`.
         :param pulumi.Input[str] firmware: The firmware for the virtual machine. One of `bios` or `efi`.
         :param pulumi.Input[str] folder: The path to the virtual machine folder in which to place the virtual machine, relative to the datacenter path (`/<datacenter-name>/vm`).  For example, `/dc-01/vm/foo`
         :param pulumi.Input[bool] force_power_off: If a guest shutdown failed or times out while updating or destroying (see `shutdown_wait_timeout`), force the power-off of the virtual machine. Default: `true`.
         :param pulumi.Input[str] guest_id: The guest ID for the operating system type. For a full list of possible values, see [here][vmware-docs-guest-ids]. Default: `otherGuest64`.
+               
+               [vmware-docs-guest-ids]: https://vdc-download.vmware.com/vmwb-repository/dcr-public/b50dcbbf-051d-4204-a3e7-e1b618c1e384/538cf2ec-b34f-4bae-a332-3820ef9e7773/vim.vm.GuestOsDescriptor.GuestOsIdentifier.html
         :param pulumi.Input[Sequence[pulumi.Input[str]]] guest_ip_addresses: The current list of IP addresses on this machine, including the value of `default_ip_address`. If VMware Tools is not running on the virtual machine, or if the virtul machine is powered off, this list will be empty.
         :param pulumi.Input[int] hardware_version: The hardware version number. Valid range is from 4 to 19. The hardware version cannot be downgraded. See [virtual machine hardware compatibility][virtual-machine-hardware-compatibility] for more information.
+               
+               [virtual-machine-hardware-compatibility]: https://kb.vmware.com/s/article/2007240
         :param pulumi.Input[str] host_system_id: The managed object reference ID of a host on which to place the virtual machine. See the section on virtual machine migration for more information on modifying this value. When using a vSphere cluster, if a `host_system_id` is not supplied, vSphere will select a host in the cluster to place the virtual machine, according to any defaults or vSphere DRS placement policies.
         :param pulumi.Input[str] hv_mode: The hardware virtualization (non-nested) setting for the virtual machine. One of `hvAuto`, `hvOn`, or `hvOff`. Default: `hvAuto`.
         :param pulumi.Input[int] ide_controller_count: The number of IDE controllers that the virtual machine. This directly affects the number of disks you can add to the virtual machine and the maximum disk unit number. Note that lowering this value does not remove controllers. Default: `2`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ignored_guest_ips: List of IP addresses and CIDR networks to ignore while waiting for an available IP address using either of the waiters. Any IP addresses in this list will be ignored so that the waiter will continue to wait for a valid IP address. Default: `[]`.
         :param pulumi.Input[bool] imported: Indicates if the virtual machine resource has been imported, or if the state has been migrated from a previous version of the resource. It influences the behavior of the first post-import apply operation. See the section on importing below.
         :param pulumi.Input[str] latency_sensitivity: Controls the scheduling delay of the virtual machine. Use a higher sensitivity for applications that require lower latency, such as VOIP, media player applications, or applications that require frequent access to mouse or keyboard devices. One of `low`, `normal`, `medium`, or `high`.
+               
+               > **NOTE:** On higher sensitivities, you may need to adjust the `memory_reservation` to the full amount of memory provisioned for the virtual machine.
         :param pulumi.Input[int] memory: The memory size to assign to the virtual machine, in MB. Default: `1024` (1 GB).
         :param pulumi.Input[bool] memory_hot_add_enabled: Allow memory to be added to the virtual machine while it is powered on.
+               
+               > **NOTE:** CPU and memory hot add options are not available on all guest operating systems. Please refer to the [VMware Guest OS Compatibility Guide][vmware-docs-compat-guide] to which settings are allow for your guest operating system. In addition, at least one `pulumi up` must be run before you are able to use CPU and memory hot add.
+               
+               [vmware-docs-compat-guide]: http://partnerweb.vmware.com/comp_guide2/pdf/VMware_GOS_Compatibility_Guide.pdf
+               
+               > **NOTE:** For Linux 64-bit guest operating systems with less than or equal to 3GB, the virtual machine must powered off to add memory beyond 3GB. Subsequent hot add of memory does not require the virtual machine to be powered-off to apply the plan. Please refer to [VMware KB 2008405][vmware-kb-2008405].
+               
+               [vmware-kb-2008405]: https://kb.vmware.com/s/article/2008405
         :param pulumi.Input[int] memory_limit: The maximum amount of memory (in MB) that th virtual machine can consume, regardless of available resources. The default is no limit.
         :param pulumi.Input[int] memory_reservation: The amount of memory (in MB) that the virtual machine is guaranteed. The default is no reservation.
         :param pulumi.Input[int] memory_share_count: The number of memory shares allocated to the virtual machine when the `memory_share_level` is `custom`.
         :param pulumi.Input[str] memory_share_level: The allocation level for the virtual machine memory resources. One of `high`, `low`, `normal`, or `custom`. Default: `custom`.
         :param pulumi.Input[int] migrate_wait_timeout: The amount of time, in minutes, to wait for a virtual machine migration to complete before failing. Default: `10` minutes. See the section on virtual machine migration for more information.
         :param pulumi.Input[str] moid: The managed object reference ID of the created virtual machine.
         :param pulumi.Input[str] name: The name of the virtual machine.
         :param pulumi.Input[bool] nested_hv_enabled: Enable nested hardware virtualization on the virtual machine, facilitating nested virtualization in the guest operating system. Default: `false`.
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineNetworkInterfaceArgs']]] network_interfaces: A specification for a virtual NIC on the virtual machine. See network interface options for more information.
         :param pulumi.Input[int] num_cores_per_socket: The number of cores per socket in the virtual machine. The number of vCPUs on the virtual machine will be `num_cpus` divided by `num_cores_per_socket`. If specified, the value supplied to `num_cpus` must be evenly divisible by this value. Default: `1`.
         :param pulumi.Input[int] num_cpus: The total number of virtual processor cores to assign to the virtual machine. Default: `1`.
         :param pulumi.Input['VirtualMachineOvfDeployArgs'] ovf_deploy: When specified, the virtual machine will be deployed from the provided OVF/OVA template. See creating a virtual machine from an OVF/OVA template for more information.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] pci_device_ids: List of host PCI device IDs in which to create PCI passthroughs.
+               
+               > **NOTE:** Cloning requires vCenter Server and is not supported on direct ESXi host connections.
         :param pulumi.Input[str] power_state: A computed value for the current power state of the virtual machine. One of `on`, `off`, or `suspended`.
         :param pulumi.Input[int] poweron_timeout: The amount of time, in seconds, that we will be trying to power on a VM
         :param pulumi.Input[bool] reboot_required: Value internal to Terraform used to determine if a configuration set change requires a reboot.
         :param pulumi.Input[str] replace_trigger: Triggers replacement of resource whenever it changes.
+               
+               For example, `replace_trigger = sha256(format("%s-%s",data.template_file.cloud_init_metadata.rendered,data.template_file.cloud_init_userdata.rendered))` will fingerprint the changes in cloud-init metadata and userdata templates. This will enable a replacement of the resource whenever the dependant template renders a new configuration. (Forces a replacement.)
         :param pulumi.Input[str] resource_pool_id: The managed object reference ID of the resource pool in which to place the virtual machine. See the Virtual Machine Migration section for more information on modifying this value.
+               
+               > **NOTE:** All clusters and standalone hosts have a default root resource pool. This resource argument does not directly accept the cluster or standalone host resource. For more information, see the section on specifying the Root Resource Pool in the `ResourcePool` data source documentation on using the root resource pool.
         :param pulumi.Input[bool] run_tools_scripts_after_power_on: Enable post-power-on scripts to run when VMware Tools is installed. Default: `true`.
         :param pulumi.Input[bool] run_tools_scripts_after_resume: Enable ost-resume scripts to run when VMware Tools is installed. Default: `true`.
         :param pulumi.Input[bool] run_tools_scripts_before_guest_reboot: Enable pre-reboot scripts to run when VMware Tools is installed. Default: `false`.
         :param pulumi.Input[bool] run_tools_scripts_before_guest_shutdown: Enable pre-shutdown scripts to run when VMware Tools is installed. Default: `true`.
         :param pulumi.Input[bool] run_tools_scripts_before_guest_standby: Enable pre-standby scripts to run when VMware Tools is installed. Default: `true`.
         :param pulumi.Input[int] sata_controller_count: The number of SATA controllers that Terraform manages on this virtual machine. This directly affects the amount of disks
                you can add to the virtual machine and the maximum disk unit number. Note that lowering this value does not remove
@@ -1376,14 +1482,16 @@
         :param pulumi.Input[str] scsi_type: The SCSI controller type for the virtual machine. One of `lsilogic` (LSI Logic Parallel), `lsilogic-sas` (LSI Logic SAS) or `pvscsi` (VMware Paravirtual). Default: `pvscsi`.
         :param pulumi.Input[int] shutdown_wait_timeout: The amount of time, in minutes, to wait for a graceful guest shutdown when making necessary updates to the virtual machine. If `force_power_off` is set to `true`, the virtual machine will be forced to power-off after the timeout, otherwise an error is returned. Default: `3` minutes.
         :param pulumi.Input[str] storage_policy_id: The ID of the storage policy to assign to the home directory of a virtual machine.
         :param pulumi.Input[str] swap_placement_policy: The swap file placement policy for the virtual machine. One of `inherit`, `hostLocal`, or `vmDirectory`. Default: `inherit`.
         :param pulumi.Input[bool] sync_time_with_host: Enable the guest operating system to synchronization its clock with the host when the virtual machine is powered on or resumed. Requires vSphere 7.0 Update 1 and later. Requires VMware Tools to be installed. Default: `false`.
         :param pulumi.Input[bool] sync_time_with_host_periodically: Enable the guest operating system to periodically synchronize its clock with the host. Requires vSphere 7.0 Update 1 and later. On previous versions, setting `sync_time_with_host` is will enable periodic synchronization. Requires VMware Tools to be installed. Default: `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource. Please refer to the `Tag` resource for more information on applying tags to virtual machine resources.
+               
+               > **NOTE:** Tagging support is unsupported on direct ESXi host connections and requires vCenter Server instance.
         :param pulumi.Input[str] tools_upgrade_policy: Enable automatic upgrade of the VMware Tools version when the virtual machine is rebooted. If necessary, VMware Tools is upgraded to the latest version supported by the host on which the virtual machine is running. Requires VMware Tools to be installed. One of `manual` or `upgradeAtPowerCycle`. Default: `manual`.
         :param pulumi.Input[str] uuid: The UUID of the virtual disk VMDK file. This is used to track the virtual disk on the virtual machine.
         :param pulumi.Input['VirtualMachineVappArgs'] vapp: Used for vApp configurations. The only sub-key available is `properties`, which is a key/value map of properties for virtual machines imported from and OVF/OVA. See Using vApp Properties for OVF/OVA Configuration for more information.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] vapp_transports: Computed value which is only valid for cloned virtual machines. A list of vApp transport methods supported by the source virtual machine or template.
         :param pulumi.Input[bool] vbs_enabled: Enable Virtualization Based Security. Requires `firmware` to be `efi`. In addition, `vvtd_enabled`, `nested_hv_enabled`, and `efi_secure_boot_enabled` must all have a value of `true`. Supported on vSphere 6.7 and later. Default: `false`.
         :param pulumi.Input[str] vmware_tools_status: The state of  VMware Tools in the guest. This will determine the proper course of action for some device operations.
         :param pulumi.Input[str] vmx_path: The path of the virtual machine configuration file on the datastore in which the virtual machine is placed.
@@ -1744,14 +1852,16 @@
         pulumi.set(self, "cpu_share_level", value)
 
     @property
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Map of custom attribute ids to attribute value strings to set for virtual machine. Please refer to the `vsphere_custom_attributes` resource for more information on setting custom attributes.
+
+        > **NOTE:** Custom attributes requires vCenter Server and is not supported on direct ESXi host connections.
         """
         return pulumi.get(self, "custom_attributes")
 
     @custom_attributes.setter
     def custom_attributes(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "custom_attributes", value)
 
@@ -1768,26 +1878,34 @@
         pulumi.set(self, "datacenter_id", value)
 
     @property
     @pulumi.getter(name="datastoreClusterId")
     def datastore_cluster_id(self) -> Optional[pulumi.Input[str]]:
         """
         The managed object reference ID of the datastore cluster in which to place the virtual machine. This setting applies to entire virtual machine and implies that you wish to use vSphere Storage DRS with the virtual machine. See the section on virtual machine migration for more information on modifying this value.
+
+        > **NOTE:** One of `datastore_id` or `datastore_cluster_id` must be specified.
+
+        > **NOTE:** Use of `datastore_cluster_id` requires vSphere Storage DRS to be enabled on the specified datastore cluster.
+
+        > **NOTE:** The `datastore_cluster_id` setting applies to the entire virtual machine resource. You cannot assign individual individual disks to datastore clusters. In addition, you cannot use the `attach` setting to attach external disks on virtual machines that are assigned to datastore clusters.
         """
         return pulumi.get(self, "datastore_cluster_id")
 
     @datastore_cluster_id.setter
     def datastore_cluster_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "datastore_cluster_id", value)
 
     @property
     @pulumi.getter(name="datastoreId")
     def datastore_id(self) -> Optional[pulumi.Input[str]]:
         """
         The managed object reference ID of the datastore in which to place the virtual machine. The virtual machine configuration files is placed here, along with any virtual disks that are created where a datastore is not explicitly specified. See the section on virtual machine migration for more information on modifying this value.
+
+        > **NOTE:** Datastores cannot be assigned to individual disks when `datastore_cluster_id` is used.
         """
         return pulumi.get(self, "datastore_id")
 
     @datastore_id.setter
     def datastore_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "datastore_id", value)
 
@@ -1816,14 +1934,16 @@
         pulumi.set(self, "disks", value)
 
     @property
     @pulumi.getter(name="efiSecureBootEnabled")
     def efi_secure_boot_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
         Use this option to enable EFI secure boot when the `firmware` type is set to is `efi`. Default: `false`.
+
+        > **NOTE:** EFI secure boot is only available on vSphere 6.5 and later.
         """
         return pulumi.get(self, "efi_secure_boot_enabled")
 
     @efi_secure_boot_enabled.setter
     def efi_secure_boot_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "efi_secure_boot_enabled", value)
 
@@ -1864,14 +1984,16 @@
         pulumi.set(self, "ept_rvi_mode", value)
 
     @property
     @pulumi.getter(name="extraConfig")
     def extra_config(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Extra configuration data for the virtual machine. Can be used to supply advanced parameters not normally in configuration, such as instance metadata and userdata.
+
+        > **NOTE:** Do not use `extra_config` when working with a template imported from OVF/OVA as your settings may be ignored. Use the `vapp` block `properties` section as described in Using vApp Properties for OVF/OVA Configuration.
         """
         return pulumi.get(self, "extra_config")
 
     @extra_config.setter
     def extra_config(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "extra_config", value)
 
@@ -1924,14 +2046,16 @@
         pulumi.set(self, "force_power_off", value)
 
     @property
     @pulumi.getter(name="guestId")
     def guest_id(self) -> Optional[pulumi.Input[str]]:
         """
         The guest ID for the operating system type. For a full list of possible values, see [here][vmware-docs-guest-ids]. Default: `otherGuest64`.
+
+        [vmware-docs-guest-ids]: https://vdc-download.vmware.com/vmwb-repository/dcr-public/b50dcbbf-051d-4204-a3e7-e1b618c1e384/538cf2ec-b34f-4bae-a332-3820ef9e7773/vim.vm.GuestOsDescriptor.GuestOsIdentifier.html
         """
         return pulumi.get(self, "guest_id")
 
     @guest_id.setter
     def guest_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "guest_id", value)
 
@@ -1948,14 +2072,16 @@
         pulumi.set(self, "guest_ip_addresses", value)
 
     @property
     @pulumi.getter(name="hardwareVersion")
     def hardware_version(self) -> Optional[pulumi.Input[int]]:
         """
         The hardware version number. Valid range is from 4 to 19. The hardware version cannot be downgraded. See [virtual machine hardware compatibility][virtual-machine-hardware-compatibility] for more information.
+
+        [virtual-machine-hardware-compatibility]: https://kb.vmware.com/s/article/2007240
         """
         return pulumi.get(self, "hardware_version")
 
     @hardware_version.setter
     def hardware_version(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "hardware_version", value)
 
@@ -2020,14 +2146,16 @@
         pulumi.set(self, "imported", value)
 
     @property
     @pulumi.getter(name="latencySensitivity")
     def latency_sensitivity(self) -> Optional[pulumi.Input[str]]:
         """
         Controls the scheduling delay of the virtual machine. Use a higher sensitivity for applications that require lower latency, such as VOIP, media player applications, or applications that require frequent access to mouse or keyboard devices. One of `low`, `normal`, `medium`, or `high`.
+
+        > **NOTE:** On higher sensitivities, you may need to adjust the `memory_reservation` to the full amount of memory provisioned for the virtual machine.
         """
         return pulumi.get(self, "latency_sensitivity")
 
     @latency_sensitivity.setter
     def latency_sensitivity(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "latency_sensitivity", value)
 
@@ -2044,14 +2172,22 @@
         pulumi.set(self, "memory", value)
 
     @property
     @pulumi.getter(name="memoryHotAddEnabled")
     def memory_hot_add_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
         Allow memory to be added to the virtual machine while it is powered on.
+
+        > **NOTE:** CPU and memory hot add options are not available on all guest operating systems. Please refer to the [VMware Guest OS Compatibility Guide][vmware-docs-compat-guide] to which settings are allow for your guest operating system. In addition, at least one `pulumi up` must be run before you are able to use CPU and memory hot add.
+
+        [vmware-docs-compat-guide]: http://partnerweb.vmware.com/comp_guide2/pdf/VMware_GOS_Compatibility_Guide.pdf
+
+        > **NOTE:** For Linux 64-bit guest operating systems with less than or equal to 3GB, the virtual machine must powered off to add memory beyond 3GB. Subsequent hot add of memory does not require the virtual machine to be powered-off to apply the plan. Please refer to [VMware KB 2008405][vmware-kb-2008405].
+
+        [vmware-kb-2008405]: https://kb.vmware.com/s/article/2008405
         """
         return pulumi.get(self, "memory_hot_add_enabled")
 
     @memory_hot_add_enabled.setter
     def memory_hot_add_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "memory_hot_add_enabled", value)
 
@@ -2200,14 +2336,16 @@
         pulumi.set(self, "ovf_deploy", value)
 
     @property
     @pulumi.getter(name="pciDeviceIds")
     def pci_device_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         List of host PCI device IDs in which to create PCI passthroughs.
+
+        > **NOTE:** Cloning requires vCenter Server and is not supported on direct ESXi host connections.
         """
         return pulumi.get(self, "pci_device_ids")
 
     @pci_device_ids.setter
     def pci_device_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "pci_device_ids", value)
 
@@ -2248,26 +2386,30 @@
         pulumi.set(self, "reboot_required", value)
 
     @property
     @pulumi.getter(name="replaceTrigger")
     def replace_trigger(self) -> Optional[pulumi.Input[str]]:
         """
         Triggers replacement of resource whenever it changes.
+
+        For example, `replace_trigger = sha256(format("%s-%s",data.template_file.cloud_init_metadata.rendered,data.template_file.cloud_init_userdata.rendered))` will fingerprint the changes in cloud-init metadata and userdata templates. This will enable a replacement of the resource whenever the dependant template renders a new configuration. (Forces a replacement.)
         """
         return pulumi.get(self, "replace_trigger")
 
     @replace_trigger.setter
     def replace_trigger(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "replace_trigger", value)
 
     @property
     @pulumi.getter(name="resourcePoolId")
     def resource_pool_id(self) -> Optional[pulumi.Input[str]]:
         """
         The managed object reference ID of the resource pool in which to place the virtual machine. See the Virtual Machine Migration section for more information on modifying this value.
+
+        > **NOTE:** All clusters and standalone hosts have a default root resource pool. This resource argument does not directly accept the cluster or standalone host resource. For more information, see the section on specifying the Root Resource Pool in the `ResourcePool` data source documentation on using the root resource pool.
         """
         return pulumi.get(self, "resource_pool_id")
 
     @resource_pool_id.setter
     def resource_pool_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "resource_pool_id", value)
 
@@ -2444,14 +2586,16 @@
         pulumi.set(self, "sync_time_with_host_periodically", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The IDs of any tags to attach to this resource. Please refer to the `Tag` resource for more information on applying tags to virtual machine resources.
+
+        > **NOTE:** Tagging support is unsupported on direct ESXi host connections and requires vCenter Server instance.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -2683,51 +2827,85 @@
         :param pulumi.Input[bool] cpu_hot_remove_enabled: Allow CPUs to be removed to the virtual machine while it is powered on.
         :param pulumi.Input[int] cpu_limit: The maximum amount of CPU (in MHz) that the virtual machine can consume, regardless of available resources. The default is no limit.
         :param pulumi.Input[bool] cpu_performance_counters_enabled: Enable CPU performance counters on the virtual machine. Default: `false`.
         :param pulumi.Input[int] cpu_reservation: The amount of CPU (in MHz) that the virtual machine is guaranteed. The default is no reservation.
         :param pulumi.Input[int] cpu_share_count: The number of CPU shares allocated to the virtual machine when the `cpu_share_level` is `custom`.
         :param pulumi.Input[str] cpu_share_level: The allocation level for the virtual machine CPU resources. One of `high`, `low`, `normal`, or `custom`. Default: `custom`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to attribute value strings to set for virtual machine. Please refer to the `vsphere_custom_attributes` resource for more information on setting custom attributes.
+               
+               > **NOTE:** Custom attributes requires vCenter Server and is not supported on direct ESXi host connections.
         :param pulumi.Input[str] datacenter_id: The datacenter ID. Required only when deploying an OVF/OVA template.
         :param pulumi.Input[str] datastore_cluster_id: The managed object reference ID of the datastore cluster in which to place the virtual machine. This setting applies to entire virtual machine and implies that you wish to use vSphere Storage DRS with the virtual machine. See the section on virtual machine migration for more information on modifying this value.
+               
+               > **NOTE:** One of `datastore_id` or `datastore_cluster_id` must be specified.
+               
+               > **NOTE:** Use of `datastore_cluster_id` requires vSphere Storage DRS to be enabled on the specified datastore cluster.
+               
+               > **NOTE:** The `datastore_cluster_id` setting applies to the entire virtual machine resource. You cannot assign individual individual disks to datastore clusters. In addition, you cannot use the `attach` setting to attach external disks on virtual machines that are assigned to datastore clusters.
         :param pulumi.Input[str] datastore_id: The managed object reference ID of the datastore in which to place the virtual machine. The virtual machine configuration files is placed here, along with any virtual disks that are created where a datastore is not explicitly specified. See the section on virtual machine migration for more information on modifying this value.
+               
+               > **NOTE:** Datastores cannot be assigned to individual disks when `datastore_cluster_id` is used.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineDiskArgs']]]] disks: A specification for a virtual disk device on the virtual machine. See disk options for more information.
         :param pulumi.Input[bool] efi_secure_boot_enabled: Use this option to enable EFI secure boot when the `firmware` type is set to is `efi`. Default: `false`.
+               
+               > **NOTE:** EFI secure boot is only available on vSphere 6.5 and later.
         :param pulumi.Input[bool] enable_disk_uuid: Expose the UUIDs of attached virtual disks to the virtual machine, allowing access to them in the guest. Default: `false`.
         :param pulumi.Input[bool] enable_logging: Enable logging of virtual machine events to a log file stored in the virtual machine directory. Default: `false`.
         :param pulumi.Input[str] ept_rvi_mode: The EPT/RVI (hardware memory virtualization) setting for the virtual machine. One of `automatic`, `on`, or `off`. Default: `automatic`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] extra_config: Extra configuration data for the virtual machine. Can be used to supply advanced parameters not normally in configuration, such as instance metadata and userdata.
+               
+               > **NOTE:** Do not use `extra_config` when working with a template imported from OVF/OVA as your settings may be ignored. Use the `vapp` block `properties` section as described in Using vApp Properties for OVF/OVA Configuration.
         :param pulumi.Input[bool] extra_config_reboot_required: Allow the virtual machine to be rebooted when a change to `extra_config` occurs. Default: `true`.
         :param pulumi.Input[str] firmware: The firmware for the virtual machine. One of `bios` or `efi`.
         :param pulumi.Input[str] folder: The path to the virtual machine folder in which to place the virtual machine, relative to the datacenter path (`/<datacenter-name>/vm`).  For example, `/dc-01/vm/foo`
         :param pulumi.Input[bool] force_power_off: If a guest shutdown failed or times out while updating or destroying (see `shutdown_wait_timeout`), force the power-off of the virtual machine. Default: `true`.
         :param pulumi.Input[str] guest_id: The guest ID for the operating system type. For a full list of possible values, see [here][vmware-docs-guest-ids]. Default: `otherGuest64`.
+               
+               [vmware-docs-guest-ids]: https://vdc-download.vmware.com/vmwb-repository/dcr-public/b50dcbbf-051d-4204-a3e7-e1b618c1e384/538cf2ec-b34f-4bae-a332-3820ef9e7773/vim.vm.GuestOsDescriptor.GuestOsIdentifier.html
         :param pulumi.Input[int] hardware_version: The hardware version number. Valid range is from 4 to 19. The hardware version cannot be downgraded. See [virtual machine hardware compatibility][virtual-machine-hardware-compatibility] for more information.
+               
+               [virtual-machine-hardware-compatibility]: https://kb.vmware.com/s/article/2007240
         :param pulumi.Input[str] host_system_id: The managed object reference ID of a host on which to place the virtual machine. See the section on virtual machine migration for more information on modifying this value. When using a vSphere cluster, if a `host_system_id` is not supplied, vSphere will select a host in the cluster to place the virtual machine, according to any defaults or vSphere DRS placement policies.
         :param pulumi.Input[str] hv_mode: The hardware virtualization (non-nested) setting for the virtual machine. One of `hvAuto`, `hvOn`, or `hvOff`. Default: `hvAuto`.
         :param pulumi.Input[int] ide_controller_count: The number of IDE controllers that the virtual machine. This directly affects the number of disks you can add to the virtual machine and the maximum disk unit number. Note that lowering this value does not remove controllers. Default: `2`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ignored_guest_ips: List of IP addresses and CIDR networks to ignore while waiting for an available IP address using either of the waiters. Any IP addresses in this list will be ignored so that the waiter will continue to wait for a valid IP address. Default: `[]`.
         :param pulumi.Input[str] latency_sensitivity: Controls the scheduling delay of the virtual machine. Use a higher sensitivity for applications that require lower latency, such as VOIP, media player applications, or applications that require frequent access to mouse or keyboard devices. One of `low`, `normal`, `medium`, or `high`.
+               
+               > **NOTE:** On higher sensitivities, you may need to adjust the `memory_reservation` to the full amount of memory provisioned for the virtual machine.
         :param pulumi.Input[int] memory: The memory size to assign to the virtual machine, in MB. Default: `1024` (1 GB).
         :param pulumi.Input[bool] memory_hot_add_enabled: Allow memory to be added to the virtual machine while it is powered on.
+               
+               > **NOTE:** CPU and memory hot add options are not available on all guest operating systems. Please refer to the [VMware Guest OS Compatibility Guide][vmware-docs-compat-guide] to which settings are allow for your guest operating system. In addition, at least one `pulumi up` must be run before you are able to use CPU and memory hot add.
+               
+               [vmware-docs-compat-guide]: http://partnerweb.vmware.com/comp_guide2/pdf/VMware_GOS_Compatibility_Guide.pdf
+               
+               > **NOTE:** For Linux 64-bit guest operating systems with less than or equal to 3GB, the virtual machine must powered off to add memory beyond 3GB. Subsequent hot add of memory does not require the virtual machine to be powered-off to apply the plan. Please refer to [VMware KB 2008405][vmware-kb-2008405].
+               
+               [vmware-kb-2008405]: https://kb.vmware.com/s/article/2008405
         :param pulumi.Input[int] memory_limit: The maximum amount of memory (in MB) that th virtual machine can consume, regardless of available resources. The default is no limit.
         :param pulumi.Input[int] memory_reservation: The amount of memory (in MB) that the virtual machine is guaranteed. The default is no reservation.
         :param pulumi.Input[int] memory_share_count: The number of memory shares allocated to the virtual machine when the `memory_share_level` is `custom`.
         :param pulumi.Input[str] memory_share_level: The allocation level for the virtual machine memory resources. One of `high`, `low`, `normal`, or `custom`. Default: `custom`.
         :param pulumi.Input[int] migrate_wait_timeout: The amount of time, in minutes, to wait for a virtual machine migration to complete before failing. Default: `10` minutes. See the section on virtual machine migration for more information.
         :param pulumi.Input[str] name: The name of the virtual machine.
         :param pulumi.Input[bool] nested_hv_enabled: Enable nested hardware virtualization on the virtual machine, facilitating nested virtualization in the guest operating system. Default: `false`.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineNetworkInterfaceArgs']]]] network_interfaces: A specification for a virtual NIC on the virtual machine. See network interface options for more information.
         :param pulumi.Input[int] num_cores_per_socket: The number of cores per socket in the virtual machine. The number of vCPUs on the virtual machine will be `num_cpus` divided by `num_cores_per_socket`. If specified, the value supplied to `num_cpus` must be evenly divisible by this value. Default: `1`.
         :param pulumi.Input[int] num_cpus: The total number of virtual processor cores to assign to the virtual machine. Default: `1`.
         :param pulumi.Input[pulumi.InputType['VirtualMachineOvfDeployArgs']] ovf_deploy: When specified, the virtual machine will be deployed from the provided OVF/OVA template. See creating a virtual machine from an OVF/OVA template for more information.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] pci_device_ids: List of host PCI device IDs in which to create PCI passthroughs.
+               
+               > **NOTE:** Cloning requires vCenter Server and is not supported on direct ESXi host connections.
         :param pulumi.Input[int] poweron_timeout: The amount of time, in seconds, that we will be trying to power on a VM
         :param pulumi.Input[str] replace_trigger: Triggers replacement of resource whenever it changes.
+               
+               For example, `replace_trigger = sha256(format("%s-%s",data.template_file.cloud_init_metadata.rendered,data.template_file.cloud_init_userdata.rendered))` will fingerprint the changes in cloud-init metadata and userdata templates. This will enable a replacement of the resource whenever the dependant template renders a new configuration. (Forces a replacement.)
         :param pulumi.Input[str] resource_pool_id: The managed object reference ID of the resource pool in which to place the virtual machine. See the Virtual Machine Migration section for more information on modifying this value.
+               
+               > **NOTE:** All clusters and standalone hosts have a default root resource pool. This resource argument does not directly accept the cluster or standalone host resource. For more information, see the section on specifying the Root Resource Pool in the `ResourcePool` data source documentation on using the root resource pool.
         :param pulumi.Input[bool] run_tools_scripts_after_power_on: Enable post-power-on scripts to run when VMware Tools is installed. Default: `true`.
         :param pulumi.Input[bool] run_tools_scripts_after_resume: Enable ost-resume scripts to run when VMware Tools is installed. Default: `true`.
         :param pulumi.Input[bool] run_tools_scripts_before_guest_reboot: Enable pre-reboot scripts to run when VMware Tools is installed. Default: `false`.
         :param pulumi.Input[bool] run_tools_scripts_before_guest_shutdown: Enable pre-shutdown scripts to run when VMware Tools is installed. Default: `true`.
         :param pulumi.Input[bool] run_tools_scripts_before_guest_standby: Enable pre-standby scripts to run when VMware Tools is installed. Default: `true`.
         :param pulumi.Input[int] sata_controller_count: The number of SATA controllers that Terraform manages on this virtual machine. This directly affects the amount of disks
                you can add to the virtual machine and the maximum disk unit number. Note that lowering this value does not remove
@@ -2739,14 +2917,16 @@
         :param pulumi.Input[str] scsi_type: The SCSI controller type for the virtual machine. One of `lsilogic` (LSI Logic Parallel), `lsilogic-sas` (LSI Logic SAS) or `pvscsi` (VMware Paravirtual). Default: `pvscsi`.
         :param pulumi.Input[int] shutdown_wait_timeout: The amount of time, in minutes, to wait for a graceful guest shutdown when making necessary updates to the virtual machine. If `force_power_off` is set to `true`, the virtual machine will be forced to power-off after the timeout, otherwise an error is returned. Default: `3` minutes.
         :param pulumi.Input[str] storage_policy_id: The ID of the storage policy to assign to the home directory of a virtual machine.
         :param pulumi.Input[str] swap_placement_policy: The swap file placement policy for the virtual machine. One of `inherit`, `hostLocal`, or `vmDirectory`. Default: `inherit`.
         :param pulumi.Input[bool] sync_time_with_host: Enable the guest operating system to synchronization its clock with the host when the virtual machine is powered on or resumed. Requires vSphere 7.0 Update 1 and later. Requires VMware Tools to be installed. Default: `false`.
         :param pulumi.Input[bool] sync_time_with_host_periodically: Enable the guest operating system to periodically synchronize its clock with the host. Requires vSphere 7.0 Update 1 and later. On previous versions, setting `sync_time_with_host` is will enable periodic synchronization. Requires VMware Tools to be installed. Default: `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource. Please refer to the `Tag` resource for more information on applying tags to virtual machine resources.
+               
+               > **NOTE:** Tagging support is unsupported on direct ESXi host connections and requires vCenter Server instance.
         :param pulumi.Input[str] tools_upgrade_policy: Enable automatic upgrade of the VMware Tools version when the virtual machine is rebooted. If necessary, VMware Tools is upgraded to the latest version supported by the host on which the virtual machine is running. Requires VMware Tools to be installed. One of `manual` or `upgradeAtPowerCycle`. Default: `manual`.
         :param pulumi.Input[pulumi.InputType['VirtualMachineVappArgs']] vapp: Used for vApp configurations. The only sub-key available is `properties`, which is a key/value map of properties for virtual machines imported from and OVF/OVA. See Using vApp Properties for OVF/OVA Configuration for more information.
         :param pulumi.Input[bool] vbs_enabled: Enable Virtualization Based Security. Requires `firmware` to be `efi`. In addition, `vvtd_enabled`, `nested_hv_enabled`, and `efi_secure_boot_enabled` must all have a value of `true`. Supported on vSphere 6.7 and later. Default: `false`.
         :param pulumi.Input[bool] vvtd_enabled: Enable Intel Virtualization Technology for Directed I/O for the virtual machine (_I/O MMU_ in the vSphere Client). Supported on vSphere 6.7 and later. Default: `false`.
         :param pulumi.Input[int] wait_for_guest_ip_timeout: The amount of time, in minutes, to wait for an available guest IP address on the virtual machine. This should only be used if the version VMware Tools does not allow the `wait_for_guest_net_timeout` waiter to be used. A value less than `1` disables the waiter. Default: `0`.
         :param pulumi.Input[bool] wait_for_guest_net_routable: Controls whether or not the guest network waiter waits for a routable address. When `false`, the waiter does not wait for a default gateway, nor are IP addresses checked against any discovered default gateways as part of its success criteria. This property is ignored if the `wait_for_guest_ip_timeout` waiter is used. Default: `true`.
         :param pulumi.Input[int] wait_for_guest_net_timeout: The amount of time, in minutes, to wait for an available guest IP address on the virtual machine. Older versions of VMware Tools do not populate this property. In those cases, this waiter can be disabled and the `wait_for_guest_ip_timeout` waiter can be used instead. A value less than `1` disables the waiter. Default: `5` minutes.
@@ -3058,57 +3238,91 @@
         :param pulumi.Input[bool] cpu_hot_remove_enabled: Allow CPUs to be removed to the virtual machine while it is powered on.
         :param pulumi.Input[int] cpu_limit: The maximum amount of CPU (in MHz) that the virtual machine can consume, regardless of available resources. The default is no limit.
         :param pulumi.Input[bool] cpu_performance_counters_enabled: Enable CPU performance counters on the virtual machine. Default: `false`.
         :param pulumi.Input[int] cpu_reservation: The amount of CPU (in MHz) that the virtual machine is guaranteed. The default is no reservation.
         :param pulumi.Input[int] cpu_share_count: The number of CPU shares allocated to the virtual machine when the `cpu_share_level` is `custom`.
         :param pulumi.Input[str] cpu_share_level: The allocation level for the virtual machine CPU resources. One of `high`, `low`, `normal`, or `custom`. Default: `custom`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to attribute value strings to set for virtual machine. Please refer to the `vsphere_custom_attributes` resource for more information on setting custom attributes.
+               
+               > **NOTE:** Custom attributes requires vCenter Server and is not supported on direct ESXi host connections.
         :param pulumi.Input[str] datacenter_id: The datacenter ID. Required only when deploying an OVF/OVA template.
         :param pulumi.Input[str] datastore_cluster_id: The managed object reference ID of the datastore cluster in which to place the virtual machine. This setting applies to entire virtual machine and implies that you wish to use vSphere Storage DRS with the virtual machine. See the section on virtual machine migration for more information on modifying this value.
+               
+               > **NOTE:** One of `datastore_id` or `datastore_cluster_id` must be specified.
+               
+               > **NOTE:** Use of `datastore_cluster_id` requires vSphere Storage DRS to be enabled on the specified datastore cluster.
+               
+               > **NOTE:** The `datastore_cluster_id` setting applies to the entire virtual machine resource. You cannot assign individual individual disks to datastore clusters. In addition, you cannot use the `attach` setting to attach external disks on virtual machines that are assigned to datastore clusters.
         :param pulumi.Input[str] datastore_id: The managed object reference ID of the datastore in which to place the virtual machine. The virtual machine configuration files is placed here, along with any virtual disks that are created where a datastore is not explicitly specified. See the section on virtual machine migration for more information on modifying this value.
+               
+               > **NOTE:** Datastores cannot be assigned to individual disks when `datastore_cluster_id` is used.
         :param pulumi.Input[str] default_ip_address: The IP address selected by the provider to be used with any provisioners configured on this resource. When possible, this is the first IPv4 address that is reachable through the default gateway configured on the machine, then the first reachable IPv6 address, and then the first general discovered address if neither exists. If  VMware Tools is not running on the virtual machine, or if the virtual machine is powered off, this value will be blank.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineDiskArgs']]]] disks: A specification for a virtual disk device on the virtual machine. See disk options for more information.
         :param pulumi.Input[bool] efi_secure_boot_enabled: Use this option to enable EFI secure boot when the `firmware` type is set to is `efi`. Default: `false`.
+               
+               > **NOTE:** EFI secure boot is only available on vSphere 6.5 and later.
         :param pulumi.Input[bool] enable_disk_uuid: Expose the UUIDs of attached virtual disks to the virtual machine, allowing access to them in the guest. Default: `false`.
         :param pulumi.Input[bool] enable_logging: Enable logging of virtual machine events to a log file stored in the virtual machine directory. Default: `false`.
         :param pulumi.Input[str] ept_rvi_mode: The EPT/RVI (hardware memory virtualization) setting for the virtual machine. One of `automatic`, `on`, or `off`. Default: `automatic`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] extra_config: Extra configuration data for the virtual machine. Can be used to supply advanced parameters not normally in configuration, such as instance metadata and userdata.
+               
+               > **NOTE:** Do not use `extra_config` when working with a template imported from OVF/OVA as your settings may be ignored. Use the `vapp` block `properties` section as described in Using vApp Properties for OVF/OVA Configuration.
         :param pulumi.Input[bool] extra_config_reboot_required: Allow the virtual machine to be rebooted when a change to `extra_config` occurs. Default: `true`.
         :param pulumi.Input[str] firmware: The firmware for the virtual machine. One of `bios` or `efi`.
         :param pulumi.Input[str] folder: The path to the virtual machine folder in which to place the virtual machine, relative to the datacenter path (`/<datacenter-name>/vm`).  For example, `/dc-01/vm/foo`
         :param pulumi.Input[bool] force_power_off: If a guest shutdown failed or times out while updating or destroying (see `shutdown_wait_timeout`), force the power-off of the virtual machine. Default: `true`.
         :param pulumi.Input[str] guest_id: The guest ID for the operating system type. For a full list of possible values, see [here][vmware-docs-guest-ids]. Default: `otherGuest64`.
+               
+               [vmware-docs-guest-ids]: https://vdc-download.vmware.com/vmwb-repository/dcr-public/b50dcbbf-051d-4204-a3e7-e1b618c1e384/538cf2ec-b34f-4bae-a332-3820ef9e7773/vim.vm.GuestOsDescriptor.GuestOsIdentifier.html
         :param pulumi.Input[Sequence[pulumi.Input[str]]] guest_ip_addresses: The current list of IP addresses on this machine, including the value of `default_ip_address`. If VMware Tools is not running on the virtual machine, or if the virtul machine is powered off, this list will be empty.
         :param pulumi.Input[int] hardware_version: The hardware version number. Valid range is from 4 to 19. The hardware version cannot be downgraded. See [virtual machine hardware compatibility][virtual-machine-hardware-compatibility] for more information.
+               
+               [virtual-machine-hardware-compatibility]: https://kb.vmware.com/s/article/2007240
         :param pulumi.Input[str] host_system_id: The managed object reference ID of a host on which to place the virtual machine. See the section on virtual machine migration for more information on modifying this value. When using a vSphere cluster, if a `host_system_id` is not supplied, vSphere will select a host in the cluster to place the virtual machine, according to any defaults or vSphere DRS placement policies.
         :param pulumi.Input[str] hv_mode: The hardware virtualization (non-nested) setting for the virtual machine. One of `hvAuto`, `hvOn`, or `hvOff`. Default: `hvAuto`.
         :param pulumi.Input[int] ide_controller_count: The number of IDE controllers that the virtual machine. This directly affects the number of disks you can add to the virtual machine and the maximum disk unit number. Note that lowering this value does not remove controllers. Default: `2`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ignored_guest_ips: List of IP addresses and CIDR networks to ignore while waiting for an available IP address using either of the waiters. Any IP addresses in this list will be ignored so that the waiter will continue to wait for a valid IP address. Default: `[]`.
         :param pulumi.Input[bool] imported: Indicates if the virtual machine resource has been imported, or if the state has been migrated from a previous version of the resource. It influences the behavior of the first post-import apply operation. See the section on importing below.
         :param pulumi.Input[str] latency_sensitivity: Controls the scheduling delay of the virtual machine. Use a higher sensitivity for applications that require lower latency, such as VOIP, media player applications, or applications that require frequent access to mouse or keyboard devices. One of `low`, `normal`, `medium`, or `high`.
+               
+               > **NOTE:** On higher sensitivities, you may need to adjust the `memory_reservation` to the full amount of memory provisioned for the virtual machine.
         :param pulumi.Input[int] memory: The memory size to assign to the virtual machine, in MB. Default: `1024` (1 GB).
         :param pulumi.Input[bool] memory_hot_add_enabled: Allow memory to be added to the virtual machine while it is powered on.
+               
+               > **NOTE:** CPU and memory hot add options are not available on all guest operating systems. Please refer to the [VMware Guest OS Compatibility Guide][vmware-docs-compat-guide] to which settings are allow for your guest operating system. In addition, at least one `pulumi up` must be run before you are able to use CPU and memory hot add.
+               
+               [vmware-docs-compat-guide]: http://partnerweb.vmware.com/comp_guide2/pdf/VMware_GOS_Compatibility_Guide.pdf
+               
+               > **NOTE:** For Linux 64-bit guest operating systems with less than or equal to 3GB, the virtual machine must powered off to add memory beyond 3GB. Subsequent hot add of memory does not require the virtual machine to be powered-off to apply the plan. Please refer to [VMware KB 2008405][vmware-kb-2008405].
+               
+               [vmware-kb-2008405]: https://kb.vmware.com/s/article/2008405
         :param pulumi.Input[int] memory_limit: The maximum amount of memory (in MB) that th virtual machine can consume, regardless of available resources. The default is no limit.
         :param pulumi.Input[int] memory_reservation: The amount of memory (in MB) that the virtual machine is guaranteed. The default is no reservation.
         :param pulumi.Input[int] memory_share_count: The number of memory shares allocated to the virtual machine when the `memory_share_level` is `custom`.
         :param pulumi.Input[str] memory_share_level: The allocation level for the virtual machine memory resources. One of `high`, `low`, `normal`, or `custom`. Default: `custom`.
         :param pulumi.Input[int] migrate_wait_timeout: The amount of time, in minutes, to wait for a virtual machine migration to complete before failing. Default: `10` minutes. See the section on virtual machine migration for more information.
         :param pulumi.Input[str] moid: The managed object reference ID of the created virtual machine.
         :param pulumi.Input[str] name: The name of the virtual machine.
         :param pulumi.Input[bool] nested_hv_enabled: Enable nested hardware virtualization on the virtual machine, facilitating nested virtualization in the guest operating system. Default: `false`.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineNetworkInterfaceArgs']]]] network_interfaces: A specification for a virtual NIC on the virtual machine. See network interface options for more information.
         :param pulumi.Input[int] num_cores_per_socket: The number of cores per socket in the virtual machine. The number of vCPUs on the virtual machine will be `num_cpus` divided by `num_cores_per_socket`. If specified, the value supplied to `num_cpus` must be evenly divisible by this value. Default: `1`.
         :param pulumi.Input[int] num_cpus: The total number of virtual processor cores to assign to the virtual machine. Default: `1`.
         :param pulumi.Input[pulumi.InputType['VirtualMachineOvfDeployArgs']] ovf_deploy: When specified, the virtual machine will be deployed from the provided OVF/OVA template. See creating a virtual machine from an OVF/OVA template for more information.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] pci_device_ids: List of host PCI device IDs in which to create PCI passthroughs.
+               
+               > **NOTE:** Cloning requires vCenter Server and is not supported on direct ESXi host connections.
         :param pulumi.Input[str] power_state: A computed value for the current power state of the virtual machine. One of `on`, `off`, or `suspended`.
         :param pulumi.Input[int] poweron_timeout: The amount of time, in seconds, that we will be trying to power on a VM
         :param pulumi.Input[bool] reboot_required: Value internal to Terraform used to determine if a configuration set change requires a reboot.
         :param pulumi.Input[str] replace_trigger: Triggers replacement of resource whenever it changes.
+               
+               For example, `replace_trigger = sha256(format("%s-%s",data.template_file.cloud_init_metadata.rendered,data.template_file.cloud_init_userdata.rendered))` will fingerprint the changes in cloud-init metadata and userdata templates. This will enable a replacement of the resource whenever the dependant template renders a new configuration. (Forces a replacement.)
         :param pulumi.Input[str] resource_pool_id: The managed object reference ID of the resource pool in which to place the virtual machine. See the Virtual Machine Migration section for more information on modifying this value.
+               
+               > **NOTE:** All clusters and standalone hosts have a default root resource pool. This resource argument does not directly accept the cluster or standalone host resource. For more information, see the section on specifying the Root Resource Pool in the `ResourcePool` data source documentation on using the root resource pool.
         :param pulumi.Input[bool] run_tools_scripts_after_power_on: Enable post-power-on scripts to run when VMware Tools is installed. Default: `true`.
         :param pulumi.Input[bool] run_tools_scripts_after_resume: Enable ost-resume scripts to run when VMware Tools is installed. Default: `true`.
         :param pulumi.Input[bool] run_tools_scripts_before_guest_reboot: Enable pre-reboot scripts to run when VMware Tools is installed. Default: `false`.
         :param pulumi.Input[bool] run_tools_scripts_before_guest_shutdown: Enable pre-shutdown scripts to run when VMware Tools is installed. Default: `true`.
         :param pulumi.Input[bool] run_tools_scripts_before_guest_standby: Enable pre-standby scripts to run when VMware Tools is installed. Default: `true`.
         :param pulumi.Input[int] sata_controller_count: The number of SATA controllers that Terraform manages on this virtual machine. This directly affects the amount of disks
                you can add to the virtual machine and the maximum disk unit number. Note that lowering this value does not remove
@@ -3120,14 +3334,16 @@
         :param pulumi.Input[str] scsi_type: The SCSI controller type for the virtual machine. One of `lsilogic` (LSI Logic Parallel), `lsilogic-sas` (LSI Logic SAS) or `pvscsi` (VMware Paravirtual). Default: `pvscsi`.
         :param pulumi.Input[int] shutdown_wait_timeout: The amount of time, in minutes, to wait for a graceful guest shutdown when making necessary updates to the virtual machine. If `force_power_off` is set to `true`, the virtual machine will be forced to power-off after the timeout, otherwise an error is returned. Default: `3` minutes.
         :param pulumi.Input[str] storage_policy_id: The ID of the storage policy to assign to the home directory of a virtual machine.
         :param pulumi.Input[str] swap_placement_policy: The swap file placement policy for the virtual machine. One of `inherit`, `hostLocal`, or `vmDirectory`. Default: `inherit`.
         :param pulumi.Input[bool] sync_time_with_host: Enable the guest operating system to synchronization its clock with the host when the virtual machine is powered on or resumed. Requires vSphere 7.0 Update 1 and later. Requires VMware Tools to be installed. Default: `false`.
         :param pulumi.Input[bool] sync_time_with_host_periodically: Enable the guest operating system to periodically synchronize its clock with the host. Requires vSphere 7.0 Update 1 and later. On previous versions, setting `sync_time_with_host` is will enable periodic synchronization. Requires VMware Tools to be installed. Default: `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource. Please refer to the `Tag` resource for more information on applying tags to virtual machine resources.
+               
+               > **NOTE:** Tagging support is unsupported on direct ESXi host connections and requires vCenter Server instance.
         :param pulumi.Input[str] tools_upgrade_policy: Enable automatic upgrade of the VMware Tools version when the virtual machine is rebooted. If necessary, VMware Tools is upgraded to the latest version supported by the host on which the virtual machine is running. Requires VMware Tools to be installed. One of `manual` or `upgradeAtPowerCycle`. Default: `manual`.
         :param pulumi.Input[str] uuid: The UUID of the virtual disk VMDK file. This is used to track the virtual disk on the virtual machine.
         :param pulumi.Input[pulumi.InputType['VirtualMachineVappArgs']] vapp: Used for vApp configurations. The only sub-key available is `properties`, which is a key/value map of properties for virtual machines imported from and OVF/OVA. See Using vApp Properties for OVF/OVA Configuration for more information.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] vapp_transports: Computed value which is only valid for cloned virtual machines. A list of vApp transport methods supported by the source virtual machine or template.
         :param pulumi.Input[bool] vbs_enabled: Enable Virtualization Based Security. Requires `firmware` to be `efi`. In addition, `vvtd_enabled`, `nested_hv_enabled`, and `efi_secure_boot_enabled` must all have a value of `true`. Supported on vSphere 6.7 and later. Default: `false`.
         :param pulumi.Input[str] vmware_tools_status: The state of  VMware Tools in the guest. This will determine the proper course of action for some device operations.
         :param pulumi.Input[str] vmx_path: The path of the virtual machine configuration file on the datastore in which the virtual machine is placed.
@@ -3348,14 +3564,16 @@
         return pulumi.get(self, "cpu_share_level")
 
     @property
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
         Map of custom attribute ids to attribute value strings to set for virtual machine. Please refer to the `vsphere_custom_attributes` resource for more information on setting custom attributes.
+
+        > **NOTE:** Custom attributes requires vCenter Server and is not supported on direct ESXi host connections.
         """
         return pulumi.get(self, "custom_attributes")
 
     @property
     @pulumi.getter(name="datacenterId")
     def datacenter_id(self) -> pulumi.Output[Optional[str]]:
         """
@@ -3364,22 +3582,30 @@
         return pulumi.get(self, "datacenter_id")
 
     @property
     @pulumi.getter(name="datastoreClusterId")
     def datastore_cluster_id(self) -> pulumi.Output[Optional[str]]:
         """
         The managed object reference ID of the datastore cluster in which to place the virtual machine. This setting applies to entire virtual machine and implies that you wish to use vSphere Storage DRS with the virtual machine. See the section on virtual machine migration for more information on modifying this value.
+
+        > **NOTE:** One of `datastore_id` or `datastore_cluster_id` must be specified.
+
+        > **NOTE:** Use of `datastore_cluster_id` requires vSphere Storage DRS to be enabled on the specified datastore cluster.
+
+        > **NOTE:** The `datastore_cluster_id` setting applies to the entire virtual machine resource. You cannot assign individual individual disks to datastore clusters. In addition, you cannot use the `attach` setting to attach external disks on virtual machines that are assigned to datastore clusters.
         """
         return pulumi.get(self, "datastore_cluster_id")
 
     @property
     @pulumi.getter(name="datastoreId")
     def datastore_id(self) -> pulumi.Output[str]:
         """
         The managed object reference ID of the datastore in which to place the virtual machine. The virtual machine configuration files is placed here, along with any virtual disks that are created where a datastore is not explicitly specified. See the section on virtual machine migration for more information on modifying this value.
+
+        > **NOTE:** Datastores cannot be assigned to individual disks when `datastore_cluster_id` is used.
         """
         return pulumi.get(self, "datastore_id")
 
     @property
     @pulumi.getter(name="defaultIpAddress")
     def default_ip_address(self) -> pulumi.Output[str]:
         """
@@ -3396,14 +3622,16 @@
         return pulumi.get(self, "disks")
 
     @property
     @pulumi.getter(name="efiSecureBootEnabled")
     def efi_secure_boot_enabled(self) -> pulumi.Output[Optional[bool]]:
         """
         Use this option to enable EFI secure boot when the `firmware` type is set to is `efi`. Default: `false`.
+
+        > **NOTE:** EFI secure boot is only available on vSphere 6.5 and later.
         """
         return pulumi.get(self, "efi_secure_boot_enabled")
 
     @property
     @pulumi.getter(name="enableDiskUuid")
     def enable_disk_uuid(self) -> pulumi.Output[Optional[bool]]:
         """
@@ -3428,14 +3656,16 @@
         return pulumi.get(self, "ept_rvi_mode")
 
     @property
     @pulumi.getter(name="extraConfig")
     def extra_config(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
         Extra configuration data for the virtual machine. Can be used to supply advanced parameters not normally in configuration, such as instance metadata and userdata.
+
+        > **NOTE:** Do not use `extra_config` when working with a template imported from OVF/OVA as your settings may be ignored. Use the `vapp` block `properties` section as described in Using vApp Properties for OVF/OVA Configuration.
         """
         return pulumi.get(self, "extra_config")
 
     @property
     @pulumi.getter(name="extraConfigRebootRequired")
     def extra_config_reboot_required(self) -> pulumi.Output[Optional[bool]]:
         """
@@ -3468,14 +3698,16 @@
         return pulumi.get(self, "force_power_off")
 
     @property
     @pulumi.getter(name="guestId")
     def guest_id(self) -> pulumi.Output[str]:
         """
         The guest ID for the operating system type. For a full list of possible values, see [here][vmware-docs-guest-ids]. Default: `otherGuest64`.
+
+        [vmware-docs-guest-ids]: https://vdc-download.vmware.com/vmwb-repository/dcr-public/b50dcbbf-051d-4204-a3e7-e1b618c1e384/538cf2ec-b34f-4bae-a332-3820ef9e7773/vim.vm.GuestOsDescriptor.GuestOsIdentifier.html
         """
         return pulumi.get(self, "guest_id")
 
     @property
     @pulumi.getter(name="guestIpAddresses")
     def guest_ip_addresses(self) -> pulumi.Output[Sequence[str]]:
         """
@@ -3484,14 +3716,16 @@
         return pulumi.get(self, "guest_ip_addresses")
 
     @property
     @pulumi.getter(name="hardwareVersion")
     def hardware_version(self) -> pulumi.Output[int]:
         """
         The hardware version number. Valid range is from 4 to 19. The hardware version cannot be downgraded. See [virtual machine hardware compatibility][virtual-machine-hardware-compatibility] for more information.
+
+        [virtual-machine-hardware-compatibility]: https://kb.vmware.com/s/article/2007240
         """
         return pulumi.get(self, "hardware_version")
 
     @property
     @pulumi.getter(name="hostSystemId")
     def host_system_id(self) -> pulumi.Output[str]:
         """
@@ -3532,14 +3766,16 @@
         return pulumi.get(self, "imported")
 
     @property
     @pulumi.getter(name="latencySensitivity")
     def latency_sensitivity(self) -> pulumi.Output[Optional[str]]:
         """
         Controls the scheduling delay of the virtual machine. Use a higher sensitivity for applications that require lower latency, such as VOIP, media player applications, or applications that require frequent access to mouse or keyboard devices. One of `low`, `normal`, `medium`, or `high`.
+
+        > **NOTE:** On higher sensitivities, you may need to adjust the `memory_reservation` to the full amount of memory provisioned for the virtual machine.
         """
         return pulumi.get(self, "latency_sensitivity")
 
     @property
     @pulumi.getter
     def memory(self) -> pulumi.Output[Optional[int]]:
         """
@@ -3548,14 +3784,22 @@
         return pulumi.get(self, "memory")
 
     @property
     @pulumi.getter(name="memoryHotAddEnabled")
     def memory_hot_add_enabled(self) -> pulumi.Output[Optional[bool]]:
         """
         Allow memory to be added to the virtual machine while it is powered on.
+
+        > **NOTE:** CPU and memory hot add options are not available on all guest operating systems. Please refer to the [VMware Guest OS Compatibility Guide][vmware-docs-compat-guide] to which settings are allow for your guest operating system. In addition, at least one `pulumi up` must be run before you are able to use CPU and memory hot add.
+
+        [vmware-docs-compat-guide]: http://partnerweb.vmware.com/comp_guide2/pdf/VMware_GOS_Compatibility_Guide.pdf
+
+        > **NOTE:** For Linux 64-bit guest operating systems with less than or equal to 3GB, the virtual machine must powered off to add memory beyond 3GB. Subsequent hot add of memory does not require the virtual machine to be powered-off to apply the plan. Please refer to [VMware KB 2008405][vmware-kb-2008405].
+
+        [vmware-kb-2008405]: https://kb.vmware.com/s/article/2008405
         """
         return pulumi.get(self, "memory_hot_add_enabled")
 
     @property
     @pulumi.getter(name="memoryLimit")
     def memory_limit(self) -> pulumi.Output[Optional[int]]:
         """
@@ -3652,14 +3896,16 @@
         return pulumi.get(self, "ovf_deploy")
 
     @property
     @pulumi.getter(name="pciDeviceIds")
     def pci_device_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         List of host PCI device IDs in which to create PCI passthroughs.
+
+        > **NOTE:** Cloning requires vCenter Server and is not supported on direct ESXi host connections.
         """
         return pulumi.get(self, "pci_device_ids")
 
     @property
     @pulumi.getter(name="powerState")
     def power_state(self) -> pulumi.Output[str]:
         """
@@ -3684,22 +3930,26 @@
         return pulumi.get(self, "reboot_required")
 
     @property
     @pulumi.getter(name="replaceTrigger")
     def replace_trigger(self) -> pulumi.Output[Optional[str]]:
         """
         Triggers replacement of resource whenever it changes.
+
+        For example, `replace_trigger = sha256(format("%s-%s",data.template_file.cloud_init_metadata.rendered,data.template_file.cloud_init_userdata.rendered))` will fingerprint the changes in cloud-init metadata and userdata templates. This will enable a replacement of the resource whenever the dependant template renders a new configuration. (Forces a replacement.)
         """
         return pulumi.get(self, "replace_trigger")
 
     @property
     @pulumi.getter(name="resourcePoolId")
     def resource_pool_id(self) -> pulumi.Output[str]:
         """
         The managed object reference ID of the resource pool in which to place the virtual machine. See the Virtual Machine Migration section for more information on modifying this value.
+
+        > **NOTE:** All clusters and standalone hosts have a default root resource pool. This resource argument does not directly accept the cluster or standalone host resource. For more information, see the section on specifying the Root Resource Pool in the `ResourcePool` data source documentation on using the root resource pool.
         """
         return pulumi.get(self, "resource_pool_id")
 
     @property
     @pulumi.getter(name="runToolsScriptsAfterPowerOn")
     def run_tools_scripts_after_power_on(self) -> pulumi.Output[Optional[bool]]:
         """
@@ -3816,14 +4066,16 @@
         return pulumi.get(self, "sync_time_with_host_periodically")
 
     @property
     @pulumi.getter
     def tags(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         The IDs of any tags to attach to this resource. Please refer to the `Tag` resource for more information on applying tags to virtual machine resources.
+
+        > **NOTE:** Tagging support is unsupported on direct ESXi host connections and requires vCenter Server instance.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="toolsUpgradePolicy")
     def tools_upgrade_policy(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/virtual_machine_snapshot.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/virtual_machine_snapshot.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/vm_storage_policy.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/vm_storage_policy.py`

 * *Files 6% similar despite different names*

```diff
@@ -185,44 +185,44 @@
         import pulumi
         import pulumi_vsphere as vsphere
 
         prod_platinum_replicated = vsphere.VmStoragePolicy("prodPlatinumReplicated",
             description="prod_platinum_replicated",
             tag_rules=[
                 vsphere.VmStoragePolicyTagRuleArgs(
-                    tag_category=data["vsphere_tag_category"]["environment"]["name"],
+                    tag_category=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                     tags=[data["vsphere_tag"]["production"]["name"]],
                     include_datastores_with_tags=True,
                 ),
                 vsphere.VmStoragePolicyTagRuleArgs(
-                    tag_category=data["vsphere_tag_category"]["service_level"]["name"],
+                    tag_category=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                     tags=[data["vsphere_tag"]["platinum"]["name"]],
                     include_datastores_with_tags=True,
                 ),
                 vsphere.VmStoragePolicyTagRuleArgs(
-                    tag_category=data["vsphere_tag_category"]["replication"]["name"],
+                    tag_category=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                     tags=[data["vsphere_tag"]["replicated"]["name"]],
                     include_datastores_with_tags=True,
                 ),
             ])
         dev_silver_nonreplicated = vsphere.VmStoragePolicy("devSilverNonreplicated",
             description="dev_silver_nonreplicated",
             tag_rules=[
                 vsphere.VmStoragePolicyTagRuleArgs(
-                    tag_category=data["vsphere_tag_category"]["environment"]["name"],
+                    tag_category=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                     tags=[data["vsphere_tag"]["development"]["name"]],
                     include_datastores_with_tags=True,
                 ),
                 vsphere.VmStoragePolicyTagRuleArgs(
-                    tag_category=data["vsphere_tag_category"]["service_level"]["name"],
+                    tag_category=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                     tags=[data["vsphere_tag"]["silver"]["name"]],
                     include_datastores_with_tags=True,
                 ),
                 vsphere.VmStoragePolicyTagRuleArgs(
-                    tag_category=data["vsphere_tag_category"]["replication"]["name"],
+                    tag_category=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                     tags=[data["vsphere_tag"]["non_replicated"]["name"]],
                     include_datastores_with_tags=True,
                 ),
             ])
         ```
 
         Lasttly, when creating a virtual machine resource, a storage policy can be specificed to direct virtual machine placement to a datastore which matches the policy's `tags_rules`.
@@ -303,44 +303,44 @@
         import pulumi
         import pulumi_vsphere as vsphere
 
         prod_platinum_replicated = vsphere.VmStoragePolicy("prodPlatinumReplicated",
             description="prod_platinum_replicated",
             tag_rules=[
                 vsphere.VmStoragePolicyTagRuleArgs(
-                    tag_category=data["vsphere_tag_category"]["environment"]["name"],
+                    tag_category=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                     tags=[data["vsphere_tag"]["production"]["name"]],
                     include_datastores_with_tags=True,
                 ),
                 vsphere.VmStoragePolicyTagRuleArgs(
-                    tag_category=data["vsphere_tag_category"]["service_level"]["name"],
+                    tag_category=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                     tags=[data["vsphere_tag"]["platinum"]["name"]],
                     include_datastores_with_tags=True,
                 ),
                 vsphere.VmStoragePolicyTagRuleArgs(
-                    tag_category=data["vsphere_tag_category"]["replication"]["name"],
+                    tag_category=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                     tags=[data["vsphere_tag"]["replicated"]["name"]],
                     include_datastores_with_tags=True,
                 ),
             ])
         dev_silver_nonreplicated = vsphere.VmStoragePolicy("devSilverNonreplicated",
             description="dev_silver_nonreplicated",
             tag_rules=[
                 vsphere.VmStoragePolicyTagRuleArgs(
-                    tag_category=data["vsphere_tag_category"]["environment"]["name"],
+                    tag_category=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                     tags=[data["vsphere_tag"]["development"]["name"]],
                     include_datastores_with_tags=True,
                 ),
                 vsphere.VmStoragePolicyTagRuleArgs(
-                    tag_category=data["vsphere_tag_category"]["service_level"]["name"],
+                    tag_category=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                     tags=[data["vsphere_tag"]["silver"]["name"]],
                     include_datastores_with_tags=True,
                 ),
                 vsphere.VmStoragePolicyTagRuleArgs(
-                    tag_category=data["vsphere_tag_category"]["replication"]["name"],
+                    tag_category=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
                     tags=[data["vsphere_tag"]["non_replicated"]["name"]],
                     include_datastores_with_tags=True,
                 ),
             ])
         ```
 
         Lasttly, when creating a virtual machine resource, a storage policy can be specificed to direct virtual machine placement to a datastore which matches the policy's `tags_rules`.
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/vmfs_datastore.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/vmfs_datastore.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,27 +27,33 @@
         :param pulumi.Input[str] host_system_id: The managed object ID of
                the host to set the datastore up on. Note that this is not necessarily the
                only host that the datastore will be set up on - see
                here for more info. Forces a
                new resource if changed.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to attribute 
                value string to set on datastore resource.
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+               and require vCenter.
         :param pulumi.Input[str] datastore_cluster_id: The managed object
                ID of a datastore cluster to put this datastore in.
                Conflicts with `folder`.
         :param pulumi.Input[str] folder: The relative path to a folder to put this datastore in.
                This is a path relative to the datacenter you are deploying the datastore to.
                Example: for the `dc1` datacenter, and a provided `folder` of `foo/bar`,
                The provider will place a datastore named `test` in a datastore folder
                located at `/dc1/datastore/foo/bar`, with the final inventory path being
                `/dc1/datastore/foo/bar/test`. Conflicts with
                `datastore_cluster_id`.
         :param pulumi.Input[str] name: The name of the datastore. Forces a new resource if
                changed.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource. 
+               
+               > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+               requires vCenter 6.0 or higher.
         """
         pulumi.set(__self__, "disks", disks)
         pulumi.set(__self__, "host_system_id", host_system_id)
         if custom_attributes is not None:
             pulumi.set(__self__, "custom_attributes", custom_attributes)
         if datastore_cluster_id is not None:
             pulumi.set(__self__, "datastore_cluster_id", datastore_cluster_id)
@@ -88,14 +94,17 @@
 
     @property
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Map of custom attribute ids to attribute 
         value string to set on datastore resource.
+
+        > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+        and require vCenter.
         """
         return pulumi.get(self, "custom_attributes")
 
     @custom_attributes.setter
     def custom_attributes(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "custom_attributes", value)
 
@@ -144,15 +153,18 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The IDs of any tags to attach to this resource.
+        The IDs of any tags to attach to this resource. 
+
+        > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+        requires vCenter 6.0 or higher.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -177,14 +189,17 @@
         """
         Input properties used for looking up and filtering VmfsDatastore resources.
         :param pulumi.Input[bool] accessible: The connectivity status of the datastore. If this is `false`,
                some other computed attributes may be out of date.
         :param pulumi.Input[int] capacity: Maximum capacity of the datastore, in megabytes.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to attribute 
                value string to set on datastore resource.
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+               and require vCenter.
         :param pulumi.Input[str] datastore_cluster_id: The managed object
                ID of a datastore cluster to put this datastore in.
                Conflicts with `folder`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] disks: The disks to use with the datastore.
         :param pulumi.Input[str] folder: The relative path to a folder to put this datastore in.
                This is a path relative to the datacenter you are deploying the datastore to.
                Example: for the `dc1` datacenter, and a provided `folder` of `foo/bar`,
@@ -199,15 +214,18 @@
                here for more info. Forces a
                new resource if changed.
         :param pulumi.Input[str] maintenance_mode: The current maintenance mode state of the datastore.
         :param pulumi.Input[bool] multiple_host_access: If `true`, more than one host in the datacenter has
                been configured with access to the datastore.
         :param pulumi.Input[str] name: The name of the datastore. Forces a new resource if
                changed.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource. 
+               
+               > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+               requires vCenter 6.0 or higher.
         :param pulumi.Input[int] uncommitted_space: Total additional storage space, in megabytes,
                potentially used by all virtual machines on this datastore.
         :param pulumi.Input[str] url: The unique locator for the datastore.
         """
         if accessible is not None:
             pulumi.set(__self__, "accessible", accessible)
         if capacity is not None:
@@ -264,14 +282,17 @@
 
     @property
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Map of custom attribute ids to attribute 
         value string to set on datastore resource.
+
+        > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+        and require vCenter.
         """
         return pulumi.get(self, "custom_attributes")
 
     @custom_attributes.setter
     def custom_attributes(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "custom_attributes", value)
 
@@ -385,15 +406,18 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The IDs of any tags to attach to this resource.
+        The IDs of any tags to attach to this resource. 
+
+        > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+        requires vCenter 6.0 or higher.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -438,14 +462,17 @@
                  __props__=None):
         """
         Create a VmfsDatastore resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to attribute 
                value string to set on datastore resource.
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+               and require vCenter.
         :param pulumi.Input[str] datastore_cluster_id: The managed object
                ID of a datastore cluster to put this datastore in.
                Conflicts with `folder`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] disks: The disks to use with the datastore.
         :param pulumi.Input[str] folder: The relative path to a folder to put this datastore in.
                This is a path relative to the datacenter you are deploying the datastore to.
                Example: for the `dc1` datacenter, and a provided `folder` of `foo/bar`,
@@ -456,15 +483,18 @@
         :param pulumi.Input[str] host_system_id: The managed object ID of
                the host to set the datastore up on. Note that this is not necessarily the
                only host that the datastore will be set up on - see
                here for more info. Forces a
                new resource if changed.
         :param pulumi.Input[str] name: The name of the datastore. Forces a new resource if
                changed.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource. 
+               
+               > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+               requires vCenter 6.0 or higher.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: VmfsDatastoreArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -551,14 +581,17 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] accessible: The connectivity status of the datastore. If this is `false`,
                some other computed attributes may be out of date.
         :param pulumi.Input[int] capacity: Maximum capacity of the datastore, in megabytes.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_attributes: Map of custom attribute ids to attribute 
                value string to set on datastore resource.
+               
+               > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+               and require vCenter.
         :param pulumi.Input[str] datastore_cluster_id: The managed object
                ID of a datastore cluster to put this datastore in.
                Conflicts with `folder`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] disks: The disks to use with the datastore.
         :param pulumi.Input[str] folder: The relative path to a folder to put this datastore in.
                This is a path relative to the datacenter you are deploying the datastore to.
                Example: for the `dc1` datacenter, and a provided `folder` of `foo/bar`,
@@ -573,15 +606,18 @@
                here for more info. Forces a
                new resource if changed.
         :param pulumi.Input[str] maintenance_mode: The current maintenance mode state of the datastore.
         :param pulumi.Input[bool] multiple_host_access: If `true`, more than one host in the datacenter has
                been configured with access to the datastore.
         :param pulumi.Input[str] name: The name of the datastore. Forces a new resource if
                changed.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The IDs of any tags to attach to this resource. 
+               
+               > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+               requires vCenter 6.0 or higher.
         :param pulumi.Input[int] uncommitted_space: Total additional storage space, in megabytes,
                potentially used by all virtual machines on this datastore.
         :param pulumi.Input[str] url: The unique locator for the datastore.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _VmfsDatastoreState.__new__(_VmfsDatastoreState)
@@ -621,14 +657,17 @@
 
     @property
     @pulumi.getter(name="customAttributes")
     def custom_attributes(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
         Map of custom attribute ids to attribute 
         value string to set on datastore resource.
+
+        > **NOTE:** Custom attributes are unsupported on direct ESXi connections
+        and require vCenter.
         """
         return pulumi.get(self, "custom_attributes")
 
     @property
     @pulumi.getter(name="datastoreClusterId")
     def datastore_cluster_id(self) -> pulumi.Output[Optional[str]]:
         """
@@ -706,15 +745,18 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def tags(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        The IDs of any tags to attach to this resource.
+        The IDs of any tags to attach to this resource. 
+
+        > **NOTE:** Tagging support is unsupported on direct ESXi connections and
+        requires vCenter 6.0 or higher.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="uncommittedSpace")
     def uncommitted_space(self) -> pulumi.Output[int]:
         """
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere/vnic.py` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere/vnic.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,26 +20,28 @@
                  distributed_port_group: Optional[pulumi.Input[str]] = None,
                  distributed_switch_port: Optional[pulumi.Input[str]] = None,
                  ipv4: Optional[pulumi.Input['VnicIpv4Args']] = None,
                  ipv6: Optional[pulumi.Input['VnicIpv6Args']] = None,
                  mac: Optional[pulumi.Input[str]] = None,
                  mtu: Optional[pulumi.Input[int]] = None,
                  netstack: Optional[pulumi.Input[str]] = None,
-                 portgroup: Optional[pulumi.Input[str]] = None):
+                 portgroup: Optional[pulumi.Input[str]] = None,
+                 services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a Vnic resource.
         :param pulumi.Input[str] host: ESX host the interface belongs to
         :param pulumi.Input[str] distributed_port_group: Key of the distributed portgroup the nic will connect to.
         :param pulumi.Input[str] distributed_switch_port: UUID of the DVSwitch the nic will be attached to. Do not set if you set portgroup.
         :param pulumi.Input['VnicIpv4Args'] ipv4: IPv4 settings. Either this or `ipv6` needs to be set. See  ipv4 options below.
         :param pulumi.Input['VnicIpv6Args'] ipv6: IPv6 settings. Either this or `ipv6` needs to be set. See  ipv6 options below.
         :param pulumi.Input[str] mac: MAC address of the interface.
         :param pulumi.Input[int] mtu: MTU of the interface.
         :param pulumi.Input[str] netstack: TCP/IP stack setting for this interface. Possible values are 'defaultTcpipStack', 'vmotion', 'vSphereProvisioning'. Changing this will force the creation of a new interface since it's not possible to change the stack once it gets created. (Default: `defaultTcpipStack`)
         :param pulumi.Input[str] portgroup: Portgroup to attach the nic to. Do not set if you set distributed_switch_port.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: Enabled services setting for this interface. Current possible values are 'vmotion', 'management', and 'vsan'.
         """
         pulumi.set(__self__, "host", host)
         if distributed_port_group is not None:
             pulumi.set(__self__, "distributed_port_group", distributed_port_group)
         if distributed_switch_port is not None:
             pulumi.set(__self__, "distributed_switch_port", distributed_switch_port)
         if ipv4 is not None:
@@ -50,14 +52,16 @@
             pulumi.set(__self__, "mac", mac)
         if mtu is not None:
             pulumi.set(__self__, "mtu", mtu)
         if netstack is not None:
             pulumi.set(__self__, "netstack", netstack)
         if portgroup is not None:
             pulumi.set(__self__, "portgroup", portgroup)
+        if services is not None:
+            pulumi.set(__self__, "services", services)
 
     @property
     @pulumi.getter
     def host(self) -> pulumi.Input[str]:
         """
         ESX host the interface belongs to
         """
@@ -159,38 +163,52 @@
         """
         return pulumi.get(self, "portgroup")
 
     @portgroup.setter
     def portgroup(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "portgroup", value)
 
+    @property
+    @pulumi.getter
+    def services(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Enabled services setting for this interface. Current possible values are 'vmotion', 'management', and 'vsan'.
+        """
+        return pulumi.get(self, "services")
+
+    @services.setter
+    def services(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "services", value)
+
 
 @pulumi.input_type
 class _VnicState:
     def __init__(__self__, *,
                  distributed_port_group: Optional[pulumi.Input[str]] = None,
                  distributed_switch_port: Optional[pulumi.Input[str]] = None,
                  host: Optional[pulumi.Input[str]] = None,
                  ipv4: Optional[pulumi.Input['VnicIpv4Args']] = None,
                  ipv6: Optional[pulumi.Input['VnicIpv6Args']] = None,
                  mac: Optional[pulumi.Input[str]] = None,
                  mtu: Optional[pulumi.Input[int]] = None,
                  netstack: Optional[pulumi.Input[str]] = None,
-                 portgroup: Optional[pulumi.Input[str]] = None):
+                 portgroup: Optional[pulumi.Input[str]] = None,
+                 services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering Vnic resources.
         :param pulumi.Input[str] distributed_port_group: Key of the distributed portgroup the nic will connect to.
         :param pulumi.Input[str] distributed_switch_port: UUID of the DVSwitch the nic will be attached to. Do not set if you set portgroup.
         :param pulumi.Input[str] host: ESX host the interface belongs to
         :param pulumi.Input['VnicIpv4Args'] ipv4: IPv4 settings. Either this or `ipv6` needs to be set. See  ipv4 options below.
         :param pulumi.Input['VnicIpv6Args'] ipv6: IPv6 settings. Either this or `ipv6` needs to be set. See  ipv6 options below.
         :param pulumi.Input[str] mac: MAC address of the interface.
         :param pulumi.Input[int] mtu: MTU of the interface.
         :param pulumi.Input[str] netstack: TCP/IP stack setting for this interface. Possible values are 'defaultTcpipStack', 'vmotion', 'vSphereProvisioning'. Changing this will force the creation of a new interface since it's not possible to change the stack once it gets created. (Default: `defaultTcpipStack`)
         :param pulumi.Input[str] portgroup: Portgroup to attach the nic to. Do not set if you set distributed_switch_port.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: Enabled services setting for this interface. Current possible values are 'vmotion', 'management', and 'vsan'.
         """
         if distributed_port_group is not None:
             pulumi.set(__self__, "distributed_port_group", distributed_port_group)
         if distributed_switch_port is not None:
             pulumi.set(__self__, "distributed_switch_port", distributed_switch_port)
         if host is not None:
             pulumi.set(__self__, "host", host)
@@ -202,14 +220,16 @@
             pulumi.set(__self__, "mac", mac)
         if mtu is not None:
             pulumi.set(__self__, "mtu", mtu)
         if netstack is not None:
             pulumi.set(__self__, "netstack", netstack)
         if portgroup is not None:
             pulumi.set(__self__, "portgroup", portgroup)
+        if services is not None:
+            pulumi.set(__self__, "services", services)
 
     @property
     @pulumi.getter(name="distributedPortGroup")
     def distributed_port_group(self) -> Optional[pulumi.Input[str]]:
         """
         Key of the distributed portgroup the nic will connect to.
         """
@@ -311,14 +331,26 @@
         """
         return pulumi.get(self, "portgroup")
 
     @portgroup.setter
     def portgroup(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "portgroup", value)
 
+    @property
+    @pulumi.getter
+    def services(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Enabled services setting for this interface. Current possible values are 'vmotion', 'management', and 'vsan'.
+        """
+        return pulumi.get(self, "services")
+
+    @services.setter
+    def services(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "services", value)
+
 
 class Vnic(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  distributed_port_group: Optional[pulumi.Input[str]] = None,
@@ -326,14 +358,15 @@
                  host: Optional[pulumi.Input[str]] = None,
                  ipv4: Optional[pulumi.Input[pulumi.InputType['VnicIpv4Args']]] = None,
                  ipv6: Optional[pulumi.Input[pulumi.InputType['VnicIpv6Args']]] = None,
                  mac: Optional[pulumi.Input[str]] = None,
                  mtu: Optional[pulumi.Input[int]] = None,
                  netstack: Optional[pulumi.Input[str]] = None,
                  portgroup: Optional[pulumi.Input[str]] = None,
+                 services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Provides a VMware vSphere vnic resource.
 
         ## Example Usage
 
         ### S
@@ -360,41 +393,14 @@
             distributed_switch_port=d1.id,
             distributed_port_group=p1.id,
             ipv4=vsphere.VnicIpv4Args(
                 dhcp=True,
             ),
             netstack="vmotion")
         ```
-        ### Create a vnic attached to a portgroup using the default TCP/IP stack
-
-        ```python
-        import pulumi
-        import pulumi_vsphere as vsphere
-
-        dc = vsphere.get_datacenter(name="mydc")
-        h1 = vsphere.get_host(name="esxi1.host.test",
-            datacenter_id=dc.id)
-        hvs1 = vsphere.HostVirtualSwitch("hvs1",
-            host_system_id=h1.id,
-            network_adapters=[
-                "vmnic3",
-                "vmnic4",
-            ],
-            active_nics=["vmnic3"],
-            standby_nics=["vmnic4"])
-        p1 = vsphere.HostPortGroup("p1",
-            virtual_switch_name=hvs1.name,
-            host_system_id=h1.id)
-        v1 = vsphere.Vnic("v1",
-            host=h1.id,
-            portgroup=p1.name,
-            ipv4=vsphere.VnicIpv4Args(
-                dhcp=True,
-            ))
-        ```
         ## Importing
 
         An existing vNic can be [imported][docs-import] into this resource
         via supplying the vNic's ID. An example is below:
 
         [docs-import]: /docs/import/index.html
 
@@ -411,14 +417,15 @@
         :param pulumi.Input[str] host: ESX host the interface belongs to
         :param pulumi.Input[pulumi.InputType['VnicIpv4Args']] ipv4: IPv4 settings. Either this or `ipv6` needs to be set. See  ipv4 options below.
         :param pulumi.Input[pulumi.InputType['VnicIpv6Args']] ipv6: IPv6 settings. Either this or `ipv6` needs to be set. See  ipv6 options below.
         :param pulumi.Input[str] mac: MAC address of the interface.
         :param pulumi.Input[int] mtu: MTU of the interface.
         :param pulumi.Input[str] netstack: TCP/IP stack setting for this interface. Possible values are 'defaultTcpipStack', 'vmotion', 'vSphereProvisioning'. Changing this will force the creation of a new interface since it's not possible to change the stack once it gets created. (Default: `defaultTcpipStack`)
         :param pulumi.Input[str] portgroup: Portgroup to attach the nic to. Do not set if you set distributed_switch_port.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: Enabled services setting for this interface. Current possible values are 'vmotion', 'management', and 'vsan'.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: VnicArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -451,41 +458,14 @@
             distributed_switch_port=d1.id,
             distributed_port_group=p1.id,
             ipv4=vsphere.VnicIpv4Args(
                 dhcp=True,
             ),
             netstack="vmotion")
         ```
-        ### Create a vnic attached to a portgroup using the default TCP/IP stack
-
-        ```python
-        import pulumi
-        import pulumi_vsphere as vsphere
-
-        dc = vsphere.get_datacenter(name="mydc")
-        h1 = vsphere.get_host(name="esxi1.host.test",
-            datacenter_id=dc.id)
-        hvs1 = vsphere.HostVirtualSwitch("hvs1",
-            host_system_id=h1.id,
-            network_adapters=[
-                "vmnic3",
-                "vmnic4",
-            ],
-            active_nics=["vmnic3"],
-            standby_nics=["vmnic4"])
-        p1 = vsphere.HostPortGroup("p1",
-            virtual_switch_name=hvs1.name,
-            host_system_id=h1.id)
-        v1 = vsphere.Vnic("v1",
-            host=h1.id,
-            portgroup=p1.name,
-            ipv4=vsphere.VnicIpv4Args(
-                dhcp=True,
-            ))
-        ```
         ## Importing
 
         An existing vNic can be [imported][docs-import] into this resource
         via supplying the vNic's ID. An example is below:
 
         [docs-import]: /docs/import/index.html
 
@@ -515,14 +495,15 @@
                  host: Optional[pulumi.Input[str]] = None,
                  ipv4: Optional[pulumi.Input[pulumi.InputType['VnicIpv4Args']]] = None,
                  ipv6: Optional[pulumi.Input[pulumi.InputType['VnicIpv6Args']]] = None,
                  mac: Optional[pulumi.Input[str]] = None,
                  mtu: Optional[pulumi.Input[int]] = None,
                  netstack: Optional[pulumi.Input[str]] = None,
                  portgroup: Optional[pulumi.Input[str]] = None,
+                 services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
@@ -535,14 +516,15 @@
             __props__.__dict__["host"] = host
             __props__.__dict__["ipv4"] = ipv4
             __props__.__dict__["ipv6"] = ipv6
             __props__.__dict__["mac"] = mac
             __props__.__dict__["mtu"] = mtu
             __props__.__dict__["netstack"] = netstack
             __props__.__dict__["portgroup"] = portgroup
+            __props__.__dict__["services"] = services
         super(Vnic, __self__).__init__(
             'vsphere:index/vnic:Vnic',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
@@ -553,15 +535,16 @@
             distributed_switch_port: Optional[pulumi.Input[str]] = None,
             host: Optional[pulumi.Input[str]] = None,
             ipv4: Optional[pulumi.Input[pulumi.InputType['VnicIpv4Args']]] = None,
             ipv6: Optional[pulumi.Input[pulumi.InputType['VnicIpv6Args']]] = None,
             mac: Optional[pulumi.Input[str]] = None,
             mtu: Optional[pulumi.Input[int]] = None,
             netstack: Optional[pulumi.Input[str]] = None,
-            portgroup: Optional[pulumi.Input[str]] = None) -> 'Vnic':
+            portgroup: Optional[pulumi.Input[str]] = None,
+            services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'Vnic':
         """
         Get an existing Vnic resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -570,28 +553,30 @@
         :param pulumi.Input[str] host: ESX host the interface belongs to
         :param pulumi.Input[pulumi.InputType['VnicIpv4Args']] ipv4: IPv4 settings. Either this or `ipv6` needs to be set. See  ipv4 options below.
         :param pulumi.Input[pulumi.InputType['VnicIpv6Args']] ipv6: IPv6 settings. Either this or `ipv6` needs to be set. See  ipv6 options below.
         :param pulumi.Input[str] mac: MAC address of the interface.
         :param pulumi.Input[int] mtu: MTU of the interface.
         :param pulumi.Input[str] netstack: TCP/IP stack setting for this interface. Possible values are 'defaultTcpipStack', 'vmotion', 'vSphereProvisioning'. Changing this will force the creation of a new interface since it's not possible to change the stack once it gets created. (Default: `defaultTcpipStack`)
         :param pulumi.Input[str] portgroup: Portgroup to attach the nic to. Do not set if you set distributed_switch_port.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: Enabled services setting for this interface. Current possible values are 'vmotion', 'management', and 'vsan'.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _VnicState.__new__(_VnicState)
 
         __props__.__dict__["distributed_port_group"] = distributed_port_group
         __props__.__dict__["distributed_switch_port"] = distributed_switch_port
         __props__.__dict__["host"] = host
         __props__.__dict__["ipv4"] = ipv4
         __props__.__dict__["ipv6"] = ipv6
         __props__.__dict__["mac"] = mac
         __props__.__dict__["mtu"] = mtu
         __props__.__dict__["netstack"] = netstack
         __props__.__dict__["portgroup"] = portgroup
+        __props__.__dict__["services"] = services
         return Vnic(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="distributedPortGroup")
     def distributed_port_group(self) -> pulumi.Output[Optional[str]]:
         """
         Key of the distributed portgroup the nic will connect to.
@@ -658,7 +643,15 @@
     @pulumi.getter
     def portgroup(self) -> pulumi.Output[Optional[str]]:
         """
         Portgroup to attach the nic to. Do not set if you set distributed_switch_port.
         """
         return pulumi.get(self, "portgroup")
 
+    @property
+    @pulumi.getter
+    def services(self) -> pulumi.Output[Optional[Sequence[str]]]:
+        """
+        Enabled services setting for this interface. Current possible values are 'vmotion', 'management', and 'vsan'.
+        """
+        return pulumi.get(self, "services")
+
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere.egg-info/PKG-INFO` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi-vsphere
-Version: 4.5.0a1684391558
+Version: 4.5.0a1684947541
 Summary: A Pulumi package for creating vsphere resources
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-vsphere
 Keywords: pulumi vsphere
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-vsphere/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-vsphere/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fvsphere.svg)](https://www.npmjs.com/package/@pulumi/vsphere)
 [![Python version](https://badge.fury.io/py/pulumi-vsphere.svg)](https://pypi.org/project/pulumi-vsphere)
 [![NuGet version](https://badge.fury.io/nu/pulumi.vsphere.svg)](https://badge.fury.io/nu/pulumi.vsphere)
```

### Comparing `pulumi_vsphere-4.5.0a1684391558/pulumi_vsphere.egg-info/SOURCES.txt` & `pulumi_vsphere-4.5.0a1684947541/pulumi_vsphere.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.5.0a1684391558/setup.py` & `pulumi_vsphere-4.5.0a1684947541/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.5.0a1684391558"
-PLUGIN_VERSION = "4.5.0-alpha.1684391558+17c12b7f"
+VERSION = "4.5.0a1684947541"
+PLUGIN_VERSION = "4.5.0-alpha.1684947541+a62efa8d"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'vsphere', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "vsphere Pulumi Package - Development Version"
 
 
 setup(name='pulumi_vsphere',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating vsphere resources",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

