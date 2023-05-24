# Comparing `tmp/crosslab_api_client-0.2.2.tar.gz` & `tmp/crosslab_api_client-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_api_client-0.2.2.tar", last modified: Wed Apr 19 18:27:18 2023, max compression
+gzip compressed data, was "crosslab_api_client-0.2.3.tar", last modified: Fri May 19 08:14:14 2023, max compression
```

## Comparing `crosslab_api_client-0.2.2.tar` & `crosslab_api_client-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:27:18.488827 crosslab_api_client-0.2.2/
--rw-r--r--   0 dev       (1000) docker-host   (967)      331 2023-04-19 18:27:18.488827 crosslab_api_client-0.2.2/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:06:55.000000 crosslab_api_client-0.2.2/README.md
--rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-02-10 09:58:35.000000 crosslab_api_client-0.2.2/pyproject.toml
--rw-r--r--   0 dev       (1000) docker-host   (967)      624 2023-04-19 18:27:18.488827 crosslab_api_client-0.2.2/setup.cfg
--rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-02-10 09:58:35.000000 crosslab_api_client-0.2.2/setup.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:27:18.485494 crosslab_api_client-0.2.2/src/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:27:18.485494 crosslab_api_client-0.2.2/src/crosslab/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:27:18.485494 crosslab_api_client-0.2.2/src/crosslab/api_client/
--rw-r--r--   0 dev       (1000) docker-host   (967)       58 2023-04-03 16:08:17.000000 crosslab_api_client-0.2.2/src/crosslab/api_client/__init__.py
--rw-r--r--   0 dev       (1000) docker-host   (967)    56595 2023-04-19 18:27:11.000000 crosslab_api_client-0.2.2/src/crosslab/api_client/client.py
--rw-r--r--   0 dev       (1000) docker-host   (967)       50 2023-02-10 09:58:35.000000 crosslab_api_client-0.2.2/src/crosslab/api_client/exceptions.py
--rw-r--r--   0 dev       (1000) docker-host   (967)      804 2023-04-03 16:08:17.000000 crosslab_api_client-0.2.2/src/crosslab/api_client/improved_client.py
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-10 09:58:35.000000 crosslab_api_client-0.2.2/src/crosslab/api_client/py.typed
--rw-r--r--   0 dev       (1000) docker-host   (967)    73241 2023-04-19 18:27:11.000000 crosslab_api_client-0.2.2/src/crosslab/api_client/schemas.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:27:18.485494 crosslab_api_client-0.2.2/src/crosslab_api_client.egg-info/
--rw-r--r--   0 dev       (1000) docker-host   (967)      331 2023-04-19 18:27:18.000000 crosslab_api_client-0.2.2/src/crosslab_api_client.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)      548 2023-04-19 18:27:18.000000 crosslab_api_client-0.2.2/src/crosslab_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-04-19 18:27:18.000000 crosslab_api_client-0.2.2/src/crosslab_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)       42 2023-04-19 18:27:18.000000 crosslab_api_client-0.2.2/src/crosslab_api_client.egg-info/requires.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-04-19 18:27:18.000000 crosslab_api_client-0.2.2/src/crosslab_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:27:18.488827 crosslab_api_client-0.2.2/tests/
--rw-r--r--   0 dev       (1000) docker-host   (967)      722 2023-04-03 16:08:17.000000 crosslab_api_client-0.2.2/tests/test_improved_client.py
--rw-r--r--   0 dev       (1000) docker-host   (967)   463687 2023-04-19 18:27:15.000000 crosslab_api_client-0.2.2/tests/test_openapi.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:14:14.638734 crosslab_api_client-0.2.3/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      331 2023-05-19 08:14:14.638734 crosslab_api_client-0.2.3/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-04-22 15:32:26.000000 crosslab_api_client-0.2.3/README.md
+-rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-02-10 09:58:35.000000 crosslab_api_client-0.2.3/pyproject.toml
+-rw-r--r--   0 dev       (1000) docker-host   (967)      624 2023-05-19 08:14:14.642068 crosslab_api_client-0.2.3/setup.cfg
+-rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-02-10 09:58:35.000000 crosslab_api_client-0.2.3/setup.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:14:14.635401 crosslab_api_client-0.2.3/src/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:14:14.635401 crosslab_api_client-0.2.3/src/crosslab/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:14:14.638734 crosslab_api_client-0.2.3/src/crosslab/api_client/
+-rw-r--r--   0 dev       (1000) docker-host   (967)       58 2023-04-03 16:08:17.000000 crosslab_api_client-0.2.3/src/crosslab/api_client/__init__.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)    58868 2023-05-19 08:14:08.000000 crosslab_api_client-0.2.3/src/crosslab/api_client/client.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)       50 2023-02-10 09:58:35.000000 crosslab_api_client-0.2.3/src/crosslab/api_client/exceptions.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)      804 2023-04-03 16:08:17.000000 crosslab_api_client-0.2.3/src/crosslab/api_client/improved_client.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-10 09:58:35.000000 crosslab_api_client-0.2.3/src/crosslab/api_client/py.typed
+-rw-r--r--   0 dev       (1000) docker-host   (967)    73916 2023-05-19 08:14:08.000000 crosslab_api_client-0.2.3/src/crosslab/api_client/schemas.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:14:14.638734 crosslab_api_client-0.2.3/src/crosslab_api_client.egg-info/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      331 2023-05-19 08:14:14.000000 crosslab_api_client-0.2.3/src/crosslab_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)      548 2023-05-19 08:14:14.000000 crosslab_api_client-0.2.3/src/crosslab_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-05-19 08:14:14.000000 crosslab_api_client-0.2.3/src/crosslab_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)       42 2023-05-19 08:14:14.000000 crosslab_api_client-0.2.3/src/crosslab_api_client.egg-info/requires.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-05-19 08:14:14.000000 crosslab_api_client-0.2.3/src/crosslab_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-05-19 08:14:14.638734 crosslab_api_client-0.2.3/tests/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      722 2023-04-03 16:08:17.000000 crosslab_api_client-0.2.3/tests/test_improved_client.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)   486304 2023-05-19 08:14:11.000000 crosslab_api_client-0.2.3/tests/test_openapi.py
```

### Comparing `crosslab_api_client-0.2.2/setup.cfg` & `crosslab_api_client-0.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_api_client
-version = 0.2.2
+version = 0.2.3
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab API Client
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
 	Operating System :: OS Independent
```

### Comparing `crosslab_api_client-0.2.2/src/crosslab/api_client/client.py` & `crosslab_api_client-0.2.3/src/crosslab/api_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     AddUsersToRoleRequest,
     AddUsersToRoleResponse,
     RemoveUsersFromRoleRequest,
     RemoveUsersFromRoleResponse,
     GetIdentityResponse,
     UpdateIdentityRequest,
     UpdateIdentityResponse,
+    RegisterRequest,
+    RegisterResponse,
     GetScheduleRequest,
     GetScheduleResponse,
     BookExperimentRequest,
     BookExperimentResponse,
     UpdateBookingRequest,
     UpdateBookingResponse,
     CancelBookingResponse,
@@ -61,14 +63,16 @@
     SendSignalingMessageRequest,
     SendSignalingMessageResponse,
     ListPeerconnectionsResponse,
     CreatePeerconnectionRequest,
     CreatePeerconnectionResponse,
     GetPeerconnectionResponse,
     DeletePeerconnectionResponse,
+    PatchPeerconnectionDeviceStatusRequest,
+    PatchPeerconnectionDeviceStatusResponse,
     ListExperimentsResponse,
     CreateExperimentRequest,
     CreateExperimentResponse,
     GetExperimentResponse,
     UpdateExperimentRequest,
     UpdateExperimentResponse,
     DeleteExperimentResponse,
@@ -633,14 +637,37 @@
         status, resp = await self._fetch(valid_url, method="patch", body=body)
            
         # transform response
         if status == 200:
             return resp
         raise Exception(f"Unexpected status code: {status}")
 
+    async def register(self, body: RegisterRequest, url: str = "/register") -> RegisterResponse:  # noqa: E501
+        """
+        Register user
+        
+        This endpoint will register a new user."""  # noqa: E501
+        if not self.BASE_URL:
+            raise Exception("No base url set")
+
+        # match path to url schema
+        m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?()(register)?$', url)
+        if m is None:
+            raise Exception("Invalid url")
+        valid_url = '/'+m.group(2)+'/register'
+        if valid_url.startswith('//'):
+            valid_url = valid_url[1:]
+        # make http call
+        status, resp = await self._fetch(valid_url, method="post", body=body)
+           
+        # transform response
+        if status == 201:
+            return resp
+        raise Exception(f"Unexpected status code: {status}")
+
     async def get_schedule(self, url: str = "/schedule", body: Optional[GetScheduleRequest] = None) -> GetScheduleResponse:  # noqa: E501
         """
         Returns the free / booked times for given experiment.
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
@@ -1156,14 +1183,45 @@
         status, resp = await self._fetch(valid_url, method="delete")
            
         # transform response
         if status == 204:
             return resp
         raise Exception(f"Unexpected status code: {status}")
 
+    async def patch_peerconnection_device_status(self, url: str, body: PatchPeerconnectionDeviceStatusRequest, device_url: str) -> PatchPeerconnectionDeviceStatusResponse:  # noqa: E501
+        """
+        Sets the peerconnection status of a single device.
+        """  # noqa: E501
+        if not self.BASE_URL:
+            raise Exception("No base url set")
+
+        # match path to url schema
+        m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(peerconnections\/[^?]*?)(\/device_status)?$', url)
+        if m is None:
+            raise Exception("Invalid url")
+        valid_url = '/'+m.group(2)+'/device_status'
+        if valid_url.startswith('//'):
+            valid_url = valid_url[1:]
+
+        # build query params
+        query_params: Dict[str, Union[List[str], str]] = {}
+        if device_url:
+            if isinstance(device_url, list):
+                query_params['device_url'] = device_url
+            else:
+                query_params['device_url'] = str(device_url)
+        
+        # make http call
+        status, resp = await self._fetch(valid_url, method="patch", body=body, params=query_params)
+           
+        # transform response
+        if status == 201:
+            return resp
+        raise Exception(f"Unexpected status code: {status}")
+
     async def list_experiments(self, url: str = "/experiments") -> ListExperimentsResponse:  # noqa: E501
         """
         List experiments
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
```

### Comparing `crosslab_api_client-0.2.2/src/crosslab/api_client/improved_client.py` & `crosslab_api_client-0.2.3/src/crosslab/api_client/improved_client.py`

 * *Files identical despite different names*

### Comparing `crosslab_api_client-0.2.2/src/crosslab/api_client/schemas.py` & `crosslab_api_client-0.2.3/src/crosslab/api_client/schemas.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,121 +34,77 @@
 
 CreateDeviceAuthenticationTokenResponse201: TypeAlias = str
 
 
 CreateDeviceAuthenticationTokenResponse: TypeAlias = CreateDeviceAuthenticationTokenResponse201
 
 
-class ListUsersResponse200ItemsRolesItems(TypedDict):
-    """
-    Properties:
-    - url
-    - id
-    - name
-    - scopes
-    """
-    url: NotRequired[str]
-    id: NotRequired[str]
-    name: NotRequired[str]
-    scopes: NotRequired[List[str]]
-
-
 class ListUsersResponse200Items(TypedDict):
     """
     Properties:
     - url
     - id
     - username
     - password
-    - roles
     """
-    url: NotRequired[str]
-    id: NotRequired[str]
-    username: NotRequired[str]
-    password: NotRequired[str]
-    roles: NotRequired[List[ListUsersResponse200ItemsRolesItems]]
+    url: str
+    id: str
+    username: str
+    password: str
 
 
 ListUsersResponse200: TypeAlias = List[ListUsersResponse200Items]
 
 
 ListUsersResponse: TypeAlias = ListUsersResponse200
 
 
 class CreateUserRequest(TypedDict):
     """
     Properties:
+    - url
+    - id
     - username
     - password
     """
+    url: str
+    id: str
     username: str
     password: str
 
 
-class CreateUserResponse201RolesItems(TypedDict):
-    """
-    Properties:
-    - url
-    - id
-    - name
-    - scopes
-    """
-    url: NotRequired[str]
-    id: NotRequired[str]
-    name: NotRequired[str]
-    scopes: NotRequired[List[str]]
-
-
 class CreateUserResponse201(TypedDict):
     """
     Properties:
     - url
     - id
     - username
     - password
-    - roles
     """
-    url: NotRequired[str]
-    id: NotRequired[str]
-    username: NotRequired[str]
-    password: NotRequired[str]
-    roles: NotRequired[List[CreateUserResponse201RolesItems]]
+    url: str
+    id: str
+    username: str
+    password: str
 
 
 CreateUserResponse: TypeAlias = CreateUserResponse201
 
 
-class GetUserResponse200RolesItems(TypedDict):
-    """
-    Properties:
-    - url
-    - id
-    - name
-    - scopes
-    """
-    url: NotRequired[str]
-    id: NotRequired[str]
-    name: NotRequired[str]
-    scopes: NotRequired[List[str]]
-
-
 class GetUserResponse200(TypedDict):
     """
     Properties:
     - url
     - id
     - username
     - password
-    - roles
     """
-    url: NotRequired[str]
-    id: NotRequired[str]
-    username: NotRequired[str]
-    password: NotRequired[str]
-    roles: NotRequired[List[GetUserResponse200RolesItems]]
+    url: str
+    id: str
+    username: str
+    password: str
 
 
 GetUserResponse: TypeAlias = GetUserResponse200
 
 
 class UpdateUserRequest(TypedDict):
     """
@@ -156,42 +112,26 @@
     - username
     - password
     """
     username: NotRequired[str]
     password: NotRequired[str]
 
 
-class UpdateUserResponse200RolesItems(TypedDict):
-    """
-    Properties:
-    - url
-    - id
-    - name
-    - scopes
-    """
-    url: NotRequired[str]
-    id: NotRequired[str]
-    name: NotRequired[str]
-    scopes: NotRequired[List[str]]
-
-
 class UpdateUserResponse200(TypedDict):
     """
     Properties:
     - url
     - id
     - username
     - password
-    - roles
     """
-    url: NotRequired[str]
-    id: NotRequired[str]
-    username: NotRequired[str]
-    password: NotRequired[str]
-    roles: NotRequired[List[UpdateUserResponse200RolesItems]]
+    url: str
+    id: str
+    username: str
+    password: str
 
 
 UpdateUserResponse: TypeAlias = UpdateUserResponse200
 
 
 DeleteUserResponse: TypeAlias = None
 
@@ -200,18 +140,18 @@
     """
     Properties:
     - url
     - id
     - name
     - scopes
     """
-    url: NotRequired[str]
-    id: NotRequired[str]
-    name: NotRequired[str]
-    scopes: NotRequired[List[str]]
+    url: str
+    id: str
+    name: str
+    scopes: List[str]
 
 
 GetRolesOfUserResponse200: TypeAlias = List[GetRolesOfUserResponse200Items]
 
 
 GetRolesOfUserResponse: TypeAlias = GetRolesOfUserResponse200
 
@@ -232,132 +172,120 @@
     """
     Properties:
     - url
     - id
     - name
     - scopes
     """
-    url: NotRequired[str]
-    id: NotRequired[str]
-    name: NotRequired[str]
-    scopes: NotRequired[List[str]]
+    url: str
+    id: str
+    name: str
+    scopes: List[str]
 
 
 ListRolesResponse200: TypeAlias = List[ListRolesResponse200Items]
 
 
 ListRolesResponse: TypeAlias = ListRolesResponse200
 
 
 class CreateRoleRequest(TypedDict):
     """
     Properties:
+    - url
+    - id
     - name
     - scopes
     """
+    url: str
+    id: str
     name: str
     scopes: List[str]
 
 
 class CreateRoleResponse201(TypedDict):
     """
     Properties:
     - url
     - id
     - name
     - scopes
     """
-    url: NotRequired[str]
-    id: NotRequired[str]
-    name: NotRequired[str]
-    scopes: NotRequired[List[str]]
+    url: str
+    id: str
+    name: str
+    scopes: List[str]
 
 
 CreateRoleResponse: TypeAlias = CreateRoleResponse201
 
 
 class GetRoleResponse200(TypedDict):
     """
     Properties:
     - url
     - id
     - name
     - scopes
     """
-    url: NotRequired[str]
-    id: NotRequired[str]
-    name: NotRequired[str]
-    scopes: NotRequired[List[str]]
+    url: str
+    id: str
+    name: str
+    scopes: List[str]
 
 
 GetRoleResponse: TypeAlias = GetRoleResponse200
 
 
 class UpdateRoleRequest(TypedDict):
     """
     Properties:
     - url
     - id
     - name
     - scopes
     """
-    url: NotRequired[str]
-    id: NotRequired[str]
-    name: NotRequired[str]
-    scopes: NotRequired[List[str]]
+    url: str
+    id: str
+    name: str
+    scopes: List[str]
 
 
 class UpdateRoleResponse200(TypedDict):
     """
     Properties:
     - url
     - id
     - name
     - scopes
     """
-    url: NotRequired[str]
-    id: NotRequired[str]
-    name: NotRequired[str]
-    scopes: NotRequired[List[str]]
+    url: str
+    id: str
+    name: str
+    scopes: List[str]
 
 
 UpdateRoleResponse: TypeAlias = UpdateRoleResponse200
 
 
 DeleteRoleResponse: TypeAlias = None
 
 
-class GetUsersWithRoleResponse200ItemsRolesItems(TypedDict):
-    """
-    Properties:
-    - url
-    - id
-    - name
-    - scopes
-    """
-    url: NotRequired[str]
-    id: NotRequired[str]
-    name: NotRequired[str]
-    scopes: NotRequired[List[str]]
-
-
 class GetUsersWithRoleResponse200Items(TypedDict):
     """
     Properties:
     - url
     - id
     - username
     - password
-    - roles
     """
-    url: NotRequired[str]
-    id: NotRequired[str]
-    username: NotRequired[str]
-    password: NotRequired[str]
-    roles: NotRequired[List[GetUsersWithRoleResponse200ItemsRolesItems]]
+    url: str
+    id: str
+    username: str
+    password: str
 
 
 GetUsersWithRoleResponse200: TypeAlias = List[GetUsersWithRoleResponse200Items]
 
 
 GetUsersWithRoleResponse: TypeAlias = GetUsersWithRoleResponse200
 
@@ -370,108 +298,69 @@
 
 RemoveUsersFromRoleRequest: TypeAlias = List[str]
 
 
 RemoveUsersFromRoleResponse: TypeAlias = None
 
 
-class GetIdentityResponse200RolesItems(TypedDict):
-    """
-    Properties:
-    - url
-    - id
-    - name
-    - scopes
-    """
-    url: NotRequired[str]
-    id: NotRequired[str]
-    name: NotRequired[str]
-    scopes: NotRequired[List[str]]
-
-
 class GetIdentityResponse200(TypedDict):
     """
     Properties:
     - url
     - id
     - username
     - password
-    - roles
     """
-    url: NotRequired[str]
-    id: NotRequired[str]
-    username: NotRequired[str]
-    password: NotRequired[str]
-    roles: NotRequired[List[GetIdentityResponse200RolesItems]]
+    url: str
+    id: str
+    username: str
+    password: str
 
 
 GetIdentityResponse: TypeAlias = GetIdentityResponse200
 
 
-class UpdateIdentityRequestRolesItems(TypedDict):
-    """
-    Properties:
-    - url
-    - id
-    - name
-    - scopes
-    """
-    url: NotRequired[str]
-    id: NotRequired[str]
-    name: NotRequired[str]
-    scopes: NotRequired[List[str]]
-
-
 class UpdateIdentityRequest(TypedDict):
     """
     Properties:
-    - url
-    - id
     - username
     - password
-    - roles
     """
-    url: NotRequired[str]
-    id: NotRequired[str]
     username: NotRequired[str]
     password: NotRequired[str]
-    roles: NotRequired[List[UpdateIdentityRequestRolesItems]]
 
 
-class UpdateIdentityResponse200RolesItems(TypedDict):
+class UpdateIdentityResponse200(TypedDict):
     """
     Properties:
     - url
     - id
-    - name
-    - scopes
+    - username
+    - password
     """
-    url: NotRequired[str]
-    id: NotRequired[str]
-    name: NotRequired[str]
-    scopes: NotRequired[List[str]]
+    url: str
+    id: str
+    username: str
+    password: str
 
 
-class UpdateIdentityResponse200(TypedDict):
+UpdateIdentityResponse: TypeAlias = UpdateIdentityResponse200
+
+
+class RegisterRequest(TypedDict):
     """
     Properties:
-    - url
-    - id
-    - username
-    - password
-    - roles
+    - username: Username of the user.
+    - password: Password of the user.
     """
-    url: NotRequired[str]
-    id: NotRequired[str]
-    username: NotRequired[str]
-    password: NotRequired[str]
-    roles: NotRequired[List[UpdateIdentityResponse200RolesItems]]
+    username: str
+    password: str
 
 
-UpdateIdentityResponse: TypeAlias = UpdateIdentityResponse200
+RegisterResponse: TypeAlias = None
 
 
 class GetScheduleRequestExperimentDevicesItems(TypedDict):
     """
     A device might either be a physical/virtual device or a group of device.Properties:
     - ID: Unique ID of the device. Contains the institution (by having an end point at that institution)
     """
@@ -797,555 +686,701 @@
     Properties:
     - url: URL of the device
     - name: Name of the device
     - description: Extended description of the device, features, etc.
     - type: Type of the device
     - owner
     """
-    url: NotRequired[str]
-    name: NotRequired[str]
+    url: str
+    name: str
     description: NotRequired[str]
-    type: NotRequired[Literal["device", "group", "edge instantiable", "cloud instantiable"]]
-    owner: NotRequired[str]
+    type: Literal["device", "group", "edge instantiable", "cloud instantiable"]
+    owner: str
 
 
 ListDevicesResponse200: TypeAlias = List[ListDevicesResponse200Items]
 
 
 ListDevicesResponse: TypeAlias = ListDevicesResponse200
 
 
-class CreateDeviceRequestAlt1AnnouncedavailabilityItems(TypedDict):
+class CreateDeviceRequestAlt1ServicesItems(TypedDict):
+    """
+    Properties:
+    - serviceType
+    - serviceId
+    - serviceDirection
+    """
+    serviceType: NotRequired[str]
+    serviceId: NotRequired[str]
+    serviceDirection: NotRequired[Literal["consumer", "producer", "prosumer"]]
+
+
+class CreateDeviceRequestAlt1(TypedDict):
     """
     Properties:
+    - url: URL of the device
+    - name: Name of the device
+    - description: Extended description of the device, features, etc.
+    - type: Type of the device
+    - owner
+    - instantiateUrl
+    - services
     """
+    url: str
+    name: str
+    description: NotRequired[str]
+    type: Literal["cloud instantiable"]
+    owner: str
+    instantiateUrl: NotRequired[str]
+    services: NotRequired[List[CreateDeviceRequestAlt1ServicesItems]]
 
 
-class CreateDeviceRequestAlt1ServicesItems(TypedDict):
+class CreateDeviceRequestAlt2AnnouncedavailabilityItems(TypedDict):
     """
     Properties:
+    - start
+    - end
     """
+    start: NotRequired[str]
+    end: NotRequired[str]
 
 
-class CreateDeviceRequestAlt1(TypedDict):
+class CreateDeviceRequestAlt2ServicesItems(TypedDict):
+    """
+    Properties:
+    - serviceType
+    - serviceId
+    - serviceDirection
+    """
+    serviceType: NotRequired[str]
+    serviceId: NotRequired[str]
+    serviceDirection: NotRequired[Literal["consumer", "producer", "prosumer"]]
+
+
+class CreateDeviceRequestAlt2(TypedDict):
     """
     Properties:
     - url: URL of the device
     - name: Name of the device
     - description: Extended description of the device, features, etc.
     - type: Type of the device
     - owner
     - connected: If true, the device is connected to the service and can be used.
 
     - announcedAvailability: A list of time slots that the maintainer of the device announced it is available
 
     - experiment
     - services
     """
-    url: NotRequired[str]
-    name: NotRequired[str]
+    url: str
+    name: str
     description: NotRequired[str]
-    type: NotRequired[Literal["device"]]
-    owner: NotRequired[str]
+    type: Literal["device"]
+    owner: str
     connected: NotRequired[bool]
-    announcedAvailability: NotRequired[List[CreateDeviceRequestAlt1AnnouncedavailabilityItems]]
+    announcedAvailability: NotRequired[List[CreateDeviceRequestAlt2AnnouncedavailabilityItems]]
     experiment: NotRequired[str]
-    services: NotRequired[List[CreateDeviceRequestAlt1ServicesItems]]
+    services: NotRequired[List[CreateDeviceRequestAlt2ServicesItems]]
 
 
-class CreateDeviceRequestAlt2DevicesItems(TypedDict):
+class CreateDeviceRequestAlt3ServicesItems(TypedDict):
     """
     Properties:
-    - url: URL of the device
+    - serviceType
+    - serviceId
+    - serviceDirection
     """
-    url: NotRequired[str]
+    serviceType: NotRequired[str]
+    serviceId: NotRequired[str]
+    serviceDirection: NotRequired[Literal["consumer", "producer", "prosumer"]]
 
 
-class CreateDeviceRequestAlt2(TypedDict):
+class CreateDeviceRequestAlt3(TypedDict):
     """
     Properties:
     - url: URL of the device
     - name: Name of the device
     - description: Extended description of the device, features, etc.
     - type: Type of the device
     - owner
-    - devices
+    - codeUrl
+    - services
     """
-    url: NotRequired[str]
-    name: NotRequired[str]
+    url: str
+    name: str
     description: NotRequired[str]
-    type: NotRequired[Literal["group"]]
-    owner: NotRequired[str]
-    devices: NotRequired[List[CreateDeviceRequestAlt2DevicesItems]]
+    type: Literal["edge instantiable"]
+    owner: str
+    codeUrl: NotRequired[str]
+    services: NotRequired[List[CreateDeviceRequestAlt3ServicesItems]]
 
 
-class CreateDeviceRequestAlt3(TypedDict):
+class CreateDeviceRequestAlt4DevicesItems(TypedDict):
+    """
+    Properties:
+    - url: URL of the device
+    """
+    url: str
+
+
+class CreateDeviceRequestAlt4(TypedDict):
     """
     Properties:
     - url: URL of the device
     - name: Name of the device
     - description: Extended description of the device, features, etc.
     - type: Type of the device
     - owner
-    - instantiate_url
+    - devices
     """
-    url: NotRequired[str]
-    name: NotRequired[str]
+    url: str
+    name: str
     description: NotRequired[str]
-    type: NotRequired[Literal["cloud instantiable"]]
-    owner: NotRequired[str]
-    instantiate_url: NotRequired[str]
+    type: Literal["group"]
+    owner: str
+    devices: List[CreateDeviceRequestAlt4DevicesItems]
 
 
-class CreateDeviceRequestAlt4(TypedDict):
+CreateDeviceRequest = Union[CreateDeviceRequestAlt1, CreateDeviceRequestAlt2, CreateDeviceRequestAlt3, CreateDeviceRequestAlt4]
+
+
+class CreateDeviceResponse201Alt1ServicesItems(TypedDict):
+    """
+    Properties:
+    - serviceType
+    - serviceId
+    - serviceDirection
+    """
+    serviceType: NotRequired[str]
+    serviceId: NotRequired[str]
+    serviceDirection: NotRequired[Literal["consumer", "producer", "prosumer"]]
+
+
+class CreateDeviceResponse201Alt1(TypedDict):
     """
     Properties:
     - url: URL of the device
     - name: Name of the device
     - description: Extended description of the device, features, etc.
     - type: Type of the device
     - owner
-    - code_url
+    - instantiateUrl
+    - services
     """
-    url: NotRequired[str]
-    name: NotRequired[str]
+    url: str
+    name: str
     description: NotRequired[str]
-    type: NotRequired[Literal["edge instantiable"]]
-    owner: NotRequired[str]
-    code_url: NotRequired[str]
-
-
-CreateDeviceRequest = Union[CreateDeviceRequestAlt1, CreateDeviceRequestAlt2, CreateDeviceRequestAlt3, CreateDeviceRequestAlt4]
+    type: Literal["cloud instantiable"]
+    owner: str
+    instantiateUrl: NotRequired[str]
+    services: NotRequired[List[CreateDeviceResponse201Alt1ServicesItems]]
 
 
-class CreateDeviceResponse201Alt1AnnouncedavailabilityItems(TypedDict):
+class CreateDeviceResponse201Alt2AnnouncedavailabilityItems(TypedDict):
     """
     Properties:
     - start
     - end
     """
     start: NotRequired[str]
     end: NotRequired[str]
 
 
-class CreateDeviceResponse201Alt1ServicesItems(TypedDict):
+class CreateDeviceResponse201Alt2ServicesItems(TypedDict):
     """
     Properties:
+    - serviceType
+    - serviceId
+    - serviceDirection
     """
+    serviceType: NotRequired[str]
+    serviceId: NotRequired[str]
+    serviceDirection: NotRequired[Literal["consumer", "producer", "prosumer"]]
 
 
-class CreateDeviceResponse201Alt1(TypedDict):
+class CreateDeviceResponse201Alt2(TypedDict):
     """
     Properties:
     - url: URL of the device
     - name: Name of the device
     - description: Extended description of the device, features, etc.
     - type: Type of the device
     - owner
     - connected: If true, the device is connected to the service and can be used.
 
     - announcedAvailability: A list of time slots that the maintainer of the device announced it is available
 
     - experiment
     - services
     """
-    url: NotRequired[str]
-    name: NotRequired[str]
+    url: str
+    name: str
     description: NotRequired[str]
-    type: NotRequired[Literal["device"]]
-    owner: NotRequired[str]
+    type: Literal["device"]
+    owner: str
     connected: NotRequired[bool]
-    announcedAvailability: NotRequired[List[CreateDeviceResponse201Alt1AnnouncedavailabilityItems]]
+    announcedAvailability: NotRequired[List[CreateDeviceResponse201Alt2AnnouncedavailabilityItems]]
     experiment: NotRequired[str]
-    services: NotRequired[List[CreateDeviceResponse201Alt1ServicesItems]]
+    services: NotRequired[List[CreateDeviceResponse201Alt2ServicesItems]]
 
 
-class CreateDeviceResponse201Alt2DevicesItems(TypedDict):
+class CreateDeviceResponse201Alt3ServicesItems(TypedDict):
     """
     Properties:
-    - url: URL of the device
+    - serviceType
+    - serviceId
+    - serviceDirection
     """
-    url: NotRequired[str]
+    serviceType: NotRequired[str]
+    serviceId: NotRequired[str]
+    serviceDirection: NotRequired[Literal["consumer", "producer", "prosumer"]]
 
 
-class CreateDeviceResponse201Alt2(TypedDict):
+class CreateDeviceResponse201Alt3(TypedDict):
     """
     Properties:
     - url: URL of the device
     - name: Name of the device
     - description: Extended description of the device, features, etc.
     - type: Type of the device
     - owner
-    - devices
+    - codeUrl
+    - services
     """
-    url: NotRequired[str]
-    name: NotRequired[str]
+    url: str
+    name: str
     description: NotRequired[str]
-    type: NotRequired[Literal["group"]]
-    owner: NotRequired[str]
-    devices: NotRequired[List[CreateDeviceResponse201Alt2DevicesItems]]
+    type: Literal["edge instantiable"]
+    owner: str
+    codeUrl: NotRequired[str]
+    services: NotRequired[List[CreateDeviceResponse201Alt3ServicesItems]]
 
 
-class CreateDeviceResponse201Alt3(TypedDict):
+class CreateDeviceResponse201Alt4DevicesItems(TypedDict):
     """
     Properties:
     - url: URL of the device
-    - name: Name of the device
-    - description: Extended description of the device, features, etc.
-    - type: Type of the device
-    - owner
-    - instantiate_url
     """
-    url: NotRequired[str]
-    name: NotRequired[str]
-    description: NotRequired[str]
-    type: NotRequired[Literal["cloud instantiable"]]
-    owner: NotRequired[str]
-    instantiate_url: NotRequired[str]
+    url: str
 
 
 class CreateDeviceResponse201Alt4(TypedDict):
     """
     Properties:
     - url: URL of the device
     - name: Name of the device
     - description: Extended description of the device, features, etc.
     - type: Type of the device
     - owner
-    - code_url
+    - devices
     """
-    url: NotRequired[str]
-    name: NotRequired[str]
+    url: str
+    name: str
     description: NotRequired[str]
-    type: NotRequired[Literal["edge instantiable"]]
-    owner: NotRequired[str]
-    code_url: NotRequired[str]
+    type: Literal["group"]
+    owner: str
+    devices: List[CreateDeviceResponse201Alt4DevicesItems]
 
 
 CreateDeviceResponse201 = Union[CreateDeviceResponse201Alt1, CreateDeviceResponse201Alt2, CreateDeviceResponse201Alt3, CreateDeviceResponse201Alt4]
 
 
 CreateDeviceResponse: TypeAlias = CreateDeviceResponse201
 
 
-class GetDeviceResponse200Alt1AnnouncedavailabilityItems(TypedDict):
+class GetDeviceResponse200Alt1ServicesItems(TypedDict):
+    """
+    Properties:
+    - serviceType
+    - serviceId
+    - serviceDirection
+    """
+    serviceType: NotRequired[str]
+    serviceId: NotRequired[str]
+    serviceDirection: NotRequired[Literal["consumer", "producer", "prosumer"]]
+
+
+class GetDeviceResponse200Alt1(TypedDict):
+    """
+    Properties:
+    - url: URL of the device
+    - name: Name of the device
+    - description: Extended description of the device, features, etc.
+    - type: Type of the device
+    - owner
+    - instantiateUrl
+    - services
+    """
+    url: str
+    name: str
+    description: NotRequired[str]
+    type: Literal["cloud instantiable"]
+    owner: str
+    instantiateUrl: NotRequired[str]
+    services: NotRequired[List[GetDeviceResponse200Alt1ServicesItems]]
+
+
+class GetDeviceResponse200Alt2AnnouncedavailabilityItems(TypedDict):
     """
     Properties:
     - start
     - end
     """
     start: NotRequired[str]
     end: NotRequired[str]
 
 
-class GetDeviceResponse200Alt1ServicesItems(TypedDict):
+class GetDeviceResponse200Alt2ServicesItems(TypedDict):
     """
     Properties:
+    - serviceType
+    - serviceId
+    - serviceDirection
     """
+    serviceType: NotRequired[str]
+    serviceId: NotRequired[str]
+    serviceDirection: NotRequired[Literal["consumer", "producer", "prosumer"]]
 
 
-class GetDeviceResponse200Alt1(TypedDict):
+class GetDeviceResponse200Alt2(TypedDict):
     """
     Properties:
     - url: URL of the device
     - name: Name of the device
     - description: Extended description of the device, features, etc.
     - type: Type of the device
     - owner
     - connected: If true, the device is connected to the service and can be used.
 
     - announcedAvailability: A list of time slots that the maintainer of the device announced it is available
 
     - experiment
     - services
     """
-    url: NotRequired[str]
-    name: NotRequired[str]
+    url: str
+    name: str
     description: NotRequired[str]
-    type: NotRequired[Literal["device"]]
-    owner: NotRequired[str]
+    type: Literal["device"]
+    owner: str
     connected: NotRequired[bool]
-    announcedAvailability: NotRequired[List[GetDeviceResponse200Alt1AnnouncedavailabilityItems]]
+    announcedAvailability: NotRequired[List[GetDeviceResponse200Alt2AnnouncedavailabilityItems]]
     experiment: NotRequired[str]
-    services: NotRequired[List[GetDeviceResponse200Alt1ServicesItems]]
+    services: NotRequired[List[GetDeviceResponse200Alt2ServicesItems]]
 
 
-class GetDeviceResponse200Alt2DevicesItems(TypedDict):
+class GetDeviceResponse200Alt3ServicesItems(TypedDict):
     """
     Properties:
-    - url: URL of the device
+    - serviceType
+    - serviceId
+    - serviceDirection
     """
-    url: NotRequired[str]
+    serviceType: NotRequired[str]
+    serviceId: NotRequired[str]
+    serviceDirection: NotRequired[Literal["consumer", "producer", "prosumer"]]
 
 
-class GetDeviceResponse200Alt2(TypedDict):
+class GetDeviceResponse200Alt3(TypedDict):
     """
     Properties:
     - url: URL of the device
     - name: Name of the device
     - description: Extended description of the device, features, etc.
     - type: Type of the device
     - owner
-    - devices
+    - codeUrl
+    - services
     """
-    url: NotRequired[str]
-    name: NotRequired[str]
+    url: str
+    name: str
     description: NotRequired[str]
-    type: NotRequired[Literal["group"]]
-    owner: NotRequired[str]
-    devices: NotRequired[List[GetDeviceResponse200Alt2DevicesItems]]
+    type: Literal["edge instantiable"]
+    owner: str
+    codeUrl: NotRequired[str]
+    services: NotRequired[List[GetDeviceResponse200Alt3ServicesItems]]
 
 
-class GetDeviceResponse200Alt3(TypedDict):
+class GetDeviceResponse200Alt4DevicesItems(TypedDict):
     """
     Properties:
     - url: URL of the device
-    - name: Name of the device
-    - description: Extended description of the device, features, etc.
-    - type: Type of the device
-    - owner
-    - instantiate_url
     """
-    url: NotRequired[str]
-    name: NotRequired[str]
-    description: NotRequired[str]
-    type: NotRequired[Literal["cloud instantiable"]]
-    owner: NotRequired[str]
-    instantiate_url: NotRequired[str]
+    url: str
 
 
 class GetDeviceResponse200Alt4(TypedDict):
     """
     Properties:
     - url: URL of the device
     - name: Name of the device
     - description: Extended description of the device, features, etc.
     - type: Type of the device
     - owner
-    - code_url
+    - devices
     """
-    url: NotRequired[str]
-    name: NotRequired[str]
+    url: str
+    name: str
     description: NotRequired[str]
-    type: NotRequired[Literal["edge instantiable"]]
-    owner: NotRequired[str]
-    code_url: NotRequired[str]
+    type: Literal["group"]
+    owner: str
+    devices: List[GetDeviceResponse200Alt4DevicesItems]
 
 
 GetDeviceResponse200 = Union[GetDeviceResponse200Alt1, GetDeviceResponse200Alt2, GetDeviceResponse200Alt3, GetDeviceResponse200Alt4]
 
 
 GetDeviceResponse: TypeAlias = GetDeviceResponse200
 
 
-class UpdateDeviceRequestAlt1AnnouncedavailabilityItems(TypedDict):
-    """
-    Properties:
-    """
-
-
 class UpdateDeviceRequestAlt1ServicesItems(TypedDict):
     """
     Properties:
+    - serviceType
+    - serviceId
+    - serviceDirection
     """
+    serviceType: NotRequired[str]
+    serviceId: NotRequired[str]
+    serviceDirection: NotRequired[Literal["consumer", "producer", "prosumer"]]
 
 
 class UpdateDeviceRequestAlt1(TypedDict):
     """
     Properties:
-    - url: URL of the device
     - name: Name of the device
     - description: Extended description of the device, features, etc.
     - type: Type of the device
-    - owner
-    - connected: If true, the device is connected to the service and can be used.
-
-    - announcedAvailability: A list of time slots that the maintainer of the device announced it is available
-
-    - experiment
+    - instantiateUrl
     - services
     """
-    url: NotRequired[str]
     name: NotRequired[str]
     description: NotRequired[str]
-    type: NotRequired[Literal["device"]]
-    owner: NotRequired[str]
-    connected: NotRequired[bool]
-    announcedAvailability: NotRequired[List[UpdateDeviceRequestAlt1AnnouncedavailabilityItems]]
-    experiment: NotRequired[str]
+    type: Literal["cloud instantiable"]
+    instantiateUrl: NotRequired[str]
     services: NotRequired[List[UpdateDeviceRequestAlt1ServicesItems]]
 
 
-class UpdateDeviceRequestAlt2DevicesItems(TypedDict):
+class UpdateDeviceRequestAlt2ServicesItems(TypedDict):
     """
     Properties:
-    - url: URL of the device
+    - serviceType
+    - serviceId
+    - serviceDirection
     """
-    url: NotRequired[str]
+    serviceType: NotRequired[str]
+    serviceId: NotRequired[str]
+    serviceDirection: NotRequired[Literal["consumer", "producer", "prosumer"]]
 
 
 class UpdateDeviceRequestAlt2(TypedDict):
     """
     Properties:
-    - url: URL of the device
     - name: Name of the device
     - description: Extended description of the device, features, etc.
     - type: Type of the device
-    - owner
-    - devices
+    - experiment
+    - services
     """
-    url: NotRequired[str]
     name: NotRequired[str]
     description: NotRequired[str]
-    type: NotRequired[Literal["group"]]
-    owner: NotRequired[str]
-    devices: NotRequired[List[UpdateDeviceRequestAlt2DevicesItems]]
+    type: Literal["device"]
+    experiment: NotRequired[str]
+    services: NotRequired[List[UpdateDeviceRequestAlt2ServicesItems]]
+
+
+class UpdateDeviceRequestAlt3ServicesItems(TypedDict):
+    """
+    Properties:
+    - serviceType
+    - serviceId
+    - serviceDirection
+    """
+    serviceType: NotRequired[str]
+    serviceId: NotRequired[str]
+    serviceDirection: NotRequired[Literal["consumer", "producer", "prosumer"]]
 
 
 class UpdateDeviceRequestAlt3(TypedDict):
     """
     Properties:
-    - url: URL of the device
     - name: Name of the device
     - description: Extended description of the device, features, etc.
     - type: Type of the device
-    - owner
-    - instantiate_url
+    - codeUrl
+    - services
     """
-    url: NotRequired[str]
     name: NotRequired[str]
     description: NotRequired[str]
-    type: NotRequired[Literal["cloud instantiable"]]
-    owner: NotRequired[str]
-    instantiate_url: NotRequired[str]
+    type: Literal["edge instantiable"]
+    codeUrl: NotRequired[str]
+    services: NotRequired[List[UpdateDeviceRequestAlt3ServicesItems]]
 
 
-class UpdateDeviceRequestAlt4(TypedDict):
+class UpdateDeviceRequestAlt4DevicesItems(TypedDict):
     """
     Properties:
     - url: URL of the device
+    """
+    url: str
+
+
+class UpdateDeviceRequestAlt4(TypedDict):
+    """
+    Properties:
     - name: Name of the device
     - description: Extended description of the device, features, etc.
     - type: Type of the device
-    - owner
-    - code_url
+    - devices
     """
-    url: NotRequired[str]
     name: NotRequired[str]
     description: NotRequired[str]
-    type: NotRequired[Literal["edge instantiable"]]
-    owner: NotRequired[str]
-    code_url: NotRequired[str]
+    type: Literal["group"]
+    devices: NotRequired[List[UpdateDeviceRequestAlt4DevicesItems]]
 
 
 UpdateDeviceRequest = Union[UpdateDeviceRequestAlt1, UpdateDeviceRequestAlt2, UpdateDeviceRequestAlt3, UpdateDeviceRequestAlt4]
 
 
-class UpdateDeviceResponse200Alt1AnnouncedavailabilityItems(TypedDict):
+class UpdateDeviceResponse200Alt1ServicesItems(TypedDict):
+    """
+    Properties:
+    - serviceType
+    - serviceId
+    - serviceDirection
+    """
+    serviceType: NotRequired[str]
+    serviceId: NotRequired[str]
+    serviceDirection: NotRequired[Literal["consumer", "producer", "prosumer"]]
+
+
+class UpdateDeviceResponse200Alt1(TypedDict):
+    """
+    Properties:
+    - url: URL of the device
+    - name: Name of the device
+    - description: Extended description of the device, features, etc.
+    - type: Type of the device
+    - owner
+    - instantiateUrl
+    - services
+    """
+    url: str
+    name: str
+    description: NotRequired[str]
+    type: Literal["cloud instantiable"]
+    owner: str
+    instantiateUrl: NotRequired[str]
+    services: NotRequired[List[UpdateDeviceResponse200Alt1ServicesItems]]
+
+
+class UpdateDeviceResponse200Alt2AnnouncedavailabilityItems(TypedDict):
     """
     Properties:
     - start
     - end
     """
     start: NotRequired[str]
     end: NotRequired[str]
 
 
-class UpdateDeviceResponse200Alt1ServicesItems(TypedDict):
+class UpdateDeviceResponse200Alt2ServicesItems(TypedDict):
     """
     Properties:
+    - serviceType
+    - serviceId
+    - serviceDirection
     """
+    serviceType: NotRequired[str]
+    serviceId: NotRequired[str]
+    serviceDirection: NotRequired[Literal["consumer", "producer", "prosumer"]]
 
 
-class UpdateDeviceResponse200Alt1(TypedDict):
+class UpdateDeviceResponse200Alt2(TypedDict):
     """
     Properties:
     - url: URL of the device
     - name: Name of the device
     - description: Extended description of the device, features, etc.
     - type: Type of the device
     - owner
     - connected: If true, the device is connected to the service and can be used.
 
     - announcedAvailability: A list of time slots that the maintainer of the device announced it is available
 
     - experiment
     - services
     """
-    url: NotRequired[str]
-    name: NotRequired[str]
+    url: str
+    name: str
     description: NotRequired[str]
-    type: NotRequired[Literal["device"]]
-    owner: NotRequired[str]
+    type: Literal["device"]
+    owner: str
     connected: NotRequired[bool]
-    announcedAvailability: NotRequired[List[UpdateDeviceResponse200Alt1AnnouncedavailabilityItems]]
+    announcedAvailability: NotRequired[List[UpdateDeviceResponse200Alt2AnnouncedavailabilityItems]]
     experiment: NotRequired[str]
-    services: NotRequired[List[UpdateDeviceResponse200Alt1ServicesItems]]
+    services: NotRequired[List[UpdateDeviceResponse200Alt2ServicesItems]]
 
 
-class UpdateDeviceResponse200Alt2DevicesItems(TypedDict):
+class UpdateDeviceResponse200Alt3ServicesItems(TypedDict):
     """
     Properties:
-    - url: URL of the device
+    - serviceType
+    - serviceId
+    - serviceDirection
     """
-    url: NotRequired[str]
+    serviceType: NotRequired[str]
+    serviceId: NotRequired[str]
+    serviceDirection: NotRequired[Literal["consumer", "producer", "prosumer"]]
 
 
-class UpdateDeviceResponse200Alt2(TypedDict):
+class UpdateDeviceResponse200Alt3(TypedDict):
     """
     Properties:
     - url: URL of the device
     - name: Name of the device
     - description: Extended description of the device, features, etc.
     - type: Type of the device
     - owner
-    - devices
+    - codeUrl
+    - services
     """
-    url: NotRequired[str]
-    name: NotRequired[str]
+    url: str
+    name: str
     description: NotRequired[str]
-    type: NotRequired[Literal["group"]]
-    owner: NotRequired[str]
-    devices: NotRequired[List[UpdateDeviceResponse200Alt2DevicesItems]]
+    type: Literal["edge instantiable"]
+    owner: str
+    codeUrl: NotRequired[str]
+    services: NotRequired[List[UpdateDeviceResponse200Alt3ServicesItems]]
 
 
-class UpdateDeviceResponse200Alt3(TypedDict):
+class UpdateDeviceResponse200Alt4DevicesItems(TypedDict):
     """
     Properties:
     - url: URL of the device
-    - name: Name of the device
-    - description: Extended description of the device, features, etc.
-    - type: Type of the device
-    - owner
-    - instantiate_url
     """
-    url: NotRequired[str]
-    name: NotRequired[str]
-    description: NotRequired[str]
-    type: NotRequired[Literal["cloud instantiable"]]
-    owner: NotRequired[str]
-    instantiate_url: NotRequired[str]
+    url: str
 
 
 class UpdateDeviceResponse200Alt4(TypedDict):
     """
     Properties:
     - url: URL of the device
     - name: Name of the device
     - description: Extended description of the device, features, etc.
     - type: Type of the device
     - owner
-    - code_url
+    - devices
     """
-    url: NotRequired[str]
-    name: NotRequired[str]
+    url: str
+    name: str
     description: NotRequired[str]
-    type: NotRequired[Literal["edge instantiable"]]
-    owner: NotRequired[str]
-    code_url: NotRequired[str]
+    type: Literal["group"]
+    owner: str
+    devices: List[UpdateDeviceResponse200Alt4DevicesItems]
 
 
 UpdateDeviceResponse200 = Union[UpdateDeviceResponse200Alt1, UpdateDeviceResponse200Alt2, UpdateDeviceResponse200Alt3, UpdateDeviceResponse200Alt4]
 
 
 UpdateDeviceResponse: TypeAlias = UpdateDeviceResponse200
 
@@ -1362,15 +1397,21 @@
     start: NotRequired[str]
     end: NotRequired[str]
 
 
 class InstantiateDeviceResponse201InstanceServicesItems(TypedDict):
     """
     Properties:
+    - serviceType
+    - serviceId
+    - serviceDirection
     """
+    serviceType: NotRequired[str]
+    serviceId: NotRequired[str]
+    serviceDirection: NotRequired[Literal["consumer", "producer", "prosumer"]]
 
 
 class InstantiateDeviceResponse201Instance(TypedDict):
     """
     Properties:
     - url: URL of the device
     - name: Name of the device
@@ -1380,33 +1421,33 @@
     - connected: If true, the device is connected to the service and can be used.
 
     - announcedAvailability: A list of time slots that the maintainer of the device announced it is available
 
     - experiment
     - services
     """
-    url: NotRequired[str]
-    name: NotRequired[str]
+    url: str
+    name: str
     description: NotRequired[str]
-    type: NotRequired[Literal["device"]]
-    owner: NotRequired[str]
+    type: Literal["device"]
+    owner: str
     connected: NotRequired[bool]
     announcedAvailability: NotRequired[List[InstantiateDeviceResponse201InstanceAnnouncedavailabilityItems]]
     experiment: NotRequired[str]
     services: NotRequired[List[InstantiateDeviceResponse201InstanceServicesItems]]
 
 
 class InstantiateDeviceResponse201(TypedDict):
     """
     Properties:
     - instance
     - deviceToken
     """
-    instance: NotRequired[InstantiateDeviceResponse201Instance]
-    deviceToken: NotRequired[str]
+    instance: InstantiateDeviceResponse201Instance
+    deviceToken: str
 
 
 InstantiateDeviceResponse: TypeAlias = InstantiateDeviceResponse201
 
 
 class AddAvailabilityRulesRequestItems(TypedDict):
     """
@@ -1466,15 +1507,15 @@
     - connectionUrl
     - services
     - tiebreaker
     - config
     """
     messageType: Literal["command"]
     command: Literal["createPeerconnection"]
-    connectionType: Literal["webrtc", "websocket"]
+    connectionType: Literal["webrtc", "websocket", "local"]
     connectionUrl: str
     services: List[SendSignalingMessageRequestAlt1ServicesItems]
     tiebreaker: bool
     config: NotRequired[SendSignalingMessageRequestAlt1Config]
 
 
 class SendSignalingMessageRequestAlt2(TypedDict):
@@ -1516,25 +1557,29 @@
 
 
 class ListPeerconnectionsResponse200ItemsDevicesItems(TypedDict):
     """
     Properties:
     - url: URL of the device
     """
-    url: NotRequired[str]
+    url: str
 
 
 class ListPeerconnectionsResponse200Items(TypedDict):
     """
     Properties:
     - url: URL of the peerconnection
+    - type: Type of the peerconnection
+    - status: The status of the peerconnection.
     - devices
     """
-    url: NotRequired[str]
-    devices: NotRequired[List[ListPeerconnectionsResponse200ItemsDevicesItems]]
+    url: str
+    type: Literal["local", "webrtc"]
+    status: NotRequired[Literal["new", "connecting", "connected", "disconnected", "failed", "closed"]]
+    devices: List[ListPeerconnectionsResponse200ItemsDevicesItems]
 
 
 ListPeerconnectionsResponse200: TypeAlias = List[ListPeerconnectionsResponse200Items]
 
 
 ListPeerconnectionsResponse: TypeAlias = ListPeerconnectionsResponse200
 
@@ -1542,17 +1587,17 @@
 class CreatePeerconnectionRequestDevicesItemsConfigServicesItems(TypedDict):
     """
     Properties:
     - serviceType
     - serviceId
     - remoteServiceId
     """
-    serviceType: NotRequired[str]
-    serviceId: NotRequired[str]
-    remoteServiceId: NotRequired[str]
+    serviceType: str
+    serviceId: str
+    remoteServiceId: str
 
 
 class CreatePeerconnectionRequestDevicesItemsConfig(TypedDict):
     """
     Properties:
     - services
     """
@@ -1561,40 +1606,42 @@
 
 class CreatePeerconnectionRequestDevicesItems(TypedDict):
     """
     Properties:
     - url: URL of the device
     - config
     """
-    url: NotRequired[str]
+    url: str
     config: NotRequired[CreatePeerconnectionRequestDevicesItemsConfig]
 
 
 class CreatePeerconnectionRequest(TypedDict):
     """
     Properties:
     - url: URL of the peerconnection
-    - devices
+    - type: Type of the peerconnection
     - status: The status of the peerconnection.
+    - devices
     """
-    url: NotRequired[str]
-    devices: NotRequired[List[CreatePeerconnectionRequestDevicesItems]]
-    status: NotRequired[Literal["waiting-for-devices", "connected", "failed", "closed"]]
+    url: str
+    type: Literal["local", "webrtc"]
+    status: NotRequired[Literal["new", "connecting", "connected", "disconnected", "failed", "closed"]]
+    devices: List[CreatePeerconnectionRequestDevicesItems]
 
 
 class CreatePeerconnectionResponse201DevicesItemsConfigServicesItems(TypedDict):
     """
     Properties:
     - serviceType
     - serviceId
     - remoteServiceId
     """
-    serviceType: NotRequired[str]
-    serviceId: NotRequired[str]
-    remoteServiceId: NotRequired[str]
+    serviceType: str
+    serviceId: str
+    remoteServiceId: str
 
 
 class CreatePeerconnectionResponse201DevicesItemsConfig(TypedDict):
     """
     Properties:
     - services
     """
@@ -1603,40 +1650,42 @@
 
 class CreatePeerconnectionResponse201DevicesItems(TypedDict):
     """
     Properties:
     - url: URL of the device
     - config
     """
-    url: NotRequired[str]
+    url: str
     config: NotRequired[CreatePeerconnectionResponse201DevicesItemsConfig]
 
 
 class CreatePeerconnectionResponse201(TypedDict):
     """
     Properties:
     - url: URL of the peerconnection
-    - devices
+    - type: Type of the peerconnection
     - status: The status of the peerconnection.
+    - devices
     """
-    url: NotRequired[str]
-    devices: NotRequired[List[CreatePeerconnectionResponse201DevicesItems]]
-    status: NotRequired[Literal["waiting-for-devices", "connected", "failed", "closed"]]
+    url: str
+    type: Literal["local", "webrtc"]
+    status: NotRequired[Literal["new", "connecting", "connected", "disconnected", "failed", "closed"]]
+    devices: List[CreatePeerconnectionResponse201DevicesItems]
 
 
 class CreatePeerconnectionResponse202DevicesItemsConfigServicesItems(TypedDict):
     """
     Properties:
     - serviceType
     - serviceId
     - remoteServiceId
     """
-    serviceType: NotRequired[str]
-    serviceId: NotRequired[str]
-    remoteServiceId: NotRequired[str]
+    serviceType: str
+    serviceId: str
+    remoteServiceId: str
 
 
 class CreatePeerconnectionResponse202DevicesItemsConfig(TypedDict):
     """
     Properties:
     - services
     """
@@ -1645,43 +1694,45 @@
 
 class CreatePeerconnectionResponse202DevicesItems(TypedDict):
     """
     Properties:
     - url: URL of the device
     - config
     """
-    url: NotRequired[str]
+    url: str
     config: NotRequired[CreatePeerconnectionResponse202DevicesItemsConfig]
 
 
 class CreatePeerconnectionResponse202(TypedDict):
     """
     Properties:
     - url: URL of the peerconnection
-    - devices
+    - type: Type of the peerconnection
     - status: The status of the peerconnection.
+    - devices
     """
-    url: NotRequired[str]
-    devices: NotRequired[List[CreatePeerconnectionResponse202DevicesItems]]
-    status: NotRequired[Literal["waiting-for-devices", "connected", "failed", "closed"]]
+    url: str
+    type: Literal["local", "webrtc"]
+    status: NotRequired[Literal["new", "connecting", "connected", "disconnected", "failed", "closed"]]
+    devices: List[CreatePeerconnectionResponse202DevicesItems]
 
 
 CreatePeerconnectionResponse: TypeAlias = Union[CreatePeerconnectionResponse201, CreatePeerconnectionResponse202]
 
 
 class GetPeerconnectionResponse200DevicesItemsConfigServicesItems(TypedDict):
     """
     Properties:
     - serviceType
     - serviceId
     - remoteServiceId
     """
-    serviceType: NotRequired[str]
-    serviceId: NotRequired[str]
-    remoteServiceId: NotRequired[str]
+    serviceType: str
+    serviceId: str
+    remoteServiceId: str
 
 
 class GetPeerconnectionResponse200DevicesItemsConfig(TypedDict):
     """
     Properties:
     - services
     """
@@ -1690,36 +1741,49 @@
 
 class GetPeerconnectionResponse200DevicesItems(TypedDict):
     """
     Properties:
     - url: URL of the device
     - config
     """
-    url: NotRequired[str]
+    url: str
     config: NotRequired[GetPeerconnectionResponse200DevicesItemsConfig]
 
 
 class GetPeerconnectionResponse200(TypedDict):
     """
     Properties:
     - url: URL of the peerconnection
-    - devices
+    - type: Type of the peerconnection
     - status: The status of the peerconnection.
+    - devices
     """
-    url: NotRequired[str]
-    devices: NotRequired[List[GetPeerconnectionResponse200DevicesItems]]
-    status: NotRequired[Literal["waiting-for-devices", "connected", "failed", "closed"]]
+    url: str
+    type: Literal["local", "webrtc"]
+    status: NotRequired[Literal["new", "connecting", "connected", "disconnected", "failed", "closed"]]
+    devices: List[GetPeerconnectionResponse200DevicesItems]
 
 
 GetPeerconnectionResponse: TypeAlias = GetPeerconnectionResponse200
 
 
 DeletePeerconnectionResponse: TypeAlias = None
 
 
+class PatchPeerconnectionDeviceStatusRequest(TypedDict):
+    """
+    Properties:
+    - status: The status of the peerconnection.
+    """
+    status: Literal["new", "connecting", "connected", "disconnected", "failed", "closed"]
+
+
+PatchPeerconnectionDeviceStatusResponse: TypeAlias = None
+
+
 class ListExperimentsResponse200Items(TypedDict):
     """
     Properties:
     - url: URL of the experiment
     - status: Status of the experiment
     """
     url: NotRequired[str]
```

### Comparing `crosslab_api_client-0.2.2/src/crosslab_api_client.egg-info/SOURCES.txt` & `crosslab_api_client-0.2.3/src/crosslab_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crosslab_api_client-0.2.2/tests/test_improved_client.py` & `crosslab_api_client-0.2.3/tests/test_improved_client.py`

 * *Files identical despite different names*

### Comparing `crosslab_api_client-0.2.2/tests/test_openapi.py` & `crosslab_api_client-0.2.3/tests/test_openapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -502,36 +502,36 @@
     url = r'/users'
     url_variant = r'users'
     full_url = BASE_URL+r'/users'
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"roles":[{"url":"https://DeURFWCx.onpu.Mw7RTfb2f0l1WRLzoCO5oU","id":"enim anim","name":"non incididunt Duis pariatur minim","scopes":["anim voluptate aute Duis"]}],"url":"https://dhvskgVWHiqwVntPoDQGF.ovePGeHEMw62XGwjeRU8wlzpIq5MThVrmqRhgckA-PLHLyY,zw+oQY"},{"roles":[{"url":"http://guBFBXETlaqfTdLLERbYNLLxZfDPO.cpikrn3,,iXCReR4ttNoe-tMnW,hKH1KPFSPED.4dVYJyHO3rzehHFgRkEY5teKM06BwHocOzVHwyg,"}],"password":"elit esse aute","username":"culpa","url":"http://ulxpvZToDIljIFfbjoFuAGBWNAOtS.fqegaiBJIsMZvyhownQK8JUbyjybkXJh,jzugkWn1ynn,-Ns3FAcYzdlQsMoygSVAjcS"},{"username":"proident Ut ad reprehenderit","roles":[{"url":"http://YfHcCjfNllGG.jvkhcj3bIX7FusXR++ln7ptUnTRvS9tw"},{"name":"aliquip ullamco culpa consequat","id":"in adipisicing","url":"https://PSkjL.rbUkxB9XvO+SAZ-s5iURdPqEn88GdVFYDNTUhtH8XsdZNZFuVC"},{"url":"http://vPvLleEDIbPSRvhKNMrErekJWIK.eibvkaeIbOawfCEA4OcE8mDAn8qofAP0Vr3cpaxvhabQWVecNZOqDCz5oJ3","scopes":["veniam non ut","exercitation commodo elit","adipisicing tempor","cupidatat Ut dolor reprehenderit","reprehenderit ut ipsum et cupidatat"],"id":"velit Excepteur occaecat"}],"url":"https://GXYKIhsWipBeJUIcBNukIdJE.hvVmOk85dI5oEflv,EDD+0-eJOa2qdHKltLPwsg9GJbzaQtJhzdVuNw3KucXXHSJzZckeMPFcGv"},{"roles":[{"url":"https://zjihqqLRdlnACjMmxxukpKeC.dovQ0iw-ZmN6q8sTZyw6F0FTZSbziJGvEeIVH1GN0ttobx0vNnfyrpwTmV5TmlGc2KNvdrmx","id":"elit sint non consectetur do","name":"laborum incididunt exercitation","scopes":["fugiat aute eiusmod aliquip","in eu Lorem","voluptate incididunt dolore dolore"]},{"url":"http://fcJDGAMVZZteWEL.lrZBLoqWr,-OhEIp52w5ni6b1KGQTs.B","scopes":["id labore ut voluptate","ex magna deserunt culpa Ut","aliquip","eu adipisicing dolore aliqua reprehenderit","elit enim commodo"]}],"password":"dolore in","id":"Excepteur dolor consectetur cupidatat","url":"https://LsSgDHAqAGEtaRzEMBLYlkq.keaOZMqdQo6mUVs3RF6NaIKRDy45Edaa6bLzykKVsfHjYxnH+qEgP5HsYmgYrYeX4","username":"cupidatat nostrud esse dolore nulla"}]')
+        response_200_dict = json.loads(r'[{"url":"http://SyrjwTQktCePOwvKc.blfpSOA","id":"amet in irure ullamco","username":"proident occaecat","password":"do"},{"url":"https://FZTzXTceuBxxrAqTMCqKPQwFuhRlTkh.ozV,iY4Cq5F6ByZLCcSu8yqfCD","id":"dolor mollit in","username":"do in dolor aliquip anim","password":"adipisicing"},{"url":"http://ShyjZbZHQpYRrA.yqwHM27xmpypXQe.OAYKAUMLLLKDlgGO2MpdZKOinzOJ4Iz.QZxUUB4WRkvFk6O5kNaDA","id":"minim adipisicing consequat nostrud","username":"id ut officia aute","password":"ullamco irure nulla magna"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_users(**parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"roles":[{"url":"https://DeURFWCx.onpu.Mw7RTfb2f0l1WRLzoCO5oU","id":"enim anim","name":"non incididunt Duis pariatur minim","scopes":["anim voluptate aute Duis"]}],"url":"https://dhvskgVWHiqwVntPoDQGF.ovePGeHEMw62XGwjeRU8wlzpIq5MThVrmqRhgckA-PLHLyY,zw+oQY"},{"roles":[{"url":"http://guBFBXETlaqfTdLLERbYNLLxZfDPO.cpikrn3,,iXCReR4ttNoe-tMnW,hKH1KPFSPED.4dVYJyHO3rzehHFgRkEY5teKM06BwHocOzVHwyg,"}],"password":"elit esse aute","username":"culpa","url":"http://ulxpvZToDIljIFfbjoFuAGBWNAOtS.fqegaiBJIsMZvyhownQK8JUbyjybkXJh,jzugkWn1ynn,-Ns3FAcYzdlQsMoygSVAjcS"},{"username":"proident Ut ad reprehenderit","roles":[{"url":"http://YfHcCjfNllGG.jvkhcj3bIX7FusXR++ln7ptUnTRvS9tw"},{"name":"aliquip ullamco culpa consequat","id":"in adipisicing","url":"https://PSkjL.rbUkxB9XvO+SAZ-s5iURdPqEn88GdVFYDNTUhtH8XsdZNZFuVC"},{"url":"http://vPvLleEDIbPSRvhKNMrErekJWIK.eibvkaeIbOawfCEA4OcE8mDAn8qofAP0Vr3cpaxvhabQWVecNZOqDCz5oJ3","scopes":["veniam non ut","exercitation commodo elit","adipisicing tempor","cupidatat Ut dolor reprehenderit","reprehenderit ut ipsum et cupidatat"],"id":"velit Excepteur occaecat"}],"url":"https://GXYKIhsWipBeJUIcBNukIdJE.hvVmOk85dI5oEflv,EDD+0-eJOa2qdHKltLPwsg9GJbzaQtJhzdVuNw3KucXXHSJzZckeMPFcGv"},{"roles":[{"url":"https://zjihqqLRdlnACjMmxxukpKeC.dovQ0iw-ZmN6q8sTZyw6F0FTZSbziJGvEeIVH1GN0ttobx0vNnfyrpwTmV5TmlGc2KNvdrmx","id":"elit sint non consectetur do","name":"laborum incididunt exercitation","scopes":["fugiat aute eiusmod aliquip","in eu Lorem","voluptate incididunt dolore dolore"]},{"url":"http://fcJDGAMVZZteWEL.lrZBLoqWr,-OhEIp52w5ni6b1KGQTs.B","scopes":["id labore ut voluptate","ex magna deserunt culpa Ut","aliquip","eu adipisicing dolore aliqua reprehenderit","elit enim commodo"]}],"password":"dolore in","id":"Excepteur dolor consectetur cupidatat","url":"https://LsSgDHAqAGEtaRzEMBLYlkq.keaOZMqdQo6mUVs3RF6NaIKRDy45Edaa6bLzykKVsfHjYxnH+qEgP5HsYmgYrYeX4","username":"cupidatat nostrud esse dolore nulla"}]')
+        response_200_dict = json.loads(r'[{"url":"http://SyrjwTQktCePOwvKc.blfpSOA","id":"amet in irure ullamco","username":"proident occaecat","password":"do"},{"url":"https://FZTzXTceuBxxrAqTMCqKPQwFuhRlTkh.ozV,iY4Cq5F6ByZLCcSu8yqfCD","id":"dolor mollit in","username":"do in dolor aliquip anim","password":"adipisicing"},{"url":"http://ShyjZbZHQpYRrA.yqwHM27xmpypXQe.OAYKAUMLLLKDlgGO2MpdZKOinzOJ4Iz.QZxUUB4WRkvFk6O5kNaDA","id":"minim adipisicing consequat nostrud","username":"id ut officia aute","password":"ullamco irure nulla magna"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_users(url=url, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"roles":[{"url":"https://DeURFWCx.onpu.Mw7RTfb2f0l1WRLzoCO5oU","id":"enim anim","name":"non incididunt Duis pariatur minim","scopes":["anim voluptate aute Duis"]}],"url":"https://dhvskgVWHiqwVntPoDQGF.ovePGeHEMw62XGwjeRU8wlzpIq5MThVrmqRhgckA-PLHLyY,zw+oQY"},{"roles":[{"url":"http://guBFBXETlaqfTdLLERbYNLLxZfDPO.cpikrn3,,iXCReR4ttNoe-tMnW,hKH1KPFSPED.4dVYJyHO3rzehHFgRkEY5teKM06BwHocOzVHwyg,"}],"password":"elit esse aute","username":"culpa","url":"http://ulxpvZToDIljIFfbjoFuAGBWNAOtS.fqegaiBJIsMZvyhownQK8JUbyjybkXJh,jzugkWn1ynn,-Ns3FAcYzdlQsMoygSVAjcS"},{"username":"proident Ut ad reprehenderit","roles":[{"url":"http://YfHcCjfNllGG.jvkhcj3bIX7FusXR++ln7ptUnTRvS9tw"},{"name":"aliquip ullamco culpa consequat","id":"in adipisicing","url":"https://PSkjL.rbUkxB9XvO+SAZ-s5iURdPqEn88GdVFYDNTUhtH8XsdZNZFuVC"},{"url":"http://vPvLleEDIbPSRvhKNMrErekJWIK.eibvkaeIbOawfCEA4OcE8mDAn8qofAP0Vr3cpaxvhabQWVecNZOqDCz5oJ3","scopes":["veniam non ut","exercitation commodo elit","adipisicing tempor","cupidatat Ut dolor reprehenderit","reprehenderit ut ipsum et cupidatat"],"id":"velit Excepteur occaecat"}],"url":"https://GXYKIhsWipBeJUIcBNukIdJE.hvVmOk85dI5oEflv,EDD+0-eJOa2qdHKltLPwsg9GJbzaQtJhzdVuNw3KucXXHSJzZckeMPFcGv"},{"roles":[{"url":"https://zjihqqLRdlnACjMmxxukpKeC.dovQ0iw-ZmN6q8sTZyw6F0FTZSbziJGvEeIVH1GN0ttobx0vNnfyrpwTmV5TmlGc2KNvdrmx","id":"elit sint non consectetur do","name":"laborum incididunt exercitation","scopes":["fugiat aute eiusmod aliquip","in eu Lorem","voluptate incididunt dolore dolore"]},{"url":"http://fcJDGAMVZZteWEL.lrZBLoqWr,-OhEIp52w5ni6b1KGQTs.B","scopes":["id labore ut voluptate","ex magna deserunt culpa Ut","aliquip","eu adipisicing dolore aliqua reprehenderit","elit enim commodo"]}],"password":"dolore in","id":"Excepteur dolor consectetur cupidatat","url":"https://LsSgDHAqAGEtaRzEMBLYlkq.keaOZMqdQo6mUVs3RF6NaIKRDy45Edaa6bLzykKVsfHjYxnH+qEgP5HsYmgYrYeX4","username":"cupidatat nostrud esse dolore nulla"}]')
+        response_200_dict = json.loads(r'[{"url":"http://SyrjwTQktCePOwvKc.blfpSOA","id":"amet in irure ullamco","username":"proident occaecat","password":"do"},{"url":"https://FZTzXTceuBxxrAqTMCqKPQwFuhRlTkh.ozV,iY4Cq5F6ByZLCcSu8yqfCD","id":"dolor mollit in","username":"do in dolor aliquip anim","password":"adipisicing"},{"url":"http://ShyjZbZHQpYRrA.yqwHM27xmpypXQe.OAYKAUMLLLKDlgGO2MpdZKOinzOJ4Iz.QZxUUB4WRkvFk6O5kNaDA","id":"minim adipisicing consequat nostrud","username":"id ut officia aute","password":"ullamco irure nulla magna"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_users(url=url_variant, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"roles":[{"url":"https://DeURFWCx.onpu.Mw7RTfb2f0l1WRLzoCO5oU","id":"enim anim","name":"non incididunt Duis pariatur minim","scopes":["anim voluptate aute Duis"]}],"url":"https://dhvskgVWHiqwVntPoDQGF.ovePGeHEMw62XGwjeRU8wlzpIq5MThVrmqRhgckA-PLHLyY,zw+oQY"},{"roles":[{"url":"http://guBFBXETlaqfTdLLERbYNLLxZfDPO.cpikrn3,,iXCReR4ttNoe-tMnW,hKH1KPFSPED.4dVYJyHO3rzehHFgRkEY5teKM06BwHocOzVHwyg,"}],"password":"elit esse aute","username":"culpa","url":"http://ulxpvZToDIljIFfbjoFuAGBWNAOtS.fqegaiBJIsMZvyhownQK8JUbyjybkXJh,jzugkWn1ynn,-Ns3FAcYzdlQsMoygSVAjcS"},{"username":"proident Ut ad reprehenderit","roles":[{"url":"http://YfHcCjfNllGG.jvkhcj3bIX7FusXR++ln7ptUnTRvS9tw"},{"name":"aliquip ullamco culpa consequat","id":"in adipisicing","url":"https://PSkjL.rbUkxB9XvO+SAZ-s5iURdPqEn88GdVFYDNTUhtH8XsdZNZFuVC"},{"url":"http://vPvLleEDIbPSRvhKNMrErekJWIK.eibvkaeIbOawfCEA4OcE8mDAn8qofAP0Vr3cpaxvhabQWVecNZOqDCz5oJ3","scopes":["veniam non ut","exercitation commodo elit","adipisicing tempor","cupidatat Ut dolor reprehenderit","reprehenderit ut ipsum et cupidatat"],"id":"velit Excepteur occaecat"}],"url":"https://GXYKIhsWipBeJUIcBNukIdJE.hvVmOk85dI5oEflv,EDD+0-eJOa2qdHKltLPwsg9GJbzaQtJhzdVuNw3KucXXHSJzZckeMPFcGv"},{"roles":[{"url":"https://zjihqqLRdlnACjMmxxukpKeC.dovQ0iw-ZmN6q8sTZyw6F0FTZSbziJGvEeIVH1GN0ttobx0vNnfyrpwTmV5TmlGc2KNvdrmx","id":"elit sint non consectetur do","name":"laborum incididunt exercitation","scopes":["fugiat aute eiusmod aliquip","in eu Lorem","voluptate incididunt dolore dolore"]},{"url":"http://fcJDGAMVZZteWEL.lrZBLoqWr,-OhEIp52w5ni6b1KGQTs.B","scopes":["id labore ut voluptate","ex magna deserunt culpa Ut","aliquip","eu adipisicing dolore aliqua reprehenderit","elit enim commodo"]}],"password":"dolore in","id":"Excepteur dolor consectetur cupidatat","url":"https://LsSgDHAqAGEtaRzEMBLYlkq.keaOZMqdQo6mUVs3RF6NaIKRDy45Edaa6bLzykKVsfHjYxnH+qEgP5HsYmgYrYeX4","username":"cupidatat nostrud esse dolore nulla"}]')
+        response_200_dict = json.loads(r'[{"url":"http://SyrjwTQktCePOwvKc.blfpSOA","id":"amet in irure ullamco","username":"proident occaecat","password":"do"},{"url":"https://FZTzXTceuBxxrAqTMCqKPQwFuhRlTkh.ozV,iY4Cq5F6ByZLCcSu8yqfCD","id":"dolor mollit in","username":"do in dolor aliquip anim","password":"adipisicing"},{"url":"http://ShyjZbZHQpYRrA.yqwHM27xmpypXQe.OAYKAUMLLLKDlgGO2MpdZKOinzOJ4Iz.QZxUUB4WRkvFk6O5kNaDA","id":"minim adipisicing consequat nostrud","username":"id ut officia aute","password":"ullamco irure nulla magna"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_users(url=full_url, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
@@ -656,41 +656,41 @@
 
 @pytest.mark.asyncio
 async def test_create_user(aioresponses: aioresponses):
     url = r'/users'
     url_variant = r'users'
     full_url = BASE_URL+r'/users'
 
-    request = json.loads(r'{"username":"occaecat ex exercitation proident dolore","password":"laborum"}')
+    request = json.loads(r'{"url":"https://FBpFkjeMvxKCcBpxVjYLeOQ.jmhVgh-F,O,iQ6yI+,lfJZ9fx7cG5,1eX.UCVrA.QH+YJ","id":"adipisicing labore Duis aliquip consectetur","username":"irure ullamco reprehenderit cillum et","password":"ea eiusmod consequat commodo"}')
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
-        response_201_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
+        response_201_dict = json.loads(r'{"url":"https://FBpFkjeMvxKCcBpxVjYLeOQ.jmhVgh-F,O,iQ6yI+,lfJZ9fx7cG5,1eX.UCVrA.QH+YJ","id":"adipisicing labore Duis aliquip consectetur","username":"irure ullamco reprehenderit cillum et","password":"ea eiusmod consequat commodo"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_user(body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
-        response_201_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
+        response_201_dict = json.loads(r'{"url":"https://FBpFkjeMvxKCcBpxVjYLeOQ.jmhVgh-F,O,iQ6yI+,lfJZ9fx7cG5,1eX.UCVrA.QH+YJ","id":"adipisicing labore Duis aliquip consectetur","username":"irure ullamco reprehenderit cillum et","password":"ea eiusmod consequat commodo"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_user(url=url, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
-        response_201_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
+        response_201_dict = json.loads(r'{"url":"https://FBpFkjeMvxKCcBpxVjYLeOQ.jmhVgh-F,O,iQ6yI+,lfJZ9fx7cG5,1eX.UCVrA.QH+YJ","id":"adipisicing labore Duis aliquip consectetur","username":"irure ullamco reprehenderit cillum et","password":"ea eiusmod consequat commodo"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_user(url=url_variant, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
-        response_201_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
+        response_201_dict = json.loads(r'{"url":"https://FBpFkjeMvxKCcBpxVjYLeOQ.jmhVgh-F,O,iQ6yI+,lfJZ9fx7cG5,1eX.UCVrA.QH+YJ","id":"adipisicing labore Duis aliquip consectetur","username":"irure ullamco reprehenderit cillum et","password":"ea eiusmod consequat commodo"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_user(url=full_url, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
@@ -818,29 +818,29 @@
     url = r'/users/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     url_variant = r'users/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     full_url = BASE_URL+r'/users/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
+        response_200_dict = json.loads(r'{"url":"https://FBpFkjeMvxKCcBpxVjYLeOQ.jmhVgh-F,O,iQ6yI+,lfJZ9fx7cG5,1eX.UCVrA.QH+YJ","id":"adipisicing labore Duis aliquip consectetur","username":"irure ullamco reprehenderit cillum et","password":"ea eiusmod consequat commodo"}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_user(url=url, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
+        response_200_dict = json.loads(r'{"url":"https://FBpFkjeMvxKCcBpxVjYLeOQ.jmhVgh-F,O,iQ6yI+,lfJZ9fx7cG5,1eX.UCVrA.QH+YJ","id":"adipisicing labore Duis aliquip consectetur","username":"irure ullamco reprehenderit cillum et","password":"ea eiusmod consequat commodo"}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_user(url=url_variant, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
+        response_200_dict = json.loads(r'{"url":"https://FBpFkjeMvxKCcBpxVjYLeOQ.jmhVgh-F,O,iQ6yI+,lfJZ9fx7cG5,1eX.UCVrA.QH+YJ","id":"adipisicing labore Duis aliquip consectetur","username":"irure ullamco reprehenderit cillum et","password":"ea eiusmod consequat commodo"}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_user(url=full_url, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
@@ -940,29 +940,29 @@
     full_url = BASE_URL+r'/users/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
 
     request = json.loads(r'{"username":"tempor","password":"ad"}')
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
+        response_200_dict = json.loads(r'{"url":"https://FBpFkjeMvxKCcBpxVjYLeOQ.jmhVgh-F,O,iQ6yI+,lfJZ9fx7cG5,1eX.UCVrA.QH+YJ","id":"adipisicing labore Duis aliquip consectetur","username":"irure ullamco reprehenderit cillum et","password":"ea eiusmod consequat commodo"}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_user(url=url, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
+        response_200_dict = json.loads(r'{"url":"https://FBpFkjeMvxKCcBpxVjYLeOQ.jmhVgh-F,O,iQ6yI+,lfJZ9fx7cG5,1eX.UCVrA.QH+YJ","id":"adipisicing labore Duis aliquip consectetur","username":"irure ullamco reprehenderit cillum et","password":"ea eiusmod consequat commodo"}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_user(url=url_variant, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
+        response_200_dict = json.loads(r'{"url":"https://FBpFkjeMvxKCcBpxVjYLeOQ.jmhVgh-F,O,iQ6yI+,lfJZ9fx7cG5,1eX.UCVrA.QH+YJ","id":"adipisicing labore Duis aliquip consectetur","username":"irure ullamco reprehenderit cillum et","password":"ea eiusmod consequat commodo"}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_user(url=full_url, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
@@ -1174,29 +1174,29 @@
     url = r'/users/c799cc2e-cdc5-4143-973a-6f56a5afa82c/roles'
     url_variant = r'users/c799cc2e-cdc5-4143-973a-6f56a5afa82c/roles'
     full_url = BASE_URL+r'/users/c799cc2e-cdc5-4143-973a-6f56a5afa82c/roles'
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"id":"nisi nostrud nulla sit","url":"https://aeUhNJdx.hxjnM137Xzngz--,VAiwP","name":"ipsum ullamco in","scopes":["Ut Duis","non consequat labore dolor Duis","anim elit sed nisi","Ut sunt exercitation non"]},{"name":"mollit qui enim ad Ut","id":"in ut eiusmod"}]')
+        response_200_dict = json.loads(r'[{"url":"https://OLpu.dtfmcuhkZO-euv+B6sOSHXAKZD5w","id":"Lorem","name":"ex dolore","scopes":["cupidatat","adipisicing ullamco proident sit tempor","anim ea fugiat enim quis"]},{"url":"http://QdzMFHAKUsxWSQmrfDLkqRlEJjZgQTzU.rjawur.KCW3oxYYuZNNphMnsZEF1zt1dgotHDgzlSHt7","id":"id nostrud amet","name":"occaecat qui cupidatat adipisicing","scopes":["cillum","nostrud ullamco in","tempor dolore culpa magna","proident et incididunt commodo in"]},{"url":"http://dyrMl.wkddWUkV0XNW8kC1V,YrjKS-j0ik2YLwXJm3nuJ30u9wexTRmdmczFG3-V3+","id":"aute sunt proident","name":"deserunt mollit","scopes":["nisi quis consectetur fugiat amet","officia commodo aliqua eiusmod","occaecat do mollit","ex in","tempor labore ut"]},{"url":"http://djtIqVvqHAiXJLDTRs.ysgueOHWIsSu6L5JukDjKjap8CaRkt.BSoqRr","id":"aute commodo consectetur","name":"cupidatat exercitation sed laborum","scopes":["incididunt laboris","id sed dolore","veniam","culpa"]},{"url":"https://tFjmRLNMKusuxdQ.vqtfHoBz0+2qM+mj1dapXXaHFguVGvQ3uhj-zAUGYvgQssJi6Iagh","id":"et veniam laborum","name":"qui sed dolor quis est","scopes":["consequat irure","in quis ex","Excepteur anim","ullamco incididunt exercitation"]}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_roles_of_user(url=url, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"id":"nisi nostrud nulla sit","url":"https://aeUhNJdx.hxjnM137Xzngz--,VAiwP","name":"ipsum ullamco in","scopes":["Ut Duis","non consequat labore dolor Duis","anim elit sed nisi","Ut sunt exercitation non"]},{"name":"mollit qui enim ad Ut","id":"in ut eiusmod"}]')
+        response_200_dict = json.loads(r'[{"url":"https://OLpu.dtfmcuhkZO-euv+B6sOSHXAKZD5w","id":"Lorem","name":"ex dolore","scopes":["cupidatat","adipisicing ullamco proident sit tempor","anim ea fugiat enim quis"]},{"url":"http://QdzMFHAKUsxWSQmrfDLkqRlEJjZgQTzU.rjawur.KCW3oxYYuZNNphMnsZEF1zt1dgotHDgzlSHt7","id":"id nostrud amet","name":"occaecat qui cupidatat adipisicing","scopes":["cillum","nostrud ullamco in","tempor dolore culpa magna","proident et incididunt commodo in"]},{"url":"http://dyrMl.wkddWUkV0XNW8kC1V,YrjKS-j0ik2YLwXJm3nuJ30u9wexTRmdmczFG3-V3+","id":"aute sunt proident","name":"deserunt mollit","scopes":["nisi quis consectetur fugiat amet","officia commodo aliqua eiusmod","occaecat do mollit","ex in","tempor labore ut"]},{"url":"http://djtIqVvqHAiXJLDTRs.ysgueOHWIsSu6L5JukDjKjap8CaRkt.BSoqRr","id":"aute commodo consectetur","name":"cupidatat exercitation sed laborum","scopes":["incididunt laboris","id sed dolore","veniam","culpa"]},{"url":"https://tFjmRLNMKusuxdQ.vqtfHoBz0+2qM+mj1dapXXaHFguVGvQ3uhj-zAUGYvgQssJi6Iagh","id":"et veniam laborum","name":"qui sed dolor quis est","scopes":["consequat irure","in quis ex","Excepteur anim","ullamco incididunt exercitation"]}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_roles_of_user(url=url_variant, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"id":"nisi nostrud nulla sit","url":"https://aeUhNJdx.hxjnM137Xzngz--,VAiwP","name":"ipsum ullamco in","scopes":["Ut Duis","non consequat labore dolor Duis","anim elit sed nisi","Ut sunt exercitation non"]},{"name":"mollit qui enim ad Ut","id":"in ut eiusmod"}]')
+        response_200_dict = json.loads(r'[{"url":"https://OLpu.dtfmcuhkZO-euv+B6sOSHXAKZD5w","id":"Lorem","name":"ex dolore","scopes":["cupidatat","adipisicing ullamco proident sit tempor","anim ea fugiat enim quis"]},{"url":"http://QdzMFHAKUsxWSQmrfDLkqRlEJjZgQTzU.rjawur.KCW3oxYYuZNNphMnsZEF1zt1dgotHDgzlSHt7","id":"id nostrud amet","name":"occaecat qui cupidatat adipisicing","scopes":["cillum","nostrud ullamco in","tempor dolore culpa magna","proident et incididunt commodo in"]},{"url":"http://dyrMl.wkddWUkV0XNW8kC1V,YrjKS-j0ik2YLwXJm3nuJ30u9wexTRmdmczFG3-V3+","id":"aute sunt proident","name":"deserunt mollit","scopes":["nisi quis consectetur fugiat amet","officia commodo aliqua eiusmod","occaecat do mollit","ex in","tempor labore ut"]},{"url":"http://djtIqVvqHAiXJLDTRs.ysgueOHWIsSu6L5JukDjKjap8CaRkt.BSoqRr","id":"aute commodo consectetur","name":"cupidatat exercitation sed laborum","scopes":["incididunt laboris","id sed dolore","veniam","culpa"]},{"url":"https://tFjmRLNMKusuxdQ.vqtfHoBz0+2qM+mj1dapXXaHFguVGvQ3uhj-zAUGYvgQssJi6Iagh","id":"et veniam laborum","name":"qui sed dolor quis est","scopes":["consequat irure","in quis ex","Excepteur anim","ullamco incididunt exercitation"]}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_roles_of_user(url=full_url, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
@@ -1526,36 +1526,36 @@
     url = r'/roles'
     url_variant = r'roles'
     full_url = BASE_URL+r'/roles'
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"id":"nisi nostrud nulla sit","url":"https://aeUhNJdx.hxjnM137Xzngz--,VAiwP","name":"ipsum ullamco in","scopes":["Ut Duis","non consequat labore dolor Duis","anim elit sed nisi","Ut sunt exercitation non"]},{"name":"mollit qui enim ad Ut","id":"in ut eiusmod"}]')
+        response_200_dict = json.loads(r'[{"url":"https://OLpu.dtfmcuhkZO-euv+B6sOSHXAKZD5w","id":"Lorem","name":"ex dolore","scopes":["cupidatat","adipisicing ullamco proident sit tempor","anim ea fugiat enim quis"]},{"url":"http://QdzMFHAKUsxWSQmrfDLkqRlEJjZgQTzU.rjawur.KCW3oxYYuZNNphMnsZEF1zt1dgotHDgzlSHt7","id":"id nostrud amet","name":"occaecat qui cupidatat adipisicing","scopes":["cillum","nostrud ullamco in","tempor dolore culpa magna","proident et incididunt commodo in"]},{"url":"http://dyrMl.wkddWUkV0XNW8kC1V,YrjKS-j0ik2YLwXJm3nuJ30u9wexTRmdmczFG3-V3+","id":"aute sunt proident","name":"deserunt mollit","scopes":["nisi quis consectetur fugiat amet","officia commodo aliqua eiusmod","occaecat do mollit","ex in","tempor labore ut"]},{"url":"http://djtIqVvqHAiXJLDTRs.ysgueOHWIsSu6L5JukDjKjap8CaRkt.BSoqRr","id":"aute commodo consectetur","name":"cupidatat exercitation sed laborum","scopes":["incididunt laboris","id sed dolore","veniam","culpa"]},{"url":"https://tFjmRLNMKusuxdQ.vqtfHoBz0+2qM+mj1dapXXaHFguVGvQ3uhj-zAUGYvgQssJi6Iagh","id":"et veniam laborum","name":"qui sed dolor quis est","scopes":["consequat irure","in quis ex","Excepteur anim","ullamco incididunt exercitation"]}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_roles(**parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"id":"nisi nostrud nulla sit","url":"https://aeUhNJdx.hxjnM137Xzngz--,VAiwP","name":"ipsum ullamco in","scopes":["Ut Duis","non consequat labore dolor Duis","anim elit sed nisi","Ut sunt exercitation non"]},{"name":"mollit qui enim ad Ut","id":"in ut eiusmod"}]')
+        response_200_dict = json.loads(r'[{"url":"https://OLpu.dtfmcuhkZO-euv+B6sOSHXAKZD5w","id":"Lorem","name":"ex dolore","scopes":["cupidatat","adipisicing ullamco proident sit tempor","anim ea fugiat enim quis"]},{"url":"http://QdzMFHAKUsxWSQmrfDLkqRlEJjZgQTzU.rjawur.KCW3oxYYuZNNphMnsZEF1zt1dgotHDgzlSHt7","id":"id nostrud amet","name":"occaecat qui cupidatat adipisicing","scopes":["cillum","nostrud ullamco in","tempor dolore culpa magna","proident et incididunt commodo in"]},{"url":"http://dyrMl.wkddWUkV0XNW8kC1V,YrjKS-j0ik2YLwXJm3nuJ30u9wexTRmdmczFG3-V3+","id":"aute sunt proident","name":"deserunt mollit","scopes":["nisi quis consectetur fugiat amet","officia commodo aliqua eiusmod","occaecat do mollit","ex in","tempor labore ut"]},{"url":"http://djtIqVvqHAiXJLDTRs.ysgueOHWIsSu6L5JukDjKjap8CaRkt.BSoqRr","id":"aute commodo consectetur","name":"cupidatat exercitation sed laborum","scopes":["incididunt laboris","id sed dolore","veniam","culpa"]},{"url":"https://tFjmRLNMKusuxdQ.vqtfHoBz0+2qM+mj1dapXXaHFguVGvQ3uhj-zAUGYvgQssJi6Iagh","id":"et veniam laborum","name":"qui sed dolor quis est","scopes":["consequat irure","in quis ex","Excepteur anim","ullamco incididunt exercitation"]}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_roles(url=url, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"id":"nisi nostrud nulla sit","url":"https://aeUhNJdx.hxjnM137Xzngz--,VAiwP","name":"ipsum ullamco in","scopes":["Ut Duis","non consequat labore dolor Duis","anim elit sed nisi","Ut sunt exercitation non"]},{"name":"mollit qui enim ad Ut","id":"in ut eiusmod"}]')
+        response_200_dict = json.loads(r'[{"url":"https://OLpu.dtfmcuhkZO-euv+B6sOSHXAKZD5w","id":"Lorem","name":"ex dolore","scopes":["cupidatat","adipisicing ullamco proident sit tempor","anim ea fugiat enim quis"]},{"url":"http://QdzMFHAKUsxWSQmrfDLkqRlEJjZgQTzU.rjawur.KCW3oxYYuZNNphMnsZEF1zt1dgotHDgzlSHt7","id":"id nostrud amet","name":"occaecat qui cupidatat adipisicing","scopes":["cillum","nostrud ullamco in","tempor dolore culpa magna","proident et incididunt commodo in"]},{"url":"http://dyrMl.wkddWUkV0XNW8kC1V,YrjKS-j0ik2YLwXJm3nuJ30u9wexTRmdmczFG3-V3+","id":"aute sunt proident","name":"deserunt mollit","scopes":["nisi quis consectetur fugiat amet","officia commodo aliqua eiusmod","occaecat do mollit","ex in","tempor labore ut"]},{"url":"http://djtIqVvqHAiXJLDTRs.ysgueOHWIsSu6L5JukDjKjap8CaRkt.BSoqRr","id":"aute commodo consectetur","name":"cupidatat exercitation sed laborum","scopes":["incididunt laboris","id sed dolore","veniam","culpa"]},{"url":"https://tFjmRLNMKusuxdQ.vqtfHoBz0+2qM+mj1dapXXaHFguVGvQ3uhj-zAUGYvgQssJi6Iagh","id":"et veniam laborum","name":"qui sed dolor quis est","scopes":["consequat irure","in quis ex","Excepteur anim","ullamco incididunt exercitation"]}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_roles(url=url_variant, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"id":"nisi nostrud nulla sit","url":"https://aeUhNJdx.hxjnM137Xzngz--,VAiwP","name":"ipsum ullamco in","scopes":["Ut Duis","non consequat labore dolor Duis","anim elit sed nisi","Ut sunt exercitation non"]},{"name":"mollit qui enim ad Ut","id":"in ut eiusmod"}]')
+        response_200_dict = json.loads(r'[{"url":"https://OLpu.dtfmcuhkZO-euv+B6sOSHXAKZD5w","id":"Lorem","name":"ex dolore","scopes":["cupidatat","adipisicing ullamco proident sit tempor","anim ea fugiat enim quis"]},{"url":"http://QdzMFHAKUsxWSQmrfDLkqRlEJjZgQTzU.rjawur.KCW3oxYYuZNNphMnsZEF1zt1dgotHDgzlSHt7","id":"id nostrud amet","name":"occaecat qui cupidatat adipisicing","scopes":["cillum","nostrud ullamco in","tempor dolore culpa magna","proident et incididunt commodo in"]},{"url":"http://dyrMl.wkddWUkV0XNW8kC1V,YrjKS-j0ik2YLwXJm3nuJ30u9wexTRmdmczFG3-V3+","id":"aute sunt proident","name":"deserunt mollit","scopes":["nisi quis consectetur fugiat amet","officia commodo aliqua eiusmod","occaecat do mollit","ex in","tempor labore ut"]},{"url":"http://djtIqVvqHAiXJLDTRs.ysgueOHWIsSu6L5JukDjKjap8CaRkt.BSoqRr","id":"aute commodo consectetur","name":"cupidatat exercitation sed laborum","scopes":["incididunt laboris","id sed dolore","veniam","culpa"]},{"url":"https://tFjmRLNMKusuxdQ.vqtfHoBz0+2qM+mj1dapXXaHFguVGvQ3uhj-zAUGYvgQssJi6Iagh","id":"et veniam laborum","name":"qui sed dolor quis est","scopes":["consequat irure","in quis ex","Excepteur anim","ullamco incididunt exercitation"]}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_roles(url=full_url, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
@@ -1680,41 +1680,41 @@
 
 @pytest.mark.asyncio
 async def test_create_role(aioresponses: aioresponses):
     url = r'/roles'
     url_variant = r'roles'
     full_url = BASE_URL+r'/roles'
 
-    request = json.loads(r'{"name":"nulla nisi","scopes":["in amet et in","cupidatat","adipisicing ad","dolore aliqua in","Ut esse ad"]}')
+    request = json.loads(r'{"url":"https://MEkpuxWXRyvKeCRFNPq.ewLyKpgX5VSi,unNtR8pGDhqelhVAcN","id":"mollit Duis sed veniam consectetur","name":"velit aliqua incididunt","scopes":["velit consectetur","aliquip Excepteur magna sed","commodo proident Ut","est dolor ad"]}')
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
-        response_201_dict = json.loads(r'{"scopes":["dolor commodo id in","ut"],"name":"commodo ad nulla nisi et"}')
+        response_201_dict = json.loads(r'{"url":"https://MEkpuxWXRyvKeCRFNPq.ewLyKpgX5VSi,unNtR8pGDhqelhVAcN","id":"mollit Duis sed veniam consectetur","name":"velit aliqua incididunt","scopes":["velit consectetur","aliquip Excepteur magna sed","commodo proident Ut","est dolor ad"]}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_role(body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
-        response_201_dict = json.loads(r'{"scopes":["dolor commodo id in","ut"],"name":"commodo ad nulla nisi et"}')
+        response_201_dict = json.loads(r'{"url":"https://MEkpuxWXRyvKeCRFNPq.ewLyKpgX5VSi,unNtR8pGDhqelhVAcN","id":"mollit Duis sed veniam consectetur","name":"velit aliqua incididunt","scopes":["velit consectetur","aliquip Excepteur magna sed","commodo proident Ut","est dolor ad"]}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_role(url=url, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
-        response_201_dict = json.loads(r'{"scopes":["dolor commodo id in","ut"],"name":"commodo ad nulla nisi et"}')
+        response_201_dict = json.loads(r'{"url":"https://MEkpuxWXRyvKeCRFNPq.ewLyKpgX5VSi,unNtR8pGDhqelhVAcN","id":"mollit Duis sed veniam consectetur","name":"velit aliqua incididunt","scopes":["velit consectetur","aliquip Excepteur magna sed","commodo proident Ut","est dolor ad"]}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_role(url=url_variant, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
-        response_201_dict = json.loads(r'{"scopes":["dolor commodo id in","ut"],"name":"commodo ad nulla nisi et"}')
+        response_201_dict = json.loads(r'{"url":"https://MEkpuxWXRyvKeCRFNPq.ewLyKpgX5VSi,unNtR8pGDhqelhVAcN","id":"mollit Duis sed veniam consectetur","name":"velit aliqua incididunt","scopes":["velit consectetur","aliquip Excepteur magna sed","commodo proident Ut","est dolor ad"]}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_role(url=full_url, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
@@ -1842,29 +1842,29 @@
     url = r'/roles/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     url_variant = r'roles/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     full_url = BASE_URL+r'/roles/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"scopes":["dolor commodo id in","ut"],"name":"commodo ad nulla nisi et"}')
+        response_200_dict = json.loads(r'{"url":"https://MEkpuxWXRyvKeCRFNPq.ewLyKpgX5VSi,unNtR8pGDhqelhVAcN","id":"mollit Duis sed veniam consectetur","name":"velit aliqua incididunt","scopes":["velit consectetur","aliquip Excepteur magna sed","commodo proident Ut","est dolor ad"]}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_role(url=url, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"scopes":["dolor commodo id in","ut"],"name":"commodo ad nulla nisi et"}')
+        response_200_dict = json.loads(r'{"url":"https://MEkpuxWXRyvKeCRFNPq.ewLyKpgX5VSi,unNtR8pGDhqelhVAcN","id":"mollit Duis sed veniam consectetur","name":"velit aliqua incididunt","scopes":["velit consectetur","aliquip Excepteur magna sed","commodo proident Ut","est dolor ad"]}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_role(url=url_variant, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"scopes":["dolor commodo id in","ut"],"name":"commodo ad nulla nisi et"}')
+        response_200_dict = json.loads(r'{"url":"https://MEkpuxWXRyvKeCRFNPq.ewLyKpgX5VSi,unNtR8pGDhqelhVAcN","id":"mollit Duis sed veniam consectetur","name":"velit aliqua incididunt","scopes":["velit consectetur","aliquip Excepteur magna sed","commodo proident Ut","est dolor ad"]}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_role(url=full_url, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
@@ -1959,34 +1959,34 @@
 
 @pytest.mark.asyncio
 async def test_update_role(aioresponses: aioresponses):
     url = r'/roles/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     url_variant = r'roles/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     full_url = BASE_URL+r'/roles/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
 
-    request = json.loads(r'{"scopes":["dolor commodo id in","ut"],"name":"commodo ad nulla nisi et"}')
+    request = json.loads(r'{"url":"https://MEkpuxWXRyvKeCRFNPq.ewLyKpgX5VSi,unNtR8pGDhqelhVAcN","id":"mollit Duis sed veniam consectetur","name":"velit aliqua incididunt","scopes":["velit consectetur","aliquip Excepteur magna sed","commodo proident Ut","est dolor ad"]}')
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"scopes":["dolor commodo id in","ut"],"name":"commodo ad nulla nisi et"}')
+        response_200_dict = json.loads(r'{"url":"https://MEkpuxWXRyvKeCRFNPq.ewLyKpgX5VSi,unNtR8pGDhqelhVAcN","id":"mollit Duis sed veniam consectetur","name":"velit aliqua incididunt","scopes":["velit consectetur","aliquip Excepteur magna sed","commodo proident Ut","est dolor ad"]}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_role(url=url, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"scopes":["dolor commodo id in","ut"],"name":"commodo ad nulla nisi et"}')
+        response_200_dict = json.loads(r'{"url":"https://MEkpuxWXRyvKeCRFNPq.ewLyKpgX5VSi,unNtR8pGDhqelhVAcN","id":"mollit Duis sed veniam consectetur","name":"velit aliqua incididunt","scopes":["velit consectetur","aliquip Excepteur magna sed","commodo proident Ut","est dolor ad"]}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_role(url=url_variant, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"scopes":["dolor commodo id in","ut"],"name":"commodo ad nulla nisi et"}')
+        response_200_dict = json.loads(r'{"url":"https://MEkpuxWXRyvKeCRFNPq.ewLyKpgX5VSi,unNtR8pGDhqelhVAcN","id":"mollit Duis sed veniam consectetur","name":"velit aliqua incididunt","scopes":["velit consectetur","aliquip Excepteur magna sed","commodo proident Ut","est dolor ad"]}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_role(url=full_url, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
@@ -2198,29 +2198,29 @@
     url = r'/roles/c799cc2e-cdc5-4143-973a-6f56a5afa82c/users'
     url_variant = r'roles/c799cc2e-cdc5-4143-973a-6f56a5afa82c/users'
     full_url = BASE_URL+r'/roles/c799cc2e-cdc5-4143-973a-6f56a5afa82c/users'
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"roles":[{"url":"https://DeURFWCx.onpu.Mw7RTfb2f0l1WRLzoCO5oU","id":"enim anim","name":"non incididunt Duis pariatur minim","scopes":["anim voluptate aute Duis"]}],"url":"https://dhvskgVWHiqwVntPoDQGF.ovePGeHEMw62XGwjeRU8wlzpIq5MThVrmqRhgckA-PLHLyY,zw+oQY"},{"roles":[{"url":"http://guBFBXETlaqfTdLLERbYNLLxZfDPO.cpikrn3,,iXCReR4ttNoe-tMnW,hKH1KPFSPED.4dVYJyHO3rzehHFgRkEY5teKM06BwHocOzVHwyg,"}],"password":"elit esse aute","username":"culpa","url":"http://ulxpvZToDIljIFfbjoFuAGBWNAOtS.fqegaiBJIsMZvyhownQK8JUbyjybkXJh,jzugkWn1ynn,-Ns3FAcYzdlQsMoygSVAjcS"},{"username":"proident Ut ad reprehenderit","roles":[{"url":"http://YfHcCjfNllGG.jvkhcj3bIX7FusXR++ln7ptUnTRvS9tw"},{"name":"aliquip ullamco culpa consequat","id":"in adipisicing","url":"https://PSkjL.rbUkxB9XvO+SAZ-s5iURdPqEn88GdVFYDNTUhtH8XsdZNZFuVC"},{"url":"http://vPvLleEDIbPSRvhKNMrErekJWIK.eibvkaeIbOawfCEA4OcE8mDAn8qofAP0Vr3cpaxvhabQWVecNZOqDCz5oJ3","scopes":["veniam non ut","exercitation commodo elit","adipisicing tempor","cupidatat Ut dolor reprehenderit","reprehenderit ut ipsum et cupidatat"],"id":"velit Excepteur occaecat"}],"url":"https://GXYKIhsWipBeJUIcBNukIdJE.hvVmOk85dI5oEflv,EDD+0-eJOa2qdHKltLPwsg9GJbzaQtJhzdVuNw3KucXXHSJzZckeMPFcGv"},{"roles":[{"url":"https://zjihqqLRdlnACjMmxxukpKeC.dovQ0iw-ZmN6q8sTZyw6F0FTZSbziJGvEeIVH1GN0ttobx0vNnfyrpwTmV5TmlGc2KNvdrmx","id":"elit sint non consectetur do","name":"laborum incididunt exercitation","scopes":["fugiat aute eiusmod aliquip","in eu Lorem","voluptate incididunt dolore dolore"]},{"url":"http://fcJDGAMVZZteWEL.lrZBLoqWr,-OhEIp52w5ni6b1KGQTs.B","scopes":["id labore ut voluptate","ex magna deserunt culpa Ut","aliquip","eu adipisicing dolore aliqua reprehenderit","elit enim commodo"]}],"password":"dolore in","id":"Excepteur dolor consectetur cupidatat","url":"https://LsSgDHAqAGEtaRzEMBLYlkq.keaOZMqdQo6mUVs3RF6NaIKRDy45Edaa6bLzykKVsfHjYxnH+qEgP5HsYmgYrYeX4","username":"cupidatat nostrud esse dolore nulla"}]')
+        response_200_dict = json.loads(r'[{"url":"http://SyrjwTQktCePOwvKc.blfpSOA","id":"amet in irure ullamco","username":"proident occaecat","password":"do"},{"url":"https://FZTzXTceuBxxrAqTMCqKPQwFuhRlTkh.ozV,iY4Cq5F6ByZLCcSu8yqfCD","id":"dolor mollit in","username":"do in dolor aliquip anim","password":"adipisicing"},{"url":"http://ShyjZbZHQpYRrA.yqwHM27xmpypXQe.OAYKAUMLLLKDlgGO2MpdZKOinzOJ4Iz.QZxUUB4WRkvFk6O5kNaDA","id":"minim adipisicing consequat nostrud","username":"id ut officia aute","password":"ullamco irure nulla magna"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_users_with_role(url=url, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"roles":[{"url":"https://DeURFWCx.onpu.Mw7RTfb2f0l1WRLzoCO5oU","id":"enim anim","name":"non incididunt Duis pariatur minim","scopes":["anim voluptate aute Duis"]}],"url":"https://dhvskgVWHiqwVntPoDQGF.ovePGeHEMw62XGwjeRU8wlzpIq5MThVrmqRhgckA-PLHLyY,zw+oQY"},{"roles":[{"url":"http://guBFBXETlaqfTdLLERbYNLLxZfDPO.cpikrn3,,iXCReR4ttNoe-tMnW,hKH1KPFSPED.4dVYJyHO3rzehHFgRkEY5teKM06BwHocOzVHwyg,"}],"password":"elit esse aute","username":"culpa","url":"http://ulxpvZToDIljIFfbjoFuAGBWNAOtS.fqegaiBJIsMZvyhownQK8JUbyjybkXJh,jzugkWn1ynn,-Ns3FAcYzdlQsMoygSVAjcS"},{"username":"proident Ut ad reprehenderit","roles":[{"url":"http://YfHcCjfNllGG.jvkhcj3bIX7FusXR++ln7ptUnTRvS9tw"},{"name":"aliquip ullamco culpa consequat","id":"in adipisicing","url":"https://PSkjL.rbUkxB9XvO+SAZ-s5iURdPqEn88GdVFYDNTUhtH8XsdZNZFuVC"},{"url":"http://vPvLleEDIbPSRvhKNMrErekJWIK.eibvkaeIbOawfCEA4OcE8mDAn8qofAP0Vr3cpaxvhabQWVecNZOqDCz5oJ3","scopes":["veniam non ut","exercitation commodo elit","adipisicing tempor","cupidatat Ut dolor reprehenderit","reprehenderit ut ipsum et cupidatat"],"id":"velit Excepteur occaecat"}],"url":"https://GXYKIhsWipBeJUIcBNukIdJE.hvVmOk85dI5oEflv,EDD+0-eJOa2qdHKltLPwsg9GJbzaQtJhzdVuNw3KucXXHSJzZckeMPFcGv"},{"roles":[{"url":"https://zjihqqLRdlnACjMmxxukpKeC.dovQ0iw-ZmN6q8sTZyw6F0FTZSbziJGvEeIVH1GN0ttobx0vNnfyrpwTmV5TmlGc2KNvdrmx","id":"elit sint non consectetur do","name":"laborum incididunt exercitation","scopes":["fugiat aute eiusmod aliquip","in eu Lorem","voluptate incididunt dolore dolore"]},{"url":"http://fcJDGAMVZZteWEL.lrZBLoqWr,-OhEIp52w5ni6b1KGQTs.B","scopes":["id labore ut voluptate","ex magna deserunt culpa Ut","aliquip","eu adipisicing dolore aliqua reprehenderit","elit enim commodo"]}],"password":"dolore in","id":"Excepteur dolor consectetur cupidatat","url":"https://LsSgDHAqAGEtaRzEMBLYlkq.keaOZMqdQo6mUVs3RF6NaIKRDy45Edaa6bLzykKVsfHjYxnH+qEgP5HsYmgYrYeX4","username":"cupidatat nostrud esse dolore nulla"}]')
+        response_200_dict = json.loads(r'[{"url":"http://SyrjwTQktCePOwvKc.blfpSOA","id":"amet in irure ullamco","username":"proident occaecat","password":"do"},{"url":"https://FZTzXTceuBxxrAqTMCqKPQwFuhRlTkh.ozV,iY4Cq5F6ByZLCcSu8yqfCD","id":"dolor mollit in","username":"do in dolor aliquip anim","password":"adipisicing"},{"url":"http://ShyjZbZHQpYRrA.yqwHM27xmpypXQe.OAYKAUMLLLKDlgGO2MpdZKOinzOJ4Iz.QZxUUB4WRkvFk6O5kNaDA","id":"minim adipisicing consequat nostrud","username":"id ut officia aute","password":"ullamco irure nulla magna"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_users_with_role(url=url_variant, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"roles":[{"url":"https://DeURFWCx.onpu.Mw7RTfb2f0l1WRLzoCO5oU","id":"enim anim","name":"non incididunt Duis pariatur minim","scopes":["anim voluptate aute Duis"]}],"url":"https://dhvskgVWHiqwVntPoDQGF.ovePGeHEMw62XGwjeRU8wlzpIq5MThVrmqRhgckA-PLHLyY,zw+oQY"},{"roles":[{"url":"http://guBFBXETlaqfTdLLERbYNLLxZfDPO.cpikrn3,,iXCReR4ttNoe-tMnW,hKH1KPFSPED.4dVYJyHO3rzehHFgRkEY5teKM06BwHocOzVHwyg,"}],"password":"elit esse aute","username":"culpa","url":"http://ulxpvZToDIljIFfbjoFuAGBWNAOtS.fqegaiBJIsMZvyhownQK8JUbyjybkXJh,jzugkWn1ynn,-Ns3FAcYzdlQsMoygSVAjcS"},{"username":"proident Ut ad reprehenderit","roles":[{"url":"http://YfHcCjfNllGG.jvkhcj3bIX7FusXR++ln7ptUnTRvS9tw"},{"name":"aliquip ullamco culpa consequat","id":"in adipisicing","url":"https://PSkjL.rbUkxB9XvO+SAZ-s5iURdPqEn88GdVFYDNTUhtH8XsdZNZFuVC"},{"url":"http://vPvLleEDIbPSRvhKNMrErekJWIK.eibvkaeIbOawfCEA4OcE8mDAn8qofAP0Vr3cpaxvhabQWVecNZOqDCz5oJ3","scopes":["veniam non ut","exercitation commodo elit","adipisicing tempor","cupidatat Ut dolor reprehenderit","reprehenderit ut ipsum et cupidatat"],"id":"velit Excepteur occaecat"}],"url":"https://GXYKIhsWipBeJUIcBNukIdJE.hvVmOk85dI5oEflv,EDD+0-eJOa2qdHKltLPwsg9GJbzaQtJhzdVuNw3KucXXHSJzZckeMPFcGv"},{"roles":[{"url":"https://zjihqqLRdlnACjMmxxukpKeC.dovQ0iw-ZmN6q8sTZyw6F0FTZSbziJGvEeIVH1GN0ttobx0vNnfyrpwTmV5TmlGc2KNvdrmx","id":"elit sint non consectetur do","name":"laborum incididunt exercitation","scopes":["fugiat aute eiusmod aliquip","in eu Lorem","voluptate incididunt dolore dolore"]},{"url":"http://fcJDGAMVZZteWEL.lrZBLoqWr,-OhEIp52w5ni6b1KGQTs.B","scopes":["id labore ut voluptate","ex magna deserunt culpa Ut","aliquip","eu adipisicing dolore aliqua reprehenderit","elit enim commodo"]}],"password":"dolore in","id":"Excepteur dolor consectetur cupidatat","url":"https://LsSgDHAqAGEtaRzEMBLYlkq.keaOZMqdQo6mUVs3RF6NaIKRDy45Edaa6bLzykKVsfHjYxnH+qEgP5HsYmgYrYeX4","username":"cupidatat nostrud esse dolore nulla"}]')
+        response_200_dict = json.loads(r'[{"url":"http://SyrjwTQktCePOwvKc.blfpSOA","id":"amet in irure ullamco","username":"proident occaecat","password":"do"},{"url":"https://FZTzXTceuBxxrAqTMCqKPQwFuhRlTkh.ozV,iY4Cq5F6ByZLCcSu8yqfCD","id":"dolor mollit in","username":"do in dolor aliquip anim","password":"adipisicing"},{"url":"http://ShyjZbZHQpYRrA.yqwHM27xmpypXQe.OAYKAUMLLLKDlgGO2MpdZKOinzOJ4Iz.QZxUUB4WRkvFk6O5kNaDA","id":"minim adipisicing consequat nostrud","username":"id ut officia aute","password":"ullamco irure nulla magna"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_users_with_role(url=full_url, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
@@ -2550,36 +2550,36 @@
     url = r'/identity'
     url_variant = r'identity'
     full_url = BASE_URL+r'/identity'
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
+        response_200_dict = json.loads(r'{"url":"https://FBpFkjeMvxKCcBpxVjYLeOQ.jmhVgh-F,O,iQ6yI+,lfJZ9fx7cG5,1eX.UCVrA.QH+YJ","id":"adipisicing labore Duis aliquip consectetur","username":"irure ullamco reprehenderit cillum et","password":"ea eiusmod consequat commodo"}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_identity(**parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
+        response_200_dict = json.loads(r'{"url":"https://FBpFkjeMvxKCcBpxVjYLeOQ.jmhVgh-F,O,iQ6yI+,lfJZ9fx7cG5,1eX.UCVrA.QH+YJ","id":"adipisicing labore Duis aliquip consectetur","username":"irure ullamco reprehenderit cillum et","password":"ea eiusmod consequat commodo"}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_identity(url=url, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
+        response_200_dict = json.loads(r'{"url":"https://FBpFkjeMvxKCcBpxVjYLeOQ.jmhVgh-F,O,iQ6yI+,lfJZ9fx7cG5,1eX.UCVrA.QH+YJ","id":"adipisicing labore Duis aliquip consectetur","username":"irure ullamco reprehenderit cillum et","password":"ea eiusmod consequat commodo"}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_identity(url=url_variant, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
+        response_200_dict = json.loads(r'{"url":"https://FBpFkjeMvxKCcBpxVjYLeOQ.jmhVgh-F,O,iQ6yI+,lfJZ9fx7cG5,1eX.UCVrA.QH+YJ","id":"adipisicing labore Duis aliquip consectetur","username":"irure ullamco reprehenderit cillum et","password":"ea eiusmod consequat commodo"}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_identity(url=full_url, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
@@ -2704,41 +2704,41 @@
 
 @pytest.mark.asyncio
 async def test_update_identity(aioresponses: aioresponses):
     url = r'/identity'
     url_variant = r'identity'
     full_url = BASE_URL+r'/identity'
 
-    request = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
+    request = json.loads(r'{"username":"tempor","password":"ad"}')
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
+        response_200_dict = json.loads(r'{"url":"https://FBpFkjeMvxKCcBpxVjYLeOQ.jmhVgh-F,O,iQ6yI+,lfJZ9fx7cG5,1eX.UCVrA.QH+YJ","id":"adipisicing labore Duis aliquip consectetur","username":"irure ullamco reprehenderit cillum et","password":"ea eiusmod consequat commodo"}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_identity(body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
+        response_200_dict = json.loads(r'{"url":"https://FBpFkjeMvxKCcBpxVjYLeOQ.jmhVgh-F,O,iQ6yI+,lfJZ9fx7cG5,1eX.UCVrA.QH+YJ","id":"adipisicing labore Duis aliquip consectetur","username":"irure ullamco reprehenderit cillum et","password":"ea eiusmod consequat commodo"}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_identity(url=url, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
+        response_200_dict = json.loads(r'{"url":"https://FBpFkjeMvxKCcBpxVjYLeOQ.jmhVgh-F,O,iQ6yI+,lfJZ9fx7cG5,1eX.UCVrA.QH+YJ","id":"adipisicing labore Duis aliquip consectetur","username":"irure ullamco reprehenderit cillum et","password":"ea eiusmod consequat commodo"}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_identity(url=url_variant, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
+        response_200_dict = json.loads(r'{"url":"https://FBpFkjeMvxKCcBpxVjYLeOQ.jmhVgh-F,O,iQ6yI+,lfJZ9fx7cG5,1eX.UCVrA.QH+YJ","id":"adipisicing labore Duis aliquip consectetur","username":"irure ullamco reprehenderit cillum et","password":"ea eiusmod consequat commodo"}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_identity(url=full_url, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
@@ -2858,14 +2858,165 @@
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.update_identity(url=full_url, body=request, **parameters)
 
 
 @pytest.mark.asyncio
+async def test_register(aioresponses: aioresponses):
+    url = r'/register'
+    url_variant = r'register'
+    full_url = BASE_URL+r'/register'
+
+    request = json.loads(r'{"username":"cillum ullamco esse in pariatur","password":"id ut velit culpa Duis"}')
+
+    parameter_list = [{}, ]
+
+    for parameters in parameter_list:
+        aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201)
+        async with APIClient(BASE_URL) as client:
+            resp = await client.register(body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201)
+        async with APIClient(BASE_URL) as client:
+            resp = await client.register(url=url, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201)
+        async with APIClient(BASE_URL) as client:
+            resp = await client.register(url=url_variant, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201)
+        async with APIClient(BASE_URL) as client:
+            resp = await client.register(url=full_url, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.register(body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.register(url=url, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.register(url=url_variant, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.register(url=full_url, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.register(body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.register(url=url, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.register(url=url_variant, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.register(url=full_url, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.register(body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.register(url=url, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.register(url=url_variant, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.register(url=full_url, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.register(body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.register(url=url, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.register(url=url_variant, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.register(url=full_url, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.register(body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.register(url=url, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.register(url=url_variant, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.register(url=full_url, body=request, **parameters)
+
+
+@pytest.mark.asyncio
 async def test_get_schedule(aioresponses: aioresponses):
     url = r'/schedule'
     url_variant = r'schedule'
     full_url = BASE_URL+r'/schedule'
 
     request = json.loads(r'{"Experiment":{"Devices":[{"ID":"https://cHaylvBKdWJSNBxjFMsRIFtEoQDGDi.kucakbCJEWoYBT7b+w9mFqQ"}],"Description":"veniam dolore elit incididunt aliquip"},"Time":{"Start":"2013-01-14T23:45:15.0Z","End":"2009-06-17T21:25:10.0Z"},"Combined":true,"onlyOwn":true}')
 
@@ -3826,36 +3977,36 @@
     url = r'/devices'
     url_variant = r'devices'
     full_url = BASE_URL+r'/devices'
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"description":"occaecat ut non anim","owner":"http://XtyFMjWKLqVNOjoFVOCibGChfLnTd.elheA5xrKYP,KYInBcyGXAo7fWTRAFLv-I66+UEa11nOnUW,yrp7vU8tJDvqx-FBcm","url":"https://gUzGKHPeV.xtseja4ThHmONE6IMx"},{"description":"officia nisi ut","name":"ad amet dolore Duis","url":"https://xuSaiEaHtcvtcAzTVACnzItZUP.dpbsi.4CSbCelm2XPG6GJifZP5BwV","type":"cloud instantiable","owner":"http://knWGbtFvjEZogFuZq.jnbimyOtjLoxNnW04vVg+28XxLvtiBbTVsIXxMSxfV-cnpmwROVBavvKOxqv7Q"},{"description":"amet eu labore","url":"https://wrEF.iaf.vje-57RTm9JYGspOOJfsTdt0qLvKg914AbmBdlJfKZA4BFoJ","name":"sint cupidatat ipsum pariatur dolore","type":"device","owner":"http://NOdjkLvvuy.fihbxtyikUqV-5dwSkcBP+E4deORAAG2KGBsiq"}]')
+        response_200_dict = json.loads(r'[{"url":"https://CBBZavgAmnNDP.cozaaKD+VaFn-J2Ta4Dp9BeG8","type":"edge instantiable","name":"non velit minim dolore","owner":"https://RUz.umOAmQVVxIGHaSFxPN7ZkMCyH20hZFJ2xhFFyvqhjswohpHuSKDsWRPbLDobXP"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_devices(**parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"description":"occaecat ut non anim","owner":"http://XtyFMjWKLqVNOjoFVOCibGChfLnTd.elheA5xrKYP,KYInBcyGXAo7fWTRAFLv-I66+UEa11nOnUW,yrp7vU8tJDvqx-FBcm","url":"https://gUzGKHPeV.xtseja4ThHmONE6IMx"},{"description":"officia nisi ut","name":"ad amet dolore Duis","url":"https://xuSaiEaHtcvtcAzTVACnzItZUP.dpbsi.4CSbCelm2XPG6GJifZP5BwV","type":"cloud instantiable","owner":"http://knWGbtFvjEZogFuZq.jnbimyOtjLoxNnW04vVg+28XxLvtiBbTVsIXxMSxfV-cnpmwROVBavvKOxqv7Q"},{"description":"amet eu labore","url":"https://wrEF.iaf.vje-57RTm9JYGspOOJfsTdt0qLvKg914AbmBdlJfKZA4BFoJ","name":"sint cupidatat ipsum pariatur dolore","type":"device","owner":"http://NOdjkLvvuy.fihbxtyikUqV-5dwSkcBP+E4deORAAG2KGBsiq"}]')
+        response_200_dict = json.loads(r'[{"url":"https://CBBZavgAmnNDP.cozaaKD+VaFn-J2Ta4Dp9BeG8","type":"edge instantiable","name":"non velit minim dolore","owner":"https://RUz.umOAmQVVxIGHaSFxPN7ZkMCyH20hZFJ2xhFFyvqhjswohpHuSKDsWRPbLDobXP"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_devices(url=url, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"description":"occaecat ut non anim","owner":"http://XtyFMjWKLqVNOjoFVOCibGChfLnTd.elheA5xrKYP,KYInBcyGXAo7fWTRAFLv-I66+UEa11nOnUW,yrp7vU8tJDvqx-FBcm","url":"https://gUzGKHPeV.xtseja4ThHmONE6IMx"},{"description":"officia nisi ut","name":"ad amet dolore Duis","url":"https://xuSaiEaHtcvtcAzTVACnzItZUP.dpbsi.4CSbCelm2XPG6GJifZP5BwV","type":"cloud instantiable","owner":"http://knWGbtFvjEZogFuZq.jnbimyOtjLoxNnW04vVg+28XxLvtiBbTVsIXxMSxfV-cnpmwROVBavvKOxqv7Q"},{"description":"amet eu labore","url":"https://wrEF.iaf.vje-57RTm9JYGspOOJfsTdt0qLvKg914AbmBdlJfKZA4BFoJ","name":"sint cupidatat ipsum pariatur dolore","type":"device","owner":"http://NOdjkLvvuy.fihbxtyikUqV-5dwSkcBP+E4deORAAG2KGBsiq"}]')
+        response_200_dict = json.loads(r'[{"url":"https://CBBZavgAmnNDP.cozaaKD+VaFn-J2Ta4Dp9BeG8","type":"edge instantiable","name":"non velit minim dolore","owner":"https://RUz.umOAmQVVxIGHaSFxPN7ZkMCyH20hZFJ2xhFFyvqhjswohpHuSKDsWRPbLDobXP"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_devices(url=url_variant, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"description":"occaecat ut non anim","owner":"http://XtyFMjWKLqVNOjoFVOCibGChfLnTd.elheA5xrKYP,KYInBcyGXAo7fWTRAFLv-I66+UEa11nOnUW,yrp7vU8tJDvqx-FBcm","url":"https://gUzGKHPeV.xtseja4ThHmONE6IMx"},{"description":"officia nisi ut","name":"ad amet dolore Duis","url":"https://xuSaiEaHtcvtcAzTVACnzItZUP.dpbsi.4CSbCelm2XPG6GJifZP5BwV","type":"cloud instantiable","owner":"http://knWGbtFvjEZogFuZq.jnbimyOtjLoxNnW04vVg+28XxLvtiBbTVsIXxMSxfV-cnpmwROVBavvKOxqv7Q"},{"description":"amet eu labore","url":"https://wrEF.iaf.vje-57RTm9JYGspOOJfsTdt0qLvKg914AbmBdlJfKZA4BFoJ","name":"sint cupidatat ipsum pariatur dolore","type":"device","owner":"http://NOdjkLvvuy.fihbxtyikUqV-5dwSkcBP+E4deORAAG2KGBsiq"}]')
+        response_200_dict = json.loads(r'[{"url":"https://CBBZavgAmnNDP.cozaaKD+VaFn-J2Ta4Dp9BeG8","type":"edge instantiable","name":"non velit minim dolore","owner":"https://RUz.umOAmQVVxIGHaSFxPN7ZkMCyH20hZFJ2xhFFyvqhjswohpHuSKDsWRPbLDobXP"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_devices(url=full_url, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
@@ -3980,41 +4131,41 @@
 
 @pytest.mark.asyncio
 async def test_create_device(aioresponses: aioresponses):
     url = r'/devices'
     url_variant = r'devices'
     full_url = BASE_URL+r'/devices'
 
-    request = json.loads(r'{"services":[],"url":"https://FFtBZqePJevWvqANceH.erzuirQaTbcwUTzpisvYDrbm0JMrsFw.-U1iS5kUOo","type":"device","connected":true,"owner":"https://mDCjpDPqCPPtDeHBrJuRtfOZdAkcLQgiM.kjDA0FCmSOocI6lV.q9RAXULVivUlme.Yb+A5VglKZF9jsM33IUv5MmtYkt4tbqo7-gGC4","description":"consequat id commodo","name":"amet Duis eiusmod dolor deserunt","experiment":"https://yZjFsGlZmXSOaJmchy.ezuSwTSEZ9RaYnbjr-R86Gm5bddW7BbgjWvaia3qfQMtJd,JFhTVyi7xYNvwoq.FegAtFIqvVB","announcedAvailability":[{"repeat":{"frequency":"DAILY","until":"1996-05-09T01:35:51.0Z"}}]}')
+    request = json.loads(r'{"url":"https://rKemGKMlhNcfBAeYBDdlNW.ieM9N.ZnfxWisMIs34TWLplCB-AYjE6sICZDnfHOU1at","type":"group","name":"proident in anim aute veniam","owner":"https://HeFvjzydnbDafLWsZ.ixrN4oC-Om8TxgI0e.UVQRAyQNqrmskvLXxQSwdSjMZxmIrHvBPiS307XfTFjCY4..V.NUWa","devices":[{"url":"http://EERXg.nkpheF89-oujBOjoCcKDypbFgx0i"},{"url":"http://fdUnFNwDkNezzoCuEPhlYWOEvUdg.rhvBAUIwDQHkbofP-+BcBFqXBdlYPoNVsh,fx4"},{"url":"https://rY.hhvlVeTbT7OW,x1xiuZKPifCtJtDRbd4VNKiO3vRRWzabEtMoO"},{"url":"https://JXERGYXtciXGYWUmSxLRqwnekbIe.pdrQmp3KnpoCaCEYnMowadp7L9pb6m3slUHiiyUGjJY-aE5oeJyEY1m3V3"}],"description":"sint sit"}')
 
     parameter_list = [{"changedUrl": "test_string", }, {}, ]
 
     for parameters in parameter_list:
-        response_201_dict = json.loads(r'{"type":"device","owner":"http://wrvuppqewWdH.omhcAwZEk9qD7opUiXkFBrRItQoqFDF7XVlUNBNhMuyCMYhjfpg7qrt-Fj5hqnNkDvd8tzmY60V61j","url":"http://uFaodEpKyQkGvFI.gotilvYR.udrlbOB-hlPogvYKzKk","description":"fugiat eiusmod","name":"aute consequat veniam","services":[],"experiment":"http://RdmTyMiQYSUxtCuahvebSpQ.enR73CD5qG","connected":false}')
+        response_201_dict = json.loads(r'{"url":"https://rKemGKMlhNcfBAeYBDdlNW.ieM9N.ZnfxWisMIs34TWLplCB-AYjE6sICZDnfHOU1at","type":"group","name":"proident in anim aute veniam","owner":"https://HeFvjzydnbDafLWsZ.ixrN4oC-Om8TxgI0e.UVQRAyQNqrmskvLXxQSwdSjMZxmIrHvBPiS307XfTFjCY4..V.NUWa","devices":[{"url":"http://EERXg.nkpheF89-oujBOjoCcKDypbFgx0i"},{"url":"http://fdUnFNwDkNezzoCuEPhlYWOEvUdg.rhvBAUIwDQHkbofP-+BcBFqXBdlYPoNVsh,fx4"},{"url":"https://rY.hhvlVeTbT7OW,x1xiuZKPifCtJtDRbd4VNKiO3vRRWzabEtMoO"},{"url":"https://JXERGYXtciXGYWUmSxLRqwnekbIe.pdrQmp3KnpoCaCEYnMowadp7L9pb6m3slUHiiyUGjJY-aE5oeJyEY1m3V3"}],"description":"sint sit"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_device(body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
-        response_201_dict = json.loads(r'{"type":"device","owner":"http://wrvuppqewWdH.omhcAwZEk9qD7opUiXkFBrRItQoqFDF7XVlUNBNhMuyCMYhjfpg7qrt-Fj5hqnNkDvd8tzmY60V61j","url":"http://uFaodEpKyQkGvFI.gotilvYR.udrlbOB-hlPogvYKzKk","description":"fugiat eiusmod","name":"aute consequat veniam","services":[],"experiment":"http://RdmTyMiQYSUxtCuahvebSpQ.enR73CD5qG","connected":false}')
+        response_201_dict = json.loads(r'{"url":"https://rKemGKMlhNcfBAeYBDdlNW.ieM9N.ZnfxWisMIs34TWLplCB-AYjE6sICZDnfHOU1at","type":"group","name":"proident in anim aute veniam","owner":"https://HeFvjzydnbDafLWsZ.ixrN4oC-Om8TxgI0e.UVQRAyQNqrmskvLXxQSwdSjMZxmIrHvBPiS307XfTFjCY4..V.NUWa","devices":[{"url":"http://EERXg.nkpheF89-oujBOjoCcKDypbFgx0i"},{"url":"http://fdUnFNwDkNezzoCuEPhlYWOEvUdg.rhvBAUIwDQHkbofP-+BcBFqXBdlYPoNVsh,fx4"},{"url":"https://rY.hhvlVeTbT7OW,x1xiuZKPifCtJtDRbd4VNKiO3vRRWzabEtMoO"},{"url":"https://JXERGYXtciXGYWUmSxLRqwnekbIe.pdrQmp3KnpoCaCEYnMowadp7L9pb6m3slUHiiyUGjJY-aE5oeJyEY1m3V3"}],"description":"sint sit"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_device(url=url, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
-        response_201_dict = json.loads(r'{"type":"device","owner":"http://wrvuppqewWdH.omhcAwZEk9qD7opUiXkFBrRItQoqFDF7XVlUNBNhMuyCMYhjfpg7qrt-Fj5hqnNkDvd8tzmY60V61j","url":"http://uFaodEpKyQkGvFI.gotilvYR.udrlbOB-hlPogvYKzKk","description":"fugiat eiusmod","name":"aute consequat veniam","services":[],"experiment":"http://RdmTyMiQYSUxtCuahvebSpQ.enR73CD5qG","connected":false}')
+        response_201_dict = json.loads(r'{"url":"https://rKemGKMlhNcfBAeYBDdlNW.ieM9N.ZnfxWisMIs34TWLplCB-AYjE6sICZDnfHOU1at","type":"group","name":"proident in anim aute veniam","owner":"https://HeFvjzydnbDafLWsZ.ixrN4oC-Om8TxgI0e.UVQRAyQNqrmskvLXxQSwdSjMZxmIrHvBPiS307XfTFjCY4..V.NUWa","devices":[{"url":"http://EERXg.nkpheF89-oujBOjoCcKDypbFgx0i"},{"url":"http://fdUnFNwDkNezzoCuEPhlYWOEvUdg.rhvBAUIwDQHkbofP-+BcBFqXBdlYPoNVsh,fx4"},{"url":"https://rY.hhvlVeTbT7OW,x1xiuZKPifCtJtDRbd4VNKiO3vRRWzabEtMoO"},{"url":"https://JXERGYXtciXGYWUmSxLRqwnekbIe.pdrQmp3KnpoCaCEYnMowadp7L9pb6m3slUHiiyUGjJY-aE5oeJyEY1m3V3"}],"description":"sint sit"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_device(url=url_variant, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
-        response_201_dict = json.loads(r'{"type":"device","owner":"http://wrvuppqewWdH.omhcAwZEk9qD7opUiXkFBrRItQoqFDF7XVlUNBNhMuyCMYhjfpg7qrt-Fj5hqnNkDvd8tzmY60V61j","url":"http://uFaodEpKyQkGvFI.gotilvYR.udrlbOB-hlPogvYKzKk","description":"fugiat eiusmod","name":"aute consequat veniam","services":[],"experiment":"http://RdmTyMiQYSUxtCuahvebSpQ.enR73CD5qG","connected":false}')
+        response_201_dict = json.loads(r'{"url":"https://rKemGKMlhNcfBAeYBDdlNW.ieM9N.ZnfxWisMIs34TWLplCB-AYjE6sICZDnfHOU1at","type":"group","name":"proident in anim aute veniam","owner":"https://HeFvjzydnbDafLWsZ.ixrN4oC-Om8TxgI0e.UVQRAyQNqrmskvLXxQSwdSjMZxmIrHvBPiS307XfTFjCY4..V.NUWa","devices":[{"url":"http://EERXg.nkpheF89-oujBOjoCcKDypbFgx0i"},{"url":"http://fdUnFNwDkNezzoCuEPhlYWOEvUdg.rhvBAUIwDQHkbofP-+BcBFqXBdlYPoNVsh,fx4"},{"url":"https://rY.hhvlVeTbT7OW,x1xiuZKPifCtJtDRbd4VNKiO3vRRWzabEtMoO"},{"url":"https://JXERGYXtciXGYWUmSxLRqwnekbIe.pdrQmp3KnpoCaCEYnMowadp7L9pb6m3slUHiiyUGjJY-aE5oeJyEY1m3V3"}],"description":"sint sit"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_device(url=full_url, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
@@ -4142,29 +4293,29 @@
     url = r'/devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     url_variant = r'devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     full_url = BASE_URL+r'/devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
 
     parameter_list = [{"flat_group": True, }, {}, ]
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"type":"device","owner":"http://wrvuppqewWdH.omhcAwZEk9qD7opUiXkFBrRItQoqFDF7XVlUNBNhMuyCMYhjfpg7qrt-Fj5hqnNkDvd8tzmY60V61j","url":"http://uFaodEpKyQkGvFI.gotilvYR.udrlbOB-hlPogvYKzKk","description":"fugiat eiusmod","name":"aute consequat veniam","services":[],"experiment":"http://RdmTyMiQYSUxtCuahvebSpQ.enR73CD5qG","connected":false}')
+        response_200_dict = json.loads(r'{"url":"https://rKemGKMlhNcfBAeYBDdlNW.ieM9N.ZnfxWisMIs34TWLplCB-AYjE6sICZDnfHOU1at","type":"group","name":"proident in anim aute veniam","owner":"https://HeFvjzydnbDafLWsZ.ixrN4oC-Om8TxgI0e.UVQRAyQNqrmskvLXxQSwdSjMZxmIrHvBPiS307XfTFjCY4..V.NUWa","devices":[{"url":"http://EERXg.nkpheF89-oujBOjoCcKDypbFgx0i"},{"url":"http://fdUnFNwDkNezzoCuEPhlYWOEvUdg.rhvBAUIwDQHkbofP-+BcBFqXBdlYPoNVsh,fx4"},{"url":"https://rY.hhvlVeTbT7OW,x1xiuZKPifCtJtDRbd4VNKiO3vRRWzabEtMoO"},{"url":"https://JXERGYXtciXGYWUmSxLRqwnekbIe.pdrQmp3KnpoCaCEYnMowadp7L9pb6m3slUHiiyUGjJY-aE5oeJyEY1m3V3"}],"description":"sint sit"}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_device(url=url, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"type":"device","owner":"http://wrvuppqewWdH.omhcAwZEk9qD7opUiXkFBrRItQoqFDF7XVlUNBNhMuyCMYhjfpg7qrt-Fj5hqnNkDvd8tzmY60V61j","url":"http://uFaodEpKyQkGvFI.gotilvYR.udrlbOB-hlPogvYKzKk","description":"fugiat eiusmod","name":"aute consequat veniam","services":[],"experiment":"http://RdmTyMiQYSUxtCuahvebSpQ.enR73CD5qG","connected":false}')
+        response_200_dict = json.loads(r'{"url":"https://rKemGKMlhNcfBAeYBDdlNW.ieM9N.ZnfxWisMIs34TWLplCB-AYjE6sICZDnfHOU1at","type":"group","name":"proident in anim aute veniam","owner":"https://HeFvjzydnbDafLWsZ.ixrN4oC-Om8TxgI0e.UVQRAyQNqrmskvLXxQSwdSjMZxmIrHvBPiS307XfTFjCY4..V.NUWa","devices":[{"url":"http://EERXg.nkpheF89-oujBOjoCcKDypbFgx0i"},{"url":"http://fdUnFNwDkNezzoCuEPhlYWOEvUdg.rhvBAUIwDQHkbofP-+BcBFqXBdlYPoNVsh,fx4"},{"url":"https://rY.hhvlVeTbT7OW,x1xiuZKPifCtJtDRbd4VNKiO3vRRWzabEtMoO"},{"url":"https://JXERGYXtciXGYWUmSxLRqwnekbIe.pdrQmp3KnpoCaCEYnMowadp7L9pb6m3slUHiiyUGjJY-aE5oeJyEY1m3V3"}],"description":"sint sit"}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_device(url=url_variant, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"type":"device","owner":"http://wrvuppqewWdH.omhcAwZEk9qD7opUiXkFBrRItQoqFDF7XVlUNBNhMuyCMYhjfpg7qrt-Fj5hqnNkDvd8tzmY60V61j","url":"http://uFaodEpKyQkGvFI.gotilvYR.udrlbOB-hlPogvYKzKk","description":"fugiat eiusmod","name":"aute consequat veniam","services":[],"experiment":"http://RdmTyMiQYSUxtCuahvebSpQ.enR73CD5qG","connected":false}')
+        response_200_dict = json.loads(r'{"url":"https://rKemGKMlhNcfBAeYBDdlNW.ieM9N.ZnfxWisMIs34TWLplCB-AYjE6sICZDnfHOU1at","type":"group","name":"proident in anim aute veniam","owner":"https://HeFvjzydnbDafLWsZ.ixrN4oC-Om8TxgI0e.UVQRAyQNqrmskvLXxQSwdSjMZxmIrHvBPiS307XfTFjCY4..V.NUWa","devices":[{"url":"http://EERXg.nkpheF89-oujBOjoCcKDypbFgx0i"},{"url":"http://fdUnFNwDkNezzoCuEPhlYWOEvUdg.rhvBAUIwDQHkbofP-+BcBFqXBdlYPoNVsh,fx4"},{"url":"https://rY.hhvlVeTbT7OW,x1xiuZKPifCtJtDRbd4VNKiO3vRRWzabEtMoO"},{"url":"https://JXERGYXtciXGYWUmSxLRqwnekbIe.pdrQmp3KnpoCaCEYnMowadp7L9pb6m3slUHiiyUGjJY-aE5oeJyEY1m3V3"}],"description":"sint sit"}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_device(url=full_url, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
@@ -4259,34 +4410,34 @@
 
 @pytest.mark.asyncio
 async def test_update_device(aioresponses: aioresponses):
     url = r'/devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     url_variant = r'devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     full_url = BASE_URL+r'/devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
 
-    request = json.loads(r'{"services":[],"url":"https://FFtBZqePJevWvqANceH.erzuirQaTbcwUTzpisvYDrbm0JMrsFw.-U1iS5kUOo","type":"device","connected":true,"owner":"https://mDCjpDPqCPPtDeHBrJuRtfOZdAkcLQgiM.kjDA0FCmSOocI6lV.q9RAXULVivUlme.Yb+A5VglKZF9jsM33IUv5MmtYkt4tbqo7-gGC4","description":"consequat id commodo","name":"amet Duis eiusmod dolor deserunt","experiment":"https://yZjFsGlZmXSOaJmchy.ezuSwTSEZ9RaYnbjr-R86Gm5bddW7BbgjWvaia3qfQMtJd,JFhTVyi7xYNvwoq.FegAtFIqvVB","announcedAvailability":[{"repeat":{"frequency":"DAILY","until":"1996-05-09T01:35:51.0Z"}}]}')
+    request = json.loads(r'{"type":"edge instantiable","name":"sunt occaecat eu aliquip dolor","description":"dolor elit","codeUrl":"https://cG.onvj8"}')
 
     parameter_list = [{"changedUrl": "test_string", }, {}, ]
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"type":"device","owner":"http://wrvuppqewWdH.omhcAwZEk9qD7opUiXkFBrRItQoqFDF7XVlUNBNhMuyCMYhjfpg7qrt-Fj5hqnNkDvd8tzmY60V61j","url":"http://uFaodEpKyQkGvFI.gotilvYR.udrlbOB-hlPogvYKzKk","description":"fugiat eiusmod","name":"aute consequat veniam","services":[],"experiment":"http://RdmTyMiQYSUxtCuahvebSpQ.enR73CD5qG","connected":false}')
+        response_200_dict = json.loads(r'{"url":"https://rKemGKMlhNcfBAeYBDdlNW.ieM9N.ZnfxWisMIs34TWLplCB-AYjE6sICZDnfHOU1at","type":"group","name":"proident in anim aute veniam","owner":"https://HeFvjzydnbDafLWsZ.ixrN4oC-Om8TxgI0e.UVQRAyQNqrmskvLXxQSwdSjMZxmIrHvBPiS307XfTFjCY4..V.NUWa","devices":[{"url":"http://EERXg.nkpheF89-oujBOjoCcKDypbFgx0i"},{"url":"http://fdUnFNwDkNezzoCuEPhlYWOEvUdg.rhvBAUIwDQHkbofP-+BcBFqXBdlYPoNVsh,fx4"},{"url":"https://rY.hhvlVeTbT7OW,x1xiuZKPifCtJtDRbd4VNKiO3vRRWzabEtMoO"},{"url":"https://JXERGYXtciXGYWUmSxLRqwnekbIe.pdrQmp3KnpoCaCEYnMowadp7L9pb6m3slUHiiyUGjJY-aE5oeJyEY1m3V3"}],"description":"sint sit"}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_device(url=url, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"type":"device","owner":"http://wrvuppqewWdH.omhcAwZEk9qD7opUiXkFBrRItQoqFDF7XVlUNBNhMuyCMYhjfpg7qrt-Fj5hqnNkDvd8tzmY60V61j","url":"http://uFaodEpKyQkGvFI.gotilvYR.udrlbOB-hlPogvYKzKk","description":"fugiat eiusmod","name":"aute consequat veniam","services":[],"experiment":"http://RdmTyMiQYSUxtCuahvebSpQ.enR73CD5qG","connected":false}')
+        response_200_dict = json.loads(r'{"url":"https://rKemGKMlhNcfBAeYBDdlNW.ieM9N.ZnfxWisMIs34TWLplCB-AYjE6sICZDnfHOU1at","type":"group","name":"proident in anim aute veniam","owner":"https://HeFvjzydnbDafLWsZ.ixrN4oC-Om8TxgI0e.UVQRAyQNqrmskvLXxQSwdSjMZxmIrHvBPiS307XfTFjCY4..V.NUWa","devices":[{"url":"http://EERXg.nkpheF89-oujBOjoCcKDypbFgx0i"},{"url":"http://fdUnFNwDkNezzoCuEPhlYWOEvUdg.rhvBAUIwDQHkbofP-+BcBFqXBdlYPoNVsh,fx4"},{"url":"https://rY.hhvlVeTbT7OW,x1xiuZKPifCtJtDRbd4VNKiO3vRRWzabEtMoO"},{"url":"https://JXERGYXtciXGYWUmSxLRqwnekbIe.pdrQmp3KnpoCaCEYnMowadp7L9pb6m3slUHiiyUGjJY-aE5oeJyEY1m3V3"}],"description":"sint sit"}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_device(url=url_variant, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"type":"device","owner":"http://wrvuppqewWdH.omhcAwZEk9qD7opUiXkFBrRItQoqFDF7XVlUNBNhMuyCMYhjfpg7qrt-Fj5hqnNkDvd8tzmY60V61j","url":"http://uFaodEpKyQkGvFI.gotilvYR.udrlbOB-hlPogvYKzKk","description":"fugiat eiusmod","name":"aute consequat veniam","services":[],"experiment":"http://RdmTyMiQYSUxtCuahvebSpQ.enR73CD5qG","connected":false}')
+        response_200_dict = json.loads(r'{"url":"https://rKemGKMlhNcfBAeYBDdlNW.ieM9N.ZnfxWisMIs34TWLplCB-AYjE6sICZDnfHOU1at","type":"group","name":"proident in anim aute veniam","owner":"https://HeFvjzydnbDafLWsZ.ixrN4oC-Om8TxgI0e.UVQRAyQNqrmskvLXxQSwdSjMZxmIrHvBPiS307XfTFjCY4..V.NUWa","devices":[{"url":"http://EERXg.nkpheF89-oujBOjoCcKDypbFgx0i"},{"url":"http://fdUnFNwDkNezzoCuEPhlYWOEvUdg.rhvBAUIwDQHkbofP-+BcBFqXBdlYPoNVsh,fx4"},{"url":"https://rY.hhvlVeTbT7OW,x1xiuZKPifCtJtDRbd4VNKiO3vRRWzabEtMoO"},{"url":"https://JXERGYXtciXGYWUmSxLRqwnekbIe.pdrQmp3KnpoCaCEYnMowadp7L9pb6m3slUHiiyUGjJY-aE5oeJyEY1m3V3"}],"description":"sint sit"}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_device(url=full_url, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
@@ -4498,29 +4649,29 @@
     url = r'/devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     url_variant = r'devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     full_url = BASE_URL+r'/devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
 
     parameter_list = [{"changedUrl": "test_string", }, {}, ]
 
     for parameters in parameter_list:
-        response_201_dict = json.loads(r'{"instance":{"announcedAvailability":[{"start":"1955-04-07T01:22:58.0Z","end":"1995-07-10T11:59:14.0Z"},{"end":"2006-05-22T14:58:01.0Z","start":"1956-06-29T18:16:35.0Z"},{"end":"2013-11-28T07:03:49.0Z"},{"end":"2015-04-21T18:19:04.0Z","start":"1975-07-14T08:16:38.0Z"}],"url":"http://uqyLriKDNyKa.qeZcaJtVX9mfvD76xUF+W4nYYFiXhN--1QmKZdxJnnq","services":[],"type":"device","connected":true,"name":"in","owner":"http://XtPxmagFFBylFzvNnkgMTYi.yvmlIqZeAORZPbJktCdGBIj2aFx5zB","description":"nostrud Lorem commodo Excepteur","experiment":"http://ziGqQoyUsaiCVXWUsGq.vgYEjjfQYlaoNU0.TNshwmZX97ESZapPxeXRR6oyHetq"},"deviceToken":"irure eu"}')
+        response_201_dict = json.loads(r'{"instance":{"url":"https://CqYON.xmnuGYeEv6A,Y1Xd","type":"device","name":"fugiat labore Lorem nostrud","owner":"http://qXJqGDlmidYcvasqfsCCA.eljeTAmkIX2L2AzMelvRPbXU2YfsxCWZ,n7TfiEJDoV5cMeYV97+9gjfC","connected":false,"description":"sint","announcedAvailability":[{"end":"1963-07-05T07:30:35.0Z"},{"end":"1944-01-03T21:37:04.0Z","start":"2008-03-20T19:50:34.0Z"},{"end":"1949-11-16T11:53:26.0Z","start":"1959-09-24T01:59:32.0Z"}],"experiment":"https://hSjlrWjjdOTifzKcyxsUt.wnzgp6pqUPFhd9zE6zHT1PW-LHrPsEIuTVAlx-pza8oCKVda","services":[{"serviceType":"http://UlpUhSJkIblJFycFQKfNQ.uytgIvHKxi7VK3RVSvVkGu.8MgKITDwWuLEVTBJkV,4qA7tV6OGerfaUrZw4wcN,o","serviceId":"mollit veniam proident occaecat","serviceDirection":"prosumer"},{"serviceId":"quis ad commodo nostrud dolor","serviceDirection":"prosumer","serviceType":"http://MOaPANKswMkLZU.gayowe-SJNQJJxwE91c"},{"serviceDirection":"prosumer","serviceId":"irure dolor exercitation pariatur consectetur"},{"serviceType":"http://AgJRgzRBfjnukmtIBBFrlUlDU.galiTbGmNW-xMV4pZWb8DrVytQtTCB1cSVCL4n2l-a3OPVNlMJjDnRSf2tBLukDnnhMUGt7M9G","serviceId":"sunt tempor sed ut nulla"},{"serviceDirection":"prosumer","serviceType":"https://KyJelqOfDmRxnJPzuJBtlBq.hobIWQQ1fv9+"}]},"deviceToken":"cillum ullamco"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.instantiate_device(url=url, **parameters)
             assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
-        response_201_dict = json.loads(r'{"instance":{"announcedAvailability":[{"start":"1955-04-07T01:22:58.0Z","end":"1995-07-10T11:59:14.0Z"},{"end":"2006-05-22T14:58:01.0Z","start":"1956-06-29T18:16:35.0Z"},{"end":"2013-11-28T07:03:49.0Z"},{"end":"2015-04-21T18:19:04.0Z","start":"1975-07-14T08:16:38.0Z"}],"url":"http://uqyLriKDNyKa.qeZcaJtVX9mfvD76xUF+W4nYYFiXhN--1QmKZdxJnnq","services":[],"type":"device","connected":true,"name":"in","owner":"http://XtPxmagFFBylFzvNnkgMTYi.yvmlIqZeAORZPbJktCdGBIj2aFx5zB","description":"nostrud Lorem commodo Excepteur","experiment":"http://ziGqQoyUsaiCVXWUsGq.vgYEjjfQYlaoNU0.TNshwmZX97ESZapPxeXRR6oyHetq"},"deviceToken":"irure eu"}')
+        response_201_dict = json.loads(r'{"instance":{"url":"https://CqYON.xmnuGYeEv6A,Y1Xd","type":"device","name":"fugiat labore Lorem nostrud","owner":"http://qXJqGDlmidYcvasqfsCCA.eljeTAmkIX2L2AzMelvRPbXU2YfsxCWZ,n7TfiEJDoV5cMeYV97+9gjfC","connected":false,"description":"sint","announcedAvailability":[{"end":"1963-07-05T07:30:35.0Z"},{"end":"1944-01-03T21:37:04.0Z","start":"2008-03-20T19:50:34.0Z"},{"end":"1949-11-16T11:53:26.0Z","start":"1959-09-24T01:59:32.0Z"}],"experiment":"https://hSjlrWjjdOTifzKcyxsUt.wnzgp6pqUPFhd9zE6zHT1PW-LHrPsEIuTVAlx-pza8oCKVda","services":[{"serviceType":"http://UlpUhSJkIblJFycFQKfNQ.uytgIvHKxi7VK3RVSvVkGu.8MgKITDwWuLEVTBJkV,4qA7tV6OGerfaUrZw4wcN,o","serviceId":"mollit veniam proident occaecat","serviceDirection":"prosumer"},{"serviceId":"quis ad commodo nostrud dolor","serviceDirection":"prosumer","serviceType":"http://MOaPANKswMkLZU.gayowe-SJNQJJxwE91c"},{"serviceDirection":"prosumer","serviceId":"irure dolor exercitation pariatur consectetur"},{"serviceType":"http://AgJRgzRBfjnukmtIBBFrlUlDU.galiTbGmNW-xMV4pZWb8DrVytQtTCB1cSVCL4n2l-a3OPVNlMJjDnRSf2tBLukDnnhMUGt7M9G","serviceId":"sunt tempor sed ut nulla"},{"serviceDirection":"prosumer","serviceType":"https://KyJelqOfDmRxnJPzuJBtlBq.hobIWQQ1fv9+"}]},"deviceToken":"cillum ullamco"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.instantiate_device(url=url_variant, **parameters)
             assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
-        response_201_dict = json.loads(r'{"instance":{"announcedAvailability":[{"start":"1955-04-07T01:22:58.0Z","end":"1995-07-10T11:59:14.0Z"},{"end":"2006-05-22T14:58:01.0Z","start":"1956-06-29T18:16:35.0Z"},{"end":"2013-11-28T07:03:49.0Z"},{"end":"2015-04-21T18:19:04.0Z","start":"1975-07-14T08:16:38.0Z"}],"url":"http://uqyLriKDNyKa.qeZcaJtVX9mfvD76xUF+W4nYYFiXhN--1QmKZdxJnnq","services":[],"type":"device","connected":true,"name":"in","owner":"http://XtPxmagFFBylFzvNnkgMTYi.yvmlIqZeAORZPbJktCdGBIj2aFx5zB","description":"nostrud Lorem commodo Excepteur","experiment":"http://ziGqQoyUsaiCVXWUsGq.vgYEjjfQYlaoNU0.TNshwmZX97ESZapPxeXRR6oyHetq"},"deviceToken":"irure eu"}')
+        response_201_dict = json.loads(r'{"instance":{"url":"https://CqYON.xmnuGYeEv6A,Y1Xd","type":"device","name":"fugiat labore Lorem nostrud","owner":"http://qXJqGDlmidYcvasqfsCCA.eljeTAmkIX2L2AzMelvRPbXU2YfsxCWZ,n7TfiEJDoV5cMeYV97+9gjfC","connected":false,"description":"sint","announcedAvailability":[{"end":"1963-07-05T07:30:35.0Z"},{"end":"1944-01-03T21:37:04.0Z","start":"2008-03-20T19:50:34.0Z"},{"end":"1949-11-16T11:53:26.0Z","start":"1959-09-24T01:59:32.0Z"}],"experiment":"https://hSjlrWjjdOTifzKcyxsUt.wnzgp6pqUPFhd9zE6zHT1PW-LHrPsEIuTVAlx-pza8oCKVda","services":[{"serviceType":"http://UlpUhSJkIblJFycFQKfNQ.uytgIvHKxi7VK3RVSvVkGu.8MgKITDwWuLEVTBJkV,4qA7tV6OGerfaUrZw4wcN,o","serviceId":"mollit veniam proident occaecat","serviceDirection":"prosumer"},{"serviceId":"quis ad commodo nostrud dolor","serviceDirection":"prosumer","serviceType":"http://MOaPANKswMkLZU.gayowe-SJNQJJxwE91c"},{"serviceDirection":"prosumer","serviceId":"irure dolor exercitation pariatur consectetur"},{"serviceType":"http://AgJRgzRBfjnukmtIBBFrlUlDU.galiTbGmNW-xMV4pZWb8DrVytQtTCB1cSVCL4n2l-a3OPVNlMJjDnRSf2tBLukDnnhMUGt7M9G","serviceId":"sunt tempor sed ut nulla"},{"serviceDirection":"prosumer","serviceType":"https://KyJelqOfDmRxnJPzuJBtlBq.hobIWQQ1fv9+"}]},"deviceToken":"cillum ullamco"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.instantiate_device(url=full_url, **parameters)
             assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
@@ -4615,15 +4766,15 @@
 
 @pytest.mark.asyncio
 async def test_add_availability_rules(aioresponses: aioresponses):
     url = r'/devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c/availability'
     url_variant = r'devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c/availability'
     full_url = BASE_URL+r'/devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c/availability'
 
-    request = json.loads(r'[{"start":"1976-10-07T22:53:32.0Z","end":"2021-01-23T10:58:58.0Z","available":true,"repeat":{"until":"1999-07-02T02:45:39.0Z"}},{"end":"1987-01-05T01:08:15.0Z"}]')
+    request = json.loads(r'[{"start":"1976-10-07T22:53:32.0Z","end":"2021-01-23T10:58:58.0Z","available":true,"repeat":{"frequency":"DAILY","count":-28462768,"until":"2022-08-07T23:17:41.0Z"}},{"repeat":{"frequency":"HOURLY"},"start":"1943-11-02T13:33:50.0Z","available":true}]')
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"end":"1992-10-14T09:14:27.0Z"},{"start":"1978-02-16T19:07:22.0Z","end":"2008-06-15T01:24:43.0Z"},{"end":"1972-02-03T10:17:33.0Z"},{"start":"1973-01-02T03:15:47.0Z","end":"1987-10-14T09:42:59.0Z"},{"end":"1980-02-28T18:27:09.0Z","start":"1991-04-19T08:25:57.0Z"}]')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
@@ -4857,15 +5008,15 @@
 
 @pytest.mark.asyncio
 async def test_send_signaling_message(aioresponses: aioresponses):
     url = r'/devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c/signaling'
     url_variant = r'devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c/signaling'
     full_url = BASE_URL+r'/devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c/signaling'
 
-    request = json.loads(r'{"messageType":"command","command":"createPeerconnection","connectionType":"websocket","connectionUrl":"http://mSxcAxcNBEEObpLmSlWMbhgcDFFq.phuibR+NAH9qR2hG,VoGNZCgZKXd5f-JF","services":[{"serviceType":"https://WN.yyqil0X0kH-nSbucxHwUKTp6riWuOEsxSyNTZz","serviceId":"ad reprehenderit","remoteServiceId":"laborum velit"},{"serviceType":"https://GaxqG.fcVGX0FK","serviceId":"exercitation","remoteServiceId":"dolor magna in proident"}],"tiebreaker":true,"config":{}}')
+    request = json.loads(r'{"messageType":"command","command":"createPeerconnection","connectionType":"local","connectionUrl":"http://mSxcAxcNBEEObpLmSlWMbhgcDFFq.phuibR+NAH9qR2hG,VoGNZCgZKXd5f-JF","services":[{"serviceType":"https://WN.yyqil0X0kH-nSbucxHwUKTp6riWuOEsxSyNTZz","serviceId":"ad reprehenderit","remoteServiceId":"laborum velit"},{"serviceType":"https://GaxqG.fcVGX0FK","serviceId":"exercitation","remoteServiceId":"dolor magna in proident"}],"tiebreaker":true,"config":{}}')
 
     parameter_list = [{"peerconnection_url": "test_string", }, ]
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200)
         async with APIClient(BASE_URL) as client:
             resp = await client.send_signaling_message(url=url, body=request, **parameters)
@@ -4976,36 +5127,36 @@
     url = r'/peerconnections'
     url_variant = r'peerconnections'
     full_url = BASE_URL+r'/peerconnections'
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"devices":[{"url":"https://AcAm.lbXLj6e"},{"url":"http://XrTgiHePnXvRPczPBULvYtI.wsavVsuGOEjKj7O3CmZC3P2wKB4,hn4VXd6cXxcgqpSF9gDwinLCTPN0xjFVloE.mcO9"}],"url":"https://HdGqlUwYyIraClLraHacgbNvWINA.clJ3KvdUzu2GNj4hKj,RdgY6seg"},{"devices":[{"url":"https://iIRIvlwbF.obmg.EeycdcbdoSy62ARR1HP7BQpX"},{"url":"https://XnJbyygWStGohyNKERsjdkm.urE4I2GeltAe-"}]}]')
+        response_200_dict = json.loads(r'[{"url":"http://ZdTGPafFTFdOrlsRXKyoRQQ.ykdvKuq2vr32FegxRPOh7SbwHe","type":"local","devices":[{"url":"http://MhMUVnnIiUwsDRP.dudoT3yvSYQE1d27VYw9SbeCwsMFSzANMjBX0khQv6NcHEvF3MocDmv3lCMsENLY2rOFl.L"},{"url":"http://bFEJIqVUszBtNaxcvsWHfk.sirLBbny3VnBXE15oLcPZcQCi+"}],"status":"failed"},{"url":"http://LSFtmxDGOckRkViTFUiPPfXHnDvVkTLb.gwgkhwi9UO6GjEY0YNIKH18qLk","type":"local","devices":[{"url":"https://iqKdIcgcdciNq.pssaJMJuCgqPDfq4OM"},{"url":"http://TAKplEZJJnnAqUfuWTtulgjbHWC.khszpn3K.Y"}],"status":"connecting"},{"url":"http://fXVcBpEXDHmsMsDObV.hfACXLVvqZIqVxD.P8LQJdNN217pP,GAcwamid57SsHQwb","type":"webrtc","devices":[{"url":"http://upvFODDKBjYeysg.sbEHDzuy6CyZ-WogHoZ.MMvsmVR4RnrN6"},{"url":"http://JVwylE.nwmvBU4d6-PXj6OVok"}],"status":"connected"},{"url":"https://rMqZjtqZAenxRreKbLZLvmhHtE.eifsXQVOsinjFLRzFcohzkpDf1fMPRcLTYJA3S9Udo3NZUTYErE,1ovL","type":"local","devices":[{"url":"https://D.ldvaox8BCk8omTCJrY"},{"url":"http://dfUr.ilZEln+qEHrE4jQIxURnGf7yU-xVT6GfYt6NCgSZxHT0zxLPX-w"}],"status":"failed"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_peerconnections(**parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"devices":[{"url":"https://AcAm.lbXLj6e"},{"url":"http://XrTgiHePnXvRPczPBULvYtI.wsavVsuGOEjKj7O3CmZC3P2wKB4,hn4VXd6cXxcgqpSF9gDwinLCTPN0xjFVloE.mcO9"}],"url":"https://HdGqlUwYyIraClLraHacgbNvWINA.clJ3KvdUzu2GNj4hKj,RdgY6seg"},{"devices":[{"url":"https://iIRIvlwbF.obmg.EeycdcbdoSy62ARR1HP7BQpX"},{"url":"https://XnJbyygWStGohyNKERsjdkm.urE4I2GeltAe-"}]}]')
+        response_200_dict = json.loads(r'[{"url":"http://ZdTGPafFTFdOrlsRXKyoRQQ.ykdvKuq2vr32FegxRPOh7SbwHe","type":"local","devices":[{"url":"http://MhMUVnnIiUwsDRP.dudoT3yvSYQE1d27VYw9SbeCwsMFSzANMjBX0khQv6NcHEvF3MocDmv3lCMsENLY2rOFl.L"},{"url":"http://bFEJIqVUszBtNaxcvsWHfk.sirLBbny3VnBXE15oLcPZcQCi+"}],"status":"failed"},{"url":"http://LSFtmxDGOckRkViTFUiPPfXHnDvVkTLb.gwgkhwi9UO6GjEY0YNIKH18qLk","type":"local","devices":[{"url":"https://iqKdIcgcdciNq.pssaJMJuCgqPDfq4OM"},{"url":"http://TAKplEZJJnnAqUfuWTtulgjbHWC.khszpn3K.Y"}],"status":"connecting"},{"url":"http://fXVcBpEXDHmsMsDObV.hfACXLVvqZIqVxD.P8LQJdNN217pP,GAcwamid57SsHQwb","type":"webrtc","devices":[{"url":"http://upvFODDKBjYeysg.sbEHDzuy6CyZ-WogHoZ.MMvsmVR4RnrN6"},{"url":"http://JVwylE.nwmvBU4d6-PXj6OVok"}],"status":"connected"},{"url":"https://rMqZjtqZAenxRreKbLZLvmhHtE.eifsXQVOsinjFLRzFcohzkpDf1fMPRcLTYJA3S9Udo3NZUTYErE,1ovL","type":"local","devices":[{"url":"https://D.ldvaox8BCk8omTCJrY"},{"url":"http://dfUr.ilZEln+qEHrE4jQIxURnGf7yU-xVT6GfYt6NCgSZxHT0zxLPX-w"}],"status":"failed"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_peerconnections(url=url, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"devices":[{"url":"https://AcAm.lbXLj6e"},{"url":"http://XrTgiHePnXvRPczPBULvYtI.wsavVsuGOEjKj7O3CmZC3P2wKB4,hn4VXd6cXxcgqpSF9gDwinLCTPN0xjFVloE.mcO9"}],"url":"https://HdGqlUwYyIraClLraHacgbNvWINA.clJ3KvdUzu2GNj4hKj,RdgY6seg"},{"devices":[{"url":"https://iIRIvlwbF.obmg.EeycdcbdoSy62ARR1HP7BQpX"},{"url":"https://XnJbyygWStGohyNKERsjdkm.urE4I2GeltAe-"}]}]')
+        response_200_dict = json.loads(r'[{"url":"http://ZdTGPafFTFdOrlsRXKyoRQQ.ykdvKuq2vr32FegxRPOh7SbwHe","type":"local","devices":[{"url":"http://MhMUVnnIiUwsDRP.dudoT3yvSYQE1d27VYw9SbeCwsMFSzANMjBX0khQv6NcHEvF3MocDmv3lCMsENLY2rOFl.L"},{"url":"http://bFEJIqVUszBtNaxcvsWHfk.sirLBbny3VnBXE15oLcPZcQCi+"}],"status":"failed"},{"url":"http://LSFtmxDGOckRkViTFUiPPfXHnDvVkTLb.gwgkhwi9UO6GjEY0YNIKH18qLk","type":"local","devices":[{"url":"https://iqKdIcgcdciNq.pssaJMJuCgqPDfq4OM"},{"url":"http://TAKplEZJJnnAqUfuWTtulgjbHWC.khszpn3K.Y"}],"status":"connecting"},{"url":"http://fXVcBpEXDHmsMsDObV.hfACXLVvqZIqVxD.P8LQJdNN217pP,GAcwamid57SsHQwb","type":"webrtc","devices":[{"url":"http://upvFODDKBjYeysg.sbEHDzuy6CyZ-WogHoZ.MMvsmVR4RnrN6"},{"url":"http://JVwylE.nwmvBU4d6-PXj6OVok"}],"status":"connected"},{"url":"https://rMqZjtqZAenxRreKbLZLvmhHtE.eifsXQVOsinjFLRzFcohzkpDf1fMPRcLTYJA3S9Udo3NZUTYErE,1ovL","type":"local","devices":[{"url":"https://D.ldvaox8BCk8omTCJrY"},{"url":"http://dfUr.ilZEln+qEHrE4jQIxURnGf7yU-xVT6GfYt6NCgSZxHT0zxLPX-w"}],"status":"failed"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_peerconnections(url=url_variant, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"devices":[{"url":"https://AcAm.lbXLj6e"},{"url":"http://XrTgiHePnXvRPczPBULvYtI.wsavVsuGOEjKj7O3CmZC3P2wKB4,hn4VXd6cXxcgqpSF9gDwinLCTPN0xjFVloE.mcO9"}],"url":"https://HdGqlUwYyIraClLraHacgbNvWINA.clJ3KvdUzu2GNj4hKj,RdgY6seg"},{"devices":[{"url":"https://iIRIvlwbF.obmg.EeycdcbdoSy62ARR1HP7BQpX"},{"url":"https://XnJbyygWStGohyNKERsjdkm.urE4I2GeltAe-"}]}]')
+        response_200_dict = json.loads(r'[{"url":"http://ZdTGPafFTFdOrlsRXKyoRQQ.ykdvKuq2vr32FegxRPOh7SbwHe","type":"local","devices":[{"url":"http://MhMUVnnIiUwsDRP.dudoT3yvSYQE1d27VYw9SbeCwsMFSzANMjBX0khQv6NcHEvF3MocDmv3lCMsENLY2rOFl.L"},{"url":"http://bFEJIqVUszBtNaxcvsWHfk.sirLBbny3VnBXE15oLcPZcQCi+"}],"status":"failed"},{"url":"http://LSFtmxDGOckRkViTFUiPPfXHnDvVkTLb.gwgkhwi9UO6GjEY0YNIKH18qLk","type":"local","devices":[{"url":"https://iqKdIcgcdciNq.pssaJMJuCgqPDfq4OM"},{"url":"http://TAKplEZJJnnAqUfuWTtulgjbHWC.khszpn3K.Y"}],"status":"connecting"},{"url":"http://fXVcBpEXDHmsMsDObV.hfACXLVvqZIqVxD.P8LQJdNN217pP,GAcwamid57SsHQwb","type":"webrtc","devices":[{"url":"http://upvFODDKBjYeysg.sbEHDzuy6CyZ-WogHoZ.MMvsmVR4RnrN6"},{"url":"http://JVwylE.nwmvBU4d6-PXj6OVok"}],"status":"connected"},{"url":"https://rMqZjtqZAenxRreKbLZLvmhHtE.eifsXQVOsinjFLRzFcohzkpDf1fMPRcLTYJA3S9Udo3NZUTYErE,1ovL","type":"local","devices":[{"url":"https://D.ldvaox8BCk8omTCJrY"},{"url":"http://dfUr.ilZEln+qEHrE4jQIxURnGf7yU-xVT6GfYt6NCgSZxHT0zxLPX-w"}],"status":"failed"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_peerconnections(url=full_url, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
@@ -5130,69 +5281,69 @@
 
 @pytest.mark.asyncio
 async def test_create_peerconnection(aioresponses: aioresponses):
     url = r'/peerconnections'
     url_variant = r'peerconnections'
     full_url = BASE_URL+r'/peerconnections'
 
-    request = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
+    request = json.loads(r'{"url":"https://DELkhyRFPtjZoXBJnD.mpcH-J-JNY1XZPh","type":"webrtc","devices":[{"url":"http://ZjhlonrKlRrZfkk.cliFiylu2KXtjdx9AydImIgMsoHaqpuiwNWj3uTBNYtyoe","config":{"services":[{"serviceType":"https://SWNzRYsADEeZRcyrFQOtuscS.hiMmf5TYqhwWOKUVSmIihYgJxiBZNtkHAhW","serviceId":"deserunt nisi est","remoteServiceId":"in veniam fugiat minim commodo"},{"serviceType":"http://sLogGylMTrxCdLCTjU.oyeyhc-FDU+4wS6XsRVXXtooW8F-DWTPS","serviceId":"Duis","remoteServiceId":"irure consequat ex"},{"serviceType":"http://wbLPLVffzYINTKXmbvyjMAVYH.ujvGmBNAwITuJI89n.iLhmgn.8146VOut-xP75Idys5rN00pHkXEDlz","serviceId":"sunt quis minim aliqua veniam","remoteServiceId":"ipsum fugiat laborum"},{"serviceType":"https://BkfmvWkW.wadmo2WfhYb.IKKeUSq9lrY","serviceId":"Duis magna","remoteServiceId":"consequat ea"},{"serviceType":"https://tBrMngaVgCtVgsi.anMa0BCd.Qisg16arV","serviceId":"eu est culpa ullamco veniam","remoteServiceId":"in ut laborum anim esse"}]}},{"url":"http://iDPxrWlVcZpRStKCKyhCkpdQXu.xxvqtfx.DmAlHgtPMRok-pXizJJ3izr6w7Dk8E.dwuqUKIav2WVdmfv8,L,Cta4C1M2HAs","config":{"services":[{"serviceType":"https://XyGLXYXytmmyqWC.azti68D6mjzmwdOhFZg6XVC9BmswoCJtC-bsVCRfK4SdL8h+.wsBgobiqGZSyWyDitY3CeWP","serviceId":"dolore qui aliqua","remoteServiceId":"dolore incididunt sit Excepteur elit"},{"serviceType":"http://OF.hhvXtULjAIq2crOh-g.FntOP8iXLGUhfWCxnkRxPaWkB","serviceId":"ut","remoteServiceId":"occaecat nisi consequat"},{"serviceType":"https://PknLXTVMCtlNoGJBAfcadpdhuGu.qsaU7Y8bqud-Ly2XyFKd9xbJFkNOdkYTCgSwjta8aiQl7OGseQAwxqcLU.1iGmJW","serviceId":"eu","remoteServiceId":"ut velit consequat Ut"}]}}],"status":"closed"}')
 
     parameter_list = [{"closedUrl": "test_string", "statusChangedUrl": "test_string", }, {"statusChangedUrl": "test_string", }, {"closedUrl": "test_string", }, {}, ]
 
     for parameters in parameter_list:
-        response_201_dict = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
+        response_201_dict = json.loads(r'{"url":"https://DELkhyRFPtjZoXBJnD.mpcH-J-JNY1XZPh","type":"webrtc","devices":[{"url":"http://ZjhlonrKlRrZfkk.cliFiylu2KXtjdx9AydImIgMsoHaqpuiwNWj3uTBNYtyoe","config":{"services":[{"serviceType":"https://SWNzRYsADEeZRcyrFQOtuscS.hiMmf5TYqhwWOKUVSmIihYgJxiBZNtkHAhW","serviceId":"deserunt nisi est","remoteServiceId":"in veniam fugiat minim commodo"},{"serviceType":"http://sLogGylMTrxCdLCTjU.oyeyhc-FDU+4wS6XsRVXXtooW8F-DWTPS","serviceId":"Duis","remoteServiceId":"irure consequat ex"},{"serviceType":"http://wbLPLVffzYINTKXmbvyjMAVYH.ujvGmBNAwITuJI89n.iLhmgn.8146VOut-xP75Idys5rN00pHkXEDlz","serviceId":"sunt quis minim aliqua veniam","remoteServiceId":"ipsum fugiat laborum"},{"serviceType":"https://BkfmvWkW.wadmo2WfhYb.IKKeUSq9lrY","serviceId":"Duis magna","remoteServiceId":"consequat ea"},{"serviceType":"https://tBrMngaVgCtVgsi.anMa0BCd.Qisg16arV","serviceId":"eu est culpa ullamco veniam","remoteServiceId":"in ut laborum anim esse"}]}},{"url":"http://iDPxrWlVcZpRStKCKyhCkpdQXu.xxvqtfx.DmAlHgtPMRok-pXizJJ3izr6w7Dk8E.dwuqUKIav2WVdmfv8,L,Cta4C1M2HAs","config":{"services":[{"serviceType":"https://XyGLXYXytmmyqWC.azti68D6mjzmwdOhFZg6XVC9BmswoCJtC-bsVCRfK4SdL8h+.wsBgobiqGZSyWyDitY3CeWP","serviceId":"dolore qui aliqua","remoteServiceId":"dolore incididunt sit Excepteur elit"},{"serviceType":"http://OF.hhvXtULjAIq2crOh-g.FntOP8iXLGUhfWCxnkRxPaWkB","serviceId":"ut","remoteServiceId":"occaecat nisi consequat"},{"serviceType":"https://PknLXTVMCtlNoGJBAfcadpdhuGu.qsaU7Y8bqud-Ly2XyFKd9xbJFkNOdkYTCgSwjta8aiQl7OGseQAwxqcLU.1iGmJW","serviceId":"eu","remoteServiceId":"ut velit consequat Ut"}]}}],"status":"closed"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_peerconnection(body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
-        response_201_dict = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
+        response_201_dict = json.loads(r'{"url":"https://DELkhyRFPtjZoXBJnD.mpcH-J-JNY1XZPh","type":"webrtc","devices":[{"url":"http://ZjhlonrKlRrZfkk.cliFiylu2KXtjdx9AydImIgMsoHaqpuiwNWj3uTBNYtyoe","config":{"services":[{"serviceType":"https://SWNzRYsADEeZRcyrFQOtuscS.hiMmf5TYqhwWOKUVSmIihYgJxiBZNtkHAhW","serviceId":"deserunt nisi est","remoteServiceId":"in veniam fugiat minim commodo"},{"serviceType":"http://sLogGylMTrxCdLCTjU.oyeyhc-FDU+4wS6XsRVXXtooW8F-DWTPS","serviceId":"Duis","remoteServiceId":"irure consequat ex"},{"serviceType":"http://wbLPLVffzYINTKXmbvyjMAVYH.ujvGmBNAwITuJI89n.iLhmgn.8146VOut-xP75Idys5rN00pHkXEDlz","serviceId":"sunt quis minim aliqua veniam","remoteServiceId":"ipsum fugiat laborum"},{"serviceType":"https://BkfmvWkW.wadmo2WfhYb.IKKeUSq9lrY","serviceId":"Duis magna","remoteServiceId":"consequat ea"},{"serviceType":"https://tBrMngaVgCtVgsi.anMa0BCd.Qisg16arV","serviceId":"eu est culpa ullamco veniam","remoteServiceId":"in ut laborum anim esse"}]}},{"url":"http://iDPxrWlVcZpRStKCKyhCkpdQXu.xxvqtfx.DmAlHgtPMRok-pXizJJ3izr6w7Dk8E.dwuqUKIav2WVdmfv8,L,Cta4C1M2HAs","config":{"services":[{"serviceType":"https://XyGLXYXytmmyqWC.azti68D6mjzmwdOhFZg6XVC9BmswoCJtC-bsVCRfK4SdL8h+.wsBgobiqGZSyWyDitY3CeWP","serviceId":"dolore qui aliqua","remoteServiceId":"dolore incididunt sit Excepteur elit"},{"serviceType":"http://OF.hhvXtULjAIq2crOh-g.FntOP8iXLGUhfWCxnkRxPaWkB","serviceId":"ut","remoteServiceId":"occaecat nisi consequat"},{"serviceType":"https://PknLXTVMCtlNoGJBAfcadpdhuGu.qsaU7Y8bqud-Ly2XyFKd9xbJFkNOdkYTCgSwjta8aiQl7OGseQAwxqcLU.1iGmJW","serviceId":"eu","remoteServiceId":"ut velit consequat Ut"}]}}],"status":"closed"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_peerconnection(url=url, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
-        response_201_dict = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
+        response_201_dict = json.loads(r'{"url":"https://DELkhyRFPtjZoXBJnD.mpcH-J-JNY1XZPh","type":"webrtc","devices":[{"url":"http://ZjhlonrKlRrZfkk.cliFiylu2KXtjdx9AydImIgMsoHaqpuiwNWj3uTBNYtyoe","config":{"services":[{"serviceType":"https://SWNzRYsADEeZRcyrFQOtuscS.hiMmf5TYqhwWOKUVSmIihYgJxiBZNtkHAhW","serviceId":"deserunt nisi est","remoteServiceId":"in veniam fugiat minim commodo"},{"serviceType":"http://sLogGylMTrxCdLCTjU.oyeyhc-FDU+4wS6XsRVXXtooW8F-DWTPS","serviceId":"Duis","remoteServiceId":"irure consequat ex"},{"serviceType":"http://wbLPLVffzYINTKXmbvyjMAVYH.ujvGmBNAwITuJI89n.iLhmgn.8146VOut-xP75Idys5rN00pHkXEDlz","serviceId":"sunt quis minim aliqua veniam","remoteServiceId":"ipsum fugiat laborum"},{"serviceType":"https://BkfmvWkW.wadmo2WfhYb.IKKeUSq9lrY","serviceId":"Duis magna","remoteServiceId":"consequat ea"},{"serviceType":"https://tBrMngaVgCtVgsi.anMa0BCd.Qisg16arV","serviceId":"eu est culpa ullamco veniam","remoteServiceId":"in ut laborum anim esse"}]}},{"url":"http://iDPxrWlVcZpRStKCKyhCkpdQXu.xxvqtfx.DmAlHgtPMRok-pXizJJ3izr6w7Dk8E.dwuqUKIav2WVdmfv8,L,Cta4C1M2HAs","config":{"services":[{"serviceType":"https://XyGLXYXytmmyqWC.azti68D6mjzmwdOhFZg6XVC9BmswoCJtC-bsVCRfK4SdL8h+.wsBgobiqGZSyWyDitY3CeWP","serviceId":"dolore qui aliqua","remoteServiceId":"dolore incididunt sit Excepteur elit"},{"serviceType":"http://OF.hhvXtULjAIq2crOh-g.FntOP8iXLGUhfWCxnkRxPaWkB","serviceId":"ut","remoteServiceId":"occaecat nisi consequat"},{"serviceType":"https://PknLXTVMCtlNoGJBAfcadpdhuGu.qsaU7Y8bqud-Ly2XyFKd9xbJFkNOdkYTCgSwjta8aiQl7OGseQAwxqcLU.1iGmJW","serviceId":"eu","remoteServiceId":"ut velit consequat Ut"}]}}],"status":"closed"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_peerconnection(url=url_variant, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
-        response_201_dict = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
+        response_201_dict = json.loads(r'{"url":"https://DELkhyRFPtjZoXBJnD.mpcH-J-JNY1XZPh","type":"webrtc","devices":[{"url":"http://ZjhlonrKlRrZfkk.cliFiylu2KXtjdx9AydImIgMsoHaqpuiwNWj3uTBNYtyoe","config":{"services":[{"serviceType":"https://SWNzRYsADEeZRcyrFQOtuscS.hiMmf5TYqhwWOKUVSmIihYgJxiBZNtkHAhW","serviceId":"deserunt nisi est","remoteServiceId":"in veniam fugiat minim commodo"},{"serviceType":"http://sLogGylMTrxCdLCTjU.oyeyhc-FDU+4wS6XsRVXXtooW8F-DWTPS","serviceId":"Duis","remoteServiceId":"irure consequat ex"},{"serviceType":"http://wbLPLVffzYINTKXmbvyjMAVYH.ujvGmBNAwITuJI89n.iLhmgn.8146VOut-xP75Idys5rN00pHkXEDlz","serviceId":"sunt quis minim aliqua veniam","remoteServiceId":"ipsum fugiat laborum"},{"serviceType":"https://BkfmvWkW.wadmo2WfhYb.IKKeUSq9lrY","serviceId":"Duis magna","remoteServiceId":"consequat ea"},{"serviceType":"https://tBrMngaVgCtVgsi.anMa0BCd.Qisg16arV","serviceId":"eu est culpa ullamco veniam","remoteServiceId":"in ut laborum anim esse"}]}},{"url":"http://iDPxrWlVcZpRStKCKyhCkpdQXu.xxvqtfx.DmAlHgtPMRok-pXizJJ3izr6w7Dk8E.dwuqUKIav2WVdmfv8,L,Cta4C1M2HAs","config":{"services":[{"serviceType":"https://XyGLXYXytmmyqWC.azti68D6mjzmwdOhFZg6XVC9BmswoCJtC-bsVCRfK4SdL8h+.wsBgobiqGZSyWyDitY3CeWP","serviceId":"dolore qui aliqua","remoteServiceId":"dolore incididunt sit Excepteur elit"},{"serviceType":"http://OF.hhvXtULjAIq2crOh-g.FntOP8iXLGUhfWCxnkRxPaWkB","serviceId":"ut","remoteServiceId":"occaecat nisi consequat"},{"serviceType":"https://PknLXTVMCtlNoGJBAfcadpdhuGu.qsaU7Y8bqud-Ly2XyFKd9xbJFkNOdkYTCgSwjta8aiQl7OGseQAwxqcLU.1iGmJW","serviceId":"eu","remoteServiceId":"ut velit consequat Ut"}]}}],"status":"closed"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_peerconnection(url=full_url, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
-        response_202_dict = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
+        response_202_dict = json.loads(r'{"url":"https://DELkhyRFPtjZoXBJnD.mpcH-J-JNY1XZPh","type":"webrtc","devices":[{"url":"http://ZjhlonrKlRrZfkk.cliFiylu2KXtjdx9AydImIgMsoHaqpuiwNWj3uTBNYtyoe","config":{"services":[{"serviceType":"https://SWNzRYsADEeZRcyrFQOtuscS.hiMmf5TYqhwWOKUVSmIihYgJxiBZNtkHAhW","serviceId":"deserunt nisi est","remoteServiceId":"in veniam fugiat minim commodo"},{"serviceType":"http://sLogGylMTrxCdLCTjU.oyeyhc-FDU+4wS6XsRVXXtooW8F-DWTPS","serviceId":"Duis","remoteServiceId":"irure consequat ex"},{"serviceType":"http://wbLPLVffzYINTKXmbvyjMAVYH.ujvGmBNAwITuJI89n.iLhmgn.8146VOut-xP75Idys5rN00pHkXEDlz","serviceId":"sunt quis minim aliqua veniam","remoteServiceId":"ipsum fugiat laborum"},{"serviceType":"https://BkfmvWkW.wadmo2WfhYb.IKKeUSq9lrY","serviceId":"Duis magna","remoteServiceId":"consequat ea"},{"serviceType":"https://tBrMngaVgCtVgsi.anMa0BCd.Qisg16arV","serviceId":"eu est culpa ullamco veniam","remoteServiceId":"in ut laborum anim esse"}]}},{"url":"http://iDPxrWlVcZpRStKCKyhCkpdQXu.xxvqtfx.DmAlHgtPMRok-pXizJJ3izr6w7Dk8E.dwuqUKIav2WVdmfv8,L,Cta4C1M2HAs","config":{"services":[{"serviceType":"https://XyGLXYXytmmyqWC.azti68D6mjzmwdOhFZg6XVC9BmswoCJtC-bsVCRfK4SdL8h+.wsBgobiqGZSyWyDitY3CeWP","serviceId":"dolore qui aliqua","remoteServiceId":"dolore incididunt sit Excepteur elit"},{"serviceType":"http://OF.hhvXtULjAIq2crOh-g.FntOP8iXLGUhfWCxnkRxPaWkB","serviceId":"ut","remoteServiceId":"occaecat nisi consequat"},{"serviceType":"https://PknLXTVMCtlNoGJBAfcadpdhuGu.qsaU7Y8bqud-Ly2XyFKd9xbJFkNOdkYTCgSwjta8aiQl7OGseQAwxqcLU.1iGmJW","serviceId":"eu","remoteServiceId":"ut velit consequat Ut"}]}}],"status":"closed"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=202, payload=response_202_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_peerconnection(body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_202_dict)
 
     for parameters in parameter_list:
-        response_202_dict = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
+        response_202_dict = json.loads(r'{"url":"https://DELkhyRFPtjZoXBJnD.mpcH-J-JNY1XZPh","type":"webrtc","devices":[{"url":"http://ZjhlonrKlRrZfkk.cliFiylu2KXtjdx9AydImIgMsoHaqpuiwNWj3uTBNYtyoe","config":{"services":[{"serviceType":"https://SWNzRYsADEeZRcyrFQOtuscS.hiMmf5TYqhwWOKUVSmIihYgJxiBZNtkHAhW","serviceId":"deserunt nisi est","remoteServiceId":"in veniam fugiat minim commodo"},{"serviceType":"http://sLogGylMTrxCdLCTjU.oyeyhc-FDU+4wS6XsRVXXtooW8F-DWTPS","serviceId":"Duis","remoteServiceId":"irure consequat ex"},{"serviceType":"http://wbLPLVffzYINTKXmbvyjMAVYH.ujvGmBNAwITuJI89n.iLhmgn.8146VOut-xP75Idys5rN00pHkXEDlz","serviceId":"sunt quis minim aliqua veniam","remoteServiceId":"ipsum fugiat laborum"},{"serviceType":"https://BkfmvWkW.wadmo2WfhYb.IKKeUSq9lrY","serviceId":"Duis magna","remoteServiceId":"consequat ea"},{"serviceType":"https://tBrMngaVgCtVgsi.anMa0BCd.Qisg16arV","serviceId":"eu est culpa ullamco veniam","remoteServiceId":"in ut laborum anim esse"}]}},{"url":"http://iDPxrWlVcZpRStKCKyhCkpdQXu.xxvqtfx.DmAlHgtPMRok-pXizJJ3izr6w7Dk8E.dwuqUKIav2WVdmfv8,L,Cta4C1M2HAs","config":{"services":[{"serviceType":"https://XyGLXYXytmmyqWC.azti68D6mjzmwdOhFZg6XVC9BmswoCJtC-bsVCRfK4SdL8h+.wsBgobiqGZSyWyDitY3CeWP","serviceId":"dolore qui aliqua","remoteServiceId":"dolore incididunt sit Excepteur elit"},{"serviceType":"http://OF.hhvXtULjAIq2crOh-g.FntOP8iXLGUhfWCxnkRxPaWkB","serviceId":"ut","remoteServiceId":"occaecat nisi consequat"},{"serviceType":"https://PknLXTVMCtlNoGJBAfcadpdhuGu.qsaU7Y8bqud-Ly2XyFKd9xbJFkNOdkYTCgSwjta8aiQl7OGseQAwxqcLU.1iGmJW","serviceId":"eu","remoteServiceId":"ut velit consequat Ut"}]}}],"status":"closed"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=202, payload=response_202_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_peerconnection(url=url, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_202_dict)
 
     for parameters in parameter_list:
-        response_202_dict = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
+        response_202_dict = json.loads(r'{"url":"https://DELkhyRFPtjZoXBJnD.mpcH-J-JNY1XZPh","type":"webrtc","devices":[{"url":"http://ZjhlonrKlRrZfkk.cliFiylu2KXtjdx9AydImIgMsoHaqpuiwNWj3uTBNYtyoe","config":{"services":[{"serviceType":"https://SWNzRYsADEeZRcyrFQOtuscS.hiMmf5TYqhwWOKUVSmIihYgJxiBZNtkHAhW","serviceId":"deserunt nisi est","remoteServiceId":"in veniam fugiat minim commodo"},{"serviceType":"http://sLogGylMTrxCdLCTjU.oyeyhc-FDU+4wS6XsRVXXtooW8F-DWTPS","serviceId":"Duis","remoteServiceId":"irure consequat ex"},{"serviceType":"http://wbLPLVffzYINTKXmbvyjMAVYH.ujvGmBNAwITuJI89n.iLhmgn.8146VOut-xP75Idys5rN00pHkXEDlz","serviceId":"sunt quis minim aliqua veniam","remoteServiceId":"ipsum fugiat laborum"},{"serviceType":"https://BkfmvWkW.wadmo2WfhYb.IKKeUSq9lrY","serviceId":"Duis magna","remoteServiceId":"consequat ea"},{"serviceType":"https://tBrMngaVgCtVgsi.anMa0BCd.Qisg16arV","serviceId":"eu est culpa ullamco veniam","remoteServiceId":"in ut laborum anim esse"}]}},{"url":"http://iDPxrWlVcZpRStKCKyhCkpdQXu.xxvqtfx.DmAlHgtPMRok-pXizJJ3izr6w7Dk8E.dwuqUKIav2WVdmfv8,L,Cta4C1M2HAs","config":{"services":[{"serviceType":"https://XyGLXYXytmmyqWC.azti68D6mjzmwdOhFZg6XVC9BmswoCJtC-bsVCRfK4SdL8h+.wsBgobiqGZSyWyDitY3CeWP","serviceId":"dolore qui aliqua","remoteServiceId":"dolore incididunt sit Excepteur elit"},{"serviceType":"http://OF.hhvXtULjAIq2crOh-g.FntOP8iXLGUhfWCxnkRxPaWkB","serviceId":"ut","remoteServiceId":"occaecat nisi consequat"},{"serviceType":"https://PknLXTVMCtlNoGJBAfcadpdhuGu.qsaU7Y8bqud-Ly2XyFKd9xbJFkNOdkYTCgSwjta8aiQl7OGseQAwxqcLU.1iGmJW","serviceId":"eu","remoteServiceId":"ut velit consequat Ut"}]}}],"status":"closed"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=202, payload=response_202_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_peerconnection(url=url_variant, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_202_dict)
 
     for parameters in parameter_list:
-        response_202_dict = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
+        response_202_dict = json.loads(r'{"url":"https://DELkhyRFPtjZoXBJnD.mpcH-J-JNY1XZPh","type":"webrtc","devices":[{"url":"http://ZjhlonrKlRrZfkk.cliFiylu2KXtjdx9AydImIgMsoHaqpuiwNWj3uTBNYtyoe","config":{"services":[{"serviceType":"https://SWNzRYsADEeZRcyrFQOtuscS.hiMmf5TYqhwWOKUVSmIihYgJxiBZNtkHAhW","serviceId":"deserunt nisi est","remoteServiceId":"in veniam fugiat minim commodo"},{"serviceType":"http://sLogGylMTrxCdLCTjU.oyeyhc-FDU+4wS6XsRVXXtooW8F-DWTPS","serviceId":"Duis","remoteServiceId":"irure consequat ex"},{"serviceType":"http://wbLPLVffzYINTKXmbvyjMAVYH.ujvGmBNAwITuJI89n.iLhmgn.8146VOut-xP75Idys5rN00pHkXEDlz","serviceId":"sunt quis minim aliqua veniam","remoteServiceId":"ipsum fugiat laborum"},{"serviceType":"https://BkfmvWkW.wadmo2WfhYb.IKKeUSq9lrY","serviceId":"Duis magna","remoteServiceId":"consequat ea"},{"serviceType":"https://tBrMngaVgCtVgsi.anMa0BCd.Qisg16arV","serviceId":"eu est culpa ullamco veniam","remoteServiceId":"in ut laborum anim esse"}]}},{"url":"http://iDPxrWlVcZpRStKCKyhCkpdQXu.xxvqtfx.DmAlHgtPMRok-pXizJJ3izr6w7Dk8E.dwuqUKIav2WVdmfv8,L,Cta4C1M2HAs","config":{"services":[{"serviceType":"https://XyGLXYXytmmyqWC.azti68D6mjzmwdOhFZg6XVC9BmswoCJtC-bsVCRfK4SdL8h+.wsBgobiqGZSyWyDitY3CeWP","serviceId":"dolore qui aliqua","remoteServiceId":"dolore incididunt sit Excepteur elit"},{"serviceType":"http://OF.hhvXtULjAIq2crOh-g.FntOP8iXLGUhfWCxnkRxPaWkB","serviceId":"ut","remoteServiceId":"occaecat nisi consequat"},{"serviceType":"https://PknLXTVMCtlNoGJBAfcadpdhuGu.qsaU7Y8bqud-Ly2XyFKd9xbJFkNOdkYTCgSwjta8aiQl7OGseQAwxqcLU.1iGmJW","serviceId":"eu","remoteServiceId":"ut velit consequat Ut"}]}}],"status":"closed"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=202, payload=response_202_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_peerconnection(url=full_url, body=request, **parameters)
             assert normalize_result(resp) == normalize_result(response_202_dict)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
@@ -5320,29 +5471,29 @@
     url = r'/peerconnections/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     url_variant = r'peerconnections/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     full_url = BASE_URL+r'/peerconnections/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
+        response_200_dict = json.loads(r'{"url":"https://DELkhyRFPtjZoXBJnD.mpcH-J-JNY1XZPh","type":"webrtc","devices":[{"url":"http://ZjhlonrKlRrZfkk.cliFiylu2KXtjdx9AydImIgMsoHaqpuiwNWj3uTBNYtyoe","config":{"services":[{"serviceType":"https://SWNzRYsADEeZRcyrFQOtuscS.hiMmf5TYqhwWOKUVSmIihYgJxiBZNtkHAhW","serviceId":"deserunt nisi est","remoteServiceId":"in veniam fugiat minim commodo"},{"serviceType":"http://sLogGylMTrxCdLCTjU.oyeyhc-FDU+4wS6XsRVXXtooW8F-DWTPS","serviceId":"Duis","remoteServiceId":"irure consequat ex"},{"serviceType":"http://wbLPLVffzYINTKXmbvyjMAVYH.ujvGmBNAwITuJI89n.iLhmgn.8146VOut-xP75Idys5rN00pHkXEDlz","serviceId":"sunt quis minim aliqua veniam","remoteServiceId":"ipsum fugiat laborum"},{"serviceType":"https://BkfmvWkW.wadmo2WfhYb.IKKeUSq9lrY","serviceId":"Duis magna","remoteServiceId":"consequat ea"},{"serviceType":"https://tBrMngaVgCtVgsi.anMa0BCd.Qisg16arV","serviceId":"eu est culpa ullamco veniam","remoteServiceId":"in ut laborum anim esse"}]}},{"url":"http://iDPxrWlVcZpRStKCKyhCkpdQXu.xxvqtfx.DmAlHgtPMRok-pXizJJ3izr6w7Dk8E.dwuqUKIav2WVdmfv8,L,Cta4C1M2HAs","config":{"services":[{"serviceType":"https://XyGLXYXytmmyqWC.azti68D6mjzmwdOhFZg6XVC9BmswoCJtC-bsVCRfK4SdL8h+.wsBgobiqGZSyWyDitY3CeWP","serviceId":"dolore qui aliqua","remoteServiceId":"dolore incididunt sit Excepteur elit"},{"serviceType":"http://OF.hhvXtULjAIq2crOh-g.FntOP8iXLGUhfWCxnkRxPaWkB","serviceId":"ut","remoteServiceId":"occaecat nisi consequat"},{"serviceType":"https://PknLXTVMCtlNoGJBAfcadpdhuGu.qsaU7Y8bqud-Ly2XyFKd9xbJFkNOdkYTCgSwjta8aiQl7OGseQAwxqcLU.1iGmJW","serviceId":"eu","remoteServiceId":"ut velit consequat Ut"}]}}],"status":"closed"}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_peerconnection(url=url, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
+        response_200_dict = json.loads(r'{"url":"https://DELkhyRFPtjZoXBJnD.mpcH-J-JNY1XZPh","type":"webrtc","devices":[{"url":"http://ZjhlonrKlRrZfkk.cliFiylu2KXtjdx9AydImIgMsoHaqpuiwNWj3uTBNYtyoe","config":{"services":[{"serviceType":"https://SWNzRYsADEeZRcyrFQOtuscS.hiMmf5TYqhwWOKUVSmIihYgJxiBZNtkHAhW","serviceId":"deserunt nisi est","remoteServiceId":"in veniam fugiat minim commodo"},{"serviceType":"http://sLogGylMTrxCdLCTjU.oyeyhc-FDU+4wS6XsRVXXtooW8F-DWTPS","serviceId":"Duis","remoteServiceId":"irure consequat ex"},{"serviceType":"http://wbLPLVffzYINTKXmbvyjMAVYH.ujvGmBNAwITuJI89n.iLhmgn.8146VOut-xP75Idys5rN00pHkXEDlz","serviceId":"sunt quis minim aliqua veniam","remoteServiceId":"ipsum fugiat laborum"},{"serviceType":"https://BkfmvWkW.wadmo2WfhYb.IKKeUSq9lrY","serviceId":"Duis magna","remoteServiceId":"consequat ea"},{"serviceType":"https://tBrMngaVgCtVgsi.anMa0BCd.Qisg16arV","serviceId":"eu est culpa ullamco veniam","remoteServiceId":"in ut laborum anim esse"}]}},{"url":"http://iDPxrWlVcZpRStKCKyhCkpdQXu.xxvqtfx.DmAlHgtPMRok-pXizJJ3izr6w7Dk8E.dwuqUKIav2WVdmfv8,L,Cta4C1M2HAs","config":{"services":[{"serviceType":"https://XyGLXYXytmmyqWC.azti68D6mjzmwdOhFZg6XVC9BmswoCJtC-bsVCRfK4SdL8h+.wsBgobiqGZSyWyDitY3CeWP","serviceId":"dolore qui aliqua","remoteServiceId":"dolore incididunt sit Excepteur elit"},{"serviceType":"http://OF.hhvXtULjAIq2crOh-g.FntOP8iXLGUhfWCxnkRxPaWkB","serviceId":"ut","remoteServiceId":"occaecat nisi consequat"},{"serviceType":"https://PknLXTVMCtlNoGJBAfcadpdhuGu.qsaU7Y8bqud-Ly2XyFKd9xbJFkNOdkYTCgSwjta8aiQl7OGseQAwxqcLU.1iGmJW","serviceId":"eu","remoteServiceId":"ut velit consequat Ut"}]}}],"status":"closed"}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_peerconnection(url=url_variant, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
+        response_200_dict = json.loads(r'{"url":"https://DELkhyRFPtjZoXBJnD.mpcH-J-JNY1XZPh","type":"webrtc","devices":[{"url":"http://ZjhlonrKlRrZfkk.cliFiylu2KXtjdx9AydImIgMsoHaqpuiwNWj3uTBNYtyoe","config":{"services":[{"serviceType":"https://SWNzRYsADEeZRcyrFQOtuscS.hiMmf5TYqhwWOKUVSmIihYgJxiBZNtkHAhW","serviceId":"deserunt nisi est","remoteServiceId":"in veniam fugiat minim commodo"},{"serviceType":"http://sLogGylMTrxCdLCTjU.oyeyhc-FDU+4wS6XsRVXXtooW8F-DWTPS","serviceId":"Duis","remoteServiceId":"irure consequat ex"},{"serviceType":"http://wbLPLVffzYINTKXmbvyjMAVYH.ujvGmBNAwITuJI89n.iLhmgn.8146VOut-xP75Idys5rN00pHkXEDlz","serviceId":"sunt quis minim aliqua veniam","remoteServiceId":"ipsum fugiat laborum"},{"serviceType":"https://BkfmvWkW.wadmo2WfhYb.IKKeUSq9lrY","serviceId":"Duis magna","remoteServiceId":"consequat ea"},{"serviceType":"https://tBrMngaVgCtVgsi.anMa0BCd.Qisg16arV","serviceId":"eu est culpa ullamco veniam","remoteServiceId":"in ut laborum anim esse"}]}},{"url":"http://iDPxrWlVcZpRStKCKyhCkpdQXu.xxvqtfx.DmAlHgtPMRok-pXizJJ3izr6w7Dk8E.dwuqUKIav2WVdmfv8,L,Cta4C1M2HAs","config":{"services":[{"serviceType":"https://XyGLXYXytmmyqWC.azti68D6mjzmwdOhFZg6XVC9BmswoCJtC-bsVCRfK4SdL8h+.wsBgobiqGZSyWyDitY3CeWP","serviceId":"dolore qui aliqua","remoteServiceId":"dolore incididunt sit Excepteur elit"},{"serviceType":"http://OF.hhvXtULjAIq2crOh-g.FntOP8iXLGUhfWCxnkRxPaWkB","serviceId":"ut","remoteServiceId":"occaecat nisi consequat"},{"serviceType":"https://PknLXTVMCtlNoGJBAfcadpdhuGu.qsaU7Y8bqud-Ly2XyFKd9xbJFkNOdkYTCgSwjta8aiQl7OGseQAwxqcLU.1iGmJW","serviceId":"eu","remoteServiceId":"ut velit consequat Ut"}]}}],"status":"closed"}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_peerconnection(url=full_url, **parameters)
             assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
@@ -5546,14 +5697,130 @@
         aioresponses.delete(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.delete_peerconnection(url=full_url, **parameters)
 
 
 @pytest.mark.asyncio
+async def test_patch_peerconnection_device_status(aioresponses: aioresponses):
+    url = r'/peerconnections/c799cc2e-cdc5-4143-973a-6f56a5afa82c/device_status'
+    url_variant = r'peerconnections/c799cc2e-cdc5-4143-973a-6f56a5afa82c/device_status'
+    full_url = BASE_URL+r'/peerconnections/c799cc2e-cdc5-4143-973a-6f56a5afa82c/device_status'
+
+    request = json.loads(r'{"status":"closed"}')
+
+    parameter_list = [{"device_url": "test_string", }, ]
+
+    for parameters in parameter_list:
+        aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201)
+        async with APIClient(BASE_URL) as client:
+            resp = await client.patch_peerconnection_device_status(url=url, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201)
+        async with APIClient(BASE_URL) as client:
+            resp = await client.patch_peerconnection_device_status(url=url_variant, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201)
+        async with APIClient(BASE_URL) as client:
+            resp = await client.patch_peerconnection_device_status(url=full_url, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.patch_peerconnection_device_status(url=url, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.patch_peerconnection_device_status(url=url_variant, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.patch_peerconnection_device_status(url=full_url, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.patch_peerconnection_device_status(url=url, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.patch_peerconnection_device_status(url=url_variant, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.patch_peerconnection_device_status(url=full_url, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.patch_peerconnection_device_status(url=url, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.patch_peerconnection_device_status(url=url_variant, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.patch_peerconnection_device_status(url=full_url, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.patch_peerconnection_device_status(url=url, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.patch_peerconnection_device_status(url=url_variant, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.patch_peerconnection_device_status(url=full_url, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.patch_peerconnection_device_status(url=url, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.patch_peerconnection_device_status(url=url_variant, body=request, **parameters)
+
+    for parameters in parameter_list:
+        aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
+        async with APIClient(BASE_URL) as client:
+            with pytest.raises(Exception):
+                resp = await client.patch_peerconnection_device_status(url=full_url, body=request, **parameters)
+
+
+@pytest.mark.asyncio
 async def test_list_experiments(aioresponses: aioresponses):
     url = r'/experiments'
     url_variant = r'experiments'
     full_url = BASE_URL+r'/experiments'
 
     parameter_list = [{}, ]
```

