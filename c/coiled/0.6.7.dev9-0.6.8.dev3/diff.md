# Comparing `tmp/coiled-0.6.7.dev9.tar.gz` & `tmp/coiled-0.6.8.dev3.tar.gz`

## Comparing `coiled-0.6.7.dev9.tar` & `coiled-0.6.8.dev3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/_version.py
--rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/analytics.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/coiled.yaml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/compatibility.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/context.py
--rw-r--r--   0        0        0   102090 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/exceptions.py
--rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/magic.py
--rw-r--r--   0        0        0    12287 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/scan.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/software.py
--rw-r--r--   0        0        0     5285 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/types.py
--rw-r--r--   0        0        0    49062 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/utils.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/websockets.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/_beta/__init__.py
--rw-r--r--   0        0        0    88106 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/_beta/cluster.py
--rw-r--r--   0        0        0    61035 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/_beta/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/_beta/cwi_log_link.py
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/_beta/states.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/_beta/widgets/__init__.py
--rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/_beta/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/_beta/widgets/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/cli/config.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/cli/core.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/cli/env.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/cli/login.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/cli/utils.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/cli/cluster/utils.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    11588 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    43611 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    26723 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/cli/setup/util.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/coiled/v2/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/README.md
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/pyproject.toml
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 coiled-0.6.7.dev9/PKG-INFO
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/_version.py
+-rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/analytics.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/coiled.yaml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/compatibility.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/context.py
+-rw-r--r--   0        0        0   102090 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/exceptions.py
+-rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/magic.py
+-rw-r--r--   0        0        0    12287 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/scan.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/software.py
+-rw-r--r--   0        0        0     9119 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/types.py
+-rw-r--r--   0        0        0    50564 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/utils.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/websockets.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/_beta/__init__.py
+-rw-r--r--   0        0        0    88451 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/_beta/cluster.py
+-rw-r--r--   0        0        0    57546 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/_beta/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/_beta/cwi_log_link.py
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/_beta/states.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/_beta/widgets/__init__.py
+-rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/_beta/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/_beta/widgets/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/cli/config.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/cli/core.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/cli/env.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/cli/login.py
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/cli/utils.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/cli/cluster/utils.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    12832 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    43611 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    26723 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/coiled/v2/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/README.md
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/pyproject.toml
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 coiled-0.6.8.dev3/PKG-INFO
```

### Comparing `coiled-0.6.7.dev9/coiled/__init__.py` & `coiled-0.6.8.dev3/coiled/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/analytics.py` & `coiled-0.6.8.dev3/coiled/analytics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/cluster.py` & `coiled-0.6.8.dev3/coiled/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/coiled.yaml` & `coiled-0.6.8.dev3/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/context.py` & `coiled-0.6.8.dev3/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/core.py` & `coiled-0.6.8.dev3/coiled/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/exceptions.py` & `coiled-0.6.8.dev3/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/magic.py` & `coiled-0.6.8.dev3/coiled/magic.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/scan.py` & `coiled-0.6.8.dev3/coiled/scan.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/software.py` & `coiled-0.6.8.dev3/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/utils.py` & `coiled-0.6.8.dev3/coiled/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,27 +20,27 @@
 import warnings
 from copy import deepcopy
 from datetime import datetime, timedelta, timezone
 from hashlib import md5
 from logging.config import dictConfig
 from math import ceil
 from pathlib import Path
-from typing import Dict, List, NoReturn, Optional, Tuple, Union
+from typing import Dict, Iterable, List, NoReturn, Optional, Tuple, Union
 from urllib.parse import unquote, urlencode, urlparse
 from zipfile import PyZipFile
 
 import backoff
 from packaging.version import Version
 
 from coiled.context import get_datadog_trace_link, track_context
 
 if sys.version_info >= (3, 8):
-    from typing import Literal, Type, TypedDict, get_args, get_origin, get_type_hints
+    from typing import Literal, Type, TypedDict
 else:
-    from typing_extensions import Literal, Type, TypedDict, get_args, get_origin, get_type_hints
+    from typing_extensions import Literal, Type, TypedDict
 
 import aiohttp
 import boto3
 import click
 import dask
 import rich
 import urllib3
@@ -55,14 +55,15 @@
     CidrInvalidError,
     GPUTypeError,
     InstanceTypeError,
     ParseIdentifierError,
     PortValidationError,
     UnsupportedBackendError,
 )
+from coiled.types import AWSOptions, FirewallOptions, GCPOptions
 
 from .compatibility import COILED_VERSION, PY_VERSION
 from .errors import ServerError
 
 logger = logging.getLogger(__name__)
 
 
@@ -1148,57 +1149,78 @@
         type_list = [type_list]
     # check supported AWS instance types and GCP type with non-guest GPU (A100)
     return any(
         re.search(r"^(((p4|p3|g5|g5g|g4dn|g4ad)\.)|(a2-))", vm_type, flags=re.IGNORECASE) for vm_type in type_list
     )
 
 
-def validate_type(type_, obj_) -> bool:
-    if hasattr(type_, "__forward_arg__"):
-        # evaluate ForwardRef types -- this function breaks if we can't
-        return validate_type(type_.__forward_arg__, obj_)
-    try:
-        if hasattr(type_, "__annotations__"):
-            # check for type TypedDict
-
-            # check that object is a dict
-            if not isinstance(obj_, dict):
-                return False
-
-            # check all the keys
-            for k, v in get_type_hints(type_).items():
-                # get so that undefined key will be None, and check will
-                # pass only if type is Optional
-                if not validate_type(v, obj_.get(k)):
-                    return False
-
-            # make sure no extra keys
-            obj_keys = set(obj_.keys())
-            type_keys = set(get_type_hints(type_).keys())
-            if len(obj_keys - type_keys):
-                return False
-
-            return True
-
-        elif hasattr(type_, "__origin__"):
-            if get_origin(type_) == Union:
-                # check for type Union (including Optional)
-                union_types = get_args(type_)
-                return any((validate_type(subtype, obj_) for subtype in union_types))
-            elif get_origin(type_) == list:
-                # for list, check that each item has correct type
-                subtype = get_args(type_)[0]
-                return all((validate_type(subtype, list_item) for list_item in obj_))
-
-        # check for other types (can check directly)
-        return isinstance(obj_, type_)
+def validate_backend_options(backend_options):
+    # both typing.TypedDict and typing_extensions.TypedDict have __optional_keys__
+    aws_keys = set(AWSOptions.__optional_keys__)  # type: ignore
+    gcp_keys = set(GCPOptions.__optional_keys__)  # type: ignore
+
+    # show warning for unknown keys
+    all_keys = set().union(aws_keys, gcp_keys)
+    for key in backend_options.keys():
+        if key in ("firewall_spec",):
+            # firewall_spec isn't currently in user-schema, but it's how we send the data
+            # to backend endpoint.
+            # `{"ingress": [...]}` (user) —> `{firewall_spec: {"ingress": [...]}` (endpoint)
+            continue
+        if key not in all_keys:
+            logger.warning(f"{key} in backend_options is not a recognized key, it will be ignored")
+        if key in ("firewall", "send_prometheus_metrics", "prometheus_write"):
+            logger.warning(f"{key} in backend_options is deprecated")
+
+    # validate that we don't have aws and gcp-specific keys
+    present_aws_keys = [key for key in backend_options.keys() if key in aws_keys - gcp_keys]
+    present_gcp_keys = [key for key in backend_options.keys() if key in gcp_keys - aws_keys]
+    if present_aws_keys and present_gcp_keys:
+        raise ValueError(
+            f"backend_options cannot have both AWS specific keys ({present_aws_keys}) "
+            f"and GCP specific keys ({present_gcp_keys}"
+        )
 
-    except Exception:
-        # assume that this function works for the types we're checking
-        return False
+    # validate firewall options
+    if backend_options.get("ingress"):
+        if not isinstance(backend_options["ingress"], Iterable):
+            raise ValueError("ingress in backend_options must be an iterable")
+
+        firewall_keys = FirewallOptions.__optional_keys__  # type: ignore
+        for fw in backend_options["ingress"]:
+            for key in fw.keys():
+                if key not in firewall_keys:
+                    logger.warning(f"{key} ({fw[key]}) in backend_options firewall config is not a recognized key")
+
+            for required_key in ("cidr", "ports"):
+                if not fw.get(required_key):
+                    raise ValueError(f"{required_key} is required for each firewall config")
+
+            if not isinstance(fw["cidr"], str):
+                raise ValueError(f"cidr ({fw['cidr']}) must be a string")
+            if not isinstance(fw["ports"], list):
+                raise ValueError(f"ports ({fw['ports']} must be a list")
+
+    # validate optional bool, dict, int, str types
+    all_key_types = {
+        **AWSOptions.__annotations__,
+        **GCPOptions.__annotations__,
+    }
+    keys_by_type = {
+        t: [k for k, key_type in all_key_types.items() if key_type == Optional[t]] for t in (bool, dict, int, str)
+    }
+    for t, schema_keys in keys_by_type.items():
+        for key in backend_options.keys():
+            if key in schema_keys:
+                val = backend_options[key]
+                # all keys as optional, but if specified, they need to match desired type
+                if val is not None and not isinstance(val, t):
+                    raise ValueError(
+                        f"{key} ({val}) in backend_options should be {t.__name__} or None, not {type(val).__name__}"
+                    )
 
 
 def validate_vm_typing(vm_types: Union[List[str], Tuple[str], None]):
     """Validate instance typing.
 
     We need to add this function because the error that our API is returning
     isn't exactly user friendly. We should raise a type error with an informative
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `coiled-0.6.7.dev9/coiled/websockets.py` & `coiled-0.6.8.dev3/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/_beta/cluster.py` & `coiled-0.6.8.dev3/coiled/_beta/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 from coiled._beta.widgets.util import simple_progress
 from coiled.cluster import CoiledAdaptive, CredentialsPreferred
 from coiled.compatibility import DISTRIBUTED_VERSION
 from coiled.context import track_context
 from coiled.core import IsAsynchronous
 from coiled.errors import ClusterCreationError, DoesNotExist
 from coiled.exceptions import ArgumentCombinationError, InstanceTypeError
-from coiled.types import ArchitectureTypesEnum, PackageLevel, PackageLevelEnum
+from coiled.types import ArchitectureTypesEnum, AWSOptions, GCPOptions, PackageLevel, PackageLevelEnum
 from coiled.utils import (
     COILED_LOGGER_NAME,
     GCP_SCHEDULER_GPU,
     any_gpu_instance_type,
     cluster_firewall,
     get_details_url,
     get_grafana_url,
@@ -64,18 +64,16 @@
     parse_identifier,
     parse_wait_for_workers,
     validate_vm_typing,
 )
 
 from ..core import Async, AWSSessionCredentials, Sync
 from .core import (
-    AWSOptions,
     CloudBeta,
     CloudBetaSyncAsync,
-    GCPOptions,
     log_cluster_debug_info,
     setup_logging,
 )
 from .cwi_log_link import cloudwatch_url
 from .states import (
     ClusterStateEnum,
     InstanceStateEnum,
@@ -998,22 +996,30 @@
                 #
                 # (We can't do this check earlier because we don't know until now if we're
                 # creating a cluster, and if we're not then "_start_n_workers" may be the wrong
                 # number of workers...)
                 parse_wait_for_workers(self._start_n_workers, self._wait_for_workers_arg)
 
                 # Determine software environment (legacy or package sync)
-                # TODO: Add GCP support for architecture detection
                 architecture = (
                     ArchitectureTypesEnum.ARM64
                     if (
-                        user_provider == "aws"
-                        and all(
-                            re.search(r"^\w+\d.*g.*", vm_type.split(".")[0], flags=re.IGNORECASE)
-                            for vm_type in chain(scheduler_vm_types_to_use, worker_vm_types_to_use)
+                        (
+                            user_provider == "aws"
+                            and all(
+                                re.search(r"^\w+\d.*g.*", vm_type.split(".")[0], flags=re.IGNORECASE)
+                                for vm_type in chain(scheduler_vm_types_to_use, worker_vm_types_to_use)
+                            )
+                        )
+                        or (
+                            user_provider == "gcp"
+                            and all(
+                                vm_type.split("-")[0].lower() == "t2a"
+                                for vm_type in chain(scheduler_vm_types_to_use, worker_vm_types_to_use)
+                            )
                         )
                     )
                     else ArchitectureTypesEnum.X86_64
                 )
 
                 # `architecture` is set to ARM64 iff *all* instances are ARM,
                 # so when architecture is X86_64 that could mean all instances are x86
```

### Comparing `coiled-0.6.7.dev9/coiled/_beta/core.py` & `coiled-0.6.8.dev3/coiled/_beta/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import asyncio
 import base64
 import datetime
 import json
 import logging
-import sys
 import weakref
 from collections import namedtuple
 from hashlib import md5
 from pathlib import Path
 from typing import (
     Awaitable,
     BinaryIO,
@@ -25,46 +24,41 @@
     cast,
     overload,
 )
 
 import backoff
 import dask
 from aiohttp import ClientResponseError, ClientSession, ContentTypeError
+from dask.utils import parse_timedelta
+from distributed.utils import Log, Logs
 from rich.progress import Progress
+from typing_extensions import TypeAlias
 
 from coiled._beta.widgets.util import simple_progress
+from coiled.cli.setup.entry import do_setup_wizard
+from coiled.context import track_context
+from coiled.core import Async, IsAsynchronous, Sync, delete_docstring, list_docstring
+from coiled.core import Cloud as OldCloud
+from coiled.errors import ClusterCreationError, DoesNotExist, ServerError
 from coiled.types import (
     ApproximatePackageRequest,
     ApproximatePackageResult,
     ArchitectureTypesEnum,
+    AWSOptions,
+    GCPOptions,
+    PackageLevel,
     PackageSchema,
     ResolvedPackageInfo,
     SoftwareEnvironmentAlias,
 )
-
-if sys.version_info >= (3, 8):
-    from typing import TypedDict
-else:
-    from typing_extensions import TypedDict
-
-from dask.utils import parse_timedelta
-from distributed.utils import Log, Logs
-from typing_extensions import TypeAlias
-
-from coiled.cli.setup.entry import do_setup_wizard
-from coiled.context import track_context
-from coiled.core import Async, IsAsynchronous, Sync, delete_docstring, list_docstring
-from coiled.core import Cloud as OldCloud
-from coiled.errors import ClusterCreationError, DoesNotExist, ServerError
-from coiled.types import PackageLevel
 from coiled.utils import (
     COILED_LOGGER_NAME,
     GatewaySecurity,
     get_grafana_url,
-    validate_type,
+    validate_backend_options,
 )
 
 from .states import (
     InstanceStateEnum,
     ProcessStateEnum,
     flatten_log_states,
     get_process_instance_state,
@@ -91,103 +85,14 @@
     if "message" in error_body:
         raise exception_cls(error_body["message"])
     if "detail" in error_body:
         raise exception_cls(error_body["detail"])
     raise exception_cls(error_body)
 
 
-class FirewallOptions(TypedDict):
-    """
-
-    A dictionary with the following key/value pairs
-
-    Parameters
-    ----------
-    ports
-        List of ports to open to cidr on the scheduler.
-        For example, ``[22, 8786]`` opens port 22 for SSH and 8786 for client to Dask connection.
-    cidr
-        CIDR block from which to allow access. For example ``0.0.0.0/0`` allows access from any IP address.
-    """
-
-    ports: List[int]
-    cidr: str
-
-
-class BackendOptions(TypedDict, total=False):
-    """
-
-    A dictionary with the following key/value pairs
-
-    Parameters
-    ----------
-    region_name
-        Region name to launch cluster in. For example: us-east-2
-    zone_name
-        Zone name to launch cluster in. For example: us-east-2a
-    firewall
-        Allows you to specify firewall for scheduler; see :py:class:`FirewallOptions` for details.
-    ingress
-        Allows you to specify multiple CIDR blocks (and corresponding ports) to open for ingress
-        on the scheduler firewall.
-    spot
-        Whether to request spot instances.
-    spot_on_demand_fallback
-        If requesting spot, whether to request non-spot instances if we get fewer spot instances
-        than desired.
-    multizone
-        Tell the cloud provider to pick zone with best availability, we'll keep workers all in the
-        same zone, scheduler may or may not be in that zone as well.
-    use_dashboard_public_ip
-        Public IP is used by default, lets you choose to use private IP for dashboard link.
-    use_dashboard_https
-        When public IP address is used for dashboard, we'll enable HTTPS + auth by default.
-        You may want to disable this if using something that needs to connect directly to
-        the scheduler dashboard without authentication, such as jupyter dask-labextension.
-    """
-
-    region_name: Optional[str]
-    zone_name: Optional[str]
-    firewall: Optional[FirewallOptions]
-    ingress: Optional[List[FirewallOptions]]
-    spot: Optional[bool]
-    spot_on_demand_fallback: Optional[bool]
-    multizone: Optional[bool]
-    use_dashboard_public_ip: Optional[bool]
-    use_dashboard_https: Optional[bool]
-    send_prometheus_metrics: Optional[bool]  # TODO deprecate
-    prometheus_write: Optional[dict]
-    network_volumes: Optional[List[dict]]
-
-
-class AWSOptions(BackendOptions, total=False):
-    """
-
-    A dictionary with the following key/value pairs plus any pairs in :py:class:`BackendOptions`
-
-    Parameters
-    ----------
-    keypair_name
-        AWS Keypair to assign worker/scheduler instances
-    """
-
-    keypair_name: Optional[str]
-    spot_replacement: Optional[bool]
-    use_placement_group: Optional[bool]
-
-
-class GCPOptions(BackendOptions, total=False):
-    scheduler_accelerator_count: Optional[int]
-    scheduler_accelerator_type: Optional[str]
-    worker_accelerator_count: Optional[int]
-    worker_accelerator_type: Optional[str]
-
-
-BackendOptionTypes = [AWSOptions, GCPOptions]
-
 CloudBetaSyncAsync: TypeAlias = Union["CloudBeta[Async]", "CloudBeta[Sync]"]
 
 
 class CloudBeta(OldCloud, Generic[IsAsynchronous]):
     _recent_sync: List[weakref.ReferenceType[CloudBeta[Sync]]] = list()
     _recent_async: List[weakref.ReferenceType[CloudBeta[Async]]] = list()
 
@@ -736,38 +641,36 @@
             "dask_config": dask_config,
             "private_to_creator": private_to_creator,
             "env_id": senv_v2_id,
             "env_name": software_environment,
             # "jupyter_on_scheduler": True,
         }
 
+        backend_options = backend_options if backend_options else {}
+
         if gcp_worker_gpu_type is not None:
             # for backwards compatibility with v1 options
-            backend_options = backend_options if backend_options else {}
             backend_options = {
                 **backend_options,
                 "worker_accelerator_count": gcp_worker_gpu_count or 1,
                 "worker_accelerator_type": gcp_worker_gpu_type,
             }
         elif gcp_worker_gpu_count:
             # not ideal but v1 only supported T4 and `worker_gpu=1` would give you one
-            backend_options = backend_options if backend_options else {}
             backend_options = {
                 **backend_options,
                 "worker_accelerator_count": gcp_worker_gpu_count,
                 "worker_accelerator_type": "nvidia-tesla-t4",
             }
 
         if use_scheduler_public_ip is False:
-            backend_options = backend_options if backend_options else {}
             if "use_dashboard_public_ip" not in backend_options:
                 backend_options["use_dashboard_public_ip"] = False
 
         if use_dashboard_https is False:
-            backend_options = backend_options if backend_options else {}
             if "use_dashboard_https" not in backend_options:
                 backend_options["use_dashboard_https"] = False
 
         if backend_options:
             # for backwards compatibility with v1 options
             if "region" in backend_options and "region_name" not in backend_options:
                 backend_options["region_name"] = backend_options["region"]  # type: ignore
@@ -776,23 +679,20 @@
                 backend_options["zone_name"] = backend_options["zone"]  # type: ignore
                 del backend_options["zone"]  # type: ignore
             # firewall just lets you specify a single CIDR block to open for ingress
             # we want to support a list of ingress CIDR blocks
             if "firewall" in backend_options:
                 backend_options["ingress"] = [backend_options.pop("firewall")]  # type: ignore
 
-            # validate against TypedDicts -- should be better (especially better errors)
-            if not any((validate_type(t, backend_options) for t in BackendOptionTypes)):
-                raise ValueError("backend_options should be an instance of coiled.BackendOptions")
-
             # convert the list of ingress rules to the FirewallSpec expected server-side
             if "ingress" in backend_options:
                 fw_spec = {"ingress": backend_options.pop("ingress")}
                 backend_options["firewall_spec"] = fw_spec  # type: ignore
 
+            validate_backend_options(backend_options)
             data["options"] = backend_options
 
         response = await self._do_request(
             "POST",
             self.server + f"/api/v2/clusters/account/{account}/",
             json=data,
         )
```

### Comparing `coiled-0.6.7.dev9/coiled/_beta/cwi_log_link.py` & `coiled-0.6.8.dev3/coiled/_beta/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/_beta/states.py` & `coiled-0.6.8.dev3/coiled/_beta/states.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/_beta/widgets/__init__.py` & `coiled-0.6.8.dev3/coiled/_beta/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/_beta/widgets/rich.py` & `coiled-0.6.8.dev3/coiled/_beta/widgets/rich.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/_beta/widgets/util.py` & `coiled-0.6.8.dev3/coiled/_beta/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/cli/config.py` & `coiled-0.6.8.dev3/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/cli/core.py` & `coiled-0.6.8.dev3/coiled/cli/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/cli/curl.py` & `coiled-0.6.8.dev3/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/cli/env.py` & `coiled-0.6.8.dev3/coiled/cli/env.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/cli/login.py` & `coiled-0.6.8.dev3/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/cli/package_sync.py` & `coiled-0.6.8.dev3/coiled/cli/package_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         if not will_sync:
             rows.append(
                 (
                     name,
                     "",
                     "cwd",
                     "",
+                    "",
                     str(Path(".") / name) if ispkg else str((Path(".") / name).with_suffix(".py")),
                     "[red]false[/red]",
                 )
             )
     for row in sorted(rows, key=lambda x: (x[5], x[0].lower())):
         table.add_row(*row)
     console = Console()
```

### Comparing `coiled-0.6.7.dev9/coiled/cli/utils.py` & `coiled-0.6.8.dev3/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/cli/cluster/__init__.py` & `coiled-0.6.8.dev3/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/cli/cluster/better_logs.py` & `coiled-0.6.8.dev3/coiled/cli/cluster/better_logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/cli/cluster/logs.py` & `coiled-0.6.8.dev3/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/cli/cluster/ssh.py` & `coiled-0.6.8.dev3/coiled/cli/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/cli/cluster/utils.py` & `coiled-0.6.8.dev3/coiled/cli/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/cli/notebook/__init__.py` & `coiled-0.6.8.dev3/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/cli/notebook/notebook.py` & `coiled-0.6.8.dev3/coiled/cli/notebook/notebook.py`

 * *Files 6% similar despite different names*

```diff
@@ -120,72 +120,109 @@
 @click.command(context_settings=CONTEXT_SETTINGS)
 @click.option(
     "--name",
     default=cwd_cluster_name(),
     help="Cluster name. If not given, defaults to a hash based on current working directory.",
 )
 @click.option(
+    "--account",
+    default=None,
+    help="Coiled account (uses default account if not specified)",
+)
+@click.option(
     "--sync",
     default=False,
     is_flag=True,
     help="Sync the working directory with the filesystem on the notebook. Requires mutagen.",
 )
 @click.option(
     "--software",
     default=None,
     help=(
-        "Software environment name to use. If not given, all the currently-installed "
-        "Python packages are replicated on the VM using package sync."
+        "Software environment name to use. If neither software nor container is specified, "
+        "all the currently-installed Python packages are replicated on the VM using package sync."
+    ),
+)
+@click.option(
+    "--container",
+    default=None,
+    help=(
+        "Container image to use. If neither software nor container is specified, "
+        "all the currently-installed Python packages are replicated on the VM using package sync."
     ),
 )
 @click.option(
     "--vm-type",
     default=[],
     multiple=True,
     help="VM type to use. Specify multiple times to provide multiple options.",
 )
 @click.option(
+    "--gpu",
+    default=False,
+    is_flag=True,
+    help="Use GPU notebook server.",
+)
+@click.option(
     "--open",
     default=True,
     is_flag=True,
     help="Whether to open the notebook in the default browser once it's launched",
 )
-def start_notebook(name: str, sync: bool, software: Optional[str], vm_type: Sequence[str], open: bool):
+def start_notebook(
+    name: str,
+    account: Optional[str],
+    sync: bool,
+    software: Optional[str],
+    container: Optional[str],
+    vm_type: Sequence[str],
+    gpu: bool,
+    open: bool,
+):
     """
     Launch or re-open a notebook session, with optional file syncing.
 
     If a notebook session with the same ``name`` already exists, it's not re-created.
     If file sync was initially not enabled, running ``coiled notebook-beta up --sync``
     will begin file sync without re-launching the notebook.
     """
 
     print(
         "[red]Warning:[/red] [bold]coiled notebook[/bold] "
         "is an experimental feature and is subject to breaking changes."
     )
     print()
 
-    if not (check_distributed_version() and check_jupyter()):
-        return
+    # when using package sync, check that local env has jupyter and recent distributed
+    if not software:
+        if not (check_distributed_version() and check_jupyter()):
+            return
 
     if sync and not (check_mutagen() and check_ssh() and check_ssh_keygen()):
         return
 
-    with coiled.Cloud() as cloud:
+    env = None
+    if container and "rapidsai" in container:
+        env = {"DISABLE_JUPYTER": "true"}  # needed for "stable" RAPIDS image
+
+    with coiled.Cloud(account=account) as cloud:
         print(f"Starting notebook [bold]{name}[/bold]...")
         # TODO how can we get the widget to show up during CLI commands?
         cluster = coiled.Cluster(
             name=name,
             cloud=cloud,
             n_workers=0,
             software=software,
+            container=container,
             jupyter=True,
             scheduler_options={"idle_timeout": "24 hours"},
             scheduler_vm_types=list(vm_type) if vm_type else None,
             allow_ssh=True,
+            environ=env,
+            scheduler_gpu=gpu,
         )
 
         url = cluster.jupyter_link
         cluster_id = cluster.cluster_id
         assert cluster_id is not None
         if sync:
             url = parse_url(url)._replace(path="/jupyter/lab/tree/synced").url
@@ -247,42 +284,52 @@
                         f"docker exec tmp-dask-1 bash -c 'mkdir -p {SYNC_TARGET} && ln -s {SYNC_TARGET} .'",
                     ],
                     check=True,
                 )
 
     print(f"[bold]Jupyter available at {url}[/]")
     print()
-    print(f"To stop this notebook server: [green]coiled notebook down --name {name}[/]")
+
+    stop_command = f"coiled notebook down --name {name}"
+    if account:
+        stop_command = f"{stop_command} --account {account}"
+
+    print(f"To stop this notebook server: [green]{stop_command}[/]")
     if open:
         webbrowser.open(url, new=2)
 
 
 @click.command(context_settings=CONTEXT_SETTINGS)
 @click.option(
     "--name",
     default=cwd_cluster_name(),
     help=("Cluster name. If not given, defaults to a hash based on current working directory."),
 )
-def stop_notebook(name: str):
+@click.option(
+    "--account",
+    default=None,
+    help="Coiled account (uses default account if not specified)",
+)
+def stop_notebook(name: str, account: Optional[str]):
     "Shut down a notebook session."
-    with coiled.Cloud() as cloud:
+    with coiled.Cloud(account=account) as cloud:
         try:
             cluster_id = cloud.get_cluster_by_name(name)
         except DoesNotExist:
-            print(f"[bold red]Cluster {name!r} does not exist[/]")
+            print(f"[bold red]Notebook {name!r} does not exist[/]")
             return  # TODO exit 1
 
         if shutil.which("mutagen") and mutagen_session_exists(cluster_id):
             # NOTE: we can't tell if the user asked for `--sync` or not at creation.
             # Best we can do is check if mutagen is installed and the session exists.
             if not (check_ssh() and check_ssh_keygen()):
                 return
 
             # Stop mutagen
-            print(f"Stopping sync with cluster {name!r} ({cluster_id})")
+            print(f"Stopping sync with notebook {name!r} ({cluster_id})")
             subprocess.run(
                 ["mutagen", "sync", "terminate", MUTAGEN_NAME_FORMAT.format(cluster_id=cluster_id)],
                 check=True,
             )
 
             ssh_info = cloud.get_ssh_key(cluster_id)
             scheduler_address = ssh_info["scheduler_public_address"]
@@ -296,15 +343,15 @@
                     "-f",
                     os.path.expanduser("~/.ssh/known_hosts"),
                     "-R",
                     scheduler_address,
                 ]
             )
 
-        print(f"Stopping cluster {name!r} ({cluster_id})...")
+        print(f"Stopping notebook {name!r} ({cluster_id})...")
         cloud.delete_cluster(cluster_id)
 
 
 @click.command(context_settings=CONTEXT_SETTINGS)
 @click.option(
     "--name",
     default=cwd_cluster_name(),
```

### Comparing `coiled-0.6.7.dev9/coiled/cli/setup/__init__.py` & `coiled-0.6.8.dev3/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/cli/setup/amp.py` & `coiled-0.6.8.dev3/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/cli/setup/aws.py` & `coiled-0.6.8.dev3/coiled/cli/setup/aws.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/cli/setup/entry.py` & `coiled-0.6.8.dev3/coiled/cli/setup/entry.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/cli/setup/gcp.py` & `coiled-0.6.8.dev3/coiled/cli/setup/gcp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/cli/setup/prometheus.py` & `coiled-0.6.8.dev3/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/coiled/v2/__init__.py` & `coiled-0.6.8.dev3/coiled/v2/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from .._beta.cluster import Cluster
-from .._beta.core import AWSOptions, BackendOptions
+from ..types import AWSOptions, GCPOptions, FirewallOptions, BackendOptions
 from .._beta.core import CloudBeta as Cloud
 from .._beta.core import (
-    FirewallOptions,
-    GCPOptions,
     better_cluster_logs,
     cluster_details,
     cluster_logs,
     create_cluster,
     delete_cluster,
     list_clusters,
     log_cluster_debug_info,
```

### Comparing `coiled-0.6.7.dev9/LICENSE` & `coiled-0.6.8.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/README.md` & `coiled-0.6.8.dev3/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/pyproject.toml` & `coiled-0.6.8.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coiled-0.6.7.dev9/PKG-INFO` & `coiled-0.6.8.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.6.7.dev9
+Version: 0.6.8.dev3
 Project-URL: Homepage, https://coiled.io
 Maintainer-email: Coiled <info@coiled.io>
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: aiohttp
 Requires-Dist: backoff
 Requires-Dist: boto3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: coiled Version: 0.6.7.dev9 Project-URL: Homepage,
+Metadata-Version: 2.1 Name: coiled Version: 0.6.8.dev3 Project-URL: Homepage,
 https://coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.7 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
 Requires-Dist: importlib-metadata Requires-Dist: ipywidgets Requires-Dist:
 jmespath Requires-Dist: jsondiff Requires-Dist: pip Requires-Dist: pip>=19.3
 Requires-Dist: prometheus-client Requires-Dist: rich>=11.2.0 Requires-Dist:
```

