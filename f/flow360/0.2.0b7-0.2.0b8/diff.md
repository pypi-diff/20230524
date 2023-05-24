# Comparing `tmp/flow360-0.2.0b7.tar.gz` & `tmp/flow360-0.2.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow360-0.2.0b7.tar", max compression
+gzip compressed data, was "flow360-0.2.0b8.tar", max compression
```

## Comparing `flow360-0.2.0b7.tar` & `flow360-0.2.0b8.tar`

### file list

```diff
@@ -1,61 +1,62 @@
--rw-r--r--   0        0        0    26526 2023-05-02 13:34:05.158936 flow360-0.2.0b7/LICENSE
--rw-r--r--   0        0        0     1493 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/__init__.py
--rw-r--r--   0        0        0       53 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/cli/__init__.py
--rw-r--r--   0        0        0     2526 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/cli/app.py
--rw-r--r--   0        0        0        0 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/cloud/__init__.py
--rw-r--r--   0        0        0     3029 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/cloud/http_util.py
--rw-r--r--   0        0        0     1191 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/cloud/rest_api.py
--rw-r--r--   0        0        0     9089 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/cloud/s3_utils.py
--rw-r--r--   0        0        0      220 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/cloud/security.py
--rw-r--r--   0        0        0        0 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/__init__.py
--rw-r--r--   0        0        0    26630 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/case.py
--rw-r--r--   0        0        0      142 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/constants.py
--rw-r--r--   0        0        0    26919 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/flow360_params/flow360_params.py
--rw-r--r--   0        0        0    21249 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/flow360_params/params_base.py
--rw-r--r--   0        0        0     8093 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/flow360_params/solvers.py
--rw-r--r--   0        0        0      220 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/meshing/__init__.py
--rw-r--r--   0        0        0     5798 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/meshing/params.py
--rw-r--r--   0        0        0     9561 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/resource_base.py
--rw-r--r--   0        0        0    10086 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/surface_mesh.py
--rw-r--r--   0        0        0     2349 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/types.py
--rw-r--r--   0        0        0     1688 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/utils.py
--rw-r--r--   0        0        0     3255 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/validator.py
--rw-r--r--   0        0        0    22242 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/component/volume_mesh.py
--rw-r--r--   0        0        0     2595 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/environment.py
--rw-r--r--   0        0        0      942 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/error_messages.py
--rw-r--r--   0        0        0      237 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/examples/__init__.py
--rw-r--r--   0        0        0     4024 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/examples/actuatorDisk/flow360.json
--rw-r--r--   0        0        0      447 2023-05-02 13:34:05.162937 flow360-0.2.0b7/flow360/examples/actuator_disk.py
--rw-r--r--   0        0        0    24017 2023-05-02 13:34:05.166937 flow360-0.2.0b7/flow360/examples/airplane/geometry.csm
--rw-r--r--   0        0        0      675 2023-05-02 13:34:05.166937 flow360-0.2.0b7/flow360/examples/airplane/surface_params.json
--rw-r--r--   0        0        0     3702 2023-05-02 13:34:05.166937 flow360-0.2.0b7/flow360/examples/airplane/volume_params.json
--rw-r--r--   0        0        0      292 2023-05-02 13:34:05.166937 flow360-0.2.0b7/flow360/examples/airplane.py
--rw-r--r--   0        0        0     5406 2023-05-02 13:34:05.166937 flow360-0.2.0b7/flow360/examples/base_test_case.py
--rw-r--r--   0        0        0  1157943 2023-05-02 13:34:05.170937 flow360-0.2.0b7/flow360/examples/betDisk/flow360.json
--rw-r--r--   0        0        0  1158028 2023-05-02 13:34:05.174937 flow360-0.2.0b7/flow360/examples/betLine/flow360.json
--rw-r--r--   0        0        0  1158029 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/betLine/release-21.3.3.0ge/flow360.json
--rw-r--r--   0        0        0      432 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/bet_disk.py
--rw-r--r--   0        0        0      432 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/bet_line.py
--rw-r--r--   0        0        0     1430 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/cylinder/flow360.json
--rw-r--r--   0        0        0     1492 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json
--rw-r--r--   0        0        0      373 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/cylinder.py
--rw-r--r--   0        0        0       63 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/om6wing/Flow360Mesh.json
--rw-r--r--   0        0        0     1500 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/om6wing/case.yaml
--rw-r--r--   0        0        0     2509 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/om6wing/flow360.json
--rw-r--r--   0        0        0      427 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/om6wing/release-22.3.3.0ge/case.yaml
--rw-r--r--   0        0        0     2305 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json
--rw-r--r--   0        0        0      391 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/om6wing.py
--rw-r--r--   0        0        0     2744 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/rotatingSpheres/flow360.json
--rw-r--r--   0        0        0      913 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/rotatingSpheres/flow360mesh.json
--rw-r--r--   0        0        0     3379 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json
--rw-r--r--   0        0        0     1177 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json
--rw-r--r--   0        0        0     3376 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json
--rw-r--r--   0        0        0     1177 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json
--rw-r--r--   0        0        0      347 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/examples/rotating_spheres.py
--rw-r--r--   0        0        0     1564 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/exceptions.py
--rw-r--r--   0        0        0     5841 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/log.py
--rw-r--r--   0        0        0     1146 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/solver_version.py
--rw-r--r--   0        0        0     3465 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/user_config.py
--rw-r--r--   0        0        0       38 2023-05-02 13:34:05.178938 flow360-0.2.0b7/flow360/version.py
--rw-r--r--   0        0        0     1465 2023-05-02 13:34:33.006559 flow360-0.2.0b7/pyproject.toml
--rw-r--r--   0        0        0     1507 1970-01-01 00:00:00.000000 flow360-0.2.0b7/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-05-04 12:53:51.957897 flow360-0.2.0b8/LICENSE
+-rw-r--r--   0        0        0     1493 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/__init__.py
+-rw-r--r--   0        0        0       53 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/cli/__init__.py
+-rw-r--r--   0        0        0     2526 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/cli/app.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/cloud/__init__.py
+-rw-r--r--   0        0        0     3029 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/cloud/http_util.py
+-rw-r--r--   0        0        0     1190 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/cloud/rest_api.py
+-rw-r--r--   0        0        0     9089 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/cloud/s3_utils.py
+-rw-r--r--   0        0        0      220 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/cloud/security.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/__init__.py
+-rw-r--r--   0        0        0    27100 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/case.py
+-rw-r--r--   0        0        0      142 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/constants.py
+-rw-r--r--   0        0        0    26987 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/flow360_params/flow360_params.py
+-rw-r--r--   0        0        0    21249 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/flow360_params/params_base.py
+-rw-r--r--   0        0        0     8093 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/flow360_params/solvers.py
+-rw-r--r--   0        0        0      717 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/interfaces.py
+-rw-r--r--   0        0        0      220 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/meshing/__init__.py
+-rw-r--r--   0        0        0     5798 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/meshing/params.py
+-rw-r--r--   0        0        0     9608 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/resource_base.py
+-rw-r--r--   0        0        0     9916 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/surface_mesh.py
+-rw-r--r--   0        0        0     2349 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/types.py
+-rw-r--r--   0        0        0     1686 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/utils.py
+-rw-r--r--   0        0        0     3255 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/validator.py
+-rw-r--r--   0        0        0    22089 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/volume_mesh.py
+-rw-r--r--   0        0        0     2595 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/environment.py
+-rw-r--r--   0        0        0     1128 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/error_messages.py
+-rw-r--r--   0        0        0      237 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/examples/__init__.py
+-rw-r--r--   0        0        0     4024 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/examples/actuatorDisk/flow360.json
+-rw-r--r--   0        0        0      447 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/examples/actuator_disk.py
+-rw-r--r--   0        0        0    24017 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/examples/airplane/geometry.csm
+-rw-r--r--   0        0        0      675 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/examples/airplane/surface_params.json
+-rw-r--r--   0        0        0     3702 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/examples/airplane/volume_params.json
+-rw-r--r--   0        0        0      292 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/examples/airplane.py
+-rw-r--r--   0        0        0     5406 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/examples/base_test_case.py
+-rw-r--r--   0        0        0  1157943 2023-05-04 12:53:51.961897 flow360-0.2.0b8/flow360/examples/betDisk/flow360.json
+-rw-r--r--   0        0        0  1158028 2023-05-04 12:53:51.965897 flow360-0.2.0b8/flow360/examples/betLine/flow360.json
+-rw-r--r--   0        0        0  1158029 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/betLine/release-21.3.3.0ge/flow360.json
+-rw-r--r--   0        0        0      432 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/bet_disk.py
+-rw-r--r--   0        0        0      432 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/bet_line.py
+-rw-r--r--   0        0        0     1430 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/cylinder/flow360.json
+-rw-r--r--   0        0        0     1492 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json
+-rw-r--r--   0        0        0      373 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/cylinder.py
+-rw-r--r--   0        0        0       63 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/om6wing/Flow360Mesh.json
+-rw-r--r--   0        0        0     1500 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/om6wing/case.yaml
+-rw-r--r--   0        0        0     2509 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/om6wing/flow360.json
+-rw-r--r--   0        0        0      427 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/om6wing/release-22.3.3.0ge/case.yaml
+-rw-r--r--   0        0        0     2305 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json
+-rw-r--r--   0        0        0      391 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/om6wing.py
+-rw-r--r--   0        0        0     2744 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/rotatingSpheres/flow360.json
+-rw-r--r--   0        0        0      913 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/rotatingSpheres/flow360mesh.json
+-rw-r--r--   0        0        0     3379 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json
+-rw-r--r--   0        0        0     1177 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json
+-rw-r--r--   0        0        0     3376 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json
+-rw-r--r--   0        0        0     1177 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json
+-rw-r--r--   0        0        0      347 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/rotating_spheres.py
+-rw-r--r--   0        0        0     1564 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/exceptions.py
+-rw-r--r--   0        0        0     5841 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/log.py
+-rw-r--r--   0        0        0     1146 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/solver_version.py
+-rw-r--r--   0        0        0     3465 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/user_config.py
+-rw-r--r--   0        0        0       38 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/version.py
+-rw-r--r--   0        0        0     1465 2023-05-04 12:54:09.209883 flow360-0.2.0b8/pyproject.toml
+-rw-r--r--   0        0        0     1507 1970-01-01 00:00:00.000000 flow360-0.2.0b8/PKG-INFO
```

### Comparing `flow360-0.2.0b7/LICENSE` & `flow360-0.2.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/__init__.py` & `flow360-0.2.0b8/flow360/__init__.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/cli/app.py` & `flow360-0.2.0b8/flow360/cli/app.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/cloud/http_util.py` & `flow360-0.2.0b8/flow360/cloud/http_util.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/cloud/rest_api.py` & `flow360-0.2.0b8/flow360/cloud/rest_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class RestApi:
     """
     RestApi class
     """
 
     # pylint: disable=redefined-builtin
     def __init__(self, endpoint, id=None):
-        is_valid_uuid(id, ignore_none=True)
+        is_valid_uuid(id, allow_none=True)
         self._id = id
         self._endpoint = endpoint
 
     def _url(self, method):
         url = f"{self._endpoint}"
         if self._id is not None:
             url += f"/{self._id}"
```

### Comparing `flow360-0.2.0b7/flow360/cloud/s3_utils.py` & `flow360-0.2.0b8/flow360/cloud/s3_utils.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/component/case.py` & `flow360-0.2.0b8/flow360/component/case.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 from typing import Iterator, List, Union
 
 import pydantic as pd
 from pylab import show, subplots
 
 from .. import error_messages
 from ..cloud.rest_api import RestApi
-from ..cloud.s3_utils import CloudFileNotFoundError, S3TransferType
+from ..cloud.s3_utils import CloudFileNotFoundError
 from ..exceptions import RuntimeError as FlRuntimeError
 from ..exceptions import ValidationError
 from ..exceptions import ValueError as FlValueError
 from ..log import log
 from .flow360_params.flow360_params import Flow360Params, UnvalidatedFlow360Params
+from .interfaces import CaseInterface, VolumeMeshInterface
 from .resource_base import (
     Flow360Resource,
     Flow360ResourceBaseModel,
     Flow360ResourceListBase,
     Flow360Status,
     ResourceDraft,
     before_submit_only,
@@ -32,16 +33,14 @@
 
 
 class CaseBase:
     """
     Case Base component
     """
 
-    _endpoint = "cases"
-
     def copy(
         self,
         name: str = None,
         params: Flow360Params = None,
         solver_version: str = None,
         tags: List[str] = None,
     ) -> CaseDraft:
@@ -265,19 +264,25 @@
                 and self.parent_case.solver_version != self.solver_version
             ):
                 raise FlRuntimeError(
                     error_messages.change_solver_version_error(
                         self.parent_case.solver_version, self.solver_version
                     )
                 )
+            self.solver_version = self.parent_case.solver_version
 
         volume_mesh_id = volume_mesh_id or self.other_case.volume_mesh_id
 
+        if self.solver_version is None:
+            volume_mesh_info = Flow360ResourceBaseModel(
+                **RestApi(VolumeMeshInterface.endpoint, id=volume_mesh_id).get()
+            )
+            self.solver_version = volume_mesh_info.solver_version
+
         is_valid_uuid(volume_mesh_id)
-        is_valid_uuid(parent_id, ignore_none=True)
         self.validator_api(
             self.params,
             volume_mesh_id=volume_mesh_id,
             solver_version=self.solver_version,
             raise_on_error=(not force_submit),
         )
 
@@ -288,15 +293,15 @@
             "tags": self.tags,
             "parentId": parent_id,
         }
 
         if self.solver_version is not None:
             data["solverVersion"] = self.solver_version
 
-        resp = RestApi(self._endpoint).post(
+        resp = RestApi(CaseInterface.endpoint).post(
             json=data,
             path=f"volumemeshes/{volume_mesh_id}/case",
         )
         info = CaseMeta(**resp)
         self._id = info.id
 
         self._submitted_case = Case(self.id)
@@ -315,15 +320,15 @@
 
         if self.parent_id is not None or self.parent_case is not None:
             if self.volume_mesh_id is not None or self.other_case is not None:
                 raise FlValueError(
                     "You cannot specify volume_mesh_id OR other_case when parent case provided."
                 )
 
-        is_valid_uuid(self.volume_mesh_id, ignore_none=True)
+        is_valid_uuid(self.volume_mesh_id, allow_none=True)
 
         if pre_submit_checks:
             is_object_cloud_resource(self.other_case)
             is_object_cloud_resource(self.parent_case)
 
     @classmethod
     def validator_api(
@@ -349,22 +354,21 @@
     """
     Case component
     """
 
     # pylint: disable=redefined-builtin
     def __init__(self, id: str):
         super().__init__(
-            resource_type="Case",
+            interface=CaseInterface,
             info_type_class=CaseMeta,
-            s3_transfer_method=S3TransferType.CASE,
-            endpoint=self._endpoint,
             id=id,
         )
 
         self._params = None
+        self._raw_params = None
         self._results = CaseResults(self)
 
     @classmethod
     def _from_meta(cls, meta: CaseMeta):
         validate_type(meta, "meta", CaseMeta)
         case = cls(id=meta.id)
         case._set_meta(meta)
@@ -372,26 +376,31 @@
 
     @property
     def params(self) -> Flow360Params:
         """
         returns case params
         """
         if self._params is None:
-            raw_params = json.loads(self.get(method="runtimeParams")["content"])
+            self._raw_params = json.loads(self.get(method="runtimeParams")["content"])
             try:
-                self._params = Flow360Params(**raw_params)
+                self._params = Flow360Params(**self._raw_params)
             except pd.ValidationError as err:
-                if self.status is Flow360Status.ERROR:
-                    log.error(f"{err}")
-                    self._params = raw_params
-                else:
-                    raise ValidationError(f"{err}") from err
+                raise ValidationError(error_messages.params_fetching_error(err)) from err
 
         return self._params
 
+    @property
+    def params_as_dict(self) -> dict:
+        """
+        returns case params as dictionary
+        """
+        if self._raw_params is None:
+            self._raw_params = json.loads(self.get(method="runtimeParams")["content"])
+        return self._raw_params
+
     def has_parent(self) -> bool:
         """Check if case has parent case
 
         Returns
         -------
         bool
             True when case has parent, False otherwise
@@ -477,14 +486,18 @@
     def is_finished(self):
         """
         returns False when case is in running or preprocessing state
         """
         return self.status.is_final()
 
     @classmethod
+    def _interface(cls):
+        return CaseInterface
+
+    @classmethod
     def _meta_class(cls):
         """
         returns case meta info class: CaseMeta
         """
         return CaseMeta
 
     @classmethod
```

### Comparing `flow360-0.2.0b7/flow360/component/flow360_params/flow360_params.py` & `flow360-0.2.0b8/flow360/component/flow360_params/flow360_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,15 +270,15 @@
 
     stationary_patches : List[str]
         A list of static patch names of an interface
 
     rotating_patches : List[str]
         A list of dynamic patch names of an interface
 
-    volume_name : str
+    volume_name : Union[str, int, List[str], List[int]]
         A list of dynamic volume zones related to the above {omega, centerOfRotation, axisOfRotation}
 
     name: str, optional
         Name of slidingInterface
 
     parent_volume_name : str, optional
         Name of the volume zone that the rotating reference frame is contained in, used to compute the acceleration in
@@ -324,15 +324,15 @@
         )
     """
 
     center: Coordinate = pd.Field(alias="centerOfRotation")
     axis: Axis = pd.Field(alias="axisOfRotation")
     stationary_patches: List[str] = pd.Field(alias="stationaryPatches")
     rotating_patches: List[str] = pd.Field(alias="rotatingPatches")
-    volume_name: str = pd.Field(alias="volumeName")
+    volume_name: Union[str, int, List[str], List[int]] = pd.Field(alias="volumeName")
     parent_volume_name: Optional[str] = pd.Field(alias="parentVolumeName")
     name: Optional[str] = pd.Field(alias="interfaceName")
     theta_radians: Optional[str] = pd.Field(alias="thetaRadians")
     theta_degrees: Optional[str] = pd.Field(alias="thetaDegrees")
     omega: Optional[Union[float, Omega]] = pd.Field()
     omega_radians: Optional[float] = pd.Field(alias="omegaRadians")
     omega_degrees: Optional[float] = pd.Field(alias="omegaDegrees")
```

### Comparing `flow360-0.2.0b7/flow360/component/flow360_params/params_base.py` & `flow360-0.2.0b8/flow360/component/flow360_params/params_base.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/component/flow360_params/solvers.py` & `flow360-0.2.0b8/flow360/component/flow360_params/solvers.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/component/meshing/params.py` & `flow360-0.2.0b8/flow360/component/meshing/params.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/component/resource_base.py` & `flow360-0.2.0b8/flow360/component/resource_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from functools import wraps
 from typing import List, Optional, Union
 
 import pydantic as pd
 
 from .. import error_messages
 from ..cloud.rest_api import RestApi
+from ..component.interfaces import BaseInterface
 from ..exceptions import RuntimeError as FlRuntimeError
 from ..log import log
 from ..user_config import UserConfig
 from .utils import is_valid_uuid, validate_type
 
 
 class Flow360Status(Enum):
@@ -164,23 +165,21 @@
 
 class Flow360Resource(RestApi):
     """
     Flow360 base resource model
     """
 
     # pylint: disable=redefined-builtin
-    def __init__(
-        self, resource_type, info_type_class, *args, s3_transfer_method=None, id=None, **kwargs
-    ):
-        is_valid_uuid(id, ignore_none=False)
-        self._resource_type = resource_type
-        self.s3_transfer_method = s3_transfer_method
+    def __init__(self, interface: BaseInterface, info_type_class, id=None):
+        is_valid_uuid(id, allow_none=False)
+        self._resource_type = interface.resource_type
+        self.s3_transfer_method = interface.s3_transfer_method
         self.info_type_class = info_type_class
         self._info = None
-        super().__init__(*args, id=id, **kwargs)
+        super().__init__(endpoint=interface.endpoint, id=id)
 
     def __str__(self):
         return self.info.__str__()
 
     def __repr__(self):
         return self.info.__repr__()
 
@@ -324,15 +323,15 @@
         ancestor_id: str = None,
         from_cloud: bool = True,
         include_deleted: bool = False,
         limit: int = 100,
         resourceClass: Flow360Resource = None,
     ):
         if from_cloud:
-            endpoint = resourceClass._endpoint
+            endpoint = resourceClass._interface().endpoint
             if limit is not None and not include_deleted:
                 endpoint += "/page"
 
             RestApi.__init__(self, endpoint=endpoint)
 
             params = {"includeDeleted": include_deleted, "limit": limit, "start": 0}
             if ancestor_id is not None:
```

### Comparing `flow360-0.2.0b7/flow360/component/surface_mesh.py` & `flow360-0.2.0b8/flow360/component/surface_mesh.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 import os
 from enum import Enum
 from typing import Iterator, List, Union
 
 import pydantic as pd
 
 from ..cloud.rest_api import RestApi
-from ..cloud.s3_utils import S3TransferType
 from ..exceptions import FileError as FlFileError
 from ..exceptions import ValueError as FlValueError
 from ..log import log
 from .flow360_params.params_base import params_generic_validator
+from .interfaces import SurfaceMeshInterface
 from .meshing.params import SurfaceMeshingParams, VolumeMeshingParams
 from .resource_base import (
     Flow360Resource,
     Flow360ResourceBaseModel,
     Flow360ResourceListBase,
     ResourceDraft,
 )
@@ -53,22 +53,15 @@
     def to_surface_mesh(self) -> SurfaceMesh:
         """
         returns VolumeMesh object from volume mesh meta info
         """
         return SurfaceMesh(self.id)
 
 
-# pylint: disable=too-few-public-methods
-class SurfaceMeshBase:
-    """SurfaceMeshBase base class"""
-
-    _endpoint = "surfacemeshes"
-
-
-class SurfaceMeshDraft(SurfaceMeshBase, ResourceDraft):
+class SurfaceMeshDraft(ResourceDraft):
     """
     Surface Mesh Draft component
     """
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
@@ -134,15 +127,15 @@
             "config": self.params.to_flow360_json(),
         }
         if self.solver_version:
             data["solverVersion"] = self.solver_version
 
         self.validator_api(self.params, solver_version=self.solver_version)
 
-        resp = RestApi(self._endpoint).post(data)
+        resp = RestApi(SurfaceMeshInterface.endpoint).post(data)
         info = SurfaceMeshMeta(**resp)
         self._id = info.id
         submitted_mesh = SurfaceMesh(self.id)
 
         _, ext = os.path.splitext(self.geometry_file)
         remote_file_name = f"geometry{ext}"
         submitted_mesh.upload_file(
@@ -156,26 +149,24 @@
     def validator_api(cls, params: SurfaceMeshingParams, solver_version=None):
         """
         validation api: validates surface meshing parameters before submitting
         """
         return Validator.SURFACE_MESH.validate(params, solver_version=solver_version)
 
 
-class SurfaceMesh(SurfaceMeshBase, Flow360Resource):
+class SurfaceMesh(Flow360Resource):
     """
     Surface mesh component
     """
 
     # pylint: disable=redefined-builtin
     def __init__(self, id: str):
         super().__init__(
-            resource_type="Surface Mesh",
+            interface=SurfaceMeshInterface,
             info_type_class=SurfaceMeshMeta,
-            s3_transfer_method=S3TransferType.SURFACE_MESH,
-            endpoint=self._endpoint,
             id=id,
         )
         self._params = None
 
     @classmethod
     def _from_meta(cls, meta: SurfaceMeshMeta):
         validate_type(meta, "meta", SurfaceMeshMeta)
@@ -241,14 +232,18 @@
         when file_name is a folder name.
         :return:
         """
 
         self.download_file("logs/flow360_surface_mesh.user.log", to_file, keep_folder)
 
     @classmethod
+    def _interface(cls):
+        return SurfaceMeshInterface
+
+    @classmethod
     def _meta_class(cls):
         """
         returns surface mesh meta info class: SurfaceMeshMeta
         """
         return SurfaceMeshMeta
 
     def _complete_upload(self, remote_file_name):
```

### Comparing `flow360-0.2.0b7/flow360/component/types.py` & `flow360-0.2.0b8/flow360/component/types.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/component/utils.py` & `flow360-0.2.0b8/flow360/component/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 from ..exceptions import TypeError as FlTypeError
 from ..exceptions import ValueError as FlValueError
 from ..log import log
 
 
 # pylint: disable=redefined-builtin
-def is_valid_uuid(id, ignore_none=False):
+def is_valid_uuid(id, allow_none=False):
     """
     Checks if id is valid
     """
-    if id is None and ignore_none:
+    if id is None and allow_none:
         return
     try:
         uuid.UUID(str(id))
     except Exception as exc:
         raise FlValueError(f"{id} is not a valid UUID.") from exc
```

### Comparing `flow360-0.2.0b7/flow360/component/validator.py` & `flow360-0.2.0b8/flow360/component/validator.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/component/volume_mesh.py` & `flow360-0.2.0b8/flow360/component/volume_mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 from enum import Enum
 from typing import Iterator, List, Optional, Union
 
 import numpy as np
 from pydantic import Extra, Field, validator
 
 from ..cloud.rest_api import RestApi
-from ..cloud.s3_utils import S3TransferType
 from ..exceptions import FileError as FlFileError
 from ..exceptions import Flow360NotImplementedError
 from ..exceptions import ValueError as FlValueError
 from ..log import log
 from ..solver_version import Flow360Version
 from .case import Case, CaseDraft
 from .flow360_params.flow360_params import (
     Flow360MeshParams,
     Flow360Params,
     NoSlipWall,
     _GenericBoundaryWrapper,
 )
 from .flow360_params.params_base import params_generic_validator
+from .interfaces import VolumeMeshInterface
 from .meshing.params import VolumeMeshingParams
 from .resource_base import (
     Flow360Resource,
     Flow360ResourceBaseModel,
     Flow360ResourceListBase,
     ResourceDraft,
 )
@@ -337,22 +337,15 @@
     def to_volume_mesh(self) -> VolumeMesh:
         """
         returns VolumeMesh object from volume mesh meta info
         """
         return VolumeMesh(self.id)
 
 
-# pylint: disable=too-few-public-methods
-class VolumeMeshBase:
-    """VolumeMeshBase base class"""
-
-    _endpoint = "volumemeshes"
-
-
-class VolumeMeshDraft(VolumeMeshBase, ResourceDraft):
+class VolumeMeshDraft(ResourceDraft):
     """
     Volume mesh draft component (before submit)
     """
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
@@ -406,15 +399,15 @@
             "config": self.params.to_flow360_json(),
             "format": "cgns",
         }
 
         if self.solver_version:
             body["solverVersion"] = self.solver_version
 
-        resp = RestApi(self._endpoint).post(body)
+        resp = RestApi(VolumeMeshInterface.endpoint).post(body)
         if not resp:
             return None
 
         info = VolumeMeshMeta(**resp)
         self._id = info.id
         mesh = VolumeMesh(self.id)
         log.info(f"VolumeMesh successfully submitted: {mesh.short_description()}")
@@ -440,15 +433,15 @@
         }
         if self.params:
             body["meshParams"] = self.params.to_flow360_json()
 
         if self.solver_version:
             body["solverVersion"] = self.solver_version
 
-        resp = RestApi(self._endpoint).post(body)
+        resp = RestApi(VolumeMeshInterface.endpoint).post(body)
         if not resp:
             return None
 
         info = VolumeMeshMeta(**resp)
         self._id = info.id
         mesh = VolumeMesh(self.id)
         remote_file_name = mesh._remote_file_name(mesh_format, compression, endianness)
@@ -485,26 +478,24 @@
     def validator_api(cls, params: VolumeMeshingParams, solver_version=None):
         """
         validation api: validates surface meshing parameters before submitting
         """
         return Validator.VOLUME_MESH.validate(params, solver_version=solver_version)
 
 
-class VolumeMesh(VolumeMeshBase, Flow360Resource):
+class VolumeMesh(Flow360Resource):
     """
     Volume mesh component
     """
 
     # pylint: disable=redefined-builtin
     def __init__(self, id: str):
         super().__init__(
-            resource_type="Volume Mesh",
+            interface=VolumeMeshInterface,
             info_type_class=VolumeMeshMeta,
-            s3_transfer_method=S3TransferType.VOLUME_MESH,
-            endpoint=self._endpoint,
             id=id,
         )
         self.__mesh_params = None
 
     @classmethod
     def _from_meta(cls, meta: VolumeMeshMeta):
         validate_type(meta, "meta", VolumeMeshMeta)
@@ -602,14 +593,18 @@
         Complete volume mesh upload
         :return:
         """
         resp = self.post({}, method=f"completeUpload?fileName={remote_file_name}")
         self._info = VolumeMeshMeta(**resp)
 
     @classmethod
+    def _interface(cls):
+        return VolumeMeshInterface
+
+    @classmethod
     def _meta_class(cls):
         """
         returns volume mesh meta info class: VolumeMeshMeta
         """
         return VolumeMeshMeta
 
     @classmethod
```

### Comparing `flow360-0.2.0b7/flow360/environment.py` & `flow360-0.2.0b8/flow360/environment.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/error_messages.py` & `flow360-0.2.0b8/flow360/error_messages.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,14 +15,22 @@
 Cannot change solver version from parent to child.
 Parent: solver_version={from_version}
 Requested: solver_version={to_version}
 You need to run sequence of all cases starting from mesh 
 """
 
 
+def params_fetching_error(err_msg):
+    return f"""\
+There was a problem when fetching params for this case
+{err_msg}
+run .params_as_dict to get parameters as a raw dictionary
+    """
+
+
 def submit_reminder(class_name):
     return f"""\
 Remember to submit your {class_name} to cloud to have it processed.
 Please run .submit() after .create()
 To suppress this message run: flow360 configure --suppress-submit-warning"""
```

### Comparing `flow360-0.2.0b7/flow360/examples/actuatorDisk/flow360.json` & `flow360-0.2.0b8/flow360/examples/actuatorDisk/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/examples/airplane/geometry.csm` & `flow360-0.2.0b8/flow360/examples/airplane/geometry.csm`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/examples/airplane/surface_params.json` & `flow360-0.2.0b8/flow360/examples/airplane/surface_params.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/examples/airplane/volume_params.json` & `flow360-0.2.0b8/flow360/examples/airplane/volume_params.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/examples/base_test_case.py` & `flow360-0.2.0b8/flow360/examples/base_test_case.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/examples/betDisk/flow360.json` & `flow360-0.2.0b8/flow360/examples/betDisk/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/examples/betLine/flow360.json` & `flow360-0.2.0b8/flow360/examples/betLine/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/examples/betLine/release-21.3.3.0ge/flow360.json` & `flow360-0.2.0b8/flow360/examples/betLine/release-21.3.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/examples/cylinder/flow360.json` & `flow360-0.2.0b8/flow360/examples/cylinder/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json` & `flow360-0.2.0b8/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/examples/om6wing/case.yaml` & `flow360-0.2.0b8/flow360/examples/om6wing/case.yaml`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/examples/om6wing/flow360.json` & `flow360-0.2.0b8/flow360/examples/om6wing/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json` & `flow360-0.2.0b8/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/examples/rotatingSpheres/flow360.json` & `flow360-0.2.0b8/flow360/examples/rotatingSpheres/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/examples/rotatingSpheres/flow360mesh.json` & `flow360-0.2.0b8/flow360/examples/rotatingSpheres/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json` & `flow360-0.2.0b8/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json` & `flow360-0.2.0b8/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json` & `flow360-0.2.0b8/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json` & `flow360-0.2.0b8/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/exceptions.py` & `flow360-0.2.0b8/flow360/exceptions.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/log.py` & `flow360-0.2.0b8/flow360/log.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/solver_version.py` & `flow360-0.2.0b8/flow360/solver_version.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/flow360/user_config.py` & `flow360-0.2.0b8/flow360/user_config.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b7/pyproject.toml` & `flow360-0.2.0b8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flow360"
-version = "v0.2.0b7"
+version = "v0.2.0b8"
 description = ""
 authors = ["Flexcompute <support@flexcompute.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.7.4"
 pydantic = "^1.9.2"
 pytest = "^7.1.2"
```

### Comparing `flow360-0.2.0b7/PKG-INFO` & `flow360-0.2.0b8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flow360
-Version: 0.2.0b7
+Version: 0.2.0b8
 Summary: 
 Author: Flexcompute
 Author-email: support@flexcompute.com
 Requires-Python: >=3.7.4,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

