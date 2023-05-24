# Comparing `tmp/flow360-0.2.0b8.tar.gz` & `tmp/flow360-0.2.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow360-0.2.0b8.tar", max compression
+gzip compressed data, was "flow360-0.2.0b9.tar", max compression
```

## Comparing `flow360-0.2.0b8.tar` & `flow360-0.2.0b9.tar`

### file list

```diff
@@ -1,62 +1,63 @@
--rw-r--r--   0        0        0    26526 2023-05-04 12:53:51.957897 flow360-0.2.0b8/LICENSE
--rw-r--r--   0        0        0     1493 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/__init__.py
--rw-r--r--   0        0        0       53 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/cli/__init__.py
--rw-r--r--   0        0        0     2526 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/cli/app.py
--rw-r--r--   0        0        0        0 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/cloud/__init__.py
--rw-r--r--   0        0        0     3029 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/cloud/http_util.py
--rw-r--r--   0        0        0     1190 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/cloud/rest_api.py
--rw-r--r--   0        0        0     9089 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/cloud/s3_utils.py
--rw-r--r--   0        0        0      220 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/cloud/security.py
--rw-r--r--   0        0        0        0 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/__init__.py
--rw-r--r--   0        0        0    27100 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/case.py
--rw-r--r--   0        0        0      142 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/constants.py
--rw-r--r--   0        0        0    26987 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/flow360_params/flow360_params.py
--rw-r--r--   0        0        0    21249 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/flow360_params/params_base.py
--rw-r--r--   0        0        0     8093 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/flow360_params/solvers.py
--rw-r--r--   0        0        0      717 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/interfaces.py
--rw-r--r--   0        0        0      220 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/meshing/__init__.py
--rw-r--r--   0        0        0     5798 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/meshing/params.py
--rw-r--r--   0        0        0     9608 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/resource_base.py
--rw-r--r--   0        0        0     9916 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/surface_mesh.py
--rw-r--r--   0        0        0     2349 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/types.py
--rw-r--r--   0        0        0     1686 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/utils.py
--rw-r--r--   0        0        0     3255 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/validator.py
--rw-r--r--   0        0        0    22089 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/component/volume_mesh.py
--rw-r--r--   0        0        0     2595 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/environment.py
--rw-r--r--   0        0        0     1128 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/error_messages.py
--rw-r--r--   0        0        0      237 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/examples/__init__.py
--rw-r--r--   0        0        0     4024 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/examples/actuatorDisk/flow360.json
--rw-r--r--   0        0        0      447 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/examples/actuator_disk.py
--rw-r--r--   0        0        0    24017 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/examples/airplane/geometry.csm
--rw-r--r--   0        0        0      675 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/examples/airplane/surface_params.json
--rw-r--r--   0        0        0     3702 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/examples/airplane/volume_params.json
--rw-r--r--   0        0        0      292 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/examples/airplane.py
--rw-r--r--   0        0        0     5406 2023-05-04 12:53:51.957897 flow360-0.2.0b8/flow360/examples/base_test_case.py
--rw-r--r--   0        0        0  1157943 2023-05-04 12:53:51.961897 flow360-0.2.0b8/flow360/examples/betDisk/flow360.json
--rw-r--r--   0        0        0  1158028 2023-05-04 12:53:51.965897 flow360-0.2.0b8/flow360/examples/betLine/flow360.json
--rw-r--r--   0        0        0  1158029 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/betLine/release-21.3.3.0ge/flow360.json
--rw-r--r--   0        0        0      432 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/bet_disk.py
--rw-r--r--   0        0        0      432 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/bet_line.py
--rw-r--r--   0        0        0     1430 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/cylinder/flow360.json
--rw-r--r--   0        0        0     1492 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json
--rw-r--r--   0        0        0      373 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/cylinder.py
--rw-r--r--   0        0        0       63 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/om6wing/Flow360Mesh.json
--rw-r--r--   0        0        0     1500 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/om6wing/case.yaml
--rw-r--r--   0        0        0     2509 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/om6wing/flow360.json
--rw-r--r--   0        0        0      427 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/om6wing/release-22.3.3.0ge/case.yaml
--rw-r--r--   0        0        0     2305 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json
--rw-r--r--   0        0        0      391 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/om6wing.py
--rw-r--r--   0        0        0     2744 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/rotatingSpheres/flow360.json
--rw-r--r--   0        0        0      913 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/rotatingSpheres/flow360mesh.json
--rw-r--r--   0        0        0     3379 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json
--rw-r--r--   0        0        0     1177 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json
--rw-r--r--   0        0        0     3376 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json
--rw-r--r--   0        0        0     1177 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json
--rw-r--r--   0        0        0      347 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/examples/rotating_spheres.py
--rw-r--r--   0        0        0     1564 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/exceptions.py
--rw-r--r--   0        0        0     5841 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/log.py
--rw-r--r--   0        0        0     1146 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/solver_version.py
--rw-r--r--   0        0        0     3465 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/user_config.py
--rw-r--r--   0        0        0       38 2023-05-04 12:53:51.969897 flow360-0.2.0b8/flow360/version.py
--rw-r--r--   0        0        0     1465 2023-05-04 12:54:09.209883 flow360-0.2.0b8/pyproject.toml
--rw-r--r--   0        0        0     1507 1970-01-01 00:00:00.000000 flow360-0.2.0b8/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-05-24 16:43:10.475267 flow360-0.2.0b9/LICENSE
+-rw-r--r--   0        0        0     1493 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/__init__.py
+-rw-r--r--   0        0        0       53 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/cli/__init__.py
+-rw-r--r--   0        0        0     2526 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/cli/app.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/cloud/__init__.py
+-rw-r--r--   0        0        0     3069 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/cloud/http_util.py
+-rw-r--r--   0        0        0     1379 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/cloud/requests.py
+-rw-r--r--   0        0        0     1190 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/cloud/rest_api.py
+-rw-r--r--   0        0        0     9170 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/cloud/s3_utils.py
+-rw-r--r--   0        0        0      220 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/cloud/security.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/component/__init__.py
+-rw-r--r--   0        0        0    27100 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/component/case.py
+-rw-r--r--   0        0        0      142 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/component/constants.py
+-rw-r--r--   0        0        0    26987 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/component/flow360_params/flow360_params.py
+-rw-r--r--   0        0        0    21249 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/component/flow360_params/params_base.py
+-rw-r--r--   0        0        0     8093 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/component/flow360_params/solvers.py
+-rw-r--r--   0        0        0      717 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/component/interfaces.py
+-rw-r--r--   0        0        0      220 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/component/meshing/__init__.py
+-rw-r--r--   0        0        0     5798 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/component/meshing/params.py
+-rw-r--r--   0        0        0    10090 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/component/resource_base.py
+-rw-r--r--   0        0        0     9916 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/component/surface_mesh.py
+-rw-r--r--   0        0        0     2349 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/component/types.py
+-rw-r--r--   0        0        0     1686 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/component/utils.py
+-rw-r--r--   0        0        0     3255 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/component/validator.py
+-rw-r--r--   0        0        0    22924 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/component/volume_mesh.py
+-rw-r--r--   0        0        0     2595 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/environment.py
+-rw-r--r--   0        0        0     1128 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/error_messages.py
+-rw-r--r--   0        0        0      237 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/examples/__init__.py
+-rw-r--r--   0        0        0     4024 2023-05-24 16:43:10.475267 flow360-0.2.0b9/flow360/examples/actuatorDisk/flow360.json
+-rw-r--r--   0        0        0      447 2023-05-24 16:43:10.479267 flow360-0.2.0b9/flow360/examples/actuator_disk.py
+-rw-r--r--   0        0        0    24017 2023-05-24 16:43:10.479267 flow360-0.2.0b9/flow360/examples/airplane/geometry.csm
+-rw-r--r--   0        0        0      675 2023-05-24 16:43:10.479267 flow360-0.2.0b9/flow360/examples/airplane/surface_params.json
+-rw-r--r--   0        0        0     3702 2023-05-24 16:43:10.479267 flow360-0.2.0b9/flow360/examples/airplane/volume_params.json
+-rw-r--r--   0        0        0      292 2023-05-24 16:43:10.479267 flow360-0.2.0b9/flow360/examples/airplane.py
+-rw-r--r--   0        0        0     5406 2023-05-24 16:43:10.479267 flow360-0.2.0b9/flow360/examples/base_test_case.py
+-rw-r--r--   0        0        0  1157943 2023-05-24 16:43:10.483267 flow360-0.2.0b9/flow360/examples/betDisk/flow360.json
+-rw-r--r--   0        0        0  1158028 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/examples/betLine/flow360.json
+-rw-r--r--   0        0        0  1158029 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/examples/betLine/release-21.3.3.0ge/flow360.json
+-rw-r--r--   0        0        0      432 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/examples/bet_disk.py
+-rw-r--r--   0        0        0      432 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/examples/bet_line.py
+-rw-r--r--   0        0        0     1430 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/examples/cylinder/flow360.json
+-rw-r--r--   0        0        0     1492 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json
+-rw-r--r--   0        0        0      373 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/examples/cylinder.py
+-rw-r--r--   0        0        0       63 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/examples/om6wing/Flow360Mesh.json
+-rw-r--r--   0        0        0     1500 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/examples/om6wing/case.yaml
+-rw-r--r--   0        0        0     2509 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/examples/om6wing/flow360.json
+-rw-r--r--   0        0        0      427 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/examples/om6wing/release-22.3.3.0ge/case.yaml
+-rw-r--r--   0        0        0     2305 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json
+-rw-r--r--   0        0        0      391 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/examples/om6wing.py
+-rw-r--r--   0        0        0     2744 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/examples/rotatingSpheres/flow360.json
+-rw-r--r--   0        0        0      913 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/examples/rotatingSpheres/flow360mesh.json
+-rw-r--r--   0        0        0     3379 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json
+-rw-r--r--   0        0        0     1177 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json
+-rw-r--r--   0        0        0     3376 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json
+-rw-r--r--   0        0        0     1177 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json
+-rw-r--r--   0        0        0      347 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/examples/rotating_spheres.py
+-rw-r--r--   0        0        0     1564 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/exceptions.py
+-rw-r--r--   0        0        0     5841 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/log.py
+-rw-r--r--   0        0        0     1146 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/solver_version.py
+-rw-r--r--   0        0        0     3465 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/user_config.py
+-rw-r--r--   0        0        0       40 2023-05-24 16:43:10.487268 flow360-0.2.0b9/flow360/version.py
+-rw-r--r--   0        0        0     1465 2023-05-24 16:43:26.234030 flow360-0.2.0b9/pyproject.toml
+-rw-r--r--   0        0        0     1507 1970-01-01 00:00:00.000000 flow360-0.2.0b9/PKG-INFO
```

### Comparing `flow360-0.2.0b8/LICENSE` & `flow360-0.2.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/__init__.py` & `flow360-0.2.0b9/flow360/__init__.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/cli/app.py` & `flow360-0.2.0b9/flow360/cli/app.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/cloud/http_util.py` & `flow360-0.2.0b9/flow360/cloud/http_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,16 @@
         """A wrapper function"""
 
         # Extend some capabilities of func
         log.debug(f"call: {func.__name__}({args}, {kwargs})")
 
         resp = func(*args, **kwargs)
 
+        log.debug(f"response: {resp}")
+
         if resp.status_code == 400:
             raise WebError(f"Web {args[1]}: Bad request error: {resp.json()['error']}")
 
         if resp.status_code == 401:
             raise AuthorisationError("Unauthorized.")
 
         if resp.status_code == 404:
```

### Comparing `flow360-0.2.0b8/flow360/cloud/rest_api.py` & `flow360-0.2.0b9/flow360/cloud/rest_api.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/cloud/s3_utils.py` & `flow360-0.2.0b9/flow360/cloud/s3_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,17 @@
     """
     if os.path.isdir(to_file):
         to_file = (
             os.path.join(to_file, path, target_name)
             if keep_folder
             else os.path.join(to_file, os.path.basename(target_name))
         )
-
-    os.makedirs(os.path.dirname(to_file), exist_ok=True)
+    dirname = os.path.dirname(to_file)
+    if dirname:
+        os.makedirs(dirname, exist_ok=True)
     return to_file
 
 
 class _S3Action(Enum):
     """
     Enum for s3 action
     """
@@ -277,14 +278,15 @@
 
                 client.download_file(
                     Bucket=token.get_bucket(),
                     Filename=to_file,
                     Key=token.get_s3_key(),
                     Callback=_call_back,
                 )
+        log.info(f"Saved to {to_file}")
 
     def _get_s3_sts_token(self, resource_id: str, file_name: str) -> _S3STSToken:
         session_key = f"{resource_id}:{self.value}:{file_name}"
         if session_key not in _s3_sts_tokens or _s3_sts_tokens[session_key].is_expired():
             path = self._get_grant_url(resource_id, file_name)
             resp = http.get(path)
             token = _S3STSToken.parse_obj(resp)
```

### Comparing `flow360-0.2.0b8/flow360/component/case.py` & `flow360-0.2.0b9/flow360/component/case.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/component/flow360_params/flow360_params.py` & `flow360-0.2.0b9/flow360/component/flow360_params/flow360_params.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/component/flow360_params/params_base.py` & `flow360-0.2.0b9/flow360/component/flow360_params/params_base.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/component/flow360_params/solvers.py` & `flow360-0.2.0b9/flow360/component/flow360_params/solvers.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/component/interfaces.py` & `flow360-0.2.0b9/flow360/component/interfaces.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/component/meshing/params.py` & `flow360-0.2.0b9/flow360/component/meshing/params.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/component/resource_base.py` & `flow360-0.2.0b9/flow360/component/resource_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Flow360 base Model
 """
+import os
 import traceback
 from abc import ABC
 from datetime import datetime
 from enum import Enum
 from functools import wraps
 from typing import List, Optional, Union
 
@@ -263,28 +264,45 @@
     @on_cloud_resource_only
     def solver_version(self):
         """
         returns solver version of resource
         """
         return self.info.solver_version
 
+    def get_download_file_list(self) -> List:
+        """return list of files available for download
+
+        Returns
+        -------
+        List
+            List of files available for download
+        """
+        return self.get(method="files")
+
     # pylint: disable=too-many-arguments
     @on_cloud_resource_only
     def download_file(
         self,
         file_name,
         to_file=".",
         keep_folder: bool = True,
         overwrite: bool = True,
         progress_callback=None,
         **kwargs,
     ):
         """
         general download functionality
         """
+
+        if to_file != ".":
+            _, file_ext = os.path.splitext(file_name)
+            _, to_file_ext = os.path.splitext(to_file)
+            if to_file_ext != file_ext:
+                to_file = to_file + file_ext
+
         return self.s3_transfer_method.download_file(
             self.id,
             file_name,
             to_file,
             keep_folder,
             overwrite=overwrite,
             progress_callback=progress_callback,
```

### Comparing `flow360-0.2.0b8/flow360/component/surface_mesh.py` & `flow360-0.2.0b9/flow360/component/surface_mesh.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/component/types.py` & `flow360-0.2.0b9/flow360/component/types.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/component/utils.py` & `flow360-0.2.0b9/flow360/component/utils.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/component/validator.py` & `flow360-0.2.0b9/flow360/component/validator.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/component/volume_mesh.py` & `flow360-0.2.0b9/flow360/component/volume_mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 import os.path
 from enum import Enum
 from typing import Iterator, List, Optional, Union
 
 import numpy as np
 from pydantic import Extra, Field, validator
 
+from ..cloud.requests import NewVolumeMeshRequest
 from ..cloud.rest_api import RestApi
+from ..exceptions import CloudFileError
 from ..exceptions import FileError as FlFileError
 from ..exceptions import Flow360NotImplementedError
 from ..exceptions import ValueError as FlValueError
 from ..log import log
 from ..solver_version import Flow360Version
 from .case import Case, CaseDraft
 from .flow360_params.flow360_params import (
@@ -417,38 +419,43 @@
     def _submit_upload_mesh(self, progress_callback=None):
         assert os.path.exists(self.file_name)
 
         compression, file_name_no_compression = CompressionFormat.detect(self.file_name)
         mesh_format = VolumeMeshFileFormat.detect(file_name_no_compression)
         endianness = UGRIDEndianness.detect(file_name_no_compression)
 
+        if mesh_format is VolumeMeshFileFormat.CGNS:
+            remote_file_name = "volumeMesh"
+        else:
+            remote_file_name = "mesh"
+        remote_file_name = (
+            f"{remote_file_name}{endianness.ext()}{mesh_format.ext()}{compression.ext()}"
+        )
+
         name = self.name
         if name is None:
             name = os.path.splitext(os.path.basename(self.file_name))[0]
 
-        body = {
-            "meshName": name,
-            "meshTags": self.tags,
-            "meshFormat": mesh_format.value,
-            "meshEndianness": endianness.value,
-        }
-        if self.params:
-            body["meshParams"] = self.params.to_flow360_json()
-
-        if self.solver_version:
-            body["solverVersion"] = self.solver_version
-
-        resp = RestApi(VolumeMeshInterface.endpoint).post(body)
+        req = NewVolumeMeshRequest(
+            name=name,
+            file_name=remote_file_name,
+            tags=self.tags,
+            format=mesh_format.value,
+            endianness=endianness.value,
+            compression=compression.value,
+            params=self.params,
+            solver_version=self.solver_version,
+        )
+        resp = RestApi(VolumeMeshInterface.endpoint).post(req.dict())
         if not resp:
             return None
 
         info = VolumeMeshMeta(**resp)
         self._id = info.id
         mesh = VolumeMesh(self.id)
-        remote_file_name = mesh._remote_file_name(mesh_format, compression, endianness)
         mesh.upload_file(remote_file_name, self.file_name, progress_callback=progress_callback)
         mesh._complete_upload(remote_file_name)
         log.info(f"VolumeMesh successfully uploaded: {mesh.short_description()}")
         return mesh
 
     def submit(self, progress_callback=None) -> VolumeMesh:
         """submit mesh to cloud
@@ -570,14 +577,21 @@
         status = self.status
         if not status.is_final():
             log.warning(f"Cannot download file because status={status}")
         else:
             remote_file_name = self.info.file_name
             if remote_file_name is None:
                 remote_file_name = self._remote_file_name()
+
+            if to_file != ".":
+                _, file_ext = os.path.splitext(remote_file_name)
+                _, to_file_ext = os.path.splitext(to_file)
+                if to_file_ext != file_ext:
+                    to_file = to_file + self._get_file_extention()
+
             super().download_file(remote_file_name, to_file, keep_folder, overwrite=overwrite)
 
     def download_log(self, log_file: VolumeMeshLog, to_file=".", keep_folder: bool = True):
         """
         Download logs
         :param log_file:
         :param to_file: file name on local disk, could be either folder or file name.
@@ -619,27 +633,38 @@
         """
         Get volume mesh info from cloud
         :param mesh_id:
         :return:
         """
         return cls(mesh_id)
 
-    def _remote_file_name(self, mesh_format=None, compression=None, endianness=None):
+    def _get_file_extention(self):
+        compression = self.info.compression
+        mesh_format = self.info.mesh_format
+        endianness = self.info.endianness
+        return f"{endianness.ext()}{mesh_format.ext()}{compression.ext()}"
+
+    def _remote_file_name(self):
         """
         mesh filename on cloud
         """
-        compression = compression or self.info.compression
-        mesh_format = mesh_format or self.info.mesh_format
-        endianness = endianness or self.info.endianness
 
-        remote_file_name = "mesh"
-        if mesh_format is VolumeMeshFileFormat.CGNS:
-            remote_file_name = self.info.name
+        remote_file_name = None
+        for file in self.get_download_file_list():
+            _, file_name_no_compression = CompressionFormat.detect(file["fileName"])
+            try:
+                VolumeMeshFileFormat.detect(file_name_no_compression)
+                remote_file_name = file["fileName"]
+            except RuntimeError:
+                continue
+
+        if remote_file_name is None:
+            raise CloudFileError(f"No volume mesh file found for id={self.id}")
 
-        return f"{remote_file_name}{endianness.ext()}{mesh_format.ext()}{compression.ext()}"
+        return remote_file_name
 
     @classmethod
     def from_file(
         cls,
         file_name: str,
         params: Union[Flow360MeshParams, None] = None,
         name: str = None,
```

### Comparing `flow360-0.2.0b8/flow360/environment.py` & `flow360-0.2.0b9/flow360/environment.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/error_messages.py` & `flow360-0.2.0b9/flow360/error_messages.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/examples/actuatorDisk/flow360.json` & `flow360-0.2.0b9/flow360/examples/actuatorDisk/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/examples/airplane/geometry.csm` & `flow360-0.2.0b9/flow360/examples/airplane/geometry.csm`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/examples/airplane/surface_params.json` & `flow360-0.2.0b9/flow360/examples/airplane/surface_params.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/examples/airplane/volume_params.json` & `flow360-0.2.0b9/flow360/examples/airplane/volume_params.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/examples/base_test_case.py` & `flow360-0.2.0b9/flow360/examples/base_test_case.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/examples/betDisk/flow360.json` & `flow360-0.2.0b9/flow360/examples/betDisk/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/examples/betLine/flow360.json` & `flow360-0.2.0b9/flow360/examples/betLine/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/examples/betLine/release-21.3.3.0ge/flow360.json` & `flow360-0.2.0b9/flow360/examples/betLine/release-21.3.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/examples/cylinder/flow360.json` & `flow360-0.2.0b9/flow360/examples/cylinder/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json` & `flow360-0.2.0b9/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/examples/om6wing/case.yaml` & `flow360-0.2.0b9/flow360/examples/om6wing/case.yaml`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/examples/om6wing/flow360.json` & `flow360-0.2.0b9/flow360/examples/om6wing/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json` & `flow360-0.2.0b9/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/examples/rotatingSpheres/flow360.json` & `flow360-0.2.0b9/flow360/examples/rotatingSpheres/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/examples/rotatingSpheres/flow360mesh.json` & `flow360-0.2.0b9/flow360/examples/rotatingSpheres/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json` & `flow360-0.2.0b9/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json` & `flow360-0.2.0b9/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json` & `flow360-0.2.0b9/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json` & `flow360-0.2.0b9/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/exceptions.py` & `flow360-0.2.0b9/flow360/exceptions.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/log.py` & `flow360-0.2.0b9/flow360/log.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/solver_version.py` & `flow360-0.2.0b9/flow360/solver_version.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/flow360/user_config.py` & `flow360-0.2.0b9/flow360/user_config.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b8/pyproject.toml` & `flow360-0.2.0b9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flow360"
-version = "v0.2.0b8"
+version = "v0.2.0b9"
 description = ""
 authors = ["Flexcompute <support@flexcompute.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.7.4"
 pydantic = "^1.9.2"
 pytest = "^7.1.2"
```

### Comparing `flow360-0.2.0b8/PKG-INFO` & `flow360-0.2.0b9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flow360
-Version: 0.2.0b8
+Version: 0.2.0b9
 Summary: 
 Author: Flexcompute
 Author-email: support@flexcompute.com
 Requires-Python: >=3.7.4,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

