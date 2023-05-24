# Comparing `tmp/pulumi_aws_iam-0.1.0.tar.gz` & `tmp/pulumi_aws_iam-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_aws_iam-0.1.0.tar", last modified: Thu Dec 22 21:59:33 2022, max compression
+gzip compressed data, was "pulumi_aws_iam-0.2.0.tar", last modified: Wed May 24 18:29:48 2023, max compression
```

## Comparing `pulumi_aws_iam-0.1.0.tar` & `pulumi_aws_iam-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 21:59:33.050206 pulumi_aws_iam-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2022-12-22 21:59:33.050206 pulumi_aws_iam-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2022-12-22 21:59:32.000000 pulumi_aws_iam-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 21:59:33.050206 pulumi_aws_iam-0.1.0/pulumi_aws_iam/
--rw-------   0 runner    (1001) docker     (123)     1768 2022-12-22 21:59:32.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam/__init__.py
--rw-------   0 runner    (1001) docker     (123)    80107 2022-12-22 21:59:32.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam/_inputs.py
--rw-------   0 runner    (1001) docker     (123)     7647 2022-12-22 21:59:32.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam/_utilities.py
--rw-------   0 runner    (1001) docker     (123)     8634 2022-12-22 21:59:32.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam/account.py
--rw-------   0 runner    (1001) docker     (123)    20225 2022-12-22 21:59:32.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam/assumable_role.py
--rw-------   0 runner    (1001) docker     (123)    16598 2022-12-22 21:59:32.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam/assumable_role_with_oidc.py
--rw-------   0 runner    (1001) docker     (123)    11837 2022-12-22 21:59:32.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam/assumable_role_with_saml.py
--rw-------   0 runner    (1001) docker     (123)    13282 2022-12-22 21:59:32.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam/assumable_roles.py
--rw-------   0 runner    (1001) docker     (123)    11842 2022-12-22 21:59:32.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam/assumable_roles_with_saml.py
--rw-------   0 runner    (1001) docker     (123)    15650 2022-12-22 21:59:32.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam/eks_role.py
--rw-------   0 runner    (1001) docker     (123)     9711 2022-12-22 21:59:32.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam/group_with_assumable_roles_policy.py
--rw-------   0 runner    (1001) docker     (123)    15848 2022-12-22 21:59:32.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam/group_with_policies.py
--rw-------   0 runner    (1001) docker     (123)    11917 2022-12-22 21:59:32.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam/outputs.py
--rw-------   0 runner    (1001) docker     (123)     9846 2022-12-22 21:59:32.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam/policy.py
--rw-------   0 runner    (1001) docker     (123)     2784 2022-12-22 21:59:32.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam/provider.py
--rw-------   0 runner    (1001) docker     (123)       44 2022-12-22 21:59:32.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (123)        0 2022-12-22 21:59:32.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam/py.typed
--rw-------   0 runner    (1001) docker     (123)    18380 2022-12-22 21:59:32.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam/read_only_policy.py
--rw-------   0 runner    (1001) docker     (123)    15384 2022-12-22 21:59:32.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam/role_for_service_accounts_eks.py
--rw-------   0 runner    (1001) docker     (123)    16968 2022-12-22 21:59:32.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 21:59:33.050206 pulumi_aws_iam-0.1.0/pulumi_aws_iam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2022-12-22 21:59:33.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2022-12-22 21:59:33.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 21:59:33.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 21:59:33.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-22 21:59:33.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-22 21:59:33.000000 pulumi_aws_iam-0.1.0/pulumi_aws_iam.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-22 21:59:33.050206 pulumi_aws_iam-0.1.0/setup.cfg
--rw-------   0 runner    (1001) docker     (123)     1836 2022-12-22 21:59:32.000000 pulumi_aws_iam-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:29:48.213239 pulumi_aws_iam-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-24 18:29:48.213239 pulumi_aws_iam-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-24 18:29:47.000000 pulumi_aws_iam-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:29:48.213239 pulumi_aws_iam-0.2.0/pulumi_aws_iam/
+-rw-------   0 runner    (1001) docker     (123)     1768 2023-05-24 18:29:47.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam/__init__.py
+-rw-------   0 runner    (1001) docker     (123)    80119 2023-05-24 18:29:47.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam/_inputs.py
+-rw-------   0 runner    (1001) docker     (123)     8061 2023-05-24 18:29:47.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam/_utilities.py
+-rw-------   0 runner    (1001) docker     (123)     8583 2023-05-24 18:29:47.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam/account.py
+-rw-------   0 runner    (1001) docker     (123)    20174 2023-05-24 18:29:47.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam/assumable_role.py
+-rw-------   0 runner    (1001) docker     (123)    16547 2023-05-24 18:29:47.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam/assumable_role_with_oidc.py
+-rw-------   0 runner    (1001) docker     (123)    11786 2023-05-24 18:29:47.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam/assumable_role_with_saml.py
+-rw-------   0 runner    (1001) docker     (123)    13231 2023-05-24 18:29:47.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam/assumable_roles.py
+-rw-------   0 runner    (1001) docker     (123)    11791 2023-05-24 18:29:47.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam/assumable_roles_with_saml.py
+-rw-------   0 runner    (1001) docker     (123)    15599 2023-05-24 18:29:47.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam/eks_role.py
+-rw-------   0 runner    (1001) docker     (123)     9660 2023-05-24 18:29:47.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam/group_with_assumable_roles_policy.py
+-rw-------   0 runner    (1001) docker     (123)    15797 2023-05-24 18:29:47.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam/group_with_policies.py
+-rw-------   0 runner    (1001) docker     (123)    11929 2023-05-24 18:29:47.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam/outputs.py
+-rw-------   0 runner    (1001) docker     (123)     9795 2023-05-24 18:29:47.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam/policy.py
+-rw-------   0 runner    (1001) docker     (123)     2733 2023-05-24 18:29:47.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam/provider.py
+-rw-------   0 runner    (1001) docker     (123)       44 2023-05-24 18:29:47.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (123)        0 2023-05-24 18:29:47.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam/py.typed
+-rw-------   0 runner    (1001) docker     (123)    18329 2023-05-24 18:29:47.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam/read_only_policy.py
+-rw-------   0 runner    (1001) docker     (123)    15333 2023-05-24 18:29:47.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam/role_for_service_accounts_eks.py
+-rw-------   0 runner    (1001) docker     (123)    16917 2023-05-24 18:29:47.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:29:48.213239 pulumi_aws_iam-0.2.0/pulumi_aws_iam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-24 18:29:48.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-24 18:29:48.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 18:29:48.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 18:29:48.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 18:29:48.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 18:29:48.000000 pulumi_aws_iam-0.2.0/pulumi_aws_iam.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 18:29:48.213239 pulumi_aws_iam-0.2.0/setup.cfg
+-rw-------   0 runner    (1001) docker     (123)     1867 2023-05-24 18:29:47.000000 pulumi_aws_iam-0.2.0/setup.py
```

### Comparing `pulumi_aws_iam-0.1.0/PKG-INFO` & `pulumi_aws_iam-0.2.0/pulumi_aws_iam.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
-Name: pulumi_aws_iam
-Version: 0.1.0
+Name: pulumi-aws-iam
+Version: 0.2.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # AWS IAM
 
 This repo is a [Pulumi Package](https://www.pulumi.com/docs/guides/pulumi-packages/) used to deploy different AWS IAM roles. This
 package is based on the [Terraform AWS IAM Module](https://github.com/terraform-aws-modules/terraform-aws-iam).
```

### Comparing `pulumi_aws_iam-0.1.0/README.md` & `pulumi_aws_iam-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_aws_iam-0.1.0/pulumi_aws_iam/__init__.py` & `pulumi_aws_iam-0.2.0/pulumi_aws_iam/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_aws_iam-0.1.0/pulumi_aws_iam/_inputs.py` & `pulumi_aws_iam-0.2.0/pulumi_aws_iam/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
```

### Comparing `pulumi_aws_iam-0.1.0/pulumi_aws_iam/_utilities.py` & `pulumi_aws_iam-0.2.0/pulumi_aws_iam/_utilities.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,14 +94,25 @@
 _version = _get_semver_version()
 _version_str = str(_version)
 
 
 def get_version():
     return _version_str
 
+def get_resource_opts_defaults() -> pulumi.ResourceOptions:
+    return pulumi.ResourceOptions(
+        version=get_version(),
+        plugin_download_url=get_plugin_download_url(),
+    )
+
+def get_invoke_opts_defaults() -> pulumi.InvokeOptions:
+    return pulumi.InvokeOptions(
+        version=get_version(),
+        plugin_download_url=get_plugin_download_url(),
+    )
 
 def get_resource_args_opts(resource_args_type, resource_options_type, *args, **kwargs):
     """
     Return the resource args and options given the *args and **kwargs of a resource's
     __init__ method.
     """
 
@@ -230,7 +241,10 @@
             'args': args_list,
             'kwargs': bound_args.kwargs
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
+
+def get_plugin_download_url():
+	return None
```

### Comparing `pulumi_aws_iam-0.1.0/pulumi_aws_iam/account.py` & `pulumi_aws_iam-0.2.0/pulumi_aws_iam/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from ._inputs import *
 
@@ -147,20 +148,17 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  account_alias: Optional[pulumi.Input[str]] = None,
                  password_policy: Optional[pulumi.Input[pulumi.InputType['AccountPasswordPolicyArgs']]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AccountArgs.__new__(AccountArgs)
```

### Comparing `pulumi_aws_iam-0.1.0/pulumi_aws_iam/assumable_role.py` & `pulumi_aws_iam-0.2.0/pulumi_aws_iam/assumable_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from ._inputs import *
 
@@ -357,20 +358,17 @@
                  role: Optional[pulumi.Input[pulumi.InputType['RoleWithMFAArgs']]] = None,
                  role_sts_external_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  trusted_role_actions: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  trusted_role_arns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  trusted_role_services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AssumableRoleArgs.__new__(AssumableRoleArgs)
```

### Comparing `pulumi_aws_iam-0.1.0/pulumi_aws_iam/assumable_role_with_oidc.py` & `pulumi_aws_iam-0.2.0/pulumi_aws_iam/assumable_role_with_oidc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from ._inputs import *
 
@@ -277,20 +278,17 @@
                  oidc_fully_qualified_audiences: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  oidc_fully_qualified_subjects: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  oidc_subjects_with_wildcards: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  provider_urls: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  role: Optional[pulumi.Input[pulumi.InputType['RoleArgs']]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AssumableRoleWithOIDCArgs.__new__(AssumableRoleWithOIDCArgs)
```

### Comparing `pulumi_aws_iam-0.1.0/pulumi_aws_iam/assumable_role_with_saml.py` & `pulumi_aws_iam-0.2.0/pulumi_aws_iam/assumable_role_with_saml.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from ._inputs import *
 
@@ -215,20 +216,17 @@
                  aws_saml_endpoint: Optional[pulumi.Input[str]] = None,
                  force_detach_policies: Optional[pulumi.Input[bool]] = None,
                  max_session_duration: Optional[pulumi.Input[int]] = None,
                  provider_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  role: Optional[pulumi.Input[pulumi.InputType['RoleArgs']]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AssumableRoleWithSAMLArgs.__new__(AssumableRoleWithSAMLArgs)
```

### Comparing `pulumi_aws_iam-0.1.0/pulumi_aws_iam/assumable_roles.py` & `pulumi_aws_iam-0.2.0/pulumi_aws_iam/assumable_roles.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from ._inputs import *
 
@@ -244,20 +245,17 @@
                  max_session_duration: Optional[pulumi.Input[int]] = None,
                  mfa_age: Optional[pulumi.Input[int]] = None,
                  poweruser: Optional[pulumi.Input[pulumi.InputType['PoweruserRoleWithMFAArgs']]] = None,
                  readonly: Optional[pulumi.Input[pulumi.InputType['ReadonlyRoleWithMFAArgs']]] = None,
                  trusted_role_arns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  trusted_role_services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AssumableRolesArgs.__new__(AssumableRolesArgs)
```

### Comparing `pulumi_aws_iam-0.1.0/pulumi_aws_iam/assumable_roles_with_saml.py` & `pulumi_aws_iam-0.2.0/pulumi_aws_iam/assumable_roles_with_saml.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from ._inputs import *
 
@@ -220,20 +221,17 @@
                  aws_saml_endpoint: Optional[pulumi.Input[str]] = None,
                  force_detach_policies: Optional[pulumi.Input[bool]] = None,
                  max_session_duration: Optional[pulumi.Input[int]] = None,
                  poweruser: Optional[pulumi.Input[pulumi.InputType['PoweruserRoleArgs']]] = None,
                  provider_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  readonly: Optional[pulumi.Input[pulumi.InputType['ReadonlyRoleArgs']]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AssumableRolesWithSAMLArgs.__new__(AssumableRolesWithSAMLArgs)
```

### Comparing `pulumi_aws_iam-0.1.0/pulumi_aws_iam/eks_role.py` & `pulumi_aws_iam-0.2.0/pulumi_aws_iam/eks_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from ._inputs import *
 
@@ -262,20 +263,17 @@
                  force_detach_policies: Optional[pulumi.Input[bool]] = None,
                  max_session_duration: Optional[pulumi.Input[int]] = None,
                  provider_url_sa_pairs: Optional[pulumi.Input[Mapping[str, pulumi.Input[Sequence[pulumi.Input[str]]]]]] = None,
                  role: Optional[pulumi.Input[pulumi.InputType['RoleArgs']]] = None,
                  role_policy_arns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = EKSRoleArgs.__new__(EKSRoleArgs)
```

### Comparing `pulumi_aws_iam-0.1.0/pulumi_aws_iam/group_with_assumable_roles_policy.py` & `pulumi_aws_iam-0.2.0/pulumi_aws_iam/group_with_assumable_roles_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['GroupWithAssumableRolesPolicyArgs', 'GroupWithAssumableRolesPolicy']
@@ -162,20 +163,17 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  assumable_roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  group_users: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = GroupWithAssumableRolesPolicyArgs.__new__(GroupWithAssumableRolesPolicyArgs)
```

### Comparing `pulumi_aws_iam-0.1.0/pulumi_aws_iam/group_with_policies.py` & `pulumi_aws_iam-0.2.0/pulumi_aws_iam/group_with_policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['GroupWithPoliciesArgs', 'GroupWithPolicies']
@@ -257,20 +258,17 @@
                  custom_group_policies: Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]]] = None,
                  custom_group_policy_arns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  group_users: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  iam_self_management_policy_name_prefix: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = GroupWithPoliciesArgs.__new__(GroupWithPoliciesArgs)
```

### Comparing `pulumi_aws_iam-0.1.0/pulumi_aws_iam/outputs.py` & `pulumi_aws_iam-0.2.0/pulumi_aws_iam/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
```

### Comparing `pulumi_aws_iam-0.1.0/pulumi_aws_iam/policy.py` & `pulumi_aws_iam-0.2.0/pulumi_aws_iam/policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['PolicyArgs', 'Policy']
@@ -206,20 +207,17 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  policy_document: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PolicyArgs.__new__(PolicyArgs)
```

### Comparing `pulumi_aws_iam-0.1.0/pulumi_aws_iam/provider.py` & `pulumi_aws_iam-0.2.0/pulumi_aws_iam/provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['ProviderArgs', 'Provider']
@@ -50,20 +51,17 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
         super(Provider, __self__).__init__(
             'aws-iam',
```

### Comparing `pulumi_aws_iam-0.1.0/pulumi_aws_iam/read_only_policy.py` & `pulumi_aws_iam-0.2.0/pulumi_aws_iam/read_only_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['ReadOnlyPolicyArgs', 'ReadOnlyPolicy']
@@ -294,20 +295,17 @@
                  allowed_services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  web_console_services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ReadOnlyPolicyArgs.__new__(ReadOnlyPolicyArgs)
```

### Comparing `pulumi_aws_iam-0.1.0/pulumi_aws_iam/role_for_service_accounts_eks.py` & `pulumi_aws_iam-0.2.0/pulumi_aws_iam/role_for_service_accounts_eks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from ._inputs import *
 
@@ -304,20 +305,17 @@
                  max_session_duration: Optional[pulumi.Input[int]] = None,
                  oidc_providers: Optional[pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['OIDCProviderArgs']]]]] = None,
                  policies: Optional[pulumi.Input[pulumi.InputType['EKSRolePoliciesArgs']]] = None,
                  policy_name_prefix: Optional[pulumi.Input[str]] = None,
                  role: Optional[pulumi.Input[pulumi.InputType['EKSServiceAccountRoleArgs']]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RoleForServiceAccountsEksArgs.__new__(RoleForServiceAccountsEksArgs)
```

### Comparing `pulumi_aws_iam-0.1.0/pulumi_aws_iam/user.py` & `pulumi_aws_iam-0.2.0/pulumi_aws_iam/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
@@ -304,20 +305,17 @@
                  permissions_boundary: Optional[pulumi.Input[str]] = None,
                  pgp_key: Optional[pulumi.Input[str]] = None,
                  ssh_key_encoding: Optional[pulumi.Input[str]] = None,
                  ssh_public_key: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  upload_iam_user_ssh_key: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = UserArgs.__new__(UserArgs)
```

### Comparing `pulumi_aws_iam-0.1.0/pulumi_aws_iam.egg-info/PKG-INFO` & `pulumi_aws_iam-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
-Name: pulumi-aws-iam
-Version: 0.1.0
+Name: pulumi_aws_iam
+Version: 0.2.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # AWS IAM
 
 This repo is a [Pulumi Package](https://www.pulumi.com/docs/guides/pulumi-packages/) used to deploy different AWS IAM roles. This
 package is based on the [Terraform AWS IAM Module](https://github.com/terraform-aws-modules/terraform-aws-iam).
```

### Comparing `pulumi_aws_iam-0.1.0/pulumi_aws_iam.egg-info/SOURCES.txt` & `pulumi_aws_iam-0.2.0/pulumi_aws_iam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_aws_iam-0.1.0/setup.py` & `pulumi_aws_iam-0.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.1.0"
-PLUGIN_VERSION = "0.1.0"
+VERSION = "0.2.0"
+PLUGIN_VERSION = "0.2.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'aws-iam', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "aws-iam Pulumi Package - Development Version"
 
 
 setup(name='pulumi_aws_iam',
+      python_requires='>=3.7',
       version=VERSION,
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
       packages=find_packages(),
```

