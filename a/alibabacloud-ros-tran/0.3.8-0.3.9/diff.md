# Comparing `tmp/alibabacloud-ros-tran-0.3.8.tar.gz` & `tmp/alibabacloud-ros-tran-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud-ros-tran-0.3.8.tar", last modified: Wed Mar 15 03:01:26 2023, max compression
+gzip compressed data, was "dist/alibabacloud-ros-tran-0.3.9.tar", last modified: Thu Apr 20 09:17:03 2023, max compression
```

## Comparing `alibabacloud-ros-tran-0.3.8.tar` & `alibabacloud-ros-tran-0.3.9.tar`

### file list

```diff
@@ -1,211 +1,211 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      107 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1860 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      605 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/alibabacloud_ros_tran.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1860 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/alibabacloud_ros_tran.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9512 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/alibabacloud_ros_tran.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/alibabacloud_ros_tran.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/alibabacloud_ros_tran.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       96 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/alibabacloud_ros_tran.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/alibabacloud_ros_tran.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       96 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/
--rw-r--r--   0 root         (0) root         (0)       22 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9328 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/cli/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2713 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/core/conditions.py
--rw-r--r--   0 root         (0) root         (0)     4223 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/core/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1550 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/core/format.py
--rw-r--r--   0 root         (0) root         (0)     2334 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/core/mappings.py
--rw-r--r--   0 root         (0) root         (0)     9533 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/core/metadata.py
--rw-r--r--   0 root         (0) root         (0)     2769 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/core/outputs.py
--rw-r--r--   0 root         (0) root         (0)     9067 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/core/parameters.py
--rw-r--r--   0 root         (0) root         (0)     8275 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/core/properties.py
--rw-r--r--   0 root         (0) root         (0)     7477 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/core/resources.py
--rw-r--r--   0 root         (0) root         (0)     8171 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/core/rules.py
--rw-r--r--   0 root         (0) root         (0)      217 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/core/settings.py
--rw-r--r--   0 root         (0) root         (0)     5168 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/core/template.py
--rw-r--r--   0 root         (0) root         (0)     2079 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/core/utils.py
--rw-r--r--   0 root         (0) root         (0)     1072 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/core/workspace.py
--rw-r--r--   0 root         (0) root         (0)      181 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/providers/
--rw-r--r--   0 root         (0) root         (0)      152 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/providers/cloudformation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/providers/cloudformation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14011 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/providers/cloudformation/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/providers/excel/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/providers/excel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5213 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/providers/excel/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/providers/terraform/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/providers/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18173 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/providers/terraform/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/builtin/
--rw-r--r--   0 root         (0) root         (0)     1146 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/builtin/association_property.yml
--rw-r--r--   0 root         (0) root         (0)      564 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/builtin/function.yml
--rw-r--r--   0 root         (0) root         (0)      212 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/builtin/meta_data.yml
--rw-r--r--   0 root         (0) root         (0)      378 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/builtin/pseudo_parameters.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/
--rw-r--r--   0 root         (0) root         (0)     1231 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_autoscaling_autoscalinggroup.yml
--rw-r--r--   0 root         (0) root         (0)      493 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_autoscaling_lifecyclehook.yml
--rw-r--r--   0 root         (0) root         (0)      291 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_cloudformation_stack.yml
--rw-r--r--   0 root         (0) root         (0)      242 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_cloudformation_waitcondition.yml
--rw-r--r--   0 root         (0) root         (0)      134 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_cloudformation_waitconditionhandle.yml
--rw-r--r--   0 root         (0) root         (0)      269 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_ec2_eip.yml
--rw-r--r--   0 root         (0) root         (0)      310 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_ec2_eipassociation.yml
--rw-r--r--   0 root         (0) root         (0)     1866 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_ec2_instance.yml
--rw-r--r--   0 root         (0) root         (0)      204 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_ec2_natgateway.yml
--rw-r--r--   0 root         (0) root         (0)      672 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_ec2_networkinterface.yml
--rw-r--r--   0 root         (0) root         (0)      306 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_ec2_networkinterfaceattachment.yml
--rw-r--r--   0 root         (0) root         (0)     1282 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_ec2_securitygroup.yml
--rw-r--r--   0 root         (0) root         (0)      499 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_ec2_subnet.yml
--rw-r--r--   0 root         (0) root         (0)      443 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_ec2_volume.yml
--rw-r--r--   0 root         (0) root         (0)      215 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_ec2_volumeattachment.yml
--rw-r--r--   0 root         (0) root         (0)      468 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_ec2_vpc.yml
--rw-r--r--   0 root         (0) root         (0)     1108 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_elasticloadbalancing_loadbalancer.yml
--rw-r--r--   0 root         (0) root         (0)      201 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_iam_accesskey.yml
--rw-r--r--   0 root         (0) root         (0)      383 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_iam_group.yml
--rw-r--r--   0 root         (0) root         (0)      338 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_iam_managedpolicy.yml
--rw-r--r--   0 root         (0) root         (0)      840 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_iam_role.yml
--rw-r--r--   0 root         (0) root         (0)      599 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_iam_user.yml
--rw-r--r--   0 root         (0) root         (0)      192 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_iam_usertogroupaddition.yml
--rw-r--r--   0 root         (0) root         (0)     2242 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_rds_dbinstance.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/
--rw-r--r--   0 root         (0) root         (0)      402 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/actiontrail.yml
--rw-r--r--   0 root         (0) root         (0)      408 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/actiontrail_trail.yml
--rw-r--r--   0 root         (0) root         (0)      222 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/alidns_domain_group.yml
--rw-r--r--   0 root         (0) root         (0)      444 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/alidns_record.yml
--rw-r--r--   0 root         (0) root         (0)      368 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/alikafka_topic.yml
--rw-r--r--   0 root         (0) root         (0)     1850 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/api_gateway_api.yml
--rw-r--r--   0 root         (0) root         (0)      238 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/api_gateway_app.yml
--rw-r--r--   0 root         (0) root         (0)      308 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/api_gateway_app_attachment.yml
--rw-r--r--   0 root         (0) root         (0)      288 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/api_gateway_group.yml
--rw-r--r--   0 root         (0) root         (0)      221 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/cas_certificate.yml
--rw-r--r--   0 root         (0) root         (0)      822 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/cdn_domain.yml
--rw-r--r--   0 root         (0) root         (0)      268 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/cdn_domain_config.yml
--rw-r--r--   0 root         (0) root         (0)      274 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/cen_bandwidth_limit.yml
--rw-r--r--   0 root         (0) root         (0)      453 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/cen_bandwidth_package.yml
--rw-r--r--   0 root         (0) root         (0)      281 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/cen_bandwidth_package_attachment.yml
--rw-r--r--   0 root         (0) root         (0)      301 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/cen_instance.yml
--rw-r--r--   0 root         (0) root         (0)      368 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/cen_instance_attachment.yml
--rw-r--r--   0 root         (0) root         (0)      417 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/common_bandwidth_package.yml
--rw-r--r--   0 root         (0) root         (0)      278 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/common_bandwidth_package_attachment.yml
--rw-r--r--   0 root         (0) root         (0)      355 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/cr_ee_repo.yml
--rw-r--r--   0 root         (0) root         (0)      267 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/cr_namespace.yml
--rw-r--r--   0 root         (0) root         (0)      326 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/cr_repo.yml
--rw-r--r--   0 root         (0) root         (0)     1786 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/cs_kubernetes.yml
--rw-r--r--   0 root         (0) root         (0)     1768 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/cs_managed_kubernetes.yml
--rw-r--r--   0 root         (0) root         (0)      814 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/cs_serverless_kubernetes.yml
--rw-r--r--   0 root         (0) root         (0)      289 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/datahub_project.yml
--rw-r--r--   0 root         (0) root         (0)      454 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/datahub_topic.yml
--rw-r--r--   0 root         (0) root         (0)      409 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/db_account.yml
--rw-r--r--   0 root         (0) root         (0)      282 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/db_account_privilege.yml
--rw-r--r--   0 root         (0) root         (0)      284 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/db_database.yml
--rw-r--r--   0 root         (0) root         (0)     1236 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/db_instance.yml
--rw-r--r--   0 root         (0) root         (0)      647 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/db_readonly_instance.yml
--rw-r--r--   0 root         (0) root         (0)      618 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/disk.yml
--rw-r--r--   0 root         (0) root         (0)      320 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/disk_attachment.yml
--rw-r--r--   0 root         (0) root         (0)      905 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/dms_enterprise_instance.yml
--rw-r--r--   0 root         (0) root         (0)      394 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/dns_domain.yml
--rw-r--r--   0 root         (0) root         (0)      206 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/dns_group.yml
--rw-r--r--   0 root         (0) root         (0)      555 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/dns_record.yml
--rw-r--r--   0 root         (0) root         (0)      383 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/drds_instance.yml
--rw-r--r--   0 root         (0) root         (0)      757 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/eci_image_cache.yml
--rw-r--r--   0 root         (0) root         (0)      976 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ecs_dedicated_host.yml
--rw-r--r--   0 root         (0) root         (0)      592 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/edas_application.yml
--rw-r--r--   0 root         (0) root         (0)      334 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/edas_cluster.yml
--rw-r--r--   0 root         (0) root         (0)      266 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/edas_deploy_group.yml
--rw-r--r--   0 root         (0) root         (0)      576 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/eip.yml
--rw-r--r--   0 root         (0) root         (0)      365 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/eip_association.yml
--rw-r--r--   0 root         (0) root         (0)     1237 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/elasticsearch.yml
--rw-r--r--   0 root         (0) root         (0)     1646 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/emr_cluster.yml
--rw-r--r--   0 root         (0) root         (0)      673 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ess_alarm.yml
--rw-r--r--   0 root         (0) root         (0)     1983 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ess_scaling_configuration.yml
--rw-r--r--   0 root         (0) root         (0)     1059 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ess_scaling_group.yml
--rw-r--r--   0 root         (0) root         (0)      750 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ess_scaling_lifecycle_hook.yml
--rw-r--r--   0 root         (0) root         (0)      859 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ess_scaling_rule.yml
--rw-r--r--   0 root         (0) root         (0)      696 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ess_scheduled_task.yml
--rw-r--r--   0 root         (0) root         (0)      697 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/fc_function.yml
--rw-r--r--   0 root         (0) root         (0)      661 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/fc_service.yml
--rw-r--r--   0 root         (0) root         (0)      531 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/fc_trigger.yml
--rw-r--r--   0 root         (0) root         (0)      450 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/forward_entry.yml
--rw-r--r--   0 root         (0) root         (0)      628 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/image.yml
--rw-r--r--   0 root         (0) root         (0)      401 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/image_copy.yml
--rw-r--r--   0 root         (0) root         (0)     2263 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/instance.yml
--rw-r--r--   0 root         (0) root         (0)      411 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/key_pair.yml
--rw-r--r--   0 root         (0) root         (0)      308 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/key_pair_attachment.yml
--rw-r--r--   0 root         (0) root         (0)      206 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/kms_alias.yml
--rw-r--r--   0 root         (0) root         (0)      850 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/kms_key.yml
--rw-r--r--   0 root         (0) root         (0)     1065 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/kvstore_instance.yml
--rw-r--r--   0 root         (0) root         (0)     1908 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/launch_template.yml
--rw-r--r--   0 root         (0) root         (0)      494 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/log_machine_group.yml
--rw-r--r--   0 root         (0) root         (0)      227 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/log_project.yml
--rw-r--r--   0 root         (0) root         (0)      709 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/log_store.yml
--rw-r--r--   0 root         (0) root         (0)      993 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/log_store_index.yml
--rw-r--r--   0 root         (0) root         (0)      419 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/market_order.yml
--rw-r--r--   0 root         (0) root         (0)      423 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/mns_queue.yml
--rw-r--r--   0 root         (0) root         (0)      270 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/mns_topic.yml
--rw-r--r--   0 root         (0) root         (0)      391 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/mns_topic_subscription.yml
--rw-r--r--   0 root         (0) root         (0)     1107 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/mongodb_instance.yml
--rw-r--r--   0 root         (0) root         (0)     1065 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/mongodb_sharding_instance.yml
--rw-r--r--   0 root         (0) root         (0)      425 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/nas_access_group.yml
--rw-r--r--   0 root         (0) root         (0)      395 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/nas_access_rule.yml
--rw-r--r--   0 root         (0) root         (0)      383 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/nas_file_system.yml
--rw-r--r--   0 root         (0) root         (0)      313 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/nas_mount_target.yml
--rw-r--r--   0 root         (0) root         (0)      687 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/nat_gateway.yml
--rw-r--r--   0 root         (0) root         (0)      812 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/oos_execution.yml
--rw-r--r--   0 root         (0) root         (0)      686 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/oos_template.yml
--rw-r--r--   0 root         (0) root         (0)     1648 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/oss_bucket.yml
--rw-r--r--   0 root         (0) root         (0)      465 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ots_instance.yml
--rw-r--r--   0 root         (0) root         (0)      715 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ots_table.yml
--rw-r--r--   0 root         (0) root         (0)      451 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/polardb_account.yml
--rw-r--r--   0 root         (0) root         (0)      407 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/polardb_account_privilege.yml
--rw-r--r--   0 root         (0) root         (0)      714 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/polardb_cluster.yml
--rw-r--r--   0 root         (0) root         (0)      316 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/polardb_database.yml
--rw-r--r--   0 root         (0) root         (0)      400 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/polardb_endpoint.yml
--rw-r--r--   0 root         (0) root         (0)      445 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/polardb_endpoint_address.yml
--rw-r--r--   0 root         (0) root         (0)      367 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/pvtz_zone.yml
--rw-r--r--   0 root         (0) root         (0)      341 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/pvtz_zone_record.yml
--rw-r--r--   0 root         (0) root         (0)      440 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ram_access_key.yml
--rw-r--r--   0 root         (0) root         (0)      286 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ram_group.yml
--rw-r--r--   0 root         (0) root         (0)      639 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ram_role.yml
--rw-r--r--   0 root         (0) root         (0)      278 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ram_role_policy_attachment.yml
--rw-r--r--   0 root         (0) root         (0)      318 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ram_user.yml
--rw-r--r--   0 root         (0) root         (0)      332 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ram_user_policy_attachment.yml
--rw-r--r--   0 root         (0) root         (0)      268 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/route_table.yml
--rw-r--r--   0 root         (0) root         (0)      267 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/route_table_attachment.yml
--rw-r--r--   0 root         (0) root         (0)     1404 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/router_interface.yml
--rw-r--r--   0 root         (0) root         (0)      427 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/router_interface_connection.yml
--rw-r--r--   0 root         (0) root         (0)      164 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/sag_acl.yml
--rw-r--r--   0 root         (0) root         (0)      480 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/sag_acl_rule.yml
--rw-r--r--   0 root         (0) root         (0)      445 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/security_group.yml
--rw-r--r--   0 root         (0) root         (0)     1054 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/security_group_rule.yml
--rw-r--r--   0 root         (0) root         (0)      767 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/slb.yml
--rw-r--r--   0 root         (0) root         (0)      404 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/slb_acl.yml
--rw-r--r--   0 root         (0) root         (0)      642 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/slb_attachment.yml
--rw-r--r--   0 root         (0) root         (0)      482 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/slb_backend_server.yml
--rw-r--r--   0 root         (0) root         (0)      388 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/slb_domain_extension.yml
--rw-r--r--   0 root         (0) root         (0)     2535 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/slb_listener.yml
--rw-r--r--   0 root         (0) root         (0)      719 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/slb_master_slave_server_group.yml
--rw-r--r--   0 root         (0) root         (0)      521 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/slb_server_certificate.yml
--rw-r--r--   0 root         (0) root         (0)      681 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/slb_server_group.yml
--rw-r--r--   0 root         (0) root         (0)      307 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/snapshot.yml
--rw-r--r--   0 root         (0) root         (0)      368 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/snat_entry.yml
--rw-r--r--   0 root         (0) root         (0)      398 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ssl_vpn_client_cert.yml
--rw-r--r--   0 root         (0) root         (0)      504 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ssl_vpn_server.yml
--rw-r--r--   0 root         (0) root         (0)      452 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/vpc.yml
--rw-r--r--   0 root         (0) root         (0)     1141 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/vpn_connection.yml
--rw-r--r--   0 root         (0) root         (0)      479 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/vswitch.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1656 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/tools/generate.py
--rw-r--r--   0 root         (0) root         (0)     6696 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/rostran/tools/parse_tf_ros.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1914 2023-03-15 03:01:26.000000 alibabacloud-ros-tran-0.3.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      107 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1860 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      605 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/alibabacloud_ros_tran.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1860 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/alibabacloud_ros_tran.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9512 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/alibabacloud_ros_tran.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/alibabacloud_ros_tran.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/alibabacloud_ros_tran.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/alibabacloud_ros_tran.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/alibabacloud_ros_tran.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9328 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/cli/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2713 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/core/conditions.py
+-rw-r--r--   0 root         (0) root         (0)     4223 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/core/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/core/format.py
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/core/mappings.py
+-rw-r--r--   0 root         (0) root         (0)     9533 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/core/metadata.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/core/outputs.py
+-rw-r--r--   0 root         (0) root         (0)     9067 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/core/parameters.py
+-rw-r--r--   0 root         (0) root         (0)     8275 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/core/properties.py
+-rw-r--r--   0 root         (0) root         (0)     7477 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/core/resources.py
+-rw-r--r--   0 root         (0) root         (0)     8171 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/core/rules.py
+-rw-r--r--   0 root         (0) root         (0)      217 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/core/settings.py
+-rw-r--r--   0 root         (0) root         (0)     5168 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/core/template.py
+-rw-r--r--   0 root         (0) root         (0)     2079 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/core/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/core/workspace.py
+-rw-r--r--   0 root         (0) root         (0)      181 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/providers/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/providers/cloudformation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/providers/cloudformation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14011 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/providers/cloudformation/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/providers/excel/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/providers/excel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5213 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/providers/excel/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/providers/terraform/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/providers/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18186 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/providers/terraform/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/builtin/
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/builtin/association_property.yml
+-rw-r--r--   0 root         (0) root         (0)      564 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/builtin/function.yml
+-rw-r--r--   0 root         (0) root         (0)      212 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/builtin/meta_data.yml
+-rw-r--r--   0 root         (0) root         (0)      378 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/builtin/pseudo_parameters.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/
+-rw-r--r--   0 root         (0) root         (0)     1231 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_autoscaling_autoscalinggroup.yml
+-rw-r--r--   0 root         (0) root         (0)      493 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_autoscaling_lifecyclehook.yml
+-rw-r--r--   0 root         (0) root         (0)      291 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_cloudformation_stack.yml
+-rw-r--r--   0 root         (0) root         (0)      242 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_cloudformation_waitcondition.yml
+-rw-r--r--   0 root         (0) root         (0)      134 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_cloudformation_waitconditionhandle.yml
+-rw-r--r--   0 root         (0) root         (0)      269 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_ec2_eip.yml
+-rw-r--r--   0 root         (0) root         (0)      310 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_ec2_eipassociation.yml
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_ec2_instance.yml
+-rw-r--r--   0 root         (0) root         (0)      204 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_ec2_natgateway.yml
+-rw-r--r--   0 root         (0) root         (0)      672 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_ec2_networkinterface.yml
+-rw-r--r--   0 root         (0) root         (0)      306 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_ec2_networkinterfaceattachment.yml
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_ec2_securitygroup.yml
+-rw-r--r--   0 root         (0) root         (0)      499 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_ec2_subnet.yml
+-rw-r--r--   0 root         (0) root         (0)      443 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_ec2_volume.yml
+-rw-r--r--   0 root         (0) root         (0)      215 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_ec2_volumeattachment.yml
+-rw-r--r--   0 root         (0) root         (0)      468 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_ec2_vpc.yml
+-rw-r--r--   0 root         (0) root         (0)     1108 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_elasticloadbalancing_loadbalancer.yml
+-rw-r--r--   0 root         (0) root         (0)      201 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_iam_accesskey.yml
+-rw-r--r--   0 root         (0) root         (0)      383 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_iam_group.yml
+-rw-r--r--   0 root         (0) root         (0)      338 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_iam_managedpolicy.yml
+-rw-r--r--   0 root         (0) root         (0)      840 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_iam_role.yml
+-rw-r--r--   0 root         (0) root         (0)      599 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_iam_user.yml
+-rw-r--r--   0 root         (0) root         (0)      192 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_iam_usertogroupaddition.yml
+-rw-r--r--   0 root         (0) root         (0)     2242 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_rds_dbinstance.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/
+-rw-r--r--   0 root         (0) root         (0)      402 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/actiontrail.yml
+-rw-r--r--   0 root         (0) root         (0)      408 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/actiontrail_trail.yml
+-rw-r--r--   0 root         (0) root         (0)      222 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/alidns_domain_group.yml
+-rw-r--r--   0 root         (0) root         (0)      444 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/alidns_record.yml
+-rw-r--r--   0 root         (0) root         (0)      368 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/alikafka_topic.yml
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/api_gateway_api.yml
+-rw-r--r--   0 root         (0) root         (0)      238 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/api_gateway_app.yml
+-rw-r--r--   0 root         (0) root         (0)      308 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/api_gateway_app_attachment.yml
+-rw-r--r--   0 root         (0) root         (0)      288 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/api_gateway_group.yml
+-rw-r--r--   0 root         (0) root         (0)      221 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/cas_certificate.yml
+-rw-r--r--   0 root         (0) root         (0)      822 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/cdn_domain.yml
+-rw-r--r--   0 root         (0) root         (0)      268 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/cdn_domain_config.yml
+-rw-r--r--   0 root         (0) root         (0)      274 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/cen_bandwidth_limit.yml
+-rw-r--r--   0 root         (0) root         (0)      453 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/cen_bandwidth_package.yml
+-rw-r--r--   0 root         (0) root         (0)      281 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/cen_bandwidth_package_attachment.yml
+-rw-r--r--   0 root         (0) root         (0)      301 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/cen_instance.yml
+-rw-r--r--   0 root         (0) root         (0)      368 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/cen_instance_attachment.yml
+-rw-r--r--   0 root         (0) root         (0)      417 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/common_bandwidth_package.yml
+-rw-r--r--   0 root         (0) root         (0)      278 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/common_bandwidth_package_attachment.yml
+-rw-r--r--   0 root         (0) root         (0)      355 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/cr_ee_repo.yml
+-rw-r--r--   0 root         (0) root         (0)      267 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/cr_namespace.yml
+-rw-r--r--   0 root         (0) root         (0)      326 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/cr_repo.yml
+-rw-r--r--   0 root         (0) root         (0)     1786 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/cs_kubernetes.yml
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/cs_managed_kubernetes.yml
+-rw-r--r--   0 root         (0) root         (0)      814 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/cs_serverless_kubernetes.yml
+-rw-r--r--   0 root         (0) root         (0)      289 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/datahub_project.yml
+-rw-r--r--   0 root         (0) root         (0)      454 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/datahub_topic.yml
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/db_account.yml
+-rw-r--r--   0 root         (0) root         (0)      282 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/db_account_privilege.yml
+-rw-r--r--   0 root         (0) root         (0)      284 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/db_database.yml
+-rw-r--r--   0 root         (0) root         (0)     1236 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/db_instance.yml
+-rw-r--r--   0 root         (0) root         (0)      647 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/db_readonly_instance.yml
+-rw-r--r--   0 root         (0) root         (0)      618 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/disk.yml
+-rw-r--r--   0 root         (0) root         (0)      320 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/disk_attachment.yml
+-rw-r--r--   0 root         (0) root         (0)      905 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/dms_enterprise_instance.yml
+-rw-r--r--   0 root         (0) root         (0)      394 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/dns_domain.yml
+-rw-r--r--   0 root         (0) root         (0)      206 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/dns_group.yml
+-rw-r--r--   0 root         (0) root         (0)      555 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/dns_record.yml
+-rw-r--r--   0 root         (0) root         (0)      383 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/drds_instance.yml
+-rw-r--r--   0 root         (0) root         (0)      757 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/eci_image_cache.yml
+-rw-r--r--   0 root         (0) root         (0)      976 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ecs_dedicated_host.yml
+-rw-r--r--   0 root         (0) root         (0)      592 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/edas_application.yml
+-rw-r--r--   0 root         (0) root         (0)      334 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/edas_cluster.yml
+-rw-r--r--   0 root         (0) root         (0)      266 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/edas_deploy_group.yml
+-rw-r--r--   0 root         (0) root         (0)      576 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/eip.yml
+-rw-r--r--   0 root         (0) root         (0)      365 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/eip_association.yml
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/elasticsearch.yml
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/emr_cluster.yml
+-rw-r--r--   0 root         (0) root         (0)      673 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ess_alarm.yml
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ess_scaling_configuration.yml
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ess_scaling_group.yml
+-rw-r--r--   0 root         (0) root         (0)      750 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ess_scaling_lifecycle_hook.yml
+-rw-r--r--   0 root         (0) root         (0)      859 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ess_scaling_rule.yml
+-rw-r--r--   0 root         (0) root         (0)      696 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ess_scheduled_task.yml
+-rw-r--r--   0 root         (0) root         (0)      697 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/fc_function.yml
+-rw-r--r--   0 root         (0) root         (0)      661 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/fc_service.yml
+-rw-r--r--   0 root         (0) root         (0)      531 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/fc_trigger.yml
+-rw-r--r--   0 root         (0) root         (0)      450 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/forward_entry.yml
+-rw-r--r--   0 root         (0) root         (0)      628 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/image.yml
+-rw-r--r--   0 root         (0) root         (0)      401 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/image_copy.yml
+-rw-r--r--   0 root         (0) root         (0)     2263 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/instance.yml
+-rw-r--r--   0 root         (0) root         (0)      411 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/key_pair.yml
+-rw-r--r--   0 root         (0) root         (0)      308 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/key_pair_attachment.yml
+-rw-r--r--   0 root         (0) root         (0)      206 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/kms_alias.yml
+-rw-r--r--   0 root         (0) root         (0)      850 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/kms_key.yml
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/kvstore_instance.yml
+-rw-r--r--   0 root         (0) root         (0)     1908 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/launch_template.yml
+-rw-r--r--   0 root         (0) root         (0)      494 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/log_machine_group.yml
+-rw-r--r--   0 root         (0) root         (0)      227 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/log_project.yml
+-rw-r--r--   0 root         (0) root         (0)      709 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/log_store.yml
+-rw-r--r--   0 root         (0) root         (0)      993 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/log_store_index.yml
+-rw-r--r--   0 root         (0) root         (0)      419 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/market_order.yml
+-rw-r--r--   0 root         (0) root         (0)      423 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/mns_queue.yml
+-rw-r--r--   0 root         (0) root         (0)      270 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/mns_topic.yml
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/mns_topic_subscription.yml
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/mongodb_instance.yml
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/mongodb_sharding_instance.yml
+-rw-r--r--   0 root         (0) root         (0)      425 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/nas_access_group.yml
+-rw-r--r--   0 root         (0) root         (0)      395 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/nas_access_rule.yml
+-rw-r--r--   0 root         (0) root         (0)      383 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/nas_file_system.yml
+-rw-r--r--   0 root         (0) root         (0)      313 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/nas_mount_target.yml
+-rw-r--r--   0 root         (0) root         (0)      687 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/nat_gateway.yml
+-rw-r--r--   0 root         (0) root         (0)      812 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/oos_execution.yml
+-rw-r--r--   0 root         (0) root         (0)      686 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/oos_template.yml
+-rw-r--r--   0 root         (0) root         (0)     1648 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/oss_bucket.yml
+-rw-r--r--   0 root         (0) root         (0)      465 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ots_instance.yml
+-rw-r--r--   0 root         (0) root         (0)      715 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ots_table.yml
+-rw-r--r--   0 root         (0) root         (0)      451 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/polardb_account.yml
+-rw-r--r--   0 root         (0) root         (0)      407 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/polardb_account_privilege.yml
+-rw-r--r--   0 root         (0) root         (0)      714 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/polardb_cluster.yml
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/polardb_database.yml
+-rw-r--r--   0 root         (0) root         (0)      400 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/polardb_endpoint.yml
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/polardb_endpoint_address.yml
+-rw-r--r--   0 root         (0) root         (0)      367 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/pvtz_zone.yml
+-rw-r--r--   0 root         (0) root         (0)      341 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/pvtz_zone_record.yml
+-rw-r--r--   0 root         (0) root         (0)      440 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ram_access_key.yml
+-rw-r--r--   0 root         (0) root         (0)      286 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ram_group.yml
+-rw-r--r--   0 root         (0) root         (0)      639 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ram_role.yml
+-rw-r--r--   0 root         (0) root         (0)      278 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ram_role_policy_attachment.yml
+-rw-r--r--   0 root         (0) root         (0)      318 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ram_user.yml
+-rw-r--r--   0 root         (0) root         (0)      332 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ram_user_policy_attachment.yml
+-rw-r--r--   0 root         (0) root         (0)      268 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/route_table.yml
+-rw-r--r--   0 root         (0) root         (0)      267 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/route_table_attachment.yml
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/router_interface.yml
+-rw-r--r--   0 root         (0) root         (0)      427 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/router_interface_connection.yml
+-rw-r--r--   0 root         (0) root         (0)      164 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/sag_acl.yml
+-rw-r--r--   0 root         (0) root         (0)      480 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/sag_acl_rule.yml
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/security_group.yml
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/security_group_rule.yml
+-rw-r--r--   0 root         (0) root         (0)      767 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/slb.yml
+-rw-r--r--   0 root         (0) root         (0)      404 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/slb_acl.yml
+-rw-r--r--   0 root         (0) root         (0)      642 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/slb_attachment.yml
+-rw-r--r--   0 root         (0) root         (0)      482 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/slb_backend_server.yml
+-rw-r--r--   0 root         (0) root         (0)      388 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/slb_domain_extension.yml
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/slb_listener.yml
+-rw-r--r--   0 root         (0) root         (0)      719 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/slb_master_slave_server_group.yml
+-rw-r--r--   0 root         (0) root         (0)      521 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/slb_server_certificate.yml
+-rw-r--r--   0 root         (0) root         (0)      681 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/slb_server_group.yml
+-rw-r--r--   0 root         (0) root         (0)      307 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/snapshot.yml
+-rw-r--r--   0 root         (0) root         (0)      368 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/snat_entry.yml
+-rw-r--r--   0 root         (0) root         (0)      398 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ssl_vpn_client_cert.yml
+-rw-r--r--   0 root         (0) root         (0)      504 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ssl_vpn_server.yml
+-rw-r--r--   0 root         (0) root         (0)      452 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/vpc.yml
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/vpn_connection.yml
+-rw-r--r--   0 root         (0) root         (0)      479 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/vswitch.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/tools/generate.py
+-rw-r--r--   0 root         (0) root         (0)     6696 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/rostran/tools/parse_tf_ros.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-04-20 09:17:03.000000 alibabacloud-ros-tran-0.3.9/setup.py
```

### Comparing `alibabacloud-ros-tran-0.3.8/LICENSE` & `alibabacloud-ros-tran-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/PKG-INFO` & `alibabacloud-ros-tran-0.3.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: alibabacloud-ros-tran
-Version: 0.3.8
+Version: 0.3.9
 Summary: Resource Orchestration Service Template Transformer.
 Home-page: https://www.alibabacloud.com/product/ros
 Author: AlibabaCloud
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache License 2.0
 Description: # ROS Template Transformer
         [ROS(Resource Orchestration Service)](https://www.alibabacloud.com/help/resource-orchestration-service) Template Transformer
```

### Comparing `alibabacloud-ros-tran-0.3.8/README.md` & `alibabacloud-ros-tran-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/alibabacloud_ros_tran.egg-info/PKG-INFO` & `alibabacloud-ros-tran-0.3.9/alibabacloud_ros_tran.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: alibabacloud-ros-tran
-Version: 0.3.8
+Version: 0.3.9
 Summary: Resource Orchestration Service Template Transformer.
 Home-page: https://www.alibabacloud.com/product/ros
 Author: AlibabaCloud
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache License 2.0
 Description: # ROS Template Transformer
         [ROS(Resource Orchestration Service)](https://www.alibabacloud.com/help/resource-orchestration-service) Template Transformer
```

### Comparing `alibabacloud-ros-tran-0.3.8/alibabacloud_ros_tran.egg-info/SOURCES.txt` & `alibabacloud-ros-tran-0.3.9/alibabacloud_ros_tran.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/cli/__main__.py` & `alibabacloud-ros-tran-0.3.9/rostran/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/core/conditions.py` & `alibabacloud-ros-tran-0.3.9/rostran/core/conditions.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/core/exceptions.py` & `alibabacloud-ros-tran-0.3.9/rostran/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/core/format.py` & `alibabacloud-ros-tran-0.3.9/rostran/core/format.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/core/mappings.py` & `alibabacloud-ros-tran-0.3.9/rostran/core/mappings.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/core/metadata.py` & `alibabacloud-ros-tran-0.3.9/rostran/core/metadata.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/core/outputs.py` & `alibabacloud-ros-tran-0.3.9/rostran/core/outputs.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/core/parameters.py` & `alibabacloud-ros-tran-0.3.9/rostran/core/parameters.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/core/properties.py` & `alibabacloud-ros-tran-0.3.9/rostran/core/properties.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/core/resources.py` & `alibabacloud-ros-tran-0.3.9/rostran/core/resources.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/core/rules.py` & `alibabacloud-ros-tran-0.3.9/rostran/core/rules.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/core/template.py` & `alibabacloud-ros-tran-0.3.9/rostran/core/template.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/core/utils.py` & `alibabacloud-ros-tran-0.3.9/rostran/core/utils.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/core/workspace.py` & `alibabacloud-ros-tran-0.3.9/rostran/core/workspace.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/providers/cloudformation/template.py` & `alibabacloud-ros-tran-0.3.9/rostran/providers/cloudformation/template.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/providers/excel/template.py` & `alibabacloud-ros-tran-0.3.9/rostran/providers/excel/template.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/providers/terraform/template.py` & `alibabacloud-ros-tran-0.3.9/rostran/providers/terraform/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 class TerraformTemplate(Template):
     PROVIDERS = (ALICLOUD, AWS,) = (
         "alicloud",
         "aws",
     )
 
-    SUPPORTED_PLAN_FORMAT_VERSIONS = ("1.0",)
+    SUPPORTED_PLAN_FORMAT_VERSIONS = ("1.0", "1.1", "1.2")
 
     PLAN_PROPERTIES = (
         P_FORMAT_VERSION,
         P_CONFIGURATION,
         P_PLANNED_VALUES,
         P_RESOURCES,
         P_PROVIDER_CONFIG,
```

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/builtin/association_property.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/builtin/association_property.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/builtin/function.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/builtin/function.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_autoscaling_autoscalinggroup.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_autoscaling_autoscalinggroup.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_ec2_instance.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_ec2_instance.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_ec2_networkinterface.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_ec2_networkinterface.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_ec2_securitygroup.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_ec2_securitygroup.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_elasticloadbalancing_loadbalancer.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_elasticloadbalancing_loadbalancer.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_iam_role.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_iam_role.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_iam_user.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_iam_user.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/cloudformation/resource/aws_rds_dbinstance.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/cloudformation/resource/aws_rds_dbinstance.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/api_gateway_api.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/api_gateway_api.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/cdn_domain.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/cdn_domain.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/cs_kubernetes.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/cs_kubernetes.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/cs_managed_kubernetes.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/cs_managed_kubernetes.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/cs_serverless_kubernetes.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/cs_serverless_kubernetes.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/db_instance.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/db_instance.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/db_readonly_instance.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/db_readonly_instance.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/disk.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/disk.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/dms_enterprise_instance.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/dms_enterprise_instance.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/dns_record.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/dns_record.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/eci_image_cache.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/eci_image_cache.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ecs_dedicated_host.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ecs_dedicated_host.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/edas_application.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/edas_application.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/eip.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/eip.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/elasticsearch.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/elasticsearch.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/emr_cluster.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/emr_cluster.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ess_alarm.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ess_alarm.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ess_scaling_configuration.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ess_scaling_configuration.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ess_scaling_group.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ess_scaling_group.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ess_scaling_lifecycle_hook.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ess_scaling_lifecycle_hook.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ess_scaling_rule.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ess_scaling_rule.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ess_scheduled_task.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ess_scheduled_task.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/fc_function.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/fc_function.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/fc_service.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/fc_service.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/fc_trigger.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/fc_trigger.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/image.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/image.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/instance.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/instance.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/kms_key.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/kms_key.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/kvstore_instance.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/kvstore_instance.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/launch_template.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/launch_template.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/log_store.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/log_store.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/log_store_index.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/log_store_index.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/mongodb_instance.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/mongodb_instance.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/mongodb_sharding_instance.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/mongodb_sharding_instance.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/nat_gateway.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/nat_gateway.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/oos_execution.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/oos_execution.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/oos_template.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/oos_template.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/oss_bucket.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/oss_bucket.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ots_table.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ots_table.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/polardb_cluster.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/polardb_cluster.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/ram_role.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/ram_role.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/router_interface.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/router_interface.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/security_group_rule.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/security_group_rule.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/slb.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/slb.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/slb_attachment.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/slb_attachment.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/slb_listener.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/slb_listener.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/slb_master_slave_server_group.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/slb_master_slave_server_group.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/slb_server_certificate.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/slb_server_certificate.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/slb_server_group.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/slb_server_group.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/rules/terraform/alicloud/vpn_connection.yml` & `alibabacloud-ros-tran-0.3.9/rostran/rules/terraform/alicloud/vpn_connection.yml`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/tools/generate.py` & `alibabacloud-ros-tran-0.3.9/rostran/tools/generate.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/rostran/tools/parse_tf_ros.py` & `alibabacloud-ros-tran-0.3.9/rostran/tools/parse_tf_ros.py`

 * *Files identical despite different names*

### Comparing `alibabacloud-ros-tran-0.3.8/setup.py` & `alibabacloud-ros-tran-0.3.9/setup.py`

 * *Files identical despite different names*

